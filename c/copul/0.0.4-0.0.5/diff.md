# Comparing `tmp/copul-0.0.4.tar.gz` & `tmp/copul-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copul-0.0.4.tar", last modified: Wed May 24 13:24:38 2023, max compression
+gzip compressed data, was "copul-0.0.5.tar", max compression
```

## Comparing `copul-0.0.4.tar` & `copul-0.0.5.tar`

### file list

```diff
@@ -1,65 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.373880 copul-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-05-21 18:41:35.000000 copul-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       30 2023-05-17 14:16:18.000000 copul-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1986 2023-05-24 13:24:38.373880 copul-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1449 2023-05-22 16:18:24.000000 copul-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.337684 copul-0.0.4/copul/
--rw-rw-rw-   0        0        0      357 2023-05-21 18:51:19.000000 copul-0.0.4/copul/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.346170 copul-0.0.4/copul/docs/
--rw-rw-rw-   0        0        0        0 2023-05-17 14:16:18.000000 copul-0.0.4/copul/docs/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.351512 copul-0.0.4/copul/families/
--rw-rw-rw-   0        0        0      293 2023-05-22 15:10:27.000000 copul-0.0.4/copul/families/__init__.py
--rw-rw-rw-   0        0        0     2380 2023-05-22 16:16:20.000000 copul-0.0.4/copul/families/abstract_copula.py
-drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.367035 copul-0.0.4/copul/families/archimedean/
--rw-rw-rw-   0        0        0     5839 2023-05-21 18:51:44.000000 copul-0.0.4/copul/families/archimedean/__init__.py
--rw-rw-rw-   0        0        0     5386 2023-05-22 15:34:05.000000 copul-0.0.4/copul/families/archimedean/archimedean_copula.py
--rw-rw-rw-   0        0        0     5160 2023-05-21 18:41:35.000000 copul-0.0.4/copul/families/archimedean/derivatives_overview_constructor.py
--rw-rw-rw-   0        0        0     1141 2023-05-24 13:23:47.000000 copul-0.0.4/copul/families/archimedean/nelsen1.py
--rw-rw-rw-   0        0        0      299 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen10.py
--rw-rw-rw-   0        0        0      294 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen11.py
--rw-rw-rw-   0        0        0      503 2023-05-22 15:14:02.000000 copul-0.0.4/copul/families/archimedean/nelsen12.py
--rw-rw-rw-   0        0        0      322 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen13.py
--rw-rw-rw-   0        0        0      531 2023-05-22 15:34:05.000000 copul-0.0.4/copul/families/archimedean/nelsen14.py
--rw-rw-rw-   0        0        0      357 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen15.py
--rw-rw-rw-   0        0        0     1079 2023-05-24 13:13:50.000000 copul-0.0.4/copul/families/archimedean/nelsen16.py
--rw-rw-rw-   0        0        0     2454 2023-05-24 13:13:50.000000 copul-0.0.4/copul/families/archimedean/nelsen17.py
--rw-rw-rw-   0        0        0      318 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen18.py
--rw-rw-rw-   0        0        0      333 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen19.py
--rw-rw-rw-   0        0        0      506 2023-05-22 14:44:54.000000 copul-0.0.4/copul/families/archimedean/nelsen2.py
--rw-rw-rw-   0        0        0      330 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen20.py
--rw-rw-rw-   0        0        0      658 2023-05-22 15:49:15.000000 copul-0.0.4/copul/families/archimedean/nelsen21.py
--rw-rw-rw-   0        0        0      686 2023-05-22 15:52:14.000000 copul-0.0.4/copul/families/archimedean/nelsen22.py
--rw-rw-rw-   0        0        0      615 2023-05-24 13:11:22.000000 copul-0.0.4/copul/families/archimedean/nelsen3.py
--rw-rw-rw-   0        0        0      354 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen4.py
--rw-rw-rw-   0        0        0      378 2023-05-24 13:13:50.000000 copul-0.0.4/copul/families/archimedean/nelsen5.py
--rw-rw-rw-   0        0        0      336 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/archimedean/nelsen6.py
--rw-rw-rw-   0        0        0      524 2023-05-22 15:12:30.000000 copul-0.0.4/copul/families/archimedean/nelsen7.py
--rw-rw-rw-   0        0        0      616 2023-05-22 15:12:30.000000 copul-0.0.4/copul/families/archimedean/nelsen8.py
--rw-rw-rw-   0        0        0      557 2023-05-21 18:54:44.000000 copul-0.0.4/copul/families/archimedean/nelsen9.py
-drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.371437 copul-0.0.4/copul/families/extreme_value/
--rw-rw-rw-   0        0        0      386 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/__init__.py
--rw-rw-rw-   0        0        0      650 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/bb5.py
--rw-rw-rw-   0        0        0     6222 2023-05-21 18:41:35.000000 copul-0.0.4/copul/families/extreme_value/extreme_value_copula.py
--rw-rw-rw-   0        0        0      619 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/galambos.py
--rw-rw-rw-   0        0        0      441 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/gumbel.py
--rw-rw-rw-   0        0        0      771 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/huesler_reiss.py
--rw-rw-rw-   0        0        0      867 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/joe.py
--rw-rw-rw-   0        0        0      527 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/marshall_olkin.py
--rw-rw-rw-   0        0        0      820 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/t_ev.py
--rw-rw-rw-   0        0        0      770 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/extreme_value/tawn.py
-drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.372440 copul-0.0.4/copul/families/other/
--rw-rw-rw-   0        0        0        0 2023-05-21 18:41:35.000000 copul-0.0.4/copul/families/other/__init__.py
--rw-rw-rw-   0        0        0      886 2023-05-21 18:54:30.000000 copul-0.0.4/copul/families/other/farlie_gumbell_morgenstern.py
--rw-rw-rw-   0        0        0      976 2023-05-22 15:32:08.000000 copul-0.0.4/copul/families/other/frechet.py
--rw-rw-rw-   0        0        0     9165 2023-05-22 16:12:09.000000 copul-0.0.4/copul/families/other/plackett.py
-drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.372440 copul-0.0.4/copul/simulations/
--rw-rw-rw-   0        0        0        0 2023-05-17 14:16:18.000000 copul-0.0.4/copul/simulations/__init__.py
--rw-rw-rw-   0        0        0     1276 2023-05-24 13:19:17.000000 copul-0.0.4/copul/sympy_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-05-24 13:24:38.346170 copul-0.0.4/copul.egg-info/
--rw-rw-rw-   0        0        0     1986 2023-05-24 13:24:38.000000 copul-0.0.4/copul.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1912 2023-05-24 13:24:38.000000 copul-0.0.4/copul.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 13:24:38.000000 copul-0.0.4/copul.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-05-24 13:24:38.000000 copul-0.0.4/copul.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-24 13:24:38.000000 copul-0.0.4/copul.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1030 2023-05-24 13:24:19.000000 copul-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-05-24 13:24:38.373880 copul-0.0.4/setup.cfg
+-rw-r--r--   0        0        0      771 2024-02-06 10:07:33.037899 copul-0.0.5/copul/__init__.py
+-rw-r--r--   0        0        0      349 2024-02-06 10:07:33.038993 copul-0.0.5/copul/basictools.py
+-rw-r--r--   0        0        0      919 2023-07-28 08:13:00.472893 copul-0.0.5/copul/cdf_wrapper.py
+-rw-r--r--   0        0        0     1535 2023-09-07 12:37:07.549187 copul-0.0.5/copul/chatterjee.py
+-rw-r--r--   0        0        0        0 2023-03-26 14:29:39.006801 copul-0.0.5/copul/docs/.gitkeep
+-rw-r--r--   0        0        0     1741 2024-02-06 10:07:33.038993 copul-0.0.5/copul/double_stochastic_matrix.py
+-rw-r--r--   0        0        0      976 2023-09-07 12:37:07.549187 copul-0.0.5/copul/email_notifier.py
+-rw-r--r--   0        0        0       96 2023-09-12 22:33:41.688323 copul-0.0.5/copul/exceptions.py
+-rw-r--r--   0        0        0     1019 2023-07-28 08:13:00.472893 copul-0.0.5/copul/families/__init__.py
+-rw-r--r--   0        0        0    29456 2024-03-29 22:27:31.563325 copul-0.0.5/copul/families/abstract_copula.py
+-rw-r--r--   0        0        0     5405 2024-04-02 17:27:52.734040 copul-0.0.5/copul/families/archimedean/__init__.py
+-rw-r--r--   0        0        0     7172 2024-02-06 10:07:33.040064 copul-0.0.5/copul/families/archimedean/archimedean_copula.py
+-rw-r--r--   0        0        0     5143 2023-10-07 06:45:17.388610 copul-0.0.5/copul/families/archimedean/derivatives_overview_constructor.py
+-rw-r--r--   0        0        0     2270 2023-10-07 06:45:17.388610 copul-0.0.5/copul/families/archimedean/heavy_compute_arch.py
+-rw-r--r--   0        0        0     3227 2023-10-22 09:01:59.700881 copul-0.0.5/copul/families/archimedean/nelsen1.py
+-rw-r--r--   0        0        0     1389 2023-10-07 06:45:17.390464 copul-0.0.5/copul/families/archimedean/nelsen10.py
+-rw-r--r--   0        0        0     4544 2023-10-07 06:45:17.390464 copul-0.0.5/copul/families/archimedean/nelsen11.py
+-rw-r--r--   0        0        0     1074 2023-10-07 06:45:17.390464 copul-0.0.5/copul/families/archimedean/nelsen12.py
+-rw-r--r--   0        0        0     1370 2023-10-07 06:45:17.392469 copul-0.0.5/copul/families/archimedean/nelsen13.py
+-rw-r--r--   0        0        0     1171 2023-10-07 06:45:17.392469 copul-0.0.5/copul/families/archimedean/nelsen14.py
+-rw-r--r--   0        0        0     1624 2023-10-22 09:09:23.858677 copul-0.0.5/copul/families/archimedean/nelsen15.py
+-rw-r--r--   0        0        0     2296 2024-02-06 10:07:33.040064 copul-0.0.5/copul/families/archimedean/nelsen16.py
+-rw-r--r--   0        0        0    34939 2024-02-06 10:07:33.041082 copul-0.0.5/copul/families/archimedean/nelsen17.py
+-rw-r--r--   0        0        0     2405 2023-10-07 06:45:17.393476 copul-0.0.5/copul/families/archimedean/nelsen18.py
+-rw-r--r--   0        0        0     1250 2023-10-07 06:45:17.393476 copul-0.0.5/copul/families/archimedean/nelsen19.py
+-rw-r--r--   0        0        0     3446 2024-02-06 10:07:33.041986 copul-0.0.5/copul/families/archimedean/nelsen2.py
+-rw-r--r--   0        0        0     2071 2023-10-07 06:45:17.393476 copul-0.0.5/copul/families/archimedean/nelsen20.py
+-rw-r--r--   0        0        0     3391 2024-02-06 10:07:33.041986 copul-0.0.5/copul/families/archimedean/nelsen21.py
+-rw-r--r--   0        0        0     2808 2023-10-07 06:45:17.393476 copul-0.0.5/copul/families/archimedean/nelsen22.py
+-rw-r--r--   0        0        0     2073 2024-02-06 10:07:33.041986 copul-0.0.5/copul/families/archimedean/nelsen3.py
+-rw-r--r--   0        0        0     1506 2023-10-07 06:45:17.393476 copul-0.0.5/copul/families/archimedean/nelsen4.py
+-rw-r--r--   0        0        0     4309 2023-10-07 06:45:17.393476 copul-0.0.5/copul/families/archimedean/nelsen5.py
+-rw-r--r--   0        0        0     2023 2023-10-07 06:45:17.393476 copul-0.0.5/copul/families/archimedean/nelsen6.py
+-rw-r--r--   0        0        0     3007 2023-10-07 06:45:17.393476 copul-0.0.5/copul/families/archimedean/nelsen7.py
+-rw-r--r--   0        0        0     2690 2023-10-07 06:45:17.393476 copul-0.0.5/copul/families/archimedean/nelsen8.py
+-rw-r--r--   0        0        0     2316 2023-10-07 06:45:17.393476 copul-0.0.5/copul/families/archimedean/nelsen9.py
+-rw-r--r--   0        0        0      298 2023-07-31 08:24:10.290358 copul-0.0.5/copul/families/elliptical/__init__.py
+-rw-r--r--   0        0        0     1298 2024-02-06 10:07:33.043079 copul-0.0.5/copul/families/elliptical/elliptical_copula.py
+-rw-r--r--   0        0        0     1859 2024-03-20 21:59:02.740462 copul-0.0.5/copul/families/elliptical/gaussian.py
+-rw-r--r--   0        0        0    11784 2024-02-06 10:07:33.044081 copul-0.0.5/copul/families/elliptical/laplace.py
+-rw-r--r--   0        0        0     1983 2024-04-02 17:27:52.743554 copul-0.0.5/copul/families/elliptical/student_t_copula.py
+-rw-r--r--   0        0        0      740 2023-10-07 06:45:17.393476 copul-0.0.5/copul/families/extreme_value/__init__.py
+-rw-r--r--   0        0        0     1959 2024-02-06 10:07:33.045262 copul-0.0.5/copul/families/extreme_value/bb5.py
+-rw-r--r--   0        0        0     3305 2024-02-06 10:07:33.045262 copul-0.0.5/copul/families/extreme_value/cuadras_auge.py
+-rw-r--r--   0        0        0     6791 2023-10-07 06:45:17.393476 copul-0.0.5/copul/families/extreme_value/extreme_value_copula.py
+-rw-r--r--   0        0        0     7157 2024-02-06 10:07:33.046319 copul-0.0.5/copul/families/extreme_value/galambos.py
+-rw-r--r--   0        0        0     1541 2024-02-06 10:07:33.046319 copul-0.0.5/copul/families/extreme_value/gumbel_hougaard.py
+-rw-r--r--   0        0        0     1209 2024-02-06 10:07:33.046319 copul-0.0.5/copul/families/extreme_value/huesler_reiss.py
+-rw-r--r--   0        0        0     4092 2024-02-06 10:07:33.047321 copul-0.0.5/copul/families/extreme_value/joeev.py
+-rw-r--r--   0        0        0     5350 2024-02-06 10:07:33.047321 copul-0.0.5/copul/families/extreme_value/marshall_olkin.py
+-rw-r--r--   0        0        0     1070 2024-02-06 10:07:33.047321 copul-0.0.5/copul/families/extreme_value/t_ev.py
+-rw-r--r--   0        0        0     3853 2024-02-06 10:07:33.048904 copul-0.0.5/copul/families/extreme_value/tawn.py
+-rw-r--r--   0        0        0        0 2023-07-28 08:13:00.504053 copul-0.0.5/copul/families/other/__init__.py
+-rw-r--r--   0        0        0     1141 2024-02-06 10:07:33.048904 copul-0.0.5/copul/families/other/b11.py
+-rw-r--r--   0        0        0     5378 2024-04-02 17:27:52.748186 copul-0.0.5/copul/families/other/checkerboard_copula.py
+-rw-r--r--   0        0        0     1099 2024-02-06 10:07:33.049910 copul-0.0.5/copul/families/other/farlie_gumbel_morgenstern.py
+-rw-r--r--   0        0        0     4304 2024-02-06 10:07:33.049910 copul-0.0.5/copul/families/other/frechet.py
+-rw-r--r--   0        0        0     1969 2024-02-06 10:07:33.049910 copul-0.0.5/copul/families/other/mardia.py
+-rw-r--r--   0        0        0    10381 2024-02-06 10:07:33.051015 copul-0.0.5/copul/families/other/plackett.py
+-rw-r--r--   0        0        0     3909 2024-02-06 10:07:33.051015 copul-0.0.5/copul/families/other/raftery.py
+-rw-r--r--   0        0        0        0 2024-02-06 10:07:33.051015 copul-0.0.5/copul/schur_order/__init__.py
+-rw-r--r--   0        0        0     1614 2024-02-06 10:07:33.052016 copul-0.0.5/copul/schur_order/checkerboarder.py
+-rw-r--r--   0        0        0     4124 2024-02-06 10:07:33.052016 copul-0.0.5/copul/schur_order/schur_order_verifier.py
+-rw-r--r--   0        0        0     1475 2024-02-06 10:07:33.052016 copul-0.0.5/copul/schur_order/schur_rearranger.py
+-rw-r--r--   0        0        0     4558 2024-04-02 17:27:35.052435 copul-0.0.5/copul/schur_order/schur_visualizer.py
+-rw-r--r--   0        0        0        0 2023-03-26 14:17:19.179954 copul-0.0.5/copul/simulations/__init__.py
+-rw-r--r--   0        0        0     4797 2024-04-02 17:27:35.069080 copul-0.0.5/copul/simulations/sample_from_cifm.R
+-rw-r--r--   0        0        0     1893 2024-04-02 17:27:35.086735 copul-0.0.5/copul/simulations/sample_from_csfm.R
+-rw-r--r--   0        0        0     1231 2024-02-06 10:07:33.053053 copul-0.0.5/copul/sympy_wrapper.py
+-rw-r--r--   0        0        0     1066 2024-04-02 17:51:00.743285 copul-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 copul-0.0.5/PKG-INFO
```

### Comparing `copul-0.0.4/copul/families/abstract_copula.py` & `copul-0.0.5/copul/families/archimedean/heavy_compute_arch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,59 @@
+import logging
+import random
+import warnings
+
+import numpy as np
 import sympy
