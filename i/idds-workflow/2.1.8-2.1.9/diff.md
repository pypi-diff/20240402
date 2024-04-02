# Comparing `tmp/idds-workflow-2.1.8.tar.gz` & `tmp/idds-workflow-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-workflow-2.1.8.tar", last modified: Wed Jan 31 16:35:24 2024, max compression
+gzip compressed data, was "idds-workflow-2.1.9.tar", last modified: Wed Jan 31 17:27:22 2024, max compression
```

## Comparing `idds-workflow-2.1.8.tar` & `idds-workflow-2.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.907243 idds-workflow-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-01-31 16:35:24.907243 idds-workflow-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.899243 idds-workflow-2.1.8/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.903243 idds-workflow-2.1.8/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.903243 idds-workflow-2.1.8/lib/idds/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflow/datawork.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflow/processingwork.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 16:35:22.000000 idds-workflow-2.1.8/lib/idds/workflow/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    80759 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflow/work.py
--rw-r--r--   0 runner    (1001) docker     (127)    91897 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.903243 idds-workflow-2.1.8/lib/idds/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflowv2/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflowv2/datawork.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflowv2/processingwork.py
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflowv2/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflowv2/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflowv2/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    82190 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflowv2/work.py
--rw-r--r--   0 runner    (1001) docker     (127)   106661 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/lib/idds/workflowv2/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.907243 idds-workflow-2.1.8/lib/idds_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-01-31 16:35:24.000000 idds-workflow-2.1.8/lib/idds_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-01-31 16:35:24.000000 idds-workflow-2.1.8/lib/idds_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 16:35:24.000000 idds-workflow-2.1.8/lib/idds_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-31 16:35:24.000000 idds-workflow-2.1.8/lib/idds_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 16:35:24.000000 idds-workflow-2.1.8/lib/idds_workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 16:35:24.907243 idds-workflow-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-01-31 16:35:12.000000 idds-workflow-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.899243 idds-workflow-2.1.8/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.907243 idds-workflow-2.1.8/tools/env/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-31 16:35:22.000000 idds-workflow-2.1.8/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.197885 idds-workflow-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-01-31 17:27:22.197885 idds-workflow-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.189885 idds-workflow-2.1.9/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.189885 idds-workflow-2.1.9/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.193885 idds-workflow-2.1.9/lib/idds/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflow/datawork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflow/processingwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 17:27:19.000000 idds-workflow-2.1.9/lib/idds/workflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80759 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflow/work.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91897 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.193885 idds-workflow-2.1.9/lib/idds/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflowv2/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflowv2/datawork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflowv2/processingwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflowv2/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflowv2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflowv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82190 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflowv2/work.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106661 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/lib/idds/workflowv2/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.197885 idds-workflow-2.1.9/lib/idds_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-01-31 17:27:22.000000 idds-workflow-2.1.9/lib/idds_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-01-31 17:27:22.000000 idds-workflow-2.1.9/lib/idds_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 17:27:22.000000 idds-workflow-2.1.9/lib/idds_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-31 17:27:22.000000 idds-workflow-2.1.9/lib/idds_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 17:27:22.000000 idds-workflow-2.1.9/lib/idds_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 17:27:22.197885 idds-workflow-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-01-31 17:27:09.000000 idds-workflow-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.189885 idds-workflow-2.1.9/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:22.197885 idds-workflow-2.1.9/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-31 17:27:19.000000 idds-workflow-2.1.9/tools/env/environment.yml
```

### Comparing `idds-workflow-2.1.8/LICENSE.rst` & `idds-workflow-2.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/PKG-INFO` & `idds-workflow-2.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-workflow
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,13 +13,13 @@
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 Requires-Dist: pip
 Requires-Dist: anytree
 Requires-Dist: networkx
-Requires-Dist: idds-common==2.1.8
+Requires-Dist: idds-common==2.1.9
 
 idds-workflow
 ====
 
 idds-workflow subpackage implements basic workflow and a DAG(Directed Acyclic Graph) workflow.
```

### Comparing `idds-workflow-2.1.8/lib/idds/workflow/base.py` & `idds-workflow-2.1.9/lib/idds/workflow/base.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/lib/idds/workflow/datawork.py` & `idds-workflow-2.1.9/lib/idds/workflow/datawork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/lib/idds/workflow/processingwork.py` & `idds-workflow-2.1.9/lib/idds/workflow/processingwork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/lib/idds/workflow/utils.py` & `idds-workflow-2.1.9/lib/idds/workflow/utils.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/lib/idds/workflow/work.py` & `idds-workflow-2.1.9/lib/idds/workflow/work.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/lib/idds/workflow/workflow.py` & `idds-workflow-2.1.9/lib/idds/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/lib/idds/workflowv2/base.py` & `idds-workflow-2.1.9/lib/idds/workflowv2/base.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/lib/idds/workflowv2/datawork.py` & `idds-workflow-2.1.9/lib/idds/workflowv2/datawork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/lib/idds/workflowv2/processingwork.py` & `idds-workflow-2.1.9/lib/idds/workflowv2/processingwork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/lib/idds/workflowv2/tree.py` & `idds-workflow-2.1.9/lib/idds/workflowv2/tree.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/lib/idds/workflowv2/utils.py` & `idds-workflow-2.1.9/lib/idds/workflowv2/utils.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/lib/idds/workflowv2/work.py` & `idds-workflow-2.1.9/lib/idds/workflowv2/work.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/lib/idds/workflowv2/workflow.py` & `idds-workflow-2.1.9/lib/idds/workflowv2/workflow.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/lib/idds_workflow.egg-info/PKG-INFO` & `idds-workflow-2.1.9/lib/idds_workflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-workflow
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,13 +13,13 @@
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 Requires-Dist: pip
 Requires-Dist: anytree
 Requires-Dist: networkx
-Requires-Dist: idds-common==2.1.8
+Requires-Dist: idds-common==2.1.9
 
 idds-workflow
 ====
 
 idds-workflow subpackage implements basic workflow and a DAG(Directed Acyclic Graph) workflow.
```

### Comparing `idds-workflow-2.1.8/lib/idds_workflow.egg-info/SOURCES.txt` & `idds-workflow-2.1.9/lib/idds_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-workflow-2.1.8/setup.py` & `idds-workflow-2.1.9/setup.py`

 * *Files identical despite different names*

