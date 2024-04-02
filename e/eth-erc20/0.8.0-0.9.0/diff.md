# Comparing `tmp/eth-erc20-0.8.0.tar.gz` & `tmp/eth-erc20-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-erc20-0.8.0.tar", last modified: Sun Aug  6 15:14:34 2023, max compression
+gzip compressed data, was "eth-erc20-0.9.0.tar", last modified: Tue Apr  2 11:43:34 2024, max compression
```

## Comparing `eth-erc20-0.8.0.tar` & `eth-erc20-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:14:34.325015 eth-erc20-0.8.0/
--rw-r--r--   0 lash      (1000) lash      (1000)     1705 2023-07-27 06:34:01.000000 eth-erc20-0.8.0/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 08:00:05.000000 eth-erc20-0.8.0/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      153 2023-02-14 06:40:00.000000 eth-erc20-0.8.0/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      786 2023-08-06 15:14:34.325015 eth-erc20-0.8.0/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 08:00:13.000000 eth-erc20-0.8.0/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 08:03:07.000000 eth-erc20-0.8.0/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:14:34.321682 eth-erc20-0.8.0/eth_erc20/
--rw-r--r--   0 lash      (1000) lash      (1000)       25 2021-05-02 11:58:48.000000 eth-erc20-0.8.0/eth_erc20/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:14:34.321682 eth-erc20-0.8.0/eth_erc20/data/
--rw-r--r--   0 lash      (1000) lash      (1000)     2605 2021-05-02 12:53:06.000000 eth-erc20-0.8.0/eth_erc20/data/ERC20.json
--rw-r--r--   0 lash      (1000) lash      (1000)     8888 2022-11-23 16:04:50.000000 eth-erc20-0.8.0/eth_erc20/erc20.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:14:34.321682 eth-erc20-0.8.0/eth_erc20/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     3344 2023-08-05 10:54:39.000000 eth-erc20-0.8.0/eth_erc20/runnable/balance.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3804 2023-02-13 06:39:32.000000 eth-erc20-0.8.0/eth_erc20/runnable/info.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3700 2022-11-06 10:30:18.000000 eth-erc20-0.8.0/eth_erc20/runnable/transfer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:14:34.321682 eth-erc20-0.8.0/eth_erc20/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-02-23 08:04:29.000000 eth-erc20-0.8.0/eth_erc20/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6429 2023-06-29 19:53:13.000000 eth-erc20-0.8.0/eth_erc20/unittest/base.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:14:34.321682 eth-erc20-0.8.0/eth_erc20.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      786 2023-08-06 15:14:34.000000 eth-erc20-0.8.0/eth_erc20.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1146 2023-08-06 15:14:34.000000 eth-erc20-0.8.0/eth_erc20.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-06 15:14:34.000000 eth-erc20-0.8.0/eth_erc20.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      288 2023-08-06 15:14:34.000000 eth-erc20-0.8.0/eth_erc20.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       67 2023-08-06 15:14:34.000000 eth-erc20-0.8.0/eth_erc20.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       44 2023-08-06 15:14:34.000000 eth-erc20-0.8.0/eth_erc20.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:14:34.325015 eth-erc20-0.8.0/giftable_erc20_token/
--rw-r--r--   0 lash      (1000) lash      (1000)      119 2023-02-14 06:40:00.000000 eth-erc20-0.8.0/giftable_erc20_token/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:14:34.325015 eth-erc20-0.8.0/giftable_erc20_token/data/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-05-08 04:03:57.000000 eth-erc20-0.8.0/giftable_erc20_token/data/.chainlib
--rw-r--r--   0 lash      (1000) lash      (1000)    18930 2023-03-26 07:09:01.000000 eth-erc20-0.8.0/giftable_erc20_token/data/GiftableToken.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     6791 2023-03-26 07:09:01.000000 eth-erc20-0.8.0/giftable_erc20_token/data/GiftableToken.json
--rw-r--r--   0 lash      (1000) lash      (1000)       66 2021-02-24 16:44:15.000000 eth-erc20-0.8.0/giftable_erc20_token/data/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5307 2023-08-04 20:44:58.000000 eth-erc20-0.8.0/giftable_erc20_token/factory.py
--rw-r--r--   0 lash      (1000) lash      (1000)      108 2023-02-13 12:12:59.000000 eth-erc20-0.8.0/giftable_erc20_token/gen.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:14:34.325015 eth-erc20-0.8.0/giftable_erc20_token/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     2803 2023-01-24 15:09:24.000000 eth-erc20-0.8.0/giftable_erc20_token/runnable/gift.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3431 2023-01-24 15:53:09.000000 eth-erc20-0.8.0/giftable_erc20_token/runnable/minter.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3255 2023-02-21 18:21:49.000000 eth-erc20-0.8.0/giftable_erc20_token/runnable/publish.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:14:34.325015 eth-erc20-0.8.0/giftable_erc20_token/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-02-21 17:44:31.000000 eth-erc20-0.8.0/giftable_erc20_token/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2056 2023-07-26 08:51:01.000000 eth-erc20-0.8.0/giftable_erc20_token/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)       67 2023-08-06 15:12:33.000000 eth-erc20-0.8.0/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1465 2023-08-06 15:14:34.328349 eth-erc20-0.8.0/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      666 2021-04-04 12:48:14.000000 eth-erc20-0.8.0/setup.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:14:34.318349 eth-erc20-0.8.0/static_token/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:14:34.325015 eth-erc20-0.8.0/static_token/data/
--rw-r--r--   0 lash      (1000) lash      (1000)    11366 2023-03-02 11:29:39.000000 eth-erc20-0.8.0/static_token/data/StaticToken.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     3288 2023-03-02 11:29:39.000000 eth-erc20-0.8.0/static_token/data/StaticToken.json
--rw-r--r--   0 lash      (1000) lash      (1000)       66 2022-04-22 18:28:18.000000 eth-erc20-0.8.0/static_token/data/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)       51 2021-05-02 12:00:59.000000 eth-erc20-0.8.0/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:14:34.325015 eth-erc20-0.8.0/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      266 2023-02-23 08:04:58.000000 eth-erc20-0.8.0/tests/test_erc20_interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4318 2023-02-22 10:16:13.000000 eth-erc20-0.8.0/tests/test_giftable.py
--rw-r--r--   0 lash      (1000) lash      (1000)      733 2023-06-29 19:52:55.000000 eth-erc20-0.8.0/tests/test_static.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:43:34.079571 eth-erc20-0.9.0/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1705 2023-07-27 06:34:01.000000 eth-erc20-0.9.0/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 08:00:05.000000 eth-erc20-0.9.0/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      153 2023-02-14 06:40:00.000000 eth-erc20-0.9.0/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      913 2024-04-02 11:43:34.079571 eth-erc20-0.9.0/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 08:00:13.000000 eth-erc20-0.9.0/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 08:03:07.000000 eth-erc20-0.9.0/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:43:34.076237 eth-erc20-0.9.0/eth_erc20/
+-rw-r--r--   0 lash      (1000) lash      (1000)       25 2021-05-02 11:58:48.000000 eth-erc20-0.9.0/eth_erc20/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:43:34.076237 eth-erc20-0.9.0/eth_erc20/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2605 2021-05-02 12:53:06.000000 eth-erc20-0.9.0/eth_erc20/data/ERC20.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     8888 2022-11-23 16:04:50.000000 eth-erc20-0.9.0/eth_erc20/erc20.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:43:34.076237 eth-erc20-0.9.0/eth_erc20/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3344 2023-08-05 10:54:39.000000 eth-erc20-0.9.0/eth_erc20/runnable/balance.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3804 2023-02-13 06:39:32.000000 eth-erc20-0.9.0/eth_erc20/runnable/info.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3700 2022-11-06 10:30:18.000000 eth-erc20-0.9.0/eth_erc20/runnable/transfer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:43:34.076237 eth-erc20-0.9.0/eth_erc20/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-02-23 08:04:29.000000 eth-erc20-0.9.0/eth_erc20/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6429 2023-06-29 19:53:13.000000 eth-erc20-0.9.0/eth_erc20/unittest/base.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:43:34.079571 eth-erc20-0.9.0/eth_erc20.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      913 2024-04-02 11:43:34.000000 eth-erc20-0.9.0/eth_erc20.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1146 2024-04-02 11:43:34.000000 eth-erc20-0.9.0/eth_erc20.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2024-04-02 11:43:34.000000 eth-erc20-0.9.0/eth_erc20.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      288 2024-04-02 11:43:34.000000 eth-erc20-0.9.0/eth_erc20.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       67 2024-04-02 11:43:34.000000 eth-erc20-0.9.0/eth_erc20.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       44 2024-04-02 11:43:34.000000 eth-erc20-0.9.0/eth_erc20.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:43:34.076237 eth-erc20-0.9.0/giftable_erc20_token/
+-rw-r--r--   0 lash      (1000) lash      (1000)      119 2023-02-14 06:40:00.000000 eth-erc20-0.9.0/giftable_erc20_token/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:43:34.076237 eth-erc20-0.9.0/giftable_erc20_token/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-05-08 04:03:57.000000 eth-erc20-0.9.0/giftable_erc20_token/data/.chainlib
+-rw-r--r--   0 lash      (1000) lash      (1000)    18930 2023-03-26 07:09:01.000000 eth-erc20-0.9.0/giftable_erc20_token/data/GiftableToken.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     6791 2023-03-26 07:09:01.000000 eth-erc20-0.9.0/giftable_erc20_token/data/GiftableToken.json
+-rw-r--r--   0 lash      (1000) lash      (1000)       66 2021-02-24 16:44:15.000000 eth-erc20-0.9.0/giftable_erc20_token/data/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5307 2023-08-04 20:44:58.000000 eth-erc20-0.9.0/giftable_erc20_token/factory.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      108 2023-02-13 12:12:59.000000 eth-erc20-0.9.0/giftable_erc20_token/gen.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:43:34.076237 eth-erc20-0.9.0/giftable_erc20_token/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2803 2023-01-24 15:09:24.000000 eth-erc20-0.9.0/giftable_erc20_token/runnable/gift.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3431 2023-01-24 15:53:09.000000 eth-erc20-0.9.0/giftable_erc20_token/runnable/minter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3255 2023-02-21 18:21:49.000000 eth-erc20-0.9.0/giftable_erc20_token/runnable/publish.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:43:34.076237 eth-erc20-0.9.0/giftable_erc20_token/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-02-21 17:44:31.000000 eth-erc20-0.9.0/giftable_erc20_token/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2056 2023-07-26 08:51:01.000000 eth-erc20-0.9.0/giftable_erc20_token/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       67 2024-04-02 11:41:01.000000 eth-erc20-0.9.0/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1465 2024-04-02 11:43:34.079571 eth-erc20-0.9.0/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      666 2021-04-04 12:48:14.000000 eth-erc20-0.9.0/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:43:34.076237 eth-erc20-0.9.0/static_token/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:43:34.079571 eth-erc20-0.9.0/static_token/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)    11366 2023-03-02 11:29:39.000000 eth-erc20-0.9.0/static_token/data/StaticToken.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     3288 2023-03-02 11:29:39.000000 eth-erc20-0.9.0/static_token/data/StaticToken.json
+-rw-r--r--   0 lash      (1000) lash      (1000)       66 2022-04-22 18:28:18.000000 eth-erc20-0.9.0/static_token/data/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2024-04-02 11:41:16.000000 eth-erc20-0.9.0/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:43:34.079571 eth-erc20-0.9.0/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      266 2023-02-23 08:04:58.000000 eth-erc20-0.9.0/tests/test_erc20_interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4318 2023-02-22 10:16:13.000000 eth-erc20-0.9.0/tests/test_giftable.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      733 2023-06-29 19:52:55.000000 eth-erc20-0.9.0/tests/test_static.py
```

### Comparing `eth-erc20-0.8.0/CHANGELOG` & `eth-erc20-0.9.0/CHANGELOG`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/LICENSE` & `eth-erc20-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/PKG-INFO` & `eth-erc20-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-erc20
-Version: 0.8.0
+Version: 0.9.0
 Summary: ERC20 interface and simple contract with deployment script that lets any address mint and gift itself tokens.
 Home-page: https://git.defalsify.org/eth-erc20
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,ethereum,token,blockchain,cryptocurrency
 Classifier: Programming Language :: Python :: 3
@@ -13,7 +13,11 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: confini~=0.6.1
+Requires-Dist: chainlib-eth~=0.6.0
+Requires-Dist: chainlib~=0.5.0
+Requires-Dist: potaahto~=0.1.1
```

