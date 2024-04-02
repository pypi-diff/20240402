# Comparing `tmp/sbmlxdf-1.0.0.tar.gz` & `tmp/sbmlxdf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmlxdf-1.0.0.tar", last modified: Mon Jan 22 15:06:21 2024, max compression
+gzip compressed data, was "sbmlxdf-1.0.1.tar", last modified: Tue Apr  2 17:03:00 2024, max compression
```

## Comparing `sbmlxdf-1.0.0.tar` & `sbmlxdf-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-01-22 15:06:21.830107 sbmlxdf-1.0.0/
--rw-r--r--   0 peter      (501) staff       (20)    35149 2020-10-27 19:48:06.000000 sbmlxdf-1.0.0/LICENSE.txt
--rw-r--r--   0 peter      (501) staff       (20)       16 2020-09-14 06:40:44.000000 sbmlxdf-1.0.0/MANIFEST.in
--rw-r--r--   0 peter      (501) staff       (20)     5928 2024-01-22 15:06:21.829619 sbmlxdf-1.0.0/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)     4888 2021-11-03 14:18:36.000000 sbmlxdf-1.0.0/README.md
--rw-r--r--   0 peter      (501) staff       (20)      104 2021-07-28 19:30:27.000000 sbmlxdf-1.0.0/pyproject.toml
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-01-22 15:06:21.825744 sbmlxdf-1.0.0/sbmlxdf/
--rw-r--r--   0 peter      (501) staff       (20)      316 2022-01-26 11:47:18.000000 sbmlxdf-1.0.0/sbmlxdf/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)       85 2024-01-22 15:04:08.000000 sbmlxdf-1.0.0/sbmlxdf/_version.py
--rw-r--r--   0 peter      (501) staff       (20)    13006 2022-10-10 17:44:27.000000 sbmlxdf-1.0.0/sbmlxdf/annotation.py
--rw-r--r--   0 peter      (501) staff       (20)     3280 2022-12-16 15:28:12.000000 sbmlxdf-1.0.0/sbmlxdf/compartments.py
--rw-r--r--   0 peter      (501) staff       (20)     3463 2022-10-11 10:52:13.000000 sbmlxdf-1.0.0/sbmlxdf/constraints.py
--rw-r--r--   0 peter      (501) staff       (20)     1363 2022-10-11 10:36:51.000000 sbmlxdf-1.0.0/sbmlxdf/cursor.py
--rw-r--r--   0 peter      (501) staff       (20)     9011 2022-10-11 11:51:42.000000 sbmlxdf-1.0.0/sbmlxdf/events.py
--rw-r--r--   0 peter      (501) staff       (20)     6518 2022-10-11 10:02:20.000000 sbmlxdf-1.0.0/sbmlxdf/fbc.py
--rw-r--r--   0 peter      (501) staff       (20)     2121 2022-10-11 07:25:58.000000 sbmlxdf-1.0.0/sbmlxdf/function_defs.py
--rw-r--r--   0 peter      (501) staff       (20)     6001 2022-10-11 07:29:17.000000 sbmlxdf-1.0.0/sbmlxdf/groups.py
--rw-r--r--   0 peter      (501) staff       (20)     2364 2022-10-11 10:46:35.000000 sbmlxdf-1.0.0/sbmlxdf/init_assign.py
--rw-r--r--   0 peter      (501) staff       (20)    15066 2024-01-19 17:44:34.000000 sbmlxdf-1.0.0/sbmlxdf/misc.py
--rw-r--r--   0 peter      (501) staff       (20)    19852 2024-01-08 20:54:12.000000 sbmlxdf-1.0.0/sbmlxdf/model.py
--rw-r--r--   0 peter      (501) staff       (20)     4985 2022-10-11 07:56:07.000000 sbmlxdf-1.0.0/sbmlxdf/model_attrs.py
--rw-r--r--   0 peter      (501) staff       (20)     2713 2022-10-11 07:32:19.000000 sbmlxdf-1.0.0/sbmlxdf/parameters.py
--rw-r--r--   0 peter      (501) staff       (20)    17068 2022-10-11 07:34:41.000000 sbmlxdf-1.0.0/sbmlxdf/reactions.py
--rw-r--r--   0 peter      (501) staff       (20)     3787 2022-10-11 10:42:23.000000 sbmlxdf-1.0.0/sbmlxdf/rules.py
--rw-r--r--   0 peter      (501) staff       (20)    14445 2022-10-11 09:57:23.000000 sbmlxdf-1.0.0/sbmlxdf/sbase.py
--rw-r--r--   0 peter      (501) staff       (20)     3281 2022-10-11 09:52:55.000000 sbmlxdf-1.0.0/sbmlxdf/sbml_container.py
--rw-r--r--   0 peter      (501) staff       (20)     6595 2022-10-11 07:41:59.000000 sbmlxdf-1.0.0/sbmlxdf/species.py
--rw-r--r--   0 peter      (501) staff       (20)     3531 2022-10-11 07:40:17.000000 sbmlxdf-1.0.0/sbmlxdf/unit_defs.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-01-22 15:06:21.829108 sbmlxdf-1.0.0/sbmlxdf.egg-info/
--rw-r--r--   0 peter      (501) staff       (20)     5928 2024-01-22 15:06:21.000000 sbmlxdf-1.0.0/sbmlxdf.egg-info/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)      663 2024-01-22 15:06:21.000000 sbmlxdf-1.0.0/sbmlxdf.egg-info/SOURCES.txt
--rw-r--r--   0 peter      (501) staff       (20)        1 2024-01-22 15:06:21.000000 sbmlxdf-1.0.0/sbmlxdf.egg-info/dependency_links.txt
--rw-r--r--   0 peter      (501) staff       (20)      106 2024-01-22 15:06:21.000000 sbmlxdf-1.0.0/sbmlxdf.egg-info/requires.txt
--rw-r--r--   0 peter      (501) staff       (20)        8 2024-01-22 15:06:21.000000 sbmlxdf-1.0.0/sbmlxdf.egg-info/top_level.txt
--rw-r--r--   0 peter      (501) staff       (20)       38 2024-01-22 15:06:21.830215 sbmlxdf-1.0.0/setup.cfg
--rwxr-xr-x   0 peter      (501) staff       (20)     1647 2023-10-10 13:31:52.000000 sbmlxdf-1.0.0/setup.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-01-22 15:06:21.828410 sbmlxdf-1.0.0/test/
--rw-rw-rw-   0 peter      (501) staff       (20)     3403 2022-10-11 11:43:39.000000 sbmlxdf-1.0.0/test/test_sbml_features.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-02 17:03:00.863026 sbmlxdf-1.0.1/
+-rw-r--r--   0 peter      (501) staff       (20)    35149 2020-10-27 19:48:06.000000 sbmlxdf-1.0.1/LICENSE.txt
+-rw-r--r--   0 peter      (501) staff       (20)       16 2020-09-14 06:40:44.000000 sbmlxdf-1.0.1/MANIFEST.in
+-rw-r--r--   0 peter      (501) staff       (20)     5928 2024-04-02 17:03:00.862339 sbmlxdf-1.0.1/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)     4888 2021-11-03 14:18:36.000000 sbmlxdf-1.0.1/README.md
+-rw-r--r--   0 peter      (501) staff       (20)      104 2021-07-28 19:30:27.000000 sbmlxdf-1.0.1/pyproject.toml
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-02 17:03:00.857108 sbmlxdf-1.0.1/sbmlxdf/
+-rw-r--r--   0 peter      (501) staff       (20)      357 2024-04-02 16:17:40.000000 sbmlxdf-1.0.1/sbmlxdf/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)       85 2024-04-02 16:58:30.000000 sbmlxdf-1.0.1/sbmlxdf/_version.py
+-rw-r--r--   0 peter      (501) staff       (20)    13074 2024-03-28 13:30:36.000000 sbmlxdf-1.0.1/sbmlxdf/annotation.py
+-rw-r--r--   0 peter      (501) staff       (20)     3280 2022-12-16 15:28:12.000000 sbmlxdf-1.0.1/sbmlxdf/compartments.py
+-rw-r--r--   0 peter      (501) staff       (20)     3463 2022-10-11 10:52:13.000000 sbmlxdf-1.0.1/sbmlxdf/constraints.py
+-rw-r--r--   0 peter      (501) staff       (20)     1363 2022-10-11 10:36:51.000000 sbmlxdf-1.0.1/sbmlxdf/cursor.py
+-rw-r--r--   0 peter      (501) staff       (20)     9011 2022-10-11 11:51:42.000000 sbmlxdf-1.0.1/sbmlxdf/events.py
+-rw-r--r--   0 peter      (501) staff       (20)     6518 2022-10-11 10:02:20.000000 sbmlxdf-1.0.1/sbmlxdf/fbc.py
+-rw-r--r--   0 peter      (501) staff       (20)     2121 2022-10-11 07:25:58.000000 sbmlxdf-1.0.1/sbmlxdf/function_defs.py
+-rw-r--r--   0 peter      (501) staff       (20)     6001 2022-10-11 07:29:17.000000 sbmlxdf-1.0.1/sbmlxdf/groups.py
+-rw-r--r--   0 peter      (501) staff       (20)     2364 2022-10-11 10:46:35.000000 sbmlxdf-1.0.1/sbmlxdf/init_assign.py
+-rw-r--r--   0 peter      (501) staff       (20)    15067 2024-03-28 10:24:37.000000 sbmlxdf-1.0.1/sbmlxdf/misc.py
+-rw-r--r--   0 peter      (501) staff       (20)    19852 2024-01-08 20:54:12.000000 sbmlxdf-1.0.1/sbmlxdf/model.py
+-rw-r--r--   0 peter      (501) staff       (20)     4985 2022-10-11 07:56:07.000000 sbmlxdf-1.0.1/sbmlxdf/model_attrs.py
+-rw-r--r--   0 peter      (501) staff       (20)     2713 2022-10-11 07:32:19.000000 sbmlxdf-1.0.1/sbmlxdf/parameters.py
+-rw-r--r--   0 peter      (501) staff       (20)    17068 2022-10-11 07:34:41.000000 sbmlxdf-1.0.1/sbmlxdf/reactions.py
+-rw-r--r--   0 peter      (501) staff       (20)     3787 2022-10-11 10:42:23.000000 sbmlxdf-1.0.1/sbmlxdf/rules.py
+-rw-r--r--   0 peter      (501) staff       (20)    14445 2022-10-11 09:57:23.000000 sbmlxdf-1.0.1/sbmlxdf/sbase.py
+-rw-r--r--   0 peter      (501) staff       (20)     3281 2022-10-11 09:52:55.000000 sbmlxdf-1.0.1/sbmlxdf/sbml_container.py
+-rw-r--r--   0 peter      (501) staff       (20)     6595 2022-10-11 07:41:59.000000 sbmlxdf-1.0.1/sbmlxdf/species.py
+-rw-r--r--   0 peter      (501) staff       (20)     3531 2022-10-11 07:40:17.000000 sbmlxdf-1.0.1/sbmlxdf/unit_defs.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-02 17:03:00.861540 sbmlxdf-1.0.1/sbmlxdf.egg-info/
+-rw-r--r--   0 peter      (501) staff       (20)     5928 2024-04-02 17:03:00.000000 sbmlxdf-1.0.1/sbmlxdf.egg-info/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)      663 2024-04-02 17:03:00.000000 sbmlxdf-1.0.1/sbmlxdf.egg-info/SOURCES.txt
+-rw-r--r--   0 peter      (501) staff       (20)        1 2024-04-02 17:03:00.000000 sbmlxdf-1.0.1/sbmlxdf.egg-info/dependency_links.txt
+-rw-r--r--   0 peter      (501) staff       (20)      106 2024-04-02 17:03:00.000000 sbmlxdf-1.0.1/sbmlxdf.egg-info/requires.txt
+-rw-r--r--   0 peter      (501) staff       (20)        8 2024-04-02 17:03:00.000000 sbmlxdf-1.0.1/sbmlxdf.egg-info/top_level.txt
+-rw-r--r--   0 peter      (501) staff       (20)       38 2024-04-02 17:03:00.863173 sbmlxdf-1.0.1/setup.cfg
+-rwxr-xr-x   0 peter      (501) staff       (20)     1647 2023-10-10 13:31:52.000000 sbmlxdf-1.0.1/setup.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-02 17:03:00.860545 sbmlxdf-1.0.1/test/
+-rw-rw-rw-   0 peter      (501) staff       (20)     3403 2022-10-11 11:43:39.000000 sbmlxdf-1.0.1/test/test_sbml_features.py
```

### Comparing `sbmlxdf-1.0.0/LICENSE.txt` & `sbmlxdf-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/PKG-INFO` & `sbmlxdf-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmlxdf
-Version: 1.0.0
+Version: 1.0.1
 Summary: convert between SBML and tabular structures
 Home-page: https://gitlab.cs.uni-duesseldorf.de/schubert/sbmlxdf
 Author: Peter Schubert
 Author-email: peter.schubert@hhu.de
 License: GPLv3
 Project-URL: Source Code, https://gitlab.cs.uni-duesseldorf.de/schubert/sbmlxdf
 Project-URL: Documentation, https://sbmlxdf.readthedocs.io
