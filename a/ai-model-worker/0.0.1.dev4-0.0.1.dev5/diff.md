# Comparing `tmp/ai_model_worker-0.0.1.dev4.tar.gz` & `tmp/ai_model_worker-0.0.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_model_worker-0.0.1.dev4.tar", max compression
+gzip compressed data, was "ai_model_worker-0.0.1.dev5.tar", max compression
```

## Comparing `ai_model_worker-0.0.1.dev4.tar` & `ai_model_worker-0.0.1.dev5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-03-28 05:12:16.751329 ai_model_worker-0.0.1.dev4/ai_model_worker/__init__.py
--rw-r--r--   0        0        0       84 2024-03-29 08:00:31.969206 ai_model_worker-0.0.1.dev4/ai_model_worker/config.py
--rw-r--r--   0        0        0        0 2024-03-29 06:43:58.407552 ai_model_worker-0.0.1.dev4/ai_model_worker/worker/__init__.py
--rw-r--r--   0        0        0     1328 2024-03-29 12:43:40.498273 ai_model_worker-0.0.1.dev4/ai_model_worker/worker/BaseWorker.py
--rw-r--r--   0        0        0      384 2024-03-29 12:44:05.805394 ai_model_worker-0.0.1.dev4/pyproject.toml
--rw-r--r--   0        0        0       73 2024-03-29 03:32:18.742397 ai_model_worker-0.0.1.dev4/README.md
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 ai_model_worker-0.0.1.dev4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-28 05:12:16.751329 ai_model_worker-0.0.1.dev5/ai_model_worker/__init__.py
+-rw-r--r--   0        0        0       84 2024-03-29 08:00:31.969206 ai_model_worker-0.0.1.dev5/ai_model_worker/config.py
+-rw-r--r--   0        0        0        0 2024-03-29 06:43:58.407552 ai_model_worker-0.0.1.dev5/ai_model_worker/worker/__init__.py
+-rw-r--r--   0        0        0     1332 2024-04-02 13:29:50.964065 ai_model_worker-0.0.1.dev5/ai_model_worker/worker/BaseWorker.py
+-rw-r--r--   0        0        0      384 2024-04-02 13:31:53.126001 ai_model_worker-0.0.1.dev5/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-03-29 03:32:18.742397 ai_model_worker-0.0.1.dev5/README.md
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 ai_model_worker-0.0.1.dev5/PKG-INFO
```

### Comparing `ai_model_worker-0.0.1.dev4/ai_model_worker/worker/BaseWorker.py` & `ai_model_worker-0.0.1.dev5/ai_model_worker/worker/BaseWorker.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from abc import ABC, abstractmethod
 
 from ai_model_worker.config import AMQP_URL
 
 
 class BaseWorker(ABC):
 
-    def __init__(self, model_name, callback):
+    def __init__(self, model_name, work_func):
         self.model_name = model_name
-        self.callback = callback
+        self.work_func = work_func
         self.connection = pika.BlockingConnection(pika.URLParameters(AMQP_URL))
         self.channel = self.connection.channel()
         self.channel.queue_declare(queue=model_name)
         self.startup()
 
     def get_worker_name(self) -> str:
         return self.__class__.__name__
@@ -26,15 +26,15 @@
     @abstractmethod
     def shutdown(self) -> None:
         pass
 
     def on_request(self, ch, method, props, body):
         print(f"body : {body}")
 
-        response = self.callback(body)
+        response = self.work_func(body)
 
         ch.basic_publish(exchange='',
                          routing_key=props.reply_to,
                          properties=pika.BasicProperties(correlation_id=props.correlation_id),
                          body=json.dumps(response))
         ch.basic_ack(delivery_tag=method.delivery_tag)
```

