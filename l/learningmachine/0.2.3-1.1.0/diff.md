# Comparing `tmp/learningmachine-0.2.3.tar.gz` & `tmp/learningmachine-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learningmachine-0.2.3.tar", last modified: Mon Feb  5 06:55:06 2024, max compression
+gzip compressed data, was "learningmachine-1.1.0.tar", last modified: Mon Apr  1 23:37:51 2024, max compression
```

## Comparing `learningmachine-0.2.3.tar` & `learningmachine-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 06:55:06.924160 learningmachine-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-02-05 06:44:09.000000 learningmachine-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-05 06:44:09.000000 learningmachine-0.2.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-05 06:44:09.000000 learningmachine-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-05 06:44:09.000000 learningmachine-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-05 06:55:06.924160 learningmachine-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-05 06:44:09.000000 learningmachine-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 06:55:06.920160 learningmachine-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-05 06:44:09.000000 learningmachine-0.2.3/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     4876 2024-02-05 06:44:09.000000 learningmachine-0.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-05 06:44:09.000000 learningmachine-0.2.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-05 06:44:09.000000 learningmachine-0.2.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-05 06:44:09.000000 learningmachine-0.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-05 06:44:09.000000 learningmachine-0.2.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-05 06:44:09.000000 learningmachine-0.2.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-05 06:44:09.000000 learningmachine-0.2.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-05 06:44:09.000000 learningmachine-0.2.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 06:55:06.920160 learningmachine-0.2.3/learningmachine/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-05 06:44:09.000000 learningmachine-0.2.3/learningmachine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-02-05 06:44:09.000000 learningmachine-0.2.3/learningmachine/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-02-05 06:44:09.000000 learningmachine-0.2.3/learningmachine/basemodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-02-05 06:44:09.000000 learningmachine-0.2.3/learningmachine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 06:55:06.924160 learningmachine-0.2.3/learningmachine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-05 06:55:06.000000 learningmachine-0.2.3/learningmachine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-05 06:55:06.000000 learningmachine-0.2.3/learningmachine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 06:55:06.000000 learningmachine-0.2.3/learningmachine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 06:55:04.000000 learningmachine-0.2.3/learningmachine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-05 06:55:06.000000 learningmachine-0.2.3/learningmachine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-05 06:55:06.000000 learningmachine-0.2.3/learningmachine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-05 06:55:06.924160 learningmachine-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-02-05 06:44:09.000000 learningmachine-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 06:55:06.924160 learningmachine-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-05 06:44:09.000000 learningmachine-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-05 06:44:09.000000 learningmachine-0.2.3/tests/test_learningmachine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:37:51.195891 learningmachine-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-01 23:37:31.000000 learningmachine-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-01 23:37:31.000000 learningmachine-1.1.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-01 23:37:31.000000 learningmachine-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-01 23:37:31.000000 learningmachine-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-01 23:37:51.195891 learningmachine-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-01 23:37:31.000000 learningmachine-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:37:51.191891 learningmachine-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 23:37:31.000000 learningmachine-1.1.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4876 2024-04-01 23:37:31.000000 learningmachine-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 23:37:31.000000 learningmachine-1.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 23:37:31.000000 learningmachine-1.1.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-01 23:37:31.000000 learningmachine-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-01 23:37:31.000000 learningmachine-1.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-01 23:37:31.000000 learningmachine-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-01 23:37:31.000000 learningmachine-1.1.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 23:37:31.000000 learningmachine-1.1.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:37:51.191891 learningmachine-1.1.0/learningmachine/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-01 23:37:31.000000 learningmachine-1.1.0/learningmachine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-04-01 23:37:31.000000 learningmachine-1.1.0/learningmachine/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-01 23:37:31.000000 learningmachine-1.1.0/learningmachine/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-01 23:37:31.000000 learningmachine-1.1.0/learningmachine/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-01 23:37:31.000000 learningmachine-1.1.0/learningmachine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:37:51.195891 learningmachine-1.1.0/learningmachine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-01 23:37:51.000000 learningmachine-1.1.0/learningmachine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-01 23:37:51.000000 learningmachine-1.1.0/learningmachine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 23:37:51.000000 learningmachine-1.1.0/learningmachine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 23:37:51.000000 learningmachine-1.1.0/learningmachine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 23:37:51.000000 learningmachine-1.1.0/learningmachine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 23:37:51.000000 learningmachine-1.1.0/learningmachine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-01 23:37:51.195891 learningmachine-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-04-01 23:37:31.000000 learningmachine-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:37:51.195891 learningmachine-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 23:37:31.000000 learningmachine-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-01 23:37:31.000000 learningmachine-1.1.0/tests/test_learningmachine.py
```

### Comparing `learningmachine-0.2.3/CONTRIBUTING.rst` & `learningmachine-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `learningmachine-0.2.3/LICENSE` & `learningmachine-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `learningmachine-0.2.3/PKG-INFO` & `learningmachine-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: learningmachine
-Version: 0.2.3
+Version: 1.1.0
 Summary: Machine Learning with uncertainty quantification and interpretability
 Home-page: https://github.com/Techtonique/learningmachine_python
 Author: T. Moudiki
 Author-email: thierry.moudiki@gmail.com
 License: BSD Clause Clear license
 Keywords: learningmachine
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: rpy2>=3.4.5
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
 
 Machine Learning with uncertainty quantification and interpretability.
