# Comparing `tmp/NeonPathPlanning-1.0.0.tar.gz` & `tmp/NeonPathPlanning-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/NeonPathPlanning/NeonPathPlanning/dist/.tmp-5lgq3_7f/NeonPathPlanning-1.0.0.tar", last modified: Fri Mar  8 14:13:15 2024, max compression
+gzip compressed data, was "/home/runner/work/NeonPathPlanning/NeonPathPlanning/dist/.tmp-9cfehf7_/NeonPathPlanning-1.0.1.tar", last modified: Tue Apr  2 14:17:02 2024, max compression
```

## Comparing `NeonPathPlanning-1.0.0.tar` & `NeonPathPlanning-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:13:15.000000 NeonPathPlanning-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-08 14:13:11.000000 NeonPathPlanning-1.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:13:15.000000 NeonPathPlanning-1.0.0/NeonPathPlanning/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-08 14:13:11.000000 NeonPathPlanning-1.0.0/NeonPathPlanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-08 14:13:11.000000 NeonPathPlanning-1.0.0/NeonPathPlanning/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-03-08 14:13:11.000000 NeonPathPlanning-1.0.0/NeonPathPlanning/limit_cycle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-03-08 14:13:11.000000 NeonPathPlanning-1.0.0/NeonPathPlanning/potential_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-03-08 14:13:11.000000 NeonPathPlanning-1.0.0/NeonPathPlanning/univector_field.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:13:15.000000 NeonPathPlanning-1.0.0/NeonPathPlanning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-08 14:13:15.000000 NeonPathPlanning-1.0.0/NeonPathPlanning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-08 14:13:15.000000 NeonPathPlanning-1.0.0/NeonPathPlanning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 14:13:15.000000 NeonPathPlanning-1.0.0/NeonPathPlanning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-08 14:13:15.000000 NeonPathPlanning-1.0.0/NeonPathPlanning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-08 14:13:15.000000 NeonPathPlanning-1.0.0/NeonPathPlanning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-08 14:13:15.000000 NeonPathPlanning-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-08 14:13:11.000000 NeonPathPlanning-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 14:13:15.000000 NeonPathPlanning-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-08 14:13:11.000000 NeonPathPlanning-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:17:02.000000 NeonPathPlanning-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-02 14:16:57.000000 NeonPathPlanning-1.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:17:02.000000 NeonPathPlanning-1.0.1/NeonPathPlanning/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 14:16:57.000000 NeonPathPlanning-1.0.1/NeonPathPlanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-02 14:16:57.000000 NeonPathPlanning-1.0.1/NeonPathPlanning/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-02 14:16:57.000000 NeonPathPlanning-1.0.1/NeonPathPlanning/limit_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-02 14:16:57.000000 NeonPathPlanning-1.0.1/NeonPathPlanning/potential_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-02 14:16:57.000000 NeonPathPlanning-1.0.1/NeonPathPlanning/univector_field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:17:02.000000 NeonPathPlanning-1.0.1/NeonPathPlanning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-02 14:17:02.000000 NeonPathPlanning-1.0.1/NeonPathPlanning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-02 14:17:02.000000 NeonPathPlanning-1.0.1/NeonPathPlanning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:17:02.000000 NeonPathPlanning-1.0.1/NeonPathPlanning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 14:17:02.000000 NeonPathPlanning-1.0.1/NeonPathPlanning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 14:17:02.000000 NeonPathPlanning-1.0.1/NeonPathPlanning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-02 14:17:02.000000 NeonPathPlanning-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-02 14:16:57.000000 NeonPathPlanning-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:17:02.000000 NeonPathPlanning-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-02 14:16:57.000000 NeonPathPlanning-1.0.1/setup.py
```

### Comparing `NeonPathPlanning-1.0.0/LICENSE` & `NeonPathPlanning-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NeonPathPlanning-1.0.0/NeonPathPlanning/commons.py` & `NeonPathPlanning-1.0.1/NeonPathPlanning/commons.py`

 * *Files identical despite different names*

### Comparing `NeonPathPlanning-1.0.0/NeonPathPlanning/limit_cycle.py` & `NeonPathPlanning-1.0.1/NeonPathPlanning/limit_cycle.py`

 * *Files identical despite different names*

### Comparing `NeonPathPlanning-1.0.0/NeonPathPlanning/potential_fields.py` & `NeonPathPlanning-1.0.1/NeonPathPlanning/potential_fields.py`

 * *Files identical despite different names*

### Comparing `NeonPathPlanning-1.0.0/NeonPathPlanning/univector_field.py` & `NeonPathPlanning-1.0.1/NeonPathPlanning/univector_field.py`

 * *Files identical despite different names*

### Comparing `NeonPathPlanning-1.0.0/NeonPathPlanning.egg-info/PKG-INFO` & `NeonPathPlanning-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,37 @@
-Metadata-Version: 2.1
-Name: NeonPathPlanning
-Version: 1.0.0
-Summary: Collection of autonomous robot path planners
-Author: Project-Neon
-Author-email: projectneon@gmail.com
-License: GNU
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # NeonPathPlanning
-Simplify autonomous navigation wit different path planning algorithms
+Simplify autonomous navigation with different path planning algorithms
 
 
 ## Requirements
 - numpy
 
 
 ## Installation
 Use the code below to install the package from PyPI:
 
-`pip install pySSLVision`
+`pip install NeonPathPlanning`
 
 
 ## Overview
 A collection of different autonomous robot path planning algorithm, originally thought to be used on soccer robotics.
 
 Current implemented:
 * Uni-Vector Field
 * Limit Cycle
 * Potential Fields
 
 ## Colaboration Guide
 In order to colaborate with this repository, clone this repository:
 
-`git clone https://github.com/project-neon/pySSLVision`
+`git clone https://github.com/project-neon/NeonPathPlanning`
 
 Open directory
 
-`cd pySSLVision`
+`cd NeonPathPlanning`
 
 Then install dependencies
 
 `pip install -r requirements.txt`
 
 Finally, install the package
```

