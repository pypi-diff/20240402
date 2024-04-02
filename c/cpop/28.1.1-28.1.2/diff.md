# Comparing `tmp/cpop-28.1.1.tar.gz` & `tmp/cpop-28.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpop-28.1.1.tar", last modified: Mon Apr  1 23:12:39 2024, max compression
+gzip compressed data, was "cpop-28.1.2.tar", last modified: Mon Apr  1 23:17:17 2024, max compression
```

## Comparing `cpop-28.1.1.tar` & `cpop-28.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:12:39.324677 cpop-28.1.1/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.1.1/LICENSE
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      134 2024-04-01 21:10:23.000000 cpop-28.1.1/MANIFEST.in
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 23:12:39.324677 cpop-28.1.1/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4063 2024-04-01 20:42:25.000000 cpop-28.1.1/README.rst
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:12:39.320677 cpop-28.1.1/cpop.egg-info/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 23:12:39.000000 cpop-28.1.1/cpop.egg-info/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      562 2024-04-01 23:12:39.000000 cpop-28.1.1/cpop.egg-info/SOURCES.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-01 23:12:39.000000 cpop-28.1.1/cpop.egg-info/dependency_links.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-01 23:12:39.000000 cpop-28.1.1/cpop.egg-info/entry_points.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      136 2024-04-01 23:12:39.000000 cpop-28.1.1/cpop.egg-info/requires.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        8 2024-04-01 23:12:39.000000 cpop-28.1.1/cpop.egg-info/top_level.txt
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:12:39.320677 cpop-28.1.1/hub/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.1.1/hub/__init__.py
--rwxrwxr-x   0 akmod     (1000) akmod     (1000)     3111 2024-04-01 22:51:27.000000 cpop-28.1.1/hub/__main__.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:12:39.324677 cpop-28.1.1/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     2131 2024-04-01 23:12:03.000000 cpop-28.1.1/pop/config.yaml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    10888 2024-04-01 16:10:17.000000 cpop-28.1.1/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   870672 2024-04-01 21:05:40.000000 cpop-28.1.1/pop/data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4437 2024-04-01 21:12:29.000000 cpop-28.1.1/pop/dirs.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.1.1/pop/exc.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    21502 2024-04-01 22:51:27.000000 cpop-28.1.1/pop/hub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11789 2024-04-01 17:46:15.000000 cpop-28.1.1/pop/loader.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:12:39.324677 cpop-28.1.1/pop/log/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4750 2024-04-01 16:10:17.000000 cpop-28.1.1/pop/log/async.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      491 2024-04-01 16:10:17.000000 cpop-28.1.1/pop/log/init.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:12:39.320677 cpop-28.1.1/pop/mods/
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:12:39.324677 cpop-28.1.1/pop/mods/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6339 2024-04-01 23:12:04.000000 cpop-28.1.1/pop/mods/pop/config.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.1.1/pop/mods/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.1.1/pop/mods/pop/dyne.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6993 2024-04-01 22:18:05.000000 cpop-28.1.1/pop/mods/pop/sub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.1.1/pop/mods/pop/test.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-01 23:11:23.000000 cpop-28.1.1/pop/pop.data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 21:18:00.000000 cpop-28.1.1/pop/pop.data.pyx
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.1.1/pop/ref.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1321 2024-03-24 19:08:30.000000 cpop-28.1.1/pop/scanner.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.1.1/pop/verify.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1328 2024-04-01 23:12:15.000000 cpop-28.1.1/pyproject.toml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-01 23:12:39.324677 cpop-28.1.1/setup.cfg
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1263 2024-04-01 21:16:30.000000 cpop-28.1.1/setup.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.689982 cpop-28.1.2/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.1.2/LICENSE
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      134 2024-04-01 21:10:23.000000 cpop-28.1.2/MANIFEST.in
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-01 23:17:17.689982 cpop-28.1.2/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4411 2024-04-01 23:16:48.000000 cpop-28.1.2/README.rst
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.685982 cpop-28.1.2/cpop.egg-info/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-01 23:17:17.000000 cpop-28.1.2/cpop.egg-info/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      562 2024-04-01 23:17:17.000000 cpop-28.1.2/cpop.egg-info/SOURCES.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-01 23:17:17.000000 cpop-28.1.2/cpop.egg-info/dependency_links.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-01 23:17:17.000000 cpop-28.1.2/cpop.egg-info/entry_points.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      136 2024-04-01 23:17:17.000000 cpop-28.1.2/cpop.egg-info/requires.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        8 2024-04-01 23:17:17.000000 cpop-28.1.2/cpop.egg-info/top_level.txt
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.685982 cpop-28.1.2/hub/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.1.2/hub/__init__.py
+-rwxrwxr-x   0 akmod     (1000) akmod     (1000)     3111 2024-04-01 22:51:27.000000 cpop-28.1.2/hub/__main__.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.689982 cpop-28.1.2/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     2137 2024-04-01 23:13:39.000000 cpop-28.1.2/pop/config.yaml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    10888 2024-04-01 16:10:17.000000 cpop-28.1.2/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   870672 2024-04-01 21:05:40.000000 cpop-28.1.2/pop/data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4437 2024-04-01 21:12:29.000000 cpop-28.1.2/pop/dirs.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.1.2/pop/exc.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    21502 2024-04-01 22:51:27.000000 cpop-28.1.2/pop/hub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11789 2024-04-01 17:46:15.000000 cpop-28.1.2/pop/loader.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.689982 cpop-28.1.2/pop/log/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4750 2024-04-01 16:10:17.000000 cpop-28.1.2/pop/log/async.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      491 2024-04-01 16:10:17.000000 cpop-28.1.2/pop/log/init.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.685982 cpop-28.1.2/pop/mods/
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 23:17:17.689982 cpop-28.1.2/pop/mods/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6339 2024-04-01 23:12:04.000000 cpop-28.1.2/pop/mods/pop/config.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.1.2/pop/mods/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.1.2/pop/mods/pop/dyne.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6993 2024-04-01 22:18:05.000000 cpop-28.1.2/pop/mods/pop/sub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.1.2/pop/mods/pop/test.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-01 23:17:08.000000 cpop-28.1.2/pop/pop.data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 21:18:00.000000 cpop-28.1.2/pop/pop.data.pyx
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.1.2/pop/ref.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1321 2024-03-24 19:08:30.000000 cpop-28.1.2/pop/scanner.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.1.2/pop/verify.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1328 2024-04-01 23:14:36.000000 cpop-28.1.2/pyproject.toml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-01 23:17:17.689982 cpop-28.1.2/setup.cfg
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1263 2024-04-01 21:16:30.000000 cpop-28.1.2/setup.py
```

### Comparing `cpop-28.1.1/LICENSE` & `cpop-28.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/PKG-INFO` & `cpop-28.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.1.1
+Version: 28.1.2
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -135,14 +135,27 @@
     import:
         - asyncio
         - importlib
         - importlib.resources
         - os
         - toml
 
