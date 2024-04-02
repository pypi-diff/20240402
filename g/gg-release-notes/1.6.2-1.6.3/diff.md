# Comparing `tmp/gg-release-notes-1.6.2.tar.gz` & `tmp/gg-release-notes-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gg-release-notes-1.6.2.tar", last modified: Tue Apr  2 08:49:50 2024, max compression
+gzip compressed data, was "gg-release-notes-1.6.3.tar", last modified: Tue Apr  2 08:53:49 2024, max compression
```

## Comparing `gg-release-notes-1.6.2.tar` & `gg-release-notes-1.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:49:50.304921 gg-release-notes-1.6.2/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     1066 2023-06-30 08:34:34.000000 gg-release-notes-1.6.2/LICENSE
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 08:49:50.304921 gg-release-notes-1.6.2/PKG-INFO
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     2593 2023-06-30 08:34:34.000000 gg-release-notes-1.6.2/README.md
--rw-rw-r--   0 rogier    (1000) rogier    (1000)       38 2024-04-02 08:49:50.304921 gg-release-notes-1.6.2/setup.cfg
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      981 2024-04-02 08:48:24.000000 gg-release-notes-1.6.2/setup.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:49:50.300922 gg-release-notes-1.6.2/src/
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:49:50.300922 gg-release-notes-1.6.2/src/gg_release_notes/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:36:47.000000 gg-release-notes-1.6.2/src/gg_release_notes/__init__.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:49:50.304921 gg-release-notes-1.6.2/src/gg_release_notes/config/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.6.2/src/gg_release_notes/config/__init__.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      323 2024-04-02 08:49:26.000000 gg-release-notes-1.6.2/src/gg_release_notes/config/env_config.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      596 2024-04-02 08:18:52.000000 gg-release-notes-1.6.2/src/gg_release_notes/config/github_config.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     1520 2024-04-02 08:18:52.000000 gg-release-notes-1.6.2/src/gg_release_notes/config/prompt_config.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     5004 2024-04-02 08:23:10.000000 gg-release-notes-1.6.2/src/gg_release_notes/generate_release_notes.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     3815 2023-06-30 08:34:34.000000 gg-release-notes-1.6.2/src/gg_release_notes/pull_request.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     4666 2024-04-02 08:18:53.000000 gg-release-notes-1.6.2/src/gg_release_notes/upload.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:49:50.304921 gg-release-notes-1.6.2/src/gg_release_notes/utils/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.6.2/src/gg_release_notes/utils/__init__.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      422 2023-06-30 08:34:34.000000 gg-release-notes-1.6.2/src/gg_release_notes/utils/encode_bs64.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     1842 2024-04-02 08:18:53.000000 gg-release-notes-1.6.2/src/gg_release_notes/version.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:49:50.304921 gg-release-notes-1.6.2/src/gg_release_notes.egg-info/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 08:49:50.000000 gg-release-notes-1.6.2/src/gg_release_notes.egg-info/PKG-INFO
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      678 2024-04-02 08:49:50.000000 gg-release-notes-1.6.2/src/gg_release_notes.egg-info/SOURCES.txt
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        1 2024-04-02 08:49:50.000000 gg-release-notes-1.6.2/src/gg_release_notes.egg-info/dependency_links.txt
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      190 2024-04-02 08:49:50.000000 gg-release-notes-1.6.2/src/gg_release_notes.egg-info/requires.txt
--rw-rw-r--   0 rogier    (1000) rogier    (1000)       17 2024-04-02 08:49:50.000000 gg-release-notes-1.6.2/src/gg_release_notes.egg-info/top_level.txt
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     1066 2023-06-30 08:34:34.000000 gg-release-notes-1.6.3/LICENSE
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/PKG-INFO
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     2593 2023-06-30 08:34:34.000000 gg-release-notes-1.6.3/README.md
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)       38 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/setup.cfg
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      981 2024-04-02 08:53:27.000000 gg-release-notes-1.6.3/setup.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/src/
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/src/gg_release_notes/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:36:47.000000 gg-release-notes-1.6.3/src/gg_release_notes/__init__.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/src/gg_release_notes/config/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.6.3/src/gg_release_notes/config/__init__.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      323 2024-04-02 08:49:26.000000 gg-release-notes-1.6.3/src/gg_release_notes/config/env_config.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      596 2024-04-02 08:18:52.000000 gg-release-notes-1.6.3/src/gg_release_notes/config/github_config.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     1520 2024-04-02 08:18:52.000000 gg-release-notes-1.6.3/src/gg_release_notes/config/prompt_config.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     5004 2024-04-02 08:23:10.000000 gg-release-notes-1.6.3/src/gg_release_notes/generate_release_notes.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     3815 2023-06-30 08:34:34.000000 gg-release-notes-1.6.3/src/gg_release_notes/pull_request.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     4666 2024-04-02 08:18:53.000000 gg-release-notes-1.6.3/src/gg_release_notes/upload.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/src/gg_release_notes/utils/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.6.3/src/gg_release_notes/utils/__init__.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      422 2023-06-30 08:34:34.000000 gg-release-notes-1.6.3/src/gg_release_notes/utils/encode_bs64.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     1842 2024-04-02 08:18:53.000000 gg-release-notes-1.6.3/src/gg_release_notes/version.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/src/gg_release_notes.egg-info/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 08:53:49.000000 gg-release-notes-1.6.3/src/gg_release_notes.egg-info/PKG-INFO
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      678 2024-04-02 08:53:49.000000 gg-release-notes-1.6.3/src/gg_release_notes.egg-info/SOURCES.txt
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        1 2024-04-02 08:53:49.000000 gg-release-notes-1.6.3/src/gg_release_notes.egg-info/dependency_links.txt
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      190 2024-04-02 08:53:49.000000 gg-release-notes-1.6.3/src/gg_release_notes.egg-info/requires.txt
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)       17 2024-04-02 08:53:49.000000 gg-release-notes-1.6.3/src/gg_release_notes.egg-info/top_level.txt
```

### Comparing `gg-release-notes-1.6.2/LICENSE` & `gg-release-notes-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.2/PKG-INFO` & `gg-release-notes-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gg-release-notes
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python Interface for generating release notes for Github Actions
 Home-page: https://github.com/DataWiz40/gg-release-notes/
 Author: DataWiz40
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `gg-release-notes-1.6.2/README.md` & `gg-release-notes-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.2/setup.py` & `gg-release-notes-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with open("./requirements-test.txt") as extra_requirements:
     EXTRA_REQUIRED = extra_requirements.read().split("\n")
 
 
 setup(
     name="gg-release-notes",
-    version="1.6.2",
+    version="1.6.3",
     description="Python Interface for generating release notes for Github Actions",
     url="https://github.com/DataWiz40/gg-release-notes/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DataWiz40",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
```

