# Comparing `tmp/async_processor-0.1.9rc1.tar.gz` & `tmp/async_processor-0.1.9rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_processor-0.1.9rc1.tar", max compression
+gzip compressed data, was "async_processor-0.1.9rc2.tar", max compression
```

## Comparing `async_processor-0.1.9rc1.tar` & `async_processor-0.1.9rc2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-10-11 13:04:00.927428 async_processor-0.1.9rc1/LICENSE
--rw-r--r--   0        0        0     3654 2023-10-11 13:04:00.927428 async_processor-0.1.9rc1/README.md
--rw-r--r--   0        0        0     1007 2023-10-11 13:04:00.927428 async_processor-0.1.9rc1/async_processor/__init__.py
--rw-r--r--   0        0        0     3974 2023-10-11 13:04:00.927428 async_processor-0.1.9rc1/async_processor/app.py
--rw-r--r--   0        0        0     2777 2023-10-11 13:04:00.927428 async_processor-0.1.9rc1/async_processor/function_service/README.md
--rw-r--r--   0        0        0      139 2023-10-11 13:04:00.927428 async_processor-0.1.9rc1/async_processor/function_service/__init__.py
--rw-r--r--   0        0        0     6195 2023-10-11 13:04:00.927428 async_processor-0.1.9rc1/async_processor/function_service/async_function_deployment.py
--rw-r--r--   0        0        0     2630 2023-10-11 13:04:00.927428 async_processor-0.1.9rc1/async_processor/function_service/utils.py
--rw-r--r--   0        0        0     4426 2023-10-11 13:04:00.927428 async_processor-0.1.9rc1/async_processor/kafka_pub_sub.py
--rw-r--r--   0        0        0      351 2023-10-11 13:04:00.931428 async_processor-0.1.9rc1/async_processor/logger.py
--rw-r--r--   0        0        0     6888 2023-10-11 13:04:00.931428 async_processor-0.1.9rc1/async_processor/nats_pub_sub.py
--rw-r--r--   0        0        0     2760 2023-10-11 13:04:00.931428 async_processor-0.1.9rc1/async_processor/processor.py
--rw-r--r--   0        0        0     3861 2023-10-11 13:04:00.931428 async_processor-0.1.9rc1/async_processor/prometheus_metrics.py
--rw-r--r--   0        0        0       67 2023-10-11 13:04:00.931428 async_processor-0.1.9rc1/async_processor/sidecar/__init__.py
--rw-r--r--   0        0        0     1520 2023-10-11 13:04:00.931428 async_processor-0.1.9rc1/async_processor/sidecar/sidecar.py
--rw-r--r--   0        0        0     2955 2023-10-11 13:04:00.931428 async_processor-0.1.9rc1/async_processor/sqs_pub_sub.py
--rw-r--r--   0        0        0     5506 2023-10-11 13:04:00.931428 async_processor-0.1.9rc1/async_processor/types.py
--rw-r--r--   0        0        0     6305 2023-10-11 13:04:00.931428 async_processor-0.1.9rc1/async_processor/worker.py
--rw-r--r--   0        0        0     1282 2023-10-11 13:04:15.371448 async_processor-0.1.9rc1/pyproject.toml
--rw-r--r--   0        0        0     4745 1970-01-01 00:00:00.000000 async_processor-0.1.9rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/LICENSE
+-rw-r--r--   0        0        0     3654 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/README.md
+-rw-r--r--   0        0        0     1007 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/__init__.py
+-rw-r--r--   0        0        0     3974 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/app.py
+-rw-r--r--   0        0        0     2777 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/function_service/README.md
+-rw-r--r--   0        0        0      139 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/function_service/__init__.py
+-rw-r--r--   0        0        0     6195 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/function_service/async_function_deployment.py
+-rw-r--r--   0        0        0     2630 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/function_service/utils.py
+-rw-r--r--   0        0        0     4426 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/kafka_pub_sub.py
+-rw-r--r--   0        0        0      351 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/logger.py
+-rw-r--r--   0        0        0     6888 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/nats_pub_sub.py
+-rw-r--r--   0        0        0     2760 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/processor.py
+-rw-r--r--   0        0        0     3861 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/prometheus_metrics.py
+-rw-r--r--   0        0        0       67 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/sidecar/__init__.py
+-rw-r--r--   0        0        0     1819 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/sidecar/sidecar.py
+-rw-r--r--   0        0        0     2955 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/sqs_pub_sub.py
+-rw-r--r--   0        0        0     5620 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/types.py
+-rw-r--r--   0        0        0     6445 2023-10-11 15:09:05.617569 async_processor-0.1.9rc2/async_processor/worker.py
+-rw-r--r--   0        0        0     1282 2023-10-11 15:09:18.341744 async_processor-0.1.9rc2/pyproject.toml
+-rw-r--r--   0        0        0     4745 1970-01-01 00:00:00.000000 async_processor-0.1.9rc2/PKG-INFO
```

### Comparing `async_processor-0.1.9rc1/LICENSE` & `async_processor-0.1.9rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_processor-0.1.9rc1/README.md` & `async_processor-0.1.9rc2/README.md`

 * *Files identical despite different names*

### Comparing `async_processor-0.1.9rc1/async_processor/__init__.py` & `async_processor-0.1.9rc2/async_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `async_processor-0.1.9rc1/async_processor/app.py` & `async_processor-0.1.9rc2/async_processor/app.py`

 * *Files identical despite different names*

