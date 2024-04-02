# Comparing `tmp/eth-erc721-0.3.0.tar.gz` & `tmp/eth-erc721-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-erc721-0.3.0.tar", last modified: Sun Aug  6 15:21:07 2023, max compression
+gzip compressed data, was "eth-erc721-0.4.0.tar", last modified: Tue Apr  2 12:20:47 2024, max compression
```

## Comparing `eth-erc721-0.3.0.tar` & `eth-erc721-0.4.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:21:07.525498 eth-erc721-0.3.0/
--rw-r--r--   0 lash      (1000) lash      (1000)      834 2023-08-06 15:20:27.000000 eth-erc721-0.3.0/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 08:05:47.000000 eth-erc721-0.3.0/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       84 2022-11-14 08:07:18.000000 eth-erc721-0.3.0/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      808 2023-08-06 15:21:07.525498 eth-erc721-0.3.0/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      870 2022-11-14 08:05:43.000000 eth-erc721-0.3.0/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1630 2022-11-14 08:05:43.000000 eth-erc721-0.3.0/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:21:07.525498 eth-erc721-0.3.0/eth_badgetoken/
--rw-r--r--   0 lash      (1000) lash      (1000)      108 2023-02-14 07:07:41.000000 eth-erc721-0.3.0/eth_badgetoken/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:21:07.525498 eth-erc721-0.3.0/eth_badgetoken/data/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-02-14 07:07:41.000000 eth-erc721-0.3.0/eth_badgetoken/data/.chainlib
--rw-r--r--   0 lash      (1000) lash      (1000)    27274 2023-03-27 06:35:28.000000 eth-erc721-0.3.0/eth_badgetoken/data/BadgeToken.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     7531 2023-03-27 06:35:28.000000 eth-erc721-0.3.0/eth_badgetoken/data/BadgeToken.json
--rw-r--r--   0 lash      (1000) lash      (1000)     8217 2023-03-27 06:35:28.000000 eth-erc721-0.3.0/eth_badgetoken/data/BadgeToken.metadata.json
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:21:07.525498 eth-erc721-0.3.0/eth_badgetoken/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     2578 2022-11-13 17:33:12.000000 eth-erc721-0.3.0/eth_badgetoken/runnable/deploy.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3393 2022-11-13 17:33:12.000000 eth-erc721-0.3.0/eth_badgetoken/runnable/mint.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4680 2023-03-26 08:58:55.000000 eth-erc721-0.3.0/eth_badgetoken/token.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:21:07.525498 eth-erc721-0.3.0/eth_badgetoken/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-03-03 09:36:07.000000 eth-erc721-0.3.0/eth_badgetoken/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1660 2023-03-04 10:27:00.000000 eth-erc721-0.3.0/eth_badgetoken/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      884 2023-03-26 08:58:55.000000 eth-erc721-0.3.0/eth_badgetoken/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:21:07.525498 eth-erc721-0.3.0/eth_erc721/
--rw-r--r--   0 lash      (1000) lash      (1000)       27 2021-05-08 06:08:13.000000 eth-erc721-0.3.0/eth_erc721/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6632 2023-03-26 08:58:55.000000 eth-erc721-0.3.0/eth_erc721/erc721.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:21:07.525498 eth-erc721-0.3.0/eth_erc721/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     3358 2023-03-03 09:36:07.000000 eth-erc721-0.3.0/eth_erc721/runnable/transfer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:21:07.525498 eth-erc721-0.3.0/eth_erc721/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-03-03 09:36:07.000000 eth-erc721-0.3.0/eth_erc721/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     7898 2023-03-04 10:27:48.000000 eth-erc721-0.3.0/eth_erc721/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2473 2023-03-03 09:36:07.000000 eth-erc721-0.3.0/eth_erc721/unittest/enum.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:21:07.525498 eth-erc721-0.3.0/eth_erc721.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      808 2023-08-06 15:21:07.000000 eth-erc721-0.3.0/eth_erc721.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      861 2023-08-06 15:21:07.000000 eth-erc721-0.3.0/eth_erc721.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-06 15:21:07.000000 eth-erc721-0.3.0/eth_erc721.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      178 2023-08-06 15:21:07.000000 eth-erc721-0.3.0/eth_erc721.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       70 2023-08-06 15:21:07.000000 eth-erc721-0.3.0/eth_erc721.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       26 2023-08-06 15:21:07.000000 eth-erc721-0.3.0/eth_erc721.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       70 2023-08-06 15:18:26.000000 eth-erc721-0.3.0/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1252 2023-08-06 15:21:07.528831 eth-erc721-0.3.0/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      502 2021-05-08 08:30:31.000000 eth-erc721-0.3.0/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       37 2023-08-06 15:19:06.000000 eth-erc721-0.3.0/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:21:07.525498 eth-erc721-0.3.0/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      421 2023-03-04 10:26:32.000000 eth-erc721-0.3.0/tests/test_app.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:20:47.286224 eth-erc721-0.4.0/
+-rw-r--r--   0 lash      (1000) lash      (1000)      834 2023-08-06 15:20:27.000000 eth-erc721-0.4.0/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 08:05:47.000000 eth-erc721-0.4.0/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       84 2022-11-14 08:07:18.000000 eth-erc721-0.4.0/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      938 2024-04-02 12:20:47.286224 eth-erc721-0.4.0/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      870 2022-11-14 08:05:43.000000 eth-erc721-0.4.0/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1630 2022-11-14 08:05:43.000000 eth-erc721-0.4.0/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:20:47.282890 eth-erc721-0.4.0/eth_badgetoken/
+-rw-r--r--   0 lash      (1000) lash      (1000)      108 2023-02-14 07:07:41.000000 eth-erc721-0.4.0/eth_badgetoken/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:20:47.282890 eth-erc721-0.4.0/eth_badgetoken/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-02-14 07:07:41.000000 eth-erc721-0.4.0/eth_badgetoken/data/.chainlib
+-rw-r--r--   0 lash      (1000) lash      (1000)    27274 2023-03-27 06:35:28.000000 eth-erc721-0.4.0/eth_badgetoken/data/BadgeToken.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     7531 2023-03-27 06:35:28.000000 eth-erc721-0.4.0/eth_badgetoken/data/BadgeToken.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     8217 2023-03-27 06:35:28.000000 eth-erc721-0.4.0/eth_badgetoken/data/BadgeToken.metadata.json
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:20:47.282890 eth-erc721-0.4.0/eth_badgetoken/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2578 2022-11-13 17:33:12.000000 eth-erc721-0.4.0/eth_badgetoken/runnable/deploy.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3393 2022-11-13 17:33:12.000000 eth-erc721-0.4.0/eth_badgetoken/runnable/mint.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4680 2023-03-26 08:58:55.000000 eth-erc721-0.4.0/eth_badgetoken/token.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:20:47.282890 eth-erc721-0.4.0/eth_badgetoken/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-03-03 09:36:07.000000 eth-erc721-0.4.0/eth_badgetoken/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1660 2023-03-04 10:27:00.000000 eth-erc721-0.4.0/eth_badgetoken/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      884 2023-03-26 08:58:55.000000 eth-erc721-0.4.0/eth_badgetoken/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:20:47.282890 eth-erc721-0.4.0/eth_erc721/
+-rw-r--r--   0 lash      (1000) lash      (1000)       27 2021-05-08 06:08:13.000000 eth-erc721-0.4.0/eth_erc721/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6632 2023-03-26 08:58:55.000000 eth-erc721-0.4.0/eth_erc721/erc721.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:20:47.286224 eth-erc721-0.4.0/eth_erc721/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3358 2023-03-03 09:36:07.000000 eth-erc721-0.4.0/eth_erc721/runnable/transfer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:20:47.286224 eth-erc721-0.4.0/eth_erc721/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-03-03 09:36:07.000000 eth-erc721-0.4.0/eth_erc721/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7898 2023-03-04 10:27:48.000000 eth-erc721-0.4.0/eth_erc721/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2473 2023-03-03 09:36:07.000000 eth-erc721-0.4.0/eth_erc721/unittest/enum.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:20:47.286224 eth-erc721-0.4.0/eth_erc721.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      938 2024-04-02 12:20:47.000000 eth-erc721-0.4.0/eth_erc721.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      861 2024-04-02 12:20:47.000000 eth-erc721-0.4.0/eth_erc721.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2024-04-02 12:20:47.000000 eth-erc721-0.4.0/eth_erc721.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      178 2024-04-02 12:20:47.000000 eth-erc721-0.4.0/eth_erc721.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       70 2024-04-02 12:20:47.000000 eth-erc721-0.4.0/eth_erc721.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       26 2024-04-02 12:20:47.000000 eth-erc721-0.4.0/eth_erc721.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       70 2024-04-02 12:19:46.000000 eth-erc721-0.4.0/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1252 2024-04-02 12:20:47.286224 eth-erc721-0.4.0/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      502 2021-05-08 08:30:31.000000 eth-erc721-0.4.0/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       38 2024-04-02 12:19:46.000000 eth-erc721-0.4.0/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 12:20:47.286224 eth-erc721-0.4.0/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      421 2023-03-04 10:26:32.000000 eth-erc721-0.4.0/tests/test_app.py
```

### Comparing `eth-erc721-0.3.0/CHANGELOG` & `eth-erc721-0.4.0/CHANGELOG`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/LICENSE` & `eth-erc721-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/PKG-INFO` & `eth-erc721-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-erc721
-Version: 0.3.0
+Version: 0.4.0
 Summary: ERC721 interface and simple contract with deployment script providing arbitrary minting of NFTs with freely settable tokenids
 Home-page: https://git.defalsify.org/eth-erc721
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum,token,nft
 Classifier: Programming Language :: Python :: 3
@@ -13,7 +13,11 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: chainlib-eth~=0.6.0
+Requires-Dist: chainlib~=0.5.0
+Requires-Dist: eth-erc20~=0.9.0
+Requires-Dist: eth-owned~=0.3.0
```

