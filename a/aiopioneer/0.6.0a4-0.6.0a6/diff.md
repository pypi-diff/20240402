# Comparing `tmp/aiopioneer-0.6.0a4.tar.gz` & `tmp/aiopioneer-0.6.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopioneer-0.6.0a4.tar", last modified: Sun Mar 31 12:01:36 2024, max compression
+gzip compressed data, was "aiopioneer-0.6.0a6.tar", last modified: Tue Apr  2 20:29:03 2024, max compression
```

## Comparing `aiopioneer-0.6.0a4.tar` & `aiopioneer-0.6.0a6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwx---   0 root         (0) adm          (4)        0 2024-03-31 12:01:36.025003 aiopioneer-0.6.0a4/
--rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.6.0a4/LICENSE
--rw-rw----   0 root         (0) adm          (4)    15367 2024-03-31 12:01:36.021640 aiopioneer-0.6.0a4/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)    14715 2024-03-13 09:14:43.000000 aiopioneer-0.6.0a4/README.md
-drwxrwx---   0 root         (0) adm          (4)        0 2024-03-31 12:01:35.555009 aiopioneer-0.6.0a4/aiopioneer/
--rw-rw----   0 root         (0) adm          (4)       68 2024-03-27 20:16:44.000000 aiopioneer-0.6.0a4/aiopioneer/__init__.py
--rw-rw----   0 root         (0) adm          (4)    11023 2024-03-30 13:13:31.000000 aiopioneer-0.6.0a4/aiopioneer/cli.py
--rw-rw----   0 root         (0) adm          (4)    12452 2024-03-30 13:20:49.000000 aiopioneer-0.6.0a4/aiopioneer/commands.py
--rw-rw----   0 root         (0) adm          (4)    15083 2024-03-31 12:01:35.000000 aiopioneer-0.6.0a4/aiopioneer/const.py
--rw-rw----   0 root         (0) adm          (4)    18687 2024-03-27 20:47:07.000000 aiopioneer-0.6.0a4/aiopioneer/param.py
-drwxrwx---   0 root         (0) adm          (4)        0 2024-03-31 12:01:35.945004 aiopioneer-0.6.0a4/aiopioneer/parsers/
--rw-rw----   0 root         (0) adm          (4)     8175 2024-03-31 07:36:23.000000 aiopioneer-0.6.0a4/aiopioneer/parsers/__init__.py
--rw-rw----   0 root         (0) adm          (4)     3419 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a4/aiopioneer/parsers/audio.py
--rw-rw----   0 root         (0) adm          (4)    19209 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a4/aiopioneer/parsers/dsp.py
--rw-rw----   0 root         (0) adm          (4)    25466 2024-03-31 11:50:52.000000 aiopioneer-0.6.0a4/aiopioneer/parsers/information.py
--rw-rw----   0 root         (0) adm          (4)      599 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a4/aiopioneer/parsers/response.py
--rw-rw----   0 root         (0) adm          (4)    23416 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a4/aiopioneer/parsers/settings.py
--rw-rw----   0 root         (0) adm          (4)    15116 2024-03-30 13:58:40.000000 aiopioneer-0.6.0a4/aiopioneer/parsers/system.py
--rw-rw----   0 root         (0) adm          (4)     6359 2024-03-31 11:46:20.000000 aiopioneer-0.6.0a4/aiopioneer/parsers/tuner.py
--rw-rw----   0 root         (0) adm          (4)     8405 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a4/aiopioneer/parsers/video.py
--rw-rw----   0 root         (0) adm          (4)    86926 2024-03-31 11:10:43.000000 aiopioneer-0.6.0a4/aiopioneer/pioneer_avr.py
--rw-rw----   0 root         (0) adm          (4)     5283 2024-03-13 09:14:31.000000 aiopioneer-0.6.0a4/aiopioneer/util.py
-drwxrwx---   0 root         (0) adm          (4)        0 2024-03-31 12:01:35.985004 aiopioneer-0.6.0a4/aiopioneer.egg-info/
--rw-rw----   0 root         (0) adm          (4)    15367 2024-03-31 12:01:34.000000 aiopioneer-0.6.0a4/aiopioneer.egg-info/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)      614 2024-03-31 12:01:34.000000 aiopioneer-0.6.0a4/aiopioneer.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) adm          (4)        1 2024-03-31 12:01:34.000000 aiopioneer-0.6.0a4/aiopioneer.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) adm          (4)       51 2024-03-31 12:01:34.000000 aiopioneer-0.6.0a4/aiopioneer.egg-info/entry_points.txt
--rw-rw----   0 root         (0) adm          (4)       11 2024-03-31 12:01:34.000000 aiopioneer-0.6.0a4/aiopioneer.egg-info/top_level.txt
--rw-rw----   0 root         (0) adm          (4)       38 2024-03-31 12:01:36.033792 aiopioneer-0.6.0a4/setup.cfg
--rw-rw----   0 root         (0) adm          (4)     1101 2024-03-31 08:50:09.000000 aiopioneer-0.6.0a4/setup.py
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-02 20:29:03.007535 aiopioneer-0.6.0a6/
+-rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.6.0a6/LICENSE
+-rw-rw----   0 root         (0) adm          (4)    15367 2024-04-02 20:29:03.005794 aiopioneer-0.6.0a6/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)    14715 2024-03-13 09:14:43.000000 aiopioneer-0.6.0a6/README.md
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-02 20:29:02.677539 aiopioneer-0.6.0a6/aiopioneer/
+-rw-rw----   0 root         (0) adm          (4)       68 2024-03-27 20:16:44.000000 aiopioneer-0.6.0a6/aiopioneer/__init__.py
+-rw-rw----   0 root         (0) adm          (4)    11031 2024-04-01 16:54:34.000000 aiopioneer-0.6.0a6/aiopioneer/cli.py
+-rw-rw----   0 root         (0) adm          (4)    13805 2024-04-01 19:37:10.000000 aiopioneer-0.6.0a6/aiopioneer/commands.py
+-rw-rw----   0 root         (0) adm          (4)    15083 2024-04-02 20:26:43.000000 aiopioneer-0.6.0a6/aiopioneer/const.py
+-rw-rw----   0 root         (0) adm          (4)    18687 2024-03-27 20:47:07.000000 aiopioneer-0.6.0a6/aiopioneer/param.py
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-02 20:29:02.967535 aiopioneer-0.6.0a6/aiopioneer/parsers/
+-rw-rw----   0 root         (0) adm          (4)     8175 2024-03-31 07:36:23.000000 aiopioneer-0.6.0a6/aiopioneer/parsers/__init__.py
+-rw-rw----   0 root         (0) adm          (4)     3419 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a6/aiopioneer/parsers/audio.py
+-rw-rw----   0 root         (0) adm          (4)    19209 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a6/aiopioneer/parsers/dsp.py
+-rw-rw----   0 root         (0) adm          (4)    25466 2024-03-31 11:50:52.000000 aiopioneer-0.6.0a6/aiopioneer/parsers/information.py
+-rw-rw----   0 root         (0) adm          (4)      599 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a6/aiopioneer/parsers/response.py
+-rw-rw----   0 root         (0) adm          (4)    23416 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a6/aiopioneer/parsers/settings.py
+-rw-rw----   0 root         (0) adm          (4)    15086 2024-04-01 23:17:50.000000 aiopioneer-0.6.0a6/aiopioneer/parsers/system.py
+-rw-rw----   0 root         (0) adm          (4)     6987 2024-04-01 21:42:04.000000 aiopioneer-0.6.0a6/aiopioneer/parsers/tuner.py
+-rw-rw----   0 root         (0) adm          (4)     8405 2024-03-13 09:14:44.000000 aiopioneer-0.6.0a6/aiopioneer/parsers/video.py
+-rw-rw----   0 root         (0) adm          (4)    86849 2024-04-02 20:28:44.000000 aiopioneer-0.6.0a6/aiopioneer/pioneer_avr.py
+-rw-rw----   0 root         (0) adm          (4)     5266 2024-04-01 23:17:31.000000 aiopioneer-0.6.0a6/aiopioneer/util.py
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-02 20:29:02.987535 aiopioneer-0.6.0a6/aiopioneer.egg-info/
+-rw-rw----   0 root         (0) adm          (4)    15367 2024-04-02 20:29:02.000000 aiopioneer-0.6.0a6/aiopioneer.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)      614 2024-04-02 20:29:02.000000 aiopioneer-0.6.0a6/aiopioneer.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) adm          (4)        1 2024-04-02 20:29:02.000000 aiopioneer-0.6.0a6/aiopioneer.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) adm          (4)       51 2024-04-02 20:29:02.000000 aiopioneer-0.6.0a6/aiopioneer.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) adm          (4)       11 2024-04-02 20:29:02.000000 aiopioneer-0.6.0a6/aiopioneer.egg-info/top_level.txt
+-rw-rw----   0 root         (0) adm          (4)       38 2024-04-02 20:29:03.010861 aiopioneer-0.6.0a6/setup.cfg
+-rw-rw----   0 root         (0) adm          (4)     1101 2024-03-31 08:50:09.000000 aiopioneer-0.6.0a6/setup.py
```

### Comparing `aiopioneer-0.6.0a4/LICENSE` & `aiopioneer-0.6.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a4/PKG-INFO` & `aiopioneer-0.6.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopioneer
-Version: 0.6.0a4
+Version: 0.6.0a6
 Summary: Asyncio Python library for controlling a Pioneer AVR via its API
 Home-page: https://github.com/crowbarz/aiopioneer.git
 Author: Crowbar Z
 Author-email: crowbarz@outlook.com
 Keywords: pioneer avr asyncio
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `aiopioneer-0.6.0a4/README.md` & `aiopioneer-0.6.0a6/README.md`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a4/aiopioneer/cli.py` & `aiopioneer-0.6.0a6/aiopioneer/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import logging
 import sys
 import json
 import argparse
 
 from aiopioneer import PioneerAVR
