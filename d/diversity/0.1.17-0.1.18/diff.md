# Comparing `tmp/diversity-0.1.17.tar.gz` & `tmp/diversity-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diversity-0.1.17.tar", max compression
+gzip compressed data, was "diversity-0.1.18.tar", max compression
```

## Comparing `diversity-0.1.17.tar` & `diversity-0.1.18.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1831 2024-02-26 15:02:57.406104 diversity-0.1.17/README.md
--rw-r--r--   0        0        0      281 2023-11-16 20:38:21.272011 diversity-0.1.17/diversity/__init__.py
--rw-r--r--   0        0        0     1726 2023-11-01 21:29:51.363577 diversity-0.1.17/diversity/compression.py
--rw-r--r--   0        0        0     3217 2023-11-14 16:35:10.728417 diversity-0.1.17/diversity/homogenization.py
--rw-r--r--   0        0        0      724 2023-11-01 21:29:53.363660 diversity-0.1.17/diversity/ngram_diversity.py
--rw-r--r--   0        0        0       84 2023-10-04 17:47:31.256275 diversity-0.1.17/diversity/patterns/__init__.py
--rw-r--r--   0        0        0     2155 2023-10-07 17:22:30.499800 diversity-0.1.17/diversity/patterns/part_of_speech.py
--rw-r--r--   0        0        0      821 2023-10-07 17:23:14.046690 diversity-0.1.17/diversity/patterns/token.py
--rw-r--r--   0        0        0       30 2023-10-10 18:40:51.809862 diversity-0.1.17/diversity/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-02-26 15:03:39.741528 diversity-0.1.17/diversity/utils/memoize.py
--rw-r--r--   0        0        0      454 2024-02-26 15:01:14.563639 diversity-0.1.17/pyproject.toml
--rw-r--r--   0        0        0     2339 1970-01-01 00:00:00.000000 diversity-0.1.17/PKG-INFO
+-rw-r--r--   0        0        0     4027 2024-04-02 18:29:23.764260 diversity-0.1.18/README.md
+-rw-r--r--   0        0        0      281 2023-11-16 20:38:21.272011 diversity-0.1.18/diversity/__init__.py
+-rw-r--r--   0        0        0     1726 2023-11-01 21:29:51.363577 diversity-0.1.18/diversity/compression.py
+-rw-r--r--   0        0        0     3371 2024-04-02 18:19:39.171871 diversity-0.1.18/diversity/functions.py
+-rw-r--r--   0        0        0     3217 2023-11-14 16:35:10.728417 diversity-0.1.18/diversity/homogenization.py
+-rw-r--r--   0        0        0      724 2023-11-01 21:29:53.363660 diversity-0.1.18/diversity/ngram_diversity.py
+-rw-r--r--   0        0        0       84 2023-10-04 17:47:31.256275 diversity-0.1.18/diversity/patterns/__init__.py
+-rw-r--r--   0        0        0     2155 2023-10-07 17:22:30.499800 diversity-0.1.18/diversity/patterns/part_of_speech.py
+-rw-r--r--   0        0        0      821 2023-10-07 17:23:14.046690 diversity-0.1.18/diversity/patterns/token.py
+-rw-r--r--   0        0        0       30 2023-10-10 18:40:51.809862 diversity-0.1.18/diversity/utils/__init__.py
+-rw-r--r--   0        0        0      951 2024-02-26 15:03:39.741528 diversity-0.1.18/diversity/utils/memoize.py
+-rw-r--r--   0        0        0      454 2024-04-02 18:31:02.444762 diversity-0.1.18/pyproject.toml
+-rw-r--r--   0        0        0     4535 1970-01-01 00:00:00.000000 diversity-0.1.18/PKG-INFO
```

### Comparing `diversity-0.1.17/diversity/compression.py` & `diversity-0.1.18/diversity/compression.py`

 * *Files identical despite different names*

### Comparing `diversity-0.1.17/diversity/homogenization.py` & `diversity-0.1.18/diversity/homogenization.py`

 * *Files identical despite different names*

### Comparing `diversity-0.1.17/diversity/ngram_diversity.py` & `diversity-0.1.18/diversity/ngram_diversity.py`

 * *Files identical despite different names*

### Comparing `diversity-0.1.17/diversity/patterns/part_of_speech.py` & `diversity-0.1.18/diversity/patterns/part_of_speech.py`

 * *Files identical despite different names*

### Comparing `diversity-0.1.17/diversity/patterns/token.py` & `diversity-0.1.18/diversity/patterns/token.py`

 * *Files identical despite different names*

### Comparing `diversity-0.1.17/diversity/utils/memoize.py` & `diversity-0.1.18/diversity/utils/memoize.py`

 * *Files identical despite different names*