### Comparing `eth-erc721-0.3.0/WAIVER` & `eth-erc721-0.4.0/WAIVER`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/WAIVER.asc` & `eth-erc721-0.4.0/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/eth_badgetoken/data/BadgeToken.bin` & `eth-erc721-0.4.0/eth_badgetoken/data/BadgeToken.bin`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/eth_badgetoken/data/BadgeToken.json` & `eth-erc721-0.4.0/eth_badgetoken/data/BadgeToken.json`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/eth_badgetoken/data/BadgeToken.metadata.json` & `eth-erc721-0.4.0/eth_badgetoken/data/BadgeToken.metadata.json`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/eth_badgetoken/runnable/deploy.py` & `eth-erc721-0.4.0/eth_badgetoken/runnable/deploy.py`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/eth_badgetoken/runnable/mint.py` & `eth-erc721-0.4.0/eth_badgetoken/runnable/mint.py`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/eth_badgetoken/token.py` & `eth-erc721-0.4.0/eth_badgetoken/token.py`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/eth_badgetoken/unittest/base.py` & `eth-erc721-0.4.0/eth_badgetoken/unittest/base.py`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/eth_badgetoken/unittest/interface.py` & `eth-erc721-0.4.0/eth_badgetoken/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/eth_erc721/erc721.py` & `eth-erc721-0.4.0/eth_erc721/erc721.py`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/eth_erc721/runnable/transfer.py` & `eth-erc721-0.4.0/eth_erc721/runnable/transfer.py`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/eth_erc721/unittest/base.py` & `eth-erc721-0.4.0/eth_erc721/unittest/base.py`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/eth_erc721/unittest/enum.py` & `eth-erc721-0.4.0/eth_erc721/unittest/enum.py`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/eth_erc721.egg-info/PKG-INFO` & `eth-erc721-0.4.0/eth_erc721.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-erc721
-Version: 0.3.0
+Version: 0.4.0
 Summary: ERC721 interface and simple contract with deployment script providing arbitrary minting of NFTs with freely settable tokenids
 Home-page: https://git.defalsify.org/eth-erc721
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum,token,nft
 Classifier: Programming Language :: Python :: 3
@@ -13,7 +13,11 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: chainlib-eth~=0.6.0
+Requires-Dist: chainlib~=0.5.0
+Requires-Dist: eth-erc20~=0.9.0
+Requires-Dist: eth-owned~=0.3.0
```

### Comparing `eth-erc721-0.3.0/eth_erc721.egg-info/SOURCES.txt` & `eth-erc721-0.4.0/eth_erc721.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-erc721-0.3.0/setup.cfg` & `eth-erc721-0.4.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-erc721
-version = 0.3.0
+version = 0.4.0
 description = ERC721 interface and simple contract with deployment script providing arbitrary minting of NFTs with freely settable tokenids
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-erc721
 keywords = 
 	dlt
 	blockchain
```

