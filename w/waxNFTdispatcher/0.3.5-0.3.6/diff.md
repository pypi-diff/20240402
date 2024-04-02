# Comparing `tmp/waxnftdispatcher-0.3.5.tar.gz` & `tmp/waxnftdispatcher-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waxnftdispatcher-0.3.5.tar", max compression
+gzip compressed data, was "waxnftdispatcher-0.3.6.tar", max compression
```

## Comparing `waxnftdispatcher-0.3.5.tar` & `waxnftdispatcher-0.3.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-05-02 20:37:23.918020 waxnftdispatcher-0.3.5/LICENSE
--rw-r--r--   0        0        0     2135 2023-08-04 09:34:02.462553 waxnftdispatcher-0.3.5/README.md
--rw-r--r--   0        0        0      588 2023-08-17 07:23:55.967901 waxnftdispatcher-0.3.5/pyproject.toml
--rw-r--r--   0        0        0       41 2023-05-02 20:37:23.918020 waxnftdispatcher-0.3.5/waxnftdispatcher/__init__.py
--rw-r--r--   0        0        0    19681 2023-08-04 09:32:03.562748 waxnftdispatcher-0.3.5/waxnftdispatcher/waxNFTdispatcher.py
--rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 waxnftdispatcher-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-02 11:12:34.520030 waxnftdispatcher-0.3.6/LICENSE
+-rw-r--r--   0        0        0     2135 2024-04-02 11:12:34.520030 waxnftdispatcher-0.3.6/README.md
+-rw-r--r--   0        0        0      601 2024-04-02 11:22:37.548011 waxnftdispatcher-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-02 11:12:34.522030 waxnftdispatcher-0.3.6/waxnftdispatcher/__init__.py
+-rw-r--r--   0        0        0    19895 2024-04-02 11:12:34.522030 waxnftdispatcher-0.3.6/waxnftdispatcher/waxNFTdispatcher.py
+-rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 waxnftdispatcher-0.3.6/PKG-INFO
```

### Comparing `waxnftdispatcher-0.3.5/LICENSE` & `waxnftdispatcher-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `waxnftdispatcher-0.3.5/README.md` & `waxnftdispatcher-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `waxnftdispatcher-0.3.5/pyproject.toml` & `waxnftdispatcher-0.3.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "waxNFTdispatcher"
-version = "0.3.5"
+version = "0.3.6"
 description = "This library will help you to transfer or to mint NFTs on the WAX blockchain"
-authors = ["Amparo Dios <amparo.dios@gmail.com>"]
+authors = ["Amparo Dios <amparo.dios@gmail.com>", "funkaclau"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/alparo/waxNFTdispatcher"
 repository = "https://github.com/alparo/waxNFTdispatcher"
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4.0"
```

### Comparing `waxnftdispatcher-0.3.5/waxnftdispatcher/waxNFTdispatcher.py` & `waxnftdispatcher-0.3.6/waxnftdispatcher/waxNFTdispatcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -286,21 +286,26 @@
             transaction_id = resp["transaction_id"]
         except KeyError:
             error_message = resp["error"]["details"][0]["message"]
             logger.error(error_message)
             return "None", False
 
         asset_id = "None"
-        if resp["processed"]["action_traces"][0]["act"]["name"] == "transfer":
-            asset_id = tuple(
-                resp["processed"]["action_traces"][0]["inline_traces"][2]["act"][
-                    "data"
-                ]["asset_ids"]
-            )
-
+        try:
+            if resp["processed"]["action_traces"][0]["act"]["name"] == "transfer":
+                asset_id = tuple(
+                    resp["processed"]["action_traces"][0]["inline_traces"][2]["act"][
+                        "data"
+                    ]["asset_ids"]
+                )
+        except KeyError:
+            error_message = resp["error"]["details"][0]["message"]
+            logger.error(error_message)
+            return "None", False
+            
         return asset_id, transaction_id
 
     def send_or_mint_assets(
         self,
         schema_template_list: Iterable[Tuple[str, str]],
         wallet: str,
         memo: str = "",
```

### Comparing `waxnftdispatcher-0.3.5/PKG-INFO` & `waxnftdispatcher-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
-Name: waxnftdispatcher
-Version: 0.3.5
+Name: waxNFTdispatcher
+Version: 0.3.6
 Summary: This library will help you to transfer or to mint NFTs on the WAX blockchain
 Home-page: https://github.com/alparo/waxNFTdispatcher
 License: MIT
 Author: Amparo Dios
 Author-email: amparo.dios@gmail.com
 Requires-Python: >=3.8.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: pyntelope (>=0.8.0,<0.9.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/alparo/waxNFTdispatcher
 Description-Content-Type: text/markdown
 
 # waxNFTdispatcher
```

