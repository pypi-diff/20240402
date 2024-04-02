# Comparing `tmp/langchain_qianwen-0.1.8.tar.gz` & `tmp/langchain_qianwen-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_qianwen-0.1.8.tar", last modified: Fri Nov  3 07:47:08 2023, max compression
+gzip compressed data, was "langchain_qianwen-0.1.9.tar", last modified: Fri Nov  3 07:56:20 2023, max compression
```

## Comparing `langchain_qianwen-0.1.8.tar` & `langchain_qianwen-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 devin      (501) staff       (20)        0 2023-11-03 07:47:08.831369 langchain_qianwen-0.1.8/
--rw-r--r--   0 devin      (501) staff       (20)     4324 2023-11-03 07:47:08.831258 langchain_qianwen-0.1.8/PKG-INFO
--rw-r--r--   0 devin      (501) staff       (20)     3898 2023-11-02 08:19:14.000000 langchain_qianwen-0.1.8/README.md
-drwxr-xr-x   0 devin      (501) staff       (20)        0 2023-11-03 07:47:08.830004 langchain_qianwen-0.1.8/langchain_qianwen/
--rw-r--r--   0 devin      (501) staff       (20)      124 2023-10-07 11:42:54.000000 langchain_qianwen-0.1.8/langchain_qianwen/__init__.py
-drwxr-xr-x   0 devin      (501) staff       (20)        0 2023-11-03 07:47:08.830779 langchain_qianwen-0.1.8/langchain_qianwen/agents/
--rw-r--r--   0 devin      (501) staff       (20)       74 2023-10-07 11:42:54.000000 langchain_qianwen-0.1.8/langchain_qianwen/agents/__init__.py
-drwxr-xr-x   0 devin      (501) staff       (20)        0 2023-11-03 07:47:08.831090 langchain_qianwen-0.1.8/langchain_qianwen/agents/mkrl_cn/
--rw-r--r--   0 devin      (501) staff       (20)       85 2023-10-07 11:42:54.000000 langchain_qianwen-0.1.8/langchain_qianwen/agents/mkrl_cn/__init__.py
--rw-r--r--   0 devin      (501) staff       (20)      882 2023-10-07 11:42:54.000000 langchain_qianwen-0.1.8/langchain_qianwen/agents/mkrl_cn/prompt.py
--rw-r--r--   0 devin      (501) staff       (20)     3105 2023-10-07 11:42:54.000000 langchain_qianwen-0.1.8/langchain_qianwen/agents/mkrl_cn/zero_shot_agent_cn.py
--rw-r--r--   0 devin      (501) staff       (20)     3175 2023-10-08 12:00:36.000000 langchain_qianwen-0.1.8/langchain_qianwen/commons.py
--rw-r--r--   0 devin      (501) staff       (20)     1609 2023-10-07 11:42:54.000000 langchain_qianwen-0.1.8/langchain_qianwen/qwen_adaptor.py
--rw-r--r--   0 devin      (501) staff       (20)    10348 2023-11-02 08:34:12.000000 langchain_qianwen-0.1.8/langchain_qianwen/qwen_chat_model.py
--rw-r--r--   0 devin      (501) staff       (20)    11056 2023-11-01 04:11:35.000000 langchain_qianwen-0.1.8/langchain_qianwen/qwen_llm.py
-drwxr-xr-x   0 devin      (501) staff       (20)        0 2023-11-03 07:47:08.830648 langchain_qianwen-0.1.8/langchain_qianwen.egg-info/
--rw-r--r--   0 devin      (501) staff       (20)     4324 2023-11-03 07:47:08.000000 langchain_qianwen-0.1.8/langchain_qianwen.egg-info/PKG-INFO
--rw-r--r--   0 devin      (501) staff       (20)      562 2023-11-03 07:47:08.000000 langchain_qianwen-0.1.8/langchain_qianwen.egg-info/SOURCES.txt
--rw-r--r--   0 devin      (501) staff       (20)        1 2023-11-03 07:47:08.000000 langchain_qianwen-0.1.8/langchain_qianwen.egg-info/dependency_links.txt
--rw-r--r--   0 devin      (501) staff       (20)       37 2023-11-03 07:47:08.000000 langchain_qianwen-0.1.8/langchain_qianwen.egg-info/requires.txt
--rw-r--r--   0 devin      (501) staff       (20)       18 2023-11-03 07:47:08.000000 langchain_qianwen-0.1.8/langchain_qianwen.egg-info/top_level.txt
--rw-r--r--   0 devin      (501) staff       (20)       38 2023-11-03 07:47:08.831405 langchain_qianwen-0.1.8/setup.cfg
--rw-r--r--   0 devin      (501) staff       (20)      695 2023-11-03 07:46:46.000000 langchain_qianwen-0.1.8/setup.py
+drwxr-xr-x   0 devin      (501) staff       (20)        0 2023-11-03 07:56:20.937730 langchain_qianwen-0.1.9/
+-rw-r--r--   0 devin      (501) staff       (20)     4324 2023-11-03 07:56:20.937590 langchain_qianwen-0.1.9/PKG-INFO
+-rw-r--r--   0 devin      (501) staff       (20)     3898 2023-11-02 08:19:14.000000 langchain_qianwen-0.1.9/README.md
+drwxr-xr-x   0 devin      (501) staff       (20)        0 2023-11-03 07:56:20.936174 langchain_qianwen-0.1.9/langchain_qianwen/
+-rw-r--r--   0 devin      (501) staff       (20)      124 2023-10-07 11:42:54.000000 langchain_qianwen-0.1.9/langchain_qianwen/__init__.py
+drwxr-xr-x   0 devin      (501) staff       (20)        0 2023-11-03 07:56:20.936961 langchain_qianwen-0.1.9/langchain_qianwen/agents/
+-rw-r--r--   0 devin      (501) staff       (20)       74 2023-10-07 11:42:54.000000 langchain_qianwen-0.1.9/langchain_qianwen/agents/__init__.py
+drwxr-xr-x   0 devin      (501) staff       (20)        0 2023-11-03 07:56:20.937384 langchain_qianwen-0.1.9/langchain_qianwen/agents/mkrl_cn/
+-rw-r--r--   0 devin      (501) staff       (20)       85 2023-10-07 11:42:54.000000 langchain_qianwen-0.1.9/langchain_qianwen/agents/mkrl_cn/__init__.py
+-rw-r--r--   0 devin      (501) staff       (20)      882 2023-10-07 11:42:54.000000 langchain_qianwen-0.1.9/langchain_qianwen/agents/mkrl_cn/prompt.py
+-rw-r--r--   0 devin      (501) staff       (20)     3105 2023-10-07 11:42:54.000000 langchain_qianwen-0.1.9/langchain_qianwen/agents/mkrl_cn/zero_shot_agent_cn.py
+-rw-r--r--   0 devin      (501) staff       (20)     3175 2023-10-08 12:00:36.000000 langchain_qianwen-0.1.9/langchain_qianwen/commons.py
+-rw-r--r--   0 devin      (501) staff       (20)     1609 2023-10-07 11:42:54.000000 langchain_qianwen-0.1.9/langchain_qianwen/qwen_adaptor.py
+-rw-r--r--   0 devin      (501) staff       (20)    10364 2023-11-03 07:55:38.000000 langchain_qianwen-0.1.9/langchain_qianwen/qwen_chat_model.py
+-rw-r--r--   0 devin      (501) staff       (20)    11056 2023-11-01 04:11:35.000000 langchain_qianwen-0.1.9/langchain_qianwen/qwen_llm.py
+drwxr-xr-x   0 devin      (501) staff       (20)        0 2023-11-03 07:56:20.936820 langchain_qianwen-0.1.9/langchain_qianwen.egg-info/
+-rw-r--r--   0 devin      (501) staff       (20)     4324 2023-11-03 07:56:20.000000 langchain_qianwen-0.1.9/langchain_qianwen.egg-info/PKG-INFO
+-rw-r--r--   0 devin      (501) staff       (20)      562 2023-11-03 07:56:20.000000 langchain_qianwen-0.1.9/langchain_qianwen.egg-info/SOURCES.txt
+-rw-r--r--   0 devin      (501) staff       (20)        1 2023-11-03 07:56:20.000000 langchain_qianwen-0.1.9/langchain_qianwen.egg-info/dependency_links.txt
+-rw-r--r--   0 devin      (501) staff       (20)       37 2023-11-03 07:56:20.000000 langchain_qianwen-0.1.9/langchain_qianwen.egg-info/requires.txt
+-rw-r--r--   0 devin      (501) staff       (20)       18 2023-11-03 07:56:20.000000 langchain_qianwen-0.1.9/langchain_qianwen.egg-info/top_level.txt
+-rw-r--r--   0 devin      (501) staff       (20)       38 2023-11-03 07:56:20.937770 langchain_qianwen-0.1.9/setup.cfg
+-rw-r--r--   0 devin      (501) staff       (20)      695 2023-11-03 07:55:52.000000 langchain_qianwen-0.1.9/setup.py
```

### Comparing `langchain_qianwen-0.1.8/PKG-INFO` & `langchain_qianwen-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_qianwen
-Version: 0.1.8
+Version: 0.1.9
 Summary: 通义千问 Qianwen Langchain adapter
 Home-page: https://github.com/dyfsquall/langchain_qianwen
 Author: Devin YF
 Author-email: dyfsquall@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `langchain_qianwen-0.1.8/README.md` & `langchain_qianwen-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `langchain_qianwen-0.1.8/langchain_qianwen/agents/mkrl_cn/prompt.py` & `langchain_qianwen-0.1.9/langchain_qianwen/agents/mkrl_cn/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_qianwen-0.1.8/langchain_qianwen/agents/mkrl_cn/zero_shot_agent_cn.py` & `langchain_qianwen-0.1.9/langchain_qianwen/agents/mkrl_cn/zero_shot_agent_cn.py`

 * *Files identical despite different names*

### Comparing `langchain_qianwen-0.1.8/langchain_qianwen/commons.py` & `langchain_qianwen-0.1.9/langchain_qianwen/commons.py`

 * *Files identical despite different names*

### Comparing `langchain_qianwen-0.1.8/langchain_qianwen/qwen_adaptor.py` & `langchain_qianwen-0.1.9/langchain_qianwen/qwen_adaptor.py`

 * *Files identical despite different names*

### Comparing `langchain_qianwen-0.1.8/langchain_qianwen/qwen_chat_model.py` & `langchain_qianwen-0.1.9/langchain_qianwen/qwen_chat_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,45 +18,45 @@
     SystemMessageChunk,
     HumanMessageChunk,
 )
 from langchain.adapters.openai import (
         convert_dict_to_message, convert_message_to_dict
     )
 
