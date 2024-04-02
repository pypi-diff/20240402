# Comparing `tmp/pyqqq-0.5.9.tar.gz` & `tmp/pyqqq-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.5.9.tar", max compression
+gzip compressed data, was "pyqqq-0.6.0.tar", max compression
```

## Comparing `pyqqq-0.5.9.tar` & `pyqqq-0.6.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.5.9/README.md
--rw-r--r--   0        0        0      727 2024-04-02 08:36:21.035273 pyqqq-0.5.9/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.5.9/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.5.9/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.5.9/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    35704 2024-03-28 00:52:30.410040 pyqqq-0.5.9/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.5.9/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    23893 2024-03-15 08:38:18.946138 pyqqq-0.5.9/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.5.9/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.5.9/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   185553 2024-03-25 09:55:40.950355 pyqqq-0.5.9/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.5.9/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.5.9/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    23713 2024-03-18 01:27:17.145321 pyqqq-0.5.9/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.5.9/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      437 2024-03-25 05:15:17.008929 pyqqq-0.5.9/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.5.9/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.5.9/pyqqq/data/daily.py
--rw-r--r--   0        0        0     4674 2024-03-25 05:39:48.241915 pyqqq-0.5.9/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     3973 2024-04-02 08:35:19.547551 pyqqq-0.5.9/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.5.9/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.878098 pyqqq-0.5.9/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.5.9/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.5.9/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.5.9/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.5.9/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.5.9/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 pyqqq-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-28 03:41:58.980653 pyqqq-0.6.0/README.md
+-rw-r--r--   0        0        0      770 2024-04-02 08:49:14.302007 pyqqq-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-28 03:41:58.982907 pyqqq-0.6.0/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 03:59:43.302843 pyqqq-0.6.0/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 03:59:24.168676 pyqqq-0.6.0/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    35704 2024-03-28 03:41:58.983298 pyqqq-0.6.0/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-28 03:41:58.983583 pyqqq-0.6.0/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    23893 2024-03-22 01:44:28.624631 pyqqq-0.6.0/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 03:41:58.983800 pyqqq-0.6.0/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-03-04 03:59:43.302986 pyqqq-0.6.0/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   185553 2024-03-28 03:41:58.984670 pyqqq-0.6.0/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-28 03:41:58.984873 pyqqq-0.6.0/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-07 02:05:26.670417 pyqqq-0.6.0/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    23713 2024-03-22 01:44:28.626215 pyqqq-0.6.0/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-22 01:44:28.626559 pyqqq-0.6.0/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      437 2024-03-29 07:10:26.944955 pyqqq-0.6.0/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 02:05:26.670533 pyqqq-0.6.0/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     4156 2024-04-02 05:12:48.319458 pyqqq-0.6.0/pyqqq/data/daily.py
+-rw-r--r--   0        0        0     4674 2024-03-28 03:41:58.985266 pyqqq-0.6.0/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     3973 2024-04-02 08:49:01.129722 pyqqq-0.6.0/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     1254 2024-03-22 01:44:28.626857 pyqqq-0.6.0/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-03-07 02:05:26.670737 pyqqq-0.6.0/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:49:01.142004 pyqqq-0.6.0/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-22 01:44:28.626942 pyqqq-0.6.0/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-03-04 03:59:43.304644 pyqqq-0.6.0/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-28 03:41:58.986410 pyqqq-0.6.0/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 02:18:36.457903 pyqqq-0.6.0/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0     1425 2024-03-04 03:59:43.304764 pyqqq-0.6.0/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.6.0/PKG-INFO
```

### Comparing `pyqqq-0.5.9/README.md` & `pyqqq-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyproject.toml` & `pyqqq-0.6.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.5.9"
+version = "0.6.0"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 tinydb = "^4.8.0"
 requests = "^2.31.0"
 python-dotenv = "^1.0.1"
 websockets = "^12.0"
 pandas = "^1.5.3"
+cssutils = "^2.10.2"
+cachetools = "^5.3.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
 sphinx = "^7.2.6"
 myst-parser = "^2.0.0"
 sphinx-rtd-theme = "^2.0.0"
 ipykernel = "^6.29.3"
```

### Comparing `pyqqq-0.5.9/pyqqq/__init__.py` & `pyqqq-0.6.0/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.6.0/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.6.0/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.6.0/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.6.0/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.6.0/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.6.0/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.6.0/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.6.0/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.6.0/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/data/daily.py` & `pyqqq-0.6.0/pyqqq/data/daily.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/data/domestic.py` & `pyqqq-0.6.0/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/data/realtime.py` & `pyqqq-0.6.0/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/datatypes.py` & `pyqqq-0.6.0/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/utils/kvstore.py` & `pyqqq-0.6.0/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/utils/limiter.py` & `pyqqq-0.6.0/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/utils/logger.py` & `pyqqq-0.6.0/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/utils/market_schedule.py` & `pyqqq-0.6.0/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/pyqqq/utils/retry.py` & `pyqqq-0.6.0/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.9/PKG-INFO` & `pyqqq-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.5.9
+Version: 0.6.0
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: cachetools (>=5.3.3,<6.0.0)
+Requires-Dist: cssutils (>=2.10.2,<3.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tinydb (>=4.8.0,<5.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Project-URL: Documentation, https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io
 Description-Content-Type: text/markdown
```

