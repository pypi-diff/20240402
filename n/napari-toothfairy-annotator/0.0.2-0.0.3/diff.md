# Comparing `tmp/napari-toothfairy-annotator-0.0.2.tar.gz` & `tmp/napari-toothfairy-annotator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-toothfairy-annotator-0.0.2.tar", last modified: Thu Mar 28 14:56:38 2024, max compression
+gzip compressed data, was "napari-toothfairy-annotator-0.0.3.tar", last modified: Tue Apr  2 09:18:14 2024, max compression
```

## Comparing `napari-toothfairy-annotator-0.0.2.tar` & `napari-toothfairy-annotator-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 14:56:38.113827 napari-toothfairy-annotator-0.0.2/
--rw-rw-rw-   0        0        0     1102 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      101 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4716 2024-03-28 14:56:38.113827 napari-toothfairy-annotator-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2968 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.2/README.md
--rw-rw-rw-   0        0        0     1233 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1927 2024-03-28 14:56:38.115943 napari-toothfairy-annotator-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-28 14:56:38.077879 napari-toothfairy-annotator-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-28 14:56:38.089980 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/
--rw-rw-rw-   0        0        0     9539 2024-03-27 18:07:08.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/FDI_Annotator.py
--rw-rw-rw-   0        0        0      335 2024-03-28 14:56:30.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/__init__.py
--rw-rw-rw-   0        0        0      812 2024-03-27 10:15:18.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/_reader.py
-drwxrwxrwx   0        0        0        0 2024-03-28 14:56:38.110827 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/_tests/
--rw-rw-rw-   0        0        0        0 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/_tests/__init__.py
--rw-rw-rw-   0        0        0     1020 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/_tests/test_reader.py
--rw-rw-rw-   0        0        0     2284 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/_tests/test_widget.py
--rw-rw-rw-   0        0        0      143 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/_tests/test_writer.py
--rw-rw-rw-   0        0        0    12280 2024-03-27 16:20:58.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/_widget.py
--rw-rw-rw-   0        0        0     1998 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/_writer.py
--rw-rw-rw-   0        0        0     1516 2024-03-28 14:54:08.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-03-28 14:56:38.111828 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator.egg-info/
--rw-rw-rw-   0        0        0     4716 2024-03-28 14:56:38.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      865 2024-03-28 14:56:38.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 14:56:38.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-03-28 14:56:38.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       89 2024-03-28 14:56:38.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-03-28 14:56:38.000000 napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 09:18:14.514538 napari-toothfairy-annotator-0.0.3/
+-rw-rw-rw-   0        0        0     1102 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-02 09:17:13.000000 napari-toothfairy-annotator-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4716 2024-04-02 09:18:14.514538 napari-toothfairy-annotator-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2968 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1233 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1927 2024-04-02 09:18:14.517534 napari-toothfairy-annotator-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 09:18:14.357374 napari-toothfairy-annotator-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 09:18:14.370493 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/
+-rw-rw-rw-   0        0        0     9570 2024-03-28 15:26:39.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/FDI_Annotator.py
+-rw-rw-rw-   0        0        0      335 2024-04-02 09:16:50.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/__init__.py
+-rw-rw-rw-   0        0        0      812 2024-03-27 10:15:18.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/_reader.py
+drwxrwxrwx   0        0        0        0 2024-04-02 09:18:14.510414 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/_tests/
+-rw-rw-rw-   0        0        0        0 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/_tests/__init__.py
+-rw-rw-rw-   0        0        0     1020 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/_tests/test_reader.py
+-rw-rw-rw-   0        0        0     2284 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/_tests/test_widget.py
+-rw-rw-rw-   0        0        0      143 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/_tests/test_writer.py
+-rw-rw-rw-   0        0        0    12279 2024-04-02 09:13:38.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/_widget.py
+-rw-rw-rw-   0        0        0     1998 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/_writer.py
+-rw-rw-rw-   0        0        0     1514 2024-04-02 09:06:47.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-04-02 09:18:14.511534 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator.egg-info/
+-rw-rw-rw-   0        0        0     4716 2024-04-02 09:18:14.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      865 2024-04-02 09:18:14.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 09:18:14.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-02 09:18:14.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2024-04-02 09:18:14.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-02 09:18:14.000000 napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator.egg-info/top_level.txt
```

### Comparing `napari-toothfairy-annotator-0.0.2/LICENSE` & `napari-toothfairy-annotator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.2/PKG-INFO` & `napari-toothfairy-annotator-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-toothfairy-annotator
-Version: 0.0.2
+Version: 0.0.3
 Summary: The plugin employed to annotate volumes employed in the ToothFairy 2 Challenge
 Home-page: https://github.com/LucaLumetti/napari-toothfairy-annotator
 Author: Luca Lumetti
 Author-email: lumetti.luca@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LucaLumetti/napari-toothfairy-annotator/issues
 Project-URL: Documentation, https://github.com/LucaLumetti/napari-toothfairy-annotator#README.md
