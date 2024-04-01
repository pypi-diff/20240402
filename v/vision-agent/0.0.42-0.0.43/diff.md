# Comparing `tmp/vision_agent-0.0.42.tar.gz` & `tmp/vision_agent-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.0.42.tar", max compression
+gzip compressed data, was "vision_agent-0.0.43.tar", max compression
```

## Comparing `vision_agent-0.0.42.tar` & `vision_agent-0.0.43.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11357 2024-04-01 20:46:10.548754 vision_agent-0.0.42/LICENSE
--rw-r--r--   0        0        0     4175 2024-04-01 20:46:10.548754 vision_agent-0.0.42/README.md
--rw-r--r--   0        0        0     2166 2024-04-01 20:46:11.104759 vision_agent-0.0.42/pyproject.toml
--rw-r--r--   0        0        0      229 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      306 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4493 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10101 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    17449 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     6151 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0       46 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/data/__init__.py
--rw-r--r--   0        0        0     5122 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/data/data.py
--rw-r--r--   0        0        0       75 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/emb/__init__.py
--rw-r--r--   0        0        0     1375 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/emb/emb.py
--rw-r--r--   0        0        0     4420 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/image_utils.py
--rw-r--r--   0        0        0       32 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     3904 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       51 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0     8438 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      235 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1416 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    23447 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7476 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/tools/video.py
--rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 vision_agent-0.0.42/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 21:55:27.829226 vision_agent-0.0.43/LICENSE
+-rw-r--r--   0        0        0     4175 2024-04-01 21:55:27.829226 vision_agent-0.0.43/README.md
+-rw-r--r--   0        0        0     2166 2024-04-01 21:55:28.405228 vision_agent-0.0.43/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4493 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10101 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    17449 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     6151 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0       46 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/data/__init__.py
+-rw-r--r--   0        0        0     5122 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/data/data.py
+-rw-r--r--   0        0        0       75 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/emb/__init__.py
+-rw-r--r--   0        0        0     1375 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/emb/emb.py
+-rw-r--r--   0        0        0     4420 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       32 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     3904 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       51 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0     8438 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      235 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1416 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0     6938 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/tools/tools.json
+-rw-r--r--   0        0        0    23747 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7476 2024-04-01 21:55:27.841226 vision_agent-0.0.43/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 vision_agent-0.0.43/PKG-INFO
```

### Comparing `vision_agent-0.0.42/LICENSE` & `vision_agent-0.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/README.md` & `vision_agent-0.0.43/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/pyproject.toml` & `vision_agent-0.0.43/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.0.42"
+version = "0.0.43"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.0.42/vision_agent/agent/easytool.py` & `vision_agent-0.0.43/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.0.43/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/vision_agent/agent/reflexion.py` & `vision_agent-0.0.43/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.0.43/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/vision_agent/agent/vision_agent.py` & `vision_agent-0.0.43/vision_agent/agent/vision_agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.0.43/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/vision_agent/data/data.py` & `vision_agent-0.0.43/vision_agent/data/data.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/vision_agent/emb/emb.py` & `vision_agent-0.0.43/vision_agent/emb/emb.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/vision_agent/image_utils.py` & `vision_agent-0.0.43/vision_agent/image_utils.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/vision_agent/llm/llm.py` & `vision_agent-0.0.43/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/vision_agent/lmm/lmm.py` & `vision_agent-0.0.43/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/vision_agent/tools/prompts.py` & `vision_agent-0.0.43/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/vision_agent/tools/tools.py` & `vision_agent-0.0.43/vision_agent/tools/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import tempfile
+import os
 from abc import ABC
 from collections import Counter as CounterClass
 from pathlib import Path
 from typing import Any, Dict, List, Tuple, Union, cast
 
 import numpy as np
 import requests
@@ -135,15 +136,15 @@
         >>> t = va.tools.GroundingDINO()
         >>> t("red line. yellow dot", "ct_scan1.jpg")
         [{'labels': ['red line', 'yellow dot'],
         'bboxes': [[0.38, 0.15, 0.59, 0.7], [0.48, 0.25, 0.69, 0.71]],
         'scores': [0.98, 0.02]}]
     """
 
-    _ENDPOINT = "https://chnicr4kes5ku77niv2zoytggq0qyqlp.lambda-url.us-east-2.on.aws"
+    _ENDPOINT = "https://soi4ewr6fjqqdf5vuss6rrilee0kumxq.lambda-url.us-east-2.on.aws"
 
     name = "grounding_dino_"
     description = "'grounding_dino_' is a tool that can detect arbitrary objects with inputs such as category names or referring expressions."
     usage = {
         "required_parameters": [
             {"name": "prompt", "type": "str"},
             {"name": "image", "type": "str"},
@@ -178,19 +179,23 @@
         Returns:
             A list of dictionaries containing the labels, scores, and bboxes. Each dictionary contains the detection result for an image.
         """
         image_size = get_image_size(image)
         image_b64 = convert_to_b64(image)
         data = {
             "prompt": prompt,
-            "images": [image_b64],
+            "images": image_b64,
+            "tool": "visual_grounding",
         }
         res = requests.post(
             self._ENDPOINT,
-            headers={"Content-Type": "application/json"},
+            headers={
+                "Content-Type": "application/json",
+                "Authorization": f"Api-Key {os.environ['BASETEN_API_KEY']}",
+            },
             json=data,
         )
         resp_json: Dict[str, Any] = res.json()
         if (
             "statusCode" in resp_json and resp_json["statusCode"] != 200
         ) or "statusCode" not in resp_json:
             _LOGGER.error(f"Request failed: {resp_json}")
@@ -226,15 +231,15 @@
         array([[0, 0, 0, ..., 0, 0, 0],
            [0, 0, 0, ..., 0, 0, 0],
            ...,
            [1, 1, 1, ..., 1, 1, 1],
            [1, 1, 1, ..., 1, 1, 1]], dtype=uint8)]}]
     """
 
-    _ENDPOINT = "https://cou5lfmus33jbddl6hoqdfbw7e0qidrw.lambda-url.us-east-2.on.aws"
+    _ENDPOINT = "https://model-owp50nlq.api.baseten.co/production/predict"
 
     name = "grounding_sam_"
     description = "'grounding_sam_' is a tool that can detect and segment arbitrary objects with inputs such as category names or referring expressions."
     usage = {
         "required_parameters": [
             {"name": "prompt", "type": "List[str]"},
             {"name": "image", "type": "str"},
@@ -270,18 +275,22 @@
             A list of dictionaries containing the labels, scores, bboxes and masks. Each dictionary contains the segmentation result for an image.
         """
         image_size = get_image_size(image)
         image_b64 = convert_to_b64(image)
         data = {
             "classes": prompt,
             "image": image_b64,
+            "tool": "visual_grounding_segment",
         }
         res = requests.post(
             self._ENDPOINT,
-            headers={"Content-Type": "application/json"},
+            headers={
+                "Content-Type": "application/json",
+                "Authorization": f"Api-Key {os.environ['BASETEN_API_KEY']}",
+            },
             json=data,
         )
         resp_json: Dict[str, Any] = res.json()
         if (
             "statusCode" in resp_json and resp_json["statusCode"] != 200
         ) or "statusCode" not in resp_json:
             _LOGGER.error(f"Request failed: {resp_json}")
```

### Comparing `vision_agent-0.0.42/vision_agent/tools/video.py` & `vision_agent-0.0.43/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.42/PKG-INFO` & `vision_agent-0.0.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.0.42
+Version: 0.0.43
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