### Comparing `eth-erc20-0.8.0/WAIVER` & `eth-erc20-0.9.0/WAIVER`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/WAIVER.asc` & `eth-erc20-0.9.0/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/eth_erc20/data/ERC20.json` & `eth-erc20-0.9.0/eth_erc20/data/ERC20.json`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/eth_erc20/erc20.py` & `eth-erc20-0.9.0/eth_erc20/erc20.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/eth_erc20/runnable/balance.py` & `eth-erc20-0.9.0/eth_erc20/runnable/balance.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/eth_erc20/runnable/info.py` & `eth-erc20-0.9.0/eth_erc20/runnable/info.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/eth_erc20/runnable/transfer.py` & `eth-erc20-0.9.0/eth_erc20/runnable/transfer.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/eth_erc20/unittest/base.py` & `eth-erc20-0.9.0/eth_erc20/unittest/base.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/eth_erc20.egg-info/PKG-INFO` & `eth-erc20-0.9.0/eth_erc20.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-erc20
-Version: 0.8.0
+Version: 0.9.0
 Summary: ERC20 interface and simple contract with deployment script that lets any address mint and gift itself tokens.
 Home-page: https://git.defalsify.org/eth-erc20
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,ethereum,token,blockchain,cryptocurrency
 Classifier: Programming Language :: Python :: 3
