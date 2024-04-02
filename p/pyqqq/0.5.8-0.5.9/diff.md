# Comparing `tmp/pyqqq-0.5.8.tar.gz` & `tmp/pyqqq-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.5.8.tar", max compression
+gzip compressed data, was "pyqqq-0.5.9.tar", max compression
```

## Comparing `pyqqq-0.5.8.tar` & `pyqqq-0.5.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.5.8/README.md
--rw-r--r--   0        0        0      727 2024-04-01 05:19:44.471043 pyqqq-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.5.8/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.5.8/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.5.8/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    35704 2024-03-28 00:52:30.410040 pyqqq-0.5.8/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.5.8/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    23893 2024-03-15 08:38:18.946138 pyqqq-0.5.8/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.5.8/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.5.8/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   185553 2024-03-25 09:55:40.950355 pyqqq-0.5.8/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.5.8/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.5.8/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    23713 2024-03-18 01:27:17.145321 pyqqq-0.5.8/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.5.8/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      437 2024-03-25 05:15:17.008929 pyqqq-0.5.8/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.5.8/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     4134 2024-04-01 05:18:46.979286 pyqqq-0.5.8/pyqqq/data/daily.py
--rw-r--r--   0        0        0     4674 2024-03-25 05:39:48.241915 pyqqq-0.5.8/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     1371 2024-03-07 01:02:36.878027 pyqqq-0.5.8/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.5.8/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.878098 pyqqq-0.5.8/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.5.8/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.5.8/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.5.8/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.5.8/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.5.8/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 pyqqq-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.5.9/README.md
+-rw-r--r--   0        0        0      727 2024-04-02 08:36:21.035273 pyqqq-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.5.9/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.5.9/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.5.9/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    35704 2024-03-28 00:52:30.410040 pyqqq-0.5.9/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.5.9/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    23893 2024-03-15 08:38:18.946138 pyqqq-0.5.9/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.5.9/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.5.9/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   185553 2024-03-25 09:55:40.950355 pyqqq-0.5.9/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.5.9/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.5.9/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    23713 2024-03-18 01:27:17.145321 pyqqq-0.5.9/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.5.9/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      437 2024-03-25 05:15:17.008929 pyqqq-0.5.9/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.5.9/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.5.9/pyqqq/data/daily.py
+-rw-r--r--   0        0        0     4674 2024-03-25 05:39:48.241915 pyqqq-0.5.9/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     3973 2024-04-02 08:35:19.547551 pyqqq-0.5.9/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.5.9/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.878098 pyqqq-0.5.9/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.5.9/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.5.9/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.5.9/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.5.9/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.5.9/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 pyqqq-0.5.9/PKG-INFO
```

### Comparing `pyqqq-0.5.8/README.md` & `pyqqq-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyproject.toml` & `pyqqq-0.5.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.5.8"
+version = "0.5.9"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.5.8/pyqqq/__init__.py` & `pyqqq-0.5.9/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.5.9/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.5.9/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.5.9/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.5.9/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.5.9/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.5.9/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.5.9/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.5.9/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.5.9/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/data/daily.py` & `pyqqq-0.5.9/pyqqq/data/daily.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         - msvolume (int): 매수체결수량
         - mdchecnt (int): 매도체결건수
         - mschecnt (int): 매수체결건수
         - cpower (float): 체결강도
         - w_avrg (int): 가중평균가
         - offerho (int): 매도호가
         - bidho (int): 매수호가
-        - status (int): 장정보 (0:장중 10:장전시간외 4:장후시간외 3:장마감)
+        - status (int): 장정보 (0:장중 10:장전시간외 4:장후시간외 3:장마감 47:시간외단일가)
         - jnilvolume (int): 전일거래량
         - shcode (str): 종목코드
 
     Examples:
         >>> df = get_tick_data(datetime.date.today() - datetime.timedelta(days=3), "017670")
         >>> print(df.head())
            mdchecnt  sign  mschecnt  mdvolume  w_avrg  cpower  offerho  cvolume  high  bidho  low  price cgubun  value  change  shcode   chetime opentime lowtime  volume  drate hightime  jnilvolume  msvolume  open  status
```

### Comparing `pyqqq-0.5.8/pyqqq/data/domestic.py` & `pyqqq-0.5.9/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/datatypes.py` & `pyqqq-0.5.9/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/utils/kvstore.py` & `pyqqq-0.5.9/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/utils/limiter.py` & `pyqqq-0.5.9/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/utils/logger.py` & `pyqqq-0.5.9/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/utils/market_schedule.py` & `pyqqq-0.5.9/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/pyqqq/utils/retry.py` & `pyqqq-0.5.9/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.5.8/PKG-INFO` & `pyqqq-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.5.8
+Version: 0.5.9
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

