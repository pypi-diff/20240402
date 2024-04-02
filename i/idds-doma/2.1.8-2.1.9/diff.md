# Comparing `tmp/idds-doma-2.1.8.tar.gz` & `tmp/idds-doma-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-doma-2.1.8.tar", last modified: Wed Jan 31 16:35:25 2024, max compression
+gzip compressed data, was "idds-doma-2.1.9.tar", last modified: Wed Jan 31 17:27:22 2024, max compression
```

## Comparing `idds-doma-2.1.8.tar` & `idds-doma-2.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.411245 idds-doma-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 16:35:12.000000 idds-doma-2.1.8/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-31 16:35:25.411245 idds-doma-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-31 16:35:12.000000 idds-doma-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.407245 idds-doma-2.1.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      747 2024-01-31 16:35:12.000000 idds-doma-2.1.8/bin/setup_panda_token
--rwxr-xr-x   0 runner    (1001) docker     (127)    10028 2024-01-31 16:35:12.000000 idds-doma-2.1.8/bin/setup_panda_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.407245 idds-doma-2.1.8/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.407245 idds-doma-2.1.8/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-doma-2.1.8/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.407245 idds-doma-2.1.8/lib/idds/doma/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-doma-2.1.8/lib/idds/doma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 16:35:22.000000 idds-doma-2.1.8/lib/idds/doma/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.407245 idds-doma-2.1.8/lib/idds/doma/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-doma-2.1.8/lib/idds/doma/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56124 2024-01-31 16:35:12.000000 idds-doma-2.1.8/lib/idds/doma/workflow/domapandawork.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.407245 idds-doma-2.1.8/lib/idds/doma/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-doma-2.1.8/lib/idds/doma/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-01-31 16:35:12.000000 idds-doma-2.1.8/lib/idds/doma/workflowv2/domaeventmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    39387 2024-01-31 16:35:12.000000 idds-doma-2.1.8/lib/idds/doma/workflowv2/domapandaeswork.py
--rw-r--r--   0 runner    (1001) docker     (127)   100504 2024-01-31 16:35:12.000000 idds-doma-2.1.8/lib/idds/doma/workflowv2/domapandawork.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-01-31 16:35:12.000000 idds-doma-2.1.8/lib/idds/doma/workflowv2/domatree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.411245 idds-doma-2.1.8/lib/idds_doma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-31 16:35:25.000000 idds-doma-2.1.8/lib/idds_doma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-31 16:35:25.000000 idds-doma-2.1.8/lib/idds_doma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 16:35:25.000000 idds-doma-2.1.8/lib/idds_doma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-31 16:35:25.000000 idds-doma-2.1.8/lib/idds_doma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 16:35:25.000000 idds-doma-2.1.8/lib/idds_doma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 16:35:25.411245 idds-doma-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-01-31 16:35:12.000000 idds-doma-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.407245 idds-doma-2.1.8/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.411245 idds-doma-2.1.8/tools/env/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-31 16:35:22.000000 idds-doma-2.1.8/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.697888 idds-doma-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 17:27:09.000000 idds-doma-2.1.9/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-31 17:27:22.697888 idds-doma-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-31 17:27:09.000000 idds-doma-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.693888 idds-doma-2.1.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      747 2024-01-31 17:27:09.000000 idds-doma-2.1.9/bin/setup_panda_token
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10028 2024-01-31 17:27:09.000000 idds-doma-2.1.9/bin/setup_panda_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.689888 idds-doma-2.1.9/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.693888 idds-doma-2.1.9/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-doma-2.1.9/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.693888 idds-doma-2.1.9/lib/idds/doma/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-doma-2.1.9/lib/idds/doma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 17:27:19.000000 idds-doma-2.1.9/lib/idds/doma/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.693888 idds-doma-2.1.9/lib/idds/doma/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-doma-2.1.9/lib/idds/doma/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56124 2024-01-31 17:27:09.000000 idds-doma-2.1.9/lib/idds/doma/workflow/domapandawork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.693888 idds-doma-2.1.9/lib/idds/doma/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-doma-2.1.9/lib/idds/doma/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-01-31 17:27:09.000000 idds-doma-2.1.9/lib/idds/doma/workflowv2/domaeventmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39387 2024-01-31 17:27:09.000000 idds-doma-2.1.9/lib/idds/doma/workflowv2/domapandaeswork.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100504 2024-01-31 17:27:09.000000 idds-doma-2.1.9/lib/idds/doma/workflowv2/domapandawork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-01-31 17:27:09.000000 idds-doma-2.1.9/lib/idds/doma/workflowv2/domatree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.697888 idds-doma-2.1.9/lib/idds_doma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-31 17:27:22.000000 idds-doma-2.1.9/lib/idds_doma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-31 17:27:22.000000 idds-doma-2.1.9/lib/idds_doma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 17:27:22.000000 idds-doma-2.1.9/lib/idds_doma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-31 17:27:22.000000 idds-doma-2.1.9/lib/idds_doma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 17:27:22.000000 idds-doma-2.1.9/lib/idds_doma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 17:27:22.697888 idds-doma-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-01-31 17:27:09.000000 idds-doma-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.693888 idds-doma-2.1.9/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.697888 idds-doma-2.1.9/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-31 17:27:19.000000 idds-doma-2.1.9/tools/env/environment.yml
```

### Comparing `idds-doma-2.1.8/LICENSE.rst` & `idds-doma-2.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-doma-2.1.8/PKG-INFO` & `idds-doma-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 Requires-Dist: pip
 Requires-Dist: futures
 Requires-Dist: panda-client-light
