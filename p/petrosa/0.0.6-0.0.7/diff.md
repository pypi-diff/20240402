# Comparing `tmp/petrosa-0.0.6-py3-none-any.whl.zip` & `tmp/petrosa-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5384 bytes, number of entries: 9
+Zip file size: 5396 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 petrosa/converters/__init__.py
--rw-r--r--  2.0 unx     2257 b- defN 20-Feb-02 00:00 petrosa/converters/backtests.py
+-rw-r--r--  2.0 unx     2322 b- defN 20-Feb-02 00:00 petrosa/converters/backtests.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 petrosa/ta/__init__.py
 -rw-r--r--  2.0 unx    22023 b- defN 20-Feb-02 00:00 petrosa/ta/strategies.py
 -rw-r--r--  2.0 unx      822 b- defN 20-Feb-02 00:00 petrosa/ta/utils.py
-?rw-r--r--  2.0 unx      716 b- defN 20-Feb-02 00:00 petrosa-0.0.6.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 petrosa-0.0.6.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1063 b- defN 20-Feb-02 00:00 petrosa-0.0.6.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      707 b- defN 20-Feb-02 00:00 petrosa-0.0.6.dist-info/RECORD
-9 files, 27675 bytes uncompressed, 4164 bytes compressed:  85.0%
+?rw-r--r--  2.0 unx      716 b- defN 20-Feb-02 00:00 petrosa-0.0.7.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 petrosa-0.0.7.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1063 b- defN 20-Feb-02 00:00 petrosa-0.0.7.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      707 b- defN 20-Feb-02 00:00 petrosa-0.0.7.dist-info/RECORD
+9 files, 27740 bytes uncompressed, 4176 bytes compressed:  84.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: petrosa/ta/strategies.py
 Comment: 
 
 Filename: petrosa/ta/utils.py
 Comment: 
 
-Filename: petrosa-0.0.6.dist-info/METADATA
+Filename: petrosa-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: petrosa-0.0.6.dist-info/WHEEL
+Filename: petrosa-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: petrosa-0.0.6.dist-info/licenses/LICENSE
+Filename: petrosa-0.0.7.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: petrosa-0.0.6.dist-info/RECORD
+Filename: petrosa-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## petrosa/converters/backtests.py

```diff
@@ -36,31 +36,31 @@
         elif isinstance(stats[key], pd.Timestamp):
             ret_res[key] = stats[key].to_pydatetime()
         else:
             ret_res[key] = stats[key]
 
     return ret_res
 
-def result_maker(stats, params, test_params, test_type):
-    if '_trades' in stats:
-        del(stats['_trades'])
-    if '_strategy' in stats:
-        del(stats['_strategy'])
-    if '_equity_curve' in stats:
-        del(stats['_equity_curve'])
+def result_maker(bt_stats, params, bt_test_params, test_type):        
+    if '_trades' in bt_stats:
+        del(bt_stats['_trades'])
+    if '_strategy' in bt_stats:
+        del(bt_stats['_strategy'])
+    if '_equity_curve' in bt_stats:
+        del(bt_stats['_equity_curve'])
         
-    if '_id' in test_params:
-        del(test_params["_id"])
+    if '_id' in bt_test_params:
+        del(bt_test_params["_id"])
 
-    stats = remove_weird_chars(stats)
-    params = remove_weird_chars(params)
+    bt_stats = remove_weird_chars(bt_stats)
+    bt_params = remove_weird_chars(bt_params)
 
-    stats = dict_time_convert(stats)
+    bt_stats = dict_time_convert(bt_stats)
     
-    ret = {**test_params, **stats, **params}
+    ret = {**bt_test_params, **bt_stats, **bt_params}
     ret['test_type'] = test_type
     ret['insert_timestamp'] = datetime.datetime.now()
         
     return ret
 
 
 def list_maker(stats, test_params):
```

## Comparing `petrosa-0.0.6.dist-info/METADATA` & `petrosa-0.0.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petrosa
-Version: 0.0.6
+Version: 0.0.7
 Summary: utilities for PETROSA
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: "@yurisa2" <yuri@sa2.com.br>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `petrosa-0.0.6.dist-info/licenses/LICENSE` & `petrosa-0.0.7.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `petrosa-0.0.6.dist-info/RECORD` & `petrosa-0.0.7.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 petrosa/converters/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-petrosa/converters/backtests.py,sha256=XCtt33mNBlP9RUaNzZ0rIe0HCn446AUtBh7ICXELas0,2257
+petrosa/converters/backtests.py,sha256=n5f6yrZstX5aOsgcGj2gl4P1hMaaoijV5NPnF2j_KeI,2322
 petrosa/ta/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 petrosa/ta/strategies.py,sha256=W_x2vxE891pOHLGKKtSRohCDWifIa70pALXevToIPSc,22023
 petrosa/ta/utils.py,sha256=77IZzQVRMw1MPwYw-MTWv-CXhtbdtppzXEzxcgvGXAw,822
-petrosa-0.0.6.dist-info/METADATA,sha256=u9DanrpuoDEzQBk5Zv6W2_8x7eTDOXSs-4JKF_MrTTE,716
-petrosa-0.0.6.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-petrosa-0.0.6.dist-info/licenses/LICENSE,sha256=laAtIGoDbZBqhkTalLLdtCwZumW9xZhoDe9AvKKviQk,1063
-petrosa-0.0.6.dist-info/RECORD,,
+petrosa-0.0.7.dist-info/METADATA,sha256=8eifqjRo7-hP8-qLCc3lWsA9K1ohSMhNU3ao28b1cNI,716
+petrosa-0.0.7.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+petrosa-0.0.7.dist-info/licenses/LICENSE,sha256=laAtIGoDbZBqhkTalLLdtCwZumW9xZhoDe9AvKKviQk,1063
+petrosa-0.0.7.dist-info/RECORD,,
```

