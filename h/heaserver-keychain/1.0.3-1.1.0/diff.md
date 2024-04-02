# Comparing `tmp/heaserver-keychain-1.0.3.tar.gz` & `tmp/heaserver-keychain-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-keychain-1.0.3.tar", last modified: Thu Mar 21 23:49:40 2024, max compression
+gzip compressed data, was "heaserver-keychain-1.1.0.tar", last modified: Tue Apr  2 21:33:21 2024, max compression
```

## Comparing `heaserver-keychain-1.0.3.tar` & `heaserver-keychain-1.1.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.290166 heaserver-keychain-1.0.3/
--rw-rw-rw-   0        0        0      325 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/.gitignore
--rw-rw-rw-   0        0        0     1579 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5094 2024-03-21 23:49:40.289146 heaserver-keychain-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3768 2024-03-21 23:48:35.000000 heaserver-keychain-1.0.3/README.md
--rw-rw-rw-   0        0        0     2654 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/RELEASING.md
--rw-rw-rw-   0        0        0      588 2024-03-02 01:08:06.000000 heaserver-keychain-1.0.3/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.105524 heaserver-keychain-1.0.3/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.105524 heaserver-keychain-1.0.3/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.191221 heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.205356 heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/__pycache__/
--rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.2384
--rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.29448
--rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.35952
--rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.36752
--rw-rw-rw-   0        0        0     4145 2024-03-02 01:08:06.000000 heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      404 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     1083 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     6556 2024-03-02 01:08:06.000000 heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      109 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/pytest.ini
--rw-rw-rw-   0        0        0      248 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/requirements_dev.txt
--rw-rw-rw-   0        0        0     1048 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-03-21 23:49:40.290166 heaserver-keychain-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1830 2024-03-21 23:48:51.000000 heaserver-keychain-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.107644 heaserver-keychain-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.106570 heaserver-keychain-1.0.3/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.215283 heaserver-keychain-1.0.3/src/heaserver/keychain/
--rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/src/heaserver/keychain/__init__.py
--rw-rw-rw-   0        0        0    17020 2024-03-02 01:08:06.000000 heaserver-keychain-1.0.3/src/heaserver/keychain/service.py
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.222790 heaserver-keychain-1.0.3/src/heaserver/keychain/wstl/
--rw-rw-rw-   0        0        0    17381 2024-03-02 01:08:06.000000 heaserver-keychain-1.0.3/src/heaserver/keychain/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.288121 heaserver-keychain-1.0.3/src/heaserver_keychain.egg-info/
--rw-rw-rw-   0        0        0     5094 2024-03-21 23:49:40.000000 heaserver-keychain-1.0.3/src/heaserver_keychain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2045 2024-03-21 23:49:40.000000 heaserver-keychain-1.0.3/src/heaserver_keychain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 23:49:40.000000 heaserver-keychain-1.0.3/src/heaserver_keychain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-03-21 23:49:40.000000 heaserver-keychain-1.0.3/src/heaserver_keychain.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-03-21 23:49:40.000000 heaserver-keychain-1.0.3/src/heaserver_keychain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-21 23:49:40.000000 heaserver-keychain-1.0.3/src/heaserver_keychain.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.108680 heaserver-keychain-1.0.3/tests/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.108680 heaserver-keychain-1.0.3/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.270567 heaserver-keychain-1.0.3/tests/heaserver/keychaintest/
--rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/tests/heaserver/keychaintest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 23:49:40.286029 heaserver-keychain-1.0.3/tests/heaserver/keychaintest/__pycache__/
--rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver-keychain-1.0.3/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.14948
--rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver-keychain-1.0.3/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.28348
--rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver-keychain-1.0.3/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.32848
--rw-rw-rw-   0        0        0     2205 2024-01-04 18:07:50.000000 heaserver-keychain-1.0.3/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.9296
--rw-rw-rw-   0        0        0     3778 2024-03-02 01:08:06.000000 heaserver-keychain-1.0.3/tests/heaserver/keychaintest/permissionstestcase.py
--rw-rw-rw-   0        0        0      404 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/tests/heaserver/keychaintest/test_all.py
--rw-rw-rw-   0        0        0     1083 2023-12-18 04:32:50.000000 heaserver-keychain-1.0.3/tests/heaserver/keychaintest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     6460 2024-03-02 01:08:06.000000 heaserver-keychain-1.0.3/tests/heaserver/keychaintest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.944562 heaserver-keychain-1.1.0/
+-rw-rw-rw-   0        0        0      325 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/.gitignore
+-rw-rw-rw-   0        0        0     1579 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5166 2024-04-02 21:33:21.942561 heaserver-keychain-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3840 2024-04-02 21:15:23.000000 heaserver-keychain-1.1.0/README.md
+-rw-rw-rw-   0        0        0     2654 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/RELEASING.md
+-rw-rw-rw-   0        0        0      588 2024-03-21 23:50:19.000000 heaserver-keychain-1.1.0/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.498855 heaserver-keychain-1.1.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.498855 heaserver-keychain-1.1.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.701391 heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.749389 heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/
+-rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.2384
+-rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.29448
+-rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.35952
+-rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.36752
+-rw-rw-rw-   0        0        0     4145 2024-03-21 23:50:19.000000 heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      404 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     1083 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     6556 2024-03-21 23:50:19.000000 heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      109 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/pytest.ini
+-rw-rw-rw-   0        0        0      248 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0     1048 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 21:33:21.945562 heaserver-keychain-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1830 2024-04-02 21:32:13.000000 heaserver-keychain-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.504852 heaserver-keychain-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.503852 heaserver-keychain-1.1.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.766389 heaserver-keychain-1.1.0/src/heaserver/keychain/
+-rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/src/heaserver/keychain/__init__.py
+-rw-rw-rw-   0        0        0    17020 2024-03-21 23:50:19.000000 heaserver-keychain-1.1.0/src/heaserver/keychain/service.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.779389 heaserver-keychain-1.1.0/src/heaserver/keychain/wstl/
+-rw-rw-rw-   0        0        0    17381 2024-03-21 23:50:19.000000 heaserver-keychain-1.1.0/src/heaserver/keychain/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.936532 heaserver-keychain-1.1.0/src/heaserver_keychain.egg-info/
+-rw-rw-rw-   0        0        0     5166 2024-04-02 21:33:21.000000 heaserver-keychain-1.1.0/src/heaserver_keychain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2045 2024-04-02 21:33:21.000000 heaserver-keychain-1.1.0/src/heaserver_keychain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 21:33:21.000000 heaserver-keychain-1.1.0/src/heaserver_keychain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-04-02 21:33:21.000000 heaserver-keychain-1.1.0/src/heaserver_keychain.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-02 21:33:21.000000 heaserver-keychain-1.1.0/src/heaserver_keychain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-02 21:33:21.000000 heaserver-keychain-1.1.0/src/heaserver_keychain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.506851 heaserver-keychain-1.1.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.507852 heaserver-keychain-1.1.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.889388 heaserver-keychain-1.1.0/tests/heaserver/keychaintest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/tests/heaserver/keychaintest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:33:21.934505 heaserver-keychain-1.1.0/tests/heaserver/keychaintest/__pycache__/
+-rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver-keychain-1.1.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.14948
+-rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver-keychain-1.1.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.28348
+-rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver-keychain-1.1.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.32848
+-rw-rw-rw-   0        0        0     2205 2024-01-04 18:07:50.000000 heaserver-keychain-1.1.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.9296
+-rw-rw-rw-   0        0        0     3778 2024-03-21 23:50:19.000000 heaserver-keychain-1.1.0/tests/heaserver/keychaintest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      404 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/tests/heaserver/keychaintest/test_all.py
+-rw-rw-rw-   0        0        0     1083 2023-12-18 04:32:50.000000 heaserver-keychain-1.1.0/tests/heaserver/keychaintest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     6460 2024-03-21 23:50:19.000000 heaserver-keychain-1.1.0/tests/heaserver/keychaintest/testcase.py
```

### Comparing `heaserver-keychain-1.0.3/Dockerfile` & `heaserver-keychain-1.1.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/LICENSE` & `heaserver-keychain-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/PKG-INFO` & `heaserver-keychain-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-keychain
-Version: 1.0.3
+Version: 1.1.0
 Summary: a service for managing laboratory credentials
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-keychain,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.8
+Requires-Dist: heaserver~=1.1.2
 
 # HEA Keychain
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA server Keychain is a service for managing laboratory and user credentials.
 
