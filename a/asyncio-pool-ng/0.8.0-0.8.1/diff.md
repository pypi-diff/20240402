# Comparing `tmp/asyncio_pool_ng-0.8.0.tar.gz` & `tmp/asyncio_pool_ng-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncio_pool_ng-0.8.0.tar", max compression
+gzip compressed data, was "asyncio_pool_ng-0.8.1.tar", max compression
```

## Comparing `asyncio_pool_ng-0.8.0.tar` & `asyncio_pool_ng-0.8.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2022-11-27 01:25:31.000000 asyncio_pool_ng-0.8.0/LICENSE
--rw-r--r--   0        0        0     4002 2023-05-22 14:00:42.724655 asyncio_pool_ng-0.8.0/README.md
--rw-r--r--   0        0        0      202 2023-05-22 14:00:42.724655 asyncio_pool_ng-0.8.0/asyncio_pool/__init__.py
--rw-r--r--   0        0        0     9080 2023-05-22 14:00:42.724655 asyncio_pool_ng-0.8.0/asyncio_pool/_pool.py
--rw-r--r--   0        0        0      244 2023-05-22 14:00:42.724655 asyncio_pool_ng-0.8.0/asyncio_pool/_typing.py
--rw-r--r--   0        0        0        0 2022-11-25 12:59:38.000000 asyncio_pool_ng-0.8.0/asyncio_pool/py.typed
--rw-r--r--   0        0        0     3621 2023-05-22 14:00:42.734655 asyncio_pool_ng-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4729 1970-01-01 00:00:00.000000 asyncio_pool_ng-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-11-27 01:25:31.000000 asyncio_pool_ng-0.8.1/LICENSE
+-rw-r--r--   0        0        0     4002 2023-05-22 14:00:42.724655 asyncio_pool_ng-0.8.1/README.md
+-rw-r--r--   0        0        0      202 2024-04-02 13:07:41.447524 asyncio_pool_ng-0.8.1/asyncio_pool/__init__.py
+-rw-r--r--   0        0        0     9966 2024-04-02 13:07:41.447524 asyncio_pool_ng-0.8.1/asyncio_pool/_pool.py
+-rw-r--r--   0        0        0      244 2023-05-22 14:00:42.724655 asyncio_pool_ng-0.8.1/asyncio_pool/_typing.py
+-rw-r--r--   0        0        0        0 2022-11-25 12:59:38.000000 asyncio_pool_ng-0.8.1/asyncio_pool/py.typed
+-rw-r--r--   0        0        0     3679 2024-04-02 13:07:41.447524 asyncio_pool_ng-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4780 1970-01-01 00:00:00.000000 asyncio_pool_ng-0.8.1/PKG-INFO
```

### Comparing `asyncio_pool_ng-0.8.0/LICENSE` & `asyncio_pool_ng-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncio_pool_ng-0.8.0/README.md` & `asyncio_pool_ng-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `asyncio_pool_ng-0.8.0/asyncio_pool/_pool.py` & `asyncio_pool_ng-0.8.1/asyncio_pool/_pool.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from asyncio import Future, Queue, Semaphore, Task, TaskGroup, create_task, sleep, wait
+from asyncio import Event, Future, Queue, Semaphore, Task, TaskGroup, create_task, sleep, wait
 from asyncio.queues import QueueEmpty
-from collections.abc import AsyncGenerator, Coroutine, Iterable
+from collections.abc import AsyncGenerator, AsyncIterable, Coroutine, Iterable
 from contextlib import AsyncExitStack, asynccontextmanager
 from contextvars import Context
 from dataclasses import dataclass
 from typing import Any, Generic, TypeVar, cast
 
 from ._typing import AsyncioPoolMapWorkerType, AsyncioPoolWorkerType
 
@@ -113,35 +113,35 @@
 
     @property
     def _exiting(self) -> bool:
         return cast(bool, self._group._exiting)  # type: ignore[attr-defined]
 
     @property
     def _tasks(self) -> set[Task[T]]:
-        return cast(set[Task[T]], self._group._tasks)  # type: ignore[attr-defined]
+        return cast(set[Task[T]], self._group._tasks)
 
     @asynccontextmanager
     async def _consumer(self) -> AsyncGenerator[Task[None], None]:
         def release(_: Task[T]) -> None:
             self._semaphore.release()
 
-        async def loop() -> None:
+        async def handler() -> None:
             while not self._exiting or len(self._pending) > 0:
                 try:
                     future, pending_task = self._queue.get_nowait()
                 except QueueEmpty:
                     await sleep(0)
                     continue
 
                 await self._semaphore.acquire()
                 coro = pending_task.wrapped(future)
                 task = self._group.create_task(coro, name=pending_task.name, context=pending_task.context)
                 task.add_done_callback(release)
 
-        task = create_task(loop(), name="AsyncioPool-consumer")
+        task = create_task(handler(), name="AsyncioPool-consumer")
         yield task
         await task
 
     async def join(self) -> None:
         """Wait for all active tasks to complete."""
         while self._pending:
             await sleep(0)
@@ -213,41 +213,59 @@
                 [contextvars.Context](https://docs.python.org/3/library/contextvars.html#contextvars.Context)
                 for the coro to run in. The current context copy is created when no context is provided.
 
         Returns:
             Set of futures which will eventually contain the results of each _func_.
         """
         name = name if name else f"map({func.__name__})"
-
         return {self.spawn(func, item, name=f"{name}[{i}]", context=context) for i, item in enumerate(iterable)}
 
     async def itermap(
         self,
         func: AsyncioPoolMapWorkerType[T, R],
-        iterable: Iterable[T],
+        iterable: Iterable[T] | AsyncIterable[T],
         name: str | None = None,
         context: Context | None = None,
         batch_duration: int | float = 1.0,
     ) -> AsyncGenerator[Future[R], None]:
         """Generate a future for _func_ for every item of _iterable_.
 
         Futures are yielded as they completed.
 
         Args:
             func: Function created with [async def](https://docs.python.org/3/reference/compound_stmts.html#async-def)
-            iterable: Iterable instance which produces values for _func_
+            iterable: Instance of Iterable or AsyncIterabl which produces values for _func_
             name: Optional name for the `asyncio.Task`
             context: Optional context argument allows specifying a custom
                 [contextvars.Context](https://docs.python.org/3/library/contextvars.html#contextvars.Context)
                 for the coro to run in. The current context copy is created when no context is provided.
             batch_duration: Duration to wait before yielding batches of completed futures.
 
         Returns:
             Async generator of futures.
         """
-        name = name if name else f"itermap({func.__name__})"
 
-        pending = self.map(func, iterable, name=name, context=context)
-        while pending:
-            done, pending = await wait(pending, timeout=batch_duration)
-            for future in done:
-                yield future
+        async def async_iterable_handler(_iterable: AsyncIterable[T]) -> None:
+            i = 0
+            async for item in _iterable:
+                pending.add(self.spawn(func, item, name=f"{name}[{i}]", context=context))
+                startup_event.set()
+                i += 1
+
+        name = name if name else f"itermap({func.__name__})"
+        pending: set[Future[R]] = set()
+        if isinstance(iterable, AsyncIterable):
+            startup_event = Event()
+            task = create_task(async_iterable_handler(iterable), name="AsyncioPool-amap")
+            await startup_event.wait()
+            while not task.done() or pending:
+                while pending:
+                    done, _ = await wait(pending, timeout=batch_duration)
+                    for future in done:
+                        yield future
+                        pending.discard(future)
+        else:
+            pending = self.map(func, iterable, name=name, context=context)
+            while pending:
+                done, pending = await wait(pending, timeout=batch_duration)
+                for future in done:
+                    yield future
```