```

### Comparing `sbmlxdf-1.0.0/README.md` & `sbmlxdf-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/annotation.py` & `sbmlxdf-1.0.1/sbmlxdf/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,16 @@
             self.sub_type = libsbml.BiolQualifierType_toString(
                                 sbml_cv.getBiologicalQualifierType())
         if qual_type_id == libsbml.MODEL_QUALIFIER:
             self.qual_type = 'bqmodel'
             self.sub_type = libsbml.ModelQualifierType_toString(
                                 sbml_cv.getModelQualifierType())
         for r_idx in range(sbml_cv.getNumResources()):
-            self.resource_uri.append(sbml_cv.getResourceURI(r_idx))
+            # stop resources uri as first semicolon
+            self.resource_uri.append((sbml_cv.getResourceURI(r_idx)).split(',')[0])
 
     def export_sbml(self, sbml_obj):
         sbml_cv = libsbml.CVTerm()
         if self.qual_type == 'bqbiol':
             sbml_cv.setQualifierType(libsbml.BIOLOGICAL_QUALIFIER)
             sbml_cv.setBiologicalQualifierType(self.sub_type)
         if self.qual_type == 'bqmodel':
```

### Comparing `sbmlxdf-1.0.0/sbmlxdf/compartments.py` & `sbmlxdf-1.0.1/sbmlxdf/compartments.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/constraints.py` & `sbmlxdf-1.0.1/sbmlxdf/constraints.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/cursor.py` & `sbmlxdf-1.0.1/sbmlxdf/cursor.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/events.py` & `sbmlxdf-1.0.1/sbmlxdf/events.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/fbc.py` & `sbmlxdf-1.0.1/sbmlxdf/fbc.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/function_defs.py` & `sbmlxdf-1.0.1/sbmlxdf/function_defs.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/groups.py` & `sbmlxdf-1.0.1/sbmlxdf/groups.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/init_assign.py` & `sbmlxdf-1.0.1/sbmlxdf/init_assign.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/misc.py` & `sbmlxdf-1.0.1/sbmlxdf/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
     if type(annotations) is str:
         for annotation in record_generator(annotations):
             fields = [item.strip() for item in annotation.split(',')]
             if qualifier is not None and fields[0] != qualifier:
                 continue
             for field in fields[1:]:
                 if database in field:
-                    refs.append(field.rsplit('/')[1])
+                    refs.append(field.rsplit('/')[-1])
     return refs
 
 
 def extract_xml_attrs(xml_annots, ns=None, token=None):
     """Extract XML-attributes from given namespace and/or token.
 
     Example of xml_annots: 'ns_uri=http://www.hhu.de/ccb/bgm/ns, prefix=bgm,
```

### Comparing `sbmlxdf-1.0.0/sbmlxdf/model.py` & `sbmlxdf-1.0.1/sbmlxdf/model.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/model_attrs.py` & `sbmlxdf-1.0.1/sbmlxdf/model_attrs.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/parameters.py` & `sbmlxdf-1.0.1/sbmlxdf/parameters.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/reactions.py` & `sbmlxdf-1.0.1/sbmlxdf/reactions.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/rules.py` & `sbmlxdf-1.0.1/sbmlxdf/rules.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/sbase.py` & `sbmlxdf-1.0.1/sbmlxdf/sbase.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/sbml_container.py` & `sbmlxdf-1.0.1/sbmlxdf/sbml_container.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/species.py` & `sbmlxdf-1.0.1/sbmlxdf/species.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf/unit_defs.py` & `sbmlxdf-1.0.1/sbmlxdf/unit_defs.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/sbmlxdf.egg-info/PKG-INFO` & `sbmlxdf-1.0.1/sbmlxdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmlxdf
-Version: 1.0.0
+Version: 1.0.1
 Summary: convert between SBML and tabular structures
 Home-page: https://gitlab.cs.uni-duesseldorf.de/schubert/sbmlxdf
 Author: Peter Schubert
 Author-email: peter.schubert@hhu.de
 License: GPLv3
 Project-URL: Source Code, https://gitlab.cs.uni-duesseldorf.de/schubert/sbmlxdf
 Project-URL: Documentation, https://sbmlxdf.readthedocs.io
```

### Comparing `sbmlxdf-1.0.0/sbmlxdf.egg-info/SOURCES.txt` & `sbmlxdf-1.0.1/sbmlxdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/setup.py` & `sbmlxdf-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `sbmlxdf-1.0.0/test/test_sbml_features.py` & `sbmlxdf-1.0.1/test/test_sbml_features.py`

 * *Files identical despite different names*

