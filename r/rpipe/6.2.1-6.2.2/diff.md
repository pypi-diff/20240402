# Comparing `tmp/rpipe-6.2.1.tar.gz` & `tmp/rpipe-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpipe-6.2.1.tar", last modified: Thu Mar 28 18:13:03 2024, max compression
+gzip compressed data, was "rpipe-6.2.2.tar", last modified: Tue Apr  2 09:42:55 2024, max compression
```

## Comparing `rpipe-6.2.1.tar` & `rpipe-6.2.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:03.176491 rpipe-6.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-28 18:12:59.000000 rpipe-6.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-03-28 18:13:03.176491 rpipe-6.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-28 18:12:59.000000 rpipe-6.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-28 18:12:59.000000 rpipe-6.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:03.168491 rpipe-6.2.1/rpipe/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:03.172491 rpipe-6.2.1/rpipe/client/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:03.172491 rpipe-6.2.1/rpipe/client/config/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/client/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/client/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/client/config/option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/client/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/client/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/client/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/client/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/client/recv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/client/send.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/client/util.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:03.176491 rpipe-6.2.1/rpipe/server/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/server/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/server/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/server/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/server/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/server/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/server/save_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/server/shutdown_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/server/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/server/write.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-28 18:12:59.000000 rpipe-6.2.1/rpipe/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:03.176491 rpipe-6.2.1/rpipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-03-28 18:13:03.000000 rpipe-6.2.1/rpipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-28 18:13:03.000000 rpipe-6.2.1/rpipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:13:03.000000 rpipe-6.2.1/rpipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-28 18:13:03.000000 rpipe-6.2.1/rpipe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 18:13:03.000000 rpipe-6.2.1/rpipe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 18:13:03.000000 rpipe-6.2.1/rpipe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 18:13:03.176491 rpipe-6.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:55.021538 rpipe-6.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 09:42:51.000000 rpipe-6.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-02 09:42:55.021538 rpipe-6.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-02 09:42:51.000000 rpipe-6.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-02 09:42:51.000000 rpipe-6.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:55.017538 rpipe-6.2.2/rpipe/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:55.017538 rpipe-6.2.2/rpipe/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:55.021538 rpipe-6.2.2/rpipe/client/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/client/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/client/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/client/config/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/client/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/client/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/client/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/client/recv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/client/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/client/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:55.021538 rpipe-6.2.2/rpipe/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/server/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/server/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/server/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/server/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/server/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/server/save_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/server/shutdown_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/server/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/server/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-02 09:42:51.000000 rpipe-6.2.2/rpipe/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:55.021538 rpipe-6.2.2/rpipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-02 09:42:55.000000 rpipe-6.2.2/rpipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-02 09:42:55.000000 rpipe-6.2.2/rpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:42:55.000000 rpipe-6.2.2/rpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 09:42:55.000000 rpipe-6.2.2/rpipe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:42:55.000000 rpipe-6.2.2/rpipe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 09:42:55.000000 rpipe-6.2.2/rpipe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:42:55.021538 rpipe-6.2.2/setup.cfg
```

### Comparing `rpipe-6.2.1/LICENSE` & `rpipe-6.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/PKG-INFO` & `rpipe-6.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: rpipe
-Version: 6.2.1
+Version: 6.2.2
 Summary: A little python remote pipe server and client.
 License: GPLv3
 Project-URL: Homepage, https://github.com/zwimer/rpipe
-Classifier: License :: OSI Approved :: BSD License
+Keywords: remote,pipe
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodomex
 Requires-Dist: requests
 Requires-Dist: waitress
 Requires-Dist: flask
```

### Comparing `rpipe-6.2.1/README.md` & `rpipe-6.2.2/README.md`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/pyproject.toml` & `rpipe-6.2.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rpipe"
 classifiers = [
-    "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
+    "Development Status :: 5 - Production/Stable",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
+keywords = ["remote", "pipe"]
 license = {text = "GPLv3"}
 description = "A little python remote pipe server and client."
 urls = {Homepage = "https://github.com/zwimer/rpipe"}
 requires-python = ">= 3.10"
 dependencies = [
     # Client
     "pycryptodomex",
@@ -44,14 +46,22 @@
 [tool.setuptools.dynamic]
 version = {attr = "rpipe.__version__"}
 
 # Tools
 
 [tool.black]
 line-length = 110
-target-version = ["py310"]
+target-version = ["py310", "py311", "py312"]
 
 [tool.ruff]
 ignore=["E731"]
 line-length = 110
+
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "F403"]
+
+[tool.bandit]
+skips = ["B201", "B104", "B403"]
+
+[tool.vulture]
+ignore_names = ["cli", "_help", "_show_version", "_channel", "strict_slashes"]
+paths = ["rpipe"]
```