-from aiopioneer.const import DEFAULT_PORT
+from aiopioneer.const import Zones, DEFAULT_PORT
 from aiopioneer.param import (
     PARAM_DEBUG_LISTENER,
     PARAM_DEBUG_RESPONDER,
     PARAM_DEBUG_UPDATER,
     PARAM_DEBUG_COMMAND,
 )
 from aiopioneer.pioneer_avr import PIONEER_COMMANDS
@@ -72,29 +72,29 @@
     if args.query_device_info:
         await pioneer.query_device_info()
     if args.query_zones:
         await pioneer.query_zones()
         _LOGGER.info("AVR zones discovered: %s", pioneer.zones)
 
     reader, _writer = await connect_stdin_stdout()
-    zone = "1"
+    zone = Zones.Z1
     while True:
         print(f"Current zone is {zone}")
         res = await reader.readline()
         if not res:
             break
         tokens = res.decode().strip().split(maxsplit=1)
         num_tokens = len(tokens)
         if num_tokens <= 0:
             continue
 
         cmd = tokens[0]
         arg = None if num_tokens == 1 else tokens[1]
         if cmd == "zone":
-            zone_new = arg
+            zone_new = Zones(arg)
             if zone_new and zone_new in pioneer.zones:
                 zone = zone_new
                 print(f"Setting current zone to {zone}")
             else:
                 print(f"ERROR: Unknown zone {zone_new}")
         elif cmd == "exit" or cmd == "quit":
             print("Exiting")
@@ -211,15 +211,15 @@
             listening_mode = arg if arg else ""
             await pioneer.set_listening_mode(listening_mode)
         elif cmd == "set_tuner_frequency":
             subargs = arg.split(" ", maxsplit=1)
             try:
                 band = subargs[0]
                 frequency = float(subargs[1]) if len(subargs) > 1 else None
-                await pioneer.set_tuner_frequency(band, frequency, zone=zone)
+                await pioneer.set_tuner_frequency(band, frequency)
             except Exception as exc:  # pylint: disable=broad-except
                 print(
                     f'ERROR: Invalid parameters for set_tuner_frequency "{arg}": {exc}'
                 )
         elif cmd in ["send_raw_command", ">"]:
             if arg:
                 print(f"Sending raw command {arg}")
