# Comparing `tmp/cpop-28.1.2.tar.gz` & `tmp/cpop-28.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpop-28.1.2.tar", last modified: Mon Apr  1 23:17:17 2024, max compression
+gzip compressed data, was "cpop-28.2.0.tar", last modified: Tue Apr  2 15:22:13 2024, max compression
```

## Comparing `cpop-28.1.2.tar` & `cpop-28.2.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.689982 cpop-28.1.2/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.1.2/LICENSE
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      134 2024-04-01 21:10:23.000000 cpop-28.1.2/MANIFEST.in
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-01 23:17:17.689982 cpop-28.1.2/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4411 2024-04-01 23:16:48.000000 cpop-28.1.2/README.rst
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.685982 cpop-28.1.2/cpop.egg-info/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-01 23:17:17.000000 cpop-28.1.2/cpop.egg-info/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      562 2024-04-01 23:17:17.000000 cpop-28.1.2/cpop.egg-info/SOURCES.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-01 23:17:17.000000 cpop-28.1.2/cpop.egg-info/dependency_links.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-01 23:17:17.000000 cpop-28.1.2/cpop.egg-info/entry_points.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      136 2024-04-01 23:17:17.000000 cpop-28.1.2/cpop.egg-info/requires.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        8 2024-04-01 23:17:17.000000 cpop-28.1.2/cpop.egg-info/top_level.txt
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.685982 cpop-28.1.2/hub/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.1.2/hub/__init__.py
--rwxrwxr-x   0 akmod     (1000) akmod     (1000)     3111 2024-04-01 22:51:27.000000 cpop-28.1.2/hub/__main__.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.689982 cpop-28.1.2/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     2137 2024-04-01 23:13:39.000000 cpop-28.1.2/pop/config.yaml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    10888 2024-04-01 16:10:17.000000 cpop-28.1.2/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   870672 2024-04-01 21:05:40.000000 cpop-28.1.2/pop/data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4437 2024-04-01 21:12:29.000000 cpop-28.1.2/pop/dirs.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.1.2/pop/exc.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    21502 2024-04-01 22:51:27.000000 cpop-28.1.2/pop/hub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11789 2024-04-01 17:46:15.000000 cpop-28.1.2/pop/loader.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.689982 cpop-28.1.2/pop/log/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4750 2024-04-01 16:10:17.000000 cpop-28.1.2/pop/log/async.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      491 2024-04-01 16:10:17.000000 cpop-28.1.2/pop/log/init.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.685982 cpop-28.1.2/pop/mods/
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.689982 cpop-28.1.2/pop/mods/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6339 2024-04-01 23:12:04.000000 cpop-28.1.2/pop/mods/pop/config.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.1.2/pop/mods/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.1.2/pop/mods/pop/dyne.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6993 2024-04-01 22:18:05.000000 cpop-28.1.2/pop/mods/pop/sub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.1.2/pop/mods/pop/test.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-01 23:17:08.000000 cpop-28.1.2/pop/pop.data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 21:18:00.000000 cpop-28.1.2/pop/pop.data.pyx
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.1.2/pop/ref.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1321 2024-03-24 19:08:30.000000 cpop-28.1.2/pop/scanner.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.1.2/pop/verify.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1328 2024-04-01 23:14:36.000000 cpop-28.1.2/pyproject.toml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-01 23:17:17.689982 cpop-28.1.2/setup.cfg
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1263 2024-04-01 21:16:30.000000 cpop-28.1.2/setup.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.703872 cpop-28.2.0/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.2.0/LICENSE
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      134 2024-04-01 21:10:23.000000 cpop-28.2.0/MANIFEST.in
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-02 15:22:13.703872 cpop-28.2.0/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4411 2024-04-01 23:16:48.000000 cpop-28.2.0/README.rst
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.699872 cpop-28.2.0/cpop.egg-info/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-02 15:22:13.000000 cpop-28.2.0/cpop.egg-info/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      546 2024-04-02 15:22:13.000000 cpop-28.2.0/cpop.egg-info/SOURCES.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-02 15:22:13.000000 cpop-28.2.0/cpop.egg-info/dependency_links.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-02 15:22:13.000000 cpop-28.2.0/cpop.egg-info/entry_points.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      136 2024-04-02 15:22:13.000000 cpop-28.2.0/cpop.egg-info/requires.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        8 2024-04-02 15:22:13.000000 cpop-28.2.0/cpop.egg-info/top_level.txt
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.699872 cpop-28.2.0/hub/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.2.0/hub/__init__.py
+-rwxrwxr-x   0 akmod     (1000) akmod     (1000)     3185 2024-04-02 15:16:07.000000 cpop-28.2.0/hub/__main__.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.703872 cpop-28.2.0/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     2156 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/config.yaml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    10479 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   870672 2024-04-01 21:05:40.000000 cpop-28.2.0/pop/data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4417 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/dirs.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.2.0/pop/exc.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    23607 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/hub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11303 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/loader.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.703872 cpop-28.2.0/pop/log/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     5219 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/log/async.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.699872 cpop-28.2.0/pop/mods/
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.703872 cpop-28.2.0/pop/mods/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6339 2024-04-01 23:12:04.000000 cpop-28.2.0/pop/mods/pop/config.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.2.0/pop/mods/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.2.0/pop/mods/pop/dyne.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6993 2024-04-01 22:18:05.000000 cpop-28.2.0/pop/mods/pop/sub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.2.0/pop/mods/pop/test.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-02 15:17:57.000000 cpop-28.2.0/pop/pop.data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 21:18:00.000000 cpop-28.2.0/pop/pop.data.pyx
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.2.0/pop/ref.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1176 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/scanner.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.2.0/pop/verify.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1328 2024-04-02 15:17:28.000000 cpop-28.2.0/pyproject.toml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-02 15:22:13.707872 cpop-28.2.0/setup.cfg
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1263 2024-04-01 21:16:30.000000 cpop-28.2.0/setup.py
```

### Comparing `cpop-28.1.2/LICENSE` & `cpop-28.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpop-28.1.2/PKG-INFO` & `cpop-28.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.1.2
+Version: 28.2.0
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.1.2/README.rst` & `cpop-28.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-28.1.2/cpop.egg-info/PKG-INFO` & `cpop-28.2.0/cpop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.1.2
+Version: 28.2.0
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.1.2/cpop.egg-info/SOURCES.txt` & `cpop-28.2.0/cpop.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -20,13 +20,12 @@
 pop/loader.py
 pop/pop.data.c
 pop/pop.data.pyx
 pop/ref.py
 pop/scanner.py
 pop/verify.py
 pop/log/async.py
