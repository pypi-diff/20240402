# Comparing `tmp/urdfeus-0.0.8.tar.gz` & `tmp/urdfeus-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urdfeus-0.0.8.tar", last modified: Tue Feb 27 06:03:20 2024, max compression
+gzip compressed data, was "urdfeus-0.0.9.tar", last modified: Tue Apr  2 14:48:28 2024, max compression
```

## Comparing `urdfeus-0.0.8.tar` & `urdfeus-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 06:03:20.137189 urdfeus-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-27 06:03:14.000000 urdfeus-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-27 06:03:14.000000 urdfeus-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-27 06:03:20.137189 urdfeus-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-27 06:03:14.000000 urdfeus-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-27 06:03:14.000000 urdfeus-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-27 06:03:20.137189 urdfeus-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-02-27 06:03:14.000000 urdfeus-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 06:03:20.137189 urdfeus-0.0.8/urdfeus/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-27 06:03:14.000000 urdfeus-0.0.8/urdfeus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 06:03:20.137189 urdfeus-0.0.8/urdfeus/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 06:03:14.000000 urdfeus-0.0.8/urdfeus/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-27 06:03:14.000000 urdfeus-0.0.8/urdfeus/apps/mesh2eus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-02-27 06:03:14.000000 urdfeus-0.0.8/urdfeus/apps/urdf2eus.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-02-27 06:03:14.000000 urdfeus-0.0.8/urdfeus/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-02-27 06:03:14.000000 urdfeus-0.0.8/urdfeus/mesh2eus.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-02-27 06:03:14.000000 urdfeus-0.0.8/urdfeus/read_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 06:03:20.137189 urdfeus-0.0.8/urdfeus/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-27 06:03:14.000000 urdfeus-0.0.8/urdfeus/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-02-27 06:03:14.000000 urdfeus-0.0.8/urdfeus/templates/euscollada-robot.l
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-27 06:03:14.000000 urdfeus-0.0.8/urdfeus/templates/urdf_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    19191 2024-02-27 06:03:14.000000 urdfeus-0.0.8/urdfeus/urdf2eus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 06:03:20.137189 urdfeus-0.0.8/urdfeus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-27 06:03:20.000000 urdfeus-0.0.8/urdfeus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-27 06:03:20.000000 urdfeus-0.0.8/urdfeus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 06:03:20.000000 urdfeus-0.0.8/urdfeus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-27 06:03:20.000000 urdfeus-0.0.8/urdfeus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 06:03:20.000000 urdfeus-0.0.8/urdfeus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-27 06:03:20.000000 urdfeus-0.0.8/urdfeus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-27 06:03:20.000000 urdfeus-0.0.8/urdfeus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:48:28.168795 urdfeus-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-02 14:48:18.000000 urdfeus-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 14:48:18.000000 urdfeus-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-02 14:48:28.168795 urdfeus-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 14:48:18.000000 urdfeus-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 14:48:18.000000 urdfeus-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-02 14:48:28.168795 urdfeus-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-02 14:48:18.000000 urdfeus-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:48:28.168795 urdfeus-0.0.9/urdfeus/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 14:48:18.000000 urdfeus-0.0.9/urdfeus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:48:28.168795 urdfeus-0.0.9/urdfeus/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:48:18.000000 urdfeus-0.0.9/urdfeus/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-02 14:48:18.000000 urdfeus-0.0.9/urdfeus/apps/mesh2eus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-02 14:48:18.000000 urdfeus-0.0.9/urdfeus/apps/urdf2eus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-02 14:48:18.000000 urdfeus-0.0.9/urdfeus/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 14:48:18.000000 urdfeus-0.0.9/urdfeus/mesh2eus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-02 14:48:18.000000 urdfeus-0.0.9/urdfeus/read_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:48:28.168795 urdfeus-0.0.9/urdfeus/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-02 14:48:18.000000 urdfeus-0.0.9/urdfeus/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-04-02 14:48:18.000000 urdfeus-0.0.9/urdfeus/templates/euscollada-robot.l
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-02 14:48:18.000000 urdfeus-0.0.9/urdfeus/templates/urdf_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19120 2024-04-02 14:48:18.000000 urdfeus-0.0.9/urdfeus/urdf2eus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:48:28.168795 urdfeus-0.0.9/urdfeus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-02 14:48:28.000000 urdfeus-0.0.9/urdfeus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-02 14:48:28.000000 urdfeus-0.0.9/urdfeus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:48:28.000000 urdfeus-0.0.9/urdfeus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-02 14:48:28.000000 urdfeus-0.0.9/urdfeus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:48:28.000000 urdfeus-0.0.9/urdfeus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 14:48:28.000000 urdfeus-0.0.9/urdfeus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 14:48:28.000000 urdfeus-0.0.9/urdfeus.egg-info/top_level.txt
```

### Comparing `urdfeus-0.0.8/LICENSE` & `urdfeus-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `urdfeus-0.0.8/PKG-INFO` & `urdfeus-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urdfeus
-Version: 0.0.8
+Version: 0.0.9
 Summary: URDF converter for Euslisp
 Home-page: https://github.com/iory/urdfeus
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `urdfeus-0.0.8/setup.py` & `urdfeus-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "0.0.8"
+version = "0.0.9"
 
 
 if sys.argv[-1] == 'release':
     # Release via github-actions.
     commands = [
         'git tag v{:s}'.format(version),
         'git push origin master --tag',
```

### Comparing `urdfeus-0.0.8/urdfeus/apps/mesh2eus.py` & `urdfeus-0.0.9/urdfeus/apps/mesh2eus.py`

 * *Files identical despite different names*

### Comparing `urdfeus-0.0.8/urdfeus/apps/urdf2eus.py` & `urdfeus-0.0.9/urdfeus/apps/urdf2eus.py`

 * *Files identical despite different names*

### Comparing `urdfeus-0.0.8/urdfeus/common.py` & `urdfeus-0.0.9/urdfeus/common.py`

 * *Files identical despite different names*

### Comparing `urdfeus-0.0.8/urdfeus/mesh2eus.py` & `urdfeus-0.0.9/urdfeus/mesh2eus.py`

 * *Files identical despite different names*

### Comparing `urdfeus-0.0.8/urdfeus/read_yaml.py` & `urdfeus-0.0.9/urdfeus/read_yaml.py`

 * *Files identical despite different names*

### Comparing `urdfeus-0.0.8/urdfeus/templates/euscollada-robot.l` & `urdfeus-0.0.9/urdfeus/templates/euscollada-robot.l`

 * *Files identical despite different names*

### Comparing `urdfeus-0.0.8/urdfeus/templates/urdf_template.py` & `urdfeus-0.0.9/urdfeus/templates/urdf_template.py`

 * *Files identical despite different names*

### Comparing `urdfeus-0.0.8/urdfeus/urdf2eus.py` & `urdfeus-0.0.9/urdfeus/urdf2eus.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,17 +212,17 @@
                      fp=sys.stdout):
     limbs = []
     if config_yaml_path is not None:
         limbs = read_config_from_yaml(robot, config_yaml_path, fp=fp)
     else:
         print("     ;; links", file=fp)
         if add_link_suffix:
-            print(f"     (setq links (list {robot.__dict__['root_link'].name}_lk", end="", file=fp)  # NOQA
+            print(f"     (setq links (list ", end="", file=fp)  # NOQA
         else:
-            print(f"     (setq links (list {robot.__dict__['root_link'].name}", end="", file=fp)  # NOQA
+            print(f"     (setq links (list ", end="", file=fp)  # NOQA
 
         if add_link_suffix:
             for link in robot.link_list:
                 print(f" {link.name}_lk", end="", file=fp)
         else:
             for link in robot.link_list:
                 print(f" {link.name}", end="", file=fp)
```

### Comparing `urdfeus-0.0.8/urdfeus.egg-info/PKG-INFO` & `urdfeus-0.0.9/urdfeus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urdfeus
-Version: 0.0.8
+Version: 0.0.9
 Summary: URDF converter for Euslisp
 Home-page: https://github.com/iory/urdfeus
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `urdfeus-0.0.8/urdfeus.egg-info/SOURCES.txt` & `urdfeus-0.0.9/urdfeus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

