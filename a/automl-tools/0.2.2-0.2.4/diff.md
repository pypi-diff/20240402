# Comparing `tmp/automl_tools-0.2.2.tar.gz` & `tmp/automl_tools-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automl_tools-0.2.2.tar", last modified: Tue Apr  2 05:56:48 2024, max compression
+gzip compressed data, was "automl_tools-0.2.4.tar", last modified: Tue Apr  2 06:08:19 2024, max compression
```

## Comparing `automl_tools-0.2.2.tar` & `automl_tools-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 05:56:48.857604 automl_tools-0.2.2/
--rw-rw-rw-   0        0        0     1092 2024-04-02 05:07:53.000000 automl_tools-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     4379 2024-04-02 05:56:48.857604 automl_tools-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3653 2024-04-02 05:07:53.000000 automl_tools-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 05:56:48.841977 automl_tools-0.2.2/automl_tools/
--rw-rw-rw-   0        0        0      140 2024-04-02 05:56:15.000000 automl_tools-0.2.2/automl_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 05:56:48.857604 automl_tools-0.2.2/automl_tools/functions/
--rw-rw-rw-   0        0        0        0 2024-04-02 05:07:53.000000 automl_tools-0.2.2/automl_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    10171 2024-04-02 05:07:53.000000 automl_tools-0.2.2/automl_tools/functions/imputation.py
--rw-rw-rw-   0        0        0     4684 2024-04-02 05:07:53.000000 automl_tools-0.2.2/automl_tools/functions/logger.py
--rw-rw-rw-   0        0        0     8043 2024-04-02 05:07:53.000000 automl_tools-0.2.2/automl_tools/functions/main.py
--rw-rw-rw-   0        0        0     5060 2024-04-02 05:07:53.000000 automl_tools-0.2.2/automl_tools/functions/modeling.py
--rw-rw-rw-   0        0        0     7806 2024-04-02 05:07:53.000000 automl_tools-0.2.2/automl_tools/functions/optimization_binary.py
--rw-rw-rw-   0        0        0     7892 2024-04-02 05:07:53.000000 automl_tools-0.2.2/automl_tools/functions/optimization_multi_class.py
--rw-rw-rw-   0        0        0     7617 2024-04-02 05:07:53.000000 automl_tools-0.2.2/automl_tools/functions/optimization_regression.py
--rw-rw-rw-   0        0        0     1091 2024-04-02 05:07:53.000000 automl_tools-0.2.2/automl_tools/functions/parameter.py
--rw-rw-rw-   0        0        0     2794 2024-04-02 05:07:53.000000 automl_tools-0.2.2/automl_tools/functions/prepare.py
--rw-rw-rw-   0        0        0     8153 2024-04-02 05:07:53.000000 automl_tools-0.2.2/automl_tools/functions/processing.py
--rw-rw-rw-   0        0        0     6851 2024-04-02 05:07:53.000000 automl_tools-0.2.2/automl_tools/functions/selection.py
--rw-rw-rw-   0        0        0     9909 2024-04-02 05:07:53.000000 automl_tools-0.2.2/automl_tools/functions/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 05:56:48.841977 automl_tools-0.2.2/automl_tools.egg-info/
--rw-rw-rw-   0        0        0     4379 2024-04-02 05:56:48.000000 automl_tools-0.2.2/automl_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      748 2024-04-02 05:56:48.000000 automl_tools-0.2.2/automl_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 05:56:48.000000 automl_tools-0.2.2/automl_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      301 2024-04-02 05:56:48.000000 automl_tools-0.2.2/automl_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-02 05:56:48.000000 automl_tools-0.2.2/automl_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      731 2024-04-02 05:34:42.000000 automl_tools-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-04-02 05:56:48.857604 automl_tools-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1128 2024-04-02 05:56:47.000000 automl_tools-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:08:19.283429 automl_tools-0.2.4/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 automl_tools-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-04-02 05:58:10.000000 automl_tools-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4379 2024-04-02 06:08:19.283429 automl_tools-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3653 2024-04-02 05:07:53.000000 automl_tools-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 06:08:19.249977 automl_tools-0.2.4/automl_tools/
+-rw-rw-rw-   0        0        0      150 2024-04-02 06:07:44.000000 automl_tools-0.2.4/automl_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:08:19.283429 automl_tools-0.2.4/automl_tools/functions/
+-rw-rw-rw-   0        0        0        0 2024-04-02 05:07:53.000000 automl_tools-0.2.4/automl_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    10171 2024-04-02 05:07:53.000000 automl_tools-0.2.4/automl_tools/functions/imputation.py
+-rw-rw-rw-   0        0        0     4684 2024-04-02 05:07:53.000000 automl_tools-0.2.4/automl_tools/functions/logger.py
+-rw-rw-rw-   0        0        0     8043 2024-04-02 05:07:53.000000 automl_tools-0.2.4/automl_tools/functions/main.py
+-rw-rw-rw-   0        0        0     5060 2024-04-02 05:07:53.000000 automl_tools-0.2.4/automl_tools/functions/modeling.py
+-rw-rw-rw-   0        0        0     7806 2024-04-02 05:07:53.000000 automl_tools-0.2.4/automl_tools/functions/optimization_binary.py
+-rw-rw-rw-   0        0        0     7892 2024-04-02 05:07:53.000000 automl_tools-0.2.4/automl_tools/functions/optimization_multi_class.py
+-rw-rw-rw-   0        0        0     7617 2024-04-02 05:07:53.000000 automl_tools-0.2.4/automl_tools/functions/optimization_regression.py
+-rw-rw-rw-   0        0        0     1091 2024-04-02 05:07:53.000000 automl_tools-0.2.4/automl_tools/functions/parameter.py
+-rw-rw-rw-   0        0        0     2794 2024-04-02 05:07:53.000000 automl_tools-0.2.4/automl_tools/functions/prepare.py
+-rw-rw-rw-   0        0        0     8153 2024-04-02 05:07:53.000000 automl_tools-0.2.4/automl_tools/functions/processing.py
+-rw-rw-rw-   0        0        0     6851 2024-04-02 05:07:53.000000 automl_tools-0.2.4/automl_tools/functions/selection.py
+-rw-rw-rw-   0        0        0     9909 2024-04-02 05:07:53.000000 automl_tools-0.2.4/automl_tools/functions/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:08:19.283429 automl_tools-0.2.4/automl_tools.egg-info/
+-rw-rw-rw-   0        0        0     4379 2024-04-02 06:08:19.000000 automl_tools-0.2.4/automl_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2024-04-02 06:08:19.000000 automl_tools-0.2.4/automl_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 06:08:19.000000 automl_tools-0.2.4/automl_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      301 2024-04-02 06:08:19.000000 automl_tools-0.2.4/automl_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-02 06:08:19.000000 automl_tools-0.2.4/automl_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      727 2024-04-02 06:05:00.000000 automl_tools-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-04-02 06:08:19.283429 automl_tools-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2024-04-02 06:08:18.000000 automl_tools-0.2.4/setup.py
```

### Comparing `automl_tools-0.2.2/LICENSE` & `automl_tools-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/PKG-INFO` & `automl_tools-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automl_tools
-Version: 0.2.2
+Version: 0.2.4
 Summary: automl_tools
 Home-page: https://github.com/jonaqp/automl_tools
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/automl_tools/archive/main.zip
 Keywords: automl
