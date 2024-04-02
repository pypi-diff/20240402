# Comparing `tmp/ctfer-io_pulumi-ctfd-0.1.21.tar.gz` & `tmp/ctfer-io_pulumi-ctfd-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctfer-io_pulumi-ctfd-0.1.21.tar", last modified: Wed Mar 20 10:47:53 2024, max compression
+gzip compressed data, was "ctfer-io_pulumi-ctfd-0.1.22.tar", last modified: Tue Apr  2 19:02:14 2024, max compression
```

## Comparing `ctfer-io_pulumi-ctfd-0.1.21.tar` & `ctfer-io_pulumi-ctfd-0.1.22.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:47:53.817143 ctfer-io_pulumi-ctfd-0.1.21/
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-03-20 10:47:53.817143 ctfer-io_pulumi-ctfd-0.1.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:47:53.817143 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11155 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    45926 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/challenge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:47:53.817143 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/get_challenges.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/get_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    19802 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    23775 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    24618 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:47:53.817143 ctfer-io_pulumi-ctfd-0.1.21/ctfer_io_pulumi_ctfd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer_io_pulumi_ctfd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer_io_pulumi_ctfd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer_io_pulumi_ctfd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer_io_pulumi_ctfd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer_io_pulumi_ctfd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/ctfer_io_pulumi_ctfd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 10:47:53.817143 ctfer-io_pulumi-ctfd-0.1.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-20 10:47:53.000000 ctfer-io_pulumi-ctfd-0.1.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:14.456696 ctfer-io_pulumi-ctfd-0.1.22/
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-02 19:02:14.456696 ctfer-io_pulumi-ctfd-0.1.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:14.456696 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11155 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45926 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/challenge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:14.456696 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/get_challenges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/get_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19802 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    23775 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24618 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:14.456696 ctfer-io_pulumi-ctfd-0.1.22/ctfer_io_pulumi_ctfd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer_io_pulumi_ctfd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer_io_pulumi_ctfd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer_io_pulumi_ctfd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer_io_pulumi_ctfd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer_io_pulumi_ctfd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/ctfer_io_pulumi_ctfd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:02:14.456696 ctfer-io_pulumi-ctfd-0.1.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-02 19:02:14.000000 ctfer-io_pulumi-ctfd-0.1.22/setup.py
```

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/PKG-INFO` & `ctfer-io_pulumi-ctfd-0.1.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctfer-io_pulumi-ctfd
-Version: 0.1.21
+Version: 0.1.22
 Summary: The CTFd provider for Pulumi, to manage its resources as code.
 Home-page: https://ctfer.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/ctfer-io/pulumi-ctfd
 Keywords: pulumi ctfd category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ctfer-io_pulumi-ctfd Version: 0.1.21 Summary: The
+Metadata-Version: 2.1 Name: ctfer-io_pulumi-ctfd Version: 0.1.22 Summary: The
 CTFd provider for Pulumi, to manage its resources as code. Home-page: https://
 ctfer.io License: Apache-2.0 Project-URL: Repository, https://github.com/ctfer-
 io/pulumi-ctfd Keywords: pulumi ctfd category/cloud Platform: UNKNOWN Requires-
 Python: >=3.8 Description-Content-Type: text/markdown
                ************ [[rreess//ccttffdd..ppnngg]]PPuulluummii CCTTFFdd PPrroovviiddeerr ************
                             LLeett''ss ccooddee yyoouurr CCTTFF((dd))
                              _[_r_e_f_e_r_e_n_c_e_][License]
```

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/README.md` & `ctfer-io_pulumi-ctfd-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/__init__.py` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/__init__.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/_inputs.py` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/_inputs.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/_utilities.py` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/_utilities.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/challenge.py` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/challenge.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/config/vars.py` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/config/vars.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/get_challenges.py` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/get_challenges.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/get_teams.py` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/get_teams.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/get_users.py` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/get_users.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/outputs.py` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/outputs.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/provider.py` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/provider.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/team.py` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/team.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer-io_pulumi-ctfd/user.py` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer-io_pulumi-ctfd/user.py`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer_io_pulumi_ctfd.egg-info/PKG-INFO` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer_io_pulumi_ctfd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctfer-io-pulumi-ctfd
-Version: 0.1.21
+Version: 0.1.22
 Summary: The CTFd provider for Pulumi, to manage its resources as code.
 Home-page: https://ctfer.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/ctfer-io/pulumi-ctfd
 Keywords: pulumi ctfd category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ctfer-io-pulumi-ctfd Version: 0.1.21 Summary: The
+Metadata-Version: 2.1 Name: ctfer-io-pulumi-ctfd Version: 0.1.22 Summary: The
 CTFd provider for Pulumi, to manage its resources as code. Home-page: https://
 ctfer.io License: Apache-2.0 Project-URL: Repository, https://github.com/ctfer-
 io/pulumi-ctfd Keywords: pulumi ctfd category/cloud Platform: UNKNOWN Requires-
 Python: >=3.8 Description-Content-Type: text/markdown
                ************ [[rreess//ccttffdd..ppnngg]]PPuulluummii CCTTFFdd PPrroovviiddeerr ************
                             LLeett''ss ccooddee yyoouurr CCTTFF((dd))
                              _[_r_e_f_e_r_e_n_c_e_][License]
```

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/ctfer_io_pulumi_ctfd.egg-info/SOURCES.txt` & `ctfer-io_pulumi-ctfd-0.1.22/ctfer_io_pulumi_ctfd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ctfer-io_pulumi-ctfd-0.1.21/setup.py` & `ctfer-io_pulumi-ctfd-0.1.22/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import errno
-import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.21"
+VERSION = "0.1.22"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "ctfd Pulumi Package - Development Version"
```

