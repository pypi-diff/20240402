# Comparing `tmp/freeplay-0.3.0a4.tar.gz` & `tmp/freeplay-0.3.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay-0.3.0a4.tar", max compression
+gzip compressed data, was "freeplay-0.3.0a5.tar", max compression
```

## Comparing `freeplay-0.3.0a4.tar` & `freeplay-0.3.0a5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1064 2023-12-22 21:44:10.116316 freeplay-0.3.0a4/LICENSE
--rw-r--r--   0        0        0      884 2024-02-06 20:30:15.805586 freeplay-0.3.0a4/README.md
--rw-r--r--   0        0        0      679 2024-03-27 15:45:24.576348 freeplay-0.3.0a4/pyproject.toml
--rw-r--r--   0        0        0      346 2024-03-21 18:17:31.171724 freeplay-0.3.0a4/src/freeplay/__init__.py
--rw-r--r--   0        0        0     2331 2024-03-26 04:46:13.134641 freeplay-0.3.0a4/src/freeplay/api_support.py
--rw-r--r--   0        0        0      631 2023-12-22 21:44:10.117226 freeplay-0.3.0a4/src/freeplay/errors.py
--rw-r--r--   0        0        0     1479 2024-03-21 18:17:31.172057 freeplay-0.3.0a4/src/freeplay/freeplay.py
--rw-r--r--   0        0        0     3460 2024-03-21 18:17:31.172317 freeplay-0.3.0a4/src/freeplay/freeplay_cli.py
--rw-r--r--   0        0        0      898 2023-12-22 21:44:10.117969 freeplay-0.3.0a4/src/freeplay/llm_parameters.py
--rw-r--r--   0        0        0      384 2024-03-21 18:17:31.172587 freeplay-0.3.0a4/src/freeplay/model.py
--rw-r--r--   0        0        0        0 2024-03-21 18:17:31.172778 freeplay-0.3.0a4/src/freeplay/resources/__init__.py
--rw-r--r--   0        0        0      527 2024-03-21 18:17:31.173057 freeplay-0.3.0a4/src/freeplay/resources/customer_feedback.py
--rw-r--r--   0        0        0    12285 2024-03-26 16:54:33.403897 freeplay-0.3.0a4/src/freeplay/resources/prompts.py
--rw-r--r--   0        0        0     5412 2024-03-26 16:54:33.416725 freeplay-0.3.0a4/src/freeplay/resources/recordings.py
--rw-r--r--   0        0        0      868 2024-03-21 18:17:31.173650 freeplay-0.3.0a4/src/freeplay/resources/sessions.py
--rw-r--r--   0        0        0     1452 2024-03-21 18:17:31.173810 freeplay-0.3.0a4/src/freeplay/resources/test_runs.py
--rw-r--r--   0        0        0     4532 2024-03-21 18:17:31.174078 freeplay-0.3.0a4/src/freeplay/support.py
--rw-r--r--   0        0        0     2064 2024-03-21 18:17:31.174333 freeplay-0.3.0a4/src/freeplay/utils.py
--rw-r--r--   0        0        0     1604 1970-01-01 00:00:00.000000 freeplay-0.3.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-01-03 16:29:40.447184 freeplay-0.3.0a5/LICENSE
+-rw-r--r--   0        0        0      884 2024-01-18 21:16:28.148908 freeplay-0.3.0a5/README.md
+-rw-r--r--   0        0        0      679 2024-04-02 19:40:56.828622 freeplay-0.3.0a5/pyproject.toml
+-rw-r--r--   0        0        0      346 2024-03-21 16:21:06.233651 freeplay-0.3.0a5/src/freeplay/__init__.py
+-rw-r--r--   0        0        0     2331 2024-03-13 23:06:12.228513 freeplay-0.3.0a5/src/freeplay/api_support.py
+-rw-r--r--   0        0        0      631 2024-01-03 16:29:40.448185 freeplay-0.3.0a5/src/freeplay/errors.py
+-rw-r--r--   0        0        0     1479 2024-03-21 16:21:06.234127 freeplay-0.3.0a5/src/freeplay/freeplay.py
+-rw-r--r--   0        0        0     3460 2024-03-21 16:21:06.234580 freeplay-0.3.0a5/src/freeplay/freeplay_cli.py
+-rw-r--r--   0        0        0      898 2024-01-03 16:29:40.448980 freeplay-0.3.0a5/src/freeplay/llm_parameters.py
+-rw-r--r--   0        0        0      384 2024-03-21 16:21:06.234863 freeplay-0.3.0a5/src/freeplay/model.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:43:25.126491 freeplay-0.3.0a5/src/freeplay/py.typed
+-rw-r--r--   0        0        0        0 2024-03-21 16:21:06.234949 freeplay-0.3.0a5/src/freeplay/resources/__init__.py
+-rw-r--r--   0        0        0      527 2024-03-21 16:21:06.235095 freeplay-0.3.0a5/src/freeplay/resources/customer_feedback.py
+-rw-r--r--   0        0        0    12400 2024-04-02 19:40:41.570999 freeplay-0.3.0a5/src/freeplay/resources/prompts.py
+-rw-r--r--   0        0        0     5412 2024-03-29 20:43:16.999199 freeplay-0.3.0a5/src/freeplay/resources/recordings.py
+-rw-r--r--   0        0        0      868 2024-03-21 16:21:06.235825 freeplay-0.3.0a5/src/freeplay/resources/sessions.py
+-rw-r--r--   0        0        0     1452 2024-03-21 16:21:06.236038 freeplay-0.3.0a5/src/freeplay/resources/test_runs.py
+-rw-r--r--   0        0        0     4532 2024-03-21 16:21:06.236528 freeplay-0.3.0a5/src/freeplay/support.py
+-rw-r--r--   0        0        0     2064 2024-03-21 16:21:06.236895 freeplay-0.3.0a5/src/freeplay/utils.py
+-rw-r--r--   0        0        0     1604 1970-01-01 00:00:00.000000 freeplay-0.3.0a5/PKG-INFO
```

### Comparing `freeplay-0.3.0a4/LICENSE` & `freeplay-0.3.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a4/README.md` & `freeplay-0.3.0a5/README.md`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a4/pyproject.toml` & `freeplay-0.3.0a5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "freeplay"
-version = "0.3.0-alpha.4"
+version = "0.3.0-alpha.5"
 description = ""
 authors = ["FreePlay Engineering <engineering@freeplay.ai>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4"
```

