# Comparing `tmp/python-ldl-0.0.1.tar.gz` & `tmp/python-ldl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ldl-0.0.1.tar", last modified: Tue Mar  5 09:07:48 2024, max compression
+gzip compressed data, was "python-ldl-0.0.2.tar", last modified: Tue Apr  2 09:09:38 2024, max compression
```

## Comparing `python-ldl-0.0.1.tar` & `python-ldl-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 09:07:48.992646 python-ldl-0.0.1/
--rw-rw-rw-   0        0        0     1069 2024-03-05 05:55:53.000000 python-ldl-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    10308 2024-03-05 09:07:48.972304 python-ldl-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9522 2024-03-05 08:26:19.000000 python-ldl-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-05 09:07:48.521573 python-ldl-0.0.1/pyldl/
--rw-rw-rw-   0        0        0       14 2024-03-05 08:56:24.000000 python-ldl-0.0.1/pyldl/__init__.py
--rw-rw-rw-   0        0        0    49414 2024-03-05 08:56:07.000000 python-ldl-0.0.1/pyldl/algorithms.py
-drwxrwxrwx   0        0        0        0 2024-03-05 09:07:48.955177 python-ldl-0.0.1/pyldl/matlab_algorithms/
--rw-rw-rw-   0        0        0       36 2023-12-06 07:12:54.000000 python-ldl-0.0.1/pyldl/matlab_algorithms/AA_BP_fit.m
--rw-rw-rw-   0        0        0      245 2023-12-06 07:12:54.000000 python-ldl-0.0.1/pyldl/matlab_algorithms/AA_BP_predict.m
--rw-rw-rw-   0        0        0       95 2023-12-06 07:12:54.000000 python-ldl-0.0.1/pyldl/matlab_algorithms/AA_KNN.m
--rw-rw-rw-   0        0        0      346 2023-12-06 07:12:54.000000 python-ldl-0.0.1/pyldl/matlab_algorithms/BFGS_Process.m
--rw-rw-rw-   0        0        0       41 2023-12-06 07:12:54.000000 python-ldl-0.0.1/pyldl/matlab_algorithms/PT_Bayes_fit.m
--rw-rw-rw-   0        0        0      114 2023-12-06 07:12:54.000000 python-ldl-0.0.1/pyldl/matlab_algorithms/PT_Bayes_predict.m
--rw-rw-rw-   0        0        0       81 2023-12-06 07:12:54.000000 python-ldl-0.0.1/pyldl/matlab_algorithms/PT_SVM_fit.m
--rw-rw-rw-   0        0        0       94 2023-12-06 07:12:54.000000 python-ldl-0.0.1/pyldl/matlab_algorithms/PT_SVM_predict.m
--rw-rw-rw-   0        0        0      102 2023-12-06 07:12:54.000000 python-ldl-0.0.1/pyldl/matlab_algorithms/SA_BFGS_fit.m
--rw-rw-rw-   0        0        0       50 2023-12-06 07:12:54.000000 python-ldl-0.0.1/pyldl/matlab_algorithms/SA_BFGS_predict.m
--rw-rw-rw-   0        0        0      136 2023-12-06 07:12:54.000000 python-ldl-0.0.1/pyldl/matlab_algorithms/SA_IIS_fit.m
--rw-rw-rw-   0        0        0       50 2023-12-06 07:12:54.000000 python-ldl-0.0.1/pyldl/matlab_algorithms/SA_IIS_predict.m
--rw-rw-rw-   0        0        0     4840 2024-03-05 08:56:50.000000 python-ldl-0.0.1/pyldl/matlab_algorithms/__init__.py
--rw-rw-rw-   0        0        0     2582 2023-12-16 07:43:15.000000 python-ldl-0.0.1/pyldl/metrics.py
--rw-rw-rw-   0        0        0     3334 2024-03-05 07:36:42.000000 python-ldl-0.0.1/pyldl/rprop.py
--rw-rw-rw-   0        0        0     2984 2024-03-05 08:56:37.000000 python-ldl-0.0.1/pyldl/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-05 09:07:48.972304 python-ldl-0.0.1/python_ldl.egg-info/
--rw-rw-rw-   0        0        0    10308 2024-03-05 09:07:48.000000 python-ldl-0.0.1/python_ldl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      782 2024-03-05 09:07:48.000000 python-ldl-0.0.1/python_ldl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 09:07:48.000000 python-ldl-0.0.1/python_ldl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-03-05 09:07:48.000000 python-ldl-0.0.1/python_ldl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-05 09:07:48.000000 python-ldl-0.0.1/python_ldl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-05 09:07:48.992646 python-ldl-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1194 2024-03-05 09:05:58.000000 python-ldl-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:09:38.567452 python-ldl-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 09:09:31.000000 python-ldl-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-04-02 09:09:38.567452 python-ldl-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-02 09:09:31.000000 python-ldl-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:09:38.559452 python-ldl-0.0.2/pyldl/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:09:38.563452 python-ldl-0.0.2/pyldl/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9886 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/algorithms/_algorithm_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/algorithms/_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/algorithms/_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/algorithms/_incomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12352 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/algorithms/_label_enhancement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/algorithms/_ldl_lrr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/algorithms/_ldl_scl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/algorithms/_ldlf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/algorithms/_problem_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/algorithms/_specialized_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/algorithms/_ssg_ldl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/algorithms/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:09:38.563452 python-ldl-0.0.2/pyldl/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/applications/emphasis_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/applications/facial_emotion_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/applications/lesion_counting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:09:38.567452 python-ldl-0.0.2/pyldl/matlab_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/matlab_algorithms/AA_BP_fit.m
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/matlab_algorithms/AA_BP_predict.m
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/matlab_algorithms/AA_KNN.m
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/matlab_algorithms/BFGS_Process.m
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/matlab_algorithms/PT_Bayes_fit.m
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/matlab_algorithms/PT_Bayes_predict.m
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/matlab_algorithms/PT_SVM_fit.m
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/matlab_algorithms/PT_SVM_predict.m
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/matlab_algorithms/SA_BFGS_fit.m
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/matlab_algorithms/SA_BFGS_predict.m
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/matlab_algorithms/SA_IIS_fit.m
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/matlab_algorithms/SA_IIS_predict.m
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/matlab_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-02 09:09:31.000000 python-ldl-0.0.2/pyldl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:09:38.567452 python-ldl-0.0.2/python_ldl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-04-02 09:09:38.000000 python-ldl-0.0.2/python_ldl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-02 09:09:38.000000 python-ldl-0.0.2/python_ldl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:09:38.000000 python-ldl-0.0.2/python_ldl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 09:09:38.000000 python-ldl-0.0.2/python_ldl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 09:09:38.000000 python-ldl-0.0.2/python_ldl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:09:38.567452 python-ldl-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-02 09:09:31.000000 python-ldl-0.0.2/setup.py
```

### Comparing `python-ldl-0.0.1/LICENSE` & `python-ldl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ldl-0.0.1/PKG-INFO` & `python-ldl-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,170 +1,163 @@
-Metadata-Version: 2.1
-Name: python-ldl
-Version: 0.0.1
-Summary: Label distribution learning (LDL) and label enhancement (LE) toolkit implemented in python.
-Home-page: https://github.com/SpriteMisaka/PyLDL
-Author: SpriteMisaka
-Author-email: SpriteMisaka@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: qpsolvers
-Requires-Dist: quadprog
-Requires-Dist: scikit-fuzzy
-Requires-Dist: scikit-learn
-Requires-Dist: scipy
-Requires-Dist: tensorflow
-Requires-Dist: tensorflow-addons
-Requires-Dist: tensorflow-probability
-
-# PyLDL
-
-Label distribution learning (LDL) and label enhancement (LE) toolkit implemented in python, including:
-
-+ LDL algorithms:
-  + ([Geng, Yin, and Zhou 2013](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2013.pdf))[*TPAMI*]: `CPNN`$^1$.
-  + ([Geng and Hou 2015](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2015.pdf))[*IJCAI*]: `LDSVR`.
-  + ⭐([Geng 2016](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2016.pdf))[*TKDE*]: `SA_BFGS`, `SA_IIS`, `AA_KNN`, `AA_BP`, `PT_Bayes`, and `PT_SVM`.
-  + ([Yang, Sun, and Sun 2017](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/yang2017.pdf))[*AAAI*]: `BCPNN` and `ACPNN`.
-  + ([Xu and Zhou 2017](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/xu2017.pdf))[*IJCAI*]: `IncomLDL`$^2$.
-  + ([Shen et al. 2017](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/shen2017.pdf))[*NeurIPS*]: `LDLF`.
-  + ([Wang and Geng 2019](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wang2019.pdf))[*IJCAI*]: `LDL4C`$^3$.
-  + ([Shen et al. 2020](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/shen2020.pdf))[*南京理工大学学报* (Chinese)]: `AdaBoostLDL`.
-  + ([González et al. 2021a](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/gonz%C3%A1lez2021a.pdf))[*Information Sciences*]: `SSG_LDL`$^4$.
-  + ([González et al. 2021b](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/gonz%C3%A1lez2021b.pdf))[*Information Fusion*]: `DF_LDL`.
-  + ([Wang and Geng 2021a](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wang2021a.pdf))[*IJCAI*]: `LDL_HR`$^3$.
-  + ([Wang and Geng 2021b](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wang2021b.pdf))[*ICML*]: `LDLM`$^3$.
-  + ([Jia et al. 2021](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/jia2021.pdf))[*TKDE*]: `LDL_SCL`.
-  + ([Jia et al. 2023](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/jia2023.pdf))[*TKDE*]: `LDL_LRR`.
-  + ([Wen et al. 2023](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wen2023.pdf))[*ICCV*]: `CAD`$^1$, `QFD2`$^1$, and `CJS`$^1$.
-+ LE algorithms:
-  + ([Xu, Liu, and Geng 2019](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/xu2019.pdf))[*TKDE*]: `FCM`, `KM`, `LP`, `ML`, and `GLLE`.
-  + ([Xu et al. 2020](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/xu2020.pdf))[*ICML*]: `LEVI`.
-  + ([Zheng, Zhu, and Tang 2023](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/zheng2023.pdf))[*CVPR*]: `LIBLE`.
-  
-+ LDL metrics: `chebyshev`, `clark`, `canberra`, `kl_divergence`, `cosine`, `intersection`, etc.
-+ LDL datasets: *Human_Gene*, *Movie*, *Natural_Scene*, *s-BU_3DFE*, *s-JAFFE*, *Yeast*, etc.
-
-> $^1$ Technically, these methods are only suitable for totally ordered labels.
->
-> $^2$ These are algorithms for incomplete LDL, so you should use `utils.random_missing` to generate the missing label distribution matrix and the corresponding mask matrix in the experiments.
->
-> $^3$ These are LDL classifiers, so you should use `predict_proba` to get label distributions and `predict` to get predicted labels.
->
-> $^4$ These are oversampling algorithms for LDL, therefore you should use `fit_transform` to generate synthetic samples.
-
-## Usage
-
-Here is an example of using PyLDL.
-
-```python
-from pyldl.utils import load_dataset
-from pyldl.algorithms import SA_BFGS
-from pyldl.metrics import score
-
-from sklearn.model_selection import train_test_split
-
-dataset_name = 'SJAFFE'
-X, y = load_dataset(dataset_name)
-X_train, X_test, y_train, y_test = train_test_split(X, y)
-
-model = SA_BFGS()
-model.fit(X_train, y_train)
-
-y_pred = model.predict(X_test)
-print(score(y_test, y_pred))
-```
-
-For those who would like to use the original implementation:
-
-1. Install MATLAB.
-2. Install MATLAB engine for python.
-3. Download LDL Package from [here](http://palm.seu.edu.cn/xgeng/LDL/download.htm).
-3. Get the package directory of PyLDL (...\\Lib\\site-packages\\pyldl).
-4. Place the *LDLPackage_v1.2* folder into the *matlab_algorithms* folder.
-
-Now, you can load the original implementation of the method, e.g.:
-
-```python
-from pyldl.matlab_algorithms import SA_IIS
-```
-
-You can visualize the performance of any model on the artificial dataset ([Geng 2016](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2016.pdf)) with the `pyldl.utils.plot_artificial` function, e.g.:
-
-```python
-from pyldl.algorithms import LDSVR, SA_BFGS, SA_IIS, AA_KNN, PT_Bayes, GLLE, LIBLE
-from pyldl.utils import plot_artificial
-
-methods = ['LDSVR', 'SA_BFGS', 'SA_IIS', 'AA_KNN', 'PT_Bayes', 'GLLE', 'LIBLE']
-
-plot_artificial(model=None, figname='GT')
-for i in methods:
-    plot_artificial(model=eval(f'{i}()'), figname=i)
-```
-
-The output images are as follows.
-
-| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/GT.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/LDSVR.jpg?raw=true" width=300> |
-| :----------------------------------------------------------: | :----------------------------------------------------------: |
-|                        (Ground Truth)                        |                           `LDSVR`                            |
-
-| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/SA_BFGS.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/SA_IIS.jpg?raw=true" width=300> |
-| :----------------------------------------------------------: | :----------------------------------------------------------: |
-|                          `SA_BFGS`                           |                           `SA_IIS`                           |
-
-| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/AA_KNN.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/PT_Bayes.jpg?raw=true" width=300> |
-| :----------------------------------------------------------: | :----------------------------------------------------------: |
-|                           `AA_KNN`                           |                          `PT_Bayes`                          |
-
-| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/GLLE.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/LIBLE.jpg?raw=true" width=300> |
-| :----------------------------------------------------------: | :----------------------------------------------------------: |
-|                            `GLLE`                            |                           `LIBLE`                            |
-
-Enjoy! :)
-
-## Experiments
-
-For each algorithm, a ten-fold cross validation is performed, repeated 10 times with *s-JAFFE* dataset and the average metrics are recorded. Therefore, the results do not fully describe the performance of the model.
-
-Results of ours are as follows.
-
-| Algorithm |    Cheby.(↓)    |    Clark(↓)     |     Can.(↓)     |     K-L(↓)      |     Cos.(↑)     |     Int.(↑)     |
-| :-------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: |
-|  SA-BFGS  | **.092 ± .010** |   .361 ± .029   |   .735 ± .060   | **.051 ± .009** | **.954 ± .009** | **.878 ± .011** |
-|  SA-IIS   |   .100 ± .009   |   .361 ± .023   |   .746 ± .050   | **.051 ± .008** |   .952 ± .007   |   .873 ± .009   |
-|  AA-kNN   |   .098 ± .011   | **.349 ± .029** | **.716 ± .062** |   .053 ± .010   |   .950 ± .009   |   .877 ± .011   |
-|   AA-BP   |   .120 ± .012   |   .426 ± .025   |   .889 ± .057   |   .073 ± .010   |   .931 ± .010   |   .848 ± .011   |
-| PT-Bayes  |   .116 ± .011   |   .425 ± .031   |   .874 ± .064   |   .073 ± .012   |   .932 ± .011   |   .850 ± .012   |
-|  PT-SVM   |   .117 ± .012   |   .422 ± .027   |   .875 ± .057   |   .072 ± .011   |   .932 ± .011   |   .850 ± .011   |
-
-Results of the original MATLAB implementation ([Geng 2016](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2016.pdf)) are as follows.
-
-| Algorithm |    Cheby.(↓)    |    Clark(↓)     |     Can.(↓)     |     K-L(↓)      |     Cos.(↑)     |     Int.(↑)     |
-| :-------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: |
-|  SA-BFGS  | **.107 ± .015** | **.399 ± .044** | **.820 ± .103** | **.064 ± .016** | **.940 ± .015** | **.860 ± .019** |
-|  SA-IIS   |   .117 ± .015   |   .419 ± .034   |   .875 ± .086   |   .070 ± .012   |   .934 ± .012   |   .851 ± .016   |
-|  AA-kNN   |   .114 ± .017   |   .410 ± .050   |   .843 ± .113   |   .071 ± .023   |   .934 ± .018   |   .855 ± .021   |
-|   AA-BP   |   .130 ± .017   |   .510 ± .054   |   1.05 ± .124   |   .113 ± .030   |   .908 ± .019   |   .824 ± .022   |
-| PT-Bayes  |   .121 ± .016   |   .430 ± .035   |   .904 ± .086   |   .074 ± .014   |   .930 ± .016   |   .846 ± .016   |
-|  PT-SVM   |   .127 ± .017   |   .457 ± .039   |   .935 ± .074   |   .086 ± .016   |   .920 ± .014   |   .839 ± .015   |
-
-## Requirements
-
-```
-matplotlib>=3.6.1
-numpy>=1.22.3
-qpsolvers>=4.0.0
-quadprog>=0.1.11
-scikit-fuzzy>=0.4.2
-scikit-learn>=1.0.2
-scipy>=1.8.0
-tensorflow>=2.8.0
-tensorflow-addons>=0.22.0
-tensorflow-probability>=0.16.0
-```
-
+# PyLDL
+
+Label distribution learning (LDL) and label enhancement (LE) toolkit implemented in python, including:
+
++ LDL algorithms:
+  + ([Geng, Yin, and Zhou 2013](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2013.pdf))[*TPAMI*]: `CPNN`$^1$.
+  + ([Geng and Hou 2015](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2015.pdf))[*IJCAI*]: `LDSVR`.
+  + ⭐([Geng 2016](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2016.pdf))[*TKDE*]: `SA_BFGS`, `SA_IIS`, `AA_KNN`, `AA_BP`, `PT_Bayes`, and `PT_SVM`.
+  + ([Yang, Sun, and Sun 2017](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/yang2017.pdf))[*AAAI*]: `BCPNN` and `ACPNN`.
+  + ([Xu and Zhou 2017](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/xu2017.pdf))[*IJCAI*]: `IncomLDL`$^2$.
+  + ([Shen et al. 2017](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/shen2017.pdf))[*NeurIPS*]: `LDLF`.
+  + ([Wang and Geng 2019](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wang2019.pdf))[*IJCAI*]: `LDL4C`$^3$.
+  + ([Shen et al. 2020](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/shen2020.pdf))[*南京理工大学学报* (Chinese)]: `AdaBoostLDL`.
+  + ([González et al. 2021a](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/gonz%C3%A1lez2021a.pdf))[*Information Sciences*]: `SSG_LDL`$^4$.
+  + ([González et al. 2021b](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/gonz%C3%A1lez2021b.pdf))[*Information Fusion*]: `DF_LDL`.
+  + ([Wang and Geng 2021a](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wang2021a.pdf))[*IJCAI*]: `LDL_HR`$^3$.
+  + ([Wang and Geng 2021b](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wang2021b.pdf))[*ICML*]: `LDLM`$^3$.
+  + ([Jia et al. 2021](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/jia2021.pdf))[*TKDE*]: `LDL_SCL`.
+  + ([Jia et al. 2023](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/jia2023.pdf))[*TKDE*]: `LDL_LRR`.
+  + ([Wen et al. 2023](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wen2023.pdf))[*ICCV*]: `CAD`$^1$, `QFD2`$^1$, and `CJS`$^1$.
++ LE algorithms:
+  + ([Xu, Liu, and Geng 2019](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/xu2019.pdf))[*TKDE*]: `FCM`, `KM`, `LP`, `ML`, and `GLLE`.
+  + ([Xu et al. 2020](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/xu2020.pdf))[*ICML*]: `LEVI`.
+  + ([Zheng, Zhu, and Tang 2023](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/zheng2023.pdf))[*CVPR*]: `LIBLE`.
++ LDL metrics: `chebyshev`, `clark`, `canberra`, `kl_divergence`, `cosine`, `intersection`, etc.
++ Structured LDL datasets: *Human_Gene*, *Movie*, *Natural_Scene*, *s-BU_3DFE*, *s-JAFFE*, *Yeast*, etc.
++ LDL applications:
+  + Facial emotion recognition (supported datasets: [*JAFFE*](https://zenodo.org/records/3451524)).
+  + ([Shirani et al. 2019](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/shirani2019.pdf))[*ACL*]: Emphasis selection (supported datasets: [*SemEval2020*](https://github.com/RiTUAL-UH/SemEval2020_Task10_Emphasis_Selection); pre-trained GloVe embeddings can be downloaded [here](https://nlp.stanford.edu/projects/glove/)).
+  + ([Wu et al. 2019](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wu2019.pdf))[*ICCV*]: Lesion counting (supported datasets: [*ACNE04*](https://drive.google.com/drive/folders/18yJcHXhzOv7H89t-Lda6phheAicLqMuZ)).
+
+> $^1$ Technically, these methods are only suitable for totally ordered labels.
+>
+> $^2$ These are algorithms for incomplete LDL, so you should use `pyldl.utils.random_missing` to generate the missing label distribution matrix and the corresponding mask matrix in the experiments.
+>
+> $^3$ These are LDL classifiers, so you should use `predict_proba` to get label distributions and `predict` to get predicted labels.
+>
+> $^4$ These are oversampling algorithms for LDL, therefore you should use `fit_transform` to generate synthetic samples.
+
+## Installation
+
+PyLDL is now available on [PyPI](https://pypi.org/project/python-ldl/). Use the following command to install.
+
+```shell
+pip install python-ldl
+```
+
+To install the newest version, you can clone this repo and run the `setup.py` file.
+
+```shell
+python setup.py install
+```
+
+## Usage
+
+Here is an example of using PyLDL.
+
+```python
+from pyldl.utils import load_dataset
+from pyldl.algorithms import SA_BFGS
+from pyldl.metrics import score
+
+from sklearn.model_selection import train_test_split
+
+dataset_name = 'SJAFFE'
+X, y = load_dataset(dataset_name)
+X_train, X_test, y_train, y_test = train_test_split(X, y)
+
+model = SA_BFGS()
+model.fit(X_train, y_train)
+
+y_pred = model.predict(X_test)
+print(score(y_test, y_pred))
+```
+
+For those who would like to use the original implementation:
+
+1. Install MATLAB.
+2. Install MATLAB engine for python.
+3. Download LDL Package [here](http://palm.seu.edu.cn/xgeng/LDL/download.htm).
+3. Get the package directory of PyLDL (...\\Lib\\site-packages\\pyldl).
+4. Place the *LDLPackage_v1.2* folder into the *matlab_algorithms* folder.
+
+Now, you can load the original implementation of the method, e.g.:
+
+```python
+from pyldl.matlab_algorithms import SA_IIS
+```
+
+You can visualize the performance of any model on the artificial dataset ([Geng 2016](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2016.pdf)) with the `pyldl.utils.plot_artificial` function, e.g.:
+
+```python
+from pyldl.algorithms import LDSVR, SA_BFGS, SA_IIS, AA_KNN, PT_Bayes, GLLE, LIBLE
+from pyldl.utils import plot_artificial
+
+methods = ['LDSVR', 'SA_BFGS', 'SA_IIS', 'AA_KNN', 'PT_Bayes', 'GLLE', 'LIBLE']
+
+plot_artificial(model=None, figname='GT')
+for i in methods:
+    plot_artificial(model=eval(f'{i}()'), figname=i)
+```
+
+The output images are as follows.
+
+| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/GT.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/LDSVR.jpg?raw=true" width=300> |
+| :----------------------------------------------------------: | :----------------------------------------------------------: |
+|                        (Ground Truth)                        |                           `LDSVR`                            |
+
+| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/SA_BFGS.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/SA_IIS.jpg?raw=true" width=300> |
+| :----------------------------------------------------------: | :----------------------------------------------------------: |
+|                          `SA_BFGS`                           |                           `SA_IIS`                           |
+
+| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/AA_KNN.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/PT_Bayes.jpg?raw=true" width=300> |
+| :----------------------------------------------------------: | :----------------------------------------------------------: |
+|                           `AA_KNN`                           |                          `PT_Bayes`                          |
+
+| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/GLLE.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/LIBLE.jpg?raw=true" width=300> |
+| :----------------------------------------------------------: | :----------------------------------------------------------: |
+|                            `GLLE`                            |                           `LIBLE`                            |
+
+Enjoy! :)
+
+## Experiments
+
+For each algorithm, a ten-fold cross validation is performed, repeated 10 times with *s-JAFFE* dataset and the average metrics are recorded. Therefore, the results do not fully describe the performance of the model.
+
+Results of ours are as follows.
+
+| Algorithm |    Cheby.(↓)    |    Clark(↓)     |     Can.(↓)     |     K-L(↓)      |     Cos.(↑)     |     Int.(↑)     |
+| :-------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: |
+|  SA-BFGS  | **.092 ± .010** |   .361 ± .029   |   .735 ± .060   | **.051 ± .009** | **.954 ± .009** | **.878 ± .011** |
+|  SA-IIS   |   .100 ± .009   |   .361 ± .023   |   .746 ± .050   | **.051 ± .008** |   .952 ± .007   |   .873 ± .009   |
+|  AA-kNN   |   .098 ± .011   | **.349 ± .029** | **.716 ± .062** |   .053 ± .010   |   .950 ± .009   |   .877 ± .011   |
+|   AA-BP   |   .120 ± .012   |   .426 ± .025   |   .889 ± .057   |   .073 ± .010   |   .931 ± .010   |   .848 ± .011   |
+| PT-Bayes  |   .116 ± .011   |   .425 ± .031   |   .874 ± .064   |   .073 ± .012   |   .932 ± .011   |   .850 ± .012   |
+|  PT-SVM   |   .117 ± .012   |   .422 ± .027   |   .875 ± .057   |   .072 ± .011   |   .932 ± .011   |   .850 ± .011   |
+
+Results of the original MATLAB implementation ([Geng 2016](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2016.pdf)) are as follows.
+
+| Algorithm |    Cheby.(↓)    |    Clark(↓)     |     Can.(↓)     |     K-L(↓)      |     Cos.(↑)     |     Int.(↑)     |
+| :-------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: |
+|  SA-BFGS  | **.107 ± .015** | **.399 ± .044** | **.820 ± .103** | **.064 ± .016** | **.940 ± .015** | **.860 ± .019** |
+|  SA-IIS   |   .117 ± .015   |   .419 ± .034   |   .875 ± .086   |   .070 ± .012   |   .934 ± .012   |   .851 ± .016   |
+|  AA-kNN   |   .114 ± .017   |   .410 ± .050   |   .843 ± .113   |   .071 ± .023   |   .934 ± .018   |   .855 ± .021   |
+|   AA-BP   |   .130 ± .017   |   .510 ± .054   |   1.05 ± .124   |   .113 ± .030   |   .908 ± .019   |   .824 ± .022   |
+| PT-Bayes  |   .121 ± .016   |   .430 ± .035   |   .904 ± .086   |   .074 ± .014   |   .930 ± .016   |   .846 ± .016   |
+|  PT-SVM   |   .127 ± .017   |   .457 ± .039   |   .935 ± .074   |   .086 ± .016   |   .920 ± .014   |   .839 ± .015   |
+
+## Requirements
+
+```
+matplotlib>=3.6.1
+numpy>=1.22.3
+qpsolvers>=4.0.0
+quadprog>=0.1.11
+scikit-fuzzy>=0.4.2
+scikit-learn>=1.0.2
+scipy>=1.8.0
+tensorflow>=2.8.0
+tensorflow-addons>=0.22.0
+tensorflow-probability>=0.16.0
+```
+
```

### Comparing `python-ldl-0.0.1/pyldl/matlab_algorithms/__init__.py` & `python-ldl-0.0.2/pyldl/matlab_algorithms/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-import io
-import os
-import numpy as np
-import matlab.engine
-
-from pyldl.algorithms import BaseLDL
-
-eng = matlab.engine.start_matlab()
-
-def _set_arr(name, arr):
-    eng.eval(f'global {name}', nargout=0)
-    eng.workspace[f'{name}'] = matlab.double(arr.tolist())
-
-
-def _get_arr(name):
-    with io.StringIO() as target:
-        eng.eval(f'tmp = {name}', nargout=0, stdout=target)
-    return np.array(eng.workspace['tmp'])
-
-
-class BaseMatlabLDL(BaseLDL):
-
-    class MatlabLDLExec:
-
-        def __enter__(self):
-            eng.cd(f'{os.path.dirname(os.path.abspath(__file__))}', nargout=0)
-            eng.eval(r'addpath("./LDLPackage_v1.2")', nargout=0)
-
-        def __exit__(self, exc_type, exc_val, exc_tb):
-            eng.eval('clear;', nargout=0)
-            eng.eval('clc;', nargout=0)
-            eng.eval(r'rmpath("./LDLPackage_v1.2")', nargout=0)
-            eng.cd(r'..', nargout=0)
-
-    def __init__(self, info_python=None, info_matlab=None, random_state=None):
-        super().__init__(random_state)
-        self._info_python, self._info_matlab = info_python, info_matlab
-        exec(f"self._{self._info_python} = None")
-    
-    def fit(self, X, y):
-        super().fit(X, y)
-
-        with BaseMatlabLDL.MatlabLDLExec():
-            _set_arr('features', X)
-            _set_arr('labels', y)
-            with io.StringIO() as target:
-                exec(f"eng.{self.__class__.__name__}_fit(nargout=0, stdout=target)")
-            if self._info_matlab == 'weights':
-                self._W = np.array(eng.workspace['weights'])
-            else:
-                self._model = eng.workspace['model']
-
-    def predict(self, X):
-        with BaseMatlabLDL.MatlabLDLExec():
-            _set_arr('features', X)
-            if self._info_matlab == 'weights':
-                exec(f"_set_arr('weights', self._{self._info_python})")
-            else:
-                eng.workspace['model'] = self._model
-            with io.StringIO() as target:
-                exec(f"eng.{self.__class__.__name__}_predict(nargout=0, stdout=target)")
-            return np.array(eng.workspace['preDistribution'])
-
-
-class _SA(BaseMatlabLDL):
-
-    def __init__(self, random_state=None):
-        super().__init__("W", "weights", random_state)
-
-
-class SA_BFGS(_SA):
-    pass
-
-
-class SA_IIS(_SA):
-    pass
-
-
-class AA_KNN(BaseMatlabLDL):
-
-    def __init__(self, random_state=None):
-        BaseLDL.__init__(self, random_state)
-    
-    def fit(self, X, y):
-        BaseLDL.fit(self, X, y)
-
-    def predict(self, X):
-        with BaseMatlabLDL.MatlabLDLExec():
-            _set_arr('features', self._X)
-            _set_arr('labels', self._y)
-            _set_arr('testFeatures', X)
-            with io.StringIO() as target:
-                eng.AA_KNN(nargout=0, stdout=target)
-            return np.array(eng.workspace['preDistribution'])
-
-
-class AA_BP(BaseMatlabLDL):
-
-    def _get_weights(name):
-        size = _get_arr(f"size(net.{name})")[0].astype(np.int32)
-        weights = [None for _ in range(size[0] * size[1])]
-        for i in range(size[0] * size[1]):
-            w = _get_arr(f"net.{name}" + r"{" + str(i // size[1] + 1) + r", " + str(i % size[1] + 1) + r"}").tolist()
-            weights[i] = matlab.double(w)
-        return weights
-
-    def _set_weights(name, weights):
-        eng.workspace[f'{name}'] = weights
-
-    def _save_net(self):
-        self._IW = AA_BP._get_weights("IW")
-        self._LW = AA_BP._get_weights("LW")
-        self._b = AA_BP._get_weights("b")
-
-    def _load_net(self):
-        AA_BP._set_weights("IW", self._IW)
-        AA_BP._set_weights("LW", self._LW)
-        AA_BP._set_weights("b", self._b)
-        
-
-    def __init__(self, random_state=None):
-        BaseLDL.__init__(self, random_state)
-    
-    def fit(self, X, y):
-        BaseLDL.fit(self, X, y)
-        with BaseMatlabLDL.MatlabLDLExec():
-            _set_arr('features', X)
-            _set_arr('labels', y)
-            with io.StringIO() as target:
-                eng.AA_BP_fit(nargout=0, stdout=target)
-            self._save_net()
-
-    def predict(self, X):
-        with BaseMatlabLDL.MatlabLDLExec():
-            _set_arr('features', self._X)
-            _set_arr('labels', self._y)
-            _set_arr('testFeatures', X)
-            self._load_net()
-            with io.StringIO() as target:
-                eng.AA_BP_predict(nargout=0, stdout=target)
-            return np.array(eng.workspace['preDistribution'])
-            
-
-class _PT(BaseMatlabLDL):
-
-    def __init__(self, random_state=None):
-        super().__init__("model", "model", random_state)
-
-
-class PT_Bayes(_PT):
-    pass
-
-
-class PT_SVM(_PT):
-    pass
-
-
-__all__ = ["SA_BFGS", "SA_IIS", "AA_KNN", "AA_BP", "PT_Bayes", "PT_SVM"]
+import io
+import os
+import numpy as np
+import matlab.engine
+
+from pyldl.algorithms.base import BaseLDL
+
+eng = matlab.engine.start_matlab()
+
+def _set_arr(name, arr):
+    eng.eval(f'global {name}', nargout=0)
+    eng.workspace[f'{name}'] = matlab.double(arr.tolist())
+
+
+def _get_arr(name):
+    with io.StringIO() as target:
+        eng.eval(f'tmp = {name}', nargout=0, stdout=target)
+    return np.array(eng.workspace['tmp'])
+
+
+class BaseMatlabLDL(BaseLDL):
+
+    class MatlabLDLExec:
+
+        def __enter__(self):
+            eng.cd(f'{os.path.dirname(os.path.abspath(__file__))}', nargout=0)
+            eng.eval(r'addpath("./LDLPackage_v1.2")', nargout=0)
+
+        def __exit__(self, exc_type, exc_val, exc_tb):
+            eng.eval('clear;', nargout=0)
+            eng.eval('clc;', nargout=0)
+            eng.eval(r'rmpath("./LDLPackage_v1.2")', nargout=0)
+            eng.cd(r'..', nargout=0)
+
+    def __init__(self, info_python=None, info_matlab=None, random_state=None):
+        super().__init__(random_state)
+        self._info_python, self._info_matlab = info_python, info_matlab
+        exec(f"self._{self._info_python} = None")
+    
+    def fit(self, X, y):
+        super().fit(X, y)
+
+        with BaseMatlabLDL.MatlabLDLExec():
+            _set_arr('features', X)
+            _set_arr('labels', y)
+            with io.StringIO() as target:
+                exec(f"eng.{self.__class__.__name__}_fit(nargout=0, stdout=target)")
+            if self._info_matlab == 'weights':
+                self._W = np.array(eng.workspace['weights'])
+            else:
+                self._model = eng.workspace['model']
+
+    def predict(self, X):
+        with BaseMatlabLDL.MatlabLDLExec():
+            _set_arr('features', X)
+            if self._info_matlab == 'weights':
+                exec(f"_set_arr('weights', self._{self._info_python})")
+            else:
+                eng.workspace['model'] = self._model
+            with io.StringIO() as target:
+                exec(f"eng.{self.__class__.__name__}_predict(nargout=0, stdout=target)")
+            return np.array(eng.workspace['preDistribution'])
+
+
+class _SA(BaseMatlabLDL):
+
+    def __init__(self, random_state=None):
+        super().__init__("W", "weights", random_state)
+
+
+class SA_BFGS(_SA):
+    pass
+
+
+class SA_IIS(_SA):
+    pass
+
+
+class AA_KNN(BaseMatlabLDL):
+
+    def __init__(self, random_state=None):
+        BaseLDL.__init__(self, random_state)
+    
+    def fit(self, X, y):
+        BaseLDL.fit(self, X, y)
+
+    def predict(self, X):
+        with BaseMatlabLDL.MatlabLDLExec():
+            _set_arr('features', self._X)
+            _set_arr('labels', self._y)
+            _set_arr('testFeatures', X)
+            with io.StringIO() as target:
+                eng.AA_KNN(nargout=0, stdout=target)
+            return np.array(eng.workspace['preDistribution'])
+
+
+class AA_BP(BaseMatlabLDL):
+
+    def _get_weights(name):
+        size = _get_arr(f"size(net.{name})")[0].astype(np.int32)
+        weights = [None for _ in range(size[0] * size[1])]
+        for i in range(size[0] * size[1]):
+            w = _get_arr(f"net.{name}" + r"{" + str(i // size[1] + 1) + r", " + str(i % size[1] + 1) + r"}").tolist()
+            weights[i] = matlab.double(w)
+        return weights
+
+    def _set_weights(name, weights):
+        eng.workspace[f'{name}'] = weights
+
+    def _save_net(self):
+        self._IW = AA_BP._get_weights("IW")
+        self._LW = AA_BP._get_weights("LW")
+        self._b = AA_BP._get_weights("b")
+
+    def _load_net(self):
+        AA_BP._set_weights("IW", self._IW)
+        AA_BP._set_weights("LW", self._LW)
+        AA_BP._set_weights("b", self._b)
+        
+
+    def __init__(self, random_state=None):
+        BaseLDL.__init__(self, random_state)
+    
+    def fit(self, X, y):
+        BaseLDL.fit(self, X, y)
+        with BaseMatlabLDL.MatlabLDLExec():
+            _set_arr('features', X)
+            _set_arr('labels', y)
+            with io.StringIO() as target:
+                eng.AA_BP_fit(nargout=0, stdout=target)
+            self._save_net()
+
+    def predict(self, X):
+        with BaseMatlabLDL.MatlabLDLExec():
+            _set_arr('features', self._X)
+            _set_arr('labels', self._y)
+            _set_arr('testFeatures', X)
+            self._load_net()
+            with io.StringIO() as target:
+                eng.AA_BP_predict(nargout=0, stdout=target)
+            return np.array(eng.workspace['preDistribution'])
+            
+
+class _PT(BaseMatlabLDL):
+
+    def __init__(self, random_state=None):
+        super().__init__("model", "model", random_state)
+
+
+class PT_Bayes(_PT):
+    pass
+
+
+class PT_SVM(_PT):
+    pass
+
+
+__all__ = ["SA_BFGS", "SA_IIS", "AA_KNN", "AA_BP", "PT_Bayes", "PT_SVM"]
```

### Comparing `python-ldl-0.0.1/pyldl/metrics.py` & `python-ldl-0.0.2/pyldl/metrics.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import numpy as np
-from scipy import stats
-from sklearn.metrics.pairwise import paired_cosine_distances
-
-
-eps = np.finfo(np.float64).eps
-
-
-def _clip(func):
-    def _wrapper(y, y_pred):
-        y = np.clip(y, eps, 1)
-        y_pred = np.clip(y_pred, eps, 1)
-        return func(y, y_pred)
-    return _wrapper
-
-
-def chebyshev(y, y_pred):
-    return np.max(np.abs(y - y_pred), 1).mean()
-
-
-@_clip
-def clark(y, y_pred):
-    return np.sqrt(np.sum(np.power(y - y_pred, 2) / np.power(y + y_pred, 2), 1)).mean()
-
-
-@_clip
-def canberra(y, y_pred):
-    return np.sum(np.abs(y - y_pred) / (y + y_pred), 1).mean()
-
-
-@_clip
-def kl_divergence(y, y_pred):
-    return np.sum(y * (np.log(y) - np.log(y_pred)), 1).mean()
-
-
-def cosine(y, y_pred):
-    return 1 - paired_cosine_distances(y, y_pred).mean()
-
-
-def intersection(y, y_pred):
-    return 1 - 0.5 * np.sum(np.abs(y - y_pred), 1).mean()
-
-
-def euclidean(y, y_pred):
-    return np.sqrt(np.sum((y - y_pred) ** 2, 1)).mean()
-
-
-@_clip
-def sorensen(y, y_pred):
-    return (np.sum(np.abs(y - y_pred), 1) / np.sum(y + y_pred, 1)).mean()
-
-
-@_clip
-def squared_chi2(y, y_pred):
-    return np.sum((y - y_pred) ** 2 / (y + y_pred), 1).mean()
-
-
-def fidelity(y, y_pred):
-    return np.sum(np.sqrt(y * y_pred), 1).mean()
-
-
-def mean_absolute_error(y, y_pred):
-    x = np.arange(1, y.shape[1] + 1)
-    yt = np.sum(y * x, axis=1)
-    yp = np.sum(y_pred * x, axis=1)
-    return np.average(np.abs(yt - yp))
-
-
-def sort_loss(y, y_pred, reduction=np.average):
-    i = np.argsort(-y)
-    h = y_pred[np.arange(y_pred.shape[0])[:, np.newaxis], i]
-    res = 0.
-    for j in range(y.shape[1] - 1):
-        for k in range(j + 1, y.shape[1]):
-            res += np.maximum(h[:, k] - h[:, j], 0.) / np.log2(j + 2)
-    res /= np.sum([1. / np.log2(j + 2) for j in range(y.shape[1] - 1)])
-    return reduction(res) if reduction is not None else res
-
-
-def spearman(y, y_pred):
-    return np.array([stats.spearmanr(y[i], y_pred[i])[0] for i in range(y.shape[0])]).mean()
-
-
-def kendall(y, y_pred):
-    return np.array([stats.kendalltau(y[i], y_pred[i], variant='c')[0] for i in range(y.shape[0])]).mean()
-
-
-def zero_one_loss(y, y_pred):
-    return 1 - (np.argmax(y, 1) == np.argmax(y_pred, 1)).mean()
-
-
-def error_probability(y, y_pred):
-    return 1 - y[np.arange(y.shape[0]), np.argmax(y_pred, 1)].mean()
-
-
-def score(y, y_pred,
-          metrics=["chebyshev", "clark", "canberra", "kl_divergence", "cosine", "intersection"]):
-    return tuple((eval(i)(y, y_pred) for i in metrics))
+import numpy as np
+from scipy import stats
+from sklearn.metrics.pairwise import paired_cosine_distances
+
+
+eps = np.finfo(np.float64).eps
+
+
+def _clip(func):
+    def _wrapper(y, y_pred):
+        y = np.clip(y, eps, 1)
+        y_pred = np.clip(y_pred, eps, 1)
+        return func(y, y_pred)
+    return _wrapper
+
+
+def chebyshev(y, y_pred):
+    return np.max(np.abs(y - y_pred), 1).mean()
+
+
+@_clip
+def clark(y, y_pred):
+    return np.sqrt(np.sum(np.power(y - y_pred, 2) / np.power(y + y_pred, 2), 1)).mean()
+
+
+@_clip
+def canberra(y, y_pred):
+    return np.sum(np.abs(y - y_pred) / (y + y_pred), 1).mean()
+
+
+@_clip
+def kl_divergence(y, y_pred):
+    return np.sum(y * (np.log(y) - np.log(y_pred)), 1).mean()
+
+
+def cosine(y, y_pred):
+    return 1 - paired_cosine_distances(y, y_pred).mean()
+
+
+def intersection(y, y_pred):
+    return 1 - 0.5 * np.sum(np.abs(y - y_pred), 1).mean()
+
+
+def euclidean(y, y_pred):
+    return np.sqrt(np.sum((y - y_pred) ** 2, 1)).mean()
+
+
+@_clip
+def sorensen(y, y_pred):
+    return (np.sum(np.abs(y - y_pred), 1) / np.sum(y + y_pred, 1)).mean()
+
+
+@_clip
+def squared_chi2(y, y_pred):
+    return np.sum((y - y_pred) ** 2 / (y + y_pred), 1).mean()
+
+
+def fidelity(y, y_pred):
+    return np.sum(np.sqrt(y * y_pred), 1).mean()
+
+
+def mean_absolute_error(y, y_pred):
+    x = np.arange(1, y.shape[1] + 1)
+    yt = np.sum(y * x, axis=1)
+    yp = np.sum(y_pred * x, axis=1)
+    return np.average(np.abs(yt - yp))
+
+
+def sort_loss(y, y_pred, reduction=np.average):
+    i = np.argsort(-y)
+    h = y_pred[np.arange(y_pred.shape[0])[:, np.newaxis], i]
+    res = 0.
+    for j in range(y.shape[1] - 1):
+        for k in range(j + 1, y.shape[1]):
+            res += np.maximum(h[:, k] - h[:, j], 0.) / np.log2(j + 2)
+    res /= np.sum([1. / np.log2(j + 2) for j in range(y.shape[1] - 1)])
+    return reduction(res) if reduction is not None else res
+
+
+def spearman(y, y_pred):
+    return np.array([stats.spearmanr(y[i], y_pred[i])[0] for i in range(y.shape[0])]).mean()
+
+
+def kendall(y, y_pred):
+    return np.array([stats.kendalltau(y[i], y_pred[i], variant='c')[0] for i in range(y.shape[0])]).mean()
+
+
+def zero_one_loss(y, y_pred):
+    return 1 - (np.argmax(y, 1) == np.argmax(y_pred, 1)).mean()
+
+
+def error_probability(y, y_pred):
+    return 1 - y[np.arange(y.shape[0]), np.argmax(y_pred, 1)].mean()
+
+
+def score(y, y_pred,
+          metrics=["chebyshev", "clark", "canberra", "kl_divergence", "cosine", "intersection"]):
+    return tuple((eval(i)(y, y_pred) for i in metrics))
```

### Comparing `python-ldl-0.0.1/python_ldl.egg-info/PKG-INFO` & `python-ldl-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,170 +1,187 @@
-Metadata-Version: 2.1
-Name: python-ldl
-Version: 0.0.1
-Summary: Label distribution learning (LDL) and label enhancement (LE) toolkit implemented in python.
-Home-page: https://github.com/SpriteMisaka/PyLDL
-Author: SpriteMisaka
-Author-email: SpriteMisaka@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: qpsolvers
-Requires-Dist: quadprog
-Requires-Dist: scikit-fuzzy
-Requires-Dist: scikit-learn
-Requires-Dist: scipy
-Requires-Dist: tensorflow
-Requires-Dist: tensorflow-addons
-Requires-Dist: tensorflow-probability
-
-# PyLDL
-
-Label distribution learning (LDL) and label enhancement (LE) toolkit implemented in python, including:
-
-+ LDL algorithms:
-  + ([Geng, Yin, and Zhou 2013](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2013.pdf))[*TPAMI*]: `CPNN`$^1$.
-  + ([Geng and Hou 2015](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2015.pdf))[*IJCAI*]: `LDSVR`.
-  + ⭐([Geng 2016](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2016.pdf))[*TKDE*]: `SA_BFGS`, `SA_IIS`, `AA_KNN`, `AA_BP`, `PT_Bayes`, and `PT_SVM`.
-  + ([Yang, Sun, and Sun 2017](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/yang2017.pdf))[*AAAI*]: `BCPNN` and `ACPNN`.
-  + ([Xu and Zhou 2017](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/xu2017.pdf))[*IJCAI*]: `IncomLDL`$^2$.
-  + ([Shen et al. 2017](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/shen2017.pdf))[*NeurIPS*]: `LDLF`.
-  + ([Wang and Geng 2019](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wang2019.pdf))[*IJCAI*]: `LDL4C`$^3$.
-  + ([Shen et al. 2020](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/shen2020.pdf))[*南京理工大学学报* (Chinese)]: `AdaBoostLDL`.
-  + ([González et al. 2021a](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/gonz%C3%A1lez2021a.pdf))[*Information Sciences*]: `SSG_LDL`$^4$.
-  + ([González et al. 2021b](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/gonz%C3%A1lez2021b.pdf))[*Information Fusion*]: `DF_LDL`.
-  + ([Wang and Geng 2021a](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wang2021a.pdf))[*IJCAI*]: `LDL_HR`$^3$.
-  + ([Wang and Geng 2021b](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wang2021b.pdf))[*ICML*]: `LDLM`$^3$.
-  + ([Jia et al. 2021](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/jia2021.pdf))[*TKDE*]: `LDL_SCL`.
-  + ([Jia et al. 2023](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/jia2023.pdf))[*TKDE*]: `LDL_LRR`.
-  + ([Wen et al. 2023](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wen2023.pdf))[*ICCV*]: `CAD`$^1$, `QFD2`$^1$, and `CJS`$^1$.
-+ LE algorithms:
-  + ([Xu, Liu, and Geng 2019](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/xu2019.pdf))[*TKDE*]: `FCM`, `KM`, `LP`, `ML`, and `GLLE`.
-  + ([Xu et al. 2020](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/xu2020.pdf))[*ICML*]: `LEVI`.
-  + ([Zheng, Zhu, and Tang 2023](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/zheng2023.pdf))[*CVPR*]: `LIBLE`.
-  
-+ LDL metrics: `chebyshev`, `clark`, `canberra`, `kl_divergence`, `cosine`, `intersection`, etc.
-+ LDL datasets: *Human_Gene*, *Movie*, *Natural_Scene*, *s-BU_3DFE*, *s-JAFFE*, *Yeast*, etc.
-
-> $^1$ Technically, these methods are only suitable for totally ordered labels.
->
-> $^2$ These are algorithms for incomplete LDL, so you should use `utils.random_missing` to generate the missing label distribution matrix and the corresponding mask matrix in the experiments.
->
-> $^3$ These are LDL classifiers, so you should use `predict_proba` to get label distributions and `predict` to get predicted labels.
->
-> $^4$ These are oversampling algorithms for LDL, therefore you should use `fit_transform` to generate synthetic samples.
-
-## Usage
-
-Here is an example of using PyLDL.
-
-```python
-from pyldl.utils import load_dataset
-from pyldl.algorithms import SA_BFGS
-from pyldl.metrics import score
-
-from sklearn.model_selection import train_test_split
-
-dataset_name = 'SJAFFE'
-X, y = load_dataset(dataset_name)
-X_train, X_test, y_train, y_test = train_test_split(X, y)
-
-model = SA_BFGS()
-model.fit(X_train, y_train)
-
-y_pred = model.predict(X_test)
-print(score(y_test, y_pred))
-```
-
-For those who would like to use the original implementation:
-
-1. Install MATLAB.
-2. Install MATLAB engine for python.
-3. Download LDL Package from [here](http://palm.seu.edu.cn/xgeng/LDL/download.htm).
-3. Get the package directory of PyLDL (...\\Lib\\site-packages\\pyldl).
-4. Place the *LDLPackage_v1.2* folder into the *matlab_algorithms* folder.
-
-Now, you can load the original implementation of the method, e.g.:
-
-```python
-from pyldl.matlab_algorithms import SA_IIS
-```
-
-You can visualize the performance of any model on the artificial dataset ([Geng 2016](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2016.pdf)) with the `pyldl.utils.plot_artificial` function, e.g.:
-
-```python
-from pyldl.algorithms import LDSVR, SA_BFGS, SA_IIS, AA_KNN, PT_Bayes, GLLE, LIBLE
-from pyldl.utils import plot_artificial
-
-methods = ['LDSVR', 'SA_BFGS', 'SA_IIS', 'AA_KNN', 'PT_Bayes', 'GLLE', 'LIBLE']
-
-plot_artificial(model=None, figname='GT')
-for i in methods:
-    plot_artificial(model=eval(f'{i}()'), figname=i)
-```
-
-The output images are as follows.
-
-| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/GT.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/LDSVR.jpg?raw=true" width=300> |
-| :----------------------------------------------------------: | :----------------------------------------------------------: |
-|                        (Ground Truth)                        |                           `LDSVR`                            |
-
-| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/SA_BFGS.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/SA_IIS.jpg?raw=true" width=300> |
-| :----------------------------------------------------------: | :----------------------------------------------------------: |
-|                          `SA_BFGS`                           |                           `SA_IIS`                           |
-
-| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/AA_KNN.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/PT_Bayes.jpg?raw=true" width=300> |
-| :----------------------------------------------------------: | :----------------------------------------------------------: |
-|                           `AA_KNN`                           |                          `PT_Bayes`                          |
-
-| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/GLLE.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/LIBLE.jpg?raw=true" width=300> |
-| :----------------------------------------------------------: | :----------------------------------------------------------: |
-|                            `GLLE`                            |                           `LIBLE`                            |
-
-Enjoy! :)
-
-## Experiments
-
-For each algorithm, a ten-fold cross validation is performed, repeated 10 times with *s-JAFFE* dataset and the average metrics are recorded. Therefore, the results do not fully describe the performance of the model.
-
-Results of ours are as follows.
-
-| Algorithm |    Cheby.(↓)    |    Clark(↓)     |     Can.(↓)     |     K-L(↓)      |     Cos.(↑)     |     Int.(↑)     |
-| :-------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: |
-|  SA-BFGS  | **.092 ± .010** |   .361 ± .029   |   .735 ± .060   | **.051 ± .009** | **.954 ± .009** | **.878 ± .011** |
-|  SA-IIS   |   .100 ± .009   |   .361 ± .023   |   .746 ± .050   | **.051 ± .008** |   .952 ± .007   |   .873 ± .009   |
-|  AA-kNN   |   .098 ± .011   | **.349 ± .029** | **.716 ± .062** |   .053 ± .010   |   .950 ± .009   |   .877 ± .011   |
-|   AA-BP   |   .120 ± .012   |   .426 ± .025   |   .889 ± .057   |   .073 ± .010   |   .931 ± .010   |   .848 ± .011   |
-| PT-Bayes  |   .116 ± .011   |   .425 ± .031   |   .874 ± .064   |   .073 ± .012   |   .932 ± .011   |   .850 ± .012   |
-|  PT-SVM   |   .117 ± .012   |   .422 ± .027   |   .875 ± .057   |   .072 ± .011   |   .932 ± .011   |   .850 ± .011   |
-
-Results of the original MATLAB implementation ([Geng 2016](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2016.pdf)) are as follows.
-
-| Algorithm |    Cheby.(↓)    |    Clark(↓)     |     Can.(↓)     |     K-L(↓)      |     Cos.(↑)     |     Int.(↑)     |
-| :-------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: |
-|  SA-BFGS  | **.107 ± .015** | **.399 ± .044** | **.820 ± .103** | **.064 ± .016** | **.940 ± .015** | **.860 ± .019** |
-|  SA-IIS   |   .117 ± .015   |   .419 ± .034   |   .875 ± .086   |   .070 ± .012   |   .934 ± .012   |   .851 ± .016   |
-|  AA-kNN   |   .114 ± .017   |   .410 ± .050   |   .843 ± .113   |   .071 ± .023   |   .934 ± .018   |   .855 ± .021   |
-|   AA-BP   |   .130 ± .017   |   .510 ± .054   |   1.05 ± .124   |   .113 ± .030   |   .908 ± .019   |   .824 ± .022   |
-| PT-Bayes  |   .121 ± .016   |   .430 ± .035   |   .904 ± .086   |   .074 ± .014   |   .930 ± .016   |   .846 ± .016   |
-|  PT-SVM   |   .127 ± .017   |   .457 ± .039   |   .935 ± .074   |   .086 ± .016   |   .920 ± .014   |   .839 ± .015   |
-
-## Requirements
-
-```
-matplotlib>=3.6.1
-numpy>=1.22.3
-qpsolvers>=4.0.0
-quadprog>=0.1.11
-scikit-fuzzy>=0.4.2
-scikit-learn>=1.0.2
-scipy>=1.8.0
-tensorflow>=2.8.0
-tensorflow-addons>=0.22.0
-tensorflow-probability>=0.16.0
-```
-
+Metadata-Version: 2.1
+Name: python-ldl
+Version: 0.0.2
+Summary: Label distribution learning (LDL) and label enhancement (LE) toolkit implemented in python.
+Home-page: https://github.com/SpriteMisaka/PyLDL
+Author: SpriteMisaka
+Author-email: SpriteMisaka@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: qpsolvers
+Requires-Dist: quadprog
+Requires-Dist: scikit-fuzzy
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: tensorflow
+Requires-Dist: tensorflow-addons
+Requires-Dist: tensorflow-probability
+
+# PyLDL
+
+Label distribution learning (LDL) and label enhancement (LE) toolkit implemented in python, including:
+
++ LDL algorithms:
+  + ([Geng, Yin, and Zhou 2013](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2013.pdf))[*TPAMI*]: `CPNN`$^1$.
+  + ([Geng and Hou 2015](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2015.pdf))[*IJCAI*]: `LDSVR`.
+  + ⭐([Geng 2016](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2016.pdf))[*TKDE*]: `SA_BFGS`, `SA_IIS`, `AA_KNN`, `AA_BP`, `PT_Bayes`, and `PT_SVM`.
+  + ([Yang, Sun, and Sun 2017](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/yang2017.pdf))[*AAAI*]: `BCPNN` and `ACPNN`.
+  + ([Xu and Zhou 2017](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/xu2017.pdf))[*IJCAI*]: `IncomLDL`$^2$.
+  + ([Shen et al. 2017](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/shen2017.pdf))[*NeurIPS*]: `LDLF`.
+  + ([Wang and Geng 2019](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wang2019.pdf))[*IJCAI*]: `LDL4C`$^3$.
+  + ([Shen et al. 2020](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/shen2020.pdf))[*南京理工大学学报* (Chinese)]: `AdaBoostLDL`.
+  + ([González et al. 2021a](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/gonz%C3%A1lez2021a.pdf))[*Information Sciences*]: `SSG_LDL`$^4$.
+  + ([González et al. 2021b](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/gonz%C3%A1lez2021b.pdf))[*Information Fusion*]: `DF_LDL`.
+  + ([Wang and Geng 2021a](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wang2021a.pdf))[*IJCAI*]: `LDL_HR`$^3$.
+  + ([Wang and Geng 2021b](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wang2021b.pdf))[*ICML*]: `LDLM`$^3$.
+  + ([Jia et al. 2021](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/jia2021.pdf))[*TKDE*]: `LDL_SCL`.
+  + ([Jia et al. 2023](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/jia2023.pdf))[*TKDE*]: `LDL_LRR`.
+  + ([Wen et al. 2023](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wen2023.pdf))[*ICCV*]: `CAD`$^1$, `QFD2`$^1$, and `CJS`$^1$.
++ LE algorithms:
+  + ([Xu, Liu, and Geng 2019](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/xu2019.pdf))[*TKDE*]: `FCM`, `KM`, `LP`, `ML`, and `GLLE`.
+  + ([Xu et al. 2020](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/xu2020.pdf))[*ICML*]: `LEVI`.
+  + ([Zheng, Zhu, and Tang 2023](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/zheng2023.pdf))[*CVPR*]: `LIBLE`.
++ LDL metrics: `chebyshev`, `clark`, `canberra`, `kl_divergence`, `cosine`, `intersection`, etc.
++ Structured LDL datasets: *Human_Gene*, *Movie*, *Natural_Scene*, *s-BU_3DFE*, *s-JAFFE*, *Yeast*, etc.
++ LDL applications:
+  + Facial emotion recognition (supported datasets: [*JAFFE*](https://zenodo.org/records/3451524)).
+  + ([Shirani et al. 2019](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/shirani2019.pdf))[*ACL*]: Emphasis selection (supported datasets: [*SemEval2020*](https://github.com/RiTUAL-UH/SemEval2020_Task10_Emphasis_Selection); pre-trained GloVe embeddings can be downloaded [here](https://nlp.stanford.edu/projects/glove/)).
+  + ([Wu et al. 2019](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/wu2019.pdf))[*ICCV*]: Lesion counting (supported datasets: [*ACNE04*](https://drive.google.com/drive/folders/18yJcHXhzOv7H89t-Lda6phheAicLqMuZ)).
+
+> $^1$ Technically, these methods are only suitable for totally ordered labels.
+>
+> $^2$ These are algorithms for incomplete LDL, so you should use `pyldl.utils.random_missing` to generate the missing label distribution matrix and the corresponding mask matrix in the experiments.
+>
+> $^3$ These are LDL classifiers, so you should use `predict_proba` to get label distributions and `predict` to get predicted labels.
+>
+> $^4$ These are oversampling algorithms for LDL, therefore you should use `fit_transform` to generate synthetic samples.
+
+## Installation
+
+PyLDL is now available on [PyPI](https://pypi.org/project/python-ldl/). Use the following command to install.
+
+```shell
+pip install python-ldl
+```
+
+To install the newest version, you can clone this repo and run the `setup.py` file.
+
+```shell
+python setup.py install
+```
+
+## Usage
+
+Here is an example of using PyLDL.
+
+```python
+from pyldl.utils import load_dataset
+from pyldl.algorithms import SA_BFGS
+from pyldl.metrics import score
+
+from sklearn.model_selection import train_test_split
+
+dataset_name = 'SJAFFE'
+X, y = load_dataset(dataset_name)
+X_train, X_test, y_train, y_test = train_test_split(X, y)
+
+model = SA_BFGS()
+model.fit(X_train, y_train)
+
+y_pred = model.predict(X_test)
+print(score(y_test, y_pred))
+```
+
+For those who would like to use the original implementation:
+
+1. Install MATLAB.
+2. Install MATLAB engine for python.
+3. Download LDL Package [here](http://palm.seu.edu.cn/xgeng/LDL/download.htm).
+3. Get the package directory of PyLDL (...\\Lib\\site-packages\\pyldl).
+4. Place the *LDLPackage_v1.2* folder into the *matlab_algorithms* folder.
+
+Now, you can load the original implementation of the method, e.g.:
+
+```python
+from pyldl.matlab_algorithms import SA_IIS
+```
+
+You can visualize the performance of any model on the artificial dataset ([Geng 2016](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2016.pdf)) with the `pyldl.utils.plot_artificial` function, e.g.:
+
+```python
+from pyldl.algorithms import LDSVR, SA_BFGS, SA_IIS, AA_KNN, PT_Bayes, GLLE, LIBLE
+from pyldl.utils import plot_artificial
+
+methods = ['LDSVR', 'SA_BFGS', 'SA_IIS', 'AA_KNN', 'PT_Bayes', 'GLLE', 'LIBLE']
+
+plot_artificial(model=None, figname='GT')
+for i in methods:
+    plot_artificial(model=eval(f'{i}()'), figname=i)
+```
+
+The output images are as follows.
+
+| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/GT.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/LDSVR.jpg?raw=true" width=300> |
+| :----------------------------------------------------------: | :----------------------------------------------------------: |
+|                        (Ground Truth)                        |                           `LDSVR`                            |
+
+| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/SA_BFGS.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/SA_IIS.jpg?raw=true" width=300> |
+| :----------------------------------------------------------: | :----------------------------------------------------------: |
+|                          `SA_BFGS`                           |                           `SA_IIS`                           |
+
+| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/AA_KNN.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/PT_Bayes.jpg?raw=true" width=300> |
+| :----------------------------------------------------------: | :----------------------------------------------------------: |
+|                           `AA_KNN`                           |                          `PT_Bayes`                          |
+
+| <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/GLLE.jpg?raw=true" width=300> | <img src="https://github.com/SpriteMisaka/PyLDL/blob/main/visualization/LIBLE.jpg?raw=true" width=300> |
+| :----------------------------------------------------------: | :----------------------------------------------------------: |
+|                            `GLLE`                            |                           `LIBLE`                            |
+
+Enjoy! :)
+
+## Experiments
+
+For each algorithm, a ten-fold cross validation is performed, repeated 10 times with *s-JAFFE* dataset and the average metrics are recorded. Therefore, the results do not fully describe the performance of the model.
+
+Results of ours are as follows.
+
+| Algorithm |    Cheby.(↓)    |    Clark(↓)     |     Can.(↓)     |     K-L(↓)      |     Cos.(↑)     |     Int.(↑)     |
+| :-------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: |
+|  SA-BFGS  | **.092 ± .010** |   .361 ± .029   |   .735 ± .060   | **.051 ± .009** | **.954 ± .009** | **.878 ± .011** |
+|  SA-IIS   |   .100 ± .009   |   .361 ± .023   |   .746 ± .050   | **.051 ± .008** |   .952 ± .007   |   .873 ± .009   |
+|  AA-kNN   |   .098 ± .011   | **.349 ± .029** | **.716 ± .062** |   .053 ± .010   |   .950 ± .009   |   .877 ± .011   |
+|   AA-BP   |   .120 ± .012   |   .426 ± .025   |   .889 ± .057   |   .073 ± .010   |   .931 ± .010   |   .848 ± .011   |
+| PT-Bayes  |   .116 ± .011   |   .425 ± .031   |   .874 ± .064   |   .073 ± .012   |   .932 ± .011   |   .850 ± .012   |
+|  PT-SVM   |   .117 ± .012   |   .422 ± .027   |   .875 ± .057   |   .072 ± .011   |   .932 ± .011   |   .850 ± .011   |
+
+Results of the original MATLAB implementation ([Geng 2016](https://github.com/SpriteMisaka/PyLDL/blob/main/bibliography/geng2016.pdf)) are as follows.
+
+| Algorithm |    Cheby.(↓)    |    Clark(↓)     |     Can.(↓)     |     K-L(↓)      |     Cos.(↑)     |     Int.(↑)     |
+| :-------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: |
+|  SA-BFGS  | **.107 ± .015** | **.399 ± .044** | **.820 ± .103** | **.064 ± .016** | **.940 ± .015** | **.860 ± .019** |
+|  SA-IIS   |   .117 ± .015   |   .419 ± .034   |   .875 ± .086   |   .070 ± .012   |   .934 ± .012   |   .851 ± .016   |
+|  AA-kNN   |   .114 ± .017   |   .410 ± .050   |   .843 ± .113   |   .071 ± .023   |   .934 ± .018   |   .855 ± .021   |
+|   AA-BP   |   .130 ± .017   |   .510 ± .054   |   1.05 ± .124   |   .113 ± .030   |   .908 ± .019   |   .824 ± .022   |
+| PT-Bayes  |   .121 ± .016   |   .430 ± .035   |   .904 ± .086   |   .074 ± .014   |   .930 ± .016   |   .846 ± .016   |
+|  PT-SVM   |   .127 ± .017   |   .457 ± .039   |   .935 ± .074   |   .086 ± .016   |   .920 ± .014   |   .839 ± .015   |
+
+## Requirements
+
+```
+matplotlib>=3.6.1
+numpy>=1.22.3
+qpsolvers>=4.0.0
+quadprog>=0.1.11
+scikit-fuzzy>=0.4.2
+scikit-learn>=1.0.2
+scipy>=1.8.0
+tensorflow>=2.8.0
+tensorflow-addons>=0.22.0
+tensorflow-probability>=0.16.0
+```
+
```

### Comparing `python-ldl-0.0.1/setup.py` & `python-ldl-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import setuptools
-
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="python-ldl",
-    version="0.0.1",
-    author="SpriteMisaka",
-    author_email="SpriteMisaka@gmail.com",
-    description="Label distribution learning (LDL) and label enhancement (LE) toolkit implemented in python.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/SpriteMisaka/PyLDL",
-
-    packages=setuptools.find_packages(),
-    package_data={
-        '': ['*.m']
-    },
-    include_package_data=True,
-    exclude_package_data={
-        '': ['__pycache__', 'LDLPackage_v1.2']
-    },
-
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-
-    install_requires=[
-        "matplotlib",
-        "numpy",
-        "qpsolvers",
-        "quadprog",
-        "scikit-fuzzy",
-        "scikit-learn",
-        "scipy",
-        "tensorflow",
-        "tensorflow-addons",
-        "tensorflow-probability"
-    ],
-
-    python_requires='>=3',
-)
+import setuptools
+
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="python-ldl",
+    version="0.0.2",
+    author="SpriteMisaka",
+    author_email="SpriteMisaka@gmail.com",
+    description="Label distribution learning (LDL) and label enhancement (LE) toolkit implemented in python.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/SpriteMisaka/PyLDL",
+
+    packages=setuptools.find_packages(),
+    package_data={
+        '': ['*.m']
+    },
+    include_package_data=True,
+    exclude_package_data={
+        '': ['__pycache__', 'LDLPackage_v1.2']
+    },
+
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+
+    install_requires=[
+        "matplotlib",
+        "numpy",
+        "qpsolvers",
+        "quadprog",
+        "scikit-fuzzy",
+        "scikit-learn",
+        "scipy",
+        "tensorflow",
+        "tensorflow-addons",
+        "tensorflow-probability"
+    ],
+
+    python_requires='>=3',
+)
```

