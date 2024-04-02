# Comparing `tmp/qa_metrics-0.2.5.tar.gz` & `tmp/qa_metrics-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qa_metrics-0.2.5.tar", last modified: Tue Apr  2 04:26:30 2024, max compression
+gzip compressed data, was "qa_metrics-0.2.6.tar", last modified: Tue Apr  2 05:48:32 2024, max compression
```

## Comparing `qa_metrics-0.2.5.tar` & `qa_metrics-0.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-02 04:26:30.550986 qa_metrics-0.2.5/
--rw-r--r--   0 zongxiali   (501) staff       (20)     1071 2024-02-27 04:41:04.000000 qa_metrics-0.2.5/LICENSE
--rw-r--r--   0 zongxiali   (501) staff       (20)       69 2024-02-27 04:41:04.000000 qa_metrics-0.2.5/MANIFEST.in
--rw-r--r--   0 zongxiali   (501) staff       (20)     7460 2024-04-02 04:26:30.550399 qa_metrics-0.2.5/PKG-INFO
--rw-r--r--   0 zongxiali   (501) staff       (20)     6779 2024-04-02 02:11:24.000000 qa_metrics-0.2.5/README.md
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-02 04:26:30.545838 qa_metrics-0.2.5/qa_metrics/
--rw-r--r--   0 zongxiali   (501) staff       (20)     5903 2024-04-02 04:25:55.000000 qa_metrics-0.2.5/qa_metrics/Prompt_LLM.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     2324 2024-03-30 03:21:43.000000 qa_metrics-0.2.5/qa_metrics/__init__.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     1122 2024-03-31 05:04:42.000000 qa_metrics-0.2.5/qa_metrics/em.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     2853 2024-03-31 04:14:56.000000 qa_metrics-0.2.5/qa_metrics/f1.py
--rw-r--r--   0 zongxiali   (501) staff       (20)    15909 2024-04-01 21:03:35.000000 qa_metrics-0.2.5/qa_metrics/pedant.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     1199 2024-04-02 04:21:21.000000 qa_metrics-0.2.5/qa_metrics/prompt_open_llm.py
--rw-r--r--   0 zongxiali   (501) staff       (20)    14173 2024-03-30 17:42:06.000000 qa_metrics-0.2.5/qa_metrics/transformerMatcher.py
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-02 04:26:30.549386 qa_metrics-0.2.5/qa_metrics/utils/
--rw-r--r--   0 zongxiali   (501) staff       (20)        0 2024-02-27 04:41:04.000000 qa_metrics-0.2.5/qa_metrics/utils/__init__.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     2724 2024-03-31 04:49:31.000000 qa_metrics-0.2.5/qa_metrics/utils/tools.py
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-02 04:26:30.548857 qa_metrics-0.2.5/qa_metrics.egg-info/
--rw-r--r--   0 zongxiali   (501) staff       (20)     7460 2024-04-02 04:26:30.000000 qa_metrics-0.2.5/qa_metrics.egg-info/PKG-INFO
--rw-r--r--   0 zongxiali   (501) staff       (20)      453 2024-04-02 04:26:30.000000 qa_metrics-0.2.5/qa_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)        1 2024-04-02 04:26:30.000000 qa_metrics-0.2.5/qa_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       75 2024-04-02 04:26:30.000000 qa_metrics-0.2.5/qa_metrics.egg-info/requires.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       11 2024-04-02 04:26:30.000000 qa_metrics-0.2.5/qa_metrics.egg-info/top_level.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       38 2024-04-02 04:26:30.551198 qa_metrics-0.2.5/setup.cfg
--rw-r--r--   0 zongxiali   (501) staff       (20)     1296 2024-04-02 04:24:32.000000 qa_metrics-0.2.5/setup.py
+drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:48:32.588061 qa_metrics-0.2.6/
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1071 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/LICENSE
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)       69 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/MANIFEST.in
+-rw-r--r--   0 zli12321 (14416) activetopic (18517)     8579 2024-04-02 05:48:32.588061 qa_metrics-0.2.6/PKG-INFO
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     7749 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/README.md
+drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:48:32.587061 qa_metrics-0.2.6/qa_metrics/
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2324 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/qa_metrics/__init__.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1122 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/qa_metrics/em.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2853 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/qa_metrics/f1.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)    15909 2024-04-02 05:44:58.000000 qa_metrics-0.2.6/qa_metrics/pedant.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     6541 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/qa_metrics/prompt_llm.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1201 2024-04-02 05:44:58.000000 qa_metrics-0.2.6/qa_metrics/prompt_open_llm.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)    14173 2024-04-02 05:44:58.000000 qa_metrics-0.2.6/qa_metrics/transformerMatcher.py
+drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:48:32.588061 qa_metrics-0.2.6/qa_metrics/utils/
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/qa_metrics/utils/__init__.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2724 2024-04-02 05:44:58.000000 qa_metrics-0.2.6/qa_metrics/utils/tools.py
+drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:48:32.587061 qa_metrics-0.2.6/qa_metrics.egg-info/
+-rw-r--r--   0 zli12321 (14416) activetopic (18517)     8579 2024-04-02 05:48:32.000000 qa_metrics-0.2.6/qa_metrics.egg-info/PKG-INFO
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)      428 2024-04-02 05:48:32.000000 qa_metrics-0.2.6/qa_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)        1 2024-04-02 05:48:32.000000 qa_metrics-0.2.6/qa_metrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)       75 2024-04-02 05:48:32.000000 qa_metrics-0.2.6/qa_metrics.egg-info/requires.txt
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)       11 2024-04-02 05:48:32.000000 qa_metrics-0.2.6/qa_metrics.egg-info/top_level.txt
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)       38 2024-04-02 05:48:32.588061 qa_metrics-0.2.6/setup.cfg
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1296 2024-04-02 05:48:22.000000 qa_metrics-0.2.6/setup.py
```

### Comparing `qa_metrics-0.2.5/LICENSE` & `qa_metrics-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.5/PKG-INFO` & `qa_metrics-0.2.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qa_metrics
-Version: 0.2.5
+Version: 0.2.6
 Summary: This package provides standard and classifier-based short form QA evaluation methods
 Home-page: https://github.com/zli12321/qa_metrics
 Author: Zongxia Li
 Author-email: zli12321@umd.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,23 +14,30 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: contractions>=0.0.1
