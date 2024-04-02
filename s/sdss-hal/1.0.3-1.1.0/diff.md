# Comparing `tmp/sdss_hal-1.0.3.tar.gz` & `tmp/sdss_hal-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_hal-1.0.3.tar", max compression
+gzip compressed data, was "sdss_hal-1.1.0.tar", max compression
```

## Comparing `sdss_hal-1.0.3.tar` & `sdss_hal-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1504 2024-03-05 20:36:44.700129 sdss_hal-1.0.3/LICENSE.md
--rw-r--r--   0        0        0      816 2024-03-05 20:36:44.700129 sdss_hal-1.0.3/README.md
--rw-r--r--   0        0        0     2644 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      483 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/__init__.py
--rw-r--r--   0        0        0     1761 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/__main__.py
--rw-r--r--   0        0        0      356 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/actor/__init__.py
--rw-r--r--   0        0        0     3070 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/actor/actor.py
--rw-r--r--   0        0        0     2939 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/actor/commands/__init__.py
--rw-r--r--   0        0        0     3478 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/actor/commands/auto.py
--rw-r--r--   0        0        0     1593 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/actor/commands/bypass.py
--rw-r--r--   0        0        0      844 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/actor/commands/calibrations.py
--rw-r--r--   0        0        0     7572 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/actor/commands/expose.py
--rw-r--r--   0        0        0     1599 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/actor/commands/goto.py
--rw-r--r--   0        0        0     4370 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/actor/commands/goto_field.py
--rw-r--r--   0        0        0     2455 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/actor/commands/script.py
--rw-r--r--   0        0        0     1419 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/actor/commands/status.py
--rw-r--r--   0        0        0      687 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/actor/commands/test.py
--rw-r--r--   0        0        0     3097 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/etc/hal.yml
--rw-r--r--   0        0        0     2189 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/etc/schema.json
--rw-r--r--   0        0        0      346 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/etc/scripts/apo/cartchange.inp
--rw-r--r--   0        0        0     1161 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/etc/scripts/apo/eveningcals.inp
--rw-r--r--   0        0        0      161 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/etc/scripts/apo/example.inp
--rw-r--r--   0        0        0     1616 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/etc/scripts/apo/morningcals.inp
--rw-r--r--   0        0        0       35 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/etc/scripts/apo/test.inp
--rw-r--r--   0        0        0      346 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/etc/scripts/lco/cartchange.inp
--rw-r--r--   0        0        0     1056 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/etc/scripts/lco/eveningcals.inp
--rw-r--r--   0        0        0     1450 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/etc/scripts/lco/morningcals.inp
--rw-r--r--   0        0        0     1180 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/exceptions.py
--rw-r--r--   0        0        0     1932 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/helpers/__init__.py
--rw-r--r--   0        0        0    10224 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/helpers/apogee.py
--rw-r--r--   0        0        0     6825 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/helpers/boss.py
--rw-r--r--   0        0        0     5011 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/helpers/cherno.py
--rw-r--r--   0        0        0     1769 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/helpers/ffs.py
--rw-r--r--   0        0        0     6585 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/helpers/jaeger.py
--rw-r--r--   0        0        0    10429 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/helpers/lamps.py
--rw-r--r--   0        0        0     4596 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/helpers/overhead.py
--rw-r--r--   0        0        0     4671 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/helpers/scripts.py
--rw-r--r--   0        0        0    13441 2024-03-05 20:36:44.704129 sdss_hal-1.0.3/src/hal/helpers/tcc.py
--rw-r--r--   0        0        0     1385 2024-03-05 20:36:44.708129 sdss_hal-1.0.3/src/hal/macros/__init__.py
--rw-r--r--   0        0        0     3692 2024-03-05 20:36:44.708129 sdss_hal-1.0.3/src/hal/macros/apogee_dome_flat.py
--rw-r--r--   0        0        0     7098 2024-03-05 20:36:44.708129 sdss_hal-1.0.3/src/hal/macros/auto.py
--rw-r--r--   0        0        0    20939 2024-03-05 20:36:44.708129 sdss_hal-1.0.3/src/hal/macros/expose.py
--rw-r--r--   0        0        0    23236 2024-03-05 20:36:44.708129 sdss_hal-1.0.3/src/hal/macros/goto_field.py
--rw-r--r--   0        0        0    18519 2024-03-05 20:36:44.708129 sdss_hal-1.0.3/src/hal/macros/macro.py
--rw-r--r--   0        0        0     1263 2024-03-05 20:36:44.708129 sdss_hal-1.0.3/src/hal/macros/test_macro.py
--rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 sdss_hal-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-04-02 04:39:15.435595 sdss_hal-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0      816 2024-04-02 04:39:15.435595 sdss_hal-1.1.0/README.md
+-rw-r--r--   0        0        0     2644 2024-04-02 04:39:15.439595 sdss_hal-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      483 2024-04-02 04:39:15.439595 sdss_hal-1.1.0/src/hal/__init__.py
+-rw-r--r--   0        0        0     1761 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/__main__.py
+-rw-r--r--   0        0        0      356 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/actor/__init__.py
+-rw-r--r--   0        0        0     3070 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/actor/actor.py
+-rw-r--r--   0        0        0     2939 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/actor/commands/__init__.py
+-rw-r--r--   0        0        0     3528 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/actor/commands/auto.py
+-rw-r--r--   0        0        0     1593 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/actor/commands/bypass.py
+-rw-r--r--   0        0        0      844 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/actor/commands/calibrations.py
+-rw-r--r--   0        0        0     7899 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/actor/commands/expose.py
+-rw-r--r--   0        0        0     1669 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/actor/commands/goto.py
+-rw-r--r--   0        0        0     4370 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/actor/commands/goto_field.py
+-rw-r--r--   0        0        0     2455 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/actor/commands/script.py
+-rw-r--r--   0        0        0     1419 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/actor/commands/status.py
+-rw-r--r--   0        0        0      687 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/actor/commands/test.py
+-rw-r--r--   0        0        0     3144 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/etc/hal.yml
+-rw-r--r--   0        0        0     2189 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/etc/schema.json
+-rw-r--r--   0        0        0      346 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/etc/scripts/apo/cartchange.inp
+-rw-r--r--   0        0        0     1161 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/etc/scripts/apo/eveningcals.inp
+-rw-r--r--   0        0        0      161 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/etc/scripts/apo/example.inp
+-rw-r--r--   0        0        0     1616 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/etc/scripts/apo/morningcals.inp
+-rw-r--r--   0        0        0       35 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/etc/scripts/apo/test.inp
+-rw-r--r--   0        0        0      346 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/etc/scripts/lco/cartchange.inp
+-rw-r--r--   0        0        0     1056 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/etc/scripts/lco/eveningcals.inp
+-rw-r--r--   0        0        0     1450 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/etc/scripts/lco/morningcals.inp
+-rw-r--r--   0        0        0     1180 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/exceptions.py
+-rw-r--r--   0        0        0     2312 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/helpers/__init__.py
+-rw-r--r--   0        0        0    10224 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/helpers/apogee.py
+-rw-r--r--   0        0        0     6825 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/helpers/boss.py
+-rw-r--r--   0        0        0     5011 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/helpers/cherno.py
+-rw-r--r--   0        0        0     1769 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/helpers/ffs.py
+-rw-r--r--   0        0        0     6710 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/helpers/jaeger.py
+-rw-r--r--   0        0        0    10429 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/helpers/lamps.py
+-rw-r--r--   0        0        0     4732 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/helpers/overhead.py
+-rw-r--r--   0        0        0     4671 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/helpers/scripts.py
+-rw-r--r--   0        0        0    13441 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/helpers/tcc.py
+-rw-r--r--   0        0        0     1385 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/macros/__init__.py
+-rw-r--r--   0        0        0     3844 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/macros/apogee_dome_flat.py
+-rw-r--r--   0        0        0     7351 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/macros/auto.py
+-rw-r--r--   0        0        0    21007 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/macros/expose.py
+-rw-r--r--   0        0        0    23236 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/macros/goto_field.py
+-rw-r--r--   0        0        0    18518 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/macros/macro.py
+-rw-r--r--   0        0        0     1263 2024-04-02 04:39:15.443595 sdss_hal-1.1.0/src/hal/macros/test_macro.py
+-rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 sdss_hal-1.1.0/PKG-INFO
```

### Comparing `sdss_hal-1.0.3/LICENSE.md` & `sdss_hal-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/README.md` & `sdss_hal-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/pyproject.toml` & `sdss_hal-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-hal"
-version = "1.0.3"
+version = "1.1.0"
 description = "High-level observing tool for SDSS-V (replaces SOP)"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/hal"
 repository = "https://github.com/sdss/hal"
 documentation = "https://sdss-hal.readthedocs.org"
