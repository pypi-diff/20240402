# Comparing `tmp/gg-release-notes-1.6.0.tar.gz` & `tmp/gg-release-notes-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gg-release-notes-1.6.0.tar", last modified: Tue Apr  2 08:37:01 2024, max compression
+gzip compressed data, was "gg-release-notes-1.6.1.tar", last modified: Tue Apr  2 08:41:19 2024, max compression
```

## Comparing `gg-release-notes-1.6.0.tar` & `gg-release-notes-1.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     1066 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/LICENSE
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/PKG-INFO
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     2593 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/README.md
--rw-rw-r--   0 rogier    (1000) rogier    (1000)       38 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/setup.cfg
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      981 2024-04-02 08:36:44.000000 gg-release-notes-1.6.0/setup.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/src/
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/src/gg_release_notes/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:36:47.000000 gg-release-notes-1.6.0/src/gg_release_notes/__init__.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/src/gg_release_notes/config/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/src/gg_release_notes/config/__init__.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      306 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/src/gg_release_notes/config/env_config.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      596 2024-04-02 08:18:52.000000 gg-release-notes-1.6.0/src/gg_release_notes/config/github_config.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     1520 2024-04-02 08:18:52.000000 gg-release-notes-1.6.0/src/gg_release_notes/config/prompt_config.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     5004 2024-04-02 08:23:10.000000 gg-release-notes-1.6.0/src/gg_release_notes/generate_release_notes.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     3815 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/src/gg_release_notes/pull_request.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     4666 2024-04-02 08:18:53.000000 gg-release-notes-1.6.0/src/gg_release_notes/upload.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/src/gg_release_notes/utils/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/src/gg_release_notes/utils/__init__.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      422 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/src/gg_release_notes/utils/encode_bs64.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     1842 2024-04-02 08:18:53.000000 gg-release-notes-1.6.0/src/gg_release_notes/version.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/src/gg_release_notes.egg-info/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 08:37:01.000000 gg-release-notes-1.6.0/src/gg_release_notes.egg-info/PKG-INFO
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      678 2024-04-02 08:37:01.000000 gg-release-notes-1.6.0/src/gg_release_notes.egg-info/SOURCES.txt
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        1 2024-04-02 08:37:01.000000 gg-release-notes-1.6.0/src/gg_release_notes.egg-info/dependency_links.txt
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      187 2024-04-02 08:37:01.000000 gg-release-notes-1.6.0/src/gg_release_notes.egg-info/requires.txt
--rw-rw-r--   0 rogier    (1000) rogier    (1000)       17 2024-04-02 08:37:01.000000 gg-release-notes-1.6.0/src/gg_release_notes.egg-info/top_level.txt
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:41:19.663026 gg-release-notes-1.6.1/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     1066 2023-06-30 08:34:34.000000 gg-release-notes-1.6.1/LICENSE
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 08:41:19.663026 gg-release-notes-1.6.1/PKG-INFO
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     2593 2023-06-30 08:34:34.000000 gg-release-notes-1.6.1/README.md
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)       38 2024-04-02 08:41:19.663026 gg-release-notes-1.6.1/setup.cfg
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      981 2024-04-02 08:40:52.000000 gg-release-notes-1.6.1/setup.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:41:19.663026 gg-release-notes-1.6.1/src/
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:41:19.663026 gg-release-notes-1.6.1/src/gg_release_notes/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:36:47.000000 gg-release-notes-1.6.1/src/gg_release_notes/__init__.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:41:19.663026 gg-release-notes-1.6.1/src/gg_release_notes/config/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.6.1/src/gg_release_notes/config/__init__.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      306 2023-06-30 08:34:34.000000 gg-release-notes-1.6.1/src/gg_release_notes/config/env_config.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      596 2024-04-02 08:18:52.000000 gg-release-notes-1.6.1/src/gg_release_notes/config/github_config.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     1520 2024-04-02 08:18:52.000000 gg-release-notes-1.6.1/src/gg_release_notes/config/prompt_config.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     5004 2024-04-02 08:23:10.000000 gg-release-notes-1.6.1/src/gg_release_notes/generate_release_notes.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     3815 2023-06-30 08:34:34.000000 gg-release-notes-1.6.1/src/gg_release_notes/pull_request.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     4666 2024-04-02 08:18:53.000000 gg-release-notes-1.6.1/src/gg_release_notes/upload.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:41:19.663026 gg-release-notes-1.6.1/src/gg_release_notes/utils/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.6.1/src/gg_release_notes/utils/__init__.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      422 2023-06-30 08:34:34.000000 gg-release-notes-1.6.1/src/gg_release_notes/utils/encode_bs64.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     1842 2024-04-02 08:18:53.000000 gg-release-notes-1.6.1/src/gg_release_notes/version.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:41:19.663026 gg-release-notes-1.6.1/src/gg_release_notes.egg-info/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 08:41:19.000000 gg-release-notes-1.6.1/src/gg_release_notes.egg-info/PKG-INFO
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      678 2024-04-02 08:41:19.000000 gg-release-notes-1.6.1/src/gg_release_notes.egg-info/SOURCES.txt
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        1 2024-04-02 08:41:19.000000 gg-release-notes-1.6.1/src/gg_release_notes.egg-info/dependency_links.txt
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      165 2024-04-02 08:41:19.000000 gg-release-notes-1.6.1/src/gg_release_notes.egg-info/requires.txt
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)       17 2024-04-02 08:41:19.000000 gg-release-notes-1.6.1/src/gg_release_notes.egg-info/top_level.txt
```

### Comparing `gg-release-notes-1.6.0/LICENSE` & `gg-release-notes-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.0/PKG-INFO` & `gg-release-notes-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gg-release-notes
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python Interface for generating release notes for Github Actions
 Home-page: https://github.com/DataWiz40/gg-release-notes/
 Author: DataWiz40
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `gg-release-notes-1.6.0/README.md` & `gg-release-notes-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.0/setup.py` & `gg-release-notes-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with open("./requirements-test.txt") as extra_requirements:
     EXTRA_REQUIRED = extra_requirements.read().split("\n")
 
 
 setup(
     name="gg-release-notes",
-    version="1.6.0",
+    version="1.6.1",
     description="Python Interface for generating release notes for Github Actions",
     url="https://github.com/DataWiz40/gg-release-notes/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DataWiz40",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
```

### Comparing `gg-release-notes-1.6.0/src/gg_release_notes/config/github_config.py` & `gg-release-notes-1.6.1/src/gg_release_notes/config/github_config.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.0/src/gg_release_notes/config/prompt_config.py` & `gg-release-notes-1.6.1/src/gg_release_notes/config/prompt_config.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.0/src/gg_release_notes/generate_release_notes.py` & `gg-release-notes-1.6.1/src/gg_release_notes/generate_release_notes.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.0/src/gg_release_notes/pull_request.py` & `gg-release-notes-1.6.1/src/gg_release_notes/pull_request.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.0/src/gg_release_notes/upload.py` & `gg-release-notes-1.6.1/src/gg_release_notes/upload.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.0/src/gg_release_notes/version.py` & `gg-release-notes-1.6.1/src/gg_release_notes/version.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.0/src/gg_release_notes.egg-info/PKG-INFO` & `gg-release-notes-1.6.1/src/gg_release_notes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gg-release-notes
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python Interface for generating release notes for Github Actions
 Home-page: https://github.com/DataWiz40/gg-release-notes/
 Author: DataWiz40
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `gg-release-notes-1.6.0/src/gg_release_notes.egg-info/SOURCES.txt` & `gg-release-notes-1.6.1/src/gg_release_notes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

