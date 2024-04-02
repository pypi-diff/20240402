# Comparing `tmp/astro_extras-0.0.4.tar.gz` & `tmp/astro_extras-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_extras-0.0.4.tar", last modified: Mon Mar 11 14:33:09 2024, max compression
+gzip compressed data, was "astro_extras-0.0.5.tar", last modified: Tue Apr  2 08:24:42 2024, max compression
```

## Comparing `astro_extras-0.0.4.tar` & `astro_extras-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-03-11 14:33:09.675922 astro_extras-0.0.4/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.0.4/LICENSE
--rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.0.4/MANIFEST.in
--rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-03-11 14:33:09.675922 astro_extras-0.0.4/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.0.4/README.md
--rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.0.4/pyproject.toml
--rw-rw-r--   0 kol       (1000) kol       (1000)      260 2024-03-11 13:15:33.000000 astro_extras-0.0.4/requirements.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-03-11 14:33:09.675922 astro_extras-0.0.4/setup.cfg
--rw-rw-r--   0 kol       (1000) kol       (1000)     1085 2024-03-11 14:32:56.000000 astro_extras-0.0.4/setup.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-03-11 14:33:09.671922 astro_extras-0.0.4/src/
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-03-11 14:33:09.671922 astro_extras-0.0.4/src/astro_extras/
--rw-rw-r--   0 kol       (1000) kol       (1000)      940 2024-03-11 13:27:59.000000 astro_extras-0.0.4/src/astro_extras/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-03-11 14:33:09.671922 astro_extras-0.0.4/src/astro_extras/hooks/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.4/src/astro_extras/hooks/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-03-11 14:33:09.675922 astro_extras-0.0.4/src/astro_extras/operators/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.4/src/astro_extras/operators/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3880 2023-10-26 14:10:20.000000 astro_extras-0.0.4/src/astro_extras/operators/direct.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    18057 2023-11-20 09:48:16.000000 astro_extras-0.0.4/src/astro_extras/operators/session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    22741 2024-03-11 14:32:23.000000 astro_extras-0.0.4/src/astro_extras/operators/table.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-03-11 14:33:09.675922 astro_extras-0.0.4/src/astro_extras/utils/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.4/src/astro_extras/utils/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    10549 2023-11-17 15:24:02.000000 astro_extras-0.0.4/src/astro_extras/utils/data_compare.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.0.4/src/astro_extras/utils/datetime_local.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5378 2024-03-11 14:28:15.000000 astro_extras-0.0.4/src/astro_extras/utils/template.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1946 2024-03-11 14:32:38.000000 astro_extras-0.0.4/src/astro_extras/utils/utils.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-03-11 14:33:09.675922 astro_extras-0.0.4/src/astro_extras.egg-info/
--rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-03-11 14:33:09.000000 astro_extras-0.0.4/src/astro_extras.egg-info/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)      751 2024-03-11 14:33:09.000000 astro_extras-0.0.4/src/astro_extras.egg-info/SOURCES.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-03-11 14:33:09.000000 astro_extras-0.0.4/src/astro_extras.egg-info/dependency_links.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)      112 2024-03-11 14:33:09.000000 astro_extras-0.0.4/src/astro_extras.egg-info/requires.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-03-11 14:33:09.000000 astro_extras-0.0.4/src/astro_extras.egg-info/top_level.txt
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-03-11 14:33:09.675922 astro_extras-0.0.4/tests/
--rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.0.4/tests/test_session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     6158 2023-11-17 10:36:18.000000 astro_extras-0.0.4/tests/test_table.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.0.4/tests/test_templates.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-03-11 14:20:58.000000 astro_extras-0.0.4/tests/test_utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.248114 astro_extras-0.0.5/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.0.5/LICENSE
+-rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.0.5/MANIFEST.in
+-rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-02 08:24:42.248114 astro_extras-0.0.5/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.0.5/README.md
+-rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.0.5/pyproject.toml
+-rw-rw-r--   0 kol       (1000) kol       (1000)      260 2024-03-11 13:15:33.000000 astro_extras-0.0.5/requirements.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-04-02 08:24:42.248114 astro_extras-0.0.5/setup.cfg
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1085 2024-04-02 07:11:17.000000 astro_extras-0.0.5/setup.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.236114 astro_extras-0.0.5/src/
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.236114 astro_extras-0.0.5/src/astro_extras/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1000 2024-04-02 07:23:04.000000 astro_extras-0.0.5/src/astro_extras/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.244114 astro_extras-0.0.5/src/astro_extras/hooks/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.5/src/astro_extras/hooks/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.244114 astro_extras-0.0.5/src/astro_extras/operators/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.5/src/astro_extras/operators/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3880 2023-10-26 14:10:20.000000 astro_extras-0.0.5/src/astro_extras/operators/direct.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    18057 2023-11-20 09:48:16.000000 astro_extras-0.0.5/src/astro_extras/operators/session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    22741 2024-03-11 14:32:23.000000 astro_extras-0.0.5/src/astro_extras/operators/table.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.248114 astro_extras-0.0.5/src/astro_extras/utils/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.5/src/astro_extras/utils/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    10549 2023-11-17 15:24:02.000000 astro_extras-0.0.5/src/astro_extras/utils/data_compare.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.0.5/src/astro_extras/utils/datetime_local.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5378 2024-03-11 14:28:15.000000 astro_extras-0.0.5/src/astro_extras/utils/template.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1952 2024-03-28 14:14:29.000000 astro_extras-0.0.5/src/astro_extras/utils/utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.248114 astro_extras-0.0.5/src/astro_extras.egg-info/
+-rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-02 08:24:42.000000 astro_extras-0.0.5/src/astro_extras.egg-info/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)      751 2024-04-02 08:24:42.000000 astro_extras-0.0.5/src/astro_extras.egg-info/SOURCES.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-04-02 08:24:42.000000 astro_extras-0.0.5/src/astro_extras.egg-info/dependency_links.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)      112 2024-04-02 08:24:42.000000 astro_extras-0.0.5/src/astro_extras.egg-info/requires.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-04-02 08:24:42.000000 astro_extras-0.0.5/src/astro_extras.egg-info/top_level.txt
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.248114 astro_extras-0.0.5/tests/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.0.5/tests/test_session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     6158 2023-11-17 10:36:18.000000 astro_extras-0.0.5/tests/test_table.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.0.5/tests/test_templates.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-03-11 14:20:58.000000 astro_extras-0.0.5/tests/test_utils.py
```

### Comparing `astro_extras-0.0.4/LICENSE` & `astro_extras-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.4/PKG-INFO` & `astro_extras-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.0.4
+Version: 0.0.5
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.0.4/README.md` & `astro_extras-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.4/setup.py` & `astro_extras-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.readlines()
 
 setuptools.setup(
     name="astro_extras",
-    version="0.0.4",
+    version="0.0.5",
     author="Kol",
     author_email="skolchin@gmail.com",
     description="Additional Astro SDK operators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/skolchin/astro-extras",
     classifiers=[
```

### Comparing `astro_extras-0.0.4/src/astro_extras/__init__.py` & `astro_extras-0.0.5/src/astro_extras/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Astro SDK Extras project
-# (c) kol, 2023
+# (c) kol, 2023-2024
 
-__version__ = '0.0.2'
+__version__ = '0.0.5'
 
 from .operators.session import (
     open_session, 
     close_session,
     ETLSession,
     get_current_session,
     get_session_period,
@@ -20,14 +20,17 @@
     update_timed_table, 
     update_timed_tables,
 )
 from .operators.direct import (
     run_sql_template,
     run_sql_templates,
 )
+from .sensors.file import (
+    FileChangedSensor
+)
 from .utils.template import (
     get_template_file,
     get_template,
 )
 from .utils.utils import (
     split_table_name,
     ensure_table,
```

### Comparing `astro_extras-0.0.4/src/astro_extras/operators/direct.py` & `astro_extras-0.0.5/src/astro_extras/operators/direct.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.4/src/astro_extras/operators/session.py` & `astro_extras-0.0.5/src/astro_extras/operators/session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.4/src/astro_extras/operators/table.py` & `astro_extras-0.0.5/src/astro_extras/operators/table.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.4/src/astro_extras/utils/data_compare.py` & `astro_extras-0.0.5/src/astro_extras/utils/data_compare.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.4/src/astro_extras/utils/datetime_local.py` & `astro_extras-0.0.5/src/astro_extras/utils/datetime_local.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.4/src/astro_extras/utils/template.py` & `astro_extras-0.0.5/src/astro_extras/utils/template.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.4/src/astro_extras/utils/utils.py` & `astro_extras-0.0.5/src/astro_extras/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     if table is None:
         return None
     if isinstance(table, BaseTable):
         return table
     if isinstance(table, str):
         schema_from_name, table = split_table_name(table)
         return Table(table, conn_id=conn_id, metadata=Metadata(schema=schema_from_name or schema, database=database))
+    
     raise TypeError(f'Either str or BaseTable expected, {table.__class__.__name__} found')
 
 def schedule_ops(ops_list: List[BaseOperator], num_parallel: int = 1) -> List[BaseOperator]:
     """ Build parallel operator chains. Returns list of last operators in each chain. """
 
     if not ops_list:
         raise ValueError('Empty list')
```

### Comparing `astro_extras-0.0.4/src/astro_extras.egg-info/PKG-INFO` & `astro_extras-0.0.5/src/astro_extras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.0.4
+Version: 0.0.5
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.0.4/src/astro_extras.egg-info/SOURCES.txt` & `astro_extras-0.0.5/src/astro_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.4/tests/test_session.py` & `astro_extras-0.0.5/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.4/tests/test_table.py` & `astro_extras-0.0.5/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.4/tests/test_templates.py` & `astro_extras-0.0.5/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.4/tests/test_utils.py` & `astro_extras-0.0.5/tests/test_utils.py`

 * *Files identical despite different names*

