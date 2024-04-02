# Comparing `tmp/datamarket-0.5.1.tar.gz` & `tmp/datamarket-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamarket-0.5.1.tar", last modified: Thu Mar 14 05:00:05 2024, max compression
+gzip compressed data, was "datamarket-0.5.2.tar", last modified: Tue Apr  2 08:08:59 2024, max compression
```

## Comparing `datamarket-0.5.1.tar` & `datamarket-0.5.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-14 05:00:05.901976 datamarket-0.5.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2024-03-14 04:40:04.000000 datamarket-0.5.1/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1671 2024-03-14 05:00:05.901976 datamarket-0.5.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2024-03-14 04:40:04.000000 datamarket-0.5.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-03-14 05:00:05.901976 datamarket-0.5.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1067 2024-03-14 04:56:50.000000 datamarket-0.5.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-14 05:00:05.897976 datamarket-0.5.1/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-14 05:00:05.897976 datamarket-0.5.1/src/datamarket/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2024-03-14 04:40:04.000000 datamarket-0.5.1/src/datamarket/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-14 05:00:05.901976 datamarket-0.5.1/src/datamarket/interfaces/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-14 04:40:04.000000 datamarket-0.5.1/src/datamarket/interfaces/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3398 2024-03-14 04:40:04.000000 datamarket-0.5.1/src/datamarket/interfaces/alchemy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2915 2024-03-14 04:40:04.000000 datamarket-0.5.1/src/datamarket/interfaces/drive.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2024-03-14 04:40:04.000000 datamarket-0.5.1/src/datamarket/interfaces/ftp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2730 2024-03-14 04:40:04.000000 datamarket-0.5.1/src/datamarket/interfaces/nominatim.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2024-03-14 04:40:04.000000 datamarket-0.5.1/src/datamarket/interfaces/proxy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2024-03-14 04:40:04.000000 datamarket-0.5.1/src/datamarket/interfaces/tinybird.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-14 05:00:05.901976 datamarket-0.5.1/src/datamarket/params/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-14 04:40:04.000000 datamarket-0.5.1/src/datamarket/params/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2024-03-14 04:40:04.000000 datamarket-0.5.1/src/datamarket/params/nominatim.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-14 05:00:05.901976 datamarket-0.5.1/src/datamarket/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2024-03-14 04:40:04.000000 datamarket-0.5.1/src/datamarket/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2270 2024-03-14 04:56:22.000000 datamarket-0.5.1/src/datamarket/utils/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2499 2024-03-14 04:40:04.000000 datamarket-0.5.1/src/datamarket/utils/selenium.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-14 05:00:05.901976 datamarket-0.5.1/src/datamarket.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1671 2024-03-14 05:00:05.000000 datamarket-0.5.1/src/datamarket.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      661 2024-03-14 05:00:05.000000 datamarket-0.5.1/src/datamarket.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-14 05:00:05.000000 datamarket-0.5.1/src/datamarket.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       80 2024-03-14 05:00:05.000000 datamarket-0.5.1/src/datamarket.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2024-03-14 05:00:05.000000 datamarket-0.5.1/src/datamarket.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 08:08:59.703861 datamarket-0.5.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2024-04-02 06:30:33.000000 datamarket-0.5.2/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1692 2024-04-02 08:08:59.703861 datamarket-0.5.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2024-04-02 06:30:33.000000 datamarket-0.5.2/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-02 08:08:59.703861 datamarket-0.5.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1080 2024-04-02 08:01:45.000000 datamarket-0.5.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 08:08:59.699861 datamarket-0.5.2/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 08:08:59.703861 datamarket-0.5.2/src/datamarket/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2024-04-02 06:30:33.000000 datamarket-0.5.2/src/datamarket/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 08:08:59.703861 datamarket-0.5.2/src/datamarket/interfaces/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 06:30:33.000000 datamarket-0.5.2/src/datamarket/interfaces/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3398 2024-04-02 06:30:33.000000 datamarket-0.5.2/src/datamarket/interfaces/alchemy.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1252 2024-04-02 07:42:08.000000 datamarket-0.5.2/src/datamarket/interfaces/aws.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2915 2024-04-02 06:30:33.000000 datamarket-0.5.2/src/datamarket/interfaces/drive.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2024-04-02 06:30:33.000000 datamarket-0.5.2/src/datamarket/interfaces/ftp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2730 2024-04-02 06:30:33.000000 datamarket-0.5.2/src/datamarket/interfaces/nominatim.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2024-04-02 06:30:33.000000 datamarket-0.5.2/src/datamarket/interfaces/proxy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2024-04-02 06:30:33.000000 datamarket-0.5.2/src/datamarket/interfaces/tinybird.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 08:08:59.703861 datamarket-0.5.2/src/datamarket/params/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 06:30:33.000000 datamarket-0.5.2/src/datamarket/params/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2024-04-02 06:30:33.000000 datamarket-0.5.2/src/datamarket/params/nominatim.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 08:08:59.703861 datamarket-0.5.2/src/datamarket/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2024-04-02 06:30:33.000000 datamarket-0.5.2/src/datamarket/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2270 2024-04-02 06:30:33.000000 datamarket-0.5.2/src/datamarket/utils/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2499 2024-04-02 06:30:33.000000 datamarket-0.5.2/src/datamarket/utils/selenium.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 08:08:59.703861 datamarket-0.5.2/src/datamarket.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1692 2024-04-02 08:08:59.000000 datamarket-0.5.2/src/datamarket.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      694 2024-04-02 08:08:59.000000 datamarket-0.5.2/src/datamarket.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-02 08:08:59.000000 datamarket-0.5.2/src/datamarket.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       86 2024-04-02 08:08:59.000000 datamarket-0.5.2/src/datamarket.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       11 2024-04-02 08:08:59.000000 datamarket-0.5.2/src/datamarket.egg-info/top_level.txt
```

### Comparing `datamarket-0.5.1/LICENSE` & `datamarket-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.1/PKG-INFO` & `datamarket-0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.5.1
+Version: 0.5.2
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,14 +15,15 @@
 Requires-Dist: sqlalchemy
 Requires-Dist: requests[socks]
 Requires-Dist: retry
 Requires-Dist: stem
 Requires-Dist: pydrive2
 Requires-Dist: undetected_chromedriver
 Requires-Dist: pendulum
