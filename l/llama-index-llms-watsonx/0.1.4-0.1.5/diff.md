# Comparing `tmp/llama_index_llms_watsonx-0.1.4.tar.gz` & `tmp/llama_index_llms_watsonx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_watsonx-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_llms_watsonx-0.1.5.tar", max compression
```

## Comparing `llama_index_llms_watsonx-0.1.4.tar` & `llama_index_llms_watsonx-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       39 2024-02-13 13:53:01.695566 llama_index_llms_watsonx-0.1.4/README.md
--rw-r--r--   0        0        0       73 2024-02-13 13:53:01.695802 llama_index_llms_watsonx-0.1.4/llama_index/llms/watsonx/__init__.py
--rw-r--r--   0        0        0     7442 2024-02-20 22:37:41.328352 llama_index_llms_watsonx-0.1.4/llama_index/llms/watsonx/base.py
--rw-r--r--   0        0        0     1255 2024-02-13 13:53:01.695962 llama_index_llms_watsonx-0.1.4/llama_index/llms/watsonx/utils.py
--rw-r--r--   0        0        0     1472 2024-02-21 18:25:19.187975 llama_index_llms_watsonx-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 llama_index_llms_watsonx-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-04-02 20:58:46.838598 llama_index_llms_watsonx-0.1.5/README.md
+-rw-r--r--   0        0        0       73 2024-04-02 20:58:46.838598 llama_index_llms_watsonx-0.1.5/llama_index/llms/watsonx/__init__.py
+-rw-r--r--   0        0        0     7907 2024-04-02 20:58:46.838598 llama_index_llms_watsonx-0.1.5/llama_index/llms/watsonx/base.py
+-rw-r--r--   0        0        0     1518 2024-04-02 20:58:46.838598 llama_index_llms_watsonx-0.1.5/llama_index/llms/watsonx/utils.py
+-rw-r--r--   0        0        0     1472 2024-04-02 20:58:46.838598 llama_index_llms_watsonx-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 llama_index_llms_watsonx-0.1.5/PKG-INFO
```

### Comparing `llama_index_llms_watsonx-0.1.4/llama_index/llms/watsonx/base.py` & `llama_index_llms_watsonx-0.1.5/llama_index/llms/watsonx/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,35 @@
     WATSONX_MODELS,
     get_from_param_or_env_without_error,
     watsonx_model_to_context_size,
 )
 
 
 class WatsonX(LLM):
-    """IBM WatsonX LLM."""
+    """IBM WatsonX LLM.
+
+    Examples:
+        `pip install llama-index-llms-watsonx`
+
+        ```python
+        from llama_index.llms.watsonx import WatsonX
+
+        credentials = {
+            "url": "https://enter.your-ibm.url",
+            "apikey": "insert_your_api_key",
+        }
+
+        project_id = "insert_your_project_id"
+
+        llm = WatsonX(credentials=credentials, project_id=project_id)
+
+        resp = llm.complete("Paul Graham is")
+        print(resp)
+        ```
+    """
 
     model_id: str = Field(description="The Model to use.")
     max_new_tokens: int = Field(description="The maximum number of tokens to generate.")
     temperature: float = Field(description="The temperature to use for sampling.")
     additional_kwargs: Dict[str, Any] = Field(
         default_factory=dict, description="Additional Kwargs for the WatsonX model"
     )
```

### Comparing `llama_index_llms_watsonx-0.1.4/llama_index/llms/watsonx/utils.py` & `llama_index_llms_watsonx-0.1.5/llama_index/llms/watsonx/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import os
 from typing import Optional, Union
 
 WATSONX_MODELS = {
+    "google/flan-t5-xl": 4096,
     "google/flan-t5-xxl": 4096,
     "google/flan-ul2": 4096,
     "bigscience/mt0-xxl": 4096,
     "eleutherai/gpt-neox-20b": 8192,
     "bigcode/starcoder": 8192,
+    "codellama/codellama-34b-instruct-hf": 4096,
+    "meta-llama/llama-2-13b-chat": 4096,
     "meta-llama/llama-2-70b-chat": 4096,
-    "ibm/mpt-7b-instruct2": 2048,
+    "ibm-mistralai/mixtral-8x7b-instruct-v01-q": 32768,
     "ibm/granite-13b-instruct-v1": 8192,
     "ibm/granite-13b-chat-v1": 8192,
+    "ibm/granite-13b-instruct-v2": 8192,
+    "ibm/granite-13b-chat-v2": 8192,
+    "ibm/granite-20b-multilingual": 8190,
 }
 
 
 def watsonx_model_to_context_size(model_id: str) -> Union[int, None]:
     """Calculate the maximum number of tokens possible to generate for a model.
 
     Args:
```

### Comparing `llama_index_llms_watsonx-0.1.4/pyproject.toml` & `llama_index_llms_watsonx-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms watsonx integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-watsonx"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 llama-index-core = "^0.10.11.post1"
 ibm-watson-machine-learning = "^1.0.342"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_llms_watsonx-0.1.4/PKG-INFO` & `llama_index_llms_watsonx-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-watsonx
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index llms watsonx integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ibm-watson-machine-learning (>=1.0.342,<2.0.0)
 Requires-Dist: llama-index-core (>=0.10.11.post1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Watsonx
```

