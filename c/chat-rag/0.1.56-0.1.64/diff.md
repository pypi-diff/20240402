# Comparing `tmp/chat_rag-0.1.56.tar.gz` & `tmp/chat_rag-0.1.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_rag-0.1.56.tar", max compression
+gzip compressed data, was "chat_rag-0.1.64.tar", max compression
```

## Comparing `chat_rag-0.1.56.tar` & `chat_rag-0.1.64.tar`

### file list

```diff
@@ -1,31 +1,35 @@
--rw-r--r--   0        0        0     1083 2024-02-07 11:08:45.534329 chat_rag-0.1.56/LICENSE
--rw-r--r--   0        0        0     1666 2024-02-07 11:08:45.534329 chat_rag-0.1.56/README.md
--rw-r--r--   0        0        0     4023 2024-02-26 10:37:30.019215 chat_rag-0.1.56/chat_rag/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/data/__init__.py
--rw-r--r--   0        0        0      788 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/data/models.py
--rw-r--r--   0        0        0    10512 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/data/parsers.py
--rw-r--r--   0        0        0    13027 2024-03-05 14:12:53.351964 chat_rag-0.1.56/chat_rag/data/splitters.py
--rw-r--r--   0        0        0      897 2024-02-26 10:37:33.379027 chat_rag-0.1.56/chat_rag/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/inf_retrieval/__init__.py
--rw-r--r--   0        0        0     3924 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/inf_retrieval/check_answ_questions.py
--rw-r--r--   0        0        0     2450 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/inf_retrieval/cross_encoder.py
--rw-r--r--   0        0        0      141 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/inf_retrieval/embedding_models/__init__.py
--rw-r--r--   0        0        0     4617 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/inf_retrieval/embedding_models/base_model.py
--rw-r--r--   0        0        0     1494 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/inf_retrieval/embedding_models/e5_model.py
--rw-r--r--   0        0        0     4693 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/inf_retrieval/query_generator.py
--rw-r--r--   0        0        0     3886 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/inf_retrieval/reference_checker.py
--rw-r--r--   0        0        0       82 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/inf_retrieval/retrievers/__init__.py
--rw-r--r--   0        0        0     7447 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/inf_retrieval/retrievers/semantic_retriever.py
--rw-r--r--   0        0        0      135 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/intent_detection/__init__.py
--rw-r--r--   0        0        0     1527 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/intent_detection/clusterize_text.py
--rw-r--r--   0        0        0     1419 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/intent_detection/gen_intent.py
--rw-r--r--   0        0        0      362 2024-02-14 11:30:45.994835 chat_rag-0.1.56/chat_rag/llms/__init__.py
--rw-r--r--   0        0        0     6995 2024-02-26 10:37:33.379027 chat_rag-0.1.56/chat_rag/llms/base_llm.py
--rw-r--r--   0        0        0     4559 2024-03-05 12:10:52.060278 chat_rag-0.1.56/chat_rag/llms/claude_client.py
--rw-r--r--   0        0        0     5219 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/llms/ggml_llm.py
--rw-r--r--   0        0        0     9255 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/llms/hf_llm.py
--rw-r--r--   0        0        0     5338 2024-02-07 11:08:45.534329 chat_rag-0.1.56/chat_rag/llms/mistral_client.py
--rw-r--r--   0        0        0     5360 2024-02-14 11:30:45.994835 chat_rag-0.1.56/chat_rag/llms/openai_client.py
--rw-r--r--   0        0        0    15362 2024-02-26 10:37:33.379027 chat_rag-0.1.56/chat_rag/llms/vllm_client.py
--rw-r--r--   0        0        0     1123 2024-03-05 16:07:44.140619 chat_rag-0.1.56/pyproject.toml
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 chat_rag-0.1.56/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-02-07 09:34:49.972743 chat_rag-0.1.64/LICENSE
+-rw-r--r--   0        0        0     1666 2023-12-13 14:55:14.591003 chat_rag-0.1.64/README.md
+-rw-r--r--   0        0        0       68 2024-04-02 12:17:40.982534 chat_rag-0.1.64/chat_rag/__init__.py
+-rw-r--r--   0        0        0     3295 2024-04-02 12:17:40.982534 chat_rag-0.1.64/chat_rag/async_rag.py
+-rw-r--r--   0        0        0        0 2023-12-13 14:55:14.591003 chat_rag-0.1.64/chat_rag/data/__init__.py
+-rw-r--r--   0        0        0      788 2024-01-31 17:51:45.327655 chat_rag-0.1.64/chat_rag/data/models.py
+-rw-r--r--   0        0        0    10492 2024-04-02 12:17:40.982534 chat_rag-0.1.64/chat_rag/data/parsers.py
+-rw-r--r--   0        0        0    13027 2024-03-06 13:48:08.349750 chat_rag-0.1.64/chat_rag/data/splitters.py
+-rw-r--r--   0        0        0      897 2024-02-26 17:12:56.927011 chat_rag-0.1.64/chat_rag/exceptions.py
+-rw-r--r--   0        0        0        0 2023-12-13 14:55:14.595003 chat_rag-0.1.64/chat_rag/inf_retrieval/__init__.py
+-rw-r--r--   0        0        0     3924 2024-01-22 11:13:32.756810 chat_rag-0.1.64/chat_rag/inf_retrieval/check_answ_questions.py
+-rw-r--r--   0        0        0     2450 2024-02-07 09:34:49.972743 chat_rag-0.1.64/chat_rag/inf_retrieval/cross_encoder.py
+-rw-r--r--   0        0        0      141 2023-12-13 14:55:14.595003 chat_rag-0.1.64/chat_rag/inf_retrieval/embedding_models/__init__.py
+-rw-r--r--   0        0        0     4617 2023-12-13 14:55:14.595003 chat_rag-0.1.64/chat_rag/inf_retrieval/embedding_models/base_model.py
+-rw-r--r--   0        0        0     1494 2024-01-18 15:08:39.142423 chat_rag-0.1.64/chat_rag/inf_retrieval/embedding_models/e5_model.py
+-rw-r--r--   0        0        0     4693 2024-01-22 11:13:32.756810 chat_rag-0.1.64/chat_rag/inf_retrieval/query_generator.py
+-rw-r--r--   0        0        0     3886 2024-02-07 09:34:49.972743 chat_rag-0.1.64/chat_rag/inf_retrieval/reference_checker.py
+-rw-r--r--   0        0        0      240 2024-04-02 12:17:40.982534 chat_rag-0.1.64/chat_rag/inf_retrieval/retrievers/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-02 12:17:40.986534 chat_rag-0.1.64/chat_rag/inf_retrieval/retrievers/rerank_retriever.py
+-rw-r--r--   0        0        0      503 2024-04-02 12:17:40.986534 chat_rag-0.1.64/chat_rag/inf_retrieval/retrievers/retriever_client.py
+-rw-r--r--   0        0        0     7447 2023-12-13 14:55:14.595003 chat_rag-0.1.64/chat_rag/inf_retrieval/retrievers/semantic_retriever.py
+-rw-r--r--   0        0        0      135 2023-12-13 14:55:14.595003 chat_rag-0.1.64/chat_rag/intent_detection/__init__.py
+-rw-r--r--   0        0        0     1527 2024-01-22 11:13:32.756810 chat_rag-0.1.64/chat_rag/intent_detection/clusterize_text.py
+-rw-r--r--   0        0        0     1419 2024-01-22 11:13:32.760810 chat_rag-0.1.64/chat_rag/intent_detection/gen_intent.py
+-rw-r--r--   0        0        0      445 2024-04-02 12:17:40.986534 chat_rag-0.1.64/chat_rag/llms/__init__.py
+-rw-r--r--   0        0        0     6995 2024-02-26 17:12:56.927011 chat_rag-0.1.64/chat_rag/llms/base_llm.py
+-rw-r--r--   0        0        0     9040 2024-04-02 12:17:40.986534 chat_rag-0.1.64/chat_rag/llms/claude_client.py
+-rw-r--r--   0        0        0     5219 2023-12-13 14:55:14.595003 chat_rag-0.1.64/chat_rag/llms/ggml_llm.py
+-rw-r--r--   0        0        0     9255 2023-12-13 14:55:14.595003 chat_rag-0.1.64/chat_rag/llms/hf_llm.py
+-rw-r--r--   0        0        0    10715 2024-04-02 12:17:40.986534 chat_rag-0.1.64/chat_rag/llms/mistral_client.py
+-rw-r--r--   0        0        0    10629 2024-04-02 12:17:40.986534 chat_rag-0.1.64/chat_rag/llms/openai_client.py
+-rw-r--r--   0        0        0    25992 2024-04-02 12:17:40.986534 chat_rag-0.1.64/chat_rag/llms/vllm_client.py
+-rw-r--r--   0        0        0     3578 2024-04-02 12:17:40.986534 chat_rag-0.1.64/chat_rag/rag.py
+-rw-r--r--   0        0        0      932 2024-04-02 12:17:40.990534 chat_rag-0.1.64/pyproject.toml
+-rw-r--r--   0        0        0     3115 1970-01-01 00:00:00.000000 chat_rag-0.1.64/PKG-INFO
```

### Comparing `chat_rag-0.1.56/LICENSE` & `chat_rag-0.1.64/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/README.md` & `chat_rag-0.1.64/README.md`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/__init__.py` & `chat_rag-0.1.64/chat_rag/rag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 from logging import getLogger
 from typing import List, Dict
 
 from chat_rag.llms import RAGLLM
-from chat_rag.inf_retrieval.cross_encoder import ReRanker
 
 logger = getLogger(__name__)
 
 
 class RAG:
     """
     Class for generating responses using the Retrieval-Augmented Generation (RAG) pattern.
     """
     def __init__(
         self,
         retriever,
         llm_model: RAGLLM,
         lang: str = "en",
-        rerank: bool = False,
     ):
         """
         Parameters
         ----------
         retriever :
             Retriever object for retrieving contexts.
         llm_model : RAGLLM
             Language model for generating responses.
         lang : str, optional
             Language of the language model, by default "en"
-        rerank : bool, optional
-            Whether to use cross-encoder for reranking contexts, by default False
         """
 
         self.retriever = retriever
         self.model = llm_model
-        self.rerank = rerank
-        if rerank:
-            self.cross_encoder = ReRanker(lang=lang, device=retriever.embedding_model.device)
         self.lang = lang
 
 
     def retrieve(
         self,
         message: str,
         prev_contents: List[str],
@@ -58,16 +51,14 @@
         Returns
         -------
         Tuple[List[str], List[Dict[str, str]]]
             List of all conversation contexts and list of the retrieved contexts for the current user message.
         """
         logger.info("Retrieving new contexts")
         contexts = self.retriever.retrieve([message], top_k=prompt_structure_dict["n_contexts_to_use"])[0] # retrieve contexts
-        if self.rerank:
-            contexts = self.cross_encoder(message, contexts) # filter contexts
         if len(contexts) == 0:
             return [], []
 
         contents = [context["content"] for context in contexts] # get unique contexts
         returned_contexts = [contexts[:prompt_structure_dict["n_contexts_to_use"]]] # structure for references
 
         # Use a list comprehension to preserve order and not adding duplicates
@@ -123,7 +114,9 @@
             stop_words=stop_words,
         )
 
         return {
             "res": output_text,
             "context": returned_contexts,
         }
+
+
```