+Requires-Dist: boto3
 
 # DataMarket scraping core
 
 ------------------------------------------------------
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `datamarket-0.5.1/README.md` & `datamarket-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.1/setup.py` & `datamarket-0.5.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,19 +11,20 @@
     "sqlalchemy",
     "requests[socks]",
     "retry",
     "stem",
     "pydrive2",
     "undetected_chromedriver",
     "pendulum",
+    "boto3",
 ]
 
 setuptools.setup(
     name="datamarket",
-    version="0.5.1",
+    version="0.5.2",
     author="DataMarket",
     author_email="techsupport@datamarket.es",
     description="Utilities that integrate advance scraping knowledge into just one library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Data-Market/datamarket",
     project_urls={
```

### Comparing `datamarket-0.5.1/src/datamarket/interfaces/alchemy.py` & `datamarket-0.5.2/src/datamarket/interfaces/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.1/src/datamarket/interfaces/drive.py` & `datamarket-0.5.2/src/datamarket/interfaces/drive.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.1/src/datamarket/interfaces/ftp.py` & `datamarket-0.5.2/src/datamarket/interfaces/ftp.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.1/src/datamarket/interfaces/nominatim.py` & `datamarket-0.5.2/src/datamarket/interfaces/nominatim.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.1/src/datamarket/interfaces/proxy.py` & `datamarket-0.5.2/src/datamarket/interfaces/proxy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.1/src/datamarket/interfaces/tinybird.py` & `datamarket-0.5.2/src/datamarket/interfaces/tinybird.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.1/src/datamarket/params/nominatim.py` & `datamarket-0.5.2/src/datamarket/params/nominatim.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.1/src/datamarket/utils/main.py` & `datamarket-0.5.2/src/datamarket/utils/main.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.1/src/datamarket/utils/selenium.py` & `datamarket-0.5.2/src/datamarket/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.1/src/datamarket.egg-info/PKG-INFO` & `datamarket-0.5.2/src/datamarket.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.5.1
+Version: 0.5.2
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,14 +15,15 @@
 Requires-Dist: sqlalchemy
 Requires-Dist: requests[socks]
 Requires-Dist: retry
 Requires-Dist: stem
 Requires-Dist: pydrive2
 Requires-Dist: undetected_chromedriver
 Requires-Dist: pendulum
+Requires-Dist: boto3
 
 # DataMarket scraping core
 
 ------------------------------------------------------
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `datamarket-0.5.1/src/datamarket.egg-info/SOURCES.txt` & `datamarket-0.5.2/src/datamarket.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/datamarket.egg-info/PKG-INFO
 src/datamarket.egg-info/SOURCES.txt
 src/datamarket.egg-info/dependency_links.txt
 src/datamarket.egg-info/requires.txt
 src/datamarket.egg-info/top_level.txt
 src/datamarket/interfaces/__init__.py
 src/datamarket/interfaces/alchemy.py
+src/datamarket/interfaces/aws.py
 src/datamarket/interfaces/drive.py
 src/datamarket/interfaces/ftp.py
 src/datamarket/interfaces/nominatim.py
 src/datamarket/interfaces/proxy.py
 src/datamarket/interfaces/tinybird.py
 src/datamarket/params/__init__.py
 src/datamarket/params/nominatim.py
```

