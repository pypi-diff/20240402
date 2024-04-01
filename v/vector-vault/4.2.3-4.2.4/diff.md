# Comparing `tmp/vector_vault-4.2.3.tar.gz` & `tmp/vector_vault-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.2.3.tar", last modified: Sat Mar 30 19:22:17 2024, max compression
+gzip compressed data, was "vector_vault-4.2.4.tar", last modified: Mon Apr  1 23:52:05 2024, max compression
```

## Comparing `vector_vault-4.2.3.tar` & `vector_vault-4.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-03-30 19:22:17.990521 vector_vault-4.2.3/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.2.3/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-03-30 19:22:17.990381 vector_vault-4.2.3/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.2.3/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-03-30 19:22:17.990552 vector_vault-4.2.3/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-03-30 18:46:20.000000 vector_vault-4.2.3/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-03-30 19:22:17.986631 vector_vault-4.2.3/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-03-30 19:22:17.000000 vector_vault-4.2.3/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-03-30 19:22:17.000000 vector_vault-4.2.3/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-03-30 19:22:17.000000 vector_vault-4.2.3/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-03-30 19:22:17.000000 vector_vault-4.2.3/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-03-30 19:22:17.000000 vector_vault-4.2.3/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-03-30 19:22:17.990052 vector_vault-4.2.3/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.2.3/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-03-26 17:36:03.000000 vector_vault-4.2.3/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.2.3/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6326 2024-03-13 21:53:47.000000 vector_vault-4.2.3/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.2.3/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.2.3/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2984 2024-03-08 18:43:23.000000 vector_vault-4.2.3/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    20549 2024-03-30 19:21:27.000000 vector_vault-4.2.3/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    57116 2024-03-30 19:04:34.000000 vector_vault-4.2.3/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     4525 2024-01-03 00:13:43.000000 vector_vault-4.2.3/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.2.3/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-01 23:52:05.598690 vector_vault-4.2.4/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.2.4/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-01 23:52:05.598557 vector_vault-4.2.4/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.2.4/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-01 23:52:05.598723 vector_vault-4.2.4/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-01 23:51:46.000000 vector_vault-4.2.4/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-01 23:52:05.596420 vector_vault-4.2.4/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-01 23:52:05.000000 vector_vault-4.2.4/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-01 23:52:05.000000 vector_vault-4.2.4/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-01 23:52:05.000000 vector_vault-4.2.4/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-01 23:52:05.000000 vector_vault-4.2.4/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-01 23:52:05.000000 vector_vault-4.2.4/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-01 23:52:05.598404 vector_vault-4.2.4/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.2.4/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-03-26 17:36:03.000000 vector_vault-4.2.4/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.2.4/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6326 2024-03-13 21:53:47.000000 vector_vault-4.2.4/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.2.4/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.2.4/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2984 2024-03-08 18:43:23.000000 vector_vault-4.2.4/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-01 23:51:29.000000 vector_vault-4.2.4/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    57116 2024-03-30 19:04:34.000000 vector_vault-4.2.4/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     4525 2024-01-03 00:13:43.000000 vector_vault-4.2.4/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.2.4/vectorvault/wrap.py
```

### Comparing `vector_vault-4.2.3/LICENSE` & `vector_vault-4.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.3/PKG-INFO` & `vector_vault-4.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.2.3
+Version: 4.2.4
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.2.3/README.md` & `vector_vault-4.2.4/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.3/setup.py` & `vector_vault-4.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.2.3",
+    version="4.2.4",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.2.3/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.2.4/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.2.3
+Version: 4.2.4
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.2.3/vectorvault/ai.py` & `vector_vault-4.2.4/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.3/vectorvault/cloud_api.py` & `vector_vault-4.2.4/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.3/vectorvault/cloudmanager.py` & `vector_vault-4.2.4/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.3/vectorvault/creds.py` & `vector_vault-4.2.4/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.3/vectorvault/download.py` & `vector_vault-4.2.4/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.3/vectorvault/itemize.py` & `vector_vault-4.2.4/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.3/vectorvault/tools_gpt.py` & `vector_vault-4.2.4/vectorvault/tools_gpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 from .ai import AI
 import time
 import ast
 
 '''
     ToolsGPT is a set of tools special to large language models. 
-    Every tool turns subjectivity into objectivity.
+    Every tool turns unstructured data into structured data.
     
-    Objectivity is needed for code. 
-    Subjectivity is the primary human input.
-    These tools bridge the gap between human interaction and code. 
+    Structure data is required to run programs. 
+    Unstructured data is the primary human output.
+    AI tools convert unstructured data into structured data, 
+    bridging the gap between humans and programs. 
+    Therefore, in the future, everything will be programmable.
     
     ToolsGPT allows you to get the following for any input:
         1. `get_rating` - returns a rating out of 10 for any input
         2. `get_yes_no` - returns a 'yes' or a 'no' to any question
         3. `get_number` - returns an integer based on your instructions
         4. `get_match` - returns a match to a list options - (single choice)
         5. `get_multi_match` - returns one or many matches to a list of options - (multiple choice)
         6. `get_topic` - returns the topic subject matter of any input 
 
         1. `get_rating`:
-            Useful to get a quality rating (integer out of 10)
+            Get a numeric rating out of 10 for anything
 
         2. `get_yes_no`:
-            Useful for getting an exact 'yes' or 'no' to any question
+            Get an exact 'yes' or 'no' to any question
 
         3. `get_number`:
-            Useful for getting something converted into an integer
+            Get an integer output for any input
         
         4. `get_match`:
-            Useful to get an exact match to a single item within a list 
+            Get an exact match to a single item within a list 
             -> in: (text and list of strings) 
             -> out: (one exact match to an answer in list -> string type)
         
         5. `get_multi_match`:
-            Useful to get many exact matches to items within a list  
+            Get many matches to items within a list  
             -> in: (text and list of answers) 
             -> out: (list of exact matches -> list type)
 
         6. `get_topic`:
             Useful to classify the topic of conversation
 '''
 
