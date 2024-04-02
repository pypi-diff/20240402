# Comparing `tmp/dvg-qdeviceio-1.2.0.tar.gz` & `tmp/dvg-qdeviceio-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvg-qdeviceio-1.2.0.tar", last modified: Mon Feb 27 14:17:43 2023, max compression
+gzip compressed data, was "dvg-qdeviceio-1.3.0.tar", last modified: Tue Apr  2 19:11:53 2024, max compression
```

## Comparing `dvg-qdeviceio-1.2.0.tar` & `dvg-qdeviceio-1.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 14:17:43.286317 dvg-qdeviceio-1.2.0/
--rw-rw-rw-   0        0        0       37 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/.coveragerc
--rw-rw-rw-   0        0        0      736 2022-09-15 13:29:04.000000 dvg-qdeviceio-1.2.0/.readthedocs.yml
--rw-rw-rw-   0        0        0       76 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3078 2023-02-27 13:52:28.000000 dvg-qdeviceio-1.2.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0     2525 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1098 2022-09-13 16:21:38.000000 dvg-qdeviceio-1.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0      289 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6030 2023-02-27 14:17:43.286317 dvg-qdeviceio-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1568 2023-02-27 14:10:43.000000 dvg-qdeviceio-1.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-27 14:17:43.281797 dvg-qdeviceio-1.2.0/docs/
--rw-rw-rw-   0        0        0   200983 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/DAQ_trigger_diagram.pdf
--rw-rw-rw-   0        0        0   113976 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/DAQ_trigger_diagram.png
--rw-rw-rw-   0        0        0      654 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/Makefile
--rw-rw-rw-   0        0        0      667 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/api-daqtrigger-continuous.rst
--rw-rw-rw-   0        0        0     1638 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/api-daqtrigger-internaltimer.rst
--rw-rw-rw-   0        0        0     2975 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/api-daqtrigger-singleshotwakeup.rst
--rw-rw-rw-   0        0        0      141 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/api-daqtrigger.rst
--rw-rw-rw-   0        0        0     1286 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/api-qdeviceio.rst
--rw-rw-rw-   0        0        0      322 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/api-workerdaq.rst
--rw-rw-rw-   0        0        0      337 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/api-workerjobs.rst
--rw-rw-rw-   0        0        0       27 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/authors.rst
--rw-rw-rw-   0        0        0       29 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/changelog.rst
--rw-rw-rw-   0        0        0     3496 2023-02-27 13:54:36.000000 dvg-qdeviceio-1.2.0/docs/conf.py
--rw-rw-rw-   0        0        0       32 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/contributing.rst
--rw-rw-rw-   0        0        0      352 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/example.rst
--rw-rw-rw-   0        0        0      480 2022-09-13 16:21:38.000000 dvg-qdeviceio-1.2.0/docs/features.rst
--rw-rw-rw-   0        0        0       45 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/genindex.rst
--rw-rw-rw-   0        0        0     1157 2022-09-15 13:29:05.000000 dvg-qdeviceio-1.2.0/docs/index.rst
--rwxrwxrwx   0        0        0      795 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/make.bat
--rw-rw-rw-   0        0        0     1200 2022-09-15 13:29:05.000000 dvg-qdeviceio-1.2.0/docs/notes.rst
--rw-rw-rw-   0        0        0       54 2022-09-15 13:29:05.000000 dvg-qdeviceio-1.2.0/docs/requirements.txt
--rw-rw-rw-   0        0        0     2505 2022-06-22 13:48:06.000000 dvg-qdeviceio-1.2.0/docs/usage.rst
--rw-rw-rw-   0        0        0       42 2023-02-27 14:17:43.286317 dvg-qdeviceio-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2718 2023-02-27 14:12:35.000000 dvg-qdeviceio-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-27 14:17:43.282305 dvg-qdeviceio-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-27 14:17:43.285317 dvg-qdeviceio-1.2.0/src/dvg_qdeviceio.egg-info/
--rw-rw-rw-   0        0        0     6030 2023-02-27 14:17:43.000000 dvg-qdeviceio-1.2.0/src/dvg_qdeviceio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      893 2023-02-27 14:17:43.000000 dvg-qdeviceio-1.2.0/src/dvg_qdeviceio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 14:17:43.000000 dvg-qdeviceio-1.2.0/src/dvg_qdeviceio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-13 12:04:50.000000 dvg-qdeviceio-1.2.0/src/dvg_qdeviceio.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       37 2023-02-27 14:17:43.000000 dvg-qdeviceio-1.2.0/src/dvg_qdeviceio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-27 14:17:43.000000 dvg-qdeviceio-1.2.0/src/dvg_qdeviceio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    67144 2023-02-27 13:51:35.000000 dvg-qdeviceio-1.2.0/src/dvg_qdeviceio.py
-drwxrwxrwx   0        0        0        0 2023-02-27 14:17:43.285317 dvg-qdeviceio-1.2.0/tests/
--rw-rw-rw-   0        0        0    23946 2023-02-27 10:12:34.000000 dvg-qdeviceio-1.2.0/tests/test_dvg_qdeviceio.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:11:53.450162 dvg-qdeviceio-1.3.0/
+-rw-rw-rw-   0        0        0       37 2020-05-27 18:27:16.000000 dvg-qdeviceio-1.3.0/.coveragerc
+-rw-rw-rw-   0        0        0      736 2022-09-14 14:04:53.000000 dvg-qdeviceio-1.3.0/.readthedocs.yml
+-rw-rw-rw-   0        0        0       76 2020-05-25 17:50:04.000000 dvg-qdeviceio-1.3.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3213 2024-04-02 19:06:44.000000 dvg-qdeviceio-1.3.0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     2525 2020-07-02 10:49:22.000000 dvg-qdeviceio-1.3.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1098 2022-09-13 19:10:08.000000 dvg-qdeviceio-1.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      289 2020-06-17 12:36:05.000000 dvg-qdeviceio-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6458 2024-04-02 19:11:53.449163 dvg-qdeviceio-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1740 2023-02-27 19:52:04.000000 dvg-qdeviceio-1.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-02 19:11:53.441092 dvg-qdeviceio-1.3.0/docs/
+-rw-rw-rw-   0        0        0   200983 2020-06-25 17:26:03.000000 dvg-qdeviceio-1.3.0/docs/DAQ_trigger_diagram.pdf
+-rw-rw-rw-   0        0        0   113976 2020-06-25 17:26:03.000000 dvg-qdeviceio-1.3.0/docs/DAQ_trigger_diagram.png
+-rw-rw-rw-   0        0        0      654 2020-06-10 12:56:24.000000 dvg-qdeviceio-1.3.0/docs/Makefile
+-rw-rw-rw-   0        0        0      667 2020-07-07 12:22:11.000000 dvg-qdeviceio-1.3.0/docs/api-daqtrigger-continuous.rst
+-rw-rw-rw-   0        0        0     1638 2020-07-15 10:21:16.000000 dvg-qdeviceio-1.3.0/docs/api-daqtrigger-internaltimer.rst
+-rw-rw-rw-   0        0        0     2975 2022-09-14 10:53:07.000000 dvg-qdeviceio-1.3.0/docs/api-daqtrigger-singleshotwakeup.rst
+-rw-rw-rw-   0        0        0      141 2020-07-07 12:22:40.000000 dvg-qdeviceio-1.3.0/docs/api-daqtrigger.rst
+-rw-rw-rw-   0        0        0     1286 2020-07-02 10:42:44.000000 dvg-qdeviceio-1.3.0/docs/api-qdeviceio.rst
+-rw-rw-rw-   0        0        0      322 2020-07-02 10:42:52.000000 dvg-qdeviceio-1.3.0/docs/api-workerdaq.rst
+-rw-rw-rw-   0        0        0      337 2020-07-02 10:42:55.000000 dvg-qdeviceio-1.3.0/docs/api-workerjobs.rst
+-rw-rw-rw-   0        0        0       27 2020-06-17 17:34:08.000000 dvg-qdeviceio-1.3.0/docs/authors.rst
+-rw-rw-rw-   0        0        0       29 2020-06-17 17:34:49.000000 dvg-qdeviceio-1.3.0/docs/changelog.rst
+-rw-rw-rw-   0        0        0     3496 2024-04-02 19:02:54.000000 dvg-qdeviceio-1.3.0/docs/conf.py
+-rw-rw-rw-   0        0        0       32 2020-06-17 17:36:57.000000 dvg-qdeviceio-1.3.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0      352 2020-06-27 17:30:39.000000 dvg-qdeviceio-1.3.0/docs/example.rst
+-rw-rw-rw-   0        0        0      480 2022-09-13 19:10:08.000000 dvg-qdeviceio-1.3.0/docs/features.rst
+-rw-rw-rw-   0        0        0       45 2020-06-17 17:41:53.000000 dvg-qdeviceio-1.3.0/docs/genindex.rst
+-rw-rw-rw-   0        0        0     1157 2022-09-14 10:49:13.000000 dvg-qdeviceio-1.3.0/docs/index.rst
+-rwxrwxrwx   0        0        0      795 2020-06-18 15:36:35.000000 dvg-qdeviceio-1.3.0/docs/make.bat
+-rw-rw-rw-   0        0        0     1200 2022-09-14 10:53:02.000000 dvg-qdeviceio-1.3.0/docs/notes.rst
+-rw-rw-rw-   0        0        0       54 2022-09-14 14:13:45.000000 dvg-qdeviceio-1.3.0/docs/requirements.txt
+-rw-rw-rw-   0        0        0     2505 2020-07-07 12:22:40.000000 dvg-qdeviceio-1.3.0/docs/usage.rst
+-rw-rw-rw-   0        0        0       42 2024-04-02 19:11:53.450162 dvg-qdeviceio-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2769 2024-04-02 19:05:20.000000 dvg-qdeviceio-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:11:53.442092 dvg-qdeviceio-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 19:11:53.448160 dvg-qdeviceio-1.3.0/src/dvg_qdeviceio.egg-info/
+-rw-rw-rw-   0        0        0     6458 2024-04-02 19:11:53.000000 dvg-qdeviceio-1.3.0/src/dvg_qdeviceio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      893 2024-04-02 19:11:53.000000 dvg-qdeviceio-1.3.0/src/dvg_qdeviceio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 19:11:53.000000 dvg-qdeviceio-1.3.0/src/dvg_qdeviceio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-14 11:02:11.000000 dvg-qdeviceio-1.3.0/src/dvg_qdeviceio.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       37 2024-04-02 19:11:53.000000 dvg-qdeviceio-1.3.0/src/dvg_qdeviceio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-02 19:11:53.000000 dvg-qdeviceio-1.3.0/src/dvg_qdeviceio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    67044 2024-04-02 19:01:14.000000 dvg-qdeviceio-1.3.0/src/dvg_qdeviceio.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:11:53.447149 dvg-qdeviceio-1.3.0/tests/
+-rw-rw-rw-   0        0        0    22593 2023-02-27 19:49:43.000000 dvg-qdeviceio-1.3.0/tests/test_dvg_qdeviceio.py
```

### Comparing `dvg-qdeviceio-1.2.0/.readthedocs.yml` & `dvg-qdeviceio-1.3.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/CHANGELOG.rst` & `dvg-qdeviceio-1.3.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+1.3.0 (2024-04-02)
+------------------
+* Support Python 3.11
+* All f-strings
+* Type checking via `isinstance()`, not type == ...
+
 1.2.0 (2023-02-27)
 ------------------
 * Deprecated `requires.io` and `travis`
 * Raise `ImportError` instead of general `Exception`
 
 1.1.2 (2022-10-26)
 ------------------
