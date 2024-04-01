# Comparing `tmp/tmnt-0.7.47.tar.gz` & `tmp/tmnt-0.7.4b20231227.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmnt-0.7.47.tar", last modified: Mon Apr  1 22:23:04 2024, max compression
+gzip compressed data, was "tmnt-0.7.4b20231227.tar", last modified: Wed Dec 27 14:49:52 2023, max compression
```

## Comparing `tmnt-0.7.47.tar` & `tmnt-0.7.4b20231227.tar`

### file list

```diff
@@ -1,35 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:23:04.679832 tmnt-0.7.47/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-01 22:22:55.000000 tmnt-0.7.47/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-01 22:22:55.000000 tmnt-0.7.47/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-01 22:23:04.679832 tmnt-0.7.47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-01 22:22:55.000000 tmnt-0.7.47/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:23:04.679832 tmnt-0.7.47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-01 22:22:56.000000 tmnt-0.7.47/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:23:04.675832 tmnt-0.7.47/tmnt/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18736 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/data_loading.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    76953 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/eval_npmi.py
--rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    33018 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:23:04.675832 tmnt-0.7.47/tmnt/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/preprocess/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/preprocess/vectorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:23:04.679832 tmnt-0.7.47/tmnt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/utils/csv2json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/utils/mat_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/utils/ngram_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/utils/pubmed_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-01 22:22:56.000000 tmnt-0.7.47/tmnt/utils/recalibrate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:23:04.679832 tmnt-0.7.47/tmnt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-01 22:23:04.000000 tmnt-0.7.47/tmnt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-01 22:23:04.000000 tmnt-0.7.47/tmnt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:23:04.000000 tmnt-0.7.47/tmnt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-01 22:23:04.000000 tmnt-0.7.47/tmnt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 22:23:04.000000 tmnt-0.7.47/tmnt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:49:52.409673 tmnt-0.7.4b20231227/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-12-27 14:49:52.409673 tmnt-0.7.4b20231227/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 14:49:52.409673 tmnt-0.7.4b20231227/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:49:52.401672 tmnt-0.7.4b20231227/tmnt/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24677 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/bert_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:49:52.405673 tmnt-0.7.4b20231227/tmnt/classifier/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/classifier/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/classifier/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/classifier/train_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/common_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18569 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/data_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:49:52.405673 tmnt-0.7.4b20231227/tmnt/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19028 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/embeddings/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/embeddings/executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/embeddings/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8554 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/embeddings/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78672 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/eval_npmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18004 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32940 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:49:52.405673 tmnt-0.7.4b20231227/tmnt/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14050 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/preprocess/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/preprocess/vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25802 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:49:52.405673 tmnt-0.7.4b20231227/tmnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/utils/csv2json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/utils/mat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/utils/ngram_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/utils/pubmed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-12-27 14:49:41.000000 tmnt-0.7.4b20231227/tmnt/utils/recalibrate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 14:49:52.409673 tmnt-0.7.4b20231227/tmnt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-12-27 14:49:52.000000 tmnt-0.7.4b20231227/tmnt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-27 14:49:52.000000 tmnt-0.7.4b20231227/tmnt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 14:49:52.000000 tmnt-0.7.4b20231227/tmnt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-27 14:49:52.000000 tmnt-0.7.4b20231227/tmnt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-27 14:49:52.000000 tmnt-0.7.4b20231227/tmnt.egg-info/top_level.txt
```

### Comparing `tmnt-0.7.47/LICENSE` & `tmnt-0.7.4b20231227/LICENSE`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.47/PKG-INFO` & `tmnt-0.7.4b20231227/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: tmnt
-Version: 0.7.47
+Version: 0.7.4b20231227
 Summary: Topic modeling neural toolkit
 Home-page: https://github.com/mitre/tmnt.git
 Author: The MITRE Corporation
 Author-email: wellner@mitre.org
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: optuna
 Requires-Dist: mantichora>=0.9.5
 Requires-Dist: transformers[torch]
 Requires-Dist: torcheval
@@ -23,23 +23,21 @@
 Requires-Dist: future>=0.18.2
 Requires-Dist: funcy>=1.16
 Requires-Dist: pandas==1.5.3
 Requires-Dist: pyOpenSSL==18.0.0
 Requires-Dist: PySocks==1.6.8
 Requires-Dist: sacremoses>=0.0.38
 Requires-Dist: sentence-splitter==1.4
-Requires-Dist: umap-learn[plot]>=0.5.5
-Requires-Dist: numba
-Requires-Dist: scipy
+Requires-Dist: umap-learn==0.4.6
 Requires-Dist: tabulate>=0.8.7
-Requires-Dist: torch>=2.1.2
+Requires-Dist: torch>=1.13.0
 Requires-Dist: torchtext>=0.13.0
 
 The Topic Modeling Neural Toolkit (TMNT) is a software library that enables training
 topic models as neural network-based variational auto-encoders.
 
-Current stable version is: 0.7.46
+Current stable version is: 0.7.04
 
 Documentation can be found here: https://tmnt.readthedocs.io/en/stable/
 
 The latest development version documentation is here: https://tmnt.readthedocs.io/en/latest
```

### Comparing `tmnt-0.7.47/setup.py` & `tmnt-0.7.4b20231227/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from os import environ
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from pathlib import Path
 
