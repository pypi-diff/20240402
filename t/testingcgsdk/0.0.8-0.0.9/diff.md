# Comparing `tmp/testingcgsdk-0.0.8-py3-none-any.whl.zip` & `tmp/testingcgsdk-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 4536 bytes, number of entries: 14
+Zip file size: 4592 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat       29 b- defN 24-Mar-28 04:54 testingcgsdk/__init__.py
--rw-rw-rw-  2.0 fat      352 b- defN 24-Apr-01 11:27 testingcgsdk/app.py
--rw-rw-rw-  2.0 fat      213 b- defN 24-Apr-01 11:07 testingcgsdk/cglense.py
+-rw-rw-rw-  2.0 fat      244 b- defN 24-Apr-02 08:11 testingcgsdk/app.py
+-rw-rw-rw-  2.0 fat      479 b- defN 24-Apr-02 08:12 testingcgsdk/cglense.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 07:55 testingcgsdk/data_load/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 07:57 testingcgsdk/data_load/config/__init__.py
 -rw-rw-rw-  2.0 fat      763 b- defN 24-Mar-27 07:58 testingcgsdk/data_load/config/database_config.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 07:56 testingcgsdk/data_load/monitor/__init__.py
 -rw-rw-rw-  2.0 fat      526 b- defN 24-Apr-01 11:06 testingcgsdk/data_load/monitor/models.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 07:58 testingcgsdk/data_load/read_data/__init__.py
 -rw-rw-rw-  2.0 fat     1106 b- defN 24-Apr-01 11:07 testingcgsdk/data_load/read_data/load_data.py
--rw-rw-rw-  2.0 fat      428 b- defN 24-Apr-02 08:01 testingcgsdk-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 08:01 testingcgsdk-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-02 08:01 testingcgsdk-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1229 b- defN 24-Apr-02 08:01 testingcgsdk-0.0.8.dist-info/RECORD
-14 files, 4751 bytes uncompressed, 2434 bytes compressed:  48.8%
+-rw-rw-rw-  2.0 fat      428 b- defN 24-Apr-02 08:13 testingcgsdk-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 08:13 testingcgsdk-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-02 08:13 testingcgsdk-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1229 b- defN 24-Apr-02 08:13 testingcgsdk-0.0.9.dist-info/RECORD
+14 files, 4909 bytes uncompressed, 2490 bytes compressed:  49.3%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: testingcgsdk/data_load/read_data/__init__.py
 Comment: 
 
 Filename: testingcgsdk/data_load/read_data/load_data.py
 Comment: 
 
-Filename: testingcgsdk-0.0.8.dist-info/METADATA
+Filename: testingcgsdk-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: testingcgsdk-0.0.8.dist-info/WHEEL
+Filename: testingcgsdk-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: testingcgsdk-0.0.8.dist-info/top_level.txt
+Filename: testingcgsdk-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: testingcgsdk-0.0.8.dist-info/RECORD
+Filename: testingcgsdk-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## testingcgsdk/app.py

```diff
@@ -1,14 +1,12 @@
 import pandas as pd
 from testingcgsdk.data_load.read_data.load_data import data_loading
-import uvicorn
-from fastapi import FastAPI
+
 
 app = FastAPI()
 @app.post("/insert_data_api")
 def insert_data(filename):
     obj = data_loading()
     return (obj._load_csv(filename))
     
 
 
-uvicorn.run("app:app", reload =False, host="127.0.0.1",port=8519)
```

## testingcgsdk/cglense.py

```diff
@@ -1,9 +1,17 @@
 from testingcgsdk.data_load.read_data.load_data import data_loading
+import uvicorn
+from fastapi import FastAPI
 
+app = FastAPI()
+@app.post("/insert_data_api")
+def insert_data(filename):
+    obj = data_loading()
+    return (obj._load_csv(filename))
 
 def read_csv(filename):
     obj = data_loading()
     return (obj._load_csv(filename))
     
     #def read_excel(self,filename):
-        
+def start_app():
+    uvicorn.run("app:app", reload =False, host="127.0.0.1",port=8519)
```

## Comparing `testingcgsdk-0.0.8.dist-info/RECORD` & `testingcgsdk-0.0.9.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 testingcgsdk/__init__.py,sha256=Mzp5XSCcmvFnNVgRveytVqDXgeeR-lZbnsY_vPVU-0o,29
-testingcgsdk/app.py,sha256=eRifHgAhN8v1S-s9Zvt9wg8Cbr45AXR0Te8B2Aivj5M,352
-testingcgsdk/cglense.py,sha256=lEFqzqYU6huGuqCeOtRyDbmSS38z0NO5ukHaQ2i9U2E,213
+testingcgsdk/app.py,sha256=qx1L_NpOtqIbFEcAWKjADX3pu83E8nPSnrF4uN2_NGU,244
+testingcgsdk/cglense.py,sha256=AeUGjC82YJ4l3GARUp9CyQ1__Jkr4img__eWo9LyIK8,479
 testingcgsdk/data_load/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 testingcgsdk/data_load/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 testingcgsdk/data_load/config/database_config.py,sha256=7n2Eygt3jt0bS-3Rm5lZo_xGn2WwxrBFT3Nq0jvDeew,763
 testingcgsdk/data_load/monitor/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 testingcgsdk/data_load/monitor/models.py,sha256=Q7Q8WkDRJKuWArvukeaG69Q3_NMhoKoe0t40cI4I7kI,526
 testingcgsdk/data_load/read_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 testingcgsdk/data_load/read_data/load_data.py,sha256=Z8hwFwgtu7ibudpDOOcmHvUUSLKLvnNVnLCdhV1_Thc,1106
-testingcgsdk-0.0.8.dist-info/METADATA,sha256=C5cPrSr6i25KXJmw2fssPNrR2dWmRv4Nuy03DFv-cVU,428
-testingcgsdk-0.0.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-testingcgsdk-0.0.8.dist-info/top_level.txt,sha256=S_hWREYGcy004BFVlcBPpnYuim5W-R3TQyOPc0JmqBI,13
-testingcgsdk-0.0.8.dist-info/RECORD,,
+testingcgsdk-0.0.9.dist-info/METADATA,sha256=5VLaCoOIKicwH2zmu58Ak1GbMHdwhuotUZwGqL5I2Xs,428
+testingcgsdk-0.0.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+testingcgsdk-0.0.9.dist-info/top_level.txt,sha256=S_hWREYGcy004BFVlcBPpnYuim5W-R3TQyOPc0JmqBI,13
+testingcgsdk-0.0.9.dist-info/RECORD,,
```

