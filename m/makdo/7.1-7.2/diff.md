# Comparing `tmp/makdo-7.1.tar.gz` & `tmp/makdo-7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makdo-7.1.tar", last modified: Mon Apr  1 18:32:34 2024, max compression
+gzip compressed data, was "makdo-7.2.tar", last modified: Mon Apr  1 19:11:36 2024, max compression
```

## Comparing `makdo-7.1.tar` & `makdo-7.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 say       (1000) say       (1000)        0 2024-04-01 18:32:34.030760 makdo-7.1/
--rw-------   0 say       (1000) say       (1000)    21832 2024-04-01 18:32:34.030760 makdo-7.1/PKG-INFO
--rw-------   0 say       (1000) say       (1000)    17888 2024-04-01 18:32:06.000000 makdo-7.1/README.txt
-drwx------   0 say       (1000) say       (1000)        0 2024-04-01 18:32:34.030760 makdo-7.1/makdo/
--rw-------   0 say       (1000) say       (1000)      137 2024-04-01 18:32:06.000000 makdo-7.1/makdo/__init__.py
--rwx------   0 say       (1000) say       (1000)   262576 2024-04-01 18:32:06.000000 makdo-7.1/makdo/makdo_docx2md.py
--rwx------   0 say       (1000) say       (1000)     4000 2024-04-01 18:32:06.000000 makdo-7.1/makdo/makdo_gui.py
--rwx------   0 say       (1000) say       (1000)   237782 2024-04-01 18:32:06.000000 makdo-7.1/makdo/makdo_md2docx.py
-drwx------   0 say       (1000) say       (1000)        0 2024-04-01 18:32:34.030760 makdo-7.1/makdo.egg-info/
--rw-------   0 say       (1000) say       (1000)    21832 2024-04-01 18:32:33.000000 makdo-7.1/makdo.egg-info/PKG-INFO
--rw-------   0 say       (1000) say       (1000)      246 2024-04-01 18:32:34.000000 makdo-7.1/makdo.egg-info/SOURCES.txt
--rw-------   0 say       (1000) say       (1000)        1 2024-04-01 18:32:33.000000 makdo-7.1/makdo.egg-info/dependency_links.txt
--rw-------   0 say       (1000) say       (1000)       32 2024-04-01 18:32:33.000000 makdo-7.1/makdo.egg-info/requires.txt
--rw-------   0 say       (1000) say       (1000)        6 2024-04-01 18:32:33.000000 makdo-7.1/makdo.egg-info/top_level.txt
--rw-------   0 say       (1000) say       (1000)       38 2024-04-01 18:32:34.030760 makdo-7.1/setup.cfg
--rw-------   0 say       (1000) say       (1000)      567 2024-04-01 18:32:06.000000 makdo-7.1/setup.py
+drwx------   0 say       (1000) say       (1000)        0 2024-04-01 19:11:36.179847 makdo-7.2/
+-rw-------   0 say       (1000) say       (1000)    21832 2024-04-01 19:11:36.179847 makdo-7.2/PKG-INFO
+-rw-------   0 say       (1000) say       (1000)    17888 2024-04-01 19:11:26.000000 makdo-7.2/README.txt
+drwx------   0 say       (1000) say       (1000)        0 2024-04-01 19:11:36.175847 makdo-7.2/makdo/
+-rw-------   0 say       (1000) say       (1000)      137 2024-04-01 19:11:26.000000 makdo-7.2/makdo/__init__.py
+-rwx------   0 say       (1000) say       (1000)   262576 2024-04-01 19:11:26.000000 makdo-7.2/makdo/makdo_docx2md.py
+-rwx------   0 say       (1000) say       (1000)     4054 2024-04-01 19:11:26.000000 makdo-7.2/makdo/makdo_gui.py
+-rwx------   0 say       (1000) say       (1000)   237782 2024-04-01 19:11:26.000000 makdo-7.2/makdo/makdo_md2docx.py
+drwx------   0 say       (1000) say       (1000)        0 2024-04-01 19:11:36.179847 makdo-7.2/makdo.egg-info/
+-rw-------   0 say       (1000) say       (1000)    21832 2024-04-01 19:11:36.000000 makdo-7.2/makdo.egg-info/PKG-INFO
+-rw-------   0 say       (1000) say       (1000)      246 2024-04-01 19:11:36.000000 makdo-7.2/makdo.egg-info/SOURCES.txt
+-rw-------   0 say       (1000) say       (1000)        1 2024-04-01 19:11:36.000000 makdo-7.2/makdo.egg-info/dependency_links.txt
+-rw-------   0 say       (1000) say       (1000)       32 2024-04-01 19:11:36.000000 makdo-7.2/makdo.egg-info/requires.txt
+-rw-------   0 say       (1000) say       (1000)        6 2024-04-01 19:11:36.000000 makdo-7.2/makdo.egg-info/top_level.txt
+-rw-------   0 say       (1000) say       (1000)       38 2024-04-01 19:11:36.179847 makdo-7.2/setup.cfg
+-rw-------   0 say       (1000) say       (1000)      567 2024-04-01 19:11:26.000000 makdo-7.2/setup.py
```

### Comparing `makdo-7.1/PKG-INFO` & `makdo-7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makdo
-Version: 7.1
+Version: 7.2
 Summary: 日本の公用文書（司法文書、行政文書）をMarkdown形式とMicrosoft Word形式との間で変換します
 Home-page: https://github.com/hata48915b/makdo/
 Author: Seiichiro HATA
 Author-email: hata48915b@post.nifty.jp
 License: GPLv3+
 Description: <!-- Time-stamp:   <2024.04.02-01:49:42-JST> -->
