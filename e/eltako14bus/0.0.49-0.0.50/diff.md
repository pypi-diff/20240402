# Comparing `tmp/eltako14bus-0.0.49.tar.gz` & `tmp/eltako14bus-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eltako14bus-0.0.49.tar", last modified: Thu Mar 28 14:57:17 2024, max compression
+gzip compressed data, was "eltako14bus-0.0.50.tar", last modified: Tue Apr  2 13:48:50 2024, max compression
```

## Comparing `eltako14bus-0.0.49.tar` & `eltako14bus-0.0.50.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:57:17.684565 eltako14bus-0.0.49/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-28 14:57:01.000000 eltako14bus-0.0.49/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-28 14:57:17.684565 eltako14bus-0.0.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-03-28 14:57:01.000000 eltako14bus-0.0.49/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:57:17.684565 eltako14bus-0.0.49/eltako14bus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-28 14:57:17.000000 eltako14bus-0.0.49/eltako14bus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-28 14:57:17.000000 eltako14bus-0.0.49/eltako14bus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:57:17.000000 eltako14bus-0.0.49/eltako14bus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:57:17.000000 eltako14bus-0.0.49/eltako14bus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-28 14:57:17.000000 eltako14bus-0.0.49/eltako14bus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:57:17.684565 eltako14bus-0.0.49/eltakobus/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-28 14:57:01.000000 eltako14bus-0.0.49/eltakobus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-03-28 14:57:01.000000 eltako14bus-0.0.49/eltakobus/bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-28 14:57:01.000000 eltako14bus-0.0.49/eltakobus/coap.py
--rw-r--r--   0 runner    (1001) docker     (127)    43177 2024-03-28 14:57:01.000000 eltako14bus-0.0.49/eltakobus/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    39509 2024-03-28 14:57:01.000000 eltako14bus-0.0.49/eltakobus/eep.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-28 14:57:01.000000 eltako14bus-0.0.49/eltakobus/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-28 14:57:01.000000 eltako14bus-0.0.49/eltakobus/locking.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-03-28 14:57:01.000000 eltako14bus-0.0.49/eltakobus/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-03-28 14:57:01.000000 eltako14bus-0.0.49/eltakobus/serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-03-28 14:57:01.000000 eltako14bus-0.0.49/eltakobus/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 14:57:17.684565 eltako14bus-0.0.49/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-03-28 14:57:01.000000 eltako14bus-0.0.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:48:50.064133 eltako14bus-0.0.50/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-02 13:48:50.064133 eltako14bus-0.0.50/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:48:50.064133 eltako14bus-0.0.50/eltako14bus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-02 13:48:50.000000 eltako14bus-0.0.50/eltako14bus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-02 13:48:50.000000 eltako14bus-0.0.50/eltako14bus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:48:50.000000 eltako14bus-0.0.50/eltako14bus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 13:48:50.000000 eltako14bus-0.0.50/eltako14bus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 13:48:50.000000 eltako14bus-0.0.50/eltako14bus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:48:50.064133 eltako14bus-0.0.50/eltakobus/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/coap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44440 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39509 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/eep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/locking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:48:50.064133 eltako14bus-0.0.50/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/setup.py
```

### Comparing `eltako14bus-0.0.49/LICENSE` & `eltako14bus-0.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.49/PKG-INFO` & `eltako14bus-0.0.50/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltako14bus
-Version: 0.0.49
+Version: 0.0.50
 Summary: Library for participating in the Eltako Series 14 RS485 bus
 Home-page: https://github.com/grimmpp/eltako14bus
 Author: chrysn, grimmpp
 Author-email: chrysn@fsfe.org, grimmpp14@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `eltako14bus-0.0.49/README.md` & `eltako14bus-0.0.50/README.md`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.49/eltako14bus.egg-info/PKG-INFO` & `eltako14bus-0.0.50/eltako14bus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltako14bus
