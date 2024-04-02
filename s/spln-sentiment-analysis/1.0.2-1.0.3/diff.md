# Comparing `tmp/spln_sentiment_analysis-1.0.2.tar.gz` & `tmp/spln_sentiment_analysis-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spln_sentiment_analysis-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "spln_sentiment_analysis-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spln_sentiment_analysis-1.0.2.tar` & `spln_sentiment_analysis-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      642 2024-04-02 10:23:16.978371 spln_sentiment_analysis-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1045 2024-04-02 08:15:55.566064 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/Token.py
--rw-r--r--   0        0        0      828 2024-04-02 07:06:10.417521 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/Trie.py
--rw-r--r--   0        0        0     4360 2024-04-02 10:23:29.044995 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 09:18:47.258851 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasetParsers/__init__.py
--rw-r--r--   0        0        0     1208 2024-04-01 15:04:17.775241 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasetParsers/leIA.py
--rw-r--r--   0        0        0      746 2024-04-01 14:56:51.608909 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasetParsers/linguaKit.py
--rw-r--r--   0        0        0     1593 2024-03-27 09:18:47.258851 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasetParsers/parse.py
--rw-r--r--   0        0        0     1038 2024-04-01 14:55:38.799217 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasetParsers/sentilex.py
--rw-r--r--   0        0        0     2327 2024-04-01 14:53:51.013045 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasetParsers/utils.py
--rw-r--r--   0        0        0    74107 2024-03-30 20:54:52.169711 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/LinguaKit/lex.txt
--rw-r--r--   0        0        0    74107 2024-03-30 20:52:57.013531 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/LinguaKit/train.txt
--rw-r--r--   0        0        0     1326 2024-04-02 07:06:10.417521 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/boosters.json
--rw-r--r--   0        0        0   207663 2024-03-30 21:00:47.594877 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/emojis.json
--rw-r--r--   0        0        0    27511 2024-03-27 09:18:47.255518 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/emojis.txt
--rw-r--r--   0        0        0      990 2024-03-27 09:18:47.248851 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/leIA/booster.txt
--rw-r--r--   0        0        0   132780 2024-03-27 09:18:47.248851 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/leIA/emojis.txt
--rw-r--r--   0        0        0       31 2024-03-27 09:18:47.248851 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/leIA/negate.txt
--rw-r--r--   0        0        0   427034 2024-03-30 20:45:52.748655 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/leIA/vader_lexicon.txt
--rw-r--r--   0        0        0   150578 2024-03-30 21:00:47.594877 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/lemmas.json
--rw-r--r--   0        0        0        1 2024-04-01 23:10:30.660791 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/multiplier.txt
--rw-r--r--   0        0        0       78 2024-03-30 21:00:47.591543 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/negate.json
--rw-r--r--   0        0        0  6935975 2024-03-30 21:01:09.464784 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/sentilex/sentilex.txt
--rw-r--r--   0        0        0  1710188 2024-03-30 21:00:47.798209 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/words.json
--rw-r--r--   0        0        0     4143 2024-04-02 07:35:12.800445 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/parser.py
--rw-r--r--   0        0        0   480823 2024-03-29 14:09:45.851453 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/tests/txt
--rw-r--r--   0        0        0      637 2024-04-02 08:19:10.508787 spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/utils.py
--rw-r--r--   0        0        0      308 1970-01-01 00:00:00.000000 spln_sentiment_analysis-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      642 2024-04-02 14:57:55.551564 spln_sentiment_analysis-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1210 2024-04-02 14:57:55.551564 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/Token.py
+-rw-r--r--   0        0        0      828 2024-04-02 07:06:10.417521 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/Trie.py
+-rw-r--r--   0        0        0     4361 2024-04-02 15:23:57.664132 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 09:18:47.258851 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasetParsers/__init__.py
+-rw-r--r--   0        0        0     1208 2024-04-01 15:04:17.775241 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasetParsers/leIA.py
+-rw-r--r--   0        0        0      746 2024-04-01 14:56:51.608909 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasetParsers/linguaKit.py
+-rw-r--r--   0        0        0     1593 2024-03-27 09:18:47.258851 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasetParsers/parse.py
+-rw-r--r--   0        0        0     1038 2024-04-01 14:55:38.799217 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasetParsers/sentilex.py
+-rw-r--r--   0        0        0     2327 2024-04-01 14:53:51.013045 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasetParsers/utils.py
+-rw-r--r--   0        0        0    74107 2024-03-30 20:54:52.169711 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/LinguaKit/lex.txt
+-rw-r--r--   0        0        0    74107 2024-03-30 20:52:57.013531 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/LinguaKit/train.txt
+-rw-r--r--   0        0        0     1326 2024-04-02 07:06:10.417521 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/boosters.json
+-rw-r--r--   0        0        0   207663 2024-03-30 21:00:47.594877 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/emojis.json
+-rw-r--r--   0        0        0    27511 2024-03-27 09:18:47.255518 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/emojis.txt
+-rw-r--r--   0        0        0      990 2024-03-27 09:18:47.248851 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/leIA/booster.txt
+-rw-r--r--   0        0        0   132780 2024-03-27 09:18:47.248851 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/leIA/emojis.txt
+-rw-r--r--   0        0        0       31 2024-03-27 09:18:47.248851 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/leIA/negate.txt
+-rw-r--r--   0        0        0   427034 2024-03-30 20:45:52.748655 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/leIA/vader_lexicon.txt
+-rw-r--r--   0        0        0   150578 2024-03-30 21:00:47.594877 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/lemmas.json
+-rw-r--r--   0        0        0        1 2024-04-01 23:10:30.660791 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/multiplier.txt
+-rw-r--r--   0        0        0       78 2024-03-30 21:00:47.591543 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/negate.json
+-rw-r--r--   0        0        0  6935975 2024-03-30 21:01:09.464784 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/sentilex/sentilex.txt
+-rw-r--r--   0        0        0  1710188 2024-03-30 21:00:47.798209 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/words.json
+-rw-r--r--   0        0        0     4124 2024-04-02 14:57:55.554897 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/parser.py
+-rw-r--r--   0        0        0   480823 2024-03-29 14:09:45.851453 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/tests/txt
+-rw-r--r--   0        0        0      640 2024-04-02 14:57:55.554897 spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/utils.py
+-rw-r--r--   0        0        0      308 1970-01-01 00:00:00.000000 spln_sentiment_analysis-1.0.3/PKG-INFO
```

### Comparing `spln_sentiment_analysis-1.0.2/pyproject.toml` & `spln_sentiment_analysis-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/Token.py` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/Token.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 class Modifier:
     def __init__(self, text: str, value: float):
         self.text = text
-        self.value = value
-        self.pos=0
+        self._value = abs(value)
+        self._negate = value < 0
 
     def __str__(self) -> str:
-        return f"<{self.text}|*{self.value}>"
+        return f"<{self.text}|{'-' if self._negate else ''}*{self._value}>"
 
     def is_modifier(self) -> bool:
         return True
     
+    def value(self, mask: float) -> float:
+        return pow(self._value, mask) * (-1 if self._negate else 1)
+    
     def to_tuple(self):
         return (self.text, self.value)
     
 class Base:
     def __init__(self, text: str, value: float):
         self.text = text
         self.base_value = value
@@ -25,14 +28,14 @@
         return f"<{self.text}|{'-' if self.base_value < 0 else '+'}{abs(self.base_value)}|{'-' if self._value < 0 else '+'}{abs(self._value)}>"
 
     def is_modifier(self) -> bool:
         return False
     
     def apply(self, modifier: Modifier, mask: float = 1):
         self.modifiers.append((modifier,mask))
-        self._value *= modifier.value * mask
+        self._value *= modifier.value(mask)
 
     def value(self) -> float:
         return self._value
 
     def to_tuple(self):
         return (self.text, self.value())
```

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/Trie.py` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/Trie.py`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/__init__.py` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     parser.py
     Token.py
     Trie.py
     utils.py
 
 '''
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 from .datasetParsers.parse import parseDatasets
 from .parser import analize,calibrate as calibrateFunc, normalize
 from .utils import collect,collectModifiers
 import sys
 from jjcli import *
 from .datasetParsers.utils import getDatasetFolder
@@ -134,8 +134,8 @@
     #Output two results, one for each polarity
     elif "-d" in cl.opt:
         print("POSITIVOS")
         handle_bases([b for b in bases if b.value() > 0], wordCount)
         print("\nNEGATIVOS")
         handle_bases([b for b in bases if b.value() < 0], wordCount)
     else:
-        handle_bases(bases, wordCount)
+        handle_bases(bases, wordCount)
```

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasetParsers/leIA.py` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasetParsers/leIA.py`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasetParsers/linguaKit.py` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasetParsers/linguaKit.py`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasetParsers/parse.py` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasetParsers/parse.py`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasetParsers/sentilex.py` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasetParsers/sentilex.py`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasetParsers/utils.py` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasetParsers/utils.py`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/LinguaKit/lex.txt` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/LinguaKit/lex.txt`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/LinguaKit/train.txt` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/LinguaKit/train.txt`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/boosters.json` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/boosters.json`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/emojis.json` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/emojis.json`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/emojis.txt` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/emojis.txt`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/leIA/booster.txt` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/leIA/booster.txt`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/leIA/emojis.txt` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/leIA/emojis.txt`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/leIA/vader_lexicon.txt` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/leIA/vader_lexicon.txt`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/lemmas.json` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/lemmas.json`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/sentilex/sentilex.txt` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/sentilex/sentilex.txt`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/datasets/words.json` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/datasets/words.json`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/parser.py` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,29 +67,28 @@
         else:
             sentence = sentence[1:]
         pos+=1
 
 
 
 
-def applyModifiers(bases:dict[int,Base],mod: list[Modifier]):
+def applyModifiers(bases:dict[int,Base],mod: Modifier):
     (before, after) = modify_mask
     
     for p,mask in enumerate(reversed(before)):
         pos = (p*-1)-1+mod.pos
         if pos in bases:
             bases[pos].apply(mod,mask)
             
     for p,mask in enumerate(after):
         pos = p+1+mod.pos
         if pos in bases:
             bases[pos].apply(mod,mask)
 
-    
-        
+
 
 #The modifier tokens act on the base values around them according to the modify_mask
 #Then the modified values are added together
 def evaluate(tokens: list[Base|Modifier]) -> list[Base]:
     modifiers=[]
     bases={}
     for t in tokens:
```

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/tests/txt` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/tests/txt`

 * *Files identical despite different names*

### Comparing `spln_sentiment_analysis-1.0.2/spln_sentiment_analysis/utils.py` & `spln_sentiment_analysis-1.0.3/spln_sentiment_analysis/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 
 def collect(lis: list[Base]) -> dict[str,list[Base]]:
     d=defaultdict(list)
     for i in lis:
         d[i.text].append(i)
     return d
 
-def collectModifiers(lis: list[Base]) -> dict[str,list[int]]:
+def collectModifiers(lis: list[Base]) -> dict[str,list[float]]:
     d=defaultdict(list)
     for i in lis:
         for mod,mask in i.modifiers:
-            d[mod.text].append(mod.value*mask)
+            d[mod.text].append(mod.value(mask))
     return d
```

