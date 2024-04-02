# Comparing `tmp/kss-5.1.0.tar.gz` & `tmp/kss-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kss-5.1.0.tar", last modified: Sun Mar 31 21:19:05 2024, max compression
+gzip compressed data, was "kss-5.2.0.tar", last modified: Mon Apr  1 23:54:54 2024, max compression
```

## Comparing `kss-5.1.0.tar` & `kss-5.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-03-31 21:19:05.572053 kss-5.1.0/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1559 2023-05-16 17:34:32.000000 kss-5.1.0/LICENSE
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      165 2024-03-31 20:17:42.000000 kss-5.1.0/MANIFEST.in
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    78567 2024-03-31 21:19:05.572240 kss-5.1.0/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    77824 2024-03-31 21:17:02.000000 kss-5.1.0/README.md
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-03-31 21:19:05.562023 kss-5.1.0/csrc/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2024-03-31 20:12:01.000000 kss-5.1.0/csrc/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      563 2024-03-31 20:36:14.000000 kss-5.1.0/csrc/kss_cython.pyx
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5965 2024-03-31 20:12:01.000000 kss-5.1.0/csrc/sentence_splitter.cpp
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7830 2024-03-31 20:12:01.000000 kss-5.1.0/csrc/sentence_splitter.h
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-03-31 21:19:05.562226 kss-5.1.0/kss/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      432 2024-03-31 20:40:11.000000 kss-5.1.0/kss/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-03-31 21:19:05.563760 kss-5.1.0/kss/_elements/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_elements/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4888 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_elements/element.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2702 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_elements/empty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      369 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_elements/subclasses.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-03-31 21:19:05.563957 kss-5.1.0/kss/_modules/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_modules/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-03-31 21:19:05.564954 kss-5.1.0/kss/_modules/morphemes/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_modules/morphemes/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2652 2024-03-31 13:42:10.000000 kss-5.1.0/kss/_modules/morphemes/analyzers.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1702 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_modules/morphemes/split_morphemes.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3403 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_modules/morphemes/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-03-31 21:19:05.569903 kss-5.1.0/kss/_modules/sentences/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_modules/sentences/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     9334 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_modules/sentences/embracing_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    22898 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_modules/sentences/sentence_postprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6751 2024-03-31 07:55:02.000000 kss-5.1.0/kss/_modules/sentences/sentence_preprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2298 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_modules/sentences/sentence_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    30242 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_modules/sentences/sentence_splitter.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    13304 2024-03-31 20:36:14.000000 kss-5.1.0/kss/_modules/sentences/sentence_splitter_fast.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6829 2024-03-31 20:48:01.000000 kss-5.1.0/kss/_modules/sentences/split_sentences.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-03-31 21:19:05.570626 kss-5.1.0/kss/_modules/summarization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_modules/summarization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      820 2023-05-16 17:34:32.000000 kss-5.1.0/kss/_modules/summarization/sentence.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3600 2023-05-16 17:34:32.000000 kss-5.1.0/kss/_modules/summarization/summarize_sentences.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2727 2023-05-16 17:34:32.000000 kss-5.1.0/kss/_modules/summarization/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-03-31 21:19:05.571829 kss-5.1.0/kss/_utils/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_utils/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    10329 2024-03-31 07:46:03.000000 kss-5.1.0/kss/_utils/const.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1408 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_utils/emojis.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      269 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_utils/logging.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1001 2023-08-22 23:38:03.000000 kss-5.1.0/kss/_utils/multiprocessing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    12324 2024-03-31 14:02:55.000000 kss-5.1.0/kss/_utils/sanity_checks.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-03-31 21:19:05.563017 kss-5.1.0/kss.egg-info/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    78567 2024-03-31 21:19:05.000000 kss-5.1.0/kss.egg-info/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1251 2024-03-31 21:19:05.000000 kss-5.1.0/kss.egg-info/SOURCES.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-03-31 21:19:05.000000 kss-5.1.0/kss.egg-info/dependency_links.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-03-31 20:01:41.000000 kss-5.1.0/kss.egg-info/not-zip-safe
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       34 2024-03-31 21:19:05.000000 kss-5.1.0/kss.egg-info/requires.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       20 2024-03-31 21:19:05.000000 kss-5.1.0/kss.egg-info/top_level.txt
--rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2024-03-31 21:19:05.572475 kss-5.1.0/setup.cfg
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3876 2024-03-31 20:35:31.000000 kss-5.1.0/setup.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.926372 kss-5.2.0/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1569 2024-04-01 04:29:21.000000 kss-5.2.0/LICENSE
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      165 2024-03-31 20:17:42.000000 kss-5.2.0/MANIFEST.in
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    78578 2024-04-01 23:54:54.926515 kss-5.2.0/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    77826 2024-04-01 04:29:21.000000 kss-5.2.0/README.md
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.918974 kss-5.2.0/csrc/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2024-03-31 20:12:01.000000 kss-5.2.0/csrc/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      563 2024-03-31 20:36:14.000000 kss-5.2.0/csrc/kss_cython.pyx
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5965 2024-03-31 20:12:01.000000 kss-5.2.0/csrc/sentence_splitter.cpp
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7830 2024-03-31 20:12:01.000000 kss-5.2.0/csrc/sentence_splitter.h
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.919088 kss-5.2.0/kss/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      432 2024-04-01 23:54:10.000000 kss-5.2.0/kss/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.920798 kss-5.2.0/kss/_elements/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_elements/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4888 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_elements/element.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2702 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_elements/empty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      369 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_elements/subclasses.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.921111 kss-5.2.0/kss/_modules/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.922027 kss-5.2.0/kss/_modules/morphemes/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/morphemes/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2652 2024-03-31 13:42:10.000000 kss-5.2.0/kss/_modules/morphemes/analyzers.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1702 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/morphemes/split_morphemes.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3403 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/morphemes/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.924256 kss-5.2.0/kss/_modules/sentences/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/sentences/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9334 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/sentences/embracing_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    22898 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/sentences/sentence_postprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6751 2024-03-31 07:55:02.000000 kss-5.2.0/kss/_modules/sentences/sentence_preprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2298 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/sentences/sentence_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    30242 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/sentences/sentence_splitter.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    13304 2024-03-31 20:36:14.000000 kss-5.2.0/kss/_modules/sentences/sentence_splitter_fast.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6829 2024-03-31 20:48:01.000000 kss-5.2.0/kss/_modules/sentences/split_sentences.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.925005 kss-5.2.0/kss/_modules/summarization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_modules/summarization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      820 2023-05-16 17:34:32.000000 kss-5.2.0/kss/_modules/summarization/sentence.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3600 2023-05-16 17:34:32.000000 kss-5.2.0/kss/_modules/summarization/summarize_sentences.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2727 2023-05-16 17:34:32.000000 kss-5.2.0/kss/_modules/summarization/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.926172 kss-5.2.0/kss/_utils/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_utils/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    10329 2024-03-31 07:46:03.000000 kss-5.2.0/kss/_utils/const.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1408 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_utils/emojis.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      269 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_utils/logging.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1001 2023-08-22 23:38:03.000000 kss-5.2.0/kss/_utils/multiprocessing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    12324 2024-03-31 14:02:55.000000 kss-5.2.0/kss/_utils/sanity_checks.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-01 23:54:54.919965 kss-5.2.0/kss.egg-info/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    78578 2024-04-01 23:54:54.000000 kss-5.2.0/kss.egg-info/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1251 2024-04-01 23:54:54.000000 kss-5.2.0/kss.egg-info/SOURCES.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-01 23:54:54.000000 kss-5.2.0/kss.egg-info/dependency_links.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-03-31 20:01:41.000000 kss-5.2.0/kss.egg-info/not-zip-safe
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       34 2024-04-01 23:54:54.000000 kss-5.2.0/kss.egg-info/requires.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       20 2024-04-01 23:54:54.000000 kss-5.2.0/kss.egg-info/top_level.txt
+-rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2024-04-01 23:54:54.926737 kss-5.2.0/setup.cfg
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5863 2024-04-01 23:54:10.000000 kss-5.2.0/setup.py
```

### Comparing `kss-5.1.0/LICENSE` & `kss-5.2.0/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2021 Hyunwoong Ko <kevin.ko@tunib.ai> and Sang-Kil Park <skpark1224@hyundai.com>
+Copyright (C) 2021 Hyunwoong Ko <kevin.brain@kakaobrain.com> and Sang-Kil Park <skpark1224@hyundai.com>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 1. Redistributions of source code must retain the above copyright
    notice, this list of conditions and the following disclaimer.