-Requires-Dist: idds-common==2.1.8
-Requires-Dist: idds-workflow==2.1.8
+Requires-Dist: idds-common==2.1.9
+Requires-Dist: idds-workflow==2.1.9
 
 idds-doma
 ====
 
 idds-doma subpackage is for DOMA hep specific functions and plugins.
 With it, iDDS can support DOMA LSST workflows.
```

### Comparing `idds-doma-2.1.8/bin/setup_panda_token` & `idds-doma-2.1.9/bin/setup_panda_token`

 * *Files identical despite different names*

### Comparing `idds-doma-2.1.8/bin/setup_panda_token.py` & `idds-doma-2.1.9/bin/setup_panda_token.py`

 * *Files identical despite different names*

### Comparing `idds-doma-2.1.8/lib/idds/doma/workflow/domapandawork.py` & `idds-doma-2.1.9/lib/idds/doma/workflow/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-2.1.8/lib/idds/doma/workflowv2/domaeventmap.py` & `idds-doma-2.1.9/lib/idds/doma/workflowv2/domaeventmap.py`

 * *Files identical despite different names*

### Comparing `idds-doma-2.1.8/lib/idds/doma/workflowv2/domapandaeswork.py` & `idds-doma-2.1.9/lib/idds/doma/workflowv2/domapandaeswork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-2.1.8/lib/idds/doma/workflowv2/domapandawork.py` & `idds-doma-2.1.9/lib/idds/doma/workflowv2/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-2.1.8/lib/idds/doma/workflowv2/domatree.py` & `idds-doma-2.1.9/lib/idds/doma/workflowv2/domatree.py`

 * *Files identical despite different names*

### Comparing `idds-doma-2.1.8/lib/idds_doma.egg-info/PKG-INFO` & `idds-doma-2.1.9/lib/idds_doma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 Requires-Dist: pip
 Requires-Dist: futures
 Requires-Dist: panda-client-light
-Requires-Dist: idds-common==2.1.8
-Requires-Dist: idds-workflow==2.1.8
+Requires-Dist: idds-common==2.1.9
+Requires-Dist: idds-workflow==2.1.9
 
 idds-doma
 ====
 
 idds-doma subpackage is for DOMA hep specific functions and plugins.
 With it, iDDS can support DOMA LSST workflows.
```

### Comparing `idds-doma-2.1.8/lib/idds_doma.egg-info/SOURCES.txt` & `idds-doma-2.1.9/lib/idds_doma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-doma-2.1.8/setup.py` & `idds-doma-2.1.9/setup.py`

 * *Files identical despite different names*

