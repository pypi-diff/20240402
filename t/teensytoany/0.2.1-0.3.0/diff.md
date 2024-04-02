# Comparing `tmp/teensytoany-0.2.1.tar.gz` & `tmp/teensytoany-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teensytoany-0.2.1.tar", last modified: Fri Jan 12 01:17:23 2024, max compression
+gzip compressed data, was "teensytoany-0.3.0.tar", last modified: Tue Apr  2 15:02:51 2024, max compression
```

## Comparing `teensytoany-0.2.1.tar` & `teensytoany-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 01:17:23.723657 teensytoany-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-12 01:17:16.000000 teensytoany-0.2.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-01-12 01:17:16.000000 teensytoany-0.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-01-12 01:17:16.000000 teensytoany-0.2.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-01-12 01:17:16.000000 teensytoany-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-12 01:17:16.000000 teensytoany-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-01-12 01:17:23.723657 teensytoany-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-12 01:17:16.000000 teensytoany-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 01:17:23.719657 teensytoany-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-01-12 01:17:16.000000 teensytoany-0.2.1/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     4963 2024-01-12 01:17:16.000000 teensytoany-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-12 01:17:16.000000 teensytoany-0.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-12 01:17:16.000000 teensytoany-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-01-12 01:17:16.000000 teensytoany-0.2.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-01-12 01:17:16.000000 teensytoany-0.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-12 01:17:16.000000 teensytoany-0.2.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-12 01:17:16.000000 teensytoany-0.2.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-12 01:17:23.723657 teensytoany-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-01-12 01:17:16.000000 teensytoany-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 01:17:23.723657 teensytoany-0.2.1/teensytoany/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-12 01:17:16.000000 teensytoany-0.2.1/teensytoany/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-12 01:17:23.723657 teensytoany-0.2.1/teensytoany/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-01-12 01:17:16.000000 teensytoany-0.2.1/teensytoany/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-01-12 01:17:16.000000 teensytoany-0.2.1/teensytoany/teensypower.py
--rw-r--r--   0 runner    (1001) docker     (127)    23114 2024-01-12 01:17:16.000000 teensytoany-0.2.1/teensytoany/teensytoany.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 01:17:23.723657 teensytoany-0.2.1/teensytoany.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-01-12 01:17:23.000000 teensytoany-0.2.1/teensytoany.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-01-12 01:17:23.000000 teensytoany-0.2.1/teensytoany.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 01:17:23.000000 teensytoany-0.2.1/teensytoany.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 01:17:23.000000 teensytoany-0.2.1/teensytoany.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-12 01:17:23.000000 teensytoany-0.2.1/teensytoany.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-12 01:17:23.000000 teensytoany-0.2.1/teensytoany.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:02:51.372447 teensytoany-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-02 15:02:47.000000 teensytoany-0.3.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-02 15:02:47.000000 teensytoany-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-02 15:02:47.000000 teensytoany-0.3.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-02 15:02:47.000000 teensytoany-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-02 15:02:47.000000 teensytoany-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-02 15:02:51.372447 teensytoany-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-02 15:02:47.000000 teensytoany-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:02:51.368447 teensytoany-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4964 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-02 15:02:51.372447 teensytoany-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-02 15:02:47.000000 teensytoany-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:02:51.372447 teensytoany-0.3.0/teensytoany/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-02 15:02:47.000000 teensytoany-0.3.0/teensytoany/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 15:02:51.372447 teensytoany-0.3.0/teensytoany/_static_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-02 15:02:47.000000 teensytoany-0.3.0/teensytoany/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-02 15:02:47.000000 teensytoany-0.3.0/teensytoany/teensypower.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23337 2024-04-02 15:02:47.000000 teensytoany-0.3.0/teensytoany/teensytoany.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:02:51.372447 teensytoany-0.3.0/teensytoany.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-02 15:02:51.000000 teensytoany-0.3.0/teensytoany.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 15:02:51.000000 teensytoany-0.3.0/teensytoany.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:02:51.000000 teensytoany-0.3.0/teensytoany.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:02:51.000000 teensytoany-0.3.0/teensytoany.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 15:02:51.000000 teensytoany-0.3.0/teensytoany.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 15:02:51.000000 teensytoany-0.3.0/teensytoany.egg-info/top_level.txt
```

### Comparing `teensytoany-0.2.1/CONTRIBUTING.md` & `teensytoany-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `teensytoany-0.2.1/HISTORY.md` & `teensytoany-0.3.0/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # History
 
+## 0.3.0 (2024-04-02)
+
+* Add a `timeout` property to the functions that deal with updating the firmware.
+
 ## 0.2.0 (2023-11-07)
 
 * Add a `timeout` property to simplify modifying the command timeout.
 
 ## 0.1.0 (2023-09-29)
 
 * Provide access the new `mcu` command that reveals the microcontroller used at
```

