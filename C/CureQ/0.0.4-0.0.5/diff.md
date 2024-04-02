# Comparing `tmp/CureQ-0.0.4.tar.gz` & `tmp/CureQ-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CureQ-0.0.4.tar", last modified: Thu Mar 21 12:30:41 2024, max compression
+gzip compressed data, was "CureQ-0.0.5.tar", last modified: Tue Apr  2 10:08:05 2024, max compression
```

## Comparing `CureQ-0.0.4.tar` & `CureQ-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 12:30:41.321420 CureQ-0.0.4/
-drwxrwxrwx   0        0        0        0 2024-03-21 12:30:41.298785 CureQ-0.0.4/CureQ/
--rw-rw-rw-   0        0        0      293 2024-03-14 12:47:34.000000 CureQ-0.0.4/CureQ/__init__.py
--rw-rw-rw-   0        0        0    41237 2024-03-21 10:36:18.000000 CureQ-0.0.4/CureQ/mea.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:30:41.316217 CureQ-0.0.4/CureQ.egg-info/
--rw-rw-rw-   0        0        0     1210 2024-03-21 12:30:40.000000 CureQ-0.0.4/CureQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-03-21 12:30:41.000000 CureQ-0.0.4/CureQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 12:30:40.000000 CureQ-0.0.4/CureQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-21 12:30:40.000000 CureQ-0.0.4/CureQ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2024-03-19 15:09:22.000000 CureQ-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1210 2024-03-21 12:30:41.318420 CureQ-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      708 2024-03-19 15:09:22.000000 CureQ-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-03-21 12:30:41.321420 CureQ-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      762 2024-03-21 12:29:12.000000 CureQ-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:08:05.584617 CureQ-0.0.5/
+drwxrwxrwx   0        0        0        0 2024-04-02 10:08:05.543839 CureQ-0.0.5/CureQ/
+-rw-rw-rw-   0        0        0      293 2024-03-14 12:47:34.000000 CureQ-0.0.5/CureQ/__init__.py
+-rw-rw-rw-   0        0        0    41237 2024-04-02 09:31:40.000000 CureQ-0.0.5/CureQ/mea.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:08:05.584617 CureQ-0.0.5/CureQ.egg-info/
+-rw-rw-rw-   0        0        0     1430 2024-04-02 10:08:04.000000 CureQ-0.0.5/CureQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-04-02 10:08:05.000000 CureQ-0.0.5/CureQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 10:08:04.000000 CureQ-0.0.5/CureQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-02 10:08:04.000000 CureQ-0.0.5/CureQ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 10:08:04.000000 CureQ-0.0.5/CureQ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2024-03-19 15:09:22.000000 CureQ-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1430 2024-04-02 10:08:05.584617 CureQ-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2024-03-19 15:09:22.000000 CureQ-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 10:08:05.584617 CureQ-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2024-04-02 10:08:00.000000 CureQ-0.0.5/setup.py
```

### Comparing `CureQ-0.0.4/CureQ/mea.py` & `CureQ-0.0.5/CureQ/mea.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Version 0.0.4
+# Version 0.0.5
 
 '''This file contains the entire MEA_analyzer pipeline, contained in functions'''
 # Imports
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.signal import butter, lfilter
 from scipy.stats import norm
```

### Comparing `CureQ-0.0.4/LICENSE` & `CureQ-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CureQ-0.0.4/README.md` & `CureQ-0.0.5/README.md`

 * *Files identical despite different names*

