# Comparing `tmp/scaleway_core-2.0.0.dev5.tar.gz` & `tmp/scaleway_core-2.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaleway_core-2.0.0.dev5.tar", max compression
+gzip compressed data, was "scaleway_core-2.0.0.dev6.tar", max compression
```

## Comparing `scaleway_core-2.0.0.dev5.tar` & `scaleway_core-2.0.0.dev6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       29 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/README.md
--rw-r--r--   0        0        0     1144 2023-11-27 13:19:44.940068 scaleway_core-2.0.0.dev5/pyproject.toml
--rw-r--r--   0        0        0      128 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/__init__.py
--rw-r--r--   0        0        0     4707 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/api.py
--rw-r--r--   0        0        0     1133 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/bridge/__init__.py
--rw-r--r--   0        0        0     1471 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/bridge/money.py
--rw-r--r--   0        0        0      188 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/bridge/region.py
--rw-r--r--   0        0        0      953 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/bridge/scwfile.py
--rw-r--r--   0        0        0     1307 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/bridge/serviceinfo.py
--rw-r--r--   0        0        0     2192 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/bridge/timeseries.py
--rw-r--r--   0        0        0      444 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/bridge/zone.py
--rw-r--r--   0        0        0     3592 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/client.py
--rw-r--r--   0        0        0      670 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/profile/__init__.py
--rw-r--r--   0        0        0      810 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/profile/env.py
--rw-r--r--   0        0        0      307 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/profile/file.py
--rw-r--r--   0        0        0     7003 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/profile/profile.py
--rw-r--r--   0        0        0        0 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/py.typed
--rw-r--r--   0        0        0      782 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/utils/__init__.py
--rw-r--r--   0        0        0     2119 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/utils/fetch_all_pages.py
--rw-r--r--   0        0        0      600 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/utils/project_or_organization_id.py
--rw-r--r--   0        0        0    50787 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/utils/random_name.py
--rw-r--r--   0        0        0     1092 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/utils/resolve_one_of.py
--rw-r--r--   0        0        0      714 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/utils/strenummeta.py
--rw-r--r--   0        0        0      512 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/utils/validate_path_param.py
--rw-r--r--   0        0        0     3532 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/utils/waiter.py
--rw-r--r--   0        0        0        0 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/validations/__init__.py
--rw-r--r--   0        0        0      998 2023-11-27 13:19:31.635713 scaleway_core-2.0.0.dev5/scaleway_core/validations/string_validation.py
--rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 scaleway_core-2.0.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/README.md
+-rw-r--r--   0        0        0     1144 2023-11-28 15:51:13.506362 scaleway_core-2.0.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/__init__.py
+-rw-r--r--   0        0        0     4707 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/api.py
+-rw-r--r--   0        0        0     1133 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/bridge/__init__.py
+-rw-r--r--   0        0        0     1471 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/bridge/money.py
+-rw-r--r--   0        0        0      188 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/bridge/region.py
+-rw-r--r--   0        0        0      953 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/bridge/scwfile.py
+-rw-r--r--   0        0        0     1307 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/bridge/serviceinfo.py
+-rw-r--r--   0        0        0     2192 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/bridge/timeseries.py
+-rw-r--r--   0        0        0      444 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/bridge/zone.py
+-rw-r--r--   0        0        0     3592 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/client.py
+-rw-r--r--   0        0        0      670 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/profile/__init__.py
+-rw-r--r--   0        0        0      810 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/profile/env.py
+-rw-r--r--   0        0        0      307 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/profile/file.py
+-rw-r--r--   0        0        0     7003 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/py.typed
+-rw-r--r--   0        0        0      782 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/utils/__init__.py
+-rw-r--r--   0        0        0     2119 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/utils/fetch_all_pages.py
+-rw-r--r--   0        0        0      600 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/utils/project_or_organization_id.py
+-rw-r--r--   0        0        0    50787 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/utils/random_name.py
+-rw-r--r--   0        0        0     1092 2023-11-28 15:50:57.342387 scaleway_core-2.0.0.dev6/scaleway_core/utils/resolve_one_of.py
+-rw-r--r--   0        0        0      714 2023-11-28 15:50:57.346387 scaleway_core-2.0.0.dev6/scaleway_core/utils/strenummeta.py
+-rw-r--r--   0        0        0      512 2023-11-28 15:50:57.346387 scaleway_core-2.0.0.dev6/scaleway_core/utils/validate_path_param.py
+-rw-r--r--   0        0        0     3532 2023-11-28 15:50:57.346387 scaleway_core-2.0.0.dev6/scaleway_core/utils/waiter.py
+-rw-r--r--   0        0        0        0 2023-11-28 15:50:57.346387 scaleway_core-2.0.0.dev6/scaleway_core/validations/__init__.py
+-rw-r--r--   0        0        0      998 2023-11-28 15:50:57.346387 scaleway_core-2.0.0.dev6/scaleway_core/validations/string_validation.py
+-rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 scaleway_core-2.0.0.dev6/PKG-INFO
```

### Comparing `scaleway_core-2.0.0.dev5/pyproject.toml` & `scaleway_core-2.0.0.dev6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scaleway-core"
-version = "2.0.0.dev5"
+version = "2.0.0.dev6"
 description = "Scaleway SDK for Python"
 authors = ["Scaleway <opensource@scaleway.com>"]
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
```

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/api.py` & `scaleway_core-2.0.0.dev6/scaleway_core/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/bridge/__init__.py` & `scaleway_core-2.0.0.dev6/scaleway_core/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/bridge/money.py` & `scaleway_core-2.0.0.dev6/scaleway_core/bridge/money.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/bridge/scwfile.py` & `scaleway_core-2.0.0.dev6/scaleway_core/bridge/scwfile.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/bridge/serviceinfo.py` & `scaleway_core-2.0.0.dev6/scaleway_core/bridge/serviceinfo.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/bridge/timeseries.py` & `scaleway_core-2.0.0.dev6/scaleway_core/bridge/timeseries.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/client.py` & `scaleway_core-2.0.0.dev6/scaleway_core/client.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/profile/__init__.py` & `scaleway_core-2.0.0.dev6/scaleway_core/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/profile/env.py` & `scaleway_core-2.0.0.dev6/scaleway_core/profile/env.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/profile/profile.py` & `scaleway_core-2.0.0.dev6/scaleway_core/profile/profile.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/utils/__init__.py` & `scaleway_core-2.0.0.dev6/scaleway_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/utils/fetch_all_pages.py` & `scaleway_core-2.0.0.dev6/scaleway_core/utils/fetch_all_pages.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/utils/project_or_organization_id.py` & `scaleway_core-2.0.0.dev6/scaleway_core/utils/project_or_organization_id.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/utils/random_name.py` & `scaleway_core-2.0.0.dev6/scaleway_core/utils/random_name.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/utils/resolve_one_of.py` & `scaleway_core-2.0.0.dev6/scaleway_core/utils/resolve_one_of.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/utils/strenummeta.py` & `scaleway_core-2.0.0.dev6/scaleway_core/utils/strenummeta.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/utils/validate_path_param.py` & `scaleway_core-2.0.0.dev6/scaleway_core/utils/validate_path_param.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/utils/waiter.py` & `scaleway_core-2.0.0.dev6/scaleway_core/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/scaleway_core/validations/string_validation.py` & `scaleway_core-2.0.0.dev6/scaleway_core/validations/string_validation.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-2.0.0.dev5/PKG-INFO` & `scaleway_core-2.0.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaleway-core
-Version: 2.0.0.dev5
+Version: 2.0.0.dev6
 Summary: Scaleway SDK for Python
 License: BSD
 Author: Scaleway
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