```

### Comparing `aiopioneer-0.6.0a4/aiopioneer/const.py` & `aiopioneer-0.6.0a6/aiopioneer/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Constants for aiopioneer."""
 
 from enum import StrEnum
 
 DEFAULT_PORT = 8102
-VERSION = "0.6.0a4"
+VERSION = "0.6.0a6"
 
 
 class Zones(StrEnum):
     """Valid aiopioneer zones."""
 
     ALL = "ALL"
     Z1 = "1"
```

### Comparing `aiopioneer-0.6.0a4/aiopioneer/param.py` & `aiopioneer-0.6.0a6/aiopioneer/param.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a4/aiopioneer/parsers/__init__.py` & `aiopioneer-0.6.0a6/aiopioneer/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a4/aiopioneer/parsers/audio.py` & `aiopioneer-0.6.0a6/aiopioneer/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a4/aiopioneer/parsers/dsp.py` & `aiopioneer-0.6.0a6/aiopioneer/parsers/dsp.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a4/aiopioneer/parsers/information.py` & `aiopioneer-0.6.0a6/aiopioneer/parsers/information.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a4/aiopioneer/parsers/response.py` & `aiopioneer-0.6.0a6/aiopioneer/parsers/response.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a4/aiopioneer/parsers/settings.py` & `aiopioneer-0.6.0a6/aiopioneer/parsers/settings.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a4/aiopioneer/parsers/system.py` & `aiopioneer-0.6.0a6/aiopioneer/parsers/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """aiopioneer response parsers for core system responses."""
 
 import re
 
 from aiopioneer.param import (
     PARAM_QUERY_SOURCES,
-    PARAM_TUNER_AM_FREQ_STEP,
     PARAM_MHL_SOURCE,
     PARAM_SPEAKER_SYSTEM_MODES,
 )
 from aiopioneer.const import (
     SOURCE_TUNER,
     MEDIA_CONTROL_SOURCES,
     SPEAKER_MODES,
```

### Comparing `aiopioneer-0.6.0a4/aiopioneer/parsers/tuner.py` & `aiopioneer-0.6.0a6/aiopioneer/parsers/tuner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 """aiopioneer response parsers for tuner parameters."""
 
-import logging
-
 from aiopioneer.param import PARAM_TUNER_AM_FREQ_STEP
 from aiopioneer.const import Zones, TunerBand
 from .response import Response
 
-_LOGGER = logging.getLogger(__name__)
-
 
 class TunerParsers:
     """Tuner response parsers."""
 
     _ignore_preset = True  # ignore first preset response
-    _cached_preset_raw: str = None  # preset updated after tuner frequency update
-    _cached_frequency: float = None  # cache frequency to clear preset
+    _current_preset_raw: str = None  # current value of preset
+    _cached_preset_raw: str = None  # cached preset, update after tuner frequency update
+    _current_freq: float = None  # current frequency, clear preset when changed
 
     @staticmethod
     def frequency_fm(raw: str, params: dict, zone=Zones.ALL, command="FR") -> list:
         """Response parser for FM tuner frequency."""
-        freq = float(raw) / 100
+        new_freq = float(raw) / 100
+        current_freq = TunerParsers._current_freq
         parsed = []
         parsed.extend(
             [
                 Response(
                     raw=raw,
                     response_command=command,
                     base_property="tuner",
@@ -34,30 +32,31 @@
                 ),
                 Response(
                     raw=raw,
                     response_command=command,
                     base_property="tuner",
                     property_name="frequency",
                     zone=zone,
-                    value=freq,
+                    value=new_freq,
                     queue_commands=None,
                 ),
             ]
         )
         if TunerParsers._cached_preset_raw:
             parsed.extend(TunerParsers._update_preset(params, zone))
-        elif TunerParsers._cached_frequency != freq:
+        elif current_freq != new_freq:
             parsed.extend(TunerParsers._clear_preset(params, zone))
-        TunerParsers._cached_frequency = freq
+        TunerParsers._current_freq = new_freq
         return parsed
 
     @staticmethod
     def frequency_am(raw: str, params: dict, zone=Zones.ALL, command="FR") -> list:
         """Response parser AM tuner frequency."""
-        freq = float(raw)
+        new_freq = float(raw)
+        current_freq = TunerParsers._current_freq
         parsed = []
         queue_commands = None
         if params.get(PARAM_TUNER_AM_FREQ_STEP) is None:
             queue_commands = ["_sleep(2)", "_calculate_am_frequency_step"]
 
         parsed.extend(
             [
@@ -72,20 +71,24 @@
                 ),
                 Response(
                     raw=raw,
                     response_command=command,
                     base_property="tuner",
                     property_name="frequency",
                     zone=zone,
-                    value=freq,
+                    value=new_freq,
                     queue_commands=None,
                 ),
             ]
         )
-        parsed.extend(TunerParsers._update_preset(params, zone))
+        if TunerParsers._cached_preset_raw:
+            parsed.extend(TunerParsers._update_preset(params, zone))
+        elif current_freq != new_freq:
+            parsed.extend(TunerParsers._clear_preset(params, zone))
+            TunerParsers._current_freq = new_freq
         return parsed
 
     @staticmethod
     def preset(raw: str, _params: dict, zone=Zones.ALL, command="PR") -> list:
         """Response parser for tuner preset. Cache until next frequency update."""
         parsed = []
         TunerParsers._cached_preset_raw = raw
@@ -102,41 +105,44 @@
         )
         return parsed
 
     @staticmethod
     def _update_preset(_params: dict, zone=Zones.ALL, command="PR") -> list:
         """Parse and update tuner preset from cached values."""
         parsed = []
-        if TunerParsers._cached_preset_raw is None:
+        current_preset_raw = TunerParsers._current_preset_raw
+        cached_preset_raw = TunerParsers._cached_preset_raw
+        ignore_preset = TunerParsers._ignore_preset
+
+        TunerParsers._current_preset_raw = cached_preset_raw
+        if cached_preset_raw is None or current_preset_raw == cached_preset_raw:
             return parsed
-        if TunerParsers._ignore_preset:
+        if ignore_preset:
             ## Ignore first preset response
-            _LOGGER.info("ignoring first preset response")
-            TunerParsers._ignore_preset = False
             TunerParsers._cached_preset_raw = None
+            TunerParsers._ignore_preset = False
             return parsed
 
-        raw = TunerParsers._cached_preset_raw
         # pylint: disable=unsubscriptable-object
-        tuner_class = raw[:1]
-        tuner_preset = int(raw[1:])
+        tuner_class = cached_preset_raw[:1]
+        tuner_preset = int(cached_preset_raw[1:])
         TunerParsers._cached_preset_raw = None
         parsed.extend(
             [
                 Response(
-                    raw=raw,
+                    raw=cached_preset_raw,
                     response_command=command,
                     base_property="tuner",
                     property_name="class",
                     zone=zone,
                     value=tuner_class,
                     queue_commands=None,
                 ),
                 Response(
-                    raw=raw,
+                    raw=cached_preset_raw,
                     response_command=command,
                     base_property="tuner",
                     property_name="preset",
                     zone=zone,
                     value=tuner_preset,
                     queue_commands=None,
                 ),
@@ -167,14 +173,16 @@
                     property_name="preset",
                     zone=zone,
                     value=None,
                     queue_commands=None,
                 ),
             ]
         )
+        TunerParsers._current_preset_raw = None
+        TunerParsers._cached_preset_raw = None
         return parsed
 
     @staticmethod
     def am_frequency_step(raw: str, _params: dict, zone=None, command="SUQ") -> list:
         """Response parser for AM frequency step. (Supported on very few AVRs)"""
         parsed = []
         parsed.append(
```

### Comparing `aiopioneer-0.6.0a4/aiopioneer/parsers/video.py` & `aiopioneer-0.6.0a6/aiopioneer/parsers/video.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a4/aiopioneer/pioneer_avr.py` & `aiopioneer-0.6.0a6/aiopioneer/pioneer_avr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Pioneer AVR API (async)."""
 
 # pylint: disable=relative-beyond-top-level disable=too-many-lines
 
