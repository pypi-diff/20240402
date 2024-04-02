# Comparing `tmp/delayed-1.0.1b1.tar.gz` & `tmp/delayed-1.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delayed-1.0.1b1.tar", last modified: Wed Mar 27 17:29:12 2024, max compression
+gzip compressed data, was "delayed-1.2.0b1.tar", last modified: Tue Apr  2 08:31:18 2024, max compression
```

## Comparing `delayed-1.0.1b1.tar` & `delayed-1.2.0b1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-03-27 17:29:12.076652 delayed-1.0.1b1/
--rw-r--r--   0 keakon     (501) staff       (20)     1063 2024-03-27 06:18:19.000000 delayed-1.0.1b1/LICENSE
--rw-r--r--   0 keakon     (501) staff       (20)       16 2024-03-27 06:18:19.000000 delayed-1.0.1b1/MANIFEST.in
--rw-r--r--   0 keakon     (501) staff       (20)     8745 2024-03-27 17:29:12.076449 delayed-1.0.1b1/PKG-INFO
--rw-r--r--   0 keakon     (501) staff       (20)     7909 2024-03-27 09:41:31.000000 delayed-1.0.1b1/README.md
-drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-03-27 17:29:12.073327 delayed-1.0.1b1/delayed/
--rw-r--r--   0 keakon     (501) staff       (20)       49 2024-03-27 17:26:03.000000 delayed-1.0.1b1/delayed/__init__.py
--rw-r--r--   0 keakon     (501) staff       (20)      177 2024-03-27 06:18:19.000000 delayed-1.0.1b1/delayed/constants.py
--rw-r--r--   0 keakon     (501) staff       (20)      638 2024-03-27 06:18:19.000000 delayed-1.0.1b1/delayed/delay.py
--rw-r--r--   0 keakon     (501) staff       (20)      718 2024-03-27 06:18:19.000000 delayed-1.0.1b1/delayed/keep_alive.py
--rw-r--r--   0 keakon     (501) staff       (20)     1510 2024-03-27 08:35:28.000000 delayed-1.0.1b1/delayed/logger.py
--rw-r--r--   0 keakon     (501) staff       (20)     4790 2024-03-27 09:53:47.000000 delayed-1.0.1b1/delayed/queue.py
--rw-r--r--   0 keakon     (501) staff       (20)     1306 2024-03-27 09:39:19.000000 delayed-1.0.1b1/delayed/sweeper.py
--rw-r--r--   0 keakon     (501) staff       (20)     3433 2024-03-27 09:00:00.000000 delayed-1.0.1b1/delayed/task.py
--rw-r--r--   0 keakon     (501) staff       (20)     3835 2024-03-27 17:21:46.000000 delayed-1.0.1b1/delayed/worker.py
-drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-03-27 17:29:12.076112 delayed-1.0.1b1/delayed.egg-info/
--rw-r--r--   0 keakon     (501) staff       (20)     8745 2024-03-27 17:29:12.000000 delayed-1.0.1b1/delayed.egg-info/PKG-INFO
--rw-r--r--   0 keakon     (501) staff       (20)      518 2024-03-27 17:29:12.000000 delayed-1.0.1b1/delayed.egg-info/SOURCES.txt
--rw-r--r--   0 keakon     (501) staff       (20)        1 2024-03-27 17:29:12.000000 delayed-1.0.1b1/delayed.egg-info/dependency_links.txt
--rw-r--r--   0 keakon     (501) staff       (20)       22 2024-03-27 17:29:12.000000 delayed-1.0.1b1/delayed.egg-info/requires.txt
--rw-r--r--   0 keakon     (501) staff       (20)        8 2024-03-27 17:29:12.000000 delayed-1.0.1b1/delayed.egg-info/top_level.txt
--rw-r--r--   0 keakon     (501) staff       (20)      191 2024-03-27 17:29:12.076945 delayed-1.0.1b1/setup.cfg
--rw-r--r--   0 keakon     (501) staff       (20)     1092 2024-03-27 08:23:52.000000 delayed-1.0.1b1/setup.py
-drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-03-27 17:29:12.075666 delayed-1.0.1b1/tests/
--rw-r--r--   0 keakon     (501) staff       (20)      403 2024-03-27 06:18:19.000000 delayed-1.0.1b1/tests/test_delay.py
--rw-r--r--   0 keakon     (501) staff       (20)      415 2024-03-27 06:18:19.000000 delayed-1.0.1b1/tests/test_keep_alive.py
--rw-r--r--   0 keakon     (501) staff       (20)      687 2024-03-27 06:18:19.000000 delayed-1.0.1b1/tests/test_logger.py
--rw-r--r--   0 keakon     (501) staff       (20)     3351 2024-03-27 06:18:19.000000 delayed-1.0.1b1/tests/test_queue.py
--rw-r--r--   0 keakon     (501) staff       (20)     1151 2024-03-27 06:18:19.000000 delayed-1.0.1b1/tests/test_sweeper.py
--rw-r--r--   0 keakon     (501) staff       (20)     1726 2024-03-27 06:18:19.000000 delayed-1.0.1b1/tests/test_task.py
--rw-r--r--   0 keakon     (501) staff       (20)      473 2024-03-27 06:18:19.000000 delayed-1.0.1b1/tests/test_worker.py
+drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-04-02 08:31:18.624708 delayed-1.2.0b1/
+-rw-r--r--   0 keakon     (501) staff       (20)     1063 2024-03-27 06:18:19.000000 delayed-1.2.0b1/LICENSE
+-rw-r--r--   0 keakon     (501) staff       (20)       16 2024-03-27 06:18:19.000000 delayed-1.2.0b1/MANIFEST.in
+-rw-r--r--   0 keakon     (501) staff       (20)     9537 2024-04-02 08:31:18.624583 delayed-1.2.0b1/PKG-INFO
+-rw-r--r--   0 keakon     (501) staff       (20)     8701 2024-04-02 08:30:03.000000 delayed-1.2.0b1/README.md
+drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-04-02 08:31:18.621639 delayed-1.2.0b1/delayed/
+-rw-r--r--   0 keakon     (501) staff       (20)       49 2024-04-02 08:30:34.000000 delayed-1.2.0b1/delayed/__init__.py
+-rw-r--r--   0 keakon     (501) staff       (20)      169 2024-03-29 02:03:21.000000 delayed-1.2.0b1/delayed/constants.py
+-rw-r--r--   0 keakon     (501) staff       (20)     1120 2024-04-02 07:53:33.000000 delayed-1.2.0b1/delayed/delay.py
+-rw-r--r--   0 keakon     (501) staff       (20)      837 2024-03-29 07:45:55.000000 delayed-1.2.0b1/delayed/keep_alive.py
+-rw-r--r--   0 keakon     (501) staff       (20)     1767 2024-03-29 03:24:55.000000 delayed-1.2.0b1/delayed/logger.py
+-rw-r--r--   0 keakon     (501) staff       (20)     5538 2024-04-02 08:16:56.000000 delayed-1.2.0b1/delayed/queue.py
+-rw-r--r--   0 keakon     (501) staff       (20)     1306 2024-03-27 09:39:19.000000 delayed-1.2.0b1/delayed/sweeper.py
+-rw-r--r--   0 keakon     (501) staff       (20)     3706 2024-04-02 08:26:28.000000 delayed-1.2.0b1/delayed/task.py
+-rw-r--r--   0 keakon     (501) staff       (20)     5107 2024-04-02 08:24:26.000000 delayed-1.2.0b1/delayed/worker.py
+drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-04-02 08:31:18.624266 delayed-1.2.0b1/delayed.egg-info/
+-rw-r--r--   0 keakon     (501) staff       (20)     9537 2024-04-02 08:31:18.000000 delayed-1.2.0b1/delayed.egg-info/PKG-INFO
+-rw-r--r--   0 keakon     (501) staff       (20)      518 2024-04-02 08:31:18.000000 delayed-1.2.0b1/delayed.egg-info/SOURCES.txt
+-rw-r--r--   0 keakon     (501) staff       (20)        1 2024-04-02 08:31:18.000000 delayed-1.2.0b1/delayed.egg-info/dependency_links.txt
+-rw-r--r--   0 keakon     (501) staff       (20)       22 2024-04-02 08:31:18.000000 delayed-1.2.0b1/delayed.egg-info/requires.txt
+-rw-r--r--   0 keakon     (501) staff       (20)        8 2024-04-02 08:31:18.000000 delayed-1.2.0b1/delayed.egg-info/top_level.txt
+-rw-r--r--   0 keakon     (501) staff       (20)      191 2024-04-02 08:31:18.624961 delayed-1.2.0b1/setup.cfg
+-rw-r--r--   0 keakon     (501) staff       (20)     1092 2024-03-27 08:23:52.000000 delayed-1.2.0b1/setup.py
+drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-04-02 08:31:18.623979 delayed-1.2.0b1/tests/
+-rw-r--r--   0 keakon     (501) staff       (20)     1555 2024-04-02 08:07:47.000000 delayed-1.2.0b1/tests/test_delay.py
+-rw-r--r--   0 keakon     (501) staff       (20)      415 2024-03-27 06:18:19.000000 delayed-1.2.0b1/tests/test_keep_alive.py
+-rw-r--r--   0 keakon     (501) staff       (20)      687 2024-03-27 06:18:19.000000 delayed-1.2.0b1/tests/test_logger.py
+-rw-r--r--   0 keakon     (501) staff       (20)     4435 2024-03-29 08:23:53.000000 delayed-1.2.0b1/tests/test_queue.py
+-rw-r--r--   0 keakon     (501) staff       (20)     1396 2024-03-29 07:35:04.000000 delayed-1.2.0b1/tests/test_sweeper.py
+-rw-r--r--   0 keakon     (501) staff       (20)     3384 2024-04-02 05:30:19.000000 delayed-1.2.0b1/tests/test_task.py
+-rw-r--r--   0 keakon     (501) staff       (20)     1198 2024-04-02 08:27:47.000000 delayed-1.2.0b1/tests/test_worker.py
```

### Comparing `delayed-1.0.1b1/LICENSE` & `delayed-1.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `delayed-1.0.1b1/PKG-INFO` & `delayed-1.2.0b1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: delayed
-Version: 1.0.1b1
-Summary: a simple but robust task queue
-Home-page: https://github.com/keakon/delayed
-Author: keakon
-Author-email: keakon@gmail.com
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: hiredis
-Requires-Dist: redis
-Requires-Dist: msgpack
-
 # delayed
 [![Build Status](https://github.com/keakon/delayed/actions/workflows/python.yml/badge.svg)](https://github.com/keakon/delayed/actions)
 [![Coverage](https://codecov.io/gh/keakon/delayed/branch/master/graph/badge.svg)](https://codecov.io/gh/keakon/delayed)
 
 Delayed is a simple but robust task queue inspired by [rq](https://python-rq.org/).
 
 ## Features
@@ -70,53 +46,64 @@
     * Four ways to enqueue Python tasks:
         1. Define a task function and enqueue it:
 
             ```python
             from delayed.delay import delayed
 
             delayed = delayed(queue)