```

### Comparing `dvg-qdeviceio-1.2.0/CONTRIBUTING.rst` & `dvg-qdeviceio-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/LICENSE.txt` & `dvg-qdeviceio-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/PKG-INFO` & `dvg-qdeviceio-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvg-qdeviceio
-Version: 1.2.0
+Version: 1.3.0
 Summary: Hassle-free PyQt/PySide interface for multithreaded data acquisition and communication with an I/O device.
 Home-page: https://python-dvg-qdeviceio.readthedocs.io/
 Author: Dennis van Gils
 Author-email: vangils.dennis@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Dennis-van-Gils/python-dvg-qdeviceio/issues
 Keywords: PyQt5,PyQt6,PySide2,PySide6,multithread,device I/O,automation,laboratory,science
@@ -16,27 +16,32 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
+Requires-Dist: dvg-debug-functions~=2.4
+Requires-Dist: numpy~=1.15
 
 .. image:: https://img.shields.io/pypi/v/dvg-qdeviceio
     :target: https://pypi.org/project/dvg-qdeviceio
 .. image:: https://img.shields.io/pypi/pyversions/dvg-qdeviceio
     :target: https://pypi.org/project/dvg-qdeviceio
 .. image:: https://github.com/Dennis-van-Gils/python-dvg-qdeviceio/actions/workflows/python-package.yml/badge.svg
     :target: https://github.com/Dennis-van-Gils/python-dvg-qdeviceio/actions/workflows/python-package.yml