-version = '0.7.47'
+version = '0.7.04'
 
 try:
     if not os.getenv('RELEASE'):
         from datetime import date
         today = date.today()
         day = today.strftime("b%Y%m%d")
         version += day
@@ -36,19 +36,17 @@
         'future>=0.18.2',
         'funcy>=1.16',
         'pandas==1.5.3',
         'pyOpenSSL==18.0.0',
         'PySocks==1.6.8',
         'sacremoses>=0.0.38',
         'sentence-splitter==1.4',
-        'umap-learn[plot]>=0.5.5',
-        'numba',
-        'scipy',
+        'umap-learn==0.4.6',
         'tabulate>=0.8.7',
-        'torch>=2.1.2',
+        'torch>=1.13.0',
         'torchtext>=0.13.0'
     ]
 
     setup(name=("tmnt"),
           version=version,
           author="The MITRE Corporation",
           author_email="wellner@mitre.org",
@@ -58,11 +56,11 @@
           url="https://github.com/mitre/tmnt.git",
           license='Apache',
           classifiers = [
               "Programming Language :: Python :: 3",
               "License :: OSI Approved :: Apache Software License",
               "Operating System :: OS Independent"
           ],
-          python_requires='>=3.10',
+          python_requires='>=3.8',
           setup_requires=setup_requires,
           install_requires=install_requires,
           packages=find_packages())
```

### Comparing `tmnt-0.7.47/tmnt/configuration.py` & `tmnt-0.7.4b20231227/tmnt/configuration.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.47/tmnt/data_loading.py` & `tmnt-0.7.4b20231227/tmnt/data_loading.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,32 +33,28 @@
 
 #### Huggingface LLM-specific dataloading ####
 
 llm_catalog = {
     'distilbert-base-uncased': (DistilBertTokenizer.from_pretrained, DistilBertModel.from_pretrained),
     'bert-base-uncased' : (AutoTokenizer.from_pretrained, BertModel.from_pretrained),
     'openai-gpt' : (AutoTokenizer.from_pretrained, OpenAIGPTModel.from_pretrained), 
-    'sentence-transformers/all-mpnet-base-v2' : (AutoTokenizer.from_pretrained, AutoModel.from_pretrained),
-    'allenai/scibert_scivocab_uncased': (AutoTokenizer.from_pretrained, AutoModel.from_pretrained),
-    'johngiorgi/declutr-sci-base': (AutoTokenizer.from_pretrained, AutoModel.from_pretrained),
-    'BAAI/bge-base-en-v1.5': (AutoTokenizer.from_pretrained, AutoModel.from_pretrained),
-    'pritamdeka/BioBERT-mnli-snli-scinli-scitail-mednli-stsb': (AutoTokenizer.from_pretrained, AutoModel.from_pretrained)
+    'sentence-transformers/all-mpnet-base-v2' : (AutoTokenizer.from_pretrained, AutoModel.from_pretrained)
     ## add more model options here if desired
     }
 
 def get_llm(model_name):
-    tok_fn, model_fn = llm_catalog.get(model_name, ((AutoTokenizer.from_pretrained, AutoModel.from_pretrained)))
+    tok_fn, model_fn = llm_catalog[model_name]
     return tok_fn(model_name), model_fn(model_name)
 
 def get_llm_tokenizer(model_name):
-    tok_fn, model_fn = llm_catalog.get(model_name, ((AutoTokenizer.from_pretrained, AutoModel.from_pretrained)))    
+    tok_fn, _ = llm_catalog[model_name]
     return tok_fn(model_name)
 
 def get_llm_model(model_name):
-    tok_fn, model_fn = llm_catalog.get(model_name, ((AutoTokenizer.from_pretrained, AutoModel.from_pretrained)))        
+    _, model_fn = llm_catalog[model_name]
     return model_fn(model_name)
 
 def get_unwrapped_llm_dataloader(data, bow_vectorizer, llm_name, label_map, batch_size, max_len, shuffle=False, device='cpu'):
     label_pipeline = lambda x: label_map.get(x, 0)
     text_pipeline  = get_llm_tokenizer(llm_name)
     
     def collate_batch(batch):
@@ -394,14 +390,27 @@
             words.append(els[0].strip())
     ln_wds = len(words)
     for i in range(ln_wds):
         w_dict[words[i]] = ln_wds - i
     return build_vocab(w_dict)
 
 
+def file_to_data(sp_file, voc_size, batch_size=1000):
+    with open(sp_file) as f:
+        for i, l in enumerate(f):
+            pass
+    data_size = i+1
+    num_batches = data_size // batch_size
+    last_batch_size = data_size % batch_size
+    X, y = load_svmlight_file(sp_file, n_features=voc_size, dtype='int32', zero_based=True)
+    wd_freqs = mx.nd.array(np.array(X.sum(axis=0)).squeeze())
+    total_words = X.sum()
+    return X, y, wd_freqs, total_words
+
+
 class StratifiedDualBatchSampler:
     """Stratified batch sampling
     Provides equal representation of target classes in each batch
     """
     def __init__(self, y_a, y_b, batch_size, num_batches, shuffle=True):
         assert len(y_a.shape) == 1 # 'label array must be 1D'
         assert len(y_b.shape) == 1
