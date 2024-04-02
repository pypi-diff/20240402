# Comparing `tmp/sed_scores_eval-0.0.1.tar.gz` & `tmp/sed_scores_eval-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sed_scores_eval-0.0.1.tar", last modified: Fri Mar 29 18:32:04 2024, max compression
+gzip compressed data, was "sed_scores_eval-0.0.2.tar", last modified: Tue Apr  2 18:32:56 2024, max compression
```

## Comparing `sed_scores_eval-0.0.1.tar` & `sed_scores_eval-0.0.2.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-03-29 18:32:04.236949 sed_scores_eval-0.0.1/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     1121 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/LICENSE
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     9774 2024-03-29 18:32:04.236608 sed_scores_eval-0.0.1/PKG-INFO
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     8505 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/README.md
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-03-29 18:32:04.216485 sed_scores_eval-0.0.1/sed_scores_eval/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      269 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/__init__.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-03-29 18:32:04.227128 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)        0 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/__init__.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     1967 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/bootstrap.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2296 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/curves.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)  1154142 2024-02-14 14:08:05.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/cy_detection.cpp
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)  1360836 2024-03-29 18:32:04.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/cy_medfilt.cpp
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     7334 2024-01-29 21:25:27.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/detection.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    11762 2024-01-29 18:55:17.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/error_rate.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     7565 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/ground_truth.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    21436 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/io.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2337 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/postprocessing.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    17659 2024-01-29 20:53:02.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/precision_recall.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     4356 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/roc.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     6745 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/scores.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    14955 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/base_modules/statistics.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-03-29 18:32:04.228923 sed_scores_eval-0.0.1/sed_scores_eval/clip_based/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      325 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/clip_based/__init__.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     7376 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/clip_based/error_rate.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     4776 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/clip_based/intermediate_statistics.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    11155 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/clip_based/precision_recall.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2861 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/clip_based/reference.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     3730 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/clip_based/roc.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-03-29 18:32:04.230631 sed_scores_eval-0.0.1/sed_scores_eval/collar_based/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      308 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/collar_based/__init__.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    10540 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/collar_based/error_rate.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    13375 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/collar_based/intermediate_statistics.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    17234 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/collar_based/precision_recall.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     3732 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/collar_based/reference.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-03-29 18:32:04.232968 sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      669 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/__init__.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     9273 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/error_rate.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    15703 2024-01-29 21:23:42.000000 sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/intermediate_statistics.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    22604 2024-03-29 18:31:03.000000 sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/pipsds.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    12320 2024-01-16 14:39:25.000000 sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/precision_recall.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    19061 2024-03-29 18:31:03.000000 sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/psds.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    11139 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/reference.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-03-29 18:32:04.234551 sed_scores_eval-0.0.1/sed_scores_eval/segment_based/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      325 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/segment_based/__init__.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     9447 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/segment_based/error_rate.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     7549 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/segment_based/intermediate_statistics.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    14560 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/segment_based/precision_recall.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     3329 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/segment_based/reference.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     5111 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/segment_based/roc.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-03-29 18:32:04.235801 sed_scores_eval-0.0.1/sed_scores_eval/utils/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      115 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/utils/__init__.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2738 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/utils/array_ops.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     3658 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/utils/nested.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     1230 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/utils/parallel.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      751 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/utils/test.py
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2299 2024-01-08 21:23:39.000000 sed_scores_eval-0.0.1/sed_scores_eval/utils/visualization.py
-drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-03-29 18:32:04.236104 sed_scores_eval-0.0.1/sed_scores_eval.egg-info/
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     9774 2024-03-29 18:32:04.000000 sed_scores_eval-0.0.1/sed_scores_eval.egg-info/PKG-INFO
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2151 2024-03-29 18:32:04.000000 sed_scores_eval-0.0.1/sed_scores_eval.egg-info/SOURCES.txt
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)        1 2024-03-29 18:32:04.000000 sed_scores_eval-0.0.1/sed_scores_eval.egg-info/dependency_links.txt
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      121 2024-03-29 18:32:04.000000 sed_scores_eval-0.0.1/sed_scores_eval.egg-info/requires.txt
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)       16 2024-03-29 18:32:04.000000 sed_scores_eval-0.0.1/sed_scores_eval.egg-info/top_level.txt
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)       38 2024-03-29 18:32:04.236995 sed_scores_eval-0.0.1/setup.cfg
--rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     1999 2024-03-29 18:31:05.000000 sed_scores_eval-0.0.1/setup.py
+drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.523325 sed_scores_eval-0.0.2/
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     1121 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/LICENSE
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     9774 2024-04-02 18:32:56.523005 sed_scores_eval-0.0.2/PKG-INFO
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     8505 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/README.md
+drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.510681 sed_scores_eval-0.0.2/sed_scores_eval/
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      269 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/__init__.py
+drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.516366 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/__init__.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     1967 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/bootstrap.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2296 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/curves.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)  1153428 2024-04-02 18:32:55.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_detection.cpp
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     4484 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_detection.pyx
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)  1360122 2024-04-02 18:32:56.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_medfilt.cpp
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    13611 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_medfilt.pyx
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     7334 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/detection.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    11762 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/error_rate.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     7565 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/ground_truth.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    21436 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/io.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2337 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/postprocessing.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    17659 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/precision_recall.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     4356 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/roc.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     6745 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/scores.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    14955 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/base_modules/statistics.py
+drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.517447 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      325 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/__init__.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     7376 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/error_rate.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     4776 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/intermediate_statistics.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    11155 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/precision_recall.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2861 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/reference.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     3730 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/clip_based/roc.py
+drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.518403 sed_scores_eval-0.0.2/sed_scores_eval/collar_based/
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      308 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/collar_based/__init__.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    10540 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/collar_based/error_rate.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    13375 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/collar_based/intermediate_statistics.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    17234 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/collar_based/precision_recall.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     3732 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/collar_based/reference.py
+drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.519899 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      669 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/__init__.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     9273 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/error_rate.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    15703 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/intermediate_statistics.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    22604 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/pipsds.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    12320 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/precision_recall.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    19061 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/psds.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    11139 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/reference.py
+drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.521118 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      325 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/__init__.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     9447 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/error_rate.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     7549 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/intermediate_statistics.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)    14560 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/precision_recall.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     3329 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/reference.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     5111 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/segment_based/roc.py
+drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.522262 sed_scores_eval-0.0.2/sed_scores_eval/utils/
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      115 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/utils/__init__.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2738 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/utils/array_ops.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     3658 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/utils/nested.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     1230 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/utils/parallel.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      751 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/utils/test.py
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2299 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/sed_scores_eval/utils/visualization.py
+drwxr-xr-x   0 ebbers   (57088704) AD\merl    (500)        0 2024-04-02 18:32:56.522547 sed_scores_eval-0.0.2/sed_scores_eval.egg-info/
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     9774 2024-04-02 18:32:56.000000 sed_scores_eval-0.0.2/sed_scores_eval.egg-info/PKG-INFO
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2241 2024-04-02 18:32:56.000000 sed_scores_eval-0.0.2/sed_scores_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)        1 2024-04-02 18:32:56.000000 sed_scores_eval-0.0.2/sed_scores_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)      121 2024-04-02 18:32:56.000000 sed_scores_eval-0.0.2/sed_scores_eval.egg-info/requires.txt
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)       16 2024-04-02 18:32:56.000000 sed_scores_eval-0.0.2/sed_scores_eval.egg-info/top_level.txt
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)       38 2024-04-02 18:32:56.523377 sed_scores_eval-0.0.2/setup.cfg
+-rw-r--r--   0 ebbers   (57088704) AD\merl    (500)     2091 2024-04-02 18:32:33.000000 sed_scores_eval-0.0.2/setup.py
```

### Comparing `sed_scores_eval-0.0.1/LICENSE` & `sed_scores_eval-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/PKG-INFO` & `sed_scores_eval-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sed_scores_eval
-Version: 0.0.1
+Version: 0.0.2
 Summary: (Threshold-Independent) Evaluation of Sound Event Detection Scores
 Home-page: https://github.com/fgnt/sed_scores_eval
 Author: Department of Communications Engineering, Paderborn University
 Author-email: sek@nt.upb.de
 License: MIT
 Keywords: sound recognition evaluation from classification scores
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sed_scores_eval-0.0.1/README.md` & `sed_scores_eval-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/base_modules/bootstrap.py` & `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/bootstrap.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/base_modules/curves.py` & `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/curves.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/base_modules/cy_detection.cpp` & `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_detection.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1655,195 +1655,195 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":759
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":766
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1876,42 +1876,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":770
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18027,261 +18027,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18290,29 +18290,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18323,15 +18323,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18340,29 +18340,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18373,15 +18373,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18390,29 +18390,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18423,15 +18423,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18440,29 +18440,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18473,15 +18473,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18490,29 +18490,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18523,209 +18523,209 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18741,15 +18741,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18757,68 +18757,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 984, __pyx_L3_error)
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 985, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18826,15 +18826,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18849,15 +18849,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18873,15 +18873,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18889,68 +18889,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 990, __pyx_L3_error)
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 991, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18958,15 +18958,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18981,15 +18981,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19005,15 +19005,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19021,68 +19021,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 996, __pyx_L3_error)
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 997, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19090,15 +19090,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19113,170 +19113,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -21697,26 +21697,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 992, __pyx_L1_error)
```

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/base_modules/cy_medfilt.cpp` & `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/cy_medfilt.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1659,195 +1659,195 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":759
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":766
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1880,42 +1880,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":770
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18902,261 +18902,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19165,29 +19165,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19198,15 +19198,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19215,29 +19215,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19248,15 +19248,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19265,29 +19265,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19298,15 +19298,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19315,29 +19315,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19348,15 +19348,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19365,29 +19365,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19398,209 +19398,209 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19616,15 +19616,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19632,68 +19632,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 984, __pyx_L3_error)
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 985, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19701,15 +19701,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19724,15 +19724,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19748,15 +19748,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19764,68 +19764,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 990, __pyx_L3_error)
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 991, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19833,15 +19833,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19856,15 +19856,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19880,15 +19880,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19896,68 +19896,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 996, __pyx_L3_error)
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 997, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19965,15 +19965,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19988,170 +19988,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -25592,26 +25592,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../Software/anaconda3/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 992, __pyx_L1_error)
```

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/base_modules/detection.py` & `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/detection.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/base_modules/error_rate.py` & `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/error_rate.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/base_modules/ground_truth.py` & `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/ground_truth.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/base_modules/io.py` & `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/io.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/base_modules/postprocessing.py` & `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/postprocessing.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/base_modules/precision_recall.py` & `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/precision_recall.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/base_modules/roc.py` & `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/roc.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/base_modules/scores.py` & `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/scores.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/base_modules/statistics.py` & `sed_scores_eval-0.0.2/sed_scores_eval/base_modules/statistics.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/clip_based/error_rate.py` & `sed_scores_eval-0.0.2/sed_scores_eval/clip_based/error_rate.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/clip_based/intermediate_statistics.py` & `sed_scores_eval-0.0.2/sed_scores_eval/clip_based/intermediate_statistics.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/clip_based/precision_recall.py` & `sed_scores_eval-0.0.2/sed_scores_eval/clip_based/precision_recall.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/clip_based/reference.py` & `sed_scores_eval-0.0.2/sed_scores_eval/clip_based/reference.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/clip_based/roc.py` & `sed_scores_eval-0.0.2/sed_scores_eval/clip_based/roc.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/collar_based/error_rate.py` & `sed_scores_eval-0.0.2/sed_scores_eval/collar_based/error_rate.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/collar_based/intermediate_statistics.py` & `sed_scores_eval-0.0.2/sed_scores_eval/collar_based/intermediate_statistics.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/collar_based/precision_recall.py` & `sed_scores_eval-0.0.2/sed_scores_eval/collar_based/precision_recall.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/collar_based/reference.py` & `sed_scores_eval-0.0.2/sed_scores_eval/collar_based/reference.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/__init__.py` & `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/__init__.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/error_rate.py` & `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/error_rate.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/intermediate_statistics.py` & `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/intermediate_statistics.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/pipsds.py` & `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/pipsds.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/precision_recall.py` & `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/precision_recall.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/psds.py` & `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/psds.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/intersection_based/reference.py` & `sed_scores_eval-0.0.2/sed_scores_eval/intersection_based/reference.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/segment_based/error_rate.py` & `sed_scores_eval-0.0.2/sed_scores_eval/segment_based/error_rate.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/segment_based/intermediate_statistics.py` & `sed_scores_eval-0.0.2/sed_scores_eval/segment_based/intermediate_statistics.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/segment_based/precision_recall.py` & `sed_scores_eval-0.0.2/sed_scores_eval/segment_based/precision_recall.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/segment_based/reference.py` & `sed_scores_eval-0.0.2/sed_scores_eval/segment_based/reference.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/segment_based/roc.py` & `sed_scores_eval-0.0.2/sed_scores_eval/segment_based/roc.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/utils/array_ops.py` & `sed_scores_eval-0.0.2/sed_scores_eval/utils/array_ops.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/utils/nested.py` & `sed_scores_eval-0.0.2/sed_scores_eval/utils/nested.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/utils/parallel.py` & `sed_scores_eval-0.0.2/sed_scores_eval/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/utils/test.py` & `sed_scores_eval-0.0.2/sed_scores_eval/utils/test.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval/utils/visualization.py` & `sed_scores_eval-0.0.2/sed_scores_eval/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval.egg-info/PKG-INFO` & `sed_scores_eval-0.0.2/sed_scores_eval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sed-scores-eval
-Version: 0.0.1
+Name: sed_scores_eval
+Version: 0.0.2
 Summary: (Threshold-Independent) Evaluation of Sound Event Detection Scores
 Home-page: https://github.com/fgnt/sed_scores_eval
 Author: Department of Communications Engineering, Paderborn University
 Author-email: sek@nt.upb.de
 License: MIT
 Keywords: sound recognition evaluation from classification scores
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sed_scores_eval-0.0.1/sed_scores_eval.egg-info/SOURCES.txt` & `sed_scores_eval-0.0.2/sed_scores_eval.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 sed_scores_eval.egg-info/dependency_links.txt
 sed_scores_eval.egg-info/requires.txt
 sed_scores_eval.egg-info/top_level.txt
 sed_scores_eval/base_modules/__init__.py
 sed_scores_eval/base_modules/bootstrap.py
 sed_scores_eval/base_modules/curves.py
 sed_scores_eval/base_modules/cy_detection.cpp
