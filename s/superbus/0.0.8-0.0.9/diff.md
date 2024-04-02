# Comparing `tmp/superbus-0.0.8.tar.gz` & `tmp/superbus-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superbus-0.0.8.tar", last modified: Tue Mar  5 08:29:49 2024, max compression
+gzip compressed data, was "superbus-0.0.9.tar", last modified: Fri Mar 29 20:36:37 2024, max compression
```

## Comparing `superbus-0.0.8.tar` & `superbus-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 starrabb1t  (1000) starrabb1t  (1000)        0 2024-03-05 08:29:49.013673 superbus-0.0.8/
--rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)     1067 2023-12-04 14:49:15.000000 superbus-0.0.8/LICENSE
--rw-r--r--   0 starrabb1t  (1000) starrabb1t  (1000)      783 2024-03-05 08:29:49.013673 superbus-0.0.8/PKG-INFO
--rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)      214 2023-12-05 13:45:14.000000 superbus-0.0.8/README.md
--rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)      103 2023-12-04 14:53:51.000000 superbus-0.0.8/pyproject.toml
--rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)      666 2024-03-05 08:29:49.013673 superbus-0.0.8/setup.cfg
-drwxrwxr-x   0 starrabb1t  (1000) starrabb1t  (1000)        0 2024-03-05 08:29:49.009673 superbus-0.0.8/src/
-drwxrwxr-x   0 starrabb1t  (1000) starrabb1t  (1000)        0 2024-03-05 08:29:49.013673 superbus-0.0.8/src/superbus/
--rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)       54 2023-12-04 22:57:45.000000 superbus-0.0.8/src/superbus/__init__.py
--rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)     2073 2024-03-05 08:26:30.000000 superbus-0.0.8/src/superbus/client.py
--rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)     2972 2023-12-11 22:12:10.000000 superbus-0.0.8/src/superbus/updater.py
--rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)     1950 2024-03-05 08:29:24.000000 superbus-0.0.8/src/superbus/utils.py
--rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)     3570 2024-01-25 09:51:44.000000 superbus-0.0.8/src/superbus/worker.py
-drwxrwxr-x   0 starrabb1t  (1000) starrabb1t  (1000)        0 2024-03-05 08:29:49.013673 superbus-0.0.8/src/superbus.egg-info/
--rw-r--r--   0 starrabb1t  (1000) starrabb1t  (1000)      783 2024-03-05 08:29:49.000000 superbus-0.0.8/src/superbus.egg-info/PKG-INFO
--rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)      338 2024-03-05 08:29:49.000000 superbus-0.0.8/src/superbus.egg-info/SOURCES.txt
--rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)        1 2024-03-05 08:29:49.000000 superbus-0.0.8/src/superbus.egg-info/dependency_links.txt
--rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)       43 2024-03-05 08:29:49.000000 superbus-0.0.8/src/superbus.egg-info/requires.txt
--rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)        9 2024-03-05 08:29:49.000000 superbus-0.0.8/src/superbus.egg-info/top_level.txt
+drwxrwxr-x   0 starrabb1t  (1000) starrabb1t  (1000)        0 2024-03-29 20:36:37.469217 superbus-0.0.9/
+-rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)     1067 2023-12-04 14:49:15.000000 superbus-0.0.9/LICENSE
+-rw-r--r--   0 starrabb1t  (1000) starrabb1t  (1000)      783 2024-03-29 20:36:37.469217 superbus-0.0.9/PKG-INFO
+-rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)      214 2023-12-05 13:45:14.000000 superbus-0.0.9/README.md
+-rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)      103 2023-12-04 14:53:51.000000 superbus-0.0.9/pyproject.toml
+-rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)      666 2024-03-29 20:36:37.469217 superbus-0.0.9/setup.cfg
+drwxrwxr-x   0 starrabb1t  (1000) starrabb1t  (1000)        0 2024-03-29 20:36:37.469217 superbus-0.0.9/src/
+drwxrwxr-x   0 starrabb1t  (1000) starrabb1t  (1000)        0 2024-03-29 20:36:37.469217 superbus-0.0.9/src/superbus/
+-rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)       54 2023-12-04 22:57:45.000000 superbus-0.0.9/src/superbus/__init__.py
+-rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)     2438 2024-03-29 20:34:27.000000 superbus-0.0.9/src/superbus/client.py
+-rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)     3096 2024-03-29 20:25:18.000000 superbus-0.0.9/src/superbus/updater.py
+-rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)     2448 2024-03-29 20:17:46.000000 superbus-0.0.9/src/superbus/utils.py
+-rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)     3762 2024-03-29 20:30:23.000000 superbus-0.0.9/src/superbus/worker.py
+drwxrwxr-x   0 starrabb1t  (1000) starrabb1t  (1000)        0 2024-03-29 20:36:37.469217 superbus-0.0.9/src/superbus.egg-info/
+-rw-r--r--   0 starrabb1t  (1000) starrabb1t  (1000)      783 2024-03-29 20:36:37.000000 superbus-0.0.9/src/superbus.egg-info/PKG-INFO
+-rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)      338 2024-03-29 20:36:37.000000 superbus-0.0.9/src/superbus.egg-info/SOURCES.txt
+-rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)        1 2024-03-29 20:36:37.000000 superbus-0.0.9/src/superbus.egg-info/dependency_links.txt
+-rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)       43 2024-03-29 20:36:37.000000 superbus-0.0.9/src/superbus.egg-info/requires.txt
+-rw-rw-r--   0 starrabb1t  (1000) starrabb1t  (1000)        9 2024-03-29 20:36:37.000000 superbus-0.0.9/src/superbus.egg-info/top_level.txt
```

### Comparing `superbus-0.0.8/LICENSE` & `superbus-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `superbus-0.0.8/PKG-INFO` & `superbus-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superbus
-Version: 0.0.8
+Version: 0.0.9
 Summary: redis-based bus to communicate between microservices that handle long-running tasks
 Home-page: https://github.com/starrabb1t/superbus
 Author: starrabb1t
 Author-email: berzin@phystech.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `superbus-0.0.8/setup.cfg` & `superbus-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = superbus
