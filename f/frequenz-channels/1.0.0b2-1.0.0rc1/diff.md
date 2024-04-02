# Comparing `tmp/frequenz-channels-1.0.0b2.tar.gz` & `tmp/frequenz-channels-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-channels-1.0.0b2.tar", last modified: Wed Nov  1 16:16:43 2023, max compression
+gzip compressed data, was "frequenz-channels-1.0.0rc1.tar", last modified: Thu Mar  7 12:54:18 2024, max compression
```

## Comparing `frequenz-channels-1.0.0b2.tar` & `frequenz-channels-1.0.0rc1.tar`

### file list

```diff
@@ -1,34 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:16:43.886059 frequenz-channels-1.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/.darglint
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2023-11-01 16:16:43.886059 frequenz-channels-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-01 16:16:43.886059 frequenz-channels-1.0.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:16:43.882059 frequenz-channels-1.0.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:16:43.882059 frequenz-channels-1.0.0b2/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:16:43.886059 frequenz-channels-1.0.0b2/src/frequenz/channels/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/_anycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/_bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)    14061 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:16:43.886059 frequenz-channels-1.0.0b2/src/frequenz/channels/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/util/_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/util/_file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/util/_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/util/_merge_named.py
--rw-r--r--   0 runner    (1001) docker     (127)    16036 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/util/_select.py
--rw-r--r--   0 runner    (1001) docker     (127)    30182 2023-11-01 16:16:23.000000 frequenz-channels-1.0.0b2/src/frequenz/channels/util/_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 16:16:43.886059 frequenz-channels-1.0.0b2/src/frequenz_channels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2023-11-01 16:16:43.000000 frequenz-channels-1.0.0b2/src/frequenz_channels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-11-01 16:16:43.000000 frequenz-channels-1.0.0b2/src/frequenz_channels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 16:16:43.000000 frequenz-channels-1.0.0b2/src/frequenz_channels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-11-01 16:16:43.000000 frequenz-channels-1.0.0b2/src/frequenz_channels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-01 16:16:43.000000 frequenz-channels-1.0.0b2/src/frequenz_channels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:18.453081 frequenz-channels-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-03-07 12:54:18.453081 frequenz-channels-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8754 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 12:54:18.453081 frequenz-channels-1.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:18.449081 frequenz-channels-1.0.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:18.449081 frequenz-channels-1.0.0rc1/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:18.453081 frequenz-channels-1.0.0rc1/src/frequenz/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/_anycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/_receiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20600 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28710 2024-03-07 12:54:09.000000 frequenz-channels-1.0.0rc1/src/frequenz/channels/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:54:18.453081 frequenz-channels-1.0.0rc1/src/frequenz_channels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-03-07 12:54:18.000000 frequenz-channels-1.0.0rc1/src/frequenz_channels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-07 12:54:18.000000 frequenz-channels-1.0.0rc1/src/frequenz_channels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 12:54:18.000000 frequenz-channels-1.0.0rc1/src/frequenz_channels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-07 12:54:18.000000 frequenz-channels-1.0.0rc1/src/frequenz_channels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-07 12:54:18.000000 frequenz-channels-1.0.0rc1/src/frequenz_channels.egg-info/top_level.txt
```

### Comparing `frequenz-channels-1.0.0b2/LICENSE` & `frequenz-channels-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-channels-1.0.0b2/pyproject.toml` & `frequenz-channels-1.0.0rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 [build-system]
 requires = [
   "setuptools == 68.1.0",
   "setuptools_scm[toml] == 7.1.0",
-  "frequenz-repo-config[lib] == 0.7.2",
+  "frequenz-repo-config[lib] == 0.9.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-channels"
 description = "Channel implementations for Python"
 readme = "README.md"
@@ -33,50 +33,54 @@
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
 [project.optional-dependencies]
 dev-flake8 = [
-  "flake8 == 6.1.0",
+  "flake8 == 7.0.0",
   "flake8-docstrings == 1.7.0",
   "flake8-pyproject == 1.2.3",  # For reading the flake8 config from pyproject.toml
-  "pydoclint == 0.3.2",
+  "pydoclint == 0.4.1",
   "pydocstyle == 6.3.0",
 ]
-dev-formatting = ["black == 23.10.1", "isort == 5.12.0"]
+dev-formatting = ["black == 24.2.0", "isort == 5.13.2"]
 dev-mkdocs = [
-  "black == 23.10.1",
-  "Markdown==3.4.4",
-  "mike == 1.1.2",
+  "Markdown == 3.5.2",
+  "black == 24.2.0",
+  "frequenz-repo-config[lib] == 0.9.1",
+  "markdown-callouts == 0.4.0",
+  "markdown-svgbob == 202112.1022",
+  "mike == 2.0.0",
   "mkdocs-gen-files == 0.5.0",
+  "mkdocs-include-markdown-plugin == 6.0.4",
   "mkdocs-literate-nav == 0.6.1",
-  "mkdocs-material == 9.3.2",
-  "mkdocs-macros-plugin == 1.0.4",
-  "mkdocstrings[python] == 0.23.0",
-  "frequenz-repo-config[lib] == 0.7.2",
+  "mkdocs-macros-plugin == 1.0.5",
+  "mkdocs-material == 9.5.12",
+  "mkdocstrings[python] == 0.24.1",
+  "pymdownx-superfence-filter-lines == 0.1.0",
 ]
 dev-mypy = [
-  "mypy == 1.6.1",
-  "types-Markdown == 3.4.2.10",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-channels[dev-mkdocs,dev-noxfile,dev-pytest]",
+  "mypy == 1.8.0",
+  "types-Markdown == 3.5.0.20240129",
 ]
-dev-noxfile = ["nox == 2023.4.22", "frequenz-repo-config[lib] == 0.7.2"]
+dev-noxfile = ["nox == 2023.4.22", "frequenz-repo-config[lib] == 0.9.1"]
 dev-pylint = [
-  "pylint == 2.17.7",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-channels[dev-mkdocs,dev-noxfile,dev-pytest]",
+  "pylint == 3.1.0",
 ]
 dev-pytest = [
-  "pytest == 7.4.3",
   "async-solipsism == 0.5",
-  "hypothesis == 6.88.1",
-  "frequenz-repo-config[extra-lint-examples] == 0.7.2",
-  "pytest-asyncio == 0.21.1",
+  "frequenz-repo-config[extra-lint-examples] == 0.9.1",
+  "hypothesis == 6.98.17",
+  "pytest == 8.1.0",
+  "pytest-asyncio == 0.23.5",
   "pytest-mock == 3.12.0",
 ]
 dev = [
   "frequenz-channels[dev-mkdocs,dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
@@ -125,14 +129,16 @@
   # disabled because it conflicts with isort
   "wrong-import-order",
   "ungrouped-imports",
   # pylint's unsubscriptable check is buggy and is not needed because
   # it is a type-check, for which we already have mypy.
   "unsubscriptable-object",
   # Checked by flake8
+  "redefined-outer-name",
+  "unused-import",
   "line-too-long",
   "unused-variable",
   "unnecessary-lambda-assignment",
 ]
 
 [tool.pytest.ini_options]
 testpaths = ["tests", "src"]
```

### Comparing `frequenz-channels-1.0.0b2/src/frequenz/channels/_bidirectional.py` & `frequenz-channels-1.0.0rc1/src/frequenz/channels/event.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,163 +1,180 @@
 # License: MIT
-# Copyright © 2022 Frequenz Energy-as-a-Service GmbH
+# Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
-"""An abstraction to provide bi-directional communication between actors."""
+"""A receiver that can be made ready directly.
 
-from __future__ import annotations
+!!! Tip inline end
 
-from typing import Generic, TypeVar
+    Read the [`Event`][frequenz.channels.event.Event] documentation for more
+    information.
 
-from ._base_classes import Receiver, Sender, T, U
-from ._broadcast import Broadcast
-from ._exceptions import ChannelError, ReceiverError, SenderError
-
-V = TypeVar("V")
-W = TypeVar("W")
-
-
-class Bidirectional(Generic[T, U]):
-    """A wrapper class for simulating bidirectional channels."""
-
-    class Handle(Sender[V], Receiver[W]):
-        """A handle to a [Bidirectional][frequenz.channels.Bidirectional] instance.
-
-        It can be used to send/receive values between the client and service.
-        """
-
-        def __init__(
-            self,
-            channel: Bidirectional[V, W] | Bidirectional[W, V],
-            sender: Sender[V],
-            receiver: Receiver[W],
-        ) -> None:
-            """Create a `Bidirectional.Handle` instance.
-
-            Args:
-                channel: The underlying channel.
-                sender: A sender to send values with.
-                receiver: A receiver to receive values from.
-            """
-            self._chan = channel
-            """The underlying channel."""
-
-            self._sender = sender
-            """The sender to send values with."""
-
-            self._receiver = receiver
-            """The receiver to receive values from."""
-
-        async def send(self, msg: V) -> None:
-            """Send a value to the other side.
-
-            Args:
-                msg: The value to send.
-
-            Raises:
-                SenderError: if the underlying channel was closed.
-                    A [ChannelClosedError][frequenz.channels.ChannelClosedError]
-                    is set as the cause.
-            """
-            try:
-                await self._sender.send(msg)
-            except SenderError as err:
-                # If this comes from a channel error, then we inject another
-                # ChannelError having the information about the Bidirectional
-                # channel to hide (at least partially) the underlying
-                # Broadcast channels we use.
-                if isinstance(err.__cause__, ChannelError):
-                    this_chan_error = ChannelError(
-                        f"Error in the underlying channel {err.__cause__.channel}: {err.__cause__}",
-                        self._chan,  # pylint: disable=protected-access
-                    )
-                    this_chan_error.__cause__ = err.__cause__
-                    err.__cause__ = this_chan_error
-                raise err
-
-        async def ready(self) -> bool:
-            """Wait until the receiver is ready with a value or an error.
-
-            Once a call to `ready()` has finished, the value should be read with
-            a call to `consume()` (`receive()` or iterated over). The receiver will
-            remain ready (this method will return immediately) until it is
-            consumed.
-
-            Returns:
-                Whether the receiver is still active.
-            """
-            return await self._receiver.ready()  # pylint: disable=protected-access
-
-        def consume(self) -> W:
-            """Return the latest value once `_ready` is complete.
-
-            Returns:
-                The next value that was received.
-
-            Raises:
-                ReceiverStoppedError: if there is some problem with the receiver.
-                ReceiverError: if there is some problem with the receiver.
-            """
-            try:
-                return self._receiver.consume()  # pylint: disable=protected-access
-            except ReceiverError as err:
-                # If this comes from a channel error, then we inject another
-                # ChannelError having the information about the Bidirectional
-                # channel to hide (at least partially) the underlying
-                # Broadcast channels we use.
-                if isinstance(err.__cause__, ChannelError):
-                    this_chan_error = ChannelError(
-                        f"Error in the underlying channel {err.__cause__.channel}: {err.__cause__}",
-                        self._chan,  # pylint: disable=protected-access
-                    )
-                    this_chan_error.__cause__ = err.__cause__
-                    err.__cause__ = this_chan_error
-                raise err
+This module contains the following:
 
-    def __init__(self, client_id: str, service_id: str) -> None:
-        """Create a `Bidirectional` instance.
+* [`Event`][frequenz.channels.event.Event]:
+    {{docstring_summary("frequenz.channels.event.Event")}}
+"""
+
+import asyncio as _asyncio
+
+from frequenz.channels import _receiver
+
+
+class Event(_receiver.Receiver[None]):
+    """A receiver that can be made ready directly.
+
+    # Usage
+
+    There are cases where it is useful to be able to send a signal to
+    a [`select()`][frequenz.channels.select] loop, for example, to stop a loop from
+    outside the loop itself.
+
+    To do that, you can use an [`Event`][frequenz.channels.event.Event] receiver and
+    call [`set()`][frequenz.channels.event.Event.set] on it when you want to make it
+    ready.
+
+    # Stopping
+
+    The receiver will be re-activated (will keep blocking) after the current set
+    event is received. To stop the receiver completely, you can call
+    [`stop()`][frequenz.channels.event.Event.stop].
+
+    # Example
+
+    Example: Exit after printing the first 5 numbers
+        ```python
+        import asyncio
+
+        from frequenz.channels import Anycast, select, selected_from
+        from frequenz.channels.event import Event
+
+        channel: Anycast[int] = Anycast(name="channel")
+        receiver = channel.new_receiver()
+        sender = channel.new_sender()
+        stop_event = Event(name="stop")
+
+
+        async def do_work() -> None:
+            async for selected in select(receiver, stop_event):
+                if selected_from(selected, receiver):
+                    print(selected.message)
+                elif selected_from(selected, stop_event):
+                    print("Stop event triggered")
+                    stop_event.stop()
+                    break
+
+
+        async def send_stuff() -> None:
+            for i in range(10):
+                if stop_event.is_stopped:
+                    break
+                await asyncio.sleep(1)
+                await sender.send(i)
+
+
+        async def main() -> None:
+            async with asyncio.TaskGroup() as task_group:
+                task_group.create_task(do_work(), name="do_work")
+                task_group.create_task(send_stuff(), name="send_stuff")
+                await asyncio.sleep(5.5)
+                stop_event.set()
+
+
+        asyncio.run(main())
+        ```
+    """
+
+    def __init__(self, *, name: str | None = None) -> None:
+        """Initialize this event.
 
         Args:
-            client_id: A name for the client, used to name the channels.
-            service_id: A name for the service end of the channels.
+            name: The name of the receiver.  If `None` an `id(self)`-based name will be
+                used. This is only for debugging purposes, it will be shown in the
+                string representation of the receiver.
         """
-        self._client_id = client_id
-        """The name for the client, used to name the channels."""
+        self._event: _asyncio.Event = _asyncio.Event()
+        """The event that is set when the receiver is ready."""
 
-        self._request_channel: Broadcast[T] = Broadcast(f"req_{service_id}_{client_id}")
-        """The channel to send requests."""
+        self._name: str = f"{id(self):_}" if name is None else name
+        """The name of the receiver.
 
-        self._response_channel: Broadcast[U] = Broadcast(
-            f"resp_{service_id}_{client_id}"
-        )
-        """The channel to send responses."""
+        This is for debugging purposes, it will be shown in the string representation
+        of the receiver.
+        """
 
-        self._client_handle = Bidirectional.Handle(
-            self,
-            self._request_channel.new_sender(),
-            self._response_channel.new_receiver(),
-        )
-        """The handle for the client side to send/receive values."""
+        self._is_set: bool = False
+        """Whether the receiver is ready to be consumed.
 
-        self._service_handle = Bidirectional.Handle(
-            self,
-            self._response_channel.new_sender(),
-            self._request_channel.new_receiver(),
-        )
-        """The handle for the service side to send/receive values."""
+        This is used to differentiate between when the receiver was stopped (the event
+        is triggered too) but still there is an event to be consumed and when it was
+        stopped but was not explicitly set().
+        """
+
+        self._is_stopped: bool = False
+        """Whether the receiver is stopped."""
 
     @property
-    def client_handle(self) -> Bidirectional.Handle[T, U]:
-        """Get a `Handle` for the client side to use.
+    def name(self) -> str:
+        """The name of this receiver.
 
-        Returns:
-            Object to send/receive messages with.
+        This is for debugging purposes, it will be shown in the string representation
+        of this receiver.
         """
-        return self._client_handle
+        return self._name
+
+    @property
+    def is_set(self) -> bool:
+        """Whether this receiver is set (ready)."""
+        return self._is_set
 
     @property
-    def service_handle(self) -> Bidirectional.Handle[U, T]:
-        """Get a `Handle` for the service side to use.
+    def is_stopped(self) -> bool:
+        """Whether this receiver is stopped."""
+        return self._is_stopped
+
+    def stop(self) -> None:
+        """Stop this receiver."""
+        self._is_stopped = True
+        self._event.set()
+
+    def set(self) -> None:
+        """Trigger the event (make the receiver ready)."""
+        self._is_set = True
+        self._event.set()
+
+    async def ready(self) -> bool:
+        """Wait until this receiver is ready.
 
         Returns:
-            Object to send/receive messages with.
+            Whether this receiver is still running.
+        """
+        if self._is_stopped:
+            return False
+        await self._event.wait()
+        return not self._is_stopped
+
+    def consume(self) -> None:
+        """Consume the event.
+
+        This makes this receiver wait again until the event is set again.
+
+        Raises:
+            ReceiverStoppedError: If this receiver is stopped.
         """
-        return self._service_handle
+        if not self._is_set and self._is_stopped:
+            raise _receiver.ReceiverStoppedError(self)
+
+        assert self._is_set, "calls to `consume()` must be follow a call to `ready()`"
+
+        self._is_set = False
+        self._event.clear()
+
+    def __str__(self) -> str:
+        """Return a string representation of this event."""
+        return f"{type(self).__name__}({self._name!r})"
+
+    def __repr__(self) -> str:
+        """Return a string representation of this event."""
+        return (
+            f"<{type(self).__name__} name={self._name!r} is_set={self.is_set!r} "
+            f"is_stopped={self.is_stopped!r}>"
+        )
```

### Comparing `frequenz-channels-1.0.0b2/src/frequenz/channels/util/_select.py` & `frequenz-channels-1.0.0rc1/src/frequenz/channels/_select.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,311 +1,408 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Select the first among multiple Receivers.
 
-Expects Receiver class to raise `StopAsyncIteration`
-exception once no more messages are expected or the channel
-is closed in case of `Receiver` class.
+# Usage
+
+If you need to receiver different types of messages from different receivers, you need
+to know the source of a particular received message to know the type of the message.
+
+[`select()`][frequenz.channels.select] allows you to do that. It is an
+[async iterator][typing.AsyncIterator] that will iterate over the messages of all
+receivers as they receive new messages.
+
+It yields a [`Selected`][frequenz.channels.Selected] object that will tell you the
+source of the received message. To make sure the received message is *cast* to the
+correct type, you need to use the [`selected_from()`][frequenz.channels.selected_from]
+function to check the source of the message, and the
+[`message`][frequenz.channels.Selected.message] attribute to access the message:
+
+```python show_lines="8:"
+from frequenz.channels import Anycast, ReceiverStoppedError, select, selected_from
+
+channel1: Anycast[int] = Anycast(name="channel1")
+channel2: Anycast[str] = Anycast(name="channel2")
+receiver1 = channel1.new_receiver()
+receiver2 = channel2.new_receiver()
+
+async for selected in select(receiver1, receiver2):
+    if selected_from(selected, receiver1):
+        print(f"Received from receiver1, next number: {selected.message + 1}")
+    elif selected_from(selected, receiver2):
+        print(f"Received from receiver2, length: {len(selected.message)}")
+    else:
+        assert False, "Unknown source, this should never happen"
+```
+
+Tip:
+    To prevent common bugs, like when a new receiver is added to the select loop but
+    the handling code is forgotten, [`select()`][frequenz.channels.select] will check
+    that all the selected receivers are handled in the if-chain.
+
+    If this happens, it will raise an
+    [`UnhandledSelectedError`][frequenz.channels.UnhandledSelectedError] exception.
+
+    If for some reason you want to ignore a received message, just add the receiver to
+    the if-chain and do nothing with the message:
+
+    ```python show_lines="8:"
+    from frequenz.channels import Anycast, select, selected_from
+
+    channel1: Anycast[int] = Anycast(name="channel1")
+    channel2: Anycast[str] = Anycast(name="channel2")
+    receiver1 = channel1.new_receiver()
+    receiver2 = channel2.new_receiver()
+
+    async for selected in select(receiver1, receiver2):
+        if selected_from(selected, receiver1):
+            continue
+        if selected_from(selected, receiver2):
+            print(f"Received from receiver2, length: {len(selected.message)}")
+    ```
+
+# Stopping
+
+The `select()` async iterator will stop as soon as all the receivers are stopped. You
+can also end the iteration early by breaking out of the loop as normal.
+
+When a single [receiver][frequenz.channels.Receiver] is stopped, it will be reported
+via the [`Selected`][frequenz.channels.Selected] object. You can use the
+[`was_stopped`][frequenz.channels.Selected.was_stopped] method to check if the
+selected [receiver][frequenz.channels.Receiver] was stopped:
+
+```python show_lines="8:"
+from frequenz.channels import Anycast, select, selected_from
+
+channel1: Anycast[int] = Anycast(name="channel1")
+channel2: Anycast[str] = Anycast(name="channel2")
+receiver1 = channel1.new_receiver()
+receiver2 = channel2.new_receiver()
+
+async for selected in select(receiver1, receiver2):
+    if selected_from(selected, receiver1):
+        if selected.was_stopped:
+            print("receiver1 was stopped")
+            continue
+        print(f"Received from receiver1, the next number is: {selected.message + 1}")
+    # ...
+```
+
+Tip:
+    The [`was_stopped`][frequenz.channels.Selected.was_stopped] method is a
+    convenience method that is equivalent to checking if the
+    [`exception`][frequenz.channels.Selected.exception] attribute is an instance of
+    [`ReceiverStoppedError`][frequenz.channels.ReceiverStoppedError].
+
+# Error Handling
+
+Tip:
+    For more information about handling errors, please refer to the
+    [Error Handling](/user-guide/error-handling/) section of the user guide.
+
+If a receiver raises an exception while receiving a message, the exception will be
+raised by the [`message`][frequenz.channels.Selected.message] attribute of the
+[`Selected`][frequenz.channels.Selected] object.
+
+You can use a try-except block to handle exceptions as usual:
+
+```python show_lines="8:"
+from frequenz.channels import Anycast, ReceiverStoppedError, select, selected_from
+
+channel1: Anycast[int] = Anycast(name="channel1")
+channel2: Anycast[str] = Anycast(name="channel2")
+receiver1 = channel1.new_receiver()
+receiver2 = channel2.new_receiver()
+
+async for selected in select(receiver1, receiver2):
+    if selected_from(selected, receiver1):
+        try:
+            print(f"Received from receiver1, next number: {selected.message + 1}")
+        except ReceiverStoppedError:
+            print("receiver1 was stopped")
+        except ValueError as value_error:
+            print(f"receiver1 raised a ValueError: {value_error}")
+        # ...
+    # ...
+```
+
+The [`Selected`][frequenz.channels.Selected] object also has a
+[`exception`][frequenz.channels.Selected.exception] attribute that will contain the
+exception that was raised by the receiver.
 """
 
 import asyncio
 from collections.abc import AsyncIterator
-from typing import Any, Generic, TypeGuard, TypeVar
+from typing import Any, Generic, TypeGuard
 
-from .._base_classes import Receiver
-from .._exceptions import ReceiverStoppedError
+from ._exceptions import Error
+from ._generic import ReceiverMessageT_co
+from ._receiver import Receiver, ReceiverStoppedError
 
-_T = TypeVar("_T")
 
+class _EmptyResult:
+    """A sentinel value to distinguish between None and empty result.
 
-class Selected(Generic[_T]):
-    """A result of a [`select()`][frequenz.channels.util.select] iteration.
+    We need a sentinel because a result can also be `None`.
+    """
 
-    The selected receiver is consumed immediately and the received value is stored in
-    the instance, unless there was an exception while receiving the value, in which case
-    the exception is stored instead.
+    def __repr__(self) -> str:
+        """Return a string with the internal representation of this instance."""
+        return "<empty>"
 
-    `Selected` instances should be used in conjunction with the
-    [`selected_from()`][frequenz.channels.util.selected_from] function to determine
-    which receiver was selected.
 
-    Please see [`select()`][frequenz.channels.util.select] for an example.
-    """
+class Selected(Generic[ReceiverMessageT_co]):
+    """A result of a [`select()`][frequenz.channels.select] iteration.
 
-    class _EmptyResult:
-        """A sentinel value to distinguish between None and empty result.
+    The selected receiver is consumed immediately and the received message is stored in
+    the instance, unless there was an exception while receiving the message, in which
+    case the exception is stored instead.
 
-        We need a sentinel because a result can also be `None`.
-        """
+    `Selected` instances should be used in conjunction with the
+    [`selected_from()`][frequenz.channels.selected_from] function to determine
+    which receiver was selected.
 
-        def __repr__(self) -> str:
-            return "<empty>"
+    Please see [`select()`][frequenz.channels.select] for an example.
+    """
 
-    def __init__(self, receiver: Receiver[_T]) -> None:
-        """Create a new instance.
+    def __init__(self, receiver: Receiver[ReceiverMessageT_co], /) -> None:
+        """Initialize this selected result.
 
         The receiver is consumed immediately when creating the instance and the received
-        value is stored in the instance for later use as
-        [`value`][frequenz.channels.util.Selected.value].  If there was an exception
-        while receiving the value, then the exception is stored in the instance instead
-        (as [`exception`][frequenz.channels.util.Selected.exception]).
+        message is stored in the instance for later use as
+        [`message`][frequenz.channels.Selected.message].  If there was an exception
+        while receiving the message, then the exception is stored in the instance
+        instead (as [`exception`][frequenz.channels.Selected.exception]).
 
         Args:
             receiver: The receiver that was selected.
         """
-        self._recv: Receiver[_T] = receiver
+        self._recv: Receiver[ReceiverMessageT_co] = receiver
         """The receiver that was selected."""
 
-        self._value: _T | Selected._EmptyResult = Selected._EmptyResult()
-        """The value that was received.
+        self._message: ReceiverMessageT_co | _EmptyResult = _EmptyResult()
+        """The message that was received.
 
-        If there was an exception while receiving the value, then this will be `None`.
+        If there was an exception while receiving the message, then this will be `None`.
         """
         self._exception: Exception | None = None
-        """The exception that was raised while receiving the value (if any)."""
+        """The exception that was raised while receiving the message (if any)."""
 
         try:
-            self._value = receiver.consume()
+            self._message = receiver.consume()
         except Exception as exc:  # pylint: disable=broad-except
             self._exception = exc
 
         self._handled: bool = False
         """Flag to indicate if this selected has been handled in the if-chain."""
 
     @property
-    def value(self) -> _T:
-        """The value that was received, if any.
+    def message(self) -> ReceiverMessageT_co:
+        """The message that was received, if any.
 
         Returns:
-            The value that was received.
+            The message that was received.
 
         Raises:
-            Exception: If there was an exception while receiving the value. Normally
+            Exception: If there was an exception while receiving the message. Normally
                 this should be an [`frequenz.channels.Error`][frequenz.channels.Error]
                 instance, but catches all exceptions in case some receivers can raise
                 anything else.
         """
         if self._exception is not None:
             raise self._exception
-        assert not isinstance(self._value, Selected._EmptyResult)
-        return self._value
+        assert not isinstance(self._message, _EmptyResult)
+        return self._message
 
     @property
     def exception(self) -> Exception | None:
-        """The exception that was raised while receiving the value (if any).
+        """The exception that was raised while receiving the message (if any).
 
         Returns:
-            The exception that was raised while receiving the value (if any).
+            The exception that was raised while receiving the message (if any).
         """
         return self._exception
 
+    @property
     def was_stopped(self) -> bool:
-        """Check if the selected receiver was stopped.
-
-        Check if the selected receiver raised
-        a [`ReceiverStoppedError`][frequenz.channels.ReceiverStoppedError] while
-        consuming a value.
-
-        Returns:
-            Whether the receiver was stopped.
-        """
+        """Whether the selected receiver was stopped while receiving a message."""
         return isinstance(self._exception, ReceiverStoppedError)
 
     def __str__(self) -> str:
-        """Return a string representation of this instance.
-
-        Returns:
-            A string representation of this instance.
-        """
+        """Return a string representation of this selected receiver."""
         return (
             f"{type(self).__name__}({self._recv}) -> "
-            f"{self._exception or self._value})"
+            f"{self._exception or self._message})"
         )
 
     def __repr__(self) -> str:
-        """Return a the internal representation of this instance.
-
-        Returns:
-            A string representation of this instance.
-        """
+        """Return a string with the internal representation of this instance."""
         return (
-            f"{type(self).__name__}({self._recv=}, {self._value=}, "
+            f"{type(self).__name__}({self._recv=}, {self._message=}, "
             f"{self._exception=}, {self._handled=})"
         )
 
 
 # It would have been nice to be able to make this a method of selected, but sadly
 # `TypeGuard`s can't be used as methods. For more information see:
 # https://github.com/microsoft/pyright/discussions/3125
 def selected_from(
-    selected: Selected[Any], receiver: Receiver[_T]
-) -> TypeGuard[Selected[_T]]:
-    """Check if the given receiver was selected by [`select()`][frequenz.channels.util.select].
+    selected: Selected[Any], receiver: Receiver[ReceiverMessageT_co]
+) -> TypeGuard[Selected[ReceiverMessageT_co]]:
+    """Check whether the given receiver was selected by [`select()`][frequenz.channels.select].
 
     This function is used in conjunction with the
-    [`Selected`][frequenz.channels.util.Selected] class to determine which receiver was
+    [`Selected`][frequenz.channels.Selected] class to determine which receiver was
     selected in `select()` iteration.
 
     It also works as a [type guard][typing.TypeGuard] to narrow the type of the
     `Selected` instance to the type of the receiver.
 
-    Please see [`select()`][frequenz.channels.util.select] for an example.
+    Please see [`select()`][frequenz.channels.select] for an example.
 
     Args:
         selected: The result of a `select()` iteration.
         receiver: The receiver to check if it was the source of a select operation.
 
     Returns:
         Whether the given receiver was selected.
     """
     if handled := selected._recv is receiver:  # pylint: disable=protected-access
         selected._handled = True  # pylint: disable=protected-access
     return handled
 
 
-class SelectError(BaseException):
-    """A base exception for [`select()`][frequenz.channels.util.select].
+class SelectError(Error):
+    """An error that happened during a [`select()`][frequenz.channels.select] operation.
 
     This exception is raised when a `select()` iteration fails.  It is raised as
     a single exception when one receiver fails during normal operation (while calling
     `ready()` for example).  It is raised as a group exception
-    ([`SelectErrorGroup`][frequenz.channels.util.SelectErrorGroup]) when a `select` loop
-    is cleaning up after it's done.
+    ([`BaseExceptionGroup`][]) when a `select` loop is cleaning up after it's done.
     """
 
 
-class UnhandledSelectedError(SelectError, Generic[_T]):
-    """A receiver was not handled in a [`select()`][frequenz.channels.util.select] loop.
+class UnhandledSelectedError(SelectError, Generic[ReceiverMessageT_co]):
+    """A receiver was not handled in a [`select()`][frequenz.channels.select] iteration.
 
-    This exception is raised when a `select()` iteration finishes without a call to
-    [`selected_from()`][frequenz.channels.util.selected_from] for the selected receiver.
+    This exception is raised when a [`select()`][frequenz.channels.select] iteration
+    finishes without a call to [`selected_from()`][frequenz.channels.selected_from] for
+    the selected receiver.
     """
 
-    def __init__(self, selected: Selected[_T]) -> None:
-        """Create a new instance.
+    def __init__(self, selected: Selected[ReceiverMessageT_co]) -> None:
+        """Initialize this error.
 
         Args:
             selected: The selected receiver that was not handled.
         """
         recv = selected._recv  # pylint: disable=protected-access
         super().__init__(f"Selected receiver {recv} was not handled in the if-chain")
-        self.selected = selected
+        self.selected: Selected[ReceiverMessageT_co] = selected
         """The selected receiver that was not handled."""
 
 
-class SelectErrorGroup(BaseExceptionGroup[BaseException], SelectError):
-    """An exception group for [`select()`][frequenz.channels.util.select] operation.
-
-    This exception group is raised when a `select()` loops fails while cleaning up
-    running tests to check for ready receivers.
-    """
-
-
 # Typing for select() is tricky.  We had the idea of using a declarative design for
 # select, something like:
 #
 # ```python
 # class MySelector(Selector):
 #     receiver1: x.new_receiver()
 #     receiver2: y.new_receiver()
 #
 # async for selected in MySelector:
 #     if selected.receiver is receiver1:
-#         # Do something with selected.value
+#         # Do something with selected.message
 #     elif selected.receiver is receiver1:
-#         # Do something with selected.value
+#         # Do something with selected.message
 # ```
 #
 # This is similar to `Enum`, but `Enum` has special support in `mypy` that we can't
 # have.
 #
 # With the current implementation, the typing could be slightly improved by using
 # `TypeVarTuple`, but we are not because "transformations" are not supported yet, see:
 # https://github.com/python/typing/issues/1216
 #
 # Also support for `TypeVarTuple` in general is still experimental (and very incomplete
 # in `mypy`).
 #
 # With this we would also probably be able to properly type `select` and *maybe* even be
-# able to leverage the exhaustiveness checking of `mypy` to make sure the selected value
-# is narrowed down to the correct type to make sure all receivers are handled, with the
-# help of `assert_never` as described in:
+# able to leverage the exhaustiveness checking of `mypy` to make sure the selected
+# message is narrowed down to the correct type to make sure all receivers are handled,
+# with the help of `assert_never` as described in:
 # https://docs.python.org/3.11/library/typing.html#typing.assert_never
 #
 # We also explored the possibility of using `match` to perform exhaustiveness checking,
 # but we couldn't find a way to make it work with `match`, and `match` is not yet
 # checked for exhaustiveness by `mypy` anyway, see:
 # https://github.com/python/mypy/issues/13597
 
 
 async def select(*receivers: Receiver[Any]) -> AsyncIterator[Selected[Any]]:
-    """Iterate over the values of all receivers as they receive new values.
+    """Iterate over the messages of all receivers as they receive new messages.
 
-    This function is used to iterate over the values of all receivers as they receive
-    new values.  It is used in conjunction with the
-    [`Selected`][frequenz.channels.util.Selected] class and the
-    [`selected_from()`][frequenz.channels.util.selected_from] function to determine
+    This function is used to iterate over the messages of all receivers as they receive
+    new messages.  It is used in conjunction with the
+    [`Selected`][frequenz.channels.Selected] class and the
+    [`selected_from()`][frequenz.channels.selected_from] function to determine
     which function to determine which receiver was selected in a select operation.
 
     An exhaustiveness check is performed at runtime to make sure all selected receivers
     are handled in the if-chain, so you should call `selected_from()` with all the
     receivers passed to `select()` inside the select loop, even if you plan to ignore
-    a value, to signal `select()` that you are purposefully ignoring the value.
+    a message, to signal `select()` that you are purposefully ignoring the message.
 
     Note:
         The `select()` function is intended to be used in cases where the set of
         receivers is static and known beforehand.  If you need to dynamically add/remove
         receivers from a select loop, there are a few alternatives.  Depending on your
         use case, one or the other could work better for you:
 
-        * Use [`Merge`][frequenz.channels.util.Merge] or
-          [`MergeNamed`][frequenz.channels.util.MergeNamed]: this is useful when you
-          have and unknown number of receivers of the same type that can be handled as
-          a group.
+        * Use [`merge()`][frequenz.channels.merge]: this is useful when you have an
+          unknown number of receivers of the same type that can be handled as a group.
         * Use tasks to manage each receiver individually: this is better if there are no
           relationships between the receivers.
         * Break the `select()` loop and start a new one with the new set of receivers
           (this should be the last resort, as it has some performance implications
            because the loop needs to be restarted).
 
     Example:
         ```python
         import datetime
         from typing import assert_never
 
-        from frequenz.channels import ReceiverStoppedError
-        from frequenz.channels.util import select, selected_from, Timer
+        from frequenz.channels import ReceiverStoppedError, select, selected_from
+        from frequenz.channels.timer import SkipMissedAndDrift, Timer, TriggerAllMissed
 
-        timer1 = Timer.periodic(datetime.timedelta(seconds=1))
-        timer2 = Timer.timeout(datetime.timedelta(seconds=0.5))
+        timer1 = Timer(datetime.timedelta(seconds=1), TriggerAllMissed())
+        timer2 = Timer(datetime.timedelta(seconds=0.5), SkipMissedAndDrift())
 
         async for selected in select(timer1, timer2):
             if selected_from(selected, timer1):
-                # Beware: `selected.value` might raise an exception, you can always
+                # Beware: `selected.message` might raise an exception, you can always
                 # check for exceptions with `selected.exception` first or use
                 # a try-except block. You can also quickly check if the receiver was
                 # stopped and let any other unexpected exceptions bubble up.
                 if selected.was_stopped:
                     print("timer1 was stopped")
                     continue
-                print(f"timer1: now={datetime.datetime.now()} drift={selected.value}")
+                print(f"timer1: now={datetime.datetime.now()} drift={selected.message}")
                 timer2.stop()
             elif selected_from(selected, timer2):
                 # Explicitly handling of exceptions
                 match selected.exception:
                     case ReceiverStoppedError():
                         print("timer2 was stopped")
                     case Exception() as exception:
                         print(f"timer2: exception={exception}")
                     case None:
-                        # All good, no exception, we can use `selected.value` safely
-                        print(
-                            f"timer2: now={datetime.datetime.now()} drift={selected.value}"
-                        )
+                        # All good, no exception, we can use `selected.message` safely
+                        print(f"timer2: now={datetime.datetime.now()} drift={selected.message}")
                     case _ as unhanded:
                         assert_never(unhanded)
             else:
                 # This is not necessary, as select() will check for exhaustiveness, but
                 # it is good practice to have it in case you forgot to handle a new
                 # receiver added to `select()` at a later point in time.
                 assert False
@@ -315,19 +412,19 @@
         *receivers: The receivers to select from.
 
     Yields:
         The currently selected item.
 
     Raises:
         UnhandledSelectedError: If a selected receiver was not handled in the if-chain.
-        SelectErrorGroup: If there is an error while finishing the select operation and
-            receivers fail while cleaning up.
+        BaseExceptionGroup: If there is an error while finishing the select operation
+            and receivers fail while cleaning up.
         SelectError: If there is an error while selecting receivers during normal
             operation.  For example if a receiver raises an exception in the `ready()`
-            method.  Normal errors while receiving values are not raised, but reported
+            method.  Normal errors while receiving messages are not raised, but reported
             via the `Selected` instance.
     """
     receivers_map: dict[str, Receiver[Any]] = {str(hash(r)): r for r in receivers}
     pending: set[asyncio.Task[bool]] = set()
 
     try:
         for name, recv in receivers_map.items():
@@ -372,15 +469,15 @@
 async def _stop_pending_tasks(pending: set[asyncio.Task[bool]]) -> None:
     """Stop all pending tasks.
 
     Args:
         pending: The pending tasks to stop.
 
     Raises:
-        SelectErrorGroup: If the receivers raise any exceptions.
+        BaseExceptionGroup: If the receivers raise any exceptions.
     """
     if pending:
         for task in pending:
             task.cancel()
         done, pending = await asyncio.wait(pending)
         assert not pending
         exceptions: list[BaseException] = []
@@ -391,8 +488,10 @@
                 exceptions.append(exception)
         if exceptions:
             # If the select loop is interrupted by a break or exception, then this
             # exception will be actually swallowed, as the select() async generator
             # will be collected by the asyncio loop. This shouldn't be too bad as
             # errors produced by receivers will be re-raised when trying to use them
             # again.
-            raise SelectErrorGroup("Some receivers failed when select()ing", exceptions)
+            raise BaseExceptionGroup(
+                "Some receivers failed when select()ing", exceptions
+            )
```

### Comparing `frequenz-channels-1.0.0b2/src/frequenz/channels/util/_timer.py` & `frequenz-channels-1.0.0rc1/src/frequenz/channels/timer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,112 @@
 # License: MIT
 # Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
-"""A timer receiver that ticks every `interval`.
+"""A receiver that sends a message regularly.
 
-Note:
-    This module always use `int`s to represent time.  The time is always in
-    microseconds, so the timer resolution is 1 microsecond.
+# Quick Start
 
-    This is to avoid floating point errors when performing calculations with
-    time, which can lead to very hard to reproduce, and debug, issues.
+Info: Important
+    This quick start is provided to have a quick feeling of how to use this module, but
+    it is extremely important to understand how timers behave when they are delayed.
+
+    We recommend emphatically to read about [missed ticks and
+    drifting](#missed-ticks-and-drifting) before using timers in production.
+
+If you need to do something as periodically as possible (avoiding
+[drifts](#missed-ticks-and-drifting)), you can use
+a [`Timer`][frequenz.channels.timer.Timer] like this:
+
+Example: Periodic Timer Example
+    ```python
+    import asyncio
+    from datetime import datetime, timedelta
+
+    from frequenz.channels.timer import Timer
+
+
+    async def main() -> None:
+        async for drift in Timer(timedelta(seconds=1.0), TriggerAllMissed()):
+            print(f"The timer has triggered at {datetime.now()} with a drift of {drift}")
+
+
+    asyncio.run(main())
+    ```
+
+    This timer will tick as close as every second as possible, even if the loop is busy
+    doing something else for a good amount of time. In extreme cases, if the loop was
+    busy for a few seconds, the timer will trigger a few times in a row to catch up, one
+    for every missed tick.
+
+If, instead, you need a timeout, for example to abort waiting for other receivers after
+a certain amount of time, you can use a [`Timer`][frequenz.channels.timer.Timer] like
+this:
+
+Example: Timeout Example
+    ```python
+    import asyncio
+    from datetime import timedelta
+
+    from frequenz.channels import Anycast, select, selected_from
+    from frequenz.channels.timer import Timer
+
+
+    async def main() -> None:
+        channel = Anycast[int](name="data-channel")
+        data_receiver = channel.new_receiver()
+
+        timer = Timer(timedelta(seconds=1.0), SkipMissedAndDrift())
+
+        async for selected in select(data_receiver, timer):
+            if selected_from(selected, data_receiver):
+                print(f"Received data: {selected.message}")
+                timer.reset()
+            elif selected_from(selected, timer):
+                drift = selected.message
+                print(f"No data received for {timer.interval + drift} seconds, giving up")
+                break
+
+
+    asyncio.run(main())
+    ```
+
+    This timer will *rearm* itself automatically after it was triggered, so it will
+    trigger again after the selected interval, no matter what the current drift was. So
+    if the loop was busy for a few seconds, the timer will trigger immediately and then
+    wait for another second before triggering again. The missed ticks are skipped.
+
+# Missed Ticks And Drifting
+
+A [`Timer`][frequenz.channels.timer.Timer] can be used to send a messages at regular
+time intervals, but there is one fundamental issue with timers in the [asyncio][] world:
+the event loop could give control to another task at any time, and that task can take
+a long time to finish, making the time it takes the next timer message to be received
+longer than the desired interval.
+
+Because of this, it is very important for users to be able to understand and control
+how timers behave when they are delayed. Timers will handle missed ticks according to
+a *missing tick policy*.
+
+The following built-in policies are available:
+
+* [`SkipMissedAndDrift`][frequenz.channels.timer.SkipMissedAndDrift]:
+    {{docstring_summary("frequenz.channels.timer.SkipMissedAndDrift")}}
+* [`SkipMissedAndResync`][frequenz.channels.timer.SkipMissedAndResync]:
+    {{docstring_summary("frequenz.channels.timer.SkipMissedAndResync")}}
+* [`TriggerAllMissed`][frequenz.channels.timer.TriggerAllMissed]:
+    {{docstring_summary("frequenz.channels.timer.TriggerAllMissed")}}
 """
 
 from __future__ import annotations
 
 import abc
 import asyncio
 from datetime import timedelta
 
-from .._base_classes import Receiver
-from .._exceptions import ReceiverStoppedError
+from ._receiver import Receiver, ReceiverStoppedError
 
 
 def _to_microseconds(time: float | timedelta) -> int:
     """Convert a time or a timedelta to microseconds.
 
     Args:
         time: The time to convert. If it is a `float`, it is assumed to be in
@@ -35,17 +119,42 @@
         time = time.total_seconds()
     return round(time * 1_000_000)
 
 
 class MissedTickPolicy(abc.ABC):
     """A policy to handle timer missed ticks.
 
-    This is only relevant if the timer is not ready to trigger when it should
-    (an interval passed) which can happen if the event loop is busy processing
-    other tasks.
+    To implement a custom policy you need to subclass
+    [`MissedTickPolicy`][frequenz.channels.timer.MissedTickPolicy] and implement the
+    [`calculate_next_tick_time`][frequenz.channels.timer.MissedTickPolicy.calculate_next_tick_time]
+    method.
+
+    Example:
+        This policy will just wait one more second than the original interval if a
+        tick is missed:
+
+        ```python
+        class WaitOneMoreSecond(MissedTickPolicy):
+            def calculate_next_tick_time(
+                self, *, interval: int, scheduled_tick_time: int, now: int
+            ) -> int:
+                return scheduled_tick_time + interval + 1_000_000
+
+
+        async def main() -> None:
+            timer = Timer(
+                interval=timedelta(seconds=1),
+                missed_tick_policy=WaitOneMoreSecond(),
+            )
+
+            async for drift in timer:
+                print(f"The timer has triggered with a drift of {drift}")
+
+        asyncio.run(main())
+        ```
     """
 
     @abc.abstractmethod
     def calculate_next_tick_time(
         self, *, interval: int, scheduled_tick_time: int, now: int
     ) -> int:
         """Calculate the next tick time according to `missed_tick_policy`.
@@ -60,45 +169,64 @@
                 trigger (in microseconds).
             now: The current loop time (in microseconds).
 
         Returns:
             The next tick time (in microseconds) according to
                 `missed_tick_policy`.
         """
-        return 0  # dummy value to avoid darglint warnings
 
     def __repr__(self) -> str:
-        """Return a string representation of the instance.
-
-        Returns:
-            The string representation of the instance.
-        """
+        """Return a string representation of this policy."""
         return f"{type(self).__name__}()"
 
 
 class TriggerAllMissed(MissedTickPolicy):
     """A policy that triggers all the missed ticks immediately until it catches up.
 
+    The [`TriggerAllMissed`][frequenz.channels.timer.TriggerAllMissed] policy will
+    trigger all missed ticks immediately until it catches up with the current time.
+    This means that if the timer is delayed for any reason, when it finally gets some
+    time to run, it will trigger all the missed ticks in a burst. The drift is not
+    accumulated and the next tick will be scheduled according to the original start
+    time.
+
     Example:
-        Assume a timer with interval 1 second, the tick `T0` happens exactly
-        at time 0, the second tick, `T1`, happens at time 1.2 (0.2 seconds
-        late), so it triggers immediately.  The third tick, `T2`, happens at
-        time 2.3 (0.3 seconds late), so it also triggers immediately.  The
-        fourth tick, `T3`, happens at time 4.3 (1.3 seconds late), so it also
-        triggers immediately as well as the fifth tick, `T4`, which was also
-        already delayed (by 0.3 seconds), so it catches up.  The sixth tick,
-        `T5`, happens at 5.1 (0.1 seconds late), so it triggers immediately
-        again. The seventh tick, `T6`, happens at 6.0, right on time.
+        This example represents a timer with interval 1 second.
 
-        ```
-        0         1         2         3         4  o      5         6
-        o---------|-o-------|--o------|---------|--o------|o--------o-----> time
+        1. The first tick, `T0` happens exactly at time 0.
+
+        2. The second tick, `T1`, happens at time 1.2 (0.2 seconds late), so it triggers
+            immediately. But it re-syncs, so the next tick is still expected at
+            2 seconds. This re-sync happens on every tick, so all ticks are expected at
+            multiples of 1 second, not matter how delayed they were.
+
+        3. The third tick, `T2`, happens at time 2.3 (0.3 seconds late), so it also
+            triggers immediately.
+
+        4. The fourth tick, `T3`, happens at time 4.3 (1.3 seconds late), so it also
+            triggers immediately.
+
+        5. The fifth tick, `T4`, which was also already delayed (by 0.3 seconds),
+            triggers immediately too, resulting in a small *catch-up* burst.
+
+        6. The sixth tick, `T5`, happens at 5.1 (0.1 seconds late), so it triggers
+            immediately again.
+
+        7. The seventh tick, `T6`, happens at 6.0, right on time.
+
+        <center>
+        ```bob
+        0         1         2         3         4   T4    5         6
+        *---------o-*-------o--*------o---------o--**-----o*--------*-----> time
         T0          T1         T2                  T3      T5       T6
-                                                   T4
+
+        -o- "Expected ticks"
+        -*- "Delivered ticks"
         ```
+        </center>
     """
 
     def calculate_next_tick_time(
         self, *, now: int, scheduled_tick_time: int, interval: int
     ) -> int:
         """Calculate the next tick time.
 
@@ -116,35 +244,54 @@
         """
         return scheduled_tick_time + interval
 
 
 class SkipMissedAndResync(MissedTickPolicy):
     """A policy that drops all the missed ticks, triggers immediately and resyncs.
 
-    If ticks are missed, the timer will trigger immediately returning the drift
-    and it will schedule to trigger again on the next multiple of `interval`,
-    effectively skipping any missed ticks, but resyncing with the original start
-    time.
+    If ticks are missed, the
+    [`SkipMissedAndResync`][frequenz.channels.timer.SkipMissedAndResync] policy will
+    make the [`Timer`][frequenz.channels.timer.Timer] trigger immediately and it will
+    schedule to trigger again on the next multiple of the
+    [interval][frequenz.channels.timer.Timer.interval], effectively skipping any missed
+    ticks, but re-syncing with the original start time.
 
     Example:
-        Assume a timer with interval 1 second, the tick `T0` happens exactly
-        at time 0, the second tick, `T1`, happens at time 1.2 (0.2 seconds
-        late), so it triggers immediately.  The third tick, `T2`, happens at
-        time 2.3 (0.3 seconds late), so it also triggers immediately.  The
-        fourth tick, `T3`, happens at time 4.3 (1.3 seconds late), so it also
-        triggers immediately but the fifth tick, `T4`, which was also
-        already delayed (by 0.3 seconds) is skipped.  The sixth tick,
-        `T5`, happens at 5.1 (0.1 seconds late), so it triggers immediately
-        again. The seventh tick, `T6`, happens at 6.0, right on time.
+        This example represents a timer with interval 1 second.
 
+        1. The first tick `T0` happens exactly at time 0.
+
+        2. The second tick, `T1`, happens at time 1.2 (0.2 seconds late), so it triggers
+            immediately. But it re-syncs, so the next tick is still expected at
+            2 seconds. This re-sync happens on every tick, so all ticks are expected at
+            multiples of 1 second, not matter how delayed they were.
+
+        3. The third tick, `T2`, happens at time 2.3 (0.3 seconds late), so it also
+            triggers immediately.
+
+        4. The fourth tick, `T3`, happens at time 4.3 (1.3 seconds late), so it also
+            triggers immediately, but there was also a tick expected at 4 seconds, `T4`,
+            which is skipped according to this policy to avoid bursts of ticks.
+
+        6. The sixth tick, `T5`, happens at 5.1 (0.1 seconds late), so it triggers
+            immediately again.
+
+        7. The seventh tick, `T6`, happens at 6.0, right on time.
+
+        <center>
+        ```bob
+        0         1         2         3         4   T4    5         6
+        *---------o-*-------o--*------o---------o--*O-----o-*-------*-----> time
+        T0          T1         T2                  T3       T5      T6
+
+        -o- "Expected ticks"
+        -*- "Delivered ticks"
+        -O- "Undelivered ticks (skipped)"
         ```
-        0         1         2         3         4  o      5         6
-        o---------|-o-------|--o------|---------|--o------|o--------o-----> time
-        T0          T1         T2                  T3      T5       T6
-        ```
+        </center>
     """
 
     def calculate_next_tick_time(
         self, *, now: int, scheduled_tick_time: int, interval: int
     ) -> int:
         """Calculate the next tick time.
 
@@ -164,45 +311,60 @@
         delta_to_next_tick = interval - (drift % interval)
         return now + delta_to_next_tick
 
 
 class SkipMissedAndDrift(MissedTickPolicy):
     """A policy that drops all the missed ticks, triggers immediately and resets.
 
-    This will behave effectively as if the timer was `reset()` at the time it
-    had triggered last, so the start time will change (and the drift will be
-    accumulated each time a tick is delayed, but only the relative drift will
-    be returned on each tick).
-
-    The reset happens only if the delay is larger than `delay_tolerance`, so
-    it is possible to ignore small delays and not drift in those cases.
+    The [`SkipMissedAndDrift`][frequenz.channels.timer.SkipMissedAndDrift] policy will
+    behave effectively as if the timer was
+    [reset][frequenz.channels.timer.Timer.reset] every time it is triggered. This means
+    the start time will change and the drift will be accumulated each time a tick is
+    delayed. Only the relative drift will be returned on each tick.
+
+    The reset happens only if the delay is larger than the
+    [delay tolerance][frequenz.channels.timer.SkipMissedAndDrift.delay_tolerance], so it
+    is possible to ignore small delays and not drift in those cases.
 
     Example:
-        Assume a timer with interval 1 second and `delay_tolerance=0.1`, the
-        first tick, `T0`, happens exactly at time 0, the second tick, `T1`,
-        happens at time 1.2 (0.2 seconds late), so the timer triggers
-        immediately but drifts a bit. The next tick, `T2.2`, happens at 2.3 seconds
-        (0.1 seconds late), so it also triggers immediately but it doesn't
-        drift because the delay is under the `delay_tolerance`. The next tick,
-        `T3.2`, triggers at 4.3 seconds (1.1 seconds late), so it also triggers
-        immediately but the timer drifts by 1.1 seconds and the tick `T4.2` is
-        skipped (not triggered). The next tick, `T5.3`, triggers at 5.3 seconds
-        so is right on time (no drift) and the same happens for tick `T6.3`,
-        which triggers at 6.3 seconds.
+        This example represents a timer with interval 1 second and delay tolerance of
+        0.1 seconds.
 
-        ```
+        1. The first tick, `T0`, happens exactly at time 0.
+
+        2. The second tick, `T1.2`, happens at time 1.2 (0.2 seconds late), so the timer
+            triggers immediately but drifts a bit (0.2 seconds), so the next tick is
+            expected at 2.2 seconds.
+
+        3. The third tick, `T2.2`, happens at 2.3 seconds (0.1 seconds late), so it also
+            triggers immediately but **it doesn't drift** because the delay is **under
+            the `delay_tolerance`**. The next tick is expected at 3.2 seconds.
+
+        4. The fourth tick, `T4.2`, triggers at 4.3 seconds (1.1 seconds late), so it
+            also triggers immediately but the timer has drifted by 1.1 seconds, so a
+            potential tick `T3.2` is skipped (not triggered).
+
+        5. The fifth tick, `T5.3`, triggers at 5.3 seconds so it is right on time (no
+            drift) and the same happens for tick `T6.3`, which triggers at 6.3 seconds.
+
+        <center>
+        ```bob
         0         1         2         3         4         5         6
-        o---------|-o-------|--o------|---------|--o------|--o------|--o--> time
-        T0          T1         T2.2                T3.2      T5.3      T6.3
+        *---------o-*-------|-o*------|-O-------|-o*------|--*------|--*--> time
+        T0          T1.2       T2.2     T3.2       T4.2      T5.3      T6.3
+
+        -o- "Expected ticks"
+        -*- "Delivered ticks"
+        -O- "Undelivered ticks (skipped)"
         ```
+        </center>
     """
 
     def __init__(self, *, delay_tolerance: timedelta = timedelta(0)):
-        """
-        Create an instance.
+        """Initialize this policy.
 
         See the class documentation for more details.
 
         Args:
             delay_tolerance: The maximum delay that is tolerated before
                 starting to drift.  If a tick is delayed less than this, then
                 it is not considered a missed tick and the timer doesn't
@@ -215,19 +377,15 @@
         """The maximum allowed delay before starting to drift."""
 
         if self._tolerance < 0:
             raise ValueError("delay_tolerance must be positive")
 
     @property
     def delay_tolerance(self) -> timedelta:
-        """Return the maximum delay that is tolerated before starting to drift.
-
-        Returns:
-            The maximum delay that is tolerated before starting to drift.
-        """
+        """The maximum delay that is tolerated before starting to drift."""
         return timedelta(microseconds=self._tolerance)
 
     def calculate_next_tick_time(
         self, *, now: int, scheduled_tick_time: int, interval: int
     ) -> int:
         """Calculate the next tick time.
 
@@ -247,160 +405,84 @@
         """
         drift = now - scheduled_tick_time
         if drift > self._tolerance:
             return now + interval
         return scheduled_tick_time + interval
 
     def __str__(self) -> str:
-        """Return a string representation of the instance.
-
-        Returns:
-            The string representation of the instance.
-        """
-        return f"{type(self).__name__}({self.delay_tolerance})"
+        """Return a string representation of this policy."""
+        return f"{type(self).__name__}()"
 
     def __repr__(self) -> str:
-        """Return a string representation of the instance.
-
-        Returns:
-            The string representation of the instance.
-        """
+        """Return a string representation of this policy."""
         return f"{type(self).__name__}({self.delay_tolerance=})"
 
 
 class Timer(Receiver[timedelta]):
-    """A timer receiver that triggers every `interval` time.
+    """A receiver that sends a message regularly.
 
-    The timer has microseconds resolution, so the
-    [`interval`][frequenz.channels.util.Timer.interval] must be at least
-    1 microsecond.
-
-    The message it produces is a [`timedelta`][datetime.timedelta] containing the drift
-    of the timer, i.e. the difference between when the timer should have triggered and
-    the time when it actually triggered.
+    [`Timer`][frequenz.channels.timer.Timer]s are started by default after they are
+    created. This can be disabled by using `auto_start=False` option when creating
+    them. In this case, the timer will not be started until
+    [`reset()`][frequenz.channels.timer.Timer.reset] is called. Receiving from the timer
+    (either using [`receive()`][frequenz.channels.timer.Timer.receive] or using the
+    async iterator interface) will also start the timer at that point.
+
+    Timers need to be created in a context where
+    a [`asyncio`][] loop is already running. If no
+    [`loop`][frequenz.channels.timer.Timer.loop] is specified, the current running loop
+    is used.
+
+    Timers can be stopped by calling [`stop()`][frequenz.channels.timer.Timer.stop].
+    A stopped timer will raise
+    a [`ReceiverStoppedError`][frequenz.channels.ReceiverStoppedError] or stop the async
+    iteration as usual.
+
+    Once a timer is explicitly stopped, it can only be started again by explicitly
+    calling [`reset()`][frequenz.channels.timer.Timer.reset] (trying to receive from it
+    or using the async iterator interface will keep failing).
+
+    Timer messages are [`timedelta`][datetime.timedelta]s containing the drift of the
+    timer, i.e. the difference between when the timer should have triggered and the time
+    when it actually triggered.
 
     This drift will likely never be `0`, because if there is a task that is
     running when it should trigger, the timer will be delayed. In this case the
     drift will be positive. A negative drift should be technically impossible,
-    as the timer uses [`asyncio`][asyncio]s loop monotonic clock.
+    as the timer uses [`asyncio`][]s loop monotonic clock.
+
+    Warning:
+        Even when the [`asyncio`][] loop's monotonic clock is a [`float`][], timers use
+        `int`s to represent time internally. The internal time is tracked in
+        microseconds, so the timer resolution is 1 microsecond
+        ([`interval`][frequenz.channels.timer.Timer.interval] must be at least
+         1 microsecond).
+
+        This is to avoid floating point errors when performing calculations with time,
+        which can lead to issues that are very hard to reproduce and debug.
 
     If the timer is delayed too much, then it will behave according to the
-    [`missed_tick_policy`][frequenz.channels.util.Timer.missed_tick_policy]. Missing
+    [`missed_tick_policy`][frequenz.channels.timer.Timer.missed_tick_policy]. Missing
     ticks might or might not trigger a message and the drift could be accumulated or not
     depending on the chosen policy.
-
-    These are the currently built-in available policies:
-
-    * [`SkipMissedAndDrift`][frequenz.channels.util.SkipMissedAndDrift]
-    * [`SkipMissedAndResync`][frequenz.channels.util.SkipMissedAndResync]
-    * [`TriggerAllMissed`][frequenz.channels.util.TriggerAllMissed]
-
-    For the most common cases, a specialized constructor is provided:
-
-    * [`periodic()`][frequenz.channels.util.Timer.periodic] (uses the
-      [`TriggerAllMissed`][frequenz.channels.util.TriggerAllMissed] or
-      [`SkipMissedAndResync`][frequenz.channels.util.SkipMissedAndResync] policy)
-    * [`timeout()`][frequenz.channels.util.Timer.timeout] (uses the
-      [`SkipMissedAndDrift`][frequenz.channels.util.SkipMissedAndDrift] policy)
-
-    The timer accepts an optional [`loop`][frequenz.channels.util.Timer.loop], which
-    will be used to track the time. If `loop` is `None`, then the running loop will be
-    used (if there is no running loop most calls will raise
-    a [`RuntimeError`][RuntimeError]).
-
-    Starting the timer can be delayed if necessary by using `auto_start=False`
-    (for example until we have a running loop). A call to
-    [`reset()`][frequenz.channels.util.Timer.reset],
-    [`ready()`][frequenz.channels.util.Timer.ready],
-    [`receive()`][frequenz.channels.util.Timer.receive] or the async iterator interface
-    to await for a new message will start the timer.
-
-    Example: Periodic timer example
-        ```python
-        async for drift in Timer.periodic(timedelta(seconds=1.0)):
-            print(f"The timer has triggered {drift=}")
-        ```
-
-        But you can also use a [`select`][frequenz.channels.util.select] to combine
-        it with other receivers, and even start it (semi) manually:
-
-        ```python
-        import logging
-        from frequenz.channels.util import select, selected_from
-        from frequenz.channels import Broadcast
-
-        timer = Timer.timeout(timedelta(seconds=1.0), auto_start=False)
-        chan = Broadcast[int]("input-chan")
-        battery_data = chan.new_receiver()
-
-        timer = Timer.timeout(timedelta(seconds=1.0), auto_start=False)
-        # Do some other initialization, the timer will start automatically if
-        # a message is awaited (or manually via `reset()`).
-        async for selected in select(battery_data, timer):
-            if selected_from(selected, battery_data):
-                if selected.was_closed():
-                    logging.warning("battery channel closed")
-                    continue
-                battery_soc = selected.value
-            elif selected_from(selected, timer):
-                # Print some regular battery data
-                print(f"Battery is charged at {battery_soc}%")
-        ```
-
-    Example: Timeout example
-        ```python
-        import logging
-        from frequenz.channels.util import select, selected_from
-        from frequenz.channels import Broadcast
-
-        def process_data(data: int):
-            logging.info("Processing data: %d", data)
-
-        def do_heavy_processing(data: int):
-            logging.info("Heavy processing data: %d", data)
-
-        timer = Timer.timeout(timedelta(seconds=1.0), auto_start=False)
-        chan1 = Broadcast[int]("input-chan-1")
-        chan2 = Broadcast[int]("input-chan-2")
-        battery_data = chan1.new_receiver()
-        heavy_process = chan2.new_receiver()
-        async for selected in select(battery_data, heavy_process, timer):
-            if selected_from(selected, battery_data):
-                if selected.was_closed():
-                    logging.warning("battery channel closed")
-                    continue
-                process_data(selected.value)
-                timer.reset()
-            elif selected_from(selected, heavy_process):
-                if selected.was_closed():
-                    logging.warning("processing channel closed")
-                    continue
-                do_heavy_processing(selected.value)
-            elif selected_from(selected, timer):
-                logging.warning("No data received in time")
-        ```
-
-        In this case `do_heavy_processing` might take 2 seconds, and we don't
-        want our timeout timer to trigger for the missed ticks, and want the
-        next tick to be relative to the time timer was last triggered.
     """
 
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         interval: timedelta,
         missed_tick_policy: MissedTickPolicy,
         /,
         *,
         auto_start: bool = True,
         start_delay: timedelta = timedelta(0),
         loop: asyncio.AbstractEventLoop | None = None,
     ) -> None:
-        """Create an instance.
+        """Initialize this timer.
 
-        See the class documentation for details.
+        See the [class documentation][frequenz.channels.timer.Timer] for details.
 
         Args:
             interval: The time between timer ticks. Must be at least
                 1 microsecond.
             missed_tick_policy: The policy of the timer when it misses a tick.
                 Commonly one of `TriggerAllMissed`, `SkipMissedAndResync`, `SkipMissedAndDrift`
                 or a custom class deriving from `MissedTickPolicy`. See the
@@ -412,17 +494,17 @@
             start_delay: The delay before the timer should start. If `auto_start` is
                 `False`, an exception is raised. This has microseconds resolution,
                 anything smaller than a microsecond means no delay.
             loop: The event loop to use to track time. If `None`,
                 `asyncio.get_running_loop()` will be used.
 
         Raises:
-            RuntimeError: if it was called without a loop and there is no
+            RuntimeError: If it was called without a loop and there is no
                 running loop.
-            ValueError: if `interval` is not positive or is smaller than 1
+            ValueError: If `interval` is not positive or is smaller than 1
                 microsecond; if `start_delay` is negative or `start_delay` was specified
                 but `auto_start` is `False`.
         """
         if interval < timedelta(microseconds=1):
             raise ValueError(
                 f"The `interval` must be positive and at least 1 microsecond, not {interval}"
             )
@@ -478,157 +560,32 @@
         `consume()` will set it back to `None` to tell `ready()` that it needs
         to wait again.
         """
 
         if auto_start:
             self.reset(start_delay=start_delay)
 
-    # We need a noqa here because the docs have a Raises section but the documented
-    # exceptions are raised indirectly.
-    @classmethod
-    def timeout(  # noqa: DOC502
-        cls,
-        delay: timedelta,
-        /,
-        *,
-        auto_start: bool = True,
-        start_delay: timedelta = timedelta(0),
-        loop: asyncio.AbstractEventLoop | None = None,
-    ) -> Timer:
-        """Create a timer useful for tracking timeouts.
-
-        This is basically a shortcut to create a timer with
-        `SkipMissedAndDrift(delay_tolerance=timedelta(0))` as the missed tick policy.
-
-        See the class documentation for details.
-
-        Args:
-            delay: The time until the timer ticks. Must be at least
-                1 microsecond.
-            auto_start: Whether the timer should be started when the
-                instance is created. This can only be `True` if there is
-                already a running loop or an explicit `loop` that is running
-                was passed.
-            start_delay: The delay before the timer should start. If `auto_start` is
-                `False`, an exception is raised. This has microseconds resolution,
-                anything smaller than a microsecond means no delay.
-            loop: The event loop to use to track time. If `None`,
-                `asyncio.get_running_loop()` will be used.
-
-        Returns:
-            The timer instance.
-
-        Raises:
-            RuntimeError: if it was called without a loop and there is no
-                running loop.
-            ValueError: if `interval` is not positive or is smaller than 1
-                microsecond; if `start_delay` is negative or `start_delay` was specified
-                but `auto_start` is `False`.
-        """
-        return Timer(
-            delay,
-            SkipMissedAndDrift(delay_tolerance=timedelta(0)),
-            auto_start=auto_start,
-            start_delay=start_delay,
-            loop=loop,
-        )
-
-    # We need a noqa here because the docs have a Raises section but the documented
-    # exceptions are raised indirectly.
-    @classmethod
-    def periodic(  # noqa: DOC502
-        cls,
-        period: timedelta,
-        /,
-        *,
-        skip_missed_ticks: bool = False,
-        auto_start: bool = True,
-        start_delay: timedelta = timedelta(0),
-        loop: asyncio.AbstractEventLoop | None = None,
-    ) -> Timer:
-        """Create a periodic timer.
-
-        This is basically a shortcut to create a timer with either
-        `TriggerAllMissed()` or `SkipMissedAndResync()` as the missed tick policy
-        (depending on `skip_missed_ticks`).
-
-        See the class documentation for details.
-
-        Args:
-            period: The time between timer ticks. Must be at least
-                1 microsecond.
-            skip_missed_ticks: Whether to skip missed ticks or trigger them
-                all until it catches up.
-            auto_start: Whether the timer should be started when the
-                instance is created. This can only be `True` if there is
-                already a running loop or an explicit `loop` that is running
-                was passed.
-            start_delay: The delay before the timer should start. If `auto_start` is
-                `False`, an exception is raised. This has microseconds resolution,
-                anything smaller than a microsecond means no delay.
-            loop: The event loop to use to track time. If `None`,
-                `asyncio.get_running_loop()` will be used.
-
-        Returns:
-            The timer instance.
-
-        Raises:
-            RuntimeError: if it was called without a loop and there is no
-                running loop.
-            ValueError: if `interval` is not positive or is smaller than 1
-                microsecond; if `start_delay` is negative or `start_delay` was specified
-                but `auto_start` is `False`.
-        """
-        missed_tick_policy = (
-            SkipMissedAndResync() if skip_missed_ticks else TriggerAllMissed()
-        )
-        return Timer(
-            period,
-            missed_tick_policy,
-            auto_start=auto_start,
-            start_delay=start_delay,
-            loop=loop,
-        )
-
     @property
     def interval(self) -> timedelta:
-        """The interval between timer ticks.
-
-        Returns:
-            The interval between timer ticks.
-        """
+        """The interval between timer ticks."""
         return timedelta(microseconds=self._interval)
 
     @property
     def missed_tick_policy(self) -> MissedTickPolicy:
-        """The policy of the timer when it misses a tick.
-
-        Returns:
-            The policy of the timer when it misses a tick.
-        """
+        """The policy of the timer when it misses a tick."""
         return self._missed_tick_policy
 
     @property
     def loop(self) -> asyncio.AbstractEventLoop:
-        """The event loop used by the timer to track time.
-
-        Returns:
-            The event loop used by the timer to track time.
-        """
+        """The event loop used by the timer to track time."""
         return self._loop
 
     @property
     def is_running(self) -> bool:
-        """Whether the timer is running.
-
-        This will be `False` if the timer was stopped, or not started yet.
-
-        Returns:
-            Whether the timer is running.
-        """
+        """Whether the timer is running."""
         return not self._stopped
 
     def reset(self, *, start_delay: timedelta = timedelta(0)) -> None:
         """Reset the timer to start timing from now (plus an optional delay).
 
         If the timer was stopped, or not started yet, it will be started.
 
@@ -636,16 +593,16 @@
         more details.
 
         Args:
             start_delay: The delay before the timer should start. This has microseconds
                 resolution, anything smaller than a microsecond means no delay.
 
         Raises:
-            RuntimeError: if it was called without a running loop.
-            ValueError: if `start_delay` is negative.
+            RuntimeError: If it was called without a running loop.
+            ValueError: If `start_delay` is negative.
         """
         start_delay_ms = _to_microseconds(start_delay)
 
         if start_delay_ms < 0:
             raise ValueError(f"`start_delay` can't be negative, got {start_delay}")
         self._stopped = False
         self._next_tick_time = self._now() + start_delay_ms + self._interval
@@ -677,15 +634,15 @@
         The timer will remain ready (this method will return immediately)
         until it is consumed.
 
         Returns:
             Whether the timer was started and it is still running.
 
         Raises:
-            RuntimeError: if it was called without a running loop.
+            RuntimeError: If it was called without a running loop.
         """
         # If there are messages waiting to be consumed, return immediately.
         if self._current_drift is not None:
             return True
 
         # If `_next_tick_time` is `None`, it means it was created with
         # `auto_start=False` and should be started.
@@ -697,18 +654,23 @@
 
         # If a stop was explicitly requested, we bail out.
         if self._stopped:
             return False
 
         now = self._now()
         time_to_next_tick = self._next_tick_time - now
+
         # If we didn't reach the tick yet, sleep until we do.
-        if time_to_next_tick > 0:
+        # We need to do this in a loop also reacting to the reset event, as the timer
+        # could be reset while we are sleeping, in which case we need to recalculate
+        # the time to the next tick and try again.
+        while time_to_next_tick > 0:
             await asyncio.sleep(time_to_next_tick / 1_000_000)
             now = self._now()
+            time_to_next_tick = self._next_tick_time - now
 
         # If a stop was explicitly requested during the sleep, we bail out.
         if self._stopped:
             return False
 
         self._current_drift = timedelta(microseconds=now - self._next_tick_time)
         self._next_tick_time = self._missed_tick_policy.calculate_next_tick_time(
@@ -727,15 +689,15 @@
         it actually triggered. See the class documentation for more details.
 
         Returns:
             The difference between when the timer should have triggered and the
                 time when it actually did.
 
         Raises:
-            ReceiverStoppedError: if the timer was stopped via `stop()`.
+            ReceiverStoppedError: If the timer was stopped via `stop()`.
         """
         # If it was stopped and there it no pending result, we raise
         # (if there is a pending result, then we still want to return it first)
         if self._stopped and self._current_drift is None:
             raise ReceiverStoppedError(self)
 
         assert (
@@ -750,24 +712,16 @@
 
         Returns:
             The current monotonic clock time in microseconds.
         """
         return _to_microseconds(self._loop.time())
 
     def __str__(self) -> str:
-        """Return a string representation of the timer.
-
-        Returns:
-            The string representation of the timer.
-        """
+        """Return a string representation of this timer."""
         return f"{type(self).__name__}({self.interval})"
 
     def __repr__(self) -> str:
-        """Return a string representation of the timer.
-
-        Returns:
-            The string representation of the timer.
-        """
+        """Return a string with the internal representation of this timer."""
         return (
             f"{type(self).__name__}<{self.interval=}, {self.missed_tick_policy=}, "
             f"{self.loop=}, {self.is_running=}>"
         )
```

### Comparing `frequenz-channels-1.0.0b2/src/frequenz_channels.egg-info/requires.txt` & `frequenz-channels-1.0.0rc1/src/frequenz_channels.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 typing-extensions<5,>=4.5.0
 watchfiles<0.22.0,>=0.15.0
 
 [dev]
 frequenz-channels[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
 [dev-flake8]
-flake8==6.1.0
+flake8==7.0.0
 flake8-docstrings==1.7.0
 flake8-pyproject==1.2.3
-pydoclint==0.3.2
+pydoclint==0.4.1
 pydocstyle==6.3.0
 
 [dev-formatting]
-black==23.10.1
-isort==5.12.0
+black==24.2.0
+isort==5.13.2
 
 [dev-mkdocs]
-black==23.10.1
-Markdown==3.4.4
-mike==1.1.2
+Markdown==3.5.2
+black==24.2.0
+frequenz-repo-config[lib]==0.9.1
+markdown-callouts==0.4.0
+markdown-svgbob==202112.1022
+mike==2.0.0
 mkdocs-gen-files==0.5.0
+mkdocs-include-markdown-plugin==6.0.4
 mkdocs-literate-nav==0.6.1
-mkdocs-material==9.3.2
-mkdocs-macros-plugin==1.0.4
-mkdocstrings[python]==0.23.0
-frequenz-repo-config[lib]==0.7.2
+mkdocs-macros-plugin==1.0.5
+mkdocs-material==9.5.12
+mkdocstrings[python]==0.24.1
+pymdownx-superfence-filter-lines==0.1.0
 
 [dev-mypy]
-mypy==1.6.1
-types-Markdown==3.4.2.10
 frequenz-channels[dev-mkdocs,dev-noxfile,dev-pytest]
+mypy==1.8.0
+types-Markdown==3.5.0.20240129
 
 [dev-noxfile]
 nox==2023.4.22
-frequenz-repo-config[lib]==0.7.2
+frequenz-repo-config[lib]==0.9.1
 
 [dev-pylint]
-pylint==2.17.7
 frequenz-channels[dev-mkdocs,dev-noxfile,dev-pytest]
+pylint==3.1.0
 
 [dev-pytest]
-pytest==7.4.3
 async-solipsism==0.5
-hypothesis==6.88.1
-frequenz-repo-config[extra-lint-examples]==0.7.2
-pytest-asyncio==0.21.1
+frequenz-repo-config[extra-lint-examples]==0.9.1
+hypothesis==6.98.17
+pytest==8.1.0
+pytest-asyncio==0.23.5
 pytest-mock==3.12.0
```

