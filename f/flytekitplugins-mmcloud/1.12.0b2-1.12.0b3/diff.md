# Comparing `tmp/flytekitplugins-mmcloud-1.12.0b2.tar.gz` & `tmp/flytekitplugins-mmcloud-1.12.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-mmcloud-1.12.0b2.tar", last modified: Fri Mar 29 21:24:55 2024, max compression
+gzip compressed data, was "flytekitplugins-mmcloud-1.12.0b3.tar", last modified: Tue Apr  2 21:31:34 2024, max compression
```

## Comparing `flytekitplugins-mmcloud-1.12.0b2.tar` & `flytekitplugins-mmcloud-1.12.0b3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:55.520307 flytekitplugins-mmcloud-1.12.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-03-29 21:24:55.520307 flytekitplugins-mmcloud-1.12.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-03-29 21:24:26.000000 flytekitplugins-mmcloud-1.12.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:55.516307 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:55.520307 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins/mmcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-29 21:24:26.000000 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins/mmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-03-29 21:24:26.000000 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins/mmcloud/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-03-29 21:24:26.000000 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins/mmcloud/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-03-29 21:24:26.000000 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins/mmcloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:55.520307 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins_mmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-03-29 21:24:55.000000 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins_mmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-29 21:24:55.000000 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins_mmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 21:24:55.000000 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins_mmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-29 21:24:55.000000 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins_mmcloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 21:24:55.000000 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins_mmcloud.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-29 21:24:55.000000 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins_mmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 21:24:55.000000 flytekitplugins-mmcloud-1.12.0b2/flytekitplugins_mmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 21:24:55.520307 flytekitplugins-mmcloud-1.12.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-29 21:24:49.000000 flytekitplugins-mmcloud-1.12.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:24:55.520307 flytekitplugins-mmcloud-1.12.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-03-29 21:24:26.000000 flytekitplugins-mmcloud-1.12.0b2/tests/test_mmcloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:34.293184 flytekitplugins-mmcloud-1.12.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-02 21:31:34.293184 flytekitplugins-mmcloud-1.12.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-02 21:31:04.000000 flytekitplugins-mmcloud-1.12.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:34.289183 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:34.293184 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins/mmcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-02 21:31:04.000000 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins/mmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-02 21:31:04.000000 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins/mmcloud/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-02 21:31:04.000000 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins/mmcloud/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-02 21:31:04.000000 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins/mmcloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:34.293184 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins_mmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-02 21:31:34.000000 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins_mmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-02 21:31:34.000000 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins_mmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:31:34.000000 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins_mmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 21:31:34.000000 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins_mmcloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 21:31:34.000000 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins_mmcloud.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 21:31:34.000000 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins_mmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 21:31:34.000000 flytekitplugins-mmcloud-1.12.0b3/flytekitplugins_mmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:31:34.293184 flytekitplugins-mmcloud-1.12.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-02 21:31:28.000000 flytekitplugins-mmcloud-1.12.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:34.293184 flytekitplugins-mmcloud-1.12.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-02 21:31:04.000000 flytekitplugins-mmcloud-1.12.0b3/tests/test_mmcloud.py
```

### Comparing `flytekitplugins-mmcloud-1.12.0b2/PKG-INFO` & `flytekitplugins-mmcloud-1.12.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-mmcloud
-Version: 1.12.0b2
+Version: 1.12.0b3
 Summary: MemVerge Flyte plugin
 Author: Edwin Yu, Helen Zhang
 Author-email: helen.zhang@memverge.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-mmcloud-1.12.0b2/README.md` & `flytekitplugins-mmcloud-1.12.0b3/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-mmcloud-1.12.0b2/flytekitplugins/mmcloud/agent.py` & `flytekitplugins-mmcloud-1.12.0b3/flytekitplugins/mmcloud/agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-mmcloud-1.12.0b2/flytekitplugins/mmcloud/task.py` & `flytekitplugins-mmcloud-1.12.0b3/flytekitplugins/mmcloud/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-mmcloud-1.12.0b2/flytekitplugins/mmcloud/utils.py` & `flytekitplugins-mmcloud-1.12.0b3/flytekitplugins/mmcloud/utils.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-mmcloud-1.12.0b2/flytekitplugins_mmcloud.egg-info/PKG-INFO` & `flytekitplugins-mmcloud-1.12.0b3/flytekitplugins_mmcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-mmcloud
-Version: 1.12.0b2
+Version: 1.12.0b3
 Summary: MemVerge Flyte plugin
 Author: Edwin Yu, Helen Zhang
 Author-email: helen.zhang@memverge.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-mmcloud-1.12.0b2/flytekitplugins_mmcloud.egg-info/SOURCES.txt` & `flytekitplugins-mmcloud-1.12.0b3/flytekitplugins_mmcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins-mmcloud-1.12.0b2/setup.py` & `flytekitplugins-mmcloud-1.12.0b3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "mmcloud"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.9.1,<2.0.0", "kubernetes"]
 
-__version__ = "1.12.0b2"
+__version__ = "1.12.0b3"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Edwin Yu, Helen Zhang",
     author_email="helen.zhang@memverge.com",
     description="MemVerge Flyte plugin",
```

### Comparing `flytekitplugins-mmcloud-1.12.0b2/tests/test_mmcloud.py` & `flytekitplugins-mmcloud-1.12.0b3/tests/test_mmcloud.py`

 * *Files identical despite different names*

