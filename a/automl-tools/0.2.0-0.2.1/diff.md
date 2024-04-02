# Comparing `tmp/automl_tools-0.2.0.tar.gz` & `tmp/automl_tools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automl_tools-0.2.0.tar", last modified: Tue Apr  2 05:24:58 2024, max compression
+gzip compressed data, was "automl_tools-0.2.1.tar", last modified: Tue Apr  2 05:38:25 2024, max compression
```

## Comparing `automl_tools-0.2.0.tar` & `automl_tools-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 05:24:58.552757 automl_tools-0.2.0/
--rw-rw-rw-   0        0        0     1092 2024-04-02 05:07:53.000000 automl_tools-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     4379 2024-04-02 05:24:58.552757 automl_tools-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3653 2024-04-02 05:07:53.000000 automl_tools-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 05:24:58.537130 automl_tools-0.2.0/automl_tools/
--rw-rw-rw-   0        0        0       71 2024-04-02 05:21:14.000000 automl_tools-0.2.0/automl_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 05:24:58.552757 automl_tools-0.2.0/automl_tools/functions/
--rw-rw-rw-   0        0        0        0 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    10171 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/imputation.py
--rw-rw-rw-   0        0        0     4684 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/logger.py
--rw-rw-rw-   0        0        0     5060 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/modeling.py
--rw-rw-rw-   0        0        0     7806 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/optimization_binary.py
--rw-rw-rw-   0        0        0     7892 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/optimization_multi_class.py
--rw-rw-rw-   0        0        0     7617 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/optimization_regression.py
--rw-rw-rw-   0        0        0     1091 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/parameter.py
--rw-rw-rw-   0        0        0     2794 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/prepare.py
--rw-rw-rw-   0        0        0     8153 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/processing.py
--rw-rw-rw-   0        0        0     6851 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/selection.py
--rw-rw-rw-   0        0        0     9909 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/functions/utils.py
--rw-rw-rw-   0        0        0     8043 2024-04-02 05:07:53.000000 automl_tools-0.2.0/automl_tools/main.py
-drwxrwxrwx   0        0        0        0 2024-04-02 05:24:58.552757 automl_tools-0.2.0/automl_tools.egg-info/
--rw-rw-rw-   0        0        0     4379 2024-04-02 05:24:58.000000 automl_tools-0.2.0/automl_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      738 2024-04-02 05:24:58.000000 automl_tools-0.2.0/automl_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 05:24:58.000000 automl_tools-0.2.0/automl_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      253 2024-04-02 05:24:58.000000 automl_tools-0.2.0/automl_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-02 05:24:58.000000 automl_tools-0.2.0/automl_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      689 2024-04-02 05:24:11.000000 automl_tools-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-04-02 05:24:58.568383 automl_tools-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1128 2024-04-02 05:22:07.000000 automl_tools-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 05:38:25.947249 automl_tools-0.2.1/
+-rw-rw-rw-   0        0        0     1092 2024-04-02 05:07:53.000000 automl_tools-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4379 2024-04-02 05:38:25.947249 automl_tools-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3653 2024-04-02 05:07:53.000000 automl_tools-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 05:38:25.913859 automl_tools-0.2.1/automl_tools/
+-rw-rw-rw-   0        0        0       71 2024-04-02 05:21:14.000000 automl_tools-0.2.1/automl_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 05:38:25.947249 automl_tools-0.2.1/automl_tools/functions/
+-rw-rw-rw-   0        0        0        0 2024-04-02 05:07:53.000000 automl_tools-0.2.1/automl_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    10171 2024-04-02 05:07:53.000000 automl_tools-0.2.1/automl_tools/functions/imputation.py
+-rw-rw-rw-   0        0        0     4684 2024-04-02 05:07:53.000000 automl_tools-0.2.1/automl_tools/functions/logger.py
+-rw-rw-rw-   0        0        0     5060 2024-04-02 05:07:53.000000 automl_tools-0.2.1/automl_tools/functions/modeling.py
+-rw-rw-rw-   0        0        0     7806 2024-04-02 05:07:53.000000 automl_tools-0.2.1/automl_tools/functions/optimization_binary.py
+-rw-rw-rw-   0        0        0     7892 2024-04-02 05:07:53.000000 automl_tools-0.2.1/automl_tools/functions/optimization_multi_class.py
+-rw-rw-rw-   0        0        0     7617 2024-04-02 05:07:53.000000 automl_tools-0.2.1/automl_tools/functions/optimization_regression.py
+-rw-rw-rw-   0        0        0     1091 2024-04-02 05:07:53.000000 automl_tools-0.2.1/automl_tools/functions/parameter.py
+-rw-rw-rw-   0        0        0     2794 2024-04-02 05:07:53.000000 automl_tools-0.2.1/automl_tools/functions/prepare.py
+-rw-rw-rw-   0        0        0     8153 2024-04-02 05:07:53.000000 automl_tools-0.2.1/automl_tools/functions/processing.py
+-rw-rw-rw-   0        0        0     6851 2024-04-02 05:07:53.000000 automl_tools-0.2.1/automl_tools/functions/selection.py
+-rw-rw-rw-   0        0        0     9909 2024-04-02 05:07:53.000000 automl_tools-0.2.1/automl_tools/functions/utils.py
+-rw-rw-rw-   0        0        0     8043 2024-04-02 05:07:53.000000 automl_tools-0.2.1/automl_tools/main.py
+drwxrwxrwx   0        0        0        0 2024-04-02 05:38:25.930523 automl_tools-0.2.1/automl_tools.egg-info/
+-rw-rw-rw-   0        0        0     4379 2024-04-02 05:38:25.000000 automl_tools-0.2.1/automl_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2024-04-02 05:38:25.000000 automl_tools-0.2.1/automl_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 05:38:25.000000 automl_tools-0.2.1/automl_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      301 2024-04-02 05:38:25.000000 automl_tools-0.2.1/automl_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-02 05:38:25.000000 automl_tools-0.2.1/automl_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      731 2024-04-02 05:34:42.000000 automl_tools-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-04-02 05:38:25.947249 automl_tools-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2024-04-02 05:38:24.000000 automl_tools-0.2.1/setup.py
```

### Comparing `automl_tools-0.2.0/LICENSE` & `automl_tools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/PKG-INFO` & `automl_tools-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automl_tools
-Version: 0.2.0
+Version: 0.2.1
 Summary: automl_tools
 Home-page: https://github.com/jonaqp/automl_tools
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/automl_tools/archive/main.zip
 Keywords: automl