-from spb import plot3d
+from scipy import optimize
+
+from copul.families.archimedean.archimedean_copula import ArchimedeanCopula
+
+log = logging.getLogger(__name__)
 
 
-class AbstractCopula:
-    u, v = sympy.symbols("u v", positive=True)
+class HeavyComputeArch(ArchimedeanCopula):
 
-    def __call__(self, **kwargs):
-        self._are_class_vars(kwargs)
-        for k, v in kwargs.items():
-            setattr(self, k, v)
-        return self
-
-    def _are_class_vars(self, kwargs):
-        class_vars = set(dir(self))
-        assert set(kwargs).issubset(class_vars), f"keys: {set(kwargs)}, free symbols: {class_vars}"
-
-    @property
-    def cdf(self):
-        return None
-
-    @property
-    def pdf(self):
-        return sympy.simplify(sympy.diff(self.cdf, self.u, self.v))
-
-    @property
-    def log_pdf(self, expand_log=False):
-        log_pdf = sympy.simplify(sympy.log(self.pdf))
-        return concrete_expand_log(log_pdf) if expand_log else log_pdf
-
-    def plot_cdf(self):
-        free_symbols = set(self.cdf.func.free_symbols) - {self.u, self.v}
-        free_symbol_dict = {str(s): getattr(self, str(s)) for s in free_symbols}
-        cdf = self.cdf(**free_symbol_dict).func
-        return plot3d(cdf, (self.u, 0, 1), (self.v, 0, 1),
-                      title=f"{type(self).__name__} Copula",
-                      xlabel="u", ylabel="v", zlabel="CDF", zlim=(0, 1))
-
-    def plot_pdf(self):
-        free_symbols = set(self.pdf.func.free_symbols) - {self.u, self.v}
-        free_symbol_dict = {str(s): getattr(self, str(s)) for s in free_symbols}
-        pdf = self.pdf(**free_symbol_dict).func
-        return plot3d(pdf, (self.u, 0, 1), (self.v, 0, 1),
-                      title=f"{type(self).__name__} Copula",
-                      xlabel="u", ylabel="v", zlabel="PDF")
-
-
-def round_expression(expr, n=2):
-    expr = sympy.simplify(expr)
-    for a in sympy.preorder_traversal(expr):
-        if isinstance(a, sympy.Float):
-            expr = expr.subs(a, round(a, n))
-    return expr
-
-
-def concrete_expand_log(expr, first_call=True):
-    import sympy as sp
-    if first_call:
-        expr = sp.expand_log(expr, force=True)
-    func = expr.func
-    args = expr.args
-    if args == ():
-        return expr
-    if func == sp.log and args[0].func == sp.concrete.products.Product:
-        prod = args[0]
-        term = prod.args[0]
-        indices = prod.args[1:]
-        return sp.Sum(sp.log(term), *indices)
-    return func(*map(lambda x: concrete_expand_log(x, False), args))
+    def rvs(self, n=1):
+        """Sample a value from the copula"""
+        results = []
+        for _ in range(n):
+            v = random.uniform(0, 1)
+            sympy_func = self.cond_distr_2().subs(self.v, v).func
+            function = sympy.lambdify(self.u, sympy_func, ["numpy"])
+            sympy_func = self.cond_distr_2().subs(self.v, v).func
+            result = np.array([self._sample_values(function, v, sympy_func) for _ in range(1)])
+            results.append(result)
+            # array of lists to array
+        print(self.err_counter)
+        return np.concatenate(results)
+
+    def _sample_values(self, function, v, sympy_func):
+        t = random.uniform(0, 1)
+
+        def func2(u):
+            return function(u) - t
+
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=RuntimeWarning)
+            try:
+                result = optimize.root_scalar(func2, x0=0.5, bracket=[0.00000001, 0.99999999])
+            except (ZeroDivisionError, ValueError, TypeError) as e:
+                log.debug(f"{self.__class__.__name__}; {type(e).__name__}: {e}")
+                self.err_counter += 1
+                return self._get_visual_solution(sympy_func - t), v
+            if not result.converged:
+                if not result.iterations:
+                    print(self.__class__.__name__)
+                self.err_counter += 1
+                return self._get_visual_solution(sympy_func - t), v
+            return result.root, v
+
+    def _get_visual_solution(self, func):
+        x_values = np.linspace(0.001, 0.999, 100)
+        y_values = np.array([func.subs(self.u, val) for val in x_values])
+        try:
+            first_positive_index = np.where(y_values > 0)[0][0]
+        except IndexError:
+            # log.warning(f"{self.__class__.__name__}: {func} has no positive values")
+            first_positive_index = np.argmax(y_values)
+        return x_values[first_positive_index]
```

### Comparing `copul-0.0.4/copul/families/archimedean/__init__.py` & `copul-0.0.5/copul/families/archimedean/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 import re
 
 import pandas as pd
 import sympy
 
