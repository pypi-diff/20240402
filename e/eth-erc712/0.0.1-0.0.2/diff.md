# Comparing `tmp/eth-erc712-0.0.1.tar.gz` & `tmp/eth-erc712-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-erc712-0.0.1.tar", last modified: Sat May 13 21:06:09 2023, max compression
+gzip compressed data, was "eth-erc712-0.0.2.tar", last modified: Tue Apr  2 12:30:35 2024, max compression
```

## Comparing `eth-erc712-0.0.1.tar` & `eth-erc712-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-13 21:06:09.056644 eth-erc712-0.0.1/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-03-29 03:37:27.000000 eth-erc712-0.0.1/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-03-29 03:36:49.000000 eth-erc712-0.0.1/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       91 2023-03-29 03:37:14.000000 eth-erc712-0.0.1/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      718 2023-05-13 21:06:09.056644 eth-erc712-0.0.1/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      870 2023-03-29 03:39:19.000000 eth-erc712-0.0.1/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)      488 2023-03-29 03:39:38.000000 eth-erc712-0.0.1/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-13 21:06:09.053310 eth-erc712-0.0.1/eth_erc712/
--rw-r--r--   0 lash      (1000) lash      (1000)       67 2023-03-28 14:23:35.000000 eth-erc712-0.0.1/eth_erc712/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3823 2023-03-29 14:01:40.000000 eth-erc712-0.0.1/eth_erc712/base.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-13 21:06:09.056644 eth-erc712-0.0.1/eth_erc712/data/
--rw-r--r--   0 lash      (1000) lash      (1000)     5742 2023-03-29 13:54:28.000000 eth-erc712-0.0.1/eth_erc712/data/ERC712Example.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     1172 2023-03-29 13:54:28.000000 eth-erc712-0.0.1/eth_erc712/data/ERC712Example.json
--rw-r--r--   0 lash      (1000) lash      (1000)     1851 2023-03-29 13:54:28.000000 eth-erc712-0.0.1/eth_erc712/data/ERC712Example.metadata.json
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-13 21:06:09.056644 eth-erc712-0.0.1/eth_erc712/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       29 2023-03-28 11:08:38.000000 eth-erc712-0.0.1/eth_erc712/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1780 2023-03-28 15:39:59.000000 eth-erc712-0.0.1/eth_erc712/unittest/base.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-13 21:06:09.053310 eth-erc712-0.0.1/eth_erc712.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      718 2023-05-13 21:06:09.000000 eth-erc712-0.0.1/eth_erc712.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      509 2023-05-13 21:06:09.000000 eth-erc712-0.0.1/eth_erc712.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-05-13 21:06:09.000000 eth-erc712-0.0.1/eth_erc712.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       55 2023-05-13 21:06:09.000000 eth-erc712-0.0.1/eth_erc712.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       11 2023-05-13 21:06:09.000000 eth-erc712-0.0.1/eth_erc712.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       55 2023-03-29 09:27:53.000000 eth-erc712-0.0.1/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      829 2023-05-13 21:06:09.056644 eth-erc712-0.0.1/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      467 2023-03-29 03:38:33.000000 eth-erc712-0.0.1/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       76 2023-03-28 11:41:56.000000 eth-erc712-0.0.1/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-13 21:06:09.056644 eth-erc712-0.0.1/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     7385 2023-03-29 14:05:02.000000 eth-erc712-0.0.1/tests/test_basic.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:30:35.259553 eth-erc712-0.0.2/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-03-29 03:37:27.000000 eth-erc712-0.0.2/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-03-29 03:36:49.000000 eth-erc712-0.0.2/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       91 2023-03-29 03:37:14.000000 eth-erc712-0.0.2/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      816 2024-04-02 12:30:35.259553 eth-erc712-0.0.2/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      870 2023-03-29 03:39:19.000000 eth-erc712-0.0.2/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)      488 2023-03-29 03:39:38.000000 eth-erc712-0.0.2/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:30:35.256220 eth-erc712-0.0.2/eth_erc712/
+-rw-r--r--   0 lash      (1000) lash      (1000)       67 2023-03-28 14:23:35.000000 eth-erc712-0.0.2/eth_erc712/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3823 2023-03-29 14:01:40.000000 eth-erc712-0.0.2/eth_erc712/base.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:30:35.259553 eth-erc712-0.0.2/eth_erc712/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5742 2023-03-29 13:54:28.000000 eth-erc712-0.0.2/eth_erc712/data/ERC712Example.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1172 2023-03-29 13:54:28.000000 eth-erc712-0.0.2/eth_erc712/data/ERC712Example.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     1851 2023-03-29 13:54:28.000000 eth-erc712-0.0.2/eth_erc712/data/ERC712Example.metadata.json
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:30:35.259553 eth-erc712-0.0.2/eth_erc712/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       29 2023-03-28 11:08:38.000000 eth-erc712-0.0.2/eth_erc712/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1780 2023-03-28 15:39:59.000000 eth-erc712-0.0.2/eth_erc712/unittest/base.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:30:35.259553 eth-erc712-0.0.2/eth_erc712.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      816 2024-04-02 12:30:35.000000 eth-erc712-0.0.2/eth_erc712.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      509 2024-04-02 12:30:35.000000 eth-erc712-0.0.2/eth_erc712.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2024-04-02 12:30:35.000000 eth-erc712-0.0.2/eth_erc712.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       53 2024-04-02 12:30:35.000000 eth-erc712-0.0.2/eth_erc712.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       11 2024-04-02 12:30:35.000000 eth-erc712-0.0.2/eth_erc712.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       53 2024-04-02 12:29:12.000000 eth-erc712-0.0.2/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      829 2024-04-02 12:30:35.259553 eth-erc712-0.0.2/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      467 2023-03-29 03:38:33.000000 eth-erc712-0.0.2/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       77 2024-04-02 12:29:12.000000 eth-erc712-0.0.2/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:30:35.259553 eth-erc712-0.0.2/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     7385 2023-03-29 14:05:02.000000 eth-erc712-0.0.2/tests/test_basic.py
```

### Comparing `eth-erc712-0.0.1/LICENSE` & `eth-erc712-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-erc712-0.0.1/WAIVER` & `eth-erc712-0.0.2/WAIVER`

 * *Files identical despite different names*

### Comparing `eth-erc712-0.0.1/eth_erc712/base.py` & `eth-erc712-0.0.2/eth_erc712/base.py`

 * *Files identical despite different names*

### Comparing `eth-erc712-0.0.1/eth_erc712/data/ERC712Example.bin` & `eth-erc712-0.0.2/eth_erc712/data/ERC712Example.bin`

 * *Files identical despite different names*

### Comparing `eth-erc712-0.0.1/eth_erc712/data/ERC712Example.json` & `eth-erc712-0.0.2/eth_erc712/data/ERC712Example.json`

 * *Files identical despite different names*

### Comparing `eth-erc712-0.0.1/eth_erc712/data/ERC712Example.metadata.json` & `eth-erc712-0.0.2/eth_erc712/data/ERC712Example.metadata.json`

 * *Files identical despite different names*

### Comparing `eth-erc712-0.0.1/eth_erc712/unittest/base.py` & `eth-erc712-0.0.2/eth_erc712/unittest/base.py`

 * *Files identical despite different names*

### Comparing `eth-erc712-0.0.1/setup.cfg` & `eth-erc712-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-erc712
-version = 0.0.1
+version = 0.0.2
 description = ERC712 typed data sign material builder
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-erc712
 keywords = 
 	dlt
 	ethereum
```

### Comparing `eth-erc712-0.0.1/tests/test_basic.py` & `eth-erc712-0.0.2/tests/test_basic.py`

 * *Files identical despite different names*

