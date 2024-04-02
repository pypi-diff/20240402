# Comparing `tmp/rank_torrent_name-0.2.8.tar.gz` & `tmp/rank_torrent_name-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rank_torrent_name-0.2.8.tar", max compression
+gzip compressed data, was "rank_torrent_name-0.2.9.tar", max compression
```

## Comparing `rank_torrent_name-0.2.8.tar` & `rank_torrent_name-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2024-04-01 01:30:30.454425 rank_torrent_name-0.2.8/LICENSE
--rw-r--r--   0        0        0    23595 2024-04-01 01:30:30.454425 rank_torrent_name-0.2.8/README.md
--rw-r--r--   0        0        0     3055 2024-04-01 01:30:30.454425 rank_torrent_name-0.2.8/RTN/__init__.py
--rw-r--r--   0        0        0      326 2024-04-01 01:30:30.454425 rank_torrent_name-0.2.8/RTN/exceptions.py
--rw-r--r--   0        0        0     7529 2024-04-01 01:30:30.454425 rank_torrent_name-0.2.8/RTN/fetch.py
--rw-r--r--   0        0        0    11949 2024-04-01 01:30:30.454425 rank_torrent_name-0.2.8/RTN/models.py
--rw-r--r--   0        0        0    19878 2024-04-01 01:30:30.458425 rank_torrent_name-0.2.8/RTN/parser.py
--rw-r--r--   0        0        0     9387 2024-04-01 01:30:30.458425 rank_torrent_name-0.2.8/RTN/patterns.py
--rw-r--r--   0        0        0    10231 2024-04-01 01:30:30.458425 rank_torrent_name-0.2.8/RTN/ranker.py
--rw-r--r--   0        0        0     2165 2024-04-01 01:30:30.458425 rank_torrent_name-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    23875 1970-01-01 00:00:00.000000 rank_torrent_name-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-01 02:32:11.432484 rank_torrent_name-0.2.9/LICENSE
+-rw-r--r--   0        0        0    23595 2024-04-01 02:32:11.432484 rank_torrent_name-0.2.9/README.md
+-rw-r--r--   0        0        0     3055 2024-04-01 02:32:11.432484 rank_torrent_name-0.2.9/RTN/__init__.py
+-rw-r--r--   0        0        0      326 2024-04-01 02:32:11.432484 rank_torrent_name-0.2.9/RTN/exceptions.py
+-rw-r--r--   0        0        0     7529 2024-04-01 02:32:11.432484 rank_torrent_name-0.2.9/RTN/fetch.py
+-rw-r--r--   0        0        0    11949 2024-04-01 02:32:11.432484 rank_torrent_name-0.2.9/RTN/models.py
+-rw-r--r--   0        0        0    19878 2024-04-01 02:32:11.432484 rank_torrent_name-0.2.9/RTN/parser.py
+-rw-r--r--   0        0        0     9387 2024-04-01 02:32:11.436484 rank_torrent_name-0.2.9/RTN/patterns.py
+-rw-r--r--   0        0        0    10258 2024-04-01 02:32:11.436484 rank_torrent_name-0.2.9/RTN/ranker.py
+-rw-r--r--   0        0        0     2165 2024-04-01 02:32:11.436484 rank_torrent_name-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    23875 1970-01-01 00:00:00.000000 rank_torrent_name-0.2.9/PKG-INFO
```

### Comparing `rank_torrent_name-0.2.8/LICENSE` & `rank_torrent_name-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rank_torrent_name-0.2.8/README.md` & `rank_torrent_name-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `rank_torrent_name-0.2.8/RTN/__init__.py` & `rank_torrent_name-0.2.9/RTN/__init__.py`

 * *Files identical despite different names*

### Comparing `rank_torrent_name-0.2.8/RTN/fetch.py` & `rank_torrent_name-0.2.9/RTN/fetch.py`

 * *Files identical despite different names*

### Comparing `rank_torrent_name-0.2.8/RTN/models.py` & `rank_torrent_name-0.2.9/RTN/models.py`

 * *Files identical despite different names*

### Comparing `rank_torrent_name-0.2.8/RTN/parser.py` & `rank_torrent_name-0.2.9/RTN/parser.py`

 * *Files identical despite different names*

### Comparing `rank_torrent_name-0.2.8/RTN/patterns.py` & `rank_torrent_name-0.2.9/RTN/patterns.py`

 * *Files identical despite different names*

### Comparing `rank_torrent_name-0.2.8/RTN/ranker.py` & `rank_torrent_name-0.2.9/RTN/ranker.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,12 +203,12 @@
             total_rank += (
                 settings.custom_ranks["dolby_video"].rank
                 if settings.custom_ranks["dolby_video"].enable
                 else rank_model.dolby_video
             )
     if data.is_complete:
         total_rank += 100
-    if len(data.season) > 0:
-        total_rank += 100 * len(data.season)
+    if len(data.season) > 0 and len(data.episode) == 0:
+        total_rank += 125 * len(data.season)
     if len(data.episode) > 0:
         total_rank += 10 * len(data.episode)
     return total_rank
```

### Comparing `rank_torrent_name-0.2.8/pyproject.toml` & `rank_torrent_name-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rank-torrent-name"
-version = "0.2.8"
+version = "0.2.9"
 description = "Parse Torrents using PTN and Rank them according to your preferences!"
 authors = ["Spoked <dreu.lavelle@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dreulavelle/rank-torrent-name"
 
 [tool.poetry.dependencies]
```

### Comparing `rank_torrent_name-0.2.8/PKG-INFO` & `rank_torrent_name-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rank-torrent-name
-Version: 0.2.8
+Version: 0.2.9
 Summary: Parse Torrents using PTN and Rank them according to your preferences!
 Home-page: https://github.com/dreulavelle/rank-torrent-name
 License: MIT
 Author: Spoked
 Author-email: dreu.lavelle@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rank-torrent-name Version: 0.2.8 Summary: Parse
+Metadata-Version: 2.1 Name: rank-torrent-name Version: 0.2.9 Summary: Parse
 Torrents using PTN and Rank them according to your preferences! Home-page:
 https://github.com/dreulavelle/rank-torrent-name License: MIT Author: Spoked
 Author-email: dreu.lavelle@gmail.com Requires-Python: >=3.11,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: levenshtein
 (>=0.25.0,<0.26.0) Requires-Dist: parse-torrent-title (>=2.8.1,<3.0.0)
```