### Comparing `rpipe-6.2.1/rpipe/client/client.py` & `rpipe-6.2.2/rpipe/client/client.py`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/rpipe/client/config/config.py` & `rpipe-6.2.2/rpipe/client/config/config.py`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/rpipe/client/config/option.py` & `rpipe-6.2.2/rpipe/client/config/option.py`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/rpipe/client/crypt.py` & `rpipe-6.2.2/rpipe/client/crypt.py`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/rpipe/client/errors.py` & `rpipe-6.2.2/rpipe/client/errors.py`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/rpipe/client/io.py` & `rpipe-6.2.2/rpipe/client/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,14 @@
         self._n: int = n
         self._log.debug("Starting up IO thread.")
         self._thread = Thread(target=self, daemon=True)
         self._thread.start()
 
     # Main Thread:
 
-    def eof(self) -> bool:
-        return self._eof and not self._buffer
-
     def read(self) -> bytes:
         """
         :param delay: sleep delay ms to allow more IO to load
         :return: Up to n bytes; returns b"" only upon final read
         """
         with self._cond:
             self._cond.wait_for(lambda: self._buffer or self._eof)
@@ -56,15 +53,15 @@
         for i in self._buffer:
             total += len(i)
             count += 1
             if total > self._n:
                 break
         if len(self._buffer) > 1:
             count -= 1
-        assert count > 0, "Write thread wrote too much data"
+        assert count > 0, "Write thread wrote too much data"  # nosec B101
         # Stitch together pieces as efficiently as possible
         if count == 1:
             return self._buffer.popleft()
         return b"".join(self._buffer.popleft() for _ in range(count))
 
     # Worker thread