+.. image:: https://coveralls.io/repos/github/Dennis-van-Gils/python-dvg-qdeviceio/badge.svg
+    :target: https://coveralls.io/github/Dennis-van-Gils/python-dvg-qdeviceio
 .. image:: https://readthedocs.org/projects/python-dvg-qdeviceio/badge/?version=latest
     :target: https://python-dvg-qdeviceio.readthedocs.io/en/latest/?badge=latest
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/License-MIT-purple.svg
     :target: https://github.com/Dennis-van-Gils/python-dvg-qdeviceio/blob/master/LICENSE.txt
 
@@ -58,14 +63,20 @@
 Installation::
 
     pip install dvg-qdeviceio
 
 Changelog
 =========
 
+1.3.0 (2024-04-02)
+------------------
+* Support Python 3.11
+* All f-strings
+* Type checking via `isinstance()`, not type == ...
+
 1.2.0 (2023-02-27)
 ------------------
 * Deprecated `requires.io` and `travis`
 * Raise `ImportError` instead of general `Exception`
 
 1.1.2 (2022-10-26)
 ------------------
```

### Comparing `dvg-qdeviceio-1.2.0/README.rst` & `dvg-qdeviceio-1.3.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 .. image:: https://img.shields.io/pypi/v/dvg-qdeviceio
     :target: https://pypi.org/project/dvg-qdeviceio
 .. image:: https://img.shields.io/pypi/pyversions/dvg-qdeviceio
     :target: https://pypi.org/project/dvg-qdeviceio
 .. image:: https://github.com/Dennis-van-Gils/python-dvg-qdeviceio/actions/workflows/python-package.yml/badge.svg
     :target: https://github.com/Dennis-van-Gils/python-dvg-qdeviceio/actions/workflows/python-package.yml
+.. image:: https://coveralls.io/repos/github/Dennis-van-Gils/python-dvg-qdeviceio/badge.svg
+    :target: https://coveralls.io/github/Dennis-van-Gils/python-dvg-qdeviceio
 .. image:: https://readthedocs.org/projects/python-dvg-qdeviceio/badge/?version=latest
     :target: https://python-dvg-qdeviceio.readthedocs.io/en/latest/?badge=latest
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/License-MIT-purple.svg
     :target: https://github.com/Dennis-van-Gils/python-dvg-qdeviceio/blob/master/LICENSE.txt
```

### Comparing `dvg-qdeviceio-1.2.0/docs/DAQ_trigger_diagram.pdf` & `dvg-qdeviceio-1.3.0/docs/DAQ_trigger_diagram.pdf`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/docs/DAQ_trigger_diagram.png` & `dvg-qdeviceio-1.3.0/docs/DAQ_trigger_diagram.png`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/docs/Makefile` & `dvg-qdeviceio-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/docs/api-daqtrigger-continuous.rst` & `dvg-qdeviceio-1.3.0/docs/api-daqtrigger-continuous.rst`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/docs/api-daqtrigger-internaltimer.rst` & `dvg-qdeviceio-1.3.0/docs/api-daqtrigger-internaltimer.rst`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/docs/api-daqtrigger-singleshotwakeup.rst` & `dvg-qdeviceio-1.3.0/docs/api-daqtrigger-singleshotwakeup.rst`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/docs/api-qdeviceio.rst` & `dvg-qdeviceio-1.3.0/docs/api-qdeviceio.rst`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/docs/conf.py` & `dvg-qdeviceio-1.3.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "DvG_QDeviceIO"
 copyright = "2022, Dennis van Gils"
 author = "Dennis van Gils"
 
 # The full version, including alpha/beta/rc tags
-release = "1.2.0"
+release = "1.3.0"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `dvg-qdeviceio-1.2.0/docs/index.rst` & `dvg-qdeviceio-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/docs/make.bat` & `dvg-qdeviceio-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/docs/notes.rst` & `dvg-qdeviceio-1.3.0/docs/notes.rst`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/docs/usage.rst` & `dvg-qdeviceio-1.3.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/setup.py` & `dvg-qdeviceio-1.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="dvg-qdeviceio",
-    version="1.2.0",
+    version="1.3.0",
     license="MIT",
     description="Hassle-free PyQt/PySide interface for multithreaded data acquisition and communication with an I/O device.",
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
@@ -53,14 +53,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
     ],
     project_urls={
         "Issue Tracker": "https://github.com/Dennis-van-Gils/python-dvg-qdeviceio/issues",
     },
     keywords=[
@@ -72,12 +73,12 @@
         "device I/O",
         "automation",
         "laboratory",
         "science",
     ],
     python_requires=">=3.6",
     install_requires=[
-        "dvg-debug-functions~=2.2",
+        "dvg-debug-functions~=2.4",
         "numpy~=1.15",
     ],
     extras_require={},
 )
```

### Comparing `dvg-qdeviceio-1.2.0/src/dvg_qdeviceio.egg-info/PKG-INFO` & `dvg-qdeviceio-1.3.0/src/dvg_qdeviceio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvg-qdeviceio
-Version: 1.2.0
+Version: 1.3.0
 Summary: Hassle-free PyQt/PySide interface for multithreaded data acquisition and communication with an I/O device.
 Home-page: https://python-dvg-qdeviceio.readthedocs.io/
 Author: Dennis van Gils
 Author-email: vangils.dennis@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Dennis-van-Gils/python-dvg-qdeviceio/issues
 Keywords: PyQt5,PyQt6,PySide2,PySide6,multithread,device I/O,automation,laboratory,science
@@ -16,27 +16,32 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
+Requires-Dist: dvg-debug-functions~=2.4
+Requires-Dist: numpy~=1.15
 
 .. image:: https://img.shields.io/pypi/v/dvg-qdeviceio
     :target: https://pypi.org/project/dvg-qdeviceio
 .. image:: https://img.shields.io/pypi/pyversions/dvg-qdeviceio
     :target: https://pypi.org/project/dvg-qdeviceio
 .. image:: https://github.com/Dennis-van-Gils/python-dvg-qdeviceio/actions/workflows/python-package.yml/badge.svg
     :target: https://github.com/Dennis-van-Gils/python-dvg-qdeviceio/actions/workflows/python-package.yml
+.. image:: https://coveralls.io/repos/github/Dennis-van-Gils/python-dvg-qdeviceio/badge.svg
+    :target: https://coveralls.io/github/Dennis-van-Gils/python-dvg-qdeviceio
 .. image:: https://readthedocs.org/projects/python-dvg-qdeviceio/badge/?version=latest
     :target: https://python-dvg-qdeviceio.readthedocs.io/en/latest/?badge=latest
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/License-MIT-purple.svg
     :target: https://github.com/Dennis-van-Gils/python-dvg-qdeviceio/blob/master/LICENSE.txt
 
@@ -58,14 +63,20 @@
 Installation::
 
     pip install dvg-qdeviceio
 
 Changelog
 =========
 
