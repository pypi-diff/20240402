# Comparing `tmp/lmcloud-1.1.6.tar.gz` & `tmp/lmcloud-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmcloud-1.1.6.tar", last modified: Mon Mar 25 07:09:07 2024, max compression
+gzip compressed data, was "lmcloud-1.1.7.tar", last modified: Tue Apr  2 07:46:28 2024, max compression
```

## Comparing `lmcloud-1.1.6.tar` & `lmcloud-1.1.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 07:09:07.847932 lmcloud-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-25 07:08:43.000000 lmcloud-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-03-25 07:09:07.847932 lmcloud-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-03-25 07:08:43.000000 lmcloud-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 07:09:07.847932 lmcloud-1.1.6/lmcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-25 07:08:43.000000 lmcloud-1.1.6/lmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-03-25 07:08:43.000000 lmcloud-1.1.6/lmcloud/client_bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-03-25 07:08:43.000000 lmcloud-1.1.6/lmcloud/client_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-03-25 07:08:43.000000 lmcloud-1.1.6/lmcloud/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-03-25 07:08:43.000000 lmcloud-1.1.6/lmcloud/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-25 07:08:43.000000 lmcloud-1.1.6/lmcloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-03-25 07:08:43.000000 lmcloud-1.1.6/lmcloud/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-03-25 07:08:43.000000 lmcloud-1.1.6/lmcloud/lm_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-03-25 07:08:43.000000 lmcloud-1.1.6/lmcloud/lm_grinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    17201 2024-03-25 07:08:43.000000 lmcloud-1.1.6/lmcloud/lm_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-03-25 07:08:43.000000 lmcloud-1.1.6/lmcloud/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 07:08:43.000000 lmcloud-1.1.6/lmcloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 07:09:07.847932 lmcloud-1.1.6/lmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-03-25 07:09:07.000000 lmcloud-1.1.6/lmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-25 07:09:07.000000 lmcloud-1.1.6/lmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 07:09:07.000000 lmcloud-1.1.6/lmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-25 07:09:07.000000 lmcloud-1.1.6/lmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-25 07:09:07.000000 lmcloud-1.1.6/lmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 07:09:07.847932 lmcloud-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-25 07:08:43.000000 lmcloud-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 07:09:07.847932 lmcloud-1.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-25 07:08:43.000000 lmcloud-1.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-03-25 07:08:43.000000 lmcloud-1.1.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-25 07:08:43.000000 lmcloud-1.1.6/tests/test_grinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-03-25 07:08:43.000000 lmcloud-1.1.6/tests/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:46:28.240892 lmcloud-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-02 07:46:09.000000 lmcloud-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-02 07:46:28.236892 lmcloud-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-02 07:46:09.000000 lmcloud-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:46:28.236892 lmcloud-1.1.7/lmcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/client_bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14859 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/client_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/lm_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/lm_grinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17749 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/lm_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:46:09.000000 lmcloud-1.1.7/lmcloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:46:28.236892 lmcloud-1.1.7/lmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-02 07:46:28.000000 lmcloud-1.1.7/lmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-02 07:46:28.000000 lmcloud-1.1.7/lmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:46:28.000000 lmcloud-1.1.7/lmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 07:46:28.000000 lmcloud-1.1.7/lmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 07:46:28.000000 lmcloud-1.1.7/lmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:46:28.240892 lmcloud-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-02 07:46:09.000000 lmcloud-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:46:28.236892 lmcloud-1.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-02 07:46:09.000000 lmcloud-1.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-02 07:46:09.000000 lmcloud-1.1.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-02 07:46:09.000000 lmcloud-1.1.7/tests/test_grinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-02 07:46:09.000000 lmcloud-1.1.7/tests/test_machine.py
```

### Comparing `lmcloud-1.1.6/LICENSE` & `lmcloud-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/PKG-INFO` & `lmcloud-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 1.1.6
+Version: 1.1.7
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-1.1.6/README.md` & `lmcloud-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/lmcloud/client_bluetooth.py` & `lmcloud-1.1.7/lmcloud/client_bluetooth.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/lmcloud/client_cloud.py` & `lmcloud-1.1.7/lmcloud/client_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     BoilerType,
     FirmwareType,
     PhysicalKey,
     PrebrewMode,
     SmartStandbyMode,
 )
 from .exceptions import AuthFail, RequestNotSuccessful
-from .models import LaMarzoccoFirmware, LaMarzoccoDeviceInfo
+from .models import LaMarzoccoFirmware, LaMarzoccoDeviceInfo, LaMarzoccoWakeUpSleepEntry
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class LaMarzoccoCloudClient:
     """La Marzocco Cloud Client."""
 
