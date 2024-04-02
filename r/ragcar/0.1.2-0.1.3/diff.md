# Comparing `tmp/ragcar-0.1.2.tar.gz` & `tmp/ragcar-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragcar-0.1.2.tar", last modified: Sat Mar 30 08:18:04 2024, max compression
+gzip compressed data, was "ragcar-0.1.3.tar", last modified: Tue Apr  2 10:40:24 2024, max compression
```

## Comparing `ragcar-0.1.2.tar` & `ragcar-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-03-30 08:18:04.720546 ragcar-0.1.2/
--rw-rw-r--   0 pcn       (1000) pcn       (1000)    11357 2024-01-21 08:27:06.000000 ragcar-0.1.2/LICENSE
--rw-r--r--   0 pcn       (1000) pcn       (1000)      681 2024-03-30 08:18:04.720546 ragcar-0.1.2/PKG-INFO
--rw-rw-r--   0 pcn       (1000) pcn       (1000)     7546 2024-03-16 08:20:47.000000 ragcar-0.1.2/README.md
-drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-03-30 08:18:04.712545 ragcar-0.1.2/ragcar/
--rw-rw-r--   0 pcn       (1000) pcn       (1000)      111 2024-03-30 08:03:25.000000 ragcar-0.1.2/ragcar/__init__.py
-drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-03-30 08:18:04.716546 ragcar-0.1.2/ragcar/models/
--rw-rw-r--   0 pcn       (1000) pcn       (1000)        0 2024-01-21 08:28:41.000000 ragcar-0.1.2/ragcar/models/__init__.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)    18373 2024-03-14 03:57:58.000000 ragcar-0.1.2/ragcar/models/base.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)    16057 2024-03-14 07:34:57.000000 ragcar-0.1.2/ragcar/models/clova.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)    16539 2024-03-30 07:59:15.000000 ragcar-0.1.2/ragcar/models/openai.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)     7835 2024-03-14 08:37:13.000000 ragcar-0.1.2/ragcar/ragcar.py
-drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-03-30 08:18:04.716546 ragcar-0.1.2/ragcar/tools/
--rw-rw-r--   0 pcn       (1000) pcn       (1000)      406 2024-03-12 04:53:06.000000 ragcar-0.1.2/ragcar/tools/__init__.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)    26487 2024-03-13 11:32:34.000000 ragcar-0.1.2/ragcar/tools/semantic_search.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)    10056 2024-03-12 05:42:32.000000 ragcar-0.1.2/ragcar/tools/semantic_textual_similarity.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)     9442 2024-03-12 06:08:29.000000 ragcar-0.1.2/ragcar/tools/sentence_embedding.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)    10938 2024-03-30 07:58:05.000000 ragcar-0.1.2/ragcar/tools/text_generation.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)     4182 2024-03-14 10:26:30.000000 ragcar-0.1.2/ragcar/tools/text_segmentation.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)     6665 2024-03-13 12:56:43.000000 ragcar-0.1.2/ragcar/tools/tokenization.py
-drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-03-30 08:18:04.716546 ragcar-0.1.2/ragcar/tools/utils/
--rw-rw-r--   0 pcn       (1000) pcn       (1000)      175 2024-03-05 07:23:32.000000 ragcar-0.1.2/ragcar/tools/utils/__init__.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)     5462 2024-03-05 07:27:54.000000 ragcar-0.1.2/ragcar/tools/utils/base.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)     9000 2024-03-12 06:25:33.000000 ragcar-0.1.2/ragcar/tools/utils/model_config.py
-drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-03-30 08:18:04.720546 ragcar-0.1.2/ragcar/utils/
--rw-rw-r--   0 pcn       (1000) pcn       (1000)      340 2024-03-05 07:24:31.000000 ragcar-0.1.2/ragcar/utils/__init__.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)     2777 2024-03-07 07:53:48.000000 ragcar-0.1.2/ragcar/utils/chat_summarizer.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)     2444 2024-03-07 07:46:23.000000 ragcar-0.1.2/ragcar/utils/history_manager.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)     1952 2024-03-07 07:21:38.000000 ragcar-0.1.2/ragcar/utils/memory_manager.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)     8562 2024-03-07 07:02:35.000000 ragcar-0.1.2/ragcar/utils/prompt_template.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)     4197 2024-03-07 07:19:19.000000 ragcar-0.1.2/ragcar/utils/token_limiter.py
--rw-rw-r--   0 pcn       (1000) pcn       (1000)    18051 2024-03-07 07:00:56.000000 ragcar-0.1.2/ragcar/utils/vector_indexer.py
-drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-03-30 08:18:04.716546 ragcar-0.1.2/ragcar.egg-info/
--rw-r--r--   0 pcn       (1000) pcn       (1000)      681 2024-03-30 08:18:04.000000 ragcar-0.1.2/ragcar.egg-info/PKG-INFO
--rw-rw-r--   0 pcn       (1000) pcn       (1000)      843 2024-03-30 08:18:04.000000 ragcar-0.1.2/ragcar.egg-info/SOURCES.txt
--rw-rw-r--   0 pcn       (1000) pcn       (1000)        1 2024-03-30 08:18:04.000000 ragcar-0.1.2/ragcar.egg-info/dependency_links.txt
--rw-rw-r--   0 pcn       (1000) pcn       (1000)      189 2024-03-30 08:18:04.000000 ragcar-0.1.2/ragcar.egg-info/requires.txt
--rw-rw-r--   0 pcn       (1000) pcn       (1000)        7 2024-03-30 08:18:04.000000 ragcar-0.1.2/ragcar.egg-info/top_level.txt
--rw-rw-r--   0 pcn       (1000) pcn       (1000)       38 2024-03-30 08:18:04.720546 ragcar-0.1.2/setup.cfg
--rw-rw-r--   0 pcn       (1000) pcn       (1000)      740 2024-03-30 08:03:16.000000 ragcar-0.1.2/setup.py
+drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-04-02 10:40:24.343767 ragcar-0.1.3/
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)    11357 2024-01-21 08:27:06.000000 ragcar-0.1.3/LICENSE
+-rw-r--r--   0 pcn       (1000) pcn       (1000)      681 2024-04-02 10:40:24.343767 ragcar-0.1.3/PKG-INFO
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)     7546 2024-03-16 08:20:47.000000 ragcar-0.1.3/README.md
+drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-04-02 10:40:24.339767 ragcar-0.1.3/ragcar/
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)      111 2024-04-02 10:28:43.000000 ragcar-0.1.3/ragcar/__init__.py
+drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-04-02 10:40:24.339767 ragcar-0.1.3/ragcar/models/
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)        0 2024-01-21 08:28:41.000000 ragcar-0.1.3/ragcar/models/__init__.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)    18284 2024-04-02 10:27:12.000000 ragcar-0.1.3/ragcar/models/base.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)    16061 2024-04-02 10:23:18.000000 ragcar-0.1.3/ragcar/models/clova.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)    16768 2024-04-02 10:20:31.000000 ragcar-0.1.3/ragcar/models/openai.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)     7835 2024-03-14 08:37:13.000000 ragcar-0.1.3/ragcar/ragcar.py
+drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-04-02 10:40:24.343767 ragcar-0.1.3/ragcar/tools/
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)      406 2024-03-12 04:53:06.000000 ragcar-0.1.3/ragcar/tools/__init__.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)    26487 2024-03-13 11:32:34.000000 ragcar-0.1.3/ragcar/tools/semantic_search.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)    10056 2024-03-12 05:42:32.000000 ragcar-0.1.3/ragcar/tools/semantic_textual_similarity.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)     9442 2024-03-12 06:08:29.000000 ragcar-0.1.3/ragcar/tools/sentence_embedding.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)    10938 2024-03-30 07:58:05.000000 ragcar-0.1.3/ragcar/tools/text_generation.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)     4182 2024-03-14 10:26:30.000000 ragcar-0.1.3/ragcar/tools/text_segmentation.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)     6665 2024-03-13 12:56:43.000000 ragcar-0.1.3/ragcar/tools/tokenization.py
+drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-04-02 10:40:24.343767 ragcar-0.1.3/ragcar/tools/utils/
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)      175 2024-03-05 07:23:32.000000 ragcar-0.1.3/ragcar/tools/utils/__init__.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)     5462 2024-03-05 07:27:54.000000 ragcar-0.1.3/ragcar/tools/utils/base.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)     9000 2024-03-12 06:25:33.000000 ragcar-0.1.3/ragcar/tools/utils/model_config.py
+drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-04-02 10:40:24.343767 ragcar-0.1.3/ragcar/utils/
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)      340 2024-03-05 07:24:31.000000 ragcar-0.1.3/ragcar/utils/__init__.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)     2777 2024-03-07 07:53:48.000000 ragcar-0.1.3/ragcar/utils/chat_summarizer.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)     2444 2024-03-07 07:46:23.000000 ragcar-0.1.3/ragcar/utils/history_manager.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)     1952 2024-03-07 07:21:38.000000 ragcar-0.1.3/ragcar/utils/memory_manager.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)     8562 2024-03-07 07:02:35.000000 ragcar-0.1.3/ragcar/utils/prompt_template.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)     4197 2024-03-07 07:19:19.000000 ragcar-0.1.3/ragcar/utils/token_limiter.py
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)    18051 2024-03-07 07:00:56.000000 ragcar-0.1.3/ragcar/utils/vector_indexer.py
+drwxrwxr-x   0 pcn       (1000) pcn       (1000)        0 2024-04-02 10:40:24.339767 ragcar-0.1.3/ragcar.egg-info/
+-rw-r--r--   0 pcn       (1000) pcn       (1000)      681 2024-04-02 10:40:24.000000 ragcar-0.1.3/ragcar.egg-info/PKG-INFO
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)      843 2024-04-02 10:40:24.000000 ragcar-0.1.3/ragcar.egg-info/SOURCES.txt
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)        1 2024-04-02 10:40:24.000000 ragcar-0.1.3/ragcar.egg-info/dependency_links.txt
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)      189 2024-04-02 10:40:24.000000 ragcar-0.1.3/ragcar.egg-info/requires.txt
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)        7 2024-04-02 10:40:24.000000 ragcar-0.1.3/ragcar.egg-info/top_level.txt
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)       38 2024-04-02 10:40:24.347767 ragcar-0.1.3/setup.cfg
+-rw-rw-r--   0 pcn       (1000) pcn       (1000)      740 2024-04-02 10:28:18.000000 ragcar-0.1.3/setup.py
```

### Comparing `ragcar-0.1.2/LICENSE` & `ragcar-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/PKG-INFO` & `ragcar-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragcar
-Version: 0.1.2
+Version: 0.1.3
 Summary: RAGCAR: Retrieval-Augmented Generative Companion for Advanced Research
 Home-page: https://github.com/leewaay/ragcar.git
 Author: Wonseok Lee
 Author-email: wonsuklee7020@gmail.com
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: torch==2.0.1
```

### Comparing `ragcar-0.1.2/README.md` & `ragcar-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/models/base.py` & `ragcar-0.1.3/ragcar/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,23 +105,21 @@
         total_cost_in_krw = total_tokens * cost_per_input_token
 
         return total_cost_in_krw
     
     def format_response(
         self, 
         response_data,
-        request_id: str,
         response_time: float
     ) -> Dict[str, Union[str, int, float, Dict]]:
         """
         Format the response from the API.
 
         Args:
             response_data (Dict): The raw response from the API, expected to contain result details.
-            request_id (str): The unique identifier of the request.
             response_time (float): The time (in seconds) it took to get the response from the API.
 
         Returns:
             Dict[str, Union[str, int, float, Dict]]: A dictionary containing formatted response details, including:
                 - id (str): The request identifier.
                 - model (str): The model name used for the request.
                 - content (str): The main content message from the response.
@@ -146,26 +144,26 @@
         model_type = self._get_model_type(self.api_url)
         predicted_cost = self._calculate_charge_per_request(model_type, total_tokens)
         
         ai_filter = result.get('aiFilter')
         if ai_filter:
             ai_filter = {item['name']: int(item['score']) for item in ai_filter}
         
-        formatted_data = {
-            "id": request_id,
-            "model": self.model_n,
+        formatted_data = response_data.get('id', {})
+        formatted_data.update({
             "content": content,
+            "model": self.model_n,
             "finish_reason": finish_reason,
             "input_tokens": input_tokens,
             "output_tokens": output_tokens,
             "total_tokens": total_tokens,
             "predicted_cost": predicted_cost if predicted_cost is not None else "Unknown",
             "response_time": response_time,
             "ai_filter": ai_filter
-        }
+        })
             
         return formatted_data
     
     def fetch(self, **kwargs: dict) -> dict:
         """
         Send a POST request to the API.
 