-from copul.families.abstract_copula import round_expression
+from copul.families import round_expression
 
-from copul.families.archimedean.nelsen1 import Nelsen1, Clayton
 from copul.families.archimedean.nelsen2 import Nelsen2
-from copul.families.archimedean.nelsen3 import Nelsen3, AliMikhailHak
-from copul.families.archimedean.nelsen4 import Nelsen4, GumbellHougaard
+from copul.families.archimedean.nelsen4 import Nelsen4, GumbelHougaard
 from copul.families.archimedean.nelsen5 import Nelsen5, Frank
-from copul.families.archimedean.nelsen6 import Nelsen6, Joe
-from copul.families.archimedean.nelsen7 import Nelsen7
 from copul.families.archimedean.nelsen8 import Nelsen8
-from copul.families.archimedean.nelsen9 import Nelsen9, GumbellBarnett
+from copul.families.archimedean.nelsen9 import Nelsen9, GumbelBarnett
 from copul.families.archimedean.nelsen10 import Nelsen10
-from copul.families.archimedean.nelsen11 import Nelsen11
 from copul.families.archimedean.nelsen12 import Nelsen12
-from copul.families.archimedean.nelsen13 import Nelsen13
 from copul.families.archimedean.nelsen14 import Nelsen14
-from copul.families.archimedean.nelsen15 import Nelsen15, GenestGhoudi
+from cop.copul.families.archimedean.nelsen15 import Nelsen15, GenestGhoudi
 from copul.families.archimedean.nelsen16 import Nelsen16
 from copul.families.archimedean.nelsen17 import Nelsen17
 from copul.families.archimedean.nelsen18 import Nelsen18
-from copul.families.archimedean.nelsen19 import Nelsen19
 from copul.families.archimedean.nelsen20 import Nelsen20
 from copul.families.archimedean.nelsen21 import Nelsen21
 from copul.families.archimedean.nelsen22 import Nelsen22
 
 
 def cleanse_latex_str(latex_str):
     def cleanse_this(input_str):
@@ -56,66 +49,100 @@
     my_copula = Nelsen17(theta_min=0)
     # conv_func, log_der_val, log_der2_val, local_min_point, local_min_val = my_copula.log2_der()
     df = pd.DataFrame(index=my_range)
     for i in my_range:
         copula_str = f"Nelsen{str(i)}"
         print(copula_str)
         copula = locals()[copula_str](theta_min=0)
-        gen_val = copula.generator
-        gen_der_val = copula.first_deriv_of_generator
-        gen_der2_val = copula.second_deriv_of_gen
+        gen_val = copula.inv_generator
+        gen_der_val = copula.first_deriv_of_inv_gen
+        gen_der2_val = copula.second_deriv_of_inv_gen
         cop_val = copula.cdf
-        conv_func, log_der_val, log_der2_val, local_min_point, local_min_val = copula.log_der()
-        conv2_func, log2_deriv_val, log2_deriv2_val, local2_min_point, local2_min_val = copula.log2_der()
+        (
+            conv_func,
+            log_der_val,
+            log_der2_val,
+            local_min_point,
+            local_min_val,
+        ) = copula.log_der()
+        (
+            conv2_func,
+            log2_deriv_val,
+            log2_deriv2_val,
+            local2_min_point,
+            local2_min_val,
+        ) = copula.log2_der()
         df.loc[i, cop] = "$" + sympy.latex(cop_val) + "$"
         df.loc[i, "$\\theta$"] = str(copula.theta_interval)
-        df.loc[i, inv_gen] = "$" + sympy.latex(copula.inverse_generator) + "$"
-        df.loc[i, inv_gen_max] = str(copula.compute_inv_gen_max())
+        df.loc[i, inv_gen] = "$" + sympy.latex(copula.generator) + "$"
+        df.loc[i, inv_gen_max] = str(copula.compute_gen_max())
         df.loc[i, gen] = "$" + sympy.latex(gen_val) + "$"
         df.loc[i, gen_der] = "$" + sympy.latex(gen_der_val) + "$"
         df.loc[i, mustbeconv] = "$" + sympy.latex(conv_func) + "$"
         df.loc[i, log_der] = "$" + sympy.latex(log_der_val) + "$"
         df.loc[i, log_der2] = "$" + sympy.latex(log_der2_val) + "$"
-        df.loc[i, f"{log_der2}-min"] = "$" + sympy.latex((local_min_point, local_min_val)) + "$"
+        df.loc[i, f"{log_der2}-min"] = (
+            "$" + sympy.latex((local_min_point, local_min_val)) + "$"
+        )
         df.loc[i, gen_der2] = "$" + sympy.latex(gen_der2_val) + "$"
         df.loc[i, mustbeconv2] = "$" + sympy.latex(conv2_func) + "$"
         df.loc[i, log2_der] = "$" + sympy.latex(log2_deriv_val) + "$"
         df.loc[i, log2_der2] = "$" + sympy.latex(log2_deriv2_val) + "$"
         df.loc[i, f"{log2_der2}-min"] = (
-                "$" + sympy.latex((local2_min_point, local2_min_val)) + "$"
+            "$" + sympy.latex((local2_min_point, local2_min_val)) + "$"
         )
     return df
 
 
-if __name__ == "__main__":
-    cop = Nelsen17()
-    gen = cop.generator.subs(cop.theta, 5.5)
-    diff2 = round_expression(sympy.diff(gen, cop.y, 2))
-    diff3 = round_expression(sympy.diff(gen, cop.y, 3))
-    diff4 = round_expression(sympy.diff(gen, cop.y, 4))
-    diff5 = round_expression(sympy.diff(gen, cop.y, 5))
-    diff6 = round_expression(sympy.diff(gen, cop.y, 6))
-    diff7 = round_expression(sympy.diff(gen, cop.y, 7))
-    my_gen_plot = sympy.plotting.plot(diff2, (cop.y, 5, 20), show=False, legend=True)
-    my_gen_plot.show()
-    cdf = cop.cdf().subs(cop.theta, 0.5)
-    my_range = list(range(16, 17))
+def produce_latex_tables():
+    my_range = list(range(1, 23))
     df = generate_notes_pdf(my_range)
