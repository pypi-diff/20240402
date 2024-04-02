# Comparing `tmp/ika-control-0.4.0.tar.gz` & `tmp/ika-control-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ika-control-0.4.0.tar", last modified: Mon Oct  9 20:59:11 2023, max compression
+gzip compressed data, was "ika-control-0.5.0.tar", last modified: Tue Apr  2 17:39:11 2024, max compression
```

## Comparing `ika-control-0.4.0.tar` & `ika-control-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-10-09 20:59:11.768164 ika-control-0.4.0/
--rw-r--r--   0 a.ruddick   (502) staff       (20)    35149 2023-01-23 17:35:20.000000 ika-control-0.4.0/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2631 2023-10-09 20:59:11.768069 ika-control-0.4.0/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1389 2023-03-16 19:17:53.000000 ika-control-0.4.0/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-10-09 20:59:11.765688 ika-control-0.4.0/ika/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2232 2023-04-10 23:30:07.000000 ika-control-0.4.0/ika/__init__.py
--rwxr-xr-x   0 a.ruddick   (502) staff       (20)    24677 2023-10-09 20:58:57.000000 ika-control-0.4.0/ika/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)    11639 2023-10-09 20:58:57.000000 ika-control-0.4.0/ika/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     8757 2023-10-09 20:58:57.000000 ika-control-0.4.0/ika/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-10-09 20:59:11.766595 ika-control-0.4.0/ika_control.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2631 2023-10-09 20:59:11.000000 ika-control-0.4.0/ika_control.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      414 2023-10-09 20:59:11.000000 ika-control-0.4.0/ika_control.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-10-09 20:59:11.000000 ika-control-0.4.0/ika_control.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       41 2023-10-09 20:59:11.000000 ika-control-0.4.0/ika_control.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      136 2023-10-09 20:59:11.000000 ika-control-0.4.0/ika_control.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        4 2023-10-09 20:59:11.000000 ika-control-0.4.0/ika_control.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      216 2023-10-09 20:59:11.768388 ika-control-0.4.0/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1508 2023-10-09 20:58:57.000000 ika-control-0.4.0/setup.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-10-09 20:59:11.767486 ika-control-0.4.0/tests/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3433 2023-10-09 19:58:17.000000 ika-control-0.4.0/tests/test_hotplate_driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3829 2023-10-09 19:58:40.000000 ika-control-0.4.0/tests/test_shaker_driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3850 2023-10-09 19:58:49.000000 ika-control-0.4.0/tests/test_stir_driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3374 2023-10-09 20:58:57.000000 ika-control-0.4.0/tests/test_vacuum_driver.py
+drwxr-xr-x   0 j.badillo   (502) staff       (20)        0 2024-04-02 17:39:11.881748 ika-control-0.5.0/
+-rw-r--r--   0 j.badillo   (502) staff       (20)    35149 2024-01-10 17:51:18.000000 ika-control-0.5.0/LICENSE
+-rw-r--r--   0 j.badillo   (502) staff       (20)     2635 2024-04-02 17:39:11.881669 ika-control-0.5.0/PKG-INFO
+-rw-r--r--   0 j.badillo   (502) staff       (20)     1389 2024-01-10 17:51:18.000000 ika-control-0.5.0/README.md
+drwxr-xr-x   0 j.badillo   (502) staff       (20)        0 2024-04-02 17:39:11.879286 ika-control-0.5.0/ika/
+-rw-r--r--   0 j.badillo   (502) staff       (20)     2232 2024-01-10 17:51:18.000000 ika-control-0.5.0/ika/__init__.py
+-rwxr-xr-x   0 j.badillo   (502) staff       (20)    24650 2024-02-12 14:19:27.000000 ika-control-0.5.0/ika/driver.py
+-rw-r--r--   0 j.badillo   (502) staff       (20)    11639 2024-01-10 17:51:18.000000 ika-control-0.5.0/ika/mock.py
+-rw-r--r--   0 j.badillo   (502) staff       (20)     8757 2024-01-10 17:51:18.000000 ika-control-0.5.0/ika/util.py
+drwxr-xr-x   0 j.badillo   (502) staff       (20)        0 2024-04-02 17:39:11.881026 ika-control-0.5.0/ika_control.egg-info/
+-rw-r--r--   0 j.badillo   (502) staff       (20)     2635 2024-04-02 17:39:11.000000 ika-control-0.5.0/ika_control.egg-info/PKG-INFO
+-rw-r--r--   0 j.badillo   (502) staff       (20)      414 2024-04-02 17:39:11.000000 ika-control-0.5.0/ika_control.egg-info/SOURCES.txt
+-rw-r--r--   0 j.badillo   (502) staff       (20)        1 2024-04-02 17:39:11.000000 ika-control-0.5.0/ika_control.egg-info/dependency_links.txt
+-rw-r--r--   0 j.badillo   (502) staff       (20)       41 2024-04-02 17:39:11.000000 ika-control-0.5.0/ika_control.egg-info/entry_points.txt
+-rw-r--r--   0 j.badillo   (502) staff       (20)      140 2024-04-02 17:39:11.000000 ika-control-0.5.0/ika_control.egg-info/requires.txt
+-rw-r--r--   0 j.badillo   (502) staff       (20)        4 2024-04-02 17:39:11.000000 ika-control-0.5.0/ika_control.egg-info/top_level.txt
+-rw-r--r--   0 j.badillo   (502) staff       (20)      179 2024-04-02 17:39:11.881997 ika-control-0.5.0/setup.cfg
+-rw-r--r--   0 j.badillo   (502) staff       (20)     1512 2024-04-02 17:32:57.000000 ika-control-0.5.0/setup.py
+drwxr-xr-x   0 j.badillo   (502) staff       (20)        0 2024-04-02 17:39:11.880820 ika-control-0.5.0/tests/
+-rw-r--r--   0 j.badillo   (502) staff       (20)     3433 2024-01-10 17:51:18.000000 ika-control-0.5.0/tests/test_hotplate_driver.py
+-rw-r--r--   0 j.badillo   (502) staff       (20)     3829 2024-01-10 17:51:18.000000 ika-control-0.5.0/tests/test_shaker_driver.py
+-rw-r--r--   0 j.badillo   (502) staff       (20)     3850 2024-01-10 17:51:18.000000 ika-control-0.5.0/tests/test_stir_driver.py
+-rw-r--r--   0 j.badillo   (502) staff       (20)     3374 2024-01-10 17:51:18.000000 ika-control-0.5.0/tests/test_vacuum_driver.py
```

### Comparing `ika-control-0.4.0/LICENSE` & `ika-control-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ika-control-0.4.0/PKG-INFO` & `ika-control-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ika-control
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python driver for IKA instruments.
 Home-page: https://github.com/numat/ika/
 Author: Alex Ruddick
 Author-email: a.ruddick@numat-tech.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