```

### Comparing `napari-toothfairy-annotator-0.0.2/README.md` & `napari-toothfairy-annotator-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.2/pyproject.toml` & `napari-toothfairy-annotator-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.2/setup.cfg` & `napari-toothfairy-annotator-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/FDI_Annotator.py` & `napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/FDI_Annotator.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,9 +93,9 @@
             "47": {"quadrant": 4, "ID": "47", "type": "Molar", "name": "Lower Right Second Molar"},
             "48": {"quadrant": 4, "ID": "48", "type": "Molar", "name": "Lower Right Third Molar (Wisdom Tooth)"}
         }
 
 
 if __name__ == "__main__":
     annot = FDI_Annotator()
-    for k in annot.inverse.keys():
-        print(k)
+    for k, name in annot.fdi_notation.items():
+        print(int(k), name['name'])
```

### Comparing `napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/_reader.py` & `napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/_tests/test_reader.py` & `napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/_tests/test_widget.py` & `napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/_widget.py` & `napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     QDir,
     QModelIndex,
     QPoint,
     QRegExp,
     QSortFilterProxyModel,
     Qt,
 )
-from PyQt5.QtGui import (
+from qtpy.QtGui import (
     QColor,
     QPainter,
     QIcon,
 )
 
 from napari.viewer import Viewer
 from magicgui.widgets import FileEdit
```

### Comparing `napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/_writer.py` & `napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator/napari.yaml` & `napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator/napari.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -11,24 +11,24 @@
       title: Open data with ToothFairy Annotator
     - id: napari-toothfairy-annotator.write_multiple
       python_name: napari_toothfairy_annotator._writer:write_multiple
       title: Save multi-layer data with ToothFairy Annotator
     - id: napari-toothfairy-annotator.write_single_image
       python_name: napari_toothfairy_annotator._writer:write_single_image
       title: Save image data with ToothFairy Annotator
-    - id: napari-toothfairy-annotator.explorer
+    - id: napari-toothfairy-annotator.annotator
       python_name: napari_toothfairy_annotator._widget:FolderBrowser
       title: Annotator
   readers:
     - command: napari-toothfairy-annotator.get_reader
       accepts_directories: true
       filename_patterns: ['*']
   writers:
     - command: napari-toothfairy-annotator.write_multiple
       layer_types: ['image*','labels*']
       filename_extensions: []
     - command: napari-toothfairy-annotator.write_single_image
       layer_types: ['image']
       filename_extensions: ['.npy']
   widgets:
-    - command: napari-toothfairy-annotator.explorer
-      display_name: File Explorer
+    - command: napari-toothfairy-annotator.annotator
+      display_name: Annotator
```

### Comparing `napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator.egg-info/PKG-INFO` & `napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-toothfairy-annotator
-Version: 0.0.2
+Version: 0.0.3
 Summary: The plugin employed to annotate volumes employed in the ToothFairy 2 Challenge
 Home-page: https://github.com/LucaLumetti/napari-toothfairy-annotator
 Author: Luca Lumetti
 Author-email: lumetti.luca@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LucaLumetti/napari-toothfairy-annotator/issues
 Project-URL: Documentation, https://github.com/LucaLumetti/napari-toothfairy-annotator#README.md
```

### Comparing `napari-toothfairy-annotator-0.0.2/src/napari_toothfairy_annotator.egg-info/SOURCES.txt` & `napari-toothfairy-annotator-0.0.3/src/napari_toothfairy_annotator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

