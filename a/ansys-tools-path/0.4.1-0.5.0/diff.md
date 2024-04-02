# Comparing `tmp/ansys_tools_path-0.4.1.tar.gz` & `tmp/ansys_tools_path-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_tools_path-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_tools_path-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_tools_path-0.4.1.tar` & `ansys_tools_path-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0     1089 2024-01-05 08:02:14.179157 ansys_tools_path-0.4.1/LICENSE
--rw-r--r--   0        0        0     4692 2024-01-05 08:02:14.179157 ansys_tools_path-0.4.1/README.rst
--rw-r--r--   0        0        0     1981 2024-01-05 08:02:14.183157 ansys_tools_path-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1631 2024-01-05 08:02:14.183157 ansys_tools_path-0.4.1/src/ansys/tools/path/__init__.py
--rw-r--r--   0        0        0      677 2024-01-05 08:02:14.183157 ansys_tools_path-0.4.1/src/ansys/tools/path/misc.py
--rw-r--r--   0        0        0    38233 2024-01-05 08:02:14.183157 ansys_tools_path-0.4.1/src/ansys/tools/path/path.py
--rw-r--r--   0        0        0        0 2024-01-05 08:02:14.183157 ansys_tools_path-0.4.1/src/ansys/tools/path/py.typed
--rw-r--r--   0        0        0     1971 2024-01-05 08:02:14.183157 ansys_tools_path-0.4.1/src/ansys/tools/path/save.py
--rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 ansys_tools_path-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-02 12:18:23.631993 ansys_tools_path-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4692 2024-04-02 12:18:23.635993 ansys_tools_path-0.5.0/README.rst
+-rw-r--r--   0        0        0     1981 2024-04-02 12:18:23.635993 ansys_tools_path-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1631 2024-04-02 12:18:23.635993 ansys_tools_path-0.5.0/src/ansys/tools/path/__init__.py
+-rw-r--r--   0        0        0      297 2024-04-02 12:18:23.635993 ansys_tools_path-0.5.0/src/ansys/tools/path/applications/__init__.py
+-rw-r--r--   0        0        0     1298 2024-04-02 12:18:23.635993 ansys_tools_path-0.5.0/src/ansys/tools/path/applications/dyna.py
+-rw-r--r--   0        0        0     1417 2024-04-02 12:18:23.635993 ansys_tools_path-0.5.0/src/ansys/tools/path/applications/mapdl.py
+-rw-r--r--   0        0        0     1726 2024-04-02 12:18:23.635993 ansys_tools_path-0.5.0/src/ansys/tools/path/applications/mechanical.py
+-rw-r--r--   0        0        0      677 2024-04-02 12:18:23.635993 ansys_tools_path-0.5.0/src/ansys/tools/path/misc.py
+-rw-r--r--   0        0        0    37880 2024-04-02 12:18:23.635993 ansys_tools_path-0.5.0/src/ansys/tools/path/path.py
+-rw-r--r--   0        0        0        0 2024-04-02 12:18:23.635993 ansys_tools_path-0.5.0/src/ansys/tools/path/py.typed
+-rw-r--r--   0        0        0     1971 2024-04-02 12:18:23.635993 ansys_tools_path-0.5.0/src/ansys/tools/path/save.py
+-rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 ansys_tools_path-0.5.0/PKG-INFO
```

### Comparing `ansys_tools_path-0.4.1/LICENSE` & `ansys_tools_path-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.4.1/README.rst` & `ansys_tools_path-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.4.1/pyproject.toml` & `ansys_tools_path-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-tools-path"
-version = "0.4.1"
+version = "0.5.0"
 description = "Library to locate Ansys products in a local machine."
 readme = "README.rst"
 requires-python = ">=3.8,<4"
 license = { file = "LICENSE" }
 authors = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 maintainers = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 
@@ -25,24 +25,24 @@
 dependencies = [
     "platformdirs>=3.6.0",
     "click>=8.1.3",        # for CLI interface
 ]
 
 
 [project.optional-dependencies]
-tests = ["pytest==7.4.4", "pytest-cov==4.1.0", "pyfakefs==5.3.2"]
+tests = ["pytest==8.1.1", "pytest-cov==5.0.0", "pyfakefs==5.3.5"]
 
 doc = [
     "Sphinx==7.2.6",
-    "numpydoc==1.6.0",
-    "ansys-sphinx-theme==0.13.0",
+    "numpydoc==1.7.0",
+    "ansys-sphinx-theme==0.15.0",
     "sphinx-copybutton==0.5.2",
 ]
 
