# Comparing `tmp/webscout-1.2.3.tar.gz` & `tmp/webscout-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.2.3.tar", last modified: Sun Mar 31 08:41:30 2024, max compression
+gzip compressed data, was "webscout-1.2.4.tar", last modified: Tue Apr  2 11:47:11 2024, max compression
```

## Comparing `webscout-1.2.3.tar` & `webscout-1.2.4.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 08:41:30.775875 webscout-1.2.3/
-drwxrwxrwx   0        0        0        0 2024-03-31 08:41:30.620113 webscout-1.2.3/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-03-30 13:50:55.000000 webscout-1.2.3/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 08:41:30.631063 webscout-1.2.3/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-03-30 12:07:30.000000 webscout-1.2.3/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-03-31 07:51:09.000000 webscout-1.2.3/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-03-31 07:29:21.000000 webscout-1.2.3/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-03-31 08:41:30.655116 webscout-1.2.3/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-03-30 12:07:30.000000 webscout-1.2.3/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-03-30 15:25:09.000000 webscout-1.2.3/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-03-30 15:31:47.000000 webscout-1.2.3/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-03-30 15:33:35.000000 webscout-1.2.3/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3846 2024-03-31 07:20:27.000000 webscout-1.2.3/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-03-31 08:41:30.665040 webscout-1.2.3/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-03-30 12:07:30.000000 webscout-1.2.3/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     1754 2024-03-30 13:44:05.000000 webscout-1.2.3/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-03-30 12:07:30.000000 webscout-1.2.3/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-03-30 04:49:10.000000 webscout-1.2.3/LICENSE.md
--rw-rw-rw-   0        0        0    21760 2024-03-31 08:41:30.772869 webscout-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    19641 2024-03-31 08:36:01.000000 webscout-1.2.3/README.md
--rw-rw-rw-   0        0        0       42 2024-03-31 08:41:30.776875 webscout-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     2789 2024-03-31 08:37:26.000000 webscout-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 08:41:30.732878 webscout-1.2.3/webscout/
--rw-rw-rw-   0        0        0    49618 2024-03-30 04:49:10.000000 webscout-1.2.3/webscout/AI.py
--rw-rw-rw-   0        0        0     2343 2024-03-30 04:49:10.000000 webscout-1.2.3/webscout/AIbase.py
--rw-rw-rw-   0        0        0    24124 2024-03-30 04:49:10.000000 webscout-1.2.3/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7135 2024-03-31 07:48:07.000000 webscout-1.2.3/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     8103 2024-03-30 04:49:10.000000 webscout-1.2.3/webscout/HelpingAI.py
--rw-rw-rw-   0        0        0     3309 2024-03-30 04:49:10.000000 webscout-1.2.3/webscout/LLM.py
--rw-rw-rw-   0        0        0      425 2024-03-30 14:17:36.000000 webscout-1.2.3/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-03-30 04:49:10.000000 webscout-1.2.3/webscout/__main__.py
--rw-rw-rw-   0        0        0    17059 2024-03-30 13:23:04.000000 webscout-1.2.3/webscout/cli.py
--rw-rw-rw-   0        0        0      276 2024-03-30 04:55:59.000000 webscout-1.2.3/webscout/exceptions.py
--rw-rw-rw-   0        0        0      692 2024-03-30 04:49:10.000000 webscout-1.2.3/webscout/models.py
--rw-rw-rw-   0        0        0     2605 2024-03-30 04:52:23.000000 webscout-1.2.3/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-03-31 08:37:34.000000 webscout-1.2.3/webscout/version.py
--rw-rw-rw-   0        0        0     3085 2024-03-30 06:47:38.000000 webscout-1.2.3/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-03-30 13:23:04.000000 webscout-1.2.3/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-03-31 08:41:30.766875 webscout-1.2.3/webscout.egg-info/
--rw-rw-rw-   0        0        0    21760 2024-03-31 08:41:29.000000 webscout-1.2.3/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      941 2024-03-31 08:41:30.000000 webscout-1.2.3/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 08:41:29.000000 webscout-1.2.3/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-03-31 08:41:29.000000 webscout-1.2.3/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      327 2024-03-31 08:41:29.000000 webscout-1.2.3/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-31 08:41:29.000000 webscout-1.2.3/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:11.536371 webscout-1.2.4/
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:10.642931 webscout-1.2.4/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:10.669937 webscout-1.2.4/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:10.873993 webscout-1.2.4/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3846 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:10.951530 webscout-1.2.4/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     1754 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-04-02 10:54:23.000000 webscout-1.2.4/LICENSE.md
+-rw-rw-rw-   0        0        0    23086 2024-04-02 11:47:11.526373 webscout-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    20920 2024-04-02 11:09:20.000000 webscout-1.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 11:47:11.537369 webscout-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     2828 2024-04-02 11:38:38.000000 webscout-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:11.439178 webscout-1.2.4/webscout/
+-rw-rw-rw-   0        0        0    49618 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/AI.py
+-rw-rw-rw-   0        0        0     2343 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    24124 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     8103 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/HelpingAI.py
+-rw-rw-rw-   0        0        0     3309 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/LLM.py
+-rw-rw-rw-   0        0        0      457 2024-04-02 11:06:30.000000 webscout-1.2.4/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/__main__.py
+-rw-rw-rw-   0        0        0    17059 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/cli.py
+-rw-rw-rw-   0        0        0      276 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/exceptions.py
+-rw-rw-rw-   0        0        0      692 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/models.py
+-rw-rw-rw-   0        0        0     7607 2024-04-02 11:05:29.000000 webscout-1.2.4/webscout/offlineAI.py
+-rw-rw-rw-   0        0        0     2605 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-04-02 11:07:23.000000 webscout-1.2.4/webscout/version.py
+-rw-rw-rw-   0        0        0     3085 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    40670 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:47:11.521368 webscout-1.2.4/webscout.egg-info/
+-rw-rw-rw-   0        0        0    23086 2024-04-02 11:47:09.000000 webscout-1.2.4/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      963 2024-04-02 11:47:10.000000 webscout-1.2.4/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 11:47:09.000000 webscout-1.2.4/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-04-02 11:47:09.000000 webscout-1.2.4/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      342 2024-04-02 11:47:09.000000 webscout-1.2.4/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-02 11:47:09.000000 webscout-1.2.4/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.2.3/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.2.4/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.2.4/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/DeepWEBS/networks/filepath_converter.py` & `webscout-1.2.4/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/DeepWEBS/networks/google_searcher.py` & `webscout-1.2.4/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/DeepWEBS/networks/network_configs.py` & `webscout-1.2.4/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.2.4/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/DeepWEBS/utilsdw/enver.py` & `webscout-1.2.4/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/DeepWEBS/utilsdw/logger.py` & `webscout-1.2.4/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/LICENSE.md` & `webscout-1.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/PKG-INFO` & `webscout-1.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.2.3
+Version: 1.2.4
 Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -41,14 +41,16 @@
 Requires-Dist: markdownify
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: sse_starlette
 Requires-Dist: termcolor
 Requires-Dist: tiktoken
 Requires-Dist: tldextract
+Requires-Dist: gpt4all
+Requires-Dist: orjson
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 
 #  webscout
 <p align="center">
 
