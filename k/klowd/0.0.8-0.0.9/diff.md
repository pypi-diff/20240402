# Comparing `tmp/klowd-0.0.8-py3-none-any.whl.zip` & `tmp/klowd-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2844 bytes, number of entries: 8
+Zip file size: 2890 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx       20 b- defN 24-Mar-06 21:09 klowd/__init__.py
 -rw-rw-r--  2.0 unx       63 b- defN 24-Mar-06 22:29 klowd/__version__.py
--rw-rw-r--  2.0 unx     1885 b- defN 24-Mar-07 11:58 klowd/core.py
--rw-rw-r--  2.0 unx      961 b- defN 24-Mar-07 12:00 klowd-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-07 12:00 klowd-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       39 b- defN 24-Mar-07 12:00 klowd-0.0.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 24-Mar-07 12:00 klowd-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      598 b- defN 24-Mar-07 12:00 klowd-0.0.8.dist-info/RECORD
-8 files, 3664 bytes uncompressed, 1798 bytes compressed:  50.9%
+-rw-rw-r--  2.0 unx     1938 b- defN 24-Mar-07 13:09 klowd/core.py
+-rw-rw-r--  2.0 unx      961 b- defN 24-Mar-07 13:09 klowd-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Mar-07 13:09 klowd-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       39 b- defN 24-Mar-07 13:09 klowd-0.0.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 24-Mar-07 13:09 klowd-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      598 b- defN 24-Mar-07 13:09 klowd-0.0.9.dist-info/RECORD
+8 files, 3717 bytes uncompressed, 1844 bytes compressed:  50.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: klowd/__version__.py
 Comment: 
 
 Filename: klowd/core.py
 Comment: 
 
-Filename: klowd-0.0.8.dist-info/METADATA
+Filename: klowd-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: klowd-0.0.8.dist-info/WHEEL
+Filename: klowd-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: klowd-0.0.8.dist-info/entry_points.txt
+Filename: klowd-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: klowd-0.0.8.dist-info/top_level.txt
+Filename: klowd-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: klowd-0.0.8.dist-info/RECORD
+Filename: klowd-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## klowd/core.py

```diff
@@ -1,7 +1,8 @@
+from typing import Any
 import anywidget
 import traitlets
 
 class GrantToken(anywidget.AnyWidget):
     _esm = """\
     function render({ model, el }) {
       const container = document.createElement("div");
@@ -49,14 +50,10 @@
             font-size: 20px;
             opacity: 0.8;
             padding: 10px 20px;
         }
     """
     value = traitlets.Unicode("").tag(sync=True)
 
-kloud_token = GrantToken()
-
-def setToken(event):
-    kloud_token.close()
-
-kloud_token.observe(setToken, 'value')
-kloud_token
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
+        self.observe(lambda e: self.close(), 'value')
```

## Comparing `klowd-0.0.8.dist-info/METADATA` & `klowd-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klowd
-Version: 0.0.8
+Version: 0.0.9
 Summary: KLOWD platform library
 Author: KLOWD
 Keywords: klowd,kloud
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `klowd-0.0.8.dist-info/RECORD` & `klowd-0.0.9.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 klowd/__init__.py,sha256=K0kNy26Vm6A-1V5lST3ily6yVsNLUbiqk6AZDFm2nJI,20
 klowd/__version__.py,sha256=UI4xhAWrh63iX8B8DrxAA-wZFvBpEpFRad-yVoqV4Po,63
-klowd/core.py,sha256=Pq5_XmPvElvutxrPKSVgy-PiKmJfQsp3s66nZLy7xrE,1885
-klowd-0.0.8.dist-info/METADATA,sha256=6gFSFV3PqYsITe9bUG07stqWZyue-sQPNizN03WDg7A,961
-klowd-0.0.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-klowd-0.0.8.dist-info/entry_points.txt,sha256=xPp6vFitqG85D-kOcIEWjIZmvD2l53YiMbrwjZFpjZw,39
-klowd-0.0.8.dist-info/top_level.txt,sha256=_Y-8NerF21pooJlxEVaB6Z5dEGr8m--py5eW0BhvOxU,6
-klowd-0.0.8.dist-info/RECORD,,
+klowd/core.py,sha256=LeATMBN4VzjnW7urBb0dFCPm9sOL463-1tuUKP0D-_8,1938
+klowd-0.0.9.dist-info/METADATA,sha256=2or6NLbsWV3CR90YQal6rUXA2QYDorpq1lSQyY7nKg4,961
+klowd-0.0.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+klowd-0.0.9.dist-info/entry_points.txt,sha256=xPp6vFitqG85D-kOcIEWjIZmvD2l53YiMbrwjZFpjZw,39
+klowd-0.0.9.dist-info/top_level.txt,sha256=_Y-8NerF21pooJlxEVaB6Z5dEGr8m--py5eW0BhvOxU,6
+klowd-0.0.9.dist-info/RECORD,,
```