@@ -391,23 +389,21 @@
             total_cost_in_usd += output_tokens * cost_per_output_token
 
         return total_cost_in_usd
 
     def format_response(
         self,
         response_data,
-        request_id: str,
         response_time: float
     ) -> Dict[str, Union[str, int, float]]:
         """
         Format the response from the API.
 
         Args:
             response_data (dict): The raw response data from the API.
-            request_id (str): The unique identifier for the request.
             response_time (float): The duration it took to receive the response, in seconds.
 
         Returns:
             Dict[str, Union[str, int, float]]: A dictionary containing the formatted response data. This includes:
                 - id (str): The request ID.
                 - model (str): The model name used for the request.
                 - content (str): The main content returned by the API.
@@ -433,25 +429,25 @@
         usage = response_data.get('usage', {})
         input_tokens = usage.get('prompt_tokens')
         output_tokens = usage.get('completion_tokens')
         total_tokens = (input_tokens or 0) + (output_tokens or 0)
         
         predicted_cost = self._calculate_charge_per_request(model_type, input_tokens, output_tokens)
         
-        formatted_data = {
-            "id": request_id,
+        formatted_data = {"id": response_data.get('id')} if  response_data.get('id') else {}
+        formatted_data.update({
             "model": self.model_n,
             "content": content,
             "finish_reason": finish_reason,
             "input_tokens": input_tokens,
             "output_tokens": output_tokens,
             "total_tokens": total_tokens,
             "predicted_cost": predicted_cost if predicted_cost is not None else "Unknown",
             "response_time": response_time
-        }
+        })
             
         return formatted_data
 
     def fetch(self, create_fn, **kwargs) -> Union[Tuple[dict, str], Tuple[Generator[dict, None, None], str]]:
         """
         Calls an external service and logs the request and response.