-pop/log/init.py
 pop/mods/pop/config.py
 pop/mods/pop/contract.py
 pop/mods/pop/dyne.py
 pop/mods/pop/sub.py
 pop/mods/pop/test.py
```

### Comparing `cpop-28.1.2/hub/__main__.py` & `cpop-28.2.0/hub/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,24 +12,25 @@
     # Manually retrieve the state using __getstate__
     state = hub.__getstate__()
     state_file.parent.mkdir(parents=True, exist_ok=True)
     with state_file.open("wb") as f:
         msgpack.dump(state, f)
 
 
-def load_hub_state(state_file: pathlib.Path):
+def load_hub_state(hub, state_file: pathlib.Path):
     if state_file.exists():
         try:
             with state_file.open("rb") as f:
                 state = msgpack.load(f)
         except:
             return
-
-        hub = pop.hub.Hub(**state["init_kwargs"])
-        return hub.__setstate__(state)
+        if hub._init_kwargs != state["init_kwargs"]:
+            hub.__init__(**state["init_kwargs"])
+        hub.__setstate__(state)
+        return hub
 
 
 def main():
     # Create the hub, loading all dynes and starting the loop
     hub = pop.hub.Hub(cli="pop_cli")
 
     args = []
@@ -37,28 +38,28 @@
 
     original_opt = hub.OPT
     ref = original_opt.pop_cli.ref
 
     # Try to get a saved hub
     if original_opt.pop_cli.hub_state:
         hub_state_file = pathlib.Path(original_opt.pop_cli.hub_state).expanduser()
-        new_hub = load_hub_state(hub_state_file)
+        new_hub = load_hub_state(hub, hub_state_file)
     else:
         hub_state_file = None
         new_hub = None
 
     # Successfully loaded a hub from a file
     if new_hub is not None:
         hub = new_hub
 
     # Override hub.OPT with the the new cli
     cli = original_opt.pop_cli.cli
     if cli:
         # Pass all remaining args onto the new parser
