# Comparing `tmp/gai-lib-0.94.tar.gz` & `tmp/gai-lib-0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gai-lib-0.94.tar", last modified: Mon Mar 25 15:22:29 2024, max compression
+gzip compressed data, was "gai-lib-0.95.tar", last modified: Tue Apr  2 15:20:45 2024, max compression
```

## Comparing `gai-lib-0.94.tar` & `gai-lib-0.95.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-03-25 15:22:29.544171 gai-lib-0.94/
--rw-r--r--   0 roylai    (1000) roylai    (1000)       57 2024-02-20 05:11:48.000000 gai-lib-0.94/MANIFEST.in
--rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-03-25 15:22:29.544171 gai-lib-0.94/PKG-INFO
--rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-03-25 15:22:26.000000 gai-lib-0.94/VERSION
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-03-25 15:22:29.534171 gai-lib-0.94/gai/
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.94/gai/__init__.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-03-25 15:22:29.534171 gai-lib-0.94/gai/common/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      930 2024-02-20 08:56:16.000000 gai-lib-0.94/gai/common/StatusListener.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1842 2024-02-20 08:56:16.000000 gai-lib-0.94/gai/common/StatusUpdater.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-20 08:56:16.000000 gai-lib-0.94/gai/common/__init__.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)       20 2024-02-20 08:56:16.000000 gai-lib-0.94/gai/common/constants.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     3188 2024-02-24 08:29:07.000000 gai-lib-0.94/gai/common/errors.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     4222 2024-02-22 17:41:30.000000 gai-lib-0.94/gai/common/file_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     5377 2024-02-20 10:00:20.000000 gai-lib-0.94/gai/common/generators_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     7950 2024-03-17 16:20:07.000000 gai-lib-0.94/gai/common/http_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1131 2024-02-20 09:56:37.000000 gai-lib-0.94/gai/common/image_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1417 2024-03-25 15:14:40.000000 gai-lib-0.94/gai/common/logging.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2712 2024-02-20 09:56:46.000000 gai-lib-0.94/gai/common/overlap_splitter.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1244 2024-02-20 09:56:53.000000 gai-lib-0.94/gai/common/sound_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     3192 2024-02-20 08:56:16.000000 gai-lib-0.94/gai/common/utils.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-03-25 15:22:29.534171 gai-lib-0.94/gai/lib/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      479 2024-02-20 10:00:58.000000 gai-lib-0.94/gai/lib/ClientBase.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     4158 2024-02-23 13:22:53.000000 gai-lib-0.94/gai/lib/GGG.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2631 2024-02-20 09:54:00.000000 gai-lib-0.94/gai/lib/ITTClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     5600 2024-02-23 16:05:13.000000 gai-lib-0.94/gai/lib/RAGClientAsync.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     8481 2024-02-25 05:19:13.000000 gai-lib-0.94/gai/lib/RAGClientSync.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2518 2024-02-20 09:55:02.000000 gai-lib-0.94/gai/lib/STTClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1724 2024-02-20 09:55:02.000000 gai-lib-0.94/gai/lib/TTSClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.94/gai/lib/__init__.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-03-25 15:22:29.534171 gai-lib-0.94/gai/lib/ttt/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      211 2024-02-19 19:45:33.000000 gai-lib-0.94/gai/lib/ttt/AnthropicChunkWrapper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1260 2024-02-19 19:45:33.000000 gai-lib-0.94/gai/lib/ttt/ChunkWrapper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)      222 2024-02-19 19:45:33.000000 gai-lib-0.94/gai/lib/ttt/OpenAIChunkWrapper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     6114 2024-03-25 14:53:27.000000 gai-lib-0.94/gai/lib/ttt/TTTClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.94/gai/lib/ttt/__init__.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-03-25 15:22:29.544171 gai-lib-0.94/gai/tools/
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1013 2024-02-22 17:41:40.000000 gai-lib-0.94/gai/tools/Chunker.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1619 2024-03-14 05:24:24.000000 gai-lib-0.94/gai/tools/Googler.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)      388 2024-02-19 19:45:33.000000 gai-lib-0.94/gai/tools/PDFConvert.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2513 2024-02-19 19:45:33.000000 gai-lib-0.94/gai/tools/Scraper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.94/gai/tools/__init__.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     3150 2024-03-17 16:29:06.000000 gai-lib-0.94/gai.yml
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-03-25 15:22:29.544171 gai-lib-0.94/gai_lib.egg-info/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-03-25 15:22:29.000000 gai-lib-0.94/gai_lib.egg-info/PKG-INFO
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1016 2024-03-25 15:22:29.000000 gai-lib-0.94/gai_lib.egg-info/SOURCES.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)        1 2024-03-25 15:22:29.000000 gai-lib-0.94/gai_lib.egg-info/dependency_links.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)      265 2024-03-25 15:22:29.000000 gai-lib-0.94/gai_lib.egg-info/entry_points.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)       88 2024-03-25 15:22:29.000000 gai-lib-0.94/gai_lib.egg-info/requires.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-03-25 15:22:29.000000 gai-lib-0.94/gai_lib.egg-info/top_level.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)      120 2024-03-25 14:35:24.000000 gai-lib-0.94/requirements.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)       38 2024-03-25 15:22:29.544171 gai-lib-0.94/setup.cfg
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2881 2024-03-25 14:35:01.000000 gai-lib-0.94/setup.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:20:45.844585 gai-lib-0.95/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       57 2024-02-20 05:11:48.000000 gai-lib-0.95/MANIFEST.in
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-02 15:20:45.844585 gai-lib-0.95/PKG-INFO
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-02 15:20:04.000000 gai-lib-0.95/VERSION
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:20:45.834585 gai-lib-0.95/gai/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.95/gai/__init__.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:20:45.834585 gai-lib-0.95/gai/common/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      930 2024-02-20 08:56:16.000000 gai-lib-0.95/gai/common/StatusListener.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1842 2024-02-20 08:56:16.000000 gai-lib-0.95/gai/common/StatusUpdater.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-20 08:56:16.000000 gai-lib-0.95/gai/common/__init__.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       20 2024-02-20 08:56:16.000000 gai-lib-0.95/gai/common/constants.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     3188 2024-02-24 08:29:07.000000 gai-lib-0.95/gai/common/errors.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     4222 2024-02-22 17:41:30.000000 gai-lib-0.95/gai/common/file_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     5369 2024-04-02 15:12:34.000000 gai-lib-0.95/gai/common/generators_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     7950 2024-03-17 16:20:07.000000 gai-lib-0.95/gai/common/http_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1131 2024-02-20 09:56:37.000000 gai-lib-0.95/gai/common/image_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1417 2024-03-25 15:14:40.000000 gai-lib-0.95/gai/common/logging.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2712 2024-02-20 09:56:46.000000 gai-lib-0.95/gai/common/overlap_splitter.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1244 2024-02-20 09:56:53.000000 gai-lib-0.95/gai/common/sound_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     3192 2024-02-20 08:56:16.000000 gai-lib-0.95/gai/common/utils.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:20:45.834585 gai-lib-0.95/gai/lib/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      479 2024-02-20 10:00:58.000000 gai-lib-0.95/gai/lib/ClientBase.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     4158 2024-02-23 13:22:53.000000 gai-lib-0.95/gai/lib/GGG.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2631 2024-02-20 09:54:00.000000 gai-lib-0.95/gai/lib/ITTClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     5600 2024-02-23 16:05:13.000000 gai-lib-0.95/gai/lib/RAGClientAsync.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     8481 2024-02-25 05:19:13.000000 gai-lib-0.95/gai/lib/RAGClientSync.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2518 2024-02-20 09:55:02.000000 gai-lib-0.95/gai/lib/STTClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1724 2024-02-20 09:55:02.000000 gai-lib-0.95/gai/lib/TTSClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.95/gai/lib/__init__.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:20:45.834585 gai-lib-0.95/gai/lib/ttt/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      211 2024-02-19 19:45:33.000000 gai-lib-0.95/gai/lib/ttt/AnthropicChunkWrapper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1260 2024-02-19 19:45:33.000000 gai-lib-0.95/gai/lib/ttt/ChunkWrapper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      222 2024-02-19 19:45:33.000000 gai-lib-0.95/gai/lib/ttt/OpenAIChunkWrapper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     6672 2024-04-02 15:18:36.000000 gai-lib-0.95/gai/lib/ttt/TTTClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.95/gai/lib/ttt/__init__.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:20:45.834585 gai-lib-0.95/gai/tools/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1013 2024-02-22 17:41:40.000000 gai-lib-0.95/gai/tools/Chunker.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1619 2024-03-14 05:24:24.000000 gai-lib-0.95/gai/tools/Googler.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      388 2024-02-19 19:45:33.000000 gai-lib-0.95/gai/tools/PDFConvert.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2513 2024-02-19 19:45:33.000000 gai-lib-0.95/gai/tools/Scraper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.95/gai/tools/__init__.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     3150 2024-03-17 16:29:06.000000 gai-lib-0.95/gai.yml
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:20:45.844585 gai-lib-0.95/gai_lib.egg-info/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-02 15:20:45.000000 gai-lib-0.95/gai_lib.egg-info/PKG-INFO
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1016 2024-04-02 15:20:45.000000 gai-lib-0.95/gai_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        1 2024-04-02 15:20:45.000000 gai-lib-0.95/gai_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      265 2024-04-02 15:20:45.000000 gai-lib-0.95/gai_lib.egg-info/entry_points.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       88 2024-04-02 15:20:45.000000 gai-lib-0.95/gai_lib.egg-info/requires.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-02 15:20:45.000000 gai-lib-0.95/gai_lib.egg-info/top_level.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      120 2024-03-25 14:35:24.000000 gai-lib-0.95/requirements.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       38 2024-04-02 15:20:45.844585 gai-lib-0.95/setup.cfg
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2881 2024-03-25 14:35:01.000000 gai-lib-0.95/setup.py
```

### Comparing `gai-lib-0.94/PKG-INFO` & `gai-lib-0.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gai-lib
-Version: 0.94
+Version: 0.95
 Author: kakkoii1337
 Author-email: kakkoii1337@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gai-lib-0.94/gai/common/StatusListener.py` & `gai-lib-0.95/gai/common/StatusListener.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/common/StatusUpdater.py` & `gai-lib-0.95/gai/common/StatusUpdater.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/common/errors.py` & `gai-lib-0.95/gai/common/errors.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/common/file_utils.py` & `gai-lib-0.95/gai/common/file_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/common/generators_utils.py` & `gai-lib-0.95/gai/common/generators_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,33 +33,33 @@
         if content:
             prompt += f"{role}: {content}"
         else:
             prompt += f"{role}:"
     return prompt
 
 # This is useful for converting text dialog to chatgpt-style dialog