-    pd.set_option('display.max_colwidth', None)
-    tables = {"Nelsen" + str(i): df.T[[i]].reset_index().rename(columns={i: "Value", "index": "Characteristic"}) for i
-              in my_range}
-    table_strs = [cleanse_latex_str(v.to_latex(escape=False)) + "\\caption{" + k + "}\\label{tab:" + k + "}" for k, v in
-                  tables.items()]
-
+    pd.set_option("display.max_colwidth", None)
+    tables = {
+        f"Nelsen{i}": df.T[[i]]
+        .reset_index()
+        .rename(columns={i: "Value", "index": "Characteristic"})
+        for i in my_range
+    }
+    table_strs = [
+        cleanse_latex_str(v.to_latex(escape=False))
+        + "\\caption{"
+        + k
+        + "}\\label{tab:"
+        + k
+        + "}"
+        for k, v in tables.items()
+    ]
 
     def table_to_formula(k, v):
         v = v.drop(v.index[[0, 1, 2, 3, 9, 14]])
-        return "\item " + k + ": \n\\begin{align}\n" + (v["Characteristic"] + " ~=~ & " + cleanse_latex_str(
-            v["Value"]) + ", \\nonumber\\\\").str.replace("$", "").str.cat(
-            sep="\n")[:-13] + "\\nonumber" + ".\n\\end{align}\n"
+        return (
+            "\item "
+            + k
+            + ": \n\\begin{align}\n"
+            + (
+                v["Characteristic"]
+                + " ~=~ & "
+                + cleanse_latex_str(v["Value"])
+                + ", \\nonumber\\\\"
+            )
+            .str.replace("$", "")
+            .str.cat(sep="\n")[:-13]
+            + "\\nonumber"
+            + ".\n\\end{align}\n"
+        )
 
     table_strs2 = {k: table_to_formula(k, v) for k, v in tables.items()}
     start_str = "\\begin{table}[H]\\begin{center}"
     end_str = "\\end{center}\\end{table}"
     full_table = "\n\n".join([start_str + tab + end_str for tab in table_strs])
-    full_table2 = "\\begin{itemize}\n" + "\n\n".join([table_strs2[tab] for tab in table_strs2]) + "\\end{itemize}"
+    full_table2 = (
+        "\\begin{itemize}\n"
+        + "\n\n".join([table_strs2[tab] for tab in table_strs2])
+        + "\\end{itemize}"
+    )
+    return full_table, full_table2
+
+
+if __name__ == "__main__":
+    table, table2 = produce_latex_tables()
     exit()
```

### Comparing `copul-0.0.4/copul/families/archimedean/archimedean_copula.py` & `copul-0.0.5/copul/families/archimedean/archimedean_copula.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,193 @@
+from abc import ABC
+
 import numpy as np
 import sympy
 from scipy import optimize
-
-from copul.families import get_simplified_solution
-from copul.families.abstract_copula import AbstractCopula, concrete_expand_log
+from copul.families import concrete_expand_log, get_simplified_solution
+from copul.families.abstract_copula import AbstractCopula
 from copul.sympy_wrapper import SymPyFunctionWrapper
 
 
-class ArchimedeanCopula(AbstractCopula):
+class ArchimedeanCopula(AbstractCopula, ABC):
     _t_min = 0
     _t_max = 1
-    y, t, theta = sympy.symbols("y t theta", positive=True)
+    y, t = sympy.symbols("y t", positive=True)
+    theta = sympy.symbols("theta")
     theta_interval = None
-    _inv_generator = None
+    params = [theta]
 
-    def __init__(self, theta_min=None, theta_max=None):
+    def __init__(self, theta_min=None, theta_max=None, **kwargs):
         if theta_min is not None:
-            self.theta_interval = sympy.Interval(theta_min, self.theta_max, left_open=self.theta_interval.left_open,
-                                                 right_open=self.theta_interval.right_open)
+            self.theta_interval = sympy.Interval(
+                theta_min,
+                self.theta_max,
+                left_open=self.theta_interval.left_open,
+                right_open=self.theta_interval.right_open,
+            )
         if theta_max is not None:
-            self.theta_interval = sympy.Interval(self.theta_min, theta_max, left_open=self.theta_interval.left_open,
-                                                 right_open=self.theta_interval.right_open)
+            self.theta_interval = sympy.Interval(
+                self.theta_min,
+                theta_max,
+                left_open=self.theta_interval.left_open,
+                right_open=self.theta_interval.right_open,
+            )
+        super().__init__(**kwargs)
+
+    def __str__(self):
+        return f"{self.__class__.__name__}({self.theta})"
+
+    @property
+    def is_symmetric(self) -> bool:
+        return True
+
+    @property
+    def intervals(self):
+        return {"theta": self.theta_interval}
+
+    @property
+    def _generator(self):
+        raise NotImplementedError
 
     @property
-    def inverse_generator(self):
-        return SymPyFunctionWrapper(self._inv_generator)
+    def generator(self):
+        return SymPyFunctionWrapper(self._generator)
 
     @property
     def theta_max(self):
         return self.theta_interval.closure.end
 
     @property
     def theta_min(self):
         return self.theta_interval.closure.inf
 
     @property
     def cdf(self):
-        """ Cumulative distribution function of the copula """
-        gen = self.generator
-        inv_gen_at_u = self._inv_generator.subs(self.t, self.u)
-        inv_gen_at_v = self._inv_generator.subs(self.t, self.v)
-        cdf = gen.subs(self.y, inv_gen_at_u + inv_gen_at_v)
+        """Cumulative distribution function of the copula"""
+        inv_gen_at_u = self._generator.subs(self.t, self.u)
+        inv_gen_at_v = self._generator.subs(self.t, self.v)
+        cdf = self.inv_generator.subs(self.y, inv_gen_at_u + inv_gen_at_v)
         return SymPyFunctionWrapper(get_simplified_solution(cdf.func))
 
     @property
     def pdf(self):
-        """ Probability density function of the copula """
-        cdf = self.cdf
-        first_diff = sympy.diff(cdf, self.u)
-        pdf = sympy.diff(first_diff, self.v)
-        simplified_pdf = get_simplified_solution(pdf.func)
-        return SymPyFunctionWrapper(simplified_pdf)
+        """Probability density function of the copula"""
+        first_diff = sympy.diff(self.cdf, self.u)
+        return sympy.diff(first_diff, self.v)
 
     @property
-    def generator(self) -> SymPyFunctionWrapper:
-        eq = sympy.Eq(self.y, self._inv_generator)
+    def inv_generator(self) -> SymPyFunctionWrapper:
+        eq = sympy.Eq(self.y, self._generator)
         sol = sympy.solve([eq, self.theta > 0, self.y > 0], self.t)
         my_sol = sol[self.t] if isinstance(sol, dict) else sol[0]
         my_simplified_sol = get_simplified_solution(my_sol)
         return SymPyFunctionWrapper(my_simplified_sol)
 
     @property
-    def first_deriv_of_generator(self):
-        diff = sympy.diff(self.generator.func, self.y)
+    def first_deriv_of_inv_gen(self):
+        diff = sympy.diff(self.inv_generator.func, self.y)
         return sympy.simplify(diff)
 
+    def tau(self):
+        inv_gen = self.generator.func
+        print("inv gen: ", inv_gen)
+        print("inv gen latex: ", sympy.latex(inv_gen))
+        inv_gen_diff = sympy.diff(inv_gen, self.t)
+        print("inv gen diff: ", inv_gen_diff)
+        print("inv gen diff latex: ", sympy.latex(inv_gen_diff))
+        frac = inv_gen / inv_gen_diff
+        print("frac: ", frac)
+        print("frac latex: ", sympy.latex(frac))
+        integral = sympy.integrate(frac, (self.t, 0, 1))
+        print("integral: ", integral)
+        print("integral latex: ", sympy.latex(integral))
+        tau = 1 + 4 * integral
+        print("tau: ", tau)
+        print("tau latex: ", sympy.latex(tau))
+        return tau
+
     @property
-    def second_deriv_of_gen(self):
-        first_diff = self.first_deriv_of_generator
+    def second_deriv_of_inv_gen(self):
+        first_diff = self.first_deriv_of_inv_gen
         second_diff = sympy.diff(first_diff, self.y)
         return sympy.simplify(second_diff)
 
+    def ltd_char(self):
+        return sympy.simplify(sympy.log(self.inv_generator.func))
+
+    def diff2_ltd_char(self):
+        beauty_func = self.ltd_char()
+        diff2 = sympy.diff(beauty_func, self.y, 2)
+        return sympy.simplify(diff2)
+
     @property
     def ci_char(self):
-        minus_gen_deriv = - self.first_deriv_of_generator
+        minus_gen_deriv = -self.first_deriv_of_inv_gen
         beauty_deriv = concrete_expand_log(sympy.simplify(sympy.log(minus_gen_deriv)))
         return SymPyFunctionWrapper(beauty_deriv)
 
-    @property
     def first_deriv_of_ci_char(self):
         chi_char_func = self.ci_char()
         return sympy.simplify(sympy.diff(chi_char_func, self.y))
 