-version = 0.0.8
+version = 0.0.9
 author = starrabb1t
 author_email = berzin@phystech.edu
 description = redis-based bus to communicate between microservices that handle long-running tasks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/starrabb1t/superbus
 classifiers =
```

### Comparing `superbus-0.0.8/src/superbus/client.py` & `superbus-0.0.9/src/superbus/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import uuid
 from .updater import *
 
-WAIT_TIMEOUT_SEC = 300
-WAIT_POLLING_PERIOD_SEC = 1
-
 class Client:
     def __init__(
         self,
         redis_host,
         redis_port=DEFAULT_REDIS_PORT,
-        redis_password = None
+        redis_password = None,
+        logical_db=0
     ):
 
         if redis_password:
-            self._redis = redis.Redis(host=redis_host, port=redis_port, password=redis_password)
+            self._redis = redis.Redis(host=redis_host, port=redis_port, password=redis_password, db=logical_db)
         else:
-            self._redis = redis.Redis(host=redis_host, port=redis_port)
+            self._redis = redis.Redis(host=redis_host, port=redis_port, db=logical_db)
 
         self.updater = StatusUpdater(self._redis)
 
     def getTask(self, task_id: str) -> Dict:
 
         task = self.updater.get_task_by_id(task_id)    
 
@@ -28,21 +26,35 @@
 
             task = task.dict()
             task["data"] = data
             return task
               
         return task.dict()
 