-def chat_string_to_list(messages,ai_name="assistant"):
+def chat_string_to_list(messages):
     # Split the messages into lines
     lines = messages.split('\n')
 
     # Prepare the result list
     result = []
 
     # Define roles
-    roles = ['system', 'user', ai_name]
+    roles = ['system', 'user', 'assistant']
 
     # Initialize current role and content
     current_role = None
     current_content = ''
 
     # Process each line
     for line in lines:
         # Check if the line starts with a role
         for role in roles:
-            if line.startswith(role + ':'):
+            if line.lower().startswith(role + ':'):
                 # If there is any content for the current role, add it to the result
                 if current_role is not None and current_content.strip() != '':
                     result.append({'role': current_role, 'content': current_content.strip()})
                 
                 # Start a new role and content
                 current_role = role
                 current_content = line[len(role) + 1:].strip()
```

### Comparing `gai-lib-0.94/gai/common/http_utils.py` & `gai-lib-0.95/gai/common/http_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/common/image_utils.py` & `gai-lib-0.95/gai/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/common/logging.py` & `gai-lib-0.95/gai/common/logging.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/common/overlap_splitter.py` & `gai-lib-0.95/gai/common/overlap_splitter.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/common/sound_utils.py` & `gai-lib-0.95/gai/common/sound_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/common/utils.py` & `gai-lib-0.95/gai/common/utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/lib/GGG.py` & `gai-lib-0.95/gai/lib/GGG.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/lib/ITTClient.py` & `gai-lib-0.95/gai/lib/ITTClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/lib/RAGClientAsync.py` & `gai-lib-0.95/gai/lib/RAGClientAsync.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/lib/RAGClientSync.py` & `gai-lib-0.95/gai/lib/RAGClientSync.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/lib/STTClient.py` & `gai-lib-0.95/gai/lib/STTClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/lib/TTSClient.py` & `gai-lib-0.95/gai/lib/TTSClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/lib/ttt/ChunkWrapper.py` & `gai-lib-0.95/gai/lib/ttt/ChunkWrapper.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/lib/ttt/TTTClient.py` & `gai-lib-0.95/gai/lib/ttt/TTTClient.py`

 * *Files 17% similar despite different names*

```diff
@@ -78,24 +78,30 @@
         if generator == "gpt-4":
             return self.gpt_4(messages=messages, stream=stream, **generator_params)
         elif generator == "claude2-100k":
             return self.claude_2(messages=messages, stream=stream, **generator_params)
         return self.api(generator, messages, stream, **generator_params)
 
     def gpt_4(self, messages=None, stream=True, **generator_params):