+Requires-Dist: joblib
+Requires-Dist: requests
+Requires-Dist: scipy>=1.5.0
+Requires-Dist: scikit-learn==1.3.2
+Requires-Dist: numpy
 
 # QA-Evaluation-Metrics
 
 [![PyPI version qa-metrics](https://img.shields.io/pypi/v/qa-metrics.svg)](https://pypi.org/project/qa-metrics/) 
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17b7vrZqH0Yun2AJaOXydYZxr3cw20Ga6?usp=sharing)
 
-QA-Evaluation-Metrics is a fast and lightweight Python package for evaluating question-answering models and prompting of black-box large language models. It provides various basic metrics to assess the performance of QA models. Check out our paper [**PANDA**](https://arxiv.org/abs/2402.11161), an efficient QA evaluation that retains competitive evaluation performance of transformer LLM models. 
+QA-Evaluation-Metrics is a fast and lightweight Python package for evaluating question-answering models and prompting of black-box and open-source large language models. It provides various basic metrics to assess the performance of QA models. Check out our paper [**PANDA**](https://arxiv.org/abs/2402.11161), an efficient QA evaluation that retains competitive evaluation performance of transformer LLM models. 
 
-- 🔥 Our package also supports prompting of OPENAI GPT-series models and Claude Series models now.
+- 🔥 Our package also supports prompting OPENAI GPT-series models and Claude Series models now. (Assuimg OPENAI version > 1.0)
+- 🔥 Our package supports prompting various open source models such as LLaMA-2-70B-chat, LLaVA-1.5 etc by calling API from [deepinfra](https://deepinfra.com/models).
 
 
 ## Installation
 
 To install the package, run the following command:
 
 ```bash
@@ -43,34 +50,47 @@
 
 #### Prompting LLM For Evaluation
 
 Note: The prompting function can be used for any prompting purposes.
 
 ###### OpenAI
 ```python
-from qa_metrics.prompt_llm import *
-set_openai_api_key(YOUR_OPENAI_KEY)
+from qa_metrics.prompt_llm import CloseLLM
+model = CloseLLM()
+model.set_openai_api_key(YOUR_OPENAI_KEY)
 prompt = 'question: What is the Capital of France?\nreference: Paris\ncandidate: The capital is Paris\nIs the candidate answer correct based on the question and reference answer? Please only output correct or incorrect.'
-prompt_gpt(prompt=prompt, model_engine='gpt-3.5-turbo', temperature=0.1, max_token=10)
+model.prompt_gpt(prompt=prompt, model_engine='gpt-3.5-turbo', temperature=0.1, max_tokens=10)
 
 '''
 'correct'
 '''
 ```
 
 ###### Anthropic
 ```python
-set_anthropic_api_key(YOUR_OPENAI_KEY)
-prompt_claude(prompt=prompt, model_engine='claude-v1', anthropic_version="2023-06-01", max_tokens_to_sample=100, temperature=0.7)
+model = CloseLLM()
+model.set_anthropic_api_key(YOUR_Anthropic_KEY)
+model.prompt_claude(prompt=prompt, model_engine='claude-v1', anthropic_version="2023-06-01", max_tokens_to_sample=100, temperature=0.7)
 
 '''
 'correct'
 '''
 ```
 
+###### deepinfra (See below for descriptions of more models)
+```python
+from qa_metrics.prompt_open_llm import OpenLLM
+model = OpenLLM()
+model.set_deepinfra_api_key(YOUR_OPENAI_KEY)
+model.prompt(prompt=prompt, model_engine='mistralai/Mixtral-8x7B-Instruct-v0.1', temperature=0.1, max_tokens=10)
+
+'''
+'correct'
+'''
+```
 
 #### Exact Match
 ```python
 from qa_metrics.em import em_match
 
 reference_answer = ["The Frog Prince", "The Princess and the Frog"]
 candidate_answer = "The movie \"The Princess and the Frog\" is loosely based off the Brother Grimm's \"Iron Henry\""
@@ -152,14 +172,16 @@
 
 ## Updates
 - Improved PANDA evaluation with more representative answer correctness training data.
 - 🔥 The full paper is uploaded and can be accessed [here](https://arxiv.org/abs/2402.11161). The dataset is expanded and leaderboard is updated.
 - Our Training Dataset is adapted and augmented from [Bulian et al](https://github.com/google-research-datasets/answer-equivalence-dataset). Our [dataset repo](https://github.com/zli12321/Answer_Equivalence_Dataset.git) includes the augmented training set and QA evaluation testing sets discussed in our paper.
 - Now our model supports [distilroberta](https://huggingface.co/Zongxia/answer_equivalence_distilroberta), [distilbert](https://huggingface.co/Zongxia/answer_equivalence_distilbert), a smaller and faster matching model than Bert!
 - Now our model supports [roberta](https://huggingface.co/Zongxia/answer_equivalence_roberta), [roberta-large](https://huggingface.co/Zongxia/answer_equivalence_roberta-large), a larger and more robust matching model than Bert!
+- Check avilability of open-source LLMs in [deepinfra](https://deepinfra.com/models)
+- deepinfra supports: "lizpreciatior/lzlv_70b_fp16_hf", "meta-llama/Llama-2-70b-chat-hf", "meta-llama/Llama-2-7b-chat-hf", "meta-llama/Llama-2-13b-chat-hf", "01-ai/Yi-34B-Chat", "google/gemma-7b-it", "llava-hf/llava-1.5-7b-hf", "mistralai/Mixtral-8x7B-Instruct-v0.1"
 
 ## License
 
 This project is licensed under the [MIT License](LICENSE.md) - see the LICENSE file for details.
 
 ## Contact
```

### Comparing `qa_metrics-0.2.5/README.md` & `qa_metrics-0.2.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # QA-Evaluation-Metrics
 
 [![PyPI version qa-metrics](https://img.shields.io/pypi/v/qa-metrics.svg)](https://pypi.org/project/qa-metrics/) 
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17b7vrZqH0Yun2AJaOXydYZxr3cw20Ga6?usp=sharing)
 
-QA-Evaluation-Metrics is a fast and lightweight Python package for evaluating question-answering models and prompting of black-box large language models. It provides various basic metrics to assess the performance of QA models. Check out our paper [**PANDA**](https://arxiv.org/abs/2402.11161), an efficient QA evaluation that retains competitive evaluation performance of transformer LLM models. 
+QA-Evaluation-Metrics is a fast and lightweight Python package for evaluating question-answering models and prompting of black-box and open-source large language models. It provides various basic metrics to assess the performance of QA models. Check out our paper [**PANDA**](https://arxiv.org/abs/2402.11161), an efficient QA evaluation that retains competitive evaluation performance of transformer LLM models. 
 
-- 🔥 Our package also supports prompting of OPENAI GPT-series models and Claude Series models now.
+- 🔥 Our package also supports prompting OPENAI GPT-series models and Claude Series models now. (Assuimg OPENAI version > 1.0)
+- 🔥 Our package supports prompting various open source models such as LLaMA-2-70B-chat, LLaVA-1.5 etc by calling API from [deepinfra](https://deepinfra.com/models).
 
 
 ## Installation
 
 To install the package, run the following command:
 
 ```bash
@@ -22,34 +23,47 @@
 
 #### Prompting LLM For Evaluation
 
 Note: The prompting function can be used for any prompting purposes.
 
 ###### OpenAI
 ```python
-from qa_metrics.prompt_llm import *
-set_openai_api_key(YOUR_OPENAI_KEY)
+from qa_metrics.prompt_llm import CloseLLM
+model = CloseLLM()
+model.set_openai_api_key(YOUR_OPENAI_KEY)
 prompt = 'question: What is the Capital of France?\nreference: Paris\ncandidate: The capital is Paris\nIs the candidate answer correct based on the question and reference answer? Please only output correct or incorrect.'
-prompt_gpt(prompt=prompt, model_engine='gpt-3.5-turbo', temperature=0.1, max_token=10)
+model.prompt_gpt(prompt=prompt, model_engine='gpt-3.5-turbo', temperature=0.1, max_tokens=10)
 
 '''
 'correct'
 '''
 ```
 
 ###### Anthropic
 ```python
-set_anthropic_api_key(YOUR_OPENAI_KEY)
-prompt_claude(prompt=prompt, model_engine='claude-v1', anthropic_version="2023-06-01", max_tokens_to_sample=100, temperature=0.7)
+model = CloseLLM()
+model.set_anthropic_api_key(YOUR_Anthropic_KEY)
+model.prompt_claude(prompt=prompt, model_engine='claude-v1', anthropic_version="2023-06-01", max_tokens_to_sample=100, temperature=0.7)
 
 '''
 'correct'
 '''
 ```
 
+###### deepinfra (See below for descriptions of more models)
+```python
+from qa_metrics.prompt_open_llm import OpenLLM
+model = OpenLLM()
+model.set_deepinfra_api_key(YOUR_OPENAI_KEY)
+model.prompt(prompt=prompt, model_engine='mistralai/Mixtral-8x7B-Instruct-v0.1', temperature=0.1, max_tokens=10)
+
+'''
+'correct'
+'''
+```
 
 #### Exact Match
 ```python
 from qa_metrics.em import em_match
 
 reference_answer = ["The Frog Prince", "The Princess and the Frog"]
 candidate_answer = "The movie \"The Princess and the Frog\" is loosely based off the Brother Grimm's \"Iron Henry\""
@@ -131,14 +145,16 @@
 
 ## Updates
 - Improved PANDA evaluation with more representative answer correctness training data.
 - 🔥 The full paper is uploaded and can be accessed [here](https://arxiv.org/abs/2402.11161). The dataset is expanded and leaderboard is updated.
 - Our Training Dataset is adapted and augmented from [Bulian et al](https://github.com/google-research-datasets/answer-equivalence-dataset). Our [dataset repo](https://github.com/zli12321/Answer_Equivalence_Dataset.git) includes the augmented training set and QA evaluation testing sets discussed in our paper.
 - Now our model supports [distilroberta](https://huggingface.co/Zongxia/answer_equivalence_distilroberta), [distilbert](https://huggingface.co/Zongxia/answer_equivalence_distilbert), a smaller and faster matching model than Bert!
 - Now our model supports [roberta](https://huggingface.co/Zongxia/answer_equivalence_roberta), [roberta-large](https://huggingface.co/Zongxia/answer_equivalence_roberta-large), a larger and more robust matching model than Bert!
+- Check avilability of open-source LLMs in [deepinfra](https://deepinfra.com/models)
+- deepinfra supports: "lizpreciatior/lzlv_70b_fp16_hf", "meta-llama/Llama-2-70b-chat-hf", "meta-llama/Llama-2-7b-chat-hf", "meta-llama/Llama-2-13b-chat-hf", "01-ai/Yi-34B-Chat", "google/gemma-7b-it", "llava-hf/llava-1.5-7b-hf", "mistralai/Mixtral-8x7B-Instruct-v0.1"
 
 ## License
 
 This project is licensed under the [MIT License](LICENSE.md) - see the LICENSE file for details.
 
 ## Contact
```

### Comparing `qa_metrics-0.2.5/qa_metrics/Prompt_LLM.py` & `qa_metrics-0.2.6/qa_metrics/prompt_llm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import os, requests
 from typing import Union, List
 import openai
+from openai import OpenAI
+
 
 '''
 This file support calling OPENAI, Anthropic, and Cohere API nd get model prompt for text generation and completion
 '''
+
 class CloseLLM:
     def __init__(self):
-        self.key = None
+        self.openai = None
+        self.anthropic = None
 
     def set_openai_api_key(self, api_key):
         os.environ["OPENAI_API_KEY"] = api_key
-        openai.api_key = os.environ["OPENAI_API_KEY"]
+        self.openai = OpenAI(api_key=api_key)  
 
     def set_anthropic_api_key(self, api_key):
         os.environ["ANTHROPIC_API_KEY"] = api_key
         api_key = os.environ["ANTHROPIC_API_KEY"]
 
     '''
     Calls openai gpt functions. Given a message, it returns the response from the model. All parameters are at OPENAI's default value unless you specify it.
@@ -49,64 +53,78 @@
         :param user: Optional user identifier.
         :return: The output from the model.
         # Get the OpenAI API key from the environment variable
         openai.api_key = os.environ["OPENAI_API_KEY"]
         '''
 
         try:
-            message = [{ "role": "user", "content": prompt}]
-            answer = openai.ChatCompletion.create(
-                model = model_engine,
-                messages=message, 
-                frequency_penalty=frequency_penalty,
-                logit_bias=logit_bias,
+            # Send the request to the OpenAI API
+            # response = client.completions.create(engine=model_engine,
+            # prompt=prompt,
+            # max_tokens=max_tokens,
+            # temperature=temperature,
+            # n=1,  # Number of responses to generate
+            # stop=None)
+
+            # # Extract the generated response from the API response
+            # generated_text = response.choices[0].text.strip()
+
+            # return generated_text
+
+            completion = self.openai.chat.completions.create(
+                model=model_engine,
+                messages=[{"role": "user", "content": prompt}], 
                 max_tokens=max_tokens,
-                n=n,
-                presence_penalty=presence_penalty,
-                stop=stop,
                 temperature=temperature,
-                top_p=top_p,
-                stream=stream,
-                user=user
+                n=1,  # Number of responses to generate
+                stop=None
             )
 
+            message_content = completion.choices[0].message.content
 
-            return answer.choices[0].message.content
+            return message_content
         except Exception as e:
-            # Send the request to the OpenAI API
-            response = openai.Completion.create(
-                    engine=model_engine,
+            # message = [{ "role": "user", "content": prompt}]
+            # answer = client.chat.completions.create(model = model_engine,
+            # messages=message, 
+            # frequency_penalty=frequency_penalty,
+            # logit_bias=logit_bias,
+            # max_tokens=max_tokens,
+            # n=n,
+            # presence_penalty=presence_penalty,
+            # stop=stop,
+            # temperature=temperature,
+            # top_p=top_p,
+            # stream=stream,
+            # user=user)
+
+            try:
+                # return answer.choices[0].message.content
+                completion = self.openai.completions.create(
+                    model=model_engine,
                     prompt=prompt,
+                    frequency_penalty=frequency_penalty,
                     max_tokens=max_tokens,
+                    n=n,
+                    presence_penalty=presence_penalty,
+                    stop=stop,
                     temperature=temperature,
-                    n=1,  # Number of responses to generate
-                    stop=None,  # Specify a stopping sequence if needed
-            )
-
-            # Extract the generated response from the API response
-            generated_text = response.choices[0].text.strip()
-
-            return generated_text
-
-        except openai.error.APIError as e:
-            print(f"OpenAI API returned an API Error: {e}")
-            return None
-
-        except openai.error.APIConnectionError as e:
-            print(f"Failed to connect to OpenAI API: {e}")
-            return None
+                    top_p=top_p,
+                    stream=stream
+                )
+
+                return completion.choices[0].text
+            except openai.APIError as e:
+                print(f"OpenAI API returned an API Error: {e}")
+                return None
 
-        except openai.error.RateLimitError as e:
-            print(f"OpenAI API request exceeded rate limit: {e}")
-            return None
+            except KeyError:
+                print("OpenAI API key not found in the environment variables.")
+                return None
 
-        except KeyError:
-            print("OpenAI API key not found in the environment variables.")
-            return None
-        
 
     def prompt_claude(self, prompt, model_engine="claude-v1", anthropic_version="2023-06-01", max_tokens_to_sample=100, temperature=0.7):
         # Set up the API endpoint URL
         url = "https://api.anthropic.com/v1/complete"
 
         # Set up the request headers
         headers = {
@@ -144,8 +162,7 @@
         except requests.exceptions.RequestException as e:
             print(f"An error occurred while calling the Anthropic API: {e}")
             return None
 
         except KeyError:
             print("Anthropic API key not found in the environment variables.")
             return None
-
```

### Comparing `qa_metrics-0.2.5/qa_metrics/__init__.py` & `qa_metrics-0.2.6/qa_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.5/qa_metrics/em.py` & `qa_metrics-0.2.6/qa_metrics/em.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.5/qa_metrics/f1.py` & `qa_metrics-0.2.6/qa_metrics/f1.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.5/qa_metrics/pedant.py` & `qa_metrics-0.2.6/qa_metrics/pedant.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.5/qa_metrics/prompt_open_llm.py` & `qa_metrics-0.2.6/qa_metrics/prompt_open_llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 See link for API key and models: https://deepinfra.com/models
 '''
 
 class OpenLLM:
     def __init__(self):
         self.openai = None
 
-    def set_deepinfra_key(self, api_key):
+    def set_deepinfra_api_key(self, api_key):
         self.openai = OpenAI(
             api_key=api_key,
             base_url="https://api.deepinfra.com/v1/openai",
         )
 
-    def prompt(self, message, model_engine="mistralai/Mixtral-8x7B-Instruct-v0.1", temperature=0.7, max_tokens=100, top_p=0.5):
+    def prompt(self, prompt, model_engine="mistralai/Mixtral-8x7B-Instruct-v0.1", temperature=0.7, max_tokens=100, top_p=0.5):
         chat_completion = self.openai.chat.completions.create(
         model = model_engine,
         temperature=temperature,
         top_p=top_p,
         max_tokens=max_tokens,
         # num_return_sequences=2,
-        messages=[{"role": "user", "content": message}],
+        messages=[{"role": "user", "content": prompt}],
         )
 
         return chat_completion.choices[0].message.content
```

### Comparing `qa_metrics-0.2.5/qa_metrics/transformerMatcher.py` & `qa_metrics-0.2.6/qa_metrics/transformerMatcher.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.5/qa_metrics/utils/tools.py` & `qa_metrics-0.2.6/qa_metrics/utils/tools.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.5/qa_metrics.egg-info/PKG-INFO` & `qa_metrics-0.2.6/qa_metrics.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qa-metrics
-Version: 0.2.5
+Version: 0.2.6
 Summary: This package provides standard and classifier-based short form QA evaluation methods
 Home-page: https://github.com/zli12321/qa_metrics
 Author: Zongxia Li
 Author-email: zli12321@umd.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,23 +14,30 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: contractions>=0.0.1
+Requires-Dist: joblib
+Requires-Dist: requests
+Requires-Dist: scipy>=1.5.0
+Requires-Dist: scikit-learn==1.3.2
+Requires-Dist: numpy
 
 # QA-Evaluation-Metrics
 
 [![PyPI version qa-metrics](https://img.shields.io/pypi/v/qa-metrics.svg)](https://pypi.org/project/qa-metrics/) 
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17b7vrZqH0Yun2AJaOXydYZxr3cw20Ga6?usp=sharing)
 
-QA-Evaluation-Metrics is a fast and lightweight Python package for evaluating question-answering models and prompting of black-box large language models. It provides various basic metrics to assess the performance of QA models. Check out our paper [**PANDA**](https://arxiv.org/abs/2402.11161), an efficient QA evaluation that retains competitive evaluation performance of transformer LLM models. 
+QA-Evaluation-Metrics is a fast and lightweight Python package for evaluating question-answering models and prompting of black-box and open-source large language models. It provides various basic metrics to assess the performance of QA models. Check out our paper [**PANDA**](https://arxiv.org/abs/2402.11161), an efficient QA evaluation that retains competitive evaluation performance of transformer LLM models. 
 
-- 🔥 Our package also supports prompting of OPENAI GPT-series models and Claude Series models now.
+- 🔥 Our package also supports prompting OPENAI GPT-series models and Claude Series models now. (Assuimg OPENAI version > 1.0)
+- 🔥 Our package supports prompting various open source models such as LLaMA-2-70B-chat, LLaVA-1.5 etc by calling API from [deepinfra](https://deepinfra.com/models).
 
 
 ## Installation
 
 To install the package, run the following command:
 
 ```bash
@@ -43,34 +50,47 @@
 
 #### Prompting LLM For Evaluation
 
 Note: The prompting function can be used for any prompting purposes.
 
 ###### OpenAI
 ```python
-from qa_metrics.prompt_llm import *
-set_openai_api_key(YOUR_OPENAI_KEY)
+from qa_metrics.prompt_llm import CloseLLM
+model = CloseLLM()
+model.set_openai_api_key(YOUR_OPENAI_KEY)
 prompt = 'question: What is the Capital of France?\nreference: Paris\ncandidate: The capital is Paris\nIs the candidate answer correct based on the question and reference answer? Please only output correct or incorrect.'
-prompt_gpt(prompt=prompt, model_engine='gpt-3.5-turbo', temperature=0.1, max_token=10)
+model.prompt_gpt(prompt=prompt, model_engine='gpt-3.5-turbo', temperature=0.1, max_tokens=10)
 
 '''
 'correct'
 '''
 ```
 
 ###### Anthropic
 ```python
-set_anthropic_api_key(YOUR_OPENAI_KEY)
-prompt_claude(prompt=prompt, model_engine='claude-v1', anthropic_version="2023-06-01", max_tokens_to_sample=100, temperature=0.7)
+model = CloseLLM()
+model.set_anthropic_api_key(YOUR_Anthropic_KEY)
+model.prompt_claude(prompt=prompt, model_engine='claude-v1', anthropic_version="2023-06-01", max_tokens_to_sample=100, temperature=0.7)
 
 '''
 'correct'
 '''
 ```
 
+###### deepinfra (See below for descriptions of more models)
+```python
+from qa_metrics.prompt_open_llm import OpenLLM
+model = OpenLLM()
+model.set_deepinfra_api_key(YOUR_OPENAI_KEY)
+model.prompt(prompt=prompt, model_engine='mistralai/Mixtral-8x7B-Instruct-v0.1', temperature=0.1, max_tokens=10)
+
+'''
+'correct'
+'''
+```
 
 #### Exact Match
 ```python
 from qa_metrics.em import em_match
 
 reference_answer = ["The Frog Prince", "The Princess and the Frog"]
 candidate_answer = "The movie \"The Princess and the Frog\" is loosely based off the Brother Grimm's \"Iron Henry\""
@@ -152,14 +172,16 @@
 
 ## Updates
 - Improved PANDA evaluation with more representative answer correctness training data.
 - 🔥 The full paper is uploaded and can be accessed [here](https://arxiv.org/abs/2402.11161). The dataset is expanded and leaderboard is updated.
 - Our Training Dataset is adapted and augmented from [Bulian et al](https://github.com/google-research-datasets/answer-equivalence-dataset). Our [dataset repo](https://github.com/zli12321/Answer_Equivalence_Dataset.git) includes the augmented training set and QA evaluation testing sets discussed in our paper.
 - Now our model supports [distilroberta](https://huggingface.co/Zongxia/answer_equivalence_distilroberta), [distilbert](https://huggingface.co/Zongxia/answer_equivalence_distilbert), a smaller and faster matching model than Bert!
 - Now our model supports [roberta](https://huggingface.co/Zongxia/answer_equivalence_roberta), [roberta-large](https://huggingface.co/Zongxia/answer_equivalence_roberta-large), a larger and more robust matching model than Bert!
+- Check avilability of open-source LLMs in [deepinfra](https://deepinfra.com/models)
+- deepinfra supports: "lizpreciatior/lzlv_70b_fp16_hf", "meta-llama/Llama-2-70b-chat-hf", "meta-llama/Llama-2-7b-chat-hf", "meta-llama/Llama-2-13b-chat-hf", "01-ai/Yi-34B-Chat", "google/gemma-7b-it", "llava-hf/llava-1.5-7b-hf", "mistralai/Mixtral-8x7B-Instruct-v0.1"
 
 ## License
 
 This project is licensed under the [MIT License](LICENSE.md) - see the LICENSE file for details.
 
 ## Contact
```

### Comparing `qa_metrics-0.2.5/setup.py` & `qa_metrics-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import os
 
 
 setup(
     name='qa_metrics',
-    version='0.2.5',
+    version='0.2.6',
     author='Zongxia Li',
     author_email='zli12321@umd.edu',
     description='This package provides standard and classifier-based short form QA evaluation methods',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/zli12321/qa_metrics',
     packages=find_packages(),
```

