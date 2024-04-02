# Comparing `tmp/keepa-1.3.8.tar.gz` & `tmp/keepa-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keepa-1.3.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "keepa-1.3.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `keepa-1.3.8.tar` & `keepa-1.3.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     9565 2023-11-02 16:26:25.453393 keepa-1.3.8/README.rst
--rw-r--r--   0        0        0     1820 2023-11-02 16:26:25.453393 keepa-1.3.8/pyproject.toml
--rw-r--r--   0        0        0      365 2023-11-02 16:26:25.453393 keepa-1.3.8/src/keepa/__init__.py
--rw-r--r--   0        0        0   124932 2023-11-02 16:26:25.453393 keepa-1.3.8/src/keepa/interface.py
--rw-r--r--   0        0        0     3842 2023-11-02 16:26:25.453393 keepa-1.3.8/src/keepa/plotting.py
--rw-r--r--   0        0        0    38339 2023-11-02 16:26:25.453393 keepa-1.3.8/src/keepa/query_keys.py
--rw-r--r--   0        0        0    10926 1970-01-01 00:00:00.000000 keepa-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     9540 2024-04-02 15:21:13.237738 keepa-1.3.9/README.rst
+-rw-r--r--   0        0        0     1545 2024-04-02 15:21:13.237738 keepa-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0      365 2024-04-02 15:21:13.237738 keepa-1.3.9/src/keepa/__init__.py
+-rw-r--r--   0        0        0   125561 2024-04-02 15:21:13.241737 keepa-1.3.9/src/keepa/interface.py
+-rw-r--r--   0        0        0     3843 2024-04-02 15:21:13.241737 keepa-1.3.9/src/keepa/plotting.py
+-rw-r--r--   0        0        0    38339 2024-04-02 15:21:13.241737 keepa-1.3.9/src/keepa/query_keys.py
+-rw-r--r--   0        0        0    10824 1970-01-01 00:00:00.000000 keepa-1.3.9/PKG-INFO
```

### Comparing `keepa-1.3.8/README.rst` & `keepa-1.3.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -290,15 +290,14 @@
 
   pytest
 
 Unit testing will automatically enforce minimum code coverage standards.
 
 Next, to ensure your code meets minimum code styling standards, run::
 
-  pip install pre-commit
   pre-commit run --all-files
 
 Finally, `create a pull request`_ from your fork and I'll be sure to review it.
 
 
 Credits
 -------
```

### Comparing `keepa-1.3.8/pyproject.toml` & `keepa-1.3.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -22,17 +22,16 @@
     "Programming Language :: Python :: 3.12",
 ]
 keywords = ["keepa"]
 dependencies = [
     "numpy >=1.9.3",
     "requests >=2.2",
     "tqdm",
-    "aiohttp; python_version!='3.12.*'",
-    "aiohttp==3.9.0b0; python_version=='3.12.*'",  # until aiohttp gets upgraded
-    "pandas",
+    "aiohttp",
+    "pandas <= 3.0",
 ]
 
 [project.urls]
 Documentation = "https://keepaapi.readthedocs.io/en/latest/"
 Source = "https://github.com/akaszynski/keepa"
 
 [project.optional-dependencies]
@@ -57,14 +56,9 @@
 # Sort by name, don't cluster "from" vs "import"
 force_sort_within_sections = true
 # Combines "as" imports on the same line
 combine_as_imports = true
 
 [tool.ruff]
 line-length = 100
-
-[tool.ruff.lint]
-# Enable Pyflakes (`F`) and a subset of the pycodestyle (`E`)  codes by default.
-# Unlike Flake8, Ruff doesn't enable pycodestyle warnings (`W`) or
-# McCabe complexity (`C901`) by default.
-select = ["E4", "E7", "E9", "F"]
+select = ["E", "F", "W", "I001"]  # pyflakes, pycodestyle, isort
 ignore = []
