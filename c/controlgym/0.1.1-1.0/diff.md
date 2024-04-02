# Comparing `tmp/controlgym-0.1.1.tar.gz` & `tmp/controlgym-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "controlgym-0.1.1.tar", max compression
+gzip compressed data, was "controlgym-1.0.tar", max compression
```

## Comparing `controlgym-0.1.1.tar` & `controlgym-1.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0     1072 2023-12-01 00:44:19.370362 controlgym-0.1.1/LICENSE
--rw-r--r--   0        0        0     3090 2023-12-01 01:48:05.492417 controlgym-0.1.1/README.md
--rw-r--r--   0        0        0      103 2023-11-27 17:46:06.398851 controlgym-0.1.1/controlgym/__init__.py
--rw-r--r--   0        0        0      222 2023-11-06 19:33:15.277887 controlgym-0.1.1/controlgym/controllers/__init__.py
--rw-r--r--   0        0        0     6656 2023-11-06 20:41:08.319763 controlgym-0.1.1/controlgym/controllers/h2hinf.py
--rw-r--r--   0        0        0     8249 2023-11-30 16:54:34.402131 controlgym-0.1.1/controlgym/controllers/lqg.py
--rw-r--r--   0        0        0     5117 2023-11-30 16:54:43.522940 controlgym-0.1.1/controlgym/controllers/lqr.py
--rw-r--r--   0        0        0    11263 2023-11-28 03:54:04.875453 controlgym-0.1.1/controlgym/controllers/ppo.py
--rw-r--r--   0        0        0     2306 2023-11-06 20:40:45.013523 controlgym-0.1.1/controlgym/controllers/zero.py
--rw-r--r--   0        0        0      728 2023-11-04 03:22:03.781064 controlgym-0.1.1/controlgym/envs/__init__.py
--rw-r--r--   0        0        0     6157 2024-02-01 21:55:09.742317 controlgym-0.1.1/controlgym/envs/allen_cahn.py
--rw-r--r--   0        0        0     5647 2024-02-01 21:55:13.621227 controlgym-0.1.1/controlgym/envs/burgers.py
--rw-r--r--   0        0        0     6313 2024-02-01 21:55:20.419089 controlgym-0.1.1/controlgym/envs/cahn_hilliard.py
--rw-r--r--   0        0        0     9286 2023-11-30 16:48:22.896978 controlgym-0.1.1/controlgym/envs/convection_diffusion_reaction.py
--rw-r--r--   0        0        0     5868 2024-02-01 21:55:32.106781 controlgym-0.1.1/controlgym/envs/fisher.py
--rw-r--r--   0        0        0     5107 2024-02-01 21:56:09.299872 controlgym-0.1.1/controlgym/envs/ginzburg_landau.py
--rw-r--r--   0        0        0     5705 2024-02-01 21:55:59.327867 controlgym-0.1.1/controlgym/envs/korteweg_de_vries.py
--rw-r--r--   0        0        0     5373 2024-02-01 21:56:21.068910 controlgym-0.1.1/controlgym/envs/kuramoto_sivashinsky.py
--rw-r--r--   0        0        0    15163 2023-11-30 16:50:55.606083 controlgym-0.1.1/controlgym/envs/linear_control.py
--rw-r--r--   0        0        0     1512 2023-10-09 21:01:01.893422 controlgym-0.1.1/controlgym/envs/linear_control_src/ac1.mat
--rw-r--r--   0        0        0     2712 2023-10-09 21:01:01.911699 controlgym-0.1.1/controlgym/envs/linear_control_src/ac10.mat
--rw-r--r--   0        0        0     1776 2023-10-09 21:01:01.896149 controlgym-0.1.1/controlgym/envs/linear_control_src/ac2.mat
--rw-r--r--   0        0        0     1136 2023-10-09 21:01:01.897674 controlgym-0.1.1/controlgym/envs/linear_control_src/ac3.mat
--rw-r--r--   0        0        0     2032 2023-10-09 21:01:01.899235 controlgym-0.1.1/controlgym/envs/linear_control_src/ac4.mat
--rw-r--r--   0        0        0     3224 2023-10-09 21:01:01.900806 controlgym-0.1.1/controlgym/envs/linear_control_src/ac5.mat
--rw-r--r--   0        0        0     3808 2023-10-09 21:01:01.902214 controlgym-0.1.1/controlgym/envs/linear_control_src/ac6.mat
--rw-r--r--   0        0        0    30432 2023-10-09 21:01:01.904891 controlgym-0.1.1/controlgym/envs/linear_control_src/ac7.mat
--rw-r--r--   0        0        0     1328 2023-10-09 21:01:01.908728 controlgym-0.1.1/controlgym/envs/linear_control_src/ac8.mat
--rw-r--r--   0        0        0    21288 2023-10-09 21:01:01.910234 controlgym-0.1.1/controlgym/envs/linear_control_src/ac9.mat
--rw-r--r--   0        0        0     3032 2023-10-09 21:01:01.913039 controlgym-0.1.1/controlgym/envs/linear_control_src/bdt1.mat
--rw-r--r--   0        0        0    63936 2023-10-09 21:01:01.921930 controlgym-0.1.1/controlgym/envs/linear_control_src/bdt2.mat
--rw-r--r--   0        0        0   983496 2023-10-09 21:01:01.965452 controlgym-0.1.1/controlgym/envs/linear_control_src/cbm.mat
--rw-r--r--   0        0        0   125664 2023-10-09 21:01:02.437126 controlgym-0.1.1/controlgym/envs/linear_control_src/cdp.mat
--rw-r--r--   0        0        0     5088 2023-10-09 21:01:02.458907 controlgym-0.1.1/controlgym/envs/linear_control_src/cm1.mat
--rw-r--r--   0        0        0    32928 2023-10-09 21:01:02.461089 controlgym-0.1.1/controlgym/envs/linear_control_src/cm2.mat
--rw-r--r--   0        0        0   122688 2023-10-09 21:01:02.473883 controlgym-0.1.1/controlgym/envs/linear_control_src/cm3.mat
--rw-r--r--   0        0        0   475008 2023-10-09 21:01:02.525852 controlgym-0.1.1/controlgym/envs/linear_control_src/cm4.mat
--rw-r--r--   0        0        0  1870848 2023-10-09 21:01:02.741829 controlgym-0.1.1/controlgym/envs/linear_control_src/cm5.mat
--rw-r--r--   0        0        0     2656 2023-10-09 21:01:06.249662 controlgym-0.1.1/controlgym/envs/linear_control_src/dis1.mat
--rw-r--r--   0        0        0     1320 2023-10-09 21:01:06.252347 controlgym-0.1.1/controlgym/envs/linear_control_src/dis2.mat
--rw-r--r--   0        0        0    29568 2023-10-09 21:01:06.254811 controlgym-0.1.1/controlgym/envs/linear_control_src/dlr.mat
--rw-r--r--   0        0        0     1136 2023-10-09 21:01:06.257003 controlgym-0.1.1/controlgym/envs/linear_control_src/he1.mat
--rw-r--r--   0        0        0     3008 2023-10-09 21:01:06.258561 controlgym-0.1.1/controlgym/envs/linear_control_src/he2.mat
--rw-r--r--   0        0        0     4672 2023-10-09 21:01:06.260106 controlgym-0.1.1/controlgym/envs/linear_control_src/he3.mat
--rw-r--r--   0        0        0     2320 2023-10-09 21:01:06.261753 controlgym-0.1.1/controlgym/envs/linear_control_src/he4.mat
--rw-r--r--   0        0        0    10592 2023-10-09 21:01:06.263616 controlgym-0.1.1/controlgym/envs/linear_control_src/he5.mat
--rw-r--r--   0        0        0    11600 2023-10-09 21:01:06.265392 controlgym-0.1.1/controlgym/envs/linear_control_src/he6.mat
--rw-r--r--   0        0        0  1197464 2023-10-09 21:01:06.290659 controlgym-0.1.1/controlgym/envs/linear_control_src/iss.mat
--rw-r--r--   0        0        0    22256 2023-10-09 21:01:06.560985 controlgym-0.1.1/controlgym/envs/linear_control_src/je1.mat
--rw-r--r--   0        0        0    10856 2023-10-09 21:01:06.563640 controlgym-0.1.1/controlgym/envs/linear_control_src/je2.mat
--rw-r--r--   0        0        0    21496 2023-10-09 21:01:06.565763 controlgym-0.1.1/controlgym/envs/linear_control_src/lah.mat
--rw-r--r--   0        0        0     1256 2023-10-09 21:01:06.569589 controlgym-0.1.1/controlgym/envs/linear_control_src/pas.mat
--rw-r--r--   0        0        0     1976 2023-10-09 21:01:06.571181 controlgym-0.1.1/controlgym/envs/linear_control_src/psm.mat
--rw-r--r--   0        0        0     1496 2023-10-09 21:01:06.572659 controlgym-0.1.1/controlgym/envs/linear_control_src/rea.mat
--rw-r--r--   0        0        0      896 2023-10-20 00:00:00.960222 controlgym-0.1.1/controlgym/envs/linear_control_src/toy.mat
--rw-r--r--   0        0        0     1728 2023-10-09 21:01:06.574055 controlgym-0.1.1/controlgym/envs/linear_control_src/umv.mat
--rw-r--r--   0        0        0    18391 2024-02-01 21:57:10.261233 controlgym-0.1.1/controlgym/envs/pde.py
--rw-r--r--   0        0        0     2746 2023-11-06 20:40:22.643309 controlgym-0.1.1/controlgym/envs/registrations.py
--rw-r--r--   0        0        0    12665 2023-11-30 16:48:08.869492 controlgym-0.1.1/controlgym/envs/schrodinger.py
--rw-r--r--   0        0        0     2640 2023-11-04 01:43:59.808650 controlgym-0.1.1/controlgym/envs/utils.py
--rw-r--r--   0        0        0    11687 2023-11-30 16:47:57.973076 controlgym-0.1.1/controlgym/envs/wave.py
--rw-r--r--   0        0        0       68 2023-11-06 18:10:03.340647 controlgym-0.1.1/controlgym/helpers/__init__.py
--rw-r--r--   0        0        0     3437 2023-11-28 16:33:05.614168 controlgym-0.1.1/controlgym/helpers/data_processing.py
--rw-r--r--   0        0        0    11742 2023-11-28 17:01:36.383984 controlgym-0.1.1/controlgym/helpers/plotting.py
--rw-r--r--   0        0        0      654 2024-02-01 22:15:20.795756 controlgym-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3824 1970-01-01 00:00:00.000000 controlgym-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-01 00:44:19.370362 controlgym-1.0/LICENSE
+-rw-r--r--   0        0        0     3034 2024-04-02 16:27:54.441313 controlgym-1.0/README.md
+-rw-r--r--   0        0        0      103 2023-11-27 17:46:06.398851 controlgym-1.0/controlgym/__init__.py
+-rw-r--r--   0        0        0      222 2023-11-06 19:33:15.277887 controlgym-1.0/controlgym/controllers/__init__.py
+-rw-r--r--   0        0        0     6656 2023-11-06 20:41:08.319763 controlgym-1.0/controlgym/controllers/h2hinf.py
+-rw-r--r--   0        0        0     8249 2023-11-30 16:54:34.402131 controlgym-1.0/controlgym/controllers/lqg.py
+-rw-r--r--   0        0        0     5117 2023-11-30 16:54:43.522940 controlgym-1.0/controlgym/controllers/lqr.py
+-rw-r--r--   0        0        0    11296 2024-04-02 03:15:45.833295 controlgym-1.0/controlgym/controllers/ppo.py
+-rw-r--r--   0        0        0     2306 2023-11-06 20:40:45.013523 controlgym-1.0/controlgym/controllers/zero.py
+-rw-r--r--   0        0        0      728 2023-11-04 03:22:03.781064 controlgym-1.0/controlgym/envs/__init__.py
+-rw-r--r--   0        0        0     6272 2024-04-02 03:14:11.599382 controlgym-1.0/controlgym/envs/allen_cahn.py
+-rw-r--r--   0        0        0     6592 2024-04-02 03:14:28.665852 controlgym-1.0/controlgym/envs/burgers.py
+-rw-r--r--   0        0        0     6541 2024-04-02 03:00:35.184670 controlgym-1.0/controlgym/envs/cahn_hilliard.py
+-rw-r--r--   0        0        0    10225 2024-04-02 03:00:49.396898 controlgym-1.0/controlgym/envs/convection_diffusion_reaction.py
+-rw-r--r--   0        0        0     6199 2024-04-02 03:01:00.333312 controlgym-1.0/controlgym/envs/fisher.py
+-rw-r--r--   0        0        0     6390 2024-04-02 03:01:29.760167 controlgym-1.0/controlgym/envs/ginzburg_landau.py
+-rw-r--r--   0        0        0     5804 2024-04-02 03:01:35.917044 controlgym-1.0/controlgym/envs/korteweg_de_vries.py
+-rw-r--r--   0        0        0     5842 2024-04-02 03:01:51.078687 controlgym-1.0/controlgym/envs/kuramoto_sivashinsky.py
+-rw-r--r--   0        0        0    15172 2024-04-02 03:13:45.684795 controlgym-1.0/controlgym/envs/linear_control.py
+-rw-r--r--   0        0        0        0 2024-03-30 15:58:46.314983 controlgym-1.0/controlgym/envs/linear_control_src/__init__.py
+-rw-r--r--   0        0        0     1512 2023-10-09 21:01:01.893422 controlgym-1.0/controlgym/envs/linear_control_src/ac1.mat
+-rw-r--r--   0        0        0     2712 2023-10-09 21:01:01.911699 controlgym-1.0/controlgym/envs/linear_control_src/ac10.mat
+-rw-r--r--   0        0        0     1776 2023-10-09 21:01:01.896149 controlgym-1.0/controlgym/envs/linear_control_src/ac2.mat
+-rw-r--r--   0        0        0     1136 2023-10-09 21:01:01.897674 controlgym-1.0/controlgym/envs/linear_control_src/ac3.mat
+-rw-r--r--   0        0        0     2032 2023-10-09 21:01:01.899235 controlgym-1.0/controlgym/envs/linear_control_src/ac4.mat
+-rw-r--r--   0        0        0     3224 2023-10-09 21:01:01.900806 controlgym-1.0/controlgym/envs/linear_control_src/ac5.mat
+-rw-r--r--   0        0        0     3808 2023-10-09 21:01:01.902214 controlgym-1.0/controlgym/envs/linear_control_src/ac6.mat
+-rw-r--r--   0        0        0    30432 2023-10-09 21:01:01.904891 controlgym-1.0/controlgym/envs/linear_control_src/ac7.mat
+-rw-r--r--   0        0        0     1328 2023-10-09 21:01:01.908728 controlgym-1.0/controlgym/envs/linear_control_src/ac8.mat
+-rw-r--r--   0        0        0    21288 2023-10-09 21:01:01.910234 controlgym-1.0/controlgym/envs/linear_control_src/ac9.mat
+-rw-r--r--   0        0        0     3032 2023-10-09 21:01:01.913039 controlgym-1.0/controlgym/envs/linear_control_src/bdt1.mat
+-rw-r--r--   0        0        0    63936 2023-10-09 21:01:01.921930 controlgym-1.0/controlgym/envs/linear_control_src/bdt2.mat
+-rw-r--r--   0        0        0   983496 2023-10-09 21:01:01.965452 controlgym-1.0/controlgym/envs/linear_control_src/cbm.mat
+-rw-r--r--   0        0        0   125664 2023-10-09 21:01:02.437126 controlgym-1.0/controlgym/envs/linear_control_src/cdp.mat
+-rw-r--r--   0        0        0     5088 2023-10-09 21:01:02.458907 controlgym-1.0/controlgym/envs/linear_control_src/cm1.mat
+-rw-r--r--   0        0        0    32928 2023-10-09 21:01:02.461089 controlgym-1.0/controlgym/envs/linear_control_src/cm2.mat
+-rw-r--r--   0        0        0   122688 2023-10-09 21:01:02.473883 controlgym-1.0/controlgym/envs/linear_control_src/cm3.mat
+-rw-r--r--   0        0        0   475008 2023-10-09 21:01:02.525852 controlgym-1.0/controlgym/envs/linear_control_src/cm4.mat
+-rw-r--r--   0        0        0  1870848 2023-10-09 21:01:02.741829 controlgym-1.0/controlgym/envs/linear_control_src/cm5.mat
+-rw-r--r--   0        0        0     2656 2023-10-09 21:01:06.249662 controlgym-1.0/controlgym/envs/linear_control_src/dis1.mat
+-rw-r--r--   0        0        0     1320 2023-10-09 21:01:06.252347 controlgym-1.0/controlgym/envs/linear_control_src/dis2.mat
+-rw-r--r--   0        0        0    29568 2023-10-09 21:01:06.254811 controlgym-1.0/controlgym/envs/linear_control_src/dlr.mat
+-rw-r--r--   0        0        0     1136 2023-10-09 21:01:06.257003 controlgym-1.0/controlgym/envs/linear_control_src/he1.mat
+-rw-r--r--   0        0        0     3008 2023-10-09 21:01:06.258561 controlgym-1.0/controlgym/envs/linear_control_src/he2.mat
+-rw-r--r--   0        0        0     4672 2023-10-09 21:01:06.260106 controlgym-1.0/controlgym/envs/linear_control_src/he3.mat
+-rw-r--r--   0        0        0     2320 2023-10-09 21:01:06.261753 controlgym-1.0/controlgym/envs/linear_control_src/he4.mat
+-rw-r--r--   0        0        0    10592 2023-10-09 21:01:06.263616 controlgym-1.0/controlgym/envs/linear_control_src/he5.mat
+-rw-r--r--   0        0        0    11600 2023-10-09 21:01:06.265392 controlgym-1.0/controlgym/envs/linear_control_src/he6.mat
+-rw-r--r--   0        0        0  1197464 2023-10-09 21:01:06.290659 controlgym-1.0/controlgym/envs/linear_control_src/iss.mat
+-rw-r--r--   0        0        0    22256 2023-10-09 21:01:06.560985 controlgym-1.0/controlgym/envs/linear_control_src/je1.mat
+-rw-r--r--   0        0        0    10856 2023-10-09 21:01:06.563640 controlgym-1.0/controlgym/envs/linear_control_src/je2.mat
+-rw-r--r--   0        0        0    21496 2023-10-09 21:01:06.565763 controlgym-1.0/controlgym/envs/linear_control_src/lah.mat
+-rw-r--r--   0        0        0     1256 2023-10-09 21:01:06.569589 controlgym-1.0/controlgym/envs/linear_control_src/pas.mat
+-rw-r--r--   0        0        0     1976 2023-10-09 21:01:06.571181 controlgym-1.0/controlgym/envs/linear_control_src/psm.mat
+-rw-r--r--   0        0        0     1496 2023-10-09 21:01:06.572659 controlgym-1.0/controlgym/envs/linear_control_src/rea.mat
+-rw-r--r--   0        0        0      896 2023-10-20 00:00:00.960222 controlgym-1.0/controlgym/envs/linear_control_src/toy.mat
+-rw-r--r--   0        0        0     1728 2023-10-09 21:01:06.574055 controlgym-1.0/controlgym/envs/linear_control_src/umv.mat
+-rw-r--r--   0        0        0    18656 2024-04-02 15:40:52.015224 controlgym-1.0/controlgym/envs/pde.py
+-rw-r--r--   0        0        0     2746 2024-02-16 18:16:20.925451 controlgym-1.0/controlgym/envs/registrations.py
+-rw-r--r--   0        0        0    13558 2024-04-02 03:02:43.681311 controlgym-1.0/controlgym/envs/schrodinger.py
+-rw-r--r--   0        0        0     2640 2023-11-04 01:43:59.808650 controlgym-1.0/controlgym/envs/utils.py
+-rw-r--r--   0        0        0    12611 2024-04-02 03:14:56.441517 controlgym-1.0/controlgym/envs/wave.py
+-rw-r--r--   0        0        0       68 2023-11-06 18:10:03.340647 controlgym-1.0/controlgym/helpers/__init__.py
+-rw-r--r--   0        0        0     3437 2024-04-02 03:22:44.346723 controlgym-1.0/controlgym/helpers/data_processing.py
+-rw-r--r--   0        0        0    11742 2023-11-28 17:01:36.383984 controlgym-1.0/controlgym/helpers/plotting.py
+-rw-r--r--   0        0        0      706 2024-04-02 16:19:53.318499 controlgym-1.0/pyproject.toml
+-rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 controlgym-1.0/PKG-INFO
```

### Comparing `controlgym-0.1.1/LICENSE` & `controlgym-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/README.md` & `controlgym-1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # controlgym
 
 ## Description
