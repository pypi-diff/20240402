# Comparing `tmp/cpop-28.2.0.tar.gz` & `tmp/cpop-28.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpop-28.2.0.tar", last modified: Tue Apr  2 15:22:13 2024, max compression
+gzip compressed data, was "cpop-28.2.1.tar", last modified: Tue Apr  2 17:24:15 2024, max compression
```

## Comparing `cpop-28.2.0.tar` & `cpop-28.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.703872 cpop-28.2.0/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.2.0/LICENSE
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      134 2024-04-01 21:10:23.000000 cpop-28.2.0/MANIFEST.in
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-02 15:22:13.703872 cpop-28.2.0/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4411 2024-04-01 23:16:48.000000 cpop-28.2.0/README.rst
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.699872 cpop-28.2.0/cpop.egg-info/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-02 15:22:13.000000 cpop-28.2.0/cpop.egg-info/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      546 2024-04-02 15:22:13.000000 cpop-28.2.0/cpop.egg-info/SOURCES.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-02 15:22:13.000000 cpop-28.2.0/cpop.egg-info/dependency_links.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-02 15:22:13.000000 cpop-28.2.0/cpop.egg-info/entry_points.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      136 2024-04-02 15:22:13.000000 cpop-28.2.0/cpop.egg-info/requires.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        8 2024-04-02 15:22:13.000000 cpop-28.2.0/cpop.egg-info/top_level.txt
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.699872 cpop-28.2.0/hub/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.2.0/hub/__init__.py
--rwxrwxr-x   0 akmod     (1000) akmod     (1000)     3185 2024-04-02 15:16:07.000000 cpop-28.2.0/hub/__main__.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.703872 cpop-28.2.0/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     2156 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/config.yaml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    10479 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   870672 2024-04-01 21:05:40.000000 cpop-28.2.0/pop/data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4417 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/dirs.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.2.0/pop/exc.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    23607 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/hub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11303 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/loader.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.703872 cpop-28.2.0/pop/log/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     5219 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/log/async.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.699872 cpop-28.2.0/pop/mods/
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 15:22:13.703872 cpop-28.2.0/pop/mods/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6339 2024-04-01 23:12:04.000000 cpop-28.2.0/pop/mods/pop/config.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.2.0/pop/mods/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.2.0/pop/mods/pop/dyne.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6993 2024-04-01 22:18:05.000000 cpop-28.2.0/pop/mods/pop/sub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.2.0/pop/mods/pop/test.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-02 15:17:57.000000 cpop-28.2.0/pop/pop.data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 21:18:00.000000 cpop-28.2.0/pop/pop.data.pyx
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.2.0/pop/ref.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1176 2024-04-02 15:16:07.000000 cpop-28.2.0/pop/scanner.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.2.0/pop/verify.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1328 2024-04-02 15:17:28.000000 cpop-28.2.0/pyproject.toml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-02 15:22:13.707872 cpop-28.2.0/setup.cfg
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1263 2024-04-01 21:16:30.000000 cpop-28.2.0/setup.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 17:24:15.577788 cpop-28.2.1/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.2.1/LICENSE
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      134 2024-04-01 21:10:23.000000 cpop-28.2.1/MANIFEST.in
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-02 17:24:15.577788 cpop-28.2.1/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4411 2024-04-01 23:16:48.000000 cpop-28.2.1/README.rst
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 17:24:15.573788 cpop-28.2.1/cpop.egg-info/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-02 17:24:15.000000 cpop-28.2.1/cpop.egg-info/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      546 2024-04-02 17:24:15.000000 cpop-28.2.1/cpop.egg-info/SOURCES.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-02 17:24:15.000000 cpop-28.2.1/cpop.egg-info/dependency_links.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-02 17:24:15.000000 cpop-28.2.1/cpop.egg-info/entry_points.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      136 2024-04-02 17:24:15.000000 cpop-28.2.1/cpop.egg-info/requires.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        8 2024-04-02 17:24:15.000000 cpop-28.2.1/cpop.egg-info/top_level.txt
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 17:24:15.573788 cpop-28.2.1/hub/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.2.1/hub/__init__.py
+-rwxrwxr-x   0 akmod     (1000) akmod     (1000)     3192 2024-04-02 17:23:45.000000 cpop-28.2.1/hub/__main__.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 17:24:15.577788 cpop-28.2.1/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     2156 2024-04-02 15:16:07.000000 cpop-28.2.1/pop/config.yaml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    10479 2024-04-02 15:16:07.000000 cpop-28.2.1/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   870672 2024-04-01 21:05:40.000000 cpop-28.2.1/pop/data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4417 2024-04-02 15:16:07.000000 cpop-28.2.1/pop/dirs.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.2.1/pop/exc.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    23607 2024-04-02 15:16:07.000000 cpop-28.2.1/pop/hub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11303 2024-04-02 15:16:07.000000 cpop-28.2.1/pop/loader.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 17:24:15.577788 cpop-28.2.1/pop/log/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     5219 2024-04-02 15:16:07.000000 cpop-28.2.1/pop/log/async.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 17:24:15.573788 cpop-28.2.1/pop/mods/
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 17:24:15.577788 cpop-28.2.1/pop/mods/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6339 2024-04-01 23:12:04.000000 cpop-28.2.1/pop/mods/pop/config.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.2.1/pop/mods/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.2.1/pop/mods/pop/dyne.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6993 2024-04-01 22:18:05.000000 cpop-28.2.1/pop/mods/pop/sub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.2.1/pop/mods/pop/test.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-02 17:24:03.000000 cpop-28.2.1/pop/pop.data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 21:18:00.000000 cpop-28.2.1/pop/pop.data.pyx
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.2.1/pop/ref.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1176 2024-04-02 15:16:07.000000 cpop-28.2.1/pop/scanner.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.2.1/pop/verify.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1328 2024-04-02 17:23:51.000000 cpop-28.2.1/pyproject.toml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-02 17:24:15.577788 cpop-28.2.1/setup.cfg
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1263 2024-04-01 21:16:30.000000 cpop-28.2.1/setup.py
```

### Comparing `cpop-28.2.0/LICENSE` & `cpop-28.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/PKG-INFO` & `cpop-28.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.2.0
+Version: 28.2.1
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.2.0/README.rst` & `cpop-28.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/cpop.egg-info/PKG-INFO` & `cpop-28.2.1/cpop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.2.0
+Version: 28.2.1
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.2.0/cpop.egg-info/SOURCES.txt` & `cpop-28.2.1/cpop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/hub/__main__.py` & `cpop-28.2.1/hub/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     # Create the hub, loading all dynes and starting the loop
     hub = pop.hub.Hub(cli="pop_cli")
 
     args = []
     kwargs = {}
 
     original_opt = hub.OPT
