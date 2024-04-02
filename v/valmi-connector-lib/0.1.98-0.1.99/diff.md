# Comparing `tmp/valmi_connector_lib-0.1.98.tar.gz` & `tmp/valmi_connector_lib-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valmi_connector_lib-0.1.98.tar", max compression
+gzip compressed data, was "valmi_connector_lib-0.1.99.tar", max compression
```

## Comparing `valmi_connector_lib-0.1.98.tar` & `valmi_connector_lib-0.1.99.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        0 2023-05-18 14:12:43.011582 valmi_connector_lib-0.1.98/README.md
--rw-r--r--   0        0        0     1661 2023-08-28 16:47:08.022253 valmi_connector_lib-0.1.98/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-18 14:12:43.012354 valmi_connector_lib-0.1.98/valmi_connector_lib/__init__.py
--rw-r--r--   0        0        0        0 2023-08-21 15:41:28.501761 valmi_connector_lib-0.1.98/valmi_connector_lib/common/__init__.py
--rw-r--r--   0        0        0       25 2023-08-22 12:52:39.925498 valmi_connector_lib-0.1.98/valmi_connector_lib/common/constants.py
--rw-r--r--   0        0        0     6100 2023-08-22 12:53:07.839529 valmi_connector_lib-0.1.98/valmi_connector_lib/common/logs.py
--rw-r--r--   0        0        0      270 2023-08-03 15:20:12.758134 valmi_connector_lib-0.1.98/valmi_connector_lib/common/metrics.py
--rw-r--r--   0        0        0      356 2023-05-26 09:10:49.515215 valmi_connector_lib-0.1.98/valmi_connector_lib/common/run_time_args.py
--rw-r--r--   0        0        0     6655 2023-08-28 16:46:59.767948 valmi_connector_lib-0.1.98/valmi_connector_lib/common/samples.py
--rw-r--r--   0        0        0        0 2023-05-18 14:12:43.012723 valmi_connector_lib-0.1.98/valmi_connector_lib/destination_wrapper/__init__.py
--rwxr-xr-x   0        0        0     8075 2023-08-25 08:43:06.469290 valmi_connector_lib-0.1.98/valmi_connector_lib/destination_wrapper/destination_container_wrapper.py
--rw-r--r--   0        0        0     6259 2023-08-16 07:49:56.189433 valmi_connector_lib-0.1.98/valmi_connector_lib/destination_wrapper/destination_write_wrapper.py
--rw-r--r--   0        0        0     7453 2023-08-16 07:12:13.049838 valmi_connector_lib-0.1.98/valmi_connector_lib/destination_wrapper/engine.py
--rw-r--r--   0        0        0     7340 2023-08-25 13:45:12.797453 valmi_connector_lib-0.1.98/valmi_connector_lib/destination_wrapper/proc_stdout_event_handlers.py
--rw-r--r--   0        0        0     4207 2023-08-22 05:22:09.410895 valmi_connector_lib-0.1.98/valmi_connector_lib/destination_wrapper/proc_stdout_handler.py
--rw-r--r--   0        0        0     2449 2023-05-18 14:12:43.014707 valmi_connector_lib-0.1.98/valmi_connector_lib/destination_wrapper/read_handlers.py
--rw-r--r--   0        0        0        0 2023-05-18 14:12:43.014759 valmi_connector_lib-0.1.98/valmi_connector_lib/source_wrapper/__init__.py
--rwxr-xr-x   0        0        0    17138 2023-08-25 14:41:07.534288 valmi_connector_lib-0.1.98/valmi_connector_lib/source_wrapper/source_container_wrapper.py
--rw-r--r--   0        0        0       80 2023-05-18 14:12:43.015309 valmi_connector_lib-0.1.98/valmi_connector_lib/valmi_destination/__init__.py
--rw-r--r--   0        0        0     8858 2023-08-14 12:34:28.108060 valmi_connector_lib-0.1.98/valmi_connector_lib/valmi_destination/valmi_destination.py
--rw-r--r--   0        0        0      679 2023-05-30 18:48:18.064345 valmi_connector_lib-0.1.98/valmi_connector_lib/valmi_protocol/__init__.py
--rw-r--r--   0        0        0      138 2023-05-18 14:12:43.016551 valmi_connector_lib-0.1.98/valmi_connector_lib/valmi_protocol/valmi_event.py
--rw-r--r--   0        0        0     6039 2023-08-25 13:10:50.395512 valmi_connector_lib-0.1.98/valmi_connector_lib/valmi_protocol/valmi_protocol.py
--rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 valmi_connector_lib-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-18 14:12:43.011582 valmi_connector_lib-0.1.99/README.md
+-rw-r--r--   0        0        0     1661 2023-08-28 17:32:05.940295 valmi_connector_lib-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-18 14:12:43.012354 valmi_connector_lib-0.1.99/valmi_connector_lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-21 15:41:28.501761 valmi_connector_lib-0.1.99/valmi_connector_lib/common/__init__.py
+-rw-r--r--   0        0        0       25 2023-08-22 12:52:39.925498 valmi_connector_lib-0.1.99/valmi_connector_lib/common/constants.py
+-rw-r--r--   0        0        0     6100 2023-08-22 12:53:07.839529 valmi_connector_lib-0.1.99/valmi_connector_lib/common/logs.py
+-rw-r--r--   0        0        0      270 2023-08-03 15:20:12.758134 valmi_connector_lib-0.1.99/valmi_connector_lib/common/metrics.py
+-rw-r--r--   0        0        0      356 2023-05-26 09:10:49.515215 valmi_connector_lib-0.1.99/valmi_connector_lib/common/run_time_args.py
+-rw-r--r--   0        0        0     6626 2023-08-28 17:32:00.235101 valmi_connector_lib-0.1.99/valmi_connector_lib/common/samples.py
+-rw-r--r--   0        0        0        0 2023-05-18 14:12:43.012723 valmi_connector_lib-0.1.99/valmi_connector_lib/destination_wrapper/__init__.py
+-rwxr-xr-x   0        0        0     8075 2023-08-25 08:43:06.469290 valmi_connector_lib-0.1.99/valmi_connector_lib/destination_wrapper/destination_container_wrapper.py
+-rw-r--r--   0        0        0     6259 2023-08-16 07:49:56.189433 valmi_connector_lib-0.1.99/valmi_connector_lib/destination_wrapper/destination_write_wrapper.py
+-rw-r--r--   0        0        0     7453 2023-08-16 07:12:13.049838 valmi_connector_lib-0.1.99/valmi_connector_lib/destination_wrapper/engine.py
+-rw-r--r--   0        0        0     7340 2023-08-25 13:45:12.797453 valmi_connector_lib-0.1.99/valmi_connector_lib/destination_wrapper/proc_stdout_event_handlers.py
+-rw-r--r--   0        0        0     4207 2023-08-22 05:22:09.410895 valmi_connector_lib-0.1.99/valmi_connector_lib/destination_wrapper/proc_stdout_handler.py
+-rw-r--r--   0        0        0     2449 2023-05-18 14:12:43.014707 valmi_connector_lib-0.1.99/valmi_connector_lib/destination_wrapper/read_handlers.py
+-rw-r--r--   0        0        0        0 2023-05-18 14:12:43.014759 valmi_connector_lib-0.1.99/valmi_connector_lib/source_wrapper/__init__.py
+-rwxr-xr-x   0        0        0    17188 2023-08-28 16:55:45.093469 valmi_connector_lib-0.1.99/valmi_connector_lib/source_wrapper/source_container_wrapper.py
+-rw-r--r--   0        0        0       80 2023-05-18 14:12:43.015309 valmi_connector_lib-0.1.99/valmi_connector_lib/valmi_destination/__init__.py
+-rw-r--r--   0        0        0     8858 2023-08-14 12:34:28.108060 valmi_connector_lib-0.1.99/valmi_connector_lib/valmi_destination/valmi_destination.py
+-rw-r--r--   0        0        0      679 2023-05-30 18:48:18.064345 valmi_connector_lib-0.1.99/valmi_connector_lib/valmi_protocol/__init__.py
+-rw-r--r--   0        0        0      138 2023-05-18 14:12:43.016551 valmi_connector_lib-0.1.99/valmi_connector_lib/valmi_protocol/valmi_event.py
+-rw-r--r--   0        0        0     6039 2023-08-25 13:10:50.395512 valmi_connector_lib-0.1.99/valmi_connector_lib/valmi_protocol/valmi_protocol.py
+-rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 valmi_connector_lib-0.1.99/PKG-INFO
```

### Comparing `valmi_connector_lib-0.1.98/pyproject.toml` & `valmi_connector_lib-0.1.99/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "valmi-connector-lib"
-version = "0.1.98"
+version = "0.1.99"
 description = ""
 authors = ["Rajashekar Varkala <raj@valmi.io>"]
 readme = "README.md"
 packages = [{include = "valmi_connector_lib"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `valmi_connector_lib-0.1.98/valmi_connector_lib/common/logs.py` & `valmi_connector_lib-0.1.99/valmi_connector_lib/common/logs.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.98/valmi_connector_lib/common/samples.py` & `valmi_connector_lib-0.1.99/valmi_connector_lib/common/samples.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             self.flush()
             self.reset()
 
     def write(self, json_log_record):
         rejection_code = json_log_record["record"]["rejection_code"] \
             if "rejected" in json_log_record["record"] and json_log_record["record"]["rejected"] else "200"
         if (self.sample_counter[rejection_code] < self.num_samples_per_code):
-            self.sample_counter[json_log_record["record"]["rejection_code"]] += 1
+            self.sample_counter[rejection_code] += 1
             self.records.append(json_log_record)
 
     def flush(self):
         if len(self.records) > 0:
             # TODO: do cloud push for aws, s3 when we do k8s
             file_path = join(self.store_config['local']['directory'],
                              self.run_id, "samples", self.connector, f'{self.metric_type}.vals')
```

### Comparing `valmi_connector_lib-0.1.98/valmi_connector_lib/destination_wrapper/destination_container_wrapper.py` & `valmi_connector_lib-0.1.99/valmi_connector_lib/destination_wrapper/destination_container_wrapper.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.98/valmi_connector_lib/destination_wrapper/destination_write_wrapper.py` & `valmi_connector_lib-0.1.99/valmi_connector_lib/destination_wrapper/destination_write_wrapper.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.98/valmi_connector_lib/destination_wrapper/engine.py` & `valmi_connector_lib-0.1.99/valmi_connector_lib/destination_wrapper/engine.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.98/valmi_connector_lib/destination_wrapper/proc_stdout_event_handlers.py` & `valmi_connector_lib-0.1.99/valmi_connector_lib/destination_wrapper/proc_stdout_event_handlers.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.98/valmi_connector_lib/destination_wrapper/proc_stdout_handler.py` & `valmi_connector_lib-0.1.99/valmi_connector_lib/destination_wrapper/proc_stdout_handler.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.98/valmi_connector_lib/destination_wrapper/read_handlers.py` & `valmi_connector_lib-0.1.99/valmi_connector_lib/destination_wrapper/read_handlers.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.98/valmi_connector_lib/source_wrapper/source_container_wrapper.py` & `valmi_connector_lib-0.1.99/valmi_connector_lib/source_wrapper/source_container_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,17 @@
 
 
 class RecordHandler(DefaultHandler):
     def __init__(self, *args, **kwargs):
         super(RecordHandler, self).__init__(*args, **kwargs)
 
     def handle(self, record):
-        self.store_writer.write(record)
+        if not record["record"]["rejected"]:
+            self.store_writer.write(record)
+
         if SingletonLogWriter.instance() is not None:
             SingletonLogWriter.instance().check_for_flush()
         # print(record)
         sample_writer = SampleWriter.get_writer_by_metric_type(metric_type=record["record"]["metric_type"])
         sample_writer.write(record)
 
     def finalize(self):
```

### Comparing `valmi_connector_lib-0.1.98/valmi_connector_lib/valmi_destination/valmi_destination.py` & `valmi_connector_lib-0.1.99/valmi_connector_lib/valmi_destination/valmi_destination.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.98/valmi_connector_lib/valmi_protocol/__init__.py` & `valmi_connector_lib-0.1.99/valmi_connector_lib/valmi_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.98/valmi_connector_lib/valmi_protocol/valmi_protocol.py` & `valmi_connector_lib-0.1.99/valmi_connector_lib/valmi_protocol/valmi_protocol.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.98/PKG-INFO` & `valmi_connector_lib-0.1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valmi-connector-lib
-Version: 0.1.98
+Version: 0.1.99
 Summary: 
 Author: Rajashekar Varkala
 Author-email: raj@valmi.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

