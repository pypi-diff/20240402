# Comparing `tmp/qa_metrics-0.1.9.tar.gz` & `tmp/qa_metrics-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qa_metrics-0.1.9.tar", last modified: Sun Jan 21 18:27:47 2024, max compression
+gzip compressed data, was "qa_metrics-0.2.1.tar", last modified: Mon Apr  1 23:40:35 2024, max compression
```

## Comparing `qa_metrics-0.1.9.tar` & `qa_metrics-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-01-21 18:27:47.498692 qa_metrics-0.1.9/
--rw-r--r--   0 zongxiali   (501) staff       (20)     1071 2024-01-21 05:47:39.000000 qa_metrics-0.1.9/LICENSE
--rw-r--r--   0 zongxiali   (501) staff       (20)       69 2024-01-21 16:07:24.000000 qa_metrics-0.1.9/MANIFEST.in
--rw-r--r--   0 zongxiali   (501) staff       (20)      949 2024-01-21 18:27:47.497756 qa_metrics-0.1.9/PKG-INFO
--rw-r--r--   0 zongxiali   (501) staff       (20)        0 2024-01-20 16:46:16.000000 qa_metrics-0.1.9/README.md
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-01-21 18:27:47.490463 qa_metrics-0.1.9/qa_metrics/
--rw-r--r--   0 zongxiali   (501) staff       (20)     2731 2024-01-21 18:14:55.000000 qa_metrics-0.1.9/qa_metrics/__init__.py
--rw-r--r--   0 zongxiali   (501) staff       (20)    12329 2024-01-21 17:01:52.000000 qa_metrics-0.1.9/qa_metrics/cfm.py
--rw-r--r--   0 zongxiali   (501) staff       (20)      995 2024-01-21 06:57:51.000000 qa_metrics-0.1.9/qa_metrics/em.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     2449 2024-01-21 06:57:53.000000 qa_metrics-0.1.9/qa_metrics/f1.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     2448 2024-01-21 18:25:45.000000 qa_metrics-0.1.9/qa_metrics/transformerMatcher.py
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-01-21 18:27:47.495172 qa_metrics-0.1.9/qa_metrics/utils/
--rw-r--r--   0 zongxiali   (501) staff       (20)        0 2024-01-21 06:58:23.000000 qa_metrics-0.1.9/qa_metrics/utils/__init__.py
--rw-r--r--   0 zongxiali   (501) staff       (20)      680 2024-01-21 16:35:36.000000 qa_metrics-0.1.9/qa_metrics/utils/tools.py
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-01-21 18:27:47.496738 qa_metrics-0.1.9/qa_metrics.egg-info/
--rw-r--r--   0 zongxiali   (501) staff       (20)      949 2024-01-21 18:27:47.000000 qa_metrics-0.1.9/qa_metrics.egg-info/PKG-INFO
--rw-r--r--   0 zongxiali   (501) staff       (20)      370 2024-01-21 18:27:47.000000 qa_metrics-0.1.9/qa_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)        1 2024-01-21 18:27:47.000000 qa_metrics-0.1.9/qa_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       83 2024-01-21 18:27:47.000000 qa_metrics-0.1.9/qa_metrics.egg-info/requires.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       11 2024-01-21 18:27:47.000000 qa_metrics-0.1.9/qa_metrics.egg-info/top_level.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       38 2024-01-21 18:27:47.498904 qa_metrics-0.1.9/setup.cfg
--rw-r--r--   0 zongxiali   (501) staff       (20)     1281 2024-01-21 17:34:07.000000 qa_metrics-0.1.9/setup.py
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:40:35.007649 qa_metrics-0.2.1/
+-rw-r--r--   0 zongxiali   (501) staff       (20)     1071 2024-02-27 04:41:04.000000 qa_metrics-0.2.1/LICENSE
+-rw-r--r--   0 zongxiali   (501) staff       (20)       69 2024-02-27 04:41:04.000000 qa_metrics-0.2.1/MANIFEST.in
+-rw-r--r--   0 zongxiali   (501) staff       (20)     6555 2024-04-01 23:40:35.007305 qa_metrics-0.2.1/PKG-INFO
+-rw-r--r--   0 zongxiali   (501) staff       (20)     5845 2024-02-29 04:35:20.000000 qa_metrics-0.2.1/README.md
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:40:35.000704 qa_metrics-0.2.1/qa_metrics/
+-rw-r--r--   0 zongxiali   (501) staff       (20)     5330 2024-04-01 23:38:55.000000 qa_metrics-0.2.1/qa_metrics/Prompt_LLM.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     2324 2024-03-30 03:21:43.000000 qa_metrics-0.2.1/qa_metrics/__init__.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     1122 2024-03-31 05:04:42.000000 qa_metrics-0.2.1/qa_metrics/em.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     2853 2024-03-31 04:14:56.000000 qa_metrics-0.2.1/qa_metrics/f1.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)    15909 2024-04-01 21:03:35.000000 qa_metrics-0.2.1/qa_metrics/pedant.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)    14173 2024-03-30 17:42:06.000000 qa_metrics-0.2.1/qa_metrics/transformerMatcher.py
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:40:35.006056 qa_metrics-0.2.1/qa_metrics/utils/
+-rw-r--r--   0 zongxiali   (501) staff       (20)        0 2024-02-27 04:41:04.000000 qa_metrics-0.2.1/qa_metrics/utils/__init__.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     2724 2024-03-31 04:49:31.000000 qa_metrics-0.2.1/qa_metrics/utils/tools.py
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:40:35.005121 qa_metrics-0.2.1/qa_metrics.egg-info/
+-rw-r--r--   0 zongxiali   (501) staff       (20)     6555 2024-04-01 23:40:34.000000 qa_metrics-0.2.1/qa_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 zongxiali   (501) staff       (20)      398 2024-04-01 23:40:34.000000 qa_metrics-0.2.1/qa_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)        1 2024-04-01 23:40:34.000000 qa_metrics-0.2.1/qa_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)       75 2024-04-01 23:40:34.000000 qa_metrics-0.2.1/qa_metrics.egg-info/requires.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)       11 2024-04-01 23:40:34.000000 qa_metrics-0.2.1/qa_metrics.egg-info/top_level.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)       38 2024-04-01 23:40:35.007763 qa_metrics-0.2.1/setup.cfg
+-rw-r--r--   0 zongxiali   (501) staff       (20)     1296 2024-04-01 23:40:28.000000 qa_metrics-0.2.1/setup.py
```

### Comparing `qa_metrics-0.1.9/LICENSE` & `qa_metrics-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.1.9/qa_metrics/__init__.py` & `qa_metrics-0.2.1/qa_metrics/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,36 @@
 import requests
 import os
