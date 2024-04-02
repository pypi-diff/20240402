# Comparing `tmp/MRCpy-2.1.7.tar.gz` & `tmp/MRCpy-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MRCpy-2.1.7.tar", last modified: Wed Feb 14 10:00:38 2024, max compression
+gzip compressed data, was "MRCpy-2.1.8.tar", last modified: Tue Apr  2 10:28:07 2024, max compression
```

## Comparing `MRCpy-2.1.7.tar` & `MRCpy-2.1.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-02-14 10:00:38.640655 MRCpy-2.1.7/
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-02-14 10:00:38.338837 MRCpy-2.1.7/MRCpy/
--rw-r--r--   0 kbondugula   (503) staff       (20)      245 2024-02-13 15:24:24.000000 MRCpy-2.1.7/MRCpy/__init__.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    27110 2024-01-26 13:03:50.000000 MRCpy-2.1.7/MRCpy/amrc.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    17242 2024-02-13 15:23:47.000000 MRCpy-2.1.7/MRCpy/base_mrc.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    28710 2024-02-13 15:23:38.000000 MRCpy-2.1.7/MRCpy/cmrc.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-02-14 10:00:38.344673 MRCpy-2.1.7/MRCpy/datasets/
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     1089 2024-01-28 20:51:11.000000 MRCpy-2.1.7/MRCpy/datasets/__init__.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-02-14 10:00:38.609831 MRCpy-2.1.7/MRCpy/datasets/data/
--rw-r--r--   0 kbondugula   (503) staff       (20)  7075696 2024-01-16 12:39:02.000000 MRCpy-2.1.7/MRCpy/datasets/data/comp-vs-sci_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20) 10629747 2024-01-16 12:39:02.000000 MRCpy-2.1.7/MRCpy/datasets/data/comp-vs-sci_Train.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  2002192 2024-01-16 12:39:02.000000 MRCpy-2.1.7/MRCpy/datasets/data/comp-vs-sci_shortTest.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  2002231 2024-01-16 12:39:02.000000 MRCpy-2.1.7/MRCpy/datasets/data/comp-vs-sci_shortTrain.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  6519380 2024-01-16 12:39:02.000000 MRCpy-2.1.7/MRCpy/datasets/data/comp-vs-talk_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  9787043 2024-01-16 12:39:02.000000 MRCpy-2.1.7/MRCpy/datasets/data/comp-vs-talk_Train.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    32719 2023-04-27 10:30:22.000000 MRCpy-2.1.7/MRCpy/datasets/data/credit.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    23118 2023-04-27 10:30:22.000000 MRCpy-2.1.7/MRCpy/datasets/data/diabetes.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    16851 2023-04-27 10:30:22.000000 MRCpy-2.1.7/MRCpy/datasets/data/ecoli.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    11293 2023-04-27 10:30:22.000000 MRCpy-2.1.7/MRCpy/datasets/data/glass.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3121 2023-04-27 10:30:22.000000 MRCpy-2.1.7/MRCpy/datasets/data/haberman.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    21189 2023-04-27 10:30:22.000000 MRCpy-2.1.7/MRCpy/datasets/data/indianLiverPatient.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     4789 2023-04-27 10:30:22.000000 MRCpy-2.1.7/MRCpy/datasets/data/iris.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)   732608 2023-04-27 10:30:22.000000 MRCpy-2.1.7/MRCpy/datasets/data/letter-recognition.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    13796 2023-04-27 10:30:22.000000 MRCpy-2.1.7/MRCpy/datasets/data/mammographic.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)   834087 2023-04-27 10:30:25.000000 MRCpy-2.1.7/MRCpy/datasets/data/optdigits.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  6344664 2024-01-16 12:39:02.000000 MRCpy-2.1.7/MRCpy/datasets/data/rec-vs-sci_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  9534428 2024-01-16 12:39:02.000000 MRCpy-2.1.7/MRCpy/datasets/data/rec-vs-sci_Train.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  5788382 2024-01-16 12:39:02.000000 MRCpy-2.1.7/MRCpy/datasets/data/rec-vs-talk_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  8691659 2024-01-16 12:39:02.000000 MRCpy-2.1.7/MRCpy/datasets/data/rec-vs-talk_Train.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    85710 2023-04-27 10:30:25.000000 MRCpy-2.1.7/MRCpy/datasets/data/redwine.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  5766341 2024-01-16 12:39:02.000000 MRCpy-2.1.7/MRCpy/datasets/data/sci-vs-talk_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  8659812 2024-01-16 12:39:02.000000 MRCpy-2.1.7/MRCpy/datasets/data/sci-vs-talk_Train.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)   370691 2023-04-27 10:30:25.000000 MRCpy-2.1.7/MRCpy/datasets/data/segment.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)   300394 2023-04-27 10:30:25.000000 MRCpy-2.1.7/MRCpy/datasets/data/usenet2.csv
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-02-14 10:00:38.627297 MRCpy-2.1.7/MRCpy/datasets/descr/
--rw-r--r--   0 kbondugula   (503) staff       (20)     2106 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/adult.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     1048 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/catsvsdogs_features_resnet18.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2218 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/credit.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     1102 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/diabetes.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3022 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/ecoli.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3666 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/glass.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     1535 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/haberman.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2582 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/indianLiverPatient.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2998 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/iris.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2734 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/letter-recognition.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3479 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/mammographic.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)      815 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/mnist_features_resnet18.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2388 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/optdigits.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3305 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/redwine.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     5250 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/satellite.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     2432 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/segment.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)       89 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/usenet2.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)        0 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/vehicle.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     1316 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/yearbook.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     1143 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/datasets/descr/yearbook_features_resnet18.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    52570 2024-02-09 13:02:57.000000 MRCpy-2.1.7/MRCpy/datasets/load.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    19745 2024-02-14 09:58:55.000000 MRCpy-2.1.7/MRCpy/dwgcs.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    28630 2024-02-13 15:34:58.000000 MRCpy-2.1.7/MRCpy/mrc.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-02-14 10:00:38.632121 MRCpy-2.1.7/MRCpy/phi/
--rw-r--r--   0 kbondugula   (503) staff       (20)      320 2024-02-09 17:31:55.000000 MRCpy-2.1.7/MRCpy/phi/__init__.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    10306 2024-01-30 14:36:53.000000 MRCpy-2.1.7/MRCpy/phi/base_phi.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     9282 2024-01-05 12:47:57.000000 MRCpy-2.1.7/MRCpy/phi/random_fourier_phi.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     9145 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/phi/random_relu_phi.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     6784 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/phi/threshold_phi.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-02-14 10:00:38.640073 MRCpy-2.1.7/MRCpy/solvers/
--rw-r--r--   0 kbondugula   (503) staff       (20)       82 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/solvers/__init__.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     1820 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/solvers/adam.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     9604 2024-02-12 18:48:43.000000 MRCpy-2.1.7/MRCpy/solvers/cg.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     2259 2024-02-12 18:46:27.000000 MRCpy-2.1.7/MRCpy/solvers/cvx.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    12950 2024-01-25 13:26:36.000000 MRCpy-2.1.7/MRCpy/solvers/nesterov.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     2833 2023-04-27 10:30:27.000000 MRCpy-2.1.7/MRCpy/solvers/sgd.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-02-14 10:00:38.342972 MRCpy-2.1.7/MRCpy.egg-info/
--rw-r--r--   0 kbondugula   (503) staff       (20)     4980 2024-02-14 10:00:38.000000 MRCpy-2.1.7/MRCpy.egg-info/PKG-INFO
--rw-r--r--   0 kbondugula   (503) staff       (20)     2312 2024-02-14 10:00:38.000000 MRCpy-2.1.7/MRCpy.egg-info/SOURCES.txt
--rw-r--r--   0 kbondugula   (503) staff       (20)        1 2024-02-14 10:00:38.000000 MRCpy-2.1.7/MRCpy.egg-info/dependency_links.txt
--rw-r--r--   0 kbondugula   (503) staff       (20)        1 2024-02-14 10:00:38.000000 MRCpy-2.1.7/MRCpy.egg-info/not-zip-safe
--rw-r--r--   0 kbondugula   (503) staff       (20)       64 2024-02-14 10:00:38.000000 MRCpy-2.1.7/MRCpy.egg-info/requires.txt
--rw-r--r--   0 kbondugula   (503) staff       (20)        6 2024-02-14 10:00:38.000000 MRCpy-2.1.7/MRCpy.egg-info/top_level.txt
--rw-r--r--   0 kbondugula   (503) staff       (20)     4980 2024-02-14 10:00:38.640870 MRCpy-2.1.7/PKG-INFO
--rw-r--r--   0 kbondugula   (503) staff       (20)     4316 2024-02-14 10:00:13.000000 MRCpy-2.1.7/README.md
--rw-r--r--   0 kbondugula   (503) staff       (20)      778 2024-02-14 09:43:37.000000 MRCpy-2.1.7/pyproject.toml
--rw-r--r--   0 kbondugula   (503) staff       (20)      160 2024-02-14 10:00:38.641574 MRCpy-2.1.7/setup.cfg
--rw-r--r--   0 kbondugula   (503) staff       (20)     2357 2024-02-14 09:37:45.000000 MRCpy-2.1.7/setup.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-02 10:28:07.858437 MRCpy-2.1.8/
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-02 10:28:07.456944 MRCpy-2.1.8/MRCpy/
+-rw-r--r--   0 kbondugula   (503) staff       (20)      245 2024-04-02 10:25:09.000000 MRCpy-2.1.8/MRCpy/__init__.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    27110 2024-01-26 13:03:50.000000 MRCpy-2.1.8/MRCpy/amrc.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    17242 2024-02-13 15:23:47.000000 MRCpy-2.1.8/MRCpy/base_mrc.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    28710 2024-02-28 16:31:33.000000 MRCpy-2.1.8/MRCpy/cmrc.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-02 10:28:07.462538 MRCpy-2.1.8/MRCpy/datasets/
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     1089 2024-01-28 20:51:11.000000 MRCpy-2.1.8/MRCpy/datasets/__init__.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-02 10:28:07.822728 MRCpy-2.1.8/MRCpy/datasets/data/
+-rw-r--r--   0 kbondugula   (503) staff       (20)  7075696 2024-01-16 12:39:02.000000 MRCpy-2.1.8/MRCpy/datasets/data/comp-vs-sci_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20) 10629747 2024-01-16 12:39:02.000000 MRCpy-2.1.8/MRCpy/datasets/data/comp-vs-sci_Train.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  2002192 2024-01-16 12:39:02.000000 MRCpy-2.1.8/MRCpy/datasets/data/comp-vs-sci_shortTest.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  2002231 2024-01-16 12:39:02.000000 MRCpy-2.1.8/MRCpy/datasets/data/comp-vs-sci_shortTrain.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  6519380 2024-01-16 12:39:02.000000 MRCpy-2.1.8/MRCpy/datasets/data/comp-vs-talk_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  9787043 2024-01-16 12:39:02.000000 MRCpy-2.1.8/MRCpy/datasets/data/comp-vs-talk_Train.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    32719 2023-04-27 10:30:22.000000 MRCpy-2.1.8/MRCpy/datasets/data/credit.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    23118 2023-04-27 10:30:22.000000 MRCpy-2.1.8/MRCpy/datasets/data/diabetes.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    16851 2023-04-27 10:30:22.000000 MRCpy-2.1.8/MRCpy/datasets/data/ecoli.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    11293 2023-04-27 10:30:22.000000 MRCpy-2.1.8/MRCpy/datasets/data/glass.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3121 2023-04-27 10:30:22.000000 MRCpy-2.1.8/MRCpy/datasets/data/haberman.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    21189 2023-04-27 10:30:22.000000 MRCpy-2.1.8/MRCpy/datasets/data/indianLiverPatient.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     4789 2023-04-27 10:30:22.000000 MRCpy-2.1.8/MRCpy/datasets/data/iris.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)   732608 2023-04-27 10:30:22.000000 MRCpy-2.1.8/MRCpy/datasets/data/letter-recognition.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    13796 2023-04-27 10:30:22.000000 MRCpy-2.1.8/MRCpy/datasets/data/mammographic.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)   834087 2023-04-27 10:30:25.000000 MRCpy-2.1.8/MRCpy/datasets/data/optdigits.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  6344664 2024-01-16 12:39:02.000000 MRCpy-2.1.8/MRCpy/datasets/data/rec-vs-sci_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  9534428 2024-01-16 12:39:02.000000 MRCpy-2.1.8/MRCpy/datasets/data/rec-vs-sci_Train.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  5788382 2024-01-16 12:39:02.000000 MRCpy-2.1.8/MRCpy/datasets/data/rec-vs-talk_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  8691659 2024-01-16 12:39:02.000000 MRCpy-2.1.8/MRCpy/datasets/data/rec-vs-talk_Train.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    85710 2023-04-27 10:30:25.000000 MRCpy-2.1.8/MRCpy/datasets/data/redwine.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  5766341 2024-01-16 12:39:02.000000 MRCpy-2.1.8/MRCpy/datasets/data/sci-vs-talk_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  8659812 2024-01-16 12:39:02.000000 MRCpy-2.1.8/MRCpy/datasets/data/sci-vs-talk_Train.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)   370691 2023-04-27 10:30:25.000000 MRCpy-2.1.8/MRCpy/datasets/data/segment.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)   300394 2023-04-27 10:30:25.000000 MRCpy-2.1.8/MRCpy/datasets/data/usenet2.csv
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-02 10:28:07.844130 MRCpy-2.1.8/MRCpy/datasets/descr/
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2106 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/adult.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     1048 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/catsvsdogs_features_resnet18.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2218 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/credit.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     1102 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/diabetes.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3022 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/ecoli.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3666 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/glass.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     1535 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/haberman.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2582 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/indianLiverPatient.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2998 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/iris.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2734 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/letter-recognition.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3479 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/mammographic.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)      815 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/mnist_features_resnet18.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2388 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/optdigits.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3305 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/redwine.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     5250 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/satellite.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2432 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/segment.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)       89 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/usenet2.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)        0 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/vehicle.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     1316 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/yearbook.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     1143 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/datasets/descr/yearbook_features_resnet18.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    52570 2024-02-09 13:02:57.000000 MRCpy-2.1.8/MRCpy/datasets/load.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    22785 2024-04-02 10:23:58.000000 MRCpy-2.1.8/MRCpy/dwgcs.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    28630 2024-02-13 15:34:58.000000 MRCpy-2.1.8/MRCpy/mrc.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-02 10:28:07.850334 MRCpy-2.1.8/MRCpy/phi/
+-rw-r--r--   0 kbondugula   (503) staff       (20)      320 2024-02-09 17:31:55.000000 MRCpy-2.1.8/MRCpy/phi/__init__.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    10306 2024-01-30 14:36:53.000000 MRCpy-2.1.8/MRCpy/phi/base_phi.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     9282 2024-01-05 12:47:57.000000 MRCpy-2.1.8/MRCpy/phi/random_fourier_phi.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     9145 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/phi/random_relu_phi.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     6784 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/phi/threshold_phi.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-02 10:28:07.857811 MRCpy-2.1.8/MRCpy/solvers/
+-rw-r--r--   0 kbondugula   (503) staff       (20)       82 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/solvers/__init__.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     1820 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/solvers/adam.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     9604 2024-02-12 18:48:43.000000 MRCpy-2.1.8/MRCpy/solvers/cg.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2259 2024-02-12 18:46:27.000000 MRCpy-2.1.8/MRCpy/solvers/cvx.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    12950 2024-01-25 13:26:36.000000 MRCpy-2.1.8/MRCpy/solvers/nesterov.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2833 2023-04-27 10:30:27.000000 MRCpy-2.1.8/MRCpy/solvers/sgd.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-02 10:28:07.460980 MRCpy-2.1.8/MRCpy.egg-info/
+-rw-r--r--   0 kbondugula   (503) staff       (20)     4980 2024-04-02 10:28:07.000000 MRCpy-2.1.8/MRCpy.egg-info/PKG-INFO
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2312 2024-04-02 10:28:07.000000 MRCpy-2.1.8/MRCpy.egg-info/SOURCES.txt
+-rw-r--r--   0 kbondugula   (503) staff       (20)        1 2024-04-02 10:28:07.000000 MRCpy-2.1.8/MRCpy.egg-info/dependency_links.txt
+-rw-r--r--   0 kbondugula   (503) staff       (20)        1 2024-04-02 10:28:07.000000 MRCpy-2.1.8/MRCpy.egg-info/not-zip-safe
+-rw-r--r--   0 kbondugula   (503) staff       (20)       64 2024-04-02 10:28:07.000000 MRCpy-2.1.8/MRCpy.egg-info/requires.txt
+-rw-r--r--   0 kbondugula   (503) staff       (20)        6 2024-04-02 10:28:07.000000 MRCpy-2.1.8/MRCpy.egg-info/top_level.txt
+-rw-r--r--   0 kbondugula   (503) staff       (20)     4980 2024-04-02 10:28:07.858695 MRCpy-2.1.8/PKG-INFO
+-rw-r--r--   0 kbondugula   (503) staff       (20)     4316 2024-02-14 10:00:13.000000 MRCpy-2.1.8/README.md
+-rw-r--r--   0 kbondugula   (503) staff       (20)      778 2024-04-02 10:25:34.000000 MRCpy-2.1.8/pyproject.toml
+-rw-r--r--   0 kbondugula   (503) staff       (20)      160 2024-04-02 10:28:07.859402 MRCpy-2.1.8/setup.cfg
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2357 2024-02-14 09:37:45.000000 MRCpy-2.1.8/setup.py
```

### Comparing `MRCpy-2.1.7/MRCpy/amrc.py` & `MRCpy-2.1.8/MRCpy/amrc.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/base_mrc.py` & `MRCpy-2.1.8/MRCpy/base_mrc.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/cmrc.py` & `MRCpy-2.1.8/MRCpy/cmrc.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/__init__.py` & `MRCpy-2.1.8/MRCpy/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/comp-vs-sci_Test.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/comp-vs-sci_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/comp-vs-sci_Train.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/comp-vs-sci_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/comp-vs-sci_shortTest.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/comp-vs-sci_shortTest.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/comp-vs-sci_shortTrain.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/comp-vs-sci_shortTrain.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/comp-vs-talk_Test.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/comp-vs-talk_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/comp-vs-talk_Train.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/comp-vs-talk_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/credit.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/credit.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/diabetes.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/diabetes.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/ecoli.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/ecoli.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/glass.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/glass.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/haberman.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/haberman.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/indianLiverPatient.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/indianLiverPatient.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/iris.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/iris.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/letter-recognition.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/letter-recognition.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/mammographic.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/mammographic.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/optdigits.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/optdigits.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/rec-vs-sci_Test.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/rec-vs-sci_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/rec-vs-sci_Train.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/rec-vs-sci_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/rec-vs-talk_Test.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/rec-vs-talk_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/rec-vs-talk_Train.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/rec-vs-talk_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/redwine.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/redwine.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/sci-vs-talk_Test.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/sci-vs-talk_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/sci-vs-talk_Train.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/sci-vs-talk_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/segment.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/segment.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/data/usenet2.csv` & `MRCpy-2.1.8/MRCpy/datasets/data/usenet2.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/adult.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/adult.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/catsvsdogs_features_resnet18.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/catsvsdogs_features_resnet18.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/credit.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/credit.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/diabetes.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/diabetes.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/ecoli.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/ecoli.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/glass.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/glass.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/haberman.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/haberman.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/indianLiverPatient.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/indianLiverPatient.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/iris.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/iris.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/letter-recognition.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/letter-recognition.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/mammographic.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/mammographic.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/mnist_features_resnet18.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/mnist_features_resnet18.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/optdigits.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/optdigits.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/redwine.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/redwine.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/satellite.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/satellite.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/segment.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/segment.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/yearbook.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/yearbook.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/descr/yearbook_features_resnet18.rst` & `MRCpy-2.1.8/MRCpy/datasets/descr/yearbook_features_resnet18.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/datasets/load.py` & `MRCpy-2.1.8/MRCpy/datasets/load.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/dwgcs.py` & `MRCpy-2.1.8/MRCpy/dwgcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,19 +52,19 @@
                     @InProceedings{SegMazLiu:23,
                     title =     {Double-Weighting for Covariate Shift Adaptation},
                     author =    {Segovia-Mart{\'i}n, Jos{\'e} I. 
                                 and Mazuelas, Santiago 
                                 and Liu, Anqi},
                     booktitle = {Proceedings of the 40th 
                                 International Conference on Machine Learning},
-                    pages = 	{30439--30457},
-                    year = 	    {2023},
-                    volume = 	{202},
-                    series = 	{Proceedings of Machine Learning Research},
-                    month = 	{23--29 Jul},
+                    pages =     {30439--30457},
+                    year =      {2023},
+                    volume =    {202},
+                    series =    {Proceedings of Machine Learning Research},
+                    month =     {23--29 Jul},
                     publisher = {PMLR},
                     }
     Parameters
     ----------
     loss : `str` {'0-1', 'log'}, default = '0-1'
         Type of loss function to use for the risk minimization. 0-1 loss
         quantifies the probability of classification error at a certain example
@@ -139,14 +139,27 @@
         The maximum number of iterations to use in case of
         ’grad’ or ’adam’ solver.
         The default value is
         100000 for ’grad’ solver and
         5000 for ’adam’ solver and 
         2000 for nesterov's gradient descent.   
 
+    weights_alpha : `array`, default = `None`
+        The weights alpha(x) associated to each testing instance.
+        Note that if just weights_beta is given, 
+        method will assume they are obtained 
+        based on robust approach, and fix beta(x) = 1.
+
+    weights_beta : `beta`, default = `None`
+        Weights beta(x) associated to each training sample.
+        Note that if just weights_beta is given, 
+        method will assume they are obtained 
+        based on reweighted approach, and fix alpha(x) = 1.
+    
+
     phi : `str` or `BasePhi` instance, default = 'linear'
         Type of feature mapping function to use for mapping the input data.
         The currenlty available feature mapping methods are
         'fourier', 'relu', and 'linear'.
         The users can also implement their own feature mapping object
         (should be a `BasePhi` instance) and pass it to this argument.
         Note that when using 'fourier' feature mapping,
@@ -187,33 +200,38 @@
                  sigma_ = None,
                  B = 1000,
                  solver='adam',
                  alpha=0.01,
                  stepsize='decay',
                  mini_batch_size=None,
                  max_iters=None,
+                 weights_beta=None,
+                 weights_alpha=None,
                  phi='linear',
                  **phi_kwargs):
         self.D = D
         self.sigma_ = sigma_
         self.B = B