-Version: 0.0.49
+Version: 0.0.50
 Summary: Library for participating in the Eltako Series 14 RS485 bus
 Home-page: https://github.com/grimmpp/eltako14bus
 Author: chrysn, grimmpp
 Author-email: chrysn@fsfe.org, grimmpp14@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `eltako14bus-0.0.49/eltakobus/bus.py` & `eltako14bus-0.0.50/eltakobus/bus.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.49/eltakobus/coap.py` & `eltako14bus-0.0.50/eltakobus/coap.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.49/eltakobus/device.py` & `eltako14bus-0.0.50/eltakobus/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import asyncio
 import binascii
 import random
 import yaml
 
 from .util import b2a, b2s, AddressExpression
 from .message import *
-from .error import UnrecognizedUpdate
-from .eep import EEP, A5_38_08, A5_12_01, F6_02_01, F6_02_02, H5_3F_7F
+from .error import *
+from .eep import EEP, A5_38_08, A5_12_01, F6_02_01, F6_02_02, H5_3F_7F, A5_10_06
 
 
 
 class KeyFunction(IntEnum):
     """Numbers of KeyFunctions from PCT14."""
     NO_FUNCTION = 0
     UNIVERSAL_PUSH_BUTTON = 1
@@ -262,15 +262,15 @@
         information and present it in a class-specific dictionary.
 
         Messages that do not fit the object raise an UnrecognizedUpdate
         exception if it expects no updates or does not know what to make of
         it."""
         raise UnrecognizedUpdate("Device is not expected to send updates")
 
-    async def get_registered_sensors(self, sensor_range:range, in_func_group:int) -> [SensorInfo]:
+    async def get_registered_sensors(self, sensor_range:range, in_func_group:int) -> list[SensorInfo]:
         result = []
         for i in sensor_range:
             mem_line:bytes = await self.read_mem_line(i)
             s_adr:bytes = mem_line[0:4]
             key = int(mem_line[4])
             func = int(mem_line[5])
             ch = int(mem_line[6])
@@ -295,15 +295,15 @@
                                 memory_line=i
                                 ))
                     ch = ch >> 1
                     address_off_set += 1
 
         return result
     
-    async def get_all_sensors(self) -> [SensorInfo]:
+    async def get_all_sensors(self) -> list[SensorInfo]:
         return []
         # return await self.get_registered_sensors(self.sensor_address_range)
 
 
 class FAM14(BusObject):
     size = 1
     discovery_name = bytes((0x07, 0xff))
@@ -328,49 +328,16 @@
         return mem_line[0:4]
 
     async def get_base_id_in_int(self) -> int:
         """Gets base id from FAM14 memory."""
         mem_line = await self.read_mem_line(1)
         return int.from_bytes(mem_line[0:4], "big") 
 
-class FAE14SSR(BusObject):
-    size = 2
-    discovery_name = bytes((0x04, 0x16))
-    thermostat_address_range = range(8,10)
-    temp_sensor_range = range(10,12)
-    smart_home_controller_address_range = range(12,14)
-    sensor_address_range = range(14, 127)
 
 
-    @classmethod
-    def annotate_memory(cls, mem):
-        return {
-                1: MemoryFileNibbleExplanationComment(
-                    "AD DR ES S, -- -- -- --", "Base address"),
-                4: MemoryFileNibbleExplanationComment(
-                    "-- RV -- -- -- -- -- --",
-                    "RV = return value, 1. bit channel 1 & 2. bit channel 2 "),
-                5: MemoryFileNibbleExplanationComment(
-                    "-- -- -- -- dt dt -- --", "temp offset channel 1 & 2"),
-                7: MemoryFileNibbleExplanationComment(
-                    "a  a  hc tp hc tp  tt tt", ""),
-                8: MemoryFileStartOfSectionComment("function group 1 / Temp Controller"),
-                10: MemoryFileStartOfSectionComment("function group 2 / Temp Sensor"),
-                12: MemoryFileStartOfSectionComment("function group 3 / Smart Home SW"),
-                14: MemoryFileStartOfSectionComment("function group 3 / switches, contacts, ..."),
-                }
-    
-    async def get_all_sensors(self) -> [SensorInfo]:
-        result = []
-        result.extend( await self.get_registered_sensors(self.thermostat_address_range, 1 ))
-        result.extend( await self.get_registered_sensors(self.temp_sensor_range, 2 ))
-        result.extend( await self.get_registered_sensors(self.smart_home_controller_address_range, 3 ))
-        result.extend( await self.get_registered_sensors(self.sensor_address_range, 4 ))
-        return result
-
 class DimmerStyle(BusObject):
     """Devices that work just the same as a FUD14. FSG14_1_10V appears to
     behave the same way in the known areas as that -- all GUIs options in the
     PCT tool even look the same."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -397,15 +364,15 @@
         # but in EltakoWrapped messages. So this address should, for other
         # purposes, be free.
         for subchannel in range(self.size):
             source_address = AddressExpression((bytes((0, 0, 0, self.address + subchannel)), None))
             await self.ensure_programmed(subchannel, source_address, A5_38_08)
             self._explicitly_configured_command_address[subchannel] = source_address
 
-    async def ensure_programmed(self, subchannel, source: AddressExpression, profile: EEP):
+    async def ensure_programmed(self, subchannel, source: AddressExpression, profile: EEP) -> bool:
         if not self.has_subchannels:
             # In a FUD14 and similar, the subchannel field is a ramp speed (and
             # 0 seems not to mean "instant")
             subchannel = 1
 
         if profile is A5_38_08:
             a = source.plain_address()
@@ -426,21 +393,22 @@
             raise ValueError("It is unknown how this profile could be programmed in.")
 
         first_empty = None
         for memory_id in range(*self.programmable_dimmer):
             line = await self.read_mem_line(memory_id)
             if line == expected_line:
                 self.bus.log.debug("%s: Found programming for profile %s in line %d", self, profile, memory_id)
-                return
+                return False
             if not any(line) and first_empty is None:
                 first_empty = memory_id
         if first_empty is None:
             raise RuntimeError("No free memory to configure this function")
         self.bus.log.info("%s: Writing programming for profile %s in line %d", self, profile, first_empty)
         await self.write_mem_line(first_empty, expected_line)
+        return True
 
     async def set_state(self, channel, dim, total_ramp_time=0):
         """Send a telegram to set the dimming state to dim (from 0 to 255). Total ramp time is the the time in seconds """
         sender = await self.find_direct_command_address(channel)
         if sender is None:
             raise RuntimeError("Can't send without any configured universal remote")
         sender = sender.plain_address()
@@ -520,15 +488,15 @@
     range_func_group_3 = range(12,127)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.programmable_dimmer = (12, self.memory_size)
         self.gfvs_code = KeyFunction.DIMMING_VALUE_FROM_CONTROLLER
 
-    async def get_all_sensors(self) -> [SensorInfo]:
+    async def get_all_sensors(self) -> list[SensorInfo]:
         result = []
         result.extend( await self.get_registered_sensors(self.range_func_group_1, 1 ))
         result.extend( await self.get_registered_sensors(self.range_func_group_2, 2 ))
         result.extend( await self.get_registered_sensors(self.range_func_group_3, 3 ))
         return result
 
 class FUD14_800W(FUD14):
@@ -590,44 +558,59 @@
         # but in EltakoWrapped messages. So this address should, for other
         # purposes, be free.
         for subchannel in range(self.size):
             source_address = AddressExpression((bytes((0, 0, 0, self.address + subchannel)), "left"))
             await self.ensure_programmed(subchannel, source_address, F6_02_01)
             self._explicitly_configured_command_address[subchannel] = source_address
 
-    async def ensure_programmed(self, subchannel, source: AddressExpression, profile: EEP):
-        if profile is F6_02_01:
+    async def ensure_programmed(self, subchannel, source: AddressExpression, profile: EEP) -> bool:
+        """
+        Checks if entry is already present and if not it writes it into the memory at a free place.
+
+        :returns: True if entry was written, False if enrity already exists
+        """
+        memory_range = self.programmable_rps
+        if profile in [F6_02_01, F6_02_02]:
             a, discriminator = source
             if discriminator == "left":
                 # programmed as function 3, key is 5 for left
                 expected_line = a + bytes((5, 3, 1 << subchannel, 0))
             elif discriminator == 'right':
                 # programmed as function 3, key is 6 for right
                 expected_line = a + bytes((6, 3, 1 << subchannel, 0))
             else:
                 raise ValueError("Unknown discriminator on address %s" % (source,))
         elif profile in [A5_38_08, H5_3F_7F]:
             a, discriminator = source
             # 51 GFVS = House Automation SW
             expected_line = a + bytes((0, self.gfvs_code, 1 << subchannel, 0))
+        elif profile in [A5_10_06]:
+            a, discriminator = source
+            # 65 GFVS = House Automation SW
+            expected_line = a + bytes((0, self.gfvs_code, 1 << subchannel, 0))
+            memory_range = (self.programmable_rps[0]+subchannel, self.programmable_rps[0]+subchannel)
         else:
             raise ValueError("It is unknown how this profile could be programmed in.")
 
         first_empty = None
-        for memory_id in range(*self.programmable_rps):
-            line = await self.read_mem_line(memory_id)
-            if line == expected_line:
-                self.bus.log.debug("%s: Found programming for subchannel %s and profile %s in line %d", self, subchannel, profile, memory_id)
-                return
-            if not any(line) and first_empty is None:
-                first_empty = memory_id
+        if memory_range[0] == memory_range[1]:
+            first_empty = memory_range[0] # force
+        else:
+            for memory_id in range(*memory_range):
+                line = await self.read_mem_line(memory_id)
+                if line == expected_line:
+                    self.bus.log.debug("%s: Found programming for subchannel %s and profile %s in line %d", self, subchannel, profile, memory_id)
+                    return False
+                if not any(line) and first_empty is None:
+                    first_empty = memory_id
         if first_empty is None:
             raise RuntimeError("No free memory to configure this function")
         self.bus.log.info("%s: Writing programming for profile %s in line %d", self, profile, first_empty)
         await self.write_mem_line(first_empty, expected_line)
+        return True
 
     async def set_state(self, channel, state: bool):
         command = await self.find_direct_command_address(channel)
         if command is None:
             raise RuntimeError("Can't send without any configured universal remote")
 
         sender, discriminator = command
@@ -703,15 +686,15 @@
 
         state = {0x50: False, 0x70: True}.get(msg.data[0])
         if state is None:
             raise UnrecognizedUpdate("Telegram is not a plain on or off message")
 
         return {subchannel: state}
     
-    async def get_all_sensors(self) -> [SensorInfo]:
+    async def get_all_sensors(self) -> list[SensorInfo]:
         result = []
         result.extend( await self.get_registered_sensors(self.sensors_func_group_1, 1) )
         result.extend( await self.get_registered_sensors(self.sensors_func_group_2, 2) )
         return result
 
 class FSR14_1x(FSR14):
     discovery_name = bytes((0x04, 0x01))
@@ -811,30 +794,35 @@
                 print(msg)
                 try:
                     interpreted = self.interpret_status_update(msg)
                     print(interpreted)
                 except Exception as e:
                     print("Something went wrong", repr(e), e)
 
-    async def get_all_sensors(self) -> [SensorInfo]:
+    async def get_all_sensors(self) -> list[SensorInfo]:
         result = []
         result.extend( await self.get_registered_sensors(self.range_func_group_1, 1) )
         result.extend( await self.get_registered_sensors(self.range_func_group_2, 2) )
         return result
 
 class F3Z14D(BusObject):
     discovery_name = bytes((0x04, 0x67))
     size = 3
 
-class FMZ14(BusObject):
+class FMZ14(BusObject, HasProgrammableRPS):
     discovery_name = bytes((0x04, 0x0e))
     size = 1
-    sensor_address_range = range(1, 120)
+    sensor_address_range = range(8, 8+47)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.programmable_rps = (8, self.memory_size)
+        self.gfvs_code = KeyFunction.SWITCHING_STATE_FROM_CONTROLLER
 
-    async def get_all_sensors(self) -> [SensorInfo]:
+    async def get_all_sensors(self) -> list[SensorInfo]:
         return await self.get_registered_sensors(self.sensor_address_range, 1)
 
 class FWG14MS(BusObject):
     discovery_name = bytes((0x04, 0x1a))
     size = 1
 
 class FSU14(BusObject):
@@ -932,14 +920,56 @@
                 14: [
                     MemoryFileStartOfSectionComment("function group 1"),
                     MemoryFileNibbleExplanationComment(
                          "AD DR ES S, KY FN CH ??",
                          "key (5 = left, 6 = right), function (eg. 32 = A5-38-08), ch = channel"),
                     ],
                 }
+    
+
+class FAE14SSR(BusObject, HasProgrammableRPS):
+    size = 2
+    discovery_name = bytes((0x04, 0x16))
+    thermostat_address_range = range(8,10)
+    temp_sensor_range = range(10,12)
+    smart_home_controller_address_range = range(12,14)
+    sensor_address_range = range(14, 127)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.programmable_rps = self.smart_home_controller_address_range
+        self.gfvs_code = KeyFunction.TEMPERATURE_CONTROLLER_SETPOINT
+
+    @classmethod
+    def annotate_memory(cls, mem):
+        return {
+                1: MemoryFileNibbleExplanationComment(
+                    "AD DR ES S, -- -- -- --", "Base address"),
+                4: MemoryFileNibbleExplanationComment(
+                    "-- RV -- -- -- -- -- --",
+                    "RV = return value, 1. bit channel 1 & 2. bit channel 2 "),
+                5: MemoryFileNibbleExplanationComment(
+                    "-- -- -- -- dt dt -- --", "temp offset channel 1 & 2"),
+                7: MemoryFileNibbleExplanationComment(
+                    "a  a  hc tp hc tp  tt tt", ""),
+                8: MemoryFileStartOfSectionComment("function group 1 / Temp Controller"),
+                10: MemoryFileStartOfSectionComment("function group 2 / Temp Sensor"),
+                12: MemoryFileStartOfSectionComment("function group 3 / Smart Home SW"),
+                14: MemoryFileStartOfSectionComment("function group 3 / switches, contacts, ..."),
+                }
+    
+    async def get_all_sensors(self) -> list[SensorInfo]:
+        result = []
+        result.extend( await self.get_registered_sensors(self.thermostat_address_range, 1 ))
+        result.extend( await self.get_registered_sensors(self.temp_sensor_range, 2 ))
+        result.extend( await self.get_registered_sensors(self.smart_home_controller_address_range, 3 ))
+        result.extend( await self.get_registered_sensors(self.sensor_address_range, 4 ))
+        return result
+
+
 
 known_objects = [FAM14, FUD14, FUD14_800W, FSB14, FSR14_1x, FSR14_2x, FSR14_4x, F4SR14_LED, F3Z14D, FMZ14, FWG14MS, FSU14, FMSR14, FWZ14_65A, FSG14_1_10V, FGW14_USB, FDG14, FAE14SSR]
 # sorted so the first match of (discovery name is a prefix, size matches) can be used
 sorted_known_objects = sorted(known_objects, key=lambda o: len(o.discovery_name) + 0.5 * (o.size is not None), reverse=True)
 
 async def create_busobject(bus, id):
     response = await bus.exchange(EltakoDiscoveryRequest(address=id), EltakoDiscoveryReply)
@@ -948,14 +978,15 @@
 
     for o in sorted_known_objects:
         if response.model.startswith(o.discovery_name) and (o.size is None or o.size == response.reported_size):
             return o(response, bus=bus)
     else:
         return BusObject(response, bus=bus)
 
+    
 
 class MemoryFile(defaultdict):
     """In-memory representation of a YAML file suitable for storing, editing,
     verifying and flashing device memory contents
 
     The YAML file is a dict of dicts, mapping bus ids and memory lines (or
     memory ranges for compression) to binascii hexdumps. The MemoryFile behaves
```

### Comparing `eltako14bus-0.0.49/eltakobus/eep.py` & `eltako14bus-0.0.50/eltakobus/eep.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.49/eltakobus/error.py` & `eltako14bus-0.0.50/eltakobus/error.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.49/eltakobus/locking.py` & `eltako14bus-0.0.50/eltakobus/locking.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.49/eltakobus/message.py` & `eltako14bus-0.0.50/eltakobus/message.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.49/eltakobus/serial.py` & `eltako14bus-0.0.50/eltakobus/serial.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.49/eltakobus/util.py` & `eltako14bus-0.0.50/eltakobus/util.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.49/setup.py` & `eltako14bus-0.0.50/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 }
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="eltako14bus",
-    version="0.0.49",
+    version="0.0.50",
     author="chrysn, grimmpp",
     author_email="chrysn@fsfe.org, grimmpp14@gmail.com",
     description="Library for participating in the Eltako Series 14 RS485 bus",
     url="https://github.com/grimmpp/eltako14bus",
     packages=setuptools.find_packages(),
     extras_require=extras_require,
     # Not that there'd be tests, but at least it fetches the right dependencies and syntax checks everything
```