-        hub.OPT = hub._sync.pop.config.load(
+        hub._opt = hub._sync.pop.config.load(
             cli=cli, parser_args=original_opt.pop_cli.args
         )
     else:
         # We are using the pop cli, treat all the extra args as parameters for the called function
         PLACEHOLDER = object()
         hold = PLACEHOLDER
         for arg in original_opt.pop_cli.args:
```

### Comparing `cpop-28.1.2/pop/config.yaml` & `cpop-28.2.0/pop/config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     ref:
       default: ""
     cli:
       default: ""
     args:
       default: []
     hub_state:
-      default:
+      default: ~/.pop/hub.msgpack
   pop:
     config:
       default: ~/.pop/config.yaml
       os: POP_CONFIG
   log:
     log_plugin:
       default: async
```

### Comparing `cpop-28.1.2/pop/contract.py` & `cpop-28.2.0/pop/contract.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,39 +106,36 @@
         self,
         hub: "pop.hub.Hub",
         contracts: list["pop.hub.Sub"],
         func: functools.partial,
         ref: str,
         name: str,
         implicit_hub: bool = True,
-        param_aliases: dict = None,
     ):
         """
         :param hub: The redistributed pop central hub
         :param contracts: Contracts functions to add to the sub
         :param func: The contracted function to call
         :param ref: The reference to the function on the hub
         :param name: An alias for the function
         :param implicit_hub: True if a hub should be implicitly injected into the "call" method
-        :param param_aliases: A dictionary that maps parameters to a set of its aliases
         """
         self.__dict__.update(
             getattr(func, "__dict__", {})
         )  # do this first so we later overwrite any conflicts
         self.func = func
         self.ref = ref
         self.__name__ = name
         self.signature = inspect.signature(self.func)
         self._sig_errors = []
         self.__wrapped__ = func
         self.hub = hub
         self.contracts = contracts or []
         self.implicit_hub = implicit_hub
         self._load_contracts()
-        self.param_aliases = param_aliases or {}
 
     def _get_contracts_by_type(self, contract_type: str = "pre") -> list["Contracted"]:
         """
         :param contract_type: One of "call", "pre", "post", or "sig"
         """
         matches = []
         fn_contract_name = f"{contract_type}_{self.__name__}"
@@ -202,36 +199,26 @@
         if STRICT_TYPE_CHECKING:
             assert strict_return_checking(self, ret)
 
         return ret
 
     def __getstate__(self):
         return dict(
-            hub=self.hub,
             ref=self.ref,
             name=self.__name__,
             implicit_hub=self.implicit_hub,
             contracts=self.contracts,
-            param_aliases=self.param_aliases,
         )
 
     def __setstate__(self, state):
-        hub = state["hub"]
-        ref = state["ref"]
-        name = state["name"]
-        func = hub[ref][name].func
-        self.__init__(
-            hub=hub,
-            func=func,
-            ref=ref,
-            name=name,
-            implicit_hub=state["implicit_hub"],
-            contracts=state["contracts"],
-            param_aliases=state["param_aliases"],
-        )
+        self.ref = state["ref"]
+        self.name = state["name"]
+        self.func = self.hub[self.ref][self.name].func
+        self.implicit_hub = state["implicit_hub"]
+        self.contracts = state["contracts"]
 
 
 class ContractedAsyncGen(Contracted):
     async def __call__(self, *args, **kwargs):
         if self.implicit_hub:
             args = (self.hub,) + args
```

### Comparing `cpop-28.1.2/pop/data.c` & `cpop-28.2.0/pop/data.c`

 * *Files identical despite different names*

### Comparing `cpop-28.1.2/pop/dirs.py` & `cpop-28.2.0/pop/dirs.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,17 +49,14 @@
 
 
 def dynamic_dirs() -> dict[str, Any]:
     """
     Iterate over the available python package imports and look for configured
     dynamic dirs in pyproject.toml
     """
-
-    len(sys.path)
-
     dirs = set()
     for dir_ in sys.path:
         if not dir_:
             continue
         path = pathlib.Path(dir_)
         if not path.is_dir():
             continue
```

### Comparing `cpop-28.1.2/pop/exc.py` & `cpop-28.2.0/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.2/pop/hub.py` & `cpop-28.2.0/pop/hub.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 import asyncio
 import importlib.machinery
 import os
 import secrets
 import sys
 from collections.abc import Coroutine
+from collections.abc import Iterable
 from types import ModuleType
 from typing import Any
 
 import pop.contract
 import pop.data
 import pop.dirs
 import pop.exc
 import pop.loader
 import pop.ref
 import pop.scanner
 import pop.verify
 