+1.3.0 (2024-04-02)
+------------------
+* Support Python 3.11
+* All f-strings
+* Type checking via `isinstance()`, not type == ...
+
 1.2.0 (2023-02-27)
 ------------------
 * Deprecated `requires.io` and `travis`
 * Raise `ImportError` instead of general `Exception`
 
 1.1.2 (2022-10-26)
 ------------------
```

### Comparing `dvg-qdeviceio-1.2.0/src/dvg_qdeviceio.egg-info/SOURCES.txt` & `dvg-qdeviceio-1.3.0/src/dvg_qdeviceio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvg-qdeviceio-1.2.0/src/dvg_qdeviceio.py` & `dvg-qdeviceio-1.3.0/src/dvg_qdeviceio.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 """PyQt/PySide framework for multithreaded data acquisition and communication
 with an I/O device.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-qdeviceio"
-__date__ = "27-02-2023"
-__version__ = "1.2.0"
-# pylint: disable=protected-access
+__date__ = "02-04-2024"
+__version__ = "1.3.0"
+# pylint: disable=protected-access, wrong-import-position, too-many-lines
 
 import os
 import sys
 import queue
 import time
 from enum import IntEnum, unique
 
@@ -49,15 +49,15 @@
             __import__(lib)
             QT_LIB = lib
             break
         except ImportError:
             pass
 
 if QT_LIB is None:
-    this_file = __file__.split(os.sep)[-1]
+    this_file = __file__.rsplit(os.sep, maxsplit=1)[-1]
     raise ImportError(
         f"{this_file} requires PyQt5, PyQt6, PySide2 or PySide6; "
         "none of these packages could be imported."
     )
 
 # fmt: off
 # pylint: disable=import-error, no-name-in-module
@@ -97,15 +97,15 @@
     print("\nCode coverage test detected\n")
 
 
 def _coverage_resolve_trace(fn):
     @wraps(fn)
     def wrapped(*args, **kwargs):
         if running_coverage:
-            sys.settrace(threading._trace_hook)
+            sys.settrace(threading._trace_hook)  # type: ignore
         fn(*args, **kwargs)
 
     return wrapped
 
 
 # Short-hand alias for DEBUG information
 def _cur_thread_name():
@@ -361,20 +361,20 @@
 
         if not hasattr(dev, "mutex"):
             dev.mutex = QtCore.QMutex()
 
         if not hasattr(dev, "is_alive"):
             dev.is_alive = True  # Assume the device is alive from the start
 
-        if type(self.dev) == self._NoDevice:
+        if isinstance(self.dev, self._NoDevice):
             self.dev = dev
         else:
             pft(
-                "Device can be attached only once. Already attached to '%s'."
-                % self.dev.name
+                "Device can be attached only once. Already attached to "
+                f"'{self.dev.name}'."
             )
             sys.exit(22)
 
     # --------------------------------------------------------------------------
     #   Create workers
     # --------------------------------------------------------------------------
 
@@ -383,28 +383,28 @@
         it to a new :class:`PyQt5.QtCore.QThread`.
 
         Args:
             **kwargs
                 Will be passed directly to :class:`Worker_DAQ` as initialization
                 parameters, :ref:`see here <Worker_DAQ_args>`.
         """
-        if type(self.dev) == self._NoDevice:
+        if isinstance(self.dev, self._NoDevice):
             pft(
                 "Can't create worker_DAQ, because there is no device attached."
                 " Did you forget to call 'attach_device()' first?"
             )
             sys.exit(99)
 
         self.worker_DAQ = Worker_DAQ(qdev=self, **kwargs)
         self._request_worker_DAQ_stop.connect(self.worker_DAQ._stop)
         self._request_worker_DAQ_pause.connect(self.worker_DAQ.pause)
         self._request_worker_DAQ_unpause.connect(self.worker_DAQ.unpause)
 
         self._thread_DAQ = QtCore.QThread()
-        self._thread_DAQ.setObjectName("%s_DAQ" % self.dev.name)
+        self._thread_DAQ.setObjectName(f"{self.dev.name}_DAQ")
         self._thread_DAQ.started.connect(self.worker_DAQ._do_work)
         self.worker_DAQ.moveToThread(self._thread_DAQ)
 
         if hasattr(self.worker_DAQ, "_timer"):
             self.worker_DAQ._timer.moveToThread(self._thread_DAQ)
 
     def create_worker_jobs(self, **kwargs):
@@ -412,25 +412,25 @@
         it to a new :class:`PyQt5.QtCore.QThread`.
 
         Args:
             **kwargs
                 Will be passed directly to :class:`Worker_jobs` as initialization
                 parameters, :ref:`see here <Worker_jobs_args>`.
         """
-        if type(self.dev) == self._NoDevice:
+        if isinstance(self.dev, self._NoDevice):
             pft(
                 "Can't create worker_jobs, because there is no device attached."
                 " Did you forget to call 'attach_device()' first?"
             )
             sys.exit(99)
 
         self.worker_jobs = Worker_jobs(qdev=self, **kwargs)
 
         self._thread_jobs = QtCore.QThread()
-        self._thread_jobs.setObjectName("%s_jobs" % self.dev.name)
+        self._thread_jobs.setObjectName(f"{self.dev.name}_jobs")
         self._thread_jobs.started.connect(self.worker_jobs._do_work)
         self.worker_jobs.moveToThread(self._thread_jobs)
 
     # --------------------------------------------------------------------------
     #   Start workers
     # --------------------------------------------------------------------------
 
@@ -480,31 +480,31 @@
                 See :meth:`start` for details.
 
         Returns:
             True if successful, False otherwise.
         """
         if self._thread_DAQ is None:
             pft(
-                "Worker_DAQ  %s: Can't start thread, because it does not exist. "
-                "Did you forget to call 'create_worker_DAQ()' first?"
-                % self.dev.name
+                f"Worker_DAQ  {self.dev.name}: Can't start thread, because it "
+                "does not exist. Did you forget to call 'create_worker_DAQ()' "
+                "first?"
             )
             sys.exit(404)  # --> leaving
 
         elif not self.dev.is_alive:
             dprint(
-                "Worker_DAQ  %s: WARNING - Device is not alive.\n"
-                % self.dev.name,
+                f"Worker_DAQ  {self.dev.name}: "
+                "WARNING - Device is not alive.\n",
                 ANSI.RED,
             )
             return False  # --> leaving
 
         if self.worker_DAQ.debug:
             tprint(
-                "Worker_DAQ  %s: start requested..." % self.dev.name,
+                f"Worker_DAQ  {self.dev.name}: start requested...",
                 ANSI.WHITE,
             )
 
         self._thread_DAQ.start(priority)
 
         # Wait for worker_DAQ to confirm having started
         locker_wait = QtCore.QMutexLocker(self._mutex_wait_worker_DAQ)
