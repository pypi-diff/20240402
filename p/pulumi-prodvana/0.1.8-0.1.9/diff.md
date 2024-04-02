# Comparing `tmp/pulumi_prodvana-0.1.8.tar.gz` & `tmp/pulumi_prodvana-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_prodvana-0.1.8.tar", last modified: Sat Jul 29 00:20:32 2023, max compression
+gzip compressed data, was "pulumi_prodvana-0.1.9.tar", last modified: Sat Jul 29 01:45:51 2023, max compression
```

## Comparing `pulumi_prodvana-0.1.8.tar` & `pulumi_prodvana-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:20:32.886030 pulumi_prodvana-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-29 00:20:32.882030 pulumi_prodvana-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:20:32.882030 pulumi_prodvana-0.1.8/pulumi_prodvana/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93070 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:20:32.882030 pulumi_prodvana-0.1.8/pulumi_prodvana/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/get_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/get_k8s_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/get_release_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/k8s_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    47464 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/managed_k8s_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    82295 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33965 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/release_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/runtime_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:20:32.882030 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:20:32.886030 pulumi_prodvana-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:45:51.177981 pulumi_prodvana-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-29 01:45:51.177981 pulumi_prodvana-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:45:51.177981 pulumi_prodvana-0.1.9/pulumi_prodvana/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93070 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:45:51.177981 pulumi_prodvana-0.1.9/pulumi_prodvana/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/get_k8s_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/get_release_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/k8s_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47464 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/managed_k8s_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82295 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33965 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/release_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/pulumi_prodvana/runtime_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:45:51.177981 pulumi_prodvana-0.1.9/pulumi_prodvana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-29 01:45:51.000000 pulumi_prodvana-0.1.9/pulumi_prodvana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-29 01:45:51.000000 pulumi_prodvana-0.1.9/pulumi_prodvana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 01:45:51.000000 pulumi_prodvana-0.1.9/pulumi_prodvana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 01:45:51.000000 pulumi_prodvana-0.1.9/pulumi_prodvana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 01:45:51.000000 pulumi_prodvana-0.1.9/pulumi_prodvana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 01:45:51.000000 pulumi_prodvana-0.1.9/pulumi_prodvana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 01:45:51.177981 pulumi_prodvana-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-29 01:45:50.000000 pulumi_prodvana-0.1.9/setup.py
```

### Comparing `pulumi_prodvana-0.1.8/PKG-INFO` & `pulumi_prodvana-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_prodvana
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Pulumi package for creating and managing Prodvana cloud resources.
 Home-page: https://prodvana.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/prodvana/pulumi-prodvana
 Keywords: pulumi prodvana category/cloud category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_prodvana-0.1.8/README.md` & `pulumi_prodvana-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/__init__.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/_inputs.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/_utilities.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,8 +243,8 @@
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
 def get_plugin_download_url():
-	return "https://github.com/prodvana/pulumi-prodvana/releases"
+	return "github://api.github.com/prodvana"
```

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/application.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/application.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/config/vars.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/get_application.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/get_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/get_k8s_runtime.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/get_k8s_runtime.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/get_release_channel.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/get_release_channel.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/k8s_runtime.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/k8s_runtime.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/managed_k8s_runtime.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/managed_k8s_runtime.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/outputs.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/provider.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/release_channel.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/release_channel.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana/runtime_link.py` & `pulumi_prodvana-0.1.9/pulumi_prodvana/runtime_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/PKG-INFO` & `pulumi_prodvana-0.1.9/pulumi_prodvana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-prodvana
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Pulumi package for creating and managing Prodvana cloud resources.
 Home-page: https://prodvana.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/prodvana/pulumi-prodvana
 Keywords: pulumi prodvana category/cloud category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/SOURCES.txt` & `pulumi_prodvana-0.1.9/pulumi_prodvana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.8/setup.py` & `pulumi_prodvana-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.8"
-PLUGIN_VERSION = "0.1.8"
+VERSION = "0.1.9"
+PLUGIN_VERSION = "0.1.9"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'prodvana', PLUGIN_VERSION, '--server', 'https://github.com/prodvana/pulumi-prodvana/releases'])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'prodvana', PLUGIN_VERSION, '--server', 'github://api.github.com/prodvana'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the prodvana resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
```