### Comparing `chat_rag-0.1.56/chat_rag/data/models.py` & `chat_rag-0.1.64/chat_rag/data/models.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/data/parsers.py` & `chat_rag-0.1.64/chat_rag/data/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import List, Optional, Union, BinaryIO, IO, Callable
 from tempfile import SpooledTemporaryFile
 
-import pandas as pd
 from unstructured.documents.elements import (
     Element,
     Text,  # Uncategorized text
     Title,
 )
 
 from unstructured.partition.auto import partition_pdf, partition_html
```

### Comparing `chat_rag-0.1.56/chat_rag/data/splitters.py` & `chat_rag-0.1.64/chat_rag/data/splitters.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/exceptions.py` & `chat_rag-0.1.64/chat_rag/exceptions.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/inf_retrieval/check_answ_questions.py` & `chat_rag-0.1.64/chat_rag/inf_retrieval/check_answ_questions.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/inf_retrieval/cross_encoder.py` & `chat_rag-0.1.64/chat_rag/inf_retrieval/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/inf_retrieval/embedding_models/base_model.py` & `chat_rag-0.1.64/chat_rag/inf_retrieval/embedding_models/base_model.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/inf_retrieval/embedding_models/e5_model.py` & `chat_rag-0.1.64/chat_rag/inf_retrieval/embedding_models/e5_model.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/inf_retrieval/query_generator.py` & `chat_rag-0.1.64/chat_rag/inf_retrieval/query_generator.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/inf_retrieval/reference_checker.py` & `chat_rag-0.1.64/chat_rag/inf_retrieval/reference_checker.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/inf_retrieval/retrievers/semantic_retriever.py` & `chat_rag-0.1.64/chat_rag/inf_retrieval/retrievers/semantic_retriever.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/intent_detection/clusterize_text.py` & `chat_rag-0.1.64/chat_rag/intent_detection/clusterize_text.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/intent_detection/gen_intent.py` & `chat_rag-0.1.64/chat_rag/intent_detection/gen_intent.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/llms/base_llm.py` & `chat_rag-0.1.64/chat_rag/llms/base_llm.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/llms/claude_client.py` & `chat_rag-0.1.64/chat_rag/llms/claude_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import List, Dict
 import os
