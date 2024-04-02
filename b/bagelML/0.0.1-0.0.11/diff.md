# Comparing `tmp/bagelML-0.0.1.tar.gz` & `tmp/bagelML-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bagelML-0.0.1.tar", last modified: Mon Apr  1 23:56:02 2024, max compression
+gzip compressed data, was "bagelML-0.0.11.tar", last modified: Tue Apr  2 01:19:00 2024, max compression
```

## Comparing `bagelML-0.0.1.tar` & `bagelML-0.0.11.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2024-04-01 23:56:02.000883 bagelML-0.0.1/
--rw-r--r--   0 bidhan     (501) staff       (20)     6712 2024-04-01 23:56:02.000403 bagelML-0.0.1/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)     5638 2024-04-01 23:36:02.000000 bagelML-0.0.1/README.md
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2024-04-01 23:56:01.990350 bagelML-0.0.1/bagel/
--rw-r--r--   0 bidhan     (501) staff       (20)      625 2024-04-01 20:06:46.000000 bagelML-0.0.1/bagel/__init__.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2024-04-01 23:56:01.994239 bagelML-0.0.1/bagel/api/
--rw-r--r--   0 bidhan     (501) staff       (20)    15137 2024-04-01 23:36:02.000000 bagelML-0.0.1/bagel/api/Cluster.py
--rw-r--r--   0 bidhan     (501) staff       (20)    12895 2024-04-01 23:36:02.000000 bagelML-0.0.1/bagel/api/__init__.py
--rw-r--r--   0 bidhan     (501) staff       (20)    19309 2024-04-01 23:36:02.000000 bagelML-0.0.1/bagel/api/fastapi.py
--rw-r--r--   0 bidhan     (501) staff       (20)    11570 2024-04-01 20:06:46.000000 bagelML-0.0.1/bagel/api/types.py
--rw-r--r--   0 bidhan     (501) staff       (20)     5965 2024-04-01 20:06:46.000000 bagelML-0.0.1/bagel/config.py
--rw-r--r--   0 bidhan     (501) staff       (20)      683 2024-04-01 20:06:46.000000 bagelML-0.0.1/bagel/errors.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2024-04-01 23:56:01.994653 bagelML-0.0.1/bagel/utils/
--rw-r--r--   0 bidhan     (501) staff       (20)        0 2024-04-01 20:06:46.000000 bagelML-0.0.1/bagel/utils/__init__.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2024-04-01 23:56:01.999744 bagelML-0.0.1/bagelML.egg-info/
--rw-r--r--   0 bidhan     (501) staff       (20)     6712 2024-04-01 23:56:01.000000 bagelML-0.0.1/bagelML.egg-info/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)      383 2024-04-01 23:56:01.000000 bagelML-0.0.1/bagelML.egg-info/SOURCES.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        1 2024-04-01 23:56:01.000000 bagelML-0.0.1/bagelML.egg-info/dependency_links.txt
--rw-r--r--   0 bidhan     (501) staff       (20)      267 2024-04-01 23:56:01.000000 bagelML-0.0.1/bagelML.egg-info/requires.txt
--rw-r--r--   0 bidhan     (501) staff       (20)       11 2024-04-01 23:56:01.000000 bagelML-0.0.1/bagelML.egg-info/top_level.txt
--rw-r--r--   0 bidhan     (501) staff       (20)       38 2024-04-01 23:56:02.000932 bagelML-0.0.1/setup.cfg
--rw-r--r--   0 bidhan     (501) staff       (20)     1216 2024-04-01 23:55:58.000000 bagelML-0.0.1/setup.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2024-04-01 23:56:01.999143 bagelML-0.0.1/test/
--rw-r--r--   0 bidhan     (501) staff       (20)        0 2024-04-01 20:06:46.000000 bagelML-0.0.1/test/__init__.py
--rw-r--r--   0 bidhan     (501) staff       (20)     2717 2024-04-01 23:36:02.000000 bagelML-0.0.1/test/client_test.py
--rw-r--r--   0 bidhan     (501) staff       (20)     2332 2024-04-01 20:06:46.000000 bagelML-0.0.1/test/opt_test.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2024-04-02 01:19:00.530842 bagelML-0.0.11/
+-rw-r--r--   0 bidhan     (501) staff       (20)     6713 2024-04-02 01:19:00.530388 bagelML-0.0.11/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)     5638 2024-04-01 23:36:02.000000 bagelML-0.0.11/README.md
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2024-04-02 01:19:00.512940 bagelML-0.0.11/bagel/
+-rw-r--r--   0 bidhan     (501) staff       (20)      376 2024-04-02 01:18:41.000000 bagelML-0.0.11/bagel/__init__.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2024-04-02 01:19:00.517767 bagelML-0.0.11/bagel/api/
+-rw-r--r--   0 bidhan     (501) staff       (20)    15205 2024-04-02 01:18:41.000000 bagelML-0.0.11/bagel/api/Cluster.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    12895 2024-04-01 23:36:02.000000 bagelML-0.0.11/bagel/api/__init__.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    19309 2024-04-02 01:00:08.000000 bagelML-0.0.11/bagel/api/fastapi.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    11570 2024-04-01 20:06:46.000000 bagelML-0.0.11/bagel/api/types.py
+-rw-r--r--   0 bidhan     (501) staff       (20)     5965 2024-04-01 20:06:46.000000 bagelML-0.0.11/bagel/config.py
+-rw-r--r--   0 bidhan     (501) staff       (20)      683 2024-04-01 20:06:46.000000 bagelML-0.0.11/bagel/errors.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2024-04-02 01:19:00.518717 bagelML-0.0.11/bagel/utils/
+-rw-r--r--   0 bidhan     (501) staff       (20)        0 2024-04-01 20:06:46.000000 bagelML-0.0.11/bagel/utils/__init__.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2024-04-02 01:19:00.529718 bagelML-0.0.11/bagelML.egg-info/
+-rw-r--r--   0 bidhan     (501) staff       (20)     6713 2024-04-02 01:19:00.000000 bagelML-0.0.11/bagelML.egg-info/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)      383 2024-04-02 01:19:00.000000 bagelML-0.0.11/bagelML.egg-info/SOURCES.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        1 2024-04-02 01:19:00.000000 bagelML-0.0.11/bagelML.egg-info/dependency_links.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)      267 2024-04-02 01:19:00.000000 bagelML-0.0.11/bagelML.egg-info/requires.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)       11 2024-04-02 01:19:00.000000 bagelML-0.0.11/bagelML.egg-info/top_level.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)       38 2024-04-02 01:19:00.530901 bagelML-0.0.11/setup.cfg
+-rw-r--r--   0 bidhan     (501) staff       (20)     1217 2024-04-02 01:18:50.000000 bagelML-0.0.11/setup.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2024-04-02 01:19:00.528559 bagelML-0.0.11/test/
+-rw-r--r--   0 bidhan     (501) staff       (20)        0 2024-04-01 20:06:46.000000 bagelML-0.0.11/test/__init__.py
+-rw-r--r--   0 bidhan     (501) staff       (20)     2717 2024-04-01 23:36:02.000000 bagelML-0.0.11/test/client_test.py
+-rw-r--r--   0 bidhan     (501) staff       (20)     2332 2024-04-01 20:06:46.000000 bagelML-0.0.11/test/opt_test.py
```

### Comparing `bagelML-0.0.1/PKG-INFO` & `bagelML-0.0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagelML
-Version: 0.0.1
+Version: 0.0.11
 Summary: BagelML is a Python library for interacting with the Bagel inference and vector embedding API.
 Home-page: https://github.com/BagelNetwork/Client
 Author: Bidhan Roy
 Author-email: bidhan@bagel.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bagelML-0.0.1/README.md` & `bagelML-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.1/bagel/api/Cluster.py` & `bagelML-0.0.11/bagel/api/Cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import TYPE_CHECKING, Optional, Tuple, cast, List, Any
 from pydantic import BaseModel, PrivateAttr
 from uuid import UUID
