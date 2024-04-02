# Comparing `tmp/delayed_rm-2.8.1.tar.gz` & `tmp/delayed_rm-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delayed_rm-2.8.1.tar", last modified: Sun Mar 10 21:20:38 2024, max compression
+gzip compressed data, was "delayed_rm-2.8.2.tar", last modified: Tue Apr  2 09:18:21 2024, max compression
```

## Comparing `delayed_rm-2.8.1.tar` & `delayed_rm-2.8.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:20:38.927302 delayed_rm-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-10 21:20:34.000000 delayed_rm-2.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-10 21:20:38.927302 delayed_rm-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-10 21:20:34.000000 delayed_rm-2.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:20:38.927302 delayed_rm-2.8.1/delayed_rm/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-10 21:20:34.000000 delayed_rm-2.8.1/delayed_rm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-03-10 21:20:34.000000 delayed_rm-2.8.1/delayed_rm/delayed_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-10 21:20:34.000000 delayed_rm-2.8.1/delayed_rm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:20:38.927302 delayed_rm-2.8.1/delayed_rm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-10 21:20:38.000000 delayed_rm-2.8.1/delayed_rm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-10 21:20:38.000000 delayed_rm-2.8.1/delayed_rm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 21:20:38.000000 delayed_rm-2.8.1/delayed_rm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-10 21:20:38.000000 delayed_rm-2.8.1/delayed_rm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-10 21:20:38.000000 delayed_rm-2.8.1/delayed_rm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-10 21:20:34.000000 delayed_rm-2.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 21:20:38.927302 delayed_rm-2.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:18:21.883568 delayed_rm-2.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 09:18:15.000000 delayed_rm-2.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-02 09:18:21.879567 delayed_rm-2.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-02 09:18:15.000000 delayed_rm-2.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:18:21.879567 delayed_rm-2.8.2/delayed_rm/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-02 09:18:15.000000 delayed_rm-2.8.2/delayed_rm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-04-02 09:18:15.000000 delayed_rm-2.8.2/delayed_rm/delayed_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 09:18:15.000000 delayed_rm-2.8.2/delayed_rm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:18:21.879567 delayed_rm-2.8.2/delayed_rm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-02 09:18:21.000000 delayed_rm-2.8.2/delayed_rm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-02 09:18:21.000000 delayed_rm-2.8.2/delayed_rm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:18:21.000000 delayed_rm-2.8.2/delayed_rm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 09:18:21.000000 delayed_rm-2.8.2/delayed_rm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 09:18:21.000000 delayed_rm-2.8.2/delayed_rm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-02 09:18:15.000000 delayed_rm-2.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:18:21.883568 delayed_rm-2.8.2/setup.cfg
```

### Comparing `delayed_rm-2.8.1/LICENSE` & `delayed_rm-2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `delayed_rm-2.8.1/PKG-INFO` & `delayed_rm-2.8.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: delayed_rm
-Version: 2.8.1
+Version: 2.8.2
 Summary: Ever wish you had a few minutes to undo an rm? Now you do!
-License: GPL
+License: GPLv3
 Project-URL: Homepage, https://github.com/zwimer/delayed_rm
+Keywords: rm
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # delayed\_rm
 Ever wish you had a few minutes to undo an rm? Now you do!
```

### Comparing `delayed_rm-2.8.1/delayed_rm/delayed_rm.py` & `delayed_rm-2.8.2/delayed_rm/delayed_rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import tempfile
 import shutil
 import time
 import sys
 import os
 
 
-__version__ = "2.8.1"
+__version__ = "2.8.2"
 
 
 #
 # Config
 #
 
 
@@ -39,15 +39,15 @@
 class _Secret:
     """
     Contains a string needed to activate the secret CLI
     Users should *not* use this, it is an internal class!
     """
 
     key: str = "DELAYED_RM_SECRET_CLI"
-    value: str = "cL5r0!L4hmWmonW7k^RZM*4nq7mR&yfF"
+    value: str = "--:://'cL5r0!L4hmWmonW7k^RZM*4nq7mR&yfF"
 
 
 #
 # Functions
 #
 
 
@@ -110,16 +110,18 @@
     """
     Move paths to a temprary directory, delete them after delay seconds
     Log's this action to the log
     If rf, acts like rm -rf
     May raise an RMError if something goes wrong
     :returns: True on success, else False
     """
-    assert tmp_d.parent.exists(), "Temp dir enclosing directory does not exist"
-    assert log_f.parent.exists(), "Log file enclosing directory does not exist"
+    if not tmp_d.parent.exists():
+        raise RuntimeError("Temp dir enclosing directory does not exist")
+    if not log_f.parent.exists():
+        raise RuntimeError("Log file enclosing directory does not exist")
     # Prep
     paths = _prep(paths, rf)
     base = Path(tempfile.mkdtemp(dir=tmp_d))
     base.chmod(0o700)
     # Init data structures
     success: list[Path] = []
     failed: list[Path] = []
@@ -189,15 +191,15 @@
     except OSError:
         print(msg)
         raise
     # Delay rm and die
     if not edited:
         shutil.rmtree(base)
     else:
-        subprocess.Popen(  # pylint: disable=consider-using-with
+        subprocess.Popen(  # pylint: disable=consider-using-with # nosec B603
             (sys.executable, __file__, _Secret.value, str(delay), base),
             env={_Secret.key: _Secret.value},
             stdout=subprocess.DEVNULL,
             stderr=subprocess.DEVNULL,
         )
     return not failed and not ctrlc
```

### Comparing `delayed_rm-2.8.1/delayed_rm.egg-info/PKG-INFO` & `delayed_rm-2.8.2/delayed_rm.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: delayed_rm
-Version: 2.8.1
+Version: 2.8.2
 Summary: Ever wish you had a few minutes to undo an rm? Now you do!
-License: GPL
+License: GPLv3
 Project-URL: Homepage, https://github.com/zwimer/delayed_rm
+Keywords: rm
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # delayed\_rm
 Ever wish you had a few minutes to undo an rm? Now you do!
```

### Comparing `delayed_rm-2.8.1/pyproject.toml` & `delayed_rm-2.8.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "delayed_rm"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
+    "Development Status :: 5 - Production/Stable",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
-license = {text = "GPL"}
+keywords = ["rm"]
+license = {text = "GPLv3"}
 description = "Ever wish you had a few minutes to undo an rm? Now you do!"
 urls = {Homepage = "https://github.com/zwimer/delayed_rm"}
 requires-python = ">= 3.10"
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
@@ -34,14 +37,21 @@
 [tool.setuptools.dynamic]
 version = {attr = "delayed_rm.__version__"}
 
 # Tools
 
 [tool.black]
 line-length = 120
-target-version = ["py310"]
+target-version = ["py310", "py311", "py312"]
 
 [tool.ruff]
 ignore=["E731","E741"]
 line-length = 120
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "F403"]
+
+[tool.bandit]
+skips = ["B404"]
+
+[tool.vulture]
+ignore_names = ["cli"]
+paths = ["delayed_rm"]
```

