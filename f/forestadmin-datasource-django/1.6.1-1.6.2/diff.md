# Comparing `tmp/forestadmin_datasource_django-1.6.1.tar.gz` & `tmp/forestadmin_datasource_django-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_datasource_django-1.6.1.tar", max compression
+gzip compressed data, was "forestadmin_datasource_django-1.6.2.tar", max compression
```

## Comparing `forestadmin_datasource_django-1.6.1.tar` & `forestadmin_datasource_django-1.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2024-03-22 10:40:33.685335 forestadmin_datasource_django-1.6.1/README.md
--rw-r--r--   0        0        0        0 2024-03-22 10:40:33.685335 forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/__init__.py
--rw-r--r--   0        0        0     3010 2024-03-22 10:40:33.685335 forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/collection.py
--rw-r--r--   0        0        0      589 2024-03-22 10:40:33.685335 forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/datasource.py
--rw-r--r--   0        0        0      217 2024-03-22 10:40:33.685335 forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/exception.py
--rw-r--r--   0        0        0      365 2024-03-22 10:40:33.685335 forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/interface.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:33.685335 forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/utils/__init__.py
--rw-r--r--   0        0        0     8327 2024-03-22 10:40:33.685335 forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/utils/model_introspection.py
--rw-r--r--   0        0        0     2177 2024-03-22 10:40:33.685335 forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/utils/native_driver_wrapper.py
--rw-r--r--   0        0        0    14254 2024-03-22 10:40:33.685335 forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/utils/query_factory.py
--rw-r--r--   0        0        0      916 2024-03-22 10:40:33.685335 forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/utils/record_serializer.py
--rw-r--r--   0        0        0     4178 2024-03-22 10:40:33.685335 forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/utils/type_converter.py
--rw-r--r--   0        0        0     1881 2024-03-22 10:40:51.901328 forestadmin_datasource_django-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 forestadmin_datasource_django-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:21.392764 forestadmin_datasource_django-1.6.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:21.392764 forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/__init__.py
+-rw-r--r--   0        0        0     3010 2024-04-02 07:31:21.392764 forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/collection.py
+-rw-r--r--   0        0        0      589 2024-04-02 07:31:21.392764 forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/datasource.py
+-rw-r--r--   0        0        0      217 2024-04-02 07:31:21.392764 forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/exception.py
+-rw-r--r--   0        0        0      365 2024-04-02 07:31:21.392764 forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/interface.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:21.392764 forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/utils/__init__.py
+-rw-r--r--   0        0        0     8327 2024-04-02 07:31:21.392764 forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/utils/model_introspection.py
+-rw-r--r--   0        0        0     2177 2024-04-02 07:31:21.392764 forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/utils/native_driver_wrapper.py
+-rw-r--r--   0        0        0    14254 2024-04-02 07:31:21.392764 forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/utils/query_factory.py
+-rw-r--r--   0        0        0      916 2024-04-02 07:31:21.392764 forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/utils/record_serializer.py
+-rw-r--r--   0        0        0     4178 2024-04-02 07:31:21.392764 forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/utils/type_converter.py
+-rw-r--r--   0        0        0     1881 2024-04-02 07:31:37.016797 forestadmin_datasource_django-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 forestadmin_datasource_django-1.6.2/PKG-INFO
```

### Comparing `forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/collection.py` & `forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/datasource.py` & `forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/utils/model_introspection.py` & `forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/utils/model_introspection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/utils/native_driver_wrapper.py` & `forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/utils/native_driver_wrapper.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/utils/query_factory.py` & `forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/utils/query_factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/utils/record_serializer.py` & `forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/utils/record_serializer.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_django-1.6.1/forestadmin/datasource_django/utils/type_converter.py` & `forestadmin_datasource_django-1.6.2/forestadmin/datasource_django/utils/type_converter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_django-1.6.1/pyproject.toml` & `forestadmin_datasource_django-1.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-datasource-django"
-version = "1.6.1"
+version = "1.6.2"
 description = "django datasource for forestadmin python agent"
 authors = [ "Julien Barreau <julien.barreau@forestadmin.com>",]
 readme = "README.md"
 repository = "https://github.com/ForestAdmin/agent-python"
 documentation = "https://docs.forestadmin.com/developer-guide-agents-python/"
 homepage = "https://www.forestadmin.com"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 typing-extensions = "~=4.2"
 django = ">=3.2,<6.0"
 psycopg2 = ">=2.8.4"
-forestadmin-datasource-toolkit = "1.6.1"
-forestadmin-agent-toolkit = "1.6.1"
+forestadmin-datasource-toolkit = "1.6.2"
+forestadmin-agent-toolkit = "1.6.2"
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "test_project_datasource.settings"
 pythonpath = "tests/test_project_datasource"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~=0.2.1"
```

### Comparing `forestadmin_datasource_django-1.6.1/PKG-INFO` & `forestadmin_datasource_django-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: forestadmin-datasource-django
-Version: 1.6.1
+Version: 1.6.2
 Summary: django datasource for forestadmin python agent
 Home-page: https://www.forestadmin.com
 Author: Julien Barreau
 Author-email: julien.barreau@forestadmin.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: django (>=3.2,<6.0)
-Requires-Dist: forestadmin-agent-toolkit (==1.6.1)
-Requires-Dist: forestadmin-datasource-toolkit (==1.6.1)
+Requires-Dist: forestadmin-agent-toolkit (==1.6.2)
+Requires-Dist: forestadmin-datasource-toolkit (==1.6.2)
 Requires-Dist: psycopg2 (>=2.8.4)
 Requires-Dist: typing-extensions (>=4.2,<5.0)
 Project-URL: Documentation, https://docs.forestadmin.com/developer-guide-agents-python/
 Project-URL: Repository, https://github.com/ForestAdmin/agent-python
 Description-Content-Type: text/markdown
```

