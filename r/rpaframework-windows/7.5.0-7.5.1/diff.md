# Comparing `tmp/rpaframework_windows-7.5.0.tar.gz` & `tmp/rpaframework_windows-7.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpaframework_windows-7.5.0.tar", max compression
+gzip compressed data, was "rpaframework_windows-7.5.1.tar", max compression
```

## Comparing `rpaframework_windows-7.5.0.tar` & `rpaframework_windows-7.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11560 2022-09-28 13:20:32.845376 rpaframework_windows-7.5.0/LICENSE
--rw-r--r--   0        0        0     2248 2023-11-21 15:59:08.175478 rpaframework_windows-7.5.0/pyproject.toml
--rw-r--r--   0        0        0      290 2022-09-28 13:20:32.846376 rpaframework_windows-7.5.0/README.rst
--rw-r--r--   0        0        0    82663 2023-11-21 16:10:29.403295 rpaframework_windows-7.5.0/RPA_Windows.libspec
--rw-r--r--   0        0        0       79 2022-09-28 13:20:32.851374 rpaframework_windows-7.5.0/src/RPA/scripts/record.py
--rw-r--r--   0        0        0    23833 2023-11-21 11:22:40.557872 rpaframework_windows-7.5.0/src/RPA/Windows/__init__.py
--rw-r--r--   0        0        0       79 2022-09-28 13:20:32.848374 rpaframework_windows-7.5.0/src/RPA/Windows/__main__.py
--rw-r--r--   0        0        0      376 2023-04-07 16:40:03.787890 rpaframework_windows-7.5.0/src/RPA/Windows/keywords/__init__.py
--rw-r--r--   0        0        0    29224 2023-04-07 16:40:03.788888 rpaframework_windows-7.5.0/src/RPA/Windows/keywords/action.py
--rw-r--r--   0        0        0      311 2023-04-07 16:40:03.788888 rpaframework_windows-7.5.0/src/RPA/Windows/keywords/context.py
--rw-r--r--   0        0        0     6403 2023-04-07 16:40:03.788888 rpaframework_windows-7.5.0/src/RPA/Windows/keywords/elements.py
--rw-r--r--   0        0        0     9027 2023-10-31 06:40:38.055555 rpaframework_windows-7.5.0/src/RPA/Windows/keywords/locators.py
--rw-r--r--   0        0        0    14382 2023-11-21 15:59:08.176482 rpaframework_windows-7.5.0/src/RPA/Windows/keywords/window.py
--rw-r--r--   0        0        0     3277 2023-04-07 16:40:03.792891 rpaframework_windows-7.5.0/src/RPA/Windows/main.py
--rw-r--r--   0        0        0      759 2023-04-07 16:40:03.793893 rpaframework_windows-7.5.0/src/RPA/Windows/utils.py
--rw-r--r--   0        0        0     2071 1970-01-01 00:00:00.000000 rpaframework_windows-7.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11560 2023-12-05 08:21:31.492158 rpaframework_windows-7.5.1/LICENSE
+-rw-r--r--   0        0        0     2248 2024-04-02 11:37:38.995162 rpaframework_windows-7.5.1/pyproject.toml
+-rw-r--r--   0        0        0      290 2023-12-05 08:21:31.492663 rpaframework_windows-7.5.1/README.rst
+-rw-r--r--   0        0        0    82663 2024-04-02 11:39:01.147182 rpaframework_windows-7.5.1/RPA_Windows.libspec
+-rw-r--r--   0        0        0       79 2023-12-05 08:21:31.494207 rpaframework_windows-7.5.1/src/RPA/scripts/record.py
+-rw-r--r--   0        0        0    23833 2023-12-05 08:21:31.493195 rpaframework_windows-7.5.1/src/RPA/Windows/__init__.py
+-rw-r--r--   0        0        0       79 2023-12-05 08:21:31.493195 rpaframework_windows-7.5.1/src/RPA/Windows/__main__.py
+-rw-r--r--   0        0        0      376 2023-12-05 08:21:31.494207 rpaframework_windows-7.5.1/src/RPA/Windows/keywords/__init__.py
+-rw-r--r--   0        0        0    29224 2023-12-05 08:21:31.494207 rpaframework_windows-7.5.1/src/RPA/Windows/keywords/action.py
+-rw-r--r--   0        0        0      311 2023-12-05 08:21:31.494207 rpaframework_windows-7.5.1/src/RPA/Windows/keywords/context.py
+-rw-r--r--   0        0        0     6403 2023-12-05 08:21:31.494207 rpaframework_windows-7.5.1/src/RPA/Windows/keywords/elements.py
+-rw-r--r--   0        0        0     9027 2023-12-05 08:21:31.494207 rpaframework_windows-7.5.1/src/RPA/Windows/keywords/locators.py
+-rw-r--r--   0        0        0    14382 2023-12-05 08:21:31.494207 rpaframework_windows-7.5.1/src/RPA/Windows/keywords/window.py
+-rw-r--r--   0        0        0     3277 2023-12-05 08:21:31.494207 rpaframework_windows-7.5.1/src/RPA/Windows/main.py
+-rw-r--r--   0        0        0      759 2023-12-05 08:21:31.494207 rpaframework_windows-7.5.1/src/RPA/Windows/utils.py
+-rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 rpaframework_windows-7.5.1/PKG-INFO
```

### Comparing `rpaframework_windows-7.5.0/LICENSE` & `rpaframework_windows-7.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rpaframework_windows-7.5.0/pyproject.toml` & `rpaframework_windows-7.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpaframework-windows"
-version = "7.5.0"
+version = "7.5.1"
 description = "Windows library for RPA Framework"
 authors = ["RPA Framework <rpafw@robocorp.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 
 homepage = "https://rpaframework.org/"
 documentation = "https://rpaframework.org/"
@@ -28,15 +28,15 @@
 include = ["*.libspec"]
 
 packages = [{ include = "RPA", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dataclasses = { version = "^0.7", python = ">=3.6,<3.7" }
-rpaframework-core = "^11.3.0"
+rpaframework-core = "^11.3.1"
 robotframework = ">=4.0.0,!=4.0.1,!=6.1.0,<7.0.0"
 robotframework-pythonlibcore = "^4.2.0"
 pynput-robocorp-fork = "^5.0.0"
 uiautomation = "^2.0.15"
 comtypes = { version = "^1.1.11", platform = "win32" }
 psutil = { version = "^5.9.0", platform = "win32" }
 pywin32 = { version = ">=300,<307", platform = "win32", python = "!=3.8.1" }
```

### Comparing `rpaframework_windows-7.5.0/RPA_Windows.libspec` & `rpaframework_windows-7.5.1/RPA_Windows.libspec`

 * *Files 0% similar despite different names*

#### Comparing `rpaframework_windows-7.5.0/RPA_Windows.libspec` & `rpaframework_windows-7.5.1/RPA_Windows.libspec`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="RPA.Windows" type="LIBRARY" format="REST" scope="GLOBAL" generated="2023-11-21T16:10:29+00:00" specversion="5" source="./RPA/Windows/__init__.py" lineno="24">
+<keywordspec name="RPA.Windows" type="LIBRARY" format="REST" scope="GLOBAL" generated="2024-04-02T11:39:01+00:00" specversion="5" source="./RPA/Windows/__init__.py" lineno="24">
   <version/>
   <doc>The `Windows` is a library that can be used for Windows desktop automation.
 
 Library is included in the **rpaframework** package by default, but as shown in the
 below example library can be also installed separately without **rpaframework**.
 
 .. code-block:: yaml
@@ -1860,15 +1860,15 @@
     print(f&quot;Previous mouse simulation: {previous} (now enabled)&quot;)</doc>
       <shortdoc>Enable or disable mouse movement simulation during clicks and other actions.</shortdoc>
       <tags>
         <tag>action</tag>
       </tags>
     </kw>
     <kw name="Set Value" source="./RPA/Windows/keywords/action.py" lineno="438">
-      <arguments repr="locator: WindowsElement | str | None = None, value: str | None = None, append: bool = False, enter: bool = False, newline: bool = False, send_keys_fallback: bool = True, validator: Callable | None = &lt;function set_value_validator at 0x000001835A8F2670&gt;">
+      <arguments repr="locator: WindowsElement | str | None = None, value: str | None = None, append: bool = False, enter: bool = False, newline: bool = False, send_keys_fallback: bool = True, validator: Callable | None = &lt;function set_value_validator at 0x000002553037C0D0&gt;">
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="locator: WindowsElement | str | None = None">
           <name>locator</name>
           <type name="Union" union="true">
             WindowsElement | str | None
             <type name="WindowsElement">WindowsElement</type>
             <type name="str" typedoc="string">str</type>
             <type name="None" typedoc="None">None</type>
@@ -1900,22 +1900,22 @@
           <default>False</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="send_keys_fallback: bool = True">
           <name>send_keys_fallback</name>
           <type name="bool" typedoc="boolean">bool</type>
           <default>True</default>
         </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="validator: Callable | None = &lt;function set_value_validator at 0x000001835A8F2670&gt;">
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="validator: Callable | None = &lt;function set_value_validator at 0x000002553037C0D0&gt;">
           <name>validator</name>
           <type name="Union" union="true">
             Callable | None
             <type name="Callable">Callable</type>
             <type name="None" typedoc="None">None</type>
           </type>
-          <default>&lt;function set_value_validator at 0x000001835A8F2670&gt;</default>
+          <default>&lt;function set_value_validator at 0x000002553037C0D0&gt;</default>
         </arg>
       </arguments>
       <doc>Set value of the element defined by the locator.
 
 *Note:* An anchor will work only on element structures where you can
 rely on the stability of that root/child element tree, as remaining the same.
 Usually these kind of structures are tables. (but not restricted to)
```

### Comparing `rpaframework_windows-7.5.0/src/RPA/Windows/__init__.py` & `rpaframework_windows-7.5.1/src/RPA/Windows/__init__.py`

 * *Files identical despite different names*

### Comparing `rpaframework_windows-7.5.0/src/RPA/Windows/keywords/action.py` & `rpaframework_windows-7.5.1/src/RPA/Windows/keywords/action.py`

 * *Files identical despite different names*

### Comparing `rpaframework_windows-7.5.0/src/RPA/Windows/keywords/elements.py` & `rpaframework_windows-7.5.1/src/RPA/Windows/keywords/elements.py`

 * *Files identical despite different names*

### Comparing `rpaframework_windows-7.5.0/src/RPA/Windows/keywords/locators.py` & `rpaframework_windows-7.5.1/src/RPA/Windows/keywords/locators.py`

 * *Files identical despite different names*

### Comparing `rpaframework_windows-7.5.0/src/RPA/Windows/keywords/window.py` & `rpaframework_windows-7.5.1/src/RPA/Windows/keywords/window.py`

 * *Files identical despite different names*

### Comparing `rpaframework_windows-7.5.0/src/RPA/Windows/main.py` & `rpaframework_windows-7.5.1/src/RPA/Windows/main.py`

 * *Files identical despite different names*

### Comparing `rpaframework_windows-7.5.0/src/RPA/Windows/utils.py` & `rpaframework_windows-7.5.1/src/RPA/Windows/utils.py`

 * *Files identical despite different names*

### Comparing `rpaframework_windows-7.5.0/PKG-INFO` & `rpaframework_windows-7.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpaframework-windows
-Version: 7.5.0
+Version: 7.5.1
 Summary: Windows library for RPA Framework
 Home-page: https://rpaframework.org/
 License: Apache-2.0
 Keywords: robotframework,rpa,automation,windows,uiautomation
 Author: RPA Framework
 Author-email: rpafw@robocorp.com
 Requires-Python: >=3.8,<4.0
@@ -15,25 +15,26 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: comtypes (>=1.1.11,<2.0.0) ; sys_platform == "win32"
 Requires-Dist: dataclasses (>=0.7,<0.8) ; python_version >= "3.6" and python_version < "3.7"
 Requires-Dist: fire (>=0.4.0,<0.5.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0) ; sys_platform == "win32"
 Requires-Dist: pynput-robocorp-fork (>=5.0.0,<6.0.0)
 Requires-Dist: pywin32 (>=300,<307) ; python_full_version != "3.8.1" and sys_platform == "win32"
 Requires-Dist: robotframework (>=4.0.0,!=4.0.1,!=6.1.0,<7.0.0)
 Requires-Dist: robotframework-pythonlibcore (>=4.2.0,<5.0.0)
-Requires-Dist: rpaframework-core (>=11.3.0,<12.0.0)
+Requires-Dist: rpaframework-core (>=11.3.1,<12.0.0)
 Requires-Dist: uiautomation (>=2.0.15,<3.0.0)
 Project-URL: Documentation, https://rpaframework.org/
 Project-URL: Repository, https://github.com/robocorp/rpaframework
 Description-Content-Type: text/x-rst
 
 rpaframework-windows
 ====================
```