-
```

### Comparing `learningmachine-0.2.3/README.rst` & `learningmachine-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `learningmachine-0.2.3/docs/Makefile` & `learningmachine-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `learningmachine-0.2.3/docs/conf.py` & `learningmachine-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `learningmachine-0.2.3/docs/installation.rst` & `learningmachine-1.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `learningmachine-0.2.3/docs/make.bat` & `learningmachine-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `learningmachine-0.2.3/learningmachine/utils.py` & `learningmachine-1.1.0/learningmachine/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -56,7 +56,19 @@
                             "-e",
                             "options(repos = c(techtonique = 'https://techtonique.r-universe.dev', CRAN = 'https://cloud.r-project.org')); install.packages('learningmachine', lib='.', dependencies = TRUE)",
                         ]
                     )
     if check_pkg_installed() == True:
         return 1
     return 0
+
+
+# Formatting object as a string
+def format_value(value):
+    if value is None:
+        return f"NULL"
+    if isinstance(value, str):
+        return f'"{value}"'
+    if isinstance(value, bool):
+        return f"{str(value).upper()}"
+    if isinstance(value, int) or isinstance(value, float):
+        return f"{value}"
```

### Comparing `learningmachine-0.2.3/learningmachine.egg-info/PKG-INFO` & `learningmachine-1.1.0/learningmachine.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: learningmachine
-Version: 0.2.3
+Version: 1.1.0
 Summary: Machine Learning with uncertainty quantification and interpretability
 Home-page: https://github.com/Techtonique/learningmachine_python
 Author: T. Moudiki
 Author-email: thierry.moudiki@gmail.com
 License: BSD Clause Clear license
 Keywords: learningmachine
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: rpy2>=3.4.5
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
 
 Machine Learning with uncertainty quantification and interpretability.
-
```

### Comparing `learningmachine-0.2.3/learningmachine.egg-info/SOURCES.txt` & `learningmachine-1.1.0/learningmachine.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 learningmachine/__init__.py
 learningmachine/base.py
-learningmachine/basemodels.py
+learningmachine/classifier.py
+learningmachine/regression.py
 learningmachine/utils.py
 learningmachine.egg-info/PKG-INFO
 learningmachine.egg-info/SOURCES.txt
 learningmachine.egg-info/dependency_links.txt
 learningmachine.egg-info/not-zip-safe
 learningmachine.egg-info/requires.txt
 learningmachine.egg-info/top_level.txt
```