@@ -270,14 +270,33 @@
     #     response = await self._rest_api_call(
     #         url=url, method=HTTPMethod.POST, data=dict(schedule)
     #     )
     #     if await self._check_cloud_command_status(serial_number, response):
     #         return True
     #     return False
 
+    async def set_wake_up_sleep(
+        self, serial_number: str, wake_up_sleep_entry: LaMarzoccoWakeUpSleepEntry
+    ) -> bool:
+        """Enable or disable wake-up sleep mode"""
+
+        url = f"{GW_MACHINE_BASE_URL}/{serial_number}/wake-up-sleep/{wake_up_sleep_entry.entry_id}"
+        data = {
+            "days": [day.value for day in wake_up_sleep_entry.days],
+            "enable": wake_up_sleep_entry.enabled,
+            "id": wake_up_sleep_entry.entry_id,
+            "steam": wake_up_sleep_entry.steam,
+            "timeOff": wake_up_sleep_entry.time_off,
+            "timeOn": wake_up_sleep_entry.time_on,
+        }
+        response = await self._rest_api_call(url=url, method=HTTPMethod.PUT, data=data)
+        if await self._check_cloud_command_status(serial_number, response):
+            return True
+        return False
+
     async def set_smart_standby(
         self,
         serial_number: str,
         enabled: bool,
         minutes: int,
         mode: SmartStandbyMode,
     ) -> bool:
```

### Comparing `lmcloud-1.1.6/lmcloud/client_local.py` & `lmcloud-1.1.7/lmcloud/client_local.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/lmcloud/const.py` & `lmcloud-1.1.7/lmcloud/const.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/lmcloud/exceptions.py` & `lmcloud-1.1.7/lmcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/lmcloud/helpers.py` & `lmcloud-1.1.7/lmcloud/helpers.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/lmcloud/lm_device.py` & `lmcloud-1.1.7/lmcloud/lm_device.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/lmcloud/lm_grinder.py` & `lmcloud-1.1.7/lmcloud/lm_grinder.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/lmcloud/lm_machine.py` & `lmcloud-1.1.7/lmcloud/lm_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     parse_wakeup_sleep_entries,
 )
 from .lm_device import LaMarzoccoDevice
 from .models import (
     LaMarzoccoCoffeeStatistics,
     LaMarzoccoMachineConfig,
     LaMarzoccoSmartStandby,
+    LaMarzoccoWakeUpSleepEntry,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class LaMarzoccoMachine(LaMarzoccoDevice):
     """Class for La Marzocco coffee machine"""
@@ -329,14 +330,26 @@
     #         m_on=m_on,
     #         m_off=m_off,
     #     )
     #     schedule = deepcopy(self.config.auto_on_off_schedule)
     #     schedule.days[day] = day_settings
     #     return await self.set_schedule(schedule)
 
+    async def set_wake_up_sleep(self, wake_up_sleep_entry: LaMarzoccoWakeUpSleepEntry):
+        """Set wake up sleep"""
+
+        if await self.cloud_client.set_wake_up_sleep(
+            self.serial_number, wake_up_sleep_entry
+        ):
+            for idx, entry in enumerate(self.config.wake_up_sleep_entries):
+                if entry.entry_id == wake_up_sleep_entry.entry_id:
+                    self.config.wake_up_sleep_entries[idx] = wake_up_sleep_entry
+                    return True
+        return False
+
     async def set_smart_standby(
         self, enabled: bool, minutes: int, mode: SmartStandbyMode
     ) -> bool:
         """Set smart standby"""
 
         if await self.cloud_client.set_smart_standby(
             serial_number=self.serial_number,
```

### Comparing `lmcloud-1.1.6/lmcloud/models.py` & `lmcloud-1.1.7/lmcloud/models.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/lmcloud.egg-info/PKG-INFO` & `lmcloud-1.1.7/lmcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 1.1.6
+Version: 1.1.7
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-1.1.6/lmcloud.egg-info/SOURCES.txt` & `lmcloud-1.1.7/lmcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/setup.py` & `lmcloud-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools  # type: ignore[import]
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="lmcloud",
-    version="1.1.6",
+    version="1.1.7",
     description="A Python implementation of the new La Marzocco API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/lmcloud",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

### Comparing `lmcloud-1.1.6/tests/__init__.py` & `lmcloud-1.1.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/tests/conftest.py` & `lmcloud-1.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/tests/test_grinder.py` & `lmcloud-1.1.7/tests/test_grinder.py`

 * *Files identical despite different names*

### Comparing `lmcloud-1.1.6/tests/test_machine.py` & `lmcloud-1.1.7/tests/test_machine.py`

 * *Files identical despite different names*

