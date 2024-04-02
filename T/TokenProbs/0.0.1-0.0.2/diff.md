# Comparing `tmp/TokenProbs-0.0.1.tar.gz` & `tmp/TokenProbs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TokenProbs-0.0.1.tar", last modified: Tue Apr  2 18:48:23 2024, max compression
+gzip compressed data, was "TokenProbs-0.0.2.tar", last modified: Tue Apr  2 19:03:40 2024, max compression
```

## Comparing `TokenProbs-0.0.1.tar` & `TokenProbs-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-02 18:48:23.034067 TokenProbs-0.0.1/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 TokenProbs-0.0.1/LICENSE
--rw-r--r--   0 faf32    (50383) faf32    (50391)     3595 2024-04-02 18:48:23.033629 TokenProbs-0.0.1/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     3035 2024-04-02 18:40:28.000000 TokenProbs-0.0.1/README.md
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-02 18:48:23.034198 TokenProbs-0.0.1/setup.cfg
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     1194 2024-04-02 18:47:33.000000 TokenProbs-0.0.1/setup.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-02 18:48:23.030357 TokenProbs-0.0.1/src/
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-02 18:48:23.031681 TokenProbs-0.0.1/src/TokenProbs/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       41 2024-04-01 21:37:16.000000 TokenProbs-0.0.1/src/TokenProbs/__init__.py
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     8407 2024-04-02 18:29:15.000000 TokenProbs-0.0.1/src/TokenProbs/logit_extraction.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-02 18:48:23.033133 TokenProbs-0.0.1/src/TokenProbs.egg-info/
--rw-r--r--   0 faf32    (50383) faf32    (50391)     3595 2024-04-02 18:48:22.000000 TokenProbs-0.0.1/src/TokenProbs.egg-info/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)      277 2024-04-02 18:48:22.000000 TokenProbs-0.0.1/src/TokenProbs.egg-info/SOURCES.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-02 18:48:22.000000 TokenProbs-0.0.1/src/TokenProbs.egg-info/dependency_links.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-02 18:48:22.000000 TokenProbs-0.0.1/src/TokenProbs.egg-info/requires.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-02 18:48:22.000000 TokenProbs-0.0.1/src/TokenProbs.egg-info/top_level.txt
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-02 19:03:40.004032 TokenProbs-0.0.2/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 TokenProbs-0.0.2/LICENSE
+-rw-r--r--   0 faf32    (50383) faf32    (50391)     3561 2024-04-02 19:03:40.003615 TokenProbs-0.0.2/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     3001 2024-04-02 19:02:43.000000 TokenProbs-0.0.2/README.md
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-02 19:03:40.004161 TokenProbs-0.0.2/setup.cfg
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     1194 2024-04-02 19:03:31.000000 TokenProbs-0.0.2/setup.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-02 19:03:40.000235 TokenProbs-0.0.2/src/
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-02 19:03:40.001569 TokenProbs-0.0.2/src/TokenProbs/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-02 19:02:11.000000 TokenProbs-0.0.2/src/TokenProbs/__init__.py
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     8407 2024-04-02 18:29:15.000000 TokenProbs-0.0.2/src/TokenProbs/logit_extraction.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-02 19:03:40.003150 TokenProbs-0.0.2/src/TokenProbs.egg-info/
+-rw-r--r--   0 faf32    (50383) faf32    (50391)     3561 2024-04-02 19:03:39.000000 TokenProbs-0.0.2/src/TokenProbs.egg-info/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)      277 2024-04-02 19:03:39.000000 TokenProbs-0.0.2/src/TokenProbs.egg-info/SOURCES.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-02 19:03:39.000000 TokenProbs-0.0.2/src/TokenProbs.egg-info/dependency_links.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-02 19:03:39.000000 TokenProbs-0.0.2/src/TokenProbs.egg-info/requires.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-02 19:03:39.000000 TokenProbs-0.0.2/src/TokenProbs.egg-info/top_level.txt
```

### Comparing `TokenProbs-0.0.1/PKG-INFO` & `TokenProbs-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TokenProbs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,15 +27,15 @@
 ```bash
 conda create -n GenCasting python=3.9
 pip install GenCasting 
 ```
 
 ## Usage
 ```python
-from TokenProbs.logit_extraction import LogitExtractor
+from TokenProbs import LogitExtractor
 
 extractor = LogitExtractor(
     model_name = 'mistralai/Mistral-7B-Instruct-v0.1',
     quantization="8bit" # None = Full precision, "4bit" also suported
 )
 
 # Test sentence
@@ -69,15 +69,15 @@
 
 ## Additional Features
 
 `LogitExtractor` also provides functionality for applying Low-rank Adaptation (LoRA) fine-tuning tailored to extracting logit scores for next-token predictions.
 
 ```python
 from datasets import load_dataset