@@ -545,31 +545,31 @@
                 See :meth:`start` for details.
 
         Returns:
             True if successful, False otherwise.
         """
         if self._thread_jobs is None:
             pft(
-                "Worker_jobs %s: Can't start thread because it does not exist. "
-                "Did you forget to call 'create_worker_jobs()' first?"
-                % self.dev.name
+                f"Worker_jobs {self.dev.name}: Can't start thread because it "
+                "does not exist. Did you forget to call 'create_worker_jobs()' "
+                "first?"
             )
             sys.exit(404)  # --> leaving
 
         elif not self.dev.is_alive:
             dprint(
-                "Worker_jobs %s: WARNING - Device is not alive.\n"
-                % self.dev.name,
+                f"Worker_jobs {self.dev.name}: "
+                "WARNING - Device is not alive.\n",
                 ANSI.RED,
             )
             return False  # --> leaving
 
         if self.worker_jobs.debug:
             tprint(
-                "Worker_jobs %s: start requested..." % self.dev.name,
+                f"Worker_jobs {self.dev.name}: start requested...",
                 ANSI.WHITE,
             )
 
         self._thread_jobs.start(priority)
 
         # Wait for worker_jobs to confirm having started
         locker_wait = QtCore.QMutexLocker(self._mutex_wait_worker_jobs)
@@ -612,23 +612,23 @@
         if self._thread_DAQ is None or not self.worker_DAQ._has_started:
             return True
 
         if self._thread_DAQ.isFinished():
             # CASE: Device has had a 'connection_lost' event during run-time,
             # which already stopped and closed the thread.
             print(
-                "Closing thread %s already closed."
-                % "{:.<16}".format(self._thread_DAQ.objectName())
+                "Closing thread "
+                f"{self._thread_DAQ.objectName():.<16} already closed."
             )
             return True
 
         if not self.worker_DAQ._has_stopped:
             if self.worker_DAQ.debug:
                 tprint(
-                    "Worker_DAQ  %s: stop requested..." % self.dev.name,
+                    f"Worker_DAQ  {self.dev.name}: stop requested...",
                     ANSI.WHITE,
                 )
 
             if self.worker_DAQ._DAQ_trigger == DAQ_TRIGGER.INTERNAL_TIMER:
                 # The QTimer inside the INTERNAL_TIMER '_do_work()'-routine
                 # /must/ be stopped from within the worker_DAQ thread. Hence,
                 # we must use a signal from out of this different thread.
@@ -653,25 +653,21 @@
 
             # Wait for worker_DAQ to confirm having stopped
             locker_wait = QtCore.QMutexLocker(self._mutex_wait_worker_DAQ)
             self._qwc_worker_DAQ_stopped.wait(self._mutex_wait_worker_DAQ)
             locker_wait.unlock()
 
         self._thread_DAQ.quit()
-        print(
-            "Closing thread %s "
-            % "{:.<16}".format(self._thread_DAQ.objectName()),
-            end="",
-        )
+        print(f"Closing thread {self._thread_DAQ.objectName():.<16} ", end="")
         if self._thread_DAQ.wait(2000):
             print("done.\n", end="")
             return True
-        else:
-            print("FAILED.\n", end="")  # pragma: no cover
-            return False  # pragma: no cover
+
+        print("FAILED.\n", end="")  # pragma: no cover
+        return False  # pragma: no cover
 
     def quit_worker_jobs(self) -> bool:
         """Stop :attr:`worker_jobs` and close its thread.
 
         Returns:
             True if successful, False otherwise.
         """
@@ -679,23 +675,23 @@
         if self._thread_jobs is None or not self.worker_jobs._has_started:
             return True
 
         if self._thread_jobs.isFinished():
             # CASE: Device has had a 'connection_lost' event during run-time,
             # which already stopped the worker and closed the thread.
             print(
-                "Closing thread %s already closed."
-                % "{:.<16}".format(self._thread_jobs.objectName())
+                "Closing thread "
+                f"{self._thread_jobs.objectName():.<16} already closed."
             )
             return True
 
         if not self.worker_jobs._has_stopped:
             if self.worker_jobs.debug:
                 tprint(
-                    "Worker_jobs %s: stop requested..." % self.dev.name,
+                    f"Worker_jobs {self.dev.name}: stop requested...",
                     ANSI.WHITE,
                 )
 
             # The QWaitCondition inside the SINGLE_SHOT_WAKE_UP '_do_work()'-
             # routine will likely have locked worker_DAQ. Hence, a
             # '_request_worker_DAQ_stop' signal might not get handled by
             # worker_DAQ when emitted from out of this thread. Instead,
@@ -705,25 +701,21 @@
 
             # Wait for worker_jobs to confirm having stopped
             locker_wait = QtCore.QMutexLocker(self._mutex_wait_worker_jobs)
             self._qwc_worker_jobs_stopped.wait(self._mutex_wait_worker_jobs)
             locker_wait.unlock()
 
         self._thread_jobs.quit()
-        print(
-            "Closing thread %s "
-            % "{:.<16}".format(self._thread_jobs.objectName()),
-            end="",
-        )
+        print(f"Closing thread {self._thread_jobs.objectName():.<16} ", end="")
         if self._thread_jobs.wait(2000):
             print("done.\n", end="")
             return True
-        else:
-            print("FAILED.\n", end="")  # pragma: no cover
-            return False  # pragma: no cover
+
+        print("FAILED.\n", end="")  # pragma: no cover
+        return False  # pragma: no cover
 
     # --------------------------------------------------------------------------
     #   worker_DAQ related
     # --------------------------------------------------------------------------
 
     @Slot()
     def pause_DAQ(self):
@@ -1020,21 +1012,27 @@
             self._mutex_wait = QtCore.QMutex()
 
         # Members specifically for CONTINUOUS
         # Note: At start-up, the worker will directly go into a paused state
         # and trigger a 'signal_DAQ_paused' PyQt signal
         elif self._DAQ_trigger == DAQ_TRIGGER.CONTINUOUS:
             self._running = True
-            self._pause = None  # Will be set at init of '_do_work()' when 'start_worker_DAQ()' is called
-            self._paused = None  # Will be set at init of '_do_work()' when 'start_worker_DAQ()' is called
+
+            self._pause = None
+            """Will be set at init of '_do_work()' when 'start_worker_DAQ()' is
+            called"""
+
+            self._paused = None
+            """Will be set at init of '_do_work()' when 'start_worker_DAQ()' is
+            called"""
 
         if self.debug:
             tprint(
-                "Worker_DAQ  %s: init @ thread %s"
-                % (self.dev.name, _cur_thread_name()),
+                f"Worker_DAQ  {self.dev.name}: "
+                f"init @ thread {_cur_thread_name()}",
                 self.debug_color,
             )
 
     @_coverage_resolve_trace
     @Slot()
     def _do_work(self):
         # fmt: off
@@ -1054,26 +1052,26 @@
             # Wait a tiny amount of extra time for QDeviceIO to have entered
             # 'self._qwc_worker_###_started.wait(self._mutex_wait_worker_###)'
             # of method 'start_worker_###()'.
             time.sleep(0.05)
 
             if self.debug:
                 tprint(
-                    "Worker_DAQ  %s: has started" % self.dev.name,
+                    f"Worker_DAQ  {self.dev.name}: has started",
                     self.debug_color,
                 )
 
             # Send confirmation
             self.qdev._qwc_worker_DAQ_started.wakeAll()
             self._has_started = True
 
         if self.debug:
             tprint(
-                "Worker_DAQ  %s: starting @ thread %s"
-                % (self.dev.name, _cur_thread_name()),
+                f"Worker_DAQ  {self.dev.name}: "
+                f"starting @ thread {_cur_thread_name()}",
                 self.debug_color,
             )
 
         # INTERNAL_TIMER
         if self._DAQ_trigger == DAQ_TRIGGER.INTERNAL_TIMER:
             self._timer.start()
             confirm_has_started(self)
@@ -1084,41 +1082,41 @@
             locker_wait.unlock()
 
             while self._running:
                 locker_wait.relock()
 
                 if self.debug:
                     tprint(
-                        "Worker_DAQ  %s: waiting for wake-up trigger"
-                        % self.dev.name,
+                        f"Worker_DAQ  {self.dev.name}: "
+                        "waiting for wake-up trigger",
                         self.debug_color,
                     )
 
                 if init:
                     confirm_has_started(self)
                     init = False
 
                 self._qwc.wait(self._mutex_wait)
 
                 if self.debug:
                     tprint(
-                        "Worker_DAQ  %s: has woken up" % self.dev.name,
+                        f"Worker_DAQ  {self.dev.name}: has woken up",
                         self.debug_color,
                     )
 
                 # Needed check to prevent _perform_DAQ() at final wake up
                 # when _stop() has been called
                 if self._running:
                     self._perform_DAQ()
 
                 locker_wait.unlock()
 
             if self.debug:
                 tprint(
-                    "Worker_DAQ  %s: has stopped" % self.dev.name,
+                    f"Worker_DAQ  {self.dev.name}: has stopped",
                     self.debug_color,
                 )
 
             # Wait a tiny amount for the other thread to have entered the
             # QWaitCondition lock, before giving a wakingAll().
             QtCore.QTimer.singleShot(
                 100,
@@ -1133,50 +1131,49 @@
 
                 if init:
                     self._pause = True
                     self._paused = True
 
                     if self.debug:
                         tprint(
-                            "Worker_DAQ  %s: starting up paused"
-                            % self.dev.name,
+                            f"Worker_DAQ  {self.dev.name}: starting up paused",
                             self.debug_color,
                         )
 
                     self.qdev.signal_DAQ_paused.emit()
 
                     confirm_has_started(self)
                     init = False
 
                 if self._pause:  # == True
                     if self._pause != self._paused:
                         if self.debug and not init:
                             tprint(
-                                "Worker_DAQ  %s: has paused" % self.dev.name,
+                                f"Worker_DAQ  {self.dev.name}: has paused",
                                 self.debug_color,
                             )
                         self.qdev.signal_DAQ_paused.emit()
                         self._paused = True
 
                     time.sleep(0.01)  # Do not hog the CPU while paused
 
                 else:  # == False
                     if self._pause != self._paused:
                         if self.debug:
                             tprint(
-                                "Worker_DAQ  %s: has unpaused" % self.dev.name,
+                                f"Worker_DAQ  {self.dev.name}: has unpaused",
                                 self.debug_color,
                             )
                         self._paused = False
 
                     self._perform_DAQ()
 
             if self.debug:
                 tprint(
-                    "Worker_DAQ  %s: has stopped" % self.dev.name,
+                    f"Worker_DAQ  {self.dev.name}: has stopped",
                     self.debug_color,
                 )
 
             # Wait a tiny amount for 'create_worker_DAQ()', which is running
             # in a different thread than this one, to have entered the
             # QWaitCondition lock, before giving a wakingAll().
             QtCore.QTimer.singleShot(
@@ -1189,16 +1186,16 @@
     @Slot()
     def _perform_DAQ(self):
         locker = QtCore.QMutexLocker(self.dev.mutex)
         self.qdev.update_counter_DAQ += 1
 
         if self.debug:
             tprint(
-                "Worker_DAQ  %s: lock   # %i"
-                % (self.dev.name, self.qdev.update_counter_DAQ),
+                f"Worker_DAQ  {self.dev.name}: "
+                f"lock   # {self.qdev.update_counter_DAQ}",
                 self.debug_color,
             )
 
         # Keep track of the obtained DAQ interval and DAQ rate
         if not self._QET_interval.isValid():
             self._QET_interval.start()
             self._QET_rate.start()
@@ -1227,15 +1224,15 @@
 
         if self.DAQ_function is not None:
             try:
                 success = self.DAQ_function()
             except Exception as err:  # pylint: disable=broad-except
                 pft(err)
                 dprint(
-                    "@ Worker_DAQ %s\n" % self.dev.name,
+                    f"@ Worker_DAQ {self.dev.name}\n",
                     ANSI.RED,
                 )
             else:
                 if success:
                     # Did return True, hence was successfull
                     # --> Reset the 'not alive' counter
                     self.qdev.not_alive_counter_DAQ = 0
@@ -1245,47 +1242,47 @@
 
         # ----------------------------------
         #   End user-supplied DAQ function
         # ----------------------------------
 
         if self.debug:
             tprint(
-                "Worker_DAQ  %s: unlock # %i"
-                % (self.dev.name, self.qdev.update_counter_DAQ),
+                f"Worker_DAQ  {self.dev.name}: "
+                f"unlock # {self.qdev.update_counter_DAQ}",
                 self.debug_color,
             )
 
         locker.unlock()
 
         # Check the not alive counter
         if self.qdev.not_alive_counter_DAQ >= self.critical_not_alive_count:
             dprint(
-                "Worker_DAQ  %s: Lost connection to device." % self.dev.name,
+                f"Worker_DAQ  {self.dev.name}: " f"Lost connection to device.",
                 ANSI.RED,
             )
             self.dev.is_alive = False
             self._stop()
             self.qdev.signal_connection_lost.emit()
             return
 
         self.qdev.signal_DAQ_updated.emit()
 
     @Slot()
     def _stop(self):
         """Stop the worker to prepare for quitting the worker thread."""
         if self.debug:
-            tprint("Worker_DAQ  %s: stopping" % self.dev.name, self.debug_color)
+            tprint(f"Worker_DAQ  {self.dev.name}: stopping", self.debug_color)
 
         if self._DAQ_trigger == DAQ_TRIGGER.INTERNAL_TIMER:
             # NOTE: The timer /must/ be stopped from the worker_DAQ thread!
             self._timer.stop()
 
             if self.debug:
                 tprint(
-                    "Worker_DAQ  %s: has stopped" % self.dev.name,
+                    f"Worker_DAQ  {self.dev.name}: has stopped",
                     self.debug_color,
                 )
 
             # Wait a tiny amount for the other thread to have entered the
             # QWaitCondition lock, before giving a wakingAll().
             QtCore.QTimer.singleShot(
                 100,
@@ -1312,15 +1309,15 @@
 
         This method should not be called from another thread. Connect this slot
         to a signal instead.
         """
         if self._DAQ_trigger == DAQ_TRIGGER.CONTINUOUS:
             if self.debug:
                 tprint(
-                    "Worker_DAQ  %s: pause requested..." % self.dev.name,
+                    f"Worker_DAQ  {self.dev.name}: pause requested...",
                     ANSI.WHITE,
                 )
 
             # The possible undefined behavior of changing variable '_pause'
             # from out of another thread gets handled acceptably correct in
             # '_do_work()' as per my design.
             self._pause = True
