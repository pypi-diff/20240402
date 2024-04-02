# Comparing `tmp/pytorch-sidu-1.0.7.tar.gz` & `tmp/pytorch-sidu-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-sidu-1.0.7.tar", last modified: Mon Apr  1 14:29:16 2024, max compression
+gzip compressed data, was "pytorch-sidu-1.0.8.tar", last modified: Mon Apr  1 14:36:23 2024, max compression
```

## Comparing `pytorch-sidu-1.0.7.tar` & `pytorch-sidu-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:16.693052 pytorch-sidu-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35150 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-01 14:29:16.693052 pytorch-sidu-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:16.693052 pytorch-sidu-1.0.7/pytorch_sidu/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/pytorch_sidu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/pytorch_sidu/sidu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:16.693052 pytorch-sidu-1.0.7/pytorch_sidu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-01 14:29:16.000000 pytorch-sidu-1.0.7/pytorch_sidu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-01 14:29:16.000000 pytorch-sidu-1.0.7/pytorch_sidu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:29:16.000000 pytorch-sidu-1.0.7/pytorch_sidu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 14:29:16.000000 pytorch-sidu-1.0.7/pytorch_sidu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 14:29:16.000000 pytorch-sidu-1.0.7/pytorch_sidu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-01 14:29:16.693052 pytorch-sidu-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:36:23.675958 pytorch-sidu-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35150 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-01 14:36:23.675958 pytorch-sidu-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:36:23.675958 pytorch-sidu-1.0.8/pytorch_sidu/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/pytorch_sidu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/pytorch_sidu/sidu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:36:23.675958 pytorch-sidu-1.0.8/pytorch_sidu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/pytorch_sidu/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:36:23.675958 pytorch-sidu-1.0.8/pytorch_sidu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-01 14:36:23.000000 pytorch-sidu-1.0.8/pytorch_sidu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-01 14:36:23.000000 pytorch-sidu-1.0.8/pytorch_sidu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:36:23.000000 pytorch-sidu-1.0.8/pytorch_sidu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 14:36:23.000000 pytorch-sidu-1.0.8/pytorch_sidu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 14:36:23.000000 pytorch-sidu-1.0.8/pytorch_sidu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-01 14:36:23.675958 pytorch-sidu-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/setup.py
```

### Comparing `pytorch-sidu-1.0.7/LICENSE` & `pytorch-sidu-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-sidu-1.0.7/PKG-INFO` & `pytorch-sidu-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-sidu
-Version: 1.0.7
+Version: 1.0.8
 Summary: SIDU: SImilarity Difference and Uniqueness method for explainable AI
 Home-page: https://github.com/MarcoParola/pytorch-sidu
 Author: Marco Parola
 Author-email: marcoparola96@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pytorch-sidu-1.0.7/README.md` & `pytorch-sidu-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-sidu-1.0.7/pytorch_sidu/sidu.py` & `pytorch-sidu-1.0.8/pytorch_sidu/sidu.py`

 * *Files identical despite different names*

### Comparing `pytorch-sidu-1.0.7/pytorch_sidu.egg-info/PKG-INFO` & `pytorch-sidu-1.0.8/pytorch_sidu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-sidu
-Version: 1.0.7
+Version: 1.0.8
 Summary: SIDU: SImilarity Difference and Uniqueness method for explainable AI
 Home-page: https://github.com/MarcoParola/pytorch-sidu
 Author: Marco Parola
 Author-email: marcoparola96@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pytorch-sidu-1.0.7/setup.cfg` & `pytorch-sidu-1.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch-sidu-1.0.7/setup.py` & `pytorch-sidu-1.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     version="0.0.0",
     author="Marco Parola",
     author_email="marcoparola96@gmail.com",
     description="SIDU: SImilarity Difference and Uniqueness method for explainable AI",
     url="https://github.com/MarcoParola/pytorch-sidu",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=["pytorch_sidu"],
+    packages=["pytorch_sidu", "pytorch_sidu.utils"],
     install_requires=requirements,
     setuptools_git_versioning={
         "enabled": True,
     },
     setup_requires=[
         "setuptools-git-versioning<2"
     ],
```