+import asyncio
+from functools import partial
 
-# from .commons import _create_retry_decorator
 from .commons import (
     completion_with_retry, response_text_format, response_handler)
 
-from typing import (Dict, Any, Optional, List, 
+from typing import (Dict, Any, Optional, List,
                     Iterator, Tuple, Mapping, AsyncIterator)
 
 logger = logging.getLogger(__name__)
 
 
 def _stream_response_to_chat_generation_chunk(
     stream_response: Dict[str, Any],
 ) -> ChatGenerationChunk:
     """Convert a stream response to a chat generation chunk."""
-    # TODO:...
     msg = stream_response["output"]["choices"][0]["message"]
     role = msg["role"]
     text = msg["content"]
 
     msg_chunk = None
-    
+
     if role == "user":
         msg_chunk = HumanMessageChunk(content=text)
     elif role == "assistant":
         msg_chunk = AIMessageChunk(content=text)
     elif role == "system":
         msg_chunk = SystemMessageChunk(content=text)
     else:
         msg_chunk = ChatMessageChunk(content=text, role=role)
-    
+
     return ChatGenerationChunk(
         message=msg_chunk,
         generation_info=dict(
             finish_reason=stream_response["output"]["choices"][0].get("finish_reason", None),
         ),
     )
 
@@ -212,29 +212,31 @@
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> AsyncIterator[ChatGenerationChunk]:
         # TODO: Implement later
         raise NotImplementedError()
 
-
     async def _agenerate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> ChatResult:
         """Top Level call"""
         # TODO: Implement later
         return await asyncio.get_running_loop().run_in_executor(
-            None, partial(self._generate, **kwargs), messages, stop, run_manager
+            None,
+            partial(self._generate, **kwargs),
+            messages,
+            stop,
+            run_manager
         )
 
-
     def _create_message_dicts(
         self, messages: List[BaseMessage], stop: Optional[List[str]]
     ) -> Tuple[List[Dict[str, Any]]]:
         message_dicts = [convert_message_to_dict(m) for m in messages]
         return message_dicts
 
     def _create_chat_result(self, response: Mapping[str, Any]) -> ChatResult:
@@ -263,15 +265,15 @@
             llm_output = {"token_usage": {"input_tokens": 0, "output_tokens": 0}, "model_name": self.model_name}
         return ChatResult(generations=generations, llm_output=llm_output)
 
     @property
     def _identifying_params(self) -> Dict[str, Any]:
         """Get the identifying parameters."""
         return {**{"model_name": self.model_name}, **self._default_params}
-    
+
     def _get_invocation_params(
         self, stop: Optional[List[str]] = None, **kwargs: Any
     ) -> Dict[str, Any]:
         """Get the parameters used to invoke the model."""
         return {
             "model": self.model_name,
             **super()._get_invocation_params(stop=stop),
```

### Comparing `langchain_qianwen-0.1.8/langchain_qianwen/qwen_llm.py` & `langchain_qianwen-0.1.9/langchain_qianwen/qwen_llm.py`

 * *Files identical despite different names*

### Comparing `langchain_qianwen-0.1.8/langchain_qianwen.egg-info/PKG-INFO` & `langchain_qianwen-0.1.9/langchain_qianwen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-qianwen
-Version: 0.1.8
+Version: 0.1.9
 Summary: 通义千问 Qianwen Langchain adapter
 Home-page: https://github.com/dyfsquall/langchain_qianwen
 Author: Devin YF
 Author-email: dyfsquall@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `langchain_qianwen-0.1.8/langchain_qianwen.egg-info/SOURCES.txt` & `langchain_qianwen-0.1.9/langchain_qianwen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langchain_qianwen-0.1.8/setup.py` & `langchain_qianwen-0.1.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='langchain_qianwen',
-    version='0.1.8',
+    version='0.1.9',
     author='Devin YF',
     author_email='dyfsquall@qq.com',
     description='通义千问 Qianwen Langchain adapter',
     install_requires=[
         'langchain==0.0.327',
         'dashscope==1.13.1',
     ],
```

