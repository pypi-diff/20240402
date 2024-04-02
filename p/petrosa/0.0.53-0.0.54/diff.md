# Comparing `tmp/petrosa-0.0.53-py3-none-any.whl.zip` & `tmp/petrosa-0.0.54-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 3218282 bytes, number of entries: 22
+Zip file size: 3218319 bytes, number of entries: 22
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 petrosa/__init__.py
 -rw-r--r--  2.0 unx     1811 b- defN 20-Feb-02 00:00 petrosa/binance/binance.py
 -rw-r--r--  2.0 unx     1473 b- defN 20-Feb-02 00:00 petrosa/checkers/consistency.py
 -rw-r--r--  2.0 unx        9 b- defN 20-Feb-02 00:00 petrosa/converters/.gitignore
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 petrosa/converters/__init__.py
 -rw-r--r--  2.0 unx     2778 b- defN 20-Feb-02 00:00 petrosa/converters/backtests.py
 -rw-r--r--  2.0 unx     1502 b- defN 20-Feb-02 00:00 petrosa/converters/data.pickle
 -rw-r--r--  2.0 unx      173 b- defN 20-Feb-02 00:00 petrosa/converters/myparams.pickle
 -rw-r--r--  2.0 unx        5 b- defN 20-Feb-02 00:00 petrosa/converters/params.pickle
 -rw-r--r--  2.0 unx 12175544 b- defN 20-Feb-02 00:00 petrosa/converters/stats.pickle
 -rw-r--r--  2.0 unx     3688 b- defN 20-Feb-02 00:00 petrosa/database/mongo.py
--rw-r--r--  2.0 unx     1621 b- defN 20-Feb-02 00:00 petrosa/database/sql.py
+-rw-r--r--  2.0 unx     1742 b- defN 20-Feb-02 00:00 petrosa/database/sql.py
 -rw-r--r--  2.0 unx      462 b- defN 20-Feb-02 00:00 petrosa/messaging/kafkaproducer.py
 -rw-r--r--  2.0 unx      547 b- defN 20-Feb-02 00:00 petrosa/messaging/kafkareceiver.py
 -rw-r--r--  2.0 unx      198 b- defN 20-Feb-02 00:00 petrosa/observability/opentel.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 petrosa/ta/__init__.py
 -rw-r--r--  2.0 unx    25122 b- defN 20-Feb-02 00:00 petrosa/ta/strategies.py
 -rw-r--r--  2.0 unx      970 b- defN 20-Feb-02 00:00 petrosa/ta/utils.py
-?rw-r--r--  2.0 unx      867 b- defN 20-Feb-02 00:00 petrosa-0.0.53.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 petrosa-0.0.53.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1063 b- defN 20-Feb-02 00:00 petrosa-0.0.53.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1823 b- defN 20-Feb-02 00:00 petrosa-0.0.53.dist-info/RECORD
-22 files, 12219743 bytes uncompressed, 3215306 bytes compressed:  73.7%
+?rw-r--r--  2.0 unx      867 b- defN 20-Feb-02 00:00 petrosa-0.0.54.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 petrosa-0.0.54.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1063 b- defN 20-Feb-02 00:00 petrosa-0.0.54.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1823 b- defN 20-Feb-02 00:00 petrosa-0.0.54.dist-info/RECORD
+22 files, 12219864 bytes uncompressed, 3215343 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: petrosa/ta/strategies.py
 Comment: 
 
 Filename: petrosa/ta/utils.py
 Comment: 
 
-Filename: petrosa-0.0.53.dist-info/METADATA
+Filename: petrosa-0.0.54.dist-info/METADATA
 Comment: 
 
-Filename: petrosa-0.0.53.dist-info/WHEEL
+Filename: petrosa-0.0.54.dist-info/WHEEL
 Comment: 
 
-Filename: petrosa-0.0.53.dist-info/licenses/LICENSE
+Filename: petrosa-0.0.54.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: petrosa-0.0.53.dist-info/RECORD
+Filename: petrosa-0.0.54.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## petrosa/database/sql.py