+            i = 0
 
             @delayed
             def delayed_add(a, b):
                 return a + b
 
+            @delayed(retry=3)
+            def retry_div(x):
+                global i
+                i += 1
+                return x / (i - 1)
+
             delayed_add.delay(1, 2)  # enqueue delayed_add
             delayed_add.delay(1, b=2)  # same as above
             delayed_add(1, 2)  # call it immediately
+            
+            retry_div.delay(1)  # enqueue retry_div
             ```
         2. Directly enqueue a function:
 
             ```python
             from delayed.delay import delayed
 
             delayed = delayed(queue)
 
             def add(a, b):
                 return a + b
 
             delayed(add).delay(1, 2)
             delayed(add).delay(1, b=2)  # same as above
+            delayed(retry=3)(add).delay(1, b=2)
+            delayed(add, retry=3).delay(1, b=2)  # same as above
             ```
         3. Create a task and enqueue it:
 
             ```python
             from delayed.task import PyTask
 
             def add(a, b):
                 return a + b
 
-            task = PyTask(func=add, args=(1,), kwargs={'b': 2})
+            task = PyTask(func=add, args=(1,), kwargs={'b': 2}, retry=1)
             queue.enqueue(task)
             ```
         4. Enqueue a predefined task function without importing it (the fastest and lightest way):
 
             ```python
             from delayed.task import PyTask
 
