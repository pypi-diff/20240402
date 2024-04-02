# Comparing `tmp/zonevu-1.1.7-py3-none-any.whl.zip` & `tmp/zonevu-1.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1643350 bytes, number of entries: 805
+Zip file size: 1643335 bytes, number of entries: 805
 -rw-r--r--  2.0 fat       36 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/.gitignore
 -rw-r--r--  2.0 fat        2 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/3.11/@plugins_snapshot.json
 -rw-r--r--  2.0 fat     8174 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/3.11/__future__.data.json
 -rw-r--r--  2.0 fat     1632 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/3.11/__future__.meta.json
 -rw-r--r--  2.0 fat   180427 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/3.11/_ast.data.json
 -rw-r--r--  2.0 fat     1649 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/3.11/_ast.meta.json
 -rw-r--r--  2.0 fat    62778 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/3.11/_codecs.data.json
@@ -797,11 +797,11 @@
 -rw-r--r--  2.0 fat     2351 b- defN 80-Jan-01 00:00 zonevu/Services/SurveyService.py
 -rw-r--r--  2.0 fat     2738 b- defN 80-Jan-01 00:00 zonevu/Services/Utils.py
 -rw-r--r--  2.0 fat     2015 b- defN 80-Jan-01 00:00 zonevu/Services/WellData.py
 -rw-r--r--  2.0 fat     3810 b- defN 80-Jan-01 00:00 zonevu/Services/WelllogService.py
 -rw-r--r--  2.0 fat     9328 b- defN 80-Jan-01 00:00 zonevu/Services/WellService.py
 -rw-r--r--  2.0 fat     2002 b- defN 80-Jan-01 00:00 zonevu/Services/WelltopService.py
 -rw-r--r--  2.0 fat     5908 b- defN 80-Jan-01 00:00 zonevu/Zonevu.py
--rw-r--r--  2.0 fat     1099 b- defN 80-Jan-01 00:00 zonevu-1.1.7.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 zonevu-1.1.7.dist-info/WHEEL
-?rw-r--r--  2.0 fat    86308 b- defN 16-Jan-01 00:00 zonevu-1.1.7.dist-info/RECORD
-805 files, 25582090 bytes uncompressed, 1501626 bytes compressed:  94.1%
+-rw-r--r--  2.0 fat     1058 b- defN 80-Jan-01 00:00 zonevu-1.1.8.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 zonevu-1.1.8.dist-info/WHEEL
+?rw-r--r--  2.0 fat    86308 b- defN 16-Jan-01 00:00 zonevu-1.1.8.dist-info/RECORD
+805 files, 25582049 bytes uncompressed, 1501611 bytes compressed:  94.1%
```

## zipnote {}

```diff
@@ -2400,17 +2400,17 @@
 
 Filename: zonevu/Services/WelltopService.py
 Comment: 
 
 Filename: zonevu/Zonevu.py
 Comment: 
 
-Filename: zonevu-1.1.7.dist-info/METADATA
+Filename: zonevu-1.1.8.dist-info/METADATA
 Comment: 
 
-Filename: zonevu-1.1.7.dist-info/WHEEL
+Filename: zonevu-1.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: zonevu-1.1.7.dist-info/RECORD
+Filename: zonevu-1.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `zonevu-1.1.7.dist-info/METADATA` & `zonevu-1.1.8.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: zonevu
-Version: 1.1.7
+Version: 1.1.8
 Summary: ZoneVu Web API Python Package
 Home-page: https://www.ubiterra.com/
 License: MIT
 Author: Ubiterra
 Author-email: support@ubiterra.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0)
 Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pygeojson (>=0.2.0,<0.3.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: strenum (>=0.4.15,<0.5.0)
 Description-Content-Type: text/markdown
```

## Comparing `zonevu-1.1.7.dist-info/RECORD` & `zonevu-1.1.8.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -796,10 +796,10 @@
 zonevu/Services/SurveyService.py,sha256=QYEH6VKKuPbeRNamun256q30_D1rtESQbFLm5nIMWTU,2351
 zonevu/Services/Utils.py,sha256=3y_H9ouSNzZoyvRcFhI4eFPqrk61RPMnNEVoKdAo6M0,2738
 zonevu/Services/WellData.py,sha256=JRl7SDoLyl57-41du7TrQk0Hn820LDWgWAzfX5X85pQ,2015
 zonevu/Services/WelllogService.py,sha256=43XlmWVynJJMaKeFMyE4aas3nd4CyIFxA7QoQewIPgA,3810
 zonevu/Services/WellService.py,sha256=VpQoMv0_kYbOXXxp5e0rZqlonFR9lqXrp_w75uuaUk4,9328
 zonevu/Services/WelltopService.py,sha256=85DFGT3DSrqZIxyam8JM8PZ_PNqeq3v0LhrgPJoLM_8,2002
 zonevu/Zonevu.py,sha256=ouU3muL7hcqMdArEKcTcOJhsCkpsmTcNQII8g-a9cJE,5908
-zonevu-1.1.7.dist-info/METADATA,sha256=Cs9Rgzy0zcVyVa05ASZZ4tcdUn4CLEoDGpE97NqccuU,1099
-zonevu-1.1.7.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-zonevu-1.1.7.dist-info/RECORD,,
+zonevu-1.1.8.dist-info/METADATA,sha256=dz6pDu-tMB-Zy126XD0p9FoJIRwL0VnZez6nJXM47fo,1058
+zonevu-1.1.8.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+zonevu-1.1.8.dist-info/RECORD,,
```

