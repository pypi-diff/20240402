# Comparing `tmp/dsame3_simple-0.0.1.tar.gz` & `tmp/dsame3_simple-0.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsame3_simple-0.0.1.tar", last modified: Tue Apr  2 16:19:35 2024, max compression
+gzip compressed data, was "dsame3_simple-0.0.1.post1.tar", last modified: Tue Apr  2 16:39:57 2024, max compression
```

## Comparing `dsame3_simple-0.0.1.tar` & `dsame3_simple-0.0.1.post1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:19:35.542086 dsame3_simple-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-02 16:19:31.000000 dsame3_simple-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10486 2024-04-02 16:19:35.542086 dsame3_simple-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-04-02 16:19:31.000000 dsame3_simple-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-02 16:19:31.000000 dsame3_simple-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:19:35.542086 dsame3_simple-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:19:35.538086 dsame3_simple-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:19:35.542086 dsame3_simple-0.0.1/src/dsame3_simple/
--rw-r--r--   0 runner    (1001) docker     (127)   275555 2024-04-02 16:19:31.000000 dsame3_simple-0.0.1/src/dsame3_simple/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-02 16:19:31.000000 dsame3_simple-0.0.1/src/dsame3_simple/dsame.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:19:35.542086 dsame3_simple-0.0.1/src/dsame3_simple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10486 2024-04-02 16:19:35.000000 dsame3_simple-0.0.1/src/dsame3_simple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-02 16:19:35.000000 dsame3_simple-0.0.1/src/dsame3_simple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:19:35.000000 dsame3_simple-0.0.1/src/dsame3_simple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 16:19:35.000000 dsame3_simple-0.0.1/src/dsame3_simple.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 16:19:35.000000 dsame3_simple-0.0.1/src/dsame3_simple.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:39:57.666433 dsame3_simple-0.0.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-02 16:39:53.000000 dsame3_simple-0.0.1.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-04-02 16:39:57.666433 dsame3_simple-0.0.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-04-02 16:39:53.000000 dsame3_simple-0.0.1.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-02 16:39:53.000000 dsame3_simple-0.0.1.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:39:57.666433 dsame3_simple-0.0.1.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:39:57.662433 dsame3_simple-0.0.1.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:39:57.662433 dsame3_simple-0.0.1.post1/src/dsame3_simple/
+-rw-r--r--   0 runner    (1001) docker     (127)   275555 2024-04-02 16:39:53.000000 dsame3_simple-0.0.1.post1/src/dsame3_simple/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-02 16:39:53.000000 dsame3_simple-0.0.1.post1/src/dsame3_simple/dsame.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:39:57.662433 dsame3_simple-0.0.1.post1/src/dsame3_simple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-04-02 16:39:57.000000 dsame3_simple-0.0.1.post1/src/dsame3_simple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-02 16:39:57.000000 dsame3_simple-0.0.1.post1/src/dsame3_simple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:39:57.000000 dsame3_simple-0.0.1.post1/src/dsame3_simple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 16:39:57.000000 dsame3_simple-0.0.1.post1/src/dsame3_simple.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 16:39:57.000000 dsame3_simple-0.0.1.post1/src/dsame3_simple.egg-info/top_level.txt
```

### Comparing `dsame3_simple-0.0.1/LICENSE` & `dsame3_simple-0.0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsame3_simple-0.0.1/PKG-INFO` & `dsame3_simple-0.0.1.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dsame3_simple
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: Simplified version of dsame3 to decode EAS SAME messages to readable text.
-Author: Joseph W. Metcalf, James Kitchens
+Author: Joseph W. Metcalf, James Kitchens, Matthew R. McDougal
 Author-email: "Matthew R. McDougal" <ka0s@arrl.net>
 Project-URL: Homepage, https://github.com/ars-ka0s/dsame3_simple
 Project-URL: Bug Tracker, https://github.com/ars-ka0s/dsame3_simple/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dsame3_simple-0.0.1/README.md` & `dsame3_simple-0.0.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `dsame3_simple-0.0.1/pyproject.toml` & `dsame3_simple-0.0.1.post1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dsame3_simple"
-version = "0.0.1"
+version = "0.0.1-1"
 dependencies = [
 ]
 authors = [
-    { name="Joseph W. Metcalf"},
-    { name="James Kitchens"},
-    { name="Matthew R. McDougal", email="ka0s@arrl.net"}
+    { name="Joseph W. Metcalf" },
+    { name="James Kitchens" },
+    { name="Matthew R. McDougal" },
+    { name="Matthew R. McDougal", email="ka0s@arrl.net" }
 ]
 description = "Simplified version of dsame3 to decode EAS SAME messages to readable text."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"Development Status :: 3 - Alpha",
```

### Comparing `dsame3_simple-0.0.1/src/dsame3_simple/defs.py` & `dsame3_simple-0.0.1.post1/src/dsame3_simple/defs.py`

 * *Files identical despite different names*

### Comparing `dsame3_simple-0.0.1/src/dsame3_simple/dsame.py` & `dsame3_simple-0.0.1.post1/src/dsame3_simple/dsame.py`

 * *Files identical despite different names*

### Comparing `dsame3_simple-0.0.1/src/dsame3_simple.egg-info/PKG-INFO` & `dsame3_simple-0.0.1.post1/src/dsame3_simple.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dsame3_simple
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: Simplified version of dsame3 to decode EAS SAME messages to readable text.
-Author: Joseph W. Metcalf, James Kitchens
+Author: Joseph W. Metcalf, James Kitchens, Matthew R. McDougal
 Author-email: "Matthew R. McDougal" <ka0s@arrl.net>
 Project-URL: Homepage, https://github.com/ars-ka0s/dsame3_simple
 Project-URL: Bug Tracker, https://github.com/ars-ka0s/dsame3_simple/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