-build = ["build==1.0.3", "twine==4.0.2"]
+build = ["build==1.2.1", "twine==5.0.0"]
 
 [tool.flit.module]
 name = "ansys.tools.path"
 
 [project.scripts]
 save-ansys-path = "ansys.tools.path.save:cli"
```

### Comparing `ansys_tools_path-0.4.1/src/ansys/tools/path/__init__.py` & `ansys_tools_path-0.5.0/src/ansys/tools/path/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.4.1/src/ansys/tools/path/misc.py` & `ansys_tools_path-0.5.0/src/ansys/tools/path/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.4.1/src/ansys/tools/path/path.py` & `ansys_tools_path-0.5.0/src/ansys/tools/path/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 import os
 import re
 from typing import Callable, Dict, Literal, Optional, Tuple, Union, cast
 import warnings
 
 import platformdirs
 
+from ansys.tools.path.applications import ApplicationPlugin, dyna, mapdl, mechanical
 from ansys.tools.path.misc import is_float, is_linux, is_windows
 
+PLUGINS: Dict[str, ApplicationPlugin] = {"mechanical": mechanical, "dyna": dyna, "mapdl": mapdl}
+
 LOG = logging.getLogger(__name__)
 
-PRODUCT_TYPE = Literal["mapdl", "mechanical"]
+PRODUCT_TYPE = Literal["mapdl", "mechanical", "dyna"]
 SUPPORTED_VERSIONS_TYPE = Dict[int, str]
 
 LINUX_DEFAULT_DIRS = [["/", "usr", "ansys_inc"], ["/", "ansys_inc"], ["/", "install", "ansys_inc"]]
 LINUX_DEFAULT_DIRS = [os.path.join(*each) for each in LINUX_DEFAULT_DIRS]
 
 CONFIG_FILE_NAME = "config.txt"
 
@@ -405,18 +408,19 @@
         ansys_bin = os.path.join(ans_path, "ansys", "bin", "winx64", f"LSDYNA{version}.exe")
     else:
         ansys_bin = os.path.join(ans_path, "ansys", "bin", f"lsdyna{version}")
     return ansys_bin, int(version) / 10
 
 
 def _find_installation(
-    product: PRODUCT_TYPE,
+    product: str,
     version: Optional[float] = None,
     supported_versions: SUPPORTED_VERSIONS_TYPE = SUPPORTED_ANSYS_VERSIONS,
 ) -> Union[Tuple[str, float], Tuple[Literal[""], Literal[""]]]:
+
     if product == "mapdl":
         return find_mapdl(version, supported_versions)
     elif product == "mechanical":
         return find_mechanical(version, supported_versions)
     elif product == "dyna":
         return find_dyna(version, supported_versions)
     raise Exception("unexpected product")
@@ -431,37 +435,20 @@
         "This method is going to be deprecated in future versions. Please use 'find_mapdl'.",
         category=DeprecationWarning,
     )
 
     return _find_installation("mapdl", version, supported_versions)
 
 
+def _has_plugin(product: str) -> bool:
+    return product in PLUGINS
+
+
 def is_valid_executable_path(product: PRODUCT_TYPE, exe_loc: str) -> bool:
-    if product == "mapdl":
-        return (
-            os.path.isfile(exe_loc)
-            and re.search(r"ansys\d\d\d", os.path.basename(os.path.normpath(exe_loc))) is not None
-        )
-    elif product == "dyna":
-        # dyna executable paths could be anything, really
-        return True
-    elif product == "mechanical":
-        if is_windows():  # pragma: no cover
-            return (
-                os.path.isfile(exe_loc)
-                and re.search(
-                    "AnsysWBU.exe", os.path.basename(os.path.normpath(exe_loc)), re.IGNORECASE
-                )
-                is not None
-            )
-        return (
-            os.path.isfile(exe_loc)
-            and re.search(".workbench", os.path.basename(os.path.normpath(exe_loc))) is not None
-        )
-    raise Exception("unexpected application")
+    return PLUGINS[product].is_valid_executable_path(exe_loc)
 
 
 def _is_common_executable_path(product: PRODUCT_TYPE, exe_loc: str) -> bool:
     if product == "mapdl":
         path = os.path.normpath(exe_loc)
         path = path.split(os.sep)
         # Look for all v(\d\d\d) to catch the last one