```

### Comparing `tmnt-0.7.47/tmnt/distribution.py` & `tmnt-0.7.4b20231227/tmnt/distribution.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,19 +41,28 @@
                      torch.ones(batch_size, self.n_latent)).sample().to(self.device)
         return (mu + torch.exp(0.5*lv).to(self.device) * eps)
 
     ## this is required by most priors
     def _get_unit_var_gaussian_sample(self, mu, batch_size):
         eps = Normal(torch.zeros(batch_size, self.n_latent), torch.ones(batch_size, self.n_latent)).sample()
         return (mu + eps).to(self.device)
-    
-    def get_mu_encoding(self, data, include_bn):
-        raise NotImplemented 
-
 
+    def get_mu_encoding(self, data, include_bn=False):
+        """Provide the distribution mean as the natural result of running the full encoder
+        
+        Parameters:
+            data (:class:`mxnet.ndarray.NDArray`): Output of pre-latent encoding layers
+        Returns:
+            encoding (:class:`mxnet.ndarray.NDArray`): Encoding vector representing unnormalized topic proportions
+        """
+        enc = self.mu_encoder(data)
+        if include_bn:
+            enc = self.mu_bn(enc)
+        return self.softplus(enc)
+        
 
 
 class GaussianDistribution(BaseDistribution):
     """Gaussian latent distribution with diagnol co-variance.
 
     Parameters:
         n_latent (int): Dimentionality of the latent distribution
@@ -78,29 +87,14 @@
         mu_bn = self.softplus(mu_bn)
         lv = self.lv_encoder(data)
         lv_bn = self.lv_bn(lv)
         z = self._get_gaussian_sample(mu_bn, lv_bn, batch_size)
         KL = self._get_kl_term(mu_bn, lv_bn)
         z = self.post_sample_dr_o(z)
         return z, KL
-    
-    def get_mu_encoding(self, data, include_bn=True, normalize=False):
-        """Provide the distribution mean as the natural result of running the full encoder
-        
-        Parameters:
-            data (:class:`mxnet.ndarray.NDArray`): Output of pre-latent encoding layers
-        Returns:
-            encoding (:class:`mxnet.ndarray.NDArray`): Encoding vector representing unnormalized topic proportions
-        """
-        enc = self.mu_encoder(data)
-        if include_bn:
-            enc = self.mu_bn(enc)
-        mu = self.softplus(enc) if normalize else enc
-        return mu
-        
 
 
 class GaussianUnitVarDistribution(BaseDistribution):
     """Gaussian latent distribution with fixed unit variance.
 
     Parameters:
         n_latent (int): Dimentionality of the latent distribution
@@ -122,29 +116,15 @@
         """
         mu = self.mu_encoder(data)
         mu_bn = self.mu_bn(mu)
         mu_bn = self.softplus(mu_bn)
         z = self._get_gaussian_sample(mu_bn, self.log_variance, batch_size)
         KL = self._get_kl_term(mu_bn)
         return self.post_sample_dr_o(z), KL
-    
-    def get_mu_encoding(self, data, include_bn=True, normalize=False):
-        """Provide the distribution mean as the natural result of running the full encoder
-        
-        Parameters:
-            data (:class:`mxnet.ndarray.NDArray`): Output of pre-latent encoding layers
-        Returns:
-            encoding (:class:`mxnet.ndarray.NDArray`): Encoding vector representing unnormalized topic proportions
-        """
-        enc = self.mu_encoder(data)
-        if include_bn:
-            enc = self.mu_bn(enc)
-        mu = self.softplus(enc) if normalize else enc 
-        return mu
-        
+
 
 class LogisticGaussianDistribution(BaseDistribution):
     """Logistic normal/Gaussian latent distribution with specified prior
 
     Parameters:
         n_latent (int): Dimentionality of the latent distribution
         device (device): Torch computational context (cpu or gpu[id])
@@ -180,28 +160,14 @@
         lv = self.lv_encoder(data)
         lv_bn = self.lv_bn(lv)
         z_p = self._get_gaussian_sample(mu_bn, lv_bn, batch_size)
         KL = self._get_kl_term(mu, lv)
         z = self.post_sample_dr_o(z_p)
         return self.softmax(z), KL
 
-    def get_mu_encoding(self, data, include_bn=True, normalize=False):
-        """Provide the distribution mean as the natural result of running the full encoder
-        
-        Parameters:
-            data (:class:`mxnet.ndarray.NDArray`): Output of pre-latent encoding layers
-        Returns:
-            encoding (:class:`mxnet.ndarray.NDArray`): Encoding vector representing unnormalized topic proportions
-        """
-        enc = self.mu_encoder(data)
-        if include_bn:
-            enc = self.mu_bn(enc)
-        mu = self.softmax(enc) if normalize else enc
-        return mu
-        
     
 class VonMisesDistribution(BaseDistribution):
     
     def __init__(self, enc_size, n_latent, kappa=100.0, dr=0.1, device='cpu'):
         super(VonMisesDistribution, self).__init__(enc_size, n_latent, device, on_simplex=False)
         self.device = device
         self.kappa = kappa
@@ -218,53 +184,25 @@
     def forward(self, data, batch_size):
         mu = self.mu_encoder(data)
         mu_bn = self.mu_bn(mu)
         mu_bn = self.softplus(mu_bn)
         z_p = VonMises(mu_bn, self.kappa).sample()
         kld = self.kld_v.expand(batch_size)
         return z_p, kld