-
 import asyncio
 import copy
 import logging
 import re
 import math
 import time
 import traceback
@@ -80,14 +79,15 @@
     DSP_DRC,
     DSP_HEIGHT_GAIN,
     DSP_VIRTUAL_DEPTH,
     DSP_DIGITAL_FILTER,
 )
 
 from .parsers import process_raw_response
+from .parsers.response import Response
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class PioneerAVR:
     """Pioneer AVR interface."""
 
@@ -113,74 +113,74 @@
         self._timeout = timeout
         self.scan_interval = scan_interval
 
         # Public properties
         self.model = None
         self.software_version = None
         self.mac_addr = None
-        self.available = False
-        self.zones = []
-        self.power = {}
-        self.volume = {}
-        self.max_volume = {}
-        self.mute = {}
-        self.source = {}
+
+        self.available = False  # connected to avr
+        self.initial_update = None  # initial update completed
+        self.zones: list[Zones] = []
+        self.power: dict[Zones, bool] = {}
+        self.volume: dict[Zones, int] = {}
+        self.max_volume: dict[Zones, int] = {}
+        self.mute: dict[Zones, bool] = {}
+        self.source: dict[Zones, str] = {}
         self.listening_mode = ""
         self.listening_mode_raw = ""
-        self.media_control_mode = {}
+        self.media_control_mode: dict[Zones, str] = {}
 
         # FUNC: TONE
-        self.tone = {}
+        self.tone: dict[Zones, dict] = {}
 
         # FUNC: AMP
-        self.amp = {}
+        self.amp: dict[str, Any] = {}
 
         # FUNC: TUNER
-        self.tuner = {}
+        self.tuner: dict[str, Any] = {}
 
         # Complex object that holds multiple different props for the CHANNEL/DSP functions
-        self.channel_levels = {}
-        self.dsp = {}
-        self.video = {}
-        self.system = {}
-        self.audio = {}
+        self.channel_levels: dict[str, Any] = {}
+        self.dsp: dict[str, Any] = {}
+        self.video: dict[str, Any] = {}
+        self.system: dict[str, Any] = {}
+        self.audio: dict[str, Any] = {}
 
         # Parameters
         self._default_params = PARAM_DEFAULTS
         self._system_params = PARAM_DEFAULTS_SYSTEM
-        self._user_params = None
-        self._params = None
+        self._user_params: dict[str, Any] = None
+        self._params: dict[str, Any] = None
         self.set_user_params(params)
 
         # Internal state
         self._connect_lock = asyncio.Lock()
         self._disconnect_lock = asyncio.Lock()
         self._update_lock = asyncio.Lock()
         self._request_lock = asyncio.Lock()
         self._update_event = asyncio.Event()
         self._response_event = asyncio.Event()
-        self._response_queue = []
+        self._response_queue: list[Response] = []
         self._queue_responses = False
         self._reconnect = True
         self._full_update = True
         self._last_updated = None
         self._last_command = None
         self._reader = None
         self._writer = None
         self._listener_task = None
         self._responder_task = None
         self._reconnect_task = None
         self._updater_task = None
         self._command_queue_task = None
-        self._defer_initial_update = None
-        # Stores a list of commands to run after receiving an event from the AVR
-        self._command_queue: list[str] = []
+        self._command_queue: list[str] = []  # queue of commands to execute
         self._power_zone_1 = None
-        self._source_name_to_id = {}
-        self._source_id_to_name = {}
+        self._source_name_to_id: dict[str, str] = {}
+        self._source_id_to_name: dict[str, str] = {}
         self._zone_callback = {}
         # self._update_callback = None
 
     def __del__(self):
         _LOGGER.debug(">> PioneerAVR.__del__()")
 
     @property