```

### Comparing `sdss_hal-1.0.3/src/hal/__main__.py` & `sdss_hal-1.1.0/src/hal/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/actor/actor.py` & `sdss_hal-1.1.0/src/hal/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/actor/commands/__init__.py` & `sdss_hal-1.1.0/src/hal/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/actor/commands/auto.py` & `sdss_hal-1.1.0/src/hal/actor/commands/auto.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # @Author: José Sánchez-Gallego (gallegoj@uw.edu)
 # @Date: 2022-12-26
 # @Filename: auto.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
+import asyncio
+
 from typing import TYPE_CHECKING
 
 import click
 
 from hal.macros.expose import ExposeMacro
 
 from . import hal_command_parser
@@ -125,14 +127,16 @@
     while True:
         # Run the auto loop until the command is cancelled.
         macro.reset(command, count=count)
         if not await macro.run():
             result = False
             break
 
+        await asyncio.sleep(0.1)
+
         if macro.cancelled:
             # Cancelled macros return result=True
             break
 
     if result is False:
         return command.fail()
```

### Comparing `sdss_hal-1.0.3/src/hal/actor/commands/bypass.py` & `sdss_hal-1.1.0/src/hal/actor/commands/bypass.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/actor/commands/calibrations.py` & `sdss_hal-1.1.0/src/hal/actor/commands/calibrations.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/actor/commands/expose.py` & `sdss_hal-1.1.0/src/hal/actor/commands/expose.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, cast
 
 import click
 
 from hal import config