-
-    def get_mu_encoding(self, data, include_bn=True, normalize=False):
-        """Provide the distribution mean as the natural result of running the full encoder
-        
-        Parameters:
-            data (:class:`mxnet.ndarray.NDArray`): Output of pre-latent encoding layers
-        Returns:
-            encoding (:class:`mxnet.ndarray.NDArray`): Encoding vector representing unnormalized topic proportions
-        """
-        enc = self.mu_encoder(data)
-        if include_bn:
-            enc = self.mu_bn(enc)
-        mu = self.softplus(enc) if normalize else enc
-        return mu
-        
     
 
 class Projection(BaseDistribution):
 
     def __init__(self, enc_size, n_latent, device='cpu'):
         super(Projection, self).__init__(enc_size, n_latent, device)
         
 
     def forward(self, data, batch_size):
         mu = self.mu_encoder(data)
         mu_bn = self.mu_bn(mu)
         kld = torch.zeros(batch_size).to(self.device)
         return mu_bn, kld
 
-    def get_mu_encoding(self, data, include_bn=True, normalize=False):
-        """Provide the distribution mean as the natural result of running the full encoder
-        
-        Parameters:
-            data (:class:`mxnet.ndarray.NDArray`): Output of pre-latent encoding layers
-        Returns:
-            encoding (:class:`mxnet.ndarray.NDArray`): Encoding vector representing unnormalized topic proportions
-        """
-        enc = self.mu_encoder(data)
-        if include_bn:
-            enc = self.mu_bn(enc)
-        return enc
-
```

### Comparing `tmnt-0.7.47/tmnt/estimator.py` & `tmnt-0.7.4b20231227/tmnt/estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,14 +296,15 @@
                 emb_size = config['derived_info'].get('embedding_size')
             if not emb_size:
                 raise Exception("Embedding size must be provided as the 'size' attribute of 'embedding' or as 'derived_info.embedding_size'")
         gamma = config.get('gamma', 1.0)
         multilabel = config.get('multilabel', False)
         lr = config['lr']
         latent_distrib = config['latent_distribution']
+        optimizer = config['optimizer']
         n_latent = int(config['n_latent'])
         enc_hidden_dim = int(config['enc_hidden_dim'])
         coherence_reg_penalty = float(config['coherence_loss_wt'])
         redundancy_reg_penalty = float(config['redundancy_loss_wt'])
         batch_size = int(config['batch_size'])
         embedding_source = config['embedding']['source']
         fixed_embedding  = config['embedding'].get('fixed') == True
@@ -321,21 +322,21 @@
         elif latent_distrib == 'vmf':
             kappa = ldist_def['kappa']
             latent_distribution = VonMisesDistribution(enc_hidden_dim, n_latent, device=device, kappa=kappa)
         else:
             latent_distribution = GaussianDistribution(enc_hidden_dim, n_latent, device=device)
         n_labels = config.get('n_labels', n_labels)
         model = \