+BASE_TYPES = (int, float, str, bytes, bool, type(None))
+
 
 def ex_path(path: str) -> list[str]:
     """
     Take a path that is sent to the Sub and expand it if it is a string or not
     """
     if isinstance(path, str):
         return path.split(",")
     elif isinstance(path, list):
         return path
     else:
         return []
 
 
 class PopMeta(pop.data.MultidictCache):
-    ...
+    def __init__(self, data: list[dict[str, any]]):
+        attrs = pop.data.NamespaceDict()
+        data.append(attrs)
+        super().__init__(data)
+        object.__setattr__(self, "_attrs", attrs)
+
+    def __setattr__(self, item: str, value):
+        if item.startswith("_"):
+            object.__setattr__(self, item, value)
+        else:
+            self._attrs[item] = value
 
 
 class SyncWrapper:
     """
     Enable synchronous calls to asynchronous hub references.
     I.e.:
 
@@ -75,14 +88,26 @@
 class Hub(PopMeta):
     """
     The redistributed pop central hub. All components of the system are
     rooted to the Hub.
     """
 
     def __init__(self, loop: asyncio.AbstractEventLoop = None, *args, **kwargs):
+        subs = pop.data.NamespaceDict()
+        sub_alias = pop.data.NamespaceDict()
+        imports = pop.data.NamespaceDict()
+        PopMeta.__init__(self, [subs, sub_alias, imports])
+        self._subs = subs
+        self._sub_alias = sub_alias
+        self._imports = imports
+        self._dynamic = None
+        self._dscan = False
+        # Set up the conf OPT structure so it is always available
+        self._opt = None
+
         # Initialize the loop
         if loop is None:
             self._loop = asyncio.new_event_loop()
         else:
             self._loop = loop
 
         asyncio.set_event_loop(self._loop)
@@ -97,22 +122,14 @@
         cli: str = None,
         logs: bool = True,
     ):
         self._init_kwargs = {
             k: v for k, v in locals().items() if k != "self" and not k.startswith("_")
         }
 
-        self._dynamic = None
-        self._dscan = False
-
-        self._subs = pop.data.NamespaceDict()
-        self._sub_alias = pop.data.NamespaceDict()
-        self._imports = pop.data.NamespaceDict()
-        super().__init__([self._subs, self._sub_alias, self._imports])
-
         # Add the dyne for python imports to live in to the hub
         self._subs["lib"] = await AsyncSub(
             self, subname="lib", dyne_name="lib", pypath=pop_mods
         )
         # Load all existing libraries onto hub.lib
         self._subs["lib"]._imports.update(
             {
@@ -127,31 +144,33 @@
 
         # Add the pop sub to the hub, this should always use pypath and
         # Should never be made dynamic. This is a core system sub and should
         # NOT be app-merged
         self._subs["pop"] = await AsyncSub(self, subname="pop", pypath=pop_mods)
         await self._subs["pop"]._load_all()
 
-        # Set up the conf OPT structure so it is always available
-        self.OPT = None
         self._sync = SyncWrapper(self)
 
         self._load_all_dynes = load_all_dynes
         self._load_all_subdirs = load_all_subdirs
         self._recurse_subdirs = recurse_subdirs
         if self._load_all_dynes:
             self._scan_dynamic()
             await self._load_all()
 
             # Overwrite opt with config data
-            self.OPT = await self.pop.config.load(cli=cli, **self._dynamic.config)
+            self._opt = await self.pop.config.load(cli=cli, **self._dynamic.config)
 
         # Set up a logger
         if logs:
-            await self.log[self.OPT.log.log_plugin].setup(self.OPT.log.copy())
+            await self.log[self._opt.log.log_plugin].setup(self._opt.log.copy())
+
+    @property
+    def OPT(self):
+        return self._opt
 
     async def _load_all(self):
         for base, imp in self._dynamic.imports.items():
             self._subs.lib._imports[base] = imp
 
         # Load all dynamic subs onto the hub
         for dyne in self._dynamic.dyne:
@@ -169,40 +188,54 @@
         Synchronous function to wait for a coroutine
         """
         while asyncio.iscoroutine(coroutine):
             coroutine = self._loop.run_until_complete(coroutine)
         return coroutine
 
     def __getstate__(self) -> dict:
