# Comparing `tmp/petrosa-0.0.7-py3-none-any.whl.zip` & `tmp/petrosa-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5396 bytes, number of entries: 9
+Zip file size: 5398 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 petrosa/converters/__init__.py
 -rw-r--r--  2.0 unx     2322 b- defN 20-Feb-02 00:00 petrosa/converters/backtests.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 petrosa/ta/__init__.py
 -rw-r--r--  2.0 unx    22023 b- defN 20-Feb-02 00:00 petrosa/ta/strategies.py
 -rw-r--r--  2.0 unx      822 b- defN 20-Feb-02 00:00 petrosa/ta/utils.py
-?rw-r--r--  2.0 unx      716 b- defN 20-Feb-02 00:00 petrosa-0.0.7.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 petrosa-0.0.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1063 b- defN 20-Feb-02 00:00 petrosa-0.0.7.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      707 b- defN 20-Feb-02 00:00 petrosa-0.0.7.dist-info/RECORD
-9 files, 27740 bytes uncompressed, 4176 bytes compressed:  84.9%
+?rw-r--r--  2.0 unx      716 b- defN 20-Feb-02 00:00 petrosa-0.0.8.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 petrosa-0.0.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1063 b- defN 20-Feb-02 00:00 petrosa-0.0.8.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      707 b- defN 20-Feb-02 00:00 petrosa-0.0.8.dist-info/RECORD
+9 files, 27740 bytes uncompressed, 4178 bytes compressed:  84.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: petrosa/ta/strategies.py
 Comment: 
 
 Filename: petrosa/ta/utils.py
 Comment: 
 
-Filename: petrosa-0.0.7.dist-info/METADATA
+Filename: petrosa-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: petrosa-0.0.7.dist-info/WHEEL
+Filename: petrosa-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: petrosa-0.0.7.dist-info/licenses/LICENSE
+Filename: petrosa-0.0.8.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: petrosa-0.0.7.dist-info/RECORD
+Filename: petrosa-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `petrosa-0.0.7.dist-info/METADATA` & `petrosa-0.0.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petrosa
-Version: 0.0.7
+Version: 0.0.8
 Summary: utilities for PETROSA
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: "@yurisa2" <yuri@sa2.com.br>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `petrosa-0.0.7.dist-info/licenses/LICENSE` & `petrosa-0.0.8.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `petrosa-0.0.7.dist-info/RECORD` & `petrosa-0.0.8.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 petrosa/converters/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 petrosa/converters/backtests.py,sha256=n5f6yrZstX5aOsgcGj2gl4P1hMaaoijV5NPnF2j_KeI,2322
 petrosa/ta/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 petrosa/ta/strategies.py,sha256=W_x2vxE891pOHLGKKtSRohCDWifIa70pALXevToIPSc,22023
 petrosa/ta/utils.py,sha256=77IZzQVRMw1MPwYw-MTWv-CXhtbdtppzXEzxcgvGXAw,822
-petrosa-0.0.7.dist-info/METADATA,sha256=8eifqjRo7-hP8-qLCc3lWsA9K1ohSMhNU3ao28b1cNI,716
-petrosa-0.0.7.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-petrosa-0.0.7.dist-info/licenses/LICENSE,sha256=laAtIGoDbZBqhkTalLLdtCwZumW9xZhoDe9AvKKviQk,1063
-petrosa-0.0.7.dist-info/RECORD,,
+petrosa-0.0.8.dist-info/METADATA,sha256=HUOPxDhWl-07IVDG3_R0NxdEmnuyBkV8eLecc3_oieE,716
+petrosa-0.0.8.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+petrosa-0.0.8.dist-info/licenses/LICENSE,sha256=laAtIGoDbZBqhkTalLLdtCwZumW9xZhoDe9AvKKviQk,1063
+petrosa-0.0.8.dist-info/RECORD,,
```

