# Comparing `tmp/filesystemserver-0.0.1-py3-none-any.whl.zip` & `tmp/filesystemserver-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8599 bytes, number of entries: 10
+Zip file size: 8619 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       82 b- defN 20-Feb-02 00:00 filesystemserver/__init__.py
 -rw-r--r--  2.0 unx    10465 b- defN 20-Feb-02 00:00 filesystemserver/filesystemserver.py
--rw-r--r--  2.0 unx     1024 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/fss.js
+-rw-r--r--  2.0 unx     1077 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/fss.js
 -rw-r--r--  2.0 unx     1736 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/browser/app.js
 -rw-r--r--  2.0 unx      814 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/browser/index.html
-?rw-r--r--  2.0 unx     2318 b- defN 20-Feb-02 00:00 filesystemserver-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 filesystemserver-0.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx       46 b- defN 20-Feb-02 00:00 filesystemserver-0.0.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1058 b- defN 20-Feb-02 00:00 filesystemserver-0.0.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      927 b- defN 20-Feb-02 00:00 filesystemserver-0.0.1.dist-info/RECORD
-10 files, 18557 bytes uncompressed, 6983 bytes compressed:  62.4%
+?rw-r--r--  2.0 unx     2318 b- defN 20-Feb-02 00:00 filesystemserver-0.0.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 filesystemserver-0.0.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx       46 b- defN 20-Feb-02 00:00 filesystemserver-0.0.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1058 b- defN 20-Feb-02 00:00 filesystemserver-0.0.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      927 b- defN 20-Feb-02 00:00 filesystemserver-0.0.2.dist-info/RECORD
+10 files, 18610 bytes uncompressed, 7003 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: filesystemserver/data/plugin/fss/browser/app.js
 Comment: 
 
 Filename: filesystemserver/data/plugin/fss/browser/index.html
 Comment: 
 
-Filename: filesystemserver-0.0.1.dist-info/METADATA
+Filename: filesystemserver-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: filesystemserver-0.0.1.dist-info/WHEEL
+Filename: filesystemserver-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: filesystemserver-0.0.1.dist-info/entry_points.txt
+Filename: filesystemserver-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: filesystemserver-0.0.1.dist-info/licenses/LICENSE
+Filename: filesystemserver-0.0.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: filesystemserver-0.0.1.dist-info/RECORD
+Filename: filesystemserver-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filesystemserver/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .filesystemserver import install, update, serve, main
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

## filesystemserver/data/plugin/fss/fss.js

### js-beautify {}

```diff
@@ -28,13 +28,14 @@
     query: (callback, queries = ["cwd", "list", "plugins"]) => {
         query = queries.map(q => `query=${q}`).join("&");
         fetch_json(`?${query}`)
             .then(callback)
             .catch(error_handler);
     },
 
-    download: (url, callback, kind = "text") => {
-        fetch_text(`?download=${url}`)
+    download: (url, callback) => {
+        const fetch_fn = url.endsWith(".json") ? fetch_json : fetch_text;
+        fetch_fn(`?download=${url}`)
             .then(callback)
             .catch(error_handler);
     },
 }
```

## Comparing `filesystemserver-0.0.1.dist-info/METADATA` & `filesystemserver-0.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: filesystemserver
-Version: 0.0.1
+Version: 0.0.2
 Summary: File System Server
 Project-URL: Homepage, https://github.com/nicholashaydensmith/filesystemserver
 Project-URL: Issues, https://github.com/nicholashaydensmith/filesystemserver/issues
 Author-email: Nicholas Smith <thesmithdynasty@gmail.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `filesystemserver-0.0.1.dist-info/licenses/LICENSE` & `filesystemserver-0.0.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

