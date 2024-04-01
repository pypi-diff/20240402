# Comparing `tmp/cpop-28.0.7.tar.gz` & `tmp/cpop-28.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpop-28.0.7.tar", last modified: Mon Apr  1 21:12:57 2024, max compression
+gzip compressed data, was "cpop-28.1.0.tar", last modified: Mon Apr  1 22:52:16 2024, max compression
```

## Comparing `cpop-28.0.7.tar` & `cpop-28.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:12:57.847197 cpop-28.0.7/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.0.7/LICENSE
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      134 2024-04-01 21:10:23.000000 cpop-28.0.7/MANIFEST.in
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 21:12:57.847197 cpop-28.0.7/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4063 2024-04-01 20:42:25.000000 cpop-28.0.7/README.rst
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:12:57.847197 cpop-28.0.7/cpop.egg-info/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 21:12:57.000000 cpop-28.0.7/cpop.egg-info/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      562 2024-04-01 21:12:57.000000 cpop-28.0.7/cpop.egg-info/SOURCES.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-01 21:12:57.000000 cpop-28.0.7/cpop.egg-info/dependency_links.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-01 21:12:57.000000 cpop-28.0.7/cpop.egg-info/entry_points.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      128 2024-04-01 21:12:57.000000 cpop-28.0.7/cpop.egg-info/requires.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        8 2024-04-01 21:12:57.000000 cpop-28.0.7/cpop.egg-info/top_level.txt
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:12:57.847197 cpop-28.0.7/hub/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.0.7/hub/__init__.py
--rwxrwxr-x   0 akmod     (1000) akmod     (1000)     1979 2024-04-01 18:01:36.000000 cpop-28.0.7/hub/__main__.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:12:57.847197 cpop-28.0.7/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1993 2024-04-01 17:53:27.000000 cpop-28.0.7/pop/config.yaml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    10888 2024-04-01 16:10:17.000000 cpop-28.0.7/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   870672 2024-04-01 21:05:40.000000 cpop-28.0.7/pop/data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4437 2024-04-01 21:12:29.000000 cpop-28.0.7/pop/dirs.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.0.7/pop/exc.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    21514 2024-04-01 20:11:42.000000 cpop-28.0.7/pop/hub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11789 2024-04-01 17:46:15.000000 cpop-28.0.7/pop/loader.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:12:57.847197 cpop-28.0.7/pop/log/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4750 2024-04-01 16:10:17.000000 cpop-28.0.7/pop/log/async.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      491 2024-04-01 16:10:17.000000 cpop-28.0.7/pop/log/init.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:12:57.843197 cpop-28.0.7/pop/mods/
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:12:57.847197 cpop-28.0.7/pop/mods/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6077 2024-04-01 20:16:36.000000 cpop-28.0.7/pop/mods/pop/config.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.0.7/pop/mods/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.0.7/pop/mods/pop/dyne.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6985 2024-04-01 17:42:04.000000 cpop-28.0.7/pop/mods/pop/sub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.0.7/pop/mods/pop/test.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-01 21:12:49.000000 cpop-28.0.7/pop/pop.data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 19:03:13.000000 cpop-28.0.7/pop/pop.data.pyx
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.0.7/pop/ref.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1321 2024-03-24 19:08:30.000000 cpop-28.0.7/pop/scanner.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.0.7/pop/verify.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1315 2024-04-01 21:10:39.000000 cpop-28.0.7/pyproject.toml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-01 21:12:57.847197 cpop-28.0.7/setup.cfg
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1264 2024-04-01 21:06:48.000000 cpop-28.0.7/setup.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 22:52:16.682852 cpop-28.1.0/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.1.0/LICENSE
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      134 2024-04-01 21:10:23.000000 cpop-28.1.0/MANIFEST.in
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 22:52:16.682852 cpop-28.1.0/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4063 2024-04-01 20:42:25.000000 cpop-28.1.0/README.rst
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 22:52:16.678852 cpop-28.1.0/cpop.egg-info/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 22:52:16.000000 cpop-28.1.0/cpop.egg-info/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      562 2024-04-01 22:52:16.000000 cpop-28.1.0/cpop.egg-info/SOURCES.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-01 22:52:16.000000 cpop-28.1.0/cpop.egg-info/dependency_links.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-01 22:52:16.000000 cpop-28.1.0/cpop.egg-info/entry_points.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      136 2024-04-01 22:52:16.000000 cpop-28.1.0/cpop.egg-info/requires.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        8 2024-04-01 22:52:16.000000 cpop-28.1.0/cpop.egg-info/top_level.txt
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 22:52:16.678852 cpop-28.1.0/hub/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.1.0/hub/__init__.py
+-rwxrwxr-x   0 akmod     (1000) akmod     (1000)     3111 2024-04-01 22:51:27.000000 cpop-28.1.0/hub/__main__.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 22:52:16.682852 cpop-28.1.0/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     2119 2024-04-01 21:41:40.000000 cpop-28.1.0/pop/config.yaml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    10888 2024-04-01 16:10:17.000000 cpop-28.1.0/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   870672 2024-04-01 21:05:40.000000 cpop-28.1.0/pop/data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4437 2024-04-01 21:12:29.000000 cpop-28.1.0/pop/dirs.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.1.0/pop/exc.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    21502 2024-04-01 22:51:27.000000 cpop-28.1.0/pop/hub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11789 2024-04-01 17:46:15.000000 cpop-28.1.0/pop/loader.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 22:52:16.682852 cpop-28.1.0/pop/log/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4750 2024-04-01 16:10:17.000000 cpop-28.1.0/pop/log/async.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      491 2024-04-01 16:10:17.000000 cpop-28.1.0/pop/log/init.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 22:52:16.678852 cpop-28.1.0/pop/mods/
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 22:52:16.682852 cpop-28.1.0/pop/mods/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6109 2024-04-01 21:16:30.000000 cpop-28.1.0/pop/mods/pop/config.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.1.0/pop/mods/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.1.0/pop/mods/pop/dyne.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6993 2024-04-01 22:18:05.000000 cpop-28.1.0/pop/mods/pop/sub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.1.0/pop/mods/pop/test.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-01 22:52:02.000000 cpop-28.1.0/pop/pop.data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 21:18:00.000000 cpop-28.1.0/pop/pop.data.pyx
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.1.0/pop/ref.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1321 2024-03-24 19:08:30.000000 cpop-28.1.0/pop/scanner.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.1.0/pop/verify.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1328 2024-04-01 22:49:45.000000 cpop-28.1.0/pyproject.toml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-01 22:52:16.682852 cpop-28.1.0/setup.cfg
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1263 2024-04-01 21:16:30.000000 cpop-28.1.0/setup.py
```

### Comparing `cpop-28.0.7/LICENSE` & `cpop-28.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/PKG-INFO` & `cpop-28.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.0.7
+Version: 28.1.0
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.0.7/README.rst` & `cpop-28.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/cpop.egg-info/PKG-INFO` & `cpop-28.1.0/cpop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.0.7
+Version: 28.1.0
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.0.7/cpop.egg-info/SOURCES.txt` & `cpop-28.1.0/cpop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pop/config.yaml` & `cpop-28.1.0/pop/config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 
 # This is where we put things that USED to be in the conf.py
 config:
   pop_cli:
     ref:
       default: ""
     cli:
