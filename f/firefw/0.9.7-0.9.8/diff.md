# Comparing `tmp/firefw-0.9.7-py3-none-any.whl.zip` & `tmp/firefw-0.9.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12439 bytes, number of entries: 9
+Zip file size: 12435 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      241 b- defN 80-Jan-01 00:00 firefw/__init__.py
 -rw-r--r--  2.0 unx     5087 b- defN 80-Jan-01 00:00 firefw/core.py
 -rw-r--r--  2.0 unx     4343 b- defN 80-Jan-01 00:00 firefw/irbuilder.py
 -rw-r--r--  2.0 unx    18974 b- defN 80-Jan-01 00:00 firefw/runtime.py
 -rw-r--r--  2.0 unx     2119 b- defN 80-Jan-01 00:00 firefw/tracing.py
--rw-r--r--  2.0 unx     1513 b- defN 80-Jan-01 00:00 firefw-0.9.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      767 b- defN 80-Jan-01 00:00 firefw-0.9.7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 firefw-0.9.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx      663 b- defN 16-Jan-01 00:00 firefw-0.9.7.dist-info/RECORD
-9 files, 33795 bytes uncompressed, 11319 bytes compressed:  66.5%
+-rw-r--r--  2.0 unx     1513 b- defN 80-Jan-01 00:00 firefw-0.9.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      767 b- defN 80-Jan-01 00:00 firefw-0.9.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 firefw-0.9.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx      663 b- defN 16-Jan-01 00:00 firefw-0.9.8.dist-info/RECORD
+9 files, 33795 bytes uncompressed, 11315 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: firefw/runtime.py
 Comment: 
 
 Filename: firefw/tracing.py
 Comment: 
 
-Filename: firefw-0.9.7.dist-info/LICENSE.txt
+Filename: firefw-0.9.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: firefw-0.9.7.dist-info/METADATA
+Filename: firefw-0.9.8.dist-info/METADATA
 Comment: 
 
-Filename: firefw-0.9.7.dist-info/WHEEL
+Filename: firefw-0.9.8.dist-info/WHEEL
 Comment: 
 
-Filename: firefw-0.9.7.dist-info/RECORD
+Filename: firefw-0.9.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `firefw-0.9.7.dist-info/LICENSE.txt` & `firefw-0.9.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `firefw-0.9.7.dist-info/METADATA` & `firefw-0.9.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefw
-Version: 0.9.7
+Version: 0.9.8
 Summary: Frame for IR Runtime
 Author: FireDucks Development Team
 Author-email: fireducks@dtd.jp.nec.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

