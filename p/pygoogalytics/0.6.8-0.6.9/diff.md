# Comparing `tmp/pygoogalytics-0.6.8.tar.gz` & `tmp/pygoogalytics-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygoogalytics-0.6.8.tar", last modified: Mon Feb 26 16:23:33 2024, max compression
+gzip compressed data, was "pygoogalytics-0.6.9.tar", last modified: Mon Mar 25 14:23:29 2024, max compression
```

## Comparing `pygoogalytics-0.6.8.tar` & `pygoogalytics-0.6.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-02-26 16:23:33.611516 pygoogalytics-0.6.8/
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.6.8/LICENCE.txt
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.6.8/LICENSE
--rw-r--r--   0 joshua     (501) staff       (20)     6443 2024-02-26 16:23:33.611390 pygoogalytics-0.6.8/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)     5699 2023-05-10 09:11:02.000000 pygoogalytics-0.6.8/README.md
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-02-26 16:23:33.609383 pygoogalytics-0.6.8/pygoogalytics/
--rw-r--r--   0 joshua     (501) staff       (20)     1212 2024-02-26 16:23:22.000000 pygoogalytics-0.6.8/pygoogalytics/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     3254 2024-02-26 09:21:45.000000 pygoogalytics-0.6.8/pygoogalytics/ads_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)     5912 2023-08-21 14:09:23.000000 pygoogalytics-0.6.8/pygoogalytics/client.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-02-26 16:23:33.610578 pygoogalytics-0.6.8/pygoogalytics/data/
--rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.6.8/pygoogalytics/data/country_iso_codes.csv
--rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.6.8/pygoogalytics/data/google_ads_location_ids.csv
--rw-r--r--   0 joshua     (501) staff       (20)      343 2023-07-12 12:37:58.000000 pygoogalytics-0.6.8/pygoogalytics/framing.py
--rw-r--r--   0 joshua     (501) staff       (20)    43525 2024-02-08 18:44:39.000000 pygoogalytics-0.6.8/pygoogalytics/googalytics_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)    36871 2023-08-10 07:47:27.000000 pygoogalytics-0.6.8/pygoogalytics/googlepandas.py
--rw-r--r--   0 joshua     (501) staff       (20)    57392 2024-02-26 16:19:37.000000 pygoogalytics-0.6.8/pygoogalytics/kwp_wrappers.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-02-26 16:23:33.611174 pygoogalytics-0.6.8/pygoogalytics/utils/
--rw-r--r--   0 joshua     (501) staff       (20)        0 2023-06-21 13:16:26.000000 pygoogalytics-0.6.8/pygoogalytics/utils/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     2804 2024-02-26 09:21:45.000000 pygoogalytics-0.6.8/pygoogalytics/utils/ads_reports_parsing.py
--rw-r--r--   0 joshua     (501) staff       (20)     3445 2023-07-03 12:25:40.000000 pygoogalytics-0.6.8/pygoogalytics/utils/ga4_parser.py
--rw-r--r--   0 joshua     (501) staff       (20)     3214 2023-07-12 12:31:51.000000 pygoogalytics-0.6.8/pygoogalytics/utils/general_utils.py
--rw-r--r--   0 joshua     (501) staff       (20)     3272 2024-02-26 09:21:45.000000 pygoogalytics-0.6.8/pygoogalytics/utils/resource_utils.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-02-26 16:23:33.610291 pygoogalytics-0.6.8/pygoogalytics.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)     6443 2024-02-26 16:23:33.000000 pygoogalytics-0.6.8/pygoogalytics.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)      695 2024-02-26 16:23:33.000000 pygoogalytics-0.6.8/pygoogalytics.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2024-02-26 16:23:33.000000 pygoogalytics-0.6.8/pygoogalytics.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)      113 2024-02-26 16:23:33.000000 pygoogalytics-0.6.8/pygoogalytics.egg-info/requires.txt
--rw-r--r--   0 joshua     (501) staff       (20)       14 2024-02-26 16:23:33.000000 pygoogalytics-0.6.8/pygoogalytics.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2024-02-26 16:23:33.611561 pygoogalytics-0.6.8/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     1297 2024-02-26 16:23:22.000000 pygoogalytics-0.6.8/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-25 14:23:29.125212 pygoogalytics-0.6.9/
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.6.9/LICENCE.txt
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.6.9/LICENSE
+-rw-r--r--   0 joshua     (501) staff       (20)     6443 2024-03-25 14:23:29.125074 pygoogalytics-0.6.9/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     5699 2023-05-10 09:11:02.000000 pygoogalytics-0.6.9/README.md
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-25 14:23:29.121906 pygoogalytics-0.6.9/pygoogalytics/
+-rw-r--r--   0 joshua     (501) staff       (20)     1212 2024-03-25 14:23:26.000000 pygoogalytics-0.6.9/pygoogalytics/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     3254 2024-02-26 09:21:45.000000 pygoogalytics-0.6.9/pygoogalytics/ads_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5914 2024-03-25 09:56:54.000000 pygoogalytics-0.6.9/pygoogalytics/client.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-25 14:23:29.123804 pygoogalytics-0.6.9/pygoogalytics/data/
+-rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.6.9/pygoogalytics/data/country_iso_codes.csv
+-rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.6.9/pygoogalytics/data/google_ads_location_ids.csv
+-rw-r--r--   0 joshua     (501) staff       (20)      343 2023-07-12 12:37:58.000000 pygoogalytics-0.6.9/pygoogalytics/framing.py
+-rw-r--r--   0 joshua     (501) staff       (20)    43525 2024-02-08 18:44:39.000000 pygoogalytics-0.6.9/pygoogalytics/googalytics_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)    36871 2023-08-10 07:47:27.000000 pygoogalytics-0.6.9/pygoogalytics/googlepandas.py
+-rw-r--r--   0 joshua     (501) staff       (20)    59317 2024-03-25 14:21:18.000000 pygoogalytics-0.6.9/pygoogalytics/kwp_wrappers.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-25 14:23:29.124760 pygoogalytics-0.6.9/pygoogalytics/utils/
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2023-06-21 13:16:26.000000 pygoogalytics-0.6.9/pygoogalytics/utils/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2804 2024-02-26 09:21:45.000000 pygoogalytics-0.6.9/pygoogalytics/utils/ads_reports_parsing.py
+-rw-r--r--   0 joshua     (501) staff       (20)     3445 2023-07-03 12:25:40.000000 pygoogalytics-0.6.9/pygoogalytics/utils/ga4_parser.py
+-rw-r--r--   0 joshua     (501) staff       (20)     3214 2023-07-12 12:31:51.000000 pygoogalytics-0.6.9/pygoogalytics/utils/general_utils.py
+-rw-r--r--   0 joshua     (501) staff       (20)     3272 2024-02-26 09:21:45.000000 pygoogalytics-0.6.9/pygoogalytics/utils/resource_utils.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-25 14:23:29.123236 pygoogalytics-0.6.9/pygoogalytics.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)     6443 2024-03-25 14:23:29.000000 pygoogalytics-0.6.9/pygoogalytics.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)      695 2024-03-25 14:23:29.000000 pygoogalytics-0.6.9/pygoogalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2024-03-25 14:23:29.000000 pygoogalytics-0.6.9/pygoogalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)      113 2024-03-25 14:23:29.000000 pygoogalytics-0.6.9/pygoogalytics.egg-info/requires.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       14 2024-03-25 14:23:29.000000 pygoogalytics-0.6.9/pygoogalytics.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2024-03-25 14:23:29.125268 pygoogalytics-0.6.9/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     1297 2024-03-25 14:23:26.000000 pygoogalytics-0.6.9/setup.py
```

### Comparing `pygoogalytics-0.6.8/LICENCE.txt` & `pygoogalytics-0.6.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.6.8/LICENSE` & `pygoogalytics-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.6.8/PKG-INFO` & `pygoogalytics-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.6.8
+Version: 0.6.9
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.6.8/README.md` & `pygoogalytics-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.6.8/pygoogalytics/__init__.py` & `pygoogalytics-0.6.9/pygoogalytics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   sc_domain='<search-console-domain>',
   view_id='<ga3-view-id>',
   ga4_property_id='<ga4-property-id>'
 )
 ```
 """
 
-__version__ = "0.6.8"
+__version__ = "0.6.9"
 __author__ = 'Joshua Prettyman'
 __credits__ = 'Blink SEO'
 
 import os
 import csv
 import logging
```