+from .utils.tools import download_link
 
-def download(model_name):
-    def download_link(file, url, name):
-        if not os.path.isfile(file):
-            print("Downloading {}...".format(name))
-            response = requests.get(url, stream=True)
-
-            if response.status_code == 200:
-                with open(file, 'wb') as f:
-                    f.write(response.content)
-                print("Download {} complete.".format(name))
-            else:
-                print("Failed to download the model. Status code:", response.status_code)
-
-    if model_name.lower() == 'bert':
-        # Download BERT model
-        model_url = 'https://drive.google.com/file/d/1ena_zUd42ju_5R3wKBidKdKuJYmF-IE_/view?usp=sharing'
-        tokenizer_url = 'https://drive.google.com/file/d/1gpmCgHKX-zLpShDr-kDrotS0Fk6F8Ht1/view?usp=sharing'
-        tokenizer_config_url = 'https://drive.google.com/file/d/1kxMwo9dD-gzgDuZMZAP64GmD_KLTofUh/view?usp=sharing'
-        config_url = 'https://drive.google.com/file/d/14d3X6BbrDrKYlnwOYBDlW7_sjK5u2Msw/view?usp=sharing'
-        vocab_url = 'https://drive.google.com/file/d/1N_kiKtJFvsIv8cwb-6ZOwXpqOi6ZLEEl/view?usp=sharing'
 
