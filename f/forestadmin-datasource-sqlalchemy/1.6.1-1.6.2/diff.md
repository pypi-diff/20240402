# Comparing `tmp/forestadmin_datasource_sqlalchemy-1.6.1.tar.gz` & `tmp/forestadmin_datasource_sqlalchemy-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_datasource_sqlalchemy-1.6.1.tar", max compression
+gzip compressed data, was "forestadmin_datasource_sqlalchemy-1.6.2.tar", max compression
```

## Comparing `forestadmin_datasource_sqlalchemy-1.6.1.tar` & `forestadmin_datasource_sqlalchemy-1.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2024-03-22 10:40:35.239349 forestadmin_datasource_sqlalchemy-1.6.1/README.md
--rw-r--r--   0        0        0        0 2024-03-22 10:40:35.239349 forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/__init__.py
--rw-r--r--   0        0        0    10651 2024-03-22 10:40:35.239349 forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/collections.py
--rw-r--r--   0        0        0     3637 2024-03-22 10:40:35.239349 forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/datasource.py
--rw-r--r--   0        0        0      612 2024-03-22 10:40:35.239349 forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/exceptions.py
--rw-r--r--   0        0        0     1923 2024-03-22 10:40:35.239349 forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/interfaces.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:35.239349 forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/utils/__init__.py
--rw-r--r--   0        0        0     5956 2024-03-22 10:40:35.239349 forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/utils/aggregation.py
--rw-r--r--   0        0        0     7050 2024-03-22 10:40:35.239349 forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/utils/model_converter.py
--rw-r--r--   0        0        0    10105 2024-03-22 10:40:35.239349 forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/utils/query_factory.py
--rw-r--r--   0        0        0     3087 2024-03-22 10:40:35.239349 forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/utils/record_serializer.py
--rw-r--r--   0        0        0      519 2024-03-22 10:40:35.243349 forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/utils/relationships.py
--rw-r--r--   0        0        0     5642 2024-03-22 10:40:35.243349 forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/utils/type_converter.py
--rw-r--r--   0        0        0     1779 2024-03-22 10:40:53.567528 forestadmin_datasource_sqlalchemy-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 forestadmin_datasource_sqlalchemy-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.636059 forestadmin_datasource_sqlalchemy-1.6.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.636059 forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    10651 2024-04-02 07:31:20.636059 forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/collections.py
+-rw-r--r--   0        0        0     3637 2024-04-02 07:31:20.636059 forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/datasource.py
+-rw-r--r--   0        0        0      612 2024-04-02 07:31:20.636059 forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/exceptions.py
+-rw-r--r--   0        0        0     1923 2024-04-02 07:31:20.636059 forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/interfaces.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.636059 forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/utils/__init__.py
+-rw-r--r--   0        0        0     5956 2024-04-02 07:31:20.636059 forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/utils/aggregation.py
+-rw-r--r--   0        0        0     7050 2024-04-02 07:31:20.636059 forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/utils/model_converter.py
+-rw-r--r--   0        0        0    10105 2024-04-02 07:31:20.636059 forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/utils/query_factory.py
+-rw-r--r--   0        0        0     3087 2024-04-02 07:31:20.636059 forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/utils/record_serializer.py
+-rw-r--r--   0        0        0      519 2024-04-02 07:31:20.636059 forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/utils/relationships.py
+-rw-r--r--   0        0        0     5642 2024-04-02 07:31:20.636059 forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/utils/type_converter.py
+-rw-r--r--   0        0        0     1779 2024-04-02 07:31:37.116137 forestadmin_datasource_sqlalchemy-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 forestadmin_datasource_sqlalchemy-1.6.2/PKG-INFO
```

### Comparing `forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/collections.py` & `forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/datasource.py` & `forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/exceptions.py` & `forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/exceptions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/interfaces.py` & `forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/interfaces.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/utils/aggregation.py` & `forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/utils/aggregation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/utils/model_converter.py` & `forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/utils/model_converter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/utils/query_factory.py` & `forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/utils/query_factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/utils/record_serializer.py` & `forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/utils/record_serializer.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/utils/relationships.py` & `forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/utils/relationships.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.6.1/forestadmin/datasource_sqlalchemy/utils/type_converter.py` & `forestadmin_datasource_sqlalchemy-1.6.2/forestadmin/datasource_sqlalchemy/utils/type_converter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.6.1/pyproject.toml` & `forestadmin_datasource_sqlalchemy-1.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-datasource-sqlalchemy"
-version = "1.6.1"
+version = "1.6.2"
 description = "sqlalchemy datasource for forestadmin python agent"
 authors = [ "Valentin Monté <valentinm@forestadmin.com>", "Julien Barreau <julien.barreau@forestadmin.com>",]
 readme = "README.md"
 repository = "https://github.com/ForestAdmin/agent-python"
 documentation = "https://docs.forestadmin.com/developer-guide-agents-python/"
 homepage = "https://www.forestadmin.com"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 typing-extensions = "~=4.2"
 sqlalchemy = ">=1.4.0"
-forestadmin-datasource-toolkit = "1.6.1"
-forestadmin-agent-toolkit = "1.6.1"
+forestadmin-datasource-toolkit = "1.6.2"
+forestadmin-agent-toolkit = "1.6.2"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~=0.2.1"
 python = "<3.9"
 extras = [ "tzdata",]
 
 [tool.poetry.group.test]
```

### Comparing `forestadmin_datasource_sqlalchemy-1.6.1/PKG-INFO` & `forestadmin_datasource_sqlalchemy-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: forestadmin-datasource-sqlalchemy
-Version: 1.6.1
+Version: 1.6.2
 Summary: sqlalchemy datasource for forestadmin python agent
 Home-page: https://www.forestadmin.com
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
-Requires-Dist: forestadmin-agent-toolkit (==1.6.1)
-Requires-Dist: forestadmin-datasource-toolkit (==1.6.1)
+Requires-Dist: forestadmin-agent-toolkit (==1.6.2)
+Requires-Dist: forestadmin-datasource-toolkit (==1.6.2)
 Requires-Dist: sqlalchemy (>=1.4.0)
 Requires-Dist: typing-extensions (>=4.2,<5.0)
 Project-URL: Documentation, https://docs.forestadmin.com/developer-guide-agents-python/
 Project-URL: Repository, https://github.com/ForestAdmin/agent-python
 Description-Content-Type: text/markdown
```

