# Comparing `tmp/p_cmd_runr-0.1.4.tar.gz` & `tmp/p_cmd_runr-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Me\forge\python\PyPi Sandbox\p_cmd_runr - clean - PyPi\dist\.tmp-p4n1bhxy\p_cmd_runr-0.1.4.tar", last modified: Sun Mar 24 01:39:48 2024, max compression
+gzip compressed data, was "C:\Users\Me\forge\python\PyPi Sandbox\p_cmd_runr - clean - PyPi\dist\.tmp-6e61dimr\p_cmd_runr-0.1.5.tar", last modified: Tue Apr  2 03:14:58 2024, max compression
```

## Comparing `p_cmd_runr-0.1.4.tar` & `p_cmd_runr-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 01:39:48.210327 p_cmd_runr-0.1.4/
--rw-rw-rw-   0        0        0    35821 2022-04-25 03:27:08.000000 p_cmd_runr-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0    19280 2024-03-24 01:39:48.209325 p_cmd_runr-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    18358 2024-03-24 01:15:51.000000 p_cmd_runr-0.1.4/README.md
--rw-rw-rw-   0        0        0       86 2022-04-21 23:21:52.000000 p_cmd_runr-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0     1345 2024-03-24 01:39:48.223066 p_cmd_runr-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-24 01:39:47.648354 p_cmd_runr-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-03-24 01:39:47.847542 p_cmd_runr-0.1.4/src/find_overlap/
--rw-rw-rw-   0        0        0     2896 2022-07-27 17:56:17.000000 p_cmd_runr-0.1.4/src/find_overlap/README.txt
--rw-rw-rw-   0        0        0        0 2022-05-05 01:32:38.000000 p_cmd_runr-0.1.4/src/find_overlap/__init__.py
--rw-rw-rw-   0        0        0     4302 2022-05-08 05:01:41.000000 p_cmd_runr-0.1.4/src/find_overlap/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-24 01:39:47.947614 p_cmd_runr-0.1.4/src/gp_cmd_runr/
--rw-rw-rw-   0        0        0     3259 2022-07-27 18:56:45.000000 p_cmd_runr-0.1.4/src/gp_cmd_runr/README.txt
--rw-rw-rw-   0        0        0        0 2022-05-01 07:11:03.000000 p_cmd_runr-0.1.4/src/gp_cmd_runr/__init__.py
--rw-rw-rw-   0        0        0     3377 2022-05-06 04:17:53.000000 p_cmd_runr-0.1.4/src/gp_cmd_runr/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-24 01:39:48.157587 p_cmd_runr-0.1.4/src/p_cmd_runr/
--rw-rw-rw-   0        0        0     4606 2022-07-27 22:42:20.000000 p_cmd_runr-0.1.4/src/p_cmd_runr/Definitions.txt
--rw-rw-rw-   0        0        0    35821 2022-04-25 03:27:08.000000 p_cmd_runr-0.1.4/src/p_cmd_runr/LICENSE.txt
--rw-rw-rw-   0        0        0    19159 2022-07-28 16:06:14.000000 p_cmd_runr-0.1.4/src/p_cmd_runr/README.md
--rw-rw-rw-   0        0        0        0 2022-04-30 02:39:35.000000 p_cmd_runr-0.1.4/src/p_cmd_runr/__init__.py
--rw-rw-rw-   0        0        0     4000 2023-10-29 04:36:41.000000 p_cmd_runr-0.1.4/src/p_cmd_runr/file_manip.py
--rw-rw-rw-   0        0        0    28619 2023-10-29 04:21:58.000000 p_cmd_runr-0.1.4/src/p_cmd_runr/p_cmd_runr.py
--rw-rw-rw-   0        0        0      102 2022-05-02 03:58:56.000000 p_cmd_runr-0.1.4/src/p_cmd_runr/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-03-24 01:39:48.207336 p_cmd_runr-0.1.4/src/p_cmd_runr.egg-info/
--rw-rw-rw-   0        0        0    19280 2024-03-24 01:39:47.000000 p_cmd_runr-0.1.4/src/p_cmd_runr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      678 2024-03-24 01:39:47.000000 p_cmd_runr-0.1.4/src/p_cmd_runr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 01:39:47.000000 p_cmd_runr-0.1.4/src/p_cmd_runr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-03-24 01:39:47.000000 p_cmd_runr-0.1.4/src/p_cmd_runr.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2024-03-24 01:39:47.000000 p_cmd_runr-0.1.4/src/p_cmd_runr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       36 2024-03-24 01:39:47.000000 p_cmd_runr-0.1.4/src/p_cmd_runr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-05-11 16:35:02.000000 p_cmd_runr-0.1.4/src/p_cmd_runr.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-04-02 03:14:58.215224 p_cmd_runr-0.1.5/
+-rw-rw-rw-   0        0        0    35821 2022-04-25 03:27:08.000000 p_cmd_runr-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0    19284 2024-04-02 03:14:58.215224 p_cmd_runr-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    18362 2024-03-24 01:52:10.000000 p_cmd_runr-0.1.5/README.md
+-rw-rw-rw-   0        0        0       86 2022-04-21 23:21:52.000000 p_cmd_runr-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1345 2024-04-02 03:14:58.230862 p_cmd_runr-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 03:14:57.605673 p_cmd_runr-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 03:14:57.871379 p_cmd_runr-0.1.5/src/find_overlap/
+-rw-rw-rw-   0        0        0     2896 2022-07-27 17:56:17.000000 p_cmd_runr-0.1.5/src/find_overlap/README.txt
+-rw-rw-rw-   0        0        0        0 2022-05-05 01:32:38.000000 p_cmd_runr-0.1.5/src/find_overlap/__init__.py
+-rw-rw-rw-   0        0        0     4302 2022-05-08 05:01:41.000000 p_cmd_runr-0.1.5/src/find_overlap/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 03:14:57.996421 p_cmd_runr-0.1.5/src/gp_cmd_runr/
+-rw-rw-rw-   0        0        0     3259 2022-07-27 18:56:45.000000 p_cmd_runr-0.1.5/src/gp_cmd_runr/README.txt
+-rw-rw-rw-   0        0        0        0 2022-05-01 07:11:03.000000 p_cmd_runr-0.1.5/src/gp_cmd_runr/__init__.py
+-rw-rw-rw-   0        0        0     3377 2022-05-06 04:17:53.000000 p_cmd_runr-0.1.5/src/gp_cmd_runr/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 03:14:58.168359 p_cmd_runr-0.1.5/src/p_cmd_runr/
+-rw-rw-rw-   0        0        0     4606 2022-07-27 22:42:20.000000 p_cmd_runr-0.1.5/src/p_cmd_runr/Definitions.txt
+-rw-rw-rw-   0        0        0    35821 2022-04-25 03:27:08.000000 p_cmd_runr-0.1.5/src/p_cmd_runr/LICENSE.txt
+-rw-rw-rw-   0        0        0    19159 2022-07-28 16:06:14.000000 p_cmd_runr-0.1.5/src/p_cmd_runr/README.md
+-rw-rw-rw-   0        0        0        0 2022-04-30 02:39:35.000000 p_cmd_runr-0.1.5/src/p_cmd_runr/__init__.py
+-rw-rw-rw-   0        0        0     4000 2023-10-29 04:36:41.000000 p_cmd_runr-0.1.5/src/p_cmd_runr/file_manip.py
+-rw-rw-rw-   0        0        0    28619 2023-10-29 04:21:58.000000 p_cmd_runr-0.1.5/src/p_cmd_runr/p_cmd_runr.py
+-rw-rw-rw-   0        0        0      102 2022-05-02 03:58:56.000000 p_cmd_runr-0.1.5/src/p_cmd_runr/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 03:14:58.215224 p_cmd_runr-0.1.5/src/p_cmd_runr.egg-info/
+-rw-rw-rw-   0        0        0    19284 2024-04-02 03:14:57.000000 p_cmd_runr-0.1.5/src/p_cmd_runr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      678 2024-04-02 03:14:57.000000 p_cmd_runr-0.1.5/src/p_cmd_runr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 03:14:57.000000 p_cmd_runr-0.1.5/src/p_cmd_runr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-02 03:14:57.000000 p_cmd_runr-0.1.5/src/p_cmd_runr.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2024-04-02 03:14:57.000000 p_cmd_runr-0.1.5/src/p_cmd_runr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       36 2024-04-02 03:14:57.000000 p_cmd_runr-0.1.5/src/p_cmd_runr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-05-11 16:35:02.000000 p_cmd_runr-0.1.5/src/p_cmd_runr.egg-info/zip-safe
```

### Comparing `p_cmd_runr-0.1.4/LICENSE.txt` & `p_cmd_runr-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `p_cmd_runr-0.1.4/PKG-INFO` & `p_cmd_runr-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p_cmd_runr
-Version: 0.1.4
+Version: 0.1.5
 Summary: A multi-purpose and flexible way to run commands on remote hosts.
 Home-page: https://github.com/kaiyoux/p_cmd_runr
 Author: Issa Lompo
 Author-email: kaiyoux@gmail.com
 Maintainer: Issa Lompo
 Maintainer-email: kaiyoux@gmail.com
 License: GNU General Public License v3 (GPLv3)
@@ -29,17 +29,17 @@
 As of **version 0.1.0**, SSH security key files are supported as an alternative to
 password authentication.
 See this [tutorial](https://phoenixnap.com/kb/setup-passwordless-ssh) on how to setup your SSH security key files.
 In general, you would generate public and private key-pair(s) on your local 
 machine, then transfer the public key(s) to your remote node(s).
 
 ### To install the package:
-**python -m pip install p_cmd_runr
+**python -m pip install p_cmd_runr**
 or
-python3 -m pip install --user p_cmd_runr**
+**python3 -m pip install --user p_cmd_runr**
 
 
 ### The p_cmd_runr package provides access to:
 - an API composed of a ConfigGrabber class, a CmdRunner class, a main function 
 called boxjumper, and other utility functions.
 - the gp_cmd_runr a general purpose command runner script.
```

