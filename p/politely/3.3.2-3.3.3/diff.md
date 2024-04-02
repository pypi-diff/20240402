# Comparing `tmp/politely-3.3.2.tar.gz` & `tmp/politely-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "politely-3.3.2.tar", max compression
+gzip compressed data, was "politely-3.3.3.tar", max compression
```

## Comparing `politely-3.3.2.tar` & `politely-3.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10975 2024-04-02 08:08:10.930859 politely-3.3.2/README.md
--rw-r--r--   0        0        0      131 2024-04-02 08:15:05.754312 politely-3.3.2/politely/__init__.py
--rw-r--r--   0        0        0      913 2024-04-02 05:16:13.209308 politely-3.3.2/politely/errors.py
--rw-r--r--   0        0        0      833 2024-04-02 05:16:13.209376 politely-3.3.2/politely/fetchers.py
--rw-r--r--   0        0        0     2287 2024-04-02 05:16:13.209452 politely-3.3.2/politely/modeling_gpt2_scorer.py
--rw-r--r--   0        0        0     1229 2024-04-02 05:16:13.209536 politely-3.3.2/politely/modeling_heuristic_scorer.py
--rw-r--r--   0        0        0      161 2024-04-02 05:16:13.209606 politely-3.3.2/politely/modeling_scorer.py
--rw-r--r--   0        0        0     5379 2024-04-02 08:08:10.933663 politely-3.3.2/politely/rules.py
--rw-r--r--   0        0        0     6848 2024-04-02 08:08:10.934043 politely-3.3.2/politely/styler.py
--rw-r--r--   0        0        0      519 2024-04-02 08:08:10.934223 politely-3.3.2/pyproject.toml
--rw-r--r--   0        0        0    11539 1970-01-01 00:00:00.000000 politely-3.3.2/PKG-INFO
+-rw-r--r--   0        0        0    10868 2024-04-02 12:25:21.947425 politely-3.3.3/README.md
+-rw-r--r--   0        0        0      131 2024-04-02 08:15:05.754312 politely-3.3.3/politely/__init__.py
+-rw-r--r--   0        0        0      913 2024-04-02 05:16:13.209308 politely-3.3.3/politely/errors.py
+-rw-r--r--   0        0        0      833 2024-04-02 05:16:13.209376 politely-3.3.3/politely/fetchers.py
+-rw-r--r--   0        0        0     2599 2024-04-02 13:24:50.383643 politely-3.3.3/politely/modeling_gpt2_scorer.py
+-rw-r--r--   0        0        0     1229 2024-04-02 05:16:13.209536 politely-3.3.3/politely/modeling_heuristic_scorer.py
+-rw-r--r--   0        0        0      161 2024-04-02 05:16:13.209606 politely-3.3.3/politely/modeling_scorer.py
+-rw-r--r--   0        0        0     5379 2024-04-02 08:08:10.933663 politely-3.3.3/politely/rules.py
+-rw-r--r--   0        0        0     6816 2024-04-02 11:53:14.169698 politely-3.3.3/politely/styler.py
+-rw-r--r--   0        0        0      439 2024-04-02 13:13:43.246394 politely-3.3.3/pyproject.toml
+-rw-r--r--   0        0        0    11432 1970-01-01 00:00:00.000000 politely-3.3.3/PKG-INFO
```

### Comparing `politely-3.3.2/README.md` & `politely-3.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Politely
 
 [![PyPI version](https://badge.fury.io/py/politely.svg)](https://badge.fury.io/py/politely)
 ![Workflow status](https://github.com/eubinecto/politely/actions/workflows/tests.yml/badge.svg)
-[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://eubinecto-politely-main-streamlit-4vmces.streamlitapp.com)
+[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://politely.streamlit.app)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1tpx_wrMmzD_pWeEibeenlU4q8TuKK1j7?usp=sharing)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Feubinecto%2Fpolitely&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 [![Downloads](https://pepy.tech/badge/politely)](https://pepy.tech/project/politely)
 [![Downloads](https://pepy.tech/badge/politely/week)](https://pepy.tech/project/politely)
 
 A rule-based politeness styler for the Korean language | 
@@ -146,38 +146,39 @@
 ```
 
 ```
 ##### lm을 쓰지 않는 경우 맥락 고려 X ######
 내일 나랑 같이 점심 먹어.
 ```
 
-`gpt2` scorer is a bit slower, but does take context into account:
+But `gpt2` scorer is a bit slower, but does take context into account:
 ```python
 from politely.modeling_gpt2_scorer import GPT2Scorer
 styler = Styler(scorer="gpt2")  # uses GPT2Scorer by default
 print("##### lm을 쓰는 경우 맥락 고려 O ######")
 print(styler("내일 저랑 같이 점심 먹어요.", 0))
 ```
 
 ```
 ##### lm을 쓰는 경우 맥락 고려 O ######
 내일 나랑 같이 점심 먹자.  # 권유가 아닌 청유이므로 이게 맞음
 ```
 
+More scoring options will be made available in the future. 
+
 ## Hosting the interactive demo 
 
-You can either host the interactive demo locally ([you first have to sign up for papago API to get your secrets](https://developers.naver.com/docs/papago/README.md))
+You can either host the interactive demo locally (You have to setup your own `OPENAI_API_KEY`)
 ```shell
-export NAVER_CLIENT_ID = ...
-export NAVER_CLIENT_SECRET = ...
+export OPENAI_API_KEY = ...
 # host the demo via streamlit
-streamlit run main_deploy.py
+streamlit run main_streamlit.py
 ```
 
-Or just visit [the demo we are hosting](https://eubinecto-politely-main-streamlit-4vmces.streamlitapp.com) for you | 
+Or just visit [the demo we are hosting](https://politely.streamlit.app) for you | 
 --- |
 <img width="743" alt="image" src="https://user-images.githubusercontent.com/56193069/177812857-afa40454-1afd-4b09-873f-aa9db3495d9e.png"> | 
 
 
 
 ## By whom? 👏
 - funded by: [Faculty of Oriental Studies](https://www.orinst.ox.ac.uk) at the University of Oxford
```

### Comparing `politely-3.3.2/politely/errors.py` & `politely-3.3.3/politely/errors.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.2/politely/fetchers.py` & `politely-3.3.3/politely/fetchers.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.2/politely/modeling_gpt2_scorer.py` & `politely-3.3.3/politely/modeling_gpt2_scorer.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,43 +7,64 @@
 from politely.modeling_scorer import Scorer
 
 
 class GPT2Scorer(Scorer):
     """
     More accurate than heuristic scorer, but slower.
     """
-    def __init__(self, device: str = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
-        self.gpt2 = GPT2LMHeadModel.from_pretrained('beomi/kykim-gpt3-kor-small_based_on_gpt2').to(device)
-        self.tokenizer = AutoTokenizer.from_pretrained('beomi/kykim-gpt3-kor-small_based_on_gpt2')
+
+    def __init__(
+        self, device: str = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    ):
+        self.gpt2 = GPT2LMHeadModel.from_pretrained(
+            "beomi/kykim-gpt3-kor-small_based_on_gpt2"
+        ).to(device)
+        self.tokenizer = AutoTokenizer.from_pretrained(
+            "beomi/kykim-gpt3-kor-small_based_on_gpt2"
+        )
         self.device = device
         self.gpt2.eval()
 
-    def __call__(self, candidates: List[List[str]], logs: dict, kiwi: Kiwi,
-                 # label_smoothing: https://ratsgo.github.io/insight-notes/docs/interpretable/smoothing
-                 label_smoothing: float = 0.2) -> List[float]:
+    def __call__(
+        self,
+        candidates: List[List[str]],
+        logs: dict,
+        kiwi: Kiwi,
+        # label_smoothing: https://ratsgo.github.io/insight-notes/docs/interpretable/smoothing
+        label_smoothing: float = 0.2,
+    ) -> list[float]:
         """
+        # label_smoothing: https://ratsgo.github.io/insight-notes/docs/interpretable/smoothing
         이걸 batched processing으로 바꾸고 계속하기. device parameter도 추가하기.
+        compute the negative log likelihood of the candidates.
         """
         # first, join the pairs into a sentence
         sents = [
             kiwi.join(tuple(pair.split(TAG)) for pair in candidate)
             for candidate in candidates
         ]
-        inputs = self.tokenizer(sents, return_tensors="pt", padding=True, truncation=True).to(self.device)  # (N, L)
+        inputs = self.tokenizer(
+            sents, return_tensors="pt", padding=True, truncation=True
+        ).to(
+            self.device
+        )  # (N, L)
         with torch.no_grad():
             # output the loss of each instance
             outputs = self.gpt2(**inputs)
-        logits = outputs['logits']  # (N, L, |V|)
+        logits = outputs["logits"]  # (N, L, |V|)
         # --- shift them --- #
         shift_logits = logits[:, :-1, :].contiguous()  # (N, L-1, |V|)
         shift_labels = inputs.input_ids[:, 1:].contiguous()  # (N, L-1)
         # flatten the tokens
         # TODO: use weight parameter to increase the losses for canonical ending like -습니다 / -어 / -어요
-        loss_fct = CrossEntropyLoss(reduction='none', ignore_index=self.tokenizer.pad_token_id,
-                                    label_smoothing=label_smoothing)
-        loss = loss_fct(shift_logits.view(-1, shift_logits.size(-1)), shift_labels.view(-1))
+        loss_fct = CrossEntropyLoss(
+            reduction="none",
+            ignore_index=self.tokenizer.pad_token_id,
+            label_smoothing=label_smoothing,
+        )
+        loss = loss_fct(
+            shift_logits.view(-1, shift_logits.size(-1)), shift_labels.view(-1)
+        )
         loss_by_sequence = loss.view(logits.size(0), -1).mean(dim=1)
         # negative log likelihood
-        loss_by_sequence = - loss_by_sequence
+        loss_by_sequence = -loss_by_sequence
         return loss_by_sequence.tolist()
-
-
```

### Comparing `politely-3.3.2/politely/modeling_heuristic_scorer.py` & `politely-3.3.3/politely/modeling_heuristic_scorer.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.2/politely/rules.py` & `politely-3.3.3/politely/rules.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.2/politely/styler.py` & `politely-3.3.3/politely/styler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import itertools
 import os
 import re
 from copy import copy, deepcopy
 import random
-from typing import Any, List, Tuple, Dict, Set
+from typing import Any, Tuple, Dict, Set
 from functools import wraps
-from loguru import logger
 import numpy as np
 import torch
 from politely.errors import EFNotSupportedError, SFNotIncludedError, EFNotIncludedError
 from politely.fetchers import fetch_kiwi
 from politely import RULES, SEP, TAG, NULL, SELF
 from politely.modeling_gpt2_scorer import GPT2Scorer
 from politely.modeling_heuristic_scorer import HeuristicScorer
```

### Comparing `politely-3.3.2/PKG-INFO` & `politely-3.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: politely
-Version: 3.3.2
+Version: 3.3.3
 Summary: An explainable styler for the Korean language
 Author: Eu-Bin KIM
 Author-email: tlrndk123@gmail.com
 Requires-Python: >=3.9.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: kiwipiepy (>=0.17.0,<0.18.0)
 Requires-Dist: torch (>=2.2.2,<3.0.0)
-Requires-Dist: transformers (>=4.39.2,<5.0.0)
+Requires-Dist: transformers (>=4.39.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Politely
 
 [![PyPI version](https://badge.fury.io/py/politely.svg)](https://badge.fury.io/py/politely)
 ![Workflow status](https://github.com/eubinecto/politely/actions/workflows/tests.yml/badge.svg)
-[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://eubinecto-politely-main-streamlit-4vmces.streamlitapp.com)
+[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://politely.streamlit.app)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1tpx_wrMmzD_pWeEibeenlU4q8TuKK1j7?usp=sharing)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Feubinecto%2Fpolitely&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 [![Downloads](https://pepy.tech/badge/politely)](https://pepy.tech/project/politely)
 [![Downloads](https://pepy.tech/badge/politely/week)](https://pepy.tech/project/politely)
 
 A rule-based politeness styler for the Korean language | 
@@ -162,38 +162,39 @@
 ```
 
 ```
 ##### lm을 쓰지 않는 경우 맥락 고려 X ######
 내일 나랑 같이 점심 먹어.
 ```
 
-`gpt2` scorer is a bit slower, but does take context into account:
+But `gpt2` scorer is a bit slower, but does take context into account:
 ```python
 from politely.modeling_gpt2_scorer import GPT2Scorer
 styler = Styler(scorer="gpt2")  # uses GPT2Scorer by default
 print("##### lm을 쓰는 경우 맥락 고려 O ######")
 print(styler("내일 저랑 같이 점심 먹어요.", 0))
 ```
 
 ```
 ##### lm을 쓰는 경우 맥락 고려 O ######
 내일 나랑 같이 점심 먹자.  # 권유가 아닌 청유이므로 이게 맞음
 ```
 
+More scoring options will be made available in the future. 
+
 ## Hosting the interactive demo 
 
-You can either host the interactive demo locally ([you first have to sign up for papago API to get your secrets](https://developers.naver.com/docs/papago/README.md))
+You can either host the interactive demo locally (You have to setup your own `OPENAI_API_KEY`)
 ```shell
-export NAVER_CLIENT_ID = ...
-export NAVER_CLIENT_SECRET = ...
+export OPENAI_API_KEY = ...
 # host the demo via streamlit
-streamlit run main_deploy.py
+streamlit run main_streamlit.py
 ```
 
-Or just visit [the demo we are hosting](https://eubinecto-politely-main-streamlit-4vmces.streamlitapp.com) for you | 
+Or just visit [the demo we are hosting](https://politely.streamlit.app) for you | 
 --- |
 <img width="743" alt="image" src="https://user-images.githubusercontent.com/56193069/177812857-afa40454-1afd-4b09-873f-aa9db3495d9e.png"> | 
 
 
 
 ## By whom? 👏
 - funded by: [Faculty of Oriental Studies](https://www.orinst.ox.ac.uk) at the University of Oxford
```

