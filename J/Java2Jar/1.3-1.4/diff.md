# Comparing `tmp/Java2Jar-1.3-py3-none-any.whl.zip` & `tmp/Java2Jar-1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,8 @@
-Zip file size: 3346 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      825 b- defN 24-Apr-02 12:03 Java2Jar/Main.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-02 12:12 Java2Jar/__init__.py
--rw-rw-rw-  2.0 fat      825 b- defN 24-Apr-02 12:03 Java2Jar-1.3.data/scripts/Main.py
--rw-rw-rw-  2.0 fat     1092 b- defN 24-Apr-02 12:28 Java2Jar-1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      780 b- defN 24-Apr-02 12:28 Java2Jar-1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 12:28 Java2Jar-1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-02 12:28 Java2Jar-1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      614 b- defN 24-Apr-02 12:28 Java2Jar-1.3.dist-info/RECORD
-8 files, 4237 bytes uncompressed, 2270 bytes compressed:  46.4%
+Zip file size: 2690 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      825 b- defN 24-Apr-02 12:03 Java2Jar-1.4.data/scripts/Main.py
+-rw-rw-rw-  2.0 fat     1092 b- defN 24-Apr-02 12:32 Java2Jar-1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      780 b- defN 24-Apr-02 12:32 Java2Jar-1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 12:32 Java2Jar-1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-02 12:32 Java2Jar-1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      468 b- defN 24-Apr-02 12:32 Java2Jar-1.4.dist-info/RECORD
+6 files, 3258 bytes uncompressed, 1838 bytes compressed:  43.6%
```

## zipnote {}

```diff
@@ -1,25 +1,19 @@
-Filename: Java2Jar/Main.py
+Filename: Java2Jar-1.4.data/scripts/Main.py
 Comment: 
 
-Filename: Java2Jar/__init__.py
+Filename: Java2Jar-1.4.dist-info/LICENSE
 Comment: 
 
-Filename: Java2Jar-1.3.data/scripts/Main.py
+Filename: Java2Jar-1.4.dist-info/METADATA
 Comment: 
 
-Filename: Java2Jar-1.3.dist-info/LICENSE
+Filename: Java2Jar-1.4.dist-info/WHEEL
 Comment: 
 
-Filename: Java2Jar-1.3.dist-info/METADATA
+Filename: Java2Jar-1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: Java2Jar-1.3.dist-info/WHEEL
-Comment: 
-
-Filename: Java2Jar-1.3.dist-info/top_level.txt
-Comment: 
-
-Filename: Java2Jar-1.3.dist-info/RECORD
+Filename: Java2Jar-1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `Java2Jar/Main.py` & `Java2Jar-1.4.data/scripts/Main.py`

 * *Files identical despite different names*

## Comparing `Java2Jar-1.3.dist-info/LICENSE` & `Java2Jar-1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Java2Jar-1.3.dist-info/METADATA` & `Java2Jar-1.4.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Java2Jar
-Version: 1.3
+Version: 1.4
 Summary: A tool to convert Java files to JAR files
 Author: Soumalya Das
 Author-email: soumalyagod21@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

