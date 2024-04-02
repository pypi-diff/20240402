# Comparing `tmp/delphai_utils-3.4.2.tar.gz` & `tmp/delphai_utils-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphai_utils-3.4.2.tar", max compression
+gzip compressed data, was "delphai_utils-4.0.0.tar", max compression
```

## Comparing `delphai_utils-3.4.2.tar` & `delphai_utils-4.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       22 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/__init__.py
--rw-r--r--   0        0        0      936 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/aio.py
--rw-r--r--   0        0        0     3842 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/authorization.py
--rw-r--r--   0        0        0      495 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/authorization_test.py
--rw-r--r--   0        0        0     2069 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/caching.py
--rw-r--r--   0        0        0     3514 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/config.py
--rw-r--r--   0        0        0     1389 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/db.py
--rw-r--r--   0        0        0      549 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/elasticsearch.py
--rw-r--r--   0        0        0     9347 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/faust.py
--rw-r--r--   0        0        0      481 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/formatting.py
--rw-r--r--   0        0        0     6728 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/gateway.py
--rw-r--r--   0        0        0     4796 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/grpc_client.py
--rw-r--r--   0        0        0     3687 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/grpc_server.py
--rw-r--r--   0        0        0     1532 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/interceptors/authentication.py
--rw-r--r--   0        0        0     5218 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/interceptors/metrics.py
--rw-r--r--   0        0        0     1482 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/keycloak.py
--rw-r--r--   0        0        0     2373 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/logging.py
--rw-r--r--   0        0        0     7182 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/monitoring.py
--rw-r--r--   0        0        0     2926 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/patches.py
--rw-r--r--   0        0        0      119 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/rpc/__init__.py
--rw-r--r--   0        0        0    10126 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/rpc/client.py
--rw-r--r--   0        0        0      393 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/rpc/errors.py
--rw-r--r--   0        0        0     4949 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/rpc/metrics.py
--rw-r--r--   0        0        0     2052 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/rpc/models.py
--rw-r--r--   0        0        0    10175 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/rpc/server.py
--rw-r--r--   0        0        0     2830 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/rpc/types.py
--rw-r--r--   0        0        0      441 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/rpc/utils.py
--rw-r--r--   0        0        0      582 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/strings/similarity.py
--rw-r--r--   0        0        0     4146 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/users.py
--rw-r--r--   0        0        0     2608 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/utils.py
--rw-r--r--   0        0        0      435 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/validation.py
--rw-r--r--   0        0        0    43882 2024-03-28 15:59:01.935570 delphai_utils-3.4.2/delphai_utils/validator.py
--rw-r--r--   0        0        0     3437 2024-03-28 15:59:01.939570 delphai_utils-3.4.2/pyproject.toml
--rw-r--r--   0        0        0     3048 1970-01-01 00:00:00.000000 delphai_utils-3.4.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/__init__.py
+-rw-r--r--   0        0        0      936 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/aio.py
+-rw-r--r--   0        0        0     3842 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/authorization.py
+-rw-r--r--   0        0        0      495 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/authorization_test.py
+-rw-r--r--   0        0        0     2069 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/caching.py
+-rw-r--r--   0        0        0     1313 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/config.py
+-rw-r--r--   0        0        0     1389 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/db.py
+-rw-r--r--   0        0        0      549 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/elasticsearch.py
+-rw-r--r--   0        0        0     9347 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/faust.py
+-rw-r--r--   0        0        0      481 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/formatting.py
+-rw-r--r--   0        0        0     6728 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/gateway.py
+-rw-r--r--   0        0        0     4796 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/grpc_client.py
+-rw-r--r--   0        0        0     3687 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/grpc_server.py
+-rw-r--r--   0        0        0     1532 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/interceptors/authentication.py
+-rw-r--r--   0        0        0     5218 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/interceptors/metrics.py
+-rw-r--r--   0        0        0     1482 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/keycloak.py
+-rw-r--r--   0        0        0     1410 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/logging.py
+-rw-r--r--   0        0        0     7182 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/monitoring.py
+-rw-r--r--   0        0        0     2926 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/patches.py
+-rw-r--r--   0        0        0      119 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/rpc/__init__.py
+-rw-r--r--   0        0        0    10126 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/rpc/client.py
+-rw-r--r--   0        0        0      393 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/rpc/errors.py
+-rw-r--r--   0        0        0     4949 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/rpc/metrics.py
+-rw-r--r--   0        0        0     2052 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/rpc/models.py
+-rw-r--r--   0        0        0    10175 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/rpc/server.py
+-rw-r--r--   0        0        0     2830 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/rpc/types.py
+-rw-r--r--   0        0        0      441 2024-04-02 07:57:24.405013 delphai_utils-4.0.0/delphai_utils/rpc/utils.py
+-rw-r--r--   0        0        0      582 2024-04-02 07:57:24.409013 delphai_utils-4.0.0/delphai_utils/strings/similarity.py
+-rw-r--r--   0        0        0     4106 2024-04-02 07:57:24.409013 delphai_utils-4.0.0/delphai_utils/users.py
+-rw-r--r--   0        0        0     2608 2024-04-02 07:57:24.409013 delphai_utils-4.0.0/delphai_utils/utils.py
+-rw-r--r--   0        0        0      435 2024-04-02 07:57:24.409013 delphai_utils-4.0.0/delphai_utils/validation.py
+-rw-r--r--   0        0        0    43882 2024-04-02 07:57:24.409013 delphai_utils-4.0.0/delphai_utils/validator.py
+-rw-r--r--   0        0        0     3196 2024-04-02 07:57:24.409013 delphai_utils-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 delphai_utils-4.0.0/PKG-INFO
```

### Comparing `delphai_utils-3.4.2/delphai_utils/aio.py` & `delphai_utils-4.0.0/delphai_utils/aio.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/authorization.py` & `delphai_utils-4.0.0/delphai_utils/authorization.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/caching.py` & `delphai_utils-4.0.0/delphai_utils/caching.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/db.py` & `delphai_utils-4.0.0/delphai_utils/db.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/elasticsearch.py` & `delphai_utils-4.0.0/delphai_utils/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/faust.py` & `delphai_utils-4.0.0/delphai_utils/faust.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/gateway.py` & `delphai_utils-4.0.0/delphai_utils/gateway.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/grpc_client.py` & `delphai_utils-4.0.0/delphai_utils/grpc_client.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/grpc_server.py` & `delphai_utils-4.0.0/delphai_utils/grpc_server.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/interceptors/authentication.py` & `delphai_utils-4.0.0/delphai_utils/interceptors/authentication.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/interceptors/metrics.py` & `delphai_utils-4.0.0/delphai_utils/interceptors/metrics.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/keycloak.py` & `delphai_utils-4.0.0/delphai_utils/keycloak.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/logging.py` & `delphai_utils-4.0.0/delphai_utils/logging.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging as _logging
-import warnings
 
 import coloredlogs
 
 from delphai_utils.config import get_config
 
 
 LOGGING_LEVEL = "INFO"
