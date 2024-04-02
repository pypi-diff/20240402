# Comparing `tmp/ai_butler_sdk-0.4.6.tar.gz` & `tmp/ai_butler_sdk-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_butler_sdk-0.4.6.tar", max compression
+gzip compressed data, was "ai_butler_sdk-0.4.7.tar", max compression
```

## Comparing `ai_butler_sdk-0.4.6.tar` & `ai_butler_sdk-0.4.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2024-03-05 08:48:36.042873 ai_butler_sdk-0.4.6/ai_butler_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 01:59:14.986379 ai_butler_sdk-0.4.6/ai_butler_sdk/apis/__init__.py
--rw-r--r--   0        0        0     3154 2024-03-25 09:55:14.636724 ai_butler_sdk-0.4.6/ai_butler_sdk/apis/client.py
--rw-r--r--   0        0        0     1638 2024-03-26 07:50:09.843149 ai_butler_sdk-0.4.6/ai_butler_sdk/celery_app/__init__.py
--rw-r--r--   0        0        0     1213 2024-04-01 09:31:19.919697 ai_butler_sdk-0.4.6/ai_butler_sdk/celery_app/task_example.py
--rw-r--r--   0        0        0     5410 2024-04-01 09:31:19.926210 ai_butler_sdk-0.4.6/ai_butler_sdk/deploy_onnx.py
--rw-r--r--   0        0        0     1128 2024-03-26 03:22:01.404933 ai_butler_sdk-0.4.6/ai_butler_sdk/settings.py
--rw-r--r--   0        0        0     6051 2024-03-25 10:43:18.071678 ai_butler_sdk-0.4.6/ai_butler_sdk/train.py
--rw-r--r--   0        0        0     5303 2024-03-27 08:27:43.941506 ai_butler_sdk-0.4.6/ai_butler_sdk/utils.py
--rw-r--r--   0        0        0      783 2024-04-01 09:31:28.021618 ai_butler_sdk-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 ai_butler_sdk-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-03-05 08:48:36.042873 ai_butler_sdk-0.4.7/ai_butler_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 01:59:14.986379 ai_butler_sdk-0.4.7/ai_butler_sdk/apis/__init__.py
+-rw-r--r--   0        0        0     3154 2024-03-25 09:55:14.636724 ai_butler_sdk-0.4.7/ai_butler_sdk/apis/client.py
+-rw-r--r--   0        0        0     1638 2024-03-26 07:50:09.843149 ai_butler_sdk-0.4.7/ai_butler_sdk/celery_app/__init__.py
+-rw-r--r--   0        0        0     1213 2024-04-01 09:31:19.919697 ai_butler_sdk-0.4.7/ai_butler_sdk/celery_app/task_example.py
+-rw-r--r--   0        0        0     5410 2024-04-01 09:31:19.926210 ai_butler_sdk-0.4.7/ai_butler_sdk/deploy_onnx.py
+-rw-r--r--   0        0        0     1128 2024-03-26 03:22:01.404933 ai_butler_sdk-0.4.7/ai_butler_sdk/settings.py
+-rw-r--r--   0        0        0     6065 2024-04-02 07:05:42.778308 ai_butler_sdk-0.4.7/ai_butler_sdk/train.py
+-rw-r--r--   0        0        0     5303 2024-03-27 08:27:43.941506 ai_butler_sdk-0.4.7/ai_butler_sdk/utils.py
+-rw-r--r--   0        0        0      783 2024-04-02 07:05:42.771660 ai_butler_sdk-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 ai_butler_sdk-0.4.7/PKG-INFO
```

### Comparing `ai_butler_sdk-0.4.6/ai_butler_sdk/apis/client.py` & `ai_butler_sdk-0.4.7/ai_butler_sdk/apis/client.py`

 * *Files identical despite different names*

### Comparing `ai_butler_sdk-0.4.6/ai_butler_sdk/celery_app/__init__.py` & `ai_butler_sdk-0.4.7/ai_butler_sdk/celery_app/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_butler_sdk-0.4.6/ai_butler_sdk/celery_app/task_example.py` & `ai_butler_sdk-0.4.7/ai_butler_sdk/celery_app/task_example.py`

 * *Files identical despite different names*

### Comparing `ai_butler_sdk-0.4.6/ai_butler_sdk/deploy_onnx.py` & `ai_butler_sdk-0.4.7/ai_butler_sdk/deploy_onnx.py`

 * *Files identical despite different names*

### Comparing `ai_butler_sdk-0.4.6/ai_butler_sdk/settings.py` & `ai_butler_sdk-0.4.7/ai_butler_sdk/settings.py`

 * *Files identical despite different names*

### Comparing `ai_butler_sdk-0.4.6/ai_butler_sdk/train.py` & `ai_butler_sdk-0.4.7/ai_butler_sdk/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     def after_train(self):
         pass
 
     def upload_result(self):
         logger.info("---------------------------------开始上传训练结果---------------------------------")
         with open(self.result_local_path, "rb") as f:
             content = f.read()
-        resp = httpx.put(self.model_weight_upload_url, content=content)
+        resp = httpx.put(self.model_weight_upload_url, content=content, timeout=None)
         if resp.status_code != 200:
             logger.error("结果权重文件上传失败!")
             raise
         logger.info("---------------------------------训练结果上传完成---------------------------------")
 
     def upload_log(self):
         logger.info("---------------------------------开始上传训练日志---------------------------------")
```

### Comparing `ai_butler_sdk-0.4.6/ai_butler_sdk/utils.py` & `ai_butler_sdk-0.4.7/ai_butler_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ai_butler_sdk-0.4.6/pyproject.toml` & `ai_butler_sdk-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   "UP",  # pyupgrade
 ]
 line-length = 120
 exclude = [".mypy_cache", ".*", "logs", "static", "migrations"]
 
 [tool.poetry]
 name = "ai-butler-sdk"
-version = "0.4.6"
+version = "0.4.7"
 description = "AI模型生产管理平台sdk"
 authors = ["王凡 <wangfan@keanbang.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 minio = "^7.2.5"
 httpx = "^0.27.0"
```

### Comparing `ai_butler_sdk-0.4.6/PKG-INFO` & `ai_butler_sdk-0.4.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-butler-sdk
-Version: 0.4.6
+Version: 0.4.7
 Summary: AI模型生产管理平台sdk
 Author: 王凡
 Author-email: wangfan@keanbang.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