+from typing import Dict, List
 
-from anthropic import Anthropic
+from anthropic import Anthropic, AsyncAnthropic
 
-from chat_rag.llms import RAGLLM, CONTEXT_PREFIX
+from chat_rag.llms import CONTEXT_PREFIX, RAGLLM
 
 
 class ClaudeChatModel(RAGLLM):
     def __init__(self, llm_name, **kwargs) -> None:
         self.llm_name = llm_name
         self.client = Anthropic(
             api_key=os.environ.get("ANTHROPIC_API_KEY"),
@@ -141,8 +141,144 @@
         )
 
         for event in stream:
             if event.type == "content_block_delta":
                 yield event.delta.text
 
         
+class AsyncClaudeChatModel(RAGLLM):
+    def __init__(self, llm_name, **kwargs) -> None:
+        self.llm_name = llm_name
+        self.client = AsyncAnthropic(
+            api_key=os.environ.get("ANTHROPIC_API_KEY")
+        )
+
+    def format_prompt(
+        self,
+        contexts: List[str],
+        system_prefix: str,
+        n_contexts_to_use: int = 3,
+        lang: str = "en",
+        **kwargs,
+    ) -> List[Dict[str, str]]:
+        """
+        Formats the prompt to be used by the model.
+        Parameters
+        ----------
+        contexts : list
+            The context to use.
+        system_prefix : str
+            The prefix to indicate instructions for the LLM.
+        system_tag : str
+            The tag to indicate the start of the system prefix for the LLM.
+        system_end : str
+            The tag to indicate the end of the system prefix for the LLM.
+        user_tag : str
+            The tag to indicate the start of the user input.
+        user_end : str
+            The tag to indicate the end of the user input.
+        assistant_tag : str
+            The tag to indicate the start of the assistant output.
+        assistant_end : str
+            The tag to indicate the end of the assistant output.
+        Returns
+        -------
+        list
+            The formatted prompt.
+        """
+        system_prompt = self.format_system_prompt(
+            contexts=contexts,
+            system_prefix=system_prefix,
+            n_contexts_to_use=n_contexts_to_use,
+            lang=lang,
+        )
+
+        return system_prompt
+    
+    async def generate(
+        self,
+        messages: List[Dict[str, str]],
+        contexts: List[str],
+        prompt_structure_dict: dict,
+        generation_config_dict: dict = None,
+        lang: str = "en",
+        **kwargs,
+    ) -> str:
+        """
+        Generate text from a prompt using the model.
+        Parameters
+        ----------
+        messages : List[Tuple[str, str]]
+            The messages to use for the prompt. Pair of (role, message).
+        contexts : List[str]
+            The contexts to use for generation.
+        prompt_structure_dict : dict
+            Dictionary containing the structure of the prompt.
+        generation_config_dict : dict
+            Keyword arguments for the generation.
+        lang : str
+            The language of the prompt.
+        Returns
+        -------
+        str
+            The generated text.
+        """
+
+        system_prompt = self.format_prompt(contexts, **prompt_structure_dict, lang=lang)
+
+        message = await self.client.messages.create(
+            model=self.llm_name,
+            system=system_prompt,
+            messages=messages,
+            max_tokens=generation_config_dict['max_new_tokens'],
+            temperature=generation_config_dict['temperature'],
+            top_p=generation_config_dict['top_p'],
+            top_k=generation_config_dict['top_k'],
+        )
+
+        return message.content[0].text
+    
+    async def stream(
+        self,
+        messages: List[Dict[str, str]],
+        contexts: List[str],
+        prompt_structure_dict: dict,
+        generation_config_dict: dict = None,
+        lang: str = "en",
+        **kwargs,
+    ):
+        """
+        Generate text from a prompt using the model.
+        Parameters
+        ----------
+        messages : List[Tuple[str, str]]
+            The messages to use for the prompt. Pair of (role, message).
+        contexts : List[str]
+            The contexts to use for generation.
+        prompt_structure_dict : dict
+            Dictionary containing the structure of the prompt.
+        generation_config_dict : dict
+            Keyword arguments for the generation.
+        lang : str
+            The language of the prompt.
+        Returns
+        -------
+        str
+            The generated text.
+        """
+
+        system_prompt = self.format_prompt(contexts, **prompt_structure_dict, lang=lang)
+
+        stream = await self.client.messages.create(
+            model=self.llm_name,
+            system=system_prompt,
+            messages=messages,
+            max_tokens=generation_config_dict['max_new_tokens'],
+            temperature=generation_config_dict['temperature'],
+            top_p=generation_config_dict['top_p'],
+            top_k=generation_config_dict['top_k'],
+            stream=True,
+        )
 
