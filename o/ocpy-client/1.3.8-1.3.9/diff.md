# Comparing `tmp/ocpy_client-1.3.8.tar.gz` & `tmp/ocpy_client-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocpy_client-1.3.8.tar", max compression
+gzip compressed data, was "ocpy_client-1.3.9.tar", max compression
```

## Comparing `ocpy_client-1.3.8.tar` & `ocpy_client-1.3.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35149 2022-03-01 09:05:41.293930 ocpy_client-1.3.8/LICENSE
--rw-r--r--   0        0        0     5753 2024-02-07 12:35:50.977626 ocpy_client-1.3.8/ocpy/__init__.py
--rw-r--r--   0        0        0     2463 2022-07-13 07:01:42.910578 ocpy_client-1.3.8/ocpy/acl_template.xml
--rw-r--r--   0        0        0     3454 2023-05-15 13:11:22.388936 ocpy_client-1.3.8/ocpy/api/__init__.py
--rw-r--r--   0        0        0        0 2022-03-01 09:05:41.293930 ocpy_client-1.3.8/ocpy/api/admin_ui/__init__.py
--rw-r--r--   0        0        0     6174 2023-03-15 07:18:11.307002 ocpy_client-1.3.8/ocpy/api/admin_ui/attachments_info.txt
--rw-r--r--   0        0        0     9387 2024-02-07 12:35:50.978626 ocpy_client-1.3.8/ocpy/api/admin_ui/event.py
--rw-r--r--   0        0        0     3208 2024-02-07 12:35:50.978626 ocpy_client-1.3.8/ocpy/api/admin_ui/index.py
--rw-r--r--   0        0        0     1666 2023-03-15 07:18:11.308002 ocpy_client-1.3.8/ocpy/api/admin_ui/resources.py
--rw-r--r--   0        0        0     2600 2022-03-01 09:05:41.293930 ocpy_client-1.3.8/ocpy/api/admin_ui/service.py
--rw-r--r--   0        0        0    10929 2022-03-01 09:05:41.293930 ocpy_client-1.3.8/ocpy/api/admin_ui/themes.py
--rw-r--r--   0        0        0     3116 2024-03-27 09:41:35.405235 ocpy_client-1.3.8/ocpy/api/api_client.py
--rw-r--r--   0        0        0     1387 2024-02-07 12:35:50.978626 ocpy_client-1.3.8/ocpy/api/assets.py
--rw-r--r--   0        0        0        0 2022-03-01 09:05:41.293930 ocpy_client-1.3.8/ocpy/api/external/__init__.py
--rw-r--r--   0        0        0     2072 2024-02-07 12:35:50.978626 ocpy_client-1.3.8/ocpy/api/external/agents.py
--rw-r--r--   0        0        0     6741 2024-02-07 12:35:50.978626 ocpy_client-1.3.8/ocpy/api/external/base.py
--rw-r--r--   0        0        0    27924 2024-02-07 12:55:18.919865 ocpy_client-1.3.8/ocpy/api/external/events.py
--rw-r--r--   0        0        0     5111 2024-02-07 12:35:50.979626 ocpy_client-1.3.8/ocpy/api/external/groups.py
--rw-r--r--   0        0        0     3114 2024-02-07 12:35:50.979626 ocpy_client-1.3.8/ocpy/api/external/index.py
--rw-r--r--   0        0        0    13672 2024-03-27 09:45:50.101212 ocpy_client-1.3.8/ocpy/api/external/series.py
--rw-r--r--   0        0        0     5080 2024-02-07 12:35:50.979626 ocpy_client-1.3.8/ocpy/api/external/users.py
--rw-r--r--   0        0        0     8082 2024-02-07 12:35:50.979626 ocpy_client-1.3.8/ocpy/api/external/workflows.py
--rw-r--r--   0        0        0     2221 2024-03-27 09:41:35.405235 ocpy_client-1.3.8/ocpy/api/info.py
--rwxr-xr-x   0        0        0    16429 2024-03-27 09:41:35.409235 ocpy_client-1.3.8/ocpy/api/ingest.py
--rw-r--r--   0        0        0     1286 2024-03-27 09:41:35.409235 ocpy_client-1.3.8/ocpy/api/org.py
--rw-r--r--   0        0        0     9999 2024-02-07 12:35:50.980626 ocpy_client-1.3.8/ocpy/api/recordings.py
--rw-r--r--   0        0        0     4823 2024-03-27 09:41:35.409235 ocpy_client-1.3.8/ocpy/api/search.py
--rw-r--r--   0        0        0    13011 2024-03-27 09:41:35.409235 ocpy_client-1.3.8/ocpy/api/service.py
--rw-r--r--   0        0        0     1912 2024-02-07 12:35:50.981626 ocpy_client-1.3.8/ocpy/api/sign.py
--rw-r--r--   0        0        0     3424 2024-03-27 09:41:35.409235 ocpy_client-1.3.8/ocpy/api/upload.py
--rwxr-xr-x   0        0        0     4212 2024-03-27 09:41:35.409235 ocpy_client-1.3.8/ocpy/api/workflow.py
--rw-r--r--   0        0        0       36 2022-03-01 09:05:41.294931 ocpy_client-1.3.8/ocpy/model/__init__.py
--rw-r--r--   0        0        0     2376 2023-08-10 09:44:25.405564 ocpy_client-1.3.8/ocpy/model/acl.py
--rw-r--r--   0        0        0     8978 2022-03-01 09:05:41.294931 ocpy_client-1.3.8/ocpy/model/event_models.py
--rw-r--r--   0        0        0     1579 2023-05-24 07:04:52.611457 ocpy_client-1.3.8/ocpy/model/mediapackage.py
--rw-r--r--   0        0        0     1411 2022-03-01 09:05:41.294931 ocpy_client-1.3.8/ocpy/model/organization.py
--rw-r--r--   0        0        0     3257 2023-05-24 07:04:52.611457 ocpy_client-1.3.8/ocpy/model/publication.py
--rw-r--r--   0        0        0     1426 2022-07-13 07:01:42.911578 ocpy_client-1.3.8/ocpy/model/scheduling.py
--rw-r--r--   0        0        0      406 2022-03-01 09:05:41.294931 ocpy_client-1.3.8/ocpy/model/server.py
--rw-r--r--   0        0        0     2833 2023-05-16 06:58:07.889725 ocpy_client-1.3.8/ocpy/model/track.py
--rw-r--r--   0        0        0        0 2022-03-01 09:05:41.294931 ocpy_client-1.3.8/ocpy/services/__init__.py
--rw-r--r--   0        0        0      504 2022-03-01 09:05:41.294931 ocpy_client-1.3.8/ocpy/services/test.py
--rw-r--r--   0        0        0     4875 2022-07-13 07:01:42.911578 ocpy_client-1.3.8/ocpy/utils.py
--rw-r--r--   0        0        0      678 2024-03-27 09:46:11.995583 ocpy_client-1.3.8/pyproject.toml
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 ocpy_client-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-03-01 09:05:41.293930 ocpy_client-1.3.9/LICENSE
+-rw-r--r--   0        0        0     5753 2024-02-07 12:35:50.977626 ocpy_client-1.3.9/ocpy/__init__.py
+-rw-r--r--   0        0        0     2463 2022-07-13 07:01:42.910578 ocpy_client-1.3.9/ocpy/acl_template.xml
+-rw-r--r--   0        0        0     3454 2023-05-15 13:11:22.388936 ocpy_client-1.3.9/ocpy/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-01 09:05:41.293930 ocpy_client-1.3.9/ocpy/api/admin_ui/__init__.py
+-rw-r--r--   0        0        0     6174 2023-03-15 07:18:11.307002 ocpy_client-1.3.9/ocpy/api/admin_ui/attachments_info.txt
+-rw-r--r--   0        0        0     9387 2024-02-07 12:35:50.978626 ocpy_client-1.3.9/ocpy/api/admin_ui/event.py
+-rw-r--r--   0        0        0     3208 2024-02-07 12:35:50.978626 ocpy_client-1.3.9/ocpy/api/admin_ui/index.py
+-rw-r--r--   0        0        0     1666 2023-03-15 07:18:11.308002 ocpy_client-1.3.9/ocpy/api/admin_ui/resources.py
+-rw-r--r--   0        0        0     2600 2022-03-01 09:05:41.293930 ocpy_client-1.3.9/ocpy/api/admin_ui/service.py
+-rw-r--r--   0        0        0    10929 2022-03-01 09:05:41.293930 ocpy_client-1.3.9/ocpy/api/admin_ui/themes.py
+-rw-r--r--   0        0        0     3116 2024-03-27 09:41:35.405235 ocpy_client-1.3.9/ocpy/api/api_client.py
+-rw-r--r--   0        0        0     1387 2024-02-07 12:35:50.978626 ocpy_client-1.3.9/ocpy/api/assets.py
+-rw-r--r--   0        0        0        0 2022-03-01 09:05:41.293930 ocpy_client-1.3.9/ocpy/api/external/__init__.py
+-rw-r--r--   0        0        0     2072 2024-02-07 12:35:50.978626 ocpy_client-1.3.9/ocpy/api/external/agents.py
+-rw-r--r--   0        0        0     6741 2024-02-07 12:35:50.978626 ocpy_client-1.3.9/ocpy/api/external/base.py
+-rw-r--r--   0        0        0    27924 2024-02-07 12:55:18.919865 ocpy_client-1.3.9/ocpy/api/external/events.py
+-rw-r--r--   0        0        0     5111 2024-02-07 12:35:50.979626 ocpy_client-1.3.9/ocpy/api/external/groups.py
+-rw-r--r--   0        0        0     3114 2024-02-07 12:35:50.979626 ocpy_client-1.3.9/ocpy/api/external/index.py
+-rw-r--r--   0        0        0    13962 2024-03-27 14:42:06.207946 ocpy_client-1.3.9/ocpy/api/external/series.py
+-rw-r--r--   0        0        0     5080 2024-02-07 12:35:50.979626 ocpy_client-1.3.9/ocpy/api/external/users.py
+-rw-r--r--   0        0        0     8082 2024-02-07 12:35:50.979626 ocpy_client-1.3.9/ocpy/api/external/workflows.py
+-rw-r--r--   0        0        0     2221 2024-03-27 09:41:35.405235 ocpy_client-1.3.9/ocpy/api/info.py
+-rwxr-xr-x   0        0        0    16429 2024-03-27 09:41:35.409235 ocpy_client-1.3.9/ocpy/api/ingest.py
+-rw-r--r--   0        0        0     1286 2024-03-27 09:41:35.409235 ocpy_client-1.3.9/ocpy/api/org.py
+-rw-r--r--   0        0        0     9999 2024-02-07 12:35:50.980626 ocpy_client-1.3.9/ocpy/api/recordings.py
+-rw-r--r--   0        0        0     4823 2024-03-27 09:41:35.409235 ocpy_client-1.3.9/ocpy/api/search.py
+-rw-r--r--   0        0        0    13011 2024-03-27 09:41:35.409235 ocpy_client-1.3.9/ocpy/api/service.py
+-rw-r--r--   0        0        0     1912 2024-02-07 12:35:50.981626 ocpy_client-1.3.9/ocpy/api/sign.py
+-rw-r--r--   0        0        0     3424 2024-03-27 09:41:35.409235 ocpy_client-1.3.9/ocpy/api/upload.py
+-rwxr-xr-x   0        0        0     4212 2024-03-27 09:41:35.409235 ocpy_client-1.3.9/ocpy/api/workflow.py
+-rw-r--r--   0        0        0       36 2022-03-01 09:05:41.294931 ocpy_client-1.3.9/ocpy/model/__init__.py
+-rw-r--r--   0        0        0     2376 2023-08-10 09:44:25.405564 ocpy_client-1.3.9/ocpy/model/acl.py
+-rw-r--r--   0        0        0     8978 2022-03-01 09:05:41.294931 ocpy_client-1.3.9/ocpy/model/event_models.py
+-rw-r--r--   0        0        0     1579 2023-05-24 07:04:52.611457 ocpy_client-1.3.9/ocpy/model/mediapackage.py
+-rw-r--r--   0        0        0     1411 2022-03-01 09:05:41.294931 ocpy_client-1.3.9/ocpy/model/organization.py
+-rw-r--r--   0        0        0     3257 2023-05-24 07:04:52.611457 ocpy_client-1.3.9/ocpy/model/publication.py
+-rw-r--r--   0        0        0     1426 2022-07-13 07:01:42.911578 ocpy_client-1.3.9/ocpy/model/scheduling.py
+-rw-r--r--   0        0        0      406 2022-03-01 09:05:41.294931 ocpy_client-1.3.9/ocpy/model/server.py
+-rw-r--r--   0        0        0     2833 2023-05-16 06:58:07.889725 ocpy_client-1.3.9/ocpy/model/track.py
+-rw-r--r--   0        0        0        0 2022-03-01 09:05:41.294931 ocpy_client-1.3.9/ocpy/services/__init__.py
+-rw-r--r--   0        0        0      504 2022-03-01 09:05:41.294931 ocpy_client-1.3.9/ocpy/services/test.py
+-rw-r--r--   0        0        0     4875 2022-07-13 07:01:42.911578 ocpy_client-1.3.9/ocpy/utils.py
+-rw-r--r--   0        0        0      678 2024-03-27 14:42:18.145110 ocpy_client-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 ocpy_client-1.3.9/PKG-INFO
```

### Comparing `ocpy_client-1.3.8/LICENSE` & `ocpy_client-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/__init__.py` & `ocpy_client-1.3.9/ocpy/__init__.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/acl_template.xml` & `ocpy_client-1.3.9/ocpy/acl_template.xml`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/__init__.py` & `ocpy_client-1.3.9/ocpy/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/admin_ui/attachments_info.txt` & `ocpy_client-1.3.9/ocpy/api/admin_ui/attachments_info.txt`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/admin_ui/event.py` & `ocpy_client-1.3.9/ocpy/api/admin_ui/event.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/admin_ui/index.py` & `ocpy_client-1.3.9/ocpy/api/admin_ui/index.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/admin_ui/resources.py` & `ocpy_client-1.3.9/ocpy/api/admin_ui/resources.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/admin_ui/service.py` & `ocpy_client-1.3.9/ocpy/api/admin_ui/service.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/admin_ui/themes.py` & `ocpy_client-1.3.9/ocpy/api/admin_ui/themes.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/api_client.py` & `ocpy_client-1.3.9/ocpy/api/api_client.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/assets.py` & `ocpy_client-1.3.9/ocpy/api/assets.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/external/agents.py` & `ocpy_client-1.3.9/ocpy/api/external/agents.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/external/base.py` & `ocpy_client-1.3.9/ocpy/api/external/base.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/external/events.py` & `ocpy_client-1.3.9/ocpy/api/external/events.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/external/groups.py` & `ocpy_client-1.3.9/ocpy/api/external/groups.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/external/index.py` & `ocpy_client-1.3.9/ocpy/api/external/index.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/external/series.py` & `ocpy_client-1.3.9/ocpy/api/external/series.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,29 +258,37 @@
         self,
         sign=True,
         with_acl=False,
         with_metadata=False,
         with_publications=False,
         series_filter=None,
         batch_size=100,
