# Comparing `tmp/funga-eth-0.7.4.tar.gz` & `tmp/funga-eth-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funga-eth-0.7.4.tar", last modified: Sat Jun 24 23:15:44 2023, max compression
+gzip compressed data, was "funga-eth-0.8.0.tar", last modified: Tue Apr  2 11:04:25 2024, max compression
```

## Comparing `funga-eth-0.7.4.tar` & `funga-eth-0.8.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-24 23:15:44.583323 funga-eth-0.7.4/
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:49:56.000000 funga-eth-0.7.4/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       82 2023-06-03 12:07:27.000000 funga-eth-0.7.4/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)     2008 2023-06-24 23:15:44.583323 funga-eth-0.7.4/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1322 2023-06-03 12:11:27.000000 funga-eth-0.7.4/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 07:51:12.000000 funga-eth-0.7.4/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1630 2022-11-14 07:51:25.000000 funga-eth-0.7.4/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-24 23:15:44.576656 funga-eth-0.7.4/funga/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-24 23:15:44.579990 funga-eth-0.7.4/funga/eth/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:17:05.000000 funga-eth-0.7.4/funga/eth/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-24 23:15:44.579990 funga-eth-0.7.4/funga/eth/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:17:05.000000 funga-eth-0.7.4/funga/eth/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3564 2021-10-10 10:17:05.000000 funga-eth-0.7.4/funga/eth/cli/handle.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2298 2021-10-15 20:57:44.000000 funga-eth-0.7.4/funga/eth/cli/http.py
--rw-r--r--   0 lash      (1000) lash      (1000)      556 2021-10-10 10:17:05.000000 funga-eth-0.7.4/funga/eth/cli/jsonrpc.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1546 2021-10-15 20:39:41.000000 funga-eth-0.7.4/funga/eth/cli/socket.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-24 23:15:44.576656 funga-eth-0.7.4/funga/eth/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-24 23:15:44.579990 funga-eth-0.7.4/funga/eth/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)       76 2021-10-10 10:17:05.000000 funga-eth-0.7.4/funga/eth/data/config/database.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       82 2021-10-10 10:17:05.000000 funga-eth-0.7.4/funga/eth/data/config/signer.ini
--rw-r--r--   0 lash      (1000) lash      (1000)     2691 2023-06-16 14:38:42.000000 funga-eth-0.7.4/funga/eth/encoding.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-24 23:15:44.579990 funga-eth-0.7.4/funga/eth/keystore/
--rw-r--r--   0 lash      (1000) lash      (1000)      209 2021-10-10 10:17:05.000000 funga-eth-0.7.4/funga/eth/keystore/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1143 2021-10-10 11:04:50.000000 funga-eth-0.7.4/funga/eth/keystore/dict.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1560 2022-01-24 11:37:10.000000 funga-eth-0.7.4/funga/eth/keystore/interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5335 2022-01-25 09:02:00.000000 funga-eth-0.7.4/funga/eth/keystore/keyfile.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3659 2021-10-30 06:00:33.000000 funga-eth-0.7.4/funga/eth/keystore/sql.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1313 2023-06-16 14:12:48.000000 funga-eth-0.7.4/funga/eth/message.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-24 23:15:44.579990 funga-eth-0.7.4/funga/eth/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     3258 2023-06-16 14:36:05.000000 funga-eth-0.7.4/funga/eth/runnable/keyfile.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2333 2023-06-24 16:35:40.000000 funga-eth-0.7.4/funga/eth/runnable/msg.py
--rwxr-xr-x   0 lash      (1000) lash      (1000)     4308 2023-06-03 12:25:41.000000 funga-eth-0.7.4/funga/eth/runnable/signer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-24 23:15:44.583323 funga-eth-0.7.4/funga/eth/signer/
--rw-r--r--   0 lash      (1000) lash      (1000)       56 2023-03-13 16:41:32.000000 funga-eth-0.7.4/funga/eth/signer/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3210 2023-03-28 15:47:47.000000 funga-eth-0.7.4/funga/eth/signer/defaultsigner.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4693 2021-10-15 20:59:28.000000 funga-eth-0.7.4/funga/eth/transaction.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-24 23:15:44.583323 funga-eth-0.7.4/funga_eth.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)     2008 2023-06-24 23:15:44.000000 funga-eth-0.7.4/funga_eth.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1006 2023-06-24 23:15:44.000000 funga-eth-0.7.4/funga_eth.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-24 23:15:44.000000 funga-eth-0.7.4/funga_eth.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      151 2023-06-24 23:15:44.000000 funga-eth-0.7.4/funga_eth.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      192 2023-06-24 23:15:44.000000 funga-eth-0.7.4/funga_eth.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        6 2023-06-24 23:15:44.000000 funga-eth-0.7.4/funga_eth.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      162 2023-06-10 08:12:46.000000 funga-eth-0.7.4/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      399 2023-06-24 23:15:44.583323 funga-eth-0.7.4/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)     1625 2023-06-24 16:53:41.000000 funga-eth-0.7.4/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       35 2021-10-10 16:05:05.000000 funga-eth-0.7.4/sql_requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 16:05:05.000000 funga-eth-0.7.4/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-24 23:15:44.583323 funga-eth-0.7.4/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     3477 2022-01-25 09:02:00.000000 funga-eth-0.7.4/tests/test_cli.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1519 2021-10-10 10:17:05.000000 funga-eth-0.7.4/tests/test_keystore_dict.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1537 2022-01-25 09:02:00.000000 funga-eth-0.7.4/tests/test_pbkdf2.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2855 2021-10-10 10:17:05.000000 funga-eth-0.7.4/tests/test_sign.py
--rw-r--r--   0 lash      (1000) lash      (1000)      268 2021-10-10 10:17:05.000000 funga-eth-0.7.4/tests/test_socket.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:04:25.716252 funga-eth-0.8.0/
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:49:56.000000 funga-eth-0.8.0/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       82 2023-06-03 12:07:27.000000 funga-eth-0.8.0/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)     2390 2024-04-02 11:04:25.716252 funga-eth-0.8.0/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1322 2023-06-03 12:11:27.000000 funga-eth-0.8.0/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 07:51:12.000000 funga-eth-0.8.0/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1630 2022-11-14 07:51:25.000000 funga-eth-0.8.0/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:04:25.712918 funga-eth-0.8.0/funga/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:04:25.712918 funga-eth-0.8.0/funga/eth/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:17:05.000000 funga-eth-0.8.0/funga/eth/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:04:25.716252 funga-eth-0.8.0/funga/eth/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:17:05.000000 funga-eth-0.8.0/funga/eth/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3564 2021-10-10 10:17:05.000000 funga-eth-0.8.0/funga/eth/cli/handle.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2298 2021-10-15 20:57:44.000000 funga-eth-0.8.0/funga/eth/cli/http.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      556 2021-10-10 10:17:05.000000 funga-eth-0.8.0/funga/eth/cli/jsonrpc.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1546 2021-10-15 20:39:41.000000 funga-eth-0.8.0/funga/eth/cli/socket.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:04:25.712918 funga-eth-0.8.0/funga/eth/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:04:25.716252 funga-eth-0.8.0/funga/eth/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)       76 2021-10-10 10:17:05.000000 funga-eth-0.8.0/funga/eth/data/config/database.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       82 2021-10-10 10:17:05.000000 funga-eth-0.8.0/funga/eth/data/config/signer.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)     2691 2023-06-16 14:38:42.000000 funga-eth-0.8.0/funga/eth/encoding.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:04:25.716252 funga-eth-0.8.0/funga/eth/keystore/
+-rw-r--r--   0 lash      (1000) lash      (1000)      209 2021-10-10 10:17:05.000000 funga-eth-0.8.0/funga/eth/keystore/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1143 2021-10-10 11:04:50.000000 funga-eth-0.8.0/funga/eth/keystore/dict.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1560 2022-01-24 11:37:10.000000 funga-eth-0.8.0/funga/eth/keystore/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5335 2022-01-25 09:02:00.000000 funga-eth-0.8.0/funga/eth/keystore/keyfile.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3659 2021-10-30 06:00:33.000000 funga-eth-0.8.0/funga/eth/keystore/sql.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1313 2023-06-16 14:12:48.000000 funga-eth-0.8.0/funga/eth/message.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:04:25.716252 funga-eth-0.8.0/funga/eth/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3258 2023-06-16 14:36:05.000000 funga-eth-0.8.0/funga/eth/runnable/keyfile.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2333 2023-06-24 16:35:40.000000 funga-eth-0.8.0/funga/eth/runnable/msg.py
+-rwxr-xr-x   0 lash      (1000) lash      (1000)     4308 2023-06-03 12:25:41.000000 funga-eth-0.8.0/funga/eth/runnable/signer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:04:25.716252 funga-eth-0.8.0/funga/eth/signer/
+-rw-r--r--   0 lash      (1000) lash      (1000)       56 2023-03-13 16:41:32.000000 funga-eth-0.8.0/funga/eth/signer/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3210 2023-03-28 15:47:47.000000 funga-eth-0.8.0/funga/eth/signer/defaultsigner.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4693 2021-10-15 20:59:28.000000 funga-eth-0.8.0/funga/eth/transaction.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:04:25.716252 funga-eth-0.8.0/funga_eth.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2390 2024-04-02 11:04:25.000000 funga-eth-0.8.0/funga_eth.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1006 2024-04-02 11:04:25.000000 funga-eth-0.8.0/funga_eth.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2024-04-02 11:04:25.000000 funga-eth-0.8.0/funga_eth.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      151 2024-04-02 11:04:25.000000 funga-eth-0.8.0/funga_eth.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      192 2024-04-02 11:04:25.000000 funga-eth-0.8.0/funga_eth.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        6 2024-04-02 11:04:25.000000 funga-eth-0.8.0/funga_eth.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      150 2024-04-02 10:08:57.000000 funga-eth-0.8.0/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      399 2024-04-02 11:04:25.716252 funga-eth-0.8.0/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)     1625 2024-04-02 11:01:10.000000 funga-eth-0.8.0/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       35 2021-10-10 16:05:05.000000 funga-eth-0.8.0/sql_requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 16:05:05.000000 funga-eth-0.8.0/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:04:25.716252 funga-eth-0.8.0/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3477 2022-01-25 09:02:00.000000 funga-eth-0.8.0/tests/test_cli.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1519 2021-10-10 10:17:05.000000 funga-eth-0.8.0/tests/test_keystore_dict.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1537 2022-01-25 09:02:00.000000 funga-eth-0.8.0/tests/test_pbkdf2.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2855 2021-10-10 10:17:05.000000 funga-eth-0.8.0/tests/test_sign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      268 2021-10-10 10:17:05.000000 funga-eth-0.8.0/tests/test_socket.py
```

### Comparing `funga-eth-0.7.4/LICENSE` & `funga-eth-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/PKG-INFO` & `funga-eth-0.8.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 Metadata-Version: 2.1
 Name: funga-eth
