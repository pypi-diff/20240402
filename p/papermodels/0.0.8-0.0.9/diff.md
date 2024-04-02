# Comparing `tmp/papermodels-0.0.8.tar.gz` & `tmp/papermodels-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papermodels-0.0.8.tar", last modified: Sat Nov 19 10:58:44 2022, max compression
+gzip compressed data, was "papermodels-0.0.9.tar", last modified: Sat Nov 19 11:01:27 2022, max compression
```

## Comparing `papermodels-0.0.8.tar` & `papermodels-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1837 2022-05-29 03:58:29.081559 papermodels-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2022-05-29 03:58:29.081559 papermodels-0.0.8/LICENSE
--rw-r--r--   0        0        0       69 2022-05-29 03:58:29.081559 papermodels-0.0.8/README.md
--rw-r--r--   0        0        0      576 2022-10-18 23:06:08.690459 papermodels-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      103 2022-11-19 10:58:26.053815 papermodels-0.0.8/src/papermodels/__init__.py
--rw-r--r--   0        0        0        0 2022-10-14 04:40:52.063624 papermodels-0.0.8/src/papermodels/datatypes/__init__.py
--rw-r--r--   0        0        0     2261 2022-10-14 05:19:14.840303 papermodels-0.0.8/src/papermodels/datatypes/annotation.py
--rw-r--r--   0        0        0      519 2022-10-14 05:12:43.155660 papermodels-0.0.8/src/papermodels/datatypes/utils.py
--rw-r--r--   0        0        0        0 2022-05-29 03:58:29.081559 papermodels-0.0.8/src/papermodels/db/__init__.py
--rw-r--r--   0        0        0     2854 2022-10-14 05:12:43.203662 papermodels-0.0.8/src/papermodels/db/data_model.py
--rw-r--r--   0        0        0        0 2022-09-02 06:16:31.209928 papermodels-0.0.8/src/papermodels/models/__init__.py
--rw-r--r--   0        0        0    11206 2022-10-14 05:12:43.279663 papermodels-0.0.8/src/papermodels/models/load_distribution.py
--rw-r--r--   0        0        0       37 2022-10-14 05:12:43.151661 papermodels-0.0.8/src/papermodels/paper/__init__.py
--rw-r--r--   0        0        0     5488 2022-11-19 10:57:52.086315 papermodels-0.0.8/src/papermodels/paper/annotations.py
--rw-r--r--   0        0        0    10120 2022-11-19 10:56:23.151657 papermodels-0.0.8/src/papermodels/paper/fdf.py
--rw-r--r--   0        0        0     2114 2022-11-19 10:57:36.554545 papermodels-0.0.8/src/papermodels/paper/plot.py
--rw-r--r--   0        0        0        0 2022-05-29 03:58:29.081559 papermodels-0.0.8/src/papermodels/post/__init__.py
--rw-r--r--   0        0        0      251 2022-10-14 05:23:25.985059 papermodels-0.0.8/tests/test_annotations.py
--rw-r--r--   0        0        0      271 2022-10-14 04:52:33.444278 papermodels-0.0.8/tests/test_imports.py
--rw-r--r--   0        0        0       58 2022-10-14 04:09:37.712805 papermodels-0.0.8/tests/test_tests.py
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 papermodels-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1837 2022-05-29 03:58:29.081559 papermodels-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2022-05-29 03:58:29.081559 papermodels-0.0.9/LICENSE
+-rw-r--r--   0        0        0       69 2022-05-29 03:58:29.081559 papermodels-0.0.9/README.md
+-rw-r--r--   0        0        0      576 2022-10-18 23:06:08.690459 papermodels-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      103 2022-11-19 11:01:02.903588 papermodels-0.0.9/src/papermodels/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-14 04:40:52.063624 papermodels-0.0.9/src/papermodels/datatypes/__init__.py
+-rw-r--r--   0        0        0     2261 2022-10-14 05:19:14.840303 papermodels-0.0.9/src/papermodels/datatypes/annotation.py
+-rw-r--r--   0        0        0      519 2022-10-14 05:12:43.155660 papermodels-0.0.9/src/papermodels/datatypes/utils.py
+-rw-r--r--   0        0        0        0 2022-05-29 03:58:29.081559 papermodels-0.0.9/src/papermodels/db/__init__.py
+-rw-r--r--   0        0        0     2854 2022-10-14 05:12:43.203662 papermodels-0.0.9/src/papermodels/db/data_model.py
+-rw-r--r--   0        0        0        0 2022-09-02 06:16:31.209928 papermodels-0.0.9/src/papermodels/models/__init__.py
+-rw-r--r--   0        0        0    11206 2022-10-14 05:12:43.279663 papermodels-0.0.9/src/papermodels/models/load_distribution.py
+-rw-r--r--   0        0        0       37 2022-10-14 05:12:43.151661 papermodels-0.0.9/src/papermodels/paper/__init__.py
+-rw-r--r--   0        0        0     5486 2022-11-19 11:00:11.364307 papermodels-0.0.9/src/papermodels/paper/annotations.py
+-rw-r--r--   0        0        0    10120 2022-11-19 10:56:23.151657 papermodels-0.0.9/src/papermodels/paper/fdf.py
+-rw-r--r--   0        0        0     2114 2022-11-19 10:57:36.554545 papermodels-0.0.9/src/papermodels/paper/plot.py
+-rw-r--r--   0        0        0        0 2022-05-29 03:58:29.081559 papermodels-0.0.9/src/papermodels/post/__init__.py
+-rw-r--r--   0        0        0      251 2022-10-14 05:23:25.985059 papermodels-0.0.9/tests/test_annotations.py
+-rw-r--r--   0        0        0      271 2022-10-14 04:52:33.444278 papermodels-0.0.9/tests/test_imports.py
+-rw-r--r--   0        0        0       58 2022-10-14 04:09:37.712805 papermodels-0.0.9/tests/test_tests.py
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 papermodels-0.0.9/PKG-INFO
```

### Comparing `papermodels-0.0.8/.gitignore` & `papermodels-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `papermodels-0.0.8/LICENSE` & `papermodels-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `papermodels-0.0.8/pyproject.toml` & `papermodels-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `papermodels-0.0.8/src/papermodels/datatypes/annotation.py` & `papermodels-0.0.9/src/papermodels/datatypes/annotation.py`

 * *Files identical despite different names*