+sed_scores_eval/base_modules/cy_detection.pyx
 sed_scores_eval/base_modules/cy_medfilt.cpp
+sed_scores_eval/base_modules/cy_medfilt.pyx
 sed_scores_eval/base_modules/detection.py
 sed_scores_eval/base_modules/error_rate.py
 sed_scores_eval/base_modules/ground_truth.py
 sed_scores_eval/base_modules/io.py
 sed_scores_eval/base_modules/postprocessing.py
 sed_scores_eval/base_modules/precision_recall.py
 sed_scores_eval/base_modules/roc.py
```

### Comparing `sed_scores_eval-0.0.1/setup.py` & `sed_scores_eval-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 st.setup(
     name='sed_scores_eval',
-    version='0.0.1',
+    version='0.0.2',
     description='(Threshold-Independent) Evaluation of Sound Event Detection Scores',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/fgnt/sed_scores_eval',
     author='Department of Communications Engineering, Paderborn University',
     author_email='sek@nt.upb.de',
     license='MIT',
@@ -58,9 +58,10 @@
         'Cython',
     ],
     extras_require={
         'dev': ['check-manifest'],
         'test': ['coverage', 'jupyter', 'matplotlib'],
     },
     ext_modules=ext_modules,
+    package_data={'sed_scores_eval': ['**/*.pyx']},  # https://stackoverflow.com/a/60751886
     include_dirs=[np.get_include()],
 )
```

