# Comparing `tmp/tranco-0.8.0.tar.gz` & `tmp/tranco-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tranco-0.8.0.tar", last modified: Tue Mar 26 19:30:47 2024, max compression
+gzip compressed data, was "tranco-0.8.1.tar", last modified: Tue Apr  2 12:49:58 2024, max compression
```

## Comparing `tranco-0.8.0.tar` & `tranco-0.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 victor     (501) staff       (20)        0 2024-03-26 19:30:47.539726 tranco-0.8.0/
--rw-rw-r--   0 victor     (501) staff       (20)     1072 2023-11-15 10:03:48.000000 tranco-0.8.0/LICENSE
--rw-r--r--   0 victor     (501) staff       (20)     3092 2024-03-26 19:30:47.539519 tranco-0.8.0/PKG-INFO
--rw-rw-r--   0 victor     (501) staff       (20)     2495 2024-03-26 19:30:41.000000 tranco-0.8.0/README.md
--rw-r--r--   0 victor     (501) staff       (20)       38 2024-03-26 19:30:47.539768 tranco-0.8.0/setup.cfg
--rw-rw-r--   0 victor     (501) staff       (20)      834 2024-03-26 14:34:16.000000 tranco-0.8.0/setup.py
-drwxr-xr-x   0 victor     (501) staff       (20)        0 2024-03-26 19:30:47.536517 tranco-0.8.0/tests/
--rw-rw-r--   0 victor     (501) staff       (20)        0 2023-11-15 15:32:56.000000 tranco-0.8.0/tests/__init__.py
--rw-rw-r--   0 victor     (501) staff       (20)      243 2024-03-26 19:02:43.000000 tranco-0.8.0/tests/conftest.py
--rw-r--r--   0 victor     (501) staff       (20)       95 2024-03-26 19:07:39.000000 tranco-0.8.0/tests/test_download.py
--rw-r--r--   0 victor     (501) staff       (20)      426 2024-03-26 19:09:28.000000 tranco-0.8.0/tests/test_parameters.py
--rw-rw-r--   0 victor     (501) staff       (20)      550 2023-11-15 16:05:01.000000 tranco-0.8.0/tests/test_performance.py
--rw-r--r--   0 victor     (501) staff       (20)      262 2024-03-26 19:07:03.000000 tranco-0.8.0/tests/test_rank.py
--rw-rw-r--   0 victor     (501) staff       (20)      163 2024-03-26 19:07:03.000000 tranco-0.8.0/tests/test_top.py
-drwxr-xr-x   0 victor     (501) staff       (20)        0 2024-03-26 19:30:47.537040 tranco-0.8.0/tranco/
--rw-rw-r--   0 victor     (501) staff       (20)       26 2023-11-15 10:03:48.000000 tranco-0.8.0/tranco/__init__.py
--rw-rw-r--   0 victor     (501) staff       (20)    10424 2024-03-26 19:23:55.000000 tranco-0.8.0/tranco/tranco.py
-drwxr-xr-x   0 victor     (501) staff       (20)        0 2024-03-26 19:30:47.539160 tranco-0.8.0/tranco.egg-info/
--rw-r--r--   0 victor     (501) staff       (20)     3092 2024-03-26 19:30:47.000000 tranco-0.8.0/tranco.egg-info/PKG-INFO
--rw-rw-r--   0 victor     (501) staff       (20)      358 2024-03-26 19:30:47.000000 tranco-0.8.0/tranco.egg-info/SOURCES.txt
--rw-rw-r--   0 victor     (501) staff       (20)        1 2024-03-26 19:30:47.000000 tranco-0.8.0/tranco.egg-info/dependency_links.txt
--rw-rw-r--   0 victor     (501) staff       (20)       34 2024-03-26 19:30:47.000000 tranco-0.8.0/tranco.egg-info/requires.txt
--rw-rw-r--   0 victor     (501) staff       (20)       13 2024-03-26 19:30:47.000000 tranco-0.8.0/tranco.egg-info/top_level.txt
+drwxr-xr-x   0 victor     (501) staff       (20)        0 2024-04-02 12:49:58.700194 tranco-0.8.1/
+-rw-rw-r--   0 victor     (501) staff       (20)     1072 2023-11-15 10:03:48.000000 tranco-0.8.1/LICENSE
+-rw-r--r--   0 victor     (501) staff       (20)     3092 2024-04-02 12:49:58.699997 tranco-0.8.1/PKG-INFO
+-rw-rw-r--   0 victor     (501) staff       (20)     2495 2024-03-26 19:30:41.000000 tranco-0.8.1/README.md
+-rw-r--r--   0 victor     (501) staff       (20)       38 2024-04-02 12:49:58.700257 tranco-0.8.1/setup.cfg
+-rw-rw-r--   0 victor     (501) staff       (20)      834 2024-04-02 12:49:03.000000 tranco-0.8.1/setup.py
+drwxr-xr-x   0 victor     (501) staff       (20)        0 2024-04-02 12:49:58.697969 tranco-0.8.1/tests/
+-rw-rw-r--   0 victor     (501) staff       (20)        0 2023-11-15 15:32:56.000000 tranco-0.8.1/tests/__init__.py
+-rw-rw-r--   0 victor     (501) staff       (20)      243 2024-03-26 19:02:43.000000 tranco-0.8.1/tests/conftest.py
+-rw-r--r--   0 victor     (501) staff       (20)       95 2024-03-26 19:07:39.000000 tranco-0.8.1/tests/test_download.py
+-rw-r--r--   0 victor     (501) staff       (20)      426 2024-03-26 19:09:28.000000 tranco-0.8.1/tests/test_parameters.py
+-rw-rw-r--   0 victor     (501) staff       (20)      550 2023-11-15 16:05:01.000000 tranco-0.8.1/tests/test_performance.py
+-rw-r--r--   0 victor     (501) staff       (20)      262 2024-03-26 19:07:03.000000 tranco-0.8.1/tests/test_rank.py
+-rw-rw-r--   0 victor     (501) staff       (20)      163 2024-03-26 19:07:03.000000 tranco-0.8.1/tests/test_top.py
+drwxr-xr-x   0 victor     (501) staff       (20)        0 2024-04-02 12:49:58.698488 tranco-0.8.1/tranco/
+-rw-rw-r--   0 victor     (501) staff       (20)       26 2023-11-15 10:03:48.000000 tranco-0.8.1/tranco/__init__.py
+-rw-r--r--   0 victor     (501) staff       (20)    10446 2024-04-02 12:49:03.000000 tranco-0.8.1/tranco/tranco.py
+drwxr-xr-x   0 victor     (501) staff       (20)        0 2024-04-02 12:49:58.699631 tranco-0.8.1/tranco.egg-info/
+-rw-r--r--   0 victor     (501) staff       (20)     3092 2024-04-02 12:49:58.000000 tranco-0.8.1/tranco.egg-info/PKG-INFO
+-rw-rw-r--   0 victor     (501) staff       (20)      358 2024-04-02 12:49:58.000000 tranco-0.8.1/tranco.egg-info/SOURCES.txt
+-rw-rw-r--   0 victor     (501) staff       (20)        1 2024-04-02 12:49:58.000000 tranco-0.8.1/tranco.egg-info/dependency_links.txt
+-rw-rw-r--   0 victor     (501) staff       (20)       34 2024-04-02 12:49:58.000000 tranco-0.8.1/tranco.egg-info/requires.txt
+-rw-rw-r--   0 victor     (501) staff       (20)       13 2024-04-02 12:49:58.000000 tranco-0.8.1/tranco.egg-info/top_level.txt
```

### Comparing `tranco-0.8.0/LICENSE` & `tranco-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tranco-0.8.0/PKG-INFO` & `tranco-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tranco
-Version: 0.8.0
+Version: 0.8.1
 Summary: Tranco: A Research-Oriented Top Sites Ranking Hardened Against Manipulation
 Home-page: https://github.com/DistriNet/tranco-python-package
 Author: Victor Le Pochat
 Author-email: victor.lepochat@kuleuven.be
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tranco-0.8.0/README.md` & `tranco-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `tranco-0.8.0/setup.py` & `tranco-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tranco",
-    version="0.8.0",
+    version="0.8.1",
     author="Victor Le Pochat",
     author_email="victor.lepochat@kuleuven.be",
     description="Tranco: A Research-Oriented Top Sites Ranking Hardened Against Manipulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DistriNet/tranco-python-package",
     packages=setuptools.find_packages(),
```