-    ref = original_opt.pop_cli.ref
+    ref = original_opt.pop_cli.ref or "."
 
     # Try to get a saved hub
     if original_opt.pop_cli.hub_state:
         hub_state_file = pathlib.Path(original_opt.pop_cli.hub_state).expanduser()
         new_hub = load_hub_state(hub, hub_state_file)
     else:
         hub_state_file = None
```

### Comparing `cpop-28.2.0/pop/config.yaml` & `cpop-28.2.1/pop/config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/contract.py` & `cpop-28.2.1/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/data.c` & `cpop-28.2.1/pop/data.c`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/dirs.py` & `cpop-28.2.1/pop/dirs.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/exc.py` & `cpop-28.2.1/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/hub.py` & `cpop-28.2.1/pop/hub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/loader.py` & `cpop-28.2.1/pop/loader.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/log/async.py` & `cpop-28.2.1/pop/log/async.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/mods/pop/config.py` & `cpop-28.2.1/pop/mods/pop/config.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/mods/pop/contract.py` & `cpop-28.2.1/pop/mods/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/mods/pop/sub.py` & `cpop-28.2.1/pop/mods/pop/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/mods/pop/test.py` & `cpop-28.2.1/pop/mods/pop/test.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/pop.data.c` & `cpop-28.2.1/pop/pop.data.c`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/pop.data.pyx` & `cpop-28.2.1/pop/pop.data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/ref.py` & `cpop-28.2.1/pop/ref.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/scanner.py` & `cpop-28.2.1/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pop/verify.py` & `cpop-28.2.1/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.0/pyproject.toml` & `cpop-28.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpop"
-version = "28.2.0"
+version = "28.2.1"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch@saltstack.com"},
 ]
 classifiers = [
```

### Comparing `cpop-28.2.0/setup.py` & `cpop-28.2.1/setup.py`

 * *Files identical despite different names*