-            task = PyTask(func='test:add', args=(1,), kwargs={'b': 2})
+            task = PyTask(func='test:add', args=(1,), kwargs={'b': 2}, retry=1)
             queue.enqueue(task)
             ```
     * Enqueue Go tasks:
 
         ```python
             from delayed.task import GoTask
 
@@ -197,14 +184,24 @@
     from delayed.logger import setup_logger
 
     setup_logger()
     ```
 
 ## Release notes
 
+* 1.2:
+    1. Adds `retry` param to functions wrapped by `delayed.delay()`.
+    2. Adds `retry` param to `Task()`.
+    3. Adds `release` param to `Queue.enqueue()`.
+    4. The `Worker` won't retry a failed task infinitely by default now. You can set `retry=-1` to `Task()` instead. (BREAKING CHANGE)
+
+* 1.1:
+    1. Adds `log_level` param to `delayed.logger.setup_logger()`.
+    2. Prevents different online workers have the same id.
+
 * 1.0:
     1. Python 2.7 is not supported anymore. (BREAKING CHANGE)
     2. Supports Go, adds `GoTask`.
     3. Use MessagePack instead of pickle to serialize / deserialize tasks. (BREAKING CHANGE)
     4. Removes `ForkedWorker` and `PreforkedWorker`. You can use `Worker` instead. (BREAKING CHANGE)
     5. Changes params of `Queue()`, removes `default_timeout`, `requeue_timeout` and `busy_len`, adds `dequeue_timeout` and `keep_alive_timeout`. (BREAKING CHANGE)
     6. Rename `Task` to `PyTask`. (BREAKING CHANGE)
```