@@ -363,18 +363,14 @@
                 delay = get_backoff_delay(retry)
                 _LOGGER.debug("waiting %ds before retrying connection", delay)
                 await asyncio.sleep(delay)
 
                 retry += 1
                 try:
                     await self.connect()
-                    # 20201212 removed as connect already schedules full update
-                    # _LOGGER.debug("Scheduling full AVR status update")
-                    # self._full_update = True
-                    # await self.update()
                     if self.available:
                         break
                 except asyncio.CancelledError:  # pylint: disable=try-except-raise
                     # pass through to outer except
                     raise
                 except Exception as exc:  # pylint: disable=broad-except
                     _LOGGER.debug(
@@ -445,24 +441,24 @@
                     self._response_event.set()
                     ## Do not yield, process all responses first
 
                 ## Detect Zone 1 power on for volume workaround
                 action = ""
                 power_on_volume_bounce = self._params[PARAM_POWER_ON_VOLUME_BOUNCE]
                 if power_on_volume_bounce and self._power_zone_1 is not None:
-                    if not self._power_zone_1 and self.power.get("1"):
+                    if not self._power_zone_1 and self.power.get(Zones.Z1):
                         ## Zone 1 powered on, schedule bounce task
                         _LOGGER.info("scheduling main zone volume workaround")
                         self.queue_command(
                             "volume_up", skip_if_queued=False, insert_at=0
                         )
                         self.queue_command(
                             "volume_down", skip_if_queued=False, insert_at=1
                         )
-                self._power_zone_1 = self.power.get("1")  # cache value
+                self._power_zone_1 = self.power.get(Zones.Z1)  # cache value
 
                 # Implement a command queue so that we can queue commands if we
                 # need to update attributes that only get updated when we
                 # request them to change.
                 if len(self._command_queue) > 0:
                     self._command_queue_schedule()
 
@@ -693,16 +689,15 @@
                 zone,
                 prefix,
                 ignore_error,
                 rate_limit,
                 suffix,
             )
 