+        attrs = {}
+        for k, v in self._attrs.items():
+            if isinstance(v, BASE_TYPES):
+                attrs[k] = v
+            elif isinstance(v, dict):
+                if all(isinstance(v2, BASE_TYPES) for v2 in v.values()):
+                    attrs[k] = v
+            elif isinstance(v, Iterable):
+                if all(isinstance(v2, BASE_TYPES) for v2 in v):
+                    attrs[k] = v
         return dict(
             init_kwargs=self._init_kwargs,
             subs={name: sub.__getstate__() for name, sub in self._subs.items()},
             aliases=self._sub_alias,
-            OPT=pop.data.unfreeze(self.OPT),
+            OPT=pop.data.unfreeze(self._opt),
             imports={subname: mod.__name__ for subname, mod in self._imports.items()},
+            attrs=attrs,
         )
 
     def __setstate__(self, state: dict):
         subs = state["subs"]
         opt = state["OPT"]
         aliases = state["aliases"]
-        # init_kwargs = state["init_kwargs"]
-        # self.__init__(**init_kwargs)
 
-        self._imports = {
-            subname: importlib.import_module(modname)
-            for subname, modname in state["imports"].items()
-        }
-        self._sub_alias = aliases
-        self.OPT = pop.data.freeze(opt)
+        for subname, modname in state["imports"].items():
+            try:
+                self._imports[subname] = importlib.import_module(modname)
+            except ModuleNotFoundError:
+                ...
+        self._attrs.update(state["attrs"])
+        self._sub_alias.update(aliases)
+        self._opt = pop.data.freeze(opt)
         for name, data in subs.items():
-            sub = Sub(hub=self, **data["init_kwargs"])
-            self._subs[name] = sub.__setstate__(data)
+            if name in self._subs:
+                sub = self._subs[name]
+            else:
+                sub = Sub(hub=self, **data["init_kwargs"])
+                self._subs[name] = sub
 
-        return self
+            sub.__setstate__(data)
 
     def _scan_dynamic(self):
         """
         Refresh the dynamic roots data used for loading app merge module roots
         """
         self._clear()
         self._dynamic = pop.dirs.dynamic_dirs()
@@ -270,30 +303,35 @@
         :param mod_basename: str: Manipulate the location in sys.modules that the plugin will be loaded to.
             Allow plugins to be loaded into a separate namespace.
         :param stop_on_failures: If any module fails to load for any reason, stacktrace and do not continue loading this sub
         :param init: bool: determine whether or not we process __init__ functions
         :param is_contract: Specify whether or not this sub is a contract
         :param sub_virtual: bool: Recursively ignore this sub and it's subs
         """
-        self._subs = pop.data.NamespaceDict()
-        self._alias = []
-        self._sub_alias = pop.data.NamespaceDict()
-        self._imports = pop.data.NamespaceDict()
-        self._loaded = pop.data.NamespaceDict()
-        # tracks what has been setattr-ed on this sub for performance; if something needs to be
-        # *removed*, we can delattr everything in _cached, it will be re-set on the next call.
-        super().__init__([self._loaded, self._subs, self._sub_alias, self._imports])
-        self._loaded_all = False
-        self._load_errors = pop.data.NamespaceDict()
-        self._vmap = pop.data.NamespaceDict()
         self._init_kwargs = {
             k: v
             for k, v in locals().items()
             if k not in ("self", "hub", "root") and not k.startswith("_")
         }
+        subs = pop.data.NamespaceDict()
+        sub_alias = pop.data.NamespaceDict()
+        imports = pop.data.NamespaceDict()
+        loaded = pop.data.NamespaceDict()
+        # tracks what has been setattr-ed on this sub for performance; if something needs to be
+        # *removed*, we can delattr everything in _cached, it will be re-set on the next call.
+        super().__init__([loaded, subs, sub_alias, imports])
+        self._subs = subs
+        self._sub_alias = sub_alias
+        self._imports = imports
+        self._loaded = loaded
+        self._reload_mods = pop.data.NamespaceDict()
+        self._alias = []
+        self._loaded_all = False
+        self._load_errors = pop.data.NamespaceDict()
+        self._vmap = pop.data.NamespaceDict()
         self._hub = hub
         self._root = root or hub
         self._subname = subname
         self._pypath = ex_path(pypath)
         self._static = ex_path(static)
         self._contracts_pypath = ex_path(contracts_pypath)
         self._contracts_static = ex_path(contracts_static)
@@ -396,51 +434,69 @@
         """
         if self._pypath:
             return self._pypath[0]
         elif self._dirs:
             return secrets.token_hex()
 
     def __getstate__(self):
