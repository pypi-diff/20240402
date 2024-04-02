# Comparing `tmp/sccastle-1.0.1.tar.gz` & `tmp/sccastle-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sccastle-1.0.1.tar", last modified: Tue Apr  2 04:51:16 2024, max compression
+gzip compressed data, was "sccastle-1.0.2.tar", last modified: Tue Apr  2 05:23:32 2024, max compression
```

## Comparing `sccastle-1.0.1.tar` & `sccastle-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 04:51:16.113214 sccastle-1.0.1/
--rw-rw-rw-   0        0        0     3215 2024-04-02 04:09:28.000000 sccastle-1.0.1/CASTLE.py
--rw-rw-rw-   0        0        0     1064 2024-03-31 14:59:09.000000 sccastle-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      744 2024-04-02 04:51:16.112214 sccastle-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4795 2024-03-31 14:59:09.000000 sccastle-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 04:51:16.099211 sccastle-1.0.1/sccastle/
--rw-rw-rw-   0        0        0      124 2024-04-02 04:09:46.000000 sccastle-1.0.1/sccastle/__init__.py
--rw-rw-rw-   0        0        0    11498 2023-12-29 13:57:50.000000 sccastle-1.0.1/sccastle/data.py
--rw-rw-rw-   0        0        0     1907 2023-08-13 14:15:10.000000 sccastle-1.0.1/sccastle/feature_spectrum.py
--rw-rw-rw-   0        0        0      680 2023-08-13 14:15:10.000000 sccastle-1.0.1/sccastle/logger.py
--rw-rw-rw-   0        0        0     8286 2024-01-31 14:10:40.000000 sccastle-1.0.1/sccastle/main.py
--rw-rw-rw-   0        0        0     2982 2023-08-13 14:15:10.000000 sccastle-1.0.1/sccastle/metrics.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:51:16.111214 sccastle-1.0.1/sccastle/model/
--rw-rw-rw-   0        0        0        0 2023-08-13 14:15:10.000000 sccastle-1.0.1/sccastle/model/__init__.py
--rw-rw-rw-   0        0        0    10718 2023-08-13 14:15:10.000000 sccastle-1.0.1/sccastle/model/castle_train.py
--rw-rw-rw-   0        0        0     7967 2023-08-13 14:15:10.000000 sccastle-1.0.1/sccastle/model/layer.py
--rw-rw-rw-   0        0        0     1741 2023-08-13 14:15:10.000000 sccastle-1.0.1/sccastle/model/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:51:16.105213 sccastle-1.0.1/sccastle.egg-info/
--rw-rw-rw-   0        0        0      744 2024-04-02 04:51:15.000000 sccastle-1.0.1/sccastle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2024-04-02 04:51:15.000000 sccastle-1.0.1/sccastle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 04:51:15.000000 sccastle-1.0.1/sccastle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2024-04-02 04:51:15.000000 sccastle-1.0.1/sccastle.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 04:51:15.000000 sccastle-1.0.1/sccastle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 04:51:16.113214 sccastle-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1178 2024-04-02 04:50:24.000000 sccastle-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 05:23:32.556609 sccastle-1.0.2/
+-rw-rw-rw-   0        0        0     3215 2024-04-02 04:09:28.000000 sccastle-1.0.2/CASTLE.py
+-rw-rw-rw-   0        0        0     1064 2024-03-31 14:59:09.000000 sccastle-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      744 2024-04-02 05:23:32.556609 sccastle-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4795 2024-03-31 14:59:09.000000 sccastle-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 05:23:32.541605 sccastle-1.0.2/sccastle/
+-rw-rw-rw-   0        0        0      124 2024-04-02 05:22:24.000000 sccastle-1.0.2/sccastle/__init__.py
+-rw-rw-rw-   0        0        0    11563 2024-04-02 05:03:34.000000 sccastle-1.0.2/sccastle/data.py
+-rw-rw-rw-   0        0        0     1907 2023-08-13 14:15:10.000000 sccastle-1.0.2/sccastle/feature_spectrum.py
+-rw-rw-rw-   0        0        0      680 2023-08-13 14:15:10.000000 sccastle-1.0.2/sccastle/logger.py
+-rw-rw-rw-   0        0        0     8286 2024-01-31 14:10:40.000000 sccastle-1.0.2/sccastle/main.py
+-rw-rw-rw-   0        0        0     2982 2023-08-13 14:15:10.000000 sccastle-1.0.2/sccastle/metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-02 05:23:32.554608 sccastle-1.0.2/sccastle/model/
+-rw-rw-rw-   0        0        0        0 2023-08-13 14:15:10.000000 sccastle-1.0.2/sccastle/model/__init__.py
+-rw-rw-rw-   0        0        0    10718 2023-08-13 14:15:10.000000 sccastle-1.0.2/sccastle/model/castle_train.py
+-rw-rw-rw-   0        0        0     7967 2023-08-13 14:15:10.000000 sccastle-1.0.2/sccastle/model/layer.py
+-rw-rw-rw-   0        0        0     1741 2023-08-13 14:15:10.000000 sccastle-1.0.2/sccastle/model/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 05:23:32.549607 sccastle-1.0.2/sccastle.egg-info/
+-rw-rw-rw-   0        0        0      744 2024-04-02 05:23:32.000000 sccastle-1.0.2/sccastle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2024-04-02 05:23:32.000000 sccastle-1.0.2/sccastle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 05:23:32.000000 sccastle-1.0.2/sccastle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2024-04-02 05:23:32.000000 sccastle-1.0.2/sccastle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 05:23:32.000000 sccastle-1.0.2/sccastle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 05:23:32.556609 sccastle-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1178 2024-04-02 05:23:05.000000 sccastle-1.0.2/setup.py
```

### Comparing `sccastle-1.0.1/CASTLE.py` & `sccastle-1.0.2/CASTLE.py`

 * *Files identical despite different names*

### Comparing `sccastle-1.0.1/LICENSE` & `sccastle-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sccastle-1.0.1/PKG-INFO` & `sccastle-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sccastle
-Version: 1.0.1
+Version: 1.0.2
 Summary: single-cell Chromatin Accessibility Sequencing data analysis via discreTe Latent Embedding
 Home-page: https://github.com/cuixj19/CASTLE
 Author: Xuejian Cui
 Author-email: cuixj19@mails.tsinghua.edu.cn
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sccastle-1.0.1/README.md` & `sccastle-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sccastle-1.0.1/sccastle/data.py` & `sccastle-1.0.2/sccastle/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,28 +231,29 @@
     sc.pp.filter_cells(adata, min_genes=min_features_)
     
     if log: log.info('Filtering features')
     min_cells_ = np.ceil(min_cells*adata.shape[0]) if type(min_cells) == float else min_cells
     sc.pp.filter_genes(adata, min_cells=min_cells_)
 
     if log: log.info('Calculating TF-IDF')
