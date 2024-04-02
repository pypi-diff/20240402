# Comparing `tmp/MohuPy-0.2.6.tar.gz` & `tmp/MohuPy-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MohuPy-0.2.6.tar", last modified: Sun Mar 24 04:42:01 2024, max compression
+gzip compressed data, was "MohuPy-0.2.7.tar", last modified: Tue Apr  2 03:46:20 2024, max compression
```

## Comparing `MohuPy-0.2.6.tar` & `MohuPy-0.2.7.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.108206 MohuPy-0.2.6/
--rw-r--r--   0 yibow      (501) staff       (20)     1061 2023-01-29 07:30:33.000000 MohuPy-0.2.6/LICENSE
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.107521 MohuPy-0.2.6/MohuPy.egg-info/
--rw-r--r--   0 yibow      (501) staff       (20)     4175 2024-03-24 04:42:01.000000 MohuPy-0.2.6/MohuPy.egg-info/PKG-INFO
--rw-r--r--   0 yibow      (501) staff       (20)     1477 2024-03-24 04:42:01.000000 MohuPy-0.2.6/MohuPy.egg-info/SOURCES.txt
--rw-r--r--   0 yibow      (501) staff       (20)        1 2024-03-24 04:42:01.000000 MohuPy-0.2.6/MohuPy.egg-info/dependency_links.txt
--rw-r--r--   0 yibow      (501) staff       (20)       39 2024-03-24 04:42:01.000000 MohuPy-0.2.6/MohuPy.egg-info/requires.txt
--rw-r--r--   0 yibow      (501) staff       (20)        7 2024-03-24 04:42:01.000000 MohuPy-0.2.6/MohuPy.egg-info/top_level.txt
--rw-r--r--   0 yibow      (501) staff       (20)     4175 2024-03-24 04:42:01.107951 MohuPy-0.2.6/PKG-INFO
--rw-r--r--   0 yibow      (501) staff       (20)     3581 2023-11-29 10:30:24.000000 MohuPy-0.2.6/README.md
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.093779 MohuPy-0.2.6/mohupy/
--rw-r--r--   0 yibow      (501) staff       (20)      956 2023-11-29 08:28:50.000000 MohuPy-0.2.6/mohupy/__init__.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.094309 MohuPy-0.2.6/mohupy/config/
--rw-r--r--   0 yibow      (501) staff       (20)      460 2023-11-29 07:37:14.000000 MohuPy-0.2.6/mohupy/config/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)      268 2023-11-29 07:40:11.000000 MohuPy-0.2.6/mohupy/config/tnorms.py
--rw-r--r--   0 yibow      (501) staff       (20)     1233 2023-11-28 09:03:14.000000 MohuPy-0.2.6/mohupy/constant.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.097315 MohuPy-0.2.6/mohupy/core/
--rw-r--r--   0 yibow      (501) staff       (20)     1312 2023-12-23 07:04:59.000000 MohuPy-0.2.6/mohupy/core/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)     2835 2023-11-29 07:28:40.000000 MohuPy-0.2.6/mohupy/core/__nums_operation.py
--rw-r--r--   0 yibow      (501) staff       (20)     4408 2023-12-23 06:58:06.000000 MohuPy-0.2.6/mohupy/core/array.py
--rw-r--r--   0 yibow      (501) staff       (20)     8332 2023-12-19 06:12:31.000000 MohuPy-0.2.6/mohupy/core/attributes.py
--rw-r--r--   0 yibow      (501) staff       (20)      441 2023-11-28 07:07:28.000000 MohuPy-0.2.6/mohupy/core/base.py
--rw-r--r--   0 yibow      (501) staff       (20)    28339 2023-12-23 06:58:43.000000 MohuPy-0.2.6/mohupy/core/function.py
--rw-r--r--   0 yibow      (501) staff       (20)     2213 2023-12-23 07:05:05.000000 MohuPy-0.2.6/mohupy/core/fuzzfunc.py
--rw-r--r--   0 yibow      (501) staff       (20)     2188 2023-12-23 06:35:06.000000 MohuPy-0.2.6/mohupy/core/nums.py
--rw-r--r--   0 yibow      (501) staff       (20)    20508 2024-01-17 16:54:16.000000 MohuPy-0.2.6/mohupy/core/operation.py
--rw-r--r--   0 yibow      (501) staff       (20)     1175 2023-12-23 06:37:21.000000 MohuPy-0.2.6/mohupy/core/package.py
--rw-r--r--   0 yibow      (501) staff       (20)     1724 2023-11-28 07:11:34.000000 MohuPy-0.2.6/mohupy/core/regedit.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.098008 MohuPy-0.2.6/mohupy/function/
--rw-r--r--   0 yibow      (501) staff       (20)      420 2023-09-23 06:14:48.000000 MohuPy-0.2.6/mohupy/function/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)     9147 2023-10-01 12:31:19.000000 MohuPy-0.2.6/mohupy/function/func.py
--rw-r--r--   0 yibow      (501) staff       (20)     4505 2023-10-01 12:31:54.000000 MohuPy-0.2.6/mohupy/function/mem_func.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.098282 MohuPy-0.2.6/mohupy/generator/
--rw-r--r--   0 yibow      (501) staff       (20)      163 2023-10-01 08:16:28.000000 MohuPy-0.2.6/mohupy/generator/__init__.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.100349 MohuPy-0.2.6/mohupy/lib/
--rw-r--r--   0 yibow      (501) staff       (20)     1345 2023-12-02 09:45:46.000000 MohuPy-0.2.6/mohupy/lib/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)      491 2023-11-28 10:38:49.000000 MohuPy-0.2.6/mohupy/lib/base.py
--rw-r--r--   0 yibow      (501) staff       (20)     3710 2023-12-23 07:16:40.000000 MohuPy-0.2.6/mohupy/lib/construct.py
--rw-r--r--   0 yibow      (501) staff       (20)     4771 2024-03-24 04:05:54.000000 MohuPy-0.2.6/mohupy/lib/io.py
--rw-r--r--   0 yibow      (501) staff       (20)     2405 2023-11-29 05:15:05.000000 MohuPy-0.2.6/mohupy/lib/measure.py
--rw-r--r--   0 yibow      (501) staff       (20)     2946 2023-11-28 11:47:35.000000 MohuPy-0.2.6/mohupy/lib/other.py
--rw-r--r--   0 yibow      (501) staff       (20)     2226 2024-01-23 13:45:06.000000 MohuPy-0.2.6/mohupy/lib/plotlib.py
--rw-r--r--   0 yibow      (501) staff       (20)      430 2023-11-29 05:15:05.000000 MohuPy-0.2.6/mohupy/lib/string.py
--rw-r--r--   0 yibow      (501) staff       (20)     4769 2023-12-11 07:01:28.000000 MohuPy-0.2.6/mohupy/lib/utils.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.101256 MohuPy-0.2.6/mohupy/math/
--rw-r--r--   0 yibow      (501) staff       (20)      318 2023-11-29 08:28:01.000000 MohuPy-0.2.6/mohupy/math/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)      494 2023-11-29 05:40:06.000000 MohuPy-0.2.6/mohupy/math/base.py
--rw-r--r--   0 yibow      (501) staff       (20)     3116 2023-11-29 08:26:50.000000 MohuPy-0.2.6/mohupy/math/norms.py
--rw-r--r--   0 yibow      (501) staff       (20)     8366 2023-11-29 08:27:39.000000 MohuPy-0.2.6/mohupy/math/product.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.102717 MohuPy-0.2.6/mohupy/measure/
--rw-r--r--   0 yibow      (501) staff       (20)      710 2023-11-29 05:09:11.000000 MohuPy-0.2.6/mohupy/measure/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)    11003 2023-11-28 12:01:09.000000 MohuPy-0.2.6/mohupy/measure/fuzzmeas.py
--rw-r--r--   0 yibow      (501) staff       (20)     5312 2023-10-01 12:26:14.000000 MohuPy-0.2.6/mohupy/measure/hasse.py
--rw-r--r--   0 yibow      (501) staff       (20)     6189 2024-02-11 15:16:13.000000 MohuPy-0.2.6/mohupy/measure/indices.py
--rw-r--r--   0 yibow      (501) staff       (20)     6566 2023-12-01 08:41:17.000000 MohuPy-0.2.6/mohupy/measure/integral.py
--rw-r--r--   0 yibow      (501) staff       (20)     5549 2023-11-25 10:47:47.000000 MohuPy-0.2.6/mohupy/measure/utils.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.103442 MohuPy-0.2.6/mohupy/random/
--rw-r--r--   0 yibow      (501) staff       (20)      311 2023-11-29 10:29:10.000000 MohuPy-0.2.6/mohupy/random/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)      489 2023-11-29 05:39:47.000000 MohuPy-0.2.6/mohupy/random/base.py
--rw-r--r--   0 yibow      (501) staff       (20)     4152 2024-02-07 12:43:53.000000 MohuPy-0.2.6/mohupy/random/rand.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.105567 MohuPy-0.2.6/mohupy/regedit/
--rw-r--r--   0 yibow      (501) staff       (20)     1076 2023-11-29 07:34:01.000000 MohuPy-0.2.6/mohupy/regedit/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)     4218 2023-11-30 04:27:07.000000 MohuPy-0.2.6/mohupy/regedit/algebraic_operation.py
--rw-r--r--   0 yibow      (501) staff       (20)     3327 2023-12-23 07:12:54.000000 MohuPy-0.2.6/mohupy/regedit/construct.py
--rw-r--r--   0 yibow      (501) staff       (20)     4539 2023-11-29 05:10:14.000000 MohuPy-0.2.6/mohupy/regedit/distance.py
--rw-r--r--   0 yibow      (501) staff       (20)     6913 2023-11-29 09:13:44.000000 MohuPy-0.2.6/mohupy/regedit/plotlib.py
--rw-r--r--   0 yibow      (501) staff       (20)     2656 2023-12-20 06:46:43.000000 MohuPy-0.2.6/mohupy/regedit/random.py
--rw-r--r--   0 yibow      (501) staff       (20)     2730 2024-03-24 03:56:45.000000 MohuPy-0.2.6/mohupy/regedit/str2num.py
--rw-r--r--   0 yibow      (501) staff       (20)      740 2023-11-29 08:36:20.000000 MohuPy-0.2.6/mohupy/runtime.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.106684 MohuPy-0.2.6/mohupy/src/
--rw-r--r--   0 yibow      (501) staff       (20)      163 2023-11-29 05:46:37.000000 MohuPy-0.2.6/mohupy/src/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)     4050 2023-11-29 06:59:55.000000 MohuPy-0.2.6/mohupy/src/algebraic.py
--rw-r--r--   0 yibow      (501) staff       (20)      495 2023-11-29 06:04:46.000000 MohuPy-0.2.6/mohupy/src/base.py
--rw-r--r--   0 yibow      (501) staff       (20)     1216 2023-11-29 06:17:55.000000 MohuPy-0.2.6/mohupy/src/einstein.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.106914 MohuPy-0.2.6/mohupy/utils/
--rw-r--r--   0 yibow      (501) staff       (20)      163 2023-11-28 12:06:14.000000 MohuPy-0.2.6/mohupy/utils/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)       38 2024-03-24 04:42:01.108250 MohuPy-0.2.6/setup.cfg
--rw-r--r--   0 yibow      (501) staff       (20)      900 2024-02-13 17:46:21.000000 MohuPy-0.2.6/setup.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-03-24 04:42:01.107156 MohuPy-0.2.6/test/
--rw-r--r--   0 yibow      (501) staff       (20)      223 2023-12-19 12:55:05.000000 MohuPy-0.2.6/test/test.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.111111 MohuPy-0.2.7/
+-rw-r--r--   0 yibow      (501) staff       (20)     1061 2023-01-29 07:30:33.000000 MohuPy-0.2.7/LICENSE
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.110593 MohuPy-0.2.7/MohuPy.egg-info/
+-rw-r--r--   0 yibow      (501) staff       (20)     4175 2024-04-02 03:46:20.000000 MohuPy-0.2.7/MohuPy.egg-info/PKG-INFO
+-rw-r--r--   0 yibow      (501) staff       (20)     1477 2024-04-02 03:46:20.000000 MohuPy-0.2.7/MohuPy.egg-info/SOURCES.txt
+-rw-r--r--   0 yibow      (501) staff       (20)        1 2024-04-02 03:46:20.000000 MohuPy-0.2.7/MohuPy.egg-info/dependency_links.txt
+-rw-r--r--   0 yibow      (501) staff       (20)       39 2024-04-02 03:46:20.000000 MohuPy-0.2.7/MohuPy.egg-info/requires.txt
+-rw-r--r--   0 yibow      (501) staff       (20)        7 2024-04-02 03:46:20.000000 MohuPy-0.2.7/MohuPy.egg-info/top_level.txt
+-rw-r--r--   0 yibow      (501) staff       (20)     4175 2024-04-02 03:46:20.110877 MohuPy-0.2.7/PKG-INFO
+-rw-r--r--   0 yibow      (501) staff       (20)     3581 2023-11-29 10:30:24.000000 MohuPy-0.2.7/README.md
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.095346 MohuPy-0.2.7/mohupy/
+-rw-r--r--   0 yibow      (501) staff       (20)      956 2023-11-29 08:28:50.000000 MohuPy-0.2.7/mohupy/__init__.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.096115 MohuPy-0.2.7/mohupy/config/
+-rw-r--r--   0 yibow      (501) staff       (20)      460 2023-11-29 07:37:14.000000 MohuPy-0.2.7/mohupy/config/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      268 2023-11-29 07:40:11.000000 MohuPy-0.2.7/mohupy/config/tnorms.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1233 2023-11-28 09:03:14.000000 MohuPy-0.2.7/mohupy/constant.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.099976 MohuPy-0.2.7/mohupy/core/
+-rw-r--r--   0 yibow      (501) staff       (20)     1312 2023-12-23 07:04:59.000000 MohuPy-0.2.7/mohupy/core/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2835 2023-11-29 07:28:40.000000 MohuPy-0.2.7/mohupy/core/__nums_operation.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4408 2023-12-23 06:58:06.000000 MohuPy-0.2.7/mohupy/core/array.py
+-rw-r--r--   0 yibow      (501) staff       (20)     8332 2023-12-19 06:12:31.000000 MohuPy-0.2.7/mohupy/core/attributes.py
+-rw-r--r--   0 yibow      (501) staff       (20)      441 2023-11-28 07:07:28.000000 MohuPy-0.2.7/mohupy/core/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)    28339 2024-04-02 03:41:55.000000 MohuPy-0.2.7/mohupy/core/function.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2213 2023-12-23 07:05:05.000000 MohuPy-0.2.7/mohupy/core/fuzzfunc.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2188 2023-12-23 06:35:06.000000 MohuPy-0.2.7/mohupy/core/nums.py
+-rw-r--r--   0 yibow      (501) staff       (20)    20508 2024-01-17 16:54:16.000000 MohuPy-0.2.7/mohupy/core/operation.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1175 2023-12-23 06:37:21.000000 MohuPy-0.2.7/mohupy/core/package.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1724 2023-11-28 07:11:34.000000 MohuPy-0.2.7/mohupy/core/regedit.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.100710 MohuPy-0.2.7/mohupy/function/
+-rw-r--r--   0 yibow      (501) staff       (20)      420 2023-09-23 06:14:48.000000 MohuPy-0.2.7/mohupy/function/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     9147 2023-10-01 12:31:19.000000 MohuPy-0.2.7/mohupy/function/func.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4505 2023-10-01 12:31:54.000000 MohuPy-0.2.7/mohupy/function/mem_func.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.100962 MohuPy-0.2.7/mohupy/generator/
+-rw-r--r--   0 yibow      (501) staff       (20)      163 2023-10-01 08:16:28.000000 MohuPy-0.2.7/mohupy/generator/__init__.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.103392 MohuPy-0.2.7/mohupy/lib/
+-rw-r--r--   0 yibow      (501) staff       (20)     1345 2023-12-02 09:45:46.000000 MohuPy-0.2.7/mohupy/lib/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      491 2023-11-28 10:38:49.000000 MohuPy-0.2.7/mohupy/lib/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)     3710 2023-12-23 07:16:40.000000 MohuPy-0.2.7/mohupy/lib/construct.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4771 2024-03-24 04:05:54.000000 MohuPy-0.2.7/mohupy/lib/io.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2405 2023-11-29 05:15:05.000000 MohuPy-0.2.7/mohupy/lib/measure.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2946 2023-11-28 11:47:35.000000 MohuPy-0.2.7/mohupy/lib/other.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2226 2024-01-23 13:45:06.000000 MohuPy-0.2.7/mohupy/lib/plotlib.py
+-rw-r--r--   0 yibow      (501) staff       (20)      430 2023-11-29 05:15:05.000000 MohuPy-0.2.7/mohupy/lib/string.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4769 2023-12-11 07:01:28.000000 MohuPy-0.2.7/mohupy/lib/utils.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.104326 MohuPy-0.2.7/mohupy/math/
+-rw-r--r--   0 yibow      (501) staff       (20)      318 2023-11-29 08:28:01.000000 MohuPy-0.2.7/mohupy/math/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      494 2023-11-29 05:40:06.000000 MohuPy-0.2.7/mohupy/math/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)     3116 2023-11-29 08:26:50.000000 MohuPy-0.2.7/mohupy/math/norms.py
+-rw-r--r--   0 yibow      (501) staff       (20)     8366 2023-11-29 08:27:39.000000 MohuPy-0.2.7/mohupy/math/product.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.105769 MohuPy-0.2.7/mohupy/measure/
+-rw-r--r--   0 yibow      (501) staff       (20)      710 2023-11-29 05:09:11.000000 MohuPy-0.2.7/mohupy/measure/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)    11003 2023-11-28 12:01:09.000000 MohuPy-0.2.7/mohupy/measure/fuzzmeas.py
+-rw-r--r--   0 yibow      (501) staff       (20)     5312 2023-10-01 12:26:14.000000 MohuPy-0.2.7/mohupy/measure/hasse.py
+-rw-r--r--   0 yibow      (501) staff       (20)     6189 2024-04-02 03:39:44.000000 MohuPy-0.2.7/mohupy/measure/indices.py
+-rw-r--r--   0 yibow      (501) staff       (20)     6566 2023-12-01 08:41:17.000000 MohuPy-0.2.7/mohupy/measure/integral.py
+-rw-r--r--   0 yibow      (501) staff       (20)     5549 2023-11-25 10:47:47.000000 MohuPy-0.2.7/mohupy/measure/utils.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.106511 MohuPy-0.2.7/mohupy/random/
+-rw-r--r--   0 yibow      (501) staff       (20)      311 2023-11-29 10:29:10.000000 MohuPy-0.2.7/mohupy/random/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      489 2023-11-29 05:39:47.000000 MohuPy-0.2.7/mohupy/random/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4235 2024-03-26 08:29:32.000000 MohuPy-0.2.7/mohupy/random/rand.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.108445 MohuPy-0.2.7/mohupy/regedit/
+-rw-r--r--   0 yibow      (501) staff       (20)     1076 2023-11-29 07:34:01.000000 MohuPy-0.2.7/mohupy/regedit/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4218 2023-11-30 04:27:07.000000 MohuPy-0.2.7/mohupy/regedit/algebraic_operation.py
+-rw-r--r--   0 yibow      (501) staff       (20)     3327 2023-12-23 07:12:54.000000 MohuPy-0.2.7/mohupy/regedit/construct.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4539 2023-11-29 05:10:14.000000 MohuPy-0.2.7/mohupy/regedit/distance.py
+-rw-r--r--   0 yibow      (501) staff       (20)     6913 2023-11-29 09:13:44.000000 MohuPy-0.2.7/mohupy/regedit/plotlib.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2656 2024-03-26 08:25:56.000000 MohuPy-0.2.7/mohupy/regedit/random.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2730 2024-03-24 03:56:45.000000 MohuPy-0.2.7/mohupy/regedit/str2num.py
+-rw-r--r--   0 yibow      (501) staff       (20)      740 2023-11-29 08:36:20.000000 MohuPy-0.2.7/mohupy/runtime.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.109417 MohuPy-0.2.7/mohupy/src/
+-rw-r--r--   0 yibow      (501) staff       (20)      163 2023-11-29 05:46:37.000000 MohuPy-0.2.7/mohupy/src/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4050 2023-11-29 06:59:55.000000 MohuPy-0.2.7/mohupy/src/algebraic.py
+-rw-r--r--   0 yibow      (501) staff       (20)      495 2023-11-29 06:04:46.000000 MohuPy-0.2.7/mohupy/src/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1216 2023-11-29 06:17:55.000000 MohuPy-0.2.7/mohupy/src/einstein.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.109703 MohuPy-0.2.7/mohupy/utils/
+-rw-r--r--   0 yibow      (501) staff       (20)      163 2023-11-28 12:06:14.000000 MohuPy-0.2.7/mohupy/utils/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)       38 2024-04-02 03:46:20.111151 MohuPy-0.2.7/setup.cfg
+-rw-r--r--   0 yibow      (501) staff       (20)      900 2024-02-13 17:46:21.000000 MohuPy-0.2.7/setup.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.110092 MohuPy-0.2.7/test/
+-rw-r--r--   0 yibow      (501) staff       (20)      223 2023-12-19 12:55:05.000000 MohuPy-0.2.7/test/test.py
```

### Comparing `MohuPy-0.2.6/LICENSE` & `MohuPy-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/MohuPy.egg-info/PKG-INFO` & `MohuPy-0.2.7/MohuPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MohuPy
-Version: 0.2.6
+Version: 0.2.7
 Summary: MohuPy is a fuzzy set calculation library, which contains fuzzy numbers, fuzzy measure, fuzzy sets and fuzzy membership functions. 
 Home-page: https://github.com/yibocat/MohuPy
 Author: Yibo Wang
 Author-email: yibocat@yeah.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `MohuPy-0.2.6/MohuPy.egg-info/SOURCES.txt` & `MohuPy-0.2.7/MohuPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/PKG-INFO` & `MohuPy-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MohuPy
-Version: 0.2.6
+Version: 0.2.7
 Summary: MohuPy is a fuzzy set calculation library, which contains fuzzy numbers, fuzzy measure, fuzzy sets and fuzzy membership functions. 
 Home-page: https://github.com/yibocat/MohuPy
 Author: Yibo Wang
 Author-email: yibocat@yeah.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `MohuPy-0.2.6/README.md` & `MohuPy-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/__init__.py` & `MohuPy-0.2.7/mohupy/__init__.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/constant.py` & `MohuPy-0.2.7/mohupy/constant.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/core/__init__.py` & `MohuPy-0.2.7/mohupy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/core/__nums_operation.py` & `MohuPy-0.2.7/mohupy/core/__nums_operation.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/core/array.py` & `MohuPy-0.2.7/mohupy/core/array.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/core/attributes.py` & `MohuPy-0.2.7/mohupy/core/attributes.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/core/function.py` & `MohuPy-0.2.7/mohupy/core/function.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/core/fuzzfunc.py` & `MohuPy-0.2.7/mohupy/core/fuzzfunc.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/core/nums.py` & `MohuPy-0.2.7/mohupy/core/nums.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/core/operation.py` & `MohuPy-0.2.7/mohupy/core/operation.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/core/package.py` & `MohuPy-0.2.7/mohupy/core/package.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/core/regedit.py` & `MohuPy-0.2.7/mohupy/core/regedit.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/function/func.py` & `MohuPy-0.2.7/mohupy/function/func.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/function/mem_func.py` & `MohuPy-0.2.7/mohupy/function/mem_func.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/lib/__init__.py` & `MohuPy-0.2.7/mohupy/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/lib/construct.py` & `MohuPy-0.2.7/mohupy/lib/construct.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/lib/io.py` & `MohuPy-0.2.7/mohupy/lib/io.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/lib/measure.py` & `MohuPy-0.2.7/mohupy/lib/measure.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/lib/other.py` & `MohuPy-0.2.7/mohupy/lib/other.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/lib/plotlib.py` & `MohuPy-0.2.7/mohupy/lib/plotlib.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/lib/utils.py` & `MohuPy-0.2.7/mohupy/lib/utils.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/math/norms.py` & `MohuPy-0.2.7/mohupy/math/norms.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/math/product.py` & `MohuPy-0.2.7/mohupy/math/product.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/measure/__init__.py` & `MohuPy-0.2.7/mohupy/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/measure/fuzzmeas.py` & `MohuPy-0.2.7/mohupy/measure/fuzzmeas.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/measure/hasse.py` & `MohuPy-0.2.7/mohupy/measure/hasse.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/measure/indices.py` & `MohuPy-0.2.7/mohupy/measure/indices.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         --------
             1.  In [1]: banzhaf([0.4,0.25,0.37,0.2], mp.lambda_meas, [0.4,0.25,0.37,0.2])
                 Out[1]: [0.17701811 0.10677004 0.16256442 0.08443251]
             2.  In [2]: mp.banzhaf([0.4,0.25,0.37], mp.lambda_meas, [0.4,0.25,0.37,0.2])
                 Out[2]: [0.0925856  0.05584383 0.0850259 ]
     """
     n = len(*args)
-    coef = 1/(2**n - 1)
+    coef = 1/2**(n - 1)
     ban = np.array([])
 
     from .utils import subsets
     for x in e:
         ts = np.array([])
         for sub in subsets(np.setdiff1d(e, x)):
             ts = np.append(ts, coef * deriv(x, sub, func, *args))
```

### Comparing `MohuPy-0.2.6/mohupy/measure/integral.py` & `MohuPy-0.2.7/mohupy/measure/integral.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/measure/utils.py` & `MohuPy-0.2.7/mohupy/measure/utils.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/random/rand.py` & `MohuPy-0.2.7/mohupy/random/rand.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #  Copyright (c) yibocat 2023 All Rights Reserved
 #  Python: 3.10.9
 #  Date: 2023/10/16 下午8:22
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
+from typing import Union
 
 from .base import Random
 
 import numpy as np
 
 from ..core import Fuzzarray, Fuzznum
 
@@ -110,15 +111,15 @@
         """
         if len(n) == 0:
             return randnum(q, mtype, minnum=self.minnum, maxnum=self.maxnum)
         else:
             return randset(q, mtype, *n, minnum=self.minnum, maxnum=self.maxnum)
 
 
