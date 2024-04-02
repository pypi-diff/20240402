# Comparing `tmp/easykube-0.2.0.tar.gz` & `tmp/easykube-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easykube-0.2.0.tar", last modified: Wed Mar 27 11:40:44 2024, max compression
+gzip compressed data, was "easykube-0.3.0.tar", last modified: Tue Apr  2 14:01:50 2024, max compression
```

## Comparing `easykube-0.2.0.tar` & `easykube-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:40:44.150607 easykube-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:40:44.142607 easykube-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:40:44.142607 easykube-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-27 11:40:24.000000 easykube-0.2.0/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-27 11:40:24.000000 easykube-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 11:40:24.000000 easykube-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-27 11:40:44.150607 easykube-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-27 11:40:24.000000 easykube-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:40:44.142607 easykube-0.2.0/easykube/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/flow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:40:44.146607 easykube-0.2.0/easykube/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/kubernetes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:40:44.146607 easykube-0.2.0/easykube/kubernetes/client/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/kubernetes/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/kubernetes/client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/kubernetes/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/kubernetes/client/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/kubernetes/client/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/kubernetes/client/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/kubernetes/client/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/kubernetes/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:40:44.146607 easykube-0.2.0/easykube/rest/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/rest/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/rest/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/rest/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-27 11:40:24.000000 easykube-0.2.0/easykube/rest/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:40:44.146607 easykube-0.2.0/easykube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-27 11:40:44.000000 easykube-0.2.0/easykube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-27 11:40:44.000000 easykube-0.2.0/easykube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 11:40:44.000000 easykube-0.2.0/easykube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 11:40:43.000000 easykube-0.2.0/easykube.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-27 11:40:44.000000 easykube-0.2.0/easykube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 11:40:44.000000 easykube-0.2.0/easykube.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-27 11:40:24.000000 easykube-0.2.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-03-27 11:40:44.150607 easykube-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-03-27 11:40:24.000000 easykube-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.182457 easykube-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.174457 easykube-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.178457 easykube-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 14:01:46.000000 easykube-0.3.0/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 14:01:46.000000 easykube-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 14:01:46.000000 easykube-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-02 14:01:50.182457 easykube-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 14:01:46.000000 easykube-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.178457 easykube-0.3.0/easykube/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.178457 easykube-0.3.0/easykube/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.178457 easykube-0.3.0/easykube/kubernetes/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.182457 easykube-0.3.0/easykube/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/rest/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/rest/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/rest/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/rest/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.182457 easykube-0.3.0/easykube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-02 14:01:50.000000 easykube-0.3.0/easykube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-02 14:01:50.000000 easykube-0.3.0/easykube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:01:50.000000 easykube-0.3.0/easykube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:01:49.000000 easykube-0.3.0/easykube.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 14:01:50.000000 easykube-0.3.0/easykube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 14:01:50.000000 easykube-0.3.0/easykube.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 14:01:46.000000 easykube-0.3.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-02 14:01:50.182457 easykube-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-04-02 14:01:46.000000 easykube-0.3.0/setup.py
```

### Comparing `easykube-0.2.0/.github/workflows/pypi-publish.yaml` & `easykube-0.3.0/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `easykube-0.2.0/LICENSE` & `easykube-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easykube-0.2.0/easykube/flow.py` & `easykube-0.3.0/easykube/flow.py`

 * *Files identical despite different names*

### Comparing `easykube-0.2.0/easykube/kubernetes/client/api.py` & `easykube-0.3.0/easykube/kubernetes/client/api.py`

 * *Files identical despite different names*

### Comparing `easykube-0.2.0/easykube/kubernetes/client/client.py` & `easykube-0.3.0/easykube/kubernetes/client/client.py`

 * *Files identical despite different names*

### Comparing `easykube-0.2.0/easykube/kubernetes/client/errors.py` & `easykube-0.3.0/easykube/kubernetes/client/errors.py`

 * *Files identical despite different names*

### Comparing `easykube-0.2.0/easykube/kubernetes/client/iterators.py` & `easykube-0.3.0/easykube/kubernetes/client/iterators.py`

 * *Files identical despite different names*

### Comparing `easykube-0.2.0/easykube/kubernetes/client/resource.py` & `easykube-0.3.0/easykube/kubernetes/client/resource.py`

 * *Files identical despite different names*

### Comparing `easykube-0.2.0/easykube/kubernetes/client/spec.py` & `easykube-0.3.0/easykube/kubernetes/client/spec.py`

 * *Files identical despite different names*