@@ -501,18 +488,18 @@
             and "aisol" in path
             and ".workbench" in path
         )
     else:
         raise Exception("unexpected application")
 
 
-def _change_default_path(product: PRODUCT_TYPE, exe_loc: str) -> None:
+def _change_default_path(application: str, exe_loc: str) -> None:
     if os.path.isfile(exe_loc):
         config_data = _read_config_file()
-        config_data[product] = exe_loc
+        config_data[application] = exe_loc
         _write_config_file(config_data)
     else:
         raise FileNotFoundError("File %s is invalid or does not exist" % exe_loc)
 
 
 def change_default_mapdl_path(exe_loc: str) -> None:
     """Change your default Ansys MAPDL path.
@@ -605,25 +592,24 @@
 
     _change_default_path("mapdl", exe_loc)
 
 
 def _save_path(
     product: PRODUCT_TYPE, exe_loc: Optional[str] = None, allow_prompt: bool = True
 ) -> str:
-    if exe_loc is None:
+    has_plugin = _has_plugin(product)
+    if exe_loc is None and has_plugin:
         exe_loc, _ = _find_installation(product)
-
-    if is_valid_executable_path(product, exe_loc):
-        _check_uncommon_executable_path(product, exe_loc)
-
-        _change_default_path(product, exe_loc)
-        return exe_loc
-
-    if allow_prompt:
+    if exe_loc == "" and allow_prompt:
         exe_loc = _prompt_path(product)  # pragma: no cover
+
+    if has_plugin:
+        if is_valid_executable_path(product, exe_loc):
+            _check_uncommon_executable_path(product, exe_loc)
+    _change_default_path(product, exe_loc)
     return exe_loc
 
 
 def save_mechanical_path(
     exe_loc: Optional[str] = None, allow_prompt: bool = True
 ) -> str:  # pragma: no cover
     """Find the Mechanical path or query user.
@@ -945,25 +931,27 @@
 def _read_executable_path_from_config_file(product_name: PRODUCT_TYPE) -> Optional[str]:
     """Read the executable path for the product given by `product_name` from config file"""
     config_data = _read_config_file()
     return config_data.get(product_name, None)
 
 
 def _get_application_path(
-    product: PRODUCT_TYPE,
+    product: str,
     allow_input: bool = True,
     version: Optional[float] = None,
     find: bool = True,
 ) -> Optional[str]:
     if version is None:
         exe_loc = _read_executable_path_from_config_file(product)
         if exe_loc is not None:
             return exe_loc
 
     LOG.debug(f"{product} path not found in config file")
+    if not _has_plugin(product):
+        raise Exception(f"Application {product} not registered.")
 
     if find:
         try:
             exe_loc, exe_version = _find_installation(product, version)
             if (exe_loc, exe_version) != ("", ""):  # executable not found
                 if os.path.isfile(exe_loc):
                     return exe_loc
```

### Comparing `ansys_tools_path-0.4.1/src/ansys/tools/path/save.py` & `ansys_tools_path-0.5.0/src/ansys/tools/path/save.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.4.1/PKG-INFO` & `ansys_tools_path-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: ansys-tools-path
-Version: 0.4.1
+Version: 0.5.0
 Summary: Library to locate Ansys products in a local machine.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: platformdirs>=3.6.0
 Requires-Dist: click>=8.1.3
-Requires-Dist: build==1.0.3 ; extra == "build"
-Requires-Dist: twine==4.0.2 ; extra == "build"
+Requires-Dist: build==1.2.1 ; extra == "build"
+Requires-Dist: twine==5.0.0 ; extra == "build"
 Requires-Dist: Sphinx==7.2.6 ; extra == "doc"
-Requires-Dist: numpydoc==1.6.0 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.13.0 ; extra == "doc"
+Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.15.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
-Requires-Dist: pytest==7.4.4 ; extra == "tests"
-Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
-Requires-Dist: pyfakefs==5.3.2 ; extra == "tests"
+Requires-Dist: pytest==8.1.1 ; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
+Requires-Dist: pyfakefs==5.3.5 ; extra == "tests"
 Project-URL: Documentation, https://path.tools.docs.pyansys.com
 Project-URL: Homepage, https://github.com/ansys/ansys-tools-path
 Project-URL: Source, https://github.com/ansys/ansys-tools-path
 Project-URL: Tracker, https://github.com/ansys/ansys-tools-path/issues
 Provides-Extra: build
 Provides-Extra: doc
 Provides-Extra: tests
```