@@ -13,7 +13,11 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: confini~=0.6.1
+Requires-Dist: chainlib-eth~=0.6.0
+Requires-Dist: chainlib~=0.5.0
+Requires-Dist: potaahto~=0.1.1
```

### Comparing `eth-erc20-0.8.0/eth_erc20.egg-info/SOURCES.txt` & `eth-erc20-0.9.0/eth_erc20.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/giftable_erc20_token/data/GiftableToken.bin` & `eth-erc20-0.9.0/giftable_erc20_token/data/GiftableToken.bin`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/giftable_erc20_token/data/GiftableToken.json` & `eth-erc20-0.9.0/giftable_erc20_token/data/GiftableToken.json`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/giftable_erc20_token/factory.py` & `eth-erc20-0.9.0/giftable_erc20_token/factory.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/giftable_erc20_token/runnable/gift.py` & `eth-erc20-0.9.0/giftable_erc20_token/runnable/gift.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/giftable_erc20_token/runnable/minter.py` & `eth-erc20-0.9.0/giftable_erc20_token/runnable/minter.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/giftable_erc20_token/runnable/publish.py` & `eth-erc20-0.9.0/giftable_erc20_token/runnable/publish.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/giftable_erc20_token/unittest/base.py` & `eth-erc20-0.9.0/giftable_erc20_token/unittest/base.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/setup.cfg` & `eth-erc20-0.9.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-erc20
-version = 0.8.0
+version = 0.9.0
 description = ERC20 interface and simple contract with deployment script that lets any address mint and gift itself tokens.
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-erc20
 keywords = 
 	dlt
 	ethereum
```

### Comparing `eth-erc20-0.8.0/setup.py` & `eth-erc20-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/static_token/data/StaticToken.bin` & `eth-erc20-0.9.0/static_token/data/StaticToken.bin`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/static_token/data/StaticToken.json` & `eth-erc20-0.9.0/static_token/data/StaticToken.json`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/tests/test_giftable.py` & `eth-erc20-0.9.0/tests/test_giftable.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.8.0/tests/test_static.py` & `eth-erc20-0.9.0/tests/test_static.py`

 * *Files identical despite different names*