+Create a pop config file:
+
+.. code-block:: yaml
+
+    # The default location is in ~/.pop/config.yaml
+    # But you can change that by setting the POP_CONFIG environment variable
+
+    pop_cli:
+        # Setting this option will make your hub persist on the cli between calls
+        hub_state: ~/.pop/hub.msgpack
+    log:
+        log_plugin: async
+
 From the above example, all arguments would be loaded onto the namespace under hub.OPT.my_namesapce.
 One config.yaml can add config options to multiple namespaces.
 They are all merged together in the order they are found in sys.path
 
 
 Testing
 =======
```

### Comparing `cpop-28.1.1/README.rst` & `cpop-28.1.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -119,14 +119,27 @@
     import:
         - asyncio
         - importlib
         - importlib.resources
         - os
         - toml
 
+Create a pop config file:
+
+.. code-block:: yaml
+
+    # The default location is in ~/.pop/config.yaml
+    # But you can change that by setting the POP_CONFIG environment variable
+
+    pop_cli:
+        # Setting this option will make your hub persist on the cli between calls
+        hub_state: ~/.pop/hub.msgpack
+    log:
+        log_plugin: async
+
 From the above example, all arguments would be loaded onto the namespace under hub.OPT.my_namesapce.
 One config.yaml can add config options to multiple namespaces.
 They are all merged together in the order they are found in sys.path
 
 
 Testing
 =======
```

### Comparing `cpop-28.1.1/cpop.egg-info/PKG-INFO` & `cpop-28.1.2/cpop.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.1.1
+Version: 28.1.2
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -135,14 +135,27 @@
     import:
         - asyncio
         - importlib
         - importlib.resources
         - os
         - toml
 
+Create a pop config file:
+
+.. code-block:: yaml
+
+    # The default location is in ~/.pop/config.yaml
+    # But you can change that by setting the POP_CONFIG environment variable
+
+    pop_cli:
+        # Setting this option will make your hub persist on the cli between calls
+        hub_state: ~/.pop/hub.msgpack
+    log:
+        log_plugin: async
+
 From the above example, all arguments would be loaded onto the namespace under hub.OPT.my_namesapce.
 One config.yaml can add config options to multiple namespaces.
 They are all merged together in the order they are found in sys.path
 
 
 Testing
 =======
```

### Comparing `cpop-28.1.1/cpop.egg-info/SOURCES.txt` & `cpop-28.1.2/cpop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/hub/__main__.py` & `cpop-28.1.2/hub/__main__.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/config.yaml` & `cpop-28.1.2/pop/config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # This is where we put things that USED to be in the conf.py
 config:
   pop_cli:
     ref:
-      default:
+      default: ""
     cli:
-      default:
+      default: ""
     args:
       default: []
     hub_state:
       default:
   pop:
     config:
       default: ~/.pop/config.yaml
```

### Comparing `cpop-28.1.1/pop/contract.py` & `cpop-28.1.2/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/data.c` & `cpop-28.1.2/pop/data.c`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/dirs.py` & `cpop-28.1.2/pop/dirs.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/exc.py` & `cpop-28.1.2/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/hub.py` & `cpop-28.1.2/pop/hub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/loader.py` & `cpop-28.1.2/pop/loader.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/log/async.py` & `cpop-28.1.2/pop/log/async.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/mods/pop/config.py` & `cpop-28.1.2/pop/mods/pop/config.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/mods/pop/contract.py` & `cpop-28.1.2/pop/mods/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/mods/pop/sub.py` & `cpop-28.1.2/pop/mods/pop/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/mods/pop/test.py` & `cpop-28.1.2/pop/mods/pop/test.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/pop.data.c` & `cpop-28.1.2/pop/pop.data.c`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/pop.data.pyx` & `cpop-28.1.2/pop/pop.data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/ref.py` & `cpop-28.1.2/pop/ref.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/scanner.py` & `cpop-28.1.2/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pop/verify.py` & `cpop-28.1.2/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-28.1.1/pyproject.toml` & `cpop-28.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpop"
-version = "28.1.1"
+version = "28.1.2"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch@saltstack.com"},
 ]
 classifiers = [
```

### Comparing `cpop-28.1.1/setup.py` & `cpop-28.1.2/setup.py`

 * *Files identical despite different names*