-`Controlgym` provides 36 safety-critical industrial control environments and 10 infinite-dimensional PDE-based control problems with continuous, unbounded action and observation spaces that are inspired by real-world applications. This project supports the Learning for Dynamics & Control (L4DC) community, focusing on vital issues: convergence of reinforcement learning (RL) algorithms in policy development, stability, safety, and robustness of learning-based controllers, and the scalability of RL algorithms to high and potentially infinite-dimensional systems. We provide a detailed description of `controlgym` in [this paper](https://arxiv.org/abs/2311.18736).
+`Controlgym` provides 36 industrial control environments and 10 infinite-dimensional PDE-based control problems with continuous, unbounded action and observation spaces that are inspired by real-world applications. This project supports the Learning for Dynamics & Control (L4DC) community, focusing on vital issues: convergence of reinforcement learning (RL) algorithms in policy development, stability, and robustness of learning-based controllers, and the scalability of RL algorithms to high and potentially infinite-dimensional systems. We provide a detailed description of `controlgym` in [this paper](https://arxiv.org/abs/2311.18736).
 
 <p align="center">
   <img src="figures/gallery.jpeg" alt="" width="700px">
 </p>
 
 
 
@@ -76,17 +76,17 @@
 </details>
 
 
 ## Getting Started
 Check out our code examples in this [Jupyter notebook file](./examples.ipynb).
 
 ## Reference
-- Zhang, X., Mao, W., Mowlavi, S., Benosman, M., & Başar, T. (2023). [Controlgym: Large-Scale Safety-Critical Control Environments for Benchmarking Reinforcement Learning Algorithms.](https://arxiv.org/abs/2311.18736) arXiv preprint arXiv:2311.18736.
+- Zhang, X., Mao, W., Mowlavi, S., Benosman, M., & Başar, T. (2023). [Controlgym: Large-Scale Control Environments for Benchmarking Reinforcement Learning Algorithms.](https://arxiv.org/abs/2311.18736) arXiv preprint arXiv:2311.18736.
   
 ```bibtex
 @article{zhang2023controlgym,
-    title = {Controlgym: Large-Scale Safety-Critical Control Environments for Benchmarking Reinforcement Learning Algorithms},
+    title = {Controlgym: Large-Scale Control Environments for Benchmarking Reinforcement Learning Algorithms},
     author = {Zhang, Xiangyuan and Mao, Weichao and Mowlavi, Saviz and Benosman, Mouhacine and Ba{\c{s}}ar, Tamer},
     journal = {arXiv preprint arXiv:2311.18736},
     year = {2023}
 }
 ```
```

### Comparing `controlgym-0.1.1/controlgym/controllers/h2hinf.py` & `controlgym-1.0/controlgym/controllers/h2hinf.py`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/controllers/lqg.py` & `controlgym-1.0/controlgym/controllers/lqg.py`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/controllers/lqr.py` & `controlgym-1.0/controlgym/controllers/lqr.py`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/controllers/ppo.py` & `controlgym-1.0/controlgym/controllers/ppo.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,16 @@
             seed: (optional int), random seed for the environment.
 
         Returns:
             total_reward: float, the accumulated reward of the trajectory.
         """
         # reset the environment
         observation, info = self.env.reset(seed=seed, state=state)
-        torch.manual_seed(seed=seed)
+        if seed is not None:
+            torch.manual_seed(seed=seed)
         # run the simulated trajectory and calculate the h2 cost
         total_reward = 0
         state_traj = np.zeros((self.env.n_state, self.env.n_steps + 1))
         state_traj[:, 0] = info["state"]
         for t in range(self.env.n_steps):
             action = self.select_action(observation, cov_param=0.0)
             observation, reward, terminated, truncated, info = self.env.step(action)
```

### Comparing `controlgym-0.1.1/controlgym/controllers/zero.py` & `controlgym-1.0/controlgym/controllers/zero.py`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/__init__.py` & `controlgym-1.0/controlgym/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/allen_cahn.py` & `controlgym-1.0/controlgym/envs/allen_cahn.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,95 +21,97 @@
     optional arguments:
     [n_steps]: the number of discrete-time steps. Default is 100.
     [domain_length]: domain length of PDE. Default is 2.0.
     [integration_time]: numerical integration time step. Default is 0.001.
     [sample_time]: each discrete-time step represents (ts) seconds. Default is 0.01.
     [process_noise_cov]: process noise covariance coefficient. Default is 0.0.
     [sensor_noise_cov]: sensor noise covariance coefficient. Default is 0.25.
-    [random_init_state_cov]: random initial state covariance coefficient. Default is 0.0.
     [target_state]: target state. Default is np.zeros(n_state).
-    [init_state]: initial state. Default is
-        (self.domain_coordinates - 0.5 * self.domain_length) ** 2 
-        * np.cos((2 * np.pi * (self.domain_coordinates - 0.5 * self.domain_length)) / self.domain_length)
+    [init_offset_mean]: mean of initial offset. Default is 0.
+    [init_offset_width]: width of initial offset. Default is 0.2.
     [diffusivity_constant]: diffusivity constant. Default is 1e-4.
     [potential_constant]: potential constant. Default is 5.0.
     [n_state]: dimension of state vector. Default is 256.
     [n_observation]: dimension of observation vector. Default is 10.
     [n_action]: dimension of control vector. Default is 8.
     [control_sup_width]: control support width. Default is 0.1.
     [Q_weight]: weight of state tracking cost. Default is 1.0.
     [R_weight]: weight of control cost. Default is 1.0.
     [action_limit]: limit of action. Default is None.
     [observation_limit]: limit of observation. Default is None.
     [reward_limit]: limit of reward. Default is 1e15.
-    [seed]: random seed. Default is 0.
+    [seed]: random seed. Default is None.
     """
     def __init__(
         self,
         n_steps: int = 100,
         domain_length: float = 2.0,
-        integration_time: float = 0.001, 
+        integration_time: float = 0.001,
         sample_time: float = 0.01,
         process_noise_cov: float = 0.0,
         sensor_noise_cov: float = 0.25,
-        random_init_state_cov: float = 0.0,
         target_state: np.ndarray[float] = None,
-        init_state: np.ndarray[float] = None,
+        init_offset_mean: float = 0.0,
+        init_offset_width: float = 0.2,
         diffusivity_constant: float = 1e-4,
         potential_constant: float = 5.0,
         n_state: int = 256,
         n_observation: int = 10,
         n_action: int = 8,
         control_sup_width: float = 0.1,
         Q_weight: float = 1.0,
         R_weight: float = 1.0,
         action_limit: float = None,
         observation_limit: float = None,
         reward_limit: float = None,
-        seed: int = 0,
+        seed: int = None,
     ):
         PDE.__init__(
             self,
             id="allen_cahn",
             n_steps=n_steps, 
             domain_length=domain_length, 
             integration_time=integration_time, 
             sample_time=sample_time, 
             process_noise_cov=process_noise_cov, 
-            sensor_noise_cov=sensor_noise_cov, 
-            random_init_state_cov=random_init_state_cov, 
+            sensor_noise_cov=sensor_noise_cov,
             target_state=target_state,
             n_state=n_state,  
             n_observation=n_observation,  
             n_action=n_action,  
             control_sup_width=control_sup_width, 
             Q_weight=Q_weight,
             R_weight=R_weight, 
             action_limit=action_limit,
             observation_limit=observation_limit,
             reward_limit=reward_limit,
             seed=seed, 
         )
 
-        if init_state is not None:
-            self.init_state = init_state
-        else:
-            self.init_state = (
-                self.domain_coordinates - 0.5 * self.domain_length
-            ) ** 2 * np.cos(
-                (2 * np.pi * (self.domain_coordinates - 0.5 * self.domain_length))
-                / self.domain_length
-            )
-        self.state = self.init_state
+        # physical parameters
         self.diffusivity_constant = diffusivity_constant
         self.potential_constant = potential_constant
 
-        # compute control sup, observation matrix
-        self.control_sup = self._compute_control_sup()
-        self.C = self._compute_C()
+        # initial state parameters
+        self.init_offset_mean = init_offset_mean
+        self.init_offset_width = init_offset_width
+        self.reset()
+
+    def select_init_state(self, init_offset=None):
+        """Function to select the initial state of the PDE."""
+        if init_offset is None:
+            random_offset = self.rng.uniform(-0.5 * self.init_offset_width, 0.5 * self.init_offset_width)
+            init_offset = self.init_offset_mean + random_offset
+        init_state = init_offset + (
+            self.domain_coordinates - 0.5 * self.domain_length
+        ) ** 2 * np.cos(
+            (2 * np.pi * (self.domain_coordinates - 0.5 * self.domain_length))
+            / self.domain_length
+        )
+        return init_state
 
     def _compute_fourier_linear_op(self):
         """Private function to compute the linear operator of the PDE in Fourier space.
 
         Args:
             None.
 
@@ -153,9 +155,11 @@
         Returns:
             a dictionary containing the parameters of the pde environment + extra parameters.
         """
         pde_dict = super().get_params_asdict()
         extra_data = {
             "diffusivity_constant": self.diffusivity_constant,
             "potential_constant": self.potential_constant,
+            "init_offset_mean": self.init_offset_mean,
+            "init_offset_width": self.init_offset_width,
         }
         return {**pde_dict, **extra_data}
```

### Comparing `controlgym-0.1.1/controlgym/envs/burgers.py` & `controlgym-1.0/controlgym/envs/fisher.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,109 +1,118 @@
 import numpy as np
 from controlgym.envs import PDE
 
 
-class BurgersEnv(PDE):
+class FisherEnv(PDE):
     """
     ### Description
 
-    This environment models the Burgers' equation, described by:
-        du/dt =  diffusivity_constant * d^2u/dx^2 - u * du/dx
+    This environment models the Fisher (or Fisher-KPP) equation, described by:
+        du/dt =  diffusivity_constant * d^2u/dx^2
+            + reaction_constant * u(1-u)
 
     ### Action Space, Observation Space, Rewards, Episode Termination
 
     See parent class `PDE` defined in pde.py for details.
 
     ### Arguments
 
     ```
-    controlgym.make('burgers')
+    controlgym.make('fisher')
     ```
     optional arguments:
     [n_steps]: the number of discrete-time steps. Default is 100.
-    [domain_length]: domain length of PDE. Default is 1.0.
+    [domain_length]: domain length of PDE. Default is 10.0.
     [integration_time]: numerical integration time step. Default is 0.001.
     [sample_time]: each discrete-time step represents (ts) seconds. Default is 0.05.
     [process_noise_cov]: process noise covariance coefficient. Default is 0.0.
     [sensor_noise_cov]: sensor noise covariance coefficient. Default is 0.25.
-    [random_init_state_cov]: random initial state covariance coefficient. Default is 0.0.
     [target_state]: target state. Default is np.zeros(n_state).
-    [init_state]: initial state. Default is
-        np.cosh(10 * (self.domain_coordinates - 1 * self.domain_length / 2)) ** (-1).
-    [diffusivity_constant]: diffusivity constant. Default is 0.001.
+    [init_amplitude_mean]: mean of initial amplitude. Default is 1.0.
+    [init_amplitude_width]: width of initial amplitude. Default is 0.2.
+    [diffusivity_constant]: diffusivity constant. Default is 0.0001.
+    [reaction_constant]: reaction constant. Default is 0.1.
     [n_state]: dimension of state vector. Default is 256.
     [n_observation]: dimension of observation vector. Default is 10.
     [n_action]: dimension of control vector. Default is 8.
     [control_sup_width]: control support width. Default is 0.1.
     [Q_weight]: weight of state tracking cost. Default is 1.0.
     [R_weight]: weight of control cost. Default is 1.0.
     [action_limit]: limit of action. Default is None.
     [observation_limit]: limit of observation. Default is None.
     [reward_limit]: limit of reward. Default is None.
-    [seed]: random seed. Default is 0.
+    [seed]: random seed. Default is None.
     """
 
     def __init__(
         self,
         n_steps: int = 100,
-        domain_length: float = 1.0,
+        domain_length: float = 10.0,
         integration_time: float = 0.001,
         sample_time: float = 0.05,
         process_noise_cov: float = 0.0,
         sensor_noise_cov: float = 0.25,
-        random_init_state_cov: float = 0.0,
         target_state: np.ndarray[float] = None,
-        init_state: np.ndarray[float] = None,
-        diffusivity_constant: float = 0.001,
+        init_amplitude_mean: float = 1.0,
+        init_amplitude_width: float = 0.2,
+        diffusivity_constant: float = 0.0001,
+        reaction_constant: float = 0.1,
         n_state: int = 256,
         n_observation: int = 10,
         n_action: int = 8,
         control_sup_width: float = 0.1,
         Q_weight: float = 1.0,
         R_weight: float = 1.0,
         action_limit: float = None,
         observation_limit: float = None,
         reward_limit: float = None,
-        seed: int = 0,
+        seed: int = None,
     ):
         PDE.__init__(
             self,
-            id="burgers",
+            id="fisher",
             n_steps=n_steps,
             domain_length=domain_length,
             integration_time=integration_time,
             sample_time=sample_time,
             process_noise_cov=process_noise_cov,
             sensor_noise_cov=sensor_noise_cov,
-            random_init_state_cov=random_init_state_cov,
             target_state=target_state,
             n_state=n_state,
             n_observation=n_observation,
             n_action=n_action,
             control_sup_width=control_sup_width,
             Q_weight=Q_weight,
             R_weight=R_weight,
             action_limit=action_limit,
             observation_limit=observation_limit,
             reward_limit=reward_limit,
             seed=seed,
         )
 
-        if init_state is not None:
-            self.init_state = init_state
-        else:
-            self.init_state = self.init_state = np.cosh(
-                10 * (self.domain_coordinates - 1 * self.domain_length / 2)
-            ) ** (-1)
-        self.state = self.init_state
+        # physical parameters
         self.diffusivity_constant = diffusivity_constant
+        self.reaction_constant = reaction_constant
 
-        # compute control sup, observation matrix
-        self.control_sup = self._compute_control_sup()
-        self.C = self._compute_C()
+        # initial state parameters
+        self.init_amplitude_mean = init_amplitude_mean
+        self.init_amplitude_width = init_amplitude_width
+        self.reset()
+
+    def select_init_state(self, init_amplitude=None):
+        """Function to select the initial state of the PDE."""
+        if init_amplitude is None:
+            random_amplitude = self.rng.uniform(
+                -0.5 * self.init_amplitude_width, 0.5 * self.init_amplitude_width
+            )
+            init_amplitude = self.init_amplitude_mean + random_amplitude
+        init_state = init_amplitude * np.sin(
+            4 * np.pi * self.domain_coordinates / self.domain_length
+        )
+        return init_state
 
     def _compute_fourier_linear_op(self):
         """Private function to compute the linear operator of the PDE in Fourier space.
 
         Args:
             None.
 
@@ -127,18 +136,17 @@
             # aa_state is the anti-aliased state; meaning the state evaluated in
             # physical space on a grid with 3/2 times more points
             aa_factor = 3 / 2
             aa_state = aa_factor * np.fft.irfft(
                 state_fourier, n=int(self.n_state * aa_factor)
             )
             right_hand_side = (
-                -0.5j
-                * self.domain_wavenumbers
+                self.reaction_constant
                 * (1 / aa_factor)
-                * np.fft.rfft(aa_state**2)[0 : int(self.n_state / 2) + 1]
+                * np.fft.rfft(aa_state * (1 - aa_state))[0 : int(self.n_state / 2) + 1]
             ) + (np.fft.rfft(self.control_sup, axis=0) @ action)
             return right_hand_side
 
         return fourier_nonlinear_op
 
     def get_params_asdict(self):
         """Save the extra environment parameters as a dictionary.
@@ -146,9 +154,14 @@
         Args:
             None.
 
         Returns:
             a dictionary containing the parameters of the pde environment + extra parameters.
         """
         pde_dict = super().get_params_asdict()
-        extra_data = {"diffusivity_constant": self.diffusivity_constant}
+        extra_data = {
+            "diffusivity_constant": self.diffusivity_constant,
+            "reaction_constant": self.reaction_constant,
+            "init_amplitude_mean": self.init_amplitude_mean,
+            "init_amplitude_width": self.init_amplitude_width,
+        }
         return {**pde_dict, **extra_data}
```

### Comparing `controlgym-0.1.1/controlgym/envs/cahn_hilliard.py` & `controlgym-1.0/controlgym/envs/cahn_hilliard.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,95 +22,99 @@
     optional arguments:
     [n_steps]: the number of discrete-time steps. Default is 50.
     [domain_length]: domain length of PDE. Default is 2.0.
     [integration_time]: numerical integration time step. Default is 0.001.
     [sample_time]: each discrete-time step represents (ts) seconds. Default is 0.01.
     [process_noise_cov]: process noise covariance coefficient. Default is 0.0.
     [sensor_noise_cov]: sensor noise covariance coefficient. Default is 0.25.
-    [random_init_state_cov]: random initial state covariance coefficient. Default is 0.0.
     [target_state]: target state. Default is np.zeros(n_state).
-    [init_state]: initial state. Default is
-        np.cos(np.pi * (self.domain_coordinates - 0.5 * self.domain_length))
-        - np.exp(-4 * (np.pi * (self.domain_coordinates - 0.5 * self.domain_length)) ** 2)
+    [init_amplitude_mean]: mean of initial amplitude. Default is 1.0.
+    [init_amplitude_width]: width of initial amplitude. Default is 0.2.
     [diffusivity_constant]: diffusivity constant. Default is 1.0.
     [surface_tension_constant]: surface tension constant. Default is 0.02.
     [n_state]: dimension of state vector. Default is 256.
     [n_observation]: dimension of observation vector. Default is 10.
     [n_action]: dimension of control vector. Default is 8.
     [control_sup_width]: control support width. Default is 0.1.
     [Q_weight]: weight of state tracking cost. Default is 1.0.
     [R_weight]: weight of control cost. Default is 1.0.
     [action_limit]: limit of action. Default is None.
     [observation_limit]: limit of observation. Default is None.
     [reward_limit]: limit of reward. Default is None.
-    [seed]: random seed. Default is 0.
+    [seed]: random seed. Default is None.
     """
 
     def __init__(
         self,
         n_steps: int = 50,
         domain_length: float = 2.0,
         integration_time: float = 0.001,
         sample_time: float = 0.01,
         process_noise_cov: float = 0.0,
         sensor_noise_cov: float = 0.25,
-        random_init_state_cov: float = 0.0,
         target_state: np.ndarray[float] = None,
-        init_state: np.ndarray[float] = None,
+        init_amplitude_mean: float = 1.0,
+        init_amplitude_width: float = 0.2,
         diffusivity_constant: float = 1.0,
         surface_tension_constant: float = 0.02,
         n_state: int = 256,
         n_observation: int = 10,
         n_action: int = 8,
         control_sup_width: float = 0.1,
         Q_weight: float = 1.0,
         R_weight: float = 1.0,
         action_limit: float = None,
         observation_limit: float = None,
         reward_limit: float = None,
-        seed: int = 0,
+        seed: int = None,
     ):
         PDE.__init__(
             self,
             id="cahn_hilliard",
             n_steps=n_steps,
             domain_length=domain_length,
             integration_time=integration_time,
             sample_time=sample_time,
             process_noise_cov=process_noise_cov,
             sensor_noise_cov=sensor_noise_cov,
-            random_init_state_cov=random_init_state_cov,
             target_state=target_state,
             n_state=n_state,
             n_observation=n_observation,
             n_action=n_action,
             control_sup_width=control_sup_width,
             Q_weight=Q_weight,
             R_weight=R_weight,
             action_limit=action_limit,
             observation_limit=observation_limit,
             reward_limit=reward_limit,
             seed=seed,
         )
 
-        if init_state is not None:
-            self.init_state = init_state
-        else:
-            self.init_state = np.cos(
-                np.pi * (self.domain_coordinates - 0.5 * self.domain_length)
-            ) - np.exp(
-                -4 * (np.pi * (self.domain_coordinates - 0.5 * self.domain_length)) ** 2
-            )
-        self.state = self.init_state
+        # physical parameters
         self.diffusivity_constant = diffusivity_constant
         self.surface_tension_constant = surface_tension_constant
 
-        # compute control sup, observation matrix
-        self.control_sup = self._compute_control_sup()
-        self.C = self._compute_C()
+        # initial state parameters
+        self.init_amplitude_mean = init_amplitude_mean
+        self.init_amplitude_width = init_amplitude_width
+        self.reset()
+
+    def select_init_state(self, init_amplitude=None):
+        """Function to select the initial state of the PDE."""
+        if init_amplitude is None:
+            random_amplitude = self.rng.uniform(
+                -0.5 * self.init_amplitude_width, 0.5 * self.init_amplitude_width
+            )
+            init_amplitude = self.init_amplitude_mean + random_amplitude
+        init_state = init_amplitude * np.cos(
+            np.pi * (self.domain_coordinates - 0.5 * self.domain_length)
+        ) - np.exp(
+            -4 * (np.pi * (self.domain_coordinates - 0.5 * self.domain_length)) ** 2
+        )
+        return init_state
 
     def _compute_fourier_linear_op(self):
         """Private function to compute the linear operator of the PDE in Fourier space.
 
         Args:
             None.
 
@@ -159,9 +163,11 @@
         Returns:
             a dictionary containing the parameters of the pde environment + extra parameters.
         """
         pde_dict = super().get_params_asdict()
         extra_data = {
             "diffusivity_constant": self.diffusivity_constant,
             "surface_tension_constant": self.surface_tension_constant,
+            "init_amplitude_mean": self.init_amplitude_mean,
+            "init_amplitude_width": self.init_amplitude_width,
         }
         return {**pde_dict, **extra_data}
```

### Comparing `controlgym-0.1.1/controlgym/envs/convection_diffusion_reaction.py` & `controlgym-1.0/controlgym/envs/convection_diffusion_reaction.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,98 +24,115 @@
     optional arguments:
     [n_steps]: the number of discrete-time steps. Default is 100.
     [domain_length]: domain length of PDE. Default is 1.0.
     [integration_time]: numerical integration time step. Default is None.
     [sample_time]: each discrete-time step represents (ts) seconds. Default is 0.1.
     [process_noise_cov]: process noise covariance coefficient. Default is 0.0.
     [sensor_noise_cov]: sensor noise covariance coefficient. Default is 0.25.
-    [random_init_state_cov]: random initial state covariance coefficient. Default is 0.0.
     [target_state]: target state. Default is np.zeros(n_state).
-    [init_state]: initial state. Default is
-        np.cosh(10 * (self.domain_coordinates - 1 * self.domain_length / 2)) ** (-1).
+    [init_amplitude_mean]: mean of initial amplitude. Default is 1.0.
+    [init_amplitude_width]: width of initial amplitude. Default is 0.2.
+    [init_spread_mean]: mean of initial spread. Default is 0.05.
+    [init_spread_width]: width of initial spread. Default is 0.02.
     [diffusivity_constant]: diffusivity constant. Default is 0.002.
     [convective_velocity]: convective velocity. Default is 0.1.
     [reaction_constant]: reaction constant. Default is 0.1.
     [n_state]: dimension of state vector. Default is 200.
     [n_observation]: dimension of observation vector. Default is 10.
     [n_action]: dimension of control vector. Default is 8.
     [control_sup_width]: control support width. Default is 0.1.
     [Q_weight]: weight of state tracking cost. Default is 1.0.
     [R_weight]: weight of control cost. Default is 1.0.
     [action_limit]: limit of action. Default is None.
     [observation_limit]: limit of observation. Default is None.
     [reward_limit]: limit of reward. Default is None.
-    [seed]: random seed. Default is 0.
+    [seed]: random seed. Default is None.
     """
 
     def __init__(
         self,
         n_steps: int = 100,
         domain_length: float = 1.0,
         integration_time: float = None,  # Use analytical solution to evolve the dynamics
         sample_time: float = 0.1,
         process_noise_cov: float = 0.0,
         sensor_noise_cov: float = 0.25,
-        random_init_state_cov: float = 0.0,
         target_state: np.ndarray[float] = None,
-        init_state: np.ndarray[float] = None,
+        init_amplitude_mean: float = 1.0,
+        init_amplitude_width: float = 0.2,
+        init_spread_mean: float = 0.05,
+        init_spread_width: float = 0.02,
         diffusivity_constant: float = 0.002,
         convective_velocity: float = 0.1,
         reaction_constant: float = 0.1,
         n_state: int = 200,
         n_observation: int = 10,
         n_action: int = 8,
         control_sup_width: float = 0.1,
         Q_weight: float = 1.0,
         R_weight: float = 1.0,
         action_limit: float = None,
         observation_limit: float = None,
         reward_limit: float = None,
-        seed: int = 0,
+        seed: int = None,
     ):
         PDE.__init__(
             self,
             id="convection_diffusion_reaction",
             n_steps=n_steps,
             domain_length=domain_length,
             integration_time=integration_time,
             sample_time=sample_time,
             process_noise_cov=process_noise_cov,
             sensor_noise_cov=sensor_noise_cov,
-            random_init_state_cov=random_init_state_cov,
             target_state=target_state,
             n_state=n_state,
             n_observation=n_observation,
             n_action=n_action,
             control_sup_width=control_sup_width,
             Q_weight=Q_weight,
             R_weight=R_weight,
             action_limit=action_limit,
             observation_limit=observation_limit,
             reward_limit=reward_limit,
             seed=seed,
         )
 
-        # the highest priority is to use the user-provided initial state
-        if init_state is not None:
-            self.init_state = init_state
-        # if the user does not provide an initial state, use the default initial state
-        else:
-            self.init_state = np.cosh(
-                10 * (self.domain_coordinates - 1 * self.domain_length / 2)
-            ) ** (-1)
-        self.state = self.init_state
+        # physical parameters
         self.diffusivity_constant = diffusivity_constant
         self.convective_velocity = convective_velocity
         self.reaction_constant = reaction_constant
 
-        # compute A, B2, C
+        # compute A and B2 matrices
         self.A, self.eigen = self._compute_A()
-        self.B2 = self._compute_control_sup()
-        self.C = self._compute_C()
+        self.B2 = self.control_sup
+
+        # initial state parameters
+        self.init_amplitude_mean = init_amplitude_mean
+        self.init_amplitude_width = init_amplitude_width
+        self.init_spread_mean = init_spread_mean
+        self.init_spread_width = init_spread_width
+        self.reset()
+
+    def select_init_state(self, init_amplitude=None, init_spread=None):
+        """Function to select the initial state of the PDE"""
+        if init_amplitude is None:
+            random_amplitude = self.rng.uniform(
+                -0.5 * self.init_amplitude_width, 0.5 * self.init_amplitude_width
+            )
+            init_amplitude = self.init_amplitude_mean + random_amplitude
+        if init_spread is None:
+            random_spread = self.rng.uniform(
+                -0.5 * self.init_spread_width, 0.5 * self.init_spread_width
+            )
+            init_spread = self.init_spread_mean + random_spread
+        init_state = init_amplitude * np.cosh(
+            1 / init_spread * (self.domain_coordinates - 0.5 * self.domain_length)
+        ) ** (-1)
+        return init_state
 
     def step(self, action: np.ndarray[float]):
         """Run one timestep of the environment's dynamics using the agent actions and optional disturbance input.
 
         When the end of an episode is reached (``terminated or truncated``), it is necessary to call reset() to
         reset this environment's state for the next episode.
 
@@ -146,15 +163,15 @@
         disturbance = self.rng.multivariate_normal(
             np.zeros(self.n_state),
             self.process_noise_cov * np.identity(self.n_state),
         )
 
         # compute the observation
         observation = self._get_obs()
-        
+
         # compute the next state
         next_state = self.A @ self.state + self.B2 @ action + disturbance
 
         # compute the reward, which happens before updating the environment state
         # because the reward (might) depends on both the current state and the next state.
         # * In the default reward function, the dependence on the current state is
         # through the self.state attribute, which will not be updated until the next line.
@@ -209,9 +226,13 @@
         """
         pde_dict = super().get_params_asdict()
         pde_dict.pop("integration_time")
         extra_data = {
             "diffusivity_constant": self.diffusivity_constant,
             "convective_velocity": self.convective_velocity,
             "reaction_constant": self.reaction_constant,
+            "init_amplitude_mean": self.init_amplitude_mean,
+            "init_amplitude_width": self.init_amplitude_width,
+            "init_spread_mean": self.init_spread_mean,
+            "init_spread_width": self.init_spread_width,
         }
         return {**pde_dict, **extra_data}
```

### Comparing `controlgym-0.1.1/controlgym/envs/fisher.py` & `controlgym-1.0/controlgym/envs/burgers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,113 +1,121 @@
 import numpy as np
 from controlgym.envs import PDE
 
 
-class FisherEnv(PDE):
+class BurgersEnv(PDE):
     """
     ### Description
 
-    This environment models the Fisher (or Fisher-KPP) equation, described by:
-        du/dt =  diffusivity_constant * d^2u/dx^2
-            + reaction_constant * u(1-u)
+    This environment models the Burgers' equation, described by:
+        du/dt =  diffusivity_constant * d^2u/dx^2 - u * du/dx
 
     ### Action Space, Observation Space, Rewards, Episode Termination
 
     See parent class `PDE` defined in pde.py for details.
 
     ### Arguments
 
     ```
-    controlgym.make('fisher')
+    controlgym.make('burgers')
     ```
     optional arguments:
     [n_steps]: the number of discrete-time steps. Default is 100.
-    [domain_length]: domain length of PDE. Default is 10.0.
+    [domain_length]: domain length of PDE. Default is 1.0.
     [integration_time]: numerical integration time step. Default is 0.001.
     [sample_time]: each discrete-time step represents (ts) seconds. Default is 0.05.
     [process_noise_cov]: process noise covariance coefficient. Default is 0.0.
     [sensor_noise_cov]: sensor noise covariance coefficient. Default is 0.25.
-    [random_init_state_cov]: random initial state covariance coefficient. Default is 0.0.
     [target_state]: target state. Default is np.zeros(n_state).
-    [init_state]: initial state. Default is
-        np.sin(4 * np.pi * self.domain_coordinates / self.domain_length)
-    [diffusivity_constant]: diffusivity constant. Default is 0.0001.
-    [reaction_constant]: reaction constant. Default is 0.1.
+    [init_amplitude_mean]: mean of initial amplitude. Default is 1.
+    [init_amplitude_width]: width of initial amplitude. Default is 0.2.
+    [init_spread_mean]: mean of initial spread. Default is 0.05.
+    [init_spread_width]: width of initial spread. Default is 0.02.
+    [diffusivity_constant]: diffusivity constant. Default is 0.001.
     [n_state]: dimension of state vector. Default is 256.
     [n_observation]: dimension of observation vector. Default is 10.
     [n_action]: dimension of control vector. Default is 8.
     [control_sup_width]: control support width. Default is 0.1.
     [Q_weight]: weight of state tracking cost. Default is 1.0.
     [R_weight]: weight of control cost. Default is 1.0.
     [action_limit]: limit of action. Default is None.
     [observation_limit]: limit of observation. Default is None.
     [reward_limit]: limit of reward. Default is None.
-    [seed]: random seed. Default is 0.
+    [seed]: random seed. Default is None.
     """
 
     def __init__(
         self,
         n_steps: int = 100,
-        domain_length: float = 10.0,
+        domain_length: float = 1.0,
         integration_time: float = 0.001,
         sample_time: float = 0.05,
         process_noise_cov: float = 0.0,
         sensor_noise_cov: float = 0.25,
-        random_init_state_cov: float = 0.0,
         target_state: np.ndarray[float] = None,
-        init_state: np.ndarray[float] = None,
-        diffusivity_constant: float = 0.0001,
-        reaction_constant: float = 0.1,
+        init_amplitude_mean: float = 1.0,
+        init_amplitude_width: float = 0.2,
+        init_spread_mean: float = 0.05,
+        init_spread_width: float = 0.02,
+        diffusivity_constant: float = 0.001,
         n_state: int = 256,
         n_observation: int = 10,
         n_action: int = 8,
         control_sup_width: float = 0.1,
         Q_weight: float = 1.0,
         R_weight: float = 1.0,
         action_limit: float = None,
         observation_limit: float = None,
         reward_limit: float = None,
-        seed: int = 0,
+        seed: int = None,
     ):
         PDE.__init__(
             self,
-            id="fisher",
+            id="burgers",
             n_steps=n_steps,
             domain_length=domain_length,
             integration_time=integration_time,
             sample_time=sample_time,
             process_noise_cov=process_noise_cov,
             sensor_noise_cov=sensor_noise_cov,
-            random_init_state_cov=random_init_state_cov,
             target_state=target_state,
             n_state=n_state,
             n_observation=n_observation,
             n_action=n_action,
             control_sup_width=control_sup_width,
             Q_weight=Q_weight,
             R_weight=R_weight,
             action_limit=action_limit,
             observation_limit=observation_limit,
             reward_limit=reward_limit,
             seed=seed,
         )
 
-        if init_state is not None:
-            self.init_state = init_state
-        else:
-            self.init_state = np.sin(
-                4 * np.pi * self.domain_coordinates / self.domain_length
-            )
-        self.state = self.init_state
+        # physical parameter
         self.diffusivity_constant = diffusivity_constant
-        self.reaction_constant = reaction_constant
 
-        # compute control sup, observation matrix
-        self.control_sup = self._compute_control_sup()
-        self.C = self._compute_C()
+        # initial state parameters
+        self.init_amplitude_mean = init_amplitude_mean
+        self.init_amplitude_width = init_amplitude_width
+        self.init_spread_mean = init_spread_mean
+        self.init_spread_width = init_spread_width
+        self.reset()
+
+    def select_init_state(self, init_amplitude=None, init_spread=None):
+        """Function to select the initial state of the PDE"""
+        if init_amplitude is None:
+            random_amplitude = self.rng.uniform(-0.5 * self.init_amplitude_width, 0.5 * self.init_amplitude_width)
+            init_amplitude = self.init_amplitude_mean + random_amplitude
+        if init_spread is None:
+            random_spread = self.rng.uniform(-0.5 * self.init_spread_width, 0.5 * self.init_spread_width)
+            init_spread = self.init_spread_mean + random_spread
+        init_state = init_amplitude * np.cosh(
+            1 / init_spread * (self.domain_coordinates - 0.5 * self.domain_length)
+        ) ** (-1)
+        return init_state
 
     def _compute_fourier_linear_op(self):
         """Private function to compute the linear operator of the PDE in Fourier space.
 
         Args:
             None.
 
@@ -131,17 +139,18 @@
             # aa_state is the anti-aliased state; meaning the state evaluated in
             # physical space on a grid with 3/2 times more points
             aa_factor = 3 / 2
             aa_state = aa_factor * np.fft.irfft(
                 state_fourier, n=int(self.n_state * aa_factor)
             )
             right_hand_side = (
-                self.reaction_constant
+                -0.5j
+                * self.domain_wavenumbers
                 * (1 / aa_factor)
-                * np.fft.rfft(aa_state * (1 - aa_state))[0 : int(self.n_state / 2) + 1]
+                * np.fft.rfft(aa_state**2)[0 : int(self.n_state / 2) + 1]
             ) + (np.fft.rfft(self.control_sup, axis=0) @ action)
             return right_hand_side
 
         return fourier_nonlinear_op
 
     def get_params_asdict(self):
         """Save the extra environment parameters as a dictionary.
@@ -151,10 +160,13 @@
 
         Returns:
             a dictionary containing the parameters of the pde environment + extra parameters.
         """
         pde_dict = super().get_params_asdict()
         extra_data = {
             "diffusivity_constant": self.diffusivity_constant,
-            "reaction_constant": self.reaction_constant,
+            "init_amplitude_mean": self.init_amplitude_mean,
+            "init_amplitude_width": self.init_amplitude_width,
+            "init_spread_mean": self.init_spread_mean,
+            "init_spread_width": self.init_spread_width,
         }
         return {**pde_dict, **extra_data}
```

### Comparing `controlgym-0.1.1/controlgym/envs/ginzburg_landau.py` & `controlgym-1.0/controlgym/envs/kuramoto_sivashinsky.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,122 @@
 import numpy as np
 from controlgym.envs import PDE
 
 
-class GinzburgLandauEnv(PDE):
+class KuramotoSivashinskyEnv(PDE):
     """
     ### Description
 
-    This environment models the Ginzburg-Landau equation for non-oscillatory bifurcations,
-    described by: du/dt = u - |u|^2u + d^2u/dx^2
+    This environment models the Kuramoto–Sivashinsky equation, described by:
+        du/dt =  -d^2u/dx^2 - u * du/dx - d^4u/dx^4
 
     ### Action Space, Observation Space, Rewards, Episode Termination
 
     See parent class `PDE` defined in pde.py for details.
 
     ### Arguments
 
     ```
-    controlgym.make('ginzburg_landau')
+    controlgym.make('kuramoto_sivashinsky')
     ```
     optional arguments:
-    [n_steps]: the number of discrete-time steps. Default is 100.
-    [domain_length]: domain length of PDE. Default is 100.0.
-    [integration_time]: numerical integration time step. Default is 0.01.
-    [sample_time]: each discrete-time step represents (ts) seconds. Default is 0.1.
+    [n_steps]: the number of discrete-time steps. Default is 500.
+    [domain_length]: domain length of PDE. Default is 32 * np.pi.
+    [integration_time]: numerical integration time step. Default is 0.005.
+    [sample_time]: each discrete-time step represents (ts) seconds. Default is 0.5.
     [process_noise_cov]: process noise covariance coefficient. Default is 0.0.
     [sensor_noise_cov]: sensor noise covariance coefficient. Default is 0.25.
-    [random_init_state_cov]: random initial state covariance coefficient. Default is 0.0.
     [target_state]: target state. Default is np.zeros(n_state).
-    [init_state]: initial state. Default is
-        0.1 * np.tanh(self.domain_coordinates - self.domain_length / 3)
-        - 0.1 * np.tanh(self.domain_coordinates - 2 * self.domain_length / 3)
+    [init_amplitude_mean]: mean of initial amplitude. Default is 1.0.
+    [init_amplitude_width]: width of initial amplitude. Default is 0.2.
     [n_state]: dimension of state vector. Default is 256.
     [n_observation]: dimension of observation vector. Default is 10.
     [n_action]: dimension of control vector. Default is 8.
     [control_sup_width]: control support width. Default is 0.1.
     [Q_weight]: weight of state tracking cost. Default is 1.0.
     [R_weight]: weight of control cost. Default is 1.0.
     [action_limit]: limit of action. Default is None.
     [observation_limit]: limit of observation. Default is None.
     [reward_limit]: limit of reward. Default is None.
-    [seed]: random seed. Default is 0.
+    [seed]: random seed. Default is None.
     """
 
     def __init__(
         self,
-        n_steps: int = 100,
-        domain_length: float = 100.0,
-        integration_time: float = 0.01,
-        sample_time: float = 0.1,
+        n_steps: int = 500,
+        domain_length: float = 32 * np.pi,
+        integration_time: float = 0.005,
+        sample_time: float = 0.5,
         process_noise_cov: float = 0.0,
         sensor_noise_cov: float = 0.25,
-        random_init_state_cov: float = 0.0,
         target_state: np.ndarray[float] = None,
-        init_state: np.ndarray[float] = None,
+        init_amplitude_mean: float = 1.0,
+        init_amplitude_width: float = 0.2,
         n_state: int = 256,
         n_observation: int = 10,
         n_action: int = 8,
         control_sup_width: float = 0.1,
         Q_weight: float = 1.0,
         R_weight: float = 1.0,
         action_limit: float = None,
         observation_limit: float = None,
         reward_limit: float = None,
-        seed: int = 0,
+        seed: int = None,
     ):
         PDE.__init__(
             self,
-            id="ginzburg_landau",
+            id="kuramoto_sivashinsky",
             n_steps=n_steps,
             domain_length=domain_length,
             integration_time=integration_time,
             sample_time=sample_time,
             process_noise_cov=process_noise_cov,
             sensor_noise_cov=sensor_noise_cov,
-            random_init_state_cov=random_init_state_cov,
             target_state=target_state,
             n_state=n_state,
             n_observation=n_observation,
             n_action=n_action,
             control_sup_width=control_sup_width,
             Q_weight=Q_weight,
             R_weight=R_weight,
             action_limit=action_limit,
             observation_limit=observation_limit,
             reward_limit=reward_limit,
             seed=seed,
         )
 
-        if init_state is not None:
-            self.init_state = init_state
-        else:
-            self.init_state = 0.1 * np.tanh(
-                self.domain_coordinates - self.domain_length / 3
-            ) - 0.1 * np.tanh(self.domain_coordinates - 2 * self.domain_length / 3)
-        self.state = self.init_state
-
-        # compute control sup, observation matrix
-        self.control_sup = self._compute_control_sup()
-        self.C = self._compute_C()
+        # initial state parameters
+        self.init_amplitude_mean = init_amplitude_mean
+        self.init_amplitude_width = init_amplitude_width
+        self.reset()
+
+    def select_init_state(self, init_amplitude=None):
+        """Function to select the initial state of the PDE."""
+        if init_amplitude is None:
+            random_amplitude = self.rng.uniform(
+                -0.5 * self.init_amplitude_width, 0.5 * self.init_amplitude_width
+            )
+            init_amplitude = self.init_amplitude_mean + random_amplitude
+        init_state = (
+            init_amplitude
+            * np.cos(2 * np.pi * self.domain_coordinates / self.domain_length)
+            * np.sin(12 * np.pi * self.domain_coordinates / self.domain_length)
+        )
+        return init_state
 
     def _compute_fourier_linear_op(self):
         """Private function to compute the linear operator of the PDE in Fourier space.
 
         Args:
             None.
 
         Returns:
             Linear operator of the PDE in Fourier space.
         """
-        fourier_linear_op = 1 - self.domain_wavenumbers**2
+        fourier_linear_op = self.domain_wavenumbers**2 - self.domain_wavenumbers**4
         return fourier_linear_op
 
     def _compute_fourier_nonlinear_op(self):
         """Private function to compute the nonlinear operator of the PDE in Fourier space.
 
         Args:
             None.
@@ -125,13 +129,31 @@
             # aa_state is the anti-aliased state; meaning the state evaluated in
             # physical space on a grid with 3/2 times more points
             aa_factor = 3 / 2
             aa_state = aa_factor * np.fft.irfft(
                 state_fourier, n=int(self.n_state * aa_factor)
             )
             right_hand_side = (
-                -(1 / aa_factor)
-                * np.fft.rfft(aa_state**3)[0 : int(self.n_state / 2) + 1]
+                -0.5j
+                * self.domain_wavenumbers
+                * (1 / aa_factor)
+                * np.fft.rfft(aa_state**2)[0 : int(self.n_state / 2) + 1]
             ) + (np.fft.rfft(self.control_sup, axis=0) @ action)
             return right_hand_side
 
         return fourier_nonlinear_op
+
+    def get_params_asdict(self):
+        """Save the extra environment parameters as a dictionary.
+
+        Args:
+            None.
+
+        Returns:
+            a dictionary containing the parameters of the pde environment + extra parameters.
+        """
+        pde_dict = super().get_params_asdict()
+        extra_data = {
+            "init_amplitude_mean": self.init_amplitude_mean,
+            "init_amplitude_width": self.init_amplitude_width,
+        }
+        return {**pde_dict, **extra_data}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `controlgym-0.1.1/controlgym/envs/korteweg_de_vries.py` & `controlgym-1.0/controlgym/envs/ginzburg_landau.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,131 +1,130 @@
 import numpy as np
 from controlgym.envs import PDE
 
 
-class KortewegDeVriesEnv(PDE):
+class GinzburgLandauEnv(PDE):
     """
     ### Description
 
-    This environment models the Korteweg De Vries equation, described by:
-        du/dt =  - d^3u/dx^3 + 6u * du/dx
+    This environment models the Ginzburg-Landau equation for non-oscillatory bifurcations,
+    described by: du/dt = u - |u|^2u + d^2u/dx^2
 
     ### Action Space, Observation Space, Rewards, Episode Termination
 
     See parent class `PDE` defined in pde.py for details.
 
     ### Arguments
 
     ```
-    controlgym.make('korteweg_de_vries')
+    controlgym.make('ginzburg_landau')
     ```
     optional arguments:
     [n_steps]: the number of discrete-time steps. Default is 100.
-    [domain_length]: domain length of PDE. Default is 10.0.
-    [integration_time]: numerical integration time step. Default is 0.00001.
-    [sample_time]: each discrete-time step represents (ts) seconds. Default is 0.01.
+    [domain_length]: domain length of PDE. Default is 100.0.
+    [integration_time]: numerical integration time step. Default is 0.01.
+    [sample_time]: each discrete-time step represents (ts) seconds. Default is 0.1.
     [process_noise_cov]: process noise covariance coefficient. Default is 0.0.
     [sensor_noise_cov]: sensor noise covariance coefficient. Default is 0.25.
-    [random_init_state_cov]: random initial state covariance coefficient. Default is 0.0.
     [target_state]: target state. Default is np.zeros(n_state).
-    [init_state]: initial state. Default is
-        -12 * (3 + np.cosh(-4 * (self.domain_coordinates - 0.5 * self.domain_length))
-        + 4 * np.cosh(-2 * (self.domain_coordinates - 0.5 * self.domain_length)))
-        / (np.cosh(-3 * (self.domain_coordinates - 0.5 * self.domain_length))
-        + 3 * np.cosh(-(self.domain_coordinates - 0.5 * self.domain_length)) ** 2)
-    [n_state]: dimension of state vector. Default is 128.
+    [init_amplitude_mean]: mean of initial amplitude. Default is 0.1.
+    [init_amplitude_width]: width of initial amplitude. Default is 0.05.
+    [init_spread_mean]: mean of initial spread. Default is 20.0.
+    [init_spread_width]: width of initial spread. Default is 10.0.
+    [n_state]: dimension of state vector. Default is 256.
     [n_observation]: dimension of observation vector. Default is 10.
     [n_action]: dimension of control vector. Default is 8.
     [control_sup_width]: control support width. Default is 0.1.
     [Q_weight]: weight of state tracking cost. Default is 1.0.
     [R_weight]: weight of control cost. Default is 1.0.
     [action_limit]: limit of action. Default is None.
     [observation_limit]: limit of observation. Default is None.
     [reward_limit]: limit of reward. Default is None.
-    [seed]: random seed. Default is 0.
+    [seed]: random seed. Default is None.
     """
 
     def __init__(
         self,
         n_steps: int = 100,
-        domain_length: float = 10.0,
-        integration_time: float = 0.00001,
-        sample_time: float = 0.01,
+        domain_length: float = 100.0,
+        integration_time: float = 0.01,
+        sample_time: float = 0.1,
         process_noise_cov: float = 0.0,
         sensor_noise_cov: float = 0.25,
-        random_init_state_cov: float = 0.0,
         target_state: np.ndarray[float] = None,
-        init_state: np.ndarray[float] = None,
-        n_state: int = 128,
+        init_amplitude_mean: float = 0.1,
+        init_amplitude_width: float = 0.05,
+        init_spread_mean: float = 20.0,
+        init_spread_width: float = 10.0,
+        n_state: int = 256,
         n_observation: int = 10,
         n_action: int = 8,
         control_sup_width: float = 0.1,
         Q_weight: float = 1.0,
         R_weight: float = 1.0,
         action_limit: float = None,
         observation_limit: float = None,
         reward_limit: float = None,
-        seed: int = 0,
+        seed: int = None,
     ):
         PDE.__init__(
             self,
-            id="korteweg_de_vries",
+            id="ginzburg_landau",
             n_steps=n_steps,
             domain_length=domain_length,
             integration_time=integration_time,
             sample_time=sample_time,
             process_noise_cov=process_noise_cov,
             sensor_noise_cov=sensor_noise_cov,
-            random_init_state_cov=random_init_state_cov,
             target_state=target_state,
             n_state=n_state,
             n_observation=n_observation,
             n_action=n_action,
             control_sup_width=control_sup_width,
             Q_weight=Q_weight,
             R_weight=R_weight,
             action_limit=action_limit,
             observation_limit=observation_limit,
             reward_limit=reward_limit,
             seed=seed,
         )
 
-        if init_state is not None:
-            self.init_state = init_state
-        else:
-            self.init_state = (
-                -12
-                * (
-                    3
-                    + np.cosh(-4 * (self.domain_coordinates - 0.5 * self.domain_length))
-                    + 4
-                    * np.cosh(-2 * (self.domain_coordinates - 0.5 * self.domain_length))
-                )
-                / (
-                    np.cosh(-3 * (self.domain_coordinates - 0.5 * self.domain_length))
-                    + 3 * np.cosh(-(self.domain_coordinates - 0.5 * self.domain_length))
-                )
-                ** 2
+        # initial state parameters
+        self.init_amplitude_mean = init_amplitude_mean
+        self.init_amplitude_width = init_amplitude_width
+        self.init_spread_mean = init_spread_mean
+        self.init_spread_width = init_spread_width
+        self.reset()
+
+    def select_init_state(self, init_amplitude=None, init_spread=None):
+        """Function to select the initial state of the PDE."""
+        if init_amplitude is None:
+            random_amplitude = self.rng.uniform(-0.5 * self.init_amplitude_width, 0.5 * self.init_amplitude_width)
+            init_amplitude = self.init_amplitude_mean + random_amplitude
+        if init_spread is None:
+            random_spread = self.rng.uniform(-0.5 * self.init_spread_width, 0.5 * self.init_spread_width)
+            init_spread = self.init_spread_mean + random_spread
+        init_state = init_amplitude * (
+            np.tanh(self.domain_coordinates - self.domain_length / 2 + init_spread / 2)
+            - np.tanh(
+                self.domain_coordinates - self.domain_length / 2 - init_spread / 2
             )
-        self.state = self.init_state
-
-        # compute control sup, observation matrix
-        self.control_sup = self._compute_control_sup()
-        self.C = self._compute_C()
+        )
+        return init_state
 
     def _compute_fourier_linear_op(self):
         """Private function to compute the linear operator of the PDE in Fourier space.
 
         Args:
             None.
 
         Returns:
             Linear operator of the PDE in Fourier space.
         """
-        fourier_linear_op = 1j * self.domain_wavenumbers**3
+        fourier_linear_op = 1 - self.domain_wavenumbers**2
         return fourier_linear_op
 
     def _compute_fourier_nonlinear_op(self):
         """Private function to compute the nonlinear operator of the PDE in Fourier space.
 
         Args:
             None.
@@ -138,15 +137,31 @@
             # aa_state is the anti-aliased state; meaning the state evaluated in
             # physical space on a grid with 3/2 times more points
             aa_factor = 3 / 2
             aa_state = aa_factor * np.fft.irfft(
                 state_fourier, n=int(self.n_state * aa_factor)
             )
             right_hand_side = (
-                3j
-                * self.domain_wavenumbers
-                * (1 / aa_factor)
-                * np.fft.rfft(aa_state**2)[0 : int(self.n_state / 2) + 1]
+                -(1 / aa_factor)
+                * np.fft.rfft(aa_state**3)[0 : int(self.n_state / 2) + 1]
             ) + (np.fft.rfft(self.control_sup, axis=0) @ action)
             return right_hand_side
 
         return fourier_nonlinear_op
+
+    def get_params_asdict(self):
+        """Save the extra environment parameters as a dictionary.
+
+        Args:
+            None.
+
+        Returns:
+            a dictionary containing the parameters of the pde environment + extra parameters.
+        """
+        pde_dict = super().get_params_asdict()
+        extra_data = {
+            "init_amplitude_mean": self.init_amplitude_mean,
+            "init_amplitude_width": self.init_amplitude_width,
+            "init_spread_mean": self.init_spread_mean,
+            "init_spread_width": self.init_spread_width,
+        }
+        return {**pde_dict, **extra_data}
```

### Comparing `controlgym-0.1.1/controlgym/envs/kuramoto_sivashinsky.py` & `controlgym-1.0/controlgym/envs/korteweg_de_vries.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,120 +1,125 @@
 import numpy as np
 from controlgym.envs import PDE
 
 
-class KuramotoSivashinskyEnv(PDE):
+class KortewegDeVriesEnv(PDE):
     """
     ### Description
 
-    This environment models the Kuramoto–Sivashinsky equation, described by:
-        du/dt =  -d^2u/dx^2 - u * du/dx - d^4u/dx^4
+    This environment models the Korteweg De Vries equation, described by:
+        du/dt =  - d^3u/dx^3 + 6u * du/dx
 
     ### Action Space, Observation Space, Rewards, Episode Termination
 
     See parent class `PDE` defined in pde.py for details.
 
     ### Arguments
 
     ```
-    controlgym.make('kuramoto_sivashinsky')
+    controlgym.make('korteweg_de_vries')
     ```
     optional arguments:
-    [n_steps]: the number of discrete-time steps. Default is 500.
-    [domain_length]: domain length of PDE. Default is 32 * np.pi.
-    [integration_time]: numerical integration time step. Default is 0.005.
-    [sample_time]: each discrete-time step represents (ts) seconds. Default is 0.5.
+    [n_steps]: the number of discrete-time steps. Default is 100.
+    [domain_length]: domain length of PDE. Default is 10.0.
+    [integration_time]: numerical integration time step. Default is 0.00001.
+    [sample_time]: each discrete-time step represents (ts) seconds. Default is 0.01.
     [process_noise_cov]: process noise covariance coefficient. Default is 0.0.
     [sensor_noise_cov]: sensor noise covariance coefficient. Default is 0.25.
-    [random_init_state_cov]: random initial state covariance coefficient. Default is 0.0.
     [target_state]: target state. Default is np.zeros(n_state).
-    [init_state]: initial state. Default is
-        np.cos(2 * np.pi * self.domain_coordinates / self.domain_length)
-        * np.sin(12 * np.pi * self.domain_coordinates / self.domain_length)
-    [n_state]: dimension of state vector. Default is 256.
+    [init_amplitude_mean]: mean of initial amplitude. Default is 2.0.
+    [init_amplitude_width]: width of initial amplitude. Default is 1.0.
+    [n_state]: dimension of state vector. Default is 128.
     [n_observation]: dimension of observation vector. Default is 10.
     [n_action]: dimension of control vector. Default is 8.
     [control_sup_width]: control support width. Default is 0.1.
     [Q_weight]: weight of state tracking cost. Default is 1.0.
     [R_weight]: weight of control cost. Default is 1.0.
     [action_limit]: limit of action. Default is None.
     [observation_limit]: limit of observation. Default is None.
     [reward_limit]: limit of reward. Default is None.
-    [seed]: random seed. Default is 0.
+    [seed]: random seed. Default is None.
     """
 
     def __init__(
         self,
-        n_steps: int = 500,
-        domain_length: float = 32 * np.pi,
-        integration_time: float = 0.005,
-        sample_time: float = 0.5,
+        n_steps: int = 100,
+        domain_length: float = 10.0,
+        integration_time: float = 0.00001,
+        sample_time: float = 0.01,
         process_noise_cov: float = 0.0,
         sensor_noise_cov: float = 0.25,
-        random_init_state_cov: float = 0.0,
         target_state: np.ndarray[float] = None,
-        init_state: np.ndarray[float] = None,
-        n_state: int = 256,
+        init_amplitude_mean: float = 2.0,
+        init_amplitude_width: float = 1.0,
+        n_state: int = 128,
         n_observation: int = 10,
         n_action: int = 8,
         control_sup_width: float = 0.1,
         Q_weight: float = 1.0,
         R_weight: float = 1.0,
         action_limit: float = None,
         observation_limit: float = None,
         reward_limit: float = None,
-        seed: int = 0,
+        seed: int = None,
     ):
         PDE.__init__(
             self,
-            id="kuramoto_sivashinsky",
+            id="korteweg_de_vries",
             n_steps=n_steps,
             domain_length=domain_length,
             integration_time=integration_time,
             sample_time=sample_time,
             process_noise_cov=process_noise_cov,
             sensor_noise_cov=sensor_noise_cov,
-            random_init_state_cov=random_init_state_cov,
             target_state=target_state,
             n_state=n_state,
             n_observation=n_observation,
             n_action=n_action,
             control_sup_width=control_sup_width,
             Q_weight=Q_weight,
             R_weight=R_weight,
             action_limit=action_limit,
             observation_limit=observation_limit,
             reward_limit=reward_limit,
             seed=seed,
         )
 
-        # the highest priority is to use the user-provided initial state
-        if init_state is not None:
-            self.init_state = init_state
-        # if the user does not provide an initial state, use the default initial state
-        else:
-            self.init_state = np.cos(
-                2 * np.pi * self.domain_coordinates / self.domain_length
-            ) * np.sin(12 * np.pi * self.domain_coordinates / self.domain_length)
-        self.state = self.init_state
-
-        # compute control sup, observation matrix
-        self.control_sup = self._compute_control_sup()
-        self.C = self._compute_C()
+        # initial state parameters
+        self.init_amplitude_mean = init_amplitude_mean
+        self.init_amplitude_width = init_amplitude_width
+        self.reset()
+
+    def select_init_state(self, init_amplitude=None):
+        """Function to select the initial state of the PDE."""
+        if init_amplitude is None:
+            random_amplitude = self.rng.uniform(-0.5 * self.init_amplitude_width, 0.5 * self.init_amplitude_width)
+            init_amplitude = self.init_amplitude_mean + random_amplitude
+        init_state = (
+            -0.5
+            * init_amplitude
+            * np.cosh(
+                0.5
+                * np.sqrt(init_amplitude)
+                * (self.domain_coordinates - 0.5 * self.domain_length)
+            )
+            ** (-2)
+        )
+        return init_state
 
     def _compute_fourier_linear_op(self):
         """Private function to compute the linear operator of the PDE in Fourier space.
 
         Args:
             None.
 
         Returns:
             Linear operator of the PDE in Fourier space.
         """
-        fourier_linear_op = self.domain_wavenumbers**2 - self.domain_wavenumbers**4
+        fourier_linear_op = 1j * self.domain_wavenumbers**3
         return fourier_linear_op
 
     def _compute_fourier_nonlinear_op(self):
         """Private function to compute the nonlinear operator of the PDE in Fourier space.
 
         Args:
             None.
@@ -127,15 +132,31 @@
             # aa_state is the anti-aliased state; meaning the state evaluated in
             # physical space on a grid with 3/2 times more points
             aa_factor = 3 / 2
             aa_state = aa_factor * np.fft.irfft(
                 state_fourier, n=int(self.n_state * aa_factor)
             )
             right_hand_side = (
-                -0.5j
+                3j
                 * self.domain_wavenumbers
                 * (1 / aa_factor)
                 * np.fft.rfft(aa_state**2)[0 : int(self.n_state / 2) + 1]
             ) + (np.fft.rfft(self.control_sup, axis=0) @ action)
             return right_hand_side
 
         return fourier_nonlinear_op
+
+    def get_params_asdict(self):
+        """Save the extra environment parameters as a dictionary.
+
+        Args:
+            None.
+
+        Returns:
+            a dictionary containing the parameters of the pde environment + extra parameters.
+        """
+        pde_dict = super().get_params_asdict()
+        extra_data = {
+            "init_amplitude_mean": self.init_amplitude_mean,
+            "init_amplitude_width": self.init_amplitude_width,
+        }
+        return {**pde_dict, **extra_data}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control.py` & `controlgym-1.0/controlgym/envs/linear_control.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
-import scipy.io as sio
-import os
 import gymnasium
+import importlib.resources as pkg_resources
+import scipy.io as sio
+from controlgym.envs import linear_control_src
 from controlgym.envs.utils import c2d
 
 class LinearControlEnv(gymnasium.Env):
     """
     ### Description
 
     This environment provides a template to model linear control problems, inheriting from gym.Env class.
@@ -46,46 +47,44 @@
     [noise_cov]: process noise covariance coefficient. Default is 0.1.
     [random_init_state_cov]: random initial state covariance coefficient. Default is 0.1.
     [init_state]: initial state. Default is 
         saved values in .mat file or np.zeros(self.n_state) + self.noise_cov * np.identity(self.n_state).
     [action_limit]: limit of action. Default is None.
     [observation_limit]: limit of observation. Default is None.
     [reward_limit]: limit of reward. Default is None.
+    [seed]: random seed. Default is None.
     """
     def __init__(
         self,
         id: str,
         n_steps: int = 1000,
         sample_time: float = 0.1,
         noise_cov: float = 0.1,
         random_init_state_cov: float = 0.1,
         init_state: np.ndarray[float] = None,
         action_limit: float = None,
         observation_limit: float = None,
         reward_limit: float = None,
-        seed: int = 0,
+        seed: int = None,
     ):
         self.n_steps = n_steps
         self.sample_time = sample_time
         self.noise_cov = noise_cov
         self.random_init_state_cov = random_init_state_cov
         self.seed = seed
         self.rng = np.random.default_rng(seed=self.seed)
 
         # setup the problem settings
         self.id = id
         self.category = "linear"
 
-        # check whether the mat file exists
-        assert os.path.exists(
-            "controlgym/envs/linear_control_src/" + self.id + ".mat"
-        ), "Enviroment id does not exist!"
-
-        # load the environment mat file
-        env = sio.loadmat("controlgym/envs/linear_control_src/" + self.id + ".mat")
+        with pkg_resources.path(linear_control_src, f"{self.id}.mat") as mat_path:
+            assert mat_path.exists(), "Environment id does not exist!"
+            # load the environment mat file
+            env = sio.loadmat(str(mat_path))
 
         # compute the discrete-time linear system parameters
         self.A, self.B1, self.B2, self.C1, self.D11, self.D12 = c2d(env["A"],
             env["B1"], env["B2"], env["C1"], env["D11"], env["D12"], self.sample_time)
         self.C = env["C"]
         self.D21 = env["D21"]
 
@@ -182,24 +181,24 @@
                 "Input disturbance has wrong dimension, the correct dimension is: "
                 + str((self.n_disturbance,))
             )
 
         # generate the observation
         observation = self._get_obs(disturbance)
         output = self._get_output(action, disturbance)
-        
+
         # step the system dynamics forward for one discrete step
         next_state = self.A @ self.state + self.B1 @ disturbance + self.B2 @ action
 
         # compute the reward, which happens before updating the environment state
         # because the reward (might) depends on both the current state and the next state.
         # * In the default reward function, the dependence on the current state is
         # through the self.state attribute, which will not be updated until the next line.
         reward = self.get_reward(action, observation, disturbance, next_state)
-        
+
         # update the environment
         self.state = next_state
 
         # terminated if the maximum episode length has been reached
         self.step_count += 1
         terminated = False if self.step_count < self.n_steps else True
         truncated = (
@@ -214,40 +213,37 @@
         """Resets the environment to an initial internal state, returning an initial observation and info.
 
         This method generates a new starting state often with some randomness to ensure that the agent explores the
         state space and learns a generalized policy about the environment. This randomness can be controlled
         with the ``seed`` parameter otherwise if the environment already has a random number generator and
         reset() is called with ``seed=None``, the RNG is not reset.
 
-        Therefore, reset() should (in the typical use case) be called with a seed right after initialization and then never again.
-
         Args:
             seed (optional int): The seed that is used to initialize the environment's PRNG (`np_random`).
             state (optional `ndarray` with shape `(n_state,)): An specific initial state to reset the environment to.
 
         Returns:
             observation (`ndarray` with shape `(n_observation,)): 
                 ** Observation is obtained based on: observation = self.C * state_t + self.D21 * disturbance
             info (dict): Contains auxillary information. In this case, it contains the state of the system to be utlized
                         for deploying state-feedback controllers. 
         """
-        super().reset(seed=seed)
+        # reset the random number generator if there is a new seed provided
+        if seed is not None:
+            self.rng = np.random.default_rng(seed=seed)
+
         # reset the system to a user-defined initial state if there is one
         if state is not None:
             assert state.shape == (
                 self.n_state,
             ), "Input state has wrong dimension, the correct dimension is: " + str(
                 (self.n_state,)
             )
             self.init_state = state
 
-        # reset the random number generator if there is a new seed provided
-        if seed is not None:
-            self.rng = np.random.default_rng(seed=seed)
-
         # add Gaussian random noise to the initial state with covaraince matrix
         # being self.random_init_state_cov * I
         self.state = self.rng.multivariate_normal(
             self.init_state,
             self.random_init_state_cov * np.identity(self.n_state),
         )
 
@@ -324,19 +320,24 @@
 
         Args:
             None.
 
         Returns:
             a dictionary containing the parameters of the environment
         """
-        return {
+        env_params = {
             "id": self.id,
             "n_steps": self.n_steps,
             "sample_time": self.sample_time,
             "noise_cov": self.noise_cov,
             "random_init_state_cov": self.random_init_state_cov,
             "init_state": self.init_state,
-            "seed": self.seed,
             "action_limit": self.action_limit,
             "observation_limit": self.observation_limit,
             "reward_limit": self.reward_limit,
-        }
+        }
+
+        # Conditionally add "seed" if it's not None
+        if self.seed is not None:
+            env_params["seed"] = self.seed
+
+        return env_params
```

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/ac1.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/ac1.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/ac10.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/ac10.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/ac2.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/ac2.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/ac3.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/ac3.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/ac4.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/ac4.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/ac5.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/ac5.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/ac6.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/ac6.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/ac7.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/ac7.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/ac8.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/ac8.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/ac9.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/ac9.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/bdt1.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/bdt1.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/bdt2.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/bdt2.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/cbm.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/cbm.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/cdp.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/cdp.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/cm1.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/cm1.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/cm2.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/cm2.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/cm3.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/cm3.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/cm4.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/cm4.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/cm5.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/cm5.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/dis1.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/dis1.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/dis2.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/dis2.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/dlr.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/dlr.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/he1.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/he1.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/he2.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/he2.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/he3.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/he3.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/he4.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/he4.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/he5.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/he5.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/he6.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/he6.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/iss.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/iss.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/je1.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/je1.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/je2.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/je2.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/lah.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/lah.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/pas.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/pas.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/psm.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/psm.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/rea.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/rea.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/toy.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/toy.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/linear_control_src/umv.mat` & `controlgym-1.0/controlgym/envs/linear_control_src/umv.mat`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/pde.py` & `controlgym-1.0/controlgym/envs/pde.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         id: str,
         n_steps: int,
         domain_length: float,
         integration_time: float,
         sample_time: float,
         process_noise_cov: float,
         sensor_noise_cov: float,
-        random_init_state_cov: float,
         target_state: np.ndarray[float],
         n_state: int,
         n_observation: int,
         n_action: int,
         control_sup_width: float,
         Q_weight: float,
         R_weight: float,
@@ -75,15 +74,14 @@
         if integration_time is not None:
             assert (
                 round(self.sample_time * 1e8) % round(self.integration_time * 1e8) == 0
             ), "sample_time must be a integer multiple of integration_time."
 
         self.process_noise_cov = process_noise_cov
         self.sensor_noise_cov = sensor_noise_cov
-        self.random_init_state_cov = random_init_state_cov
 
         self.seed = seed
         self.rng = np.random.default_rng(seed=self.seed)
 
         self.n_state = n_state
         # check whether the n_state is even
         assert self.n_state % 2 == 0, "n_state must be even."
@@ -104,14 +102,18 @@
         self.domain_coordinates = np.linspace(
             0, self.domain_length - (self.domain_length / self.n_state), self.n_state
         )
         self.domain_wavenumbers = (
             np.fft.rfftfreq(self.n_state, self.domain_length / self.n_state) * 2 * np.pi
         )
 
+        # compute control support and observation matrix
+        self.control_sup = self._compute_control_sup()
+        self.C = self._compute_C()
+
         # set up the weighting matrices
         self.Q = Q_weight * np.identity(self.n_state)
         self.R = R_weight * np.identity(self.n_action)
 
         # set up the gym.Env attributes
         self.action_limit = np.inf if action_limit is None else action_limit
         self.observation_limit = (
@@ -227,15 +229,15 @@
                 print(
                     "Overflow encountered, choose a smaller integration_time or reduce n_state."
                 )
                 break
 
         # set the new system state
         next_state = np.fft.irfft(state_fourier) + disturbance
-       
+
         # compute the reward, which happens before updating the environment state
         # because the reward (might) depends on both the current state and the next state.
         # * In the default reward function, the dependence on the current state is
         # through the self.state attribute, which will not be updated until the next line.
         reward = self.get_reward(action, observation, disturbance, next_state)
 
         # update the environment
@@ -251,62 +253,70 @@
 
         # return the observation and stage cost
         return observation, reward, terminated, truncated, info
 
     def reset(self, seed: int = None, state: np.ndarray[float] = None):
         """Resets the environment to an initial internal state, returning an initial observation and info.
 
-        This method generates a new starting state often with some randomness to ensure that the agent explores the
+        This method generates a new starting state with some randomness to ensure that the agent explores the
         state space and learns a generalized policy about the environment. This randomness can be controlled
         with the ``seed`` parameter otherwise if the environment already has a random number generator and
         reset() is called with ``seed=None``, the RNG is not reset.
 
-        Therefore, reset() should (in the typical use case) be called with a seed right after initialization and then never again.
-
         Args:
             seed (optional int): The seed that is used to initialize the environment's PRNG (`np_random`).
             state (optional `ndarray` with shape `(n_state,)): An specific initial state to reset the environment to.
 
         Returns:
             observation (`ndarray` with shape `(n_observation,)):
                 ** observation is generated by: observation = C * state + noise,
                 where C is the observation matrix and noise is a Gaussian random vector with zero
                 mean and covariance matrix being self.sensor_noise_cov * I
             info (dict): Contains auxillary information. In this case, it contains the state of the system to be utlized
                         for deploying state-feedback controllers.
         """
-        super().reset(seed=seed)
-        # reset the system to a user-defined initial state if there is one
-        if state is not None:
+        # reset the random number generator if there is a new seed provided
+        if seed is not None:
+            self.rng = np.random.default_rng(seed=seed)
+
+        # randomly generate a state (see child classes for individual implementations)
+        if state is None:
+            state = self.select_init_state()
+        else: # check whether the input state is of the right dimension
             assert state.shape == (
                 self.n_state,
             ), "Input state has wrong dimension, the correct dimension is: " + str(
                 (self.n_state,)
             )
-            self.init_state = state
-
-        # reset the random number generator if there is a new seed provided
-        if seed is not None:
-            self.rng = np.random.default_rng(seed=seed)
-
-        # add Gaussian random noise to the initial state with covaraince matrix
-        # being self.random_init_state_cov * I
-        self.state = self.rng.multivariate_normal(
-            self.init_state,
-            self.random_init_state_cov * np.identity(self.n_state),
-        )
+        self.state = state
 
         # generate the observation
         observation = self._get_obs()
         info = {"state": self.state}
         self.step_count = 0
 
-        # return the state resetting to and the observation
         return observation, info
 
+    def set_target_state(self, state: np.ndarray[float]):
+        """Set the target state of the system
+
+        Args:
+            target_state (`ndarray` with shape `(n_state,)`): the target state of the system
+
+        Returns:
+            None.
+        """
+        # check whether the input target state is of the right dimension
+        assert state.shape == (
+            self.n_state,
+        ), "Input target state has wrong dimension, the correct dimension is: " + str(
+            (self.n_state,)
+        )
+        self.target_state = state
+
     def _get_obs(self):
         """private function to generate the observation for pdes
 
         Args:
             None.
 
         Returns:
@@ -346,15 +356,15 @@
             env = gym.make('env_id', **kwargs)
             env.get_reward = custom_get_reward.__get__(env)
         ```
         """
         reward = - float((self.state - self.target_state).T @ self.Q @ (self.state - self.target_state) 
                          + action.T @ self.R @ action)
         return reward
-    
+
     def _compute_fourier_linear_op(self):
         """
         template function to be implemented in child classes for nonlinear PDEs
         """
         raise NotImplementedError
 
     def _compute_fourier_nonlinear_op(self):
@@ -410,26 +420,31 @@
 
         Args:
             None.
 
         Returns:
             a dictionary containing the parameters of the pde environment
         """
-        return {
+        env_params =  {
             "id": self.id,
             "n_steps": self.n_steps,
             "domain_length": self.domain_length,
             "integration_time": self.integration_time,
             "sample_time": self.sample_time,
             "process_noise_cov": self.process_noise_cov,
             "sensor_noise_cov": self.sensor_noise_cov,
-            "random_init_state_cov": self.random_init_state_cov,
-            "init_state": self.init_state,
             "n_state": self.n_state,
             "n_observation": self.n_observation,
             "n_action": self.n_action,
             "control_sup_width": self.control_sup_width,
-            "seed": self.seed,
             "action_limit": self.action_limit,
             "observation_limit": self.observation_limit,
             "reward_limit": self.reward_limit,
         }
+
+        if self.seed is not None:
+            env_params["seed"] = self.seed
+
+        if self.target_state is not None:
+            env_params["target_state"] = self.target_state
+
+        return env_params
```

### Comparing `controlgym-0.1.1/controlgym/envs/registrations.py` & `controlgym-1.0/controlgym/envs/registrations.py`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/schrodinger.py` & `controlgym-1.0/controlgym/envs/schrodinger.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,112 +28,126 @@
     optional arguments:
     [n_steps]: the number of discrete-time steps. Default is 100.
     [domain_length]: domain length of PDE. Default is 1.0.
     [integration_time]: numerical integration time step. Default is None.
     [sample_time]: each discrete-time step represents (ts) seconds. Default is 0.005.
     [process_noise_cov]: process noise covariance coefficient. Default is 0.0.
     [sensor_noise_cov]: sensor noise covariance coefficient. Default is 0.25.
-    [random_init_state_cov]: random initial state covariance coefficient. Default is 0.0.
     [target_state]: target state. Default is np.zeros(n_state).
-    [init_state]: initial state. Default is
-        np.cosh(10 * (self.domain_coordinates - 1 * self.domain_length / 2)) ** (-1).
+    [init_amplitude_mean]: mean of initial amplitude. Default is 1.0.
+    [init_amplitude_width]: width of initial amplitude. Default is 0.2.
+    [init_spread_mean]: mean of initial spread. Default is 0.05.
+    [init_spread_width]: width of initial spread. Default is 0.02.
     [planck_constant]: planck constant. Default is 1.0.
     [particle_mass]: particle mass. Default is 1.0.
     [potential]: potential. Default is 0.0.
     [n_state]: dimension of state vector. Default is 256.
     [n_observation]: dimension of observation vector. Default is 10.
     [n_action]: dimension of control vector. Default is 8.
     [control_sup_width]: control support width. Default is 0.1.
     [Q_weight]: weight of state tracking cost. Default is 1.0.
     [R_weight]: weight of control cost. Default is 1.0.
     [action_limit]: limit of action. Default is None.
     [observation_limit]: limit of observation. Default is None.
     [reward_limit]: limit of reward. Default is None.
-    [seed]: random seed. Default is 0.
+    [seed]: random seed. Default is None.
     """
 
     def __init__(
         self,
         n_steps: int = 500,
         domain_length: float = 1.0,
         integration_time: float = None,  # Use analytical solution to evolve the dynamics
         sample_time: float = 0.001,
         process_noise_cov: float = 0.0,
         sensor_noise_cov: float = 0.25,
-        random_init_state_cov: float = 0.0,
         target_state: np.ndarray[float] = None,
-        init_state: np.ndarray[float] = None,
+        init_amplitude_mean: float = 1.0,
+        init_amplitude_width: float = 0.2,
+        init_spread_mean: float = 0.05,
+        init_spread_width: float = 0.02,
         planck_constant: float = 1.0,
         particle_mass: float = 1.0,
         potential: float = 0.0,
         n_state: int = 256,
         n_observation: int = 10,
         n_action: int = 8,
         control_sup_width: float = 0.1,
         Q_weight: float = 1.0,
         R_weight: float = 1.0,
         action_limit: float = None,
         observation_limit: float = None,
         reward_limit: float = None,
-        seed: int = 0,
+        seed: int = None,
     ):
+        self.n_state_half = int(n_state / 2)
         PDE.__init__(
             self,
             id="schrodinger",
             n_steps=n_steps,
             domain_length=domain_length,
             integration_time=integration_time,
             sample_time=sample_time,
             process_noise_cov=process_noise_cov,
             sensor_noise_cov=sensor_noise_cov,
-            random_init_state_cov=random_init_state_cov,
             target_state=target_state,
             n_state=n_state,
             n_observation=n_observation,
             n_action=n_action,
             control_sup_width=control_sup_width,
             Q_weight=Q_weight,
             R_weight=R_weight,
             action_limit=action_limit,
             observation_limit=observation_limit,
             reward_limit=reward_limit,
             seed=seed,
         )
 
-        self.n_state_half = int(self.n_state / 2)
-
         # set up the grid parameters: since the state x comprises both the reak and
         # imaginary parts of u, the number of grid points is half the dimension of x
         self.domain_coordinates = np.linspace(
             0,
             self.domain_length - (self.domain_length / self.n_state_half),
             self.n_state_half,
         )
 
-        # the highest priority is to use the user-provided initial state
-        if init_state is not None:
-            self.init_state = init_state
-        else:
-            # if the user does not provide an initial state, use the default initial state
-            init_u = np.cosh(
-                10 * (self.domain_coordinates - 1 * self.domain_length / 2)
-            ) ** (-1)
-            init_v = np.zeros(self.n_state_half)
-            self.init_state = np.concatenate((init_u, init_v))
-        self.state = self.init_state
-
         # set up the physical parameters
         self.planck_constant = planck_constant
         self.particle_mass = particle_mass
         self.potential = potential
-
-        # compute A, B2, C
+        
+        # compute A and B2 matrices
         self.A = self._compute_A()
-        self.B2 = self._compute_control_sup()
-        self.C = self._compute_C()
+        self.B2 = self.control_sup
+
+        # initial state parameters
+        self.init_amplitude_mean = init_amplitude_mean
+        self.init_amplitude_width = init_amplitude_width
+        self.init_spread_mean = init_spread_mean
+        self.init_spread_width = init_spread_width
+        self.reset()
+
+    def select_init_state(self, init_amplitude=None, init_spread=None):
+        """Function to select the initial state of the PDE."""
+        if init_amplitude is None:
+            random_amplitude = self.rng.uniform(
+                -0.5 * self.init_amplitude_width, 0.5 * self.init_amplitude_width
+            )
+            init_amplitude = self.init_amplitude_mean + random_amplitude
+        if init_spread is None:
+            random_spread = self.rng.uniform(
+                -0.5 * self.init_spread_width, 0.5 * self.init_spread_width
+            )
+            init_spread = self.init_spread_mean + random_spread
+        init_u = init_amplitude * np.cosh(
+            1 / init_spread * (self.domain_coordinates - 1 * self.domain_length / 2)
+        ) ** (-1)
+        init_v = np.zeros(self.n_state_half)
+        init_state = np.concatenate((init_u, init_v))
+        return init_state
 
     def step(self, action: np.ndarray[float]):
         """Run one timestep of the environment's dynamics using the agent actions and optional disturbance input.
 
         When the end of an episode is reached (``terminated or truncated``), it is necessary to call reset() to
         reset this environment's state for the next episode.
 
@@ -164,27 +178,27 @@
         disturbance = self.rng.multivariate_normal(
             np.zeros(self.n_state),
             self.process_noise_cov * np.identity(self.n_state),
         )
 
         # compute the observation
         observation = self._get_obs()
-        
+
         # compute the next state
         next_state = self.A @ self.state + self.B2 @ action + disturbance
 
         # compute the reward, which happens before updating the environment state
         # because the reward (might) depends on both the current state and the next state.
         # * In the default reward function, the dependence on the current state is
         # through the self.state attribute, which will not be updated until the next line.
         reward = self.get_reward(action, observation, disturbance, next_state)
 
         # update the environment
         self.state = next_state
-        
+
         # terminated if the cost is too large
         self.step_count += 1
         terminated = False if self.step_count < self.n_steps else True
         truncated = (
             False if self.reward_range[0] <= reward <= self.reward_range[1] else True
         )
         info = {"state": self.state}
@@ -296,9 +310,13 @@
         """
         pde_dict = super().get_params_asdict()
         pde_dict.pop("integration_time")
         extra_data = {
             "planck_constant": self.planck_constant,
             "particle_mass": self.particle_mass,
             "potential": self.potential,
+            "init_amplitude_mean": self.init_amplitude_mean,
+            "init_amplitude_width": self.init_amplitude_width,
+            "init_spread_mean": self.init_spread_mean,
+            "init_spread_width": self.init_spread_width,
         }
         return {**pde_dict, **extra_data}
```

### Comparing `controlgym-0.1.1/controlgym/envs/utils.py` & `controlgym-1.0/controlgym/envs/utils.py`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/envs/wave.py` & `controlgym-1.0/controlgym/envs/wave.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,108 +23,122 @@
     optional arguments:
     [n_steps]: the number of discrete-time steps. Default is 100.
     [domain_length]: domain length of PDE. Default is 1.0.
     [integration_time]: numerical integration time step. Default is None.
     [sample_time]: each discrete-time step represents (ts) seconds. Default is 0.1.
     [process_noise_cov]: process noise covariance coefficient. Default is 0.0.
     [sensor_noise_cov]: sensor noise covariance coefficient. Default is 0.25.
-    [random_init_state_cov]: random initial state covariance coefficient. Default is 0.0.
     [target_state]: target state. Default is np.zeros(n_state).
-    [init_state]: initial state. Default is
-        np.cosh(10 * (self.domain_coordinates - 1 * self.domain_length / 2)) ** (-1).
+    [init_amplitude_mean]: mean of initial amplitude. Default is 1.0.
+    [init_amplitude_width]: width of initial amplitude. Default is 0.2.
+    [init_spread_mean]: mean of initial spread. Default is 0.05.
+    [init_spread_width]: width of initial spread. Default is 0.02.
     [wave_speed]: wave speed. Default is 0.1.
     [n_state]: dimension of state vector. Default is 200.
     [n_observation]: dimension of observation vector. Default is 10.
     [n_action]: dimension of control vector. Default is 8.
     [control_sup_width]: control support width. Default is 0.1.
     [Q_weight]: weight of state tracking cost. Default is 1.0.
     [R_weight]: weight of control cost. Default is 1.0.
     [action_limit]: limit of action. Default is None.
     [observation_limit]: limit of observation. Default is None.
     [reward_limit]: limit of reward. Default is None.
-    [seed]: random seed. Default is 0.
+    [seed]: random seed. Default is None.
     """
 
     def __init__(
         self,
         n_steps: int = 200,
         domain_length: float = 1.0,
         integration_time: float = None,  # Use analytical solution to evolve the dynamics
         sample_time: float = 0.1,
         process_noise_cov: float = 0.0,
         sensor_noise_cov: float = 0.25,
-        random_init_state_cov: float = 0.0,
         target_state: np.ndarray[float] = None,
-        init_state: np.ndarray[float] = None,
+        init_amplitude_mean: float = 1.0,
+        init_amplitude_width: float = 0.2,
+        init_spread_mean: float = 0.05,
+        init_spread_width: float = 0.02,
         wave_speed: float = 0.1,
         n_state: int = 200,
         n_observation: int = 10,
         n_action: int = 8,
         control_sup_width: float = 0.1,
         Q_weight: float = 1.0,
         R_weight: float = 1.0,
         action_limit: float = None,
         observation_limit: float = None,
         reward_limit: float = 1e15,
-        seed: int = 0,
+        seed: int = None,
     ):
+        self.n_state_half = int(n_state / 2)
         PDE.__init__(
             self,
             id="wave",
             n_steps=n_steps,
             domain_length=domain_length,
             integration_time=integration_time,
             sample_time=sample_time,
             process_noise_cov=process_noise_cov,
             sensor_noise_cov=sensor_noise_cov,
-            random_init_state_cov=random_init_state_cov,
             target_state=target_state,
             n_state=n_state,
             n_observation=n_observation,
             n_action=n_action,
             control_sup_width=control_sup_width,
             Q_weight=Q_weight,
             R_weight=R_weight,
             action_limit=action_limit,
             observation_limit=observation_limit,
             reward_limit=reward_limit,
             seed=seed,
         )
 
-        self.n_state_half = int(self.n_state / 2)
-
         # set up the grid parameters: since the state x comprises both u in
         # the wave equation and its time derivative, the number of grid
         # points is half the dimension of x
         self.domain_coordinates = np.linspace(
             0,
             self.domain_length - (self.domain_length / self.n_state_half),
             self.n_state_half,
         )
 
-        # the highest priority is to use the user-provided initial state
-        if init_state is not None:
-            self.init_state = init_state
-        else:
-            # if the user does not provide an initial state, use the default initial state
-            init_u = np.cosh(
-                10 * (self.domain_coordinates - 1 * self.domain_length / 2)
-            ) ** (-1)
-            init_v = np.zeros(self.n_state_half)
-            self.init_state = np.concatenate((init_u, init_v))
-        self.state = self.init_state
-
         # set up the wave speed
         assert wave_speed >= 0, "wave speed must be non-negative"
         self.wave_speed = wave_speed
 
-        # compute A, B2, C
+        # compute A and B2 matrices
         self.A = self._compute_A()
-        self.B2 = self._compute_control_sup()
-        self.C = self._compute_C()
+        self.B2 = self.control_sup
+
+        # initial state parameters
+        self.init_amplitude_mean = init_amplitude_mean
+        self.init_amplitude_width = init_amplitude_width
+        self.init_spread_mean = init_spread_mean
+        self.init_spread_width = init_spread_width
+        self.reset()
+
+    def select_init_state(self, init_amplitude=None, init_spread=None):
+        """Function to select the initial state of the PDE."""
+        if init_amplitude is None:
+            random_amplitude = self.rng.uniform(
+                -0.5 * self.init_amplitude_width, 0.5 * self.init_amplitude_width
+            )
+            init_amplitude = self.init_amplitude_mean + random_amplitude
+        if init_spread is None:
+            random_spread = self.rng.uniform(
+                -0.5 * self.init_spread_width, 0.5 * self.init_spread_width
+            )
+            init_spread = self.init_spread_mean + random_spread
+        init_u = init_amplitude * np.cosh(
+            1 / init_spread * (self.domain_coordinates - 1 * self.domain_length / 2)
+        ) ** (-1)
+        init_v = np.zeros(self.n_state_half)
+        init_state = np.concatenate((init_u, init_v))
+        return init_state
 
     def step(self, action: np.ndarray[float]):
         """Run one timestep of the environment's dynamics using the agent actions and optional disturbance input.
 
         When the end of an episode is reached (``terminated or truncated``), it is necessary to call reset() to
         reset this environment's state for the next episode.
 
@@ -274,9 +288,15 @@
             None.
 
         Returns:
             a dictionary containing the parameters of the pde environment + extra parameters.
         """
         pde_dict = super().get_params_asdict()
         pde_dict.pop("integration_time")
-        extra_data = {"wave_speed": self.wave_speed}
+        extra_data = {
+            "wave_speed": self.wave_speed,
+            "init_amplitude_mean": self.init_amplitude_mean,
+            "init_amplitude_width": self.init_amplitude_width,
+            "init_spread_mean": self.init_spread_mean,
+            "init_spread_width": self.init_spread_width,
+        }
         return {**pde_dict, **extra_data}
```

### Comparing `controlgym-0.1.1/controlgym/helpers/data_processing.py` & `controlgym-1.0/controlgym/helpers/data_processing.py`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/controlgym/helpers/plotting.py` & `controlgym-1.0/controlgym/helpers/plotting.py`

 * *Files identical despite different names*

### Comparing `controlgym-0.1.1/pyproject.toml` & `controlgym-1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "controlgym"
-version = "0.1.1"
+version = "1.0"
 description = "large-scale safety-critical control benchmarks for reinforcement learning algorithms"
 authors = ["Xiangyuan Zhang <xz7@illinois.edu>", 
             "Weichao Mao <weichao2@illinois.edu>",
             "Saviz Mowlavi <mowlavi@merl.com>"]
 license = "MIT"
 readme = "README.md"
+include = ["controlgym/envs/linear_control_src/*.mat"]
 exclude = ["examples.ipynb", "requirements.txt", "setup.py", "**/.conda", "**/.vscode"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.23.5"
 scipy = "^1.11.1"
 matplotlib = "^3.7.1"
 torch = "^2.0.1"
 gymnasium = "0.29.1"
 
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `controlgym-0.1.1/PKG-INFO` & `controlgym-1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: controlgym
-Version: 0.1.1
+Version: 1.0
 Summary: large-scale safety-critical control benchmarks for reinforcement learning algorithms
 License: MIT
 Author: Xiangyuan Zhang
 Author-email: xz7@illinois.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # controlgym
 
 ## Description
-`Controlgym` provides 36 safety-critical industrial control environments and 10 infinite-dimensional PDE-based control problems with continuous, unbounded action and observation spaces that are inspired by real-world applications. This project supports the Learning for Dynamics & Control (L4DC) community, focusing on vital issues: convergence of reinforcement learning (RL) algorithms in policy development, stability, safety, and robustness of learning-based controllers, and the scalability of RL algorithms to high and potentially infinite-dimensional systems. We provide a detailed description of `controlgym` in [this paper](https://arxiv.org/abs/2311.18736).
+`Controlgym` provides 36 industrial control environments and 10 infinite-dimensional PDE-based control problems with continuous, unbounded action and observation spaces that are inspired by real-world applications. This project supports the Learning for Dynamics & Control (L4DC) community, focusing on vital issues: convergence of reinforcement learning (RL) algorithms in policy development, stability, and robustness of learning-based controllers, and the scalability of RL algorithms to high and potentially infinite-dimensional systems. We provide a detailed description of `controlgym` in [this paper](https://arxiv.org/abs/2311.18736).
 
 <p align="center">
   <img src="figures/gallery.jpeg" alt="" width="700px">
 </p>
 
 
 
@@ -96,17 +96,17 @@
 </details>
 
 
 ## Getting Started
 Check out our code examples in this [Jupyter notebook file](./examples.ipynb).
 
 ## Reference
-- Zhang, X., Mao, W., Mowlavi, S., Benosman, M., & Başar, T. (2023). [Controlgym: Large-Scale Safety-Critical Control Environments for Benchmarking Reinforcement Learning Algorithms.](https://arxiv.org/abs/2311.18736) arXiv preprint arXiv:2311.18736.
+- Zhang, X., Mao, W., Mowlavi, S., Benosman, M., & Başar, T. (2023). [Controlgym: Large-Scale Control Environments for Benchmarking Reinforcement Learning Algorithms.](https://arxiv.org/abs/2311.18736) arXiv preprint arXiv:2311.18736.
   
 ```bibtex
 @article{zhang2023controlgym,
-    title = {Controlgym: Large-Scale Safety-Critical Control Environments for Benchmarking Reinforcement Learning Algorithms},
+    title = {Controlgym: Large-Scale Control Environments for Benchmarking Reinforcement Learning Algorithms},
     author = {Zhang, Xiangyuan and Mao, Weichao and Mowlavi, Saviz and Benosman, Mouhacine and Ba{\c{s}}ar, Tamer},
     journal = {arXiv preprint arXiv:2311.18736},
     year = {2023}
 }
 ```
```