+        async for event in stream:
+            if event.type == "content_block_delta":
+                yield event.delta.text
```

### Comparing `chat_rag-0.1.56/chat_rag/llms/ggml_llm.py` & `chat_rag-0.1.64/chat_rag/llms/ggml_llm.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/llms/hf_llm.py` & `chat_rag-0.1.64/chat_rag/llms/hf_llm.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.56/chat_rag/llms/openai_client.py` & `chat_rag-0.1.64/chat_rag/llms/openai_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import List, Dict
 import os
+from typing import Dict, List
 
-from openai import OpenAI
+from openai import AsyncOpenAI, OpenAI
 
 from chat_rag.llms import RAGLLM
 
 
 class OpenAIChatModel(RAGLLM):
     def __init__(
         self,
@@ -114,15 +114,15 @@
         self,
         messages: List[Dict[str, str]],
         contexts: List[str],
         prompt_structure_dict: dict,
         generation_config_dict: dict = None,
         lang: str = "en",
         **kwargs,
-    ) -> str:
+    ):
         """
         Generate text from a prompt using the model in streaming mode.
         Parameters
         ----------
         messages : List[Tuple[str, str]]
             The messages to use for the prompt. Pair of (role, message).
         contexts : List[str]
@@ -158,7 +158,165 @@
         n=1,
         stream=True)
         for chunk in response:
             if chunk.choices[0].finish_reason == "stop":
                 return
             if chunk.choices[0].delta.content is not None:
                 yield chunk.choices[0].delta.content # return the delta text message
+
+
+class AsyncOpenAIChatModel(RAGLLM):
+    def __init__(
+        self,
+        llm_name: str,
+        **kwargs,
+    ):
+        self.client = AsyncOpenAI(api_key=os.environ["OPENAI_API_KEY"])
+        self.llm_name = llm_name
+
+    def format_prompt(
+        self,
+        messages: List[Dict[str, str]],
+        contexts: List[str],
+        system_prefix: str,
+        n_contexts_to_use: int = 3,
+        lang: str = "en",
+        **kwargs,
+    ) -> List[Dict[str, str]]:
+        """
+        Formats the prompt to be used by the model.
+        Parameters
+        ----------
+        messages : List[Tuple[str, str]]
+            The messages to use for the prompt. Pair of (role, message).
+        contexts : list
+            The context to use.
+        system_prefix : str
+            The prefix to indicate instructions for the LLM.
+        system_tag : str
+            The tag to indicate the start of the system prefix for the LLM.
+        system_end : str
+            The tag to indicate the end of the system prefix for the LLM.
+        user_tag : str
+            The tag to indicate the start of the user input.
+        user_end : str
+            The tag to indicate the end of the user input.
+        assistant_tag : str
+            The tag to indicate the start of the assistant output.
+        assistant_end : str
+            The tag to indicate the end of the assistant output.
+            The tag to indicate the end of the role (system role, user role, assistant role).
+        n_contexts_to_use : int, optional
+            The number of contexts to use, by default 3
+        lang : str, optional
+            The language of the prompt, by default 'en'
+        """
+        system_prompt = self.format_system_prompt(
+            contexts=contexts,
+            system_prefix=system_prefix,
+            n_contexts_to_use=n_contexts_to_use,
+            lang=lang,
+        )
+
+        final_messages = [{'role': 'system', 'content': system_prompt}] + messages
+
+        return final_messages
+
+    async def generate(
+        self,
+        messages: List[Dict[str, str]],
+        contexts: List[str],
+        prompt_structure_dict: dict,
+        generation_config_dict: dict = None,
+        lang: str = "en",
+        **kwargs,
+    ) -> str:
+        """
+        Generate text from a prompt using the model.
+        Parameters
+        ----------
+        messages : List[Tuple[str, str]]
+            The messages to use for the prompt. Pair of (role, message).
+        contexts : List[str]
+            The contexts to use for generation.
+        prompt_structure_dict : dict
+            Dictionary containing the structure of the prompt.
+        generation_config_dict : dict
+            Keyword arguments for the generation.
+        lang : str
+            The language of the prompt.
+        Returns
+        -------
+        str
+            The generated text.
+        """
+
+        messages = self.format_prompt(
+            messages=messages,
+            contexts=contexts,
+            **prompt_structure_dict,
+            lang=lang,
+        )
+
+        response = await self.client.chat.completions.create(model=self.llm_name,
+        messages=messages,
+        max_tokens=generation_config_dict["max_new_tokens"],
+        temperature=generation_config_dict["temperature"],
+        top_p=generation_config_dict["top_p"],
+        presence_penalty=generation_config_dict["repetition_penalty"],
+        seed=generation_config_dict["seed"],
+        n=1,
+        stream=False)
+        return response.choices[0].message.content
+    
+    async def stream(
+        self,
+        messages: List[Dict[str, str]],
+        contexts: List[str],
+        prompt_structure_dict: dict,
+        generation_config_dict: dict = None,
+        lang: str = "en",
+        **kwargs,
+    ):
+        """
+        Generate text from a prompt using the model in streaming mode.
+        Parameters
+        ----------
+        messages : List[Tuple[str, str]]
+            The messages to use for the prompt. Pair of (role, message).
+        contexts : List[str]
+            The contexts to use for generation.
+        prompt_structure_dict : dict
+            Dictionary containing the structure of the prompt.
+        generation_config_dict : dict
+            Keyword arguments for the generation.
+        lang : str
+            The language of the prompt.
+        Returns
+        -------
+        str
+            The generated text.
+        """
+
+        messages = self.format_prompt(
+            messages=messages,
+            contexts=contexts,
+            **prompt_structure_dict,
+            lang=lang,
+        )
+
+        print(messages)
+
+        response = await self.client.chat.completions.create(model=self.llm_name,
+        messages=messages,
+        max_tokens=generation_config_dict["max_new_tokens"],
+        temperature=generation_config_dict["temperature"],
+        top_p=generation_config_dict["top_p"],
+        presence_penalty=generation_config_dict["repetition_penalty"],
+        seed=generation_config_dict["seed"],
+        n=1,
+        stream=True)
+        async for chunk in response:
+            if chunk.choices[0].finish_reason == "stop":
+                return
+            if chunk.choices[0].delta.content is not None:
+                yield chunk.choices[0].delta.content
```

### Comparing `chat_rag-0.1.56/pyproject.toml` & `chat_rag-0.1.64/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 [tool.poetry]
 name = "chat-rag"
-version = "0.1.56"
+version = "0.1.64"
 description = ""
 authors = ["Diego Peláez Paquico <diego.pelaez@with-madrid.com>"]
 readme = "README.md"
 packages = [{ include = "chat_rag" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+python-dotenv = "^0.21.0"
 numpy = "1.23.5"
 pandas = "1.4.4"
-transformers = "^4.35.2"
-sentence-transformers = "^2.2.2"
-pyarrow = "^12.0.0"
-python-dotenv = "^0.21.0"
-torch = [
-    { version = "^2.1.0", source = "torch" },
-]
-ctransformers = "^0.2.10"
 tqdm = "^4.65.0"
-einops = "^0.6.1"
-openai = "^1.3.4"
-accelerate = "^0.21.0"
-unstructured = {extras = ["pdf"], version = "0.12.0", python = ">=3.10,<3.12"}
+pyarrow = "^12.0.0"
 pillow = "^10.1.0"
 certifi = "^2023.7.22"
 urllib3 = "^1.26.18"
 aiohttp = "^3.8.5"
 cryptography = "^41.0.4"
+torch = "^2.1.0"
+transformers = "^4.38.2"
+sentence-transformers = "^2.3.0"
+ctransformers = "^0.2.10"
+einops = "^0.6.1"
+accelerate = "^0.21.0"
+autoawq = "0.1.7"
+unstructured = {extras = ["pdf"], version = "0.12.0", python = ">=3.10,<3.12"}
 unstructured-inference = "0.7.21"
 torchvision = "0.16.0"
+openai = "^1.3.4"
 anthropic = "0.18.1"
-autoawq = "0.1.7"
 mistralai = "0.0.9"
+protobuf = "3.20.2"
+ragatouille = "^0.0.8.post2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
-[[tool.poetry.source]]
-name = "test"
-url = "https://test.pypi.org/simple/"
-secondary = true
-
-[[tool.poetry.source]]
-name = "torch"
-url = "https://download.pytorch.org/whl/cpu"
-priority = "explicit"
```

### Comparing `chat_rag-0.1.56/PKG-INFO` & `chat_rag-0.1.64/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: chat-rag
-Version: 0.1.56
+Version: 0.1.64
 Summary: 
 Author: Diego Peláez Paquico
 Author-email: diego.pelaez@with-madrid.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: accelerate (>=0.21.0,<0.22.0)
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: anthropic (==0.18.1)
 Requires-Dist: autoawq (==0.1.7)
 Requires-Dist: certifi (>=2023.7.22,<2024.0.0)
 Requires-Dist: cryptography (>=41.0.4,<42.0.0)
 Requires-Dist: ctransformers (>=0.2.10,<0.3.0)
 Requires-Dist: einops (>=0.6.1,<0.7.0)
 Requires-Dist: mistralai (==0.0.9)
 Requires-Dist: numpy (==1.23.5)
 Requires-Dist: openai (>=1.3.4,<2.0.0)
 Requires-Dist: pandas (==1.4.4)
 Requires-Dist: pillow (>=10.1.0,<11.0.0)
+Requires-Dist: protobuf (==3.20.2)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
-Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
+Requires-Dist: ragatouille (>=0.0.8.post2,<0.0.9)
+Requires-Dist: sentence-transformers (>=2.3.0,<3.0.0)
 Requires-Dist: torch (>=2.1.0,<3.0.0)
 Requires-Dist: torchvision (==0.16.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: transformers (>=4.35.2,<5.0.0)
+Requires-Dist: transformers (>=4.38.2,<5.0.0)
 Requires-Dist: unstructured-inference (==0.7.21)
 Requires-Dist: unstructured[pdf] (==0.12.0) ; python_version >= "3.10" and python_version < "3.12"
 Requires-Dist: urllib3 (>=1.26.18,<2.0.0)
 Description-Content-Type: text/markdown
 
 # ChatFAQ NLP Engine
```