### Comparing `freeplay-0.3.0a4/src/freeplay/api_support.py` & `freeplay-0.3.0a5/src/freeplay/api_support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a4/src/freeplay/errors.py` & `freeplay-0.3.0a5/src/freeplay/errors.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a4/src/freeplay/freeplay.py` & `freeplay-0.3.0a5/src/freeplay/freeplay.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a4/src/freeplay/freeplay_cli.py` & `freeplay-0.3.0a5/src/freeplay/freeplay_cli.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a4/src/freeplay/llm_parameters.py` & `freeplay-0.3.0a5/src/freeplay/llm_parameters.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a4/src/freeplay/resources/customer_feedback.py` & `freeplay-0.3.0a5/src/freeplay/resources/customer_feedback.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a4/src/freeplay/resources/prompts.py` & `freeplay-0.3.0a5/src/freeplay/resources/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import json
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, Optional, List, cast, Any
 
 from freeplay.errors import FreeplayConfigurationError, FreeplayClientError
@@ -69,15 +70,16 @@
 
     @staticmethod
     def __format_messages_for_flavor(
             flavor_name: str,
             messages: List[Dict[str, str]]
     ) -> List[Dict[str, str]]:
         if flavor_name == 'azure_openai_chat' or flavor_name == 'openai_chat':
-            return messages
+            # We need a deepcopy here to avoid referential equality with the llm_prompt
+            return copy.deepcopy(messages)
         elif flavor_name == 'anthropic_chat':
             messages_without_system = [message for message in messages if message['role'] != 'system']
             return messages_without_system
         raise MissingFlavorError(flavor_name)
 
     def format(
             self,
```

### Comparing `freeplay-0.3.0a4/src/freeplay/resources/recordings.py` & `freeplay-0.3.0a5/src/freeplay/resources/recordings.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a4/src/freeplay/resources/sessions.py` & `freeplay-0.3.0a5/src/freeplay/resources/sessions.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a4/src/freeplay/resources/test_runs.py` & `freeplay-0.3.0a5/src/freeplay/resources/test_runs.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a4/src/freeplay/support.py` & `freeplay-0.3.0a5/src/freeplay/support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a4/src/freeplay/utils.py` & `freeplay-0.3.0a5/src/freeplay/utils.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a4/PKG-INFO` & `freeplay-0.3.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplay
-Version: 0.3.0a4
+Version: 0.3.0a5
 Summary: 
 License: MIT
 Author: FreePlay Engineering
 Author-email: engineering@freeplay.ai
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