-    @property
     def second_deriv_of_ci_char(self):
         chi_char_func_deriv = self.first_deriv_of_ci_char()
         return sympy.simplify(sympy.diff(chi_char_func_deriv, self.y))
 
-    @property
-    def mtp2_char(self):
-        second_deriv = self.second_deriv_of_gen
+    def tp2_char(self, u, v):
+        second_deriv = self.second_deriv_of_inv_gen.subs([(self.u, u), (self.v, v)])
         beauty_2deriv = concrete_expand_log(sympy.simplify(sympy.log(second_deriv)))
+        print(sympy.latex(second_deriv))
         return SymPyFunctionWrapper(beauty_2deriv)
 
-    @property
-    def first_deriv_of_mtp2_char(self):
-        mtp2_char = self.mtp2_char()
-        return sympy.simplify(sympy.diff(mtp2_char, self.y))
+    def first_deriv_of_tp2_char(self):
+        mtp2_char = self.tp2_char(self.u, self.v)
+        return sympy.simplify(sympy.diff(mtp2_char.func, self.y))
 
-    @property
-    def second_deriv_of_mtp2_char(self):
-        mtp2_char_deriv = self.first_deriv_of_mtp2_char()
-        return sympy.simplify(sympy.diff(mtp2_char_deriv, self.y))
+    def second_deriv_of_tp2_char(self):
+        return sympy.simplify(sympy.diff(self.tp2_char(self.u, self.v).func, self.y, 2))
 
     @property
     def log_der(self):
         minus_log_derivative = self.ci_char()
         first_deriv = self.first_deriv_of_ci_char()
         second_deriv = self.second_deriv_of_ci_char()
         return self._compute_log2_der_of(first_deriv, minus_log_derivative, second_deriv)
 
     @property
     def log2_der(self):
-        log_second_derivative = self.mtp2_char()
-        first_deriv = self.first_deriv_of_mtp2_char()
-        second_deriv = self.second_deriv_of_mtp2_char()
+        log_second_derivative = self.tp2_char(self.u, self.v)
+        first_deriv = self.first_deriv_of_tp2_char()
+        second_deriv = self.second_deriv_of_tp2_char()
         return self._compute_log2_der_of(first_deriv, log_second_derivative, second_deriv)
 
     def _compute_log2_der_of(self, first_deriv, log_second_derivative, second_deriv):
         log_der_lambda = sympy.lambdify([(self.y, self.theta)], second_deriv)
         bounds = [(self._t_min, self._t_max), (self.theta_min, self.theta_max)]
-        starting_point = np.array([min(self._t_min + 0.5, self._t_max), min(self.theta_min + 0.5, self.theta_max)])
+        starting_point = np.array(
+            [min(self._t_min + 0.5, self._t_max), min(self.theta_min + 0.5, self.theta_max)]
+        )
         min_val = optimize.minimize(log_der_lambda, starting_point, bounds=bounds)
-        return log_second_derivative, first_deriv, second_deriv, [round(val, 2) for val in min_val.x], round(
-            log_der_lambda(min_val.x), 2)
+        return (
+            log_second_derivative,
+            first_deriv,
+            second_deriv,
+            [round(val, 2) for val in min_val.x],
+            round(log_der_lambda(min_val.x), 2),
+        )
 
-    def compute_inv_gen_max(self):
+    def compute_gen_max(self):
         try:
-            limit = sympy.limit(self._inv_generator, self.t, 0)
+            limit = sympy.limit(self._generator, self.t, 0)
         except TypeError:
-            limit = sympy.limit(self._inv_generator.subs(self.theta, (self.theta_max - self.theta_min) / 2), self.t, 0)
+            limit = sympy.limit(
+                self._generator.subs(self.theta, (self.theta_max - self.theta_min) / 2), self.t, 0
+            )
         return sympy.simplify(limit)
+
+    def lambda_L(self):
+        expr = self.inv_generator(y=2 * self.y).func / self.inv_generator(y=self.y).func
+        return sympy.limit(expr, self.y, sympy.oo, dir="-")
+
+    def lambda_U(self):
+        expr = (1 - self.inv_generator(y=2 * self.y).func) / (1 - self.inv_generator(y=self.y).func)
+        return sympy.simplify(2 - sympy.limit(expr, self.y, 0, dir="+"))
```

### Comparing `copul-0.0.4/copul/families/archimedean/derivatives_overview_constructor.py` & `copul-0.0.5/copul/families/archimedean/derivatives_overview_constructor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 
 import pandas as pd
 import sympy
 
-import families.archimedean.nelsen2
+import copul
 
 
 class DerivativesOverviewConstructor:
 
     def __init__(self):
         pass
 
@@ -33,31 +33,31 @@
         mustbeconv = "$\\log(-\\psi')(y)$"
         log_der = "$(\\log(-\\psi'))'(y)$"
         log_der2 = "$(\\log(-\\psi'))''(y)$"
         gen_der2 = "$\\psi''(y)$"
         mustbeconv2 = "$\\log(\\psi'')(y)$"
         log2_der = "$(\\log(\\psi''))'(y)$"
         log2_der2 = "$(\\log(\\psi''))''(y)$"
-        my_copula = families.archimedean.nelsen17.Nelsen17(theta_min=0)
+        my_copula = copul.families.archimedean.nelsen17.Nelsen17(theta_min=0)
         # conv_func, log_der_val, log_der2_val, local_min_point, local_min_val = my_copula.log2_der()
         df = pd.DataFrame(index=my_range)
         for i in my_range:
             copula_str = f"Nelsen{i}"
             print(copula_str)
             copula = locals()[copula_str](theta_min=0)
-            gen_val = copula.generator
-            gen_der_val = copula.first_deriv_of_generator()
-            gen_der2_val = copula.second_deriv_of_gen
+            gen_val = copula.inv_generator
+            gen_der_val = copula.first_deriv_of_inv_gen()
+            gen_der2_val = copula.second_deriv_of_inv_gen
             cop_val = copula.cdf
             conv_func, log_der_val, log_der2_val, local_min_point, local_min_val = copula.log_der()
             conv2_func, log2_deriv_val, log2_deriv2_val, local2_min_point, local2_min_val = copula.log2_der()
             df.loc[i, cop] = "$" + sympy.latex(cop_val) + "$"
             df.loc[i, "$\\theta$"] = str(copula.theta_interval)
-            df.loc[i, inv_gen] = "$" + sympy.latex(copula.inverse_generator) + "$"
-            df.loc[i, inv_gen_max] = str(copula.compute_inv_gen_max())
+            df.loc[i, inv_gen] = "$" + sympy.latex(copula.generator) + "$"
+            df.loc[i, inv_gen_max] = str(copula.compute_gen_max())
             df.loc[i, gen] = "$" + sympy.latex(gen_val) + "$"
             df.loc[i, gen_der] = "$" + sympy.latex(gen_der_val) + "$"
             df.loc[i, mustbeconv] = "$" + sympy.latex(conv_func) + "$"
             df.loc[i, log_der] = "$" + sympy.latex(log_der_val) + "$"
             df.loc[i, log_der2] = "$" + sympy.latex(log_der2_val) + "$"
             df.loc[i, f"{log_der2}-min"] = f"${sympy.latex((local_min_point, local_min_val))}$"
             df.loc[i, gen_der2] = f"${sympy.latex(gen_der2_val)}$"
@@ -94,15 +94,15 @@
     for a in sympy.preorder_traversal(expr):
         if isinstance(a, sympy.Float):
             expr = expr.subs(a, round(a, 2))
     return expr
 
 
 if __name__ == "__main__":
-    my_cop = families.archimedean.nelsen2.Nelsen2()
+    my_cop = copul.families.archimedean.nelsen2.Nelsen2()
     # gen = cop.generator().subs(cop.theta, 5.5)
     # diff2 = round_expression(sympy.diff(gen, cop.y, 2))
     # diff3 = round_expression(sympy.diff(gen, cop.y, 3))
     # diff4 = round_expression(sympy.diff(gen, cop.y, 4))
     # diff5 = round_expression(sympy.diff(gen, cop.y, 5))
     # diff6 = round_expression(sympy.diff(gen, cop.y, 6))
     # diff7 = round_expression(sympy.diff(gen, cop.y, 7))
```

### Comparing `copul-0.0.4/copul/families/archimedean/nelsen1.py` & `copul-0.0.5/copul/families/archimedean/nelsen14.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import numpy as np
 import sympy
 
 from copul.families.archimedean.archimedean_copula import ArchimedeanCopula
 from copul.sympy_wrapper import SymPyFunctionWrapper
 
 
-class Clayton(ArchimedeanCopula):
+class Nelsen14(ArchimedeanCopula):
     ac = ArchimedeanCopula
-    _inv_generator = ((1 / ac.t) ** ac.theta - 1) / ac.theta
-    theta_interval = sympy.Interval(0, np.inf, left_open=False, right_open=True)
+    theta = sympy.symbols("theta", positive=True)
+    theta_interval = sympy.Interval(1, np.inf, left_open=False, right_open=True)
 
     @property
-    def generator(self):  # ToDo add indicator
-        return SymPyFunctionWrapper((self.theta * self.y + 1)**(-1/self.theta))
+    def is_absolutely_continuous(self) -> bool:
+        return True
 
     @property