```

### Comparing `makdo-7.1/README.txt` & `makdo-7.2/README.txt`

 * *Files identical despite different names*

### Comparing `makdo-7.1/makdo/makdo_docx2md.py` & `makdo-7.2/makdo/makdo_docx2md.py`

 * *Files identical despite different names*

### Comparing `makdo-7.1/makdo/makdo_gui.py` & `makdo-7.2/makdo/makdo_gui.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 # Name:         makdo-gui.py
 # Version:      v07 Furuichibashi
-# Time-stamp:   <2024.04.02-03:25:09-JST>
+# Time-stamp:   <2024.04.02-04:09:36-JST>
 
 # makdo-gui.py
 # Copyright (C) 2022-2024  Seiichiro HATA
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -43,16 +43,17 @@
 import tempfile
 from makdo.makdo_md2docx import Md2Docx
 from makdo.makdo_docx2md import Docx2Md
 
 
 __version__ = 'v07 Furuichibashi'
 
+VERSION = 'v07.02'
 
-WINDOW_SIZE = "552x276"
+WINDOW_SIZE = "601x276"
 
 
 class Makdo:
 
     receipt_number = 0
 
     def __init__(self):
@@ -90,19 +91,20 @@
             else:
                 textarea.insert('end', '不適切なファイルです\n')
             sys.stderr = stderr
             textarea.insert('end', '\nここにmdファイル又はdocxファイルをドロップしてください\n')
 
         win = TkinterDnD.Tk()
         win.geometry(WINDOW_SIZE)
-        win.title("MAKDO（mdファイルをdocxファイルに、docxファイルをmdファイルに変換します）")
+        win.title("MAKDO " + VERSION
+                  + " （mdファイルをdocxファイルに、docxファイルをmdファイルに変換します）")
 
         frame = ttk.Frame(win)
-        textarea = tk.Text(frame, width=111, height=30)
-        # textarea = tk.Text(frame, width=74, height=20)
+        textarea = tk.Text(frame, width=120, height=30)
+        # textarea = tk.Text(frame, width=80, height=20)
         textarea.drop_target_register(DND_FILES)
         textarea.insert('end', 'ここにmdファイル又はdocxファイルをドロップしてください\n')
         textarea.dnd_bind('<<Drop>>', drop)
 
         frame.pack(expand=True, fill=tk.X, padx=16, pady=8)
         textarea.pack(side=tk.LEFT)
```

### Comparing `makdo-7.1/makdo/makdo_md2docx.py` & `makdo-7.2/makdo/makdo_md2docx.py`

 * *Files identical despite different names*

### Comparing `makdo-7.1/makdo.egg-info/PKG-INFO` & `makdo-7.2/makdo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makdo
-Version: 7.1
+Version: 7.2
 Summary: 日本の公用文書（司法文書、行政文書）をMarkdown形式とMicrosoft Word形式との間で変換します
 Home-page: https://github.com/hata48915b/makdo/
 Author: Seiichiro HATA
 Author-email: hata48915b@post.nifty.jp
 License: GPLv3+
 Description: <!-- Time-stamp:   <2024.04.02-01:49:42-JST> -->
```

### Comparing `makdo-7.1/setup.py` & `makdo-7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='makdo',
-    version='07.01',
+    version='07.02',
     description='日本の公用文書（司法文書、行政文書）をMarkdown形式とMicrosoft Word形式との間で変換します',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Seiichiro HATA',
     author_email='hata48915b@post.nifty.jp',
     url='https://github.com/hata48915b/makdo/',
     license='GPLv3+',
```