### Comparing `delayed-1.0.1b1/README.md` & `delayed-1.2.0b1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: delayed
+Version: 1.2.0b1
+Summary: a simple but robust task queue
+Home-page: https://github.com/keakon/delayed
+Author: keakon
+Author-email: keakon@gmail.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=2.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: hiredis
+Requires-Dist: redis
+Requires-Dist: msgpack
+
 # delayed
 [![Build Status](https://github.com/keakon/delayed/actions/workflows/python.yml/badge.svg)](https://github.com/keakon/delayed/actions)
 [![Coverage](https://codecov.io/gh/keakon/delayed/branch/master/graph/badge.svg)](https://codecov.io/gh/keakon/delayed)
 
 Delayed is a simple but robust task queue inspired by [rq](https://python-rq.org/).
 
 ## Features
@@ -46,53 +70,64 @@
     * Four ways to enqueue Python tasks:
         1. Define a task function and enqueue it:
 
             ```python
             from delayed.delay import delayed
 
             delayed = delayed(queue)
+            i = 0
 
             @delayed
             def delayed_add(a, b):
                 return a + b
 
+            @delayed(retry=3)
+            def retry_div(x):
+                global i
+                i += 1
+                return x / (i - 1)
+
             delayed_add.delay(1, 2)  # enqueue delayed_add
             delayed_add.delay(1, b=2)  # same as above
             delayed_add(1, 2)  # call it immediately
+            
+            retry_div.delay(1)  # enqueue retry_div
             ```
         2. Directly enqueue a function:
 
             ```python
             from delayed.delay import delayed
 
             delayed = delayed(queue)
 
             def add(a, b):
                 return a + b
 
             delayed(add).delay(1, 2)
             delayed(add).delay(1, b=2)  # same as above
+            delayed(retry=3)(add).delay(1, b=2)
+            delayed(add, retry=3).delay(1, b=2)  # same as above
             ```
         3. Create a task and enqueue it:
 
             ```python
             from delayed.task import PyTask
 
             def add(a, b):
                 return a + b
 
-            task = PyTask(func=add, args=(1,), kwargs={'b': 2})
+            task = PyTask(func=add, args=(1,), kwargs={'b': 2}, retry=1)
             queue.enqueue(task)
             ```
         4. Enqueue a predefined task function without importing it (the fastest and lightest way):
 
             ```python
             from delayed.task import PyTask
 
-            task = PyTask(func='test:add', args=(1,), kwargs={'b': 2})
+            task = PyTask(func='test:add', args=(1,), kwargs={'b': 2}, retry=1)
             queue.enqueue(task)
             ```
     * Enqueue Go tasks:
 
         ```python
             from delayed.task import GoTask
 
@@ -173,14 +208,24 @@
     from delayed.logger import setup_logger
 
     setup_logger()
     ```
 
 ## Release notes
 
+* 1.2:
+    1. Adds `retry` param to functions wrapped by `delayed.delay()`.
+    2. Adds `retry` param to `Task()`.
+    3. Adds `release` param to `Queue.enqueue()`.
+    4. The `Worker` won't retry a failed task infinitely by default now. You can set `retry=-1` to `Task()` instead. (BREAKING CHANGE)
+
+* 1.1:
+    1. Adds `log_level` param to `delayed.logger.setup_logger()`.
+    2. Prevents different online workers have the same id.
+
 * 1.0:
     1. Python 2.7 is not supported anymore. (BREAKING CHANGE)
     2. Supports Go, adds `GoTask`.
     3. Use MessagePack instead of pickle to serialize / deserialize tasks. (BREAKING CHANGE)
     4. Removes `ForkedWorker` and `PreforkedWorker`. You can use `Worker` instead. (BREAKING CHANGE)
     5. Changes params of `Queue()`, removes `default_timeout`, `requeue_timeout` and `busy_len`, adds `dequeue_timeout` and `keep_alive_timeout`. (BREAKING CHANGE)
     6. Rename `Task` to `PyTask`. (BREAKING CHANGE)
```

### Comparing `delayed-1.0.1b1/delayed/keep_alive.py` & `delayed-1.2.0b1/delayed/keep_alive.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import threading
+from typing import TYPE_CHECKING
 
 from .constants import Status
 from .logger import logger
 
+if TYPE_CHECKING:  # pragma: no cover
+    from .worker import Worker
+
 
 class KeepAliveThread(threading.Thread):
-    def __init__(self, worker):
+    def __init__(self, worker: 'Worker'):
         super(KeepAliveThread, self).__init__()
         self._worker = worker
 
     def run(self):
         worker = self._worker
         queue = worker._queue
         interval = self._worker._keep_alive_interval
         while worker._status != Status.STOPPED:  # this thread can eventually see worker._status changed by other thread
             try:
                 queue.keep_alive()
             except Exception:
                 logger.exception('Failed to keep alive.')
             with worker._cond:
                 worker._cond.wait(interval)
-        queue._die()
+        queue.go_offline()
```

### Comparing `delayed-1.0.1b1/delayed/logger.py` & `delayed-1.2.0b1/delayed/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,55 @@
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 logger.propagate = False
 _null_handler = logging.NullHandler()
 logger.addHandler(_null_handler)
 
 
-def set_handler(handler):
+def set_handler(handler: logging.Handler):
     """Set the handler of the logger.
 
     Args:
         handler (logging.Handler): The handler to be set.
     """
     logger.handlers = [handler]
 
 
-def setup_logger(date_format: str = DEFAULT_DATE_FORMAT, log_format: str = DEFAULT_LOG_FORMAT):
+def setup_logger(
+    date_format: str = DEFAULT_DATE_FORMAT,
+    log_format: str = DEFAULT_LOG_FORMAT,
+    log_level: int = logging.DEBUG
+):
     """Setup a console logger.
 
     Args:
         date_format (str): The date format of the logger.
         log_format (str): The log format of the logger.
+        log_level (int): The log level of the logger.
     """
     logger.removeHandler(_null_handler)
     if logger.handlers:
         for handler in logger.handlers:
-            _setup_handler(handler, date_format, log_format)
+            _setup_handler(handler, date_format, log_format, log_level)
     else:
         handler = logging.StreamHandler()
-        _setup_handler(handler, date_format, log_format)
+        _setup_handler(handler, date_format, log_format, log_level)
         logger.addHandler(handler)
 
 
-def _setup_handler(handler, date_format: str, log_format: str):
+def _setup_handler(
+    handler: logging.Handler,
+    date_format: str,
+    log_format: str,
+    log_level: int = logging.DEBUG
+):
     """Setup a handler for the logger.
 
     Args:
         handler (logging.Handler): The handler to be setup.
         date_format (str): The date format of the handler.
         log_format (str): The log format of the handler.
+        log_level (int): The log level of the handler.
     """
-    handler.setLevel(logging.DEBUG)
+    handler.setLevel(log_level)
     formatter = logging.Formatter(fmt=log_format, datefmt=date_format)
     handler.setFormatter(formatter)
```

### Comparing `delayed-1.0.1b1/delayed/queue.py` & `delayed-1.2.0b1/delayed/queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
+from math import ceil
 from typing import Optional, Union
 
 import redis
 
 from .logger import logger
-from .task import PyTask
+from .task import GoTask, PyTask
 
 
 # KEYS: queue_name, processing_key
 # ARGV: worker_id
 _DEQUEUE_SCRIPT = '''local task = redis.call('lpop', KEYS[1])
 if task == nil then
     return nil
@@ -51,38 +52,49 @@
         name (str): The task queue name.
         conn (redis.Redis): A redis connection.
         dequeue_timeout (int or float): The dequeue timeout in seconds of the task queue.
             The task queue will block at most `dequeue_timeout` seconds for receiving a new task.
         keep_alive_timeout (int or float): The keep alive timeout in seconds of the worker.
     """
 
-    def __init__(self, name: str, conn: redis.Redis, dequeue_timeout: Union[int, float] = 1, keep_alive_timeout: Union[int, float] = 60):
-        self._worker_id: Optional[bytes] = None
+    def __init__(
+        self, name: str,
+        conn: redis.Redis,
+        dequeue_timeout: Union[int, float] = 1,
+        keep_alive_timeout: Union[int, float] = 60
+    ):
+        self._worker_id: Optional[int] = None
         self._name = name
         self._noti_key = name + _NOTI_KEY_SUFFIX
         self._processing_key = name + _PROCESSING_KEY_SUFFIX
         self._conn = conn
         self._dequeue_timeout = dequeue_timeout
         self._keep_alive_timeout = keep_alive_timeout
         self._dequeue_script = conn.register_script(_DEQUEUE_SCRIPT)
         self._requeue_lost_script = conn.register_script(_REQUEUE_LOST_SCRIPT)
 
-    def enqueue(self, task: PyTask):
+    def enqueue(self, task: Union[GoTask, PyTask], release=False):
         """Enqueues a task to the queue.
 
         Args:
             task (delayed.task.PyTask or delayed.task.GoTask): The task to be enqueued.
+            relase (bool): Whether to release the previous dequeued task after enqueuing.
         """
         logger.debug('Enqueuing task %s.', task._func_path)
         data = task.serialize()
-        with self._conn.pipeline() as pipe:
-            pipe.rpush(self._name, data)
-            pipe.rpush(self._noti_key, '1')
-            pipe.execute()
-        logger.debug('Enqueued task %s.', task._func_path)
+        if data:
+            with self._conn.pipeline() as pipe:
+                pipe.rpush(self._name, data)
+                pipe.rpush(self._noti_key, '1')
+                if release:
+                    self._conn.hdel(self._processing_key, self._worker_id)
+                pipe.execute()
+            logger.debug('Enqueued task %s.', task._func_path)
+        else:  # pragma: no cover
+            logger.error('Failed to serialize task %s.', task._func_path)
 
     def dequeue(self) -> Optional[PyTask]:
         """Dequeues a task from the queue.
 
         Returns:
             delayed.task.PyTask or None: The dequeued task, or None if the queue is empty.
         """
@@ -112,25 +124,32 @@
         """Requeues lost tasks.
         It should be called periodically to prevent losing tasks.
         The lost tasks were those popped from the queue, but its dead worker hadn't released it.
 
         Returns:
             int: The requeued task count.
         """
-        count = self._requeue_lost_script(
+        count: int = self._requeue_lost_script(
             keys=(self._name, self._noti_key, self._processing_key))
         if count >= 1:
             if count == 1:
                 logger.debug('Requeued 1 lost task.')
             else:
                 logger.debug('Requeued %d lost tasks.', count)
         return count
 
     def keep_alive(self):
         """Set the worker of the queue alive."""
         self._conn.setex(self._worker_id, self._keep_alive_timeout, 1)
         logger.debug('Worker %s is alive.', self._worker_id)
 
-    def _die(self):
-        """Set the worker of the queue dead."""
+    def go_offline(self):
+        """Set the worker of the queue offline."""
         self._conn.delete(self._worker_id)
-        logger.debug('Worker %s dies.', self._worker_id)
+        logger.debug('Worker %s is offline.', self._worker_id)
+
+    def try_online(self) -> bool:
+        """Try to set the worker of the queue online."""
+        if self._conn.set(self._worker_id, 1, ex=ceil(self._keep_alive_timeout), nx=True):
+            logger.debug('Worker %s is online.', self._worker_id)
+            return True
+        return False
```

### Comparing `delayed-1.0.1b1/delayed/sweeper.py` & `delayed-1.2.0b1/delayed/sweeper.py`

 * *Files identical despite different names*

### Comparing `delayed-1.0.1b1/delayed/task.py` & `delayed-1.2.0b1/delayed/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,54 +14,64 @@
 
     Args:
         func (callable or str): The task function or function path.
             The function should be defined in module level (except the `__main__` module).
             The function path format is "module.path:func_name".
         args (list or tuple): Variable length argument list of the task function.
         kwargs (dict): Arbitrary keyword arguments of the task function.
+        retry (int): The number of retry times. Minus value means retry until succeeds.
     """
 
-    __slots__ = ['_func_path', '_args', '_kwargs', '_data']
+    __slots__ = ['_func_path', '_args', '_kwargs', '_data', '_retry']
 
-    def __init__(self, func: Union[Callable, str], args: Union[list, tuple, None] = None, kwargs: Optional[dict] = None):
+    def __init__(
+        self,
+        func: Union[Callable, str],
+        args: Union[list, tuple, None] = None,
+        kwargs: Optional[dict] = None,
+        retry: int = 0,
+    ):
         if isinstance(func, str):
             self._func_path = func
         elif callable(func):
             self._func_path = func.__module__ + SEP + func.__name__
         else:
             raise ValueError('Invalid func %r' % func)
         self._args = () if args is None else args
         self._kwargs = {} if kwargs is None else kwargs
+        self._retry = retry
         self._data = None
 
     def serialize(self) -> Optional[bytes]:
         """Serializes the task to bytes.
 
         Returns:
-            str: The serialized data.
+            bytes: The serialized data.
         """
         if self._data is None:
-            data = self._func_path, self._args, self._kwargs
+            data = self._func_path, self._args, self._kwargs, self._retry
 
             i = 0
-            if not self._kwargs:
+            if self._retry <= 0:
                 i -= 1
-                if not self._args:
+                if not self._kwargs:
                     i -= 1
+                    if not self._args:
+                        i -= 1
             if i < 0:
                 data = data[:i]
             self._data = packb(data)
         return self._data
 
     @classmethod
-    def deserialize(cls, data) -> 'PyTask':
+    def deserialize(cls, data: bytes) -> 'PyTask':
         """Deserialize a task from the bytes.
 
         Args:
-            data (str): The string to be deserialize.
+            data (bytes): The bytes to be deserialize.
 
         Returns:
             PyTask: The deserialized task.
         """
         task = cls(*unpackb(data))
         task._data = data
         return task
@@ -87,15 +97,15 @@
         func_path (str): The task function path.
             The format is "package/path.func_name".
         args (any): Arguments of the task function.
     """
 
     __slots__ = ['_func_path', '_args', '_payload', '_data']
 
-    def __init__(self, func_path: str, args: Optional[list] = None):
+    def __init__(self, func_path: str, args: Any = None):
         self._func_path = func_path
         self._args = args
         self._payload = None
         self._data = None
 
     def serialize(self) -> Optional[bytes]:
         """Serializes the task to bytes.
```

### Comparing `delayed-1.0.1b1/delayed/worker.py` & `delayed-1.2.0b1/delayed/worker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,139 @@
 # -*- coding: utf-8 -*-
 
-import binascii
-import os
+from secrets import randbits
 import signal
-import sys
-import threading
-import time
-import traceback
+from sys import exc_info
+from threading import Condition
+from time import sleep
 from typing import Union
 
 from .constants import DEFAULT_SLEEP_TIME, MAX_SLEEP_TIME, Status
 from .keep_alive import KeepAliveThread
 from .logger import logger
 from .queue import Queue
 from .task import PyTask
 
 class Worker:
     """Worker is the class of Python task worker.
 
     Args:
         queue (delayed.queue.Queue): The task queue of the worker.
         keep_alive_interval (int or float): The worker marks itself as alive for every `keep_alive_interval` seconds.
+        id_bits (int): The bits used for the worker ID. The default value is 16, which is enough for 2 ** 16 workers.
     """
 
-    def __init__(self, queue: Queue, keep_alive_interval: Union[int, float] = 15):
-        queue._worker_id = self._id = binascii.hexlify(os.urandom(16))
+    def __init__(
+        self,
+        queue: Queue,
+        keep_alive_interval: Union[int, float] = 15,
+        id_bits: int = 16
+    ):
         self._queue = queue
         self._keep_alive_interval = keep_alive_interval
+        self._id_bits = id_bits
         self._status = Status.STOPPED
-        self._cond = threading.Condition()
+        self._cond = Condition()
+
+    def generate_id(self):
+        """Generates a random ID for the worker."""
+        while True:
+            self._queue._worker_id = self._id = randbits(self._id_bits)
+            if self._queue.try_online():
+                return
 
     def run(self):  # pragma: no cover
         """Runs the worker."""
-        logger.debug('Starting worker %s.', self._id)
+        self.generate_id()
+
+        logger.debug('Starting worker %d.', self._id)
         self._status = Status.RUNNING
         self._register_signals()
 
         thread = KeepAliveThread(self)
         thread.start()
 
         try:
             sleep_time = DEFAULT_SLEEP_TIME
             while self._status == Status.RUNNING:
                 try:
                     task = self._queue.dequeue()
                 except Exception:  # pragma: no cover
                     logger.exception('Failed to dequeue task.')
-                    time.sleep(sleep_time)
+                    sleep(sleep_time)
                     sleep_time *= 2
                     if sleep_time > MAX_SLEEP_TIME:
                         sleep_time = MAX_SLEEP_TIME
                 else:
                     sleep_time = DEFAULT_SLEEP_TIME
                     if task:
                         try:
                             task.execute()
                         except Exception:
                             logger.exception('Failed to execute task %s.', task._func_path)
 
-                            _, _, exc_traceback = sys.exc_info()
-                            if len(traceback.format_tb(exc_traceback)) > 2:
-                                self._requeue_task(task)
+                            need_retry = False
+                            if task._retry:
+                                _, _, exc_traceback = exc_info()
+                                if exc_traceback:
+                                    tb_next = exc_traceback.tb_next
+                                    if tb_next:
+                                        tb_next2 = tb_next.tb_next
+                                        if tb_next2:
+                                            # invalid call, should not be retried
+                                            need_retry = True
+                                            # delete tracebacks to avoid memory leak
+                                            del tb_next2
+                                        del tb_next
+                                    del exc_traceback
+
+                            if need_retry:
+                                self._retry_task(task)
                             else:
-                                # invalid call, should not be retried
                                 self._release_task()
                         else:
                             self._release_task()
         finally:
             self._unregister_signals()
             self._status = Status.STOPPED
             with self._cond:
                 self._cond.notify()
             thread.join()
-            logger.debug('Stopped worker %s.', self._id)
+            logger.debug('Stopped worker %d.', self._id)
 
     def stop(self):
         """Stops the worker."""
         if self._status == Status.RUNNING:
-            logger.debug('Stopping worker %s.', self._id)
+            logger.debug('Stopping worker %d.', self._id)
             self._status = Status.STOPPING
 
-    def _requeue_task(self, task: PyTask):
-        """Requeues a dequeued task.
+    def _retry_task(self, task: PyTask):
+        """Retries a dequeued task.
 
         Args:
-            task (delayed.task.PyTask): The task to be requeued.
+            task (delayed.task.PyTask): The task to be retried.
         """
-        logger.debug('Requeuing task %s', task._func_path)
-        try:
-            self._queue.enqueue(task)
-        except Exception:
-            logger.exception('Failed to requeue task %s', task._func_path)
+        if task._retry:
+            if task._retry > 0:
+                task._retry -= 1
+            task._data = None
+            task.serialize()
+
+            logger.debug('Retrying task %s', task._func_path)
+            try:
+                self._queue.enqueue(task, release=True)
+            except Exception:  # pragma: no cover
+                logger.exception('Failed to retry task %s', task._func_path)
 
     def _release_task(self):
         """Releases the currently dequeued task."""
         try:
             self._queue.release()
         except Exception:  # pragma: no cover
-            logger.exception('Failed to release task of worker %s.', self._id)
+            logger.exception('Failed to release task of worker %d.', self._id)
 
     def _register_signals(self):
         """Registers signal handlers."""
         def stop(signum, frame):
             logger.debug('Received SIGHUP.')
             self.stop()
         signal.signal(signal.SIGHUP, stop)
```

### Comparing `delayed-1.0.1b1/delayed.egg-info/PKG-INFO` & `delayed-1.2.0b1/delayed.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delayed
-Version: 1.0.1b1
+Version: 1.2.0b1
 Summary: a simple but robust task queue
 Home-page: https://github.com/keakon/delayed
 Author: keakon
 Author-email: keakon@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -70,53 +70,64 @@
     * Four ways to enqueue Python tasks:
         1. Define a task function and enqueue it:
 
             ```python
             from delayed.delay import delayed
 
             delayed = delayed(queue)
+            i = 0
 
             @delayed
             def delayed_add(a, b):
                 return a + b
 
+            @delayed(retry=3)
+            def retry_div(x):
+                global i
+                i += 1
+                return x / (i - 1)
+
             delayed_add.delay(1, 2)  # enqueue delayed_add
             delayed_add.delay(1, b=2)  # same as above
             delayed_add(1, 2)  # call it immediately
+            
+            retry_div.delay(1)  # enqueue retry_div
             ```
         2. Directly enqueue a function:
 
             ```python
             from delayed.delay import delayed
 
             delayed = delayed(queue)
 
             def add(a, b):
                 return a + b
 
             delayed(add).delay(1, 2)
             delayed(add).delay(1, b=2)  # same as above
+            delayed(retry=3)(add).delay(1, b=2)
+            delayed(add, retry=3).delay(1, b=2)  # same as above
             ```
         3. Create a task and enqueue it:
 
             ```python
             from delayed.task import PyTask
 
             def add(a, b):
                 return a + b
 
-            task = PyTask(func=add, args=(1,), kwargs={'b': 2})
+            task = PyTask(func=add, args=(1,), kwargs={'b': 2}, retry=1)
             queue.enqueue(task)
             ```
         4. Enqueue a predefined task function without importing it (the fastest and lightest way):
 
             ```python
             from delayed.task import PyTask
 
-            task = PyTask(func='test:add', args=(1,), kwargs={'b': 2})
+            task = PyTask(func='test:add', args=(1,), kwargs={'b': 2}, retry=1)
             queue.enqueue(task)
             ```
     * Enqueue Go tasks:
 
         ```python
             from delayed.task import GoTask
 
@@ -197,14 +208,24 @@
     from delayed.logger import setup_logger
 
     setup_logger()
     ```
 
 ## Release notes
 
+* 1.2:
+    1. Adds `retry` param to functions wrapped by `delayed.delay()`.
+    2. Adds `retry` param to `Task()`.
+    3. Adds `release` param to `Queue.enqueue()`.
+    4. The `Worker` won't retry a failed task infinitely by default now. You can set `retry=-1` to `Task()` instead. (BREAKING CHANGE)
+
+* 1.1:
+    1. Adds `log_level` param to `delayed.logger.setup_logger()`.
+    2. Prevents different online workers have the same id.
+
 * 1.0:
     1. Python 2.7 is not supported anymore. (BREAKING CHANGE)
     2. Supports Go, adds `GoTask`.
     3. Use MessagePack instead of pickle to serialize / deserialize tasks. (BREAKING CHANGE)
     4. Removes `ForkedWorker` and `PreforkedWorker`. You can use `Worker` instead. (BREAKING CHANGE)
     5. Changes params of `Queue()`, removes `default_timeout`, `requeue_timeout` and `busy_len`, adds `dequeue_timeout` and `keep_alive_timeout`. (BREAKING CHANGE)
     6. Rename `Task` to `PyTask`. (BREAKING CHANGE)
```

### Comparing `delayed-1.0.1b1/delayed.egg-info/SOURCES.txt` & `delayed-1.2.0b1/delayed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delayed-1.0.1b1/setup.py` & `delayed-1.2.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `delayed-1.0.1b1/tests/test_logger.py` & `delayed-1.2.0b1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `delayed-1.0.1b1/tests/test_queue.py` & `delayed-1.2.0b1/tests/test_queue.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding: utf-8 -*-
 
+from delayed.queue import Queue
 from delayed.task import GoTask, PyTask
+from delayed.worker import Worker
 
 from .common import CONN, func, NOTI_KEY, PROCESSING_KEY, QUEUE, QUEUE_NAME
 
 
-class TestQueue(object):
+class TestQueue:
     def test_enqueue(self):
         CONN.delete(QUEUE_NAME, NOTI_KEY)
 
         task = PyTask(func, (1, 2))
         QUEUE.enqueue(task)
         assert CONN.llen(QUEUE_NAME) == 1
         assert CONN.llen(NOTI_KEY) == 1
@@ -35,30 +37,33 @@
         task2 = PyTask(func, (3,), {'b': 4})
         task3 = PyTask(func, kwargs={'a': 5, 'b': 6})
         QUEUE.enqueue(task1)
         QUEUE.enqueue(task2)
         QUEUE.enqueue(task3)
 
         task = QUEUE.dequeue()
+        assert task is not None
         assert CONN.llen(QUEUE_NAME) == 2
         assert CONN.llen(NOTI_KEY) == 2
         assert CONN.hget(PROCESSING_KEY, QUEUE._worker_id) == task._data
         assert task._func_path == 'tests.common:func'
         assert task._args == [1, 2]
         assert task._kwargs == {}
 
         task = QUEUE.dequeue()
+        assert task is not None
         assert CONN.llen(QUEUE_NAME) == 1
         assert CONN.llen(NOTI_KEY) == 1
         assert CONN.hget(PROCESSING_KEY, QUEUE._worker_id) == task._data
         assert task._func_path == 'tests.common:func'
         assert task._args == [3]
         assert task._kwargs == {'b': 4}
 
         task = QUEUE.dequeue()
+        assert task is not None
         assert CONN.llen(QUEUE_NAME) == 0
         assert CONN.llen(NOTI_KEY) == 0
         assert CONN.hget(PROCESSING_KEY, QUEUE._worker_id) == task._data
         assert task._func_path == 'tests.common:func'
         assert task._args == []
         assert task._kwargs == {'a': 5, 'b': 6}
 
@@ -96,17 +101,49 @@
 
         task = PyTask(func, (1, 2))
         QUEUE.enqueue(task)
         assert QUEUE.len() == 1
         assert QUEUE.requeue_lost() == 0
 
         QUEUE.dequeue()
+        # WORKER.generate_id() set the queue to online for at least 1 second.
+        # It prevents the queue to go offline in the middle of the test.
+        QUEUE.go_offline()
         assert QUEUE.requeue_lost() == 1
         assert QUEUE.len() == 1
 
         QUEUE.keep_alive()
         QUEUE.dequeue()
         assert QUEUE.requeue_lost() == 0
-        QUEUE._die()
+        QUEUE.go_offline()
         assert QUEUE.requeue_lost() == 1
 
+        task = PyTask(func, (2, 3))
+        QUEUE.enqueue(task)
+        assert QUEUE.len() == 2
+
+        queue = Queue(QUEUE_NAME, CONN, 0.01)
+        worker = Worker(queue)
+        worker.generate_id()
+        queue.go_offline()
+        assert QUEUE.dequeue()
+        assert queue.dequeue()
+        assert QUEUE.requeue_lost() == 2
+
         CONN.delete(QUEUE_NAME, NOTI_KEY, PROCESSING_KEY)
+
+    def test_try_online(self):
+        QUEUE.go_offline()
+        assert QUEUE.try_online()
+        assert not QUEUE.try_online()
+
+        QUEUE.go_offline()
+        assert QUEUE.try_online()
+
+        queue = Queue(QUEUE_NAME, CONN, 0.01)
+        queue._worker_id = QUEUE._worker_id
+        assert not queue.try_online()
+
+        QUEUE.go_offline()
+        assert queue.try_online()
+
+        queue.go_offline()
```

### Comparing `delayed-1.0.1b1/tests/test_sweeper.py` & `delayed-1.2.0b1/tests/test_sweeper.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,47 +2,54 @@
 
 import threading
 import time
 
 from delayed.queue import Queue, _NOTI_KEY_SUFFIX
 from delayed.sweeper import Sweeper
 from delayed.task import PyTask
+from pytest import fail
 
 from .common import CONN, func, QUEUE, QUEUE_NAME, NOTI_KEY
 
 
-class TestSweeper(object):
+class TestSweeper:
     def test_run(self):
         queue_name = 'test'
         noti_key = queue_name + _NOTI_KEY_SUFFIX
         CONN.delete(QUEUE_NAME, NOTI_KEY, queue_name, noti_key)
 
         queue = Queue('test', CONN, 0.01)
-        queue._worker_id = 'test'
+        queue._worker_id = 123
         sweeper = Sweeper([QUEUE, queue], 0.05)
 
         task = PyTask(func, (1, 2))
         QUEUE.enqueue(task)
         CONN.lpop(NOTI_KEY)
 
         task = QUEUE.dequeue()
         assert task is None
 
         thread = threading.Thread(target=sweeper.run)
         thread.start()
 
-        time.sleep(0.1)
-        task = QUEUE.dequeue()
-        assert task is not None
-        QUEUE.release()
-
-        task2 = PyTask(func, (1, 2))
-        queue.enqueue(task2)
-        CONN.lpop(noti_key)
-
-        time.sleep(0.1)
-        task2 = queue.dequeue()
-        assert task2 is not None
-        queue.release()
-
-        sweeper.stop()
-        thread.join()
+        try:
+            time.sleep(0.1)
+            task = QUEUE.dequeue()
+            assert task is not None
+            QUEUE.release()
+
+            task2 = PyTask(func, (1, 2))
+            queue.enqueue(task2)
+            CONN.lpop(noti_key)
+
+            for _ in range(10):  # retry for slow machines
+                time.sleep(0.1)
+                task2 = queue.dequeue()
+                if task2 is not None:
+                    break
+            else:
+                fail('task2 is None')
+
+            queue.release()
+        finally:
+            sweeper.stop()
+            thread.join()
```

