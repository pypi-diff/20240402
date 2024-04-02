# Comparing `tmp/mximport-0.0.1.tar.gz` & `tmp/mximport-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mximport-0.0.1.tar", last modified: Sun Mar 31 18:20:38 2024, max compression
+gzip compressed data, was "mximport-0.1.0.tar", last modified: Tue Apr  2 05:29:08 2024, max compression
```

## Comparing `mximport-0.0.1.tar` & `mximport-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-03-31 18:20:38.554906 mximport-0.0.1/
--rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mximport-0.0.1/MANIFEST.in
--rw-r--r--   0 yl        (1000) yl        (1000)      513 2024-03-31 18:20:38.554906 mximport-0.0.1/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)     1101 2024-03-31 18:17:48.000000 mximport-0.0.1/README.md
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-03-31 18:20:38.550907 mximport-0.0.1/mximport/
--rw-rw-r--   0 yl        (1000) yl        (1000)      616 2024-03-31 17:44:15.000000 mximport-0.0.1/mximport/__info__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)       96 2024-03-31 17:21:18.000000 mximport-0.0.1/mximport/__init__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     2923 2024-03-31 18:12:09.000000 mximport-0.0.1/mximport/main.py
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-03-31 18:20:38.554906 mximport-0.0.1/mximport.egg-info/
--rw-r--r--   0 yl        (1000) yl        (1000)      513 2024-03-31 18:20:38.000000 mximport-0.0.1/mximport.egg-info/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)      217 2024-03-31 18:20:38.000000 mximport-0.0.1/mximport.egg-info/SOURCES.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-03-31 18:20:38.000000 mximport-0.0.1/mximport.egg-info/dependency_links.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        9 2024-03-31 18:20:38.000000 mximport-0.0.1/mximport.egg-info/top_level.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-03-31 18:20:38.554906 mximport-0.0.1/setup.cfg
--rw-rw-r--   0 yl        (1000) yl        (1000)      966 2024-03-31 17:14:58.000000 mximport-0.0.1/setup.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-02 05:29:08.733122 mximport-0.1.0/
+-rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mximport-0.1.0/MANIFEST.in
+-rw-r--r--   0 yl        (1000) yl        (1000)      513 2024-04-02 05:29:08.729122 mximport-0.1.0/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)     1436 2024-04-02 05:23:02.000000 mximport-0.1.0/README.md
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-02 05:29:08.729122 mximport-0.1.0/mximport/
+-rw-rw-r--   0 yl        (1000) yl        (1000)      616 2024-04-02 05:28:58.000000 mximport-0.1.0/mximport/__info__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)      125 2024-04-02 04:02:06.000000 mximport-0.1.0/mximport/__init__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     4252 2024-04-02 05:23:02.000000 mximport-0.1.0/mximport/main.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-02 05:29:08.729122 mximport-0.1.0/mximport.egg-info/
+-rw-r--r--   0 yl        (1000) yl        (1000)      513 2024-04-02 05:29:08.000000 mximport-0.1.0/mximport.egg-info/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)      217 2024-04-02 05:29:08.000000 mximport-0.1.0/mximport.egg-info/SOURCES.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-04-02 05:29:08.000000 mximport-0.1.0/mximport.egg-info/dependency_links.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        9 2024-04-02 05:29:08.000000 mximport-0.1.0/mximport.egg-info/top_level.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-04-02 05:29:08.733122 mximport-0.1.0/setup.cfg
+-rw-rw-r--   0 yl        (1000) yl        (1000)      966 2024-03-31 17:14:58.000000 mximport-0.1.0/setup.py
```

### Comparing `mximport-0.0.1/PKG-INFO` & `mximport-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mximport
-Version: 0.0.1
+Version: 0.1.0
 Summary: Remove all limits on Python package imports
 Home-page: https://github.com/magic-python-toolbox/mximport
 Author: DIYer22
 Author-email: ylxx@live.com
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mximport-0.0.1/README.md` & `mximport-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # `mximport`: Remove all limits on Python package imports 🚀
 
-```
+```bash
 pip install mximport
 ```
 ## ▮ Painless Relative Import
 
 Relative imports in Python can become annoying because they prevent the current code from being run directly.  
 For example:
 ```python
@@ -25,29 +25,44 @@
 ~/pkg$ python main.py
 Traceback (most recent call last):
   File "~/pkg/main.py", line 1, in <module>
     from .utils import *
 ImportError: attempted relative import with no known parent package
 ```
 
-`mximport.inpkg()` can remove this limitation.
+`mximport.inpkg()` can remove this limitation:
 
 ```python
 # pkg/main.py
 from mximport import inpkg
 with inpkg():
     from .utils import *
 
 if __name__ == "__main__":
     print("This is the main file")
 ```
 Then every thing is OK! Say goodbye to `python -m pkg.main`
 
 
+## ▮ Temporary add relative path in sys.path
+
+Temporary add the relative path to sys.path during with statement
+
+Usage：
+```python
+from mximport import syspath
+with syspath(".."):  # relative path
+    import father_module
+
+with syspath("/abspath/to/module/dir"):
+    import module
+```
+
 ## ▮ Import by Path
 
 import `.py` file or package by path, return a moudle object
-```
-module = import_by_path('/path/to/module.py')
+```python
+from mximport import import_by_path
 
+module = import_by_path('/path/to/module.py')
 pkg = import_by_path('/path/to/pkg')
 ```
```

### Comparing `mximport-0.0.1/mximport/__info__.py` & `mximport-0.1.0/mximport/__info__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __description__ = "Remove all limits on Python package imports"
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `mximport-0.0.1/mximport.egg-info/PKG-INFO` & `mximport-0.1.0/mximport.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mximport
-Version: 0.0.1
+Version: 0.1.0
 Summary: Remove all limits on Python package imports
 Home-page: https://github.com/magic-python-toolbox/mximport
 Author: DIYer22
 Author-email: ylxx@live.com
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mximport-0.0.1/setup.py` & `mximport-0.1.0/setup.py`

 * *Files identical despite different names*