```

### Comparing `keepa-1.3.8/src/keepa/interface.py` & `keepa-1.3.9/src/keepa/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Interface module to download Amazon product and history data from keepa.com."""
+
 import asyncio
 import datetime
 import json
 import logging
 import time
 from typing import List
 
@@ -39,16 +40,16 @@
     "402": "PAYMENT_REQUIRED",
     "405": "METHOD_NOT_ALLOWED",
     "429": "NOT_ENOUGH_TOKEN",
 }
 
 # domain codes
 # Valid values: [ 1: com | 2: co.uk | 3: de | 4: fr | 5:
-#                 co.jp | 6: ca | 7: cn | 8: it | 9: es | 10: in | 11: com.mx ]
-DCODES = ["RESERVED", "US", "GB", "DE", "FR", "JP", "CA", "CN", "IT", "ES", "IN", "MX"]
+#                 co.jp | 6: ca | 7: cn | 8: it | 9: es | 10: in | 11: com.mx | 12: com.br ]
+DCODES = ["RESERVED", "US", "GB", "DE", "FR", "JP", "CA", "CN", "IT", "ES", "IN", "MX", "BR"]
 
 # csv indices. used when parsing csv and stats fields.
 # https://github.com/keepacom/api_backend
 # see api_backend/src/main/java/com/keepa/api/backend/structs/Product.java
 # [index in csv, key name, isfloat(is price or rating)]
 csv_indices = [
     [0, "AMAZON", True],
@@ -501,17 +502,17 @@
             Last x days (positive integer value): calculates the stats
             of the last x days, where x is the value of the stats
             parameter.  Interval: You can provide a date range for the
             stats calculation. You can specify the range via two
             timestamps (unix epoch time milliseconds) or two date
             strings (ISO8601, with or without time in UTC).
 
-        domain : str, optional
+        domain : str, default: "US"
             One of the following Amazon domains: RESERVED, US, GB, DE,
-            FR, JP, CA, CN, IT, ES, IN, MX Defaults to US.
+            FR, JP, CA, CN, IT, ES, IN, MX, BR.
 
         offers : int, optional
             Adds available offers to product data. Default 0.  Must be between
             20 and 100. Enabling this also enables the ``"buyBoxUsedHistory"``.
 
         update : int, optional
             if data is older than the input integer, keepa will
@@ -881,15 +882,15 @@
             Interpret product codes as ASINs only.
 
         stats : int or date format
             Set the stats time for get sales rank inside this range
 
         domain : str
             One of the following Amazon domains:
-            RESERVED, US, GB, DE, FR, JP, CA, CN, IT, ES, IN, MX
+            RESERVED, US, GB, DE, FR, JP, CA, CN, IT, ES, IN, MX, BR.
 
         offers : bool, optional
             Adds product offers to product data.
 
         update : int, optional
             If data is older than the input integer, keepa will update
             their database and return live data.  If set to 0 (live
@@ -1017,18 +1018,17 @@
         Parameters
         ----------
         category : str
             The category node id of the category you want to request
             the best sellers list for. You can find category node ids
             via the category search "search_for_categories".
 
-        domain : str
-            Amazon locale you want to access. Must be one of the following
-            RESERVED, US, GB, DE, FR, JP, CA, CN, IT, ES, IN, MX
-            Default US.
+        domain : str, default: "US"
+            Amazon locale you want to access. Must be one of the following:
+            RESERVED, US, GB, DE, FR, JP, CA, CN, IT, ES, IN, MX, BR.
 
         wait : bool, optional
             Wait available token before doing effective query.
             Defaults to ``True``.
 
         Returns
         -------
@@ -1073,15 +1073,18 @@
          'B09SP8JPPK',
          '0999296345',
          'B07HPG684T',
          '1984825577',
         ...
 
         """
-        assert domain in DCODES, "Invalid domain code"
+        if domain not in DCODES:
+            raise ValueError(
+                f"Invalid domain code {domain}. Should be one of the following:\n{DCODES}"
+            )
 
         payload = {
             "key": self.accesskey,
             "domain": DCODES.index(domain),
             "category": category,
             "range": rank_avg_range,
         }
@@ -1096,18 +1099,17 @@
         """Search for categories from Amazon.
 
         Parameters
         ----------
         searchterm : str
             Input search term.
 
-        domain : str, default: 'US'
-            Amazon locale you want to access. Must be one of the following
-            RESERVED, US, GB, DE, FR, JP, CA, CN, IT, ES, IN, MX
-            Default US.
+        domain : str, default: "US"
+            Amazon locale you want to access. Must be one of the following:
+            RESERVED, US, GB, DE, FR, JP, CA, CN, IT, ES, IN, MX, BR.
 
         wait : bool, default: True
             Wait available token before doing effective query.
             Defaults to ``True``.
 
         Returns
         -------
@@ -1132,15 +1134,18 @@
         12805 Science & Religion
         13445 Astrophysics & Space Science
         12038 Science Fiction & Fantasy
         3207 Science, Nature & How It Works
         144 Science Fiction & Fantasy
 
         """
-        assert domain in DCODES, "Invalid domain code"
+        if domain not in DCODES:
+            raise ValueError(
+                f"Invalid domain code {domain}. Should be one of the following:\n{DCODES}"
+            )
 
         payload = {
             "key": self.accesskey,
             "domain": DCODES.index(domain),
             "type": "category",
             "term": searchterm,
         }
@@ -1158,17 +1163,16 @@
         Parameters
         ----------
         category_id : int
             ID for specific category or 0 to return a list of root
             categories.
 
         domain : str, default: "US"