+        self.beta_ = weights_beta
+        self.alpha_ = weights_alpha
         super().__init__(loss,
                          None,
                          deterministic,
                          random_state,
                          fit_intercept,
                          solver,
                          alpha,
                          stepsize,
                          mini_batch_size,
                          max_iters,
                          phi,
                          **phi_kwargs)
     
     def fit(self, xTr, yTr, xTe=None):
+        print("Running latest version")
         '''
         Fit the MRC model.
 
         Computes the parameters required for the minimax risk optimization
         and then calls the `minimax_risk` function to solve the optimization.
 
         Parameters
@@ -279,16 +297,35 @@
                                      **self.phi_kwargs)
         elif not isinstance(self.phi, BasePhi):
             raise ValueError('Unexpected feature mapping type ... ')
 
         # Fit the feature mappings
         self.phi.fit(xTr, yTr)
         
-        # Compute weights alpha and beta
-        self.DWKMM(xTr,xTe)
+        if self.alpha_ is None and self.beta_ is None:
+            # Compute weights alpha and beta
+            print("Computing both weights")
+            self.DWKMM(xTr,xTe)
+        elif self.alpha_ is None and self.beta_ is not None:
+            # Fix self.alpha_ == 1 
+            print("Fixing alpha weights equal 1")
+            self.alpha_ = np.ones((xTe.shape[0],1))
+            self.beta_ = np.reshape(self.beta_, (xTr.shape[0], 1))
+        elif self.alpha_ is not None and self.beta_ is None:
+            # Fix self.beta_ == 1 
+            print("Fixing beta weights equal 1")
+            self.beta_ = np.ones((xTr.shape[0],1))
+            self.alpha_ = np.reshape(self.alpha_, (xTe.shape[0], 1))
+        else:
+            # Make sure the size of alpha and beta are as desired
+            print("Weights were given")
+            self.beta_ = np.reshape(self.beta_, (xTr.shape[0], 1))
+            self.alpha_ = np.reshape(self.alpha_, (xTe.shape[0], 1))
+            
+        
 
         # Compute the expectation estimates
         tau_ = self.compute_tau(xTr, yTr)
         lambda_ = self.compute_lambda(xTe, tau_, n_classes)
 
         # Fit the MRC classifier
         self.minimax_risk(xTe, tau_, lambda_, n_classes)
@@ -342,56 +379,88 @@
             alpha_ = np.ones((t, 1))
             # Define the objetive function
             objective = cvx.Minimize(cvx.quad_form(cvx.vstack([beta_/n, -alpha_/t]), cvx.psd_wrap(K)))
             # Define the constraints
             constraints = [ 
                 beta_ >= np.zeros((n, 1)),
                 beta_ <= (self.B / np.sqrt(self.D)) * np.ones((n, 1)),
-                cvx.abs(cvx.sum(beta_) / n - 1) <= epsilon_,
+                cvx.sum(beta_) / n - 1 <= epsilon_,
+                -  epsilon_ <= cvx.sum(beta_) / n - 1,
             ]
             problem = cvx.Problem(objective,constraints)
             try:
                 problem.solve(solver = 'ECOS')
             except cvx.error.SolverError:
                 try:
                     problem.solve(solver = 'OSQP')
                 except cvx.error.SolverError:
                     raise ValueError('CVXpy couldn\'t find a solution for ' + \
                                      'alpha and beta .... ' + \
-                         'The problem is ', prob.status)
+                         'The problem is ', problem.status)
 
             self.beta_ = beta_.value
             self.alpha_ = alpha_
             self.min_DWKMM = problem.value
 
+        elif self.D == np.inf:
+            # Define the variables of the opt. problem
+            print('Solving DWKMM for D equal infinity')
+            beta_ = np.ones((n, 1))
+            alpha_ = cvx.Variable((t, 1))
+            epsilon_ = 1 - 1 / (np.sqrt(t))
+            # Define the objetive function
+            objective = cvx.Minimize(cvx.quad_form(cvx.vstack([beta_/n, -alpha_/t]), cvx.psd_wrap(K)))
+            # Define the constraints
+            constraints = [ 
+                alpha_ >= np.zeros((n, 1)),
+                alpha_ <= np.ones((n, 1)),
+                cvx.sum(alpha_) / t - 1 <= epsilon_,
+                -  epsilon_ <= cvx.sum(alpha_) / t - 1,
+            ]
+            problem = cvx.Problem(objective,constraints)
+            try:
+                problem.solve(solver = 'ECOS')
+            except cvx.error.SolverError:
+                try:
+                    problem.solve(solver = 'OSQP')
+                except cvx.error.SolverError:
+                    raise ValueError('CVXpy couldn\'t find a solution for ' + \
+                                     'alpha and beta .... ' + \
+                         'The problem is ', problem.status)
+
+            self.beta_ = beta_
+            self.alpha_ = alpha_.value
+            self.min_DWKMM = problem.value
+
         else:
             # Define the variables of the opt. problem
             beta_ = cvx.Variable((n, 1))
             alpha_ = cvx.Variable((t, 1))
             # Define the objetive function
             objective = cvx.Minimize(cvx.quad_form(cvx.vstack([beta_/n, -alpha_/t]), cvx.psd_wrap(K)))
             # Define the constraints
             constraints = [ 
                 beta_ >= np.zeros((n, 1)),
                 beta_ <= (self.B / np.sqrt(self.D)) * np.ones((n, 1)),
                 alpha_ >= np.zeros((t, 1)),
                 alpha_ <= np.ones((t, 1)),
-                cvx.abs(cvx.sum(beta_) / n - cvx.sum(alpha_) / t) <= epsilon_,
+                cvx.sum(beta_) / n - cvx.sum(alpha_) / t <= epsilon_,
+                - epsilon_ <= cvx.sum(beta_) / n - cvx.sum(alpha_) / t,
                 cvx.norm(alpha_ - np.ones((t, 1))) <= (1 - 1 / np.sqrt(self.D)) * np.sqrt(t)
             ]
             problem = cvx.Problem(objective,constraints)
             try:
                 problem.solve(solver = 'ECOS')
             except cvx.error.SolverError:
                 try:
                     problem.solve(solver = 'OSQP')
                 except cvx.error.SolverError:
                     raise ValueError('CVXpy couldn\'t find a solution for ' + \
                                      'alpha and beta .... ' + \
-                         'The problem is ', prob.status)
+                         'The problem is ', problem.status)
 
             self.beta_ = beta_.value
             self.alpha_ = alpha_.value
             self.min_DWKMM = problem.value
 
         return self
```

### Comparing `MRCpy-2.1.7/MRCpy/mrc.py` & `MRCpy-2.1.8/MRCpy/mrc.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/phi/base_phi.py` & `MRCpy-2.1.8/MRCpy/phi/base_phi.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/phi/random_fourier_phi.py` & `MRCpy-2.1.8/MRCpy/phi/random_fourier_phi.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/phi/random_relu_phi.py` & `MRCpy-2.1.8/MRCpy/phi/random_relu_phi.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/phi/threshold_phi.py` & `MRCpy-2.1.8/MRCpy/phi/threshold_phi.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/solvers/adam.py` & `MRCpy-2.1.8/MRCpy/solvers/adam.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/solvers/cg.py` & `MRCpy-2.1.8/MRCpy/solvers/cg.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/solvers/cvx.py` & `MRCpy-2.1.8/MRCpy/solvers/cvx.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/solvers/nesterov.py` & `MRCpy-2.1.8/MRCpy/solvers/nesterov.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy/solvers/sgd.py` & `MRCpy-2.1.8/MRCpy/solvers/sgd.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/MRCpy.egg-info/PKG-INFO` & `MRCpy-2.1.8/MRCpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MRCpy
-Version: 2.1.7
+Version: 2.1.8
 Summary: Library for minimax risk classifiers
 Home-page: https://github.com/MachineLearningBCAM/MRCpy
 Author-email: Kartheek Bondugula <kbondugula@bcamath.org>
 Project-URL: Homepage, https://github.com/MachineLearningBCAM/MRCpy
 Project-URL: Issues, https://github.com/MachineLearningBCAM/MRCpy/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `MRCpy-2.1.7/MRCpy.egg-info/SOURCES.txt` & `MRCpy-2.1.8/MRCpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/PKG-INFO` & `MRCpy-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MRCpy
-Version: 2.1.7
+Version: 2.1.8
 Summary: Library for minimax risk classifiers
 Home-page: https://github.com/MachineLearningBCAM/MRCpy
 Author-email: Kartheek Bondugula <kbondugula@bcamath.org>
 Project-URL: Homepage, https://github.com/MachineLearningBCAM/MRCpy
 Project-URL: Issues, https://github.com/MachineLearningBCAM/MRCpy/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `MRCpy-2.1.7/README.md` & `MRCpy-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `MRCpy-2.1.7/pyproject.toml` & `MRCpy-2.1.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "MRCpy"
-version = "2.1.7"
+version = "2.1.8"
 authors = [
   { name="Kartheek Bondugula", email="kbondugula@bcamath.org" },
 ]
 description = "Library for minimax risk classifiers"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `MRCpy-2.1.7/setup.py` & `MRCpy-2.1.8/setup.py`

 * *Files identical despite different names*

