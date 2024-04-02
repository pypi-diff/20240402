# Comparing `tmp/ggun-0.0.2-py3-none-any.whl.zip` & `tmp/ggun-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9065 bytes, number of entries: 12
+Zip file size: 9052 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       23 b- defN 24-Mar-31 13:35 ggun/__init__.py
 -rw-rw-r--  2.0 unx     5419 b- defN 24-Mar-31 13:35 ggun/main.py
 -rw-rw-r--  2.0 unx       20 b- defN 24-Mar-31 13:47 ggun/commands/__init__.py
 -rw-rw-r--  2.0 unx    14277 b- defN 24-Mar-31 20:49 ggun/commands/test.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Mar-31 13:35 utils/__init__.py
--rw-rw-r--  2.0 unx     1591 b- defN 24-Mar-31 13:35 utils/api_call.py
+-rw-rw-r--  2.0 unx     1577 b- defN 24-Apr-02 13:45 utils/api_call.py
 -rw-rw-r--  2.0 unx     2261 b- defN 24-Mar-31 13:35 utils/list_files.py
--rw-rw-r--  2.0 unx      241 b- defN 24-Mar-31 20:50 ggun-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-31 20:50 ggun-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       35 b- defN 24-Mar-31 20:50 ggun-0.0.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       11 b- defN 24-Mar-31 20:50 ggun-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      897 b- defN 24-Mar-31 20:50 ggun-0.0.2.dist-info/RECORD
-12 files, 24867 bytes uncompressed, 7571 bytes compressed:  69.6%
+-rw-rw-r--  2.0 unx      241 b- defN 24-Apr-02 13:46 ggun-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-02 13:46 ggun-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       35 b- defN 24-Apr-02 13:46 ggun-0.0.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       11 b- defN 24-Apr-02 13:46 ggun-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      897 b- defN 24-Apr-02 13:46 ggun-0.0.3.dist-info/RECORD
+12 files, 24853 bytes uncompressed, 7558 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: utils/api_call.py
 Comment: 
 
 Filename: utils/list_files.py
 Comment: 
 
-Filename: ggun-0.0.2.dist-info/METADATA
+Filename: ggun-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: ggun-0.0.2.dist-info/WHEEL
+Filename: ggun-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: ggun-0.0.2.dist-info/entry_points.txt
+Filename: ggun-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ggun-0.0.2.dist-info/top_level.txt
+Filename: ggun-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ggun-0.0.2.dist-info/RECORD
+Filename: ggun-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## utils/api_call.py

```diff
@@ -2,15 +2,15 @@
 import os
 
 # API_URL = os.getenv("API_URL")
 # if API_URL is None:
 #     raise ValueError(
 #         "API_URL environment variable not set. Please set the API_URL environment variable."
 #     )
-API_URL = "https://34.49.175.177.nip.io/ggun-proxy"
+API_URL = "https://api.ggun.app:8080"
 
 TIMEOUT_TIME = 120
 
 
 def api_call(api_key, endpoint, req_type, data=None, files=None):
     endpoint_fmtd = f"/{endpoint}" if not endpoint.startswith("/") else endpoint
     url = f"{API_URL}/{endpoint_fmtd}"
```

## Comparing `ggun-0.0.2.dist-info/RECORD` & `ggun-0.0.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ggun/__init__.py,sha256=ZuXHO-b9d-MyvTiU9PSfWItKChRjKMqjHD15a7a9pZk,23
 ggun/main.py,sha256=3wdcbj0gOxT2WvAbIXeGlp8xgD2ydKtESEsYPCcZxzo,5419
 ggun/commands/__init__.py,sha256=NN4uHMI_a8xSJCUbzuPTfd14fY-t0vPGHwWjrmzgSL4,20
 ggun/commands/test.py,sha256=0yn47XU1AbHI-ox8wA0XO1yCj1lpKNSGcQWGGqSTQzk,14277
 utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-utils/api_call.py,sha256=k1b2IU8ieBA6WlVIKXCZ3flRPvM6FitxwM93i29mAi0,1591
+utils/api_call.py,sha256=Spd8Fjzdaw4ZGNxfO13O0pKskf-3cTSLhx53D1Xg58w,1577
 utils/list_files.py,sha256=_b3bvoTMb7gQh0DrgpXXk_F1Epdju67Bz0KR4hAGB_E,2261
-ggun-0.0.2.dist-info/METADATA,sha256=zYjScDb8Q8JQLzzNqaPDaruvC5AEf7YQ7bZ4_W_pClE,241
-ggun-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ggun-0.0.2.dist-info/entry_points.txt,sha256=YdLq3ka3RZvTQrtNCRK17TS8pXpWX4-tNzRL-uEpTC0,35
-ggun-0.0.2.dist-info/top_level.txt,sha256=7KfY85D4hwH5PHyWRel9YWjQzZNDVOugwhYxA64r0Qs,11
-ggun-0.0.2.dist-info/RECORD,,
+ggun-0.0.3.dist-info/METADATA,sha256=YNAV8BYhy1ORPrRJWBNfPGqIWhqjHMjOaW7J1omNoRw,241
+ggun-0.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ggun-0.0.3.dist-info/entry_points.txt,sha256=YdLq3ka3RZvTQrtNCRK17TS8pXpWX4-tNzRL-uEpTC0,35
+ggun-0.0.3.dist-info/top_level.txt,sha256=7KfY85D4hwH5PHyWRel9YWjQzZNDVOugwhYxA64r0Qs,11
+ggun-0.0.3.dist-info/RECORD,,
```

