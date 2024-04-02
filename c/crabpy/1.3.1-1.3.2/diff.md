# Comparing `tmp/crabpy-1.3.1.tar.gz` & `tmp/crabpy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crabpy-1.3.1.tar", last modified: Fri Nov 24 14:13:30 2023, max compression
+gzip compressed data, was "crabpy-1.3.2.tar", last modified: Tue Apr  2 11:34:10 2024, max compression
```

## Comparing `crabpy-1.3.1.tar` & `crabpy-1.3.2.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-11-24 14:13:30.840226 crabpy-1.3.1/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7185 2023-11-24 14:13:18.000000 crabpy-1.3.1/CHANGES.rst
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 12:57:29.000000 crabpy-1.3.1/LICENSE
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       76 2023-04-13 12:57:29.000000 crabpy-1.3.1/MANIFEST.in
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8836 2023-11-24 14:13:30.840226 crabpy-1.3.1/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      941 2023-04-13 12:57:29.000000 crabpy-1.3.1/README.rst
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-11-24 14:13:30.836226 crabpy-1.3.1/crabpy/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.3.1/crabpy/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7552 2023-05-15 12:05:37.000000 crabpy-1.3.1/crabpy/client.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-11-24 14:13:30.840226 crabpy-1.3.1/crabpy/data/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    97092 2023-05-23 09:14:50.000000 crabpy-1.3.1/crabpy/data/deelgemeenten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   167480 2023-05-03 12:29:06.000000 crabpy-1.3.1/crabpy/data/gemeenten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      547 2023-05-03 12:29:06.000000 crabpy-1.3.1/crabpy/data/gewesten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      803 2023-05-04 09:43:10.000000 crabpy-1.3.1/crabpy/data/provincies.json
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-11-24 14:13:30.840226 crabpy-1.3.1/crabpy/gateway/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.3.1/crabpy/gateway/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    33688 2023-11-24 12:17:03.000000 crabpy-1.3.1/crabpy/gateway/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    28420 2023-04-13 12:57:29.000000 crabpy-1.3.1/crabpy/gateway/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    85501 2023-04-13 12:57:29.000000 crabpy-1.3.1/crabpy/gateway/crab.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      991 2023-04-13 12:57:29.000000 crabpy-1.3.1/crabpy/gateway/exception.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1083 2023-04-13 12:57:29.000000 crabpy-1.3.1/crabpy/wsa.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2719 2023-04-13 12:57:29.000000 crabpy-1.3.1/crabpy/wsse.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-11-24 14:13:30.836226 crabpy-1.3.1/crabpy.egg-info/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8836 2023-11-24 14:13:30.000000 crabpy-1.3.1/crabpy.egg-info/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      578 2023-11-24 14:13:30.000000 crabpy-1.3.1/crabpy.egg-info/SOURCES.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-11-24 14:13:30.000000 crabpy-1.3.1/crabpy.egg-info/dependency_links.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-11-24 14:13:30.000000 crabpy-1.3.1/crabpy.egg-info/entry_points.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 12:57:59.000000 crabpy-1.3.1/crabpy.egg-info/not-zip-safe
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       41 2023-11-24 14:13:30.000000 crabpy-1.3.1/crabpy.egg-info/requires.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        7 2023-11-24 14:13:30.000000 crabpy-1.3.1/crabpy.egg-info/top_level.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       38 2023-11-24 14:13:30.840226 crabpy-1.3.1/setup.cfg
--rwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)     1278 2023-11-24 14:13:18.000000 crabpy-1.3.1/setup.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2024-04-02 11:34:10.458039 crabpy-1.3.2/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7264 2024-04-02 11:19:52.000000 crabpy-1.3.2/CHANGES.rst
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 12:57:29.000000 crabpy-1.3.2/LICENSE
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       76 2023-04-13 12:57:29.000000 crabpy-1.3.2/MANIFEST.in
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8915 2024-04-02 11:34:10.458039 crabpy-1.3.2/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      941 2023-04-13 12:57:29.000000 crabpy-1.3.2/README.rst
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2024-04-02 11:34:10.454039 crabpy-1.3.2/crabpy/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.3.2/crabpy/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7674 2024-04-02 11:19:52.000000 crabpy-1.3.2/crabpy/client.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2024-04-02 11:34:10.454039 crabpy-1.3.2/crabpy/data/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    97092 2023-05-23 09:14:50.000000 crabpy-1.3.2/crabpy/data/deelgemeenten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   167480 2023-05-03 12:29:06.000000 crabpy-1.3.2/crabpy/data/gemeenten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      547 2023-05-03 12:29:06.000000 crabpy-1.3.2/crabpy/data/gewesten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      803 2023-05-04 09:43:10.000000 crabpy-1.3.2/crabpy/data/provincies.json
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2024-04-02 11:34:10.458039 crabpy-1.3.2/crabpy/gateway/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.3.2/crabpy/gateway/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    33688 2024-04-02 11:19:52.000000 crabpy-1.3.2/crabpy/gateway/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    28420 2023-04-13 12:57:29.000000 crabpy-1.3.2/crabpy/gateway/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    85501 2023-04-13 12:57:29.000000 crabpy-1.3.2/crabpy/gateway/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      991 2023-04-13 12:57:29.000000 crabpy-1.3.2/crabpy/gateway/exception.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1083 2023-04-13 12:57:29.000000 crabpy-1.3.2/crabpy/wsa.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2719 2023-04-13 12:57:29.000000 crabpy-1.3.2/crabpy/wsse.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2024-04-02 11:34:10.454039 crabpy-1.3.2/crabpy.egg-info/
+-rw-r--r--   0 claeyswo  (1001) claeyswo  (1001)     8915 2024-04-02 11:34:10.000000 crabpy-1.3.2/crabpy.egg-info/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      636 2024-04-02 11:34:10.000000 crabpy-1.3.2/crabpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2024-04-02 11:34:10.000000 crabpy-1.3.2/crabpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2024-04-02 11:34:10.000000 crabpy-1.3.2/crabpy.egg-info/entry_points.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 12:57:59.000000 crabpy-1.3.2/crabpy.egg-info/not-zip-safe
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       41 2024-04-02 11:34:10.000000 crabpy-1.3.2/crabpy.egg-info/requires.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        7 2024-04-02 11:34:10.000000 crabpy-1.3.2/crabpy.egg-info/top_level.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       38 2024-04-02 11:34:10.458039 crabpy-1.3.2/setup.cfg
+-rwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)     1278 2024-04-02 11:19:52.000000 crabpy-1.3.2/setup.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2024-04-02 11:34:10.458039 crabpy-1.3.2/tests/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5818 2024-04-02 11:21:07.000000 crabpy-1.3.2/tests/test_client.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      881 2023-04-13 12:57:29.000000 crabpy-1.3.2/tests/test_wsa.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1320 2023-04-13 12:57:29.000000 crabpy-1.3.2/tests/test_wsse.py
```

### Comparing `crabpy-1.3.1/CHANGES.rst` & `crabpy-1.3.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+1.3.2 (02-04-2024)
+------------------
+
+- Set x-api-key on all requests (#248)
+
 1.3.1 (23-11-2023)
 ------------------
 
 - Fix None rendering as string
 
 1.3.0 (23-11-2023)
 ------------------
```

### Comparing `crabpy-1.3.1/LICENSE` & `crabpy-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crabpy-1.3.1/PKG-INFO` & `crabpy-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: Interact with geographical webservices by Informatie Vlaanderen.
 Home-page: http://github.com/onroerenderfgoed/crabpy
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,19 @@
         :target: https://travis-ci.org/OnroerendErfgoed/crabpy
 .. image:: https://coveralls.io/repos/OnroerendErfgoed/crabpy/badge.png?branch=master
         :target: https://coveralls.io/r/OnroerendErfgoed/crabpy?branch=master
 .. image:: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/badges/quality-score.png?b=master
         :target: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/?branch=master
 
 
+1.3.2 (02-04-2024)
+------------------
+
+- Set x-api-key on all requests (#248)
+
 1.3.1 (23-11-2023)
 ------------------
 
 - Fix None rendering as string
 
 1.3.0 (23-11-2023)
 ------------------
```

### Comparing `crabpy-1.3.1/README.rst` & `crabpy-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `crabpy-1.3.1/crabpy/client.py` & `crabpy-1.3.2/crabpy/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,19 @@
                 result.extend(response[response_key])
         except RequestException as e:
             raise AdressenRegisterClientException from e
         return result
 
     def _get(self, url, params=None):
         try:
-            response = self.session.get(f"{self.base_url}{url}", params=params)
+            response = self.session.get(
+                f"{self.base_url}{url}",
+                params=params,
+                headers=self.v2_header if "v2" in url else self.v1_header,
+            )
             response.raise_for_status()
             return response.json()
         except RequestException as e:
             raise AdressenRegisterClientException from e
 
     def get_gemeente(self, gemeente_id):
         return self._get(f"/v2/gemeenten/{gemeente_id}")
```

### Comparing `crabpy-1.3.1/crabpy/data/deelgemeenten.json` & `crabpy-1.3.2/crabpy/data/deelgemeenten.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.3.1/crabpy/data/gemeenten.json` & `crabpy-1.3.2/crabpy/data/gemeenten.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.3.1/crabpy/data/gewesten.json` & `crabpy-1.3.2/crabpy/data/gewesten.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.3.1/crabpy/data/provincies.json` & `crabpy-1.3.2/crabpy/data/provincies.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.3.1/crabpy/gateway/adressenregister.py` & `crabpy-1.3.2/crabpy/gateway/adressenregister.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.3.1/crabpy/gateway/capakey.py` & `crabpy-1.3.2/crabpy/gateway/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.3.1/crabpy/gateway/crab.py` & `crabpy-1.3.2/crabpy/gateway/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.3.1/crabpy/gateway/exception.py` & `crabpy-1.3.2/crabpy/gateway/exception.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.3.1/crabpy/wsa.py` & `crabpy-1.3.2/crabpy/wsa.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.3.1/crabpy/wsse.py` & `crabpy-1.3.2/crabpy/wsse.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.3.1/crabpy.egg-info/PKG-INFO` & `crabpy-1.3.2/crabpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: Interact with geographical webservices by Informatie Vlaanderen.
 Home-page: http://github.com/onroerenderfgoed/crabpy
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,19 @@
         :target: https://travis-ci.org/OnroerendErfgoed/crabpy
 .. image:: https://coveralls.io/repos/OnroerendErfgoed/crabpy/badge.png?branch=master
         :target: https://coveralls.io/r/OnroerendErfgoed/crabpy?branch=master
 .. image:: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/badges/quality-score.png?b=master
         :target: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/?branch=master
 
 
+1.3.2 (02-04-2024)
+------------------
+
+- Set x-api-key on all requests (#248)
+
 1.3.1 (23-11-2023)
 ------------------
 
 - Fix None rendering as string
 
 1.3.0 (23-11-2023)
 ------------------
```

### Comparing `crabpy-1.3.1/setup.py` & `crabpy-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "crabpy",
 ]
 
 requires = ["suds-py3>=1.4.4.1", "dogpile.cache", "requests"]
 
 setup(
     name="crabpy",
-    version="1.3.1",
+    version="1.3.2",
     description="Interact with geographical webservices by Informatie Vlaanderen.",
     long_description=open("README.rst").read() + "\n\n" + open("CHANGES.rst").read(),
     author="Onroerend Erfgoed",
     author_email="ict@onroerenderfgoed.be",
     url="http://github.com/onroerenderfgoed/crabpy",
     packages=find_packages(exclude=["tests*"]),
     package_data={"": ["LICENSE"]},
```