-        import os
-        import openai
+        # import os
+        # import openai
+        # from openai import OpenAI
+        # from dotenv import load_dotenv
+        # load_dotenv()
+        # if not os.environ.get("OPENAI_API_KEY"):
+        #     raise Exception(
+        #         "OPENAI_API_KEY not found in environment variables")
+        #openai.api_key = os.environ["OPENAI_API_KEY"]
+
+
         from openai import OpenAI
-        from dotenv import load_dotenv
-        load_dotenv()
-        if not os.environ.get("OPENAI_API_KEY"):
-            raise Exception(
-                "OPENAI_API_KEY not found in environment variables")
-        openai.api_key = os.environ["OPENAI_API_KEY"]
-        client = OpenAI()
+        OPENAI_API_KEY = generator_params.pop("OPENAI_API_KEY", None)
+        if not OPENAI_API_KEY:
+            raise Exception("OPENAI_API_KEY not provided in generator_params")
+        client = OpenAI(api_key=OPENAI_API_KEY)
 
         if not messages:
             raise Exception("Messages not provided")
 
         def streamer(response):
             for chunk in response:
                 yield OpenAIChunkWrapper(chunk)
@@ -128,22 +134,28 @@
         if not stream:
             response.decode = lambda: response.choices[
                 0].message.content if response.choices[0].message.content else ""
             return response
         return streamer(response)
 
     def claude_2(self, messages=None, stream=True, **generator_params):
