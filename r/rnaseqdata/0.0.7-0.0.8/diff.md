# Comparing `tmp/rnaseqdata-0.0.7.tar.gz` & `tmp/rnaseqdata-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnaseqdata-0.0.7.tar", last modified: Mon Mar 25 16:08:56 2024, max compression
+gzip compressed data, was "rnaseqdata-0.0.8.tar", last modified: Mon Apr  1 22:33:15 2024, max compression
```

## Comparing `rnaseqdata-0.0.7.tar` & `rnaseqdata-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:08:56.388526 rnaseqdata-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-03-25 16:08:56.388526 rnaseqdata-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:08:56.388526 rnaseqdata-0.0.7/rnaseqdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-03-25 16:08:56.000000 rnaseqdata-0.0.7/rnaseqdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-25 16:08:56.000000 rnaseqdata-0.0.7/rnaseqdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 16:08:56.000000 rnaseqdata-0.0.7/rnaseqdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-25 16:08:56.000000 rnaseqdata-0.0.7/rnaseqdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-25 16:08:56.000000 rnaseqdata-0.0.7/rnaseqdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 16:08:56.388526 rnaseqdata-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:08:56.384526 rnaseqdata-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:08:56.384526 rnaseqdata-0.0.7/tests/localtests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/tests/localtests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/tests/localtests/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/tests/localtests/test_seq_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/tests/localtests/test_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:08:56.384526 rnaseqdata-0.0.7/tests/unittests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/tests/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/tests/unittests/test_annot_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12525 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/tests/unittests/test_node_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/tests/unittests/test_random_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/tests/unittests/test_root_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/tests/unittests/test_seq_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-25 16:08:48.000000 rnaseqdata-0.0.7/tests/unittests/test_stat_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:33:15.894610 rnaseqdata-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 22:33:11.000000 rnaseqdata-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-01 22:33:15.894610 rnaseqdata-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-01 22:33:11.000000 rnaseqdata-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:33:15.894610 rnaseqdata-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-01 22:33:11.000000 rnaseqdata-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:33:15.890610 rnaseqdata-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:33:15.890610 rnaseqdata-0.0.8/src/rnaseqdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-01 22:33:11.000000 rnaseqdata-0.0.8/src/rnaseqdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-01 22:33:11.000000 rnaseqdata-0.0.8/src/rnaseqdata/annot_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-01 22:33:11.000000 rnaseqdata-0.0.8/src/rnaseqdata/bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-01 22:33:11.000000 rnaseqdata-0.0.8/src/rnaseqdata/node_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-01 22:33:11.000000 rnaseqdata-0.0.8/src/rnaseqdata/random_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-01 22:33:11.000000 rnaseqdata-0.0.8/src/rnaseqdata/root_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-01 22:33:11.000000 rnaseqdata-0.0.8/src/rnaseqdata/seq_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-01 22:33:11.000000 rnaseqdata-0.0.8/src/rnaseqdata/stat_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:33:15.890610 rnaseqdata-0.0.8/src/rnaseqdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-01 22:33:15.000000 rnaseqdata-0.0.8/src/rnaseqdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-01 22:33:15.000000 rnaseqdata-0.0.8/src/rnaseqdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:33:15.000000 rnaseqdata-0.0.8/src/rnaseqdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 22:33:15.000000 rnaseqdata-0.0.8/src/rnaseqdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 22:33:15.000000 rnaseqdata-0.0.8/src/rnaseqdata.egg-info/top_level.txt
```

### Comparing `rnaseqdata-0.0.7/LICENSE` & `rnaseqdata-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rnaseqdata-0.0.7/PKG-INFO` & `rnaseqdata-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rnaseqdata
-Version: 0.0.7
+Version: 0.0.8
 Summary: New Data type known as SeqData for RNA-Seq data analysis
 Home-page: https://github.com/Tiezhengyuan/ernav2_seqdata
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `rnaseqdata-0.0.7/README.md` & `rnaseqdata-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `rnaseqdata-0.0.7/rnaseqdata.egg-info/PKG-INFO` & `rnaseqdata-0.0.8/src/rnaseqdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rnaseqdata
-Version: 0.0.7
+Version: 0.0.8
 Summary: New Data type known as SeqData for RNA-Seq data analysis
 Home-page: https://github.com/Tiezhengyuan/ernav2_seqdata
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `rnaseqdata-0.0.7/setup.py` & `rnaseqdata-0.0.8/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="rnaseqdata",
-    version='0.0.7',
+    version='0.0.8',
     author="Tiezheng Yuan",
     author_email="tiezhengyuan@hotmail.com",
     description="New Data type known as SeqData for RNA-Seq data analysis",
     url = "https://github.com/Tiezhengyuan/ernav2_seqdata",
     long_description_content_type="text/markdown",
     long_description=long_description,
-    packages=find_packages(),
+    package_dir={'': 'src'},
     install_requires=['numpy', 'pandas'],
     keywords=['pypi', 'cicd', 'python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

