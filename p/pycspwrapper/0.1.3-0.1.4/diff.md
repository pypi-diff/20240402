# Comparing `tmp/pycspwrapper-0.1.3-py3-none-any.whl.zip` & `tmp/pycspwrapper-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3994 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     3207 b- defN 24-Mar-21 11:16 pycspwrapper/LVStat.py
+Zip file size: 4006 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     3352 b- defN 24-Apr-02 14:56 pycspwrapper/LVStat.py
 -rw-rw-r--  2.0 unx       74 b- defN 24-Mar-21 09:50 pycspwrapper/__init__.py
--rw-rw-r--  2.0 unx     1075 b- defN 24-Mar-21 11:19 pycspwrapper-0.1.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1645 b- defN 24-Mar-21 11:19 pycspwrapper-0.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-21 11:19 pycspwrapper-0.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 24-Mar-21 11:19 pycspwrapper-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      569 b- defN 24-Mar-21 11:19 pycspwrapper-0.1.3.dist-info/RECORD
-7 files, 6675 bytes uncompressed, 2980 bytes compressed:  55.4%
+-rw-rw-r--  2.0 unx     1075 b- defN 24-Apr-02 15:16 pycspwrapper-0.1.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1595 b- defN 24-Apr-02 15:16 pycspwrapper-0.1.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-02 15:16 pycspwrapper-0.1.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       13 b- defN 24-Apr-02 15:16 pycspwrapper-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      569 b- defN 24-Apr-02 15:16 pycspwrapper-0.1.4.dist-info/RECORD
+7 files, 6770 bytes uncompressed, 2992 bytes compressed:  55.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pycspwrapper/LVStat.py
 Comment: 
 
 Filename: pycspwrapper/__init__.py
 Comment: 
 
-Filename: pycspwrapper-0.1.3.dist-info/LICENSE
+Filename: pycspwrapper-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: pycspwrapper-0.1.3.dist-info/METADATA
+Filename: pycspwrapper-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: pycspwrapper-0.1.3.dist-info/WHEEL
+Filename: pycspwrapper-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: pycspwrapper-0.1.3.dist-info/top_level.txt
+Filename: pycspwrapper-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pycspwrapper-0.1.3.dist-info/RECORD
+Filename: pycspwrapper-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pycspwrapper/LVStat.py

```diff
@@ -6,27 +6,32 @@
     def __init__(self, lang, *args):
         self.ids = list(args)
         self.url = 'https://data.stat.gov.lv/api/v1/{}/OSP_PUB/'.format(lang)
         self.url_out = 'https://data.stat.gov.lv/pxweb/{}/OSP_PUB/START__'.format(lang)
         self.query = {"query": [], 
                       "response": {"format": "json"}
                       }
+        self._info = None
 
     def info(self):
         """ Returns the metadata associated with the current folder. """
-        response = session.get(self.url + '/'.join(self.ids))
-        return response.json()
+        if not self._info:
+            response = session.get(self.url + '/'.join(self.ids))
+            self._info = response.json()
+        return self._info
 
     def go_down(self, *args):
         """ Goes deeper in the hierarchical metadata structure. """
         self.ids += list(args)
+        self._info = None
 
     def go_up(self, k=1):
         """ Goes k levels up in the hierarchical metadata structure. """
         self.ids = self.ids[:-k]
+        self._info = None
 
     def get_url(self):
         """ Returns the url to the current folder. """
         if len(self.ids[-1]) >= 3:
             try:
                 int(self.ids[-1][3])
             except ValueError:
```

## Comparing `pycspwrapper-0.1.3.dist-info/LICENSE` & `pycspwrapper-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pycspwrapper-0.1.3.dist-info/METADATA` & `pycspwrapper-0.1.4.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycspwrapper
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python wrapper for Latvian official statistics portal API: https://stat.gov.lv/en/api-and-code-list-registry.
 Home-page: https://github.com/vf42/pycspwrapper
 Author: Vadim Fedorov
 Author-email: vadim@vf42.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,15 +27,15 @@
 ```
 
 To import: 
 ```python
 from pycspwrapper import LVStat
 ```
 
-For info on usage, see the included notebooks. TODO: Update the notebooks for the Latvian stats.
+For info on usage, see the included notebooks.
 
 ## Changelog
 
 News in version 0.1.3:
 Updated query generation code to use variable and value codes instead of text values.
 
 News in version 0.1.2:
```

## Comparing `pycspwrapper-0.1.3.dist-info/RECORD` & `pycspwrapper-0.1.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-pycspwrapper/LVStat.py,sha256=9fEc-oKmjTfZagGXHG886YEtHDWGbfK1bYYCM5Pc2ZE,3207
+pycspwrapper/LVStat.py,sha256=cDEbRHySxjysygOt7yJEe6ZYbxUZnRFKhZlOmG0vXA8,3352
 pycspwrapper/__init__.py,sha256=jCTs9WKyHVKczEosY0ByeLNC8ce0xPFMlP547d-pvdc,74
-pycspwrapper-0.1.3.dist-info/LICENSE,sha256=63oS5eWBoaAGaCBZGLXIt416uVOwCJP_bWByadRxGR8,1075
-pycspwrapper-0.1.3.dist-info/METADATA,sha256=7Whe7F-pCOWvR1eQgiwuM4JznlfrR4ZYDuK0kRvhig8,1645
-pycspwrapper-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pycspwrapper-0.1.3.dist-info/top_level.txt,sha256=nxUNjbb0Hnxi2eo94ZyHX2qyYvnZa_RenKjZGhF8kIs,13
-pycspwrapper-0.1.3.dist-info/RECORD,,
+pycspwrapper-0.1.4.dist-info/LICENSE,sha256=63oS5eWBoaAGaCBZGLXIt416uVOwCJP_bWByadRxGR8,1075
+pycspwrapper-0.1.4.dist-info/METADATA,sha256=phws3O8eX97Z9IYaslNVW2zAleCEZSz90GQ_NwR6L_Q,1595
+pycspwrapper-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pycspwrapper-0.1.4.dist-info/top_level.txt,sha256=nxUNjbb0Hnxi2eo94ZyHX2qyYvnZa_RenKjZGhF8kIs,13
+pycspwrapper-0.1.4.dist-info/RECORD,,
```

