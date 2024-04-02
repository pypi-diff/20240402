# Comparing `tmp/vesselasid-1.0.8.tar.gz` & `tmp/vesselasid-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vesselasid-1.0.8.tar", last modified: Fri Mar  1 23:59:58 2024, max compression
+gzip compressed data, was "vesselasid-1.0.9.tar", last modified: Tue Mar 12 03:39:40 2024, max compression
```

## Comparing `vesselasid-1.0.8.tar` & `vesselasid-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:59:58.241180 vesselasid-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:59:58.237180 vesselasid-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:59:58.237180 vesselasid-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-01 23:59:56.000000 vesselasid-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-01 23:59:56.000000 vesselasid-1.0.8/.github/workflows/tests-unit.yml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-01 23:59:58.000000 vesselasid-1.0.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-01 23:59:58.000000 vesselasid-1.0.8/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-01 23:59:56.000000 vesselasid-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-01 23:59:58.241180 vesselasid-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-03-01 23:59:56.000000 vesselasid-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-01 23:59:56.000000 vesselasid-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-01 23:59:58.241180 vesselasid-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-01 23:59:56.000000 vesselasid-1.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-01 23:59:56.000000 vesselasid-1.0.8/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:59:58.237180 vesselasid-1.0.8/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5516 2024-03-01 23:59:56.000000 vesselasid-1.0.8/tests/test_asid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      246 2024-03-01 23:59:56.000000 vesselasid-1.0.8/tests/test_asm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:59:58.237180 vesselasid-1.0.8/vesselasid/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8881 2024-03-01 23:59:56.000000 vesselasid-1.0.8/vesselasid/asid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4220 2024-03-01 23:59:56.000000 vesselasid-1.0.8/vesselasid/asidrenderer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      532 2024-03-01 23:59:56.000000 vesselasid-1.0.8/vesselasid/asm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-03-01 23:59:56.000000 vesselasid-1.0.8/vesselasid/baserender.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      584 2024-03-01 23:59:56.000000 vesselasid-1.0.8/vesselasid/examplerender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:59:58.241180 vesselasid-1.0.8/vesselasid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-01 23:59:58.000000 vesselasid-1.0.8/vesselasid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-01 23:59:58.000000 vesselasid-1.0.8/vesselasid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 23:59:58.000000 vesselasid-1.0.8/vesselasid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-01 23:59:58.000000 vesselasid-1.0.8/vesselasid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 23:59:58.000000 vesselasid-1.0.8/vesselasid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-01 23:59:58.000000 vesselasid-1.0.8/vesselasid.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-01 23:59:58.000000 vesselasid-1.0.8/vesselasid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-01 23:59:58.000000 vesselasid-1.0.8/vesselasid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:39:40.601950 vesselasid-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:39:40.601950 vesselasid-1.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-12 03:39:38.000000 vesselasid-1.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:39:40.601950 vesselasid-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-12 03:39:38.000000 vesselasid-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-12 03:39:38.000000 vesselasid-1.0.9/.github/workflows/tests-unit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-12 03:39:40.000000 vesselasid-1.0.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-12 03:39:40.000000 vesselasid-1.0.9/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-12 03:39:38.000000 vesselasid-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-12 03:39:40.601950 vesselasid-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-03-12 03:39:38.000000 vesselasid-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-12 03:39:38.000000 vesselasid-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-12 03:39:40.601950 vesselasid-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-12 03:39:38.000000 vesselasid-1.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-12 03:39:38.000000 vesselasid-1.0.9/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:39:40.601950 vesselasid-1.0.9/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5516 2024-03-12 03:39:38.000000 vesselasid-1.0.9/tests/test_asid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      246 2024-03-12 03:39:38.000000 vesselasid-1.0.9/tests/test_asm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:39:40.601950 vesselasid-1.0.9/vesselasid/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8881 2024-03-12 03:39:38.000000 vesselasid-1.0.9/vesselasid/asid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5044 2024-03-12 03:39:38.000000 vesselasid-1.0.9/vesselasid/asidrenderer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      532 2024-03-12 03:39:38.000000 vesselasid-1.0.9/vesselasid/asm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-03-12 03:39:38.000000 vesselasid-1.0.9/vesselasid/baserender.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      584 2024-03-12 03:39:38.000000 vesselasid-1.0.9/vesselasid/examplerender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:39:40.601950 vesselasid-1.0.9/vesselasid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-12 03:39:40.000000 vesselasid-1.0.9/vesselasid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-12 03:39:40.000000 vesselasid-1.0.9/vesselasid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 03:39:40.000000 vesselasid-1.0.9/vesselasid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-12 03:39:40.000000 vesselasid-1.0.9/vesselasid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 03:39:40.000000 vesselasid-1.0.9/vesselasid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-12 03:39:40.000000 vesselasid-1.0.9/vesselasid.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-12 03:39:40.000000 vesselasid-1.0.9/vesselasid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-12 03:39:40.000000 vesselasid-1.0.9/vesselasid.egg-info/top_level.txt
```

### Comparing `vesselasid-1.0.8/.github/workflows/release.yml` & `vesselasid-1.0.9/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -20,11 +20,11 @@
       - name: Set up python-${{ env.RELEASE_PY_VER }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ env.RELEASE_PY_VER }}
       - name: Build python package
         run: python3 setup.py sdist
       - name: Publish python package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.10
