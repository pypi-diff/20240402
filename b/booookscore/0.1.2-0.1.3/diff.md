# Comparing `tmp/booookscore-0.1.2.tar.gz` & `tmp/booookscore-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "booookscore-0.1.2.tar", last modified: Tue Apr  2 16:13:17 2024, max compression
+gzip compressed data, was "booookscore-0.1.3.tar", last modified: Tue Apr  2 20:55:23 2024, max compression
```

## Comparing `booookscore-0.1.2.tar` & `booookscore-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwsr-x   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)        0 2024-04-02 16:13:17.366670 booookscore-0.1.2/
--rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     1067 2024-04-02 02:21:29.000000 booookscore-0.1.2/LICENSE
--rw-r--r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)      321 2024-04-02 16:13:17.362058 booookscore-0.1.2/PKG-INFO
--rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     5958 2024-04-02 16:09:36.000000 booookscore-0.1.2/README.md
-drwxrwsr-x   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)        0 2024-04-02 16:13:17.334517 booookscore-0.1.2/booookscore/
--rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)        0 2024-03-13 23:55:14.000000 booookscore-0.1.2/booookscore/__init__.py
--rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     3671 2024-04-02 16:10:47.000000 booookscore-0.1.2/booookscore/chunk.py
--rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     1596 2024-04-02 03:18:39.000000 booookscore-0.1.2/booookscore/postprocess.py
--rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     8471 2024-04-02 03:13:54.000000 booookscore-0.1.2/booookscore/score.py
--rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)    16428 2024-04-02 16:05:23.000000 booookscore-0.1.2/booookscore/summ.py
--rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     1284 2024-04-02 02:24:11.000000 booookscore-0.1.2/booookscore/utils.py
-drwxrwsr-x   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)        0 2024-04-02 16:13:17.356160 booookscore-0.1.2/booookscore.egg-info/
--rw-r--r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)      321 2024-04-02 16:13:17.000000 booookscore-0.1.2/booookscore.egg-info/PKG-INFO
--rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)      300 2024-04-02 16:13:17.000000 booookscore-0.1.2/booookscore.egg-info/SOURCES.txt
--rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)        1 2024-04-02 16:13:17.000000 booookscore-0.1.2/booookscore.egg-info/dependency_links.txt
--rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)       12 2024-04-02 16:13:17.000000 booookscore-0.1.2/booookscore.egg-info/top_level.txt
--rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)       38 2024-04-02 16:13:17.372246 booookscore-0.1.2/setup.cfg
--rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)      504 2024-04-02 16:11:52.000000 booookscore-0.1.2/setup.py
+drwxrwsr-x   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)        0 2024-04-02 20:55:23.315140 booookscore-0.1.3/
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     1067 2024-04-02 02:21:29.000000 booookscore-0.1.3/LICENSE
+-rw-r--r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     8246 2024-04-02 20:55:23.308414 booookscore-0.1.3/PKG-INFO
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     7551 2024-04-02 20:53:04.000000 booookscore-0.1.3/README.md
+drwxrwsr-x   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)        0 2024-04-02 20:55:23.254853 booookscore-0.1.3/booookscore/
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)        0 2024-03-13 23:55:14.000000 booookscore-0.1.3/booookscore/__init__.py
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     3639 2024-04-02 19:24:48.000000 booookscore-0.1.3/booookscore/chunk.py
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     1689 2024-04-02 20:46:51.000000 booookscore-0.1.3/booookscore/postprocess.py
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     8585 2024-04-02 20:53:09.000000 booookscore-0.1.3/booookscore/score.py
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)    16557 2024-04-02 20:53:36.000000 booookscore-0.1.3/booookscore/summ.py
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     3516 2024-04-02 20:53:13.000000 booookscore-0.1.3/booookscore/utils.py
+drwxrwsr-x   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)        0 2024-04-02 20:55:23.298643 booookscore-0.1.3/booookscore.egg-info/
+-rw-r--r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)     8246 2024-04-02 20:55:22.000000 booookscore-0.1.3/booookscore.egg-info/PKG-INFO
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)      334 2024-04-02 20:55:22.000000 booookscore-0.1.3/booookscore.egg-info/SOURCES.txt
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)        1 2024-04-02 20:55:22.000000 booookscore-0.1.3/booookscore.egg-info/dependency_links.txt
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)      167 2024-04-02 20:55:22.000000 booookscore-0.1.3/booookscore.egg-info/requires.txt
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)       12 2024-04-02 20:55:22.000000 booookscore-0.1.3/booookscore.egg-info/top_level.txt
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)       38 2024-04-02 20:55:23.318010 booookscore-0.1.3/setup.cfg
+-rw-rw-r--   0 yapeichang_umass_edu  (1389) pi_miyyer_umass_edu (10067)      809 2024-04-02 20:54:53.000000 booookscore-0.1.3/setup.py
```

### Comparing `booookscore-0.1.2/LICENSE` & `booookscore-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `booookscore-0.1.2/booookscore/chunk.py` & `booookscore-0.1.3/booookscore/chunk.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,25 +87,25 @@
         if not args.include_empty_lines:
             paragraphs = [p for p in paragraphs if len(p) > 0]
         if count_tokens('\n'.join(paragraphs)) <= chunk_size:
             new_data[book] = ['\n'.join(paragraphs)]
         else:
             chunks = chunk_text(paragraphs, chunk_size)
             len_diff = count_tokens(''.join(paragraphs).replace('\n', '')) - count_tokens(''.join(chunks).replace('\n', ''))
-            assert len_diff < 100, f"Too much data lost: {len_diff}"
+            assert len_diff == 0, f"Information lost: {len_diff}"
             new_data[book] = chunks
         print(f"{book} chunk sizes: {[count_tokens(c) for c in new_data[book]]}")
         pickle.dump(new_data, open(output_path, 'wb'))
     pickle.dump(new_data, open(output_path, 'wb'))
     return new_data
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--chunk_size", type=int, default=2048)
     parser.add_argument("--input_path", type=str)
+    parser.add_argument("--output_path", type=str)
     parser.add_argument("--include_empty_lines", action="store_true")
     args = parser.parse_args()
 
-    output_path = args.input_path.replace(".pkl", f"_chunked_{args.chunk_size}.pkl")
     books = pickle.load(open(args.input_path, 'rb'))
-    process_books(books, args.chunk_size, output_path)
+    process_books(books, args.chunk_size, args.output_path)
```