+import time
 
 from bagel.api.types import (
     ClusterMetadata,
     Embedding,
     Include,
     Metadata,
     Document,
@@ -130,14 +131,17 @@
             ids, embeddings, metadatas, documents
         )
 
         self._client._add(
             ids, self.id, embeddings, metadatas, documents, increment_index
         )
 
+        # Syncing time after add
+        time.sleep(1)
+
     def get(
         self,
         ids: Optional[OneOrMany[ID]] = None,
         where: Optional[Where] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         where_document: Optional[WhereDocument] = None,
```

### Comparing `bagelML-0.0.1/bagel/api/__init__.py` & `bagelML-0.0.11/bagel/api/__init__.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.1/bagel/api/fastapi.py` & `bagelML-0.0.11/bagel/api/fastapi.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.1/bagel/api/types.py` & `bagelML-0.0.11/bagel/api/types.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.1/bagel/config.py` & `bagelML-0.0.11/bagel/config.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.1/bagel/errors.py` & `bagelML-0.0.11/bagel/errors.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.1/bagelML.egg-info/PKG-INFO` & `bagelML-0.0.11/bagelML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagelML
-Version: 0.0.1
+Version: 0.0.11
 Summary: BagelML is a Python library for interacting with the Bagel inference and vector embedding API.
 Home-page: https://github.com/BagelNetwork/Client
 Author: Bidhan Roy
 Author-email: bidhan@bagel.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bagelML-0.0.1/setup.py` & `bagelML-0.0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bagelML",
-    version="0.0.1",
+    version="0.0.11",
     description="BagelML is a Python library for interacting with the Bagel inference and vector embedding API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bidhan Roy",
     author_email="bidhan@bagel.net",
     url="https://github.com/BagelNetwork/Client",
     packages=find_packages(),
```

### Comparing `bagelML-0.0.1/test/client_test.py` & `bagelML-0.0.11/test/client_test.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.1/test/opt_test.py` & `bagelML-0.0.11/test/opt_test.py`

 * *Files identical despite different names*