@@ -72,24 +74,27 @@
             return int(answer) # try to return an int zero shot
         except:
             return self.retry_until_its_a_number(answer, model=model, loop_limit=loop_limit) # force the integer if zero shot fails
         
         
     def get_number(self, concept, content: str, model='gpt-3.5-turbo', loop_limit=5) -> int:
         '''
-            param: `concept` - i.e. "The following content should be a number between 1 and 100" 
-            Your content will be injected into this prompt: 
-            Prompt = f"{concept} \n\n{content}"
+            param: `concept` - is the idea used to generate a number with - i.e. "How many students are in the professor's class?" 
+            param: `content` - is the content to generate a number for - i.e. "I had 400 students in my class last year, but this year, I have 10% more." 
         '''
         response = self.retry_llm(f'{concept} \n\n{content}', model=model, loop_limit=loop_limit)
         print("Initial number extraction response:", response) if self.verbose else 0
         return response if type(response) is int else self.retry_until_its_a_number(response, model=model, loop_limit=loop_limit)
         
     
     def retry_until_its_a_number(self, content: str, model='gpt-3.5-turbo', loop_limit=5) -> int:
+        '''
+            param: `content` - the AI will return an integer based on the content you input
+        '''
+
         prompt_template = """Respond only with a number in integer format...
 Example content: 'The revenue for the last fiscal year was $1,200,000.' Example answer: '1200000'
 Example content 2: 'The company has been in business for twenty years.' Example answer 2: '20'
 Example content 3: 'The recipe calls for three cups of flour.' Example answer 3: '3'
 Example content 4: 'The event will take place on the 15th of next month.' Example answer 4: '15'
 Example content 5: 'The building has a total of fourteen floors.' Example answer 5: '14'
 Example content 6: 'There are one hundred and fifty employees in the company.' Example answer 6: '150'
```

### Comparing `vector_vault-4.2.3/vectorvault/vault.py` & `vector_vault-4.2.4/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.3/vectorvault/vecreq.py` & `vector_vault-4.2.4/vectorvault/vecreq.py`

 * *Files identical despite different names*