### Comparing `p_cmd_runr-0.1.4/README.md` & `p_cmd_runr-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 As of **version 0.1.0**, SSH security key files are supported as an alternative to
 password authentication.
 See this [tutorial](https://phoenixnap.com/kb/setup-passwordless-ssh) on how to setup your SSH security key files.
 In general, you would generate public and private key-pair(s) on your local 
 machine, then transfer the public key(s) to your remote node(s).
 
 ### To install the package:
-**python -m pip install p_cmd_runr
+**python -m pip install p_cmd_runr**
 or
-python3 -m pip install --user p_cmd_runr**
+**python3 -m pip install --user p_cmd_runr**
 
 
 ### The p_cmd_runr package provides access to:
 - an API composed of a ConfigGrabber class, a CmdRunner class, a main function 
 called boxjumper, and other utility functions.
 - the gp_cmd_runr a general purpose command runner script.
```

### Comparing `p_cmd_runr-0.1.4/setup.cfg` & `p_cmd_runr-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 5f63 6d64 5f72 756e 720d 0a76   = p_cmd_runr..v
-00000020: 6572 7369 6f6e 203d 2030 2e31 2e34 0d0a  ersion = 0.1.4..
+00000020: 6572 7369 6f6e 203d 2030 2e31 2e35 0d0a  ersion = 0.1.5..
 00000030: 6175 7468 6f72 203d 2049 7373 6120 4c6f  author = Issa Lo
 00000040: 6d70 6f0d 0a61 7574 686f 725f 656d 6169  mpo..author_emai
 00000050: 6c20 3d20 6b61 6979 6f75 7840 676d 6169  l = kaiyoux@gmai
 00000060: 6c2e 636f 6d0d 0a6d 6169 6e74 6169 6e65  l.com..maintaine
 00000070: 7220 3d20 4973 7361 204c 6f6d 706f 0d0a  r = Issa Lompo..
 00000080: 6d61 696e 7461 696e 6572 5f65 6d61 696c  maintainer_email
 00000090: 203d 206b 6169 796f 7578 4067 6d61 696c   = kaiyoux@gmail
```

### Comparing `p_cmd_runr-0.1.4/src/find_overlap/README.txt` & `p_cmd_runr-0.1.5/src/find_overlap/README.txt`

 * *Files identical despite different names*

### Comparing `p_cmd_runr-0.1.4/src/find_overlap/__main__.py` & `p_cmd_runr-0.1.5/src/find_overlap/__main__.py`

 * *Files identical despite different names*

### Comparing `p_cmd_runr-0.1.4/src/gp_cmd_runr/README.txt` & `p_cmd_runr-0.1.5/src/gp_cmd_runr/README.txt`

 * *Files identical despite different names*

### Comparing `p_cmd_runr-0.1.4/src/gp_cmd_runr/__main__.py` & `p_cmd_runr-0.1.5/src/gp_cmd_runr/__main__.py`

 * *Files identical despite different names*

### Comparing `p_cmd_runr-0.1.4/src/p_cmd_runr/Definitions.txt` & `p_cmd_runr-0.1.5/src/p_cmd_runr/Definitions.txt`

 * *Files identical despite different names*

### Comparing `p_cmd_runr-0.1.4/src/p_cmd_runr/LICENSE.txt` & `p_cmd_runr-0.1.5/src/p_cmd_runr/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `p_cmd_runr-0.1.4/src/p_cmd_runr/README.md` & `p_cmd_runr-0.1.5/src/p_cmd_runr/README.md`

 * *Files identical despite different names*

### Comparing `p_cmd_runr-0.1.4/src/p_cmd_runr/file_manip.py` & `p_cmd_runr-0.1.5/src/p_cmd_runr/file_manip.py`

 * *Files identical despite different names*

### Comparing `p_cmd_runr-0.1.4/src/p_cmd_runr/p_cmd_runr.py` & `p_cmd_runr-0.1.5/src/p_cmd_runr/p_cmd_runr.py`

 * *Files identical despite different names*

### Comparing `p_cmd_runr-0.1.4/src/p_cmd_runr.egg-info/PKG-INFO` & `p_cmd_runr-0.1.5/src/p_cmd_runr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p_cmd_runr
-Version: 0.1.4
+Version: 0.1.5
 Summary: A multi-purpose and flexible way to run commands on remote hosts.
 Home-page: https://github.com/kaiyoux/p_cmd_runr
 Author: Issa Lompo
 Author-email: kaiyoux@gmail.com
 Maintainer: Issa Lompo
 Maintainer-email: kaiyoux@gmail.com
 License: GNU General Public License v3 (GPLv3)
@@ -29,17 +29,17 @@
 As of **version 0.1.0**, SSH security key files are supported as an alternative to
 password authentication.
 See this [tutorial](https://phoenixnap.com/kb/setup-passwordless-ssh) on how to setup your SSH security key files.
 In general, you would generate public and private key-pair(s) on your local 
 machine, then transfer the public key(s) to your remote node(s).
 
 ### To install the package:
-**python -m pip install p_cmd_runr
+**python -m pip install p_cmd_runr**
 or
-python3 -m pip install --user p_cmd_runr**
+**python3 -m pip install --user p_cmd_runr**
 
 
 ### The p_cmd_runr package provides access to:
 - an API composed of a ConfigGrabber class, a CmdRunner class, a main function 
 called boxjumper, and other utility functions.
 - the gp_cmd_runr a general purpose command runner script.
```

### Comparing `p_cmd_runr-0.1.4/src/p_cmd_runr.egg-info/SOURCES.txt` & `p_cmd_runr-0.1.5/src/p_cmd_runr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

