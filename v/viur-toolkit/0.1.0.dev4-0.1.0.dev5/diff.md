# Comparing `tmp/viur-toolkit-0.1.0.dev4.tar.gz` & `tmp/viur-toolkit-0.1.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur-toolkit-0.1.0.dev4.tar", last modified: Fri Mar 15 19:20:12 2024, max compression
+gzip compressed data, was "viur-toolkit-0.1.0.dev5.tar", last modified: Tue Apr  2 15:53:20 2024, max compression
```

## Comparing `viur-toolkit-0.1.0.dev4.tar` & `viur-toolkit-0.1.0.dev5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:20:12.759919 viur-toolkit-0.1.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-15 19:20:12.759919 viur-toolkit-0.1.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-15 19:20:12.759919 viur-toolkit-0.1.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:20:12.755919 viur-toolkit-0.1.0.dev4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:20:12.751919 viur-toolkit-0.1.0.dev4/src/viur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:20:12.755919 viur-toolkit-0.1.0.dev4/src/viur/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/src/viur/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/src/viur/toolkit/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/src/viur/toolkit/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/src/viur/toolkit/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/src/viur/toolkit/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/src/viur/toolkit/memcache.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/src/viur/toolkit/numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/src/viur/toolkit/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/src/viur/toolkit/report.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/src/viur/toolkit/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-15 19:20:08.000000 viur-toolkit-0.1.0.dev4/src/viur/toolkit/viur.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:20:12.755919 viur-toolkit-0.1.0.dev4/src/viur_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-15 19:20:12.000000 viur-toolkit-0.1.0.dev4/src/viur_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-15 19:20:12.000000 viur-toolkit-0.1.0.dev4/src/viur_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 19:20:12.000000 viur-toolkit-0.1.0.dev4/src/viur_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-15 19:20:12.000000 viur-toolkit-0.1.0.dev4/src/viur_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 19:20:12.000000 viur-toolkit-0.1.0.dev4/src/viur_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:53:20.507153 viur-toolkit-0.1.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-02 15:53:20.507153 viur-toolkit-0.1.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-02 15:53:20.507153 viur-toolkit-0.1.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:53:20.503153 viur-toolkit-0.1.0.dev5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:53:20.503153 viur-toolkit-0.1.0.dev5/src/viur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:53:20.503153 viur-toolkit-0.1.0.dev5/src/viur/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/memcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 15:53:11.000000 viur-toolkit-0.1.0.dev5/src/viur/toolkit/viur.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:53:20.507153 viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-02 15:53:20.000000 viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-02 15:53:20.000000 viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:53:20.000000 viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 15:53:20.000000 viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 15:53:20.000000 viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/top_level.txt
```

### Comparing `viur-toolkit-0.1.0.dev4/LICENSE` & `viur-toolkit-0.1.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev4/PKG-INFO` & `viur-toolkit-0.1.0.dev5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-toolkit
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: A kit of helpers and tools to simplify more intensive use of ViUR
 Home-page: https://github.com/viur-framework/viur-toolkit
 Author: Sven Eberth
 Author-email: se@mausbrand.de
 Maintainer: Sven Eberth
 Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev4 Summary: A kit of
+Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev5 Summary: A kit of
 helpers and tools to simplify more intensive use of ViUR Home-page: https://
 github.com/viur-framework/viur-toolkit Author: Sven Eberth Author-email:
 se@mausbrand.de Maintainer: Sven Eberth Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
```

### Comparing `viur-toolkit-0.1.0.dev4/setup.cfg` & `viur-toolkit-0.1.0.dev5/setup.cfg`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev4/src/viur/toolkit/checks.py` & `viur-toolkit-0.1.0.dev5/src/viur/toolkit/checks.py`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev4/src/viur/toolkit/context.py` & `viur-toolkit-0.1.0.dev5/src/viur/toolkit/context.py`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev4/src/viur/toolkit/db.py` & `viur-toolkit-0.1.0.dev5/src/viur/toolkit/db.py`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev4/src/viur/toolkit/decorators.py` & `viur-toolkit-0.1.0.dev5/src/viur/toolkit/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,42 @@
 import functools
 import json
 import logging
 import types
+import typing as t
 
 from viur.core import current, errors, securitykey
 
 __all__ = [
     "asJsonResponse",
     "cache_call_for_request",
+    "debug",
     "parseRequestPayload",
     "skeyRequired",
 ]
 
 logger = logging.getLogger(__name__)
 
 
+def debug(func: t.Callable):
+    """Decorator to print the function signature and return value"""
+
+    @functools.wraps(func)
+    def wrapper_debug(*args, **kwargs):
+        args_repr = list(map(repr, args))
+        kwargs_repr = [f"{k!s}={v!r}" for k, v in kwargs.items()]
+        signature = ", ".join(args_repr + kwargs_repr)
+        logging.info(f"CALLING {func.__name__}({signature})")
+        value = func(*args, **kwargs)
+        logging.info(f"{func.__name__} RETURNED {value}")
+        return value
+
+    return wrapper_debug
+
+
 def skeyRequired(func=None, **decoratorKwArgs):
     """Decorator that checks the skey before the method is called.
 
     Optional callable to pass keyword-arguments for the securitykey.validate-call.
 
     Example:
         >>> from viur.core import exposed
```

### Comparing `viur-toolkit-0.1.0.dev4/src/viur/toolkit/memcache.py` & `viur-toolkit-0.1.0.dev5/src/viur/toolkit/memcache.py`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev4/src/viur/toolkit/property.py` & `viur-toolkit-0.1.0.dev5/src/viur/toolkit/property.py`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev4/src/viur/toolkit/report.py` & `viur-toolkit-0.1.0.dev5/src/viur/toolkit/report.py`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev4/src/viur/toolkit/viur.py` & `viur-toolkit-0.1.0.dev5/src/viur/toolkit/viur.py`

 * *Files identical despite different names*

### Comparing `viur-toolkit-0.1.0.dev4/src/viur_toolkit.egg-info/PKG-INFO` & `viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-toolkit
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: A kit of helpers and tools to simplify more intensive use of ViUR
 Home-page: https://github.com/viur-framework/viur-toolkit
 Author: Sven Eberth
 Author-email: se@mausbrand.de
 Maintainer: Sven Eberth
 Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev4 Summary: A kit of
+Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev5 Summary: A kit of
 helpers and tools to simplify more intensive use of ViUR Home-page: https://
 github.com/viur-framework/viur-toolkit Author: Sven Eberth Author-email:
 se@mausbrand.de Maintainer: Sven Eberth Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
```

### Comparing `viur-toolkit-0.1.0.dev4/src/viur_toolkit.egg-info/SOURCES.txt` & `viur-toolkit-0.1.0.dev5/src/viur_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