-from TokenProbs.logit_extraction import LogitExtractor
+from TokenProbs import LogitExtractor
 
 # Load dataset
 dataset = load_dataset("financial_phrasebank",'sentences_50agree')['train']
 # Apply training and test split
 dataset = dataset.train_test_split(seed=42)
 train = dataset['train']
```

### Comparing `TokenProbs-0.0.1/README.md` & `TokenProbs-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ```bash
 conda create -n GenCasting python=3.9
 pip install GenCasting 
 ```
 
 ## Usage
 ```python
-from TokenProbs.logit_extraction import LogitExtractor
+from TokenProbs import LogitExtractor
 
 extractor = LogitExtractor(
     model_name = 'mistralai/Mistral-7B-Instruct-v0.1',
     quantization="8bit" # None = Full precision, "4bit" also suported
 )
 
 # Test sentence
@@ -50,15 +50,15 @@
 
 ## Additional Features
 
 `LogitExtractor` also provides functionality for applying Low-rank Adaptation (LoRA) fine-tuning tailored to extracting logit scores for next-token predictions.
 
 ```python
 from datasets import load_dataset
-from TokenProbs.logit_extraction import LogitExtractor
+from TokenProbs import LogitExtractor
 
 # Load dataset
 dataset = load_dataset("financial_phrasebank",'sentences_50agree')['train']
 # Apply training and test split
 dataset = dataset.train_test_split(seed=42)
 train = dataset['train']
```

### Comparing `TokenProbs-0.0.1/setup.py` & `TokenProbs-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Extract token-level probabilities from LLMs for classification-type outputs.'
 LONG_DESCRIPTION = 'A package that allows one to extract token-level probabilities. This method can be used for example to extract sentiment class probabilities or other probability-based queries instead of parsing text-generation outputs.'
 
 # Setting up
 setup(
     name="TokenProbs",
     version=VERSION,
```

### Comparing `TokenProbs-0.0.1/src/TokenProbs/logit_extraction.py` & `TokenProbs-0.0.2/src/TokenProbs/logit_extraction.py`

 * *Files identical despite different names*

### Comparing `TokenProbs-0.0.1/src/TokenProbs.egg-info/PKG-INFO` & `TokenProbs-0.0.2/src/TokenProbs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TokenProbs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,15 +27,15 @@
 ```bash
 conda create -n GenCasting python=3.9
 pip install GenCasting 
 ```
 
 ## Usage
 ```python
-from TokenProbs.logit_extraction import LogitExtractor
+from TokenProbs import LogitExtractor
 
 extractor = LogitExtractor(
     model_name = 'mistralai/Mistral-7B-Instruct-v0.1',
     quantization="8bit" # None = Full precision, "4bit" also suported
 )
 
 # Test sentence
@@ -69,15 +69,15 @@
 
 ## Additional Features
 
 `LogitExtractor` also provides functionality for applying Low-rank Adaptation (LoRA) fine-tuning tailored to extracting logit scores for next-token predictions.
 
 ```python
 from datasets import load_dataset
-from TokenProbs.logit_extraction import LogitExtractor
+from TokenProbs import LogitExtractor
 
 # Load dataset
 dataset = load_dataset("financial_phrasebank",'sentences_50agree')['train']
 # Apply training and test split
 dataset = dataset.train_test_split(seed=42)
 train = dataset['train']
```