@@ -21,17 +21,17 @@
 License-File: LICENSE
 Requires-Dist: pyserial
 Provides-Extra: test
 Requires-Dist: pytest<8,>=6; extra == "test"
 Requires-Dist: pytest-cov<5,>=4; extra == "test"
 Requires-Dist: pytest-asyncio==0.*; extra == "test"
 Requires-Dist: pytest-xdist==3.*; extra == "test"
-Requires-Dist: ruff==0.0.291; extra == "test"
-Requires-Dist: mypy==1.5.1; extra == "test"
-Requires-Dist: types-pyserial==3.5.0.10; extra == "test"
+Requires-Dist: ruff==0.3.5; extra == "test"
+Requires-Dist: mypy==1.9.0; extra == "test"
+Requires-Dist: types-pyserial==3.5.0.20240311; extra == "test"
 
 ika
 ===
 
 Python ≥3.8 driver and command-line tool for IKA products.
  - Eurostar 60/100 control overhead stirrers
  - MATRIX ORBITAL shaker
```

### Comparing `ika-control-0.4.0/README.md` & `ika-control-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ika-control-0.4.0/ika/__init__.py` & `ika-control-0.5.0/ika/__init__.py`

 * *Files identical despite different names*

### Comparing `ika-control-0.4.0/ika/driver.py` & `ika-control-0.5.0/ika/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,17 +482,17 @@
 
     async def get_pressure(self) -> float:
         """Get vacuum pressure, converting to mmHg."""
         raw_pressure = await self.query(self.READ_ACTUAL_PRESSURE)
         return round(float(raw_pressure) / 1.333, 2)
 
     async def get_pressure_setpoint(self) -> float:
-        """Get vacuum pressure setpoint, converting to mmHg."""
+        """Get vacuum pressure setpoint, in mmHg."""
         raw_sp = await self.query(self.READ_SET_PRESSURE)
