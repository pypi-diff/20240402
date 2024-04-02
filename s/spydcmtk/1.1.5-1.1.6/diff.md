# Comparing `tmp/spydcmtk-1.1.5.tar.gz` & `tmp/spydcmtk-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spydcmtk-1.1.5.tar", last modified: Wed Mar  6 21:06:53 2024, max compression
+gzip compressed data, was "spydcmtk-1.1.6.tar", last modified: Tue Apr  2 11:48:55 2024, max compression
```

## Comparing `spydcmtk-1.1.5.tar` & `spydcmtk-1.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-03-06 21:06:53.286189 spydcmtk-1.1.5/
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     1076 2023-11-05 16:19:14.000000 spydcmtk-1.1.5/LICENSE
--rw-r--r--   0 fraser    (1000) fraser    (1000)     4252 2024-03-06 21:06:53.286189 spydcmtk-1.1.5/PKG-INFO
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     3435 2024-03-04 14:18:23.000000 spydcmtk-1.1.5/README.md
--rw-rw-r--   0 fraser    (1000) fraser    (1000)       38 2024-03-06 21:06:53.286189 spydcmtk-1.1.5/setup.cfg
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     3899 2024-03-06 21:05:55.000000 spydcmtk-1.1.5/setup.py
-drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-03-06 21:06:53.286189 spydcmtk-1.1.5/spydcmtk/
--rw-rw-r--   0 fraser    (1000) fraser    (1000)  3728964 2023-11-05 16:19:14.000000 spydcmtk-1.1.5/spydcmtk/ParaViewGlance.html
--rw-rw-r--   0 fraser    (1000) fraser    (1000)      169 2023-09-04 08:30:32.000000 spydcmtk-1.1.5/spydcmtk/__init__.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)    45265 2024-03-04 14:18:23.000000 spydcmtk-1.1.5/spydcmtk/dcmTK.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)    18903 2024-03-04 14:18:23.000000 spydcmtk-1.1.5/spydcmtk/dcmTools.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)    19675 2024-03-04 14:18:23.000000 spydcmtk-1.1.5/spydcmtk/dcmVTKTK.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)    23753 2024-03-04 14:18:23.000000 spydcmtk-1.1.5/spydcmtk/spydcm.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     3009 2024-03-04 14:18:23.000000 spydcmtk-1.1.5/spydcmtk/spydcm_config.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     1781 2024-03-04 14:18:23.000000 spydcmtk-1.1.5/spydcmtk/spydcmtk.conf
-drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-03-06 21:06:53.286189 spydcmtk-1.1.5/spydcmtk.egg-info/
--rw-r--r--   0 fraser    (1000) fraser    (1000)     4252 2024-03-06 21:06:53.000000 spydcmtk-1.1.5/spydcmtk.egg-info/PKG-INFO
--rw-rw-r--   0 fraser    (1000) fraser    (1000)      398 2024-03-06 21:06:53.000000 spydcmtk-1.1.5/spydcmtk.egg-info/SOURCES.txt
--rw-rw-r--   0 fraser    (1000) fraser    (1000)        1 2024-03-06 21:06:53.000000 spydcmtk-1.1.5/spydcmtk.egg-info/dependency_links.txt
--rw-rw-r--   0 fraser    (1000) fraser    (1000)       50 2024-03-06 21:06:53.000000 spydcmtk-1.1.5/spydcmtk.egg-info/entry_points.txt
--rw-rw-r--   0 fraser    (1000) fraser    (1000)       65 2024-03-06 21:06:53.000000 spydcmtk-1.1.5/spydcmtk.egg-info/requires.txt
--rw-rw-r--   0 fraser    (1000) fraser    (1000)        9 2024-03-06 21:06:53.000000 spydcmtk-1.1.5/spydcmtk.egg-info/top_level.txt
+drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-04-02 11:48:55.466254 spydcmtk-1.1.6/
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     1076 2023-11-05 16:19:14.000000 spydcmtk-1.1.6/LICENSE
+-rw-r--r--   0 fraser    (1000) fraser    (1000)     3350 2024-04-02 11:48:55.462254 spydcmtk-1.1.6/PKG-INFO
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     2533 2024-04-02 11:47:41.000000 spydcmtk-1.1.6/README.md
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)       38 2024-04-02 11:48:55.466254 spydcmtk-1.1.6/setup.cfg
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     3899 2024-04-02 11:47:41.000000 spydcmtk-1.1.6/setup.py
+drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-04-02 11:48:55.462254 spydcmtk-1.1.6/spydcmtk/
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)  3728964 2023-11-05 16:19:14.000000 spydcmtk-1.1.6/spydcmtk/ParaViewGlance.html
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)      169 2023-09-04 08:30:32.000000 spydcmtk-1.1.6/spydcmtk/__init__.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)    45265 2024-03-04 14:18:23.000000 spydcmtk-1.1.6/spydcmtk/dcmTK.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)    18903 2024-03-27 22:25:56.000000 spydcmtk-1.1.6/spydcmtk/dcmTools.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)    19675 2024-03-04 14:18:23.000000 spydcmtk-1.1.6/spydcmtk/dcmVTKTK.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)    23753 2024-03-04 14:18:23.000000 spydcmtk-1.1.6/spydcmtk/spydcm.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     3009 2024-03-04 14:18:23.000000 spydcmtk-1.1.6/spydcmtk/spydcm_config.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     1781 2024-03-04 14:18:23.000000 spydcmtk-1.1.6/spydcmtk/spydcmtk.conf
+drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-04-02 11:48:55.462254 spydcmtk-1.1.6/spydcmtk.egg-info/
+-rw-r--r--   0 fraser    (1000) fraser    (1000)     3350 2024-04-02 11:48:55.000000 spydcmtk-1.1.6/spydcmtk.egg-info/PKG-INFO
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)      398 2024-04-02 11:48:55.000000 spydcmtk-1.1.6/spydcmtk.egg-info/SOURCES.txt
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)        1 2024-04-02 11:48:55.000000 spydcmtk-1.1.6/spydcmtk.egg-info/dependency_links.txt
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)       50 2024-04-02 11:48:55.000000 spydcmtk-1.1.6/spydcmtk.egg-info/entry_points.txt
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)       65 2024-04-02 11:48:55.000000 spydcmtk-1.1.6/spydcmtk.egg-info/requires.txt
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)        9 2024-04-02 11:48:55.000000 spydcmtk-1.1.6/spydcmtk.egg-info/top_level.txt
```

### Comparing `spydcmtk-1.1.5/LICENSE` & `spydcmtk-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spydcmtk-1.1.5/README.md` & `spydcmtk-1.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,55 @@
+Metadata-Version: 2.1
+Name: spydcmtk
+Version: 1.1.6
+Summary: Simple python dicom toolkit.
+Home-page: https://github.com/fraser29/spydcmtk
+Author: Fraser M. Callaghan
+Author-email: callaghan.fm@gmail.com
+License: MIT
+Keywords: medical,imaging,mri,ct,dicom
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.9.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pydicom>=2.0.0
+Requires-Dist: numpy>=1.26.2
+Requires-Dist: tqdm>=4.66.1
+Requires-Dist: vtk==9.3.0
+Requires-Dist: python-gdcm
+
+
 # *spydcmtk*
 
 *Simple PYthon DiCoM Tool Kit*
 
 Dicom organisational, querying and conversion toolkit
 
 *spydcmtk* is a pure Python package built on top of [*pydicom*](https://github.com/pydicom/pydicom).
 
 This package extends pydicom with a class structure based upon the Patient-Study-Series-Image hierarchy. In addition, it provides a number of built in routines for common actions when working with dicom files, such as human readable renaming, anonymisation, searching and summarising. 
 
 ## Version
 
-Current is VERSION 1.1.4 Release. 
+Current is VERSION 1.1.5 Release. 
 
+1.1.5: Add option to retrieve tag value from commandline. Small bug fix on safe naming. 
 1.1.4: Additional configuration moved to config file. DCM2VTI active. 
 1.1.1: Add option to keep private tags when running anonymisation. Dcm2nii path configurable from config file. 
 1.1.0: Some bug fixes and restrict the use of dicom to vti (WIP)
 1.0.0: Initial Release
 
 ## Installation
 
-Using [pip](https://pip.pypa.io/en/stable/):
+Using [pip](https://pypi.org/project/spydcmtk/):
 ```
 pip install spydcmtk
 ```
 
 ## Quick start
 
 If you installed via pip then *spydcmtk* console script will be exposed in your python environment. 
@@ -36,16 +62,18 @@
 
 
 If you would like to incorporate spydcmtk into your python project, then import as:
 ```python
 import spydcmtk
 
 listOfStudies = spydcmtk.dcmTK.ListOfDicomStudies.setFromDirectory(MY_DICOM_DIRECTORY)
+# Example filtering
 dcmStudy = listOfStudies.getStudyByDate('20230429') # Dates in dicom standard string format: YYYYMMDD
 dcmSeries = dcmStudy.getSeriesBySeriesNumber(1)
+# Example writing new dicom files with anonymisation
 dcmStudy.writeToOrganisedFileStructure(tmpDir, anonName='Not A Name')
 
 ```
 
 
 # Configuration
 
@@ -65,33 +93,8 @@
 
 `spydcmtk -INFO` 
 
 
 ## Documentation
 
 Clear documentation of basic features can be seen by running the *"spycmtk -h"* command as referenced above. 
-
-For detailed documentation please see [wiki](https://github.com/fraser29/spydcmtk/wiki)
-
-Some format conversions are provided by this package:
-
-### Dicom to Nifti
-
-Relies on [*dcm2niix*](https://github.com/rordenlab/dcm2niix), which must be installed and in path (or set in config file).
-
-### Dicom to HTML
-
-Will build a standalone .html file to display dicom series in [*ParaView Glance*](https://www.kitware.com/exporting-paraview-scenes-to-paraview-glance/) renderer. 
-
-
-### Dicom to VTK
-
-A dicom to vtk format conversion is provided. See VTK format documentation [*here*](https://examples.vtk.org/site/VTKFileFormats/). 
-
-Format conversions are: 
-
-- dicom to image data (vti format). Suitable for 3D image volumes. This format is axis aligned (there is no embedded transformation). But "Field Data" embedded in the file are included as "ImageOrientationPatient" which, along with the Image Origin and Image Spacing methods can be used to construct a transformation matrix allowing conversion form image to real world coordinate space. 
-
-- *WORK IN PROGRESS*: dicom to structured dataset (vts format). 
-
-- *WORK IN PROGRESS*: dicom to planar dataset (vtp format).
-
+For detailed documentation please see [spydcmtk-documnetation](https://fraser29.github.io/spydcmtk/)
```

### Comparing `spydcmtk-1.1.5/setup.py` & `spydcmtk-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'spydcmtk'
 DESCRIPTION = 'Simple python dicom toolkit.'
 URL = 'https://github.com/fraser29/spydcmtk'
 EMAIL = 'callaghan.fm@gmail.com'
 AUTHOR = 'Fraser M. Callaghan'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '1.1.5'
+VERSION = '1.1.6'
 KEYWORDS="medical, imaging, mri, ct, dicom"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'pydicom>=2.0.0', 'numpy>=1.26.2', 'tqdm>=4.66.1', 'vtk==9.3.0', 'python-gdcm'
 ]
```

### Comparing `spydcmtk-1.1.5/spydcmtk/ParaViewGlance.html` & `spydcmtk-1.1.6/spydcmtk/ParaViewGlance.html`

 * *Files identical despite different names*

### Comparing `spydcmtk-1.1.5/spydcmtk/dcmTK.py` & `spydcmtk-1.1.6/spydcmtk/dcmTK.py`

 * *Files identical despite different names*

### Comparing `spydcmtk-1.1.5/spydcmtk/dcmTools.py` & `spydcmtk-1.1.6/spydcmtk/dcmTools.py`

 * *Files identical despite different names*

### Comparing `spydcmtk-1.1.5/spydcmtk/dcmVTKTK.py` & `spydcmtk-1.1.6/spydcmtk/dcmVTKTK.py`

 * *Files identical despite different names*

### Comparing `spydcmtk-1.1.5/spydcmtk/spydcm.py` & `spydcmtk-1.1.6/spydcmtk/spydcm.py`

 * *Files identical despite different names*

### Comparing `spydcmtk-1.1.5/spydcmtk/spydcm_config.py` & `spydcmtk-1.1.6/spydcmtk/spydcm_config.py`

 * *Files identical despite different names*

### Comparing `spydcmtk-1.1.5/spydcmtk/spydcmtk.conf` & `spydcmtk-1.1.6/spydcmtk/spydcmtk.conf`

 * *Files identical despite different names*