### Comparing `easykube-0.2.0/easykube/kubernetes/config.py` & `easykube-0.3.0/easykube/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `easykube-0.2.0/easykube/kubernetes/resources.py` & `easykube-0.3.0/easykube/kubernetes/resources.py`

 * *Files identical despite different names*

### Comparing `easykube-0.2.0/easykube/rest/client.py` & `easykube-0.3.0/easykube/rest/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,44 +2,25 @@
 import json
 import logging
 
 import httpx
 
 from ..flow import Flowable, flow, AsyncExecutor, SyncExecutor
 
-from .util import PropertyDict
-
 
 logger = logging.getLogger(__name__)
 
 
-class JsonEncoder:
-    """
-    JSON encoder that can serialize our PropertyDict and calls out to a
-    child encoder for all other object types.
-    """
-    def __init__(self, wrapped_encoder):
-        self.wrapped_encoder = wrapped_encoder
-
-    def __call__(self, obj):
-        if isinstance(obj, PropertyDict):
-            return dict(obj)
-        if self.wrapped_encoder:
-            return self.wrapped_encoder(obj)
-        else:
-            raise TypeError
-
-
 class BaseClient(Flowable):
     """
     Base class for sync and async REST clients.
     """
     def __init__(self, /, json_encoder = None, **kwargs):
         super().__init__(**kwargs)
-        self._json_encoder = JsonEncoder(json_encoder)
+        self._json_encoder = json_encoder
 
     @flow
     def request(self, method, url, **kwargs):
         """
         Builds and sends a request, respecting any custom JSON encoder.
         """
         content = kwargs.get("content")
```

### Comparing `easykube-0.2.0/easykube/rest/iterators.py` & `easykube-0.3.0/easykube/rest/iterators.py`

 * *Files identical despite different names*

### Comparing `easykube-0.2.0/easykube/rest/resource.py` & `easykube-0.3.0/easykube/rest/resource.py`

 * *Files identical despite different names*

### Comparing `easykube-0.2.0/easykube/rest/util.py` & `easykube-0.3.0/easykube/rest/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from collections.abc import MutableMapping
 
 
-class PropertyDict(MutableMapping):
+class PropertyDict(dict):
     """
-    View onto a dictionary that allows property-based access.
+    Dictionary that also supports property access.
     """
-    def __init__(self, wrapped):
-        self.__dict__["_wrapped"] = wrapped
+    def __init__(self, *args, **kwargs):
+        super().__init__(
+            {
+                k: self._wrap(v)
+                for k, v in dict(*args, **kwargs).items()
+            }
+        )
 
     def _wrap(self, value):
-        """
-        If the given value is a dict, wrap it in a property dict.
-        """
-        return self.__class__(value) if isinstance(value, dict) else value
-
-    def __getitem__(self, key):
-        return self._wrap(self.__dict__["_wrapped"].__getitem__(key))
+        if isinstance(value, PropertyDict):
+            return value
+        elif isinstance(value, dict):
+            return PropertyDict(value)
+        else:
+            return value
 
     def __setitem__(self, key, value):
-        self.__dict__["_wrapped"].__setitem__(key, value)
-
-    def __delitem__(self, key):
-        self.__dict__["_wrapped"].__delitem__(key)
+        super().__setitem__(key, self._wrap(value))
 
-    def __iter__(self):
-        yield from self.__dict__["_wrapped"].keys()
+    def setdefault(self, key, default = None):
+        return super().setdefault(key, self._wrap(default))
 
-    def __len__(self):
-        return self.__dict__["_wrapped"].__len__()
+    def update(self, *args, **kwargs):
+        super().update(
+            {
+                k: self._wrap(v)
+                for k, v in dict(*args, **kwargs).items()
+            }
+        )
 
     def __getattr__(self, name):
         try:
             return self[name]
         except KeyError:
             raise AttributeError(f"'{self.__class__.__name__}' has no attribute '{name}'")
 
-    def __setattr__(self, name, value):
-        self[name] = value
-
     def __repr__(self):
-        class_name = self.__class__.__name__
-        data = self.__dict__["_wrapped"].__repr__()
-        return f"{class_name}({data})"
+        return f"{self.__class__.__name__}({super().__repr__()})"
```

### Comparing `easykube-0.2.0/easykube.egg-info/SOURCES.txt` & `easykube-0.3.0/easykube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

