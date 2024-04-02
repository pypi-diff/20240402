# Comparing `tmp/idds-client-2.1.8.tar.gz` & `tmp/idds-client-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-client-2.1.8.tar", last modified: Wed Jan 31 16:35:23 2024, max compression
+gzip compressed data, was "idds-client-2.1.9.tar", last modified: Wed Jan 31 17:27:21 2024, max compression
```

## Comparing `idds-client-2.1.8.tar` & `idds-client-2.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.907238 idds-client-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 16:35:12.000000 idds-client-2.1.8/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-01-31 16:35:23.907238 idds-client-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-31 16:35:12.000000 idds-client-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.903238 idds-client-2.1.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    15447 2024-01-31 16:35:12.000000 idds-client-2.1.8/bin/idds
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.903238 idds-client-2.1.8/etc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.903238 idds-client-2.1.8/etc/idds/
--rwxr-xr-x   0 runner    (1001) docker     (127)      649 2024-01-31 16:35:12.000000 idds-client-2.1.8/etc/idds/idds.cfg.client.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.903238 idds-client-2.1.8/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.903238 idds-client-2.1.8/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-client-2.1.8/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.907238 idds-client-2.1.8/lib/idds/client/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-client-2.1.8/lib/idds/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-01-31 16:35:12.000000 idds-client-2.1.8/lib/idds/client/authclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-01-31 16:35:12.000000 idds-client-2.1.8/lib/idds/client/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-01-31 16:35:12.000000 idds-client-2.1.8/lib/idds/client/cacherclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-01-31 16:35:12.000000 idds-client-2.1.8/lib/idds/client/catalogclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-01-31 16:35:12.000000 idds-client-2.1.8/lib/idds/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30096 2024-01-31 16:35:12.000000 idds-client-2.1.8/lib/idds/client/clientmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-01-31 16:35:12.000000 idds-client-2.1.8/lib/idds/client/hpoclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-01-31 16:35:12.000000 idds-client-2.1.8/lib/idds/client/logsclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-01-31 16:35:12.000000 idds-client-2.1.8/lib/idds/client/messageclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-01-31 16:35:12.000000 idds-client-2.1.8/lib/idds/client/pingclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-01-31 16:35:12.000000 idds-client-2.1.8/lib/idds/client/requestclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 16:35:22.000000 idds-client-2.1.8/lib/idds/client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.907238 idds-client-2.1.8/lib/idds_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-01-31 16:35:23.000000 idds-client-2.1.8/lib/idds_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-01-31 16:35:23.000000 idds-client-2.1.8/lib/idds_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 16:35:23.000000 idds-client-2.1.8/lib/idds_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-31 16:35:23.000000 idds-client-2.1.8/lib/idds_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 16:35:23.000000 idds-client-2.1.8/lib/idds_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 16:35:23.907238 idds-client-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-01-31 16:35:12.000000 idds-client-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.903238 idds-client-2.1.8/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.907238 idds-client-2.1.8/tools/env/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-31 16:35:22.000000 idds-client-2.1.8/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.209879 idds-client-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 17:27:09.000000 idds-client-2.1.9/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-01-31 17:27:21.209879 idds-client-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-31 17:27:09.000000 idds-client-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.205879 idds-client-2.1.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15447 2024-01-31 17:27:09.000000 idds-client-2.1.9/bin/idds
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.201879 idds-client-2.1.9/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.205879 idds-client-2.1.9/etc/idds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      649 2024-01-31 17:27:09.000000 idds-client-2.1.9/etc/idds/idds.cfg.client.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.201879 idds-client-2.1.9/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.205879 idds-client-2.1.9/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-client-2.1.9/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.205879 idds-client-2.1.9/lib/idds/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-client-2.1.9/lib/idds/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-01-31 17:27:09.000000 idds-client-2.1.9/lib/idds/client/authclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-01-31 17:27:09.000000 idds-client-2.1.9/lib/idds/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-01-31 17:27:09.000000 idds-client-2.1.9/lib/idds/client/cacherclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-01-31 17:27:09.000000 idds-client-2.1.9/lib/idds/client/catalogclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-01-31 17:27:09.000000 idds-client-2.1.9/lib/idds/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30096 2024-01-31 17:27:09.000000 idds-client-2.1.9/lib/idds/client/clientmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-01-31 17:27:09.000000 idds-client-2.1.9/lib/idds/client/hpoclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-01-31 17:27:09.000000 idds-client-2.1.9/lib/idds/client/logsclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-01-31 17:27:09.000000 idds-client-2.1.9/lib/idds/client/messageclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-01-31 17:27:09.000000 idds-client-2.1.9/lib/idds/client/pingclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-01-31 17:27:09.000000 idds-client-2.1.9/lib/idds/client/requestclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 17:27:19.000000 idds-client-2.1.9/lib/idds/client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.209879 idds-client-2.1.9/lib/idds_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-01-31 17:27:21.000000 idds-client-2.1.9/lib/idds_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-01-31 17:27:21.000000 idds-client-2.1.9/lib/idds_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 17:27:21.000000 idds-client-2.1.9/lib/idds_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-31 17:27:21.000000 idds-client-2.1.9/lib/idds_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 17:27:21.000000 idds-client-2.1.9/lib/idds_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 17:27:21.209879 idds-client-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-01-31 17:27:09.000000 idds-client-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.201879 idds-client-2.1.9/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.209879 idds-client-2.1.9/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-31 17:27:19.000000 idds-client-2.1.9/tools/env/environment.yml
```

### Comparing `idds-client-2.1.8/LICENSE.rst` & `idds-client-2.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/PKG-INFO` & `idds-client-2.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-client
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 Requires-Dist: pip
 Requires-Dist: requests
 Requires-Dist: urllib3
 Requires-Dist: tabulate
 Requires-Dist: argcomplete