+        print_progress=False,
         generator=False,
     ):
         result = []
+        count = 0
         while True:
+            if print_progress:
+                logger.info(
+                    f"requesting {batch_size} starting from offset {count}"
+                )
             res = self.get_series(
                 sign=sign,
                 with_acl=with_acl,
                 with_metadata=with_metadata,
                 with_publications=with_publications,
                 series_filter=series_filter,
                 limit=batch_size,
-                offset=len(result),
+                offset=count,
             )
             if res is None or len(res) <= 0:
+                logger.debug(f"DONE; got {len(result)} series")
                 break
+            count += len(res)
             if generator:
                 for r in res:
                     yield r
             else:
                 result.extend(res)
         if generator:
             return
```

### Comparing `ocpy_client-1.3.8/ocpy/api/external/users.py` & `ocpy_client-1.3.9/ocpy/api/external/users.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/external/workflows.py` & `ocpy_client-1.3.9/ocpy/api/external/workflows.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/info.py` & `ocpy_client-1.3.9/ocpy/api/info.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/ingest.py` & `ocpy_client-1.3.9/ocpy/api/ingest.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/org.py` & `ocpy_client-1.3.9/ocpy/api/org.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/recordings.py` & `ocpy_client-1.3.9/ocpy/api/recordings.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/search.py` & `ocpy_client-1.3.9/ocpy/api/search.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/service.py` & `ocpy_client-1.3.9/ocpy/api/service.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/sign.py` & `ocpy_client-1.3.9/ocpy/api/sign.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/upload.py` & `ocpy_client-1.3.9/ocpy/api/upload.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/api/workflow.py` & `ocpy_client-1.3.9/ocpy/api/workflow.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/model/acl.py` & `ocpy_client-1.3.9/ocpy/model/acl.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/model/event_models.py` & `ocpy_client-1.3.9/ocpy/model/event_models.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/model/mediapackage.py` & `ocpy_client-1.3.9/ocpy/model/mediapackage.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/model/organization.py` & `ocpy_client-1.3.9/ocpy/model/organization.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/model/publication.py` & `ocpy_client-1.3.9/ocpy/model/publication.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/model/scheduling.py` & `ocpy_client-1.3.9/ocpy/model/scheduling.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/model/track.py` & `ocpy_client-1.3.9/ocpy/model/track.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/ocpy/utils.py` & `ocpy_client-1.3.9/ocpy/utils.py`

 * *Files identical despite different names*

### Comparing `ocpy_client-1.3.8/pyproject.toml` & `ocpy_client-1.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ocpy-client"
-version = "1.3.8"
+version = "1.3.9"
 description = "Python client library to access the different APIs of OpenCast, tested with OC13.5."
 authors = ["Tobias Kurze <it@t-kurze.de>"]
 license = "GPL"
 packages = [
     { include = "ocpy" },
 ]
```

### Comparing `ocpy_client-1.3.8/PKG-INFO` & `ocpy_client-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocpy-client
-Version: 1.3.8
+Version: 1.3.9
 Summary: Python client library to access the different APIs of OpenCast, tested with OC13.5.
 License: GPL
 Author: Tobias Kurze
 Author-email: it@t-kurze.de
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

