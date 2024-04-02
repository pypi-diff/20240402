# Comparing `tmp/pre5g-0.9.tar.gz` & `tmp/pre5g-0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pre5g-0.9.tar", last modified: Mon Apr  1 11:30:48 2024, max compression
+gzip compressed data, was "dist/pre5g-0.91.tar", last modified: Mon Apr  1 11:34:33 2024, max compression
```

## Comparing `pre5g-0.9.tar` & `pre5g-0.91.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:30:48.087291 pre5g-0.9/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-0.9/LICENSE
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-01 11:30:48.087291 pre5g-0.9/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-0.9/README.md
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:30:48.086291 pre5g-0.9/pre5g/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      650 2024-04-01 11:29:32.000000 pre5g-0.9/pre5g/__init__.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1330 2024-04-01 11:28:19.000000 pre5g-0.9/pre5g/labelen.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2687 2024-04-01 11:28:46.000000 pre5g-0.9/pre5g/normalization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1318 2024-04-01 11:26:36.000000 pre5g-0.9/pre5g/onehoten.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2679 2024-04-01 11:29:12.000000 pre5g-0.9/pre5g/robustscaler.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3143 2024-04-01 11:29:20.000000 pre5g-0.9/pre5g/standardization.py
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:30:48.087291 pre5g-0.9/pre5g.egg-info/
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-01 11:30:48.000000 pre5g-0.9/pre5g.egg-info/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      265 2024-04-01 11:30:48.000000 pre5g-0.9/pre5g.egg-info/SOURCES.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-01 11:30:48.000000 pre5g-0.9/pre5g.egg-info/dependency_links.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-01 11:30:48.000000 pre5g-0.9/pre5g.egg-info/top_level.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-01 11:30:48.087291 pre5g-0.9/setup.cfg
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      601 2024-04-01 11:30:41.000000 pre5g-0.9/setup.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:34:33.721542 pre5g-0.91/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-0.91/LICENSE
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-01 11:34:33.720542 pre5g-0.91/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-0.91/README.md
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:34:33.719542 pre5g-0.91/pre5g/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      650 2024-04-01 11:33:58.000000 pre5g-0.91/pre5g/__init__.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1330 2024-04-01 11:28:19.000000 pre5g-0.91/pre5g/labelen.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-0.91/pre5g/normalization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1319 2024-04-01 11:33:05.000000 pre5g-0.91/pre5g/onehoten.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2679 2024-04-01 11:29:12.000000 pre5g-0.91/pre5g/robustscaler.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:33:29.000000 pre5g-0.91/pre5g/standardization.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:34:33.720542 pre5g-0.91/pre5g.egg-info/
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-01 11:34:33.000000 pre5g-0.91/pre5g.egg-info/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      265 2024-04-01 11:34:33.000000 pre5g-0.91/pre5g.egg-info/SOURCES.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-01 11:34:33.000000 pre5g-0.91/pre5g.egg-info/dependency_links.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-01 11:34:33.000000 pre5g-0.91/pre5g.egg-info/top_level.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-01 11:34:33.721542 pre5g-0.91/setup.cfg
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      602 2024-04-01 11:34:17.000000 pre5g-0.91/setup.py
```

### Comparing `pre5g-0.9/LICENSE` & `pre5g-0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `pre5g-0.9/pre5g/__init__.py` & `pre5g-0.91/pre5g/__init__.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.9/pre5g/labelen.py` & `pre5g-0.91/pre5g/labelen.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.9/pre5g/normalization.py` & `pre5g-0.91/pre5g/normalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import pandas as pd
 def normalize_all(data):
     """
     Normalize all columns in the dataset, retaining string values.
 
     Args:
     - data (list of lists): The data containing columns to normalize.
```

### Comparing `pre5g-0.9/pre5g/onehoten.py` & `pre5g-0.91/pre5g/onehoten.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pands as pd
+import pandas as pd
 
 # def one_hot_encoding_all(data):
 #     """
 #     Apply one-hot encoding to all columns containing categorical values in the dataset.
 
 #     Parameters:
 #     data (list of lists): Input dataset.
```

### Comparing `pre5g-0.9/pre5g/robustscaler.py` & `pre5g-0.91/pre5g/robustscaler.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.9/pre5g/standardization.py` & `pre5g-0.91/pre5g/standardization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pandas as pd
-import pandas as pd
+
 import numpy as np
 
 def standardize_all(data):
     """
     Standardize all columns in the dataset.
 
     Args:
```