```

### Comparing `ragcar-0.1.2/ragcar/models/clova.py` & `ragcar-0.1.3/ragcar/models/clova.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,17 +241,19 @@
     
     def _output(
         self,
         res,
         request_id,
         start_time
     ) -> Dict[str, Union[str, int, float]]:
+        res["id"] = request_id
+        
         if self.formatting:
             response_time = time.time() - start_time
-            formatted_data = self.format_response(res, request_id, response_time)
+            formatted_data = self.format_response(res, response_time)
             
             logger.info(json.dumps(res, ensure_ascii=False, indent=4))
             return formatted_data
         else:
             return res
     
     def _stream_output(
@@ -293,15 +295,15 @@
                             response_time = time.time() - start_time
                             
                             default_format = {"result": current_event['data']}
                             
                             yield {
                                     "id": request_id,
                                     "event": "finish",
-                                    "data": self.format_response(default_format, request_id, response_time)
+                                    "data": self.format_response(default_format, response_time)
                                 }
                     else:
                         yield current_event
                 
                     current_event = {}
     
     def create(self, messages: str, **kwargs) -> Union[str, Generator[str, None, None]]:
@@ -354,15 +356,15 @@
                             response_time = time.time() - start_time
                             
                             default_format = {"result": current_event['data']}
                             
                             yield {
                                     "id": request_id,
                                     "event": "finish",
-                                    "data": self.format_response(default_format, request_id, response_time)
+                                    "data": self.format_response(default_format, response_time)
                                 }
                     else:
                         yield current_event
     
     async def acreate(self, messages: str, **kwargs) -> Union[str, AsyncGenerator[str, None]]:
         params = self._get_params(messages, **kwargs)
```

### Comparing `ragcar-0.1.2/ragcar/models/openai.py` & `ragcar-0.1.3/ragcar/models/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,17 +109,19 @@
     
     def _output(
         self,
         res,
         request_id,
         start_time
     ) -> Dict[str, Union[str, int, float]]:
+        res["id"] = request_id
+        
         if self.formatting:
             response_time = time.time() - start_time
-            formatted_data = self.format_response(res, request_id, response_time)
+            formatted_data = self.format_response(res, response_time)
         
             logger.info(json.dumps(res, ensure_ascii=False, indent=4))
             return formatted_data
         else:
             return res
     
     def _stream_output(
@@ -128,14 +130,16 @@
         request_id,
         start_time,
         has_functions,
         prompt
     ) -> Generator[str, None, None]:
         message = ""
         for chunk in res:
+            chunk["id"] = request_id
+            
             if self.formatting:
                 logger.info(json.dumps(chunk, ensure_ascii=False, indent=4))
                 
                 choice = chunk.get('choices', [{}])[0]
                 
                 delta = choice.get('delta', {})
                 finish_reason = choice.get('finish_reason')
@@ -175,15 +179,15 @@
                             "total_tokens": prompt_tokens + completion_tokens
                         }
                     }
                     
                     yield {
                         "id": request_id,
                         "event": "finish",
-                        "data": self.format_response(default_format, request_id, response_time)
+                        "data": self.format_response(default_format, response_time)
                     }
             else:
                 chunk["id"] = request_id
                 yield chunk
     
     def create(
         self, 
@@ -206,14 +210,16 @@
         request_id,
         start_time,
         has_functions,
         prompt
     ) -> AsyncGenerator[str, None]:
         message = ""
         async for chunk in res:
+            chunk["id"] = request_id
+            
             if self.formatting:
                 logger.info(json.dumps(chunk, ensure_ascii=False, indent=4))
                 
                 choice = chunk.get('choices', [{}])[0]
                 
                 delta = choice.get('delta', {})
                 finish_reason = choice.get('finish_reason')
@@ -253,15 +259,15 @@
                             "total_tokens": prompt_tokens + completion_tokens
                         }
                     }
                     
                     yield {
                         "id": request_id,
                         "event": "finish",
-                        "data": self.format_response(default_format, request_id, response_time)
+                        "data": self.format_response(default_format, response_time)
                     }
             else:
                 chunk["id"] = request_id
                 yield chunk
     
     async def acreate(self, messages, **kwargs) -> Union[str, AsyncGenerator[str, None]]:
         params = self._get_params(messages, **kwargs)
@@ -334,17 +340,19 @@
     
     def _output(
         self,
         res,
         request_id,
         start_time
     ) -> Dict[str, Union[str, int, float]]:
+        res["id"] = request_id
+        
         if self.formatting:
             response_time = time.time() - start_time
-            formatted_data = self.format_response(res, request_id, response_time)
+            formatted_data = self.format_response(res, response_time)
         
             logger.info(json.dumps(res, ensure_ascii=False, indent=4))
             return formatted_data
         else:
             return res
     
     def _stream_output(
@@ -352,14 +360,16 @@
         res, 
         request_id, 
         start_time,
         prompt
     ) -> Generator[str, None, None]:
         message = ""
         for chunk in res:
+            chunk["id"] = request_id
+            
             if self.formatting:
                 logger.info(json.dumps(chunk, ensure_ascii=False, indent=4))
                 
                 choice = chunk.get('choices', [{}])[0]
                 
                 content = choice[0].get('text', {})
                 finish_reason = choice.get('finish_reason')
@@ -390,15 +400,15 @@
                             "total_tokens": prompt_tokens + completion_tokens
                         }
                     }
                     
                     yield {
                         "id": request_id,
                         "event": "finish",
-                        "data": self.format_response(default_format, request_id, response_time)
+                        "data": self.format_response(default_format, response_time)
                     }
             else:
                 chunk["id"] = request_id
                 yield chunk
     
     def create(self, prompt, **kwargs) -> Union[str, Generator[str, None, None]]:
         params = self._get_params(prompt, **kwargs)
@@ -407,17 +417,25 @@
         res, request_id = self.fetch(openai.Completion.create, **params)
         
         if params.get('stream'):
             return self._stream_output(res, request_id, start_time, params.get("functions"), prompt)
         
         return self._output(res, request_id, start_time)
 
-    async def _astream_output(self, res, request_id) -> AsyncGenerator[str, None]:
+    async def _astream_output(
+        self, 
+        res, 
+        request_id, 
+        start_time,
+        prompt
+    ) -> AsyncGenerator[str, None]:
         message = ""
         async for chunk in res:
+            chunk["id"] = request_id
+            
             if self.formatting:
                 logger.info(json.dumps(chunk, ensure_ascii=False, indent=4))
                 
                 choice = chunk.get('choices', [{}])[0]
                 
                 content = choice[0].get('text', {})
                 finish_reason = choice.get('finish_reason')
@@ -448,24 +466,23 @@
                             "total_tokens": prompt_tokens + completion_tokens
                         }
                     }
                     
                     yield {
                         "id": request_id,
                         "event": "finish",
-                        "data": self.format_response(default_format, request_id, response_time)
+                        "data": self.format_response(default_format, response_time)
                     }
             else:
                 chunk["id"] = request_id
                 yield chunk
     
     async def acreate(self, prompt, **kwargs) -> Union[str, AsyncGenerator[str, None]]:
         params = self._get_params(prompt, **kwargs)
         
         start_time = time.time()
         res, request_id = await self.afetch(openai.Completion.acreate, **params)
-        response_time = time.time() - start_time
         
         if params.get('stream'):
-            return self._stream_output(res, request_id, start_time, params.get("functions"), prompt)
+            return self._astream_output(res, request_id, start_time, params.get("functions"), prompt)
         
         return self._output(res, request_id, start_time)
```

### Comparing `ragcar-0.1.2/ragcar/ragcar.py` & `ragcar-0.1.3/ragcar/ragcar.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/tools/semantic_search.py` & `ragcar-0.1.3/ragcar/tools/semantic_search.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/tools/semantic_textual_similarity.py` & `ragcar-0.1.3/ragcar/tools/semantic_textual_similarity.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/tools/sentence_embedding.py` & `ragcar-0.1.3/ragcar/tools/sentence_embedding.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/tools/text_generation.py` & `ragcar-0.1.3/ragcar/tools/text_generation.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/tools/text_segmentation.py` & `ragcar-0.1.3/ragcar/tools/text_segmentation.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/tools/tokenization.py` & `ragcar-0.1.3/ragcar/tools/tokenization.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/tools/utils/base.py` & `ragcar-0.1.3/ragcar/tools/utils/base.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/tools/utils/model_config.py` & `ragcar-0.1.3/ragcar/tools/utils/model_config.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/utils/chat_summarizer.py` & `ragcar-0.1.3/ragcar/utils/chat_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/utils/history_manager.py` & `ragcar-0.1.3/ragcar/utils/history_manager.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/utils/memory_manager.py` & `ragcar-0.1.3/ragcar/utils/memory_manager.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/utils/prompt_template.py` & `ragcar-0.1.3/ragcar/utils/prompt_template.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/utils/token_limiter.py` & `ragcar-0.1.3/ragcar/utils/token_limiter.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar/utils/vector_indexer.py` & `ragcar-0.1.3/ragcar/utils/vector_indexer.py`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/ragcar.egg-info/PKG-INFO` & `ragcar-0.1.3/ragcar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragcar
-Version: 0.1.2
+Version: 0.1.3
 Summary: RAGCAR: Retrieval-Augmented Generative Companion for Advanced Research
 Home-page: https://github.com/leewaay/ragcar.git
 Author: Wonseok Lee
 Author-email: wonsuklee7020@gmail.com
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: torch==2.0.1
```

### Comparing `ragcar-0.1.2/ragcar.egg-info/SOURCES.txt` & `ragcar-0.1.3/ragcar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ragcar-0.1.2/setup.py` & `ragcar-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ragcar', 
-    version='0.1.2', 
+    version='0.1.3', 
     url='https://github.com/leewaay/ragcar.git', 
     author='Wonseok Lee', 
     author_email='wonsuklee7020@gmail.com', 
     description='RAGCAR: Retrieval-Augmented Generative Companion for Advanced Research', 
     packages=find_packages(), 
     python_requires='>=3.8',
     install_requires=[
```