-def rand(q: int, mtype: str, *n, minnum=1, maxnum=5):
+def rand(q: int, mtype: str, *n, minnum=1, maxnum=5) -> Union[Fuzzarray, Fuzznum]:
     return Rand(minnum, maxnum)(q, mtype, *n)
 
 
 class Choice(Random):
     def function(self, f, n, replace):
         """
             Randomly select a fuzzy number
@@ -146,13 +147,13 @@
                 newset = Fuzzarray(f.qrung, f.mtype)
                 newset.array = np.random.choice(f.array, size=n, replace=replace)
                 return newset
         else:
             return np.random.choice(f.array.flatten())
 
 
-def choice(f, size: (int, tuple[int], list[int]) = None, replace=False):
+def choice(f, size: (int, tuple[int], list[int]) = None, replace=False) -> Union[Fuzzarray, Fuzznum]:
     return Choice()(f, size, replace)
 
 
 def seed(x):
     np.random.seed(x)
```

### Comparing `MohuPy-0.2.6/mohupy/regedit/__init__.py` & `MohuPy-0.2.7/mohupy/regedit/__init__.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/regedit/algebraic_operation.py` & `MohuPy-0.2.7/mohupy/regedit/algebraic_operation.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/regedit/construct.py` & `MohuPy-0.2.7/mohupy/regedit/construct.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/regedit/distance.py` & `MohuPy-0.2.7/mohupy/regedit/distance.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/regedit/plotlib.py` & `MohuPy-0.2.7/mohupy/regedit/plotlib.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/regedit/random.py` & `MohuPy-0.2.7/mohupy/regedit/random.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/regedit/str2num.py` & `MohuPy-0.2.7/mohupy/regedit/str2num.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/runtime.py` & `MohuPy-0.2.7/mohupy/runtime.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/src/algebraic.py` & `MohuPy-0.2.7/mohupy/src/algebraic.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/mohupy/src/einstein.py` & `MohuPy-0.2.7/mohupy/src/einstein.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.6/setup.py` & `MohuPy-0.2.7/setup.py`

 * *Files identical despite different names*

