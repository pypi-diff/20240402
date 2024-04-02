# Comparing `tmp/krules_companion_client-0.9rc2.tar.gz` & `tmp/krules_companion_client-0.9rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krules_companion_client-0.9rc2.tar", max compression
+gzip compressed data, was "krules_companion_client-0.9rc3.tar", max compression
```

## Comparing `krules_companion_client-0.9rc2.tar` & `krules_companion_client-0.9rc3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-07-18 15:35:18.000000 krules_companion_client-0.9rc2/README.md
--rw-r--r--   0        0        0       93 2024-02-06 17:06:41.057258 krules_companion_client-0.9rc2/krules_companion_client/__init__.py
--rw-r--r--   0        0        0    13964 2024-02-06 17:07:10.804816 krules_companion_client-0.9rc2/krules_companion_client/commands.py
--rw-r--r--   0        0        0     3974 2024-02-07 11:06:50.287189 krules_companion_client-0.9rc2/krules_companion_client/google/__init__.py
--rw-r--r--   0        0        0     3100 2024-02-07 12:58:22.738971 krules_companion_client-0.9rc2/krules_companion_client/http/__init__.py
--rw-r--r--   0        0        0     1131 2024-01-22 16:33:52.254619 krules_companion_client-0.9rc2/krules_companion_client/models.py
--rw-r--r--   0        0        0      849 2024-02-07 16:05:46.191165 krules_companion_client-0.9rc2/pyproject.toml
--rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 krules_companion_client-0.9rc2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-18 15:35:18.000000 krules_companion_client-0.9rc3/README.md
+-rw-r--r--   0        0        0       93 2024-02-06 17:06:41.057258 krules_companion_client-0.9rc3/krules_companion_client/__init__.py
+-rw-r--r--   0        0        0    13964 2024-02-06 17:07:10.804816 krules_companion_client-0.9rc3/krules_companion_client/commands.py
+-rw-r--r--   0        0        0     3974 2024-02-07 11:06:50.287189 krules_companion_client-0.9rc3/krules_companion_client/google/__init__.py
+-rw-r--r--   0        0        0     3100 2024-02-07 12:58:22.738971 krules_companion_client-0.9rc3/krules_companion_client/http/__init__.py
+-rw-r--r--   0        0        0     1131 2024-01-22 16:33:52.254619 krules_companion_client-0.9rc3/krules_companion_client/models.py
+-rw-r--r--   0        0        0      851 2024-02-07 16:08:31.788163 krules_companion_client-0.9rc3/pyproject.toml
+-rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 krules_companion_client-0.9rc3/PKG-INFO
```

### Comparing `krules_companion_client-0.9rc2/krules_companion_client/commands.py` & `krules_companion_client-0.9rc3/krules_companion_client/commands.py`

 * *Files identical despite different names*

### Comparing `krules_companion_client-0.9rc2/krules_companion_client/google/__init__.py` & `krules_companion_client-0.9rc3/krules_companion_client/google/__init__.py`

 * *Files identical despite different names*

### Comparing `krules_companion_client-0.9rc2/krules_companion_client/http/__init__.py` & `krules_companion_client-0.9rc3/krules_companion_client/http/__init__.py`

 * *Files identical despite different names*

### Comparing `krules_companion_client-0.9rc2/krules_companion_client/models.py` & `krules_companion_client-0.9rc3/krules_companion_client/models.py`

 * *Files identical despite different names*

### Comparing `krules_companion_client-0.9rc2/pyproject.toml` & `krules_companion_client-0.9rc3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "krules-companion-client"
-version = "0.9rc2"
+version = "0.9rc3"
 description = "KRules Companion Client"
 authors = ["AdE <alberto@airspot.tech>"]
 readme = "README.md"
 packages = [{include = "krules_companion_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = {extras = ["all"], version = "^0.9.0"}
 requests = "^2.31.0"
 validators = "^0.20.0"
 tomli = "^2.0.1"
 typing-extensions = "^4.8.0"
 pydantic = "^2.5.3"
-cloudevents = {version="^1.7.1", optional = true}
-google-cloud-pubsub = {version="^2.19.1", optional = true}
+cloudevents = {version="^1.10.1", optional = true}
+google-cloud-pubsub = {version="^2.13.11", optional = true}
 
 [tool.poetry.extras]
 google=["google-cloud-pubsub", "cloudevents"]
 
 [tool.poetry.scripts]
 cm = "krules_companion_client.commands:main"
```

### Comparing `krules_companion_client-0.9rc2/PKG-INFO` & `krules_companion_client-0.9rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: krules-companion-client
-Version: 0.9rc2
+Version: 0.9rc3
 Summary: KRules Companion Client
 Author: AdE
 Author-email: alberto@airspot.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: google
-Requires-Dist: cloudevents (>=1.7.1,<2.0.0) ; extra == "google"
-Requires-Dist: google-cloud-pubsub (>=2.19.1,<3.0.0) ; extra == "google"
+Requires-Dist: cloudevents (>=1.10.1,<2.0.0) ; extra == "google"
+Requires-Dist: google-cloud-pubsub (>=2.13.11,<3.0.0) ; extra == "google"
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: typing-extensions (>=4.8.0,<5.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
```