### Comparing `tranco-0.8.0/tests/test_performance.py` & `tranco-0.8.1/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `tranco-0.8.0/tranco/tranco.py` & `tranco-0.8.1/tranco/tranco.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import requests
 import os
 import platform
 import zipfile
 from warnings import warn
 from enum import IntEnum
 
-VERSION = '0.8.0'
+VERSION = '0.8.1'
 
 
 class TrancoList:
     def __init__(self, date: str, list_id: str, lst: List[str]) -> None:
         self.date: str = date
         self.list_id: str = list_id
         self.list_page: str = "https://tranco-list.eu/list/{}/".format(list_id)
@@ -126,15 +126,15 @@
 
         if not self._is_cached(list_id, full):
             self._download_file(list_id, full)  # download list and load into cache
         with open(self._cache_path(list_id)) as f:  # read list from cache
             if full:
                 top_list_lines = f.read().splitlines()
             else:
-                top_list_lines = list(islice(f, 1000000))
+                top_list_lines = [line.rstrip() for line in islice(f, 1000000)]
 
         return TrancoList(date, list_id, list(map(lambda x: x[x.index(',') + 1:], top_list_lines)))
 
     def _get_list_id_for_date(self, date: str, subdomains: bool = False) -> str:
         r1 = self.session.get(
             'https://tranco-list.eu/daily_list_id?date={}&subdomains={}'.format(date, str(subdomains).lower()))
         if r1.status_code == 200:
```

### Comparing `tranco-0.8.0/tranco.egg-info/PKG-INFO` & `tranco-0.8.1/tranco.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tranco
-Version: 0.8.0
+Version: 0.8.1
 Summary: Tranco: A Research-Oriented Top Sites Ranking Hardened Against Manipulation
 Home-page: https://github.com/DistriNet/tranco-python-package
 Author: Victor Le Pochat
 Author-email: victor.lepochat@kuleuven.be
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