-      default:
+      default: ""
     args:
       default: []
+    hub_state:
+      default: ""
   pop:
     config:
       default: ~/.pop/config.yaml
   log:
     log_plugin:
       default: async
       os: POP_LOG_PLUGIN
@@ -39,14 +41,16 @@
       nargs: "?"
     cli:
       help: The namespace to use as the authoritative CLI
     args:
       help: Any additional arguments to forward to the next cli
       positional: True
       nargs: "..."
+    hub_state:
+      help: The location of a msgpack file that has a re-usable hub object
   pop:
     config:
       help: The config file used for POP
       options:
         - -c
   log:
     log_plugin:
```

### Comparing `cpop-28.0.7/pop/contract.py` & `cpop-28.1.0/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pop/data.c` & `cpop-28.1.0/pop/data.c`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pop/dirs.py` & `cpop-28.1.0/pop/dirs.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pop/exc.py` & `cpop-28.1.0/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pop/hub.py` & `cpop-28.1.0/pop/hub.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import copy
 import importlib.machinery
 import os
 import secrets
 import sys
 from collections.abc import Coroutine
 from types import ModuleType
 from typing import Any
@@ -94,26 +93,29 @@
         load_all_dynes: bool = True,
         load_all_subdirs: bool = True,
         recurse_subdirs: bool = True,
         pop_mods: list[str] = None,
         cli: str = None,
         logs: bool = True,
     ):
+        self._init_kwargs = {
+            k: v for k, v in locals().items() if k != "self" and not k.startswith("_")
+        }
 
         self._dynamic = None
         self._dscan = False
 
         self._subs = pop.data.NamespaceDict()
         self._sub_alias = pop.data.NamespaceDict()
         self._imports = pop.data.NamespaceDict()
         super().__init__([self._subs, self._sub_alias, self._imports])
 
         # Add the dyne for python imports to live in to the hub
         self._subs["lib"] = await AsyncSub(
-            self, "lib", dyne_name="lib", pypath=pop_mods
+            self, subname="lib", dyne_name="lib", pypath=pop_mods
         )
         # Load all existing libraries onto hub.lib
         self._subs["lib"]._imports.update(
             {
                 base: mod
                 for base, mod in sys.modules.items()
                 if not base.startswith("_") and "." not in base
@@ -122,15 +124,15 @@
 
         if pop_mods is None:
             pop_mods = ["pop.mods.pop"]
 
         # Add the pop sub to the hub, this should always use pypath and
         # Should never be made dynamic. This is a core system sub and should
         # NOT be app-merged
-        self._subs["pop"] = await AsyncSub(self, "pop", pypath=pop_mods)
+        self._subs["pop"] = await AsyncSub(self, subname="pop", pypath=pop_mods)
         await self._subs["pop"]._load_all()
 
         # Set up the conf OPT structure so it is always available
         self.OPT = None
         self._sync = SyncWrapper(self)
 
         self._load_all_dynes = load_all_dynes
@@ -142,15 +144,14 @@
 
             # Overwrite opt with config data
             self.OPT = await self.pop.config.load(cli=cli, **self._dynamic.config)
 
         # Set up a logger
         if logs:
             await self.log[self.OPT.log.log_plugin].setup(self.OPT.log.copy())
-            
 
     async def _load_all(self):
         for base, imp in self._dynamic.imports.items():
             self._subs.lib._imports[base] = imp
 
         # Load all dynamic subs onto the hub
         for dyne in self._dynamic.dyne:
@@ -169,43 +170,39 @@
         """
         while asyncio.iscoroutine(coroutine):
             coroutine = self._loop.run_until_complete(coroutine)
         return coroutine
 
     def __getstate__(self) -> dict:
         return dict(
-            subs=self._subs,
-            OPT=copy.copy(self.OPT),
+            init_kwargs=self._init_kwargs,
+            subs={name: sub.__getstate__() for name, sub in self._subs.items()},
+            aliases=self._sub_alias,
+            OPT=pop.data.unfreeze(self.OPT),
             imports={subname: mod.__name__ for subname, mod in self._imports.items()},
         )
 
     def __setstate__(self, state: dict):
-        self.__init__()
         subs = state["subs"]
         opt = state["OPT"]
+        aliases = state["aliases"]
+        # init_kwargs = state["init_kwargs"]
+        # self.__init__(**init_kwargs)
 
         self._imports = {
             subname: importlib.import_module(modname)
             for subname, modname in state["imports"].items()
         }
-        self.OPT = pop.data.ImmutableNamespaceDict(opt)
-        self._restore_subs(subs, self)
-        self._clear()
+        self._sub_alias = aliases
+        self.OPT = pop.data.freeze(opt)
+        for name, data in subs.items():
+            sub = Sub(hub=self, **data["init_kwargs"])
+            self._subs[name] = sub.__setstate__(data)
 
-    def _restore_subs(self, subs: dict[str, "Sub"], root):
-        """
-        Recursively restore all pickled subs that were added to this hub.
-        Make sure they are prepared properly with inits/virtuals/loadedmods
-        """
-        self._clear()
-        for name, sub in subs.items():
-            self._sync(
-                self.pop.sub.add(sub=root, load_all=True, **sub._restoreable_state)
-            )
-            self._restore_subs(sub._subs, root[name])
+        return self
 
     def _scan_dynamic(self):
         """
         Refresh the dynamic roots data used for loading app merge module roots
         """
         self._clear()
         self._dynamic = pop.dirs.dynamic_dirs()
@@ -221,32 +218,19 @@
 
 
 class Sub(PopMeta):
     """
     The pop object that contains the loaded module data
     """
 
-    def __init__(self):
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
-
-    async def __ainit__(
+    def __init__(
         self,
         hub: Hub,
-        subname: str,
         *,
+        subname: str,
         root: PopMeta = None,
         pypath: list[str] = None,
         static: list[str] = None,
         contracts_pypath: list[str] = None,
         contracts_static: list[str] = None,
         default_contracts: list[str] = None,
         virtual: bool = True,
@@ -286,14 +270,30 @@
         :param mod_basename: str: Manipulate the location in sys.modules that the plugin will be loaded to.
             Allow plugins to be loaded into a separate namespace.
         :param stop_on_failures: If any module fails to load for any reason, stacktrace and do not continue loading this sub
         :param init: bool: determine whether or not we process __init__ functions
         :param is_contract: Specify whether or not this sub is a contract
         :param sub_virtual: bool: Recursively ignore this sub and it's subs
         """
+        self._subs = pop.data.NamespaceDict()
+        self._alias = []
+        self._sub_alias = pop.data.NamespaceDict()
+        self._imports = pop.data.NamespaceDict()
+        self._loaded = pop.data.NamespaceDict()
+        # tracks what has been setattr-ed on this sub for performance; if something needs to be
+        # *removed*, we can delattr everything in _cached, it will be re-set on the next call.
+        super().__init__([self._loaded, self._subs, self._sub_alias, self._imports])
+        self._loaded_all = False
+        self._load_errors = pop.data.NamespaceDict()
+        self._vmap = pop.data.NamespaceDict()
+        self._init_kwargs = {
+            k: v
+            for k, v in locals().items()
+            if k not in ("self", "hub", "root") and not k.startswith("_")
+        }
         self._hub = hub
         self._root = root or hub
         self._subname = subname
         self._pypath = ex_path(pypath)
         self._static = ex_path(static)
         self._contracts_pypath = ex_path(contracts_pypath)
         self._contracts_static = ex_path(contracts_static)
@@ -308,14 +308,16 @@
         self._omit_func = omit_func
         self._omit_class = omit_class
         self._omit_vars = omit_vars
         self._mod_basename = mod_basename
         self._stop_on_failures = stop_on_failures
         self._is_contract = is_contract
         self._process_init = init
+
+    async def __ainit__(self):
         await self._prepare()
 
     async def _prepare(self):
         self._dirs = pop.dirs.dir_list(
             self._pypath,
             self._static,
         )
@@ -395,49 +397,50 @@
         if self._pypath:
             return self._pypath[0]
         elif self._dirs:
             return secrets.token_hex()
 
     def __getstate__(self):
         return dict(
-            pypath=self._pypath,
-            subname=self._subname,
-            static=self._static,
-            contracts_pypath=self._contracts_pypath,
-            contracts_static=self._contracts_static,
-            default_contracts=self._default_contracts,
-            virtual=self._virtual,
-            dyne_name=self._dyne_name,
-            omit_start=self._omit_start,
-            omit_end=self._omit_end,
-            omit_func=self._omit_func,
-            omit_class=self._omit_class,
-            omit_vars=self._omit_vars,
-            mod_basename=self._mod_basename,
-            stop_on_failures=self._stop_on_failures,
-            init=self._process_init,
-            recursive_contracts_static=self._recursive_contracts_static,
-            default_recursive_contracts=self._default_recursive_contracts,
-            _subs=self._subs,
+            init_kwargs=self._init_kwargs,
+            # TODO Make Loaded mod serializable
+            # loaded = self._loaded,
+            subs={name: sub.__getstate__() for name, sub in self._subs.items()},
+            aliases=self._sub_alias,
             imports={subname: mod.__name__ for subname, mod in self._imports.items()},
         )
 
     def __setstate__(self, state: dict):
         """
         Only a hub can truly restore a sub because of their interdependency
         """
-        self._subs = state.pop("_subs")
-        imports = state.pop("imports", {})
+        subs = state["subs"]
+        aliases = state["aliases"]
+        imports = state["imports"]
+        # loaded = state["loaded"]
+        # init_kwargs = state["init_kwargs"]
+
+        # self.__init__(**init_kwargs)
+        self._sub_alias = aliases
+
         self._imports = {
             subname: importlib.import_module(modname)
             for subname, modname in imports.items()
         }
-        # This will have all the arguments needed to recreate the Sub with pop.sub.add
-        self._restoreable_state = state
-        self._clear()
+
+        for name, data in subs.items():
+            sub = Sub(hub=self._hub, **data["init_kwargs"])
+            self._subs[name] = sub.__setstate__(data)
+
+        # TODO later it would be better to get all the serialized mods, for now just reload all
+        # for name, module in loaded.items():
+        #    ...
+        self._hub._synchronize(self.__ainit__())
+
+        return self
 
     def __getattr__(self, item: str):
         """
         If the item should be loaded, load it, else serve it
         """
         if item.startswith("_"):
             return self.__getattribute__(item)
@@ -593,13 +596,13 @@
 
 
 class AsyncInitWrapper:
     def __init__(self, cls):
         self.cls = cls
 
     async def __call__(self, *args, **kwargs):
-        instance = self.cls()
-        await instance.__ainit__(*args, **kwargs)
+        instance = self.cls(*args, **kwargs)
+        await instance.__ainit__()
         return instance
 
 
 AsyncSub = AsyncInitWrapper(Sub)
```

