# Comparing `tmp/approck_aiogram_utils-0.1.0.tar.gz` & `tmp/approck_aiogram_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_aiogram_utils-0.1.0.tar", max compression
+gzip compressed data, was "approck_aiogram_utils-0.1.1.tar", max compression
```

## Comparing `approck_aiogram_utils-0.1.0.tar` & `approck_aiogram_utils-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0       23 2024-03-19 20:20:49.625423 approck_aiogram_utils-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-19 20:20:49.647422 approck_aiogram_utils-0.1.0/approck_aiogram_utils/__init__.py
--rw-r--r--   0        0        0     5100 2024-03-19 20:20:49.625423 approck_aiogram_utils-0.1.0/approck_aiogram_utils/message.py
--rw-r--r--   0        0        0      693 2024-03-19 20:20:49.626423 approck_aiogram_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-02 20:06:43.647464 approck_aiogram_utils-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 20:06:43.671464 approck_aiogram_utils-0.1.1/approck_aiogram_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 20:06:43.672464 approck_aiogram_utils-0.1.1/approck_aiogram_utils/integration/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 20:06:43.672464 approck_aiogram_utils-0.1.1/approck_aiogram_utils/integration/uprock/__init__.py
+-rw-r--r--   0        0        0     1314 2024-04-02 20:06:43.647464 approck_aiogram_utils-0.1.1/approck_aiogram_utils/integration/uprock/app.py
+-rw-r--r--   0        0        0     5100 2024-04-02 20:06:43.647464 approck_aiogram_utils-0.1.1/approck_aiogram_utils/message.py
+-rw-r--r--   0        0        0      771 2024-04-02 20:06:43.648464 approck_aiogram_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.1/PKG-INFO
```

### Comparing `approck_aiogram_utils-0.1.0/approck_aiogram_utils/message.py` & `approck_aiogram_utils-0.1.1/approck_aiogram_utils/message.py`

 * *Files identical despite different names*

### Comparing `approck_aiogram_utils-0.1.0/pyproject.toml` & `approck_aiogram_utils-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [tool.poetry]
 name = "approck-aiogram-utils"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Aleksey Dalekin <ald@approck.pro>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 aiogram = "^3.4.1"
 approck-messaging = [
     { version = "0.1.2" },
     { version = "0.1.2", extras = ["transport"], optional = true }
 ]
 loguru = "^0.7.2"
 pydantic = { extras = ["email", "dotenv"], version = ">=2.4.1,<2.6" }
 pydantic-settings = "^2.1.0"
 python = "^3.10"
+uprock-sdk = { version = "^0.1.10", optional = true }
 
 [tool.poetry.extras]
 transport = ["approck-messaging"]
+uprock = ["uprock-sdk"]
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.1.1"
 pre-commit = "^3.1.0"
 pytest = "^8.1.1"
 ruff = "^0.3.0"
```

### Comparing `approck_aiogram_utils-0.1.0/PKG-INFO` & `approck_aiogram_utils-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: approck-aiogram-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Aleksey Dalekin
 Author-email: ald@approck.pro
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: transport
+Provides-Extra: uprock
 Requires-Dist: aiogram (>=3.4.1,<4.0.0)
 Requires-Dist: approck-messaging (==0.1.2) ; extra == "transport"
 Requires-Dist: approck-messaging[transport] (==0.1.2) ; extra == "transport"
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
 Requires-Dist: pydantic[dotenv,email] (>=2.4.1,<2.6)
+Requires-Dist: uprock-sdk (>=0.1.10,<0.2.0) ; extra == "uprock"
 Description-Content-Type: text/markdown
 
 # Approck Aiogram Utils
```