```

### Comparing `automl_tools-0.2.0/README.md` & `automl_tools-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/automl_tools/functions/imputation.py` & `automl_tools-0.2.1/automl_tools/functions/imputation.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/automl_tools/functions/logger.py` & `automl_tools-0.2.1/automl_tools/functions/logger.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/automl_tools/functions/modeling.py` & `automl_tools-0.2.1/automl_tools/functions/modeling.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/automl_tools/functions/optimization_binary.py` & `automl_tools-0.2.1/automl_tools/functions/optimization_binary.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/automl_tools/functions/optimization_multi_class.py` & `automl_tools-0.2.1/automl_tools/functions/optimization_multi_class.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/automl_tools/functions/optimization_regression.py` & `automl_tools-0.2.1/automl_tools/functions/optimization_regression.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/automl_tools/functions/parameter.py` & `automl_tools-0.2.1/automl_tools/functions/parameter.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/automl_tools/functions/prepare.py` & `automl_tools-0.2.1/automl_tools/functions/prepare.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/automl_tools/functions/processing.py` & `automl_tools-0.2.1/automl_tools/functions/processing.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/automl_tools/functions/selection.py` & `automl_tools-0.2.1/automl_tools/functions/selection.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/automl_tools/functions/utils.py` & `automl_tools-0.2.1/automl_tools/functions/utils.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/automl_tools/main.py` & `automl_tools-0.2.1/automl_tools/main.py`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/automl_tools.egg-info/PKG-INFO` & `automl_tools-0.2.1/automl_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automl-tools
-Version: 0.2.0
+Version: 0.2.1
 Summary: automl_tools
 Home-page: https://github.com/jonaqp/automl_tools
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/automl_tools/archive/main.zip
 Keywords: automl
```

### Comparing `automl_tools-0.2.0/automl_tools.egg-info/SOURCES.txt` & `automl_tools-0.2.1/automl_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automl_tools-0.2.0/pyproject.toml` & `automl_tools-0.2.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -19,16 +19,18 @@
 seaborn = "^0.13.2"
 colorama = "^0.4.6"
 tabulate = "^0.9.0"
 certifi = "^2024.2.2"
 pandas = "^2.2.1"
 wheel = "0.40"
 setuptools = "58.2.0"
+scikit-learn = "1.2.2"
 
 
 
 [tool.poetry.group.dev.dependencies]
+twine = "^5.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `automl_tools-0.2.0/setup.py` & `automl_tools-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='automl_tools',
     packages=find_packages(),
-    version='0.2.0',
+    version='0.2.1',
     description='automl_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/automl_tools',
     download_url='https://github.com/jonaqp/automl_tools/archive/main.zip',
```