### Comparing `booookscore-0.1.2/booookscore/postprocess.py` & `booookscore-0.1.3/booookscore/postprocess.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 import pickle
 import json
 import argparse
 from tqdm import tqdm
-from booookscore.utils import OpenAIClient, count_tokens
+from booookscore.utils import APIClient, count_tokens
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--input_path", type=str)
-parser.add_argument("--model", type=str, help="model name", default="gpt-4")
-parser.add_argument("--openai_key", type=str, help="openai key")
-parser.add_argument("--remove_artifacts", action="store_true", help="Whether to explicitly as a model to remove artifacts from summaries")
+parser.add_argument("--model", type=str, help="model name")
+parser.add_argument("--api", type=str, help="api to use", choices=["openai", "anthropic", "together"])
+parser.add_argument("--api_key", type=str, help="path to the api key")
+parser.add_argument("--remove_artifacts", action="store_true", help="whether to explicitly as a model to remove artifacts from summaries")
 args = parser.parse_args()
 
 if args.remove_artifacts:
-    client = OpenAIClient(args.openai_key, args.model)
+    client = APIClient(args.api, args.api_key, args.model)
     with open(f"prompts/remove_artifacts.txt", "r") as f:
         template = f.read()
 
 data = json.load(open(args.input_path, 'r'))
 save_path = args.input_path.replace('.json', '_cleaned.json')
 cleaned_summaries = {}
 if os.path.exists(save_path):
```

### Comparing `booookscore-0.1.2/booookscore/score.py` & `booookscore-0.1.3/booookscore/score.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 import traceback
 from tqdm import tqdm
 from nltk.tokenize import sent_tokenize
 from collections import defaultdict
 from typing import List, Any, Dict, Optional
 from multiprocessing.pool import ThreadPool
 from threading import Lock
-from booookscore.utils import OpenAIClient
+from booookscore.utils import APIClient
 
 
 class Scorer():
     def __init__(self,
         model,
-        openai_key,
+        api,
+        api_key,
         summ_path,
         annot_path,
         template_path,
         v2=False,
         batch_size=10
     ):
-        self.client = OpenAIClient(openai_key, model)
+        self.client = APIClient(api, api_key, model)
         self.summ_path = summ_path
         self.annot_path = annot_path
         self.template_path = template_path
         self.v2 = v2
         self.batch_size = batch_size
         self.all_labels = ['entity omission', 'event omission', 'causal omission', 'salience', 'discontinuity', 'duplication', 'inconsistency', 'language']
 