-    def cdf(self):
-        cdf = sympy.Max(
-            (self.u ** (-self.theta) + self.v ** (-self.theta) - 1)
-            ** (-1 / self.theta),
-            0,
-        )
-        return SymPyFunctionWrapper(cdf)
+    def _generator(self):
+        return (self.t ** (-1 / self.theta) - 1) ** self.theta
+
+    @property
+    def inv_generator(self):
+        gen = (self.y ** (1 / self.theta) + 1) ** (-self.theta)
+        return SymPyFunctionWrapper(gen)
 
     @property
-    def pdf(self):
-        pdf = sympy.Max(
-            0,
-            (self.u ** (-self.theta) + self.v ** (-self.theta) - 1)
-            ** (-2 - 1 / self.theta)
-            * self.u ** (-self.theta - 1)
-            * self.v ** (-self.theta - 1)
-            * (self.theta + 1),
-        )
-        return SymPyFunctionWrapper(pdf)
+    def cdf(self):
+        cdf = (
+            1
+            + (
+                (self.u ** (-1 / self.theta) - 1) ** self.theta
+                + (self.v ** (-1 / self.theta) - 1) ** self.theta
+            )
+            ** (1 / self.theta)
+        ) ** (-self.theta)
+        return SymPyFunctionWrapper(cdf)
 
+    def lambda_L(self):
+        return 1 / 2
 
-Nelsen1 = Clayton
+    def lambda_U(self):
+        return 2 - 2 ** (1 / self.theta)
```

### Comparing `copul-0.0.4/copul/families/archimedean/nelsen16.py` & `copul-0.0.5/copul/families/other/farlie_gumbel_morgenstern.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,43 @@
-import numpy as np
 import sympy
 
-from copul.families.archimedean.archimedean_copula import ArchimedeanCopula
+from copul.families.abstract_copula import AbstractCopula
 from copul.sympy_wrapper import SymPyFunctionWrapper
 
 
-class Nelsen16(ArchimedeanCopula):
-    ac = ArchimedeanCopula
-    _inv_generator = (ac.theta / ac.t + 1) * (1 - ac.t)
-    theta_interval = sympy.Interval(0, np.inf, left_open=True, right_open=True)
-
-    @property
-    def generator(self):
-        gen = (
-            -self.theta / 2
-            - self.y / 2
-            + 1 / 2
-            + 1 / 2 * sympy.sqrt((self.theta + self.y - 1) ** 2 + 4 * self.theta)
-        )
-        return SymPyFunctionWrapper(gen)
-
-    @property
-    def first_deriv_of_generator(self):
-        return (self.theta + self.y - 1) / (
-            2 * ((self.theta + self.y - 1) ** 2 + 4 * self.theta)
-        ) - 1 / 2
-
-    @property
-    def ci_char(self):
-        ci_char = sympy.log(
-            1 / 2
-            - (self.theta + self.y - 1) / (8 * self.theta + 2 * (self.theta + self.y - 1) ** 2)
-        )
-        return SymPyFunctionWrapper(ci_char)
+class FarlieGumbelMorgenstern(AbstractCopula):
+    theta = sympy.symbols("theta")
+    params = [theta]
+    intervals = {"theta": sympy.Interval(-1, 1, left_open=False, right_open=False)}
+
+    @property
+    def is_absolutely_continuous(self) -> bool:
+        return True
+
+    @property
+    def is_symmetric(self) -> bool:
+        return True
+
+    @property
+    def cdf(self):
+        u = self.u
+        v = self.v
+        cdf = u * v + self.theta * u * v * (1 - u) * (1 - v)
+        return SymPyFunctionWrapper(cdf)
+
+    def cond_distr_2(self):
+        return SymPyFunctionWrapper(self.u + self.theta * self.u * (1 - self.u) * (1 - 2 * self.v))
+
+    @property
+    def pdf(self):
+        return 1 + self.theta * (1 - 2 * self.u) * (1 - 2 * self.v)
+
+    @property
+    def spearmans_rho(self):
+        return self.theta / 3
+
+    @property
+    def kendalls_tau(self):
+        return 2 * self.theta / 9
+
+
+B10 = FarlieGumbelMorgenstern
```

### Comparing `copul-0.0.4/copul/families/archimedean/nelsen17.py` & `copul-0.0.5/copul/families/extreme_value/gumbel_hougaard.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,50 @@
 import numpy as np
 import sympy
 
-from copul.families.archimedean.archimedean_copula import ArchimedeanCopula
+from copul.families.extreme_value.extreme_value_copula import ExtremeValueCopula
+from copul.sympy_wrapper import SymPyFunctionWrapper
 
 
-class Nelsen17(ArchimedeanCopula):
-    ac = ArchimedeanCopula
-    _inv_generator = -sympy.log(((1 + ac.t) ** (-ac.theta) - 1) / (2 ** (-ac.theta) - 1))
-    theta_interval = sympy.Interval(-np.inf, np.inf, left_open=False, right_open=True)
+class GumbelHougaard(ExtremeValueCopula):
+    @property
+    def is_absolutely_continuous(self) -> bool:
+        return True
 
     @property
-    def first_deriv_of_generator(self):
-        return sympy.simplify(
-            (
-                2**self.theta
-                * sympy.exp(self.y)
-                / (2**self.theta * sympy.exp(self.y) - 2**self.theta + 1)
-            )
-            ** (1 / self.theta)
-            * (2**self.theta * (-(2**self.theta) + 1))
-            / (
-                2**self.theta
-                * self.theta
-                * (2**self.theta * sympy.exp(self.y) - 2**self.theta + 1)
-            )
-        )
+    def is_symmetric(self) -> bool:
+        return True
+
+    theta = sympy.symbols("theta", positive=True)
+    params = [theta]
+    intervals = {"theta": sympy.Interval(1, np.inf, left_open=False, right_open=True)}
 
     @property
-    def second_deriv_of_gen(self):
-        return sympy.simplify(
-            (
-                2**self.theta
-                * sympy.exp(self.y)
-                / (2**self.theta * sympy.exp(self.y) - 2**self.theta + 1)
-            )
-            ** (1 / self.theta)
-            * (
-                2**self.theta * self.theta * (-(2**self.theta) + 1) * sympy.exp(self.y)
-                - 2 ** (self.theta + 1) * self.theta * (-(2**self.theta) + 1) * sympy.exp(self.y)
-                + (2**self.theta - 1) ** 2
-            )
-            / (self.theta**2 * (2**self.theta * sympy.exp(self.y) - 2**self.theta + 1) ** 2)
-        )
+    def pickand(self):
+        return (self.t**self.theta + (1 - self.t) ** self.theta) ** (1 / self.theta)
 
     @property
