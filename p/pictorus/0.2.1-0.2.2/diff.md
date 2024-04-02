# Comparing `tmp/pictorus-0.2.1.tar.gz` & `tmp/pictorus-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pictorus-0.2.1.tar", last modified: Wed Feb 28 21:05:10 2024, max compression
+gzip compressed data, was "pictorus-0.2.2.tar", last modified: Tue Apr  2 20:11:23 2024, max compression
```

## Comparing `pictorus-0.2.1.tar` & `pictorus-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       31 2024-02-05 17:27:18.447001 pictorus-0.2.1/.flake8
--rw-r--r--   0        0        0     1358 2024-02-15 20:20:41.417522 pictorus-0.2.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.2.1/.gitignore
--rw-r--r--   0        0        0      987 2024-02-15 20:20:41.417758 pictorus-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        6 2023-06-20 17:57:52.943257 pictorus-0.2.1/.python-version
--rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.2.1/LICENSE
--rw-r--r--   0        0        0      749 2023-06-19 23:08:46.580929 pictorus-0.2.1/PUB_README.md
--rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.2.1/README.md
--rw-r--r--   0        0        0     1228 2024-02-15 20:20:41.418116 pictorus-0.2.1/pyproject.toml
--rwxr-xr-x   0        0        0      483 2024-02-15 20:20:41.418402 pictorus-0.2.1/script/setup
--rw-r--r--   0        0        0       61 2024-02-28 20:37:32.275708 pictorus-0.2.1/src/pictorus/__init__.py
--rw-r--r--   0        0        0    16613 2024-02-28 21:05:07.936582 pictorus-0.2.1/src/pictorus/app_manager.py
--rw-r--r--   0        0        0     1995 2024-02-15 20:20:41.419443 pictorus-0.2.1/src/pictorus/command.py
--rw-r--r--   0        0        0     3614 2024-02-05 17:27:18.448390 pictorus-0.2.1/src/pictorus/config.py
--rw-r--r--   0        0        0      875 2024-02-15 20:20:41.419712 pictorus-0.2.1/src/pictorus/constants.py
--rw-r--r--   0        0        0      264 2024-02-15 20:20:41.419940 pictorus-0.2.1/src/pictorus/date_utils.py
--rw-r--r--   0        0        0     1945 2024-02-15 20:20:41.420191 pictorus-0.2.1/src/pictorus/embedded_target_manager.py
--rw-r--r--   0        0        0     5931 2024-02-15 20:20:41.420926 pictorus-0.2.1/src/pictorus/local_server.py
--rw-r--r--   0        0        0      244 2023-09-28 16:25:58.267963 pictorus-0.2.1/src/pictorus/logging_utils.py
--rw-r--r--   0        0        0     5578 2024-02-15 20:20:41.421375 pictorus-0.2.1/src/pictorus/pictorus_cli.py
--rwxr-xr-x   0        0        0      695 2024-02-15 20:20:41.421617 pictorus-0.2.1/src/pictorus/pictorus_device_manager.py
--rw-r--r--   0        0        0     6786 2024-02-15 20:20:41.422156 pictorus-0.2.1/src/pictorus/proc_target_manager.py
--rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.2.1/src/pictorus/systemd.py
--rw-r--r--   0        0        0     5097 2024-02-05 17:27:18.450570 pictorus-0.2.1/src/pictorus/target_manager.py
--rw-r--r--   0        0        0      577 2024-02-15 20:20:41.422410 pictorus-0.2.1/src/pictorus/target_state.py
--rw-r--r--   0        0        0     4704 2024-02-15 20:20:41.422916 pictorus-0.2.1/src/pictorus/telemetry_manager.py
--rw-r--r--   0        0        0     3602 2024-02-15 20:20:41.423093 pictorus-0.2.1/src/pictorus/version_manager.py
--rw-r--r--   0        0        0        0 2023-09-28 16:25:58.268901 pictorus-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      347 2024-02-05 17:27:18.451098 pictorus-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-09-28 16:25:58.269155 pictorus-0.2.1/tests/pictorus/__init__.py
--rw-r--r--   0        0        0     7676 2024-02-28 21:05:07.937033 pictorus-0.2.1/tests/pictorus/test_app_manager.py
--rw-r--r--   0        0        0     4022 2024-02-05 17:27:18.451666 pictorus-0.2.1/tests/pictorus/test_embedded_target_manager.py
--rw-r--r--   0        0        0     5448 2024-02-05 17:27:18.452034 pictorus-0.2.1/tests/pictorus/test_local_server.py
--rw-r--r--   0        0        0     8176 2024-02-05 17:27:18.452295 pictorus-0.2.1/tests/pictorus/test_proc_target_manager.py
--rw-r--r--   0        0        0     2758 2024-01-09 22:24:36.010715 pictorus-0.2.1/tests/pictorus/test_telemetry_manager.py
--rw-r--r--   0        0        0     2532 2023-06-21 04:42:19.639081 pictorus-0.2.1/tests/pictorus/test_version_manager.py
--rw-r--r--   0        0        0     1400 2024-02-05 17:27:18.452565 pictorus-0.2.1/tests/utils.py
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 pictorus-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       31 2024-02-05 17:27:18.447001 pictorus-0.2.2/.flake8
+-rw-r--r--   0        0        0     1358 2024-02-15 20:20:41.417522 pictorus-0.2.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.2.2/.gitignore
+-rw-r--r--   0        0        0      987 2024-02-15 20:20:41.417758 pictorus-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        6 2023-06-20 17:57:52.943257 pictorus-0.2.2/.python-version
+-rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.2.2/LICENSE
+-rw-r--r--   0        0        0      749 2023-06-19 23:08:46.580929 pictorus-0.2.2/PUB_README.md
+-rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.2.2/README.md
+-rw-r--r--   0        0        0     1228 2024-02-15 20:20:41.418116 pictorus-0.2.2/pyproject.toml
+-rwxr-xr-x   0        0        0      483 2024-02-15 20:20:41.418402 pictorus-0.2.2/script/setup
+-rw-r--r--   0        0        0       61 2024-04-02 20:10:55.300861 pictorus-0.2.2/src/pictorus/__init__.py
+-rw-r--r--   0        0        0    16613 2024-02-28 21:05:07.936582 pictorus-0.2.2/src/pictorus/app_manager.py
+-rw-r--r--   0        0        0     1995 2024-02-15 20:20:41.419443 pictorus-0.2.2/src/pictorus/command.py
+-rw-r--r--   0        0        0     3614 2024-02-05 17:27:18.448390 pictorus-0.2.2/src/pictorus/config.py
+-rw-r--r--   0        0        0      875 2024-02-15 20:20:41.419712 pictorus-0.2.2/src/pictorus/constants.py
+-rw-r--r--   0        0        0      264 2024-02-15 20:20:41.419940 pictorus-0.2.2/src/pictorus/date_utils.py
+-rw-r--r--   0        0        0     1945 2024-02-15 20:20:41.420191 pictorus-0.2.2/src/pictorus/embedded_target_manager.py
+-rw-r--r--   0        0        0     6117 2024-04-02 20:10:52.936065 pictorus-0.2.2/src/pictorus/local_server.py
+-rw-r--r--   0        0        0      244 2023-09-28 16:25:58.267963 pictorus-0.2.2/src/pictorus/logging_utils.py
+-rw-r--r--   0        0        0     5578 2024-02-15 20:20:41.421375 pictorus-0.2.2/src/pictorus/pictorus_cli.py
+-rwxr-xr-x   0        0        0      695 2024-02-15 20:20:41.421617 pictorus-0.2.2/src/pictorus/pictorus_device_manager.py
+-rw-r--r--   0        0        0     6786 2024-02-15 20:20:41.422156 pictorus-0.2.2/src/pictorus/proc_target_manager.py
+-rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.2.2/src/pictorus/systemd.py
+-rw-r--r--   0        0        0     5097 2024-02-05 17:27:18.450570 pictorus-0.2.2/src/pictorus/target_manager.py
+-rw-r--r--   0        0        0      577 2024-02-15 20:20:41.422410 pictorus-0.2.2/src/pictorus/target_state.py
+-rw-r--r--   0        0        0     4704 2024-02-15 20:20:41.422916 pictorus-0.2.2/src/pictorus/telemetry_manager.py
+-rw-r--r--   0        0        0     3602 2024-02-15 20:20:41.423093 pictorus-0.2.2/src/pictorus/version_manager.py
+-rw-r--r--   0        0        0        0 2023-09-28 16:25:58.268901 pictorus-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      347 2024-02-05 17:27:18.451098 pictorus-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-09-28 16:25:58.269155 pictorus-0.2.2/tests/pictorus/__init__.py
+-rw-r--r--   0        0        0     7630 2024-02-28 21:05:41.097625 pictorus-0.2.2/tests/pictorus/test_app_manager.py
+-rw-r--r--   0        0        0     4022 2024-02-05 17:27:18.451666 pictorus-0.2.2/tests/pictorus/test_embedded_target_manager.py
+-rw-r--r--   0        0        0     5448 2024-02-05 17:27:18.452034 pictorus-0.2.2/tests/pictorus/test_local_server.py
+-rw-r--r--   0        0        0     8176 2024-02-05 17:27:18.452295 pictorus-0.2.2/tests/pictorus/test_proc_target_manager.py
+-rw-r--r--   0        0        0     2758 2024-01-09 22:24:36.010715 pictorus-0.2.2/tests/pictorus/test_telemetry_manager.py
+-rw-r--r--   0        0        0     2532 2023-06-21 04:42:19.639081 pictorus-0.2.2/tests/pictorus/test_version_manager.py
+-rw-r--r--   0        0        0     1400 2024-02-05 17:27:18.452565 pictorus-0.2.2/tests/utils.py
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 pictorus-0.2.2/PKG-INFO
```

### Comparing `pictorus-0.2.1/.github/workflows/test.yaml` & `pictorus-0.2.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/.gitignore` & `pictorus-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/.pre-commit-config.yaml` & `pictorus-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/LICENSE` & `pictorus-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/PUB_README.md` & `pictorus-0.2.2/PUB_README.md`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/README.md` & `pictorus-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/pyproject.toml` & `pictorus-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/src/pictorus/app_manager.py` & `pictorus-0.2.2/src/pictorus/app_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/src/pictorus/command.py` & `pictorus-0.2.2/src/pictorus/command.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/src/pictorus/config.py` & `pictorus-0.2.2/src/pictorus/config.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/src/pictorus/constants.py` & `pictorus-0.2.2/src/pictorus/constants.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/src/pictorus/embedded_target_manager.py` & `pictorus-0.2.2/src/pictorus/embedded_target_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/src/pictorus/local_server.py` & `pictorus-0.2.2/src/pictorus/local_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,30 +41,33 @@
                     pass
 
             self._data[key].append(val)
 
     def get_telem(
         self, requested_start_time: Union[int, float], max_age_s: Union[int, float]
     ) -> Dict:
-        timestamp_data = self._data.get("utctime")
+        # Copy the current data to lists. This prevents other threads
+        # from modifying the data while we're iterating over it.
+        data = {key: list(vals) for key, vals in self._data.items()}
+        timestamp_data = data.get("utctime")
         if not timestamp_data:
             start_index = 0
         else:
             utc_now = utc_timestamp_ms()
             start_time = max(utc_now - max_age_s * 1000, requested_start_time)
             start_index = next(
                 (
                     i
                     for i, ts in enumerate(timestamp_data)
                     if isinstance(ts, float) or isinstance(ts, int) and ts > start_time
                 ),
                 0,
             )
 
-        return {key: list(vals)[start_index:] for key, vals in self._data.items()}
+        return {key: vals[start_index:] for key, vals in data.items()}
 
     def clear(self):
         self._data.clear()
         self.reported_state = None
         self.commands = Queue()
```

