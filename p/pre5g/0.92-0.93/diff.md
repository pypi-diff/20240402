# Comparing `tmp/pre5g-0.92.tar.gz` & `tmp/pre5g-0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pre5g-0.92.tar", last modified: Tue Apr  2 05:40:17 2024, max compression
+gzip compressed data, was "dist/pre5g-0.93.tar", last modified: Tue Apr  2 08:34:49 2024, max compression
```

## Comparing `pre5g-0.92.tar` & `pre5g-0.93.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-02 05:40:17.381939 pre5g-0.92/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-0.92/LICENSE
--rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-02 05:40:17.381939 pre5g-0.92/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-0.92/README.md
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-02 05:40:17.380939 pre5g-0.92/pre5g/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      650 2024-04-02 05:39:34.000000 pre5g-0.92/pre5g/__init__.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1625 2024-04-02 05:38:57.000000 pre5g-0.92/pre5g/labelen.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-0.92/pre5g/normalization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1589 2024-04-02 05:34:03.000000 pre5g-0.92/pre5g/onehoten.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2679 2024-04-01 11:29:12.000000 pre5g-0.92/pre5g/robustscaler.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-0.92/pre5g/standardization.py
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-02 05:40:17.380939 pre5g-0.92/pre5g.egg-info/
--rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-02 05:40:17.000000 pre5g-0.92/pre5g.egg-info/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      265 2024-04-02 05:40:17.000000 pre5g-0.92/pre5g.egg-info/SOURCES.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-02 05:40:17.000000 pre5g-0.92/pre5g.egg-info/dependency_links.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-02 05:40:17.000000 pre5g-0.92/pre5g.egg-info/top_level.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-02 05:40:17.381939 pre5g-0.92/setup.cfg
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      602 2024-04-02 05:39:45.000000 pre5g-0.92/setup.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-02 08:34:49.644710 pre5g-0.93/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-0.93/LICENSE
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-02 08:34:49.644710 pre5g-0.93/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-0.93/README.md
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-02 08:34:49.642711 pre5g-0.93/pre5g/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      650 2024-04-02 05:39:34.000000 pre5g-0.93/pre5g/__init__.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1625 2024-04-02 05:38:57.000000 pre5g-0.93/pre5g/labelen.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-0.93/pre5g/normalization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1589 2024-04-02 05:34:03.000000 pre5g-0.93/pre5g/onehoten.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2679 2024-04-01 11:29:12.000000 pre5g-0.93/pre5g/robustscaler.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-0.93/pre5g/standardization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2029 2024-04-02 08:33:25.000000 pre5g-0.93/pre5g/winsorization.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-02 08:34:49.643710 pre5g-0.93/pre5g.egg-info/
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-02 08:34:49.000000 pre5g-0.93/pre5g.egg-info/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      288 2024-04-02 08:34:49.000000 pre5g-0.93/pre5g.egg-info/SOURCES.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-02 08:34:49.000000 pre5g-0.93/pre5g.egg-info/dependency_links.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-02 08:34:49.000000 pre5g-0.93/pre5g.egg-info/top_level.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-02 08:34:49.644710 pre5g-0.93/setup.cfg
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      602 2024-04-02 08:34:06.000000 pre5g-0.93/setup.py
```

### Comparing `pre5g-0.92/LICENSE` & `pre5g-0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `pre5g-0.92/pre5g/__init__.py` & `pre5g-0.93/pre5g/__init__.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.92/pre5g/labelen.py` & `pre5g-0.93/pre5g/labelen.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.92/pre5g/normalization.py` & `pre5g-0.93/pre5g/normalization.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.92/pre5g/onehoten.py` & `pre5g-0.93/pre5g/onehoten.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.92/pre5g/robustscaler.py` & `pre5g-0.93/pre5g/robustscaler.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.92/pre5g/standardization.py` & `pre5g-0.93/pre5g/standardization.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.92/setup.py` & `pre5g-0.93/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pre5g',
-    version='0.92',
+    version='0.93',
     packages=find_packages(),
     description='An preprocessing package',
     author='SnehaM',
     author_email='1js20cs161@gmail.com',
     license='MIT',
     keywords=['example', 'package'],
     classifiers=[
```