-            Amazon locale you want to access. Must be one of the following
-            RESERVED, US, GB, DE, FR, JP, CA, CN, IT, ES, IN, MX
-            Default US
+            Amazon locale you want to access. Must be one of the following:
+            RESERVED, US, GB, DE, FR, JP, CA, CN, IT, ES, IN, MX, BR.
 
         include_parents : bool, default: False
             Include parents.
 
         wait : bool, default: True
             Wait available token before doing effective query.
 
@@ -1207,15 +1211,17 @@
          'productCount': 6417325,
          'contextFreeName': 'Kindle Store',
          'lowestRank': 1,
          'matched': True}
 
         """
         if domain not in DCODES:
-            raise ValueError("Invalid domain code")
+            raise ValueError(
+                f"Invalid domain code {domain}. Should be one of the following:\n{DCODES}"
+            )
 
         payload = {
             "key": self.accesskey,
             "domain": DCODES.index(domain),
             "category": category_id,
             "parents": int(include_parents),
         }
@@ -2880,15 +2886,18 @@
                     product["stats_parsed"] = _parse_stats(stats, to_datetime)
 
         return response
 
     @is_documented_by(Keepa.best_sellers_query)
     async def best_sellers_query(self, category, rank_avg_range=0, domain="US", wait=True):
         """Documented by Keepa.best_sellers_query."""
-        assert domain in DCODES, "Invalid domain code"
+        if domain not in DCODES:
+            raise ValueError(
+                f"Invalid domain code {domain}. Should be one of the following:\n{DCODES}"
+            )
 
         payload = {
             "key": self.accesskey,
             "domain": DCODES.index(domain),
             "category": category,
             "range": rank_avg_range,
         }
@@ -2898,15 +2907,18 @@
             return response["bestSellersList"]["asinList"]
         else:  # pragma: no cover
             log.info("Best sellers search results not yet available")
 
     @is_documented_by(Keepa.search_for_categories)
     async def search_for_categories(self, searchterm, domain="US", wait=True):
         """Documented by Keepa.search_for_categories."""
-        assert domain in DCODES, "Invalid domain code"
+        if domain not in DCODES:
+            raise ValueError(
+                f"Invalid domain code {domain}. Should be one of the following:\n{DCODES}"
+            )
 
         payload = {
             "key": self.accesskey,
             "domain": DCODES.index(domain),
             "type": "category",
             "term": searchterm,
         }
@@ -2918,15 +2930,18 @@
             )
         else:
             return response["categories"]
 
     @is_documented_by(Keepa.category_lookup)
     async def category_lookup(self, category_id, domain="US", include_parents=0, wait=True):
         """Documented by Keepa.category_lookup."""
-        assert domain in DCODES, "Invalid domain code"
+        if domain not in DCODES:
+            raise ValueError(
+                f"Invalid domain code {domain}. Should be one of the following:\n{DCODES}"
+            )
 
         payload = {
             "key": self.accesskey,
             "domain": DCODES.index(domain),
             "category": category_id,
             "parents": include_parents,
         }
```

### Comparing `keepa-1.3.8/src/keepa/plotting.py` & `keepa-1.3.9/src/keepa/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Plotting module product data returned from keepa interface module."""
+
 import numpy as np
 
 from keepa.interface import keepa_minutes_to_time, parse_csv
 
 
 def plot_product(
     product, keys=["AMAZON", "USED", "COUNT_USED", "SALES"], price_limit=1000, show=True
```

### Comparing `keepa-1.3.8/src/keepa/query_keys.py` & `keepa-1.3.9/src/keepa/query_keys.py`

 * *Files identical despite different names*

### Comparing `keepa-1.3.8/PKG-INFO` & `keepa-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepa
-Version: 1.3.8
+Version: 1.3.9
 Summary: Interfaces with keepa.com's API.
 Keywords: keepa
 Author-email: Alex Kaszynski <akascap@gmail.com>
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Database :: Front-Ends
@@ -13,17 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy >=1.9.3
 Requires-Dist: requests >=2.2
 Requires-Dist: tqdm
-Requires-Dist: aiohttp; python_version!='3.12.*'
-Requires-Dist: aiohttp==3.9.0b0; python_version=='3.12.*'
-Requires-Dist: pandas
+Requires-Dist: aiohttp
+Requires-Dist: pandas <= 3.0
 Requires-Dist: sphinx==6.1.2 ; extra == "doc"
 Requires-Dist: pydata-sphinx-theme==0.14.2 ; extra == "doc"
 Requires-Dist: matplotlib ; extra == "test"
 Requires-Dist: pandas ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
@@ -324,15 +323,14 @@
 
   pytest
 
 Unit testing will automatically enforce minimum code coverage standards.
 
 Next, to ensure your code meets minimum code styling standards, run::
 
-  pip install pre-commit
   pre-commit run --all-files
 
 Finally, `create a pull request`_ from your fork and I'll be sure to review it.
 
 
 Credits
 -------
```