+from hal.helpers import get_default_exposure_time
 from hal.macros.macro import StageType, flatten
 
 from . import hal_command_parser, stages
 
 
 if TYPE_CHECKING:
     from hal.macros.expose import ExposeMacro
@@ -201,15 +202,19 @@
     # for each instrument.
     if (apogee_exposure_time and boss_exposure_time) or (count_apogee and count_boss):
         disable_readout_matching = True
 
     # If nothing has been defined explicitely, revert to the defaults.
     if not exposure_time:
         if not boss_exposure_time and not apogee_exposure_time:
-            exposure_time = config["macros"]["expose"]["fallback"]["exptime"]
+            design_mode: str | None = None
+            assert command.actor.helpers.jaeger, "Jaeger helper not available."
+            if command.actor.helpers.jaeger.configuration:
+                design_mode = command.actor.helpers.jaeger.configuration.design_mode
+            exposure_time = get_default_exposure_time(design_mode)
         elif apogee_exposure_time and not boss_exposure_time:
             boss_exposure_time = apogee_exposure_time
             disable_readout_matching = True
 
     if not count and not count_boss and not count_apogee:
         count = config["macros"]["expose"]["fallback"]["count"]
 
@@ -260,14 +265,15 @@
         return command.fail("The expose macro is already running.")
 
     macro.reset(
         command,
         selected_stages,
         initial_apogee_dither=initial_apogee_dither,
         with_fpi=with_fpi,
+        force=False,
         **params,
     )
 
     result = await macro.run()
 
     if result is False:
         return command.fail()
```

### Comparing `sdss_hal-1.0.3/src/hal/actor/commands/goto.py` & `sdss_hal-1.1.0/src/hal/actor/commands/goto.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 __all__ = ["gotoStow"]
 
 
 async def goto_position(command: HALCommandType, name: str):
     """Go to position."""
 
     try:
+        assert command.actor.helpers.tcc, "TCC helper not available."
         await command.actor.helpers.tcc.goto_position(command, name)
     except HALError as err:
         return command.fail(f"Goto position failed with error: {err}")
 
     return command.finish()
