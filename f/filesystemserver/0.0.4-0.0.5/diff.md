# Comparing `tmp/filesystemserver-0.0.4-py3-none-any.whl.zip` & `tmp/filesystemserver-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12002 bytes, number of entries: 12
+Zip file size: 12020 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       82 b- defN 20-Feb-02 00:00 filesystemserver/__init__.py
--rw-r--r--  2.0 unx    11580 b- defN 20-Feb-02 00:00 filesystemserver/filesystemserver.py
+-rw-r--r--  2.0 unx    11673 b- defN 20-Feb-02 00:00 filesystemserver/filesystemserver.py
 -rw-r--r--  2.0 unx     2941 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/favicon.png
 -rw-r--r--  2.0 unx     1542 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/fss.js
 -rw-r--r--  2.0 unx     1811 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/browser/app.js
 -rw-r--r--  2.0 unx      353 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/browser/index.html
 -rw-r--r--  2.0 unx      472 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/browser/style.css
-?rw-r--r--  2.0 unx     2757 b- defN 20-Feb-02 00:00 filesystemserver-0.0.4.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 filesystemserver-0.0.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx       46 b- defN 20-Feb-02 00:00 filesystemserver-0.0.4.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1058 b- defN 20-Feb-02 00:00 filesystemserver-0.0.4.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1134 b- defN 20-Feb-02 00:00 filesystemserver-0.0.4.dist-info/RECORD
-12 files, 23863 bytes uncompressed, 10046 bytes compressed:  57.9%
+?rw-r--r--  2.0 unx     2757 b- defN 20-Feb-02 00:00 filesystemserver-0.0.5.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 filesystemserver-0.0.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx       46 b- defN 20-Feb-02 00:00 filesystemserver-0.0.5.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1058 b- defN 20-Feb-02 00:00 filesystemserver-0.0.5.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1134 b- defN 20-Feb-02 00:00 filesystemserver-0.0.5.dist-info/RECORD
+12 files, 23956 bytes uncompressed, 10064 bytes compressed:  58.0%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: filesystemserver/data/plugin/fss/browser/index.html
 Comment: 
 
 Filename: filesystemserver/data/plugin/fss/browser/style.css
 Comment: 
 
-Filename: filesystemserver-0.0.4.dist-info/METADATA
+Filename: filesystemserver-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: filesystemserver-0.0.4.dist-info/WHEEL
+Filename: filesystemserver-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: filesystemserver-0.0.4.dist-info/entry_points.txt
+Filename: filesystemserver-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: filesystemserver-0.0.4.dist-info/licenses/LICENSE
+Filename: filesystemserver-0.0.5.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: filesystemserver-0.0.4.dist-info/RECORD
+Filename: filesystemserver-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filesystemserver/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .filesystemserver import install, update, serve, main
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

## filesystemserver/filesystemserver.py

```diff
@@ -17,15 +17,19 @@
 ) < (3, 11):
     import tomli as toml
 else:
     import tomllib as toml
 
 
 def resolve_git_repo(url):
-    if not url.startswith("http"):
+    if (
+        not url.startswith("http")
+        and not url.startswith("ssh")
+        and not url.startswith("git@")
+    ):
         url = f"https://github.com/{url}"
     plugin_dir = "/".join(url.split("/")[-2:])
     return url, plugin_dir
 
 
 def installed_plugins(plugin_dir):
     index = "index.html"
```

## Comparing `filesystemserver-0.0.4.dist-info/METADATA` & `filesystemserver-0.0.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: filesystemserver
-Version: 0.0.4
+Version: 0.0.5
 Summary: File System Server
 Project-URL: Homepage, https://github.com/nicholashaydensmith/filesystemserver
 Project-URL: Issues, https://github.com/nicholashaydensmith/filesystemserver/issues
 Author-email: Nicholas Smith <thesmithdynasty@gmail.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `filesystemserver-0.0.4.dist-info/licenses/LICENSE` & `filesystemserver-0.0.5.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `filesystemserver-0.0.4.dist-info/RECORD` & `filesystemserver-0.0.5.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-filesystemserver/__init__.py,sha256=4caxBttXKxnasLQn6PrjHt3TNoSTkRx_74LiJD09Bmc,82
-filesystemserver/filesystemserver.py,sha256=vlBH6umsTU2ps3CqmgFUH6-7DIJrsJg5BRBp52OrHTw,11580
+filesystemserver/__init__.py,sha256=stMXE3Lde2NzKNP0-S8A7l4BaloJdTITQNL8tmCEi0w,82
+filesystemserver/filesystemserver.py,sha256=dsWeHS-arPfijOreWyiIYl0B0fm3rrXMxY3oRyFN4aM,11673
 filesystemserver/data/plugin/fss/favicon.png,sha256=jfu_rDdgAb0ulGnX9TxdM1vj4f0ZpRkEE0DpB1I4cNM,2941
 filesystemserver/data/plugin/fss/fss.js,sha256=gHeQgbKESwUWWLXUpke2xmOY89QR5waOCtkSKV-8L2U,1542
 filesystemserver/data/plugin/fss/browser/app.js,sha256=DtxRIt8wm_RskX-LZWQJiroBUK7AIXqIy34EVaHUtvA,1811
 filesystemserver/data/plugin/fss/browser/index.html,sha256=aU5EcD4xZ_UrEWLXPmHMYDe86Tyu7V7B6vB0qjJ8sdY,353
 filesystemserver/data/plugin/fss/browser/style.css,sha256=8VNeUDCQV5APkjShPTa3vAWKAu-uPkoTXxvWygh_D70,472
-filesystemserver-0.0.4.dist-info/METADATA,sha256=RdgT2PJO5i3gspuS7nJHMB0n1ZOU75E3zmTCbEo09m0,2757
-filesystemserver-0.0.4.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
-filesystemserver-0.0.4.dist-info/entry_points.txt,sha256=v8bckKCYnwAeArNNyRB1mYpv_LCSZHDKQDWPypN0tf8,46
-filesystemserver-0.0.4.dist-info/licenses/LICENSE,sha256=Ks3vDJNeEsRGdqidSQvxrke32irrL4Xez7qVE4DBEik,1058
-filesystemserver-0.0.4.dist-info/RECORD,,
+filesystemserver-0.0.5.dist-info/METADATA,sha256=9bCFuJL40Hp34U9l2M7FQrbr9uVesxRqn5G-m6v02CM,2757
+filesystemserver-0.0.5.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
+filesystemserver-0.0.5.dist-info/entry_points.txt,sha256=v8bckKCYnwAeArNNyRB1mYpv_LCSZHDKQDWPypN0tf8,46
+filesystemserver-0.0.5.dist-info/licenses/LICENSE,sha256=Ks3vDJNeEsRGdqidSQvxrke32irrL4Xez7qVE4DBEik,1058
+filesystemserver-0.0.5.dist-info/RECORD,,
```