```diff
@@ -65,13 +65,16 @@
 
 
 def run_generic_sql(sql_str):
     logging.info(f"Running Generic SQL {sql_str}")
     cnx, cursor = connect_mysql()
 
     cursor.execute(sql_str)
-    rows = cursor.fetchall()
+    if(sql_str[:5] == "SELECT" or sql_str[:5] == "select" or sql_str[:5] == "Select"):
+        rows = cursor.fetchall()
+    else:
+        rows = None
     cnx.commit()
     cursor.close()
     cnx.close()
 
     return rows
```

## Comparing `petrosa-0.0.53.dist-info/METADATA` & `petrosa-0.0.54.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petrosa
-Version: 0.0.53
+Version: 0.0.54
 Summary: utilities for PETROSA
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: "@yurisa2" <yuri@sa2.com.br>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `petrosa-0.0.53.dist-info/licenses/LICENSE` & `petrosa-0.0.54.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `petrosa-0.0.53.dist-info/RECORD` & `petrosa-0.0.54.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 petrosa/converters/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 petrosa/converters/backtests.py,sha256=qzBezorvhz1eJOBEpCC7iiOi0FwsfRWEns0wOwXIZxM,2778
 petrosa/converters/data.pickle,sha256=4ZRZzV7J6e7RmvQIFOByGY49z13GF1prScyiPxzyXRI,1502
 petrosa/converters/myparams.pickle,sha256=pT7nHfsgiqi4nKWc3cZmPYuBOeOc5ZuYV_sYowcwtQc,173
 petrosa/converters/params.pickle,sha256=kmJI5S0fpTLDF-N9ok7WUq5kEQ-CGcteBhZovTCR8Eg,5
 petrosa/converters/stats.pickle,sha256=22SCtV1DXDvZLIQxn01XRLll97bxQd7j0dmxJyXPRn0,12175544
 petrosa/database/mongo.py,sha256=xXvDA43TTPtyF0ysvf1YPrHg8JrZ_Se4dTjN2takbC8,3688
-petrosa/database/sql.py,sha256=3PzBsjzENSfsV6przKmArD5sUsg2Cdb4PMMeWzYApWo,1621
+petrosa/database/sql.py,sha256=WthuNgT21WexfYHFkl17xN0lfLoR3RVHESJVDFy2hEw,1742
 petrosa/messaging/kafkaproducer.py,sha256=1QoL2eHPSq2NMPTm0XJn0_DXC4EmFNrMLxLBWk5bEdM,462
 petrosa/messaging/kafkareceiver.py,sha256=kUYbOBODRCyNraavliBYEFmoEm_Wj4YCNwJnj5nlnog,547
 petrosa/observability/opentel.py,sha256=cHlDr30pIJrKXwgn54ZGnBASz-4dw7bDG4Ic444ymsQ,198
 petrosa/ta/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 petrosa/ta/strategies.py,sha256=jD_J8Y80eE9CeDpwYgj-CMht4magQs6dIRXODzIGLVY,25122
 petrosa/ta/utils.py,sha256=13byDJmIn4mdescxByhDQX68sRV-ycKjRLJhUWIxHc0,970
-petrosa-0.0.53.dist-info/METADATA,sha256=6pJWXaw7gF3480spzAkp2LUuI7YTwsQ8WPrFG1zgwb4,867
-petrosa-0.0.53.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-petrosa-0.0.53.dist-info/licenses/LICENSE,sha256=laAtIGoDbZBqhkTalLLdtCwZumW9xZhoDe9AvKKviQk,1063
-petrosa-0.0.53.dist-info/RECORD,,
+petrosa-0.0.54.dist-info/METADATA,sha256=sBhkIudiX86fr2IfkOdHXiXeHY2g6txJ_zw0sG43Zdo,867
+petrosa-0.0.54.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+petrosa-0.0.54.dist-info/licenses/LICENSE,sha256=laAtIGoDbZBqhkTalLLdtCwZumW9xZhoDe9AvKKviQk,1063
+petrosa-0.0.54.dist-info/RECORD,,
```