### Comparing `asyncio_pool_ng-0.8.0/pyproject.toml` & `asyncio_pool_ng-0.8.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [build-system]
-requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core"]
 
 [tool.black]
 line-length = 120
 
 [tool.mypy]
-strict = true
 packages = ["asyncio_pool", "tests"]
+strict = true
 
 [tool.poetry]
-name = "asyncio-pool-ng"
-version = "0.8.0"
-description = "A pool of coroutine functions."
 authors = ["Kyle Smith <smithk86@smc3.com>"]
-license = "MIT"
-readme = "README.md"
-homepage = "https://github.com/smithk86/asyncio-pool-ng"
-repository = "https://github.com/smithk86/asyncio-pool-ng"
-documentation = "https://smithk86.github.io/asyncio-pool-ng"
 classifiers = [
     "Intended Audience :: Developers",
     "Framework :: AsyncIO",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
+description = "A pool of coroutine functions."
+documentation = "https://smithk86.github.io/asyncio-pool-ng"
+homepage = "https://github.com/smithk86/asyncio-pool-ng"
+license = "MIT"
+name = "asyncio-pool-ng"
 packages = [{ include = "asyncio_pool" }]
+readme = "README.md"
+repository = "https://github.com/smithk86/asyncio-pool-ng"
+version = "0.8.1"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4"
 
 [tool.poetry.group.dev.dependencies]
+mypy = "*"
 pytest = ">=7.0"
 pytest-asyncio = ">=0.20"
-mypy = "*"
 pytest-mypy = "*"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "*"
 mkdocs-material = "*"
 mkdocstrings = { version = "*", extras = ["python"] }
 
@@ -51,14 +51,36 @@
 addopts = "--mypy"
 testpaths = ["tests"]
 
 [tool.slotscheck]
 strict-imports = false
 
 [tool.ruff]
+exclude = ["__pycache__", "venv", ".venv"]
+line-length = 120                          # match Black
+target-version = 'py311'
+
+[tool.ruff.lint]
+ignore = [
+    "A003",  # flake8-builtins - class attribute {name} is shadowing a python builtin
+    "B010",  # flake8-bugbear - do not call setattr with a constant attribute value
+    "D100",  # pydocstyle - missing docstring in public module
+    "D101",  # pydocstyle - missing docstring in public class
+    "D102",  # pydocstyle - missing docstring in public method
+    "D103",  # pydocstyle - missing docstring in public function
+    "D104",  # pydocstyle - missing docstring in public package
+    "D105",  # pydocstyle - missing docstring in magic method
+    "D106",  # pydocstyle - missing docstring in public nested class
+    "D107",  # pydocstyle - missing docstring in __init__
+    "D202",  # pydocstyle - no blank lines allowed after function docstring
+    "D205",  # pydocstyle - 1 blank line required between summary line and description
+    "D415",  # pydocstyle - first line should end with a period, question mark, or exclamation point
+    "E501",  # pycodestyle line too long, handled by black
+    "UP037", # pyupgrade - removes quotes from type annotation
+]
 select = [
     "A",   # flake8-builtins
     "B",   # flake8-bugbear
     "BLE", # flake8-blind-except
     "C4",  # flake8-comprehensions
     "C90", # mccabe
     "D",   # pydocstyle
@@ -87,37 +109,17 @@
     "T20", # flake8-print
     "TCH", # flake8-type-checking
     "TID", # flake8-tidy-imports
     "UP",  # pyupgrade
     "W",   # pycodestyle - warning
     "YTT", # flake8-2020
 ]
-exclude = ["__pycache__", "venv", ".venv"]
-ignore = [
-    "A003",  # flake8-builtins - class attribute {name} is shadowing a python builtin
-    "B010",  # flake8-bugbear - do not call setattr with a constant attribute value
-    "D100",  # pydocstyle - missing docstring in public module
-    "D101",  # pydocstyle - missing docstring in public class
-    "D102",  # pydocstyle - missing docstring in public method
-    "D103",  # pydocstyle - missing docstring in public function
-    "D104",  # pydocstyle - missing docstring in public package
-    "D105",  # pydocstyle - missing docstring in magic method
-    "D106",  # pydocstyle - missing docstring in public nested class
-    "D107",  # pydocstyle - missing docstring in __init__
-    "D202",  # pydocstyle - no blank lines allowed after function docstring
-    "D205",  # pydocstyle - 1 blank line required between summary line and description
-    "D415",  # pydocstyle - first line should end with a period, question mark, or exclamation point
-    "E501",  # pycodestyle line too long, handled by black
-    "UP037", # pyupgrade - removes quotes from type annotation
-]
-line-length = 120 # match Black
-target-version = 'py311'
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 12
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/**/*.*" = ["BLE001", "S101"]
 "tests/loadtest.py" = ["T201"]
```

### Comparing `asyncio_pool_ng-0.8.0/PKG-INFO` & `asyncio_pool_ng-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: asyncio-pool-ng
-Version: 0.8.0
+Version: 0.8.1
 Summary: A pool of coroutine functions.
 Home-page: https://github.com/smithk86/asyncio-pool-ng
 License: MIT
 Author: Kyle Smith
 Author-email: smithk86@smc3.com
 Requires-Python: >=3.11,<4
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Documentation, https://smithk86.github.io/asyncio-pool-ng
 Project-URL: Repository, https://github.com/smithk86/asyncio-pool-ng
 Description-Content-Type: text/markdown
 
 # asyncio-pool-ng
```

