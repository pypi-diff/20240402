# Comparing `tmp/aiospb-3.0.2.tar.gz` & `tmp/aiospb-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiospb-3.0.2.tar", max compression
+gzip compressed data, was "aiospb-3.0.3.tar", max compression
```

## Comparing `aiospb-3.0.2.tar` & `aiospb-3.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6189 2024-02-15 15:15:58.185081 aiospb-3.0.2/README.md
--rw-r--r--   0        0        0      691 2024-03-30 10:36:42.009590 aiospb-3.0.2/aiospb/__init__.py
--rw-r--r--   0        0        0     7387 2024-03-30 17:37:06.742476 aiospb-3.0.2/aiospb/data.py
--rw-r--r--   0        0        0     2916 2024-03-20 12:16:36.181503 aiospb-3.0.2/aiospb/groups.py
--rw-r--r--   0        0        0     4810 2024-03-30 10:36:42.009590 aiospb-3.0.2/aiospb/hosts.py
--rw-r--r--   0        0        0     5124 2024-03-30 18:34:00.952951 aiospb-3.0.2/aiospb/messages.py
--rw-r--r--   0        0        0     1308 2024-03-30 10:36:42.009590 aiospb-3.0.2/aiospb/mqtt/__init__.py
--rw-r--r--   0        0        0      491 2024-03-30 10:36:42.016256 aiospb-3.0.2/aiospb/mqtt/encoding.py
--rw-r--r--   0        0        0     2399 2024-03-30 18:40:15.880336 aiospb-3.0.2/aiospb/mqtt/paho.py
--rw-r--r--   0        0        0    13552 2024-03-30 17:53:30.462637 aiospb-3.0.2/aiospb/nodes.py
--rw-r--r--   0        0        0     1003 2024-03-30 18:39:36.093947 aiospb-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     6643 1970-01-01 00:00:00.000000 aiospb-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6189 2024-02-15 15:15:58.185081 aiospb-3.0.3/README.md
+-rw-r--r--   0        0        0      691 2024-03-30 10:36:42.009590 aiospb-3.0.3/aiospb/__init__.py
+-rw-r--r--   0        0        0     7387 2024-03-30 17:37:06.742476 aiospb-3.0.3/aiospb/data.py
+-rw-r--r--   0        0        0     2916 2024-03-20 12:16:36.181503 aiospb-3.0.3/aiospb/groups.py
+-rw-r--r--   0        0        0     4810 2024-03-30 10:36:42.009590 aiospb-3.0.3/aiospb/hosts.py
+-rw-r--r--   0        0        0     5124 2024-03-30 18:34:00.952951 aiospb-3.0.3/aiospb/messages.py
+-rw-r--r--   0        0        0     1308 2024-03-30 10:36:42.009590 aiospb-3.0.3/aiospb/mqtt/__init__.py
+-rw-r--r--   0        0        0      491 2024-03-30 10:36:42.016256 aiospb-3.0.3/aiospb/mqtt/encoding.py
+-rw-r--r--   0        0        0     2399 2024-03-30 18:40:15.880336 aiospb-3.0.3/aiospb/mqtt/paho.py
+-rw-r--r--   0        0        0    14048 2024-04-02 05:19:24.738030 aiospb-3.0.3/aiospb/nodes.py
+-rw-r--r--   0        0        0     1003 2024-04-02 04:56:14.960888 aiospb-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6643 1970-01-01 00:00:00.000000 aiospb-3.0.3/PKG-INFO
```

### Comparing `aiospb-3.0.2/README.md` & `aiospb-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aiospb-3.0.2/aiospb/__init__.py` & `aiospb-3.0.3/aiospb/__init__.py`

 * *Files identical despite different names*

### Comparing `aiospb-3.0.2/aiospb/data.py` & `aiospb-3.0.3/aiospb/data.py`

 * *Files identical despite different names*

### Comparing `aiospb-3.0.2/aiospb/groups.py` & `aiospb-3.0.3/aiospb/groups.py`

 * *Files identical despite different names*

### Comparing `aiospb-3.0.2/aiospb/hosts.py` & `aiospb-3.0.3/aiospb/hosts.py`

 * *Files identical despite different names*

### Comparing `aiospb-3.0.2/aiospb/messages.py` & `aiospb-3.0.3/aiospb/messages.py`

 * *Files identical despite different names*

### Comparing `aiospb-3.0.2/aiospb/mqtt/__init__.py` & `aiospb-3.0.3/aiospb/mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `aiospb-3.0.2/aiospb/mqtt/paho.py` & `aiospb-3.0.3/aiospb/mqtt/paho.py`

 * *Files identical despite different names*

