# Comparing `tmp/radifox-1.0.8.tar.gz` & `tmp/radifox-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radifox-1.0.8.tar", last modified: Mon Apr  1 21:10:30 2024, max compression
+gzip compressed data, was "radifox-1.0.9.tar", last modified: Tue Apr  2 01:21:35 2024, max compression
```

## Comparing `radifox-1.0.8.tar` & `radifox-1.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.169299 radifox-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-01 21:10:25.000000 radifox-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46888 2024-04-01 21:10:30.169299 radifox-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    45907 2024-04-01 21:10:25.000000 radifox-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.169299 radifox-1.0.8/radifox/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 21:10:30.169299 radifox-1.0.8/radifox/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.161299 radifox-1.0.8/radifox/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13538 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/dicom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/lut.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    55768 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/nib_parrec_fork.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/parrec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox/conversion/parrec_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/parrec_templates/gen_info.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/parrec_templates/pixel_values.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/parrec_templates/top_header.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/parrec_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16756 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/modules/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox/naming/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/naming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/naming/imagefile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox/qa/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox/qa/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/templates/conversion.html
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/templates/processing.html
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/templates/project.html
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/templates/subject.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox/records/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/records/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/records/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46888 2024-04-01 21:10:30.000000 radifox-1.0.8/radifox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-01 21:10:30.000000 radifox-1.0.8/radifox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:10:30.000000 radifox-1.0.8/radifox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 21:10:30.000000 radifox-1.0.8/radifox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-01 21:10:30.000000 radifox-1.0.8/radifox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 21:10:30.000000 radifox-1.0.8/radifox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:10:30.169299 radifox-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-01 21:10:25.000000 radifox-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.503653 radifox-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-02 01:21:29.000000 radifox-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46888 2024-04-02 01:21:35.503653 radifox-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    45907 2024-04-02 01:21:29.000000 radifox-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.503653 radifox-1.0.9/radifox/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 01:21:35.503653 radifox-1.0.9/radifox/_static_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.499653 radifox-1.0.9/radifox/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/dicom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/lut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55768 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/nib_parrec_fork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/parrec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.499653 radifox-1.0.9/radifox/conversion/parrec_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/parrec_templates/gen_info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/parrec_templates/pixel_values.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/parrec_templates/top_header.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/parrec_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.499653 radifox-1.0.9/radifox/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16756 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/modules/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.499653 radifox-1.0.9/radifox/naming/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/naming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/naming/imagefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.499653 radifox-1.0.9/radifox/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.503653 radifox-1.0.9/radifox/qa/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/templates/conversion.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/templates/processing.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/templates/project.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/templates/subject.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.503653 radifox-1.0.9/radifox/records/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/records/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/records/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.503653 radifox-1.0.9/radifox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46888 2024-04-02 01:21:35.000000 radifox-1.0.9/radifox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-02 01:21:35.000000 radifox-1.0.9/radifox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:21:35.000000 radifox-1.0.9/radifox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 01:21:35.000000 radifox-1.0.9/radifox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 01:21:35.000000 radifox-1.0.9/radifox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 01:21:35.000000 radifox-1.0.9/radifox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:21:35.503653 radifox-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-02 01:21:29.000000 radifox-1.0.9/setup.py
```

### Comparing `radifox-1.0.8/LICENSE` & `radifox-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/PKG-INFO` & `radifox-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radifox
-Version: 1.0.8
+Version: 1.0.9
 Summary: RADIFOX is the RADiological Image File Ontology eXtension, a Python package for the organization and management of medical images.
 Home-page: https://github.com/jh-mipc/radifox
 Author: Blake Dewey
 Author-email: blake.dewey@jhu.edu
 License: Apache License, 2.0
 Keywords: mri conversion
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `radifox-1.0.8/README.md` & `radifox-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/_version.py` & `radifox-1.0.9/radifox/_version.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/conversion/base.py` & `radifox-1.0.9/radifox/conversion/base.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/conversion/cli.py` & `radifox-1.0.9/radifox/conversion/cli.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/conversion/dicom.py` & `radifox-1.0.9/radifox/conversion/dicom.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
     for scan in dicom_sort_dict:
         count_dict[scan[0]] += 1
         new_series_uids[scan] = scan[0] + (".%02d" % count_dict[scan[0]])
 
     # Find new series that have scans that share DICOM files (multi-frame)
     uids_by_files = defaultdict(list)
     for scan, dcm_list in dicom_sort_dict.items():
-        uids_by_files[tuple(dcm[0] for dcm in dcm_list)].append(scan)
+        uids_by_files[tuple(sorted(set(dcm[0] for dcm in dcm_list)))].append(scan)
     # Merge new series uids that share DICOM files
     for scans in uids_by_files.values():
         if len(scans) > 1:
             for scan in scans:
                 new_series_uids[scan] = ".".join(new_series_uids[scan].split(".")[:-1])
 
     for new_dcm_dir in new_series_uids.values():
```

### Comparing `radifox-1.0.8/radifox/conversion/exec.py` & `radifox-1.0.9/radifox/conversion/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,20 +76,20 @@
         type_folder = session_path / ("parrec" if parrec else "dcm")
         if not rerun:
             if source.is_dir():
                 if link is not None:
                     logging.info("Linking files from source to %s folder" % type_folder.name)
                     if link not in ["symlink", "hardlink"]:
                         raise ValueError("Unsupported linking type.")
