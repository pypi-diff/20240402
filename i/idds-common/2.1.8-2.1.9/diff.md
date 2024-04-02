# Comparing `tmp/idds-common-2.1.8.tar.gz` & `tmp/idds-common-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-common-2.1.8.tar", last modified: Wed Jan 31 16:35:22 2024, max compression
+gzip compressed data, was "idds-common-2.1.9.tar", last modified: Wed Jan 31 17:27:19 2024, max compression
```

## Comparing `idds-common-2.1.8.tar` & `idds-common-2.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:22.579231 idds-common-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 16:35:12.000000 idds-common-2.1.8/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-31 16:35:22.579231 idds-common-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-31 16:35:12.000000 idds-common-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:22.571231 idds-common-2.1.8/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:22.575231 idds-common-2.1.8/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:22.575231 idds-common-2.1.8/lib/idds/common/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24353 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/common/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/common/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/common/dict_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    16087 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/common/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:22.575231 idds-common-2.1.8/lib/idds/common/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/common/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/common/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/common/plugin/plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/common/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20151 2024-01-31 16:35:12.000000 idds-common-2.1.8/lib/idds/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 16:35:22.000000 idds-common-2.1.8/lib/idds/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:22.579231 idds-common-2.1.8/lib/idds_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-31 16:35:22.000000 idds-common-2.1.8/lib/idds_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-01-31 16:35:22.000000 idds-common-2.1.8/lib/idds_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 16:35:22.000000 idds-common-2.1.8/lib/idds_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-31 16:35:22.000000 idds-common-2.1.8/lib/idds_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 16:35:22.000000 idds-common-2.1.8/lib/idds_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 16:35:22.579231 idds-common-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-01-31 16:35:12.000000 idds-common-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:22.571231 idds-common-2.1.8/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:22.579231 idds-common-2.1.8/tools/env/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-31 16:35:22.000000 idds-common-2.1.8/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:19.917872 idds-common-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 17:27:09.000000 idds-common-2.1.9/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-31 17:27:19.917872 idds-common-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-31 17:27:09.000000 idds-common-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:19.913872 idds-common-2.1.9/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:19.913872 idds-common-2.1.9/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:19.913872 idds-common-2.1.9/lib/idds/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24353 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/common/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/common/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/common/dict_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16087 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/common/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:19.917872 idds-common-2.1.9/lib/idds/common/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/common/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/common/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/common/plugin/plugin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/common/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20151 2024-01-31 17:27:09.000000 idds-common-2.1.9/lib/idds/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 17:27:19.000000 idds-common-2.1.9/lib/idds/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:19.917872 idds-common-2.1.9/lib/idds_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-31 17:27:19.000000 idds-common-2.1.9/lib/idds_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-01-31 17:27:19.000000 idds-common-2.1.9/lib/idds_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 17:27:19.000000 idds-common-2.1.9/lib/idds_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-31 17:27:19.000000 idds-common-2.1.9/lib/idds_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 17:27:19.000000 idds-common-2.1.9/lib/idds_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 17:27:19.917872 idds-common-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-01-31 17:27:09.000000 idds-common-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:19.913872 idds-common-2.1.9/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:19.917872 idds-common-2.1.9/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-31 17:27:19.000000 idds-common-2.1.9/tools/env/environment.yml
```

### Comparing `idds-common-2.1.8/LICENSE.rst` & `idds-common-2.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-common-2.1.8/PKG-INFO` & `idds-common-2.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-common
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-common-2.1.8/lib/idds/common/authentication.py` & `idds-common-2.1.9/lib/idds/common/authentication.py`

 * *Files identical despite different names*

### Comparing `idds-common-2.1.8/lib/idds/common/cache.py` & `idds-common-2.1.9/lib/idds/common/cache.py`

 * *Files identical despite different names*

### Comparing `idds-common-2.1.8/lib/idds/common/config.py` & `idds-common-2.1.9/lib/idds/common/config.py`

 * *Files identical despite different names*

### Comparing `idds-common-2.1.8/lib/idds/common/constants.py` & `idds-common-2.1.9/lib/idds/common/constants.py`

 * *Files identical despite different names*

### Comparing `idds-common-2.1.8/lib/idds/common/dict_class.py` & `idds-common-2.1.9/lib/idds/common/dict_class.py`

 * *Files identical despite different names*

### Comparing `idds-common-2.1.8/lib/idds/common/event.py` & `idds-common-2.1.9/lib/idds/common/event.py`

 * *Files identical despite different names*

### Comparing `idds-common-2.1.8/lib/idds/common/exceptions.py` & `idds-common-2.1.9/lib/idds/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `idds-common-2.1.8/lib/idds/common/plugin/plugin_base.py` & `idds-common-2.1.9/lib/idds/common/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `idds-common-2.1.8/lib/idds/common/plugin/plugin_utils.py` & `idds-common-2.1.9/lib/idds/common/plugin/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-2.1.8/lib/idds/common/status_utils.py` & `idds-common-2.1.9/lib/idds/common/status_utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-2.1.8/lib/idds/common/utils.py` & `idds-common-2.1.9/lib/idds/common/utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-2.1.8/lib/idds_common.egg-info/PKG-INFO` & `idds-common-2.1.9/lib/idds_common.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-common
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-common-2.1.8/lib/idds_common.egg-info/SOURCES.txt` & `idds-common-2.1.9/lib/idds_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-common-2.1.8/setup.py` & `idds-common-2.1.9/setup.py`

 * *Files identical despite different names*