### Comparing `aiospb-3.0.2/aiospb/nodes.py` & `aiospb-3.0.3/aiospb/nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -224,15 +224,20 @@
     async def _scan_metrics(self):
         scan_rate = int(self._inner_metrics["Node Control/Scan Rate"].value)
         while True and scan_rate:
             now = self._clock.now()
             next_scan_time = (now // scan_rate + 1) * scan_rate
             await self._clock.asleep((next_scan_time - now) / 1000)
 
-            metrics = await self._driver.scan_metrics()
+            try:
+                metrics = await self._driver.scan_metrics()
+            except Exception as e:
+                logger.error(f"Scanning task stopped at {self._name} by an exception")
+                logger.exception(e)
+                raise e
 
             changes = []
             for metric in metrics:
                 old_metric = self._metrics_by_name[metric.name]
                 change = old_metric.compare(metric)
                 if change:
                     self._add_metric(metric)
@@ -254,15 +259,20 @@
             else:
                 logger.debug(f"{self._name} is storing changes in historical")
                 await self._historical_store.save(changes)
 
     async def _handle_incomming_messages(self):
         while True:
             message: m.Message = await self._client.deliver_message()
-            await self._handle_content(message.content)
+            try:
+                await self._handle_content(message.content)
+            except Exception as e:
+                logger.error(f"Error handling incoming at {self._name}")
+                logger.exception(e)
+                raise e
 
     @singledispatchmethod
     async def _handle_content(self, content: m.MessageContent):
         raise NotImplementedError(
             f"Content type {type(content)} is not managed by a Edge Node"
         )
 
@@ -276,15 +286,14 @@
 
     @_handle_content.register
     async def _handle_command_content(self, content: m.NcmdContent):
         logger.debug(f"{self._name} has recieved command {content}")
         for request in content.requests:
             if request.metric_name == "Node Control/Rebirth" and request.value is True:
                 self._state = "online"  # Stops sending data
-                # topic = f"spBv1.0/{self.group_name}/NDATA/{self.name}"
                 await self._client.publish(
                     m.Message.create(
                         self._name,
                         m.NdataContent(
                             self._get_seq(),
                             [
                                 MetricChange(
@@ -305,15 +314,21 @@
                 await self.terminate_session()
                 await self.establish_session()
             else:
                 loop = asyncio.get_event_loop()
                 loop.create_task(self._process_metric_change(request))
 
     async def _process_metric_change(self, request: MetricChangeRequest):
-        change = await self._driver.write_metric(request)
+        try:
+            change = await self._driver.write_metric(request)
+        except Exception as e:
+            logger.error(f"Error writing change at {self._name}, stopping")
+            logger.exception(e)
+            raise e
+
         logger.debug(f"{self._name} has procesed change {change}")
 
         metric = (
             self._metrics_by_alias[change.alias]
             if change.alias
             else self._metrics_by_name[change.metric_name]
         )
```

### Comparing `aiospb-3.0.2/pyproject.toml` & `aiospb-3.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiospb"
-version = "3.0.2"
+version = "3.0.3"
 description = "Library to comunicate with MQTT following Sparkplug B estandard"
 authors = ["Salvador Ruiz <sruiz@indoorclima.com>"]
 license = "LGPL"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `aiospb-3.0.2/PKG-INFO` & `aiospb-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiospb
-Version: 3.0.2
+Version: 3.0.3
 Summary: Library to comunicate with MQTT following Sparkplug B estandard
 License: LGPL
 Author: Salvador Ruiz
 Author-email: sruiz@indoorclima.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

