# Comparing `tmp/alicat-0.6.1.tar.gz` & `tmp/alicat-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicat-0.6.1.tar", last modified: Wed Nov 15 17:41:43 2023, max compression
+gzip compressed data, was "alicat-0.6.2.tar", last modified: Tue Apr  2 15:02:48 2024, max compression
```

## Comparing `alicat-0.6.1.tar` & `alicat-0.6.2.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-11-15 17:41:43.505739 alicat-0.6.1/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       61 2023-04-25 18:35:30.000000 alicat-0.6.1/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18027 2023-10-17 05:09:32.000000 alicat-0.6.1/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     6194 2023-11-15 17:41:43.505668 alicat-0.6.1/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     4894 2023-04-12 17:39:23.000000 alicat-0.6.1/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-11-15 17:41:43.504171 alicat-0.6.1/alicat/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     4570 2023-05-22 22:05:57.000000 alicat-0.6.1/alicat/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18962 2023-11-15 17:39:08.000000 alicat-0.6.1/alicat/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2882 2023-04-27 18:39:33.000000 alicat-0.6.1/alicat/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:10:43.000000 alicat-0.6.1/alicat/py.typed
--rw-r--r--   0 a.ruddick   (502) staff       (20)     7988 2023-11-15 17:41:00.000000 alicat-0.6.1/alicat/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-11-15 17:41:43.504947 alicat-0.6.1/alicat.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     6194 2023-11-15 17:41:43.000000 alicat-0.6.1/alicat.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      332 2023-11-15 17:41:43.000000 alicat-0.6.1/alicat.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-11-15 17:41:43.000000 alicat-0.6.1/alicat.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       47 2023-11-15 17:41:43.000000 alicat-0.6.1/alicat.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      124 2023-11-15 17:41:43.000000 alicat-0.6.1/alicat.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        7 2023-11-15 17:41:43.000000 alicat-0.6.1/alicat.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      201 2023-11-15 17:41:43.505957 alicat-0.6.1/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1659 2023-11-15 17:41:03.000000 alicat-0.6.1/setup.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-11-15 17:41:43.505062 alicat-0.6.1/tests/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2142 2023-07-11 15:59:52.000000 alicat-0.6.1/tests/test_driver.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-02 15:02:48.292003 alicat-0.6.2/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    18027 2024-02-04 23:54:06.000000 alicat-0.6.2/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5857 2024-04-02 15:02:48.292003 alicat-0.6.2/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4894 2024-02-04 23:54:06.000000 alicat-0.6.2/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-02 15:02:48.292003 alicat-0.6.2/alicat/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4570 2024-02-04 23:54:06.000000 alicat-0.6.2/alicat/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20850 2024-04-02 15:00:31.000000 alicat-0.6.2/alicat/driver.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2861 2024-02-09 17:09:56.000000 alicat-0.6.2/alicat/mock.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2024-02-04 23:54:06.000000 alicat-0.6.2/alicat/py.typed
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8040 2024-04-02 14:54:48.000000 alicat-0.6.2/alicat/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-02 15:02:48.292003 alicat-0.6.2/alicat.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5857 2024-04-02 15:02:48.000000 alicat-0.6.2/alicat.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      300 2024-04-02 15:02:48.000000 alicat-0.6.2/alicat.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-04-02 15:02:48.000000 alicat-0.6.2/alicat.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       48 2024-04-02 15:02:48.000000 alicat-0.6.2/alicat.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      127 2024-04-02 15:02:48.000000 alicat-0.6.2/alicat.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2024-04-02 15:02:48.000000 alicat-0.6.2/alicat.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      201 2024-04-02 15:02:48.292003 alicat-0.6.2/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1660 2024-04-02 15:01:57.000000 alicat-0.6.2/setup.py
```

### Comparing `alicat-0.6.1/LICENSE` & `alicat-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alicat-0.6.1/PKG-INFO` & `alicat-0.6.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 Metadata-Version: 2.1
 Name: alicat
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python driver for Alicat mass flow controllers.
 Home-page: https://github.com/numat/alicat/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 Maintainer: Alex Ruddick
-Maintainer-email: alex@numat-tech.com
+Maintainer-email: alex@ruddick.tech
 License: GPLv2
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyserial
 Provides-Extra: test