@@ -1334,15 +1331,15 @@
 
         This method should not be called from another thread. Connect this slot
         to a signal instead.
         """
         if self._DAQ_trigger == DAQ_TRIGGER.CONTINUOUS:
             if self.debug:
                 tprint(
-                    "Worker_DAQ  %s: unpause requested..." % self.dev.name,
+                    f"Worker_DAQ  {self.dev.name}: unpause requested...",
                     ANSI.WHITE,
                 )
 
             # The possible undefined behavior of changing variable '_pause'
             # from out of another thread gets handled acceptably correct in
             # '_do_work()' as per my design.
             self._pause = False
@@ -1357,15 +1354,15 @@
         description at :meth:`QDeviceIO.wake_up_DAQ`.
 
         This method can be called from another thread.
         """
         if self._DAQ_trigger == DAQ_TRIGGER.SINGLE_SHOT_WAKE_UP:
             if self.debug:
                 tprint(
-                    "Worker_DAQ  %s: wake-up requested..." % self.dev.name,
+                    f"Worker_DAQ  {self.dev.name}: wake-up requested...",
                     ANSI.WHITE,
                 )
 
             self._qwc.wakeAll()
 
 
 # ------------------------------------------------------------------------------
@@ -1512,16 +1509,16 @@
         # to ensure proper multithreaded operation.
         self._sentinel = None
         self._queue = queue.Queue()
         self._queue.put(self._sentinel)
 
         if self.debug:
             tprint(
-                "Worker_jobs %s: init @ thread %s"
-                % (self.dev.name, _cur_thread_name()),
+                f"Worker_jobs {self.dev.name}: "
+                f"init @ thread {_cur_thread_name()}",
                 self.debug_color,
             )
 
     @_coverage_resolve_trace
     @Slot()
     def _do_work(self):
         # fmt: off