+        attrs = {}
+        for k, v in self._attrs.items():
+            if isinstance(v, BASE_TYPES):
+                attrs[k] = v
+            elif isinstance(v, dict):
+                if all(isinstance(v2, BASE_TYPES) for v2 in v.values()):
+                    attrs[k] = v
+            elif isinstance(v, Iterable):
+                if all(isinstance(v2, BASE_TYPES) for v2 in v):
+                    attrs[k] = v
+
         return dict(
             init_kwargs=self._init_kwargs,
-            # TODO Make Loaded mod serializable
-            # loaded = self._loaded,
+            loaded={
+                item: dict(
+                    iface=iface, bname=bname, state=self._loaded[item].__getstate__()
+                )
+                for item, (iface, bname) in self._reload_mods.items()
+            },
             subs={name: sub.__getstate__() for name, sub in self._subs.items()},
             aliases=self._sub_alias,
             imports={subname: mod.__name__ for subname, mod in self._imports.items()},
+            attrs=attrs,
         )
 
     def __setstate__(self, state: dict):
         """
         Only a hub can truly restore a sub because of their interdependency
         """
         subs = state["subs"]
         aliases = state["aliases"]
         imports = state["imports"]
-        # loaded = state["loaded"]
-        # init_kwargs = state["init_kwargs"]
+        loaded = state["loaded"]
 
-        # self.__init__(**init_kwargs)
-        self._sub_alias = aliases
+        self._sub_alias.update(aliases)
+        self._attrs.update(state["attrs"])
 
-        self._imports = {
-            subname: importlib.import_module(modname)
-            for subname, modname in imports.items()
-        }
+        for subname, modname in imports.items():
+            try:
+                self._imports[subname] = importlib.import_module(modname)
+            except ModuleNotFoundError:
+                ...
 
         for name, data in subs.items():
             sub = Sub(hub=self._hub, **data["init_kwargs"])
-            self._subs[name] = sub.__setstate__(data)
+            sub.__setstate__(data)
+            self._subs[name] = sub
 
-        # TODO later it would be better to get all the serialized mods, for now just reload all
-        # for name, module in loaded.items():
-        #    ...
+        # Initialize the Sub
         self._hub._synchronize(self.__ainit__())
+        self._hub._synchronize(self._load_all())
 
-        return self
+        # Make sure all unique items make it back onto the loaded mod
+        for item, data in loaded.items():
+            self._loaded[item].__setstate__(data["state"])
 
     def __getattr__(self, item: str):
         """
         If the item should be loaded, load it, else serve it
         """
         if item.startswith("_"):
             return self.__getattribute__(item)
@@ -478,22 +534,24 @@
         :return a loaded mod_dict
         """
         for iface in self._scan:
             for bname in self._scan[iface]:
                 if os.path.basename(bname) == item:
                     await self._load_item(iface, bname)
             if item in self._loaded:
+                self._reload_mods[item] = (iface, bname)
                 return self._loaded[item]
         if not match_only:
             for iface in self._scan:
                 for bname in self._scan[iface]:
                     if self._scan[iface][bname].get("loaded"):
                         continue
                     await self._load_item(iface, bname)
                     if item in self._loaded:
+                        self._reload_mods[item] = (iface, bname)
                         return self._loaded[item]
         # Let's see if the module being lookup is in the load errors dictionary
         if item in self._load_errors:
             # Return the LoadError
             return self._load_errors[item]
 
     async def _load_item(self, iface: str, bname: str):
```

### Comparing `cpop-28.1.2/pop/loader.py` & `cpop-28.2.0/pop/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Load the files detected from the scanner
 """
 import asyncio
 import importlib.machinery
 import importlib.util
 import inspect
 import os
-import re
 import sys
 import types
 from collections.abc import Callable
 from typing import Any
 from typing import List
 
 import pop.contract
@@ -237,19 +236,19 @@
         name = func_alias
         if not this_sub._omit_vars:
             if (
                 not inspect.isfunction(func)
                 and not inspect.isclass(func)
                 and type(func).__name__ != "cython_function_or_method"
             ):
-                lmod._vars[name] = func
+                setattr(lmod, name, func)
                 continue
-        if attr.startswith(this_sub._omit_start):
+        if attr.startswith(tuple(this_sub._omit_start)):
             continue
