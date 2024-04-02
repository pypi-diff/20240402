# Comparing `tmp/rab_the_bit-0.0.92.tar.gz` & `tmp/rab_the_bit-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rab_the_bit-0.0.92.tar", max compression
+gzip compressed data, was "rab_the_bit-0.0.93.tar", max compression
```

## Comparing `rab_the_bit-0.0.92.tar` & `rab_the_bit-0.0.93.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1090 2024-03-27 17:26:53.714162 rab_the_bit-0.0.92/LICENSE
--rw-r--r--   0        0        0     2315 2024-03-27 17:26:53.714162 rab_the_bit-0.0.92/README.rst
--rw-r--r--   0        0        0     1387 2024-03-27 17:26:53.714162 rab_the_bit-0.0.92/pyproject.toml
--rw-r--r--   0        0        0      182 2024-03-27 17:26:53.714162 rab_the_bit-0.0.92/rab_the_bit/__init__.py
--rw-r--r--   0        0        0       83 2024-03-27 17:26:53.714162 rab_the_bit-0.0.92/rab_the_bit/__version__.py
--rw-r--r--   0        0        0    11860 2024-03-27 17:26:53.714162 rab_the_bit-0.0.92/rab_the_bit/rab_the_bit.py
--rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 rab_the_bit-0.0.92/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-04-02 13:55:33.601821 rab_the_bit-0.0.93/LICENSE
+-rw-r--r--   0        0        0     2315 2024-04-02 13:55:33.601821 rab_the_bit-0.0.93/README.rst
+-rw-r--r--   0        0        0     1387 2024-04-02 13:55:33.601821 rab_the_bit-0.0.93/pyproject.toml
+-rw-r--r--   0        0        0      182 2024-04-02 13:55:33.601821 rab_the_bit-0.0.93/rab_the_bit/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-02 13:55:33.601821 rab_the_bit-0.0.93/rab_the_bit/__version__.py
+-rw-r--r--   0        0        0    11864 2024-04-02 13:55:33.601821 rab_the_bit-0.0.93/rab_the_bit/rab_the_bit.py
+-rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 rab_the_bit-0.0.93/PKG-INFO
```

### Comparing `rab_the_bit-0.0.92/LICENSE` & `rab_the_bit-0.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `rab_the_bit-0.0.92/README.rst` & `rab_the_bit-0.0.93/README.rst`

 * *Files identical despite different names*

### Comparing `rab_the_bit-0.0.92/pyproject.toml` & `rab_the_bit-0.0.93/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rab_the_bit"
-version = "0.0.92"
+version = "0.0.93"
 description = "A wrapper around Kombu to use RabbitMQ, specialy on docker images"
 authors = ["Vlaams Instituut voor de Zee (VLIZ), João Santos <jotaflame@gmail.com>"]
 readme = "README.rst"
 packages = [{include = "rab_the_bit"}]
 license = "MIT"
 
 repository = "https://github.com/vliz-be-opsci/py-rabbit"
```

### Comparing `rab_the_bit-0.0.92/rab_the_bit/rab_the_bit.py` & `rab_the_bit-0.0.93/rab_the_bit/rab_the_bit.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self,
         amqp_url,
         exchange_name,
         # queue_name,
         # routing_key,
         connection_args={},
         exchange_args={"type": "topic"},
-        queue_args={},
+        # queue_args={},
         log=None,
         errback=None,
     ):
         """
         Initializes the RabbitProducer with the given parameters.
 
         :param amqp_url: The URL for the AMQP server.
@@ -66,15 +66,15 @@
     def send_message(self, message, routing_key):
         """
         Sends a message to the queue with the given routing key.
 
         :param message: The message to send.
         :param routing_key: The routing key for the message.
         """
-        self.queue.routing_key = routing_key
+        # self.queue.routing_key = routing_key
         # self.queue.declare()
         with self.connection.Producer() as producer:
             producer.publish(
                 message,
                 exchange=self.exchange,
                 routing_key=routing_key,
                 # declare=[self.queue],
```

### Comparing `rab_the_bit-0.0.92/PKG-INFO` & `rab_the_bit-0.0.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rab_the_bit
-Version: 0.0.92
+Version: 0.0.93
 Summary: A wrapper around Kombu to use RabbitMQ, specialy on docker images
 Home-page: https://github.com/vliz-be-opsci/py-rabbit
 License: MIT
 Author: Vlaams Instituut voor de Zee (VLIZ), João Santos
 Author-email: jotaflame@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

