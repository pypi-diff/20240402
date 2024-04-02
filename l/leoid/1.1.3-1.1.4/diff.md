# Comparing `tmp/leoid-1.1.3.tar.gz` & `tmp/leoid-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leoid-1.1.3.tar", last modified: Sun Mar 31 22:46:11 2024, max compression
+gzip compressed data, was "leoid-1.1.4.tar", last modified: Tue Apr  2 21:19:50 2024, max compression
```

## Comparing `leoid-1.1.3.tar` & `leoid-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jayticku   (501) staff       (20)        0 2024-03-31 22:46:11.395612 leoid-1.1.3/
--rw-r--r--   0 jayticku   (501) staff       (20)       19 2024-03-28 19:04:31.000000 leoid-1.1.3/MANIFEST.in
--rw-r--r--   0 jayticku   (501) staff       (20)      723 2024-03-31 22:46:11.395412 leoid-1.1.3/PKG-INFO
--rw-r--r--   0 jayticku   (501) staff       (20)      242 2024-03-31 22:43:03.000000 leoid-1.1.3/README.md
-drwxr-xr-x   0 jayticku   (501) staff       (20)        0 2024-03-31 22:46:11.385729 leoid-1.1.3/leoid/
--rw-r--r--   0 jayticku   (501) staff       (20)       25 2024-03-28 18:09:40.000000 leoid-1.1.3/leoid/__init__.py
--rw-r--r--   0 jayticku   (501) staff       (20)     1192 2024-03-31 22:41:24.000000 leoid-1.1.3/leoid/leoid.py
--rw-r--r--   0 jayticku   (501) staff       (20)   560307 2024-03-28 20:02:00.000000 leoid-1.1.3/leoid/stage_1.pkl
--rw-r--r--   0 jayticku   (501) staff       (20) 10242284 2024-03-28 19:56:06.000000 leoid-1.1.3/leoid/stage_2.pkl
-drwxr-xr-x   0 jayticku   (501) staff       (20)        0 2024-03-31 22:46:11.395179 leoid-1.1.3/leoid.egg-info/
--rw-r--r--   0 jayticku   (501) staff       (20)      723 2024-03-31 22:46:11.000000 leoid-1.1.3/leoid.egg-info/PKG-INFO
--rw-r--r--   0 jayticku   (501) staff       (20)      243 2024-03-31 22:46:11.000000 leoid-1.1.3/leoid.egg-info/SOURCES.txt
--rw-r--r--   0 jayticku   (501) staff       (20)        1 2024-03-31 22:46:11.000000 leoid-1.1.3/leoid.egg-info/dependency_links.txt
--rw-r--r--   0 jayticku   (501) staff       (20)       61 2024-03-31 22:46:11.000000 leoid-1.1.3/leoid.egg-info/requires.txt
--rw-r--r--   0 jayticku   (501) staff       (20)        6 2024-03-31 22:46:11.000000 leoid-1.1.3/leoid.egg-info/top_level.txt
--rw-r--r--   0 jayticku   (501) staff       (20)       38 2024-03-31 22:46:11.395664 leoid-1.1.3/setup.cfg
--rw-r--r--   0 jayticku   (501) staff       (20)      774 2024-03-31 22:43:43.000000 leoid-1.1.3/setup.py
+drwxr-xr-x   0 jayticku   (501) staff       (20)        0 2024-04-02 21:19:50.418295 leoid-1.1.4/
+-rw-r--r--   0 jayticku   (501) staff       (20)       19 2024-03-28 19:04:31.000000 leoid-1.1.4/MANIFEST.in
+-rw-r--r--   0 jayticku   (501) staff       (20)      844 2024-04-02 21:19:50.418072 leoid-1.1.4/PKG-INFO
+-rw-r--r--   0 jayticku   (501) staff       (20)      363 2024-04-02 21:19:20.000000 leoid-1.1.4/README.md
+drwxr-xr-x   0 jayticku   (501) staff       (20)        0 2024-04-02 21:19:50.406624 leoid-1.1.4/leoid/
+-rw-r--r--   0 jayticku   (501) staff       (20)       25 2024-03-28 18:09:40.000000 leoid-1.1.4/leoid/__init__.py
+-rw-r--r--   0 jayticku   (501) staff       (20)     1192 2024-03-31 22:41:24.000000 leoid-1.1.4/leoid/leoid.py
+-rw-r--r--   0 jayticku   (501) staff       (20)   560307 2024-03-28 20:02:00.000000 leoid-1.1.4/leoid/stage_1.pkl
+-rw-r--r--   0 jayticku   (501) staff       (20) 10242284 2024-03-28 19:56:06.000000 leoid-1.1.4/leoid/stage_2.pkl
+drwxr-xr-x   0 jayticku   (501) staff       (20)        0 2024-04-02 21:19:50.417852 leoid-1.1.4/leoid.egg-info/
+-rw-r--r--   0 jayticku   (501) staff       (20)      844 2024-04-02 21:19:50.000000 leoid-1.1.4/leoid.egg-info/PKG-INFO
+-rw-r--r--   0 jayticku   (501) staff       (20)      243 2024-04-02 21:19:50.000000 leoid-1.1.4/leoid.egg-info/SOURCES.txt
+-rw-r--r--   0 jayticku   (501) staff       (20)        1 2024-04-02 21:19:50.000000 leoid-1.1.4/leoid.egg-info/dependency_links.txt
+-rw-r--r--   0 jayticku   (501) staff       (20)       61 2024-04-02 21:19:50.000000 leoid-1.1.4/leoid.egg-info/requires.txt
+-rw-r--r--   0 jayticku   (501) staff       (20)        6 2024-04-02 21:19:50.000000 leoid-1.1.4/leoid.egg-info/top_level.txt
+-rw-r--r--   0 jayticku   (501) staff       (20)       38 2024-04-02 21:19:50.418343 leoid-1.1.4/setup.cfg
+-rw-r--r--   0 jayticku   (501) staff       (20)      774 2024-04-02 21:19:34.000000 leoid-1.1.4/setup.py
```

### Comparing `leoid-1.1.3/leoid/leoid.py` & `leoid-1.1.4/leoid/leoid.py`

 * *Files identical despite different names*

### Comparing `leoid-1.1.3/leoid/stage_1.pkl` & `leoid-1.1.4/leoid/stage_1.pkl`

 * *Files identical despite different names*

### Comparing `leoid-1.1.3/leoid/stage_2.pkl` & `leoid-1.1.4/leoid/stage_2.pkl`

 * *Files identical despite different names*

### Comparing `leoid-1.1.3/setup.py` & `leoid-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'leoid',
-    version = '1.1.3',
+    version = '1.1.4',
     author = 'Jay Ticku',
     description = 'LEOID Python Package',
     long_description = long_description,
     long_description_content_type='text/markdown',
     install_requires = [
         'imbalanced-learn==0.12.0',
         'scikit-learn==1.2.2',
```

