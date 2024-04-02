# Comparing `tmp/cf-remote-0.4.8.tar.gz` & `tmp/cf-remote-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf-remote-0.4.8.tar", last modified: Fri Jun 16 16:22:57 2023, max compression
+gzip compressed data, was "cf-remote-0.4.9.tar", last modified: Mon Jul  3 16:51:09 2023, max compression
```

## Comparing `cf-remote-0.4.8.tar` & `cf-remote-0.4.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:22:57.906336 cf-remote-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 16:22:47.000000 cf-remote-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-16 16:22:57.906336 cf-remote-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-06-16 16:22:47.000000 cf-remote-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:22:57.906336 cf-remote-0.4.8/cf_remote/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 16:22:57.000000 cf-remote-0.4.8/cf_remote/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/aramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/cloud_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    26809 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    14132 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-16 16:22:47.000000 cf-remote-0.4.8/cf_remote/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:22:57.906336 cf-remote-0.4.8/cf_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-16 16:22:57.000000 cf-remote-0.4.8/cf_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-16 16:22:57.000000 cf-remote-0.4.8/cf_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:22:57.000000 cf-remote-0.4.8/cf_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 16:22:57.000000 cf-remote-0.4.8/cf_remote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 16:22:57.000000 cf-remote-0.4.8/cf_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 16:22:57.000000 cf-remote-0.4.8/cf_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:22:57.906336 cf-remote-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-16 16:22:47.000000 cf-remote-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:22:57.906336 cf-remote-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:22:47.000000 cf-remote-0.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-16 16:22:47.000000 cf-remote-0.4.8/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-16 16:22:47.000000 cf-remote-0.4.8/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-16 16:22:47.000000 cf-remote-0.4.8/tests/test_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:51:08.996538 cf-remote-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 16:50:57.000000 cf-remote-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-03 16:51:08.996538 cf-remote-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-07-03 16:50:57.000000 cf-remote-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:51:08.996538 cf-remote-0.4.9/cf_remote/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 16:51:08.000000 cf-remote-0.4.9/cf_remote/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/aramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/cloud_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26809 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14132 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-03 16:50:57.000000 cf-remote-0.4.9/cf_remote/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:51:08.996538 cf-remote-0.4.9/cf_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-03 16:51:08.000000 cf-remote-0.4.9/cf_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-03 16:51:08.000000 cf-remote-0.4.9/cf_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:51:08.000000 cf-remote-0.4.9/cf_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 16:51:08.000000 cf-remote-0.4.9/cf_remote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 16:51:08.000000 cf-remote-0.4.9/cf_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 16:51:08.000000 cf-remote-0.4.9/cf_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:51:08.996538 cf-remote-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-03 16:50:57.000000 cf-remote-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:51:08.996538 cf-remote-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:50:57.000000 cf-remote-0.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-03 16:50:57.000000 cf-remote-0.4.9/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-03 16:50:57.000000 cf-remote-0.4.9/tests/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 16:50:57.000000 cf-remote-0.4.9/tests/test_ssh.py
```

### Comparing `cf-remote-0.4.8/LICENSE` & `cf-remote-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/PKG-INFO` & `cf-remote-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-remote
-Version: 0.4.8
+Version: 0.4.9
 Summary: Tooling to deploy CFEngine (and much more)
 Home-page: https://github.com/cfengine/cf-remote
 Author: Northern.tech, Inc.
 Author-email: contact@northern.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `cf-remote-0.4.8/README.md` & `cf-remote-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/cf_remote/aramid.py` & `cf-remote-0.4.9/cf_remote/aramid.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/cf_remote/cloud_data.py` & `cf-remote-0.4.9/cf_remote/cloud_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     "ubuntu-22-04-arm64": {
         "ami": "ami-00c50882a52d323a6",
         "user": "ubuntu",
         "size": "t4g.micro",
         "xlsize": "t4g.xlarge",
     },
     "ubuntu-22-04-x64": {
-        "ami": "ami-0d75513e7706cf2d9",
+        "ami": "ami-01dd271720c1ba44f",
         "user": "ubuntu",
         "size": "t2.small",
         "xlsize": "t3.xlarge",
     },
     "ubuntu-20-04-x64": {
         "ami": "ami-0aef57767f5404a3c",
         "user": "ubuntu",
```

### Comparing `cf-remote-0.4.8/cf_remote/commands.py` & `cf-remote-0.4.9/cf_remote/commands.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/cf_remote/demo.py` & `cf-remote-0.4.9/cf_remote/demo.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/cf_remote/log.py` & `cf-remote-0.4.9/cf_remote/log.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/cf_remote/main.py` & `cf-remote-0.4.9/cf_remote/main.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/cf_remote/packages.py` & `cf-remote-0.4.9/cf_remote/packages.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/cf_remote/paths.py` & `cf-remote-0.4.9/cf_remote/paths.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/cf_remote/remote.py` & `cf-remote-0.4.9/cf_remote/remote.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/cf_remote/spawn.py` & `cf-remote-0.4.9/cf_remote/spawn.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/cf_remote/ssh.py` & `cf-remote-0.4.9/cf_remote/ssh.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/cf_remote/utils.py` & `cf-remote-0.4.9/cf_remote/utils.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/cf_remote/web.py` & `cf-remote-0.4.9/cf_remote/web.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/cf_remote.egg-info/PKG-INFO` & `cf-remote-0.4.9/cf_remote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-remote
-Version: 0.4.8
+Version: 0.4.9
 Summary: Tooling to deploy CFEngine (and much more)
 Home-page: https://github.com/cfengine/cf-remote
 Author: Northern.tech, Inc.
 Author-email: contact@northern.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `cf-remote-0.4.8/cf_remote.egg-info/SOURCES.txt` & `cf-remote-0.4.9/cf_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/setup.py` & `cf-remote-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/tests/test_cache.py` & `cf-remote-0.4.9/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `cf-remote-0.4.8/tests/test_packages.py` & `cf-remote-0.4.9/tests/test_packages.py`

 * *Files identical despite different names*