-Requires-Dist: pytest<8,>=6; extra == "test"
-Requires-Dist: pytest-cov<5,>=4; extra == "test"
-Requires-Dist: pytest-asyncio==0.*; extra == "test"
-Requires-Dist: pytest-xdist==3.*; extra == "test"
-Requires-Dist: ruff==0.1.5; extra == "test"
-Requires-Dist: mypy==1.7.0; extra == "test"
-Requires-Dist: types-pyserial; extra == "test"
+License-File: LICENSE
 
 alicat
 ======
 
 TCP/Serial driver and command line tool for
 [Alicat mass flow controllers](http://www.alicat.com/products/mass-flow-meters-and-controllers/mass-flow-controllers/).
 
@@ -176,7 +169,9 @@
 `0.5.0`
 - Support only `asyncio`.  The last version with synchronous code was `0.4.1`.
 - Rename `address`/`-a` to `unit`/`-u` to match Alicat's documentation
 - Rename `-u` to `-ul` (for `--unlock`)
 
 `0.4.1`
 Remove TCP support.  Use `pip install alicat==0.3.1` if needed
+
+
```

### Comparing `alicat-0.6.1/README.md` & `alicat-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `alicat-0.6.1/alicat/__init__.py` & `alicat-0.6.2/alicat/__init__.py`

 * *Files identical despite different names*

### Comparing `alicat-0.6.1/alicat/driver.py` & `alicat-0.6.2/alicat/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -373,14 +373,59 @@
                 purchase. Likely in psia.
         """
         if self.control_point in ['mass flow', 'vol flow']:
             await self._set_setpoint(0)
             await self._set_control_point('abs pressure')
         await self._set_setpoint(pressure)
 
+    async def get_totalizer_batch(self, batch: int = 1) -> str:
+        """Get the totalizer batch volume.
+
+        Args:
+            batch: Which of the two totalizer batches to query.
+                Default is 1; some devices have 2
+
+        Returns:
+            line: Current value of totalizer batch
+        """
+        command = f'{self.unit}$$TB {batch}'
+        line = await self._write_and_read(command)
+
+        if line == '?':
+            raise OSError("Unable to read totalizer batch volume.")
+        else:
+            values = line.split(" ")  # type: ignore[union-attr]
+            return f'{values[2]} {values[4]}' # returns 'batch vol' 'units'
+
+    async def set_totalizer_batch(self, batch_volume: float, batch: int = 1, units: str = 'default') -> None:
+        """Set the totalizer batch volume.
+
+        Args:
+            batch: Which of the two totalizer batches to set.
+                Default is 1; some devices have 2
+            batch_volume: Target batch volume, in same units as units
+                on device
+            units: Units of the volume being provided. Default
+                is 0, so device returns default engineering units.
+        """
+        engineering_units_table = {"default":0, "SμL":2, "SmL":3, "SL":4, \
+                    "Scm3":6, "Sm3":7, "Sin3":8, "Sft3":9, "kSft3":10, "NμL":32, \
+                    "NmL":33, "NL":34, "Ncm3":36, "Nm3":37}
+
+        if units in engineering_units_table:
+            units_no = engineering_units_table[units]
+        else:
+            raise ValueError("Units not in unit list. Please consult Appendix B-3 of the Alicat Serial Primer.")
+
+        command = f'{self.unit}$$TB {batch} {batch_volume} {units_no}'
+        line = await self._write_and_read(command)
+
+        if line == '?':
+            raise OSError("Unable to set totalizer batch volume. Check if volume is out of range for device.")
+
     async def hold(self) -> None:
         """Override command to issue a valve hold.
 
         For a single valve controller, hold the valve at the present value.
         For a dual valve flow controller, hold the valve at the present value.
         For a dual valve pressure controller, close both valves.
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alicat-0.6.1/alicat/mock.py` & `alicat-0.6.2/alicat/mock.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,28 +34,28 @@
             'unit': unit,
             'volumetric_flow': 0.0,
         }
         self.unit: str = unit
         self.button_lock: bool = False
         self.keys = ['pressure', 'temperature', 'volumetric_flow', 'mass_flow',
                      'setpoint', 'gas']