-Requires-Dist: idds-common==2.1.8
-Requires-Dist: idds-workflow==2.1.8
+Requires-Dist: idds-common==2.1.9
+Requires-Dist: idds-workflow==2.1.9
 
 idds-client
 ====
 
 idds-client subpackage is for iDDS rest client.
```

### Comparing `idds-client-2.1.8/bin/idds` & `idds-client-2.1.9/bin/idds`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/etc/idds/idds.cfg.client.template` & `idds-client-2.1.9/etc/idds/idds.cfg.client.template`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/lib/idds/client/authclient.py` & `idds-client-2.1.9/lib/idds/client/authclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/lib/idds/client/base.py` & `idds-client-2.1.9/lib/idds/client/base.py`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/lib/idds/client/cacherclient.py` & `idds-client-2.1.9/lib/idds/client/cacherclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/lib/idds/client/catalogclient.py` & `idds-client-2.1.9/lib/idds/client/catalogclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/lib/idds/client/client.py` & `idds-client-2.1.9/lib/idds/client/client.py`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/lib/idds/client/clientmanager.py` & `idds-client-2.1.9/lib/idds/client/clientmanager.py`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/lib/idds/client/hpoclient.py` & `idds-client-2.1.9/lib/idds/client/hpoclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/lib/idds/client/logsclient.py` & `idds-client-2.1.9/lib/idds/client/logsclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/lib/idds/client/messageclient.py` & `idds-client-2.1.9/lib/idds/client/messageclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/lib/idds/client/pingclient.py` & `idds-client-2.1.9/lib/idds/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/lib/idds/client/requestclient.py` & `idds-client-2.1.9/lib/idds/client/requestclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/lib/idds_client.egg-info/PKG-INFO` & `idds-client-2.1.9/lib/idds_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-client
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 Requires-Dist: pip
 Requires-Dist: requests
 Requires-Dist: urllib3
 Requires-Dist: tabulate
 Requires-Dist: argcomplete
-Requires-Dist: idds-common==2.1.8
-Requires-Dist: idds-workflow==2.1.8
+Requires-Dist: idds-common==2.1.9
+Requires-Dist: idds-workflow==2.1.9
 
 idds-client
 ====
 
 idds-client subpackage is for iDDS rest client.
```

### Comparing `idds-client-2.1.8/lib/idds_client.egg-info/SOURCES.txt` & `idds-client-2.1.9/lib/idds_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-client-2.1.8/setup.py` & `idds-client-2.1.9/setup.py`

 * *Files identical despite different names*

