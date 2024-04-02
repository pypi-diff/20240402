# Comparing `tmp/smyth-0.3.0.tar.gz` & `tmp/smyth-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smyth-0.3.0.tar", max compression
+gzip compressed data, was "smyth-0.3.1.tar", max compression
```

## Comparing `smyth-0.3.0.tar` & `smyth-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1512 2024-03-28 21:12:42.997709 smyth-0.3.0/LICENCE
--rw-r--r--   0        0        0    16050 2024-03-28 21:12:42.997709 smyth-0.3.0/README.md
--rw-r--r--   0        0        0     1539 2024-03-28 21:12:42.997709 smyth-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/__init__.py
--rw-r--r--   0        0        0     2487 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/__main__.py
--rw-r--r--   0        0        0     1142 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/app.py
--rw-r--r--   0        0        0     2063 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/config.py
--rw-r--r--   0        0        0     1028 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/context.py
--rw-r--r--   0        0        0        1 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/dispatcher/__init__.py
--rw-r--r--   0        0        0     3980 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/dispatcher/dispatcher.py
--rw-r--r--   0        0        0      278 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/dispatcher/exceptions.py
--rw-r--r--   0        0        0     3999 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/dispatcher/process.py
--rw-r--r--   0        0        0     5251 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/dispatcher/runner.py
--rw-r--r--   0        0        0     2318 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/dispatcher/strategy.py
--rw-r--r--   0        0        0      685 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/dispatcher/type.py
--rw-r--r--   0        0        0      169 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/endpoints/__init__.py
--rw-r--r--   0        0        0     1362 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/endpoints/invoker.py
--rw-r--r--   0        0        0     1010 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/endpoints/status.py
--rw-r--r--   0        0        0      951 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/event.py
--rw-r--r--   0        0        0      167 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/exceptions.py
--rw-r--r--   0        0        0     2997 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/process.py
--rw-r--r--   0        0        0        0 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/py.typed
--rw-r--r--   0        0        0     4583 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/runner.py
--rw-r--r--   0        0        0      674 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/schema.py
--rw-r--r--   0        0        0     2927 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/server.py
--rw-r--r--   0        0        0      542 2024-03-28 21:12:42.997709 smyth-0.3.0/src/smyth/utils.py
--rw-r--r--   0        0        0    17194 1970-01-01 00:00:00.000000 smyth-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-04-02 14:37:56.851748 smyth-0.3.1/LICENCE
+-rw-r--r--   0        0        0    16050 2024-04-02 14:37:56.851748 smyth-0.3.1/README.md
+-rw-r--r--   0        0        0     1539 2024-04-02 14:37:56.851748 smyth-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/__init__.py
+-rw-r--r--   0        0        0     2487 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/__main__.py
+-rw-r--r--   0        0        0     1142 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/app.py
+-rw-r--r--   0        0        0     2063 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/config.py
+-rw-r--r--   0        0        0     1028 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/context.py
+-rw-r--r--   0        0        0        1 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/dispatcher/__init__.py
+-rw-r--r--   0        0        0     3975 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/dispatcher/dispatcher.py
+-rw-r--r--   0        0        0      278 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/dispatcher/exceptions.py
+-rw-r--r--   0        0        0     3999 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/dispatcher/process.py
+-rw-r--r--   0        0        0     5251 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/dispatcher/runner.py
+-rw-r--r--   0        0        0     2318 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/dispatcher/strategy.py
+-rw-r--r--   0        0        0      685 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/dispatcher/type.py
+-rw-r--r--   0        0        0      169 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/endpoints/__init__.py
+-rw-r--r--   0        0        0     1362 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/endpoints/invoker.py
+-rw-r--r--   0        0        0     1010 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/endpoints/status.py
+-rw-r--r--   0        0        0      951 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/event.py
+-rw-r--r--   0        0        0      167 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/exceptions.py
+-rw-r--r--   0        0        0     2997 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/process.py
+-rw-r--r--   0        0        0        0 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/py.typed
+-rw-r--r--   0        0        0     4583 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/runner.py
+-rw-r--r--   0        0        0      674 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/schema.py
+-rw-r--r--   0        0        0     2927 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/server.py
+-rw-r--r--   0        0        0      542 2024-04-02 14:37:56.851748 smyth-0.3.1/src/smyth/utils.py
+-rw-r--r--   0        0        0    17194 1970-01-01 00:00:00.000000 smyth-0.3.1/PKG-INFO
```

### Comparing `smyth-0.3.0/LICENCE` & `smyth-0.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/README.md` & `smyth-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/pyproject.toml` & `smyth-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smyth"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Mirumee <it@mirumee.com>"]
 readme = "README.md"
 packages = [{include = "smyth", from = "src"}]
 license = "BSD-3-Clause"
 repository = "https://github.com/mirumee/smyth"
 classifiers = [
```

### Comparing `smyth-0.3.0/src/smyth/__main__.py` & `smyth-0.3.1/src/smyth/__main__.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/app.py` & `smyth-0.3.1/src/smyth/app.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/config.py` & `smyth-0.3.1/src/smyth/config.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/context.py` & `smyth-0.3.1/src/smyth/context.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/dispatcher/dispatcher.py` & `smyth-0.3.1/src/smyth/dispatcher/dispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                     name=f"{process_definition.name}:{index}",
                     handler_config=process_definition.handler_config,
                 )
                 process_groups[process_definition.name].append(process)
         return process_groups
 
     def get_process_definition(self, path: str) -> ProcessDefinition:
-        for path, process_def in self.process_definitions.items():
+        for process_def in self.process_definitions.values():
             if process_def.url_path.match(path):
                 return process_def
         raise ProcessDefinitionNotFoundError(
             f"No process definition found for path {path}"
         )
 
     async def dispatch(self, request: Request):
```

### Comparing `smyth-0.3.0/src/smyth/dispatcher/process.py` & `smyth-0.3.1/src/smyth/dispatcher/process.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/dispatcher/runner.py` & `smyth-0.3.1/src/smyth/dispatcher/runner.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/dispatcher/strategy.py` & `smyth-0.3.1/src/smyth/dispatcher/strategy.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/dispatcher/type.py` & `smyth-0.3.1/src/smyth/dispatcher/type.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/endpoints/invoker.py` & `smyth-0.3.1/src/smyth/endpoints/invoker.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/endpoints/status.py` & `smyth-0.3.1/src/smyth/endpoints/status.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/event.py` & `smyth-0.3.1/src/smyth/event.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/process.py` & `smyth-0.3.1/src/smyth/process.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/runner.py` & `smyth-0.3.1/src/smyth/runner.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/schema.py` & `smyth-0.3.1/src/smyth/schema.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/server.py` & `smyth-0.3.1/src/smyth/server.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/src/smyth/utils.py` & `smyth-0.3.1/src/smyth/utils.py`

 * *Files identical despite different names*

### Comparing `smyth-0.3.0/PKG-INFO` & `smyth-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smyth
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Home-page: https://github.com/mirumee/smyth
 License: BSD-3-Clause
 Author: Mirumee
 Author-email: it@mirumee.com
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 3 - Alpha
```