```

### Comparing `automl_tools-0.2.2/README.md` & `automl_tools-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/automl_tools/functions/imputation.py` & `automl_tools-0.2.4/automl_tools/functions/imputation.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/automl_tools/functions/logger.py` & `automl_tools-0.2.4/automl_tools/functions/logger.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/automl_tools/functions/main.py` & `automl_tools-0.2.4/automl_tools/functions/main.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/automl_tools/functions/modeling.py` & `automl_tools-0.2.4/automl_tools/functions/modeling.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/automl_tools/functions/optimization_binary.py` & `automl_tools-0.2.4/automl_tools/functions/optimization_binary.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/automl_tools/functions/optimization_multi_class.py` & `automl_tools-0.2.4/automl_tools/functions/optimization_multi_class.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/automl_tools/functions/optimization_regression.py` & `automl_tools-0.2.4/automl_tools/functions/optimization_regression.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/automl_tools/functions/parameter.py` & `automl_tools-0.2.4/automl_tools/functions/parameter.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/automl_tools/functions/prepare.py` & `automl_tools-0.2.4/automl_tools/functions/prepare.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/automl_tools/functions/processing.py` & `automl_tools-0.2.4/automl_tools/functions/processing.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/automl_tools/functions/selection.py` & `automl_tools-0.2.4/automl_tools/functions/selection.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/automl_tools/functions/utils.py` & `automl_tools-0.2.4/automl_tools/functions/utils.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.2/automl_tools.egg-info/PKG-INFO` & `automl_tools-0.2.4/automl_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automl-tools
-Version: 0.2.2
+Version: 0.2.4
 Summary: automl_tools
 Home-page: https://github.com/jonaqp/automl_tools
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/automl_tools/archive/main.zip
 Keywords: automl
```

### Comparing `automl_tools-0.2.2/automl_tools.egg-info/SOURCES.txt` & `automl_tools-0.2.4/automl_tools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 automl_tools/__init__.py
 automl_tools.egg-info/PKG-INFO
 automl_tools.egg-info/SOURCES.txt
```

### Comparing `automl_tools-0.2.2/setup.py` & `automl_tools-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='automl_tools',
     packages=find_packages(),
-    version='0.2.2',
+    version='0.2.4',
     description='automl_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/automl_tools',
     download_url='https://github.com/jonaqp/automl_tools/archive/main.zip',
```

