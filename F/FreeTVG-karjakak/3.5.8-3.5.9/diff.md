# Comparing `tmp/FreeTVG-karjakak-3.5.8.tar.gz` & `tmp/FreeTVG-karjakak-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeTVG-karjakak-3.5.8.tar", last modified: Sat Mar  2 11:02:43 2024, max compression
+gzip compressed data, was "FreeTVG-karjakak-3.5.9.tar", last modified: Mon Mar  4 08:54:03 2024, max compression
```

## Comparing `FreeTVG-karjakak-3.5.8.tar` & `FreeTVG-karjakak-3.5.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-03-02 11:02:43.604462 FreeTVG-karjakak-3.5.8/
-drwxrwxrwx   0        0        0        0 2024-03-02 11:02:43.603124 FreeTVG-karjakak-3.5.8/FreeTVG_karjakak.egg-info/
--rw-rw-rw-   0        0        0    17683 2024-03-02 11:02:43.000000 FreeTVG-karjakak-3.5.8/FreeTVG_karjakak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      638 2024-03-02 11:02:43.000000 FreeTVG-karjakak-3.5.8/FreeTVG_karjakak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-02 11:02:43.000000 FreeTVG-karjakak-3.5.8/FreeTVG_karjakak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-03-02 11:02:43.000000 FreeTVG-karjakak-3.5.8/FreeTVG_karjakak.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      210 2024-03-02 11:02:43.000000 FreeTVG-karjakak-3.5.8/FreeTVG_karjakak.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-03-02 11:02:43.000000 FreeTVG-karjakak-3.5.8/FreeTVG_karjakak.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.8/LICENSE
--rw-rw-rw-   0        0        0    17683 2024-03-02 11:02:43.604462 FreeTVG-karjakak-3.5.8/PKG-INFO
--rw-rw-rw-   0        0        0    16656 2024-02-29 10:28:44.000000 FreeTVG-karjakak-3.5.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-02 11:02:43.579185 FreeTVG-karjakak-3.5.8/TVG/
--rw-rw-rw-   0        0        0   155208 2024-03-01 04:53:26.000000 FreeTVG-karjakak-3.5.8/TVG/FreeTVG.py
--rw-rw-rw-   0        0        0   384401 2024-03-01 05:50:24.000000 FreeTVG-karjakak-3.5.8/TVG/Tutorial TVG.pdf
--rw-rw-rw-   0        0        0       49 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.8/TVG/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-02 11:02:43.583545 FreeTVG-karjakak-3.5.8/TVG/bible_reader/
-drwxrwxrwx   0        0        0        0 2024-03-02 11:02:43.584740 FreeTVG-karjakak-3.5.8/TVG/bible_reader/.Bible/
--rw-rw-rw-   0        0        0  5214233 2023-11-24 12:25:30.000000 FreeTVG-karjakak-3.5.8/TVG/bible_reader/.Bible/KJV.xml
--rw-rw-rw-   0        0        0       68 2023-11-24 12:25:30.000000 FreeTVG-karjakak-3.5.8/TVG/bible_reader/__init__.py
--rw-rw-rw-   0        0        0     5559 2023-11-24 12:25:30.000000 FreeTVG-karjakak-3.5.8/TVG/bible_reader/bible_creator.py
--rw-rw-rw-   0        0        0     9830 2024-03-01 05:02:19.000000 FreeTVG-karjakak-3.5.8/TVG/bible_reader/layout_BR.py
-drwxrwxrwx   0        0        0        0 2024-03-02 11:02:43.592573 FreeTVG-karjakak-3.5.8/TVG/structure/
--rw-rw-rw-   0        0        0      101 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.8/TVG/structure/__init__.py
--rw-rw-rw-   0        0        0    27554 2024-03-02 10:38:49.000000 FreeTVG-karjakak-3.5.8/TVG/structure/frame_layouts.py
-drwxrwxrwx   0        0        0        0 2024-03-02 11:02:43.602099 FreeTVG-karjakak-3.5.8/TVG/utility/
--rw-rw-rw-   0        0        0      925 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.8/TVG/utility/RegMail.py
--rw-rw-rw-   0        0        0      162 2023-11-14 18:21:31.000000 FreeTVG-karjakak-3.5.8/TVG/utility/__init__.py
--rw-rw-rw-   0        0        0     8471 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.8/TVG/utility/data_parse.py
--rw-rw-rw-   0        0        0     3796 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.8/TVG/utility/database_tvg.py
--rw-rw-rw-   0        0        0     7742 2024-03-01 06:00:23.000000 FreeTVG-karjakak-3.5.8/TVG/utility/mdh.py
--rw-rw-rw-   0        0        0      108 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.8/pyproject.toml
--rw-rw-rw-   0        0        0     1103 2024-03-02 11:02:43.604462 FreeTVG-karjakak-3.5.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-04 08:54:03.182963 FreeTVG-karjakak-3.5.9/
+drwxrwxrwx   0        0        0        0 2024-03-04 08:54:03.181952 FreeTVG-karjakak-3.5.9/FreeTVG_karjakak.egg-info/
+-rw-rw-rw-   0        0        0    17941 2024-03-04 08:54:03.000000 FreeTVG-karjakak-3.5.9/FreeTVG_karjakak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2024-03-04 08:54:03.000000 FreeTVG-karjakak-3.5.9/FreeTVG_karjakak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-04 08:54:03.000000 FreeTVG-karjakak-3.5.9/FreeTVG_karjakak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-03-04 08:54:03.000000 FreeTVG-karjakak-3.5.9/FreeTVG_karjakak.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      210 2024-03-04 08:54:03.000000 FreeTVG-karjakak-3.5.9/FreeTVG_karjakak.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-03-04 08:54:03.000000 FreeTVG-karjakak-3.5.9/FreeTVG_karjakak.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.9/LICENSE
+-rw-rw-rw-   0        0        0    17941 2024-03-04 08:54:03.182963 FreeTVG-karjakak-3.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0    16914 2024-03-02 11:25:31.000000 FreeTVG-karjakak-3.5.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-04 08:54:03.158412 FreeTVG-karjakak-3.5.9/TVG/
+-rw-rw-rw-   0        0        0   155142 2024-03-04 07:28:48.000000 FreeTVG-karjakak-3.5.9/TVG/FreeTVG.py
+-rw-rw-rw-   0        0        0   384401 2024-03-01 05:50:24.000000 FreeTVG-karjakak-3.5.9/TVG/Tutorial TVG.pdf
+-rw-rw-rw-   0        0        0       49 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.9/TVG/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-04 08:54:03.162809 FreeTVG-karjakak-3.5.9/TVG/bible_reader/
+drwxrwxrwx   0        0        0        0 2024-03-04 08:54:03.163819 FreeTVG-karjakak-3.5.9/TVG/bible_reader/.Bible/
+-rw-rw-rw-   0        0        0  5214233 2023-11-24 12:25:30.000000 FreeTVG-karjakak-3.5.9/TVG/bible_reader/.Bible/KJV.xml
+-rw-rw-rw-   0        0        0       68 2023-11-24 12:25:30.000000 FreeTVG-karjakak-3.5.9/TVG/bible_reader/__init__.py
+-rw-rw-rw-   0        0        0     5559 2023-11-24 12:25:30.000000 FreeTVG-karjakak-3.5.9/TVG/bible_reader/bible_creator.py
+-rw-rw-rw-   0        0        0     9830 2024-03-01 05:02:19.000000 FreeTVG-karjakak-3.5.9/TVG/bible_reader/layout_BR.py
+drwxrwxrwx   0        0        0        0 2024-03-04 08:54:03.174566 FreeTVG-karjakak-3.5.9/TVG/structure/
+-rw-rw-rw-   0        0        0      101 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.9/TVG/structure/__init__.py
+-rw-rw-rw-   0        0        0    27554 2024-03-02 10:38:49.000000 FreeTVG-karjakak-3.5.9/TVG/structure/frame_layouts.py
+drwxrwxrwx   0        0        0        0 2024-03-04 08:54:03.179480 FreeTVG-karjakak-3.5.9/TVG/utility/
+-rw-rw-rw-   0        0        0      925 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.9/TVG/utility/RegMail.py
+-rw-rw-rw-   0        0        0      162 2023-11-14 18:21:31.000000 FreeTVG-karjakak-3.5.9/TVG/utility/__init__.py
+-rw-rw-rw-   0        0        0     8471 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.9/TVG/utility/data_parse.py
+-rw-rw-rw-   0        0        0     3796 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.9/TVG/utility/database_tvg.py
+-rw-rw-rw-   0        0        0     7742 2024-03-01 06:00:23.000000 FreeTVG-karjakak-3.5.9/TVG/utility/mdh.py
+-rw-rw-rw-   0        0        0      108 2023-11-14 18:07:57.000000 FreeTVG-karjakak-3.5.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1103 2024-03-04 08:54:03.183991 FreeTVG-karjakak-3.5.9/setup.cfg
```

### Comparing `FreeTVG-karjakak-3.5.8/FreeTVG_karjakak.egg-info/PKG-INFO` & `FreeTVG-karjakak-3.5.9/FreeTVG_karjakak.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.5.8
+Version: 3.5.9
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
@@ -488,14 +488,21 @@
     * **The layout for writing entry appearance has been fixed for Windows and MacOS as well**
   * **Version 3.5.5**
     * **Direct PDF creation for Windows**
       * **[Direct Print PDF](#direct-print-pdf)**
   * **Version 3.5.6**
     * **Markdown marking highlight stay yellow and font color turn to black**
     * **Infor-Bar font smaller in Windows**
+  * **Version 3.5.8**
+    * **Fix bugs for previous version**
+    * **Some tweak on appearance in Windows**
+      * **Font look smaller on Buttons**
+      * **Font look smaller on Bible**
+      * **Font look smaller on info-bar**
+      * **others..**
 
 [⬆️](#freetvg-tree-view-gui)
 
 ## TVG
 
 ![TVG](Pics/TVG.png)
```

### Comparing `FreeTVG-karjakak-3.5.8/FreeTVG_karjakak.egg-info/SOURCES.txt` & `FreeTVG-karjakak-3.5.9/FreeTVG_karjakak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.5.8/LICENSE` & `FreeTVG-karjakak-3.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.5.8/PKG-INFO` & `FreeTVG-karjakak-3.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.5.8
+Version: 3.5.9
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
@@ -488,14 +488,21 @@
     * **The layout for writing entry appearance has been fixed for Windows and MacOS as well**
   * **Version 3.5.5**
     * **Direct PDF creation for Windows**
       * **[Direct Print PDF](#direct-print-pdf)**
   * **Version 3.5.6**
     * **Markdown marking highlight stay yellow and font color turn to black**
     * **Infor-Bar font smaller in Windows**
+  * **Version 3.5.8**
+    * **Fix bugs for previous version**
+    * **Some tweak on appearance in Windows**
+      * **Font look smaller on Buttons**
+      * **Font look smaller on Bible**
+      * **Font look smaller on info-bar**
+      * **others..**
 
 [⬆️](#freetvg-tree-view-gui)
 
 ## TVG
 
 ![TVG](Pics/TVG.png)
```

### Comparing `FreeTVG-karjakak-3.5.8/README.md` & `FreeTVG-karjakak-3.5.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -459,14 +459,21 @@
     * **The layout for writing entry appearance has been fixed for Windows and MacOS as well**
   * **Version 3.5.5**
     * **Direct PDF creation for Windows**
       * **[Direct Print PDF](#direct-print-pdf)**
   * **Version 3.5.6**
     * **Markdown marking highlight stay yellow and font color turn to black**
     * **Infor-Bar font smaller in Windows**
+  * **Version 3.5.8**
+    * **Fix bugs for previous version**
+    * **Some tweak on appearance in Windows**
+      * **Font look smaller on Buttons**
+      * **Font look smaller on Bible**
+      * **Font look smaller on info-bar**
+      * **others..**
 
 [⬆️](#freetvg-tree-view-gui)
 
 ## TVG
 
 ![TVG](Pics/TVG.png)
```

### Comparing `FreeTVG-karjakak-3.5.8/TVG/FreeTVG.py` & `FreeTVG-karjakak-3.5.9/TVG/FreeTVG.py`

 * *Files 1% similar despite different names*

```diff
@@ -582,15 +582,14 @@
             for fr in frm:
                 fr.pack_forget()
             with open(pth, "w") as bh:
                 bh.write("buttons hide")
         else:
             for fr in frm:
                 fr.pack(side=TOP, fill="x")
-            self.stl.configure("TButton", font="verdana 8 bold")
             os.remove(pth)
         self.tframe.pack(anchor="w", side=TOP, fill="both", expand=1)
         self.tframe.update()
         self.fscr.pack(fill="x")
         self.fscr.update()
         self.fframe.pack(fill="x")
         self.fframe.update()
```

### Comparing `FreeTVG-karjakak-3.5.8/TVG/Tutorial TVG.pdf` & `FreeTVG-karjakak-3.5.9/TVG/Tutorial TVG.pdf`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.5.8/TVG/bible_reader/.Bible/KJV.xml` & `FreeTVG-karjakak-3.5.9/TVG/bible_reader/.Bible/KJV.xml`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.5.8/TVG/bible_reader/bible_creator.py` & `FreeTVG-karjakak-3.5.9/TVG/bible_reader/bible_creator.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.5.8/TVG/bible_reader/layout_BR.py` & `FreeTVG-karjakak-3.5.9/TVG/bible_reader/layout_BR.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.5.8/TVG/structure/frame_layouts.py` & `FreeTVG-karjakak-3.5.9/TVG/structure/frame_layouts.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.5.8/TVG/utility/RegMail.py` & `FreeTVG-karjakak-3.5.9/TVG/utility/RegMail.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.5.8/TVG/utility/data_parse.py` & `FreeTVG-karjakak-3.5.9/TVG/utility/data_parse.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.5.8/TVG/utility/database_tvg.py` & `FreeTVG-karjakak-3.5.9/TVG/utility/database_tvg.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.5.8/TVG/utility/mdh.py` & `FreeTVG-karjakak-3.5.9/TVG/utility/mdh.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.5.8/setup.cfg` & `FreeTVG-karjakak-3.5.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2046 7265 6554 5647 2d6b 6172 6a61   = FreeTVG-karja
 00000020: 6b61 6b0d 0a76 6572 7369 6f6e 203d 2033  kak..version = 3
-00000030: 2e35 2e38 0d0a 6175 7468 6f72 203d 206b  .5.8..author = k
+00000030: 2e35 2e39 0d0a 6175 7468 6f72 203d 206b  .5.9..author = k
 00000040: 6172 6a61 6b61 6b0d 0a61 7574 686f 725f  arjakak..author_
 00000050: 656d 6169 6c20 3d20 6b61 6b6b 6172 6a61  email = kakkarja
 00000060: 2e67 6974 6875 6240 676d 6169 6c2e 636f  .github@gmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2054 7265 6520 5669 6577 2047 7569 2066   Tree View Gui f
 00000090: 6f72 206f 7574 6c69 6e65 2074 7265 6576  or outline treev
 000000a0: 6965 7720 6e6f 7465 2e0d 0a6c 6f6e 675f  iew note...long_
```

