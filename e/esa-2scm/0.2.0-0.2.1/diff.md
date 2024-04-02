# Comparing `tmp/esa-2scm-0.2.0.tar.gz` & `tmp/esa-2scm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esa-2scm-0.2.0.tar", last modified: Sat Mar 30 13:20:15 2024, max compression
+gzip compressed data, was "esa-2scm-0.2.1.tar", last modified: Tue Apr  2 10:58:05 2024, max compression
```

## Comparing `esa-2scm-0.2.0.tar` & `esa-2scm-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-03-30 13:20:15.535250 esa-2scm-0.2.0/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-28 16:38:21.000000 esa-2scm-0.2.0/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)       87 2024-01-25 20:49:15.000000 esa-2scm-0.2.0/MANIFEST.in
--rw-r--r--   0 soli      (1000) soli      (1000)     6143 2024-03-30 13:20:15.535250 esa-2scm-0.2.0/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)     5856 2024-03-28 16:40:40.000000 esa-2scm-0.2.0/README.md
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-03-30 13:20:15.525250 esa-2scm-0.2.0/esa_2scm/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-28 16:05:50.000000 esa-2scm-0.2.0/esa_2scm/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)      559 2024-03-30 13:17:27.000000 esa-2scm-0.2.0/esa_2scm/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     7824 2024-03-30 13:16:32.000000 esa-2scm-0.2.0/esa_2scm/models.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-03-30 13:20:15.535250 esa-2scm-0.2.0/esa_2scm/syniv/
--rw-r--r--   0 soli      (1000) soli      (1000)      541 2024-03-29 17:57:48.000000 esa-2scm-0.2.0/esa_2scm/syniv/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     5155 2024-03-29 17:57:59.000000 esa-2scm-0.2.0/esa_2scm/syniv/esa.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-03-30 13:20:15.535250 esa-2scm-0.2.0/esa_2scm.egg-info/
--rw-r--r--   0 soli      (1000) soli      (1000)     6143 2024-03-30 13:20:15.000000 esa-2scm-0.2.0/esa_2scm.egg-info/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)      360 2024-03-30 13:20:15.000000 esa-2scm-0.2.0/esa_2scm.egg-info/SOURCES.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-03-30 13:20:15.000000 esa-2scm-0.2.0/esa_2scm.egg-info/dependency_links.txt
--rw-r--r--   0 soli      (1000) soli      (1000)       32 2024-03-30 13:20:15.000000 esa-2scm-0.2.0/esa_2scm.egg-info/requires.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        9 2024-03-30 13:20:15.000000 esa-2scm-0.2.0/esa_2scm.egg-info/top_level.txt
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-03-30 13:20:15.535250 esa-2scm-0.2.0/examples/
--rw-r--r--   0 soli      (1000) soli      (1000)        0 2024-01-24 23:44:02.000000 esa-2scm-0.2.0/examples/tmp.ipynb
--rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-03-30 13:20:15.535250 esa-2scm-0.2.0/setup.cfg
--rw-r--r--   0 soli      (1000) soli      (1000)      664 2024-03-30 13:17:38.000000 esa-2scm-0.2.0/setup.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-03-30 13:20:15.535250 esa-2scm-0.2.0/test/
--rw-r--r--   0 soli      (1000) soli      (1000)     2101 2024-03-28 16:37:14.000000 esa-2scm-0.2.0/test/test_model.py
--rw-r--r--   0 soli      (1000) soli      (1000)     2627 2024-03-23 19:40:59.000000 esa-2scm-0.2.0/test/test_syniv.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-02 10:58:05.780815 esa-2scm-0.2.1/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-28 16:38:21.000000 esa-2scm-0.2.1/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)       87 2024-01-25 20:49:15.000000 esa-2scm-0.2.1/MANIFEST.in
+-rw-r--r--   0 soli      (1000) soli      (1000)     6209 2024-04-02 10:58:05.780815 esa-2scm-0.2.1/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)     5922 2024-04-02 10:57:13.000000 esa-2scm-0.2.1/README.md
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-02 10:58:05.780815 esa-2scm-0.2.1/esa_2scm/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-28 16:05:50.000000 esa-2scm-0.2.1/esa_2scm/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)      559 2024-04-02 10:52:22.000000 esa-2scm-0.2.1/esa_2scm/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     7824 2024-04-02 10:47:30.000000 esa-2scm-0.2.1/esa_2scm/models.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-02 10:58:05.780815 esa-2scm-0.2.1/esa_2scm/syniv/
+-rw-r--r--   0 soli      (1000) soli      (1000)      541 2024-04-02 10:47:01.000000 esa-2scm-0.2.1/esa_2scm/syniv/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     5155 2024-04-02 10:47:08.000000 esa-2scm-0.2.1/esa_2scm/syniv/esa.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-02 10:58:05.780815 esa-2scm-0.2.1/esa_2scm.egg-info/
+-rw-r--r--   0 soli      (1000) soli      (1000)     6209 2024-04-02 10:58:05.000000 esa-2scm-0.2.1/esa_2scm.egg-info/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)      364 2024-04-02 10:58:05.000000 esa-2scm-0.2.1/esa_2scm.egg-info/SOURCES.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-02 10:58:05.000000 esa-2scm-0.2.1/esa_2scm.egg-info/dependency_links.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)       32 2024-04-02 10:58:05.000000 esa-2scm-0.2.1/esa_2scm.egg-info/requires.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        9 2024-04-02 10:58:05.000000 esa-2scm-0.2.1/esa_2scm.egg-info/top_level.txt
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-02 10:58:05.780815 esa-2scm-0.2.1/examples/
+-rw-r--r--   0 soli      (1000) soli      (1000)   134081 2024-04-02 10:51:28.000000 esa-2scm-0.2.1/examples/example.ipynb
+-rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-02 10:58:05.780815 esa-2scm-0.2.1/setup.cfg
+-rw-r--r--   0 soli      (1000) soli      (1000)     1173 2024-04-02 10:50:05.000000 esa-2scm-0.2.1/setup.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-02 10:58:05.780815 esa-2scm-0.2.1/test/
+-rw-r--r--   0 soli      (1000) soli      (1000)     2101 2024-03-28 16:37:14.000000 esa-2scm-0.2.1/test/test_model.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     2627 2024-03-23 19:40:59.000000 esa-2scm-0.2.1/test/test_syniv.py
```

### Comparing `esa-2scm-0.2.0/LICENSE` & `esa-2scm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.0/PKG-INFO` & `esa-2scm-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esa-2scm
-Version: 0.2.0
+Version: 0.2.1
 Summary: ESA-2SCM Python Package for Causal Discovery
 Home-page: https://github.com/DSsoli/esa-2scm.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,15 +13,15 @@
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/DSsoli/esa-2scm/blob/main/LICENSE)
 
 ESA-2SCM is a new method for detecting causality based on Elastic Segment Allocation-based synthetic instrumental variables with 2SLS application for estimating structural causal models. 
 <br>
 <br>
 For details of the model design, please refer to my Original Article:
 