-        import os
+        # import os
+        # from anthropic import Anthropic
+        # from dotenv import load_dotenv
+        # load_dotenv()
+        # if not os.environ.get("ANTHROPIC_API_KEY"):
+        #     raise Exception(
+        #         "ANTHROPIC_API_KEY not found in environment variables")
+        # client = Anthropic()
+
         from anthropic import Anthropic
-        from dotenv import load_dotenv
-        load_dotenv()
-        if not os.environ.get("ANTHROPIC_API_KEY"):
-            raise Exception(
-                "ANTHROPIC_API_KEY not found in environment variables")
-        client = Anthropic()
+        ANTHROPIC_API_KEY = generator_params.pop("ANTHROPIC_API_KEY", None)
+        if not ANTHROPIC_API_KEY:
+            raise Exception("ANTHROPIC_API_KEY not provided in generator_params")
+        client = Anthropic(api_key=ANTHROPIC_API_KEY)
 
         if not messages:
             raise Exception("Messages not provided")
 
         def streamer(response):
             for chunk in response:
                 yield AnthropicChunkWrapper(chunk)
```

### Comparing `gai-lib-0.94/gai/tools/Chunker.py` & `gai-lib-0.95/gai/tools/Chunker.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/tools/Googler.py` & `gai-lib-0.95/gai/tools/Googler.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai/tools/Scraper.py` & `gai-lib-0.95/gai/tools/Scraper.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai.yml` & `gai-lib-0.95/gai.yml`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/gai_lib.egg-info/PKG-INFO` & `gai-lib-0.95/gai_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gai-lib
-Version: 0.94
+Version: 0.95
 Author: kakkoii1337
 Author-email: kakkoii1337@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gai-lib-0.94/gai_lib.egg-info/SOURCES.txt` & `gai-lib-0.95/gai_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gai-lib-0.94/setup.py` & `gai-lib-0.95/setup.py`

 * *Files identical despite different names*

