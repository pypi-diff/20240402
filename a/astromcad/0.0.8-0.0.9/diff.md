# Comparing `tmp/astromcad-0.0.8.tar.gz` & `tmp/astromcad-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromcad-0.0.8.tar", last modified: Sun Mar 31 23:01:57 2024, max compression
+gzip compressed data, was "astromcad-0.0.9.tar", last modified: Sun Mar 31 23:04:47 2024, max compression
```

## Comparing `astromcad-0.0.8.tar` & `astromcad-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-03-31 23:01:57.924321 astromcad-0.0.8/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      295 2024-03-31 23:01:57.923838 astromcad-0.0.8/PKG-INFO
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-03-31 23:01:57.920116 astromcad-0.0.8/astromcad/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.0.8/astromcad/__init__.py
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     8926 2024-03-31 23:00:30.000000 astromcad-0.0.8/astromcad/astromcad.py
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-03-31 23:01:57.922963 astromcad-0.0.8/astromcad.egg-info/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      295 2024-03-31 23:01:57.000000 astromcad-0.0.8/astromcad.egg-info/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      217 2024-03-31 23:01:57.000000 astromcad-0.0.8/astromcad.egg-info/SOURCES.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-03-31 23:01:57.000000 astromcad-0.0.8/astromcad.egg-info/dependency_links.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       47 2024-03-31 23:01:57.000000 astromcad-0.0.8/astromcad.egg-info/requires.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-03-31 23:01:57.000000 astromcad-0.0.8/astromcad.egg-info/top_level.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-03-31 23:01:57.924444 astromcad-0.0.8/setup.cfg
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      650 2024-03-31 23:01:54.000000 astromcad-0.0.8/setup.py
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-03-31 23:04:47.990951 astromcad-0.0.9/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      295 2024-03-31 23:04:47.990450 astromcad-0.0.9/PKG-INFO
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-03-31 23:04:47.987298 astromcad-0.0.9/astromcad/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.0.9/astromcad/__init__.py
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     8926 2024-03-31 23:04:08.000000 astromcad-0.0.9/astromcad/astromcad.py
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-03-31 23:04:47.989848 astromcad-0.0.9/astromcad.egg-info/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      295 2024-03-31 23:04:47.000000 astromcad-0.0.9/astromcad.egg-info/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      217 2024-03-31 23:04:47.000000 astromcad-0.0.9/astromcad.egg-info/SOURCES.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-03-31 23:04:47.000000 astromcad-0.0.9/astromcad.egg-info/dependency_links.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       47 2024-03-31 23:04:47.000000 astromcad-0.0.9/astromcad.egg-info/requires.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-03-31 23:04:47.000000 astromcad-0.0.9/astromcad.egg-info/top_level.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-03-31 23:04:47.991081 astromcad-0.0.9/setup.cfg
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      650 2024-03-31 23:04:14.000000 astromcad-0.0.9/setup.py
```

### Comparing `astromcad-0.0.8/astromcad/astromcad.py` & `astromcad-0.0.9/astromcad/astromcad.py`

 * *Files identical despite different names*

### Comparing `astromcad-0.0.8/setup.py` & `astromcad-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Anomaly Detection for Astronomical Transients'
 LONG_DESCRIPTION = 'Train custom classifiers to be used as anomaly detectors for astronmical transients'
 
 # Setting up
 setup(
     name="astromcad",
     version=VERSION,
```

