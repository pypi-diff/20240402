# Comparing `tmp/politely-3.3.1.tar.gz` & `tmp/politely-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "politely-3.3.2.tar", max compression
```

## Comparing `politely-3.3.1.tar` & `politely-3.3.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 politely-3.3.1/politely/__init__.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 politely-3.3.1/politely/errors.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 politely-3.3.1/politely/fetchers.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 politely-3.3.1/politely/modeling_gpt2_scorer.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 politely-3.3.1/politely/modeling_heuristic_scorer.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 politely-3.3.1/politely/modeling_scorer.py
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 politely-3.3.1/politely/rules.py
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 politely-3.3.1/politely/styler.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 politely-3.3.1/.gitignore
--rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 politely-3.3.1/README.md
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 politely-3.3.1/pyproject.toml
--rw-r--r--   0        0        0    11101 2020-02-02 00:00:00.000000 politely-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0    10975 2024-04-02 08:08:10.930859 politely-3.3.2/README.md
+-rw-r--r--   0        0        0      131 2024-04-02 08:15:05.754312 politely-3.3.2/politely/__init__.py
+-rw-r--r--   0        0        0      913 2024-04-02 05:16:13.209308 politely-3.3.2/politely/errors.py
+-rw-r--r--   0        0        0      833 2024-04-02 05:16:13.209376 politely-3.3.2/politely/fetchers.py
+-rw-r--r--   0        0        0     2287 2024-04-02 05:16:13.209452 politely-3.3.2/politely/modeling_gpt2_scorer.py
+-rw-r--r--   0        0        0     1229 2024-04-02 05:16:13.209536 politely-3.3.2/politely/modeling_heuristic_scorer.py
+-rw-r--r--   0        0        0      161 2024-04-02 05:16:13.209606 politely-3.3.2/politely/modeling_scorer.py
+-rw-r--r--   0        0        0     5379 2024-04-02 08:08:10.933663 politely-3.3.2/politely/rules.py
+-rw-r--r--   0        0        0     6848 2024-04-02 08:08:10.934043 politely-3.3.2/politely/styler.py
+-rw-r--r--   0        0        0      519 2024-04-02 08:08:10.934223 politely-3.3.2/pyproject.toml
+-rw-r--r--   0        0        0    11539 1970-01-01 00:00:00.000000 politely-3.3.2/PKG-INFO
```

### Comparing `politely-3.3.1/politely/errors.py` & `politely-3.3.2/politely/errors.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.1/politely/fetchers.py` & `politely-3.3.2/politely/fetchers.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.1/politely/modeling_gpt2_scorer.py` & `politely-3.3.2/politely/modeling_gpt2_scorer.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.1/politely/modeling_heuristic_scorer.py` & `politely-3.3.2/politely/modeling_heuristic_scorer.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.1/politely/rules.py` & `politely-3.3.2/politely/rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     f"죠{TAG}EF",
     f"래요{TAG}EF",
     f"네요{TAG}EF",
     f"나요{TAG}EF",
     f"대요{TAG}EF",
     f"ᆯ게요{TAG}EF",
     f"ᆫ대요{TAG}EF",
-    f"ᆫ가요{TAG}EF"
+    f"ᆫ가요{TAG}EF",
+    f"세요{TAG}EF"
 }
 
 FORMAL = {
     f"습니다{TAG}EF",
     f"습니까{TAG}EF",
     f"랍니다{TAG}EF",
     f"ᆸ니까{TAG}EF",
@@ -218,14 +219,25 @@
             {f"ᆫ가요{TAG}EF"},
             {f"ᆸ니까{TAG}EF"}
         )
     }
 )
 
 
