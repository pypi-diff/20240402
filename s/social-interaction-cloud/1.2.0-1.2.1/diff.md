# Comparing `tmp/social_interaction_cloud-1.2.0.tar.gz` & `tmp/social_interaction_cloud-1.2.1.tar.gz`

## Comparing `social_interaction_cloud-1.2.0.tar` & `social_interaction_cloud-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.0/src/social_interaction_cloud/__init__.py
--rw-r--r--   0        0        0    41166 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.0/src/social_interaction_cloud/abstract_connector.py
--rw-r--r--   0        0        0    44875 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.0/src/social_interaction_cloud/basic_connector.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.0/src/social_interaction_cloud/choregraphe_to_json.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.0/src/social_interaction_cloud/detection_result_pb2.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.0/src/social_interaction_cloud/tracking_result_pb2.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.0/LICENSE
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.0/README.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.1/src/social_interaction_cloud/__init__.py
+-rw-r--r--   0        0        0    41181 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.1/src/social_interaction_cloud/abstract_connector.py
+-rw-r--r--   0        0        0    44875 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.1/src/social_interaction_cloud/basic_connector.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.1/src/social_interaction_cloud/choregraphe_to_json.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.1/src/social_interaction_cloud/detection_result_pb2.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.1/src/social_interaction_cloud/tracking_result_pb2.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.1/LICENSE
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.1/README.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.1/PKG-INFO
```

### Comparing `social_interaction_cloud-1.2.0/src/social_interaction_cloud/abstract_connector.py` & `social_interaction_cloud-1.2.1/src/social_interaction_cloud/abstract_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -721,17 +721,17 @@
                 pipe.publish(name, cam)
         elif name == 'intent_detection' or name == 'sentiment_analysis':
             for mic in self.devices[self.device_types['mic']]:
                 pipe.publish(name, mic)
         elif name == 'text_to_speech':
             for speaker in self.devices[self.device_types['speaker']]:
                 pipe.publish(name, speaker)
-        elif name == 'robot_memory':
-            for memory in self.devices[self.device_types['robot']]:
-                pipe.publish(name, memory)
+        elif name == 'robot_memory' or name == 'llm':
+            for robot in self.devices[self.device_types['robot']]:
+                pipe.publish(name, robot)
         else:
             print('Unknown service: ' + name)
         pipe.execute()
 
     def start(self) -> None:
         """Start the application"""
         self.__running = True
```

### Comparing `social_interaction_cloud-1.2.0/src/social_interaction_cloud/basic_connector.py` & `social_interaction_cloud-1.2.1/src/social_interaction_cloud/basic_connector.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.0/src/social_interaction_cloud/choregraphe_to_json.py` & `social_interaction_cloud-1.2.1/src/social_interaction_cloud/choregraphe_to_json.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.0/src/social_interaction_cloud/detection_result_pb2.py` & `social_interaction_cloud-1.2.1/src/social_interaction_cloud/detection_result_pb2.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.0/src/social_interaction_cloud/tracking_result_pb2.py` & `social_interaction_cloud-1.2.1/src/social_interaction_cloud/tracking_result_pb2.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.0/LICENSE` & `social_interaction_cloud-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.0/pyproject.toml` & `social_interaction_cloud-1.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "social_interaction_cloud"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Mike Ligthart", email="m.e.u.ligthart@vu.nl" },
 ]
 description = "Connector to the Social Interaction Cloud"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `social_interaction_cloud-1.2.0/PKG-INFO` & `social_interaction_cloud-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: social_interaction_cloud
-Version: 1.2.0
+Version: 1.2.1
 Summary: Connector to the Social Interaction Cloud
 Project-URL: Source, https://bitbucket.org/socialroboticshub/connectors/src/master/python/sic/
 Project-URL: Wiki, https://socialrobotics.atlassian.net/wiki/spaces/CBSR/overview
 Author-email: Mike Ligthart <m.e.u.ligthart@vu.nl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