-        zone = Zones(zone)
-        raw_command = PIONEER_COMMANDS.get(command, {}).get(zone.value)
+        raw_command = PIONEER_COMMANDS.get(command, {}).get(zone)
         try:
             if type(raw_command) is list:
                 if len(raw_command) == 2:
                     # Handle command as request
                     expected_response = raw_command[1]
                     raw_command = raw_command[0]
                     response = await self.send_raw_request(
@@ -728,76 +723,84 @@
             _LOGGER.error("cannot execute %s command: %s", command, exc)
             return False
 
     # Initialisation functions
     async def query_zones(self, force_update: bool = False) -> None:
         """Query zones on Pioneer AVR by querying power status."""
         _LOGGER.info("querying available zones on AVR")
-        ignored_zones = self._params[PARAM_IGNORED_ZONES]
+        ignored_zones = [Zones(z) for z in self._params[PARAM_IGNORED_ZONES]]
         ignore_volume_check = self._params[PARAM_IGNORE_VOLUME_CHECK]
         added_zones = False
         # Defer updates to after query_zones has completed
         async with self._update_lock:
-            if await self.send_command("query_power", "1", ignore_error=True) and (
+            if await self.send_command("query_power", Zones.Z1, ignore_error=True) and (
                 ignore_volume_check
-                or await self.send_command("query_volume", "1", ignore_error=True)
+                or await self.send_command("query_volume", Zones.Z1, ignore_error=True)
             ):
-                if "1" not in self.zones and "1" not in ignored_zones:
+                if Zones.Z1 not in self.zones and Zones.Z1 not in ignored_zones:
                     _LOGGER.info("Zone 1 discovered")
-                    self.zones.append("1")
+                    self.zones.append(Zones.Z1)
                     added_zones = True
-                    self.max_volume["1"] = self._params[PARAM_MAX_VOLUME]
+                    self.max_volume[Zones.Z1] = self._params[PARAM_MAX_VOLUME]
                     await asyncio.sleep(0)  # yield to listener task
 
-                    if not self.power["1"] and self._defer_initial_update is False:
+                    if not self.power[Zones.Z1] and self.initial_update is None:
                         ## Defer initial update if Zone 1 is not powered on
                         _LOGGER.debug("deferring initial update")
-                        self._defer_initial_update = True
+                        self.initial_update = False
             else:
                 raise RuntimeError("Zone 1 not found on AVR")
 
-            if await self.send_command("query_power", "2", ignore_error=True) and (
+            if await self.send_command("query_power", Zones.Z2, ignore_error=True) and (
                 ignore_volume_check
-                or await self.send_command("query_volume", "2", ignore_error=True)
+                or await self.send_command("query_volume", Zones.Z2, ignore_error=True)
             ):
-                if "2" not in self.zones and "2" not in ignored_zones:
+                if Zones.Z2 not in self.zones and Zones.Z2 not in ignored_zones:
                     _LOGGER.info("Zone 2 discovered")
-                    self.zones.append("2")
+                    self.zones.append(Zones.Z2)
                     added_zones = True
-                    self.max_volume["2"] = self._params[PARAM_MAX_VOLUME_ZONEX]
+                    self.max_volume[Zones.Z2.value] = self._params[
+                        PARAM_MAX_VOLUME_ZONEX
+                    ]
 
-            if await self.send_command("query_power", "3", ignore_error=True) and (
+            if await self.send_command("query_power", Zones.Z3, ignore_error=True) and (
                 ignore_volume_check
-                or await self.send_command("query_volume", "3", ignore_error=True)
+                or await self.send_command("query_volume", Zones.Z3, ignore_error=True)
             ):
-                if "3" not in self.zones and "3" not in ignored_zones:
+                if Zones.Z3 not in self.zones and Zones.Z3 not in ignored_zones:
                     _LOGGER.info("Zone 3 discovered")
-                    self.zones.append("3")
+                    self.zones.append(Zones.Z3)
                     added_zones = True
-                    self.max_volume["3"] = self._params[PARAM_MAX_VOLUME_ZONEX]
-            if await self.send_command("query_power", "Z", ignore_error=True) and (
+                    self.max_volume[Zones.Z3.value] = self._params[
+                        PARAM_MAX_VOLUME_ZONEX
+                    ]
+            if await self.send_command(
+                "query_power", Zones.HDZ, ignore_error=True
+            ) and (
                 ignore_volume_check
-                or await self.send_command("query_volume", "Z", ignore_error=True)
+                or await self.send_command("query_volume", Zones.HDZ, ignore_error=True)
             ):
-                if "Z" not in self.zones and "Z" not in ignored_zones:
+                if Zones.HDZ not in self.zones and Zones.HDZ not in ignored_zones:
                     _LOGGER.info("HDZone discovered")
-                    self.zones.append("Z")
+                    self.zones.append(Zones.HDZ)
                     added_zones = True
-                    self.max_volume["Z"] = self._params[PARAM_MAX_VOLUME_ZONEX]
+                    self.max_volume[Zones.HDZ.value] = self._params[
+                        PARAM_MAX_VOLUME_ZONEX
+                    ]
         if added_zones or force_update:
             await self.update(full=True)
 
     async def update_zones(self) -> None:
         """Update zones from ignored_zones and re-query zones."""
         removed_zones = False
         for zone in [Zones(z) for z in self._params[PARAM_IGNORED_ZONES]]:
-            if zone.value in self.zones:
+            if zone in self.zones:
                 zone_name = "HDZone" if zone == Zones.HDZ else zone
-                _LOGGER.info("Removing zone %s", zone_name)
-                self.zones.remove(zone.value)
+                _LOGGER.info("removing zone %s", zone_name)
+                self.zones.remove(zone)
                 self._call_zone_callbacks([zone])  # update availability
                 removed_zones = True
         await self.query_zones(force_update=removed_zones)
 
     def set_source_dict(self, sources: dict[str, str]) -> None:
         """Manually set source id<->name translation tables."""
         self._set_query_sources(False)
@@ -828,15 +831,14 @@
                 elif response is not False:
                     timeouts = 0
         if not self._source_name_to_id:
             _LOGGER.warning("no input sources found on AVR")
 
     def get_source_list(self, zone: Zones = Zones.Z1) -> list[str]:
         """Return list of available input sources."""
-        zone = Zones(zone)
         source_ids = self._params.get(PARAM_ZONE_SOURCES[zone], [])
         return list(
             self._source_name_to_id.keys()
             if not source_ids
             else [
                 self._source_id_to_name[s]
                 for s in source_ids
@@ -844,15 +846,14 @@
             ]
         )
 
     def get_source_dict(self, zone: Zones = None) -> dict[str, str]:
         """Return source id<->name translation tables."""
         if zone is None:
             return MappingProxyType(self._source_name_to_id)
-        zone = Zones(zone)
         source_ids = self._params.get(PARAM_ZONE_SOURCES[zone], [])
         return (
             self._source_name_to_id
             if not source_ids
             else {k: v for k, v in self._source_name_to_id.items() if v in source_ids}
         )
 
@@ -869,20 +870,17 @@
         source_name = None
         if source_id in self._source_id_to_name:
             source_name = self._source_id_to_name[source_id]
             self._source_id_to_name.pop(source_id)
         if source_name in self._source_name_to_id:
             self._source_name_to_id.pop(source_name)
 
-    def get_zone_listening_modes(
-        self, zone: Zones = Zones.Z1
-    ) -> dict[str, str] | None:
+    def get_zone_listening_modes(self, zone: Zones = Zones.Z1) -> dict[str, str] | None:
         """Return dict of valid listening modes and names for zone."""
         ## Listening modes only supported on main zone
-        zone = Zones(zone)
         if zone == Zones.Z1:
             multichannel = self.audio.get("input_multichannel")
             listening_modes = self._params.get(PARAM_AVAILABLE_LISTENING_MODES, {})
             zone_listening_modes = {}
             for mode_id, mode_details in listening_modes.items():
                 if (multichannel and mode_details[2]) or (
                     not multichannel and mode_details[1]
@@ -939,40 +937,34 @@
             ]
         )
 
     def get_supported_media_controls(self, zone: Zones) -> list[str] | None:
         """Return a list of all valid media control actions for a given zone.
         If the provided zone source is not currently compatible with media controls,
         null will be returned."""
-        zone = Zones(zone)
-        if self.media_control_mode.get(zone.value) is not None:
+        if self.media_control_mode.get(zone) is not None:
             return list(
                 [
                     k
                     for k in MEDIA_CONTROL_COMMANDS.get(
-                        self.media_control_mode.get(zone.value)
+                        self.media_control_mode.get(zone)
                     ).keys()
                 ]
             )
         else:
             return None
 
     async def query_device_info(self) -> None:
         """Query device information from Pioneer AVR."""
         _LOGGER.info("querying device information")
         commands = [k for k in PIONEER_COMMANDS if k.startswith("system_query_")]
         for command in commands:
             await self.send_command(command, ignore_error=True)
         await asyncio.sleep(0)  # yield to updater task
 
-        ## Retry device info query on initial update
-        if not self.zones and self._defer_initial_update is None:
-            _LOGGER.debug("deferring device information query")
-            self._defer_initial_update = False
-
         self._set_default_params_model()  # Update default params for this model
         self._update_listening_modes()  # Update valid listening modes
 
     def queue_device_info_query(self) -> None:
         """Queue device information query from Pioneer AVR."""
         commands = [k for k in PIONEER_COMMANDS if k.startswith("system_query_")]
         for command in commands:
@@ -984,39 +976,38 @@
         #
         # https://github.com/home-assistant/architecture/blob/master/adr/0004-webscraping.md
         #
         # VSX-930 will report model and software version, but not MAC address.
         # It will report software version only if Zone 1 is powered on.
         # It is unknown how iControlAV5 determines this on a routed network.
 
-    # Callback functions
+    ## Callback functions
+
     def set_zone_callback(
         self, zone: Zones, callback: Callable[..., None] | None = None
     ) -> None:
         """Register a callback for a zone."""
-        zone = Zones(zone)
-        if zone.value in self.zones:
+        if zone in self.zones or zone == Zones.ALL:
             if callback:
-                self._zone_callback[zone.value] = callback
+                self._zone_callback[zone] = callback
             else:
-                self._zone_callback.pop(zone.value)
+                self._zone_callback.pop(zone)
 
     def clear_zone_callbacks(self) -> None:
         """Clear all callbacks for a zone."""
         self._zone_callback = {}
 
     def _call_zone_callbacks(self, zones: list[Zones] | None = None) -> None:
         """Call callbacks to signal updated zone(s)."""
-        if not zones or Zones.ALL in zones:
-            zones = self.zones
-        for zone in [Zones(z) for z in zones]:
-            if zone.value in self._zone_callback:
-                callback = self._zone_callback[zone.value]
+        if not zones:
+            zones = self.zones + [Zones.ALL]
+        for zone in zones:
+            if zone in self._zone_callback:
+                callback = self._zone_callback[zone]
                 if callback:
-                    # _LOGGER.debug("calling callback for zone %s", zone)
                     callback()
 
     # Update functions
     def _parse_response(self, response_raw: str) -> dict[str, Any]:
         """Parse response and update cached parameters."""
         updated_zones = set()
 
@@ -1026,39 +1017,39 @@
                 if isfunction(response.base_property):
                     ## Call a function
                     response.base_property(self)
                 elif response.base_property is not None:
                     current_base = getattr(self, response.base_property)
                     is_global = response.zone in [Zones.ALL, None]
                     if response.property_name is None and not is_global:
-                        current_value = current_base.get(response.zone.value)
+                        current_value = current_base.get(response.zone)
                         if current_value != response.value:
-                            current_base[response.zone.value] = response.value
+                            current_base[response.zone] = response.value
                             setattr(self, response.base_property, current_base)
                             _LOGGER.info(
                                 "Zone %s: %s: %s -> %s (%s)",
-                                response.zone.value,
+                                response.zone,
                                 response.base_property,
                                 current_value,
                                 response.value,
                                 response.raw,
                             )
                     elif response.property_name is not None and not is_global:
                         ## Default zone dict first, otherwise we hit an exception
-                        current_base.setdefault(response.zone.value, {})
-                        current_prop = current_base.get(response.zone.value)
+                        current_base.setdefault(response.zone, {})
+                        current_prop = current_base.get(response.zone)
                         current_value = current_prop.get(response.property_name)
                         if current_value != response.value:
-                            current_base[response.zone.value][
+                            current_base[response.zone][
                                 response.property_name
                             ] = response.value
                             setattr(self, response.base_property, current_base)
                             _LOGGER.info(
                                 "Zone %s: %s.%s: %s -> %s (%s)",
-                                response.zone.value,
+                                response.zone,
                                 response.base_property,
                                 response.property_name,
                                 current_value,
                                 response.value,
                                 response.raw,
                             )
                     elif response.property_name is None and is_global:
@@ -1095,34 +1086,31 @@
                         self.queue_command(command)
 
                 # Some specific overrides for the command queue, these are only
                 # requested if we are not doing a full update
                 if (
                     response.base_property == "power"
                     and response.value
-                    and self._defer_initial_update
+                    and not self.initial_update
                 ):
                     ## Perform full update on first power on of Zone 1
                     _LOGGER.info(
                         "retrying device information query on Zone 1 first power on"
                     )
                     self.queue_device_info_query()
                     self.queue_command("_full_update")
-                    self._defer_initial_update = None
                 elif (
                     (response.response_command in ["PWR", "FN", "AUB", "AUA"])
                     and (not self._full_update)
                     and (not self._params.get(PARAM_DISABLE_AUTO_QUERY))
-                    and (
-                        self.power.get("1")
-                        or self.power.get("2")
-                        or self.power.get("3")
-                        or self.power.get(
-                            "Z"
-                        )  # These should only queue if the AVR is on
+                    and (  # These should only queue if the AVR is on
+                        self.power.get(Zones.Z1)
+                        or self.power.get(Zones.Z2)
+                        or self.power.get(Zones.Z3)
+                        or self.power.get(Zones.HDZ)
                     )
                 ):
                     ## TODO: not sure why check self.tuner here?
                     if self.tuner is not None:
                         self.queue_command("_sleep(4)")
                         self.queue_command("query_listening_mode")
                         self.queue_command("query_audio_information")
@@ -1202,34 +1190,34 @@
         ):
             # Timeout occurred, indicates AVR disconnected
             raise TimeoutError("Timeout waiting for data")
 
         # Zone 1 updates only, we loop through this to allow us to add commands
         # to read without needing to add it here, also only do this if the zone
         # is powered on
-        if Zones(zone) is Zones.Z1 and bool(self.power.get("1")):
+        if Zones(zone) is Zones.Z1 and bool(self.power.get(Zones.Z1)):
             for comm in query_commands:
-                if PIONEER_COMMANDS.get(comm).get("1"):
+                if PIONEER_COMMANDS.get(comm).get(Zones.Z1):
                     await self.send_command(comm, zone, ignore_error=True)
 
         # Zone 2 updates only, only available if zone 2 is on
-        if Zones(zone) is Zones.Z2 and bool(self.power.get("2")):
+        if Zones(zone) is Zones.Z2 and bool(self.power.get(Zones.Z2)):
             for comm in query_commands:
-                if PIONEER_COMMANDS.get(comm).get("2"):
+                if PIONEER_COMMANDS.get(comm).get(Zones.Z2):
                     await self.send_command(comm, zone, ignore_error=True)
 
         # CHANNEL updates are handled differently as it requires more complex
         # logic to send the commands we use the set_channel_levels command
         # and prefix the query to it.
         # Only run this if the main zone is on
         # HDZone does not have any channels
         if ("channels" in self._params.get(PARAM_ENABLED_FUNCTIONS)) and (
             not self._params.get(PARAM_DISABLE_AUTO_QUERY)
         ):
-            if bool(self.power.get("1")) and Zones(zone) is not Zones.HDZ:
+            if bool(self.power.get(Zones.Z1)) and Zones(zone) is not Zones.HDZ:
                 for k in CHANNEL_LEVELS_OBJ:
                     if len(k) == 1:
                         # Add two underscores
                         k = k + "__"
                     elif len(k) == 2:
                         # Add one underscore
                         k = k + "_"
@@ -1268,29 +1256,33 @@
                 _LOGGER.info(
                     "updating AVR status (full=%s, zones=%s, last updated %s)",
                     full_update,
                     self.zones,
                     since_updated_str,
                 )
                 self._last_updated = now
-                self._full_update = False
                 try:
                     ## TODO: update audio, video and display information
                     for zone in self.zones:
                         await self._update_zone(zone)
                     if full_update:
+                        if self.power[Zones.Z1]:
+                            _LOGGER.debug("completed initial update")
+                            self.initial_update = True
+
                         # Trigger updates to all zones on full update
                         self._call_zone_callbacks()
                 except Exception as exc:  # pylint: disable=broad-except
                     _LOGGER.error(
                         "could not update AVR status: %s: %s",
                         type(exc).__name__,
                         str(exc),
                     )
                     _rc = False
+                self._full_update = False
             else:
                 # NOTE: any response from the AVR received within
                 # scan_interval, including keepalives and responses triggered
                 # via the remote and by other clients, will cause the next
                 # update to be skipped if that update is scheduled to occur
                 # within scan_interval of the response.
                 ##
@@ -1334,16 +1326,15 @@
         if len(items) == 0:
             raise ValueError(f"Parameter {val} does not exist for this option")
         else:
             return str(items[0])
 
     def _check_zone(self, zone: Zones) -> Zones:
         """Check that specified zone is valid."""
-        zone = Zones(zone)
-        if zone.value not in self.zones:
+        if zone not in self.zones:
             raise ValueError(f"zone {zone} does not exist on AVR")
         return zone
 
     async def turn_on(self, zone: Zones = Zones.Z1) -> bool | None:
         """Turn on the Pioneer AVR."""
         zone = self._check_zone(zone)
         return await self.send_command("turn_on", zone)
@@ -1841,17 +1832,15 @@
         """Set the level (gain) for amplifier channel in zone."""
         zone = self._check_zone(zone)
         if self.channel_levels.get(zone.value) is None:
             raise ValueError(f"channel level not supported for zone {zone}")
 
         # Check the channel exists
         if self.channel_levels[zone.value].get(channel.upper()) is None:
-            raise ValueError(
-                f"invalid channel {channel} for zone {zone}"
-            )
+            raise ValueError(f"invalid channel {channel} for zone {zone}")
 
         # Append underscores depending on length
         if len(channel) == 1:
             channel = channel + "__"
         elif len(channel) == 2:
             channel = channel + "_"
 
@@ -1859,20 +1848,20 @@
         level = int((level * 2) + 50)
         return await self.send_command(
             "set_channel_levels", zone, channel + str(level), ignore_error=False
         )
 
     async def set_video_settings(self, **arguments) -> bool:
         """Set video settings for a given zone."""
-        zone = str(arguments.get("zone"))
+        zone = Zones(arguments.get("zone"))
         zone = self._check_zone(zone)
 
         # This function is only valid for zone 1, no video settings are
         # available for zone 2, 3, 4 and HDZone
-        if zone != "1":
+        if zone != Zones.Z1:
             raise ValueError(f"Invalid zone {zone}")
 
         # This is a complex function and supports handles requests to update any
         # video related parameters
         for arg in arguments:
             if arg != "zone":
                 if arguments.get(arg) is not None:
@@ -1932,17 +1921,17 @@
                         )
 
         ## TODO: check command rc, refactor to use match
         return True
 
     async def set_dsp_settings(self, **arguments) -> bool:
         """Set the DSP settings for the amplifier."""
-        zone = str(arguments.get("zone"))
+        zone = Zones(arguments.get("zone"))
         zone = self._check_zone(zone)
-        if zone != "1":
+        if zone != Zones.Z1:
             raise ValueError(f"Invalid zone {zone}")
 
         for arg in arguments:
             if arg != "zone":
                 if arguments.get(arg) is not None:
                     if self.dsp.get(arg) is not arguments.get(arg):
                         if isinstance(arguments.get(arg), str):
@@ -2014,15 +2003,15 @@
 
     async def media_control(self, action: str, zone: Zones = Zones.Z1) -> bool:
         """
         Perform media control activities such as play, pause, stop, fast forward
         or rewind.
         """
         zone = self._check_zone(zone)
-        media_commands = self.media_control_mode.get(zone.value)
+        media_commands = self.media_control_mode.get(zone)
         if media_commands is not None:
             command = MEDIA_CONTROL_COMMANDS.get(media_commands, {}).get(action)
             if command is not None:
                 # These commands are ALWAYS sent to zone 1 because each zone
                 # does not have unique commands
                 return await self.send_command(command, Zones.Z1, ignore_error=False)
             else:
```

### Comparing `aiopioneer-0.6.0a4/aiopioneer/util.py` & `aiopioneer-0.6.0a6/aiopioneer/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Pioneer AVR utils. """
+
 import asyncio
-import contextlib
 import socket
 import random
 import logging
 
 RECONNECT_DELAY_MAX = 64
 
 _LOGGER = logging.getLogger(__name__)
```

### Comparing `aiopioneer-0.6.0a4/aiopioneer.egg-info/PKG-INFO` & `aiopioneer-0.6.0a6/aiopioneer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopioneer
-Version: 0.6.0a4
+Version: 0.6.0a6
 Summary: Asyncio Python library for controlling a Pioneer AVR via its API
 Home-page: https://github.com/crowbarz/aiopioneer.git
 Author: Crowbar Z
 Author-email: crowbarz@outlook.com
 Keywords: pioneer avr asyncio
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `aiopioneer-0.6.0a4/aiopioneer.egg-info/SOURCES.txt` & `aiopioneer-0.6.0a6/aiopioneer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0a4/setup.py` & `aiopioneer-0.6.0a6/setup.py`

 * *Files identical despite different names*