@@ -19,8 +19,8 @@
 ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
 LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
 CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE.
+POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `kss-5.1.0/PKG-INFO` & `kss-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: kss
-Version: 5.1.0
+Version: 5.2.0
 Summary: A Toolkit for Korean sentence segmentation
 Home-page: https://github.com/hyunwoongko/kss
 Author: Hyunwoong Ko
-Author-email: kevin.ko@tunib.ai
+Author-email: kevin.brain@kakaobrain.com
 License: BSD 3-Clause "New" or "Revised" License
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -25,15 +25,15 @@
 
 This repository contains the source code of Kss, a representative Korean sentence segmentation toolkit. I also conduct ongoing research about Korean sentence segmentation algorithms and report the results to this repository.
 If you have some good ideas about Korean sentence segmentation, please feel free to talk through the [issue](https://github.com/hyunwoongko/kss/issues).
 
 <br>
 
 ### What's New:
-- March 31, 2024 [Released Kss 5.0 Python](https://github.com/hyunwoongko/kss/releases/tag/5.0.0).
+- March 31, 2024 [Released Kss 5.0 Python](https://github.com/hyunwoongko/kss/releases/tag/5.1.0).
 - December 19, 2022 [Released Kss 4.0 Python](https://github.com/hyunwoongko/kss/releases/tag/4.0.0).
 - May 5, 2022 [Released Kss Fluter](https://github.com/khjde1207/kss_dart).
 - August 25, 2021 [Released Kss Java](https://github.com/sangdee/kss-java).
 - August 18, 2021 [Released Kss 3.0 Python](https://github.com/hyunwoongko/kss/releases/tag/3.0.1).
 - December 21, 2020 [Released Kss 2.0 Python](https://github.com/hyunwoongko/kss/releases/tag/3.0.1).
 - August 16, 2019 [Released Kss 1.0 C++](https://github.com/hyunwoongko/kss/releases/tag/3.0.1).
 
@@ -765,29 +765,29 @@
 
 If you want to split sentences quickly, you can use the `split_sentences` function with the `backend='fast'` option from Kss 5.0.0.
 This method is based on the fast algorithm utilized in Kss versions prior to 3.0.
 It offers significantly faster processing compared to the `mecab` backend, but less accurate.
 Therefore, This feature could be useful when you need to split sentences very quickly but don't need high accuracy.
 Furthermore, the `fast` backend has been implemented in both Python and Cython.
 
-- If your environment supports the installation of `Cython`, Kss will use the Cython implementation, which boasts the fastest performance (**x600 faster than `mecab`**).
-- Otherwise, it will use the Python implementation, which is slower than the Cython version but faster than the `mecab` backend **(x4 faster than `mecab`)**.
+- If your environment supports the installation of `Cython`, Kss will use the Cython implementation, which boasts the fastest performance (**x600 faster than** `mecab`).
+- Otherwise, it will use the Python implementation, which is slower than the Cython version but faster than the `mecab` backend (**x4 faster than** `mecab`).
 
 Given the substantial speed advantage of the Cython implementation, it is strongly recommended over the Python alternative.
 Kss automatically detects the availability of Cython in your environment and will install it if feasible, so you don't need to worry about Cython and C++ dependencies.
 
-### Accuracy (Normalized F1)
+#### Accuracy (Normalized F1)
 
 | Backend         | blogs_ko   | blogs_lee  | nested     | sample     | tweets     | v_ending   | wikipedia  |
 |-----------------|------------|------------|------------|------------|------------|------------|------------|
 | `mecab`         | **0.8860** | **0.8887** | **0.9206** | **0.9682** | **0.8137** | **0.4815** | **1.0000** |
 | `fast` (Python) | 0.6281     | 0.7899     | 0.6899     | 0.7482     | 0.5315     | 0.1596     | 0.7358     |
 | `fast` (Cython) | 0.6545     | 0.8132     | 0.6372     | 0.8407     | 0.5892     | 0.1596     | 0.9566     |
 
-### Speed (msec)
+#### Speed (msec)
 
 | Backend         | blogs_ko | blogs_lee | nested   | sample   | tweets   | v_ending | wikipedia |
 |-----------------|----------|-----------|----------|----------|----------|----------|-----------|
 | `mecab`         | 538.10   | 293.31    | 225.05   | 56.35    | 184.91   | 20.55    | 899.99    |
 | `fast` (Python) | 146.75   | 70.94     | 52.84    | 12.11    | 37.80    | 4.69     | 255.90    |
 | `fast` (Cython) | **0.91** | **0.55**  | **0.46** | **0.09** | **0.40** | **0.05** | **1.12**  |
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: kss Version: 5.1.0 Summary: A Toolkit for Korean
+Metadata-Version: 2.1 Name: kss Version: 5.2.0 Summary: A Toolkit for Korean
 sentence segmentation Home-page: https://github.com/hyunwoongko/kss Author:
-Hyunwoong Ko Author-email: kevin.ko@tunib.ai License: BSD 3-Clause "New" or
-"Revised" License Platform: any Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2 Classifier: Programming
-Language :: Python :: 3.3 Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # Kss: A Toolkit
-for Korean sentence segmentation _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_I_s_s_u_e_s_]This repository
-contains the source code of Kss, a representative Korean sentence segmentation
-toolkit. I also conduct ongoing research about Korean sentence segmentation
-algorithms and report the results to this repository. If you have some good
-ideas about Korean sentence segmentation, please feel free to talk through the
-[issue](https://github.com/hyunwoongko/kss/issues).
+Hyunwoong Ko Author-email: kevin.brain@kakaobrain.com License: BSD 3-Clause
+"New" or "Revised" License Platform: any Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.2 Classifier:
+Programming Language :: Python :: 3.3 Classifier: Programming Language ::
+Python :: 3.4 Classifier: Programming Language :: Python :: 3.5 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Requires-
+Python: >=3 Description-Content-Type: text/markdown License-File: LICENSE #
+Kss: A Toolkit for Korean sentence segmentation _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_I_s_s_u_e_s_]This
+repository contains the source code of Kss, a representative Korean sentence
+segmentation toolkit. I also conduct ongoing research about Korean sentence
+segmentation algorithms and report the results to this repository. If you have
+some good ideas about Korean sentence segmentation, please feel free to talk
+through the [issue](https://github.com/hyunwoongko/kss/issues).
 ### What's New: - March 31, 2024 [Released Kss 5.0 Python](https://github.com/
-hyunwoongko/kss/releases/tag/5.0.0). - December 19, 2022 [Released Kss 4.0
+hyunwoongko/kss/releases/tag/5.1.0). - December 19, 2022 [Released Kss 4.0
 Python](https://github.com/hyunwoongko/kss/releases/tag/4.0.0). - May 5, 2022
 [Released Kss Fluter](https://github.com/khjde1207/kss_dart). - August 25, 2021
 [Released Kss Java](https://github.com/sangdee/kss-java). - August 18, 2021
 [Released Kss 3.0 Python](https://github.com/hyunwoongko/kss/releases/tag/
 3.0.1). - December 21, 2020 [Released Kss 2.0 Python](https://github.com/
 hyunwoongko/kss/releases/tag/3.0.1). - August 16, 2019 [Released Kss 1.0 C++]
 (https://github.com/hyunwoongko/kss/releases/tag/3.0.1). ## Installation ###
@@ -658,28 +658,28 @@
 function with the `backend='fast'` option from Kss 5.0.0. This method is based
 on the fast algorithm utilized in Kss versions prior to 3.0. It offers
 significantly faster processing compared to the `mecab` backend, but less
 accurate. Therefore, This feature could be useful when you need to split
 sentences very quickly but don't need high accuracy. Furthermore, the `fast`
 backend has been implemented in both Python and Cython. - If your environment
 supports the installation of `Cython`, Kss will use the Cython implementation,
-which boasts the fastest performance (**x600 faster than `mecab`**). -
+which boasts the fastest performance (**x600 faster than** `mecab`). -
 Otherwise, it will use the Python implementation, which is slower than the
-Cython version but faster than the `mecab` backend **(x4 faster than
-`mecab`)**. Given the substantial speed advantage of the Cython implementation,
+Cython version but faster than the `mecab` backend (**x4 faster than**
+`mecab`). Given the substantial speed advantage of the Cython implementation,
 it is strongly recommended over the Python alternative. Kss automatically
 detects the availability of Cython in your environment and will install it if
-feasible, so you don't need to worry about Cython and C++ dependencies. ###
+feasible, so you don't need to worry about Cython and C++ dependencies. ####
 Accuracy (Normalized F1) | Backend | blogs_ko | blogs_lee | nested | sample |
 tweets | v_ending | wikipedia | |-----------------|------------|------------|--
 ----------|------------|------------|------------|------------| | `mecab` |
 **0.8860** | **0.8887** | **0.9206** | **0.9682** | **0.8137** | **0.4815** |
 **1.0000** | | `fast` (Python) | 0.6281 | 0.7899 | 0.6899 | 0.7482 | 0.5315 |
 0.1596 | 0.7358 | | `fast` (Cython) | 0.6545 | 0.8132 | 0.6372 | 0.8407 |
-0.5892 | 0.1596 | 0.9566 | ### Speed (msec) | Backend | blogs_ko | blogs_lee |
+0.5892 | 0.1596 | 0.9566 | #### Speed (msec) | Backend | blogs_ko | blogs_lee |
 nested | sample | tweets | v_ending | wikipedia | |-----------------|----------
 |-----------|----------|----------|----------|----------|-----------| | `mecab`
 | 538.10 | 293.31 | 225.05 | 56.35 | 184.91 | 20.55 | 899.99 | | `fast`
 (Python) | 146.75 | 70.94 | 52.84 | 12.11 | 37.80 | 4.69 | 255.90 | | `fast`
 (Cython) | **0.91** | **0.55** | **0.46** | **0.09** | **0.40** | **0.05** |
 **1.12** | Please note that while the core algorithm in the `fast` backend
 mirrors that of Kss C++ 1.3.1, several bugs identified in the original
```