-        if attr.endswith(this_sub._omit_end):
+        if attr.endswith(tuple(this_sub._omit_end)):
             continue
         if (
             inspect.isfunction(func)
             or inspect.isbuiltin(func)
             or type(func).__name__ == "cython_function_or_method"
         ):
             obj = pop.contract.create_contracted(
@@ -260,15 +259,14 @@
                 name,
             )
             if not this_sub._omit_func:
                 if this_sub._pypath and not func.__module__.startswith(mod.__name__):
                     # We're only interested in functions defined in this module, not
                     # imported functions
                     continue
-                check_param_alias(obj)
                 lmod._funcs[name] = obj
         else:
             klass = func
             if not this_sub._omit_class and inspect.isclass(klass):
                 # We're only interested in classes defined in this module, not
                 # imported classes
                 if not klass.__module__.startswith(mod.__name__):
@@ -284,62 +282,55 @@
                 func_alias,
                 ref,
                 attr,
                 implicit_hub=False,
             )
             lmod._funcs[attr] = obj
 
-    # Ensure that the __verify_order__ function exists on contract modules
-    verify_order: Callable = getattr(mod, "__verify_order__", lambda *_: True)
-    lmod.__verify_order__ = pop.contract.create_contracted(
-        this_sub._hub,
-        ordered_contracts,
-        verify_order,
-        ref,
-        attr,
-        implicit_hub=True,
-    )
-
     return lmod
 
 
-def check_param_alias(func: "pop.contract.Contracted"):
-    """
-    Verify that parameter aliases are unique
-    """
-    params_and_aliases = set(func.signature.parameters.keys())
-    for param, signature in func.signature.parameters.items():
-        match = re.findall(r"alias=(\w+)", str(signature.annotation))
-        for alias in match:
-            if alias in params_and_aliases:
-                raise SyntaxError(
-                    f"Multiple aliases or definitions of '{alias}' in '{func.ref}.{func.__name__}'"
-                )
-            else:
-                if param not in func.param_aliases:
-                    func.param_aliases[param] = {param}
-                func.param_aliases[param].add(alias)
-                params_and_aliases.add(alias)
-
-
 class LoadedMod(types.ModuleType):
     """
     The LoadedMod class allows for the module loaded onto the sub to return
     custom sequencing, for instance it can be iterated over to return all
     functions
     """
 
     def __init__(self, name: str):
         super().__init__(name)
-        self._vars = pop.data.NamespaceDict()
-        self._funcs = pop.data.NamespaceDict()
-        self._classes = pop.data.NamespaceDict()
-        self._attrs = pop.data.MultidictCache([self._vars, self._funcs, self._classes])
+        vars = pop.data.NamespaceDict()
+        funcs = pop.data.NamespaceDict()
+        classes = pop.data.NamespaceDict()
+        self._attrs = pop.data.MultidictCache([funcs, classes, vars])
+        self._vars = vars
+        self._funcs = funcs
+        self._classes = classes
 
     def __getattr__(self, item: str):
+        if item.startswith("_"):
+            return self.__getattribute__(item)
         try:
             return self._attrs[item]
         except KeyError as e:
             raise AttributeError(e)
 
     def __getitem__(self, item: str):
         return self._attrs[item]
+
+    def __setattr__(self, item: str, value):
+        if item.startswith("_"):
+            object.__setattr__(self, item, value)
+        elif isinstance(value, types.FunctionType):
+            self._funcs[item] = value
+        elif isinstance(value, type):
+            self._classes[item] = value
+        else:
+            self._vars[item] = value
+
+    def __getstate__(self):
+        return {
+            "vars": self._vars,
+        }
+
+    def __setstate__(self, state: dict[str, any]):
+        self._vars.update(state["vars"])
```

### Comparing `cpop-28.1.2/pop/log/async.py` & `cpop-28.2.0/pop/log/async.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 import inspect
 import sys
 
 import pop.contract
 
 
+async def __init__(hub):
+    hub.log.LOGGER = {}
+    hub.log.FILE_HANDLER = None
+    hub.log.STREAM_HANDLER = None
+    hub.log.LEVEL = {
+        "notset": hub.lib.logging.NOTSET,
+        "trace": 5,
+        "debug": hub.lib.logging.DEBUG,
+        "info": hub.lib.logging.INFO,
+        "warn": hub.lib.logging.WARN,
+        "warning": hub.lib.logging.WARNING,
+        "error": hub.lib.logging.ERROR,
+        "fatal": hub.lib.logging.FATAL,
+        "critical": hub.lib.logging.CRITICAL,
+    }
+
+
 def _stack_frames(relative_start: int) -> inspect.FrameInfo:
     """
     Efficiently access stack frames.
     :param relative_start: Starting stack depth; The default, 2 is the parent of the
             caller of stack_frames - the first function that may be unknown.
     :return: a stack frame
     """
