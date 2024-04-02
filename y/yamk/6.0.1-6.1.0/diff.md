# Comparing `tmp/yamk-6.0.1.tar.gz` & `tmp/yamk-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamk-6.0.1.tar", max compression
+gzip compressed data, was "yamk-6.1.0.tar", max compression
```

## Comparing `yamk-6.0.1.tar` & `yamk-6.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2836 2024-01-03 22:37:04.548545 yamk-6.0.1/docs/README.md
--rw-r--r--   0        0        0     3106 2024-03-31 00:22:50.569597 yamk-6.0.1/pyproject.toml
--rw-r--r--   0        0        0       70 2024-03-31 00:22:57.251493 yamk-6.0.1/src/yamk/__init__.py
--rw-r--r--   0        0        0     3942 2024-02-02 16:31:24.557219 yamk-6.0.1/src/yamk/functions.py
--rw-r--r--   0        0        0    14899 2024-03-30 17:50:42.073390 yamk-6.0.1/src/yamk/lib.py
--rw-r--r--   0        0        0     3006 2023-10-18 12:01:10.428210 yamk-6.0.1/src/yamk/main.py
--rw-r--r--   0        0        0    11152 2024-03-28 16:45:20.274356 yamk-6.0.1/src/yamk/make.py
--rw-r--r--   0        0        0        0 2023-10-18 12:01:10.428210 yamk-6.0.1/src/yamk/py.typed
--rw-r--r--   0        0        0       79 2023-10-18 12:01:10.428210 yamk-6.0.1/src/yamk/types.py
--rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 yamk-6.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2836 2024-01-03 22:37:04.548545 yamk-6.1.0/docs/README.md
+-rw-r--r--   0        0        0     3086 2024-04-02 11:33:51.761680 yamk-6.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-02 11:33:53.284982 yamk-6.1.0/src/yamk/__init__.py
+-rw-r--r--   0        0        0     3942 2024-02-02 16:31:24.557219 yamk-6.1.0/src/yamk/functions.py
+-rw-r--r--   0        0        0    15347 2024-04-02 11:19:46.905445 yamk-6.1.0/src/yamk/lib.py
+-rw-r--r--   0        0        0     3006 2023-10-18 12:01:10.428210 yamk-6.1.0/src/yamk/main.py
+-rw-r--r--   0        0        0    11159 2024-04-02 11:22:17.639095 yamk-6.1.0/src/yamk/make.py
+-rw-r--r--   0        0        0        0 2023-10-18 12:01:10.428210 yamk-6.1.0/src/yamk/py.typed
+-rw-r--r--   0        0        0       79 2023-10-18 12:01:10.428210 yamk-6.1.0/src/yamk/types.py
+-rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 yamk-6.1.0/PKG-INFO
```

### Comparing `yamk-6.0.1/docs/README.md` & `yamk-6.1.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `yamk-6.0.1/pyproject.toml` & `yamk-6.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "yamk"
-version = "6.0.1"
+version = "6.1.0"
 description = "Yet another make"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "docs/README.md"
@@ -157,15 +157,14 @@
 
 [tool.poetry.dependencies]
 # python version
 python = "^3.8"
 
 # dependencies
 dj_settings = "^5.0"
-packaging = "^24.0"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = { version = "^0.13", python = "^3.10" }
 ipython = { version = "^8.21", python = "^3.10" }
 pickleshare = { version = "^0.7", python = "^3.10" }
 pipdeptree = "^2.13"
```

### Comparing `yamk-6.0.1/src/yamk/functions.py` & `yamk-6.1.0/src/yamk/functions.py`

 * *Files identical despite different names*

### Comparing `yamk-6.0.1/src/yamk/lib.py` & `yamk-6.1.0/src/yamk/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,14 +387,31 @@
             indicator,
             f"`{self.command}`",
             padding,
             f"{timing_colour}{timing}{ANSIEscape.ENDC}",
         )
 
 
+@dataclass(frozen=True, order=True)
+class Version:
+    major: int
+    minor: int
+    patch: int
+
+    @classmethod
+    def from_string(cls, version: str) -> Version:
+        version = re.sub("[^.0-9].*", "", version)
+        if version.endswith("."):
+            version += "0"
+        while version.count(".") < 2:
+            version += ".0"
+        major, minor, patch, *_ = map(int, version.split("."))
+        return cls(major, minor, patch)
+
+
 def flatten_vars(
     variables: dict[str, dict[str, Any]], base_dir: Path
 ) -> dict[str, Any]:
     order = [
         "env",
         "arg",
         "global",
```

### Comparing `yamk-6.0.1/src/yamk/main.py` & `yamk-6.1.0/src/yamk/main.py`

 * *Files identical despite different names*

### Comparing `yamk-6.0.1/src/yamk/make.py` & `yamk-6.1.0/src/yamk/make.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import re
 import subprocess
 import sys
 from time import perf_counter_ns, sleep
 from typing import Any, cast
 
 from dj_settings import ConfigParser
-from packaging.version import Version
 
 from yamk import __version__, lib
 
 
 class MakeCommand:
     def __init__(self, args: argparse.Namespace):
         self.verbosity = args.verbose
@@ -34,15 +33,15 @@
         cookbook = self.find_cookbook(args)
         self.base_dir = cookbook.parent
         self.phony_dir = self.base_dir.joinpath(".yamk")
         self.arg_vars = dict(var.split("=", maxsplit=1) for var in args.variables)
         parsed_cookbook = ConfigParser([cookbook], force_type=args.cookbook_type).data
         self.globals = parsed_cookbook.pop("$globals", {})
         self.version = self._get_version()
-        if self.version > __version__:
+        if self.version > lib.Version.from_string(__version__):
             msg = f"This cookbook requires an yamk >= v{self.version}"
             raise RuntimeError(msg)
         self.up_to_date = args.assume
         self._parse_recipes(parsed_cookbook)
         self.subprocess_kwargs = {
             "shell": True,
             "cwd": self.base_dir,
@@ -301,9 +300,9 @@
 
         if not recipe.keep_ts:
             msg = "Existence commands needs either exists_only or keep_ts"
             raise ValueError(msg)
 
         return path.stat().st_mtime
 
-    def _get_version(self) -> Version:
-        return Version(self.globals["version"])
+    def _get_version(self) -> lib.Version:
+        return lib.Version.from_string(self.globals["version"])
```

### Comparing `yamk-6.0.1/PKG-INFO` & `yamk-6.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamk
-Version: 6.0.1
+Version: 6.1.0
 Summary: Yet another make
 Home-page: https://yamk.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: make,build,cli
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.8,<4.0
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: dj_settings (>=5.0,<6.0)
-Requires-Dist: packaging (>=24.0,<25.0)
 Project-URL: Documentation, https://yamk.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/spapanik/yamk
 Description-Content-Type: text/markdown
 
 # yam: yet another make
 
 [![tests][test_badge]][test_url]
```