-                cls(vocabulary=vocabulary,
+                cls(vocabulary,
                     n_labels=n_labels,
                     gamma = gamma,
                     multilabel = multilabel,
                     validate_each_epoch=validate_each_epoch,
                     coherence_coefficient=coherence_coefficient,
-                    device=device, lr=lr, latent_distribution=latent_distribution, 
+                    device=device, lr=lr, latent_distribution=latent_distribution, optimizer=optimizer,
                     enc_hidden_dim=enc_hidden_dim,
                     coherence_reg_penalty=coherence_reg_penalty,
                     redundancy_reg_penalty=redundancy_reg_penalty, batch_size=batch_size, 
                     embedding_source=embedding_source, embedding_size=emb_size, fixed_embedding=fixed_embedding,
                     num_enc_layers=n_encoding_layers, enc_dr=enc_dr, 
                     epochs=epochs, log_method='log', coherence_via_encoder=coherence_via_encoder,
                     pretrained_param_file = pretrained_param_file,
@@ -381,15 +382,15 @@
         #self.model.save_parameters(pfile)
         torch.save(self.model, pfile)
         config = self._get_config()
         specs = json.dumps(config, sort_keys=True, indent=4)
         with io.open(sp_file, 'w') as fp:
             fp.write(specs)
         with io.open(vocab_file, 'w') as fp:
-            json.dump(self.vocabulary.get_stoi(), fp)
+            json.dump(self.model.vocabulary.get_stoi(), fp)
 
 
     def _get_wd_freqs(self, X, max_sample_size=1000000):
         sample_size = min(max_sample_size, X.shape[0])
         sums = np.array(X[:sample_size].sum(axis=0))
         return sums
 
@@ -733,19 +734,31 @@
         """
         Initializes embedding weights and returns a `BowVAEModel` with hyperparameters provided.
 
         Returns:
             (:class:`BowVAEModel`) initialized using provided hyperparameters
         """
         #vocab, emb_size = self._initialize_embedding_layer(self.embedding_source, self.embedding_size)
-        emb_size = self.embedding_size
+        if self.embedding_source != 'random':
+            pt_embedding = pretrained_aliases('glove.6B.100d')
+            pretrained = pt_embedding.get_vecs_by_tokens(self.vocabulary)
+            emb_size = 100
+
+            #e_type, e_name = tuple(self.embedding_source.split(':'))
+            #pt_embedding = nlp.embedding.create(e_type, source=e_name)
+            #self.vocabulary.set_embedding(pt_embedding)
+            #emb_size = len(self.vocabulary.embedding.idx_to_vec[0])
+            #for word in self.vocabulary.embedding._idx_to_token:
+            #    if (self.vocabulary.embedding[word] == torch.zeros(emb_size)).sum() == emb_size:
+            #        self.vocabulary.embedding[word] = torch.random.normal(0, 0.1, emb_size)
+        else:
+            emb_size = self.embedding_size
         model = \
                 BowVAEModel(self.enc_hidden_dim, emb_size, n_encoding_layers=self.n_encoding_layers,
-                            vocab_size=len(self.vocabulary),
-                            enc_dr=self.enc_dr, 
+                            enc_dr=self.enc_dr, fixed_embedding=self.fixed_embedding,
                             classifier_dropout=self.classifier_dropout,
                             n_labels = self.n_labels,
                             gamma = self.gamma,
                             multilabel = self.multilabel,
                             latent_distribution=self.latent_distribution, 
                             coherence_reg_penalty=self.coherence_reg_penalty, redundancy_reg_penalty=self.redundancy_reg_penalty,
                             n_covars=0, device=self.device)
@@ -1111,16 +1124,15 @@
                  gamma=1.0,
                  multilabel=False,
                  decoder_lr = 0.01,
                  checkpoint_dir = None,
                  classifier_dropout = 0.0,
                  pure_classifier_objective = False,
                  validate_each_epoch = False,
-                 entropy_loss_coef = 0.0,
-                 pool_encoder = True,
+                 entropy_loss_coef = 1000.0,
                  **kwargs):
         super(SeqBowEstimator, self).__init__(*args, **kwargs)
         self.pure_classifier_objective = pure_classifier_objective
         self.validate_each_epoch = validate_each_epoch
         self.minimum_lr = 1e-9
         self.checkpoint_dir = checkpoint_dir
         self.llm_model_name = llm_model_name
@@ -1132,15 +1144,14 @@
         self.warmup_ratio = warmup_ratio
         self.log_interval = log_interval
         self.loss_function = torch.nn.BCEWithLogitsLoss() if multilabel else torch.nn.CrossEntropyLoss()
         self.gamma = gamma
         self.decoder_lr = decoder_lr
         self._bow_matrix = None
         self.entropy_loss_coef = entropy_loss_coef
-        self.pool_encoder = pool_encoder
 
 
     @classmethod
     def from_config(cls,
                     config: Union[str, dict],
                     vocabulary: torchtext.vocab.Vocab,
                     log_interval: int = 1,
@@ -1215,15 +1226,15 @@
         model.initialize_bias_terms(tr_bow_counts)
         return model
         
     
     def _get_model(self):
         llm_base_model = get_llm_model(self.llm_model_name).to(self.device)
         model = SeqBowVED(llm_base_model, self.latent_distribution, num_classes=self.n_labels, device=self.device, 
-                          vocab_size = len(self.vocabulary), use_pooling = self.pool_encoder,
+                          vocab_size = len(self.vocabulary), use_pooling = (self.llm_model_name.startswith("sentence-transformers")),
                           entropy_loss_coef=self.entropy_loss_coef,
                           dropout=self.classifier_dropout)
         return model
 
     def _get_config(self):
         config = {}
         config['lr'] = self.lr
@@ -1401,15 +1412,15 @@
         decay_parameters = [name for name in decay_parameters if "bias" not in name]
         non_llm_parameters = [name for name,_ in model.named_parameters() if not name.startswith("llm")]
         optimizer_grouped_parameters = [
             {
                 "params": [
                     p for n, p in model.llm.named_parameters() if (n in decay_parameters and p.requires_grad)
                 ],
-                "weight_decay": 1e-3,
+                "weight_decay": 1e-5,
             },
             { "params": [
                 p for n, p in model.llm.named_parameters() if (n not in decay_parameters and p.requires_grad)
             ],
               "weight_decay": 0.0
              }
         ]
@@ -1441,22 +1452,18 @@
         def update_loss_details(total_ls, elbo_ls, red_ls, class_ls):
             loss_details['step_loss'] += float(total_ls.mean())
             loss_details['elbo_loss'] += float(elbo_ls.mean())
             loss_details['red_loss'] += float(red_ls.mean())
             if class_ls is not None:
                 loss_details['class_loss'] += float(class_ls.mean())
             
-        sc_obj = None
-        v_res  = None
-        
         for epoch_id in range(self.epochs):
             if self.metric is not None:
                 self.metric.reset()
             model.train()
-            model.llm.train()
             
             for (batch_id, (data, aux_batch)) in enumerate(joint_loader):
                 # data_batch is either a 2-tuple of: (labeled, unlabeled)
                 # OR a 1-tuple of (labeled,)
                 
                 # forward and backward with optional auxilliary data
                 elbo_ls, rec_ls, kl_ls, red_ls, label_ls, total_ls = self._get_losses(model, data)
@@ -1465,23 +1472,21 @@
                     elbo_ls_2, rec_ls_2, kl_ls_2, red_ls_2, total_ls_2 = self._get_unlabeled_losses(model, aux_batch)
                     total_ls_2.backward()
                 else:
                     total_ls.backward()
                 update_loss_details(total_ls, elbo_ls, red_ls, label_ls)
                 if aux_batch is not None:
                     update_loss_details(total_ls_2, elbo_ls_2, red_ls_2, None)
-                    
-                #debug
 
                 if not accumulate or (batch_id + 1) % accumulate == 0:
-                    #torch.nn.utils.clip_grad.clip_grad_value_(model.llm.parameters(), 1.0)
-                    optimizer.step()
-                    dec_optimizer.step()
                     lr_scheduler.step()
+                    dec_optimizer.step()
                     model.zero_grad()
+                    # clip gradients for the underlying LLM Transformer-based encoder
+                    torch.nn.utils.clip_grad.clip_grad_value_(model.llm.parameters(), 1.0)
                     step_num += 1
                 if (batch_id + 1) % (self.log_interval) == 0:
                     lr = lr_scheduler.get_last_lr()[0] # get lr from first group
                     self.log_train(batch_id, num_train_steps // self.epochs, loss_details['step_loss'],
                                        loss_details['elbo_loss'], loss_details['red_loss'], loss_details['class_loss'], self.log_interval,
                                        epoch_id, lr)
                     ## reset loss details
@@ -1523,14 +1528,21 @@
         sc_obj = self._get_objective_from_validation_result(v_res)
         if 'accuracy' in v_res:
             self._output_status("Epoch [{}]. Objective = {} ==> PPL = {}. NPMI ={}. Redundancy = {}. Accuracy = {}."
                                 .format(epoch_id, sc_obj, v_res['ppl'], v_res['npmi'], v_res['redundancy'], v_res['accuracy']))
         else:
             self._output_status("Epoch [{}]. Objective = {} ==> PPL = {}. NPMI ={}. Redundancy = {}."
                                 .format(epoch_id, sc_obj, v_res['ppl'], v_res['npmi'], v_res['redundancy']))
+        #if self.reporter:
+        #if 'accuracy' in v_res:
+            #session.report({"objective": sc_obj, "coherence": v_res['npmi'], "perplexity": v_res['ppl'],
+            #                "redundancy": v_res['redundancy'], "accuracy": v_res['accuracy']})
+        #else:
+            #session.report({"objective": sc_obj, "coherence": v_res['npmi'], "perplexity": v_res['ppl'],
+            #            "redundancy": v_res['redundancy']})
         return sc_obj, v_res
                 
     
     def validate(self, model, dataloader):
         bow_matrix = self._bow_matrix if self._bow_matrix is not None else self._get_bow_matrix(dataloader, cache=True)
         num_words = torch.sparse.sum(bow_matrix)
         npmi, redundancy = self._compute_coherence(model, 10, bow_matrix, log_terms=True)
@@ -1568,47 +1580,50 @@
             self._output_status("Validation metric: {:.6}".format(metric_val[0]))
             v_res['accuracy'] = metric_val[0]
         return v_res, metric_nm, metric_val
 
 
 class SeqBowMetricEstimator(SeqBowEstimator):
 
-    def __init__(self, *args, sdml_smoothing_factor=0.3, metric_loss_temp=0.1, 
-                 use_sdml=False, non_scoring_index=-1, **kwargs):
+    def __init__(self, *args, sdml_smoothing_factor=0.3, metric_loss_temp=0.1, non_scoring_index=-1, **kwargs):
         super(SeqBowMetricEstimator, self).__init__(*args, **kwargs)
-        self.loss_function = \
-            GeneralizedSDMLLoss(smoothing_parameter=sdml_smoothing_factor, x2_downweight_idx=non_scoring_index) if use_sdml \
-            else MultiNegativeCrossEntropyLoss(smoothing_parameter=sdml_smoothing_factor, metric_loss_temp=metric_loss_temp)
+        #self.loss_function = GeneralizedSDMLLoss(smoothing_parameter=sdml_smoothing_factor, x2_downweight_idx=non_scoring_index)
+        self.loss_function = MultiNegativeCrossEntropyLoss(smoothing_parameter=sdml_smoothing_factor, metric_loss_temp=metric_loss_temp)
         self.non_scoring_index = non_scoring_index ## if >=0 this will avoid considering this label index in evaluation
 
 
     @classmethod
     def from_config(cls, *args, **kwargs):
         est = super().from_config(*args, **kwargs)
         return est
     
 
     def _get_model(self):
         llm_base_model = get_llm_model(self.llm_model_name).to(self.device)
         model = MetricSeqBowVED(llm_base_model, self.latent_distribution, num_classes=self.n_labels, device=self.device, 
-                                vocab_size = len(self.vocabulary), use_pooling=self.pool_encoder,
+                                vocab_size = len(self.vocabulary), use_pooling=(self.llm_model_name.startswith("sentence-transformers")),
                                 dropout=self.classifier_dropout, entropy_loss_coef=self.entropy_loss_coef)
         return model
         
     def _get_bow_wd_counts(self, dataloader):
         sums = torch.zeros(len(self.vocabulary)).to(self.device)
         for i, (data_a, data_b) in enumerate(dataloader):
             seqs_a = data_a
             bow_batch_a = seqs_a[3].to_dense()
             seqs_b = data_b
             bow_batch_b = seqs_b[3].to_dense()
             sums += bow_batch_a.sum(axis=0)
             sums += bow_batch_b.sum(axis=0)
-        return sums.cpu().numpy()        
+        return sums.cpu().numpy()                               #def _get_model_bias_initialize(self, train_data):
+    #    model = self._get_model()
+    #    tr_bow_matrix = self._get_bow_matrix(train_data)
+        #model.initialize_bias_terms(tr_bow_matrix.sum(axis=0))
+    #    return model
         
+
     def _get_bow_matrix(self, dataloader, cache=False):
         bow_matrix = []
         for _, seqs in enumerate(dataloader):
             batch_1, batch_2 = seqs                
             bow_matrix.extend(list(batch_2[3].to_dense().squeeze(axis=1)))
             bow_matrix.extend(list(batch_1[3].to_dense().squeeze(axis=1)))
         bow_matrix = torch.vstack(bow_matrix)
@@ -1654,9 +1669,14 @@
                 
 
             
     def _perform_validation(self, model, dev_data, epoch_id):
         v_res = self.validate(model, dev_data, epoch_id)
         self._output_status("Epoch [{}]. ==> elbo loss = {}; kldiv loss = {}"
                             .format(epoch_id, v_res['elbo_ls'], v_res['kl_ls']))
+        #session.report({"objective": sc_obj, "coherence": v_res['npmi'], "perplexity": v_res['ppl'],
+        #                "redundancy": v_res['redundancy']})
+        #if self.reporter:
+        #    self.reporter(epoch=epoch_id+1, objective=v_res['avg_prec'], time_step=time.time(), coherence=0.0,
+        #                  perplexity=0.0, redundancy=0.0)
         return v_res['kl_ls'], v_res
```

### Comparing `tmnt-0.7.47/tmnt/eval_npmi.py` & `tmnt-0.7.4b20231227/tmnt/eval_npmi.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.47/tmnt/inference.py` & `tmnt-0.7.4b20231227/tmnt/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,26 @@
 Inferencers to make predictions and analyze data using trained topic models.
 """
 
 import json
 import numpy as np
 import io
 import os
+import scipy
 import torch
+#import umap
+import logging
 import pickle
 from tmnt.modeling import BowVAEModel, CovariateBowVAEModel, SeqBowVED, MetricSeqBowVED
 from tmnt.estimator import BowEstimator, CovariateBowEstimator, SeqBowEstimator, SeqBowMetricEstimator
-from tmnt.data_loading import SparseDataLoader
+from tmnt.data_loading import file_to_data, SparseDataLoader
 from tmnt.preprocess.vectorizer import TMNTVectorizer
+from tmnt.distribution import LogisticGaussianDistribution
 from tmnt.utils.recalibrate import recalibrate_scores
+from multiprocessing import Pool
 from sklearn.datasets import load_svmlight_file
 from functools import partial
 from tmnt.data_loading import get_llm_tokenizer
 
 from typing import List, Tuple, Dict, Optional, Union, NoReturn
 
 
@@ -73,16 +78,16 @@
     """
     """
     def __init__(self, estimator, pre_vectorizer=None):
         super().__init__(estimator,
                          pre_vectorizer or TMNTVectorizer(initial_vocabulary=estimator.model.vocabulary),
                          estimator.model.device)
         self.max_batch_size = 16
-        self.vocab = estimator.vocabulary
-        self.n_latent = estimator.n_latent
+        self.vocab = estimator.model.vocabulary
+        self.n_latent = estimator.model.n_latent
         self.model = estimator.model
         if isinstance(estimator.model, CovariateBowVAEModel):
             self.covar_model = True
             self.n_covars = estimator.model.n_covars
             self.covar_net_layers = estimator.model.covar_net_layers
         else:
             self.covar_model = False
```

### Comparing `tmnt-0.7.47/tmnt/modeling.py` & `tmnt-0.7.4b20231227/tmnt/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,21 +86,22 @@
 class BowVAEModel(BaseVAE):
     """
     Defines the neural architecture for a bag-of-words topic model.
 
     Parameters:
         enc_dim (int): Number of dimension of input encoder (first FC layer)
         embedding_size (int): Number of dimensions for embedding layer
+        fixed_embedding (bool): Whether to fix embedding weights (default = False)
         n_encoding_layers (int): Number of layers used for the encoder. (default = 1)
         enc_dr (float): Dropout after each encoder layer. (default = 0.1)
         n_covars (int): Number of values for categorical co-variate (0 for non-CovariateData BOW model)
         device (str): context device 
     """
     def __init__(self,
-                 enc_dim, embedding_size, n_encoding_layers, enc_dr, 
+                 enc_dim, embedding_size, n_encoding_layers, enc_dr, fixed_embedding,
                  n_labels=0,
                  gamma=1.0,
                  multilabel=False,
                  classifier_dropout=0.1,
                  *args, **kwargs):
         super(BowVAEModel, self).__init__(*args, **kwargs)
         self.embedding_size = embedding_size
@@ -469,15 +470,15 @@
                  llm,
                  latent_dist,
                  num_classes=0,
                  dropout=0.0,
                  vocab_size=2000,
                  kld=0.1,
                  device='cpu',
-                 use_pooling=True,
+                 use_pooling=False,
                  entropy_loss_coef=1000.0,
                  redundancy_reg_penalty=0.0, pre_trained_embedding = None):
         super(BaseSeqBowVED, self).__init__(device=device, vocab_size=vocab_size)
         self.n_latent = latent_dist.n_latent
         self.llm = llm
         self.kld_wt = kld
         self.has_classifier = num_classes >= 2
@@ -489,17 +490,15 @@
         self.decoder = nn.Linear(self.n_latent, vocab_size, bias=True).to(device)
         self.coherence_regularization = CoherenceRegularizer(0.0, self.redundancy_reg_penalty)
         self.use_pooling = use_pooling
         self.entropy_loss_coef = entropy_loss_coef
         if pre_trained_embedding is not None:
             self.embedding = nn.Linear(len(pre_trained_embedding.idx_to_vec),
                                            pre_trained_embedding.idx_to_vec[0].size, bias=False)
-        #self.apply(self._init_weights)
-        self.latent_distribution.apply(self._init_weights)
-        self.decoder.apply(self._init_weights)
+        self.apply(self._init_weights)
 
     def _init_weights(self, module):
         if isinstance(module, torch.nn.Linear):
             torch.nn.init.xavier_uniform_(module.weight.data)
 
     def _get_embedding(self, model_output, attention_mask):
         if self.use_pooling:
@@ -591,19 +590,18 @@
         enc1 = self._get_embedding(llm_out1, mask1)
         enc2 = self._get_embedding(llm_out2, mask2)
         elbo1, rec_loss1, KL_loss1, entropy_loss1 = self._get_elbo(bow1, enc1)
         elbo2, rec_loss2, KL_loss2, entropy_loss2 = self._get_elbo(bow2, enc2)
         elbo = elbo1 + elbo2
         rec_loss = rec_loss1 + rec_loss2
         KL_loss = KL_loss1 + KL_loss2
-        #z_mu1 = self.latent_distribution.get_mu_encoding(enc2)
-        #z_mu2 = self.latent_distribution.get_mu_encoding(enc2)
+        z_mu1 = self.latent_distribution.get_mu_encoding(enc1)
+        z_mu2 = self.latent_distribution.get_mu_encoding(enc2)
         redundancy_loss = entropy_loss1 + entropy_loss2 #self.get_redundancy_penalty()
-        #return elbo, rec_loss, KL_loss, redundancy_loss, z_mu1, z_mu2
-        return elbo, rec_loss, KL_loss, redundancy_loss, enc1, enc2
+        return elbo, rec_loss, KL_loss, redundancy_loss, z_mu1, z_mu2
 
 
 class GeneralizedSDMLLoss(_Loss):
     r"""Calculates Batchwise Smoothed Deep Metric Learning (SDML) Loss given two input tensors and a smoothing weight
     SDM Loss learns similarity between paired samples by using unpaired samples in the minibatch
     as potential negative examples.
```

### Comparing `tmnt-0.7.47/tmnt/preprocess/tokenizer.py` & `tmnt-0.7.4b20231227/tmnt/preprocess/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.47/tmnt/preprocess/vectorizer.py` & `tmnt-0.7.4b20231227/tmnt/preprocess/vectorizer.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.47/tmnt/utils/csv2json.py` & `tmnt-0.7.4b20231227/tmnt/utils/csv2json.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.47/tmnt/utils/log_utils.py` & `tmnt-0.7.4b20231227/tmnt/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.47/tmnt/utils/mat_utils.py` & `tmnt-0.7.4b20231227/tmnt/utils/mat_utils.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.47/tmnt/utils/ngram_helpers.py` & `tmnt-0.7.4b20231227/tmnt/utils/ngram_helpers.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.47/tmnt/utils/pubmed_utils.py` & `tmnt-0.7.4b20231227/tmnt/utils/pubmed_utils.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.47/tmnt/utils/recalibrate.py` & `tmnt-0.7.4b20231227/tmnt/utils/recalibrate.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.47/tmnt.egg-info/PKG-INFO` & `tmnt-0.7.4b20231227/tmnt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: tmnt
-Version: 0.7.47
+Version: 0.7.4b20231227
 Summary: Topic modeling neural toolkit
 Home-page: https://github.com/mitre/tmnt.git
 Author: The MITRE Corporation
 Author-email: wellner@mitre.org
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: optuna
 Requires-Dist: mantichora>=0.9.5
 Requires-Dist: transformers[torch]
 Requires-Dist: torcheval
@@ -23,23 +23,21 @@
 Requires-Dist: future>=0.18.2
 Requires-Dist: funcy>=1.16
 Requires-Dist: pandas==1.5.3
 Requires-Dist: pyOpenSSL==18.0.0
 Requires-Dist: PySocks==1.6.8
 Requires-Dist: sacremoses>=0.0.38
 Requires-Dist: sentence-splitter==1.4
-Requires-Dist: umap-learn[plot]>=0.5.5
-Requires-Dist: numba
-Requires-Dist: scipy
+Requires-Dist: umap-learn==0.4.6
 Requires-Dist: tabulate>=0.8.7
-Requires-Dist: torch>=2.1.2
+Requires-Dist: torch>=1.13.0
 Requires-Dist: torchtext>=0.13.0
 
 The Topic Modeling Neural Toolkit (TMNT) is a software library that enables training
 topic models as neural network-based variational auto-encoders.
 
-Current stable version is: 0.7.46
+Current stable version is: 0.7.04
 
 Documentation can be found here: https://tmnt.readthedocs.io/en/stable/
 
 The latest development version documentation is here: https://tmnt.readthedocs.io/en/latest
```