-        model_dir = os.path.join(os.path.dirname(__file__), 'transformer_models/bert')
-        model_path = os.path.join(model_dir, 'ae_tuned_bert.bin')
-        tokenizer_path = os.path.join(model_dir, 'tokenizer.json')
-        tokenizer_config_path = os.path.join(model_dir, 'tokenizer_config.json')
-        config_path = os.path.join(model_dir, 'config.json')
-        vocab_path = os.path.join(model_dir, 'vocab.txt')
-
-        if not os.path.exists(model_dir):
-            os.makedirs(model_dir)
-
-        download_link(model_path, model_url, 'Fine-tuned BERT model')
-        download_link(tokenizer_path, tokenizer_url, 'BERT tokenizer')
-        download_link(tokenizer_config_path, tokenizer_config_url, 'BERT tokenizer config')
-        download_link(config_path, config_url, 'BERT config')
-        download_link(vocab_path, vocab_url, 'BERT vocab')        
+def download(model_name):
+    # if model_name.lower() == 'bert':
+    #     # Download BERT model
+    #     model_url = 'https://drive.google.com/file/d/1ena_zUd42ju_5R3wKBidKdKuJYmF-IE_/view?usp=sharing'
+    #     tokenizer_url = 'https://drive.google.com/file/d/1gpmCgHKX-zLpShDr-kDrotS0Fk6F8Ht1/view?usp=sharing'
+    #     tokenizer_config_url = 'https://drive.google.com/file/d/1kxMwo9dD-gzgDuZMZAP64GmD_KLTofUh/view?usp=sharing'
+    #     config_url = 'https://drive.google.com/file/d/14d3X6BbrDrKYlnwOYBDlW7_sjK5u2Msw/view?usp=sharing'
+    #     vocab_url = 'https://drive.google.com/file/d/1N_kiKtJFvsIv8cwb-6ZOwXpqOi6ZLEEl/view?usp=sharing'
+
+    #     model_dir = os.path.join(os.path.dirname(__file__), 'transformer_models/bert')
+    #     model_path = os.path.join(model_dir, 'ae_tuned_bert.bin')
+    #     tokenizer_path = os.path.join(model_dir, 'tokenizer.json')
+    #     tokenizer_config_path = os.path.join(model_dir, 'tokenizer_config.json')
+    #     config_path = os.path.join(model_dir, 'config.json')
+    #     vocab_path = os.path.join(model_dir, 'vocab.txt')
+
+    #     if not os.path.exists(model_dir):
+    #         os.makedirs(model_dir)
+
+    #     download_link(model_path, model_url, 'Fine-tuned BERT model')
+    #     download_link(tokenizer_path, tokenizer_url, 'BERT tokenizer')
+    #     download_link(tokenizer_config_path, tokenizer_config_url, 'BERT tokenizer config')
+    #     download_link(config_path, config_url, 'BERT config')
+    #     download_link(vocab_path, vocab_url, 'BERT vocab')        
         
         
     if model_name.lower() == 'cfm':
         clf_url = 'https://github.com/zli12321/qa_metrics/raw/master/qa_metrics/classifier/lr_classifier'
         vectorizer_url = 'https://github.com/zli12321/qa_metrics/raw/master/qa_metrics/classifier/tf-idf_vectorizer'
         model_dir = os.path.join(os.path.dirname(__file__), 'classifier')
         model_path = os.path.join(model_dir, 'lr_classifier.pkl')
```

### Comparing `qa_metrics-0.1.9/qa_metrics/f1.py` & `qa_metrics-0.2.1/qa_metrics/f1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from .utils.tools import normalize_answer
+from .utils.tools import normalize_answer, remove_punctuation
 
