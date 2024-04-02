# Comparing `tmp/streamlit_analytics2-0.6.4.tar.gz` & `tmp/streamlit_analytics2-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_analytics2-0.6.4.tar", last modified: Mon Mar 18 08:08:39 2024, max compression
+gzip compressed data, was "streamlit_analytics2-0.6.5.tar", last modified: Tue Apr  2 19:22:25 2024, max compression
```

## Comparing `streamlit_analytics2-0.6.4.tar` & `streamlit_analytics2-0.6.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:08:39.650752 streamlit_analytics2-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:08:39.650752 streamlit_analytics2-0.6.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-03-18 08:08:01.000000 streamlit_analytics2-0.6.4/.github/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-18 08:08:01.000000 streamlit_analytics2-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-03-18 08:08:39.650752 streamlit_analytics2-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-18 08:08:01.000000 streamlit_analytics2-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 08:08:39.650752 streamlit_analytics2-0.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:08:39.646752 streamlit_analytics2-0.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:08:39.650752 streamlit_analytics2-0.6.4/src/streamlit_analytics2/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-18 08:08:01.000000 streamlit_analytics2-0.6.4/src/streamlit_analytics2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-03-18 08:08:01.000000 streamlit_analytics2-0.6.4/src/streamlit_analytics2/display.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-18 08:08:01.000000 streamlit_analytics2-0.6.4/src/streamlit_analytics2/firestore.py
--rw-r--r--   0 runner    (1001) docker     (127)    20067 2024-03-18 08:08:01.000000 streamlit_analytics2-0.6.4/src/streamlit_analytics2/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-18 08:08:01.000000 streamlit_analytics2-0.6.4/src/streamlit_analytics2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:08:39.650752 streamlit_analytics2-0.6.4/src/streamlit_analytics2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-03-18 08:08:39.000000 streamlit_analytics2-0.6.4/src/streamlit_analytics2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-18 08:08:39.000000 streamlit_analytics2-0.6.4/src/streamlit_analytics2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 08:08:39.000000 streamlit_analytics2-0.6.4/src/streamlit_analytics2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-18 08:08:39.000000 streamlit_analytics2-0.6.4/src/streamlit_analytics2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-18 08:08:39.000000 streamlit_analytics2-0.6.4/src/streamlit_analytics2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:08:39.650752 streamlit_analytics2-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-18 08:08:01.000000 streamlit_analytics2-0.6.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:22:25.335568 streamlit_analytics2-0.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:22:25.335568 streamlit_analytics2-0.6.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-02 19:21:44.000000 streamlit_analytics2-0.6.5/.github/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-02 19:21:44.000000 streamlit_analytics2-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-02 19:22:25.335568 streamlit_analytics2-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-02 19:21:44.000000 streamlit_analytics2-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:22:25.335568 streamlit_analytics2-0.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:22:25.331568 streamlit_analytics2-0.6.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:22:25.335568 streamlit_analytics2-0.6.5/src/streamlit_analytics2/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 19:21:44.000000 streamlit_analytics2-0.6.5/src/streamlit_analytics2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-02 19:21:44.000000 streamlit_analytics2-0.6.5/src/streamlit_analytics2/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-02 19:21:44.000000 streamlit_analytics2-0.6.5/src/streamlit_analytics2/firestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20067 2024-04-02 19:21:44.000000 streamlit_analytics2-0.6.5/src/streamlit_analytics2/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-02 19:21:44.000000 streamlit_analytics2-0.6.5/src/streamlit_analytics2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:22:25.335568 streamlit_analytics2-0.6.5/src/streamlit_analytics2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-02 19:22:25.000000 streamlit_analytics2-0.6.5/src/streamlit_analytics2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-02 19:22:25.000000 streamlit_analytics2-0.6.5/src/streamlit_analytics2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:22:25.000000 streamlit_analytics2-0.6.5/src/streamlit_analytics2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 19:22:25.000000 streamlit_analytics2-0.6.5/src/streamlit_analytics2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 19:22:25.000000 streamlit_analytics2-0.6.5/src/streamlit_analytics2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:22:25.335568 streamlit_analytics2-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 19:21:44.000000 streamlit_analytics2-0.6.5/tests/test_utils.py
```

### Comparing `streamlit_analytics2-0.6.4/.github/README.md` & `streamlit_analytics2-0.6.5/.github/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.6.4/LICENSE` & `streamlit_analytics2-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.6.4/PKG-INFO` & `streamlit_analytics2-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_analytics2
-Version: 0.6.4
+Version: 0.6.5
 Summary: Track & visualize user interactions with your streamlit app.
 Author-email: 444B <contact+pypi@444b.me>
 License: MIT License
         
         Copyright (c) 2021 Johannes Rieke
         
         Copyright (c) 2024 444B
```

### Comparing `streamlit_analytics2-0.6.4/pyproject.toml` & `streamlit_analytics2-0.6.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.1.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit_analytics2"
-version = "0.6.4"
+version = "0.6.5"
 description = "Track & visualize user interactions with your streamlit app."
 authors = [{ name = "444B", email = "contact+pypi@444b.me" }]
 license = { file = "LICENSE" }
 readme = {file = ".github/README.md", content-type = "text/markdown"}
 keywords = ["streamlit", "analytics", "visualization", "streamlit-analytics", "streamlit-analytics2"]
 classifiers = [
     "Programming Language :: Python :: 3.9",
```

### Comparing `streamlit_analytics2-0.6.4/src/streamlit_analytics2/display.py` & `streamlit_analytics2-0.6.5/src/streamlit_analytics2/display.py`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.6.4/src/streamlit_analytics2/firestore.py` & `streamlit_analytics2-0.6.5/src/streamlit_analytics2/firestore.py`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.6.4/src/streamlit_analytics2/main.py` & `streamlit_analytics2-0.6.5/src/streamlit_analytics2/main.py`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.6.4/src/streamlit_analytics2/utils.py` & `streamlit_analytics2-0.6.5/src/streamlit_analytics2/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.6.4/src/streamlit_analytics2.egg-info/PKG-INFO` & `streamlit_analytics2-0.6.5/src/streamlit_analytics2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_analytics2
-Version: 0.6.4
+Version: 0.6.5
 Summary: Track & visualize user interactions with your streamlit app.
 Author-email: 444B <contact+pypi@444b.me>
 License: MIT License
         
         Copyright (c) 2021 Johannes Rieke
         
         Copyright (c) 2024 444B
```

### Comparing `streamlit_analytics2-0.6.4/tests/test_utils.py` & `streamlit_analytics2-0.6.5/tests/test_utils.py`

 * *Files identical despite different names*

