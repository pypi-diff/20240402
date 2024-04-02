# Comparing `tmp/dbt-starrocks-1.4.2.tar.gz` & `tmp/dbt-starrocks-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-starrocks-1.4.2.tar", last modified: Mon Jan 15 02:46:18 2024, max compression
+gzip compressed data, was "dbt-starrocks-1.6.1.tar", last modified: Wed Mar 20 03:24:03 2024, max compression
```

## Comparing `dbt-starrocks-1.4.2.tar` & `dbt-starrocks-1.6.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-01-15 02:46:18.397738 dbt-starrocks-1.4.2/
--rw-r--r--   0 lixueyan   (501) staff       (20)      656 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/MANIFEST.in
--rw-r--r--   0 lixueyan   (501) staff       (20)     7560 2024-01-15 02:46:18.396955 dbt-starrocks-1.4.2/PKG-INFO
--rw-r--r--   0 lixueyan   (501) staff       (20)     6599 2024-01-15 02:46:05.000000 dbt-starrocks-1.4.2/README.md
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-01-15 02:46:18.363964 dbt-starrocks-1.4.2/dbt/
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-01-15 02:46:18.363756 dbt-starrocks-1.4.2/dbt/adapters/
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-01-15 02:46:18.371949 dbt-starrocks-1.4.2/dbt/adapters/starrocks/
--rw-r--r--   0 lixueyan   (501) staff       (20)      968 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/adapters/starrocks/__init__.py
--rw-r--r--   0 lixueyan   (501) staff       (20)      647 2024-01-12 05:46:10.000000 dbt-starrocks-1.4.2/dbt/adapters/starrocks/__version__.py
--rw-r--r--   0 lixueyan   (501) staff       (20)     1898 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/adapters/starrocks/column.py
--rw-r--r--   0 lixueyan   (501) staff       (20)     6663 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/adapters/starrocks/connections.py
--rw-r--r--   0 lixueyan   (501) staff       (20)     7187 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/adapters/starrocks/impl.py
--rw-r--r--   0 lixueyan   (501) staff       (20)     2950 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/adapters/starrocks/relation.py
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-01-15 02:46:18.364110 dbt-starrocks-1.4.2/dbt/include/
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-01-15 02:46:18.375343 dbt-starrocks-1.4.2/dbt/include/starrocks/
--rw-r--r--   0 lixueyan   (501) staff       (20)      680 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/__init__.py
--rw-r--r--   0 lixueyan   (501) staff       (20)      687 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/dbt_project.yml
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-01-15 02:46:18.364833 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-01-15 02:46:18.380951 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/adapters/
--rw-r--r--   0 lixueyan   (501) staff       (20)     1258 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/adapters/columns.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)      711 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/adapters/freshness.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)     3585 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/adapters/metadata.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)     2054 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/adapters/relation.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)     5197 2024-01-12 08:43:35.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/adapters/relation_helpers.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)      807 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/adapters/schema.sql
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-01-15 02:46:18.381718 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/get_custom_name/
--rw-r--r--   0 lixueyan   (501) staff       (20)      754 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/get_custom_name/get_custom_database.sql
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-01-15 02:46:18.382505 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-01-15 02:46:18.386457 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/models/
--rw-r--r--   0 lixueyan   (501) staff       (20)     2631 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/models/materialized_view.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)     1511 2024-01-15 02:46:05.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/models/table.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)      846 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/models/view.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)     1648 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/seeds.sql
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-01-15 02:46:18.389923 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/snapshot/
--rw-r--r--   0 lixueyan   (501) staff       (20)     5737 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)     1524 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)      857 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/snapshot/strategies.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)      903 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/profile_template.yml
--rw-r--r--   0 lixueyan   (501) staff       (20)      960 2024-01-08 07:20:45.000000 dbt-starrocks-1.4.2/dbt/include/starrocks/sample_profiles.yml
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-01-15 02:46:18.395912 dbt-starrocks-1.4.2/dbt_starrocks.egg-info/
--rw-r--r--   0 lixueyan   (501) staff       (20)     7560 2024-01-15 02:46:18.000000 dbt-starrocks-1.4.2/dbt_starrocks.egg-info/PKG-INFO
--rw-r--r--   0 lixueyan   (501) staff       (20)     1466 2024-01-15 02:46:18.000000 dbt-starrocks-1.4.2/dbt_starrocks.egg-info/SOURCES.txt
--rw-r--r--   0 lixueyan   (501) staff       (20)        1 2024-01-15 02:46:18.000000 dbt-starrocks-1.4.2/dbt_starrocks.egg-info/dependency_links.txt
--rw-r--r--   0 lixueyan   (501) staff       (20)        1 2023-08-14 08:38:03.000000 dbt-starrocks-1.4.2/dbt_starrocks.egg-info/not-zip-safe
--rw-r--r--   0 lixueyan   (501) staff       (20)       44 2024-01-15 02:46:18.000000 dbt-starrocks-1.4.2/dbt_starrocks.egg-info/requires.txt
--rw-r--r--   0 lixueyan   (501) staff       (20)        4 2024-01-15 02:46:18.000000 dbt-starrocks-1.4.2/dbt_starrocks.egg-info/top_level.txt
--rw-r--r--   0 lixueyan   (501) staff       (20)       38 2024-01-15 02:46:18.397953 dbt-starrocks-1.4.2/setup.cfg
--rw-r--r--   0 lixueyan   (501) staff       (20)     2800 2024-01-12 05:46:10.000000 dbt-starrocks-1.4.2/setup.py
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:03.020585 dbt-starrocks-1.6.1/
+-rw-r--r--   0 lixueyan   (501) staff       (20)      656 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/MANIFEST.in
+-rw-r--r--   0 lixueyan   (501) staff       (20)     7594 2024-03-20 03:24:03.018355 dbt-starrocks-1.6.1/PKG-INFO
+-rw-r--r--   0 lixueyan   (501) staff       (20)     6660 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/README.md
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.967088 dbt-starrocks-1.6.1/dbt/
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.966934 dbt-starrocks-1.6.1/dbt/adapters/
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.978448 dbt-starrocks-1.6.1/dbt/adapters/starrocks/
+-rw-r--r--   0 lixueyan   (501) staff       (20)      968 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/adapters/starrocks/__init__.py
+-rw-r--r--   0 lixueyan   (501) staff       (20)      647 2024-03-20 03:18:53.000000 dbt-starrocks-1.6.1/dbt/adapters/starrocks/__version__.py
+-rw-r--r--   0 lixueyan   (501) staff       (20)     1898 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/adapters/starrocks/column.py
+-rw-r--r--   0 lixueyan   (501) staff       (20)     7209 2024-03-20 02:47:04.000000 dbt-starrocks-1.6.1/dbt/adapters/starrocks/connections.py
+-rw-r--r--   0 lixueyan   (501) staff       (20)     6882 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/adapters/starrocks/impl.py
+-rw-r--r--   0 lixueyan   (501) staff       (20)     2966 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/adapters/starrocks/relation.py
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.967200 dbt-starrocks-1.6.1/dbt/include/
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.984760 dbt-starrocks-1.6.1/dbt/include/starrocks/
+-rw-r--r--   0 lixueyan   (501) staff       (20)      680 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/__init__.py
+-rw-r--r--   0 lixueyan   (501) staff       (20)      687 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/dbt_project.yml
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.967840 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.993320 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/
+-rw-r--r--   0 lixueyan   (501) staff       (20)     1258 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/columns.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)      711 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/freshness.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)     3585 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/metadata.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)     2054 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/relation.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)     5197 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/relation_helpers.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)      807 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/schema.sql
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.994487 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/get_custom_name/
+-rw-r--r--   0 lixueyan   (501) staff       (20)      754 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/get_custom_name/get_custom_database.sql
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.995724 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:03.000055 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/
+-rw-r--r--   0 lixueyan   (501) staff       (20)     2631 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/materialized_view.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)     1511 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/table.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)      846 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/view.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)     1648 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/seeds.sql
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:03.004743 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/
+-rw-r--r--   0 lixueyan   (501) staff       (20)     5737 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)     1524 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)      857 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/strategies.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)      994 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/profile_template.yml
+-rw-r--r--   0 lixueyan   (501) staff       (20)      960 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/sample_profiles.yml
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:03.016011 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/
+-rw-r--r--   0 lixueyan   (501) staff       (20)     7594 2024-03-20 03:24:02.000000 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/PKG-INFO
+-rw-r--r--   0 lixueyan   (501) staff       (20)     1466 2024-03-20 03:24:02.000000 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/SOURCES.txt
+-rw-r--r--   0 lixueyan   (501) staff       (20)        1 2024-03-20 03:24:02.000000 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/dependency_links.txt
+-rw-r--r--   0 lixueyan   (501) staff       (20)        1 2024-03-20 03:24:02.000000 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/not-zip-safe
+-rw-r--r--   0 lixueyan   (501) staff       (20)       44 2024-03-20 03:24:02.000000 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/requires.txt
+-rw-r--r--   0 lixueyan   (501) staff       (20)        4 2024-03-20 03:24:02.000000 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/top_level.txt
+-rw-r--r--   0 lixueyan   (501) staff       (20)       38 2024-03-20 03:24:03.020841 dbt-starrocks-1.6.1/setup.cfg
+-rw-r--r--   0 lixueyan   (501) staff       (20)     2773 2024-03-20 03:18:53.000000 dbt-starrocks-1.6.1/setup.py
```

### Comparing `dbt-starrocks-1.4.2/MANIFEST.in` & `dbt-starrocks-1.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/PKG-INFO` & `dbt-starrocks-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: dbt-starrocks
-Version: 1.4.2
+Version: 1.6.1
 Summary: The Starrocks adapter plugin for dbt
