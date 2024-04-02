# Comparing `tmp/csv2database-0.0.4.tar.gz` & `tmp/csv2database-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv2database-0.0.4.tar", last modified: Sun Mar 31 22:40:55 2024, max compression
+gzip compressed data, was "csv2database-0.0.5.tar", last modified: Tue Apr  2 09:32:54 2024, max compression
```

## Comparing `csv2database-0.0.4.tar` & `csv2database-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 22:40:55.484615 csv2database-0.0.4/
--rw-rw-rw-   0        0        0     1094 2024-03-31 20:09:12.000000 csv2database-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      741 2024-03-31 22:40:55.482641 csv2database-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-31 22:40:55.485592 csv2database-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1113 2024-03-31 22:40:39.000000 csv2database-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 22:40:55.436061 csv2database-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-03-31 22:40:55.479925 csv2database-0.0.4/src/csv2database.egg-info/
--rw-rw-rw-   0        0        0      741 2024-03-31 22:40:55.000000 csv2database-0.0.4/src/csv2database.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-03-31 22:40:55.000000 csv2database-0.0.4/src/csv2database.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 22:40:55.000000 csv2database-0.0.4/src/csv2database.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-03-31 22:40:55.000000 csv2database-0.0.4/src/csv2database.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       89 2024-03-31 22:40:55.000000 csv2database-0.0.4/src/csv2database.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 22:40:55.000000 csv2database-0.0.4/src/csv2database.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 09:32:54.088657 csv2database-0.0.5/
+-rw-rw-rw-   0        0        0     1094 2024-03-31 20:09:12.000000 csv2database-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      741 2024-04-02 09:32:53.999909 csv2database-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-02 09:32:54.089656 csv2database-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2024-04-02 09:31:02.000000 csv2database-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 09:32:53.970256 csv2database-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 09:32:53.998691 csv2database-0.0.5/src/csv2database.egg-info/
+-rw-rw-rw-   0        0        0      741 2024-04-02 09:32:53.000000 csv2database-0.0.5/src/csv2database.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-04-02 09:32:53.000000 csv2database-0.0.5/src/csv2database.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 09:32:53.000000 csv2database-0.0.5/src/csv2database.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-02 09:32:53.000000 csv2database-0.0.5/src/csv2database.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2024-04-02 09:32:53.000000 csv2database-0.0.5/src/csv2database.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 09:32:53.000000 csv2database-0.0.5/src/csv2database.egg-info/top_level.txt
```

### Comparing `csv2database-0.0.4/LICENSE.txt` & `csv2database-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `csv2database-0.0.4/PKG-INFO` & `csv2database-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv2database
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for importing CSV files into a MySQL database
 Home-page: https://github.com/mdarfaanbaig/csv2database
 Author: Md Arfaan Baig
 Author-email: mdarfaanbaig@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `csv2database-0.0.4/setup.py` & `csv2database-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='csv2database',
-    version='0.0.4',
+    version='0.0.5',
     author='Md Arfaan Baig',
     author_email='mdarfaanbaig@gmail.com',
     description='A package for importing CSV files into a MySQL database',
     long_description='This package provides functionality to import CSV files into a MySQL database, supporting both local and Google Drive sources.',
     url='https://github.com/mdarfaanbaig/csv2database',
     license='MIT',
     package_dir={'': 'src'},  # Source code directory
```

### Comparing `csv2database-0.0.4/src/csv2database.egg-info/PKG-INFO` & `csv2database-0.0.5/src/csv2database.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv2database
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for importing CSV files into a MySQL database
 Home-page: https://github.com/mdarfaanbaig/csv2database
 Author: Md Arfaan Baig
 Author-email: mdarfaanbaig@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

