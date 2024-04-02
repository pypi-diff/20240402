# Comparing `tmp/flytekitplugins-flyteinteractive-1.12.0b2.tar.gz` & `tmp/flytekitplugins-flyteinteractive-1.12.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-flyteinteractive-1.12.0b2.tar", last modified: Fri Mar 29 21:24:52 2024, max compression
+gzip compressed data, was "flytekitplugins-flyteinteractive-1.12.0b3.tar", last modified: Tue Apr  2 21:31:31 2024, max compression
```

## Comparing `flytekitplugins-flyteinteractive-1.12.0b2.tar` & `flytekitplugins-flyteinteractive-1.12.0b3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:52.960283 flytekitplugins-flyteinteractive-1.12.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-29 21:24:52.960283 flytekitplugins-flyteinteractive-1.12.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:52.956282 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:52.956282 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:52.956282 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/jupyter_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/jupyter_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/jupyter_lib/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/jupyter_lib/jupyter_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:52.960283 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/vscode_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/vscode_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/vscode_lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18774 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/vscode_lib/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/vscode_lib/vscode_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:52.960283 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins_flyteinteractive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-29 21:24:52.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins_flyteinteractive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-29 21:24:52.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins_flyteinteractive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 21:24:52.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins_flyteinteractive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-29 21:24:52.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins_flyteinteractive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 21:24:52.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins_flyteinteractive.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-29 21:24:52.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins_flyteinteractive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 21:24:52.000000 flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins_flyteinteractive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 21:24:52.960283 flytekitplugins-flyteinteractive-1.12.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-29 21:24:49.000000 flytekitplugins-flyteinteractive-1.12.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:52.960283 flytekitplugins-flyteinteractive-1.12.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/tests/test_flyteinteractive_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/tests/test_flyteinteractive_vscode.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-29 21:24:26.000000 flytekitplugins-flyteinteractive-1.12.0b2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:31.761186 flytekitplugins-flyteinteractive-1.12.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-02 21:31:31.761186 flytekitplugins-flyteinteractive-1.12.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:31.757187 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:31.757187 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:31.757187 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/jupyter_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/jupyter_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/jupyter_lib/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/jupyter_lib/jupyter_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:31.757187 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/vscode_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/vscode_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/vscode_lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18774 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/vscode_lib/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/vscode_lib/vscode_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:31.761186 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins_flyteinteractive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-02 21:31:31.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins_flyteinteractive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 21:31:31.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins_flyteinteractive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:31:31.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins_flyteinteractive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 21:31:31.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins_flyteinteractive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 21:31:31.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins_flyteinteractive.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 21:31:31.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins_flyteinteractive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 21:31:31.000000 flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins_flyteinteractive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:31:31.761186 flytekitplugins-flyteinteractive-1.12.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-02 21:31:28.000000 flytekitplugins-flyteinteractive-1.12.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:31.761186 flytekitplugins-flyteinteractive-1.12.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/tests/test_flyteinteractive_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/tests/test_flyteinteractive_vscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 21:31:04.000000 flytekitplugins-flyteinteractive-1.12.0b3/tests/test_utils.py
```

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/PKG-INFO` & `flytekitplugins-flyteinteractive-1.12.0b3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-flyteinteractive
-Version: 1.12.0b2
+Version: 1.12.0b3
 Summary: This package holds the flyteinteractive plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/README.md` & `flytekitplugins-flyteinteractive-1.12.0b3/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/__init__.py` & `flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/jupyter_lib/decorator.py` & `flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/jupyter_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/utils.py` & `flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/utils.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/vscode_lib/config.py` & `flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/vscode_lib/config.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/vscode_lib/decorator.py` & `flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/vscode_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins/flyteinteractive/vscode_lib/vscode_constants.py` & `flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins/flyteinteractive/vscode_lib/vscode_constants.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins_flyteinteractive.egg-info/PKG-INFO` & `flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins_flyteinteractive.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-flyteinteractive
-Version: 1.12.0b2
+Version: 1.12.0b3
 Summary: This package holds the flyteinteractive plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/flytekitplugins_flyteinteractive.egg-info/SOURCES.txt` & `flytekitplugins-flyteinteractive-1.12.0b3/flytekitplugins_flyteinteractive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/setup.py` & `flytekitplugins-flyteinteractive-1.12.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "flyteinteractive"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.1.0b0,<2.0.0", "jupyter"]
 
-__version__ = "1.12.0b2"
+__version__ = "1.12.0b3"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the flyteinteractive plugins for flytekit",
```

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/tests/test_flyteinteractive_jupyter.py` & `flytekitplugins-flyteinteractive-1.12.0b3/tests/test_flyteinteractive_jupyter.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/tests/test_flyteinteractive_vscode.py` & `flytekitplugins-flyteinteractive-1.12.0b3/tests/test_flyteinteractive_vscode.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-flyteinteractive-1.12.0b2/tests/test_utils.py` & `flytekitplugins-flyteinteractive-1.12.0b3/tests/test_utils.py`

 * *Files identical despite different names*