+        uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `vesselasid-1.0.8/.github/workflows/tests-unit.yml` & `vesselasid-1.0.9/.github/workflows/tests-unit.yml`

 * *Files identical despite different names*

### Comparing `vesselasid-1.0.8/LICENSE` & `vesselasid-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vesselasid-1.0.8/PKG-INFO` & `vesselasid-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vesselasid
-Version: 1.0.8
+Version: 1.0.9
 Summary: Vessel ASID client
 Home-page: https://github.com/anarkiwi/vessel
 Author: Josh Bailey
 Author-email: josh@vandervecken.com
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `vesselasid-1.0.8/README.md` & `vesselasid-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -133,17 +133,7 @@
 2024-03-01 08:52:43,042 found ExampleAsidRenderer
 2024-03-01 08:52:43,042 program 0 is ExampleAsidRenderer
 2024-03-01 08:52:43,042 using Scarlett 4i4 USB:Scarlett 4i4 USB MIDI 1 20:0 for ASID
 2024-03-01 08:52:43,042 using Midi Through:Midi Through Port-0 14:0 for control input
 2024-03-01 08:52:43,044 starting renderer ExampleAsidRenderer
 2024-03-01 08:52:49,049 note_off channel=0 note=90 velocity=0 time=0
 ```
-
-### macosx
-
-```
-$ MIDO_BACKEND=mido.backends.portmidi asidrenderer --asid-port ...
-````
-
-
-
-
```

### Comparing `vesselasid-1.0.8/setup.cfg` & `vesselasid-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `vesselasid-1.0.8/tests/test_asid.py` & `vesselasid-1.0.9/tests/test_asid.py`

 * *Files identical despite different names*

### Comparing `vesselasid-1.0.8/vesselasid/asid.py` & `vesselasid-1.0.9/vesselasid/asid.py`

 * *Files identical despite different names*

### Comparing `vesselasid-1.0.8/vesselasid/asidrenderer.py` & `vesselasid-1.0.9/vesselasid/asidrenderer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,40 @@
 from argparse import ArgumentParser, BooleanOptionalAction
 import importlib
 import inspect
 import logging
 import time
+import os
+import platform
 import mido
 from vesselasid.asid import Asid
 from vesselasid.baserender import VesselAsidRenderer
 
 
+def known_loopbacks(names):
+    loopbacks = set()
+    for name in names:
+        for loopback in ("IAC Driver", "Midi Through"):
+            if loopback in name:
+                loopbacks.add(name)
+                break
+    others = set(names) - loopbacks
+    return sorted(list(loopbacks), reverse=True), sorted(list(others), reverse=True)
+
+
 def main():
     logging.basicConfig(level=logging.DEBUG, format="%(asctime)s %(message)s")
+
+    if platform.system() == "Darwin" and os.getenv("MIDO_BACKEND", None) is None:
+        mido.set_backend("mido.backends.portmidi")
     if not mido.get_output_names():
         logging.fatal("no output ports available")
         raise ValueError
     if not mido.get_input_names():
-        logging.fatal("no input ports avaialable")
+        logging.fatal("no input ports available")
         raise ValueError
 
     parser = ArgumentParser()
     parser.add_argument(
         "--asid-port",
         dest="asid_port",
         type=str,
@@ -78,31 +94,38 @@
     if options.default_renderer not in renderers_map:
         logging.fatal("default renderer %u not in renders", options.default_renderer)
         raise ValueError
 
     asid_port = options.asid_port
     if not asid_port:
         asid_port = mido.get_output_names()[0]
+        loopbacks, others = known_loopbacks(mido.get_output_names())
+        if others:
+            asid_port = others[0]
     ctrl_port = options.ctrl_port
     if not ctrl_port:
         ctrl_port = mido.get_input_names()[0]
+        loopbacks, others = known_loopbacks(mido.get_input_names())
+        if loopbacks:
+            ctrl_port = loopbacks[0]
     logging.info("using %s for ASID", asid_port)
     logging.info("using %s for control input", ctrl_port)
 
     asid_out_port = mido.open_output(asid_port)
     asid_in_port = None
     if options.asid_input:
         asid_in_port = mido.open_input(asid_port)
 
     asid = Asid(asid_out_port, in_port=asid_in_port)
 
     def get_renderer(r):
         logging.info("starting renderer %u (%s)", r, renderers_map[r][0])
         renderer = renderers_map[r][1](asid)
         renderer.start()
+        logging.info("renderer %u (%s) started", r, renderers_map[r][0])
         return renderer
 
     with mido.open_input(ctrl_port) as ctrl_in_port:
         renderer = get_renderer(options.default_renderer)
         try:
             for msg in ctrl_in_port:
                 if msg.type == "program_change":
```

### Comparing `vesselasid-1.0.8/vesselasid/asm.py` & `vesselasid-1.0.9/vesselasid/asm.py`

 * *Files identical despite different names*

### Comparing `vesselasid-1.0.8/vesselasid/examplerender.py` & `vesselasid-1.0.9/vesselasid/examplerender.py`

 * *Files identical despite different names*

### Comparing `vesselasid-1.0.8/vesselasid.egg-info/PKG-INFO` & `vesselasid-1.0.9/vesselasid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vesselasid
-Version: 1.0.8
+Version: 1.0.9
 Summary: Vessel ASID client
 Home-page: https://github.com/anarkiwi/vessel
 Author: Josh Bailey
 Author-email: josh@vandervecken.com
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