-* [Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 16. <snbperi.org/article/227>](http://www.snbperi.org/article/227)
+* [Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230>](http://www.snbperi.org/article/230)
 
 ## Model Overview
 Suppose that you are interested in discovering the causal relationship between $x_1$ and $x_2$ (e.g., determining the *true causal direction*: $x_1$ -> $x_2$ vs. $x_2$ -> $x_1$, measuring the magnitude of *causal impact*):
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/1.png?raw=true", width="200"/>
 </p>
 
@@ -37,15 +37,15 @@
 
 thus,
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/4.png?raw=true" width="500"/>
 </p>
 
 
-The estimators are also inconsistent, as:
+The estimators are also asymptotically inconsistent, as:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/5.png?raw=true" width="310"/>
 </p>
 
 
 **ESA-2SCM** provides a countermeasure to such problem, enabling the determination of true *causal direction* and estimation of the true *causal coefficient* through the following procedures.
 1. Vector definition:
@@ -61,23 +61,23 @@
 3. Set initial number of segments *(M)*:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/8.png?raw=true" width="500"/>
 </p>
 
 4. Segment size allocation:
 <p align="center">
-  <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/9.png?raw=true" width="400"/>
+  <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/9.png?raw=true" width="460"/>
 </p>
 
 5. Elastic adjustment algorithm for adjusting the number of segments:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/10.png?raw=true" width="580"/>
 </p>
 
-6. Grouping:
+6. Grouping based on the adjusted sizes and number of segments:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/11.png?raw=true" width="450"/>
 </p>
 
 7. Segment value assignment:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/12.png?raw=true" width="420"/>
@@ -147,21 +147,21 @@
 
 # For model summary:
 model.summary()
 ```
 
 ## Documentation
 Original Article of the ESA-2SCM:
-* Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 16. <snbperi.org/article/227> [[ARTICLE LINK]](http://www.snbperi.org/article/227)
+* Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230> [[ARTICLE LINK]](http://www.snbperi.org/article/230)
 
 ## Examples
 Examples of running ESA-2SCM in Jupyter Notebook are included in [esa_2scm/examples](https://github.com/DSsoli/esa-2scm/tree/main/examples)
 
 ## License
 My package is licensed under the terms of the [MIT license](https://github.com/DSsoli/esa-2scm/blob/main/LICENSE)
 
 ## References
 
 ### ESA-2SCM Package
 
 Should you use my package to perform ESA-2SCM for causal discovery, please kindly cite my Original Article:
-* Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 16. <snbperi.org/article/227> [[ARTICLE LINK]](http://www.snbperi.org/article/227)
+* Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230> [[ARTICLE LINK]](http://www.snbperi.org/article/230)
```

### Comparing `esa-2scm-0.2.0/README.md` & `esa-2scm-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/DSsoli/esa-2scm/blob/main/LICENSE)
 
 ESA-2SCM is a new method for detecting causality based on Elastic Segment Allocation-based synthetic instrumental variables with 2SLS application for estimating structural causal models. 
 <br>
 <br>
 For details of the model design, please refer to my Original Article:
 
-* [Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 16. <snbperi.org/article/227>](http://www.snbperi.org/article/227)
+* [Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230>](http://www.snbperi.org/article/230)
 
 ## Model Overview
 Suppose that you are interested in discovering the causal relationship between $x_1$ and $x_2$ (e.g., determining the *true causal direction*: $x_1$ -> $x_2$ vs. $x_2$ -> $x_1$, measuring the magnitude of *causal impact*):
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/1.png?raw=true", width="200"/>
 </p>
 
@@ -27,15 +27,15 @@
 
 thus,
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/4.png?raw=true" width="500"/>
 </p>
 
 
-The estimators are also inconsistent, as:
+The estimators are also asymptotically inconsistent, as:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/5.png?raw=true" width="310"/>
 </p>
 
 
 **ESA-2SCM** provides a countermeasure to such problem, enabling the determination of true *causal direction* and estimation of the true *causal coefficient* through the following procedures.
 1. Vector definition:
@@ -51,23 +51,23 @@
 3. Set initial number of segments *(M)*:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/8.png?raw=true" width="500"/>
 </p>
 
 4. Segment size allocation:
 <p align="center">
-  <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/9.png?raw=true" width="400"/>
+  <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/9.png?raw=true" width="460"/>
 </p>
 
 5. Elastic adjustment algorithm for adjusting the number of segments:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/10.png?raw=true" width="580"/>
 </p>
 
-6. Grouping:
+6. Grouping based on the adjusted sizes and number of segments:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/11.png?raw=true" width="450"/>
 </p>
 
 7. Segment value assignment:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/12.png?raw=true" width="420"/>
@@ -137,21 +137,21 @@
 
 # For model summary:
 model.summary()
 ```
 
 ## Documentation
 Original Article of the ESA-2SCM:
-* Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 16. <snbperi.org/article/227> [[ARTICLE LINK]](http://www.snbperi.org/article/227)
+* Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230> [[ARTICLE LINK]](http://www.snbperi.org/article/230)
 
 ## Examples
 Examples of running ESA-2SCM in Jupyter Notebook are included in [esa_2scm/examples](https://github.com/DSsoli/esa-2scm/tree/main/examples)
 
 ## License
 My package is licensed under the terms of the [MIT license](https://github.com/DSsoli/esa-2scm/blob/main/LICENSE)
 
 ## References
 
 ### ESA-2SCM Package
 
 Should you use my package to perform ESA-2SCM for causal discovery, please kindly cite my Original Article:
-* Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 16. <snbperi.org/article/227> [[ARTICLE LINK]](http://www.snbperi.org/article/227)
+* Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230> [[ARTICLE LINK]](http://www.snbperi.org/article/230)
```

### Comparing `esa-2scm-0.2.0/esa_2scm/LICENSE` & `esa-2scm-0.2.1/esa_2scm/LICENSE`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.0/esa_2scm/__init__.py` & `esa-2scm-0.2.1/esa_2scm/syniv/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """
 The esa-2scm package is an implementation of the ESA-2SCM algorithm (Sanghoon Lee, 2024)
-For documentation and algorithm/methodology details, please refer to my original article: http://www.snbperi.org/article/227
+For documentation and algorithm/methodology details, please refer to my original article: http://www.snbperi.org/article/230
 
 Should you use this package, I kindly request you to cite my article:
-Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 16. <snbperi.org/article/227>
+Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 21. <snbperi.org/article/230>
 """
 
 
-__version__ = "0.2.0"
-
-from .models import Esa2Scm
+from .esa import SynIV, r2_score
```

### Comparing `esa-2scm-0.2.0/esa_2scm/models.py` & `esa-2scm-0.2.1/esa_2scm/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 The esa-2scm package is an implementation of the ESA-2SCM algorithm (Sanghoon Lee, 2024)
-For documentation and algorithm/methodology details, please refer to my original article: http://www.snbperi.org/article/227
+For documentation and algorithm/methodology details, please refer to my original article: http://www.snbperi.org/article/230
 
 Should you use this package, I kindly request you to cite my article:
-Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 16. <snbperi.org/article/227>
+Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 21. <snbperi.org/article/230>
 """
 
 
 import numpy as np
 import pandas as pd
 from typing import Union, List
 from .syniv import SynIV, r2_score
```

### Comparing `esa-2scm-0.2.0/esa_2scm/syniv/__init__.py` & `esa-2scm-0.2.1/esa_2scm/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 The esa-2scm package is an implementation of the ESA-2SCM algorithm (Sanghoon Lee, 2024)
-For documentation and algorithm/methodology details, please refer to my original article: http://www.snbperi.org/article/227
+For documentation and algorithm/methodology details, please refer to my original article: http://www.snbperi.org/article/230
 
 Should you use this package, I kindly request you to cite my article:
-Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 16. <snbperi.org/article/227>
+Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 21. <snbperi.org/article/230>
 """
 
 
-from .esa import SynIV, r2_score
+__version__ = "0.2.1"
+
+from .models import Esa2Scm
```

### Comparing `esa-2scm-0.2.0/esa_2scm/syniv/esa.py` & `esa-2scm-0.2.1/esa_2scm/syniv/esa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 The esa-2scm package is an implementation of the ESA-2SCM algorithm (Sanghoon Lee, 2024)
-For documentation and algorithm/methodology details, please refer to my original article: http://www.snbperi.org/article/227
+For documentation and algorithm/methodology details, please refer to my original article: http://www.snbperi.org/article/230
 
 Should you use this package, I kindly request you to cite my article:
-Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 16. <snbperi.org/article/227>
+Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 21. <snbperi.org/article/230>
 """
 
 
 import numpy as np
 import scipy.stats as ss
 import warnings
```

### Comparing `esa-2scm-0.2.0/esa_2scm.egg-info/PKG-INFO` & `esa-2scm-0.2.1/esa_2scm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esa-2scm
-Version: 0.2.0
+Version: 0.2.1
 Summary: ESA-2SCM Python Package for Causal Discovery
 Home-page: https://github.com/DSsoli/esa-2scm.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,15 +13,15 @@
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/DSsoli/esa-2scm/blob/main/LICENSE)
 
 ESA-2SCM is a new method for detecting causality based on Elastic Segment Allocation-based synthetic instrumental variables with 2SLS application for estimating structural causal models. 
 <br>
 <br>
 For details of the model design, please refer to my Original Article:
 
-* [Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 16. <snbperi.org/article/227>](http://www.snbperi.org/article/227)
+* [Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230>](http://www.snbperi.org/article/230)
 
 ## Model Overview
 Suppose that you are interested in discovering the causal relationship between $x_1$ and $x_2$ (e.g., determining the *true causal direction*: $x_1$ -> $x_2$ vs. $x_2$ -> $x_1$, measuring the magnitude of *causal impact*):
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/1.png?raw=true", width="200"/>
 </p>
 
@@ -37,15 +37,15 @@
 
 thus,
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/4.png?raw=true" width="500"/>
 </p>
 
 
-The estimators are also inconsistent, as:
+The estimators are also asymptotically inconsistent, as:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/5.png?raw=true" width="310"/>
 </p>
 
 
 **ESA-2SCM** provides a countermeasure to such problem, enabling the determination of true *causal direction* and estimation of the true *causal coefficient* through the following procedures.
 1. Vector definition:
@@ -61,23 +61,23 @@
 3. Set initial number of segments *(M)*:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/8.png?raw=true" width="500"/>
 </p>
 
 4. Segment size allocation:
 <p align="center">
-  <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/9.png?raw=true" width="400"/>
+  <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/9.png?raw=true" width="460"/>
 </p>
 
 5. Elastic adjustment algorithm for adjusting the number of segments:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/10.png?raw=true" width="580"/>
 </p>
 
-6. Grouping:
+6. Grouping based on the adjusted sizes and number of segments:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/11.png?raw=true" width="450"/>
 </p>
 
 7. Segment value assignment:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/12.png?raw=true" width="420"/>
@@ -147,21 +147,21 @@
 
 # For model summary:
 model.summary()
 ```
 
 ## Documentation
 Original Article of the ESA-2SCM:
-* Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 16. <snbperi.org/article/227> [[ARTICLE LINK]](http://www.snbperi.org/article/227)
+* Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230> [[ARTICLE LINK]](http://www.snbperi.org/article/230)
 
 ## Examples
 Examples of running ESA-2SCM in Jupyter Notebook are included in [esa_2scm/examples](https://github.com/DSsoli/esa-2scm/tree/main/examples)
 
 ## License
 My package is licensed under the terms of the [MIT license](https://github.com/DSsoli/esa-2scm/blob/main/LICENSE)
 
 ## References
 
 ### ESA-2SCM Package
 
 Should you use my package to perform ESA-2SCM for causal discovery, please kindly cite my Original Article:
-* Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 16. <snbperi.org/article/227> [[ARTICLE LINK]](http://www.snbperi.org/article/227)
+* Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230> [[ARTICLE LINK]](http://www.snbperi.org/article/230)
```

### Comparing `esa-2scm-0.2.0/test/test_model.py` & `esa-2scm-0.2.1/test/test_model.py`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.0/test/test_syniv.py` & `esa-2scm-0.2.1/test/test_syniv.py`

 * *Files identical despite different names*