@@ -1541,64 +1538,63 @@
             # Wait a tiny amount of extra time for QDeviceIO to have entered
             # 'self._qwc_worker_###_started.wait(self._mutex_wait_worker_###)'
             # of method 'start_worker_###()'.
             time.sleep(0.05)
 
             if self.debug:
                 tprint(
-                    "Worker_jobs %s: has started" % self.dev.name,
+                    f"Worker_jobs {self.dev.name}: has started",
                     self.debug_color,
                 )
 
             # Send confirmation
             self.qdev._qwc_worker_jobs_started.wakeAll()
             self._has_started = True
 
         if self.debug:
             tprint(
-                "Worker_jobs %s: starting @ thread %s"
-                % (self.dev.name, _cur_thread_name()),
+                f"Worker_jobs {self.dev.name}: "
+                f"starting @ thread {_cur_thread_name()}",
                 self.debug_color,
             )
 
         locker_wait = QtCore.QMutexLocker(self._mutex_wait)
         locker_wait.unlock()
 
         while self._running:
             locker_wait.relock()
 
             if self.debug:
                 tprint(
-                    "Worker_jobs %s: waiting for wake-up trigger"
-                    % self.dev.name,
+                    f"Worker_jobs {self.dev.name}: waiting for wake-up trigger",
                     self.debug_color,
                 )
 
             if init:
                 confirm_has_started(self)
                 init = False
 
             self._qwc.wait(self._mutex_wait)
 
             if self.debug:
                 tprint(
-                    "Worker_jobs %s: has woken up" % self.dev.name,
+                    f"Worker_jobs {self.dev.name}: has woken up",
                     self.debug_color,
                 )
 
             # Needed check to prevent _perform_jobs() at final wake up
             # when _stop() has been called
             if self._running:
                 self._perform_jobs()
 
             locker_wait.unlock()
 
         if self.debug:
             tprint(
-                "Worker_jobs %s: has stopped" % self.dev.name,
+                f"Worker_jobs {self.dev.name}: has stopped",
                 self.debug_color,
             )
 
         # Wait a tiny amount for the other thread to have entered the
         # QWaitCondition lock, before giving a wakingAll().
         QtCore.QTimer.singleShot(
             100,
@@ -1610,76 +1606,78 @@
     @Slot()
     def _perform_jobs(self):
         locker = QtCore.QMutexLocker(self.dev.mutex)
         self.qdev.update_counter_jobs += 1
 
         if self.debug:
             tprint(
-                "Worker_jobs %s: lock   # %i"
-                % (self.dev.name, self.qdev.update_counter_jobs),
+                f"Worker_jobs {self.dev.name}: "
+                f"lock   # {self.qdev.update_counter_jobs}",
                 self.debug_color,
             )
 
         # Process all jobs until the queue is empty. We must iterate 2 times
         # because we use a sentinel in a FIFO queue. First iter removes the old
         # sentinel. Second iter processes the remaining queue items and will put
         # back a new sentinel again.
         for _i in range(2):
             for job in iter(self._queue.get_nowait, self._sentinel):
                 func = job[0]
                 args = job[1:]
 
                 if self.debug:
-                    if type(func) == str:
+                    if isinstance(func, str):
                         tprint(
-                            "Worker_jobs %s: %s %s"
-                            % (self.dev.name, func, args),
+                            f"Worker_jobs {self.dev.name}: "
+                            f"{func} "
+                            f"{args}",
                             self.debug_color,
                         )
                     else:
                         tprint(
-                            "Worker_jobs %s: %s %s"
-                            % (self.dev.name, func.__name__, args),
+                            f"Worker_jobs {self.dev.name}: "
+                            f"{func.__name__} "
+                            f"{args}",
                             self.debug_color,
                         )
 
                 if self.jobs_function is None:
                     # Default job processing:
                     # Send I/O operation to the device
                     try:
                         func(*args)
                     except Exception as err:  # pylint: disable=broad-except
                         pft(err)
                         dprint(
-                            "@ Worker_jobs %s\n" % self.dev.name,
+                            f"@ Worker_jobs {self.dev.name}\n",
                             ANSI.RED,
                         )
                 else:
                     # User-supplied job processing
                     self.jobs_function(func, args)
 
             # Put sentinel back in
             self._queue.put(self._sentinel)
 
         if self.debug:
             tprint(
-                "Worker_jobs %s: unlock # %i"
-                % (self.dev.name, self.qdev.update_counter_jobs),
+                f"Worker_jobs {self.dev.name}: "
+                f"unlock # {self.qdev.update_counter_jobs}",
                 self.debug_color,
             )
 
         locker.unlock()
         self.qdev.signal_jobs_updated.emit()
 
     @Slot()
     def _stop(self):
         """Stop the worker to prepare for quitting the worker thread"""
         if self.debug:
             tprint(
-                "Worker_jobs %s: stopping" % self.dev.name,
+                f"Worker_jobs {self.dev.name}: stopping",
                 self.debug_color,
             )
 
         self._running = False
         self._qwc.wakeAll()  # Wake up for the final time
 
     # ----------------------------------------------------------------------
@@ -1699,27 +1697,27 @@
     # ----------------------------------------------------------------------
 
     def add_to_queue(self, instruction, pass_args=()):
         """See the description at :meth:`QDeviceIO.add_to_jobs_queue`.
 
         This method can be called from another thread.
         """
-        if type(pass_args) is not tuple:
+        if not isinstance(pass_args, tuple):
             pass_args = (pass_args,)
         self._queue.put((instruction, *pass_args))
 
     # ----------------------------------------------------------------------
     #   process_queue
     # ----------------------------------------------------------------------
 
     def process_queue(self):
         """See the description at :meth:`QDeviceIO.process_jobs_queue`.
 
         This method can be called from another thread.
         """
         if self.debug:
             tprint(
-                "Worker_jobs %s: wake-up requested..." % self.dev.name,
+                f"Worker_jobs {self.dev.name}: wake-up requested...",
                 ANSI.WHITE,
             )
 
         self._qwc.wakeAll()
```

### Comparing `dvg-qdeviceio-1.2.0/tests/test_dvg_qdeviceio.py` & `dvg-qdeviceio-1.3.0/tests/test_dvg_qdeviceio.py`

 * *Files 7% similar despite different names*

```diff
@@ -697,65 +697,27 @@
 
 
 # ------------------------------------------------------------------------------
 # ------------------------------------------------------------------------------
 
 
 if __name__ == "__main__":
-    ALL = True
-    if ALL:
-        test_Worker_DAQ___INTERNAL_TIMER()
-        test_Worker_DAQ___INTERNAL_TIMER__start_dead()
-        test_Worker_DAQ___SINGLE_SHOT_WAKE_UP()
-        test_Worker_DAQ___SINGLE_SHOT_WAKE_UP__start_dead()
-        test_Worker_DAQ___CONTINUOUS()
-        test_Worker_DAQ___CONTINUOUS__start_dead()
-        test_Worker_jobs()
-        test_Worker_jobs__start_dead()
-        test_Worker_jobs__jobs_function()
-        test_attach_device_twice()
-        test_Worker_DAQ___no_device_attached()
-        test_Worker_jobs__no_device_attached()
-        test_Worker_DAQ___start_without_create()
-        test_Worker_jobs__start_without_create()
-        test_Worker_DAQ___quit_without_start()
-        test_Worker_jobs__quit_without_start()
-        test_Worker_DAQ___rate()
-        test_Worker_DAQ___lose_connection()
-        test_Worker_DAQ___INTERNAL_TIMER__subclassed()
-        test_Worker_DAQ___ILLEGAL_DAQ_FUNCTION()
-    else:
-        # test_Worker_DAQ___INTERNAL_TIMER()
-        # test_Worker_DAQ___INTERNAL_TIMER__start_dead()
-        # test_Worker_DAQ___SINGLE_SHOT_WAKE_UP()
-        # test_Worker_DAQ___SINGLE_SHOT_WAKE_UP__start_dead()
-
-        """
-        import msvcrt
-        while True:
-            test_Worker_DAQ___CONTINUOUS()
-            if msvcrt.kbhit() and msvcrt.getch() == chr(27).encode():
-                break
-        """
-
-        test_Worker_DAQ___CONTINUOUS()
-        # test_Worker_DAQ___CONTINUOUS__start_dead()
-
-        # test_Worker_DAQ___rate()
-        # test_Worker_DAQ___lose_connection()
-        # test_Worker_DAQ___no_device_attached()
-        # test_Worker_DAQ___start_without_create()
-
-        # test_Worker_jobs()
-        # test_Worker_jobs__start_dead()
-        # test_Worker_jobs__jobs_function()
-        # test_Worker_jobs__no_device_attached()
-        # test_Worker_jobs__start_without_create()
-
-        # test_Worker_DAQ___quit_without_start()
-        # test_Worker_jobs__quit_without_start()
-
-        # test_attach_device_twice()
-
-        # test_Worker_DAQ___INTERNAL_TIMER__subclassed()
-        # test_Worker_DAQ___lose_connection()
-        # test_Worker_DAQ___ILLEGAL_DAQ_FUNCTION()
+    test_Worker_DAQ___INTERNAL_TIMER()
+    test_Worker_DAQ___INTERNAL_TIMER__start_dead()
+    test_Worker_DAQ___SINGLE_SHOT_WAKE_UP()
+    test_Worker_DAQ___SINGLE_SHOT_WAKE_UP__start_dead()
+    test_Worker_DAQ___CONTINUOUS()
+    test_Worker_DAQ___CONTINUOUS__start_dead()
+    test_Worker_jobs()
+    test_Worker_jobs__start_dead()
+    test_Worker_jobs__jobs_function()
+    test_attach_device_twice()
+    test_Worker_DAQ___no_device_attached()
+    test_Worker_jobs__no_device_attached()
+    test_Worker_DAQ___start_without_create()
+    test_Worker_jobs__start_without_create()
+    test_Worker_DAQ___quit_without_start()
+    test_Worker_jobs__quit_without_start()
+    test_Worker_DAQ___rate()
+    test_Worker_DAQ___lose_connection()
+    test_Worker_DAQ___INTERNAL_TIMER__subclassed()
+    test_Worker_DAQ___ILLEGAL_DAQ_FUNCTION()
```