### Comparing `pygoogalytics-0.6.8/pygoogalytics/ads_wrapper.py` & `pygoogalytics-0.6.9/pygoogalytics/ads_wrapper.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.6.8/pygoogalytics/client.py` & `pygoogalytics-0.6.9/pygoogalytics/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,7 +137,9 @@
                                       language_id=language_id)
 
     def report_service(self, customer_id: str):
         if customer_id is None:
             customer_id = self.default_customer_id
         return AdsWrapper(googleads_client=self.googleads_client,
                           customer_id=parse_ads_id(customer_id))
+
+
```

### Comparing `pygoogalytics-0.6.8/pygoogalytics/data/country_iso_codes.csv` & `pygoogalytics-0.6.9/pygoogalytics/data/country_iso_codes.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.6.8/pygoogalytics/data/google_ads_location_ids.csv` & `pygoogalytics-0.6.9/pygoogalytics/data/google_ads_location_ids.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.6.8/pygoogalytics/googalytics_wrapper.py` & `pygoogalytics-0.6.9/pygoogalytics/googalytics_wrapper.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.6.8/pygoogalytics/googlepandas.py` & `pygoogalytics-0.6.9/pygoogalytics/googlepandas.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.6.8/pygoogalytics/kwp_wrappers.py` & `pygoogalytics-0.6.9/pygoogalytics/kwp_wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -913,14 +913,26 @@
 
         _df = pd.DataFrame(keyword_ideas)
         _df["volume_trend_coef"] = _df["volume_trend"].apply(_three_month_trend_coef)
         _df["latest_volume"] = _df["volume_trend"].apply(_latest_volume)
 
         return _df
 
