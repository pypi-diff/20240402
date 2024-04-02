# Comparing `tmp/pre5g-0.91.tar.gz` & `tmp/pre5g-0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pre5g-0.91.tar", last modified: Mon Apr  1 11:34:33 2024, max compression
+gzip compressed data, was "dist/pre5g-0.92.tar", last modified: Tue Apr  2 05:40:17 2024, max compression
```

## Comparing `pre5g-0.91.tar` & `pre5g-0.92.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:34:33.721542 pre5g-0.91/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-0.91/LICENSE
--rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-01 11:34:33.720542 pre5g-0.91/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-0.91/README.md
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:34:33.719542 pre5g-0.91/pre5g/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      650 2024-04-01 11:33:58.000000 pre5g-0.91/pre5g/__init__.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1330 2024-04-01 11:28:19.000000 pre5g-0.91/pre5g/labelen.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-0.91/pre5g/normalization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1319 2024-04-01 11:33:05.000000 pre5g-0.91/pre5g/onehoten.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2679 2024-04-01 11:29:12.000000 pre5g-0.91/pre5g/robustscaler.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:33:29.000000 pre5g-0.91/pre5g/standardization.py
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:34:33.720542 pre5g-0.91/pre5g.egg-info/
--rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-01 11:34:33.000000 pre5g-0.91/pre5g.egg-info/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      265 2024-04-01 11:34:33.000000 pre5g-0.91/pre5g.egg-info/SOURCES.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-01 11:34:33.000000 pre5g-0.91/pre5g.egg-info/dependency_links.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-01 11:34:33.000000 pre5g-0.91/pre5g.egg-info/top_level.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-01 11:34:33.721542 pre5g-0.91/setup.cfg
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      602 2024-04-01 11:34:17.000000 pre5g-0.91/setup.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-02 05:40:17.381939 pre5g-0.92/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-0.92/LICENSE
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-02 05:40:17.381939 pre5g-0.92/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-0.92/README.md
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-02 05:40:17.380939 pre5g-0.92/pre5g/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      650 2024-04-02 05:39:34.000000 pre5g-0.92/pre5g/__init__.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1625 2024-04-02 05:38:57.000000 pre5g-0.92/pre5g/labelen.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-0.92/pre5g/normalization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1589 2024-04-02 05:34:03.000000 pre5g-0.92/pre5g/onehoten.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2679 2024-04-01 11:29:12.000000 pre5g-0.92/pre5g/robustscaler.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-0.92/pre5g/standardization.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-02 05:40:17.380939 pre5g-0.92/pre5g.egg-info/
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-02 05:40:17.000000 pre5g-0.92/pre5g.egg-info/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      265 2024-04-02 05:40:17.000000 pre5g-0.92/pre5g.egg-info/SOURCES.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-02 05:40:17.000000 pre5g-0.92/pre5g.egg-info/dependency_links.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-02 05:40:17.000000 pre5g-0.92/pre5g.egg-info/top_level.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-02 05:40:17.381939 pre5g-0.92/setup.cfg
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      602 2024-04-02 05:39:45.000000 pre5g-0.92/setup.py
```

### Comparing `pre5g-0.91/LICENSE` & `pre5g-0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `pre5g-0.91/pre5g/__init__.py` & `pre5g-0.92/pre5g/__init__.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.91/pre5g/normalization.py` & `pre5g-0.92/pre5g/normalization.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.91/pre5g/robustscaler.py` & `pre5g-0.92/pre5g/robustscaler.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.91/pre5g/standardization.py` & `pre5g-0.92/pre5g/standardization.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.91/setup.py` & `pre5g-0.92/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pre5g',
-    version='0.91',
+    version='0.92',
     packages=find_packages(),
     description='An preprocessing package',
     author='SnehaM',
     author_email='1js20cs161@gmail.com',
     license='MIT',
     keywords=['example', 'package'],
     classifiers=[
```

