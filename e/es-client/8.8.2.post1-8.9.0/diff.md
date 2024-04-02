# Comparing `tmp/es_client-8.8.2.post1.tar.gz` & `tmp/es_client-8.9.0.tar.gz`

## Comparing `es_client-8.8.2.post1.tar` & `es_client-8.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/.readthedocs.yaml
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/cli.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/example.yml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/es_client/__init__.py
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/es_client/builder.py
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/es_client/cli_example.py
--rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/es_client/defaults.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/es_client/exceptions.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/es_client/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/es_client/helpers/__init__.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/es_client/helpers/schemacheck.py
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/es_client/helpers/utils.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/LICENSE
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/README.rst
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/pyproject.toml
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 es_client-8.8.2.post1/PKG-INFO
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 es_client-8.9.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 es_client-8.9.0/cli.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 es_client-8.9.0/example.yml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 es_client-8.9.0/es_client/__init__.py
+-rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 es_client-8.9.0/es_client/builder.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 es_client-8.9.0/es_client/cli_example.py
+-rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 es_client-8.9.0/es_client/defaults.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 es_client-8.9.0/es_client/exceptions.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 es_client-8.9.0/es_client/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 es_client-8.9.0/es_client/helpers/__init__.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 es_client-8.9.0/es_client/helpers/schemacheck.py
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 es_client-8.9.0/es_client/helpers/utils.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 es_client-8.9.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 es_client-8.9.0/LICENSE
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 es_client-8.9.0/README.rst
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 es_client-8.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 es_client-8.9.0/PKG-INFO
```

### Comparing `es_client-8.8.2.post1/es_client/builder.py` & `es_client-8.9.0/es_client/builder.py`

 * *Files identical despite different names*

### Comparing `es_client-8.8.2.post1/es_client/cli_example.py` & `es_client-8.9.0/es_client/cli_example.py`

 * *Files identical despite different names*

### Comparing `es_client-8.8.2.post1/es_client/defaults.py` & `es_client-8.9.0/es_client/defaults.py`

 * *Files identical despite different names*

### Comparing `es_client-8.8.2.post1/es_client/exceptions.py` & `es_client-8.9.0/es_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `es_client-8.8.2.post1/es_client/helpers/schemacheck.py` & `es_client-8.9.0/es_client/helpers/schemacheck.py`

 * *Files identical despite different names*

### Comparing `es_client-8.8.2.post1/es_client/helpers/utils.py` & `es_client-8.9.0/es_client/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `es_client-8.8.2.post1/.gitignore` & `es_client-8.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `es_client-8.8.2.post1/LICENSE` & `es_client-8.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `es_client-8.8.2.post1/README.rst` & `es_client-8.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `es_client-8.8.2.post1/pyproject.toml` & `es_client-8.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 keywords = [
     "elasticsearch",
     "client",
     "connect",
     "command-line"
 ]
 dependencies = [
-    "elasticsearch8==8.8.2",
-    "click==8.1.4",
+    "elasticsearch8==8.9.0",
+    "click==8.1.6",
     "pyyaml==6.0.1",
     "voluptuous>=0.13.1",
-    "certifi>=2023.5.7",
+    "certifi>=2023.7.22",
     "six>=1.16.0",
 ]
 
 [project.optional-dependencies]
 test = [
     "requests",
     "pytest >=7.2.1",
```

### Comparing `es_client-8.8.2.post1/PKG-INFO` & `es_client-8.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: es_client
-Version: 8.8.2.post1
+Version: 8.9.0
 Summary: Elasticsearch Client builder, complete with schema validation
 Project-URL: Homepage, https://github.com/untergeek/es_client
 Project-URL: Bug Tracker, https://github.com/untergeek/es_client/issues
 Project-URL: Documentation, https://es-client.readthedocs.io/
 Project-URL: Source Code, http://github.com/untergeek/es_client
 Project-URL: Release Notes, https://github.com/untergeek/es_client/releases
 Author-email: Aaron Mildenstein <aaron@mildensteins.com>
@@ -15,17 +15,17 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: certifi>=2023.5.7
-Requires-Dist: click==8.1.4
-Requires-Dist: elasticsearch8==8.8.2
+Requires-Dist: certifi>=2023.7.22
+Requires-Dist: click==8.1.6
+Requires-Dist: elasticsearch8==8.9.0
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: six>=1.16.0
 Requires-Dist: voluptuous>=0.13.1
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == 'doc'
 Requires-Dist: sphinx-rtd-theme; extra == 'doc'
 Provides-Extra: test
```

