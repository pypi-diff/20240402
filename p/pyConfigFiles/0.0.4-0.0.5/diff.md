# Comparing `tmp/pyConfigFiles-0.0.4.tar.gz` & `tmp/pyConfigFiles-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyConfigFiles-0.0.4.tar", last modified: Mon Apr  1 02:03:29 2024, max compression
+gzip compressed data, was "pyConfigFiles-0.0.5.tar", last modified: Tue Apr  2 00:47:40 2024, max compression
```

## Comparing `pyConfigFiles-0.0.4.tar` & `pyConfigFiles-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 02:03:29.366396 pyConfigFiles-0.0.4/
--rw-rw-rw-   0        0        0     9070 2024-04-01 02:03:29.365388 pyConfigFiles-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     8679 2024-04-01 01:57:28.000000 pyConfigFiles-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 02:03:29.350121 pyConfigFiles-0.0.4/pyConfigFiles/
--rw-rw-rw-   0        0        0       81 2024-03-26 08:27:26.000000 pyConfigFiles-0.0.4/pyConfigFiles/__init__.py
--rw-rw-rw-   0        0        0     2956 2024-04-01 02:00:17.000000 pyConfigFiles-0.0.4/pyConfigFiles/base.py
-drwxrwxrwx   0        0        0        0 2024-04-01 02:03:29.363374 pyConfigFiles-0.0.4/pyConfigFiles.egg-info/
--rw-rw-rw-   0        0        0     9070 2024-04-01 02:03:29.000000 pyConfigFiles-0.0.4/pyConfigFiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-01 02:03:29.000000 pyConfigFiles-0.0.4/pyConfigFiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 02:03:29.000000 pyConfigFiles-0.0.4/pyConfigFiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-01 02:03:29.000000 pyConfigFiles-0.0.4/pyConfigFiles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 02:03:29.366396 pyConfigFiles-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      657 2024-04-01 01:48:34.000000 pyConfigFiles-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:47:40.130612 pyConfigFiles-0.0.5/
+-rw-rw-rw-   0        0        0     9070 2024-04-02 00:47:40.129615 pyConfigFiles-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8679 2024-04-01 01:57:28.000000 pyConfigFiles-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 00:47:40.116123 pyConfigFiles-0.0.5/pyConfigFiles/
+-rw-rw-rw-   0        0        0       81 2024-03-26 08:27:26.000000 pyConfigFiles-0.0.5/pyConfigFiles/__init__.py
+-rw-rw-rw-   0        0        0     3004 2024-04-02 00:45:35.000000 pyConfigFiles-0.0.5/pyConfigFiles/base.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:47:40.128613 pyConfigFiles-0.0.5/pyConfigFiles.egg-info/
+-rw-rw-rw-   0        0        0     9070 2024-04-02 00:47:40.000000 pyConfigFiles-0.0.5/pyConfigFiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-04-02 00:47:40.000000 pyConfigFiles-0.0.5/pyConfigFiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 00:47:40.000000 pyConfigFiles-0.0.5/pyConfigFiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-02 00:47:40.000000 pyConfigFiles-0.0.5/pyConfigFiles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 00:47:40.130612 pyConfigFiles-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      657 2024-04-02 00:47:28.000000 pyConfigFiles-0.0.5/setup.py
```

### Comparing `pyConfigFiles-0.0.4/PKG-INFO` & `pyConfigFiles-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyConfigFiles
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/RPeschke/PyConfigFiles
 Author: Richard Peschke
 Author-email: peschke@hawaii.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pyConfigFiles-0.0.4/README.md` & `pyConfigFiles-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyConfigFiles-0.0.4/pyConfigFiles/base.py` & `pyConfigFiles-0.0.5/pyConfigFiles/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,18 +91,19 @@
         for f in files:
 
             new_path = os.path.join(directory_path, f)
             file_hash =  calculate_hash(new_path) 
             if file_hash in  self.__files__: 
                 continue
             fs[new_path] =  import_from_filepath(new_path)
-            self.__files__.append(file_hash)
 
 
         for file in fs.keys():
+            file_hash =  calculate_hash(file) 
+            self.__files__.append(file_hash)
             for fun in fs[file]:
                 fun(self)
```

### Comparing `pyConfigFiles-0.0.4/pyConfigFiles.egg-info/PKG-INFO` & `pyConfigFiles-0.0.5/pyConfigFiles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyConfigFiles
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/RPeschke/PyConfigFiles
 Author: Richard Peschke
 Author-email: peschke@hawaii.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pyConfigFiles-0.0.4/setup.py` & `pyConfigFiles-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyConfigFiles", 
-    version="0.0.4",
+    version="0.0.5",
     author="Richard Peschke",
     author_email="peschke@hawaii.edu",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/RPeschke/PyConfigFiles",
     packages=setuptools.find_packages(),
```