-                    copytree_link(source, type_folder, link == "symlink")
+                    copytree_link(source, type_folder, link)
                     logging.info("Linking complete")
                 else:
                     logging.info("Copying files from source to %s folder" % type_folder.name)
                     # noinspection PyTypeChecker
-                    shutil.copytree(source, type_folder, copy_function=shutil.copyfile)
+                    copytree_link(source, type_folder, "copy")
                     logging.info("Copying complete")
             elif any([source.name.endswith(ext) for ext in allowed_archives()[1]]):
                 extract_archive(source, type_folder)
             else:
                 raise ValueError(
                     "Source is not a directory, but does not match one of "
                     "the available archive formats (%s)" % ", ".join(allowed_archives()[0])
```

### Comparing `radifox-1.0.8/radifox/conversion/json.py` & `radifox-1.0.9/radifox/conversion/json.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/conversion/logging.py` & `radifox-1.0.9/radifox/conversion/logging.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/conversion/lut.py` & `radifox-1.0.9/radifox/conversion/lut.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/conversion/metadata.py` & `radifox-1.0.9/radifox/conversion/metadata.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/conversion/nib_parrec_fork.py` & `radifox-1.0.9/radifox/conversion/nib_parrec_fork.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/conversion/parrec.py` & `radifox-1.0.9/radifox/conversion/parrec.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/conversion/parrec_templates/gen_info.txt` & `radifox-1.0.9/radifox/conversion/parrec_templates/gen_info.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/conversion/parrec_templates/pixel_values.txt` & `radifox-1.0.9/radifox/conversion/parrec_templates/pixel_values.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/conversion/parrec_writer.py` & `radifox-1.0.9/radifox/conversion/parrec_writer.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/conversion/utils.py` & `radifox-1.0.9/radifox/conversion/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from codecs import BOM_UTF8
 from collections.abc import Sequence
 import csv
 from datetime import datetime, date, time, timedelta
 import hashlib
 import logging
+import os
 from pathlib import Path
 import re
 import shutil
 from subprocess import check_output
 
 import nibabel as nib
 from pydicom.dataset import Dataset, FileDataset, Tag
@@ -16,25 +17,26 @@
 
 
 # http://stackoverflow.com/a/22718321
 def mkdir_p(path: Path, mode: int = 0o777) -> None:
     path.mkdir(mode=mode, parents=True, exist_ok=True)
 
 
-def copytree_link(source: Path, dest: Path, symlink: bool) -> None:
+def copytree_link(source: Path, dest: Path, method: str) -> None:
+    if method in ["hardlink", "softlink", "copy"]:
+        func = {"hardlink": os.link, "symlink": os.symlink, "copy": shutil.copyfile}[method]
+    else:
+        raise ValueError(f"Unsupported copy method: {method}")
     dest.mkdir(parents=True, exist_ok=True)
     for path in source.glob("*"):
         if path.is_file():
-            if symlink:
-                (dest / path.name).symlink_to(path)
-            else:
-                (dest / path.name).hardlink_to(path)
+            func(path, dest / path.name)
         elif path.is_dir():
             (dest / path.name).mkdir()
-            copytree_link(path, dest / path.name, symlink)
+            copytree_link(path, dest / path.name, method)
 
 
 # http://stackoverflow.com/a/10840586
 def silentremove(filename: Path) -> None:
     import shutil
     import errno
```

### Comparing `radifox-1.0.8/radifox/modules/staging.py` & `radifox-1.0.9/radifox/modules/staging.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/naming/imagefile.py` & `radifox-1.0.9/radifox/naming/imagefile.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/qa/app.py` & `radifox-1.0.9/radifox/qa/app.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/qa/create.py` & `radifox-1.0.9/radifox/qa/create.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/qa/run.py` & `radifox-1.0.9/radifox/qa/run.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/qa/templates/conversion.html` & `radifox-1.0.9/radifox/qa/templates/conversion.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/qa/templates/index.html` & `radifox-1.0.9/radifox/qa/templates/index.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/qa/templates/login.html` & `radifox-1.0.9/radifox/qa/templates/login.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/qa/templates/processing.html` & `radifox-1.0.9/radifox/qa/templates/processing.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/qa/templates/project.html` & `radifox-1.0.9/radifox/qa/templates/project.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/qa/templates/subject.html` & `radifox-1.0.9/radifox/qa/templates/subject.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/records/processing.py` & `radifox-1.0.9/radifox/records/processing.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox/records/utils.py` & `radifox-1.0.9/radifox/records/utils.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/radifox.egg-info/PKG-INFO` & `radifox-1.0.9/radifox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radifox
-Version: 1.0.8
+Version: 1.0.9
 Summary: RADIFOX is the RADiological Image File Ontology eXtension, a Python package for the organization and management of medical images.
 Home-page: https://github.com/jh-mipc/radifox
 Author: Blake Dewey
 Author-email: blake.dewey@jhu.edu
 License: Apache License, 2.0
 Keywords: mri conversion
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `radifox-1.0.8/radifox.egg-info/SOURCES.txt` & `radifox-1.0.9/radifox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.0.8/setup.py` & `radifox-1.0.9/setup.py`

 * *Files identical despite different names*

