# Comparing `tmp/GenCasting-0.0.5.tar.gz` & `tmp/GenCasting-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenCasting-0.0.5.tar", last modified: Mon Apr  1 20:57:00 2024, max compression
+gzip compressed data, was "GenCasting-0.0.6.tar", last modified: Mon Apr  1 21:50:07 2024, max compression
```

## Comparing `GenCasting-0.0.5.tar` & `GenCasting-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:57:00.097855 GenCasting-0.0.5/
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:57:00.095595 GenCasting-0.0.5/GenCasting/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       41 2024-04-01 20:07:30.000000 GenCasting-0.0.5/GenCasting/__init__.py
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     6781 2024-04-01 19:53:44.000000 GenCasting-0.0.5/GenCasting/logit_extraction.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:57:00.096939 GenCasting-0.0.5/GenCasting.egg-info/
--rw-r--r--   0 faf32    (50383) faf32    (50391)      598 2024-04-01 20:57:00.096014 GenCasting-0.0.5/GenCasting.egg-info/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)      249 2024-04-01 20:57:00.096252 GenCasting-0.0.5/GenCasting.egg-info/SOURCES.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-01 20:57:00.096465 GenCasting-0.0.5/GenCasting.egg-info/dependency_links.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-01 20:57:00.096673 GenCasting-0.0.5/GenCasting.egg-info/requires.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-01 20:57:00.096993 GenCasting-0.0.5/GenCasting.egg-info/top_level.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 GenCasting-0.0.5/LICENSE
--rw-r--r--   0 faf32    (50383) faf32    (50391)      598 2024-04-01 20:57:00.097366 GenCasting-0.0.5/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       37 2024-04-01 19:42:20.000000 GenCasting-0.0.5/README.md
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-01 20:57:00.097916 GenCasting-0.0.5/setup.cfg
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     1120 2024-04-01 20:56:39.000000 GenCasting-0.0.5/setup.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 21:50:07.492378 GenCasting-0.0.6/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 GenCasting-0.0.6/LICENSE
+-rw-r--r--   0 faf32    (50383) faf32    (50391)      598 2024-04-01 21:50:07.492013 GenCasting-0.0.6/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       37 2024-04-01 19:42:20.000000 GenCasting-0.0.6/README.md
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-01 21:50:07.492510 GenCasting-0.0.6/setup.cfg
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     1159 2024-04-01 21:38:24.000000 GenCasting-0.0.6/setup.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 21:50:07.489155 GenCasting-0.0.6/src/
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 21:50:07.490342 GenCasting-0.0.6/src/GenCasting/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       41 2024-04-01 21:37:16.000000 GenCasting-0.0.6/src/GenCasting/__init__.py
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     6809 2024-04-01 21:27:06.000000 GenCasting-0.0.6/src/GenCasting/logit_extraction.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 21:50:07.491677 GenCasting-0.0.6/src/GenCasting.egg-info/
+-rw-r--r--   0 faf32    (50383) faf32    (50391)      598 2024-04-01 21:50:07.490824 GenCasting-0.0.6/src/GenCasting.egg-info/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)      277 2024-04-01 21:50:07.491070 GenCasting-0.0.6/src/GenCasting.egg-info/SOURCES.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-01 21:50:07.491286 GenCasting-0.0.6/src/GenCasting.egg-info/dependency_links.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-01 21:50:07.491506 GenCasting-0.0.6/src/GenCasting.egg-info/requires.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-01 21:50:07.491732 GenCasting-0.0.6/src/GenCasting.egg-info/top_level.txt
```

### Comparing `GenCasting-0.0.5/GenCasting/logit_extraction.py` & `GenCasting-0.0.6/src/GenCasting/logit_extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 from accelerate import Accelerator
 from peft import LoraConfig
 from trl import SFTTrainer,DataCollatorForCompletionOnlyLM
 
 
 class GenerativeForecaster:
 
-    def __init__(self,model_name,class_tokens,quantization=None,load_model=True):
+    def __init__(self,model_name,quantization=None):
+        '''
+        model_name: str
+        
+        '''
 
         self.model_name = model_name
         self.tokens = class_tokens
         
         self.load_model(quantization)
         self.token_dict = self.identify_tokens(self.tokens)
```

### Comparing `GenCasting-0.0.5/GenCasting.egg-info/PKG-INFO` & `GenCasting-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenCasting
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `GenCasting-0.0.5/PKG-INFO` & `GenCasting-0.0.6/src/GenCasting.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenCasting
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `GenCasting-0.0.5/setup.py` & `GenCasting-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Extract token-level probabilities from LLMs for classification-type outputs.'
 LONG_DESCRIPTION = 'A package that allows one to extract token-level probabilities. This method can be used for example to extract sentiment class probabilities instead of parsing text-generation outputs.'
 
 # Setting up
 setup(
     name="GenCasting",
     version=VERSION,
     author="Francesco A. Fabozzi",
     author_email="francescoafabozzi@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
-    packages=find_packages(),
+    package_dir={"":"src"},
+    packages=find_packages(where="src"),
     install_requires=['bitsandbytes', 'datasets', 'accelerate', 'loralib', 'transformers','peft','trl'],
     keywords=['python', 'LLMs', 'finance', 'forecasting', 'language models', 'huggingface'],
     classifiers=[
         "Development Status :: 1 - Planning"
     ]
 )
```