-    def first_deriv_of_ci_char(self):
-        return sympy.simplify(
-            (
-                2**self.theta * (-(2**self.theta) + 1)
-                - 4**self.theta * self.theta * sympy.exp(self.y)
-            )
-            / (
-                2**self.theta
-                * self.theta
-                * (2**self.theta * sympy.exp(self.y) - 2**self.theta + 1)
+    def cdf(self):
+        cdf = sympy.exp(
+            -(
+                (sympy.log(1 / self.v) ** self.theta + sympy.log(1 / self.u) ** self.theta)
+                ** (1 / self.theta)
             )
         )
+        return SymPyFunctionWrapper(cdf)
 
-    def first_deriv_of_mtp2_char(self):
-        return 1 / self.theta + 2**self.theta * sympy.exp(self.y) * (
-            1 / (2**self.theta * sympy.exp(self.y) - 2**self.theta + 1)
-            + self.theta / (2**self.theta * self.theta * sympy.exp(self.y) + 2**self.theta + 1)
-            - 1
-            / (
-                2**self.theta * self.theta * sympy.exp(self.y)
-                - 2**self.theta * self.theta
-                + self.theta
-            )
-        )
+    def _rho(self):
+        t = self.t
+        theta = self.theta
+        integrand = ((t**theta + (1 - t) ** theta) ** (1 / theta) + 1) ** (-2)
+        sympy.plot(integrand.subs(theta, 2), (t, 0, 1))
+        # integrand = (
+        #     (t * (1 - t)) ** (1 / theta - 1)
+        #     / (1 + t ** (1 / theta) + (1 - t) ** (1 / theta)) ** 2
+        #     * 1
+        #     / theta
+        # )
+        # sympy.plot(integrand.subs(theta, 2), (t, 0, 1))
+        return 12 * sympy.Integral(integrand, (t, 0, 1)) - 3
+
+    def tau(self):
+        return (self.theta - 1) / self.theta
```

### Comparing `copul-0.0.4/copul/families/archimedean/nelsen8.py` & `copul-0.0.5/copul/families/archimedean/nelsen19.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,38 @@
 import numpy as np
 import sympy
 
 from copul.families.archimedean.archimedean_copula import ArchimedeanCopula
+from copul.families.archimedean.nelsen1 import PiOverSigmaMinusPi
 from copul.sympy_wrapper import SymPyFunctionWrapper
 
 
-class Nelsen8(ArchimedeanCopula):
+class Nelsen19(ArchimedeanCopula):
     ac = ArchimedeanCopula
-    _inv_generator = (1 - ac.t) / (1 + (ac.theta - 1) * ac.t)
-    theta_interval = sympy.Interval(1, np.inf, left_open=False, right_open=True)
+    theta = sympy.symbols("theta", nonnegative=True)
+    theta_interval = sympy.Interval(0, np.inf, left_open=False, right_open=True)
+
+    def __call__(self, **kwargs):
+        if "theta" in kwargs and kwargs["theta"] == 0:
+            del kwargs["theta"]
+            return PiOverSigmaMinusPi()(**kwargs)
+        return super().__call__(**kwargs)
+
+    @property
+    def is_absolutely_continuous(self) -> bool:
+        return True
+
+    @property
+    def _generator(self):
+        return sympy.exp(self.theta / self.t) - sympy.exp(self.theta)
+
+    @property
+    def inv_generator(self):
+        gen = self.theta / sympy.log(self.y + sympy.exp(self.theta))
+        return SymPyFunctionWrapper(gen)
 
     @property
     def cdf(self):
-        num = self.theta**2*self.u*self.v - (1-self.u)*(1-self.v)
-        den = self.theta**2 - (self.theta - 1)**2*(1-self.u)*(1-self.v)
-        return SymPyFunctionWrapper(sympy.Max(num/den, 0))
+        cdf = self.theta / sympy.log(
+            -sympy.exp(self.theta) + sympy.exp(self.theta / self.u) + sympy.exp(self.theta / self.v)
+        )
+        return SymPyFunctionWrapper(cdf)
```

### Comparing `copul-0.0.4/copul/families/extreme_value/extreme_value_copula.py` & `copul-0.0.5/copul/families/extreme_value/extreme_value_copula.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,140 +1,187 @@
-import itertools
+import warnings
+from contextlib import contextmanager
 
 import numpy as np
 import scipy
 import sympy
-from sympy import log, Subs, Derivative
+from sympy import Derivative, Subs, log
 
+from copul.families.abstract_copula import AbstractCopula
+from copul.sympy_wrapper import SymPyFunctionWrapper
 
-class ExtremeValueCopula:
+
+class ExtremeValueCopula(AbstractCopula):
     _t_min = 0
     _t_max = 1
     t = sympy.symbols("t", positive=True)
     pickand = sympy.Function("A")(t)
     intervals = None
 
-    def get_free_symbols(self):
-        return self.pickand.free_symbols - {self.t}
+    def deriv_pickand_at_0(self):
+        diff = sympy.simplify(sympy.diff(self.pickand, self.t))
+        diff_at_0 = sympy.limit(diff, self.t, 0)
+        return diff_at_0
 
     def sample_parameters(self, n=1):
-        return {k: list(np.random.uniform(max(-10, v.start), min(10, v.end), n)) for k, v in self.intervals.items()}
+        return {
+            k: list(np.random.uniform(max(-10, v.start), min(10, v.end), n))
+            for k, v in self.intervals.items()
+        }
 
     @property
     def cdf(self):
-        """ Cumulative distribution function of the copula """
-        u, v = sympy.symbols("u v")
-        cop = (u * v) ** self.pickand.subs(self.t, sympy.ln(v) / sympy.ln(u * v))
+        """Cumulative distribution function of the copula"""
+        cop = (self.u * self.v) ** self.pickand.subs(
+            self.t, sympy.ln(self.v) / sympy.ln(self.u * self.v)
+        )
         cop = self._get_simplified_solution(cop)
-        return cop
-
-    def compute_pdf(self):
-        cdf = self.cdf
-        pdf = sympy.diff(sympy.diff(cdf, "u"), "v")
-        pdf = self._get_simplified_solution(pdf)
-        return pdf.doit()
+        return SymPyFunctionWrapper(cop)
 
     @property
     def pdf(self):
-        """ Probability density function of the copula """
+        """Probability density function of the copula"""
         _xi_1, u, v = sympy.symbols("_xi_1 u v")
-        pdf = (u * v) ** self.pickand.subs(self.t, log(v) / log(u * v)) * (-(
-                (log(v) - log(u * v)) * Subs(Derivative(self.pickand.subs(self.t, _xi_1), _xi_1), _xi_1,
-                                             log(v) / log(u * v)) - self.pickand.subs(self.t, log(v) / log(u * v)) *
-                log(u * v)) * (self.pickand.subs(self.t, log(v) / log(u * v)) * log(u * v) - log(v) *
-                               Subs(Derivative(self.pickand.subs(self.t, _xi_1), _xi_1), _xi_1, log(v) / log(u * v))) *
-                                                                           log(u * v) + (log(v) - log(u * v)) * log(
-                v) * Subs(Derivative(self.pickand.subs(self.t, _xi_1), (_xi_1, 2)), _xi_1, log(v) / log(u * v))) / (
-                      u * v * log(u * v) ** 3)
+        pickand = self.pickand
+        t = self.t
+        pdf = (
+            (u * v) ** pickand.subs(t, log(v) / log(u * v))
+            * (
+                -(
+                    (log(v) - log(u * v))
+                    * Subs(Derivative(pickand.subs(t, _xi_1), _xi_1), _xi_1, log(v) / log(u * v))
+                    - pickand.subs(t, log(v) / log(u * v)) * log(u * v)
+                )
+                * (
+                    pickand.subs(t, log(v) / log(u * v)) * log(u * v)
+                    - log(v)
+                    * Subs(Derivative(pickand.subs(t, _xi_1), _xi_1), _xi_1, log(v) / log(u * v))
+                )
+                * log(u * v)
+                + (log(v) - log(u * v))
+                * log(v)
+                * Subs(Derivative(pickand.subs(t, _xi_1), (_xi_1, 2)), _xi_1, log(v) / log(u * v))
+            )
+            / (u * v * log(u * v) ** 3)
+        )
         return self._get_simplified_solution(pdf)
 
-    def is_mtp2(self):
-        pdf = self.pdf
-        log_pdf = sympy.simplify(sympy.ln(pdf))
-        x1, x2, y1, y2 = sympy.symbols("x1 x2 y1 y2")
-        log_pdf_deriv = sympy.diff(sympy.simplify(sympy.diff(log_pdf, "u")), "v")
-        simplified_log_pdf_deriv = sympy.simplify(log_pdf_deriv)
-        parameters = list(self.intervals.keys())
-        mtp2_lambda = sympy.lambdify([x1, x2, y1, y2] + parameters, simplified_log_pdf_deriv,
-                                     modules=['scipy', 'numpy', 'sympy'])
-        solution, x0 = self.minimize_func_empirically(mtp2_lambda, parameters)
-        mtp2_lambda(0.5, 0.5, 0.5, 0.5, 0.5, 0.5)
-        return solution, x0
-
-    @property
-    def spearmans_rho(self):
-        integrand = (self.pickand + 1) ** (-2)  # nelsen 5.15
-        integral = 12 * sympy.integrate(integrand, (self.t, 0, 1)) - 3
-        return sympy.simplify(integral)
-
-    @property
-    def kendalls_tau(self):  # nelsen 5.15
-        diff_pickand = sympy.simplify(sympy.diff(sympy.simplify(sympy.diff(self.pickand, self.t)), self.t))
-        integrand = self.t * (1 - self.t) / self.pickand * diff_pickand
-        integral = sympy.integrate(integrand, (self.t, 0, 1))
-        return sympy.simplify(integral)
+    def rho(self):
+        integrand = self._rho_int_1()  # nelsen 5.15
+        print("integrand: ", integrand)
+        print("integrand latex: ", sympy.latex(integrand))
+        rho = self._rho()
+        print("rho: ", rho)
+        print("rho latex: ", sympy.latex(rho))
+        return rho
+
+    def _rho_int_1(self):
+        return sympy.simplify((self.pickand + 1) ** (-2))
+
+    def _rho(self):
+        return sympy.simplify(12 * sympy.integrate(self._rho_int_1(), (self.t, 0, 1)) - 3)
+
+    def tau(self):  # nelsen 5.15
+        t = self.t
+        diff2_pickand = sympy.diff(self.pickand, t, 2)
+        integrand = sympy.simplify(t * (1 - t) / self.pickand * diff2_pickand)
+        print("integrand: ", integrand)
+        print("integrand latex: ", sympy.latex(integrand))
+        integral = sympy.integrate(integrand, (t, 0, 1))
+        tau = sympy.simplify(integral)
+        print("tau: ", tau)
+        print("tau latex: ", sympy.latex(tau))
+        return tau
 
     def minimize_func(self, sympy_func):
         parameters = self.intervals.keys()
 
         def func(x):
             x1_float, x2_float, y1_float, y2_float = x[:4]
             par_dict = dict(zip(parameters, x[4:]))
-            return sympy_func.subs({"x1": x1_float, "x2": x2_float, "y1": y1_float, "y2": y2_float} | par_dict).evalf()
+            return sympy_func.subs(
+                {"x1": x1_float, "x2": x2_float, "y1": y1_float, "y2": y2_float} | par_dict
+            ).evalf()
 
         b = [0, 1]
         bounds = [b, b, b, b]
-        parameter_bounds = [[self.intervals[par].inf, self.intervals[par].sup] for par in parameters]
+        parameter_bounds = [
+            [self.intervals[par].inf, self.intervals[par].sup] for par in parameters
+        ]
         bounds += parameter_bounds
-        start_parameters = [min(self.intervals[par].inf + 0.5, self.intervals[par].sup) for par in parameters]
+        start_parameters = [
+            min(self.intervals[par].inf + 0.5, self.intervals[par].sup) for par in parameters
+        ]
         i = 0
         x0 = None
         while i < 4:
             x0 = np.concatenate((np.random.rand(4), start_parameters))
             try:
                 solution = scipy.optimize.minimize(func, x0, bounds=bounds)
                 return solution, x0
             except TypeError:
                 i += 1
                 print(i)
                 continue
         return None, x0
 
-    @staticmethod
-    def _get_function_graph(func, par):
-        return sympy.plotting.plot(func, show=False, xlim=(0, 1), ylim=(0, 1), label=par, legend=True,
-                                   axis_center=(0, 0))
-
-    def plot_pickand(self, sub_dict):
-        if sub_dict is None:
-            sub_dict = {}
-        for key, value in sub_dict.items():
+    def _get_function_graph(self, func, par):
+        params = {param: getattr(self, param) for param in [*self.intervals]}
+        defined_params = {k: v for k, v in params.items() if not isinstance(v, sympy.Symbol)}
+        dict_str = ", ".join(f"\\{key}={value}" for key, value in defined_params.items())
+        x_label = f"$t$ (with ${dict_str}$)"
+        par_str = ", ".join(f"\\{key}={value}" for key, value in par.items())
+        return sympy.plotting.plot(
+            func,
+            show=False,
+            xlim=(0, 1),
+            ylim=(0, 1),
+            label=f"${par_str}$",
+            legend=True,
+            axis_center=(0, 0),
+            xlabel=x_label,
+            ylabel="$A(t)$",
+            title=f"{self.__class__.__name__}",
+        )
+
+    def plot_pickand(self, subs):
+        if subs is None:
+            subs = {}
+        subs = {getattr(self, k) if isinstance(k, str) else k: v for k, v in subs.items()}
+        for key, value in subs.items():
             if not isinstance(value, list):
-                sub_dict[key] = [value]
-        keys_to_cross_product = [key for key, value in sub_dict.items() if isinstance(value, (str, list))]
-        values_to_cross_product = [value if isinstance(value, list) else [value] for value in sub_dict.values()]
-        cross_product = list(itertools.product(*values_to_cross_product))
-        plot_vals = [dict(zip(keys_to_cross_product, cross_product[i])) for i in range(len(cross_product))]
-
+                subs[key] = [value]
+        plot_vals = self._mix_params(subs)
         plots = []
         for plot_val in plot_vals:
             pickand = self.pickand.subs(plot_val)
             p = self._get_function_graph(pickand, plot_val)
             plots.append(p)
         p1 = plots[0]
         [p1.extend(p) for p in plots[1:]]
-        p1.show()
+
+        @contextmanager
+        def suppress_warnings():
+            warnings.filterwarnings("ignore")
+            yield
+            warnings.filterwarnings("default")
+
+        with suppress_warnings():
+            p1.show()
         return None
 
     def minimize_func_empirically(self, func, parameters):
-        b = [0.01, .99]
+        b = [0.01, 0.99]
         bounds = [b, b, b, b]
-        parameter_bounds = [[max(self.intervals[par].inf, -10), min(self.intervals[par].sup, 10)] for par in parameters]
+        parameter_bounds = [
+            [max(self.intervals[par].inf, -10), min(self.intervals[par].sup, 10)]
+            for par in parameters
+        ]
         bounds += parameter_bounds
-        linspaces = [np.linspace(start=float(bound[0]), stop=float(bound[1]), num=5) for bound in bounds]
+        linspaces = [np.linspace(start=float(b[0]), stop=float(b[1]), num=5) for b in bounds]
         meshgrid = np.meshgrid(*linspaces)
         func_vals = func(*meshgrid)
         return min(func_vals)
 
     @staticmethod
     def _get_simplified_solution(sol):
         simplified_sol = sympy.simplify(sol)
```

### Comparing `copul-0.0.4/copul/families/extreme_value/joe.py` & `copul-0.0.5/copul/families/extreme_value/t_ev.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 import numpy as np
 import sympy
+from sympy import stats
 
 from copul.families.extreme_value.extreme_value_copula import ExtremeValueCopula
 
 
-class Joe(ExtremeValueCopula):
-    psi1, psi2, delta = sympy.symbols("psi1 psi2 delta")
-
-    def __init__(self):
-        self.pickand = 1 - ((self.psi1 * (1 - self.t)) ** (-self.delta) + (self.psi2 * self.t) ** (-self.delta)) ** (
-                -1 / self.delta)
-        self.intervals = {
-            self.psi1: sympy.Interval(0, 1, left_open=False, right_open=False),
-            self.psi2: sympy.Interval(0, 1, left_open=False, right_open=False),
-            self.delta: sympy.Interval(0, np.inf, left_open=True, right_open=True),
-        }
-
-
-if __name__ == '__main__':
-    copul = Joe()
-    sub_dict = {copul.delta: [0.1, 0.5, 1, 5, 100], copul.psi1: [0.2, 0.8], copul.psi2: 1}
-    copul.plot_pickand(sub_dict)
-    exit()
+# noinspection PyPep8Naming
+class tEV(ExtremeValueCopula):
+    @property
+    def is_symmetric(self) -> bool:
+        pass
+
+    rho = sympy.symbols("rho")
+    nu = sympy.symbols("nu", positive=True)
+    params = [nu, rho]
+    intervals = {
+        "nu": sympy.Interval(0, np.inf, left_open=True, right_open=True),
+        "rho": sympy.Interval(-1, 1, left_open=True, right_open=True),
+    }
+
+    @property
+    def is_absolutely_continuous(self) -> bool:
+        return True
+
+    @property
+    def pickand(self):
+        def z(t):
+            return (
+                (1 + self.nu) ** (1 / 2)
+                * ((t / (1 - t)) ** (1 / self.nu) - self.rho)
+                * (1 - self.rho**2) ** (-1 / 2)
+            )
+
+        return (1 - self.t) * stats.cdf(stats.StudentT("x", self.nu + 1))(
+            z(1 - self.t)
+        ) + self.t * stats.cdf(stats.StudentT("x", self.nu + 1))(z(self.t))
```

### Comparing `copul-0.0.4/copul/families/extreme_value/t_ev.py` & `copul-0.0.5/copul/families/archimedean/nelsen12.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,39 @@
 import numpy as np
 import sympy
-from sympy import stats
 
-from copul.families.extreme_value.extreme_value_copula import ExtremeValueCopula
+from copul.families.archimedean.archimedean_copula import ArchimedeanCopula
+from copul.sympy_wrapper import SymPyFunctionWrapper
 
 
-# noinspection PyPep8Naming
-class tEV(ExtremeValueCopula):
-    nu, rho = sympy.symbols("nu rho")
-
-    def __init__(self):
-        def z(t):
-            return (1 + self.nu) ** (1 / 2) * ((t / (1 - t)) ** (1 / self.nu) - self.rho) * (1 - self.rho ** 2) ** (
-                    -1 / 2)
-
-        self.pickand = (1 - self.t) * stats.cdf(stats.StudentT("x", self.nu + 1))(z(1 - self.t)) + self.t * stats.cdf(
-            stats.StudentT("x", self.nu + 1))(z(self.t))
-        self.intervals = {
-            self.nu: sympy.Interval(0, np.inf, left_open=True, right_open=True),
-            self.rho: sympy.Interval(-1, 1, left_open=True, right_open=True),
-        }
+class Nelsen12(ArchimedeanCopula):
+    ac = ArchimedeanCopula
+    theta = sympy.symbols("theta", positive=True)
+    theta_interval = sympy.Interval(1, np.inf, left_open=False, right_open=True)
+
+    @property
+    def is_absolutely_continuous(self) -> bool:
+        return True
+
+    @property
+    def _generator(self):
+        return (1 / self.t - 1) ** self.theta
+
+    @property
+    def inv_generator(self):
+        gen = 1 / (self.y ** (1 / self.theta) + 1)
+        return SymPyFunctionWrapper(gen)
+
+    @property
+    def cdf(self):
+        cdf = (
+            1
+            + ((self.u ** (-1) - 1) ** self.theta + (self.v ** (-1) - 1) ** self.theta)
+            ** (1 / self.theta)
+        ) ** (-1)
+        return SymPyFunctionWrapper(cdf)
+
+    def lambda_L(self):
+        return 2 ** (-1 / self.theta)
+
+    def lambda_U(self):
+        return 2 - 2 ** (1 / self.theta)
```

### Comparing `copul-0.0.4/copul/sympy_wrapper.py` & `copul-0.0.5/copul/sympy_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 import sympy
 
 
 class SymPyFunctionWrapper:
     def __init__(self, sympy_func):
-        allowed = (
-            sympy.Pow,
-            sympy.Mul,
-            sympy.Add,
-            sympy.Max,
-            sympy.log,
-            sympy.exp,
-            sympy.core.numbers.Zero,
-        )
-        assert isinstance(
-            sympy_func, allowed
-        ), f"Function must be from sympy, but is {type(sympy_func)}"
+        if isinstance(sympy_func, SymPyFunctionWrapper):
+            sympy_func = sympy_func.func
+        type_ = type(sympy_func)
+        assert isinstance(sympy_func, sympy.Expr), f"Function must be from sympy, but is {type_}"
         self._func = sympy_func
 
     def __str__(self):
         return str(self._func)
 
     def __repr__(self):
         return repr(self._func)
@@ -39,7 +31,10 @@
     def subs(self, *args, **kwargs):
         self._func = self._func.subs(*args, **kwargs)
         return self
 
     def diff(self, *args, **kwargs):
         self._func = self._func.diff(*args, **kwargs)
         return self
+
+    def to_latex(self):
+        return sympy.latex(self._func)
```