-        return round(float(raw_sp) / 1.333, 2)
+        return round(float(raw_sp), 2)
 
     async def get_status(self) -> bool:
         """Get vacuum status and convert to running/not running bool.
 
         TODO: Figure out the actual status bit (bit 25?)
         """
         raw_status = await self.query(self.READ_VAC_STATUS)
@@ -533,15 +533,15 @@
         return response
 
     async def set(self, setpoint: float):
         """Set a vacuum pressure setpoint, converting from mmHg to mbar.
 
         Unlike other commands, the vacuum echoes back, so use query().
         """
-        setpoint_mbar = str(int(setpoint * 1.333))
+        setpoint_mbar = str(int(setpoint))
         await self.query(self.SET_PRESSURE + setpoint_mbar)
 
     async def set_mode(self, mode: VacuumProtocol.Mode):
         """Set the operating mode.
 
         Unlike other commands, the vacuum echoes back, so use query().
         """
```

### Comparing `ika-control-0.4.0/ika/mock.py` & `ika-control-0.5.0/ika/mock.py`

 * *Files identical despite different names*

### Comparing `ika-control-0.4.0/ika/util.py` & `ika-control-0.5.0/ika/util.py`

 * *Files identical despite different names*

### Comparing `ika-control-0.4.0/ika_control.egg-info/PKG-INFO` & `ika-control-0.5.0/ika_control.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ika-control
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python driver for IKA instruments.
 Home-page: https://github.com/numat/ika/
 Author: Alex Ruddick
 Author-email: a.ruddick@numat-tech.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
@@ -21,17 +21,17 @@
 License-File: LICENSE
 Requires-Dist: pyserial
 Provides-Extra: test
 Requires-Dist: pytest<8,>=6; extra == "test"
 Requires-Dist: pytest-cov<5,>=4; extra == "test"
 Requires-Dist: pytest-asyncio==0.*; extra == "test"
 Requires-Dist: pytest-xdist==3.*; extra == "test"
-Requires-Dist: ruff==0.0.291; extra == "test"
-Requires-Dist: mypy==1.5.1; extra == "test"
-Requires-Dist: types-pyserial==3.5.0.10; extra == "test"
+Requires-Dist: ruff==0.3.5; extra == "test"
+Requires-Dist: mypy==1.9.0; extra == "test"
+Requires-Dist: types-pyserial==3.5.0.20240311; extra == "test"
 
 ika
 ===
 
 Python ≥3.8 driver and command-line tool for IKA products.
  - Eurostar 60/100 control overhead stirrers
  - MATRIX ORBITAL shaker
```

### Comparing `ika-control-0.4.0/setup.py` & `ika-control-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 from setuptools import setup
 
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="ika-control",
-    version="0.4.0",
+    version="0.5.0",
     description="Python driver for IKA instruments.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/numat/ika/",
     author="Alex Ruddick",
     author_email="a.ruddick@numat-tech.com",
     packages=['ika'],
     install_requires=['pyserial'],
     extras_require={
         'test': [
             'pytest>=6,<8',
             'pytest-cov>=4,<5',
             'pytest-asyncio==0.*',
             'pytest-xdist==3.*',
-            'ruff==0.0.291',
-            'mypy==1.5.1',
-            'types-pyserial==3.5.0.10'
+            'ruff==0.3.5',
+            'mypy==1.9.0',
+            'types-pyserial==3.5.0.20240311'
         ],
     },
     entry_points={
         'console_scripts': [('ika = ika:command_line')]
     },
     license='GPLv3',
     classifiers=[
```

### Comparing `ika-control-0.4.0/tests/test_hotplate_driver.py` & `ika-control-0.5.0/tests/test_hotplate_driver.py`

 * *Files identical despite different names*

### Comparing `ika-control-0.4.0/tests/test_shaker_driver.py` & `ika-control-0.5.0/tests/test_shaker_driver.py`

 * *Files identical despite different names*

### Comparing `ika-control-0.4.0/tests/test_stir_driver.py` & `ika-control-0.5.0/tests/test_stir_driver.py`

 * *Files identical despite different names*

### Comparing `ika-control-0.4.0/tests/test_vacuum_driver.py` & `ika-control-0.5.0/tests/test_vacuum_driver.py`

 * *Files identical despite different names*