+'''
+Return the F1 score, precision, and recall of the candidate answer given the reference answer
+'''
 def f1_score_with_precision_recall(reference, candidate):
     # Split the strings into sets of words
-    reference = normalize_answer(str(reference))
-    candidate = normalize_answer(str(candidate))
+    reference = remove_punctuation(normalize_answer(str(reference)))
+    candidate = remove_punctuation(normalize_answer(str(candidate)))
     words_reference = set(reference.split())
     words_candidate = set(candidate.split())
 
     # Calculate true positives, false positives, and false negatives
     tp = len(words_reference.intersection(words_candidate))
     fp = len(words_reference - words_candidate)
     fn = len(words_candidate - words_reference)
@@ -17,49 +20,55 @@
     recall = tp / (tp + fn) if (tp + fn) > 0 else 0
 
     # Calculate F1 score
     f1_score = 2 * (precision * recall) / (precision + recall) if (precision + recall) > 0 else 0
 
     return {'f1': f1_score, 'precision': precision, 'recall': recall}
 
+
+'''
+Return the F1 score of the candidate answer given the reference answer
+'''
 def f1_score(reference, candidate):
     f1_stats = f1_score_with_precision_recall(reference, candidate)
     return f1_stats['f1']
 
+
+
 '''
 Given a reference answer and a candidate answer, return True if the F1 score is greater than the threshold
 '''
 def f1_match(reference, candidate, threshold=0.5):
     if isinstance(reference, list) and isinstance(candidate, list):
-        references = [normalize_answer(str(ele)) for ele in reference]
-        candidates = [normalize_answer(str(ele)) for ele in candidate]
+        references = [remove_punctuation(normalize_answer(str(ele))) for ele in reference]
+        candidates = [remove_punctuation(normalize_answer(str(ele))) for ele in candidate]
 
         f1_scores = []
         for reference in references:
             for candidate in candidates:
                 f1_scores.append(f1_score(reference, candidate))
 
         return max(f1_scores) > threshold
     elif isinstance(reference, list):
-        references = [normalize_answer(str(ele)) for ele in reference]
-        candidate = normalize_answer(str(candidate))
+        references = [remove_punctuation(normalize_answer(str(ele))) for ele in reference]
+        candidate = remove_punctuation(normalize_answer(str(candidate)))
 
         f1_scores = []
         for reference in references:
             f1_scores.append(f1_score(reference, candidate))
 
         return max(f1_scores) > threshold
     elif isinstance(candidate, list):
-        candidates = [normalize_answer(str(ele)) for ele in candidate]
-        reference = normalize_answer(str(reference))
+        candidates = [remove_punctuation(normalize_answer(str(ele))) for ele in candidate]
+        reference = remove_punctuation(normalize_answer(str(reference)))
 
         f1_scores = []
         for candidate in candidates:
             f1_scores.append(f1_score(reference, candidate))
 
         return max(f1_scores) > threshold
     else:
-        reference = normalize_answer(str(reference))
-        candidate = normalize_answer(str(candidate))
+        reference = remove_punctuation(normalize_answer(str(reference)))
+        candidate = remove_punctuation(normalize_answer(str(candidate)))
 
         return f1_score(reference, candidate) > threshold
```

### Comparing `qa_metrics-0.1.9/setup.py` & `qa_metrics-0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import os
 
 
 setup(
     name='qa_metrics',
-    version='0.1.9',
+    version='0.2.1',
     author='Zongxia Li',
     author_email='zli12321@umd.edu',
     description='This package provides standard and classifier-based short form QA evaluation methods',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/zli12321/qa_metrics',
     packages=find_packages(),
@@ -19,22 +19,24 @@
     },
     install_requires=[
     'contractions>=0.0.1',
     'joblib',
     'requests',
     'scipy>=1.5.0',
     'scikit-learn==1.3.2',
-    'numpy==1.26.3',  # Specify numpy version here
+    'numpy'
     ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-    python_requires='>=3.7',
-)
+    python_requires='>=3.6',
+
+    )
```