@@ -181,27 +182,29 @@
         return avg_score
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--summ_path", type=str, help="must set if you don't have annotations yet")
     parser.add_argument("--annot_path", type=str, help="path to save annotations to")
-    parser.add_argument("--openai_key", type=str, help="path to a txt file storing your OpenAI api key")
+    parser.add_argument("--api", type=str, help="api to use", choices=["openai", "anthropic", "together"])
+    parser.add_argument("--api_key", type=str, help="path to a txt file storing your OpenAI api key")
     parser.add_argument("--model", type=str, default="gpt-4", help="evaluator model")
     parser.add_argument("--v2", action="store_true", help="use v2, which batches sentences during annotation (this setup was not used in the paper)")
-    parser.add_argument("--batch_size", type=int, default=10, help="batch size if v2 is used")
+    parser.add_argument("--batch_size", type=int, help="batch size if v2 is used")
     args = parser.parse_args()
 
     if args.v2:
         template_path = "prompts/get_annotations_v2.txt"
     else:
         template_path = "prompts/get_annotations.txt"
     scorer = Scorer(
         model=args.model,
-        openai_key=args.openai_key,
+        api=args.api,
+        api_key=args.api_key,
         summ_path=args.summ_path,
         annot_path=args.annot_path,
         template_path=template_path,
         v2=args.v2,
         batch_size=args.batch_size
     )
     score = scorer.get_score()
```

### Comparing `booookscore-0.1.2/booookscore/summ.py` & `booookscore-0.1.3/booookscore/summ.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 import time
 import argparse
 import json
 import math
 import tiktoken
 from tqdm import tqdm
 from collections import defaultdict
-from booookscore.utils import OpenAIClient, count_tokens
+from utils import APIClient, count_tokens
 
 
 class Summarizer():
     def __init__(self,
         model,
-        openai_key,
+        api,
+        api_key,
         summ_path,
         method,
         chunk_size,
         max_context_len,
         max_summary_len,
         word_ratio=0.65
     ):
-        self.client = OpenAIClient(openai_key, model)
+        self.client = APIClient(api, api_key, model)
         self.summ_path = summ_path
         assert method in ['inc', 'hier']
         self.method = method
         self.chunk_size = chunk_size
         self.max_context_len = max_context_len
         self.max_summary_len = max_summary_len
         self.word_ratio = word_ratio
@@ -195,18 +196,18 @@
             if book in summaries:
                 print("Already processed, skipping...")
                 continue
             chunks = data[book]
             summaries[book] = {
                 'summaries_dict': defaultdict(list)
             }
-        final_summary, summaries = self.summarize_book(book, chunks, summaries)
-        summaries[book]['final_summary'] = final_summary
-        with open(self.summ_path, 'w') as f:
-            json.dump(summaries, f)
+            final_summary, summaries = self.summarize_book(book, chunks, summaries)
+            summaries[book]['final_summary'] = final_summary
+            with open(self.summ_path, 'w') as f:
+                json.dump(summaries, f)
 
     def compress(self, response, summary, chunk, summary_len, word_limit, num_chunks, j):
         chunk_trims = 0
         compressed_summary = None
         summary_words = len(summary.split())
         ori_expected_words = int(word_limit * j / num_chunks)  # no need to be j + 1 since we're compressing the summary at the previous chunk
         expected_words = ori_expected_words
@@ -326,24 +327,26 @@
 if __name__ == "__main__":
     encoding = tiktoken.get_encoding('cl100k_base')
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--book_path", type=str, help="path to the file containing the chunked data")
     parser.add_argument("--summ_path", type=str, help="path to the json file to save the data")
     parser.add_argument("--model", type=str, help="summarizer model")
-    parser.add_argument("--openai_key", type=str, help="path to a txt file storing your OpenAI api key")
+    parser.add_argument("--api", type=str, help="api to use", choices=["openai", "anthropic", "together"])
+    parser.add_argument("--api_key", type=str, help="path to a txt file storing your OpenAI api key")
     parser.add_argument("--method", type=str, help="method for summarization", choices=['inc', 'hier'])
     parser.add_argument("--chunk_size", type=int, default=2048)
     parser.add_argument("--max_context_len", type=int, help="max content length of the model")
     parser.add_argument("--max_summary_len", type=int, default=900, help="max length of the final summary")
     args = parser.parse_args()
 
     summarizer = Summarizer(
         args.model,
-        args.openai_key,
+        args.api,
+        args.api_key,
         args.summ_path,
         args.method,
         args.chunk_size,
         args.max_context_len,
         args.max_summary_len
     )
     summarizer.get_summaries(args.book_path)
```