### Comparing `cpop-28.0.7/pop/loader.py` & `cpop-28.1.0/pop/loader.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pop/log/async.py` & `cpop-28.1.0/pop/log/async.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pop/mods/pop/config.py` & `cpop-28.1.0/pop/mods/pop/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,19 @@
         config_data = {}
 
     # Get the plain config data that will tell us about OS vars and defaults
     if not config:
         config = hub._dynamic.config.get("config") or {}
 
     OPT = await hub.pop.config.prioritize(
-        cli=cli, cli_opts=cli_opts, config=config, config_file_data=config_data, global_clis=global_clis
+        cli=cli,
+        cli_opts=cli_opts,
+        config=config,
+        config_file_data=config_data,
+        global_clis=global_clis,
     )
 
     return pop.data.freeze(OPT)
 
 
 async def parse_cli(
     hub,
@@ -158,15 +162,15 @@
     OPT = hub.lib.collections.defaultdict(dict)
     for namespace, args in config.items():
         for arg, data in args.items():
             # Initialize value to None
             value = None
 
             # 1. Check CLI options first
-            if (namespace == cli  or namespace in global_clis) and arg in cli_opts:
+            if (namespace == cli or namespace in global_clis) and arg in cli_opts:
                 value = cli_opts.get(arg, PLACEHOLDER)
 
             # 2. Check config file data if CLI option is not set
             if value is None:
                 value = config_file_data.get(namespace, {}).get(arg, PLACEHOLDER)
 
             # Skip malformed config
```

### Comparing `cpop-28.0.7/pop/mods/pop/contract.py` & `cpop-28.1.0/pop/mods/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pop/mods/pop/sub.py` & `cpop-28.1.0/pop/mods/pop/sub.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     if python_import:
         root._imports[subname] = hub.lib.importlib.import_module(python_import)
         return
 
     root._clear()
     root._subs[subname] = await pop.hub.AsyncSub(
         hub,
-        subname,
+        subname=subname,
         root=root,
         pypath=pypath,
         static=static,
         contracts_pypath=contracts_pypath,
         contracts_static=contracts_static,
         default_contracts=default_contracts,
         virtual=virtual,
```

### Comparing `cpop-28.0.7/pop/mods/pop/test.py` & `cpop-28.1.0/pop/mods/pop/test.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pop/pop.data.c` & `cpop-28.1.0/pop/pop.data.c`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pop/pop.data.pyx` & `cpop-28.1.0/pop/pop.data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pop/ref.py` & `cpop-28.1.0/pop/ref.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pop/scanner.py` & `cpop-28.1.0/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pop/verify.py` & `cpop-28.1.0/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.7/pyproject.toml` & `cpop-28.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpop"
-version = "28.0.7"
+version = "28.1.0"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch@saltstack.com"},
 ]
 classifiers = [
@@ -21,14 +21,15 @@
 requires-python = ">=3.10"
 
 
 dependencies = [
   "aiofiles",
   "aiologger",
   "argparse",
+  "msgpack",
   "PyYaml",
 ]
 
 [project.optional-dependencies]
 test = [
   "nest-asyncio",
   "pytest",
```

### Comparing `cpop-28.0.7/setup.py` & `cpop-28.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from Cython.Build import cythonize
 from setuptools import Command
 from setuptools import setup
 
 NAME = "cPop"
 SETUP_DIRNAME = os.path.dirname(__file__)
 
+
 class Clean(Command):
     user_options = []
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
@@ -36,14 +37,12 @@
             pdir = os.path.relpath(root, SETUP_DIRNAME)
             modname = pdir.replace(os.sep, ".")
             if modname not in skip_mods:
                 modules.append(modname)
     return modules
 
 
-
 setup(
     ext_modules=cythonize(os.path.join("pop", "pop.data.pyx")),
     packages=discover_packages(),
     cmdclass={"clean": Clean},
-
 )
```

