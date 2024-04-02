# Comparing `tmp/nltko-0.0.0-py2.py3-none-any.whl.zip` & `tmp/nltko-0.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,15 @@
-Zip file size: 2857 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      105 b- defN 24-Mar-21 03:40 nltko/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Mar-21 03:40 nltko/_token/__init__.py
--rw-rw-r--  2.0 unx       63 b- defN 24-Mar-21 03:40 nltko/_token/base.py
--rw-rw-r--  2.0 unx       56 b- defN 24-Mar-21 03:40 nltko/_token/code.py
--rw-rw-r--  2.0 unx     1072 b- defN 24-Mar-21 04:52 nltko-0.0.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      595 b- defN 24-Mar-21 04:52 nltko-0.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 24-Mar-21 04:52 nltko-0.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 24-Mar-21 04:52 nltko-0.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      676 b- defN 24-Mar-21 04:52 nltko-0.0.0.dist-info/RECORD
-9 files, 2683 bytes uncompressed, 1691 bytes compressed:  37.0%
+Zip file size: 8378 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      134 b- defN 24-Mar-22 07:33 nltko/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-21 10:36 nltko/_token/__init__.py
+-rw-rw-r--  2.0 unx      319 b- defN 24-Apr-02 05:03 nltko/_token/base.py
+-rw-rw-r--  2.0 unx     5778 b- defN 24-Mar-26 08:22 nltko/_token/morph.py
+-rw-rw-r--  2.0 unx     2548 b- defN 24-Mar-21 12:36 nltko/_token/news.py
+-rw-rw-r--  2.0 unx     4821 b- defN 24-Apr-02 04:55 nltko/_token/token.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-26 13:05 nltko/utils/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Mar-26 13:05 nltko/utils/base.py
+-rw-rw-r--  2.0 unx     1072 b- defN 24-Apr-02 05:03 nltko-0.0.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      740 b- defN 24-Apr-02 05:03 nltko-0.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-Apr-02 05:03 nltko-0.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 24-Apr-02 05:03 nltko-0.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      985 b- defN 24-Apr-02 05:03 nltko-0.0.1.dist-info/RECORD
+13 files, 16513 bytes uncompressed, 6740 bytes compressed:  59.2%
```

## zipnote {}

```diff
@@ -3,26 +3,38 @@
 
 Filename: nltko/_token/__init__.py
 Comment: 
 
 Filename: nltko/_token/base.py
 Comment: 
 
-Filename: nltko/_token/code.py
+Filename: nltko/_token/morph.py
 Comment: 
 
-Filename: nltko-0.0.0.dist-info/LICENSE
+Filename: nltko/_token/news.py
 Comment: 
 
-Filename: nltko-0.0.0.dist-info/METADATA
+Filename: nltko/_token/token.py
 Comment: 
 
-Filename: nltko-0.0.0.dist-info/WHEEL
+Filename: nltko/utils/__init__.py
 Comment: 
 
-Filename: nltko-0.0.0.dist-info/top_level.txt
+Filename: nltko/utils/base.py
 Comment: 
 
-Filename: nltko-0.0.0.dist-info/RECORD
+Filename: nltko-0.0.1.dist-info/LICENSE
+Comment: 
+
+Filename: nltko-0.0.1.dist-info/METADATA
+Comment: 
+
+Filename: nltko-0.0.1.dist-info/WHEEL
+Comment: 
+
+Filename: nltko-0.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: nltko-0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nltko/__init__.py

```diff
@@ -1,5 +1,6 @@
 #!/usr/bin/env python
 # -*- coding: utf-8, euc-kr -*-
 ## :e ++enc=utf-8
 
-from ._token.code import cal_sum
+from ._token.news import News
+from ._token.morph import Morph
```

## nltko/_token/base.py

```diff
@@ -1,4 +1,14 @@
 import re
 import random
+import pandas
 import itertools
-import multiprocessing
+import multiprocessing
+
+from tqdm import tqdm
+from konlpy.tag import Mecab
+from collections import Counter
+from nltk.util import bigrams
+from nltk.tokenize import word_tokenize, sent_tokenize
+
+from pytip import file_pickle, elapsed_time
+from kiwipiepy import Kiwi
```

## Comparing `nltko-0.0.0.dist-info/LICENSE` & `nltko-0.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