+    def historical_metrics_generator(self,
+                                     keywords: str | list[str] | None = None,
+                                     include_adult_keywords: bool = True,
+                                     location_codes: list[str] = None,
+                                     language_id: str = None,
+                                     calculated_fields: bool = True,
+                                     concat_locations: bool = True,
+                                     print_progress: bool = False):
+
+        pass
+
+
     def generate_historical_metrics(self,
                                    keywords: str | list[str] | None = None,
                                    include_adult_keywords: bool = True,
                                    location_codes: list[str] = None,
                                    language_id: str = None,
                                     calculated_fields: bool = True,
                                     concat_locations: bool = True,
@@ -985,23 +997,38 @@
         monthly_volume_df['month_enum'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[2])
         monthly_volume_df['month'] = monthly_volume_df['month_enum'].apply(_get_month_from_enum_value)
         monthly_volume_df['year'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[1])
 
         monthly_volume_df.dropna(axis='index', subset=['month'], inplace=True)
 
         monthly_volume_df['record_date'] = monthly_volume_df.apply(
-            lambda df: _conv_date(df['year'], df['month'], 15, month_index=0),
+            lambda _mvdf: _conv_date(_mvdf['year'], _mvdf['month'], 15, month_index=0),
             axis=1
         )
         monthly_volume_df['volume'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[0])
 
         monthly_volume_df.drop(
             columns=['month_enum', 'volume_trend_tuples', 'month', 'year', 'month_name'],
             inplace=True
         )
+        monthly_volume_df.fillna(value={'competition': "UNSPECIFIED", 'competition_index': 0.0}, inplace=True)
+
+            # monthly_volume_df = pd.DataFrame(
+            #     columns=[
+            #         "country_iso_code",
+            #         "date_obtained",
+            #         "query",
+            #         "keyword",
+            #         "status",
+            #         "record_date",
+            #         "volume",
+            #         "competition",
+            #         "competition_index"
+            #     ]
+            # )
 
         metrics_df.drop_duplicates(subset=["country_iso_code", "query", "keyword"], keep="first", inplace=True)
         monthly_volume_df.drop_duplicates(subset=["country_iso_code", "query", "keyword", "record_date"], keep="first", inplace=True)
 
         metrics_df.reset_index(drop=True, inplace=True)
         monthly_volume_df.reset_index(drop=True, inplace=True)
 
@@ -1099,28 +1126,34 @@
                     "competition_index": _m.keyword_metrics.competition_index,
                     "low_top_of_page_bid_micros": _m.keyword_metrics.low_top_of_page_bid_micros,
                     "high_top_of_page_bid_micros": _m.keyword_metrics.high_top_of_page_bid_micros,
                     "volume_trend": [v.monthly_searches for v in _m.keyword_metrics.monthly_search_volumes],
                     "volume_trend_tuples": [(v.monthly_searches, v.year, v.month.value, v.month.name)
                                                 for v in _m.keyword_metrics.monthly_search_volumes]
                 }