### Comparing `kss-5.1.0/README.md` & `kss-5.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This repository contains the source code of Kss, a representative Korean sentence segmentation toolkit. I also conduct ongoing research about Korean sentence segmentation algorithms and report the results to this repository.
 If you have some good ideas about Korean sentence segmentation, please feel free to talk through the [issue](https://github.com/hyunwoongko/kss/issues).
 
 <br>
 
 ### What's New:
-- March 31, 2024 [Released Kss 5.0 Python](https://github.com/hyunwoongko/kss/releases/tag/5.0.0).
+- March 31, 2024 [Released Kss 5.0 Python](https://github.com/hyunwoongko/kss/releases/tag/5.1.0).
 - December 19, 2022 [Released Kss 4.0 Python](https://github.com/hyunwoongko/kss/releases/tag/4.0.0).
 - May 5, 2022 [Released Kss Fluter](https://github.com/khjde1207/kss_dart).
 - August 25, 2021 [Released Kss Java](https://github.com/sangdee/kss-java).
 - August 18, 2021 [Released Kss 3.0 Python](https://github.com/hyunwoongko/kss/releases/tag/3.0.1).
 - December 21, 2020 [Released Kss 2.0 Python](https://github.com/hyunwoongko/kss/releases/tag/3.0.1).
 - August 16, 2019 [Released Kss 1.0 C++](https://github.com/hyunwoongko/kss/releases/tag/3.0.1).
 
@@ -744,29 +744,29 @@
 
 If you want to split sentences quickly, you can use the `split_sentences` function with the `backend='fast'` option from Kss 5.0.0.
 This method is based on the fast algorithm utilized in Kss versions prior to 3.0.
 It offers significantly faster processing compared to the `mecab` backend, but less accurate.
 Therefore, This feature could be useful when you need to split sentences very quickly but don't need high accuracy.
 Furthermore, the `fast` backend has been implemented in both Python and Cython.
 
-- If your environment supports the installation of `Cython`, Kss will use the Cython implementation, which boasts the fastest performance (**x600 faster than `mecab`**).
-- Otherwise, it will use the Python implementation, which is slower than the Cython version but faster than the `mecab` backend **(x4 faster than `mecab`)**.
+- If your environment supports the installation of `Cython`, Kss will use the Cython implementation, which boasts the fastest performance (**x600 faster than** `mecab`).
+- Otherwise, it will use the Python implementation, which is slower than the Cython version but faster than the `mecab` backend (**x4 faster than** `mecab`).
 
 Given the substantial speed advantage of the Cython implementation, it is strongly recommended over the Python alternative.
 Kss automatically detects the availability of Cython in your environment and will install it if feasible, so you don't need to worry about Cython and C++ dependencies.
 
-### Accuracy (Normalized F1)
+#### Accuracy (Normalized F1)
 
 | Backend         | blogs_ko   | blogs_lee  | nested     | sample     | tweets     | v_ending   | wikipedia  |
 |-----------------|------------|------------|------------|------------|------------|------------|------------|
 | `mecab`         | **0.8860** | **0.8887** | **0.9206** | **0.9682** | **0.8137** | **0.4815** | **1.0000** |
 | `fast` (Python) | 0.6281     | 0.7899     | 0.6899     | 0.7482     | 0.5315     | 0.1596     | 0.7358     |
 | `fast` (Cython) | 0.6545     | 0.8132     | 0.6372     | 0.8407     | 0.5892     | 0.1596     | 0.9566     |
 
-### Speed (msec)
+#### Speed (msec)
 
 | Backend         | blogs_ko | blogs_lee | nested   | sample   | tweets   | v_ending | wikipedia |
 |-----------------|----------|-----------|----------|----------|----------|----------|-----------|
 | `mecab`         | 538.10   | 293.31    | 225.05   | 56.35    | 184.91   | 20.55    | 899.99    |
 | `fast` (Python) | 146.75   | 70.94     | 52.84    | 12.11    | 37.80    | 4.69     | 255.90    |
 | `fast` (Cython) | **0.91** | **0.55**  | **0.46** | **0.09** | **0.40** | **0.05** | **1.12**  |
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # Kss: A Toolkit for Korean sentence segmentation _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_I_s_s_u_e_s_]This
 repository contains the source code of Kss, a representative Korean sentence
 segmentation toolkit. I also conduct ongoing research about Korean sentence
 segmentation algorithms and report the results to this repository. If you have
 some good ideas about Korean sentence segmentation, please feel free to talk
 through the [issue](https://github.com/hyunwoongko/kss/issues).
 ### What's New: - March 31, 2024 [Released Kss 5.0 Python](https://github.com/
-hyunwoongko/kss/releases/tag/5.0.0). - December 19, 2022 [Released Kss 4.0
+hyunwoongko/kss/releases/tag/5.1.0). - December 19, 2022 [Released Kss 4.0
 Python](https://github.com/hyunwoongko/kss/releases/tag/4.0.0). - May 5, 2022
 [Released Kss Fluter](https://github.com/khjde1207/kss_dart). - August 25, 2021
 [Released Kss Java](https://github.com/sangdee/kss-java). - August 18, 2021
 [Released Kss 3.0 Python](https://github.com/hyunwoongko/kss/releases/tag/
 3.0.1). - December 21, 2020 [Released Kss 2.0 Python](https://github.com/
 hyunwoongko/kss/releases/tag/3.0.1). - August 16, 2019 [Released Kss 1.0 C++]
 (https://github.com/hyunwoongko/kss/releases/tag/3.0.1). ## Installation ###
@@ -648,28 +648,28 @@
 function with the `backend='fast'` option from Kss 5.0.0. This method is based
 on the fast algorithm utilized in Kss versions prior to 3.0. It offers
 significantly faster processing compared to the `mecab` backend, but less
 accurate. Therefore, This feature could be useful when you need to split
 sentences very quickly but don't need high accuracy. Furthermore, the `fast`
 backend has been implemented in both Python and Cython. - If your environment
 supports the installation of `Cython`, Kss will use the Cython implementation,
-which boasts the fastest performance (**x600 faster than `mecab`**). -
+which boasts the fastest performance (**x600 faster than** `mecab`). -
 Otherwise, it will use the Python implementation, which is slower than the
-Cython version but faster than the `mecab` backend **(x4 faster than
-`mecab`)**. Given the substantial speed advantage of the Cython implementation,
+Cython version but faster than the `mecab` backend (**x4 faster than**
+`mecab`). Given the substantial speed advantage of the Cython implementation,
 it is strongly recommended over the Python alternative. Kss automatically
 detects the availability of Cython in your environment and will install it if
-feasible, so you don't need to worry about Cython and C++ dependencies. ###
+feasible, so you don't need to worry about Cython and C++ dependencies. ####
 Accuracy (Normalized F1) | Backend | blogs_ko | blogs_lee | nested | sample |
 tweets | v_ending | wikipedia | |-----------------|------------|------------|--
 ----------|------------|------------|------------|------------| | `mecab` |
 **0.8860** | **0.8887** | **0.9206** | **0.9682** | **0.8137** | **0.4815** |
 **1.0000** | | `fast` (Python) | 0.6281 | 0.7899 | 0.6899 | 0.7482 | 0.5315 |
 0.1596 | 0.7358 | | `fast` (Cython) | 0.6545 | 0.8132 | 0.6372 | 0.8407 |
-0.5892 | 0.1596 | 0.9566 | ### Speed (msec) | Backend | blogs_ko | blogs_lee |
+0.5892 | 0.1596 | 0.9566 | #### Speed (msec) | Backend | blogs_ko | blogs_lee |
 nested | sample | tweets | v_ending | wikipedia | |-----------------|----------
 |-----------|----------|----------|----------|----------|-----------| | `mecab`
 | 538.10 | 293.31 | 225.05 | 56.35 | 184.91 | 20.55 | 899.99 | | `fast`
 (Python) | 146.75 | 70.94 | 52.84 | 12.11 | 37.80 | 4.69 | 255.90 | | `fast`
 (Cython) | **0.91** | **0.55** | **0.46** | **0.09** | **0.40** | **0.05** |
 **1.12** | Please note that while the core algorithm in the `fast` backend
 mirrors that of Kss C++ 1.3.1, several bugs identified in the original
```

### Comparing `kss-5.1.0/csrc/kss_cython.pyx` & `kss-5.2.0/csrc/kss_cython.pyx`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/csrc/sentence_splitter.cpp` & `kss-5.2.0/csrc/sentence_splitter.cpp`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/csrc/sentence_splitter.h` & `kss-5.2.0/csrc/sentence_splitter.h`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_elements/element.py` & `kss-5.2.0/kss/_elements/element.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_elements/empty.py` & `kss-5.2.0/kss/_elements/empty.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_modules/morphemes/analyzers.py` & `kss-5.2.0/kss/_modules/morphemes/analyzers.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_modules/morphemes/split_morphemes.py` & `kss-5.2.0/kss/_modules/morphemes/split_morphemes.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_modules/morphemes/utils.py` & `kss-5.2.0/kss/_modules/morphemes/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_modules/sentences/embracing_processor.py` & `kss-5.2.0/kss/_modules/sentences/embracing_processor.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_modules/sentences/sentence_postprocessor.py` & `kss-5.2.0/kss/_modules/sentences/sentence_postprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_modules/sentences/sentence_preprocessor.py` & `kss-5.2.0/kss/_modules/sentences/sentence_preprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_modules/sentences/sentence_processor.py` & `kss-5.2.0/kss/_modules/sentences/sentence_processor.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_modules/sentences/sentence_splitter.py` & `kss-5.2.0/kss/_modules/sentences/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_modules/sentences/sentence_splitter_fast.py` & `kss-5.2.0/kss/_modules/sentences/sentence_splitter_fast.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_modules/sentences/split_sentences.py` & `kss-5.2.0/kss/_modules/sentences/split_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_modules/summarization/sentence.py` & `kss-5.2.0/kss/_modules/summarization/sentence.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_modules/summarization/summarize_sentences.py` & `kss-5.2.0/kss/_modules/summarization/summarize_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_modules/summarization/utils.py` & `kss-5.2.0/kss/_modules/summarization/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_utils/const.py` & `kss-5.2.0/kss/_utils/const.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_utils/emojis.py` & `kss-5.2.0/kss/_utils/emojis.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_utils/multiprocessing.py` & `kss-5.2.0/kss/_utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss/_utils/sanity_checks.py` & `kss-5.2.0/kss/_utils/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `kss-5.1.0/kss.egg-info/PKG-INFO` & `kss-5.2.0/kss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: kss
-Version: 5.1.0
+Version: 5.2.0
 Summary: A Toolkit for Korean sentence segmentation
 Home-page: https://github.com/hyunwoongko/kss
 Author: Hyunwoong Ko
-Author-email: kevin.ko@tunib.ai
+Author-email: kevin.brain@kakaobrain.com
 License: BSD 3-Clause "New" or "Revised" License
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -25,15 +25,15 @@
 
 This repository contains the source code of Kss, a representative Korean sentence segmentation toolkit. I also conduct ongoing research about Korean sentence segmentation algorithms and report the results to this repository.
 If you have some good ideas about Korean sentence segmentation, please feel free to talk through the [issue](https://github.com/hyunwoongko/kss/issues).
 
 <br>
 
 ### What's New:
-- March 31, 2024 [Released Kss 5.0 Python](https://github.com/hyunwoongko/kss/releases/tag/5.0.0).
+- March 31, 2024 [Released Kss 5.0 Python](https://github.com/hyunwoongko/kss/releases/tag/5.1.0).
 - December 19, 2022 [Released Kss 4.0 Python](https://github.com/hyunwoongko/kss/releases/tag/4.0.0).
 - May 5, 2022 [Released Kss Fluter](https://github.com/khjde1207/kss_dart).
 - August 25, 2021 [Released Kss Java](https://github.com/sangdee/kss-java).
 - August 18, 2021 [Released Kss 3.0 Python](https://github.com/hyunwoongko/kss/releases/tag/3.0.1).
 - December 21, 2020 [Released Kss 2.0 Python](https://github.com/hyunwoongko/kss/releases/tag/3.0.1).
 - August 16, 2019 [Released Kss 1.0 C++](https://github.com/hyunwoongko/kss/releases/tag/3.0.1).
 
@@ -765,29 +765,29 @@
 
 If you want to split sentences quickly, you can use the `split_sentences` function with the `backend='fast'` option from Kss 5.0.0.
 This method is based on the fast algorithm utilized in Kss versions prior to 3.0.
 It offers significantly faster processing compared to the `mecab` backend, but less accurate.
 Therefore, This feature could be useful when you need to split sentences very quickly but don't need high accuracy.
 Furthermore, the `fast` backend has been implemented in both Python and Cython.
 
-- If your environment supports the installation of `Cython`, Kss will use the Cython implementation, which boasts the fastest performance (**x600 faster than `mecab`**).
-- Otherwise, it will use the Python implementation, which is slower than the Cython version but faster than the `mecab` backend **(x4 faster than `mecab`)**.
+- If your environment supports the installation of `Cython`, Kss will use the Cython implementation, which boasts the fastest performance (**x600 faster than** `mecab`).
+- Otherwise, it will use the Python implementation, which is slower than the Cython version but faster than the `mecab` backend (**x4 faster than** `mecab`).
 
 Given the substantial speed advantage of the Cython implementation, it is strongly recommended over the Python alternative.
 Kss automatically detects the availability of Cython in your environment and will install it if feasible, so you don't need to worry about Cython and C++ dependencies.
 
-### Accuracy (Normalized F1)
+#### Accuracy (Normalized F1)
 
 | Backend         | blogs_ko   | blogs_lee  | nested     | sample     | tweets     | v_ending   | wikipedia  |
 |-----------------|------------|------------|------------|------------|------------|------------|------------|
 | `mecab`         | **0.8860** | **0.8887** | **0.9206** | **0.9682** | **0.8137** | **0.4815** | **1.0000** |
 | `fast` (Python) | 0.6281     | 0.7899     | 0.6899     | 0.7482     | 0.5315     | 0.1596     | 0.7358     |
 | `fast` (Cython) | 0.6545     | 0.8132     | 0.6372     | 0.8407     | 0.5892     | 0.1596     | 0.9566     |
 
-### Speed (msec)
+#### Speed (msec)
 
 | Backend         | blogs_ko | blogs_lee | nested   | sample   | tweets   | v_ending | wikipedia |
 |-----------------|----------|-----------|----------|----------|----------|----------|-----------|
 | `mecab`         | 538.10   | 293.31    | 225.05   | 56.35    | 184.91   | 20.55    | 899.99    |
 | `fast` (Python) | 146.75   | 70.94     | 52.84    | 12.11    | 37.80    | 4.69     | 255.90    |
 | `fast` (Cython) | **0.91** | **0.55**  | **0.46** | **0.09** | **0.40** | **0.05** | **1.12**  |
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: kss Version: 5.1.0 Summary: A Toolkit for Korean
+Metadata-Version: 2.1 Name: kss Version: 5.2.0 Summary: A Toolkit for Korean
 sentence segmentation Home-page: https://github.com/hyunwoongko/kss Author:
-Hyunwoong Ko Author-email: kevin.ko@tunib.ai License: BSD 3-Clause "New" or
-"Revised" License Platform: any Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2 Classifier: Programming
-Language :: Python :: 3.3 Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # Kss: A Toolkit
-for Korean sentence segmentation _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_I_s_s_u_e_s_]This repository
-contains the source code of Kss, a representative Korean sentence segmentation
-toolkit. I also conduct ongoing research about Korean sentence segmentation
-algorithms and report the results to this repository. If you have some good
-ideas about Korean sentence segmentation, please feel free to talk through the
-[issue](https://github.com/hyunwoongko/kss/issues).
+Hyunwoong Ko Author-email: kevin.brain@kakaobrain.com License: BSD 3-Clause
+"New" or "Revised" License Platform: any Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.2 Classifier:
+Programming Language :: Python :: 3.3 Classifier: Programming Language ::
+Python :: 3.4 Classifier: Programming Language :: Python :: 3.5 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Requires-
+Python: >=3 Description-Content-Type: text/markdown License-File: LICENSE #
+Kss: A Toolkit for Korean sentence segmentation _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_I_s_s_u_e_s_]This
+repository contains the source code of Kss, a representative Korean sentence
+segmentation toolkit. I also conduct ongoing research about Korean sentence
+segmentation algorithms and report the results to this repository. If you have
+some good ideas about Korean sentence segmentation, please feel free to talk
+through the [issue](https://github.com/hyunwoongko/kss/issues).
 ### What's New: - March 31, 2024 [Released Kss 5.0 Python](https://github.com/
-hyunwoongko/kss/releases/tag/5.0.0). - December 19, 2022 [Released Kss 4.0
+hyunwoongko/kss/releases/tag/5.1.0). - December 19, 2022 [Released Kss 4.0
 Python](https://github.com/hyunwoongko/kss/releases/tag/4.0.0). - May 5, 2022
 [Released Kss Fluter](https://github.com/khjde1207/kss_dart). - August 25, 2021
 [Released Kss Java](https://github.com/sangdee/kss-java). - August 18, 2021
 [Released Kss 3.0 Python](https://github.com/hyunwoongko/kss/releases/tag/
 3.0.1). - December 21, 2020 [Released Kss 2.0 Python](https://github.com/
 hyunwoongko/kss/releases/tag/3.0.1). - August 16, 2019 [Released Kss 1.0 C++]
 (https://github.com/hyunwoongko/kss/releases/tag/3.0.1). ## Installation ###
@@ -658,28 +658,28 @@
 function with the `backend='fast'` option from Kss 5.0.0. This method is based
 on the fast algorithm utilized in Kss versions prior to 3.0. It offers
 significantly faster processing compared to the `mecab` backend, but less
 accurate. Therefore, This feature could be useful when you need to split
 sentences very quickly but don't need high accuracy. Furthermore, the `fast`
 backend has been implemented in both Python and Cython. - If your environment
 supports the installation of `Cython`, Kss will use the Cython implementation,
-which boasts the fastest performance (**x600 faster than `mecab`**). -
+which boasts the fastest performance (**x600 faster than** `mecab`). -
 Otherwise, it will use the Python implementation, which is slower than the
-Cython version but faster than the `mecab` backend **(x4 faster than
-`mecab`)**. Given the substantial speed advantage of the Cython implementation,
+Cython version but faster than the `mecab` backend (**x4 faster than**
+`mecab`). Given the substantial speed advantage of the Cython implementation,
 it is strongly recommended over the Python alternative. Kss automatically
 detects the availability of Cython in your environment and will install it if
-feasible, so you don't need to worry about Cython and C++ dependencies. ###
+feasible, so you don't need to worry about Cython and C++ dependencies. ####
 Accuracy (Normalized F1) | Backend | blogs_ko | blogs_lee | nested | sample |
 tweets | v_ending | wikipedia | |-----------------|------------|------------|--
 ----------|------------|------------|------------|------------| | `mecab` |
 **0.8860** | **0.8887** | **0.9206** | **0.9682** | **0.8137** | **0.4815** |
 **1.0000** | | `fast` (Python) | 0.6281 | 0.7899 | 0.6899 | 0.7482 | 0.5315 |
 0.1596 | 0.7358 | | `fast` (Cython) | 0.6545 | 0.8132 | 0.6372 | 0.8407 |
-0.5892 | 0.1596 | 0.9566 | ### Speed (msec) | Backend | blogs_ko | blogs_lee |
+0.5892 | 0.1596 | 0.9566 | #### Speed (msec) | Backend | blogs_ko | blogs_lee |
 nested | sample | tweets | v_ending | wikipedia | |-----------------|----------
 |-----------|----------|----------|----------|----------|-----------| | `mecab`
 | 538.10 | 293.31 | 225.05 | 56.35 | 184.91 | 20.55 | 899.99 | | `fast`
 (Python) | 146.75 | 70.94 | 52.84 | 12.11 | 37.80 | 4.69 | 255.90 | | `fast`
 (Cython) | **0.91** | **0.55** | **0.46** | **0.09** | **0.40** | **0.05** |
 **1.12** | Please note that while the core algorithm in the `fast` backend
 mirrors that of Kss C++ 1.3.1, several bugs identified in the original
```

### Comparing `kss-5.1.0/kss.egg-info/SOURCES.txt` & `kss-5.2.0/kss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

