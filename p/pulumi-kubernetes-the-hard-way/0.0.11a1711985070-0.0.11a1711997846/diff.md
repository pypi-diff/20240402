# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.11a1711985070.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.11a1711997846.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.11a1711985070.tar", last modified: Mon Apr  1 15:26:09 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.11a1711997846.tar", last modified: Mon Apr  1 18:59:15 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070.tar` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:09.980953 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-01 15:26:09.980953 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:09.972953 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     2434 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)      334 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/_enums.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:09.976953 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      318 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      463 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)     4567 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     2843 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)    11932 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/etcd.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:09.976953 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)      295 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     8177 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)     6927 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/remote/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:09.976953 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      403 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)      942 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     1401 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    18602 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    14904 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4166 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)    15417 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:09.976953 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      369 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     8252 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    10335 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    19738 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    10270 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    11452 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    12663 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:09.980953 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-01 15:26:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-01 15:26:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:26:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 15:26:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 15:26:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      860 2024-04-01 15:26:02.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:26:09.980953 pulumi_kubernetes_the_hard_way-0.0.11a1711985070/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:15.220798 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-01 18:59:15.220798 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:15.216798 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     2285 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:15.216798 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      318 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      463 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     4567 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     2843 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:15.216798 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)      345 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      334 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     8177 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12010 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)     6927 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/remote/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:15.220798 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      403 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      942 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     1401 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    18602 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    14904 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4166 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)    15417 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:15.220798 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      369 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     8252 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    10335 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    19738 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    10270 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    11452 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    12663 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:15.220798 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-01 18:59:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-01 18:59:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:59:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 18:59:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 18:59:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      860 2024-04-01 18:59:09.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:59:15.220798 pulumi_kubernetes_the_hard_way-0.0.11a1711997846/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.11a1711985070
+Version: 0.0.11a1711997846
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/README.md` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-language-python. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
-from ._enums import *
-from .etcd import *
 from .provider import *
 
 # Make subpackages available:
 if typing.TYPE_CHECKING:
     import pulumi_kubernetes_the_hard_way.config as __config
     config = __config
     import pulumi_kubernetes_the_hard_way.remote as __remote
@@ -26,26 +24,19 @@
     tools = _utilities.lazy_import('pulumi_kubernetes_the_hard_way.tools')
 
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "kubernetes-the-hard-way",
-  "mod": "index",
-  "fqn": "pulumi_kubernetes_the_hard_way",
-  "classes": {
-   "kubernetes-the-hard-way:index:Etcd": "Etcd"
-  }
- },
- {
-  "pkg": "kubernetes-the-hard-way",
   "mod": "remote",
   "fqn": "pulumi_kubernetes_the_hard_way.remote",
   "classes": {
    "kubernetes-the-hard-way:remote:Download": "Download",
+   "kubernetes-the-hard-way:remote:EtcdInstall": "EtcdInstall",
    "kubernetes-the-hard-way:remote:File": "File"
   }
  },
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "tls",
   "fqn": "pulumi_kubernetes_the_hard_way.tls",
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
-from . import remote as _remote
-from . import tools as _tools
+from .. import _utilities
+from .. import tools as _tools
 from ._enums import *
+from .download import Download
 import pulumi_command
 
-__all__ = ['EtcdArgs', 'Etcd']
+__all__ = ['EtcdInstallArgs', 'EtcdInstall']
 
 @pulumi.input_type
-class EtcdArgs:
+class EtcdInstallArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  download_directory: Optional[pulumi.Input[str]] = None,
                  install_directory: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Etcd resource.
+        The set of arguments for constructing a EtcdInstall resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The connection details.
         :param pulumi.Input['Architecture'] architecture: The etcd CPU architecture.
         :param pulumi.Input[str] download_directory: Temporary directory to download files to. Defaults to `/tmp/<random string>`.
         :param pulumi.Input[str] install_directory: Directory to install the `etcd` and `etcdctl` binaries.
         :param pulumi.Input[str] version: The version of etcd to install.
         """
         pulumi.set(__self__, "connection", connection)
@@ -100,15 +100,15 @@
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
 
-class Etcd(pulumi.ComponentResource):
+class EtcdInstall(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  download_directory: Optional[pulumi.Input[str]] = None,
@@ -126,26 +126,26 @@
         :param pulumi.Input[str] install_directory: Directory to install the `etcd` and `etcdctl` binaries.
         :param pulumi.Input[str] version: The version of etcd to install.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: EtcdArgs,
+                 args: EtcdInstallArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Represents an etcd binary on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param EtcdArgs args: The arguments to use to populate this resource's properties.
+        :param EtcdInstallArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(EtcdArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(EtcdInstallArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -160,15 +160,15 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = EtcdArgs.__new__(EtcdArgs)
+            __props__ = EtcdInstallArgs.__new__(EtcdInstallArgs)
 
             __props__.__dict__["architecture"] = architecture
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["download_directory"] = download_directory
             if install_directory is None:
@@ -182,16 +182,16 @@
             __props__.__dict__["etcdctl_path"] = None
             __props__.__dict__["install_mkdir"] = None
             __props__.__dict__["mv_etcd"] = None
             __props__.__dict__["mv_etcdctl"] = None
             __props__.__dict__["name"] = None
             __props__.__dict__["tar"] = None
             __props__.__dict__["url"] = None
-        super(Etcd, __self__).__init__(
-            'kubernetes-the-hard-way:index:Etcd',
+        super(EtcdInstall, __self__).__init__(
+            'kubernetes-the-hard-way:remote:EtcdInstall',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
@@ -207,15 +207,15 @@
         """
         The name of the etcd release archive.
         """
         return pulumi.get(self, "archive_name")
 
     @property
     @pulumi.getter
-    def download(self) -> pulumi.Output['_remote.Download']:
+    def download(self) -> pulumi.Output['Download']:
         """
         The etcd download operation.
         """
         return pulumi.get(self, "download")
 
     @property
     @pulumi.getter(name="downloadDirectory")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.11a1711985070
+Version: 0.0.11a1711997846
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 README.md
 pyproject.toml
 pulumi_kubernetes_the_hard_way/__init__.py
-pulumi_kubernetes_the_hard_way/_enums.py
 pulumi_kubernetes_the_hard_way/_utilities.py
-pulumi_kubernetes_the_hard_way/etcd.py
 pulumi_kubernetes_the_hard_way/provider.py
 pulumi_kubernetes_the_hard_way/pulumi-plugin.json
 pulumi_kubernetes_the_hard_way/py.typed
 pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
 pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
 pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
 pulumi_kubernetes_the_hard_way.egg-info/requires.txt
 pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
 pulumi_kubernetes_the_hard_way/config/__init__.py
 pulumi_kubernetes_the_hard_way/config/_enums.py
 pulumi_kubernetes_the_hard_way/config/_inputs.py
 pulumi_kubernetes_the_hard_way/config/outputs.py
 pulumi_kubernetes_the_hard_way/remote/__init__.py
+pulumi_kubernetes_the_hard_way/remote/_enums.py
 pulumi_kubernetes_the_hard_way/remote/download.py
+pulumi_kubernetes_the_hard_way/remote/etcd_install.py
 pulumi_kubernetes_the_hard_way/remote/file.py
 pulumi_kubernetes_the_hard_way/tls/__init__.py
 pulumi_kubernetes_the_hard_way/tls/_enums.py
 pulumi_kubernetes_the_hard_way/tls/_inputs.py
 pulumi_kubernetes_the_hard_way/tls/certificate.py
 pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
 pulumi_kubernetes_the_hard_way/tls/encryption_key.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711985070/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.11a1711997846/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "pulumi-command>=0.9.0,<1.0.0", "pulumi-random>=4.0.0,<5.0.0", "pulumi-tls>=5.0.0,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.11a1711985070"
+  version = "0.0.11a1711997846"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