### Comparing `pictorus-0.2.1/src/pictorus/pictorus_cli.py` & `pictorus-0.2.2/src/pictorus/pictorus_cli.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/src/pictorus/pictorus_device_manager.py` & `pictorus-0.2.2/src/pictorus/pictorus_device_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/src/pictorus/proc_target_manager.py` & `pictorus-0.2.2/src/pictorus/proc_target_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/src/pictorus/systemd.py` & `pictorus-0.2.2/src/pictorus/systemd.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/src/pictorus/target_manager.py` & `pictorus-0.2.2/src/pictorus/target_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/src/pictorus/target_state.py` & `pictorus-0.2.2/src/pictorus/target_state.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/src/pictorus/telemetry_manager.py` & `pictorus-0.2.2/src/pictorus/telemetry_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/src/pictorus/version_manager.py` & `pictorus-0.2.2/src/pictorus/version_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/tests/pictorus/test_app_manager.py` & `pictorus-0.2.2/tests/pictorus/test_app_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
         target_mgr = MagicMock()
         with AppManager(Mock()) as mgr:
             # Attempt to start an app for a target that doesn't exist
             mgr._on_shadow_delta_updated(
                 ShadowDeltaUpdatedEvent(state={"target_states": {target_id: {"run_app": True}}})
             )
             target_mgr.handle_command.assert_not_called()