+# # --- 으세요 -> 으십시오 --- #
+# RULES.update(
+#     {
+#         rf"(?P<MASK>으세요{TAG}EF)": (
+#             {f"어{TAG}EF"},
+#             {f"으세요{TAG}EF"},
+#             {f"ᆸ시오{TAG}EF"}
+#         )
+#     }
+# )
+
 # ---- to be used for scoring -- #
 PREFERENCES = {
     f"어{TAG}EF",
     f"어요{TAG}EF",
     f"어요{TAG}EF",
     f"습니다{TAG}EF",
     f"ᆸ니다{TAG}EF"
```

### Comparing `politely-3.3.1/politely/styler.py` & `politely-3.3.2/politely/styler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,90 @@
 import itertools
 import os
 import re
 from copy import copy, deepcopy
 import random
 from typing import Any, List, Tuple, Dict, Set
 from functools import wraps
+from loguru import logger
 import numpy as np
 import torch
 from politely.errors import EFNotSupportedError, SFNotIncludedError, EFNotIncludedError
 from politely.fetchers import fetch_kiwi
 from politely import RULES, SEP, TAG, NULL, SELF
 from politely.modeling_gpt2_scorer import GPT2Scorer
+from politely.modeling_heuristic_scorer import HeuristicScorer
 from politely.modeling_scorer import Scorer
 from politely.rules import EFS
 
 
 def log(f):
     @wraps(f)
     def wrapper(*args, **kwargs):
-        out = f(*args, **kwargs)
         # get the function signature
+        f_out = f(*args, **kwargs)
         names = f.__code__.co_varnames[: f.__code__.co_argcount]
-        args[0].logs[f.__name__] = {"in": dict(zip(names, args)), "out": copy(args[0].out)}
-        return out
+        styler_instance: Styler = args[0]
+        # exclude self
+        styler_instance.log[f.__name__] = {"in": dict(zip(names[1:], args[1:])), "out": copy(styler_instance.out)}
+        return f_out # return the out
     return wrapper
 
 
 class Styler:
     """
     A rule-based Korean Politeness Styler
     """
-    def __init__(self, strict: bool = False, scorer: Scorer = GPT2Scorer()):
-        #  --- object-owned attributes --- #
-        self.scorer = scorer
+    def __init__(self, strict: bool = False, scorer: str = "gpt2"):
+        #  --- object-owned attributes --- #\
+        if scorer == "heuristic":
+            self.scorer: Scorer = HeuristicScorer()
+        elif scorer == "gpt2":
+            self.scorer: Scorer = GPT2Scorer()
+        else:
+            raise ValueError(f"scorer should be either 'heuristic' or 'gpt2', but got {scorer}")
         self.strict = strict
         self.out: Any = None
         self.kiwi = fetch_kiwi()
         self.rules = deepcopy(RULES)
-        self.logs = dict()
+        self.log = dict()
 
-    @log
     def __call__(self, sent: str, politeness: int) -> str:
         """
         Style a sentence with the given politeness (0, 1, 2)
         """
         self.setup() \
             .preprocess(sent) \
             .analyze() \
             .check() \
             .honorify(politeness) \
             .guess() \
+            .elect() \
             .conjugate()
         return self.out
 
     def setup(self):
         """
         Reset the out and clear all the logs,
         """
         self.out = None
-        self.logs.clear()
-        self.logs.update({"conjugations": set(), "honorifics": set()})
+        self.log.clear()
+        self.log.update({"conjugations": set(), "honorifics": set()})
         # --- seed everything --- #
         seed = 318
         random.seed(seed)
         os.environ['PYTHONHASHSEED'] = str(seed)
         np.random.seed(seed)
         torch.manual_seed(seed)
         torch.cuda.manual_seed(seed)
         torch.backends.cudnn.deterministic = True
         torch.backends.cudnn.benchmark = True
         return self
 
+    @log
     def preprocess(self, sent: str):
         """
         Make sure each sentence ends with a period, if it does not end with any SF.
         We do this to increase the accuracy of `kiwi.join`.
         """
         self.out = re.sub(r"([^!?.]+)$", r"\1.", sent.strip())
         return self
@@ -143,27 +153,37 @@
         return self
 
     @log
     def guess(self):
         """
         Guess the scores.
         """
-        self.out: List[List[str]]
-        # score each candidate
-        scores = self.scorer(self.out, self.logs, self.kiwi)
+        self.out: list[list[str]]
+        scores = self.scorer(self.out, self.log, self.kiwi)
         self.out = [(candidate, score) for candidate, score in zip(self.out, scores)]
         return self
+    
+    @log
+    def elect(self):
+        """
+        Elect the best candidate.
+        """
+        self.out: list[tuple[list[str], float]]
+        best = max(self.out, key=lambda x: x[1])
+        self.out = best
+        return self
 
+    @log
     def conjugate(self):
         """
-        Elect the best candidate and conjugate its pairs.
+        conjugate the best candidate.
         """
-        self.out: List[Tuple[List[str], float]]
-        best = max(self.out, key=lambda x: x[1])[0]
-        self.out = self.kiwi.join([(pair.split(TAG)[0], pair.split(TAG)[1]) for pair in best])
+        self.out: tuple[list[str], float]
+        sent = self.out[0]
+        self.out = self.kiwi.join([(pair.split(TAG)[0], pair.split(TAG)[1]) for pair in sent])
         return self
 
     def add_rules(self, rules: Dict[str, Tuple[Set,
                                                Set,
                                                Set]]):
         """
         Add rules to the existing rules.
```

### Comparing `politely-3.3.1/README.md` & `politely-3.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: politely
+Version: 3.3.2
+Summary: An explainable styler for the Korean language
+Author: Eu-Bin KIM
+Author-email: tlrndk123@gmail.com
+Requires-Python: >=3.9.12,<4.0.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: kiwipiepy (>=0.17.0,<0.18.0)
+Requires-Dist: torch (>=2.2.2,<3.0.0)
+Requires-Dist: transformers (>=4.39.2,<5.0.0)
+Description-Content-Type: text/markdown
+
 # Politely
 
 [![PyPI version](https://badge.fury.io/py/politely.svg)](https://badge.fury.io/py/politely)
 ![Workflow status](https://github.com/eubinecto/politely/actions/workflows/tests.yml/badge.svg)
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://eubinecto-politely-main-streamlit-4vmces.streamlitapp.com)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1tpx_wrMmzD_pWeEibeenlU4q8TuKK1j7?usp=sharing)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -132,15 +148,40 @@
 아버지께서 정실에 들어가셔요.
 [(['아버지🏷NNG', '께서🏷JKS', '정실🏷NNG', '에🏷JKB', '들어가🏷VV', '시🏷EP', '어요🏷EF', '.🏷SF'],
   0.0125),
  (['아버님🏷NNG', '께서🏷JKS', '정실🏷NNG', '에🏷JKB', '들어가🏷VV', '시🏷EP', '어요🏷EF', '.🏷SF'],
   0.0125)]
 ```
 
+### 5️⃣ Take contexts into account with the `gpt2` scorer 
+
+`heuristic` scorer is fast, but falls short at taking context into account:
+```python
+styler = Styler(scorer="heuristic")
+print("##### lm을 쓰지 않는 경우 맥락 고려 X ######")
+print(styler("내일 저랑 같이 점심 먹어요.", 0))
+```
 
+```
+##### lm을 쓰지 않는 경우 맥락 고려 X ######
+내일 나랑 같이 점심 먹어.
+```
+
+`gpt2` scorer is a bit slower, but does take context into account:
+```python
+from politely.modeling_gpt2_scorer import GPT2Scorer
+styler = Styler(scorer="gpt2")  # uses GPT2Scorer by default
+print("##### lm을 쓰는 경우 맥락 고려 O ######")
+print(styler("내일 저랑 같이 점심 먹어요.", 0))
+```
+
+```
+##### lm을 쓰는 경우 맥락 고려 O ######
+내일 나랑 같이 점심 먹자.  # 권유가 아닌 청유이므로 이게 맞음
+```
 
 ## Hosting the interactive demo 
 
 You can either host the interactive demo locally ([you first have to sign up for papago API to get your secrets](https://developers.naver.com/docs/papago/README.md))
 ```shell
 export NAVER_CLIENT_ID = ...
 export NAVER_CLIENT_SECRET = ...
@@ -156,7 +197,8 @@
 
 ## By whom? 👏
 - funded by: [Faculty of Oriental Studies](https://www.orinst.ox.ac.uk) at the University of Oxford 
 - led & developed by: [Jieun Kiaer](https://www.orinst.ox.ac.uk/people/jieun-kiaer) (Associate Professor of Korean Language and Linguistics at the University of Oxford)
 - co-developed by: Research assistant Eu-Bin KIM (Msc. in Applied Linguistics at the University of Oxford, Bsc. in AI at the University of Manchester )
 
 
+
```

### Comparing `politely-3.3.1/PKG-INFO` & `politely-3.3.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: politely
-Version: 3.3.1
-Summary: A rule-based politeness styler for the Korean Language
-Project-URL: Documentation, https://github.com/unknown/politely#readme
-Project-URL: Issues, https://github.com/unknown/politely/issues
-Project-URL: Source, https://github.com/unknown/politely
-Author-email: Eu-Bin KIM <tlrndk123@gmail.com>
-License-Expression: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Requires-Dist: cmake>=3.25.2
-Requires-Dist: kiwipiepy>=0.14.1
-Requires-Dist: torch>=2.0.1
-Requires-Dist: transformers>=4.29.1
-Description-Content-Type: text/markdown
-
 # Politely
 
 [![PyPI version](https://badge.fury.io/py/politely.svg)](https://badge.fury.io/py/politely)
 ![Workflow status](https://github.com/eubinecto/politely/actions/workflows/tests.yml/badge.svg)
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://eubinecto-politely-main-streamlit-4vmces.streamlitapp.com)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1tpx_wrMmzD_pWeEibeenlU4q8TuKK1j7?usp=sharing)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -156,15 +132,40 @@
 아버지께서 정실에 들어가셔요.
 [(['아버지🏷NNG', '께서🏷JKS', '정실🏷NNG', '에🏷JKB', '들어가🏷VV', '시🏷EP', '어요🏷EF', '.🏷SF'],
   0.0125),
  (['아버님🏷NNG', '께서🏷JKS', '정실🏷NNG', '에🏷JKB', '들어가🏷VV', '시🏷EP', '어요🏷EF', '.🏷SF'],
   0.0125)]
 ```
 
+### 5️⃣ Take contexts into account with the `gpt2` scorer 
+
+`heuristic` scorer is fast, but falls short at taking context into account:
+```python
+styler = Styler(scorer="heuristic")
+print("##### lm을 쓰지 않는 경우 맥락 고려 X ######")
+print(styler("내일 저랑 같이 점심 먹어요.", 0))
+```
+
+```
+##### lm을 쓰지 않는 경우 맥락 고려 X ######
+내일 나랑 같이 점심 먹어.
+```
+
+`gpt2` scorer is a bit slower, but does take context into account:
+```python
+from politely.modeling_gpt2_scorer import GPT2Scorer
+styler = Styler(scorer="gpt2")  # uses GPT2Scorer by default
+print("##### lm을 쓰는 경우 맥락 고려 O ######")
+print(styler("내일 저랑 같이 점심 먹어요.", 0))
+```
 
+```
+##### lm을 쓰는 경우 맥락 고려 O ######
+내일 나랑 같이 점심 먹자.  # 권유가 아닌 청유이므로 이게 맞음
+```
 
 ## Hosting the interactive demo 
 
 You can either host the interactive demo locally ([you first have to sign up for papago API to get your secrets](https://developers.naver.com/docs/papago/README.md))
 ```shell
 export NAVER_CLIENT_ID = ...
 export NAVER_CLIENT_SECRET = ...
```

