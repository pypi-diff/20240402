# Comparing `tmp/feilian-1.1.8.tar.gz` & `tmp/feilian-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feilian-1.1.8.tar", last modified: Thu Mar 21 02:25:05 2024, max compression
+gzip compressed data, was "feilian-1.1.9.tar", last modified: Tue Apr  2 03:16:45 2024, max compression
```

## Comparing `feilian-1.1.8.tar` & `feilian-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 02:25:05.401142 feilian-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-21 02:25:05.401142 feilian-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 02:24:47.000000 feilian-1.1.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      117 2024-03-21 02:24:47.000000 feilian-1.1.8/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 02:25:05.397142 feilian-1.1.8/feilian/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-21 02:24:47.000000 feilian-1.1.8/feilian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-21 02:25:05.000000 feilian-1.1.8/feilian/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-03-21 02:24:47.000000 feilian-1.1.8/feilian/arg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-03-21 02:24:47.000000 feilian-1.1.8/feilian/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-21 02:24:47.000000 feilian-1.1.8/feilian/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-21 02:24:47.000000 feilian-1.1.8/feilian/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-21 02:24:47.000000 feilian-1.1.8/feilian/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-21 02:24:47.000000 feilian-1.1.8/feilian/string.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-21 02:24:47.000000 feilian-1.1.8/feilian/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 02:25:05.397142 feilian-1.1.8/feilian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-21 02:25:05.000000 feilian-1.1.8/feilian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-21 02:25:05.000000 feilian-1.1.8/feilian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 02:25:05.000000 feilian-1.1.8/feilian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-21 02:25:05.000000 feilian-1.1.8/feilian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-21 02:24:47.000000 feilian-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-21 02:24:47.000000 feilian-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 02:25:05.401142 feilian-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:16:45.297059 feilian-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-02 03:16:45.297059 feilian-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 03:16:21.000000 feilian-1.1.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      117 2024-04-02 03:16:21.000000 feilian-1.1.9/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:16:45.293058 feilian-1.1.9/feilian/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-02 03:16:21.000000 feilian-1.1.9/feilian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 03:16:45.000000 feilian-1.1.9/feilian/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-04-02 03:16:21.000000 feilian-1.1.9/feilian/arg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-04-02 03:16:21.000000 feilian-1.1.9/feilian/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-02 03:16:21.000000 feilian-1.1.9/feilian/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 03:16:21.000000 feilian-1.1.9/feilian/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-02 03:16:21.000000 feilian-1.1.9/feilian/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-02 03:16:21.000000 feilian-1.1.9/feilian/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-02 03:16:21.000000 feilian-1.1.9/feilian/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-02 03:16:21.000000 feilian-1.1.9/feilian/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:16:45.293058 feilian-1.1.9/feilian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-02 03:16:45.000000 feilian-1.1.9/feilian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-02 03:16:45.000000 feilian-1.1.9/feilian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 03:16:45.000000 feilian-1.1.9/feilian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 03:16:45.000000 feilian-1.1.9/feilian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-02 03:16:21.000000 feilian-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 03:16:21.000000 feilian-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 03:16:45.297059 feilian-1.1.9/setup.cfg
```

### Comparing `feilian-1.1.8/PKG-INFO` & `feilian-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feilian
-Version: 1.1.8
+Version: 1.1.9
 Summary: General data processing tool.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/feilian
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Provides-Extra: extra
 Requires-Dist: tqdm; extra == "extra"
```

### Comparing `feilian-1.1.8/README.md` & `feilian-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `feilian-1.1.8/feilian/__init__.py` & `feilian-1.1.9/feilian/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 from .io import ensure_parent_dir_exist
 from .dataframe import read_dataframe, save_dataframe, extract_dataframe_sample, merge_dataframe_rows, iter_dataframe
 from .dataframe import is_empty_text, is_nonempty_text, is_blank_text, is_non_blank_text
 from .datetime import format_time, format_date
 from .arg import ArgValueParser
 from .json import read_json, save_json
+from .utils import flatten_dict
 from .version import __version__
 
 __all__ = [
     'ensure_parent_dir_exist',
     'read_dataframe', 'save_dataframe', 'extract_dataframe_sample', 'merge_dataframe_rows', 'iter_dataframe',
     'is_empty_text', 'is_nonempty_text', 'is_blank_text', 'is_non_blank_text',
     'format_time', 'format_date',
     'ArgValueParser',
     'read_json', 'save_json',
+    'flatten_dict',
     '__version__',
 ]
```

### Comparing `feilian-1.1.8/feilian/arg.py` & `feilian-1.1.9/feilian/arg.py`

 * *Files identical despite different names*

### Comparing `feilian-1.1.8/feilian/dataframe.py` & `feilian-1.1.9/feilian/dataframe.py`

 * *Files identical despite different names*

### Comparing `feilian-1.1.8/feilian/datetime.py` & `feilian-1.1.9/feilian/datetime.py`

 * *Files identical despite different names*

### Comparing `feilian-1.1.8/feilian/json.py` & `feilian-1.1.9/feilian/json.py`

 * *Files identical despite different names*

### Comparing `feilian-1.1.8/feilian.egg-info/PKG-INFO` & `feilian-1.1.9/feilian.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feilian
-Version: 1.1.8
+Version: 1.1.9
 Summary: General data processing tool.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/feilian
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Provides-Extra: extra
 Requires-Dist: tqdm; extra == "extra"
```

### Comparing `feilian-1.1.8/pyproject.toml` & `feilian-1.1.9/pyproject.toml`

 * *Files identical despite different names*