### Comparing `teensytoany-0.2.1/LICENSE` & `teensytoany-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `teensytoany-0.2.1/PKG-INFO` & `teensytoany-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: teensytoany
-Version: 0.2.1
+Version: 0.3.0
 Summary: A pythonic way to access the teensytoany board
 Home-page: https://github.com/ramonaoptics/python-teensytoany
 Author: Ramona Optics Inc.
 Author-email: info@ramonaoptics.com
 License: BSD license
 Keywords: teensytoany
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial
 Requires-Dist: packaging
 
 # Python TeensyToAny
 
@@ -49,14 +48,18 @@
 [hmaarrfk/cookiecutter-pypackage](https://github.com/hmaarrfk/cookiecutter-pypackage)
 project template.
 
 
 
 # History
 
+## 0.3.0 (2024-04-02)
+
+* Add a `timeout` property to the functions that deal with updating the firmware.
+
 ## 0.2.0 (2023-11-07)
 
 * Add a `timeout` property to simplify modifying the command timeout.
 
 ## 0.1.0 (2023-09-29)
 
 * Provide access the new `mcu` command that reveals the microcontroller used at
```

### Comparing `teensytoany-0.2.1/README.md` & `teensytoany-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `teensytoany-0.2.1/docs/Makefile` & `teensytoany-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `teensytoany-0.2.1/docs/conf.py` & `teensytoany-0.3.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
+
 sys.path.insert(0, os.path.abspath('..'))
 
 import python_teensytoany
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
```

### Comparing `teensytoany-0.2.1/docs/installation.rst` & `teensytoany-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `teensytoany-0.2.1/docs/make.bat` & `teensytoany-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `teensytoany-0.2.1/setup.py` & `teensytoany-0.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 
 # Loads _version.py module without importing the whole package.
 def get_version_and_cmdclass(pkg_path):
     import os
     from importlib.util import module_from_spec, spec_from_file_location
     spec = spec_from_file_location(
@@ -31,21 +31,20 @@
     author_email='info@ramonaoptics.com',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.9',
     description="A pythonic way to access the teensytoany board",
     install_requires=requirements,
     license="BSD license",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='teensytoany',
```

### Comparing `teensytoany-0.2.1/teensytoany/_version.py` & `teensytoany-0.3.0/teensytoany/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file is part of 'miniver': https://github.com/jbweston/miniver
 #
-from collections import namedtuple
 import os
+from collections import namedtuple
 
 Version = namedtuple("Version", ("release", "dev", "labels"))
 
 # No public API
 __all__ = []
 
 package_root = os.path.dirname(os.path.realpath(__file__))
@@ -53,14 +53,15 @@
         version_parts.append(".".join(labels))
 
     return "".join(version_parts)
 
 
 def get_version_from_git():
     import subprocess
+
     # The '--long' flag gets us the 'dev' version and
     # The '--dirty' flag helps identify if files have been modified
     # git hash, '--always' returns the git hash even if there are no tags.
     for opts in [[]]:
         try:
             p = subprocess.Popen(
                 ["git", "describe", "--long", "--always", "--dirty", "--tags"] + opts,
```

### Comparing `teensytoany-0.2.1/teensytoany/teensypower.py` & `teensytoany-0.3.0/teensytoany/teensypower.py`

 * *Files identical despite different names*

### Comparing `teensytoany-0.2.1/teensytoany/teensytoany.py` & `teensytoany-0.3.0/teensytoany/teensytoany.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import os
+import subprocess
+import tempfile
+from time import sleep
 from typing import Sequence
 
-from serial import Serial, LF
-from serial.tools.list_ports import comports
-import os
 from packaging.version import Version
-from time import sleep
+from serial import LF, Serial
+from serial.tools.list_ports import comports
 
 __all__ = ['TeensyToAny', 'known_devices', 'known_serial_numbers']
 
 known_devices = [
     # Example device structure
     # These include useful information about the hardware that is created and
     # burned in with the serial numbers.
@@ -128,21 +130,21 @@
         """
         pairs = TeensyToAny._device_serial_number_pairs(
             serial_numbers=serial_numbers, device_name=device_name)
         _, serial_numbers = zip(*pairs)
         return serial_numbers
 
     @staticmethod
-    def _get_latest_available_firmware():
-        import requests
+    def _get_latest_available_firmware(*, timeout=2):
+        import requests  # pylint: disable=import-outside-toplevel
 
         repo_url = "https://api.github.com/repos/ramonaoptics/teensy-to-any"
         releases_url = f"{repo_url}/releases/latest"
 
-        response = requests.get(releases_url)
+        response = requests.get(releases_url, timeout=timeout)
 
         if response.status_code != 200:
             raise RuntimeError(
                 "Failed to fetch the latest release information. "
                 f"Status code: {response.status_code}")
         release_data = response.json()
         latest_release_version = release_data["tag_name"]
@@ -167,16 +169,16 @@
             )
         return pairs
 
     @property
     def mcu(self):
         return self._ask('mcu')
 
-    def _update_firmware(self, *, mcu=None, force=False):
-        from packaging.version import Version
+    def _update_firmware(self, *, mcu=None, force=False, timeout=2):
+        import requests  # pylint: disable=import-outside-toplevel
 
         current_version = self.version
         if mcu is None:
             mcu = self.mcu
 
         if mcu is None:
             raise RuntimeError(
@@ -184,27 +186,24 @@
                 "before attempting to update the firmware.")
 
         if os.name == 'nt':
             # We do supporting updating, but it is "scary" to do so since
             # there is no serial number specificity
             raise RuntimeError("We do not supporting updating MCUs on windows")
 
-        latest_version = self._get_latest_available_firmware()
+        latest_version = self._get_latest_available_firmware(timeout=timeout)
         if not force:
             if Version(current_version) >= Version(latest_version):
                 return
 
-        file_url = f"https://github.com/ramonaoptics/teensy-to-any/releases/download/{latest_version}/firmware_{mcu.lower()}.hex"  # noqa
+        file_url = f"https://github.com/ramonaoptics/teensy-to-any/releases/download/{latest_version}/firmware_{mcu.lower()}.hex"  # noqa # pylint: disable=line-too-long
 
-        import tempfile
-        import requests
-        import subprocess
         firmware_filename = tempfile.mktemp(suffix='.hex')
 
-        response = requests.get(file_url)
+        response = requests.get(file_url, timeout=timeout)
         if response.status_code != 200:
             raise RuntimeError("Failed to download firmware")
 
         # Open the file for binary writing
         with open(firmware_filename, 'wb') as file:
             # Write the content to the file in chunks
             for chunk in response.iter_content(chunk_size=4096):
@@ -222,16 +221,21 @@
         self.close()
         subprocess.check_call(cmd_list)
         # Wait for the device to reboot
         sleep(1)
         self._requested_serial_number = requested_serial_number
         self.open()
 
-    def __init__(self, serial_number=None, *,
-                 baudrate=115200, timeout=0.205, open=True):
+    def __init__(
+        self,
+        serial_number=None, *,
+        baudrate=115200,
+        timeout=0.205,
+        open=True,  # pylint: disable=redefined-builtin
+    ):
         """A class to control the TeensyToAny Debugger.
 
         Parameters
         ----------
         serial_number: optional
             If provided, will attempt to open the specified serial number
 
@@ -242,14 +246,15 @@
 
         """
 
         self._requested_serial_number = serial_number
         self._baudrate = baudrate
         self._timeout = timeout
         self._serial = None
+        self.serial_number = None
         self._version = None
         if open:
             self.open()
 
     def open(self):
         try:
             self._open()
@@ -277,15 +282,15 @@
 
         # Cache the version number so we don't keep asking it for speed
         response_version = self._ask("version")
         self._version = response_version
         good_version = False
         try:
             good_version = Version(self.version) > Version("0.0.0")
-        except Exception:
+        except Exception:  # pylint: disable=broad-exception-caught
             pass
 
         if not good_version:
             raise RuntimeError(
                 f"Unkown version '{response_version}'. "
                 "Please contact Ramona Optics for help with this error."
             )
@@ -324,18 +329,19 @@
             string of data read.
 
         """
         if self._serial is None:
             raise RuntimeError("Device must be opened first")
 
         data = self._serial.read_until(LF, size=size)
+
         if decode:
-            return data.decode()
-        else:
-            return data
+            data = data.decode()
+
+        return data
 
     def _ask(self, data, *, size=1024, decode=True) -> str:
         self._write(data)
         returned = self._read(size=size, decode=decode)
         if len(returned) == 0:
             raise RuntimeError(f"Failed to read a response for command: {data}")
 
@@ -429,31 +435,29 @@
                 self._ask(
                     f"i2c_write_uint16 "
                     f"0x{address:02x} 0x{register_address:04x} 0x{data:04x}")
             else:
                 raise NotImplementedError()
 
     def i2c_read_payload(self, address: int, register_address: int, num_bytes: int) -> Sequence:
-
-        if Version(self.version) >= Version("0.0.14"):
-            cmd = f"i2c_read_payload 0x{address:02x} 0x{register_address:02x} {num_bytes}"
-            returned = self._ask(cmd)
-            register_data = [int(val, base=0) for val in returned.split()]  # returns big endian
-            return register_data
-
-        else:
+        if Version(self.version) < Version("0.0.14"):
             if num_bytes != 1:
                 raise NotImplementedError()
             returned = self._ask(f"i2c_read_no_register_uint8 0x{address:02x}")
             register_data = int(returned, base=0)
             return int.to_bytes(
                 int(register_data),
                 length=num_bytes, byteorder='big',
                 signed=False)
 
+        cmd = f"i2c_read_payload 0x{address:02x} 0x{register_address:02x} {num_bytes}"
+        returned = self._ask(cmd)
+        register_data = [int(val, base=0) for val in returned.split()]  # returns big endian
+        return register_data
+
     def gpio_digital_write(self, pin, value):
         """Call the ardunio DigitalWrite function.
 
         Parameters
         ----------
         pin: int
             Pin number to control.
```

### Comparing `teensytoany-0.2.1/teensytoany.egg-info/PKG-INFO` & `teensytoany-0.3.0/teensytoany.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: teensytoany
-Version: 0.2.1
+Version: 0.3.0
 Summary: A pythonic way to access the teensytoany board
 Home-page: https://github.com/ramonaoptics/python-teensytoany
 Author: Ramona Optics Inc.
 Author-email: info@ramonaoptics.com
 License: BSD license
 Keywords: teensytoany
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial
 Requires-Dist: packaging
 
 # Python TeensyToAny
 
@@ -49,14 +48,18 @@
 [hmaarrfk/cookiecutter-pypackage](https://github.com/hmaarrfk/cookiecutter-pypackage)
 project template.
 
 
 
 # History
 
+## 0.3.0 (2024-04-02)
+
+* Add a `timeout` property to the functions that deal with updating the firmware.
+
 ## 0.2.0 (2023-11-07)
 
 * Add a `timeout` property to simplify modifying the command timeout.
 
 ## 0.1.0 (2023-09-29)
 
 * Provide access the new `mcu` command that reveals the microcontroller used at
```

### Comparing `teensytoany-0.2.1/teensytoany.egg-info/SOURCES.txt` & `teensytoany-0.3.0/teensytoany.egg-info/SOURCES.txt`

 * *Files identical despite different names*

