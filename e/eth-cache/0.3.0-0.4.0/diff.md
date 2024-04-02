# Comparing `tmp/eth-cache-0.3.0.tar.gz` & `tmp/eth-cache-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-cache-0.3.0.tar", last modified: Sun Aug  6 13:08:28 2023, max compression
+gzip compressed data, was "eth-cache-0.4.0.tar", last modified: Tue Apr  2 10:37:21 2024, max compression
```

## Comparing `eth-cache-0.3.0.tar` & `eth-cache-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:08:28.764729 eth-cache-0.3.0/
--rw-r--r--   0 lash      (1000) lash      (1000)      364 2023-08-06 13:07:56.000000 eth-cache-0.3.0/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:57:03.000000 eth-cache-0.3.0/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       62 2022-11-14 07:58:10.000000 eth-cache-0.3.0/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      705 2023-08-06 13:08:28.764729 eth-cache-0.3.0/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 07:57:16.000000 eth-cache-0.3.0/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1626 2022-11-14 07:57:19.000000 eth-cache-0.3.0/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:08:28.764729 eth-cache-0.3.0/eth_cache/
--rw-r--r--   0 lash      (1000) lash      (1000)     2646 2022-11-10 15:21:42.000000 eth-cache-0.3.0/eth_cache/rpc.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:08:28.764729 eth-cache-0.3.0/eth_cache/store/
--rw-r--r--   0 lash      (1000) lash      (1000)     5114 2022-10-13 14:11:16.000000 eth-cache-0.3.0/eth_cache/store/file.py
--rw-r--r--   0 lash      (1000) lash      (1000)      616 2022-03-01 11:45:36.000000 eth-cache-0.3.0/eth_cache/store/null.py
--rw-r--r--   0 lash      (1000) lash      (1000)      569 2022-05-06 08:05:25.000000 eth-cache-0.3.0/eth_cache/tx.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:08:28.764729 eth-cache-0.3.0/eth_cache.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      705 2023-08-06 13:08:28.000000 eth-cache-0.3.0/eth_cache.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      406 2023-08-06 13:08:28.000000 eth-cache-0.3.0/eth_cache.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-06 13:08:28.000000 eth-cache-0.3.0/eth_cache.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       64 2023-08-06 13:08:28.000000 eth-cache-0.3.0/eth_cache.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       71 2023-08-06 13:08:28.000000 eth-cache-0.3.0/eth_cache.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       10 2023-08-06 13:08:28.000000 eth-cache-0.3.0/eth_cache.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       71 2023-08-06 13:06:09.000000 eth-cache-0.3.0/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      846 2023-08-06 13:08:28.764729 eth-cache-0.3.0/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      494 2022-03-01 10:50:07.000000 eth-cache-0.3.0/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       76 2022-03-01 13:53:15.000000 eth-cache-0.3.0/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:08:28.764729 eth-cache-0.3.0/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     4920 2022-03-01 18:44:59.000000 eth-cache-0.3.0/tests/test_basic.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 10:37:21.246262 eth-cache-0.4.0/
+-rw-r--r--   0 lash      (1000) lash      (1000)      364 2023-08-06 13:07:56.000000 eth-cache-0.4.0/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:57:03.000000 eth-cache-0.4.0/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       62 2022-11-14 07:58:10.000000 eth-cache-0.4.0/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      836 2024-04-02 10:37:21.246262 eth-cache-0.4.0/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 07:57:16.000000 eth-cache-0.4.0/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1626 2022-11-14 07:57:19.000000 eth-cache-0.4.0/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 10:37:21.242928 eth-cache-0.4.0/eth_cache/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2646 2022-11-10 15:21:42.000000 eth-cache-0.4.0/eth_cache/rpc.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 10:37:21.242928 eth-cache-0.4.0/eth_cache/store/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5114 2022-10-13 14:11:16.000000 eth-cache-0.4.0/eth_cache/store/file.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      616 2022-03-01 11:45:36.000000 eth-cache-0.4.0/eth_cache/store/null.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      569 2022-05-06 08:05:25.000000 eth-cache-0.4.0/eth_cache/tx.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 10:37:21.242928 eth-cache-0.4.0/eth_cache.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      836 2024-04-02 10:37:21.000000 eth-cache-0.4.0/eth_cache.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      406 2024-04-02 10:37:21.000000 eth-cache-0.4.0/eth_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2024-04-02 10:37:21.000000 eth-cache-0.4.0/eth_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       64 2024-04-02 10:37:21.000000 eth-cache-0.4.0/eth_cache.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       71 2024-04-02 10:37:21.000000 eth-cache-0.4.0/eth_cache.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       10 2024-04-02 10:37:21.000000 eth-cache-0.4.0/eth_cache.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       71 2024-04-02 10:37:16.000000 eth-cache-0.4.0/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      846 2024-04-02 10:37:21.246262 eth-cache-0.4.0/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      494 2022-03-01 10:50:07.000000 eth-cache-0.4.0/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       76 2022-03-01 13:53:15.000000 eth-cache-0.4.0/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 10:37:21.242928 eth-cache-0.4.0/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     4920 2022-03-01 18:44:59.000000 eth-cache-0.4.0/tests/test_basic.py
```

### Comparing `eth-cache-0.3.0/LICENSE` & `eth-cache-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-cache-0.3.0/PKG-INFO` & `eth-cache-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-cache
-Version: 0.3.0
+Version: 0.4.0
 Summary: Ethereum chain data caching tools
 Home-page: https://git.defalsify.org/eth-cache
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
@@ -13,7 +13,11 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: hexathon~=0.1.7
+Requires-Dist: jsonrpc-std~=0.1.0
+Requires-Dist: leveldir~=0.3.0
+Requires-Dist: chainlib-eth~=0.6.0
```

### Comparing `eth-cache-0.3.0/WAIVER` & `eth-cache-0.4.0/WAIVER`

 * *Files identical despite different names*

### Comparing `eth-cache-0.3.0/WAIVER.asc` & `eth-cache-0.4.0/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `eth-cache-0.3.0/eth_cache/rpc.py` & `eth-cache-0.4.0/eth_cache/rpc.py`

 * *Files identical despite different names*

### Comparing `eth-cache-0.3.0/eth_cache/store/file.py` & `eth-cache-0.4.0/eth_cache/store/file.py`

 * *Files identical despite different names*

### Comparing `eth-cache-0.3.0/eth_cache/store/null.py` & `eth-cache-0.4.0/eth_cache/store/null.py`

 * *Files identical despite different names*

### Comparing `eth-cache-0.3.0/eth_cache/tx.py` & `eth-cache-0.4.0/eth_cache/tx.py`

 * *Files identical despite different names*

### Comparing `eth-cache-0.3.0/eth_cache.egg-info/PKG-INFO` & `eth-cache-0.4.0/eth_cache.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-cache
-Version: 0.3.0
+Version: 0.4.0
 Summary: Ethereum chain data caching tools
 Home-page: https://git.defalsify.org/eth-cache
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
@@ -13,7 +13,11 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: hexathon~=0.1.7
+Requires-Dist: jsonrpc-std~=0.1.0
+Requires-Dist: leveldir~=0.3.0
+Requires-Dist: chainlib-eth~=0.6.0
```

### Comparing `eth-cache-0.3.0/setup.cfg` & `eth-cache-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-cache
-version = 0.3.0
+version = 0.4.0
 description = Ethereum chain data caching tools
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-cache
 keywords = 
 	dlt
 	blockchain
```

### Comparing `eth-cache-0.3.0/tests/test_basic.py` & `eth-cache-0.4.0/tests/test_basic.py`

 * *Files identical despite different names*