+## Version 1.1.0
+* Pass desktop object permissions back to clients.
+
 ## Version 1.0.3
 * Improved performance.
 
 ## Version 1.0.2
 * Added endpoint and links for generating an AWS CLI .aws/credentials file.
 
 ## Version 1.0.1
```

### Comparing `heaserver-keychain-1.0.3/README.md` & `heaserver-keychain-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Keychain
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA server Keychain is a service for managing laboratory and user credentials.
 
+## Version 1.1.0
+* Pass desktop object permissions back to clients.
+
 ## Version 1.0.3
 * Improved performance.
 
 ## Version 1.0.2
 * Added endpoint and links for generating an AWS CLI .aws/credentials file.
 
 ## Version 1.0.1
```

### Comparing `heaserver-keychain-1.0.3/RELEASING.md` & `heaserver-keychain-1.1.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/docker-entrypoint.sh` & `heaserver-keychain-1.1.0/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.2384` & `heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.2384`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.29448` & `heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.29448`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.35952` & `heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.35952`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.36752` & `heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.36752`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py` & `heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py` & `heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/integrationtests/heaserver/keychainintegrationtest/testcase.py` & `heaserver-keychain-1.1.0/integrationtests/heaserver/keychainintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/run-swaggerui.py` & `heaserver-keychain-1.1.0/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/setup.py` & `heaserver-keychain-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-keychain',
-    version='1.0.3',
+    version='1.1.0',
     description="a service for managing laboratory credentials",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.keychain'],
     package_data={'heaserver.keychain': ['wstl/*.json']},