-Version: 0.7.4
+Version: 0.8.0
 Summary: Ethereum implementation of the funga keystore and signer
 Home-page: https://git.defalsify.org/funga-eth
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Description-Content-Type: text/markdown
-Provides-Extra: sql
 License-File: LICENSE
+Requires-Dist: cryptography==3.2.1
+Requires-Dist: safe-pysha3==1.0.4
+Requires-Dist: rlp==3.0.0
+Requires-Dist: json-rpc==1.13.0
+Requires-Dist: confini~=0.6.0
+Requires-Dist: coincurve==15.0.0
+Requires-Dist: hexathon~=0.1.6
+Requires-Dist: pycryptodome==3.10.1
+Requires-Dist: funga~=0.5.6
+Provides-Extra: sql
+Requires-Dist: psycopg2==2.8.6; extra == "sql"
+Requires-Dist: sqlalchemy==1.3.20; extra == "sql"
 
 # funga-eth
 
 Ethereum implementation of the `funga` signer interface.
 
 See https://git.defalsify.org/funga for more details.
```

### Comparing `funga-eth-0.7.4/README.md` & `funga-eth-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/WAIVER` & `funga-eth-0.8.0/WAIVER`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/WAIVER.asc` & `funga-eth-0.8.0/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/cli/handle.py` & `funga-eth-0.8.0/funga/eth/cli/handle.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/cli/http.py` & `funga-eth-0.8.0/funga/eth/cli/http.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/cli/jsonrpc.py` & `funga-eth-0.8.0/funga/eth/cli/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/cli/socket.py` & `funga-eth-0.8.0/funga/eth/cli/socket.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/encoding.py` & `funga-eth-0.8.0/funga/eth/encoding.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/keystore/dict.py` & `funga-eth-0.8.0/funga/eth/keystore/dict.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/keystore/interface.py` & `funga-eth-0.8.0/funga/eth/keystore/interface.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/keystore/keyfile.py` & `funga-eth-0.8.0/funga/eth/keystore/keyfile.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/keystore/sql.py` & `funga-eth-0.8.0/funga/eth/keystore/sql.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/message.py` & `funga-eth-0.8.0/funga/eth/message.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/runnable/keyfile.py` & `funga-eth-0.8.0/funga/eth/runnable/keyfile.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/runnable/msg.py` & `funga-eth-0.8.0/funga/eth/runnable/msg.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/runnable/signer.py` & `funga-eth-0.8.0/funga/eth/runnable/signer.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/signer/defaultsigner.py` & `funga-eth-0.8.0/funga/eth/signer/defaultsigner.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga/eth/transaction.py` & `funga-eth-0.8.0/funga/eth/transaction.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/funga_eth.egg-info/PKG-INFO` & `funga-eth-0.8.0/funga_eth.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 Metadata-Version: 2.1
 Name: funga-eth
-Version: 0.7.4
+Version: 0.8.0
 Summary: Ethereum implementation of the funga keystore and signer
 Home-page: https://git.defalsify.org/funga-eth
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Description-Content-Type: text/markdown
-Provides-Extra: sql
 License-File: LICENSE
+Requires-Dist: cryptography==3.2.1
+Requires-Dist: safe-pysha3==1.0.4
+Requires-Dist: rlp==3.0.0
+Requires-Dist: json-rpc==1.13.0
+Requires-Dist: confini~=0.6.0
+Requires-Dist: coincurve==15.0.0
+Requires-Dist: hexathon~=0.1.6
+Requires-Dist: pycryptodome==3.10.1
+Requires-Dist: funga~=0.5.6
+Provides-Extra: sql
+Requires-Dist: psycopg2==2.8.6; extra == "sql"
+Requires-Dist: sqlalchemy==1.3.20; extra == "sql"
 
 # funga-eth
 
 Ethereum implementation of the `funga` signer interface.
 
 See https://git.defalsify.org/funga for more details.
```

### Comparing `funga-eth-0.7.4/funga_eth.egg-info/SOURCES.txt` & `funga-eth-0.8.0/funga_eth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/setup.py` & `funga-eth-0.8.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 f = open('README.md', 'r')
 description = f.read()
 f.close()
 
 setup(
         name="funga-eth",
-        version="0.7.4",
+        version="0.8.0",
         description="Ethereum implementation of the funga keystore and signer",
         author="Louis Holbrook",
         author_email="dev@holbrook.no",
         packages=[
             'funga.eth.signer',
             'funga.eth',
             'funga.eth.cli',
```

### Comparing `funga-eth-0.7.4/tests/test_cli.py` & `funga-eth-0.8.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/tests/test_keystore_dict.py` & `funga-eth-0.8.0/tests/test_keystore_dict.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/tests/test_pbkdf2.py` & `funga-eth-0.8.0/tests/test_pbkdf2.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.4/tests/test_sign.py` & `funga-eth-0.8.0/tests/test_sign.py`

 * *Files identical despite different names*