@@ -47,43 +46,7 @@
     loggers_levels = dict(LOGGERS_LEVELS, **(loggers_levels or {}))
     for logger_name, logger_level in loggers_levels.items():
         _logging.getLogger(logger_name).setLevel(logger_level)
 
     for logger_name, logger_config in logging_config.get("loggers", {}).items():
         if "level" in logger_config:
             _logging.getLogger(logger_name).setLevel(logger_config["level"])
-
-
-def error_with_traceback():
-    """
-    Writes to log an occured exception with a last line of traceback
-    """
-
-    warnings.warn(
-        'Use `logger.exception("Your message")` instead of:',
-        RuntimeWarning,
-        stacklevel=2,
-    )
-    _logging.exception("Error")
-
-
-class _LoggingWrapper:
-    def __getattr__(self, name):
-        if "warning_showed" not in self.__dict__:
-            self.warning_showed = True
-
-            if not _logging.root.handlers:
-                warnings.warn(
-                    "You need to initialize logging by calling `delphai_utils.logging.configure_logging()`",
-                    RuntimeWarning,
-                    stacklevel=2,
-                )
-
-        warnings.warn(
-            "Use internal logging ( https://wiki.delphai.dev/wiki/Logging ) instead of:",
-            RuntimeWarning,
-            stacklevel=2,
-        )
-        return getattr(_logging, name)
-
-
-logging = _LoggingWrapper()
```

### Comparing `delphai_utils-3.4.2/delphai_utils/monitoring.py` & `delphai_utils-4.0.0/delphai_utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/patches.py` & `delphai_utils-4.0.0/delphai_utils/patches.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/rpc/client.py` & `delphai_utils-4.0.0/delphai_utils/rpc/client.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/rpc/metrics.py` & `delphai_utils-4.0.0/delphai_utils/rpc/metrics.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/rpc/models.py` & `delphai_utils-4.0.0/delphai_utils/rpc/models.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/rpc/server.py` & `delphai_utils-4.0.0/delphai_utils/rpc/server.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/rpc/types.py` & `delphai_utils-4.0.0/delphai_utils/rpc/types.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/strings/similarity.py` & `delphai_utils-4.0.0/delphai_utils/strings/similarity.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/users.py` & `delphai_utils-4.0.0/delphai_utils/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Dict, List, Tuple, Union
-from grpc.aio import ServicerContext
-from delphai_utils.keycloak import decode_token
 import asyncio