-Home-page: https://github.com/StarRocks/starrocks/tree/main/contrib/dbt-connector
+Home-page: https://github.com/StarRocks/dbt-starrocks/
 Author: fujianhj, long2ice, astralidea
 Author-email: fujianhj@gmail.com, long2ice@gmail.com, astralidea@163.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7,<3.12
 Description-Content-Type: text/markdown
-Requires-Dist: dbt-core==1.6.2
+Requires-Dist: dbt-core~=1.6.0
 Requires-Dist: mysql-connector-python>=8.1
 
 # dbt-starrocks
 
 ![PyPI](https://img.shields.io/pypi/v/dbt-starrocks)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dbt-starrocks)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/dbt-starrocks)
@@ -153,11 +153,15 @@
 Finally, you might use below marco quote 
 ```
 {{ source('external_example', 'hive_table_name') }}
 ```
 
 
 ## Test Adapter
+Run the following
+```
+python3 -m pytest tests/functional
+```
 consult [the project](https://github.com/dbt-labs/dbt-adapter-tests)
 
 ## Contributing
 We welcome you to contribute to dbt-starrocks. Please see the [Contributing Guide](https://github.com/StarRocks/starrocks/blob/main/CONTRIBUTING.md) for more information.
```

### Comparing `dbt-starrocks-1.4.2/README.md` & `dbt-starrocks-1.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -131,11 +131,15 @@
 Finally, you might use below marco quote 
 ```
 {{ source('external_example', 'hive_table_name') }}
 ```
 
 
 ## Test Adapter
+Run the following
+```
+python3 -m pytest tests/functional
+```
 consult [the project](https://github.com/dbt-labs/dbt-adapter-tests)
 
 ## Contributing
 We welcome you to contribute to dbt-starrocks. Please see the [Contributing Guide](https://github.com/StarRocks/starrocks/blob/main/CONTRIBUTING.md) for more information.
```

### Comparing `dbt-starrocks-1.4.2/dbt/adapters/starrocks/__init__.py` & `dbt-starrocks-1.6.1/dbt/adapters/starrocks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/adapters/starrocks/__version__.py` & `dbt-starrocks-1.6.1/dbt/adapters/starrocks/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-version = "1.4.2"
+version = "1.6.1"
```

### Comparing `dbt-starrocks-1.4.2/dbt/adapters/starrocks/column.py` & `dbt-starrocks-1.6.1/dbt/adapters/starrocks/column.py`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/adapters/starrocks/connections.py` & `dbt-starrocks-1.6.1/dbt/adapters/starrocks/connections.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     if '-' in result:
         first_part = result.split('-')[0]
     if ' ' in result:
         first_part = result.split(' ')[0]
 
     if first_part and len(first_part.split('.')) == 3:
-        return first_part[0], first_part[1], first_part[2]
+        return int(first_part[0]), int(first_part[2]), int(first_part[4])
 
     return default_version
 
 class StarRocksConnectionManager(SQLConnectionManager):
     TYPE = 'starrocks'
 
     @classmethod
@@ -102,31 +102,43 @@
             logger.debug('Connection is already open, skipping open.')
             return connection
 
         credentials = cls.get_credentials(connection.credentials)
         kwargs = {"host": credentials.host, "username": credentials.username,
                   "password": credentials.password, "database": credentials.catalog + "." + credentials.schema}
 
+        kwargs["buffered"] = True
+        
         if credentials.port:
             kwargs["port"] = credentials.port
 
         try:
             connection.handle = mysql.connector.connect(**kwargs)
             connection.state = 'open'
         except mysql.connector.Error:
 
             try:
                 logger.debug("Failed connection without supplying the `database`. "
                              "Trying again with `database` included.")
 
                 # Try again with the database included
+                database_toBeCreated = kwargs["database"]
                 kwargs["database"] = "information_schema"
 
                 connection.handle = mysql.connector.connect(**kwargs)
                 connection.state = 'open'
+
+                mycursor = connection.handle.cursor()
+
+                mycursor.execute("CREATE DATABASE " + database_toBeCreated)
+                kwargs["database"] = database_toBeCreated;
+
+                connection.handle = mysql.connector.connect(**kwargs)
+                connection.state = 'open'
+
             except mysql.connector.Error as e:
 
                 logger.debug("Got an error when attempting to open a StarRocks "
                              "connection: '{}'".format(e))
 
                 connection.handle = None
                 connection.state = 'fail'
@@ -140,14 +152,16 @@
                 connection.handle.server_version = _parse_version(cursor.fetchone()[0])
             except Exception as e:
                 logger.debug("Got an error when obtain StarRocks version exception: '{}'".format(e))
         else:
             version = credentials.version.strip().split('.')
             if len(version) == 3:
                 connection.handle.server_version = (int(version[0]), int(version[1]), int(version[2]))
+            elif len(version) == 2:
+                connection.handle.server_version = (int(version[0]), int(version[1]), 0)
             else:
                 logger.debug("Config version '{}' is invalid".format(version))
 
         return connection
 
     @classmethod
     def get_credentials(cls, credentials):
```

### Comparing `dbt-starrocks-1.4.2/dbt/adapters/starrocks/impl.py` & `dbt-starrocks-1.6.1/dbt/adapters/starrocks/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,22 +140,17 @@
         return table.where(_catalog_filter_schemas(manifest))
 
     @available
     def is_before_version(self, version: str) -> bool:
         conn = self.connections.get_if_exists()
         if conn:
             server_version = conn.handle.server_version
-            version_detail = version.split(".")
-            version_detail = (int(version_detail[0]), int(version_detail[1]), int(version_detail[2]))
-            if version_detail[0] > server_version[0]:
-                return True
-            elif version_detail[0] == server_version[0] and version_detail[1] > server_version[1]:
-                return True
-            elif version_detail[0] == server_version[0] and version_detail[1] == server_version[1] \
-                    and version_detail[2] > server_version[2]:
+            server_version_tuple = tuple(server_version)
+            version_detail_tuple = tuple(int(part) for part in version.split(".") if part.isdigit())
+            if version_detail_tuple > server_version_tuple:
                 return True
         return False
 
     @available
     def current_version(self):
         conn = self.connections.get_if_exists()
         if conn:
```

### Comparing `dbt-starrocks-1.4.2/dbt/adapters/starrocks/relation.py` & `dbt-starrocks-1.6.1/dbt/adapters/starrocks/relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     identifier: bool = True
 
 class StarRocksRelationType(StrEnum):
     Table = "table"
     View = "view"
     MaterializedView = "materialized_view"
     SystemView = "system_view"
+    CTE = "cte"
     Unknown = "unknown"
 
 @dataclass(frozen=True, eq=False, repr=False)
 class StarRocksRelation(BaseRelation):
     type: Optional[StarRocksRelationType] = None  # type: ignore
     include_policy: StarRocksIncludePolicy = field(default_factory=lambda: StarRocksIncludePolicy())
     quote_policy: StarRocksQuotePolicy = field(default_factory=lambda: StarRocksQuotePolicy())
```

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/__init__.py` & `dbt-starrocks-1.6.1/dbt/include/starrocks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/dbt_project.yml` & `dbt-starrocks-1.6.1/dbt/include/starrocks/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/adapters/columns.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/adapters/freshness.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/adapters/metadata.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/adapters/relation.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/adapters/relation_helpers.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/relation_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/adapters/schema.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/get_custom_name/get_custom_database.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/models/materialized_view.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/models/table.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/models/view.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/seeds.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/seeds.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/snapshot/snapshot.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/macros/materializations/snapshot/strategies.sql` & `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt/include/starrocks/sample_profiles.yml` & `dbt-starrocks-1.6.1/dbt/include/starrocks/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/dbt_starrocks.egg-info/PKG-INFO` & `dbt-starrocks-1.6.1/dbt_starrocks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: dbt-starrocks
-Version: 1.4.2
+Version: 1.6.1
 Summary: The Starrocks adapter plugin for dbt
-Home-page: https://github.com/StarRocks/starrocks/tree/main/contrib/dbt-connector
+Home-page: https://github.com/StarRocks/dbt-starrocks/
 Author: fujianhj, long2ice, astralidea
 Author-email: fujianhj@gmail.com, long2ice@gmail.com, astralidea@163.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7,<3.12
 Description-Content-Type: text/markdown
-Requires-Dist: dbt-core==1.6.2
+Requires-Dist: dbt-core~=1.6.0
 Requires-Dist: mysql-connector-python>=8.1
 
 # dbt-starrocks
 
 ![PyPI](https://img.shields.io/pypi/v/dbt-starrocks)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dbt-starrocks)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/dbt-starrocks)
@@ -153,11 +153,15 @@
 Finally, you might use below marco quote 
 ```
 {{ source('external_example', 'hive_table_name') }}
 ```
 
 
 ## Test Adapter
+Run the following
+```
+python3 -m pytest tests/functional
+```
 consult [the project](https://github.com/dbt-labs/dbt-adapter-tests)
 
 ## Contributing
 We welcome you to contribute to dbt-starrocks. Please see the [Contributing Guide](https://github.com/StarRocks/starrocks/blob/main/CONTRIBUTING.md) for more information.
```

### Comparing `dbt-starrocks-1.4.2/dbt_starrocks.egg-info/SOURCES.txt` & `dbt-starrocks-1.6.1/dbt_starrocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.4.2/setup.py` & `dbt-starrocks-1.6.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,31 +37,31 @@
 # pull long description from README
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 package_name = "dbt-starrocks"
 # make sure this always matches dbt/adapters/starrocks/__version__.py
-package_version = "1.4.2"
+package_version = "1.6.1"
 description = """The Starrocks adapter plugin for dbt"""
 
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="fujianhj, long2ice, astralidea",
     author_email="fujianhj@gmail.com, long2ice@gmail.com, astralidea@163.com",
-    url="https://github.com/StarRocks/starrocks/tree/main/contrib/dbt-connector",
+    url="https://github.com/StarRocks/dbt-starrocks/",
     packages=find_namespace_packages(include=['dbt', 'dbt.*']),
     include_package_data=True,
     install_requires=[
-        "dbt-core==1.6.2",
+        "dbt-core~=1.6.0",
         "mysql-connector-python>=8.1",
     ],
     zip_safe=False,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
 
         'License :: OSI Approved :: Apache Software License',
```