### Comparing `papermodels-0.0.8/src/papermodels/datatypes/utils.py` & `papermodels-0.0.9/src/papermodels/datatypes/utils.py`

 * *Files identical despite different names*

### Comparing `papermodels-0.0.8/src/papermodels/db/data_model.py` & `papermodels-0.0.9/src/papermodels/db/data_model.py`

 * *Files identical despite different names*

### Comparing `papermodels-0.0.8/src/papermodels/models/load_distribution.py` & `papermodels-0.0.9/src/papermodels/models/load_distribution.py`

 * *Files identical despite different names*

### Comparing `papermodels-0.0.8/src/papermodels/paper/annotations.py` & `papermodels-0.0.9/src/papermodels/paper/annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,20 +44,18 @@
 
 def filter_annotations(annots: list[Annotation], properties: dict) -> list[Annotation]:
     """
     Returns a list of annotations from 'annots' that have properties that match
     the keywords in 'properties'.
     Note: The filtering process currently requires that both the keys AND values in 'properties'
     be hashable.
-
     'properties' is a dictionary of annotation properties and their values, e.g.
         {'line_weight': 3.0, 'line_color': (1, 0, 0)}
         or 
         {'text': "Slab Outline"}
-
     The returned annotations will only be annotations that match ALL of the properties
     described.
     """
     filtered = []
     for annot in annots:
         if (annot.__dict__.items() & properties.items()) == properties.items():
             filtered.append(annot)
```

### Comparing `papermodels-0.0.8/src/papermodels/paper/fdf.py` & `papermodels-0.0.9/src/papermodels/paper/fdf.py`

 * *Files identical despite different names*

### Comparing `papermodels-0.0.8/src/papermodels/paper/plot.py` & `papermodels-0.0.9/src/papermodels/paper/plot.py`

 * *Files identical despite different names*

