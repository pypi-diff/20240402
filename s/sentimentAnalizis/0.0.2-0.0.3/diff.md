# Comparing `tmp/sentimentanalizis-0.0.2.tar.gz` & `tmp/sentimentanalizis-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentimentanalizis-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sentimentanalizis-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sentimentanalizis-0.0.2.tar` & `sentimentanalizis-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      624 2024-04-02 09:36:53.473762 sentimentanalizis-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1045 2024-04-02 08:15:55.566064 sentimentanalizis-0.0.2/sentimentAnalizis/Token.py
--rw-r--r--   0        0        0      828 2024-04-02 07:06:10.417521 sentimentanalizis-0.0.2/sentimentAnalizis/Trie.py
--rw-r--r--   0        0        0     4360 2024-04-02 09:41:49.715791 sentimentanalizis-0.0.2/sentimentAnalizis/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 09:18:47.258851 sentimentanalizis-0.0.2/sentimentAnalizis/datasetParsers/__init__.py
--rw-r--r--   0        0        0     1208 2024-04-01 15:04:17.775241 sentimentanalizis-0.0.2/sentimentAnalizis/datasetParsers/leIA.py
--rw-r--r--   0        0        0      746 2024-04-01 14:56:51.608909 sentimentanalizis-0.0.2/sentimentAnalizis/datasetParsers/linguaKit.py
--rw-r--r--   0        0        0     1593 2024-03-27 09:18:47.258851 sentimentanalizis-0.0.2/sentimentAnalizis/datasetParsers/parse.py
--rw-r--r--   0        0        0     1038 2024-04-01 14:55:38.799217 sentimentanalizis-0.0.2/sentimentAnalizis/datasetParsers/sentilex.py
--rw-r--r--   0        0        0     2327 2024-04-01 14:53:51.013045 sentimentanalizis-0.0.2/sentimentAnalizis/datasetParsers/utils.py
--rw-r--r--   0        0        0    74107 2024-03-30 20:54:52.169711 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/LinguaKit/lex.txt
--rw-r--r--   0        0        0    74107 2024-03-30 20:52:57.013531 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/LinguaKit/train.txt
--rw-r--r--   0        0        0     1326 2024-04-02 07:06:10.417521 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/boosters.json
--rw-r--r--   0        0        0   207663 2024-03-30 21:00:47.594877 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/emojis.json
--rw-r--r--   0        0        0    27511 2024-03-27 09:18:47.255518 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/emojis.txt
--rw-r--r--   0        0        0      990 2024-03-27 09:18:47.248851 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/leIA/booster.txt
--rw-r--r--   0        0        0   132780 2024-03-27 09:18:47.248851 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/leIA/emojis.txt
--rw-r--r--   0        0        0       31 2024-03-27 09:18:47.248851 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/leIA/negate.txt
--rw-r--r--   0        0        0   427034 2024-03-30 20:45:52.748655 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/leIA/vader_lexicon.txt
--rw-r--r--   0        0        0   150578 2024-03-30 21:00:47.594877 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/lemmas.json
--rw-r--r--   0        0        0        1 2024-04-01 23:10:30.660791 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/multiplier.txt
--rw-r--r--   0        0        0       78 2024-03-30 21:00:47.591543 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/negate.json
--rw-r--r--   0        0        0  6935975 2024-03-30 21:01:09.464784 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/sentilex/sentilex.txt
--rw-r--r--   0        0        0  1710188 2024-03-30 21:00:47.798209 sentimentanalizis-0.0.2/sentimentAnalizis/datasets/words.json
--rw-r--r--   0        0        0     4143 2024-04-02 07:35:12.800445 sentimentanalizis-0.0.2/sentimentAnalizis/parser.py
--rw-r--r--   0        0        0   480823 2024-03-29 14:09:45.851453 sentimentanalizis-0.0.2/sentimentAnalizis/tests/txt
--rw-r--r--   0        0        0      637 2024-04-02 08:19:10.508787 sentimentanalizis-0.0.2/sentimentAnalizis/utils.py
--rw-r--r--   0        0        0      287 1970-01-01 00:00:00.000000 sentimentanalizis-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      618 2024-04-02 09:50:03.479899 sentimentanalizis-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1045 2024-04-02 08:15:55.566064 sentimentanalizis-0.0.3/sentimentAnalizis/Token.py
+-rw-r--r--   0        0        0      828 2024-04-02 07:06:10.417521 sentimentanalizis-0.0.3/sentimentAnalizis/Trie.py
+-rw-r--r--   0        0        0     4360 2024-04-02 09:50:20.186474 sentimentanalizis-0.0.3/sentimentAnalizis/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 09:18:47.258851 sentimentanalizis-0.0.3/sentimentAnalizis/datasetParsers/__init__.py
+-rw-r--r--   0        0        0     1208 2024-04-01 15:04:17.775241 sentimentanalizis-0.0.3/sentimentAnalizis/datasetParsers/leIA.py
+-rw-r--r--   0        0        0      746 2024-04-01 14:56:51.608909 sentimentanalizis-0.0.3/sentimentAnalizis/datasetParsers/linguaKit.py
+-rw-r--r--   0        0        0     1593 2024-03-27 09:18:47.258851 sentimentanalizis-0.0.3/sentimentAnalizis/datasetParsers/parse.py
+-rw-r--r--   0        0        0     1038 2024-04-01 14:55:38.799217 sentimentanalizis-0.0.3/sentimentAnalizis/datasetParsers/sentilex.py
+-rw-r--r--   0        0        0     2327 2024-04-01 14:53:51.013045 sentimentanalizis-0.0.3/sentimentAnalizis/datasetParsers/utils.py
+-rw-r--r--   0        0        0    74107 2024-03-30 20:54:52.169711 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/LinguaKit/lex.txt
+-rw-r--r--   0        0        0    74107 2024-03-30 20:52:57.013531 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/LinguaKit/train.txt
+-rw-r--r--   0        0        0     1326 2024-04-02 07:06:10.417521 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/boosters.json
+-rw-r--r--   0        0        0   207663 2024-03-30 21:00:47.594877 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/emojis.json
+-rw-r--r--   0        0        0    27511 2024-03-27 09:18:47.255518 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/emojis.txt
+-rw-r--r--   0        0        0      990 2024-03-27 09:18:47.248851 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/leIA/booster.txt
+-rw-r--r--   0        0        0   132780 2024-03-27 09:18:47.248851 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/leIA/emojis.txt
+-rw-r--r--   0        0        0       31 2024-03-27 09:18:47.248851 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/leIA/negate.txt
+-rw-r--r--   0        0        0   427034 2024-03-30 20:45:52.748655 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/leIA/vader_lexicon.txt
+-rw-r--r--   0        0        0   150578 2024-03-30 21:00:47.594877 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/lemmas.json
+-rw-r--r--   0        0        0        1 2024-04-01 23:10:30.660791 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/multiplier.txt
+-rw-r--r--   0        0        0       78 2024-03-30 21:00:47.591543 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/negate.json
+-rw-r--r--   0        0        0  6935975 2024-03-30 21:01:09.464784 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/sentilex/sentilex.txt
+-rw-r--r--   0        0        0  1710188 2024-03-30 21:00:47.798209 sentimentanalizis-0.0.3/sentimentAnalizis/datasets/words.json
+-rw-r--r--   0        0        0     4143 2024-04-02 07:35:12.800445 sentimentanalizis-0.0.3/sentimentAnalizis/parser.py
+-rw-r--r--   0        0        0   480823 2024-03-29 14:09:45.851453 sentimentanalizis-0.0.3/sentimentAnalizis/tests/txt
+-rw-r--r--   0        0        0      637 2024-04-02 08:19:10.508787 sentimentanalizis-0.0.3/sentimentAnalizis/utils.py
+-rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 sentimentanalizis-0.0.3/PKG-INFO
```

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/Token.py` & `sentimentanalizis-0.0.3/sentimentAnalizis/Token.py`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/Trie.py` & `sentimentanalizis-0.0.3/sentimentAnalizis/Trie.py`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/__init__.py` & `sentimentanalizis-0.0.3/sentimentAnalizis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     parser.py
     Token.py
     Trie.py
     utils.py
 
 '''
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 from .datasetParsers.parse import parseDatasets
 from .parser import analize,calibrate as calibrateFunc, normalize
 from .utils import collect,collectModifiers
 import sys
 from jjcli import *
 from .datasetParsers.utils import getDatasetFolder
```

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasetParsers/leIA.py` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasetParsers/leIA.py`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasetParsers/linguaKit.py` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasetParsers/linguaKit.py`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasetParsers/parse.py` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasetParsers/parse.py`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasetParsers/sentilex.py` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasetParsers/sentilex.py`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasetParsers/utils.py` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasetParsers/utils.py`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasets/LinguaKit/lex.txt` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasets/LinguaKit/lex.txt`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasets/LinguaKit/train.txt` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasets/LinguaKit/train.txt`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasets/boosters.json` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasets/boosters.json`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasets/emojis.json` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasets/emojis.json`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasets/emojis.txt` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasets/emojis.txt`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasets/leIA/booster.txt` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasets/leIA/booster.txt`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasets/leIA/emojis.txt` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasets/leIA/emojis.txt`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasets/leIA/vader_lexicon.txt` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasets/leIA/vader_lexicon.txt`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasets/lemmas.json` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasets/lemmas.json`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasets/sentilex/sentilex.txt` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasets/sentilex/sentilex.txt`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/datasets/words.json` & `sentimentanalizis-0.0.3/sentimentAnalizis/datasets/words.json`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/parser.py` & `sentimentanalizis-0.0.3/sentimentAnalizis/parser.py`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/tests/txt` & `sentimentanalizis-0.0.3/sentimentAnalizis/tests/txt`

 * *Files identical despite different names*

### Comparing `sentimentanalizis-0.0.2/sentimentAnalizis/utils.py` & `sentimentanalizis-0.0.3/sentimentAnalizis/utils.py`

 * *Files identical despite different names*