+
+                if not _metric["volume_trend"]:
+                    _metric["status"] = "NO_VOLUME_DATA"
+                    _metric["volume_trend"] = [0]*12
+                    _metric["volume_trend_tuples"] = _empty_volume_trend_tuples()
+
                 metrics.append(_metric)
 
         empty_metric = {
             "date_obtained": _date_today,
             "country_iso_code": '-'.join(location_codes),
             "query": "",
             "status": "NOT_OBTAINED",
             "avg_searches": 0,
             "competition": "",
             "competition_index": None,
             "low_top_of_page_bid_micros": 0,
             "high_top_of_page_bid_micros": 0,
-            "volume_trend": [],
-            "volume_trend_tuples": []
+            "volume_trend": [0]*12,
+            "volume_trend_tuples": _empty_volume_trend_tuples()
         }
 
         for _missing_keyword in set(keywords) - set(m.get("keyword") for m in metrics):
             _metric = empty_metric.copy()
             _metric["keyword"] = _missing_keyword
             metrics.append(_metric)
 
@@ -1338,14 +1371,32 @@
 def _get_month_from_enum_value(month_enum_value):
     if month_enum_value <= 1:
         return None
     else:
         return month_enum_value - 2
 
 
+def _add_months(dt: datetime.date, months: int) -> datetime.date:
+    m = dt.month - 1 + months
+    return datetime.date(
+        year=dt.year + m // 12,
+        month=m % 12 + 1,
+        day=dt.day)
+
+
+def _empty_volume_trend_tuples(n: int = 12):
+    _last_month = _add_months(datetime.date.today(), -1)
+    months = [_add_months(datetime.date(_last_month.year, _last_month.month, 15), -i) for i in range(n)]
+    return [(0.0,
+             d.year,
+             d.month + 1,
+             d.strftime('%B').upper()
+             ) for d in months]
+
+
 def strip_illegal_chars(s, language_id):
     # lower case obvs
     s = s.lower()
     # replace `‘’ with simple '
     s = re.sub(r"[`‘’]+", "'", s)
     # first remove any non-ascii characters, replace with a space
     if language_id in ['1001']:  # when german language_id don't replace one of [Ä, ä, Ö, ö, Ü, ü, ß]
```

### Comparing `pygoogalytics-0.6.8/pygoogalytics/utils/ads_reports_parsing.py` & `pygoogalytics-0.6.9/pygoogalytics/utils/ads_reports_parsing.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.6.8/pygoogalytics/utils/ga4_parser.py` & `pygoogalytics-0.6.9/pygoogalytics/utils/ga4_parser.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.6.8/pygoogalytics/utils/general_utils.py` & `pygoogalytics-0.6.9/pygoogalytics/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.6.8/pygoogalytics/utils/resource_utils.py` & `pygoogalytics-0.6.9/pygoogalytics/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.6.8/pygoogalytics.egg-info/PKG-INFO` & `pygoogalytics-0.6.9/pygoogalytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.6.8
+Version: 0.6.9
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.6.8/pygoogalytics.egg-info/SOURCES.txt` & `pygoogalytics-0.6.9/pygoogalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.6.8/setup.py` & `pygoogalytics-0.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # twine upload dist/*
 
 _desc = """PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 in the form of a pandas dataframe."""
 
 setup(
     name='pygoogalytics',
-    version='0.6.8',
+    version='0.6.9',
     description=_desc,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Blink-SEO/pygoogalytics',
     author='Joshua Prettyman',
     author_email='joshua@blinkseo.co.uk',
     license='MIT',
```