-        self.firmware: str = '6v21.0-R22 Nov 30 2016,16:04:20'
+        self.firmware = '6v21.0-R22 Nov 30 2016,16:04:20'
 
     async def get(self) -> Dict[str, Union[str, float]]:
         """Return the full state."""
         sleep(random() * 0.25)
         return self.state
 
     async def _set_setpoint(self, setpoint: float) -> None:
         """Set the target setpoint."""
         self.state['setpoint'] = setpoint
 
-    async def _set_control_point(self, control_point: str) -> None:
+    async def _set_control_point(self, point: str) -> None:
         """Set the control point, either 'flow' or 'pressure'."""
-        self.control_point = control_point
+        self.control_point = point
 
     async def _get_control_point(self) -> str:
         """Return the control point, either 'flow' or 'pressure'."""
         return self.control_point
 
     async def set_flow_rate(self, flowrate: float) -> None:
         """Set the flowrate setpoint."""
```

### Comparing `alicat-0.6.1/alicat/util.py` & `alicat-0.6.2/alicat/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,15 +177,16 @@
                              f'{self.timeouts} times.')
                 await self.close()
             return None
 
     async def close(self) -> None:
         """Close the TCP connection."""
         if self.open:
-            await self.connection['writer'].close()
+            self.connection['writer'].close()
+            await self.connection['writer'].wait_closed()
         self.open = False
 
 
 class SerialClient(Client):
     """Client using a directly-connected RS232 serial device."""
 
     def __init__(self, address: str, baudrate: int=19200, timeout: float=.15,
```

### Comparing `alicat-0.6.1/alicat.egg-info/PKG-INFO` & `alicat-0.6.2/alicat.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 Metadata-Version: 2.1
 Name: alicat
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python driver for Alicat mass flow controllers.
 Home-page: https://github.com/numat/alicat/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 Maintainer: Alex Ruddick
-Maintainer-email: alex@numat-tech.com
+Maintainer-email: alex@ruddick.tech
 License: GPLv2
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyserial
 Provides-Extra: test
-Requires-Dist: pytest<8,>=6; extra == "test"
-Requires-Dist: pytest-cov<5,>=4; extra == "test"
-Requires-Dist: pytest-asyncio==0.*; extra == "test"
-Requires-Dist: pytest-xdist==3.*; extra == "test"
-Requires-Dist: ruff==0.1.5; extra == "test"
-Requires-Dist: mypy==1.7.0; extra == "test"
-Requires-Dist: types-pyserial; extra == "test"
+License-File: LICENSE
 
 alicat
 ======
 
 TCP/Serial driver and command line tool for
 [Alicat mass flow controllers](http://www.alicat.com/products/mass-flow-meters-and-controllers/mass-flow-controllers/).
 
@@ -176,7 +169,9 @@
 `0.5.0`
 - Support only `asyncio`.  The last version with synchronous code was `0.4.1`.
 - Rename `address`/`-a` to `unit`/`-u` to match Alicat's documentation
 - Rename `-u` to `-ul` (for `--unlock`)
 
 `0.4.1`
 Remove TCP support.  Use `pip install alicat==0.3.1` if needed
+
+
```

### Comparing `alicat-0.6.1/setup.py` & `alicat-0.6.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 from setuptools import setup
 
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="alicat",
-    version="0.6.1",
+    version="0.6.2",
     description="Python driver for Alicat mass flow controllers.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/numat/alicat/",
     author="Patrick Fuller",
     author_email="pat@numat-tech.com",
     maintainer="Alex Ruddick",
-    maintainer_email="alex@numat-tech.com",
+    maintainer_email="alex@ruddick.tech",
     packages=["alicat"],
     package_data={"alicat": ["py.typed"]},
     install_requires=["pyserial"],
     extras_require={
             'test': [
-                'pytest>=6,<8',
-                'pytest-cov>=4,<5',
-                'pytest-asyncio==0.*',
+                'pytest>=8,<9',
+                'pytest-cov>=5,<6',
+                'pytest-asyncio>=0.23.5',
                 'pytest-xdist==3.*',
-                'ruff==0.1.5',
-                'mypy==1.7.0',
+                'ruff==0.3.5',
+                'mypy==1.9.0',
                 'types-pyserial',
             ],
         },
     entry_points={
         "console_scripts": [("alicat = alicat:command_line")]
     },
     license="GPLv2",
```

