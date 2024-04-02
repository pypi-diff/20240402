# Comparing `tmp/stock-open-api-0.0.8.tar.gz` & `tmp/stock-open-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stock-open-api-0.0.8.tar", last modified: Mon Jul 24 06:54:37 2023, max compression
+gzip compressed data, was "dist/stock-open-api-0.0.9.tar", last modified: Tue Jul 25 05:50:27 2023, max compression
```

## Comparing `stock-open-api-0.0.8.tar` & `stock-open-api-0.0.9.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/
--rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/api/bse/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/bse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/company.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/company_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/hk_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/hk_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/kcb_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/kcb_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/neeq_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/neeq_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/sh_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/sz_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/us_chinese_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/us_chinese_stock_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/api/sse/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/sse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/sse/sh_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/sse/sh_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/items/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/items/list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/utils/iterator_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/utils/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/utils/request_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/utils/time_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/utils/ua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/stock_open_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/stock_open_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/stock_open_api/api/bse/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/bse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/company.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/company_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/hk_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/hk_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/kcb_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/kcb_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/neeq_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/neeq_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/sh_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/sz_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/us_chinese_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/eastmoney/us_chinese_stock_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/stock_open_api/api/jqka/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/jqka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/jqka/company.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/stock_open_api/api/sse/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/sse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/sse/sh_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/api/sse/sh_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/stock_open_api/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/items/list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/stock_open_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/utils/iterator_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/utils/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/utils/request_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/utils/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/utils/ua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 05:50:14.000000 stock-open-api-0.0.9/stock_open_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/stock_open_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-25 05:50:26.000000 stock-open-api-0.0.9/stock_open_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-25 05:50:27.000000 stock-open-api-0.0.9/stock_open_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:50:26.000000 stock-open-api-0.0.9/stock_open_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 05:50:26.000000 stock-open-api-0.0.9/stock_open_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 05:50:26.000000 stock-open-api-0.0.9/stock_open_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:50:26.000000 stock-open-api-0.0.9/stock_open_api.egg-info/zip-safe
```

### Comparing `stock-open-api-0.0.8/PKG-INFO` & `stock-open-api-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
         
@@ -124,14 +124,15 @@
             - github: [https://github.com/akfamily/akshare](https://github.com/akfamily/akshare)
             - doc: [https://akshare.akfamily.xyz/](https://akshare.akfamily.xyz/)
         
         - Tushare 免费提供各类数据 , 助力行业和量化研究。 
             - github: [https://github.com/waditu/tushare](https://github.com/waditu/tushare)
             - doc: [http://tushare.org/index.html](http://tushare.org/index.html)
             - pro doc: [https://tushare.pro/](https://tushare.pro/)
+        
 Keywords: stock,api
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `stock-open-api-0.0.8/README.md` & `stock-open-api-0.0.9/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -115,8 +115,8 @@
 - AKShare 开源财经数据接口库 
     - github: [https://github.com/akfamily/akshare](https://github.com/akfamily/akshare)
     - doc: [https://akshare.akfamily.xyz/](https://akshare.akfamily.xyz/)
 
 - Tushare 免费提供各类数据 , 助力行业和量化研究。 
     - github: [https://github.com/waditu/tushare](https://github.com/waditu/tushare)
     - doc: [http://tushare.org/index.html](http://tushare.org/index.html)
-    - pro doc: [https://tushare.pro/](https://tushare.pro/)
+    - pro doc: [https://tushare.pro/](https://tushare.pro/)
```

### Comparing `stock-open-api-0.0.8/setup.py` & `stock-open-api-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/eastmoney/company.py` & `stock-open-api-0.0.9/stock_open_api/api/eastmoney/company.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/eastmoney/company_config.py` & `stock-open-api-0.0.9/stock_open_api/api/eastmoney/company_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/eastmoney/hk_stock.py` & `stock-open-api-0.0.9/stock_open_api/api/eastmoney/hk_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/eastmoney/hk_stock_config.py` & `stock-open-api-0.0.9/stock_open_api/api/eastmoney/hk_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/eastmoney/kcb_stock.py` & `stock-open-api-0.0.9/stock_open_api/api/eastmoney/kcb_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/eastmoney/kcb_stock_config.py` & `stock-open-api-0.0.9/stock_open_api/api/eastmoney/kcb_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/eastmoney/neeq_stock.py` & `stock-open-api-0.0.9/stock_open_api/api/eastmoney/neeq_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/eastmoney/neeq_stock_config.py` & `stock-open-api-0.0.9/stock_open_api/api/eastmoney/neeq_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/eastmoney/sh_stock.py` & `stock-open-api-0.0.9/stock_open_api/api/eastmoney/sh_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/eastmoney/sz_stock.py` & `stock-open-api-0.0.9/stock_open_api/api/eastmoney/sz_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/eastmoney/us_chinese_stock.py` & `stock-open-api-0.0.9/stock_open_api/api/eastmoney/us_chinese_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/eastmoney/us_chinese_stock_config.py` & `stock-open-api-0.0.9/stock_open_api/api/eastmoney/us_chinese_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/sse/sh_stock.py` & `stock-open-api-0.0.9/stock_open_api/api/sse/sh_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/api/sse/sh_stock_config.py` & `stock-open-api-0.0.9/stock_open_api/api/sse/sh_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/log.py` & `stock-open-api-0.0.9/stock_open_api/log.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api/utils/request_util.py` & `stock-open-api-0.0.9/stock_open_api/utils/request_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.8/stock_open_api.egg-info/PKG-INFO` & `stock-open-api-0.0.9/stock_open_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
         
@@ -124,14 +124,15 @@
             - github: [https://github.com/akfamily/akshare](https://github.com/akfamily/akshare)
             - doc: [https://akshare.akfamily.xyz/](https://akshare.akfamily.xyz/)
         
         - Tushare 免费提供各类数据 , 助力行业和量化研究。 
             - github: [https://github.com/waditu/tushare](https://github.com/waditu/tushare)
             - doc: [http://tushare.org/index.html](http://tushare.org/index.html)
             - pro doc: [https://tushare.pro/](https://tushare.pro/)
+        
 Keywords: stock,api
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `stock-open-api-0.0.8/stock_open_api.egg-info/SOURCES.txt` & `stock-open-api-0.0.9/stock_open_api.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 stock_open_api/api/eastmoney/kcb_stock_config.py
 stock_open_api/api/eastmoney/neeq_stock.py
 stock_open_api/api/eastmoney/neeq_stock_config.py
 stock_open_api/api/eastmoney/sh_stock.py
 stock_open_api/api/eastmoney/sz_stock.py
 stock_open_api/api/eastmoney/us_chinese_stock.py
 stock_open_api/api/eastmoney/us_chinese_stock_config.py
+stock_open_api/api/jqka/__init__.py
+stock_open_api/api/jqka/company.py
 stock_open_api/api/sse/__init__.py
 stock_open_api/api/sse/sh_stock.py
 stock_open_api/api/sse/sh_stock_config.py
 stock_open_api/items/__init__.py
 stock_open_api/items/list_item.py
 stock_open_api/utils/__init__.py
 stock_open_api/utils/iterator_util.py
```

