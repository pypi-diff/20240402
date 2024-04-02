# Comparing `tmp/cit-pydata-0.0.1.dev0.tar.gz` & `tmp/cit-pydata-0.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cit-pydata/cit-pydata/dist/.tmp-u8g1c4r6/cit-pydata-0.0.1.dev0.tar", last modified: Tue Mar 26 14:01:47 2024, max compression
+gzip compressed data, was "/home/runner/work/cit-pydata/cit-pydata/dist/.tmp-wnk4i6t7/cit-pydata-0.0.1.dev1.tar", last modified: Tue Apr  2 19:11:51 2024, max compression
```

## Comparing `cit-pydata-0.0.1.dev0.tar` & `cit-pydata-0.0.1.dev1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/aws/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/aws/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/box/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/box/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/box/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/joblog/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/joblog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/joblog/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/marketo/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/marketo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/marketo/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/salesforce/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/salesforce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21390 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/salesforce/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/sfsync/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/sfsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/sfsync/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/sftp/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/sftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/sftp/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36075 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/sql/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/util/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-03-26 14:01:41.000000 cit-pydata-0.0.1.dev0/src/cit_pydata/util/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-26 14:01:47.000000 cit-pydata-0.0.1.dev0/src/cit_pydata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/aws/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/box/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/box/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/box/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/joblog/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/joblog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/joblog/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/marketo/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/marketo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/marketo/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/salesforce/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/salesforce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21390 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/salesforce/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sfsync/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sfsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sfsync/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sftp/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sftp/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36075 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sql/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/util/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/top_level.txt
```

### Comparing `cit-pydata-0.0.1.dev0/LICENSE` & `cit-pydata-0.0.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev0/PKG-INFO` & `cit-pydata-0.0.1.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cit-pydata
-Version: 0.0.1.dev0
+Version: 0.0.1.dev1
 Summary: Python clients for commonly used api services including Salesforce, SQL, Marketo, Box, SFSync*, and JobLog*
 Author-email: Dionis Wang <dwang@eab.com>
 Project-URL: Homepage, https://github.com/EAB-IT-DEV/cit-pydata
 Project-URL: Issues, https://github.com/EAB-IT-DEV/cit-pydata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cit-pydata-0.0.1.dev0/pyproject.toml` & `cit-pydata-0.0.1.dev1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cit-pydata"
-version = "0.0.1.dev0"
+version = "0.0.1.dev1"
 authors = [
   { name="Dionis Wang", email="dwang@eab.com" },
 ]
 description = "Python clients for commonly used api services including Salesforce, SQL, Marketo, Box, SFSync*, and JobLog*"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -22,15 +22,15 @@
 
 [project.optional-dependencies]
 aws = ["aws-lambda-powertools"]
 box = ["boxsdk"]
 joblog = ["marketorestpython"]
 salesforce = ["simple_salesforce","pyforce"]
 sftp = ["paramiko"]
-sql = ["SQLAlchemy==1.4.25", "numpy", "pandas"]
-sql-pyodbc = ["SQLAlchemy==1.4.25", "pyodbc", "numpy", "pandas"]
-sql-pymssql = ["SQLAlchemy==1.4.25", "pymssql", "numpy", "pandas"]
-sql-psycopg2 = ["SQLAlchemy==1.4.25", "psycopg2-binary==2.9.6", "numpy", "pandas"]
-sql-mssql = ["SQLAlchemy==1.4.25", "pymssql", "numpy", "pandas"]
-sql-postgres = ["SQLAlchemy==1.4.25", "psycopg2-binary==2.9.6", "numpy", "pandas"]
+sql = ["SQLAlchemy<2.0", "numpy", "pandas"]
+sql-pyodbc = ["SQLAlchemy<2.0", "pyodbc", "numpy", "pandas"]
+sql-pymssql = ["SQLAlchemy<2.0", "pymssql", "numpy", "pandas"]
+sql-psycopg2 = ["SQLAlchemy<2.0", "psycopg2-binary", "numpy", "pandas"]
+sql-mssql = ["SQLAlchemy<2.0", "pymssql", "numpy", "pandas"]
+sql-postgres = ["SQLAlchemy<2.0", "psycopg2-binary", "numpy", "pandas"]
 local = ["python-dotenv", "boto3"]
-all = ["aws-lambda-powertools","pandas","boxsdk","marketorestpython","simple_salesforce","pyforce","paramiko","SQLAlchemy==1.4.25", "pyodbc","pymssql", "numpy", "pandas","psycopg2-binary==2.9.6","python-dotenv", "boto3"]
+all = ["aws-lambda-powertools","pandas","boxsdk","marketorestpython","simple_salesforce","pyforce","paramiko","SQLAlchemy<2.0", "pyodbc","pymssql", "numpy", "pandas","psycopg2-binary","python-dotenv", "boto3"]
```

### Comparing `cit-pydata-0.0.1.dev0/src/cit_pydata/aws/api.py` & `cit-pydata-0.0.1.dev1/src/cit_pydata/aws/api.py`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev0/src/cit_pydata/box/api.py` & `cit-pydata-0.0.1.dev1/src/cit_pydata/box/api.py`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev0/src/cit_pydata/joblog/api.py` & `cit-pydata-0.0.1.dev1/src/cit_pydata/joblog/api.py`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev0/src/cit_pydata/marketo/api.py` & `cit-pydata-0.0.1.dev1/src/cit_pydata/marketo/api.py`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev0/src/cit_pydata/salesforce/api.py` & `cit-pydata-0.0.1.dev1/src/cit_pydata/salesforce/api.py`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev0/src/cit_pydata/sfsync/api.py` & `cit-pydata-0.0.1.dev1/src/cit_pydata/sfsync/api.py`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev0/src/cit_pydata/sftp/api.py` & `cit-pydata-0.0.1.dev1/src/cit_pydata/sftp/api.py`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev0/src/cit_pydata/sql/api.py` & `cit-pydata-0.0.1.dev1/src/cit_pydata/sql/api.py`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev0/src/cit_pydata/util/api.py` & `cit-pydata-0.0.1.dev1/src/cit_pydata/util/api.py`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev0/src/cit_pydata.egg-info/PKG-INFO` & `cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cit-pydata
-Version: 0.0.1.dev0
+Version: 0.0.1.dev1
 Summary: Python clients for commonly used api services including Salesforce, SQL, Marketo, Box, SFSync*, and JobLog*
 Author-email: Dionis Wang <dwang@eab.com>
 Project-URL: Homepage, https://github.com/EAB-IT-DEV/cit-pydata
 Project-URL: Issues, https://github.com/EAB-IT-DEV/cit-pydata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cit-pydata-0.0.1.dev0/src/cit_pydata.egg-info/SOURCES.txt` & `cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