+
+    def getQueue(self, workflow: List[str] = None):
+
+        queue = {}
+
+        if workflow:
+            for node in workflow:
+                queue[node] = self._redis.llen(node)
+        else:
+            for node in self._redis.smembers("REGISTERED_OPERATORS"):
+                queue[node.decode()] = self._redis.llen(node)
+
+        return queue
+
     def pushTask(
         self,
         task_data: Dict,
         workflow: List,
         wait_result=False,
-        wait_timeout = WAIT_TIMEOUT_SEC,
-        wait_polling = WAIT_POLLING_PERIOD_SEC,
+        wait_timeout = CLIENT_WAIT_TIMEOUT_SEC,
+        wait_polling = CLIENT_WAIT_POLLING_PERIOD_SEC,
         webhook=None,
     ) -> Dict:
         
         try:
 
             task = TaskModel(
                 id=uuid.uuid4().hex,
```

### Comparing `superbus-0.0.8/src/superbus/updater.py` & `superbus-0.0.9/src/superbus/updater.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import time
 from datetime import datetime
 import httpx
-import traceback
 from .utils import *
 import redis
 
-
 class StatusUpdater:
     def __init__(self, r: redis.Redis):
         self._redis = r
 
     def get_task_by_id(self, task_id: str) -> TaskModel:
 
         task = self._redis.hget("tasks", task_id)
@@ -87,11 +85,15 @@
                 return self.get_timeout(task)
 
     def send_webhook_post(self, task_dict : Dict, url : str) -> None:
         
         task_id = task_dict["id"]
         task_json = json.dumps(task_dict)
 
-        r = httpx.post(url, json=task_json)
-        logger.info(
-            f"post to webhook {url} for task '{task_id}' completed with status {r.status_code}"
-        )
+        try:
+            r = httpx.post(url, json=task_json, timeout=DEFAULT_WEBHOOK_TIMEOUT_SEC)
+            logger.info(
+                f"post to webhook {url} for task '{task_id}' completed with status {r.status_code}"
+            )
+        except httpx.TimeoutException as e:
+            logging.warning(e)
+
```

### Comparing `superbus-0.0.8/src/superbus/worker.py` & `superbus-0.0.9/src/superbus/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,81 @@
 from .updater import *
 
-WORKER_POLLING_PERIOD_SEC = 0.1
 
 class Worker:
     def __init__(
         self,
         redis_host,
         redis_port=DEFAULT_REDIS_PORT,
-        redis_password = None,
-        polling_period = WORKER_POLLING_PERIOD_SEC
+        redis_password=None,
+        polling_period=WORKER_POLLING_PERIOD_SEC,
+        logical_db=0
     ):
-        
+
         if redis_password:
-            self._redis = redis.Redis(host=redis_host, port=redis_port, password=redis_password)
+            self._redis = redis.Redis(
+                host=redis_host, port=redis_port, password=redis_password, db=logical_db)
         else:
-            self._redis = redis.Redis(host=redis_host, port=redis_port)
+            self._redis = redis.Redis(
+                host=redis_host, port=redis_port, db=logical_db)
 
         self.polling_period = polling_period
         self.updater = StatusUpdater(self._redis)
 
         logging.info("worker ready!")
+        
 
     def run(self, operators: dict):
 
         for op_name in operators:
             self._redis.sadd("REGISTERED_OPERATORS", op_name)
 
         task = None
+        terminator = Terminator()
 
-        while True:
+        while not terminator.terminate:
 
             try:
                 time.sleep(self.polling_period)
 
                 for op_name in operators:
 
                     if self._redis.llen(op_name) != 0:
 
                         task_id = self._redis.rpop(op_name)
 
                         if task_id is None:
                             continue
 
                         logger.info(f"received task '{task_id}'")
-                        
+
                         task = self.updater.get_task_by_id(task_id)
                         task_data = self.updater.get_task_data_by_id(task_id)
 
                         task.stage = op_name
                         self.updater.set_in_progress(task)
 
                         operator_func = operators[op_name]
                         result_data = operator_func(task_data)
                         result_data_json = json.dumps(result_data)
-                        
-                        self._redis.hset("task_data", task.id, result_data_json)
+
+                        self._redis.hset("task_data", task.id,
+                                         result_data_json)
                         keydb_expiremember(self._redis, "task_data", task.id)
 
                         if task.workflow.index(op_name) == len(task.workflow) - 1:
-            
+
                             self.updater.set_success(task)
                             logger.info(f"task succeeded '{task.id}'")
 
                             if task.webhook:
                                 task_dict = task.dict()
                                 task_dict["data"] = result_data
-                                self.updater.send_webhook_post(task_dict, task.webhook)
+                                self.updater.send_webhook_post(
+                                    task_dict, task.webhook)
 
                         else:
                             next_op_name = task.workflow[
                                 task.workflow.index(op_name) + 1
                             ]
                             task.stage = next_op_name
                             self.updater.set_created(task)
@@ -93,8 +99,11 @@
                     )
 
                 try:
                     if task.webhook:
                         task_dict = task.dict()
                         self.updater.send_webhook_post(task_dict, task.webhook)
                 except:
-                    logger.error(f"post to webhook failed! Traceback: {traceback.format_exc()}")
+                    logger.error(
+                        f"post to webhook failed! Traceback: {traceback.format_exc()}")
+
+        logging.info("worker terminated!")
```

### Comparing `superbus-0.0.8/src/superbus.egg-info/PKG-INFO` & `superbus-0.0.9/src/superbus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superbus
-Version: 0.0.8
+Version: 0.0.9
 Summary: redis-based bus to communicate between microservices that handle long-running tasks
 Home-page: https://github.com/starrabb1t/superbus
 Author: starrabb1t
 Author-email: berzin@phystech.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