-    install_requires=['heaserver~=1.0.8'],
+    install_requires=['heaserver~=1.1.2'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-keychain-1.0.3/src/heaserver/keychain/service.py` & `heaserver-keychain-1.1.0/src/heaserver/keychain/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/src/heaserver/keychain/wstl/all.json` & `heaserver-keychain-1.1.0/src/heaserver/keychain/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/src/heaserver_keychain.egg-info/PKG-INFO` & `heaserver-keychain-1.1.0/src/heaserver_keychain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-keychain
-Version: 1.0.3
+Version: 1.1.0
 Summary: a service for managing laboratory credentials
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-keychain,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.8
+Requires-Dist: heaserver~=1.1.2
 
 # HEA Keychain
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA server Keychain is a service for managing laboratory and user credentials.
 
+## Version 1.1.0
+* Pass desktop object permissions back to clients.
+
 ## Version 1.0.3
 * Improved performance.
 
 ## Version 1.0.2
 * Added endpoint and links for generating an AWS CLI .aws/credentials file.
 
 ## Version 1.0.1
```

### Comparing `heaserver-keychain-1.0.3/src/heaserver_keychain.egg-info/SOURCES.txt` & `heaserver-keychain-1.1.0/src/heaserver_keychain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.14948` & `heaserver-keychain-1.1.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.14948`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.28348` & `heaserver-keychain-1.1.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.28348`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.32848` & `heaserver-keychain-1.1.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.32848`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.9296` & `heaserver-keychain-1.1.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.9296`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/tests/heaserver/keychaintest/permissionstestcase.py` & `heaserver-keychain-1.1.0/tests/heaserver/keychaintest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/tests/heaserver/keychaintest/test_all_with_bad_permissions.py` & `heaserver-keychain-1.1.0/tests/heaserver/keychaintest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.3/tests/heaserver/keychaintest/testcase.py` & `heaserver-keychain-1.1.0/tests/heaserver/keychaintest/testcase.py`

 * *Files identical despite different names*

