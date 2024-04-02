# Comparing `tmp/botocore-a-la-carte-emr-1.34.8.tar.gz` & `tmp/botocore-a-la-carte-emr-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-emr-1.34.8.tar", last modified: Wed Dec 27 01:06:42 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-emr-1.34.9.tar", last modified: Thu Dec 28 01:06:43 2023, max compression
```

## Comparing `botocore-a-la-carte-emr-1.34.8.tar` & `botocore-a-la-carte-emr-1.34.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:42.327312 botocore-a-la-carte-emr-1.34.8/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-27 01:06:42.000000 botocore-a-la-carte-emr-1.34.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-27 01:06:42.327312 botocore-a-la-carte-emr-1.34.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:42.323312 botocore-a-la-carte-emr-1.34.8/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:42.323312 botocore-a-la-carte-emr-1.34.8/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:42.323312 botocore-a-la-carte-emr-1.34.8/botocore/data/emr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:42.327312 botocore-a-la-carte-emr-1.34.8/botocore/data/emr/2009-03-31/
--rw-r--r--   0 runner    (1001) docker     (127)    15342 2023-12-27 01:06:29.000000 botocore-a-la-carte-emr-1.34.8/botocore/data/emr/2009-03-31/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-27 01:06:29.000000 botocore-a-la-carte-emr-1.34.8/botocore/data/emr/2009-03-31/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2023-12-27 01:06:29.000000 botocore-a-la-carte-emr-1.34.8/botocore/data/emr/2009-03-31/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   283950 2023-12-27 01:06:29.000000 botocore-a-la-carte-emr-1.34.8/botocore/data/emr/2009-03-31/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-12-27 01:06:29.000000 botocore-a-la-carte-emr-1.34.8/botocore/data/emr/2009-03-31/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:42.327312 botocore-a-la-carte-emr-1.34.8/botocore_a_la_carte_emr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-27 01:06:42.000000 botocore-a-la-carte-emr-1.34.8/botocore_a_la_carte_emr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-27 01:06:42.000000 botocore-a-la-carte-emr-1.34.8/botocore_a_la_carte_emr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 01:06:42.000000 botocore-a-la-carte-emr-1.34.8/botocore_a_la_carte_emr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-27 01:06:42.000000 botocore-a-la-carte-emr-1.34.8/botocore_a_la_carte_emr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 01:06:42.327312 botocore-a-la-carte-emr-1.34.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-12-27 01:06:42.000000 botocore-a-la-carte-emr-1.34.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.854295 botocore-a-la-carte-emr-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:43.000000 botocore-a-la-carte-emr-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-28 01:06:43.854295 botocore-a-la-carte-emr-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.850295 botocore-a-la-carte-emr-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.850295 botocore-a-la-carte-emr-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.850295 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.850295 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/
+-rw-r--r--   0 runner    (1001) docker     (127)    15342 2023-12-28 01:06:26.000000 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2023-12-28 01:06:26.000000 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   285772 2023-12-28 01:06:26.000000 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-12-28 01:06:26.000000 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.854295 botocore-a-la-carte-emr-1.34.9/botocore_a_la_carte_emr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-28 01:06:43.000000 botocore-a-la-carte-emr-1.34.9/botocore_a_la_carte_emr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-28 01:06:43.000000 botocore-a-la-carte-emr-1.34.9/botocore_a_la_carte_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:43.000000 botocore-a-la-carte-emr-1.34.9/botocore_a_la_carte_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:43.000000 botocore-a-la-carte-emr-1.34.9/botocore_a_la_carte_emr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:43.854295 botocore-a-la-carte-emr-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-12-28 01:06:43.000000 botocore-a-la-carte-emr-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-emr-1.34.8/LICENSE.txt` & `botocore-a-la-carte-emr-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-emr-1.34.8/PKG-INFO` & `botocore-a-la-carte-emr-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-emr
-Version: 1.34.8
+Version: 1.34.9
 Summary: emr data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-emr-1.34.8/botocore/data/emr/2009-03-31/endpoint-rule-set-1.json` & `botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-emr-1.34.8/botocore/data/emr/2009-03-31/paginators-1.json` & `botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-emr-1.34.8/botocore/data/emr/2009-03-31/service-2.json` & `botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997878787878788%*

 * *Differences: {"'operations'": "{'SetKeepJobFlowAliveWhenNoSteps': OrderedDict([('name', "*

 * *                 "'SetKeepJobFlowAliveWhenNoSteps'), ('http', OrderedDict([('method', 'POST'), "*

 * *                 "('requestUri', '/')])), ('input', OrderedDict([('shape', "*

 * *                 "'SetKeepJobFlowAliveWhenNoStepsInput')])), ('errors', [OrderedDict([('shape', "*

 * *                 "'InternalServerError')])]), ('documentation', '<p>You can use the "*

 * *                 '<code>SetKeepJobFlowAliveWhenNoSteps</code> to configure a  […]*

```diff
@@ -950,14 +950,30 @@
                 "shape": "RunJobFlowInput"
             },
             "name": "RunJobFlow",
             "output": {
                 "shape": "RunJobFlowOutput"
             }
         },
+        "SetKeepJobFlowAliveWhenNoSteps": {
+            "documentation": "<p>You can use the <code>SetKeepJobFlowAliveWhenNoSteps</code> to configure a cluster (job flow) to terminate after the step execution, i.e., all your steps are executed. If you want a transient cluster that shuts down after the last of the current executing steps are completed, you can configure <code>SetKeepJobFlowAliveWhenNoSteps</code> to false. If you want a long running cluster, configure <code>SetKeepJobFlowAliveWhenNoSteps</code> to true.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/emr/latest/ManagementGuide/UsingEMR_TerminationProtection.html\">Managing Cluster Termination</a> in the <i>Amazon EMR Management Guide</i>.</p>",
+            "errors": [
+                {
+                    "shape": "InternalServerError"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "SetKeepJobFlowAliveWhenNoStepsInput"
+            },
+            "name": "SetKeepJobFlowAliveWhenNoSteps"
+        },
         "SetTerminationProtection": {
             "documentation": "<p>SetTerminationProtection locks a cluster (job flow) so the Amazon EC2 instances in the cluster cannot be terminated by user intervention, an API call, or in the event of a job-flow error. The cluster still terminates upon successful completion of the job flow. Calling <code>SetTerminationProtection</code> on a cluster is similar to calling the Amazon EC2 <code>DisableAPITermination</code> API on all Amazon EC2 instances in a cluster.</p> <p> <code>SetTerminationProtection</code> is used to prevent accidental termination of a cluster and to ensure that in the event of an error, the instances persist so that you can recover any data stored in their ephemeral instance storage.</p> <p> To terminate a cluster that has been locked by setting <code>SetTerminationProtection</code> to <code>true</code>, you must first unlock the job flow by a subsequent call to <code>SetTerminationProtection</code> in which you set the value to <code>false</code>. </p> <p> For more information, see<a href=\"https://docs.aws.amazon.com/emr/latest/ManagementGuide/UsingEMR_TerminationProtection.html\">Managing Cluster Termination</a> in the <i>Amazon EMR Management Guide</i>. </p>",
             "errors": [
                 {
                     "shape": "InternalServerError"
                 }
             ],
@@ -5385,14 +5401,31 @@
         },
         "SessionMappingSummaryList": {
             "member": {
                 "shape": "SessionMappingSummary"
             },
             "type": "list"
         },
+        "SetKeepJobFlowAliveWhenNoStepsInput": {
+            "members": {
+                "JobFlowIds": {
+                    "documentation": "<p>A list of strings that uniquely identify the clusters to protect. This identifier is returned by <a href=\"https://docs.aws.amazon.com/emr/latest/APIReference/API_RunJobFlow.html\">RunJobFlow</a> and can also be obtained from <a href=\"https://docs.aws.amazon.com/emr/latest/APIReference/API_DescribeJobFlows.html\">DescribeJobFlows</a>.</p>",
+                    "shape": "XmlStringList"
+                },
+                "KeepJobFlowAliveWhenNoSteps": {
+                    "documentation": "<p>A Boolean that indicates whether to terminate the cluster after all steps are executed.</p>",
+                    "shape": "Boolean"
+                }
+            },
+            "required": [
+                "JobFlowIds",
+                "KeepJobFlowAliveWhenNoSteps"
+            ],
+            "type": "structure"
+        },
         "SetTerminationProtectionInput": {
             "documentation": "<p> The input argument to the <a>TerminationProtection</a> operation. </p>",
             "members": {
                 "JobFlowIds": {
                     "documentation": "<p> A list of strings that uniquely identify the clusters to protect. This identifier is returned by <a>RunJobFlow</a> and can also be obtained from <a>DescribeJobFlows</a> . </p>",
                     "shape": "XmlStringList"
                 },
```

### Comparing `botocore-a-la-carte-emr-1.34.8/botocore/data/emr/2009-03-31/waiters-2.json` & `botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-emr-1.34.8/botocore_a_la_carte_emr.egg-info/PKG-INFO` & `botocore-a-la-carte-emr-1.34.9/botocore_a_la_carte_emr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-emr
-Version: 1.34.8
+Version: 1.34.9
 Summary: emr data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-emr-1.34.8/setup.py` & `botocore-a-la-carte-emr-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-emr',
-    version="1.34.8",
+    version="1.34.9",
     description='emr data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/emr/*/*.json'],
```