-import nest_asyncio
 
-nest_asyncio.apply()
+from grpc.aio import ServicerContext
+from typing import Dict, List, Tuple, Union
+
+from delphai_utils.keycloak import decode_token
 
 
 def get_user(context: ServicerContext) -> Dict:
     """
     Get x-delphai-user information.
     :param grpc.aio.ServicerContext context: context passed to grpc endpoints
     :raises: KeyError
```

### Comparing `delphai_utils-3.4.2/delphai_utils/utils.py` & `delphai_utils-4.0.0/delphai_utils/utils.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/delphai_utils/validator.py` & `delphai_utils-4.0.0/delphai_utils/validator.py`

 * *Files identical despite different names*

### Comparing `delphai_utils-3.4.2/pyproject.toml` & `delphai_utils-4.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,73 +1,63 @@
 [tool.poetry]
 name = "delphai-utils"
-version = "3.4.2"
+version = "4.0.0"
 description = "delphai backend utilities"
 authors = ["Barath Kumar <barath@delphai.com>"]
 homepage = "https://github.com/delphai/delphai-utils"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+aiokafka = { version = "0.7.2", optional = true }
+dataclasses-avroschema = { version = "^0.30.3", optional = true }
+python-schema-registry-client = { version = "^2.4.1", optional = true }
 omegaconf = { version = "^2.1.0", optional = true }
-memoization = { version = "^0.3.1", optional = true }
 python-dotenv = { version = "^0.14.0", optional = true }
-kubernetes = { version = "^25.3.0", optional = true }
 coloredlogs = { version = "^14.0", optional = true }
-deepmerge = { version = "^0.1.0", optional = true }
 grpcio = { version = "^1.32.0", optional = true }
 starlette = { version = "^0", optional = true }
 hypercorn = { version = "^0.10.2", optional = true }
 validate_email = { version = "^1.3", optional = true }
 ipaddress = { version = "^1.0.23", optional = true }
 jinja2 = { version = "^2.11.2", optional = true }
-markupsafe = { version = "~2.0", optional = true }
 starlette-prometheus = { version = ">=0.7.0 <1.0.0", optional = true }
 grpcio-health-checking = { version = "^1.32.0", optional = true }
 grpcio-reflection = { version = "^1.32.0", optional = true }
 googleapis-common-protos = { version = "^1.52.0", optional = true }
 elasticsearch = { extras = ["async"], version = "^7.9.1", optional = true }
 motor = { version = "^2.3.0", optional = true }
-keyring = { version = "^21.5.0", optional = true }
 httpx = { version = "^0.23.1", optional = true, extras = ["http2"] }
 python-jose = { version = "^3.2.0", optional = true }
 grpclib = { version = "^0.4.2", optional = true }
 faust-streaming = { version = "^0.6.9", optional = true }
 dacite = { version = "^1.6.0", optional = true }
 confluent-kafka = { version = "^1.7.0", optional = true }
 betterproto = { version = "2.0.0b3", extras = ["compiler"], optional = true }
-nest-asyncio = "^1.5.1"
-aiokafka = "0.7.2"
-dataclasses-avroschema = "^0.30.3"
-python-schema-registry-client = "^2.4.1"
-protobuf = "^3.20"
+protobuf = { version = "^3.20", optional = true }
 aio-pika = { version = "^9.1.4", optional = true }
 pydantic = { version = "^2.2", optional = true }
 msgpack = { version = "^1.0.5", optional = true }
 prometheus-client = {version = "^0", optional = true}
 
 [tool.poetry.extras]
 config = [
   "omegaconf",
-  "memoization",
   "python-dotenv",
-  "kubernetes",
-  "deepmerge",
-  "keyring",
   "coloredlogs",
   "dacite",
 ]
 
 grpc = [
+  "protobuf",
   "grpcio",
   "starlette",
   "hypercorn",
   "validate_email",
   "ipaddress",
   "jinja2",
-  "markupsafe",
   "starlette-prometheus",
   "grpcio-health-checking",
   "grpcio-reflection",
   "googleapis-common-protos",
   "httpx",
   "python-jose",
 ]
@@ -78,15 +68,14 @@
 
 streaming = [
   "aiokafka",
   "betterproto",
   "confluent-kafka",
   "faust-streaming",
   "grpclib",
-  "markupsafe",
   "dataclasses-avroschema",
   "python-schema-registry-client",
 ]
 
 keycloak = ["httpx", "python-jose"]
 
 rpc = ["aio-pika", "pydantic", "msgpack", "prometheus-client"]
```

### Comparing `delphai_utils-3.4.2/PKG-INFO` & `delphai_utils-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphai-utils
-Version: 3.4.2
+Version: 4.0.0
 Summary: delphai backend utilities
 Home-page: https://github.com/delphai/delphai-utils
 Author: Barath Kumar
 Author-email: barath@delphai.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -22,36 +22,30 @@
 Requires-Dist: aio-pika (>=9.1.4,<10.0.0) ; extra == "rpc"
 Requires-Dist: aiokafka (==0.7.2) ; extra == "streaming"
 Requires-Dist: betterproto[compiler] (==2.0.0b3) ; extra == "streaming"
 Requires-Dist: coloredlogs (>=14.0,<15.0) ; extra == "config"
 Requires-Dist: confluent-kafka (>=1.7.0,<2.0.0) ; extra == "streaming"
 Requires-Dist: dacite (>=1.6.0,<2.0.0) ; extra == "config"
 Requires-Dist: dataclasses-avroschema (>=0.30.3,<0.31.0) ; extra == "streaming"
-Requires-Dist: deepmerge (>=0.1.0,<0.2.0) ; extra == "config"
 Requires-Dist: elasticsearch[async] (>=7.9.1,<8.0.0) ; extra == "elasticsearch"
 Requires-Dist: faust-streaming (>=0.6.9,<0.7.0) ; extra == "streaming"
 Requires-Dist: googleapis-common-protos (>=1.52.0,<2.0.0) ; extra == "grpc"
 Requires-Dist: grpcio (>=1.32.0,<2.0.0) ; extra == "grpc"
 Requires-Dist: grpcio-health-checking (>=1.32.0,<2.0.0) ; extra == "grpc"
 Requires-Dist: grpcio-reflection (>=1.32.0,<2.0.0) ; extra == "grpc"
 Requires-Dist: grpclib (>=0.4.2,<0.5.0) ; extra == "streaming"
 Requires-Dist: httpx[http2] (>=0.23.1,<0.24.0) ; extra == "grpc" or extra == "keycloak"
 Requires-Dist: hypercorn (>=0.10.2,<0.11.0) ; extra == "grpc"
 Requires-Dist: ipaddress (>=1.0.23,<2.0.0) ; extra == "grpc"
 Requires-Dist: jinja2 (>=2.11.2,<3.0.0) ; extra == "grpc"
-Requires-Dist: keyring (>=21.5.0,<22.0.0) ; extra == "config"
-Requires-Dist: kubernetes (>=25.3.0,<26.0.0) ; extra == "config"
-Requires-Dist: markupsafe (>=2.0,<2.1) ; extra == "grpc" or extra == "streaming"
-Requires-Dist: memoization (>=0.3.1,<0.4.0) ; extra == "config"
 Requires-Dist: motor (>=2.3.0,<3.0.0) ; extra == "database"
 Requires-Dist: msgpack (>=1.0.5,<2.0.0) ; extra == "rpc"
-Requires-Dist: nest-asyncio (>=1.5.1,<2.0.0)
 Requires-Dist: omegaconf (>=2.1.0,<3.0.0) ; extra == "config"
 Requires-Dist: prometheus-client (>=0,<1) ; extra == "rpc"
-Requires-Dist: protobuf (>=3.20,<4.0)
+Requires-Dist: protobuf (>=3.20,<4.0) ; extra == "grpc"
 Requires-Dist: pydantic (>=2.2,<3.0) ; extra == "rpc"
 Requires-Dist: python-dotenv (>=0.14.0,<0.15.0) ; extra == "config"
 Requires-Dist: python-jose (>=3.2.0,<4.0.0) ; extra == "grpc" or extra == "keycloak"
 Requires-Dist: python-schema-registry-client (>=2.4.1,<3.0.0) ; extra == "streaming"
 Requires-Dist: starlette (>=0,<1) ; extra == "grpc"
 Requires-Dist: starlette-prometheus (>=0.7.0,<1.0.0) ; extra == "grpc"
 Requires-Dist: validate_email (>=1.3,<2.0) ; extra == "grpc"
```