-            print(m_shadow_req.mock_calls[0])
             assert m_shadow_req.mock_calls[1][2]["state"].desired["target_states"] == {
                 target_id: None
             }
 
     @patch("pictorus.app_manager.iotshadow.UpdateShadowRequest")
     def test_starts_and_stops_app_based_on_thread_comms(self, m_shadow_req, _):
         target_id = "foo"
```

### Comparing `pictorus-0.2.1/tests/pictorus/test_embedded_target_manager.py` & `pictorus-0.2.2/tests/pictorus/test_embedded_target_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/tests/pictorus/test_local_server.py` & `pictorus-0.2.2/tests/pictorus/test_local_server.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/tests/pictorus/test_proc_target_manager.py` & `pictorus-0.2.2/tests/pictorus/test_proc_target_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/tests/pictorus/test_telemetry_manager.py` & `pictorus-0.2.2/tests/pictorus/test_telemetry_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/tests/pictorus/test_version_manager.py` & `pictorus-0.2.2/tests/pictorus/test_version_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/tests/utils.py` & `pictorus-0.2.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.1/PKG-INFO` & `pictorus-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pictorus
-Version: 0.2.1
+Version: 0.2.2
 Summary: Pictorus device manager package
 Author-email: Pictorus Inc <contact@pictor.us>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: awsiotsdk~=1.11.9; python_version <= "3.6"
 Requires-Dist: awsiotsdk~=1.19.0; python_version > "3.6"
```

