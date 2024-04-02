# Comparing `tmp/webthing_client-0.2.6.tar.gz` & `tmp/webthing_client-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webthing_client-0.2.6.tar", max compression
+gzip compressed data, was "webthing_client-0.2.7.tar", max compression
```

## Comparing `webthing_client-0.2.6.tar` & `webthing_client-0.2.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1649 2023-02-06 09:57:29.936975 webthing_client-0.2.6/LICENSE
--rw-r--r--   0        0        0      629 2024-03-20 08:04:47.252005 webthing_client-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      325 2023-09-01 06:19:20.858836 webthing_client-0.2.6/README.md
--rw-r--r--   0        0        0        0 2023-09-01 06:19:20.859837 webthing_client-0.2.6/webthing_client/__init__.py
--rw-r--r--   0        0        0    23693 2024-03-19 09:38:14.081023 webthing_client-0.2.6/webthing_client/client.py
--rw-r--r--   0        0        0     1110 2024-02-25 09:18:17.801821 webthing_client-0.2.6/webthing_client/input/action/event_input.py
--rw-r--r--   0        0        0      559 2024-02-25 09:18:25.339336 webthing_client-0.2.6/webthing_client/input/action/event_type_input.py
--rw-r--r--   0        0        0      552 2024-02-28 12:31:21.667211 webthing_client-0.2.6/webthing_client/input/action/from_to_user_input.py
--rw-r--r--   0        0        0      335 2024-02-25 09:18:47.773047 webthing_client-0.2.6/webthing_client/input/action/iri_user_input.py
--rw-r--r--   0        0        0      958 2024-02-25 09:50:00.172735 webthing_client-0.2.6/webthing_client/input/action/resolution_input.py
--rw-r--r--   0        0        0      501 2024-02-28 12:31:21.674209 webthing_client-0.2.6/webthing_client/input/from_to_input.py
--rw-r--r--   0        0        0      284 2024-02-25 09:17:40.428692 webthing_client-0.2.6/webthing_client/input/iri_input.py
--rw-r--r--   0        0        0      573 2024-02-29 08:15:42.300381 webthing_client-0.2.6/webthing_client/input/property_observations_input.py
--rw-r--r--   0        0        0     1497 2024-03-07 08:08:34.615412 webthing_client-0.2.6/webthing_client/model/action/action.py
--rw-r--r--   0        0        0      483 2024-02-25 08:39:10.164817 webthing_client-0.2.6/webthing_client/model/action/base.py
--rw-r--r--   0        0        0     5769 2024-03-07 08:10:40.389847 webthing_client-0.2.6/webthing_client/model/action/operation/operation.py
--rw-r--r--   0        0        0     1354 2024-03-07 08:09:59.699008 webthing_client-0.2.6/webthing_client/model/action/request.py
--rw-r--r--   0        0        0     2371 2024-03-07 08:10:15.315997 webthing_client-0.2.6/webthing_client/model/action/resolution.py
--rw-r--r--   0        0        0     2576 2024-03-08 10:35:26.561490 webthing_client-0.2.6/webthing_client/model/event/event.py
--rw-r--r--   0        0        0     2167 2024-03-07 08:11:29.041992 webthing_client-0.2.6/webthing_client/model/event/event_type.py
--rw-r--r--   0        0        0     1078 2024-02-25 09:10:43.844340 webthing_client-0.2.6/webthing_client/model/event/feedback.py
--rw-r--r--   0        0        0     2792 2024-03-07 14:05:26.244036 webthing_client-0.2.6/webthing_client/model/event/feedback_schema.py
--rw-r--r--   0        0        0      845 2024-02-28 12:31:21.667211 webthing_client-0.2.6/webthing_client/model/event/observation.py
--rw-r--r--   0        0        0     1276 2024-02-23 16:53:39.147090 webthing_client-0.2.6/webthing_client/model/event/stimulus.py
--rw-r--r--   0        0        0      125 2024-03-07 08:09:17.428059 webthing_client-0.2.6/webthing_client/model/ontology.py
--rw-r--r--   0        0        0      591 2024-02-29 09:01:40.135207 webthing_client-0.2.6/webthing_client/model/property/observable_property.py
--rw-r--r--   0        0        0      871 2024-02-25 08:42:01.491567 webthing_client-0.2.6/webthing_client/model/system/sensor.py
--rw-r--r--   0        0        0      890 2024-02-25 08:41:34.495865 webthing_client-0.2.6/webthing_client/model/system/system.py
--rw-r--r--   0        0        0     1635 2024-03-07 08:12:27.305511 webthing_client-0.2.6/webthing_client/model/user/user.py
--rw-r--r--   0        0        0      900 2024-02-28 12:31:21.670210 webthing_client-0.2.6/webthing_client/model/webthing_observation.py
--rw-r--r--   0        0        0        0 2021-11-19 14:10:06.477733 webthing_client-0.2.6/webthing_client/standard_api/__init__.py
--rw-r--r--   0        0        0     9996 2023-06-07 11:34:51.827080 webthing_client-0.2.6/webthing_client/standard_api/api_handler.py
--rw-r--r--   0        0        0     1651 2021-11-29 12:35:22.731824 webthing_client-0.2.6/webthing_client/standard_api/api_marshalling.py
--rw-r--r--   0        0        0     6354 2024-03-20 12:02:38.241459 webthing_client-0.2.6/webthing_client/stomp.py
--rw-r--r--   0        0        0     1552 2024-03-05 12:21:27.646974 webthing_client-0.2.6/webthing_client/utils.py
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 webthing_client-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1649 2023-02-06 09:57:29.936975 webthing_client-0.2.7/LICENSE
+-rw-r--r--   0        0        0      629 2024-04-02 11:11:27.210775 webthing_client-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-09-01 06:19:20.858836 webthing_client-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2023-09-01 06:19:20.859837 webthing_client-0.2.7/webthing_client/__init__.py
+-rw-r--r--   0        0        0    24696 2024-04-02 09:28:40.558278 webthing_client-0.2.7/webthing_client/client.py
+-rw-r--r--   0        0        0     1110 2024-02-25 09:18:17.801821 webthing_client-0.2.7/webthing_client/input/action/event_input.py
+-rw-r--r--   0        0        0      559 2024-02-25 09:18:25.339336 webthing_client-0.2.7/webthing_client/input/action/event_type_input.py
+-rw-r--r--   0        0        0      552 2024-02-28 12:31:21.667211 webthing_client-0.2.7/webthing_client/input/action/from_to_user_input.py
+-rw-r--r--   0        0        0      335 2024-02-25 09:18:47.773047 webthing_client-0.2.7/webthing_client/input/action/iri_user_input.py
+-rw-r--r--   0        0        0      958 2024-02-25 09:50:00.172735 webthing_client-0.2.7/webthing_client/input/action/resolution_input.py
+-rw-r--r--   0        0        0      501 2024-02-28 12:31:21.674209 webthing_client-0.2.7/webthing_client/input/from_to_input.py
+-rw-r--r--   0        0        0      284 2024-02-25 09:17:40.428692 webthing_client-0.2.7/webthing_client/input/iri_input.py
+-rw-r--r--   0        0        0      573 2024-02-29 08:15:42.300381 webthing_client-0.2.7/webthing_client/input/property_observations_input.py
+-rw-r--r--   0        0        0     1497 2024-03-07 08:08:34.615412 webthing_client-0.2.7/webthing_client/model/action/action.py
+-rw-r--r--   0        0        0      483 2024-02-25 08:39:10.164817 webthing_client-0.2.7/webthing_client/model/action/base.py
+-rw-r--r--   0        0        0     5769 2024-03-07 08:10:40.389847 webthing_client-0.2.7/webthing_client/model/action/operation/operation.py
+-rw-r--r--   0        0        0     1354 2024-03-07 08:09:59.699008 webthing_client-0.2.7/webthing_client/model/action/request.py
+-rw-r--r--   0        0        0     2303 2024-04-02 09:37:23.149678 webthing_client-0.2.7/webthing_client/model/action/resolution.py
+-rw-r--r--   0        0        0     2576 2024-03-08 10:35:26.561490 webthing_client-0.2.7/webthing_client/model/event/event.py
+-rw-r--r--   0        0        0     2167 2024-03-07 08:11:29.041992 webthing_client-0.2.7/webthing_client/model/event/event_type.py
+-rw-r--r--   0        0        0     1078 2024-02-25 09:10:43.844340 webthing_client-0.2.7/webthing_client/model/event/feedback.py
+-rw-r--r--   0        0        0     2792 2024-03-07 14:05:26.244036 webthing_client-0.2.7/webthing_client/model/event/feedback_schema.py
+-rw-r--r--   0        0        0      845 2024-02-28 12:31:21.667211 webthing_client-0.2.7/webthing_client/model/event/observation.py
+-rw-r--r--   0        0        0     1276 2024-02-23 16:53:39.147090 webthing_client-0.2.7/webthing_client/model/event/stimulus.py
+-rw-r--r--   0        0        0      125 2024-03-07 08:09:17.428059 webthing_client-0.2.7/webthing_client/model/ontology.py
+-rw-r--r--   0        0        0      591 2024-02-29 09:01:40.135207 webthing_client-0.2.7/webthing_client/model/property/observable_property.py
+-rw-r--r--   0        0        0      871 2024-02-25 08:42:01.491567 webthing_client-0.2.7/webthing_client/model/system/sensor.py
+-rw-r--r--   0        0        0      890 2024-02-25 08:41:34.495865 webthing_client-0.2.7/webthing_client/model/system/system.py
+-rw-r--r--   0        0        0     1635 2024-03-07 08:12:27.305511 webthing_client-0.2.7/webthing_client/model/user/user.py
+-rw-r--r--   0        0        0      900 2024-02-28 12:31:21.670210 webthing_client-0.2.7/webthing_client/model/webthing_observation.py
+-rw-r--r--   0        0        0        0 2021-11-19 14:10:06.477733 webthing_client-0.2.7/webthing_client/standard_api/__init__.py
+-rw-r--r--   0        0        0     9996 2023-06-07 11:34:51.827080 webthing_client-0.2.7/webthing_client/standard_api/api_handler.py
+-rw-r--r--   0        0        0     1651 2021-11-29 12:35:22.731824 webthing_client-0.2.7/webthing_client/standard_api/api_marshalling.py
+-rw-r--r--   0        0        0     6354 2024-03-20 12:02:38.241459 webthing_client-0.2.7/webthing_client/stomp.py
+-rw-r--r--   0        0        0     1552 2024-03-05 12:21:27.646974 webthing_client-0.2.7/webthing_client/utils.py
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 webthing_client-0.2.7/PKG-INFO
```

### Comparing `webthing_client-0.2.6/LICENSE` & `webthing_client-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/pyproject.toml` & `webthing_client-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webthing-client"
-version = "0.2.6"
+version = "0.2.7"
 description = "Client for the Dynamic Dashboard Webthings"
 authors = ["Emile Deman"]
 maintainers = [
     "Emile Deman <emile.deman@ugent.be>",
 	"Stef Pletinck <s@stefpletinck.be>"
 ]
 readme = "README.md"