@@ -88,14 +90,15 @@
     - [3. `You.com` - search with you.com](#3-youcom---search-with-youcom)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
+    - [9. `GPT4ALL` - chat offline with Language models using gpt4all from webscout](#9-gpt4all---chat-offline-with-language-models-using-gpt4all-from-webscout)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
 
 ## Install
 ```python
 pip install -U webscout
 ```
@@ -601,14 +604,45 @@
 
 opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30)
 # This example sends a simple greeting and prints the response
 prompt = "tell me about india"
 response_str = opengpt.chat(prompt)
 print(response_str)
 ```
+### 9. `GPT4ALL` - chat offline with Language models using gpt4all from webscout
+```python
+from webscout import GPT4ALL
+
+# Initialize the GPT4ALL class with your model path and other optional parameters
+gpt4all_instance = GPT4ALL(
+    model="path/to/your/model/file", # Replace with the actual path to your model file
+    is_conversation=True,
+    max_tokens=800,
+    temperature=0.7,
+    presence_penalty=0,
+    frequency_penalty=1.18,
+    top_p=0.4,
+    intro="Hello, how can I assist you today?",
+    filepath="path/to/conversation/history/file", # Optional, for conversation history
+    update_file=True,
+    history_offset=10250,
+    act=None # Optional, for using an awesome prompt as intro
+)
+
+# Generate a response from the AI model
+response = gpt4all_instance.chat(
+    prompt="What is the weather like today?",
+    stream=False, # Set to True if you want to stream the response
+    optimizer=None, # Optional, specify an optimizer if needed
+    conversationally=False # Set to True for conversationally generated responses
+)
+
+# Print the generated response
+print(response)
+```
 
 ## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.2.3 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.2.4 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
 Author: OEvortex Author-email: helpingai5@gmail.com License: HelpingAI
 Simplified Universal License Project-URL: Documentation, https://github.com/OE-
 LUCIFER/Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/
 Webscout Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex Classifier: Development
@@ -20,16 +20,17 @@
 curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
 asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
 Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
 Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
 Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
-Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist:
-pytest>=7.4.2; extra == "dev" # webscout
+Requires-Dist: gpt4all Requires-Dist: orjson Provides-Extra: dev Requires-Dist:
+ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev" #
+webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
 you.com, etc Also containes AI models Also containes AI models that you can use
  ## Table of Contents - [webscout](#webscout) - [Table of Contents](#table-of-
 contents) - [Install](#install) - [CLI version](#cli-version) - [CLI version of
 webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
 [Regions](#regions) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
@@ -55,15 +56,17 @@
   [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
 `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
   [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
  webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
   using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
   searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
  perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-   opengpt---chat-with-opengpt) - [usage of special .LLM file from webscout
+   opengpt---chat-with-opengpt) - [9. `GPT4ALL` - chat offline with Language
+ models using gpt4all from webscout](#9-gpt4all---chat-offline-with-language-
+models-using-gpt4all-from-webscout) - [usage of special .LLM file from webscout
 (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm) - [`LLM`]
     (#llm) ## Install ```python pip install -U webscout ``` ## CLI version
 ```python3 python -m webscout --help ``` | Command | Description | |-----------
 --------------------------------|----------------------------------------------
 ---------------------------------------------------------| | python -m webscout
 answers -k Text | CLI function to perform an answers search using Webscout. | |
  python -m webscout images -k Text | CLI function to perform an images search
@@ -239,14 +242,27 @@
   7. `PERPLEXITY` - Search With PERPLEXITY ```python from webscout.AI import
 PERPLEXITY # Create an instance of the PERPLEXITY class perplexity = PERPLEXITY
    () # Example usage: prompt = "Explain the concept of recursion in simple
 terms." response = perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT`
 - chat With OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
   (is_conversation=True, max_tokens=8000, timeout=30) # This example sends a
     simple greeting and prints the response prompt = "tell me about india"
-response_str = opengpt.chat(prompt) print(response_str) ``` ## usage of special
- .LLM file from webscout (webscout.LLM) ### `LLM` ```python from webscout.LLM
-   import LLM def chat(model_name, system_message="You are Jarvis"):# system
-     prompt AI = LLM(model_name, system_message) AI.chat() if __name__ ==
-  "__main__": model_name = "mistralai/Mistral-7B-Instruct-v0.1" # name of the
-model you wish to use It supports ALL text generation models on deepinfra.com.
-                             chat(model_name) ```
+response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `GPT4ALL` -
+ chat offline with Language models using gpt4all from webscout ```python from
+webscout import GPT4ALL # Initialize the GPT4ALL class with your model path and
+  other optional parameters gpt4all_instance = GPT4ALL( model="path/to/your/
+        model/file", # Replace with the actual path to your model file
+  is_conversation=True, max_tokens=800, temperature=0.7, presence_penalty=0,
+frequency_penalty=1.18, top_p=0.4, intro="Hello, how can I assist you today?",
+  filepath="path/to/conversation/history/file", # Optional, for conversation
+history update_file=True, history_offset=10250, act=None # Optional, for using
+an awesome prompt as intro ) # Generate a response from the AI model response =
+gpt4all_instance.chat( prompt="What is the weather like today?", stream=False,
+ # Set to True if you want to stream the response optimizer=None, # Optional,
+    specify an optimizer if needed conversationally=False # Set to True for
+  conversationally generated responses ) # Print the generated response print
+ (response) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
+       `LLM` ```python from webscout.LLM import LLM def chat(model_name,
+     system_message="You are Jarvis"):# system prompt AI = LLM(model_name,
+ system_message) AI.chat() if __name__ == "__main__": model_name = "mistralai/
+ Mistral-7B-Instruct-v0.1" # name of the model you wish to use It supports ALL
+         text generation models on deepinfra.com. chat(model_name) ```
```

### Comparing `webscout-1.2.3/README.md` & `webscout-1.2.4/webscout.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,60 @@
+Metadata-Version: 2.1
+Name: webscout
+Version: 1.2.4
+Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
+Author: OEvortex
+Author-email: helpingai5@gmail.com
+License: HelpingAI Simplified Universal License
+Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
+Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
+Project-URL: YouTube, https://youtube.com/@OEvortex
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: docstring_inheritance>=2.1.2
+Requires-Dist: click>=8.1.7
+Requires-Dist: curl_cffi>=0.6.0b7
+Requires-Dist: lxml>=5.1.0
+Requires-Dist: nest-asyncio>=1.6.0
+Requires-Dist: selenium>=4.1.3
+Requires-Dist: tqdm>=4.64.0
+Requires-Dist: webdriver-manager>=3.5.4
+Requires-Dist: halo>=0.0.31
+Requires-Dist: g4f>=0.2.2.3
+Requires-Dist: rich
+Requires-Dist: python-dotenv
+Requires-Dist: Helpingai-T2
+Requires-Dist: beautifulsoup4
+Requires-Dist: markdownify
+Requires-Dist: pydantic
+Requires-Dist: requests
+Requires-Dist: sse_starlette
+Requires-Dist: termcolor
+Requires-Dist: tiktoken
+Requires-Dist: tldextract
+Requires-Dist: gpt4all
+Requires-Dist: orjson
+Provides-Extra: dev
+Requires-Dist: ruff>=0.1.6; extra == "dev"
+Requires-Dist: pytest>=7.4.2; extra == "dev"
+
 #  webscout
 <p align="center">
 
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
 Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
@@ -37,14 +90,15 @@
     - [3. `You.com` - search with you.com](#3-youcom---search-with-youcom)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
+    - [9. `GPT4ALL` - chat offline with Language models using gpt4all from webscout](#9-gpt4all---chat-offline-with-language-models-using-gpt4all-from-webscout)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
 
 ## Install
 ```python
 pip install -U webscout
 ```
@@ -550,14 +604,45 @@
 
 opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30)
 # This example sends a simple greeting and prints the response
 prompt = "tell me about india"
 response_str = opengpt.chat(prompt)
 print(response_str)
 ```
+### 9. `GPT4ALL` - chat offline with Language models using gpt4all from webscout
+```python
+from webscout import GPT4ALL
+
+# Initialize the GPT4ALL class with your model path and other optional parameters
+gpt4all_instance = GPT4ALL(
+    model="path/to/your/model/file", # Replace with the actual path to your model file
+    is_conversation=True,
+    max_tokens=800,
+    temperature=0.7,
+    presence_penalty=0,
+    frequency_penalty=1.18,
+    top_p=0.4,
+    intro="Hello, how can I assist you today?",
+    filepath="path/to/conversation/history/file", # Optional, for conversation history
+    update_file=True,
+    history_offset=10250,
+    act=None # Optional, for using an awesome prompt as intro
+)
+
+# Generate a response from the AI model
+response = gpt4all_instance.chat(
+    prompt="What is the weather like today?",
+    stream=False, # Set to True if you want to stream the response
+    optimizer=None, # Optional, specify an optimizer if needed
+    conversationally=False # Set to True for conversationally generated responses
+)
+
+# Print the generated response
+print(response)
+```
 
 ## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
```

#### html2text {}

```diff
@@ -1,8 +1,36 @@
-# webscout
+Metadata-Version: 2.1 Name: webscout Version: 1.2.4 Summary: Search for words,
+documents, images, videos, news, maps and text translation using the Google,
+DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
+Author: OEvortex Author-email: helpingai5@gmail.com License: HelpingAI
+Simplified Universal License Project-URL: Documentation, https://github.com/OE-
+LUCIFER/Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/
+Webscout Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
+Project-URL: YouTube, https://youtube.com/@OEvortex Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
+docstring_inheritance>=2.1.2 Requires-Dist: click>=8.1.7 Requires-Dist:
+curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
+asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
+Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
+Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
+Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
+Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
+Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
+Requires-Dist: gpt4all Requires-Dist: orjson Provides-Extra: dev Requires-Dist:
+ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev" #
+webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
 you.com, etc Also containes AI models Also containes AI models that you can use
  ## Table of Contents - [webscout](#webscout) - [Table of Contents](#table-of-
 contents) - [Install](#install) - [CLI version](#cli-version) - [CLI version of
 webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
 [Regions](#regions) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
@@ -28,15 +56,17 @@
   [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
 `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
   [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
  webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
   using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
   searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
  perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-   opengpt---chat-with-opengpt) - [usage of special .LLM file from webscout
+   opengpt---chat-with-opengpt) - [9. `GPT4ALL` - chat offline with Language
+ models using gpt4all from webscout](#9-gpt4all---chat-offline-with-language-
+models-using-gpt4all-from-webscout) - [usage of special .LLM file from webscout
 (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm) - [`LLM`]
     (#llm) ## Install ```python pip install -U webscout ``` ## CLI version
 ```python3 python -m webscout --help ``` | Command | Description | |-----------
 --------------------------------|----------------------------------------------
 ---------------------------------------------------------| | python -m webscout
 answers -k Text | CLI function to perform an answers search using Webscout. | |
  python -m webscout images -k Text | CLI function to perform an images search
@@ -212,14 +242,27 @@
   7. `PERPLEXITY` - Search With PERPLEXITY ```python from webscout.AI import
 PERPLEXITY # Create an instance of the PERPLEXITY class perplexity = PERPLEXITY
    () # Example usage: prompt = "Explain the concept of recursion in simple
 terms." response = perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT`
 - chat With OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
   (is_conversation=True, max_tokens=8000, timeout=30) # This example sends a
     simple greeting and prints the response prompt = "tell me about india"
-response_str = opengpt.chat(prompt) print(response_str) ``` ## usage of special
- .LLM file from webscout (webscout.LLM) ### `LLM` ```python from webscout.LLM
-   import LLM def chat(model_name, system_message="You are Jarvis"):# system
-     prompt AI = LLM(model_name, system_message) AI.chat() if __name__ ==
-  "__main__": model_name = "mistralai/Mistral-7B-Instruct-v0.1" # name of the
-model you wish to use It supports ALL text generation models on deepinfra.com.
-                             chat(model_name) ```
+response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `GPT4ALL` -
+ chat offline with Language models using gpt4all from webscout ```python from
+webscout import GPT4ALL # Initialize the GPT4ALL class with your model path and
+  other optional parameters gpt4all_instance = GPT4ALL( model="path/to/your/
+        model/file", # Replace with the actual path to your model file
+  is_conversation=True, max_tokens=800, temperature=0.7, presence_penalty=0,
+frequency_penalty=1.18, top_p=0.4, intro="Hello, how can I assist you today?",
+  filepath="path/to/conversation/history/file", # Optional, for conversation
+history update_file=True, history_offset=10250, act=None # Optional, for using
+an awesome prompt as intro ) # Generate a response from the AI model response =
+gpt4all_instance.chat( prompt="What is the weather like today?", stream=False,
+ # Set to True if you want to stream the response optimizer=None, # Optional,
+    specify an optimizer if needed conversationally=False # Set to True for
+  conversationally generated responses ) # Print the generated response print
+ (response) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
+       `LLM` ```python from webscout.LLM import LLM def chat(model_name,
+     system_message="You are Jarvis"):# system prompt AI = LLM(model_name,
+ system_message) AI.chat() if __name__ == "__main__": model_name = "mistralai/
+ Mistral-7B-Instruct-v0.1" # name of the model you wish to use It supports ALL
+         text generation models on deepinfra.com. chat(model_name) ```
```

### Comparing `webscout-1.2.3/setup.py` & `webscout-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     exec(version_file.read())
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.2.3", # Use the version variable from the version.py file
+    version="1.2.4", # Use the version variable from the version.py file
     description="Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
@@ -49,14 +49,16 @@
         "markdownify",
         "pydantic",
         "requests",
         "sse_starlette",
         "termcolor",
         "tiktoken",
         "tldextract",
+        "gpt4all",
+        "orjson",
     ],
     entry_points={
         "console_scripts": [
             "WEBS = webscout.cli:cli",
             "webscout-ai-phindsearch = webscout.AI:phindsearch",
             "webscout-ai-yepchat = webscout.AI:yepchat",
             "webscout-ai = webscout.AI:cli",
```

### Comparing `webscout-1.2.3/webscout/AI.py` & `webscout-1.2.4/webscout/AI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/webscout/AIbase.py` & `webscout-1.2.4/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/webscout/AIutel.py` & `webscout-1.2.4/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/webscout/DWEBS.py` & `webscout-1.2.4/webscout/DWEBS.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,446 +1,459 @@
-00000000: 0a66 726f 6d20 7079 6461 6e74 6963 2069  .from pydantic i
-00000010: 6d70 6f72 7420 4261 7365 4d6f 6465 6c2c  mport BaseModel,
-00000020: 2046 6965 6c64 0a66 726f 6d20 7479 7069   Field.from typi
-00000030: 6e67 2069 6d70 6f72 7420 556e 696f 6e0a  ng import Union.
-00000040: 0a66 726f 6d20 4465 6570 5745 4253 2e75  .from DeepWEBS.u
-00000050: 7469 6c73 6477 2e6c 6f67 6765 7220 696d  tilsdw.logger im
-00000060: 706f 7274 206c 6f67 6765 720a 6672 6f6d  port logger.from
-00000070: 2044 6565 7057 4542 532e 6e65 7477 6f72   DeepWEBS.networ
-00000080: 6b73 2e67 6f6f 676c 655f 7365 6172 6368  ks.google_search
-00000090: 6572 2069 6d70 6f72 7420 476f 6f67 6c65  er import Google
-000000a0: 5365 6172 6368 6572 0a66 726f 6d20 4465  Searcher.from De
-000000b0: 6570 5745 4253 2e6e 6574 776f 726b 732e  epWEBS.networks.
-000000c0: 7765 6270 6167 655f 6665 7463 6865 7220  webpage_fetcher 
-000000d0: 696d 706f 7274 2042 6174 6368 5765 6270  import BatchWebp
-000000e0: 6167 6546 6574 6368 6572 0a66 726f 6d20  ageFetcher.from 
-000000f0: 4465 6570 5745 4253 2e64 6f63 756d 656e  DeepWEBS.documen
-00000100: 7473 2e71 7565 7279 5f72 6573 756c 7473  ts.query_results
-00000110: 5f65 7874 7261 6374 6f72 2069 6d70 6f72  _extractor impor
-00000120: 7420 5175 6572 7952 6573 756c 7473 4578  t QueryResultsEx
-00000130: 7472 6163 746f 720a 6672 6f6d 2044 6565  tractor.from Dee
-00000140: 7057 4542 532e 646f 6375 6d65 6e74 732e  pWEBS.documents.
-00000150: 7765 6270 6167 655f 636f 6e74 656e 745f  webpage_content_
-00000160: 6578 7472 6163 746f 7220 696d 706f 7274  extractor import
-00000170: 2042 6174 6368 5765 6270 6167 6543 6f6e   BatchWebpageCon
-00000180: 7465 6e74 4578 7472 6163 746f 720a 6672  tentExtractor.fr
-00000190: 6f6d 2044 6565 7057 4542 532e 7574 696c  om DeepWEBS.util
-000001a0: 7364 772e 6c6f 6767 6572 2069 6d70 6f72  sdw.logger impor
-000001b0: 7420 6c6f 6767 6572 0a69 6d70 6f72 7420  t logger.import 
-000001c0: 6172 6770 6172 7365 0a0a 636c 6173 7320  argparse..class 
-000001d0: 4465 6570 5745 4253 3a0a 2020 2020 6465  DeepWEBS:.    de
-000001e0: 6620 5f5f 696e 6974 5f5f 2873 656c 6629  f __init__(self)
-000001f0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00000200: 2020 2020 636c 6173 7320 4465 6570 5365      class DeepSe
-00000210: 6172 6368 2842 6173 654d 6f64 656c 293a  arch(BaseModel):
-00000220: 0a20 2020 2020 2020 2071 7565 7269 6573  .        queries
-00000230: 3a20 6c69 7374 203d 2046 6965 6c64 280a  : list = Field(.
-00000240: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-00000250: 756c 743d 5b22 225d 2c0a 2020 2020 2020  ult=[""],.      
-00000260: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00000270: 6e3d 2228 6c69 7374 5b73 7472 5d29 2051  n="(list[str]) Q
-00000280: 7565 7269 6573 2074 6f20 7365 6172 6368  ueries to search
-00000290: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
-000002a0: 2020 2020 2072 6573 756c 745f 6e75 6d3a       result_num:
-000002b0: 2069 6e74 203d 2046 6965 6c64 280a 2020   int = Field(.  
-000002c0: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
-000002d0: 743d 3130 2c0a 2020 2020 2020 2020 2020  t=10,.          
-000002e0: 2020 6465 7363 7269 7074 696f 6e3d 2228    description="(
-000002f0: 696e 7429 204e 756d 6265 7220 6f66 2073  int) Number of s
-00000300: 6561 7263 6820 7265 7375 6c74 7322 2c0a  earch results",.
-00000310: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00000320: 2020 7361 6665 3a20 626f 6f6c 203d 2046    safe: bool = F
-00000330: 6965 6c64 280a 2020 2020 2020 2020 2020  ield(.          
-00000340: 2020 6465 6661 756c 743d 4661 6c73 652c    default=False,
-00000350: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00000360: 6372 6970 7469 6f6e 3d22 2862 6f6f 6c29  cription="(bool)
-00000370: 2045 6e61 626c 6520 5361 6665 5365 6172   Enable SafeSear
-00000380: 6368 222c 0a20 2020 2020 2020 2029 0a20  ch",.        ). 
-00000390: 2020 2020 2020 2074 7970 6573 3a20 6c69         types: li
-000003a0: 7374 203d 2046 6965 6c64 280a 2020 2020  st = Field(.    
-000003b0: 2020 2020 2020 2020 6465 6661 756c 743d          default=
-000003c0: 5b22 7765 6222 5d2c 0a20 2020 2020 2020  ["web"],.       
-000003d0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-000003e0: 3d22 286c 6973 745b 7374 725d 2920 5479  ="(list[str]) Ty
-000003f0: 7065 7320 6f66 2073 6561 7263 6820 7265  pes of search re
-00000400: 7375 6c74 733a 2060 7765 6260 2c20 6069  sults: `web`, `i
-00000410: 6d61 6765 602c 2060 7669 6465 6f73 602c  mage`, `videos`,
-00000420: 2060 6e65 7773 6022 2c0a 2020 2020 2020   `news`",.      
-00000430: 2020 290a 2020 2020 2020 2020 6578 7472    ).        extr
-00000440: 6163 745f 7765 6270 6167 653a 2062 6f6f  act_webpage: boo
-00000450: 6c20 3d20 4669 656c 6428 0a20 2020 2020  l = Field(.     
-00000460: 2020 2020 2020 2064 6566 6175 6c74 3d46         default=F
-00000470: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00000480: 2020 6465 7363 7269 7074 696f 6e3d 2228    description="(
-00000490: 626f 6f6c 2920 456e 6162 6c65 2065 7874  bool) Enable ext
-000004a0: 7261 6374 696e 6720 6d61 696e 2074 6578  racting main tex
-000004b0: 7420 636f 6e74 656e 7473 2066 726f 6d20  t contents from 
-000004c0: 7765 6270 6167 652c 2077 696c 6c20 6164  webpage, will ad
-000004d0: 6420 6074 6578 7460 2066 696c 6564 2069  d `text` filed i
-000004e0: 6e20 6561 6368 2060 7175 6572 795f 7265  n each `query_re
-000004f0: 7375 6c74 6020 6469 6374 222c 0a20 2020  sult` dict",.   
-00000500: 2020 2020 2029 0a20 2020 2020 2020 206f       ).        o
-00000510: 7665 7277 7269 7465 5f71 7565 7279 5f68  verwrite_query_h
-00000520: 746d 6c3a 2062 6f6f 6c20 3d20 4669 656c  tml: bool = Fiel
-00000530: 6428 0a20 2020 2020 2020 2020 2020 2064  d(.            d
-00000540: 6566 6175 6c74 3d46 616c 7365 2c0a 2020  efault=False,.  
-00000550: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00000560: 7074 696f 6e3d 2228 626f 6f6c 2920 4f76  ption="(bool) Ov
-00000570: 6572 7772 6974 6520 4854 4d4c 2066 696c  erwrite HTML fil
-00000580: 6520 6f66 2071 7565 7279 2072 6573 756c  e of query resul
-00000590: 7473 222c 0a20 2020 2020 2020 2029 0a20  ts",.        ). 
-000005a0: 2020 2020 2020 206f 7665 7277 7269 7465         overwrite
-000005b0: 5f77 6562 7061 6765 5f68 746d 6c3a 2062  _webpage_html: b
-000005c0: 6f6f 6c20 3d20 4669 656c 6428 0a20 2020  ool = Field(.   
-000005d0: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-000005e0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-000005f0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-00000600: 2228 626f 6f6c 2920 4f76 6572 7772 6974  "(bool) Overwrit
-00000610: 6520 4854 4d4c 2066 696c 6573 206f 6620  e HTML files of 
-00000620: 7765 6270 6167 6573 2066 726f 6d20 7175  webpages from qu
-00000630: 6572 7920 7265 7375 6c74 7322 2c0a 2020  ery results",.  
-00000640: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-00000650: 2071 7565 7269 6573 5f74 6f5f 7365 6172   queries_to_sear
-00000660: 6368 5f72 6573 756c 7473 2873 656c 662c  ch_results(self,
-00000670: 2069 7465 6d3a 2044 6565 7053 6561 7263   item: DeepSearc
-00000680: 6829 3a0a 2020 2020 2020 2020 676f 6f67  h):.        goog
-00000690: 6c65 5f73 6561 7263 6865 7220 3d20 476f  le_searcher = Go
-000006a0: 6f67 6c65 5365 6172 6368 6572 2829 0a20  ogleSearcher(). 
-000006b0: 2020 2020 2020 2071 7565 7269 6573 5f73         queries_s
-000006c0: 6561 7263 685f 7265 7375 6c74 7320 3d20  earch_results = 
-000006d0: 5b5d 0a20 2020 2020 2020 2066 6f72 2071  [].        for q
-000006e0: 7565 7279 2069 6e20 6974 656d 2e71 7565  uery in item.que
-000006f0: 7269 6573 3a0a 2020 2020 2020 2020 2020  ries:.          
-00000700: 2020 7175 6572 795f 7265 7375 6c74 735f    query_results_
-00000710: 6578 7472 6163 746f 7220 3d20 5175 6572  extractor = Quer
-00000720: 7952 6573 756c 7473 4578 7472 6163 746f  yResultsExtracto
-00000730: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
-00000740: 6966 206e 6f74 2071 7565 7279 2e73 7472  if not query.str
-00000750: 6970 2829 3a0a 2020 2020 2020 2020 2020  ip():.          
-00000760: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-00000770: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000790: 7175 6572 795f 6874 6d6c 5f70 6174 6820  query_html_path 
-000007a0: 3d20 676f 6f67 6c65 5f73 6561 7263 6865  = google_searche
-000007b0: 722e 7365 6172 6368 280a 2020 2020 2020  r.search(.      
-000007c0: 2020 2020 2020 2020 2020 2020 2020 7175                qu
-000007d0: 6572 793d 7175 6572 792c 0a20 2020 2020  ery=query,.     
-000007e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000007f0: 6573 756c 745f 6e75 6d3d 6974 656d 2e72  esult_num=item.r
-00000800: 6573 756c 745f 6e75 6d2c 0a20 2020 2020  esult_num,.     
-00000810: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00000820: 6166 653d 6974 656d 2e73 6166 652c 0a20  afe=item.safe,. 
-00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000840: 2020 206f 7665 7277 7269 7465 3d69 7465     overwrite=ite
-00000850: 6d2e 6f76 6572 7772 6974 655f 7175 6572  m.overwrite_quer
-00000860: 795f 6874 6d6c 2c0a 2020 2020 2020 2020  y_html,.        
-00000870: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00000880: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00000890: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
-000008a0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-000008b0: 6765 722e 6572 726f 7228 6622 4661 696c  ger.error(f"Fail
-000008c0: 6564 2074 6f20 7365 6172 6368 2066 6f72  ed to search for
-000008d0: 2071 7565 7279 2027 7b71 7565 7279 7d27   query '{query}'
-000008e0: 3a20 7b65 7d22 290a 2020 2020 2020 2020  : {e}").        
-000008f0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00000900: 0a0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
-00000910: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-00000920: 2020 2071 7565 7279 5f73 6561 7263 685f     query_search_
-00000930: 7265 7375 6c74 7320 3d20 7175 6572 795f  results = query_
-00000940: 7265 7375 6c74 735f 6578 7472 6163 746f  results_extracto
-00000950: 722e 6578 7472 6163 7428 7175 6572 795f  r.extract(query_
-00000960: 6874 6d6c 5f70 6174 6829 0a20 2020 2020  html_path).     
-00000970: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-00000980: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
-00000990: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000009a0: 6767 6572 2e65 7272 6f72 2866 2246 6169  gger.error(f"Fai
-000009b0: 6c65 6420 746f 2065 7874 7261 6374 2073  led to extract s
-000009c0: 6561 7263 6820 7265 7375 6c74 7320 666f  earch results fo
-000009d0: 7220 7175 6572 7920 277b 7175 6572 797d  r query '{query}
-000009e0: 273a 207b 657d 2229 0a20 2020 2020 2020  ': {e}").       
-000009f0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00000a00: 650a 0a20 2020 2020 2020 2020 2020 2071  e..            q
-00000a10: 7565 7269 6573 5f73 6561 7263 685f 7265  ueries_search_re
-00000a20: 7375 6c74 732e 6170 7065 6e64 2871 7565  sults.append(que
-00000a30: 7279 5f73 6561 7263 685f 7265 7375 6c74  ry_search_result
-00000a40: 7329 0a20 2020 2020 2020 206c 6f67 6765  s).        logge
-00000a50: 722e 6e6f 7465 2871 7565 7269 6573 5f73  r.note(queries_s
-00000a60: 6561 7263 685f 7265 7375 6c74 7329 0a0a  earch_results)..
-00000a70: 2020 2020 2020 2020 6966 2069 7465 6d2e          if item.
-00000a80: 6578 7472 6163 745f 7765 6270 6167 653a  extract_webpage:
-00000a90: 0a20 2020 2020 2020 2020 2020 2071 7565  .            que
-00000aa0: 7269 6573 5f73 6561 7263 685f 7265 7375  ries_search_resu
-00000ab0: 6c74 7320 3d20 7365 6c66 2e65 7874 7261  lts = self.extra
-00000ac0: 6374 5f77 6562 7061 6765 7328 0a20 2020  ct_webpages(.   
-00000ad0: 2020 2020 2020 2020 2020 2020 2071 7565               que
-00000ae0: 7269 6573 5f73 6561 7263 685f 7265 7375  ries_search_resu
-00000af0: 6c74 732c 0a20 2020 2020 2020 2020 2020  lts,.           
-00000b00: 2020 2020 206f 7665 7277 7269 7465 5f77       overwrite_w
-00000b10: 6562 7061 6765 5f68 746d 6c3d 6974 656d  ebpage_html=item
-00000b20: 2e6f 7665 7277 7269 7465 5f77 6562 7061  .overwrite_webpa
-00000b30: 6765 5f68 746d 6c2c 0a20 2020 2020 2020  ge_html,.       
-00000b40: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
-00000b50: 6574 7572 6e20 7175 6572 6965 735f 7365  eturn queries_se
-00000b60: 6172 6368 5f72 6573 756c 7473 0a0a 2020  arch_results..  
-00000b70: 2020 6465 6620 6578 7472 6163 745f 7765    def extract_we
-00000b80: 6270 6167 6573 2873 656c 662c 2071 7565  bpages(self, que
-00000b90: 7269 6573 5f73 6561 7263 685f 7265 7375  ries_search_resu
-00000ba0: 6c74 732c 206f 7665 7277 7269 7465 5f77  lts, overwrite_w
-00000bb0: 6562 7061 6765 5f68 746d 6c3d 4661 6c73  ebpage_html=Fals
-00000bc0: 6529 3a0a 2020 2020 2020 2020 666f 7220  e):.        for 
-00000bd0: 7175 6572 795f 6964 782c 2071 7565 7279  query_idx, query
-00000be0: 5f73 6561 7263 685f 7265 7375 6c74 7320  _search_results 
-00000bf0: 696e 2065 6e75 6d65 7261 7465 2871 7565  in enumerate(que
-00000c00: 7269 6573 5f73 6561 7263 685f 7265 7375  ries_search_resu
-00000c10: 6c74 7329 3a0a 2020 2020 2020 2020 2020  lts):.          
-00000c20: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00000c30: 2020 2020 2020 2023 2046 6574 6368 2077         # Fetch w
-00000c40: 6562 7061 6765 7320 7769 7468 2075 726c  ebpages with url
-00000c50: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00000c60: 2020 6261 7463 685f 7765 6270 6167 655f    batch_webpage_
-00000c70: 6665 7463 6865 7220 3d20 4261 7463 6857  fetcher = BatchW
-00000c80: 6562 7061 6765 4665 7463 6865 7228 290a  ebpageFetcher().
-00000c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ca0: 7572 6c73 203d 205b 0a20 2020 2020 2020  urls = [.       
-00000cb0: 2020 2020 2020 2020 2020 2020 2071 7565               que
-00000cc0: 7279 5f72 6573 756c 745b 2275 726c 225d  ry_result["url"]
-00000cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ce0: 2020 2020 2066 6f72 2071 7565 7279 5f72       for query_r
-00000cf0: 6573 756c 7420 696e 2071 7565 7279 5f73  esult in query_s
-00000d00: 6561 7263 685f 7265 7375 6c74 735b 2271  earch_results["q
-00000d10: 7565 7279 5f72 6573 756c 7473 225d 0a20  uery_results"]. 
-00000d20: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00000d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d40: 2075 726c 5f61 6e64 5f68 746d 6c5f 7061   url_and_html_pa
-00000d50: 7468 5f6c 6973 7420 3d20 6261 7463 685f  th_list = batch_
-00000d60: 7765 6270 6167 655f 6665 7463 6865 722e  webpage_fetcher.
-00000d70: 6665 7463 6828 0a20 2020 2020 2020 2020  fetch(.         
-00000d80: 2020 2020 2020 2020 2020 2075 726c 732c             urls,
-00000d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000da0: 2020 2020 206f 7665 7277 7269 7465 3d6f       overwrite=o
-00000db0: 7665 7277 7269 7465 5f77 6562 7061 6765  verwrite_webpage
-00000dc0: 5f68 746d 6c2c 0a20 2020 2020 2020 2020  _html,.         
-00000dd0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00000de0: 745f 7061 7265 6e74 3d71 7565 7279 5f73  t_parent=query_s
-00000df0: 6561 7263 685f 7265 7375 6c74 735b 2271  earch_results["q
-00000e00: 7565 7279 225d 2c0a 2020 2020 2020 2020  uery"],.        
-00000e10: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00000e20: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00000e30: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
-00000e40: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00000e50: 6765 722e 6572 726f 7228 6622 4661 696c  ger.error(f"Fail
-00000e60: 6564 2074 6f20 6665 7463 6820 7765 6270  ed to fetch webp
-00000e70: 6167 6573 2066 6f72 2071 7565 7279 2027  ages for query '
-00000e80: 7b71 7565 7279 5f73 6561 7263 685f 7265  {query_search_re
-00000e90: 7375 6c74 735b 2771 7565 7279 275d 7d27  sults['query']}'
-00000ea0: 3a20 7b65 7d22 290a 2020 2020 2020 2020  : {e}").        
-00000eb0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00000ec0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00000ed0: 4578 7472 6163 7420 7765 6270 6167 6520  Extract webpage 
-00000ee0: 636f 6e74 656e 7473 2066 726f 6d20 6874  contents from ht
-00000ef0: 6d6c 730a 2020 2020 2020 2020 2020 2020  mls.            
-00000f00: 6874 6d6c 5f70 6174 6873 203d 205b 0a20  html_paths = [. 
-00000f10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00000f20: 7472 2875 726c 5f61 6e64 5f68 746d 6c5f  tr(url_and_html_
-00000f30: 7061 7468 5b22 6874 6d6c 5f70 6174 6822  path["html_path"
-00000f40: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00000f50: 2020 2066 6f72 2075 726c 5f61 6e64 5f68     for url_and_h
-00000f60: 746d 6c5f 7061 7468 2069 6e20 7572 6c5f  tml_path in url_
-00000f70: 616e 645f 6874 6d6c 5f70 6174 685f 6c69  and_html_path_li
-00000f80: 7374 0a20 2020 2020 2020 2020 2020 205d  st.            ]
-00000f90: 0a20 2020 2020 2020 2020 2020 2062 6174  .            bat
-00000fa0: 6368 5f77 6562 7061 6765 5f63 6f6e 7465  ch_webpage_conte
-00000fb0: 6e74 5f65 7874 7261 6374 6f72 203d 2042  nt_extractor = B
-00000fc0: 6174 6368 5765 6270 6167 6543 6f6e 7465  atchWebpageConte
-00000fd0: 6e74 4578 7472 6163 746f 7228 290a 2020  ntExtractor().  
-00000fe0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-00001000: 746d 6c5f 7061 7468 5f61 6e64 5f65 7874  tml_path_and_ext
-00001010: 7261 6374 6564 5f63 6f6e 7465 6e74 5f6c  racted_content_l
-00001020: 6973 7420 3d20 280a 2020 2020 2020 2020  ist = (.        
-00001030: 2020 2020 2020 2020 2020 2020 6261 7463              batc
-00001040: 685f 7765 6270 6167 655f 636f 6e74 656e  h_webpage_conten
-00001050: 745f 6578 7472 6163 746f 722e 6578 7472  t_extractor.extr
-00001060: 6163 7428 6874 6d6c 5f70 6174 6873 290a  act(html_paths).
-00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001080: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
-00001090: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-000010a0: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-000010b0: 2020 2020 206c 6f67 6765 722e 6572 726f       logger.erro
-000010c0: 7228 6622 4661 696c 6564 2074 6f20 6578  r(f"Failed to ex
-000010d0: 7472 6163 7420 7765 6270 6167 6520 636f  tract webpage co
-000010e0: 6e74 656e 7473 2066 6f72 2071 7565 7279  ntents for query
-000010f0: 2027 7b71 7565 7279 5f73 6561 7263 685f   '{query_search_
-00001100: 7265 7375 6c74 735b 2771 7565 7279 275d  results['query']
-00001110: 7d27 3a20 7b65 7d22 290a 2020 2020 2020  }': {e}").      
-00001120: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00001130: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
-00001140: 2320 4275 696c 6420 7468 6520 6d61 7020  # Build the map 
-00001150: 6f66 2075 726c 2074 6f20 6578 7472 6163  of url to extrac
-00001160: 7465 645f 636f 6e74 656e 740a 2020 2020  ted_content.    
-00001170: 2020 2020 2020 2020 6874 6d6c 5f70 6174          html_pat
-00001180: 685f 746f 5f75 726c 5f64 6963 7420 3d20  h_to_url_dict = 
-00001190: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000011a0: 2020 7374 7228 7572 6c5f 616e 645f 6874    str(url_and_ht
-000011b0: 6d6c 5f70 6174 685b 2268 746d 6c5f 7061  ml_path["html_pa
-000011c0: 7468 225d 293a 2075 726c 5f61 6e64 5f68  th"]): url_and_h
-000011d0: 746d 6c5f 7061 7468 5b22 7572 6c22 5d0a  tml_path["url"].
-000011e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011f0: 666f 7220 7572 6c5f 616e 645f 6874 6d6c  for url_and_html
-00001200: 5f70 6174 6820 696e 2075 726c 5f61 6e64  _path in url_and
-00001210: 5f68 746d 6c5f 7061 7468 5f6c 6973 740a  _html_path_list.
-00001220: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00001230: 2020 2020 2020 2020 2020 7572 6c5f 746f            url_to
-00001240: 5f65 7874 7261 6374 6564 5f63 6f6e 7465  _extracted_conte
-00001250: 6e74 5f64 6963 7420 3d20 7b0a 2020 2020  nt_dict = {.    
-00001260: 2020 2020 2020 2020 2020 2020 6874 6d6c              html
-00001270: 5f70 6174 685f 746f 5f75 726c 5f64 6963  _path_to_url_dic
-00001280: 745b 0a20 2020 2020 2020 2020 2020 2020  t[.             
-00001290: 2020 2020 2020 2068 746d 6c5f 7061 7468         html_path
-000012a0: 5f61 6e64 5f65 7874 7261 6374 6564 5f63  _and_extracted_c
-000012b0: 6f6e 7465 6e74 5b22 6874 6d6c 5f70 6174  ontent["html_pat
-000012c0: 6822 5d0a 2020 2020 2020 2020 2020 2020  h"].            
-000012d0: 2020 2020 5d3a 2068 746d 6c5f 7061 7468      ]: html_path
-000012e0: 5f61 6e64 5f65 7874 7261 6374 6564 5f63  _and_extracted_c
-000012f0: 6f6e 7465 6e74 5b22 6578 7472 6163 7465  ontent["extracte
-00001300: 645f 636f 6e74 656e 7422 5d0a 2020 2020  d_content"].    
-00001310: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00001320: 6874 6d6c 5f70 6174 685f 616e 645f 6578  html_path_and_ex
-00001330: 7472 6163 7465 645f 636f 6e74 656e 7420  tracted_content 
-00001340: 696e 2068 746d 6c5f 7061 7468 5f61 6e64  in html_path_and
-00001350: 5f65 7874 7261 6374 6564 5f63 6f6e 7465  _extracted_conte
-00001360: 6e74 5f6c 6973 740a 2020 2020 2020 2020  nt_list.        
-00001370: 2020 2020 7d0a 0a20 2020 2020 2020 2020      }..         
-00001380: 2020 2023 2057 7269 7465 2065 7874 7261     # Write extra
-00001390: 6374 6564 2063 6f6e 7465 6e74 7320 2861  cted contents (a
-000013a0: 7320 2774 6578 7427 2066 6965 6c64 2920  s 'text' field) 
-000013b0: 746f 2071 7565 7279 5f73 6561 7263 685f  to query_search_
-000013c0: 7265 7375 6c74 730a 2020 2020 2020 2020  results.        
-000013d0: 2020 2020 666f 7220 7175 6572 795f 7265      for query_re
-000013e0: 7375 6c74 5f69 6478 2c20 7175 6572 795f  sult_idx, query_
-000013f0: 7265 7375 6c74 2069 6e20 656e 756d 6572  result in enumer
-00001400: 6174 6528 0a20 2020 2020 2020 2020 2020  ate(.           
-00001410: 2020 2020 2071 7565 7279 5f73 6561 7263       query_searc
-00001420: 685f 7265 7375 6c74 735b 2271 7565 7279  h_results["query
-00001430: 5f72 6573 756c 7473 225d 0a20 2020 2020  _results"].     
-00001440: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00001450: 2020 2020 2020 2020 2020 7572 6c20 3d20            url = 
-00001460: 7175 6572 795f 7265 7375 6c74 5b22 7572  query_result["ur
-00001470: 6c22 5d0a 2020 2020 2020 2020 2020 2020  l"].            
-00001480: 2020 2020 6578 7472 6163 7465 645f 636f      extracted_co
-00001490: 6e74 656e 7420 3d20 7572 6c5f 746f 5f65  ntent = url_to_e
-000014a0: 7874 7261 6374 6564 5f63 6f6e 7465 6e74  xtracted_content
-000014b0: 5f64 6963 742e 6765 7428 7572 6c2c 2022  _dict.get(url, "
-000014c0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-000014d0: 2020 2071 7565 7269 6573 5f73 6561 7263     queries_searc
-000014e0: 685f 7265 7375 6c74 735b 7175 6572 795f  h_results[query_
-000014f0: 6964 785d 5b22 7175 6572 795f 7265 7375  idx]["query_resu
-00001500: 6c74 7322 5d5b 7175 6572 795f 7265 7375  lts"][query_resu
-00001510: 6c74 5f69 6478 5d5b 0a20 2020 2020 2020  lt_idx][.       
-00001520: 2020 2020 2020 2020 2020 2020 2022 7465               "te
-00001530: 7874 220a 2020 2020 2020 2020 2020 2020  xt".            
-00001540: 2020 2020 5d20 3d20 6578 7472 6163 7465      ] = extracte
-00001550: 645f 636f 6e74 656e 740a 0a20 2020 2020  d_content..     
-00001560: 2020 2072 6574 7572 6e20 7175 6572 6965     return querie
-00001570: 735f 7365 6172 6368 5f72 6573 756c 7473  s_search_results
-00001580: 0a0a 0a63 6c61 7373 2041 7267 5061 7273  ...class ArgPars
-00001590: 6572 2861 7267 7061 7273 652e 4172 6775  er(argparse.Argu
-000015a0: 6d65 6e74 5061 7273 6572 293a 0a20 2020  mentParser):.   
-000015b0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-000015c0: 6c66 2c20 2a61 7267 732c 202a 2a6b 7761  lf, *args, **kwa
-000015d0: 7267 7329 3a0a 2020 2020 2020 2020 7375  rgs):.        su
-000015e0: 7065 7228 4172 6750 6172 7365 722c 2073  per(ArgParser, s
-000015f0: 656c 6629 2e5f 5f69 6e69 745f 5f28 2a61  elf).__init__(*a
-00001600: 7267 732c 202a 2a6b 7761 7267 7329 0a0a  rgs, **kwargs)..
-00001610: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
-00001620: 5f61 7267 756d 656e 7428 0a20 2020 2020  _argument(.     
-00001630: 2020 2020 2020 2022 2d71 222c 0a20 2020         "-q",.   
-00001640: 2020 2020 2020 2020 2022 2d2d 7175 6572           "--quer
-00001650: 6965 7322 2c0a 2020 2020 2020 2020 2020  ies",.          
-00001660: 2020 7479 7065 3d73 7472 2c0a 2020 2020    type=str,.    
-00001670: 2020 2020 2020 2020 6e61 7267 733d 222b          nargs="+
-00001680: 222c 0a20 2020 2020 2020 2020 2020 2072  ",.            r
-00001690: 6571 7569 7265 643d 5472 7565 2c0a 2020  equired=True,.  
-000016a0: 2020 2020 2020 2020 2020 6865 6c70 3d22            help="
-000016b0: 5175 6572 6965 7320 746f 2073 6561 7263  Queries to searc
-000016c0: 6822 2c0a 2020 2020 2020 2020 290a 2020  h",.        ).  
-000016d0: 2020 2020 2020 7365 6c66 2e61 6464 5f61        self.add_a
-000016e0: 7267 756d 656e 7428 0a20 2020 2020 2020  rgument(.       
-000016f0: 2020 2020 2022 2d6e 222c 0a20 2020 2020       "-n",.     
-00001700: 2020 2020 2020 2022 2d2d 7265 7375 6c74         "--result
-00001710: 5f6e 756d 222c 0a20 2020 2020 2020 2020  _num",.         
-00001720: 2020 2074 7970 653d 696e 742c 0a20 2020     type=int,.   
-00001730: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-00001740: 3d31 302c 0a20 2020 2020 2020 2020 2020  =10,.           
-00001750: 2068 656c 703d 224e 756d 6265 7220 6f66   help="Number of
-00001760: 2073 6561 7263 6820 7265 7375 6c74 7322   search results"
-00001770: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00001780: 2020 2020 7365 6c66 2e61 6464 5f61 7267      self.add_arg
-00001790: 756d 656e 7428 0a20 2020 2020 2020 2020  ument(.         
-000017a0: 2020 2022 2d73 222c 0a20 2020 2020 2020     "-s",.       
-000017b0: 2020 2020 2022 2d2d 7361 6665 222c 0a20       "--safe",. 
-000017c0: 2020 2020 2020 2020 2020 2064 6566 6175             defau
-000017d0: 6c74 3d46 616c 7365 2c0a 2020 2020 2020  lt=False,.      
-000017e0: 2020 2020 2020 6163 7469 6f6e 3d22 7374        action="st
-000017f0: 6f72 655f 7472 7565 222c 0a20 2020 2020  ore_true",.     
-00001800: 2020 2020 2020 2068 656c 703d 2245 6e61         help="Ena
-00001810: 626c 6520 5361 6665 5365 6172 6368 222c  ble SafeSearch",
-00001820: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00001830: 2020 2073 656c 662e 6164 645f 6172 6775     self.add_argu
-00001840: 6d65 6e74 280a 2020 2020 2020 2020 2020  ment(.          
-00001850: 2020 222d 7422 2c0a 2020 2020 2020 2020    "-t",.        
-00001860: 2020 2020 222d 2d74 7970 6573 222c 0a20      "--types",. 
-00001870: 2020 2020 2020 2020 2020 2074 7970 653d             type=
-00001880: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
-00001890: 206e 6172 6773 3d22 2b22 2c0a 2020 2020   nargs="+",.    
-000018a0: 2020 2020 2020 2020 6465 6661 756c 743d          default=
-000018b0: 5b22 7765 6222 5d2c 0a20 2020 2020 2020  ["web"],.       
-000018c0: 2020 2020 2063 686f 6963 6573 3d5b 2277       choices=["w
-000018d0: 6562 222c 2022 696d 6167 6522 2c20 2276  eb", "image", "v
-000018e0: 6964 656f 7322 2c20 226e 6577 7322 5d2c  ideos", "news"],
-000018f0: 0a20 2020 2020 2020 2020 2020 2068 656c  .            hel
-00001900: 703d 2254 7970 6573 206f 6620 7365 6172  p="Types of sear
-00001910: 6368 2072 6573 756c 7473 222c 0a20 2020  ch results",.   
-00001920: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-00001930: 656c 662e 6164 645f 6172 6775 6d65 6e74  elf.add_argument
-00001940: 280a 2020 2020 2020 2020 2020 2020 222d  (.            "-
-00001950: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00001960: 222d 2d65 7874 7261 6374 5f77 6562 7061  "--extract_webpa
-00001970: 6765 222c 0a20 2020 2020 2020 2020 2020  ge",.           
-00001980: 2064 6566 6175 6c74 3d46 616c 7365 2c0a   default=False,.
-00001990: 2020 2020 2020 2020 2020 2020 6163 7469              acti
-000019a0: 6f6e 3d22 7374 6f72 655f 7472 7565 222c  on="store_true",
-000019b0: 0a20 2020 2020 2020 2020 2020 2068 656c  .            hel
-000019c0: 703d 2245 6e61 626c 6520 6578 7472 6163  p="Enable extrac
-000019d0: 7469 6e67 206d 6169 6e20 7465 7874 2063  ting main text c
-000019e0: 6f6e 7465 6e74 7320 6672 6f6d 2077 6562  ontents from web
-000019f0: 7061 6765 222c 0a20 2020 2020 2020 2029  page",.        )
-00001a00: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-00001a10: 645f 6172 6775 6d65 6e74 280a 2020 2020  d_argument(.    
-00001a20: 2020 2020 2020 2020 222d 6f22 2c0a 2020          "-o",.  
-00001a30: 2020 2020 2020 2020 2020 222d 2d6f 7665            "--ove
-00001a40: 7277 7269 7465 5f71 7565 7279 5f68 746d  rwrite_query_htm
-00001a50: 6c22 2c0a 2020 2020 2020 2020 2020 2020  l",.            
-00001a60: 6465 6661 756c 743d 4661 6c73 652c 0a20  default=False,. 
-00001a70: 2020 2020 2020 2020 2020 2061 6374 696f             actio
-00001a80: 6e3d 2273 746f 7265 5f74 7275 6522 2c0a  n="store_true",.
-00001a90: 2020 2020 2020 2020 2020 2020 6865 6c70              help
-00001aa0: 3d22 4f76 6572 7772 6974 6520 4854 4d4c  ="Overwrite HTML
-00001ab0: 2066 696c 6520 6f66 2071 7565 7279 2072   file of query r
-00001ac0: 6573 756c 7473 222c 0a20 2020 2020 2020  esults",.       
-00001ad0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-00001ae0: 6164 645f 6172 6775 6d65 6e74 280a 2020  add_argument(.  
-00001af0: 2020 2020 2020 2020 2020 222d 7722 2c0a            "-w",.
-00001b00: 2020 2020 2020 2020 2020 2020 222d 2d6f              "--o
-00001b10: 7665 7277 7269 7465 5f77 6562 7061 6765  verwrite_webpage
-00001b20: 5f68 746d 6c22 2c0a 2020 2020 2020 2020  _html",.        
-00001b30: 2020 2020 6465 6661 756c 743d 4661 6c73      default=Fals
-00001b40: 652c 0a20 2020 2020 2020 2020 2020 2061  e,.            a
-00001b50: 6374 696f 6e3d 2273 746f 7265 5f74 7275  ction="store_tru
-00001b60: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00001b70: 6865 6c70 3d22 4f76 6572 7772 6974 6520  help="Overwrite 
-00001b80: 4854 4d4c 2066 696c 6573 206f 6620 7765  HTML files of we
-00001b90: 6270 6167 6573 2066 726f 6d20 7175 6572  bpages from quer
-00001ba0: 7920 7265 7375 6c74 7322 2c0a 2020 2020  y results",.    
-00001bb0: 2020 2020 290a 0a20 2020 2020 2020 2073      )..        s
-00001bc0: 656c 662e 6172 6773 203d 2073 656c 662e  elf.args = self.
-00001bd0: 7061 7273 655f 6172 6773 2829 0a0a 0a    parse_args()...
+00000000: 0d0a 6672 6f6d 2070 7964 616e 7469 6320  ..from pydantic 
+00000010: 696d 706f 7274 2042 6173 654d 6f64 656c  import BaseModel
+00000020: 2c20 4669 656c 640d 0a66 726f 6d20 7479  , Field..from ty
+00000030: 7069 6e67 2069 6d70 6f72 7420 556e 696f  ping import Unio
+00000040: 6e0d 0a0d 0a66 726f 6d20 4465 6570 5745  n....from DeepWE
+00000050: 4253 2e75 7469 6c73 6477 2e6c 6f67 6765  BS.utilsdw.logge
+00000060: 7220 696d 706f 7274 206c 6f67 6765 720d  r import logger.
+00000070: 0a66 726f 6d20 4465 6570 5745 4253 2e6e  .from DeepWEBS.n
+00000080: 6574 776f 726b 732e 676f 6f67 6c65 5f73  etworks.google_s
+00000090: 6561 7263 6865 7220 696d 706f 7274 2047  earcher import G
+000000a0: 6f6f 676c 6553 6561 7263 6865 720d 0a66  oogleSearcher..f
+000000b0: 726f 6d20 4465 6570 5745 4253 2e6e 6574  rom DeepWEBS.net
+000000c0: 776f 726b 732e 7765 6270 6167 655f 6665  works.webpage_fe
+000000d0: 7463 6865 7220 696d 706f 7274 2042 6174  tcher import Bat
+000000e0: 6368 5765 6270 6167 6546 6574 6368 6572  chWebpageFetcher
+000000f0: 0d0a 6672 6f6d 2044 6565 7057 4542 532e  ..from DeepWEBS.
+00000100: 646f 6375 6d65 6e74 732e 7175 6572 795f  documents.query_
+00000110: 7265 7375 6c74 735f 6578 7472 6163 746f  results_extracto
+00000120: 7220 696d 706f 7274 2051 7565 7279 5265  r import QueryRe
+00000130: 7375 6c74 7345 7874 7261 6374 6f72 0d0a  sultsExtractor..
+00000140: 6672 6f6d 2044 6565 7057 4542 532e 646f  from DeepWEBS.do
+00000150: 6375 6d65 6e74 732e 7765 6270 6167 655f  cuments.webpage_
+00000160: 636f 6e74 656e 745f 6578 7472 6163 746f  content_extracto
+00000170: 7220 696d 706f 7274 2042 6174 6368 5765  r import BatchWe
+00000180: 6270 6167 6543 6f6e 7465 6e74 4578 7472  bpageContentExtr
+00000190: 6163 746f 720d 0a66 726f 6d20 4465 6570  actor..from Deep
+000001a0: 5745 4253 2e75 7469 6c73 6477 2e6c 6f67  WEBS.utilsdw.log
+000001b0: 6765 7220 696d 706f 7274 206c 6f67 6765  ger import logge
+000001c0: 720d 0a69 6d70 6f72 7420 6172 6770 6172  r..import argpar
+000001d0: 7365 0d0a 0d0a 636c 6173 7320 4465 6570  se....class Deep
+000001e0: 5745 4253 3a0d 0a20 2020 2064 6566 205f  WEBS:..    def _
+000001f0: 5f69 6e69 745f 5f28 7365 6c66 293a 0d0a  _init__(self):..
+00000200: 2020 2020 2020 2020 7061 7373 0d0a 0d0a          pass....
+00000210: 2020 2020 636c 6173 7320 4465 6570 5365      class DeepSe
+00000220: 6172 6368 2842 6173 654d 6f64 656c 293a  arch(BaseModel):
+00000230: 0d0a 2020 2020 2020 2020 7175 6572 6965  ..        querie
+00000240: 733a 206c 6973 7420 3d20 4669 656c 6428  s: list = Field(
+00000250: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
+00000260: 6661 756c 743d 5b22 225d 2c0d 0a20 2020  fault=[""],..   
+00000270: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00000280: 7469 6f6e 3d22 286c 6973 745b 7374 725d  tion="(list[str]
+00000290: 2920 5175 6572 6965 7320 746f 2073 6561  ) Queries to sea
+000002a0: 7263 6822 2c0d 0a20 2020 2020 2020 2029  rch",..        )
+000002b0: 0d0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+000002c0: 5f6e 756d 3a20 696e 7420 3d20 4669 656c  _num: int = Fiel
+000002d0: 6428 0d0a 2020 2020 2020 2020 2020 2020  d(..            
+000002e0: 6465 6661 756c 743d 3130 2c0d 0a20 2020  default=10,..   
+000002f0: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00000300: 7469 6f6e 3d22 2869 6e74 2920 4e75 6d62  tion="(int) Numb
+00000310: 6572 206f 6620 7365 6172 6368 2072 6573  er of search res
+00000320: 756c 7473 222c 0d0a 2020 2020 2020 2020  ults",..        
+00000330: 290d 0a20 2020 2020 2020 2073 6166 653a  )..        safe:
+00000340: 2062 6f6f 6c20 3d20 4669 656c 6428 0d0a   bool = Field(..
+00000350: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+00000360: 756c 743d 4661 6c73 652c 0d0a 2020 2020  ult=False,..    
+00000370: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00000380: 696f 6e3d 2228 626f 6f6c 2920 456e 6162  ion="(bool) Enab
+00000390: 6c65 2053 6166 6553 6561 7263 6822 2c0d  le SafeSearch",.
+000003a0: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
+000003b0: 2020 2020 7479 7065 733a 206c 6973 7420      types: list 
+000003c0: 3d20 4669 656c 6428 0d0a 2020 2020 2020  = Field(..      
+000003d0: 2020 2020 2020 6465 6661 756c 743d 5b22        default=["
+000003e0: 7765 6222 5d2c 0d0a 2020 2020 2020 2020  web"],..        
+000003f0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
+00000400: 2228 6c69 7374 5b73 7472 5d29 2054 7970  "(list[str]) Typ
+00000410: 6573 206f 6620 7365 6172 6368 2072 6573  es of search res
+00000420: 756c 7473 3a20 6077 6562 602c 2060 696d  ults: `web`, `im
+00000430: 6167 6560 2c20 6076 6964 656f 7360 2c20  age`, `videos`, 
+00000440: 606e 6577 7360 222c 0d0a 2020 2020 2020  `news`",..      
+00000450: 2020 290d 0a20 2020 2020 2020 2065 7874    )..        ext
+00000460: 7261 6374 5f77 6562 7061 6765 3a20 626f  ract_webpage: bo
+00000470: 6f6c 203d 2046 6965 6c64 280d 0a20 2020  ol = Field(..   
+00000480: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+00000490: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
+000004a0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+000004b0: 3d22 2862 6f6f 6c29 2045 6e61 626c 6520  ="(bool) Enable 
+000004c0: 6578 7472 6163 7469 6e67 206d 6169 6e20  extracting main 
+000004d0: 7465 7874 2063 6f6e 7465 6e74 7320 6672  text contents fr
+000004e0: 6f6d 2077 6562 7061 6765 2c20 7769 6c6c  om webpage, will
+000004f0: 2061 6464 2060 7465 7874 6020 6669 6c65   add `text` file
+00000500: 6420 696e 2065 6163 6820 6071 7565 7279  d in each `query
+00000510: 5f72 6573 756c 7460 2064 6963 7422 2c0d  _result` dict",.
+00000520: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
+00000530: 2020 2020 6f76 6572 7772 6974 655f 7175      overwrite_qu
+00000540: 6572 795f 6874 6d6c 3a20 626f 6f6c 203d  ery_html: bool =
+00000550: 2046 6965 6c64 280d 0a20 2020 2020 2020   Field(..       
+00000560: 2020 2020 2064 6566 6175 6c74 3d46 616c       default=Fal
+00000570: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
+00000580: 2064 6573 6372 6970 7469 6f6e 3d22 2862   description="(b
+00000590: 6f6f 6c29 204f 7665 7277 7269 7465 2048  ool) Overwrite H
+000005a0: 544d 4c20 6669 6c65 206f 6620 7175 6572  TML file of quer
+000005b0: 7920 7265 7375 6c74 7322 2c0d 0a20 2020  y results",..   
+000005c0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+000005d0: 6f76 6572 7772 6974 655f 7765 6270 6167  overwrite_webpag
+000005e0: 655f 6874 6d6c 3a20 626f 6f6c 203d 2046  e_html: bool = F
+000005f0: 6965 6c64 280d 0a20 2020 2020 2020 2020  ield(..         
+00000600: 2020 2064 6566 6175 6c74 3d46 616c 7365     default=False
+00000610: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
+00000620: 6573 6372 6970 7469 6f6e 3d22 2862 6f6f  escription="(boo
+00000630: 6c29 204f 7665 7277 7269 7465 2048 544d  l) Overwrite HTM
+00000640: 4c20 6669 6c65 7320 6f66 2077 6562 7061  L files of webpa
+00000650: 6765 7320 6672 6f6d 2071 7565 7279 2072  ges from query r
+00000660: 6573 756c 7473 222c 0d0a 2020 2020 2020  esults",..      
+00000670: 2020 290d 0a0d 0a20 2020 2064 6566 2071    )....    def q
+00000680: 7565 7269 6573 5f74 6f5f 7365 6172 6368  ueries_to_search
+00000690: 5f72 6573 756c 7473 2873 656c 662c 2069  _results(self, i
+000006a0: 7465 6d3a 2044 6565 7053 6561 7263 6829  tem: DeepSearch)
+000006b0: 3a0d 0a20 2020 2020 2020 2067 6f6f 676c  :..        googl
+000006c0: 655f 7365 6172 6368 6572 203d 2047 6f6f  e_searcher = Goo
+000006d0: 676c 6553 6561 7263 6865 7228 290d 0a20  gleSearcher().. 
+000006e0: 2020 2020 2020 2071 7565 7269 6573 5f73         queries_s
+000006f0: 6561 7263 685f 7265 7375 6c74 7320 3d20  earch_results = 
+00000700: 5b5d 0d0a 2020 2020 2020 2020 666f 7220  []..        for 
+00000710: 7175 6572 7920 696e 2069 7465 6d2e 7175  query in item.qu
+00000720: 6572 6965 733a 0d0a 2020 2020 2020 2020  eries:..        
+00000730: 2020 2020 7175 6572 795f 7265 7375 6c74      query_result
+00000740: 735f 6578 7472 6163 746f 7220 3d20 5175  s_extractor = Qu
+00000750: 6572 7952 6573 756c 7473 4578 7472 6163  eryResultsExtrac
+00000760: 746f 7228 290d 0a20 2020 2020 2020 2020  tor()..         
+00000770: 2020 2069 6620 6e6f 7420 7175 6572 792e     if not query.
+00000780: 7374 7269 7028 293a 0d0a 2020 2020 2020  strip():..      
+00000790: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+000007a0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+000007b0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+000007c0: 2020 2020 2020 7175 6572 795f 6874 6d6c        query_html
+000007d0: 5f70 6174 6820 3d20 676f 6f67 6c65 5f73  _path = google_s
+000007e0: 6561 7263 6865 722e 7365 6172 6368 280d  earcher.search(.
+000007f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000800: 2020 2020 2071 7565 7279 3d71 7565 7279       query=query
+00000810: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000820: 2020 2020 2020 2072 6573 756c 745f 6e75         result_nu
+00000830: 6d3d 6974 656d 2e72 6573 756c 745f 6e75  m=item.result_nu
+00000840: 6d2c 0d0a 2020 2020 2020 2020 2020 2020  m,..            
+00000850: 2020 2020 2020 2020 7361 6665 3d69 7465          safe=ite
+00000860: 6d2e 7361 6665 2c0d 0a20 2020 2020 2020  m.safe,..       
+00000870: 2020 2020 2020 2020 2020 2020 206f 7665               ove
+00000880: 7277 7269 7465 3d69 7465 6d2e 6f76 6572  rwrite=item.over
+00000890: 7772 6974 655f 7175 6572 795f 6874 6d6c  write_query_html
+000008a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000008b0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+000008c0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+000008d0: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
+000008e0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+000008f0: 2e65 7272 6f72 2866 2246 6169 6c65 6420  .error(f"Failed 
+00000900: 746f 2073 6561 7263 6820 666f 7220 7175  to search for qu
+00000910: 6572 7920 277b 7175 6572 797d 273a 207b  ery '{query}': {
+00000920: 657d 2229 0d0a 2020 2020 2020 2020 2020  e}")..          
+00000930: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
+00000940: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+00000950: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+00000960: 2020 2020 7175 6572 795f 7365 6172 6368      query_search
+00000970: 5f72 6573 756c 7473 203d 2071 7565 7279  _results = query
+00000980: 5f72 6573 756c 7473 5f65 7874 7261 6374  _results_extract
+00000990: 6f72 2e65 7874 7261 6374 2871 7565 7279  or.extract(query
+000009a0: 5f68 746d 6c5f 7061 7468 290d 0a20 2020  _html_path)..   
+000009b0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+000009c0: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
+000009d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000009e0: 206c 6f67 6765 722e 6572 726f 7228 6622   logger.error(f"
+000009f0: 4661 696c 6564 2074 6f20 6578 7472 6163  Failed to extrac
+00000a00: 7420 7365 6172 6368 2072 6573 756c 7473  t search results
+00000a10: 2066 6f72 2071 7565 7279 2027 7b71 7565   for query '{que
+00000a20: 7279 7d27 3a20 7b65 7d22 290d 0a20 2020  ry}': {e}")..   
+00000a30: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00000a40: 7469 6e75 650d 0a0d 0a20 2020 2020 2020  tinue....       
+00000a50: 2020 2020 2071 7565 7269 6573 5f73 6561       queries_sea
+00000a60: 7263 685f 7265 7375 6c74 732e 6170 7065  rch_results.appe
+00000a70: 6e64 2871 7565 7279 5f73 6561 7263 685f  nd(query_search_
+00000a80: 7265 7375 6c74 7329 0d0a 2020 2020 2020  results)..      
+00000a90: 2020 6c6f 6767 6572 2e6e 6f74 6528 7175    logger.note(qu
+00000aa0: 6572 6965 735f 7365 6172 6368 5f72 6573  eries_search_res
+00000ab0: 756c 7473 290d 0a0d 0a20 2020 2020 2020  ults)....       
+00000ac0: 2069 6620 6974 656d 2e65 7874 7261 6374   if item.extract
+00000ad0: 5f77 6562 7061 6765 3a0d 0a20 2020 2020  _webpage:..     
+00000ae0: 2020 2020 2020 2071 7565 7269 6573 5f73         queries_s
+00000af0: 6561 7263 685f 7265 7375 6c74 7320 3d20  earch_results = 
+00000b00: 7365 6c66 2e65 7874 7261 6374 5f77 6562  self.extract_web
+00000b10: 7061 6765 7328 0d0a 2020 2020 2020 2020  pages(..        
+00000b20: 2020 2020 2020 2020 7175 6572 6965 735f          queries_
+00000b30: 7365 6172 6368 5f72 6573 756c 7473 2c0d  search_results,.
+00000b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000b50: 206f 7665 7277 7269 7465 5f77 6562 7061   overwrite_webpa
+00000b60: 6765 5f68 746d 6c3d 6974 656d 2e6f 7665  ge_html=item.ove
+00000b70: 7277 7269 7465 5f77 6562 7061 6765 5f68  rwrite_webpage_h
+00000b80: 746d 6c2c 0d0a 2020 2020 2020 2020 2020  tml,..          
+00000b90: 2020 290d 0a20 2020 2020 2020 2072 6574    )..        ret
+00000ba0: 7572 6e20 7175 6572 6965 735f 7365 6172  urn queries_sear
+00000bb0: 6368 5f72 6573 756c 7473 0d0a 0d0a 2020  ch_results....  
+00000bc0: 2020 6465 6620 6578 7472 6163 745f 7765    def extract_we
+00000bd0: 6270 6167 6573 2873 656c 662c 2071 7565  bpages(self, que
+00000be0: 7269 6573 5f73 6561 7263 685f 7265 7375  ries_search_resu
+00000bf0: 6c74 732c 206f 7665 7277 7269 7465 5f77  lts, overwrite_w
+00000c00: 6562 7061 6765 5f68 746d 6c3d 4661 6c73  ebpage_html=Fals
+00000c10: 6529 3a0d 0a20 2020 2020 2020 2066 6f72  e):..        for
+00000c20: 2071 7565 7279 5f69 6478 2c20 7175 6572   query_idx, quer
+00000c30: 795f 7365 6172 6368 5f72 6573 756c 7473  y_search_results
+00000c40: 2069 6e20 656e 756d 6572 6174 6528 7175   in enumerate(qu
+00000c50: 6572 6965 735f 7365 6172 6368 5f72 6573  eries_search_res
+00000c60: 756c 7473 293a 0d0a 2020 2020 2020 2020  ults):..        
+00000c70: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00000c80: 2020 2020 2020 2020 2020 2320 4665 7463            # Fetc
+00000c90: 6820 7765 6270 6167 6573 2077 6974 6820  h webpages with 
+00000ca0: 7572 6c73 0d0a 2020 2020 2020 2020 2020  urls..          
+00000cb0: 2020 2020 2020 6261 7463 685f 7765 6270        batch_webp
+00000cc0: 6167 655f 6665 7463 6865 7220 3d20 4261  age_fetcher = Ba
+00000cd0: 7463 6857 6562 7061 6765 4665 7463 6865  tchWebpageFetche
+00000ce0: 7228 290d 0a20 2020 2020 2020 2020 2020  r()..           
+00000cf0: 2020 2020 2075 726c 7320 3d20 5b0d 0a20       urls = [.. 
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 2020 2071 7565 7279 5f72 6573 756c 745b     query_result[
+00000d20: 2275 726c 225d 0d0a 2020 2020 2020 2020  "url"]..        
+00000d30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00000d40: 7175 6572 795f 7265 7375 6c74 2069 6e20  query_result in 
+00000d50: 7175 6572 795f 7365 6172 6368 5f72 6573  query_search_res
+00000d60: 756c 7473 5b22 7175 6572 795f 7265 7375  ults["query_resu
+00000d70: 6c74 7322 5d0d 0a20 2020 2020 2020 2020  lts"]..         
+00000d80: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+00000d90: 2020 2020 2020 2020 2020 7572 6c5f 616e            url_an
+00000da0: 645f 6874 6d6c 5f70 6174 685f 6c69 7374  d_html_path_list
+00000db0: 203d 2062 6174 6368 5f77 6562 7061 6765   = batch_webpage
+00000dc0: 5f66 6574 6368 6572 2e66 6574 6368 280d  _fetcher.fetch(.
+00000dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000de0: 2020 2020 2075 726c 732c 0d0a 2020 2020       urls,..    
+00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e00: 6f76 6572 7772 6974 653d 6f76 6572 7772  overwrite=overwr
+00000e10: 6974 655f 7765 6270 6167 655f 6874 6d6c  ite_webpage_html
+00000e20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000e30: 2020 2020 2020 206f 7574 7075 745f 7061         output_pa
+00000e40: 7265 6e74 3d71 7565 7279 5f73 6561 7263  rent=query_searc
+00000e50: 685f 7265 7375 6c74 735b 2271 7565 7279  h_results["query
+00000e60: 225d 2c0d 0a20 2020 2020 2020 2020 2020  "],..           
+00000e70: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00000e80: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00000e90: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
+00000ea0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00000eb0: 6572 2e65 7272 6f72 2866 2246 6169 6c65  er.error(f"Faile
+00000ec0: 6420 746f 2066 6574 6368 2077 6562 7061  d to fetch webpa
+00000ed0: 6765 7320 666f 7220 7175 6572 7920 277b  ges for query '{
+00000ee0: 7175 6572 795f 7365 6172 6368 5f72 6573  query_search_res
+00000ef0: 756c 7473 5b27 7175 6572 7927 5d7d 273a  ults['query']}':
+00000f00: 207b 657d 2229 0d0a 2020 2020 2020 2020   {e}")..        
+00000f10: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00000f20: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00000f30: 2320 4578 7472 6163 7420 7765 6270 6167  # Extract webpag
+00000f40: 6520 636f 6e74 656e 7473 2066 726f 6d20  e contents from 
+00000f50: 6874 6d6c 730d 0a20 2020 2020 2020 2020  htmls..         
+00000f60: 2020 2068 746d 6c5f 7061 7468 7320 3d20     html_paths = 
+00000f70: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+00000f80: 2020 2073 7472 2875 726c 5f61 6e64 5f68     str(url_and_h
+00000f90: 746d 6c5f 7061 7468 5b22 6874 6d6c 5f70  tml_path["html_p
+00000fa0: 6174 6822 5d29 0d0a 2020 2020 2020 2020  ath"])..        
+00000fb0: 2020 2020 2020 2020 666f 7220 7572 6c5f          for url_
+00000fc0: 616e 645f 6874 6d6c 5f70 6174 6820 696e  and_html_path in
+00000fd0: 2075 726c 5f61 6e64 5f68 746d 6c5f 7061   url_and_html_pa
+00000fe0: 7468 5f6c 6973 740d 0a20 2020 2020 2020  th_list..       
+00000ff0: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
+00001000: 2020 2020 6261 7463 685f 7765 6270 6167      batch_webpag
+00001010: 655f 636f 6e74 656e 745f 6578 7472 6163  e_content_extrac
+00001020: 746f 7220 3d20 4261 7463 6857 6562 7061  tor = BatchWebpa
+00001030: 6765 436f 6e74 656e 7445 7874 7261 6374  geContentExtract
+00001040: 6f72 2829 0d0a 2020 2020 2020 2020 2020  or()..          
+00001050: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+00001060: 2020 2020 2020 2020 6874 6d6c 5f70 6174          html_pat
+00001070: 685f 616e 645f 6578 7472 6163 7465 645f  h_and_extracted_
+00001080: 636f 6e74 656e 745f 6c69 7374 203d 2028  content_list = (
+00001090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000010a0: 2020 2020 2020 6261 7463 685f 7765 6270        batch_webp
+000010b0: 6167 655f 636f 6e74 656e 745f 6578 7472  age_content_extr
+000010c0: 6163 746f 722e 6578 7472 6163 7428 6874  actor.extract(ht
+000010d0: 6d6c 5f70 6174 6873 290d 0a20 2020 2020  ml_paths)..     
+000010e0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+000010f0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00001100: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+00001110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001120: 2020 6c6f 6767 6572 2e65 7272 6f72 2866    logger.error(f
+00001130: 2246 6169 6c65 6420 746f 2065 7874 7261  "Failed to extra
+00001140: 6374 2077 6562 7061 6765 2063 6f6e 7465  ct webpage conte
+00001150: 6e74 7320 666f 7220 7175 6572 7920 277b  nts for query '{
+00001160: 7175 6572 795f 7365 6172 6368 5f72 6573  query_search_res
+00001170: 756c 7473 5b27 7175 6572 7927 5d7d 273a  ults['query']}':
+00001180: 207b 657d 2229 0d0a 2020 2020 2020 2020   {e}")..        
+00001190: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+000011a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000011b0: 2320 4275 696c 6420 7468 6520 6d61 7020  # Build the map 
+000011c0: 6f66 2075 726c 2074 6f20 6578 7472 6163  of url to extrac
+000011d0: 7465 645f 636f 6e74 656e 740d 0a20 2020  ted_content..   
+000011e0: 2020 2020 2020 2020 2068 746d 6c5f 7061           html_pa
+000011f0: 7468 5f74 6f5f 7572 6c5f 6469 6374 203d  th_to_url_dict =
+00001200: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00001210: 2020 2020 7374 7228 7572 6c5f 616e 645f      str(url_and_
+00001220: 6874 6d6c 5f70 6174 685b 2268 746d 6c5f  html_path["html_
+00001230: 7061 7468 225d 293a 2075 726c 5f61 6e64  path"]): url_and
+00001240: 5f68 746d 6c5f 7061 7468 5b22 7572 6c22  _html_path["url"
+00001250: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00001260: 2020 2066 6f72 2075 726c 5f61 6e64 5f68     for url_and_h
+00001270: 746d 6c5f 7061 7468 2069 6e20 7572 6c5f  tml_path in url_
+00001280: 616e 645f 6874 6d6c 5f70 6174 685f 6c69  and_html_path_li
+00001290: 7374 0d0a 2020 2020 2020 2020 2020 2020  st..            
+000012a0: 7d0d 0a20 2020 2020 2020 2020 2020 2075  }..            u
+000012b0: 726c 5f74 6f5f 6578 7472 6163 7465 645f  rl_to_extracted_
+000012c0: 636f 6e74 656e 745f 6469 6374 203d 207b  content_dict = {
+000012d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000012e0: 2020 6874 6d6c 5f70 6174 685f 746f 5f75    html_path_to_u
+000012f0: 726c 5f64 6963 745b 0d0a 2020 2020 2020  rl_dict[..      
+00001300: 2020 2020 2020 2020 2020 2020 2020 6874                ht
+00001310: 6d6c 5f70 6174 685f 616e 645f 6578 7472  ml_path_and_extr
+00001320: 6163 7465 645f 636f 6e74 656e 745b 2268  acted_content["h
+00001330: 746d 6c5f 7061 7468 225d 0d0a 2020 2020  tml_path"]..    
+00001340: 2020 2020 2020 2020 2020 2020 5d3a 2068              ]: h
+00001350: 746d 6c5f 7061 7468 5f61 6e64 5f65 7874  tml_path_and_ext
+00001360: 7261 6374 6564 5f63 6f6e 7465 6e74 5b22  racted_content["
+00001370: 6578 7472 6163 7465 645f 636f 6e74 656e  extracted_conten
+00001380: 7422 5d0d 0a20 2020 2020 2020 2020 2020  t"]..           
+00001390: 2020 2020 2066 6f72 2068 746d 6c5f 7061       for html_pa
+000013a0: 7468 5f61 6e64 5f65 7874 7261 6374 6564  th_and_extracted
+000013b0: 5f63 6f6e 7465 6e74 2069 6e20 6874 6d6c  _content in html
+000013c0: 5f70 6174 685f 616e 645f 6578 7472 6163  _path_and_extrac
+000013d0: 7465 645f 636f 6e74 656e 745f 6c69 7374  ted_content_list
+000013e0: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
+000013f0: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
+00001400: 2057 7269 7465 2065 7874 7261 6374 6564   Write extracted
+00001410: 2063 6f6e 7465 6e74 7320 2861 7320 2774   contents (as 't
+00001420: 6578 7427 2066 6965 6c64 2920 746f 2071  ext' field) to q
+00001430: 7565 7279 5f73 6561 7263 685f 7265 7375  uery_search_resu
+00001440: 6c74 730d 0a20 2020 2020 2020 2020 2020  lts..           
+00001450: 2066 6f72 2071 7565 7279 5f72 6573 756c   for query_resul
+00001460: 745f 6964 782c 2071 7565 7279 5f72 6573  t_idx, query_res
+00001470: 756c 7420 696e 2065 6e75 6d65 7261 7465  ult in enumerate
+00001480: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00001490: 2020 2071 7565 7279 5f73 6561 7263 685f     query_search_
+000014a0: 7265 7375 6c74 735b 2271 7565 7279 5f72  results["query_r
+000014b0: 6573 756c 7473 225d 0d0a 2020 2020 2020  esults"]..      
+000014c0: 2020 2020 2020 293a 0d0a 2020 2020 2020        ):..      
+000014d0: 2020 2020 2020 2020 2020 7572 6c20 3d20            url = 
+000014e0: 7175 6572 795f 7265 7375 6c74 5b22 7572  query_result["ur
+000014f0: 6c22 5d0d 0a20 2020 2020 2020 2020 2020  l"]..           
+00001500: 2020 2020 2065 7874 7261 6374 6564 5f63       extracted_c
+00001510: 6f6e 7465 6e74 203d 2075 726c 5f74 6f5f  ontent = url_to_
+00001520: 6578 7472 6163 7465 645f 636f 6e74 656e  extracted_conten
+00001530: 745f 6469 6374 2e67 6574 2875 726c 2c20  t_dict.get(url, 
+00001540: 2222 290d 0a20 2020 2020 2020 2020 2020  "")..           
+00001550: 2020 2020 2071 7565 7269 6573 5f73 6561       queries_sea
+00001560: 7263 685f 7265 7375 6c74 735b 7175 6572  rch_results[quer
+00001570: 795f 6964 785d 5b22 7175 6572 795f 7265  y_idx]["query_re
+00001580: 7375 6c74 7322 5d5b 7175 6572 795f 7265  sults"][query_re
+00001590: 7375 6c74 5f69 6478 5d5b 0d0a 2020 2020  sult_idx][..    
+000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015b0: 2274 6578 7422 0d0a 2020 2020 2020 2020  "text"..        
+000015c0: 2020 2020 2020 2020 5d20 3d20 6578 7472          ] = extr
+000015d0: 6163 7465 645f 636f 6e74 656e 740d 0a0d  acted_content...
+000015e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000015f0: 7175 6572 6965 735f 7365 6172 6368 5f72  queries_search_r
+00001600: 6573 756c 7473 0d0a 0d0a 0d0a 636c 6173  esults......clas
+00001610: 7320 4172 6750 6172 7365 7228 6172 6770  s ArgParser(argp
+00001620: 6172 7365 2e41 7267 756d 656e 7450 6172  arse.ArgumentPar
+00001630: 7365 7229 3a0d 0a20 2020 2064 6566 205f  ser):..    def _
+00001640: 5f69 6e69 745f 5f28 7365 6c66 2c20 2a61  _init__(self, *a
+00001650: 7267 732c 202a 2a6b 7761 7267 7329 3a0d  rgs, **kwargs):.
+00001660: 0a20 2020 2020 2020 2073 7570 6572 2841  .        super(A
+00001670: 7267 5061 7273 6572 2c20 7365 6c66 292e  rgParser, self).
+00001680: 5f5f 696e 6974 5f5f 282a 6172 6773 2c20  __init__(*args, 
+00001690: 2a2a 6b77 6172 6773 290d 0a0d 0a20 2020  **kwargs)....   
+000016a0: 2020 2020 2073 656c 662e 6164 645f 6172       self.add_ar
+000016b0: 6775 6d65 6e74 280d 0a20 2020 2020 2020  gument(..       
+000016c0: 2020 2020 2022 2d71 222c 0d0a 2020 2020       "-q",..    
+000016d0: 2020 2020 2020 2020 222d 2d71 7565 7269          "--queri
+000016e0: 6573 222c 0d0a 2020 2020 2020 2020 2020  es",..          
+000016f0: 2020 7479 7065 3d73 7472 2c0d 0a20 2020    type=str,..   
+00001700: 2020 2020 2020 2020 206e 6172 6773 3d22           nargs="
+00001710: 2b22 2c0d 0a20 2020 2020 2020 2020 2020  +",..           
+00001720: 2072 6571 7569 7265 643d 5472 7565 2c0d   required=True,.
+00001730: 0a20 2020 2020 2020 2020 2020 2068 656c  .            hel
+00001740: 703d 2251 7565 7269 6573 2074 6f20 7365  p="Queries to se
+00001750: 6172 6368 222c 0d0a 2020 2020 2020 2020  arch",..        
+00001760: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00001770: 6164 645f 6172 6775 6d65 6e74 280d 0a20  add_argument(.. 
+00001780: 2020 2020 2020 2020 2020 2022 2d6e 222c             "-n",
+00001790: 0d0a 2020 2020 2020 2020 2020 2020 222d  ..            "-
+000017a0: 2d72 6573 756c 745f 6e75 6d22 2c0d 0a20  -result_num",.. 
+000017b0: 2020 2020 2020 2020 2020 2074 7970 653d             type=
+000017c0: 696e 742c 0d0a 2020 2020 2020 2020 2020  int,..          
+000017d0: 2020 6465 6661 756c 743d 3130 2c0d 0a20    default=10,.. 
+000017e0: 2020 2020 2020 2020 2020 2068 656c 703d             help=
+000017f0: 224e 756d 6265 7220 6f66 2073 6561 7263  "Number of searc
+00001800: 6820 7265 7375 6c74 7322 2c0d 0a20 2020  h results",..   
+00001810: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00001820: 7365 6c66 2e61 6464 5f61 7267 756d 656e  self.add_argumen
+00001830: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00001840: 222d 7322 2c0d 0a20 2020 2020 2020 2020  "-s",..         
+00001850: 2020 2022 2d2d 7361 6665 222c 0d0a 2020     "--safe",..  
+00001860: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
+00001870: 743d 4661 6c73 652c 0d0a 2020 2020 2020  t=False,..      
+00001880: 2020 2020 2020 6163 7469 6f6e 3d22 7374        action="st
+00001890: 6f72 655f 7472 7565 222c 0d0a 2020 2020  ore_true",..    
+000018a0: 2020 2020 2020 2020 6865 6c70 3d22 456e          help="En
+000018b0: 6162 6c65 2053 6166 6553 6561 7263 6822  able SafeSearch"
+000018c0: 2c0d 0a20 2020 2020 2020 2029 0d0a 2020  ,..        )..  
+000018d0: 2020 2020 2020 7365 6c66 2e61 6464 5f61        self.add_a
+000018e0: 7267 756d 656e 7428 0d0a 2020 2020 2020  rgument(..      
+000018f0: 2020 2020 2020 222d 7422 2c0d 0a20 2020        "-t",..   
+00001900: 2020 2020 2020 2020 2022 2d2d 7479 7065           "--type
+00001910: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
+00001920: 2074 7970 653d 7374 722c 0d0a 2020 2020   type=str,..    
+00001930: 2020 2020 2020 2020 6e61 7267 733d 222b          nargs="+
+00001940: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00001950: 6465 6661 756c 743d 5b22 7765 6222 5d2c  default=["web"],
+00001960: 0d0a 2020 2020 2020 2020 2020 2020 6368  ..            ch
+00001970: 6f69 6365 733d 5b22 7765 6222 2c20 2269  oices=["web", "i
+00001980: 6d61 6765 222c 2022 7669 6465 6f73 222c  mage", "videos",
+00001990: 2022 6e65 7773 225d 2c0d 0a20 2020 2020   "news"],..     
+000019a0: 2020 2020 2020 2068 656c 703d 2254 7970         help="Typ
+000019b0: 6573 206f 6620 7365 6172 6368 2072 6573  es of search res
+000019c0: 756c 7473 222c 0d0a 2020 2020 2020 2020  ults",..        
+000019d0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000019e0: 6164 645f 6172 6775 6d65 6e74 280d 0a20  add_argument(.. 
+000019f0: 2020 2020 2020 2020 2020 2022 2d65 222c             "-e",
+00001a00: 0d0a 2020 2020 2020 2020 2020 2020 222d  ..            "-
+00001a10: 2d65 7874 7261 6374 5f77 6562 7061 6765  -extract_webpage
+00001a20: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00001a30: 6465 6661 756c 743d 4661 6c73 652c 0d0a  default=False,..
+00001a40: 2020 2020 2020 2020 2020 2020 6163 7469              acti
+00001a50: 6f6e 3d22 7374 6f72 655f 7472 7565 222c  on="store_true",
+00001a60: 0d0a 2020 2020 2020 2020 2020 2020 6865  ..            he
+00001a70: 6c70 3d22 456e 6162 6c65 2065 7874 7261  lp="Enable extra
+00001a80: 6374 696e 6720 6d61 696e 2074 6578 7420  cting main text 
+00001a90: 636f 6e74 656e 7473 2066 726f 6d20 7765  contents from we
+00001aa0: 6270 6167 6522 2c0d 0a20 2020 2020 2020  bpage",..       
+00001ab0: 2029 0d0a 2020 2020 2020 2020 7365 6c66   )..        self
+00001ac0: 2e61 6464 5f61 7267 756d 656e 7428 0d0a  .add_argument(..
+00001ad0: 2020 2020 2020 2020 2020 2020 222d 6f22              "-o"
+00001ae0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00001af0: 2d2d 6f76 6572 7772 6974 655f 7175 6572  --overwrite_quer
+00001b00: 795f 6874 6d6c 222c 0d0a 2020 2020 2020  y_html",..      
+00001b10: 2020 2020 2020 6465 6661 756c 743d 4661        default=Fa
+00001b20: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00001b30: 2020 6163 7469 6f6e 3d22 7374 6f72 655f    action="store_
+00001b40: 7472 7565 222c 0d0a 2020 2020 2020 2020  true",..        
+00001b50: 2020 2020 6865 6c70 3d22 4f76 6572 7772      help="Overwr
+00001b60: 6974 6520 4854 4d4c 2066 696c 6520 6f66  ite HTML file of
+00001b70: 2071 7565 7279 2072 6573 756c 7473 222c   query results",
+00001b80: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
+00001b90: 2020 2020 2073 656c 662e 6164 645f 6172       self.add_ar
+00001ba0: 6775 6d65 6e74 280d 0a20 2020 2020 2020  gument(..       
+00001bb0: 2020 2020 2022 2d77 222c 0d0a 2020 2020       "-w",..    
+00001bc0: 2020 2020 2020 2020 222d 2d6f 7665 7277          "--overw
+00001bd0: 7269 7465 5f77 6562 7061 6765 5f68 746d  rite_webpage_htm
+00001be0: 6c22 2c0d 0a20 2020 2020 2020 2020 2020  l",..           
+00001bf0: 2064 6566 6175 6c74 3d46 616c 7365 2c0d   default=False,.
+00001c00: 0a20 2020 2020 2020 2020 2020 2061 6374  .            act
+00001c10: 696f 6e3d 2273 746f 7265 5f74 7275 6522  ion="store_true"
+00001c20: 2c0d 0a20 2020 2020 2020 2020 2020 2068  ,..            h
+00001c30: 656c 703d 224f 7665 7277 7269 7465 2048  elp="Overwrite H
+00001c40: 544d 4c20 6669 6c65 7320 6f66 2077 6562  TML files of web
+00001c50: 7061 6765 7320 6672 6f6d 2071 7565 7279  pages from query
+00001c60: 2072 6573 756c 7473 222c 0d0a 2020 2020   results",..    
+00001c70: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
+00001c80: 2073 656c 662e 6172 6773 203d 2073 656c   self.args = sel
+00001c90: 662e 7061 7273 655f 6172 6773 2829 0d0a  f.parse_args()..
+00001ca0: 0d0a 0d0a                                ....
```

### Comparing `webscout-1.2.3/webscout/HelpingAI.py` & `webscout-1.2.4/webscout/HelpingAI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/webscout/LLM.py` & `webscout-1.2.4/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/webscout/cli.py` & `webscout-1.2.4/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/webscout/models.py` & `webscout-1.2.4/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/webscout/utils.py` & `webscout-1.2.4/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/webscout/webscout_search.py` & `webscout-1.2.4/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/webscout/webscout_search_async.py` & `webscout-1.2.4/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.3/webscout.egg-info/PKG-INFO` & `webscout-1.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,58 +1,7 @@
-Metadata-Version: 2.1
-Name: webscout
-Version: 1.2.3
-Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
-Author: OEvortex
-Author-email: helpingai5@gmail.com
-License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
-Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
-Project-URL: YouTube, https://youtube.com/@OEvortex
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: docstring_inheritance>=2.1.2
-Requires-Dist: click>=8.1.7
-Requires-Dist: curl_cffi>=0.6.0b7
-Requires-Dist: lxml>=5.1.0
-Requires-Dist: nest-asyncio>=1.6.0
-Requires-Dist: selenium>=4.1.3
-Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4
-Requires-Dist: halo>=0.0.31
-Requires-Dist: g4f>=0.2.2.3
-Requires-Dist: rich
-Requires-Dist: python-dotenv
-Requires-Dist: Helpingai-T2
-Requires-Dist: beautifulsoup4
-Requires-Dist: markdownify
-Requires-Dist: pydantic
-Requires-Dist: requests
-Requires-Dist: sse_starlette
-Requires-Dist: termcolor
-Requires-Dist: tiktoken
-Requires-Dist: tldextract
-Provides-Extra: dev
-Requires-Dist: ruff>=0.1.6; extra == "dev"
-Requires-Dist: pytest>=7.4.2; extra == "dev"
-
 #  webscout
 <p align="center">
 
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
 Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
@@ -88,14 +37,15 @@
     - [3. `You.com` - search with you.com](#3-youcom---search-with-youcom)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
+    - [9. `GPT4ALL` - chat offline with Language models using gpt4all from webscout](#9-gpt4all---chat-offline-with-language-models-using-gpt4all-from-webscout)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
 
 ## Install
 ```python
 pip install -U webscout
 ```
@@ -601,14 +551,45 @@
 
 opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30)
 # This example sends a simple greeting and prints the response
 prompt = "tell me about india"
 response_str = opengpt.chat(prompt)
 print(response_str)
 ```
+### 9. `GPT4ALL` - chat offline with Language models using gpt4all from webscout
+```python
+from webscout import GPT4ALL
+
+# Initialize the GPT4ALL class with your model path and other optional parameters
+gpt4all_instance = GPT4ALL(
+    model="path/to/your/model/file", # Replace with the actual path to your model file
+    is_conversation=True,
+    max_tokens=800,
+    temperature=0.7,
+    presence_penalty=0,
+    frequency_penalty=1.18,
+    top_p=0.4,
+    intro="Hello, how can I assist you today?",
+    filepath="path/to/conversation/history/file", # Optional, for conversation history
+    update_file=True,
+    history_offset=10250,
+    act=None # Optional, for using an awesome prompt as intro
+)
+
+# Generate a response from the AI model
+response = gpt4all_instance.chat(
+    prompt="What is the weather like today?",
+    stream=False, # Set to True if you want to stream the response
+    optimizer=None, # Optional, specify an optimizer if needed
+    conversationally=False # Set to True for conversationally generated responses
+)
+
+# Print the generated response
+print(response)
+```
 
 ## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
```

#### html2text {}

```diff
@@ -1,35 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.2.3 Summary: Search for words,
-documents, images, videos, news, maps and text translation using the Google,
-DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
-Author: OEvortex Author-email: helpingai5@gmail.com License: HelpingAI
-Simplified Universal License Project-URL: Documentation, https://github.com/OE-
-LUCIFER/Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/
-Webscout Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
-Project-URL: YouTube, https://youtube.com/@OEvortex Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-docstring_inheritance>=2.1.2 Requires-Dist: click>=8.1.7 Requires-Dist:
-curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
-Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
-Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
-Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
-Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist:
-pytest>=7.4.2; extra == "dev" # webscout
+# webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
 you.com, etc Also containes AI models Also containes AI models that you can use
  ## Table of Contents - [webscout](#webscout) - [Table of Contents](#table-of-
 contents) - [Install](#install) - [CLI version](#cli-version) - [CLI version of
 webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
 [Regions](#regions) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
@@ -55,15 +28,17 @@
   [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
 `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
   [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
  webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
   using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
   searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
  perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-   opengpt---chat-with-opengpt) - [usage of special .LLM file from webscout
+   opengpt---chat-with-opengpt) - [9. `GPT4ALL` - chat offline with Language
+ models using gpt4all from webscout](#9-gpt4all---chat-offline-with-language-
+models-using-gpt4all-from-webscout) - [usage of special .LLM file from webscout
 (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm) - [`LLM`]
     (#llm) ## Install ```python pip install -U webscout ``` ## CLI version
 ```python3 python -m webscout --help ``` | Command | Description | |-----------
 --------------------------------|----------------------------------------------
 ---------------------------------------------------------| | python -m webscout
 answers -k Text | CLI function to perform an answers search using Webscout. | |
  python -m webscout images -k Text | CLI function to perform an images search
@@ -239,14 +214,27 @@
   7. `PERPLEXITY` - Search With PERPLEXITY ```python from webscout.AI import
 PERPLEXITY # Create an instance of the PERPLEXITY class perplexity = PERPLEXITY
    () # Example usage: prompt = "Explain the concept of recursion in simple
 terms." response = perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT`
 - chat With OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
   (is_conversation=True, max_tokens=8000, timeout=30) # This example sends a
     simple greeting and prints the response prompt = "tell me about india"
-response_str = opengpt.chat(prompt) print(response_str) ``` ## usage of special
- .LLM file from webscout (webscout.LLM) ### `LLM` ```python from webscout.LLM
-   import LLM def chat(model_name, system_message="You are Jarvis"):# system
-     prompt AI = LLM(model_name, system_message) AI.chat() if __name__ ==
-  "__main__": model_name = "mistralai/Mistral-7B-Instruct-v0.1" # name of the
-model you wish to use It supports ALL text generation models on deepinfra.com.
-                             chat(model_name) ```
+response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `GPT4ALL` -
+ chat offline with Language models using gpt4all from webscout ```python from
+webscout import GPT4ALL # Initialize the GPT4ALL class with your model path and
+  other optional parameters gpt4all_instance = GPT4ALL( model="path/to/your/
+        model/file", # Replace with the actual path to your model file
+  is_conversation=True, max_tokens=800, temperature=0.7, presence_penalty=0,
+frequency_penalty=1.18, top_p=0.4, intro="Hello, how can I assist you today?",
+  filepath="path/to/conversation/history/file", # Optional, for conversation
+history update_file=True, history_offset=10250, act=None # Optional, for using
+an awesome prompt as intro ) # Generate a response from the AI model response =
+gpt4all_instance.chat( prompt="What is the weather like today?", stream=False,
+ # Set to True if you want to stream the response optimizer=None, # Optional,
+    specify an optimizer if needed conversationally=False # Set to True for
+  conversationally generated responses ) # Print the generated response print
+ (response) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
+       `LLM` ```python from webscout.LLM import LLM def chat(model_name,
+     system_message="You are Jarvis"):# system prompt AI = LLM(model_name,
+ system_message) AI.chat() if __name__ == "__main__": model_name = "mistralai/
+ Mistral-7B-Instruct-v0.1" # name of the model you wish to use It supports ALL
+         text generation models on deepinfra.com. chat(model_name) ```
```

### Comparing `webscout-1.2.3/webscout.egg-info/SOURCES.txt` & `webscout-1.2.4/webscout.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 webscout/HelpingAI.py
 webscout/LLM.py
 webscout/__init__.py
 webscout/__main__.py
 webscout/cli.py
 webscout/exceptions.py
 webscout/models.py
+webscout/offlineAI.py
 webscout/utils.py
 webscout/version.py
 webscout/webscout_search.py
 webscout/webscout_search_async.py
 webscout.egg-info/PKG-INFO
 webscout.egg-info/SOURCES.txt
 webscout.egg-info/dependency_links.txt
```