### Comparing `async_processor-0.1.9rc1/async_processor/function_service/README.md` & `async_processor-0.1.9rc2/async_processor/function_service/README.md`

 * *Files identical despite different names*

### Comparing `async_processor-0.1.9rc1/async_processor/function_service/async_function_deployment.py` & `async_processor-0.1.9rc2/async_processor/function_service/async_function_deployment.py`

 * *Files identical despite different names*

### Comparing `async_processor-0.1.9rc1/async_processor/function_service/utils.py` & `async_processor-0.1.9rc2/async_processor/function_service/utils.py`

 * *Files identical despite different names*

### Comparing `async_processor-0.1.9rc1/async_processor/kafka_pub_sub.py` & `async_processor-0.1.9rc2/async_processor/kafka_pub_sub.py`

 * *Files identical despite different names*

### Comparing `async_processor-0.1.9rc1/async_processor/nats_pub_sub.py` & `async_processor-0.1.9rc2/async_processor/nats_pub_sub.py`

 * *Files identical despite different names*

### Comparing `async_processor-0.1.9rc1/async_processor/processor.py` & `async_processor-0.1.9rc2/async_processor/processor.py`

 * *Files identical despite different names*

### Comparing `async_processor-0.1.9rc1/async_processor/prometheus_metrics.py` & `async_processor-0.1.9rc2/async_processor/prometheus_metrics.py`

 * *Files identical despite different names*

### Comparing `async_processor-0.1.9rc1/async_processor/sidecar/sidecar.py` & `async_processor-0.1.9rc2/async_processor/sidecar/sidecar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from typing import Optional
 
 import aiohttp
 from pydantic import BaseSettings, confloat
 
-from async_processor import AsyncProcessor, InputMessage
+from async_processor import AsyncProcessor, InputMessage, OutputMessage, ProcessStatus
 from async_processor.logger import logger
 
 
 class Settings(BaseSettings):
     destination_url: str
     request_timeout: confloat(gt=0) = 3.0
 
@@ -37,18 +37,23 @@
                 logger.warning(
                     "Cannot connect to %s retrying in 1 second. " "%s",
                     settings.destination_url,
                     str(ex),
                 )
                 await asyncio.sleep(1.0)
 
-    async def process(self, input_message: InputMessage) -> str:
+    async def process(self, input_message: InputMessage) -> OutputMessage:
         async with self._client_session.post(
             settings.destination_url,
             json=input_message.body,
             timeout=settings.request_timeout,
         ) as response:
-            response.raise_for_status()
-            return await response.text()
+            return OutputMessage(
+                request_id=input_message.request_id,
+                status=ProcessStatus.SUCCESS if response.ok else ProcessStatus.FAILED,
+                body=await response.text(),
+                status_code=response.status,
+                content_type=response.headers["content-type"],
+            )
 
 
 app = SidecarProcessor().build_app()
```

### Comparing `async_processor-0.1.9rc1/async_processor/sqs_pub_sub.py` & `async_processor-0.1.9rc2/async_processor/sqs_pub_sub.py`

 * *Files identical despite different names*

### Comparing `async_processor-0.1.9rc1/async_processor/types.py` & `async_processor-0.1.9rc2/async_processor/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 
 class OutputMessage(BaseModel):
     request_id: str
     status: ProcessStatus
     body: Optional[Any] = None
     error: Optional[str] = None
 
+    # these are experimental fields
+    status_code: Optional[str] = None
+    content_type: Optional[str] = None
+
     class Config:
         use_enum_values = True
 
 
 class InputMessageFetchFailure(Exception):
     ...
```

### Comparing `async_processor-0.1.9rc1/async_processor/worker.py` & `async_processor-0.1.9rc2/async_processor/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,19 +110,22 @@
         input_message: Optional[InputMessage] = None
         with collect_total_message_processing_metrics():
             try:
                 input_message = self._processor.input_deserializer(
                     serialized_input_message
                 )
                 result = await self._processor.process(input_message=input_message)
-                output_message = OutputMessage(
-                    status=ProcessStatus.SUCCESS,
-                    request_id=input_message.request_id,
-                    body=result,
-                )
+                if isinstance(result, OutputMessage):
+                    output_message = result
+                else:
+                    output_message = OutputMessage(
+                        status=ProcessStatus.SUCCESS,
+                        request_id=input_message.request_id,
+                        body=result,
+                    )
                 serialized_output_message = self._processor.output_serializer(
                     output_message
                 )
             except Exception as ex:
                 logger.exception("error raised while handling message")
                 if input_message:
                     output_message = OutputMessage(
```

### Comparing `async_processor-0.1.9rc1/pyproject.toml` & `async_processor-0.1.9rc2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-processor"
-version = "0.1.9rc1"
+version = "0.1.9rc2"
 description = ""
 authors = ["debajyoti-truefoundry <debajyoti@truefoundry.com>"]
 readme = "README.md"
 packages = [{include = "async_processor"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `async_processor-0.1.9rc1/PKG-INFO` & `async_processor-0.1.9rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-processor
-Version: 0.1.9rc1
+Version: 0.1.9rc2
 Summary: 
 Author: debajyoti-truefoundry
 Author-email: debajyoti@truefoundry.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