-    adata = cal_tfidf(adata)
+    adata = cal_tfidf1(adata)
     
     if log: log.info('Normalizing total per cell')
     sc.pp.normalize_total(adata)
     
     if log: log.info('Max-min scaling')
     adata = maxmin_scale(adata)
     
     if log: log.info('Processed dataset shape: {}'.format(adata.shape))
     return adata
 
 
 # Perform Signac TF-IDF (count_mat: cell*peak)
 def cal_tfidf(adata, chunk_size=10000):
+    adata.X = adata.X.todense()
     a = np.sum(adata.X,axis=0)
     b = np.sum(adata.X,axis=1)
     adata.X = adata.X / b
     adata.X = adata.X / a
     c = 1e4 * adata.X.shape[0]
     c1, c2 = 1 / c, np.log(c)
     ct = adata.X.shape[0]/chunk_size
@@ -264,14 +265,15 @@
     else:
         adata.X = np.log(c1 + adata.X)
     adata.X = adata.X + c2
     adata.X = scipy.sparse.csr_matrix(adata.X)
     return adata
 
 def cal_tfidf1(adata):
+    adata.X = adata.X.todense()
     a = np.sum(adata.X,axis=0)
     b = np.sum(adata.X,axis=1)
     adata.X = adata.X / b
     adata.X = adata.X / a
     adata.X = np.log(1 + 1e4 * adata.X.shape[0] * adata.X)
     adata.X = scipy.sparse.csr_matrix(adata.X)
     return adata
```

### Comparing `sccastle-1.0.1/sccastle/feature_spectrum.py` & `sccastle-1.0.2/sccastle/feature_spectrum.py`

 * *Files identical despite different names*

### Comparing `sccastle-1.0.1/sccastle/logger.py` & `sccastle-1.0.2/sccastle/logger.py`

 * *Files identical despite different names*

### Comparing `sccastle-1.0.1/sccastle/main.py` & `sccastle-1.0.2/sccastle/main.py`

 * *Files identical despite different names*

### Comparing `sccastle-1.0.1/sccastle/metrics.py` & `sccastle-1.0.2/sccastle/metrics.py`

 * *Files identical despite different names*

### Comparing `sccastle-1.0.1/sccastle/model/castle_train.py` & `sccastle-1.0.2/sccastle/model/castle_train.py`

 * *Files identical despite different names*

### Comparing `sccastle-1.0.1/sccastle/model/layer.py` & `sccastle-1.0.2/sccastle/model/layer.py`

 * *Files identical despite different names*

### Comparing `sccastle-1.0.1/sccastle/model/utils.py` & `sccastle-1.0.2/sccastle/model/utils.py`

 * *Files identical despite different names*

### Comparing `sccastle-1.0.1/sccastle.egg-info/PKG-INFO` & `sccastle-1.0.2/sccastle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sccastle
-Version: 1.0.1
+Version: 1.0.2
 Summary: single-cell Chromatin Accessibility Sequencing data analysis via discreTe Latent Embedding
 Home-page: https://github.com/cuixj19/CASTLE
 Author: Xuejian Cui
 Author-email: cuixj19@mails.tsinghua.edu.cn
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sccastle-1.0.1/setup.py` & `sccastle-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(name='sccastle',
-      version='1.0.1',
+      version='1.0.2',
       packages=find_packages(),
       description='single-cell Chromatin Accessibility Sequencing data analysis via discreTe Latent Embedding',
       long_description='',
 
       author='Xuejian Cui',
       author_email='cuixj19@mails.tsinghua.edu.cn',
       url="https://github.com/cuixj19/CASTLE",
```

