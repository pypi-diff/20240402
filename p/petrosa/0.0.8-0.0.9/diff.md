# Comparing `tmp/petrosa-0.0.8-py3-none-any.whl.zip` & `tmp/petrosa-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 5398 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 petrosa/converters/__init__.py
--rw-r--r--  2.0 unx     2322 b- defN 20-Feb-02 00:00 petrosa/converters/backtests.py
+-rw-r--r--  2.0 unx     2325 b- defN 20-Feb-02 00:00 petrosa/converters/backtests.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 petrosa/ta/__init__.py
 -rw-r--r--  2.0 unx    22023 b- defN 20-Feb-02 00:00 petrosa/ta/strategies.py
 -rw-r--r--  2.0 unx      822 b- defN 20-Feb-02 00:00 petrosa/ta/utils.py
-?rw-r--r--  2.0 unx      716 b- defN 20-Feb-02 00:00 petrosa-0.0.8.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 petrosa-0.0.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1063 b- defN 20-Feb-02 00:00 petrosa-0.0.8.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      707 b- defN 20-Feb-02 00:00 petrosa-0.0.8.dist-info/RECORD
-9 files, 27740 bytes uncompressed, 4178 bytes compressed:  84.9%
+?rw-r--r--  2.0 unx      716 b- defN 20-Feb-02 00:00 petrosa-0.0.9.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 petrosa-0.0.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1063 b- defN 20-Feb-02 00:00 petrosa-0.0.9.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      707 b- defN 20-Feb-02 00:00 petrosa-0.0.9.dist-info/RECORD
+9 files, 27743 bytes uncompressed, 4178 bytes compressed:  84.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: petrosa/ta/strategies.py
 Comment: 
 
 Filename: petrosa/ta/utils.py
 Comment: 
 
-Filename: petrosa-0.0.8.dist-info/METADATA
+Filename: petrosa-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: petrosa-0.0.8.dist-info/WHEEL
+Filename: petrosa-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: petrosa-0.0.8.dist-info/licenses/LICENSE
+Filename: petrosa-0.0.9.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: petrosa-0.0.8.dist-info/RECORD
+Filename: petrosa-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## petrosa/converters/backtests.py

```diff
@@ -36,15 +36,15 @@
         elif isinstance(stats[key], pd.Timestamp):
             ret_res[key] = stats[key].to_pydatetime()
         else:
             ret_res[key] = stats[key]
 
     return ret_res
 
-def result_maker(bt_stats, params, bt_test_params, test_type):        
+def result_maker(bt_stats, bt_params, bt_test_params, test_type):        
     if '_trades' in bt_stats:
         del(bt_stats['_trades'])
     if '_strategy' in bt_stats:
         del(bt_stats['_strategy'])
     if '_equity_curve' in bt_stats:
         del(bt_stats['_equity_curve'])
```

## Comparing `petrosa-0.0.8.dist-info/METADATA` & `petrosa-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petrosa
-Version: 0.0.8
+Version: 0.0.9
 Summary: utilities for PETROSA
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: "@yurisa2" <yuri@sa2.com.br>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `petrosa-0.0.8.dist-info/licenses/LICENSE` & `petrosa-0.0.9.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

