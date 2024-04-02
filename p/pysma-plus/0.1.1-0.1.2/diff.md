# Comparing `tmp/pysma-plus-0.1.1.tar.gz` & `tmp/pysma-plus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysma-plus-0.1.1.tar", last modified: Mon Apr  1 14:09:32 2024, max compression
+gzip compressed data, was "pysma-plus-0.1.2.tar", last modified: Tue Apr  2 12:36:26 2024, max compression
```

## Comparing `pysma-plus-0.1.1.tar` & `pysma-plus-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-01 14:09:32.810427 pysma-plus-0.1.1/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1075 2024-03-27 10:30:58.000000 pysma-plus-0.1.1/LICENSE
--rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-03-30 19:14:11.000000 pysma-plus-0.1.1/MANIFEST.in
--rw-r--r--   0 sven      (1001) sven      (1001)     2669 2024-04-01 14:09:32.810427 pysma-plus-0.1.1/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)      642 2024-03-30 18:43:59.000000 pysma-plus-0.1.1/README.md
--rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-04-01 14:09:25.000000 pysma-plus-0.1.1/pyproject.toml
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-01 14:09:32.810427 pysma-plus-0.1.1/pysma_plus.egg-info/
--rw-r--r--   0 sven      (1001) sven      (1001)     2669 2024-04-01 14:09:32.000000 pysma-plus-0.1.1/pysma_plus.egg-info/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)      597 2024-04-01 14:09:32.000000 pysma-plus-0.1.1/pysma_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-04-01 14:09:32.000000 pysma-plus-0.1.1/pysma_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-04-01 14:09:32.000000 pysma-plus-0.1.1/pysma_plus.egg-info/requires.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-04-01 14:09:32.000000 pysma-plus-0.1.1/pysma_plus.egg-info/top_level.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-03-30 19:16:34.000000 pysma-plus-0.1.1/pysma_plus.egg-info/zip-safe
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-01 14:09:32.810427 pysma-plus-0.1.1/pysmaplus/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1920 2024-03-29 07:19:41.000000 pysma-plus-0.1.1/pysmaplus/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6668 2024-03-31 12:59:54.000000 pysma-plus-0.1.1/pysmaplus/const.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21131 2024-03-28 08:57:32.000000 pysma-plus-0.1.1/pysmaplus/definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      507 2024-03-27 12:21:42.000000 pysma-plus-0.1.1/pysmaplus/device.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-03-27 10:31:31.000000 pysma-plus-0.1.1/pysmaplus/exceptions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-03-27 10:31:31.000000 pysma-plus-0.1.1/pysmaplus/helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6237 2024-03-31 12:44:16.000000 pysma-plus-0.1.1/pysmaplus/sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    13827 2024-03-31 17:59:40.000000 pysma-plus-0.1.1/pysmaplus/smaennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     9378 2024-04-01 14:05:43.000000 pysma-plus-0.1.1/pysmaplus/smaspeedwireem.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    16136 2024-03-27 12:04:04.000000 pysma-plus-0.1.1/pysmaplus/smawebconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-04-01 14:09:32.811427 pysma-plus-0.1.1/setup.cfg
--rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-04-01 14:09:25.000000 pysma-plus-0.1.1/setup.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-01 14:09:32.810427 pysma-plus-0.1.1/tests/
--rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-03-27 10:30:58.000000 pysma-plus-0.1.1/tests/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      883 2024-03-27 10:30:58.000000 pysma-plus-0.1.1/tests/test_definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-03-27 10:30:58.000000 pysma-plus-0.1.1/tests/test_helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17280 2024-03-27 10:30:58.000000 pysma-plus-0.1.1/tests/test_init.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     4785 2024-03-27 10:30:58.000000 pysma-plus-0.1.1/tests/test_sensor.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-02 12:36:26.305646 pysma-plus-0.1.2/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1075 2024-03-27 10:30:58.000000 pysma-plus-0.1.2/LICENSE
+-rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-03-30 19:14:11.000000 pysma-plus-0.1.2/MANIFEST.in
+-rw-r--r--   0 sven      (1001) sven      (1001)     2669 2024-04-02 12:36:26.305646 pysma-plus-0.1.2/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)      642 2024-03-30 18:43:59.000000 pysma-plus-0.1.2/README.md
+-rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-04-02 12:36:16.000000 pysma-plus-0.1.2/pyproject.toml
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-02 12:36:26.305646 pysma-plus-0.1.2/pysma_plus.egg-info/
+-rw-r--r--   0 sven      (1001) sven      (1001)     2669 2024-04-02 12:36:26.000000 pysma-plus-0.1.2/pysma_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)      597 2024-04-02 12:36:26.000000 pysma-plus-0.1.2/pysma_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-04-02 12:36:26.000000 pysma-plus-0.1.2/pysma_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-04-02 12:36:26.000000 pysma-plus-0.1.2/pysma_plus.egg-info/requires.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-04-02 12:36:26.000000 pysma-plus-0.1.2/pysma_plus.egg-info/top_level.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-03-30 19:16:34.000000 pysma-plus-0.1.2/pysma_plus.egg-info/zip-safe
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-02 12:36:26.305646 pysma-plus-0.1.2/pysmaplus/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1920 2024-03-29 07:19:41.000000 pysma-plus-0.1.2/pysmaplus/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6668 2024-03-31 12:59:54.000000 pysma-plus-0.1.2/pysmaplus/const.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21131 2024-03-28 08:57:32.000000 pysma-plus-0.1.2/pysmaplus/definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      507 2024-03-27 12:21:42.000000 pysma-plus-0.1.2/pysmaplus/device.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-03-27 10:31:31.000000 pysma-plus-0.1.2/pysmaplus/exceptions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-03-27 10:31:31.000000 pysma-plus-0.1.2/pysmaplus/helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6237 2024-03-31 12:44:16.000000 pysma-plus-0.1.2/pysmaplus/sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    13923 2024-04-02 12:33:41.000000 pysma-plus-0.1.2/pysmaplus/smaennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     9378 2024-04-01 14:05:43.000000 pysma-plus-0.1.2/pysmaplus/smaspeedwireem.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    16136 2024-03-27 12:04:04.000000 pysma-plus-0.1.2/pysmaplus/smawebconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-04-02 12:36:26.305646 pysma-plus-0.1.2/setup.cfg
+-rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-04-02 12:36:16.000000 pysma-plus-0.1.2/setup.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-02 12:36:26.305646 pysma-plus-0.1.2/tests/
+-rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-03-27 10:30:58.000000 pysma-plus-0.1.2/tests/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      883 2024-03-27 10:30:58.000000 pysma-plus-0.1.2/tests/test_definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-03-27 10:30:58.000000 pysma-plus-0.1.2/tests/test_helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17280 2024-03-27 10:30:58.000000 pysma-plus-0.1.2/tests/test_init.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     4785 2024-03-27 10:30:58.000000 pysma-plus-0.1.2/tests/test_sensor.py
```

### Comparing `pysma-plus-0.1.1/LICENSE` & `pysma-plus-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.1/PKG-INFO` & `pysma-plus-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.1
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.2
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 kellerza
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysma-plus-0.1.1/README.md` & `pysma-plus-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.1/pyproject.toml` & `pysma-plus-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysma-plus"
-version = "0.1.1"
+version = "0.1.2"
 description = "Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices"
 readme = "README.md"
 authors = [{ name = "Sven Bursch-Osewold", email = "sb_pysma@bursch.com" },{ name = "Johann Kellerman" , email ="kellerza@gmail.com"} ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pysma-plus-0.1.1/pysma_plus.egg-info/PKG-INFO` & `pysma-plus-0.1.2/pysma_plus.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.1
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.2
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 kellerza
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysma-plus-0.1.1/pysma_plus.egg-info/SOURCES.txt` & `pysma-plus-0.1.2/pysma_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.1/pysmaplus/__init__.py` & `pysma-plus-0.1.2/pysmaplus/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.1/pysmaplus/const.py` & `pysma-plus-0.1.2/pysmaplus/const.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.1/pysmaplus/definitions.py` & `pysma-plus-0.1.2/pysmaplus/definitions.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.1/pysmaplus/helpers.py` & `pysma-plus-0.1.2/pysmaplus/helpers.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.1/pysmaplus/sensor.py` & `pysma-plus-0.1.2/pysmaplus/sensor.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.1/pysmaplus/smaennexos.py` & `pysma-plus-0.1.2/pysmaplus/smaennexos.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,14 +261,16 @@
         """Get the sensors that are present on the device.
 
         Returns:
             Sensors: Sensors object containing Sensor objects
         """
         device_sensors = Sensors()
         ret = await self._get_livedata()
+        _LOGGER.debug("Found Sensors: %s", ret)
+
         for s in ennexosSensors:
             if s.name:
                 device_sensors.add(copy.copy(s))
         return device_sensors
 
 
     async def close_session(self) -> None:
@@ -330,14 +332,15 @@
             dict: dict containing serial, name, type, manufacturer and sw_version
         """
         url = self._url + '/api/v1/plants/Plant:1/devices/IGULD:SELF'
         requestdata = { 
              'headers': self._authorization_header
         }
         dev = await self._jsonrequest(url,requestdata, hdrs.METH_GET)
+        _LOGGER.debug("Found Device: %s", dev)
         device_info = {
             "serial": dev["serial"],
             "name": dev["product"],
             "type": dev["name"],
             "manufacturer": dev["vendor"],
             "sw_version": dev["firmwareVersion"],
         }
```

### Comparing `pysma-plus-0.1.1/pysmaplus/smaspeedwireem.py` & `pysma-plus-0.1.2/pysmaplus/smaspeedwireem.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.1/pysmaplus/smawebconnect.py` & `pysma-plus-0.1.2/pysmaplus/smawebconnect.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.1/setup.py` & `pysma-plus-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """pysma library setup."""
 from pathlib import Path
 
 from setuptools import setup
 
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 URL = "https://github.com/littleyoda/pysma"
 
 setup(
     name="pysma-plus",
     version=VERSION,
     description="Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices",
     long_description=Path("README.md").read_text(),
```

### Comparing `pysma-plus-0.1.1/tests/__init__.py` & `pysma-plus-0.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.1/tests/test_definitions.py` & `pysma-plus-0.1.2/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.1/tests/test_init.py` & `pysma-plus-0.1.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.1/tests/test_sensor.py` & `pysma-plus-0.1.2/tests/test_sensor.py`

 * *Files identical despite different names*