```

### Comparing `sdss_hal-1.0.3/src/hal/actor/commands/goto_field.py` & `sdss_hal-1.1.0/src/hal/actor/commands/goto_field.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/actor/commands/script.py` & `sdss_hal-1.1.0/src/hal/actor/commands/script.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/actor/commands/status.py` & `sdss_hal-1.1.0/src/hal/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/actor/commands/test.py` & `sdss_hal-1.1.0/src/hal/actor/commands/test.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/etc/hal.yml` & `sdss_hal-1.1.0/src/hal/etc/hal.yml`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,17 @@
     pairs: true
     dither: true
     initial_apogee_dither: null
     with_fpi: true
     readout_matching: true
     fallback:
       count: 1
-      exptime: 900.0
+      exptime:
+        default: 900
+        bright_design_mode: 730
 
   auto:
     guider_time: 15
     min_rms: 3.0
     count: 1
 
 goto:
```

### Comparing `sdss_hal-1.0.3/src/hal/etc/schema.json` & `sdss_hal-1.1.0/src/hal/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/etc/scripts/apo/eveningcals.inp` & `sdss_hal-1.1.0/src/hal/etc/scripts/apo/eveningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/etc/scripts/apo/morningcals.inp` & `sdss_hal-1.1.0/src/hal/etc/scripts/apo/morningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/etc/scripts/lco/eveningcals.inp` & `sdss_hal-1.1.0/src/hal/etc/scripts/lco/eveningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/etc/scripts/lco/morningcals.inp` & `sdss_hal-1.1.0/src/hal/etc/scripts/lco/morningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/exceptions.py` & `sdss_hal-1.1.0/src/hal/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/helpers/__init__.py` & `sdss_hal-1.1.0/src/hal/helpers/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, cast
 
 from clu import Command, CommandStatus
 
+from hal import config
 from hal.exceptions import HALError
 
 
 if TYPE_CHECKING:
     from hal.actor import HALActor, HALCommandType
 
 
@@ -55,14 +56,21 @@
                 raise HALError(f"Command '{target} {cmd_str}' timed out.")
             else:
                 raise HALError(f"Command '{target} {cmd_str}' failed.")
 
         return cast(Command, cmd)
 
 
+def get_default_exposure_time(design_mode: str | None = None):
+    """Returns the default exposure time for the current design mode."""
+    if design_mode is not None and "bright" in design_mode:
+        return config["macros"]["expose"]["fallback"]["exptime"]["bright_design_mode"]
+    return config["macros"]["expose"]["fallback"]["exptime"]["default"]
+
+
 from .apogee import *
 from .boss import *
 from .cherno import *
 from .ffs import *
 from .jaeger import *
 from .lamps import *
 from .overhead import *
```

### Comparing `sdss_hal-1.0.3/src/hal/helpers/apogee.py` & `sdss_hal-1.1.0/src/hal/helpers/apogee.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/helpers/boss.py` & `sdss_hal-1.1.0/src/hal/helpers/boss.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/helpers/cherno.py` & `sdss_hal-1.1.0/src/hal/helpers/cherno.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/helpers/ffs.py` & `sdss_hal-1.1.0/src/hal/helpers/ffs.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/helpers/jaeger.py` & `sdss_hal-1.1.0/src/hal/helpers/jaeger.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     field_id: int | None = None
     cloned: bool = False
     preloaded: bool = False
     is_rm_field: bool = False
     new_field: bool = True
     observed: bool = False
     goto_complete: bool = False
+    design_mode: str | None = None
 
     def __post_init__(self):
         if self.design_id is None or self.design_id < 0:
             return
 
         if self.check_db():
             self.set_field_id()
@@ -79,22 +80,22 @@
                 self.warn(f"Failed getting field_id: {err}")
                 return
 
         # Determine if a field is RM/AQMES. Worst case, just assume it is not.
         self.is_rm_field = False
 
         try:
-            design_mode_label = (
+            self.design_mode = (
                 targetdb.Design.select(targetdb.Design.design_mode)
                 .where(targetdb.Design.design_id == self.design_id)
                 .scalar()
             )
-            if design_mode_label is None:
+            if self.design_mode is None:
                 self.warn(f"Cannot find design_mode_label for design {self.design_id}")
-            elif design_mode_label in ["dark_monit", "dark_rm"]:
+            elif self.design_mode in ["dark_monit", "dark_rm"]:
                 self.is_rm_field = True
         except Exception as err:
             self.warn(f"Failed determining RM/AQMES: {err}")
 
         return
 
 
@@ -118,23 +119,28 @@
         self.model["design_preloaded"].register_callback(self._design_preloaded)
 
     def warn(self, message: str):
         """Warns users."""
 
         self.actor.write("w", error=message)
 
-    async def load_from_queue(self, command: HALCommandType, preload: bool = False):
+    async def load_from_queue(
+        self,
+        command: HALCommandType,
+        preload: bool = False,
+        extra_epoch_delay: float = 0.0,
+    ):
         """(Pre-)Loads a design from the queue."""
 
         verb = "preload" if preload else "load"
 
         cmd = await self._send_command(
             command,
             "jaeger",
-            f"configuration {verb} --epoch-delay 600",
+            f"configuration {verb} --extra-epoch-delay {extra_epoch_delay}",
             raise_on_fail=False,
         )
 
         if cmd.status.did_fail:
             self.warn("Failed loading design from the queue.")
             return False
```

### Comparing `sdss_hal-1.0.3/src/hal/helpers/lamps.py` & `sdss_hal-1.1.0/src/hal/helpers/lamps.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/helpers/overhead.py` & `sdss_hal-1.1.0/src/hal/helpers/overhead.py`

 * *Files 8% similar despite different names*

```diff
@@ -130,17 +130,21 @@
         if not database.connected:
             warnings.warn(
                 "Failed connecting to DB. Overhead cannot be recorded.",
                 HALWarning,
             )
             return
 
-        current_macro_id = Overhead.select(peewee.fn.MAX(Overhead.macro_id)).scalar()
+        try:
+            macro_id_last = Overhead.select(peewee.fn.MAX(Overhead.macro_id)).scalar()
+        except Exception as err:
+            warnings.warn(f"Failed getting macro_id: {err}", HALWarning)
+            return
 
-        return (current_macro_id or 0) + 1
+        return (macro_id_last or 0) + 1
 
     def update_database(self):
         """Updates the database with the overhead."""
 
         command = self.macro.command
 
         if not database.connected:
```

### Comparing `sdss_hal-1.0.3/src/hal/helpers/scripts.py` & `sdss_hal-1.1.0/src/hal/helpers/scripts.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/helpers/tcc.py` & `sdss_hal-1.1.0/src/hal/helpers/tcc.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/macros/__init__.py` & `sdss_hal-1.1.0/src/hal/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/macros/apogee_dome_flat.py` & `sdss_hal-1.1.0/src/hal/macros/apogee_dome_flat.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,16 @@
             raise MacroError("The APOGEE gang connector is not at the cart.")
 
         return True
 
     async def ffs(self):
         """Check the FFS status and closes it."""
 
+        assert self.command.actor.helpers.ffs, "FFS helper not available."
+
         if self.command.actor.helpers.ffs.all_closed():
             self.command.debug("FFS already closed.")
             self.__ffs_initial_state = "closed"
             return
         elif self.command.actor.helpers.ffs.all_open():
             self.__ffs_initial_state = "open"
         else:
@@ -104,14 +106,16 @@
                 raise MacroError("Failed flashing lamps.")
 
         return
 
     async def cleanup(self):
         """Closes the shutter and does cleanup."""
 
+        assert self.command.actor.helpers.ffs, "FFS helper not available."
+
         apogee = self.command.actor.helpers.apogee
 
         try:
             self.command.actor.models["apogee"]["utrReadState"].remove_callback(
                 self._flash_lamps
             )
         except AssertionError:
```

### Comparing `sdss_hal-1.0.3/src/hal/macros/auto.py` & `sdss_hal-1.1.0/src/hal/macros/auto.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from __future__ import annotations
 
 import asyncio
 from contextlib import suppress
 
 from hal import config
 from hal.exceptions import MacroError
+from hal.helpers import get_default_exposure_time
 from hal.macros.macro import Macro
 
 
 class AutoModeMacro(Macro):
     """A macro that runs one iteration of the auto mode."""
 
     name = "auto"
@@ -139,16 +140,21 @@
             self.message("RMS not reched yet. Waiting for guider to converge.")
             try:
                 await self.helpers.cherno.wait_for_rms(min_rms, max_wait=180)
             except asyncio.TimeoutError:
                 raise MacroError("Timed out waiting for guider to converge.")
 
         # Calculate expose time and schedule preloading a design.
+        # The exposure time depends on the design mode.
+        design_mode: str | None = None
+        if self.helpers.jaeger.configuration:
+            design_mode = self.helpers.jaeger.configuration.design_mode
+        exptime = get_default_exposure_time(design_mode)
+
         count = self.config["count"]
-        exptime = config["macros"]["expose"]["fallback"]["exptime"]
         flushing = config["durations"]["boss"][self.actor.observatory]["flushing"]
         readout = config["durations"]["boss"][self.actor.observatory]["readout"]
         total_time = (exptime + flushing + readout) * count - readout
 
         wait_design_load = int(total_time - 180)
         self.message(f"Scheduling next design preload in {wait_design_load} s.", "d")
         await self._preload_design(wait_design_load)
```

### Comparing `sdss_hal-1.0.3/src/hal/macros/expose.py` & `sdss_hal-1.1.0/src/hal/macros/expose.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 __all__ = ["ExposeMacro"]
 
 
 @dataclass
 class ExposeParameters:
     """Expose macro parameters."""
 
-    boss_exptime: float | None = config["macros"]["expose"]["fallback"]["exptime"]
+    boss_exptime: float | None = config["macros"]["expose"]["fallback"]["exptime"]["default"]  # fmt: skip  # noqa
     apogee_exptime: float | None = None
     count_apogee: int | None = 1
     count_boss: int | None = 1
     pairs: bool = True
     dither: bool = True
     initial_apogee_dither: str = "A"
     readout_matching: bool = True
@@ -472,14 +472,15 @@
                 raise MacroError("Some lamps are on.")
         else:
             self.command.warning("Skipping lamps check for now.")
 
         # Concurrent tasks to run.
         tasks = []
         if self.command.actor.observatory == "APO":
+            assert self.helpers.ffs
             tasks.append(self.helpers.ffs.open(self.command))
 
         if do_apogee:
             initial_dither = self.config["initial_apogee_dither"]
             if initial_dither:
                 tasks.append(
                     self.helpers.apogee.set_dither_position(
```

### Comparing `sdss_hal-1.0.3/src/hal/macros/goto_field.py` & `sdss_hal-1.1.0/src/hal/macros/goto_field.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/src/hal/macros/macro.py` & `sdss_hal-1.1.0/src/hal/macros/macro.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import asyncio
 import enum
 import warnings
 from collections import defaultdict
 from contextlib import suppress
 
-from typing import TYPE_CHECKING, Any, Awaitable, ClassVar, Coroutine, Optional, Union
+from typing import TYPE_CHECKING, Any, ClassVar, Coroutine, Optional, Union
 
 from clu import Command, CommandStatus
 
 from hal import config
 from hal.exceptions import HALUserWarning, MacroError
 from hal.helpers.overhead import OverheadHelper
 
@@ -32,15 +32,15 @@
 
 StageType = Union[str, tuple[str, ...], list[str]]
 
 
 def record_overhead(macro: Macro):
     """Runs a macro stage and records its overhead."""
 
-    async def record_overhead_wrapper(stage_coro: Awaitable[None]):
+    async def record_overhead_wrapper(stage_coro: Coroutine[Any, Any, None]):
         overhead_helper = OverheadHelper(
             macro,
             stage_coro.__name__,
             macro_id=macro.macro_id,
         )
         async with overhead_helper:
             await stage_coro
```

### Comparing `sdss_hal-1.0.3/src/hal/macros/test_macro.py` & `sdss_hal-1.1.0/src/hal/macros/test_macro.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.0.3/PKG-INFO` & `sdss_hal-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-hal
-Version: 1.0.3
+Version: 1.1.0
 Summary: High-level observing tool for SDSS-V (replaces SOP)
 Home-page: https://github.com/sdss/hal
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<4.0
```