### Comparing `gg-release-notes-1.6.2/src/gg_release_notes/config/github_config.py` & `gg-release-notes-1.6.3/src/gg_release_notes/config/github_config.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.2/src/gg_release_notes/config/prompt_config.py` & `gg-release-notes-1.6.3/src/gg_release_notes/config/prompt_config.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.2/src/gg_release_notes/generate_release_notes.py` & `gg-release-notes-1.6.3/src/gg_release_notes/generate_release_notes.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.2/src/gg_release_notes/pull_request.py` & `gg-release-notes-1.6.3/src/gg_release_notes/pull_request.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.2/src/gg_release_notes/upload.py` & `gg-release-notes-1.6.3/src/gg_release_notes/upload.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.2/src/gg_release_notes/version.py` & `gg-release-notes-1.6.3/src/gg_release_notes/version.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.2/src/gg_release_notes.egg-info/PKG-INFO` & `gg-release-notes-1.6.3/src/gg_release_notes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gg-release-notes
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python Interface for generating release notes for Github Actions
 Home-page: https://github.com/DataWiz40/gg-release-notes/
 Author: DataWiz40
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `gg-release-notes-1.6.2/src/gg_release_notes.egg-info/SOURCES.txt` & `gg-release-notes-1.6.3/src/gg_release_notes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

