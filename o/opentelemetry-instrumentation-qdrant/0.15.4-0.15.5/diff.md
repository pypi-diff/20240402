# Comparing `tmp/opentelemetry_instrumentation_qdrant-0.15.4.tar.gz` & `tmp/opentelemetry_instrumentation_qdrant-0.15.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_qdrant-0.15.4.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_qdrant-0.15.5.tar", max compression
```

## Comparing `opentelemetry_instrumentation_qdrant-0.15.4.tar` & `opentelemetry_instrumentation_qdrant-0.15.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      572 2024-03-31 07:52:14.197635 opentelemetry_instrumentation_qdrant-0.15.4/README.md
--rw-r--r--   0        0        0     1925 2024-03-31 07:52:14.197635 opentelemetry_instrumentation_qdrant-0.15.4/opentelemetry/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     2943 2024-03-31 07:52:14.197635 opentelemetry_instrumentation_qdrant-0.15.4/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json
--rw-r--r--   0        0        0     2828 2024-03-31 07:52:14.197635 opentelemetry_instrumentation_qdrant-0.15.4/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json
--rw-r--r--   0        0        0       23 2024-03-31 07:52:14.197635 opentelemetry_instrumentation_qdrant-0.15.4/opentelemetry/instrumentation/qdrant/version.py
--rw-r--r--   0        0        0     3657 2024-03-31 07:52:14.197635 opentelemetry_instrumentation_qdrant-0.15.4/opentelemetry/instrumentation/qdrant/wrapper.py
--rw-r--r--   0        0        0     1351 2024-03-31 07:52:38.105748 opentelemetry_instrumentation_qdrant-0.15.4/pyproject.toml
--rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_qdrant-0.15.4/PKG-INFO
+-rw-r--r--   0        0        0      572 2024-04-02 12:58:50.155935 opentelemetry_instrumentation_qdrant-0.15.5/README.md
+-rw-r--r--   0        0        0     1925 2024-04-02 12:58:50.155935 opentelemetry_instrumentation_qdrant-0.15.5/opentelemetry/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     2943 2024-04-02 12:58:50.155935 opentelemetry_instrumentation_qdrant-0.15.5/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json
+-rw-r--r--   0        0        0     2828 2024-04-02 12:58:50.155935 opentelemetry_instrumentation_qdrant-0.15.5/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json
+-rw-r--r--   0        0        0       23 2024-04-02 12:58:50.155935 opentelemetry_instrumentation_qdrant-0.15.5/opentelemetry/instrumentation/qdrant/version.py
+-rw-r--r--   0        0        0     3657 2024-04-02 12:58:50.155935 opentelemetry_instrumentation_qdrant-0.15.5/opentelemetry/instrumentation/qdrant/wrapper.py
+-rw-r--r--   0        0        0     1351 2024-04-02 12:59:15.075854 opentelemetry_instrumentation_qdrant-0.15.5/pyproject.toml
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_qdrant-0.15.5/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_qdrant-0.15.4/README.md` & `opentelemetry_instrumentation_qdrant-0.15.5/README.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.15.4/opentelemetry/instrumentation/qdrant/__init__.py` & `opentelemetry_instrumentation_qdrant-0.15.5/opentelemetry/instrumentation/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.15.4/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json` & `opentelemetry_instrumentation_qdrant-0.15.5/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.15.4/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json` & `opentelemetry_instrumentation_qdrant-0.15.5/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.15.4/opentelemetry/instrumentation/qdrant/wrapper.py` & `opentelemetry_instrumentation_qdrant-0.15.5/opentelemetry/instrumentation/qdrant/wrapper.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.15.4/pyproject.toml` & `opentelemetry_instrumentation_qdrant-0.15.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-instrumentation-qdrant"
-version = "0.15.4"
+version = "0.15.5"
 description = "OpenTelemetry Qdrant instrumentation"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
   "Tomer Friedman <tomer@traceloop.com>"
 ]
 repository = "https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-qdrant"
@@ -26,15 +26,15 @@
 python = ">=3.9,<4"
 opentelemetry-api = "^1.23.0"
 opentelemetry-instrumentation = "0.44b0"
 opentelemetry-semantic-conventions = "0.44b0"
 opentelemetry-semantic-conventions-ai = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
-autopep8 = "2.0.4"
+autopep8 = "2.1.0"
 flake8 = "7.0.0"
 
 [tool.poetry.group.test.dependencies]
 qdrant-client = "^1.7.3"
 pytest = "8.1.0"
 pytest-sugar = "1.0.0"
 opentelemetry-sdk = "^1.23.0"
```

### Comparing `opentelemetry_instrumentation_qdrant-0.15.4/PKG-INFO` & `opentelemetry_instrumentation_qdrant-0.15.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-qdrant
-Version: 0.15.4
+Version: 0.15.5
 Summary: OpenTelemetry Qdrant instrumentation
 Home-page: https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-qdrant
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: opentelemetry-instrumentation-qdrant Version:
-0.15.4 Summary: OpenTelemetry Qdrant instrumentation Home-page: https://
+0.15.5 Summary: OpenTelemetry Qdrant instrumentation Home-page: https://
 github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-
 instrumentation-qdrant License: Apache-2.0 Author: Gal Kleinman Author-email:
 gal@traceloop.com Requires-Python: >=3.9,<4 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: instruments
```

