# Comparing `tmp/spark_dql_tools-0.7.1.tar.gz` & `tmp/spark_dql_tools-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_dql_tools-0.7.1.tar", last modified: Sun Mar 24 18:26:05 2024, max compression
+gzip compressed data, was "spark_dql_tools-0.7.2.tar", last modified: Tue Apr  2 00:03:03 2024, max compression
```

## Comparing `spark_dql_tools-0.7.1.tar` & `spark_dql_tools-0.7.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 18:26:05.133229 spark_dql_tools-0.7.1/
--rw-rw-rw-   0        0        0     1092 2023-09-08 22:42:23.000000 spark_dql_tools-0.7.1/LICENSE
--rw-rw-rw-   0        0        0       44 2024-03-24 18:25:54.000000 spark_dql_tools-0.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2825 2024-03-24 18:26:05.133229 spark_dql_tools-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     2048 2023-09-08 22:42:23.000000 spark_dql_tools-0.7.1/README.md
--rw-rw-rw-   0        0        0      469 2024-02-20 18:04:13.000000 spark_dql_tools-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-03-24 18:26:05.134328 spark_dql_tools-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1194 2024-03-24 18:25:23.000000 spark_dql_tools-0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-24 18:26:05.100048 spark_dql_tools-0.7.1/spark_dql_tools/
--rw-rw-rw-   0        0        0     1078 2024-03-13 10:02:10.000000 spark_dql_tools-0.7.1/spark_dql_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-24 18:26:05.122227 spark_dql_tools-0.7.1/spark_dql_tools/functions/
--rw-rw-rw-   0        0        0        0 2023-09-08 22:42:23.000000 spark_dql_tools-0.7.1/spark_dql_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    79446 2024-03-24 13:11:49.000000 spark_dql_tools-0.7.1/spark_dql_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2024-03-24 18:26:05.132229 spark_dql_tools-0.7.1/spark_dql_tools/utils/
--rw-rw-rw-   0        0        0       75 2023-09-08 22:42:23.000000 spark_dql_tools-0.7.1/spark_dql_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      501 2023-09-08 22:42:23.000000 spark_dql_tools-0.7.1/spark_dql_tools/utils/utilitty.py
-drwxrwxrwx   0        0        0        0 2024-03-24 18:26:05.121227 spark_dql_tools-0.7.1/spark_dql_tools.egg-info/
--rw-rw-rw-   0        0        0     2825 2024-03-24 18:26:05.000000 spark_dql_tools-0.7.1/spark_dql_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2024-03-24 18:26:05.000000 spark_dql_tools-0.7.1/spark_dql_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 18:26:05.000000 spark_dql_tools-0.7.1/spark_dql_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-03-24 18:26:05.000000 spark_dql_tools-0.7.1/spark_dql_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-24 18:26:05.000000 spark_dql_tools-0.7.1/spark_dql_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 00:03:03.200400 spark_dql_tools-0.7.2/
+-rw-rw-rw-   0        0        0     1092 2023-09-08 22:42:23.000000 spark_dql_tools-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0       40 2024-04-02 00:03:01.000000 spark_dql_tools-0.7.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2825 2024-04-02 00:03:03.200400 spark_dql_tools-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2048 2023-09-08 22:42:23.000000 spark_dql_tools-0.7.2/README.md
+-rw-rw-rw-   0        0        0      469 2024-02-20 18:04:13.000000 spark_dql_tools-0.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-04-02 00:03:03.200400 spark_dql_tools-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1194 2024-04-02 00:03:01.000000 spark_dql_tools-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:03:03.150357 spark_dql_tools-0.7.2/spark_dql_tools/
+-rw-rw-rw-   0        0        0     1078 2024-03-13 10:02:10.000000 spark_dql_tools-0.7.2/spark_dql_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:03:03.181608 spark_dql_tools-0.7.2/spark_dql_tools/functions/
+-rw-rw-rw-   0        0        0        0 2023-09-08 22:42:23.000000 spark_dql_tools-0.7.2/spark_dql_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    79446 2024-03-24 13:11:49.000000 spark_dql_tools-0.7.2/spark_dql_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:03:03.181608 spark_dql_tools-0.7.2/spark_dql_tools/utils/
+-rw-rw-rw-   0        0        0       75 2023-09-08 22:42:23.000000 spark_dql_tools-0.7.2/spark_dql_tools/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:03:03.200400 spark_dql_tools-0.7.2/spark_dql_tools/utils/resource/
+-rw-rw-rw-   0        0        0    26044 2024-02-22 10:16:01.000000 spark_dql_tools-0.7.2/spark_dql_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0      501 2023-09-08 22:42:23.000000 spark_dql_tools-0.7.2/spark_dql_tools/utils/utilitty.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:03:03.165983 spark_dql_tools-0.7.2/spark_dql_tools.egg-info/
+-rw-rw-rw-   0        0        0     2825 2024-04-02 00:03:03.000000 spark_dql_tools-0.7.2/spark_dql_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2024-04-02 00:03:03.000000 spark_dql_tools-0.7.2/spark_dql_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 00:03:03.000000 spark_dql_tools-0.7.2/spark_dql_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-02 00:03:03.000000 spark_dql_tools-0.7.2/spark_dql_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-02 00:03:03.000000 spark_dql_tools-0.7.2/spark_dql_tools.egg-info/top_level.txt
```

### Comparing `spark_dql_tools-0.7.1/LICENSE` & `spark_dql_tools-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_dql_tools-0.7.1/PKG-INFO` & `spark_dql_tools-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_dql_tools
-Version: 0.7.1
+Version: 0.7.2
 Summary: spark_dql_tools
 Home-page: https://github.com/jonaqp/spark_dql_mvp_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dql_mvp_tools/archive/main.zip
 Keywords: spark,dql,rules,hammurabies,haas,mvp
```

### Comparing `spark_dql_tools-0.7.1/README.md` & `spark_dql_tools-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `spark_dql_tools-0.7.1/setup.py` & `spark_dql_tools-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_dql_tools',
     packages=find_packages(),
-    version='0.7.1',
+    version='0.7.2',
     description='spark_dql_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_dql_mvp_tools/',
     download_url='https://github.com/jonaqp/spark_dql_mvp_tools/archive/main.zip',
```

### Comparing `spark_dql_tools-0.7.1/spark_dql_tools/__init__.py` & `spark_dql_tools-0.7.2/spark_dql_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_dql_tools-0.7.1/spark_dql_tools/functions/generator.py` & `spark_dql_tools-0.7.2/spark_dql_tools/functions/generator.py`

 * *Files identical despite different names*

### Comparing `spark_dql_tools-0.7.1/spark_dql_tools.egg-info/PKG-INFO` & `spark_dql_tools-0.7.2/spark_dql_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-dql-tools
-Version: 0.7.1
+Version: 0.7.2
 Summary: spark_dql_tools
 Home-page: https://github.com/jonaqp/spark_dql_mvp_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dql_mvp_tools/archive/main.zip
 Keywords: spark,dql,rules,hammurabies,haas,mvp
```