```

### Comparing `rpipe-6.2.1/rpipe/client/main.py` & `rpipe-6.2.2/rpipe/client/main.py`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/rpipe/client/recv.py` & `rpipe-6.2.2/rpipe/client/recv.py`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/rpipe/client/send.py` & `rpipe-6.2.2/rpipe/client/send.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,28 +24,33 @@
     Raise an exception according to the send response error
     """
     match UploadErrorCode(r.status_code):
         case UploadErrorCode.illegal_version:
             raise VersionError(f"Server requires version >= {r.text}")
         case UploadErrorCode.conflict:
             raise MultipleClients("The stream ID changed mid-upload; maybe the channel was cleared?")
-        case UploadErrorCode.wrong_version | UploadErrorCode.too_big | UploadErrorCode.forbidden | UploadErrorCode.stream_id:
+        case (
+            UploadErrorCode.wrong_version
+            | UploadErrorCode.too_big
+            | UploadErrorCode.forbidden
+            | UploadErrorCode.stream_id
+        ):
             raise ReportThis(r.text)
         case _:
             raise RuntimeError(r)
 
 
 def _send_block(data: bytes, config: Config, params: UploadRequestParams) -> None:
     """
     Upload the given block of data; updates params for next block
     """
     r = request("PUT", channel_url(config), params=params.to_dict(), data=data)
     if r.ok:
         headers = UploadResponseHeaders.from_dict(r.headers)
-        assert params.stream_id == headers.stream_id
+        assert params.stream_id == headers.stream_id  # nosec B101
     elif r.status_code == UploadErrorCode.wait.value:
         getLogger(_LOG).debug("Pipe full, sleeping for %s seconds.", WAIT_DELAY_SEC)
         sleep(WAIT_DELAY_SEC)
         _send_block(data, config, params)
     else:
         _send_error(r)
```

### Comparing `rpipe-6.2.1/rpipe/client/util.py` & `rpipe-6.2.2/rpipe/client/util.py`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/rpipe/server/data.py` & `rpipe-6.2.2/rpipe/server/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from ..version import Version
 
 
 CHARSET = string.ascii_lowercase + string.ascii_uppercase + string.digits
 
 
 def _uid() -> str:
-    return "".join(random.choices(CHARSET, k=32))
+    return "".join(random.choices(CHARSET, k=32))  # nosec B311
 
 
 @dataclass(kw_only=True)
 class Stream:
     """
     Holds data about a stream
     """
```

### Comparing `rpipe-6.2.1/rpipe/server/main.py` & `rpipe-6.2.2/rpipe/server/main.py`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/rpipe/server/read.py` & `rpipe-6.2.2/rpipe/server/read.py`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/rpipe/server/save_state.py` & `rpipe-6.2.2/rpipe/server/save_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     if len(streams):
         raise RuntimeError("Do not load a state on top of an existing state")
     print("Loading saved program state...")
     with lock:
         for p in dir_.iterdir():
             _log.debug("Loading channel %s", p.name)
             with p.open("rb") as f:
-                streams[p.name] = pickle.load(f)
+                streams[p.name] = pickle.load(f)  # nosec B301
 
 
 def save(dir_: Path):
     """
     Save the program state
     Do not call this unless the server is shutdown!
     """
```

### Comparing `rpipe-6.2.1/rpipe/server/server.py` & `rpipe-6.2.2/rpipe/server/server.py`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/rpipe/server/shutdown_handler.py` & `rpipe-6.2.2/rpipe/server/shutdown_handler.py`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/rpipe/server/util.py` & `rpipe-6.2.2/rpipe/server/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 if TYPE_CHECKING:
     from enum import Enum
     from typing import TypeVar, Any
     from collections.abc import Callable, Iterable
     from ..shared import UploadRequestParams, DownloadRequestParams
 
 if TYPE_CHECKING:
-    ArgsT = TypeVar("ArgsT", bound=Callable)
+    _ArgsT = TypeVar("_ArgsT", bound=Callable)
 
 
 class Boolean:
     """
     A mutable boolean
     """
 
@@ -101,15 +101,15 @@
 
 
 def log_response(log_name: str = "util"):
     """
     A decorator that logs the returned flask Responses to the log log_name
     """
 
-    def decorator(func: Callable[[ArgsT], Response]) -> Callable[[ArgsT], Response]:
+    def decorator(func: Callable[[_ArgsT], Response]) -> Callable[[_ArgsT], Response]:
         def inner(*args, **kwargs) -> Response:
             ret: Response = func(*args, **kwargs)
             _log_response(getLogger(log_name), ret)
             return ret
 
         return inner
```

### Comparing `rpipe-6.2.1/rpipe/server/write.py` & `rpipe-6.2.2/rpipe/server/write.py`

 * *Files identical despite different names*

### Comparing `rpipe-6.2.1/rpipe/shared.py` & `rpipe-6.2.2/rpipe/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 if TYPE_CHECKING:
     from requests.structures import CaseInsensitiveDict
     from werkzeug.datastructures import MultiDict
 
 
 WEB_VERSION = Version("0.0.0")
-assert not WEB_VERSION.invalid()
+assert not WEB_VERSION.invalid()  # nosec B101
 
 
 @dataclass
 class _ToDict:
     def to_dict(self) -> dict[str, str]:
         return {i.replace("_", "-"): str(k) for i, k in asdict(self).items() if k is not None}
```

### Comparing `rpipe-6.2.1/rpipe/version.py` & `rpipe-6.2.2/rpipe/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 
-__version__: str = "6.2.1"  # Must be "<major>.<minor>.<patch>", all numbers
+__version__: str = "6.2.2"  # Must be "<major>.<minor>.<patch>", all numbers
 
 
 class Version:
     _invalid = (-1, -1, -1)
 
     def __init__(self, v: str):
         self.str = v
```

### Comparing `rpipe-6.2.1/rpipe.egg-info/PKG-INFO` & `rpipe-6.2.2/rpipe.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: rpipe
-Version: 6.2.1
+Version: 6.2.2
 Summary: A little python remote pipe server and client.
 License: GPLv3
 Project-URL: Homepage, https://github.com/zwimer/rpipe
-Classifier: License :: OSI Approved :: BSD License
+Keywords: remote,pipe
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodomex
 Requires-Dist: requests
 Requires-Dist: waitress
 Requires-Dist: flask
```

### Comparing `rpipe-6.2.1/rpipe.egg-info/SOURCES.txt` & `rpipe-6.2.2/rpipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