```

### Comparing `webthing_client-0.2.6/webthing_client/client.py` & `webthing_client-0.2.7/webthing_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         """Get event with view as user set in client.
 
         Args:
             event_iri (str): The IRI
         Returns:
             Event: Event.
         """
-        return self.get_event_user_view(self._user_iri)
+        return self.get_event_user_view(self._user_iri, event_iri)
     
     def get_events(self, from_: Optional[datetime]=None, to: Optional[datetime]=None) -> List[Event]:
         """Get all events in optional range.
 
         Args:
             from_ (Optional[datetime], optional): From time. Defaults to None.
             to (Optional[datetime], optional): To time. Defaults to None.
@@ -350,14 +350,36 @@
         Returns:
             List[Request[Any, Operation]]: All linked requests.
         """
         json_array: List[Dict[str, Any]] = self._api_requester.call('get_requests_resource',
             IRIInput.to_json_object(resource_iri))
         return [Request.from_json_object(request_object) for request_object in json_array]
     
+    def get_unresolved_requests(self) -> List[Request[Any, Operation]]:
+        """Get all unresolved requests.
+
+        Returns:
+            List[Request[Any, Operation]]: All unresolved requests.
+        """
+        json_array: List[Dict[str, Any]] = self._api_requester.call('get_unresolved_requests')
+        return [Request.from_json_object(request_object) for request_object in json_array]
+    
+    def get_unresolved_requests_resource(self, resource_iri: str) -> List[Request[Any, Operation]]:
+        """Get all unresolved requests linked to resource IRI.
+
+        Args:
+            resource_iri (str): The IRI of the resource.
+
+        Returns:
+            List[Request[Any, Operation]]: All linked unresolved requests.
+        """
+        json_array: List[Dict[str, Any]] = self._api_requester.call('get_unresolved_requests_resource',
+            IRIInput.to_json_object(resource_iri))
+        return [Request.from_json_object(request_object) for request_object in json_array]
+    
     def get_action(self, action_iri: str) -> Action:
         """Get the Action by IRI.
 
         Args:
             action_iri (str): Action IRI.
 
         Returns:
```

### Comparing `webthing_client-0.2.6/webthing_client/input/action/event_input.py` & `webthing_client-0.2.7/webthing_client/input/action/event_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/input/action/event_type_input.py` & `webthing_client-0.2.7/webthing_client/input/action/event_type_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/input/action/from_to_user_input.py` & `webthing_client-0.2.7/webthing_client/input/action/from_to_user_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/input/action/resolution_input.py` & `webthing_client-0.2.7/webthing_client/input/action/resolution_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/input/property_observations_input.py` & `webthing_client-0.2.7/webthing_client/input/property_observations_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/action/action.py` & `webthing_client-0.2.7/webthing_client/model/action/action.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/action/operation/operation.py` & `webthing_client-0.2.7/webthing_client/model/action/operation/operation.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/action/request.py` & `webthing_client-0.2.7/webthing_client/model/action/request.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/action/resolution.py` & `webthing_client-0.2.7/webthing_client/model/action/resolution.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations # Allow referencing enclosing class in typings
 from datetime import datetime
 from enum import Enum
 from typing import *
 
 from webthing_client import utils
 from ..ontology import WETHING_ONTOLOGY_PREFIX
-from .request import Request
 from .base import Base
 
 
 class Resolution(Base):
 
     type: ClassVar[str] = WETHING_ONTOLOGY_PREFIX + 'Resolution'
 
@@ -20,15 +19,15 @@
 
     def __init__(self, iri: str, result_time: datetime, user_iri: str, verdicts: List[Verdict], action_iri: Optional[str]) -> None:
         super().__init__(iri, result_time, user_iri)
         self.verdicts = verdicts
         self.action_iri = action_iri
     
     @classmethod
-    def from_json_object(cls, json_object: Dict[str, Any]) -> Request:
+    def from_json_object(cls, json_object: Dict[str, Any]) -> Resolution:
         return cls(
             json_object['$iri'],
             utils.parse_iso_time_format(json_object['resultTime']),
             json_object['user'],
             [Verdict.from_json_object(verdict) for verdict in json_object['verdict']],
             json_object.get('action')
         )
@@ -54,26 +53,26 @@
     type: ClassVar[str] = WETHING_ONTOLOGY_PREFIX + 'Verdict'
 
     iri: ClassVar[str] = None
 
 
     verdict_result: VerdictResultType
 
-    request: Request[Any]
+    request_iri: str
 
-    def __init__(self, verdict_result: VerdictResultType, request: Request[Any]) -> None:
+    def __init__(self, verdict_result: VerdictResultType, request_iri: str) -> None:
         self.verdict_result = verdict_result
-        self.request = request
+        self.request_iri = request_iri
 
     @classmethod
-    def from_json_object(cls, json_object: Dict[str, Any]) -> Request:
+    def from_json_object(cls, json_object: Dict[str, Any]) -> Verdict:
         return cls(
             json_object['verdictResult'],
-            Request.from_json_object(json_object['request'])
+            json_object['request']
         )
     
     def to_json_object(self) -> Dict[str, Any]:
         return {
             '$class': self.type,
             '$iri': self.iri,
-            'request': self.request.to_json_object()
+            'request': self.request_iri
         }
```

### Comparing `webthing_client-0.2.6/webthing_client/model/event/event.py` & `webthing_client-0.2.7/webthing_client/model/event/event.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/event/event_type.py` & `webthing_client-0.2.7/webthing_client/model/event/event_type.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/event/feedback.py` & `webthing_client-0.2.7/webthing_client/model/event/feedback.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/event/feedback_schema.py` & `webthing_client-0.2.7/webthing_client/model/event/feedback_schema.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/event/observation.py` & `webthing_client-0.2.7/webthing_client/model/event/observation.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/event/stimulus.py` & `webthing_client-0.2.7/webthing_client/model/event/stimulus.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/property/observable_property.py` & `webthing_client-0.2.7/webthing_client/model/property/observable_property.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/system/sensor.py` & `webthing_client-0.2.7/webthing_client/model/system/sensor.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/system/system.py` & `webthing_client-0.2.7/webthing_client/model/system/system.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/user/user.py` & `webthing_client-0.2.7/webthing_client/model/user/user.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/model/webthing_observation.py` & `webthing_client-0.2.7/webthing_client/model/webthing_observation.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/standard_api/api_handler.py` & `webthing_client-0.2.7/webthing_client/standard_api/api_handler.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/standard_api/api_marshalling.py` & `webthing_client-0.2.7/webthing_client/standard_api/api_marshalling.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/stomp.py` & `webthing_client-0.2.7/webthing_client/stomp.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/webthing_client/utils.py` & `webthing_client-0.2.7/webthing_client/utils.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.6/PKG-INFO` & `webthing_client-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webthing-client
-Version: 0.2.6
+Version: 0.2.7
 Summary: Client for the Dynamic Dashboard Webthings
 Home-page: https://github.com/predict-idlab/webthing-client-python
 Author: Emile Deman
 Maintainer: Emile Deman
 Maintainer-email: emile.deman@ugent.be
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