@@ -89,40 +106,39 @@
     raw_level = conf["log_level"].strip().lower()
     hub.log.INT_LEVEL = (
         int(raw_level)
         if raw_level.isdigit()
         else hub.log.LEVEL.get(raw_level, hub.log.LEVEL["info"])
     )
 
-    # Get the root logger
-    root = _get_logger(hub, name="")
-    root.level = hub.log.INT_LEVEL
-
     # Set up the console handler
     console_formatter = hub.lib.aiologger.formatters.base.Formatter(
         fmt=conf["log_fmt_console"], datefmt=conf["log_datefmt"]
     )
     console_handler = hub.lib.aiologger.handlers.streams.AsyncStreamHandler(
         formatter=console_formatter, stream=hub.lib.sys.stderr
     )
-    root.add_handler(console_handler)
+    console_handler.level = hub.log.INT_LEVEL
     hub.log.STREAM_HANDLER = console_handler
 
     # Set up the file handler
     log_file = hub.lib.pathlib.Path(conf["log_file"]).expanduser()
     log_file.parent.mkdir(parents=True, exist_ok=True)
 
     file_formatter = hub.lib.aiologger.formatters.base.Formatter(
         fmt=conf["log_fmt_logfile"], datefmt=conf["log_datefmt"]
     )
     file_handler = hub.lib.aiologger.handlers.files.AsyncFileHandler(log_file)
     file_handler.formatter = file_formatter
-    root.add_handler(file_handler)
+    file_handler.level = hub.log.INT_LEVEL
     hub.log.FILE_HANDLER = file_handler
 
+    # Setup the root logger
+    _get_logger(hub, name="")
+
     # Put all these functions higher up on the hub
     hub.log.log = hub.log["async"].log
     hub.log.trace = lambda msg, *args, **kwargs: hub.log.log(
         level=5, msg=msg, *args, **kwargs
     )
     hub.log.debug = lambda msg, *args, **kwargs: hub.log.log(
         level=hub.lib.aiologger.levels.LogLevel.DEBUG, msg=msg, *args, **kwargs
```

### Comparing `cpop-28.1.2/pop/mods/pop/config.py` & `cpop-28.2.0/pop/mods/pop/config.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.2/pop/mods/pop/contract.py` & `cpop-28.2.0/pop/mods/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.2/pop/mods/pop/sub.py` & `cpop-28.2.0/pop/mods/pop/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.2/pop/mods/pop/test.py` & `cpop-28.2.0/pop/mods/pop/test.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.2/pop/pop.data.c` & `cpop-28.2.0/pop/pop.data.c`

 * *Files identical despite different names*

### Comparing `cpop-28.1.2/pop/pop.data.pyx` & `cpop-28.2.0/pop/pop.data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-28.1.2/pop/ref.py` & `cpop-28.2.0/pop/ref.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.2/pop/scanner.py` & `cpop-28.2.0/pop/scanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 import collections
 import os
 from collections.abc import Iterable
 from typing import Any
 
 PY_END = (".py", ".pyc", ".pyo")
-CYTHON_END = (".pyx",)
 
 
 def scan(dirs: Iterable[str]) -> dict[str, dict[str, Any]]:
     """
     :param dirs: A list of locations to search for importables files
     :return A description of importable files
     """
@@ -39,10 +38,7 @@
     full = os.path.join(dir_, fn_)
     if "." not in full:
         return
     bname = full[: full.rindex(".")]
     if fn_.endswith(PY_END):
         if bname not in ret["python"]:
             ret["python"][bname] = {"path": full}
-    if fn_.endswith(CYTHON_END):
-        if bname not in ret["cython"]:
-            ret["cython"][bname] = {"path": full}
```

### Comparing `cpop-28.1.2/pop/verify.py` & `cpop-28.2.0/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.2/pyproject.toml` & `cpop-28.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpop"
-version = "28.1.2"
+version = "28.2.0"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch@saltstack.com"},
 ]
 classifiers = [
```

### Comparing `cpop-28.1.2/setup.py` & `cpop-28.2.0/setup.py`

 * *Files identical despite different names*

