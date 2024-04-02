# Comparing `tmp/vision_agent-0.0.44.tar.gz` & `tmp/vision_agent-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.0.44.tar", max compression
+gzip compressed data, was "vision_agent-0.0.45.tar", max compression
```

## Comparing `vision_agent-0.0.44.tar` & `vision_agent-0.0.45.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-04-01 22:02:10.870361 vision_agent-0.0.44/LICENSE
--rw-r--r--   0        0        0     4175 2024-04-01 22:02:10.870361 vision_agent-0.0.44/README.md
--rw-r--r--   0        0        0     2166 2024-04-01 22:02:11.458363 vision_agent-0.0.44/pyproject.toml
--rw-r--r--   0        0        0      229 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      306 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4493 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10101 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    17449 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     6151 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0       46 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/data/__init__.py
--rw-r--r--   0        0        0     5122 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/data/data.py
--rw-r--r--   0        0        0       75 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/emb/__init__.py
--rw-r--r--   0        0        0     1375 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/emb/emb.py
--rw-r--r--   0        0        0     4420 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/image_utils.py
--rw-r--r--   0        0        0       32 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     3904 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       51 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0     8438 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      235 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1416 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    23447 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7476 2024-04-01 22:02:10.882361 vision_agent-0.0.44/vision_agent/tools/video.py
--rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 vision_agent-0.0.44/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 23:22:01.202070 vision_agent-0.0.45/LICENSE
+-rw-r--r--   0        0        0     4191 2024-04-01 23:22:01.202070 vision_agent-0.0.45/README.md
+-rw-r--r--   0        0        0     2166 2024-04-01 23:22:01.746071 vision_agent-0.0.45/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4493 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10101 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    17449 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     6151 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0       46 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/data/__init__.py
+-rw-r--r--   0        0        0     5122 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/data/data.py
+-rw-r--r--   0        0        0       75 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/emb/__init__.py
+-rw-r--r--   0        0        0     1375 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/emb/emb.py
+-rw-r--r--   0        0        0     4420 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       32 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     3904 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       51 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0     8438 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      235 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1416 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    23447 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7476 2024-04-01 23:22:01.214070 vision_agent-0.0.45/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     5340 1970-01-01 00:00:00.000000 vision_agent-0.0.45/PKG-INFO
```

### Comparing `vision_agent-0.0.44/LICENSE` & `vision_agent-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/README.md` & `vision_agent-0.0.45/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -38,63 +38,62 @@
 
 ### Vision Agents
 You can interact with the agents as you would with any LLM or LMM model:
 
 ```python
 >>> import vision_agent as va
 >>> agent = VisionAgent()
->>> agent("How many apples are in this image?", image="apples.jpg")
-"There are 2 apples in the image."
+>>> agent("What percentage of the area of this jar is filled with coffee beans?", image="jar.jpg")
+"The percentage of area of the jar filled with coffee beans is 25%."
 ```
 
 To better understand how the model came up with it's answer, you can also run it in
 debug mode by passing in the verbose argument:
 
 ```python
 >>> agent = VisionAgent(verbose=True)
 ```
 
 You can also have it return the workflow it used to complete the task along with all
 the individual steps and tools to get the answer:
 
 ```python
->>> resp, workflow = agent.chat_with_workflow([{"role": "user", "content": "How many apples are in this image?"}], image="apples.jpg")
+>>> resp, workflow = agent.chat_with_workflow([{"role": "user", "content": "What percentage of the area of this jar is filled with coffee beans?"}], image="jar.jpg")
 >>> print(workflow)
-[{"task": "Count the number of apples using 'grounding_dino_'.",
-  "tool": "grounding_dino_",
-  "parameters": {"prompt": "apple", "image": "apples.jpg"},
+[{"task": "Segment the jar using 'grounding_sam_'.",
+  "tool": "grounding_sam_",
+  "parameters": {"prompt": "jar", "image": "jar.jpg"},
   "call_results": [[
     {
-      "labels": ["apple", "apple"],
-      "scores": [0.99, 0.95],
+      "labels": ["jar"],
+      "scores": [0.99],
       "bboxes": [
         [0.58, 0.2, 0.72, 0.45],
-        [0.94, 0.57, 0.98, 0.66],
-      ]
+      ],
+      "masks": "mask.png"
     }
   ]],
-  "answer": "There are 2 apples in the image.",
+  "answer": "The jar is located at [0.58, 0.2, 0.72, 0.45].",
 }]
 ```
 
 ### Tools
 There are a variety of tools for the model or the user to use. Some are executed locally
 while others are hosted for you. You can also ask an LLM directly to build a tool for
 you. For example:
 
 ```python
 >>> import vision_agent as va
 >>> llm = va.llm.OpenAILLM()
->>> detector = llm.generate_detector("Can you build an apple detector for me?")
->>> detector("apples.jpg")
-[{"labels": ["apple", "apple"],
-  "scores": [0.99, 0.95],
+>>> detector = llm.generate_detector("Can you build a jar detector for me?")
+>>> detector("jar.jpg")
+[{"labels": ["jar",],
+  "scores": [0.99],
   "bboxes": [
     [0.58, 0.2, 0.72, 0.45],
-    [0.94, 0.57, 0.98, 0.66],
   ]
 }]
 ```
 
 | Tool | Description |
 | --- | --- |
 | CLIP | CLIP is a tool that can classify or tag any image given a set of input classes or tags. |
```

### Comparing `vision_agent-0.0.44/pyproject.toml` & `vision_agent-0.0.45/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.0.44"
+version = "0.0.45"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.0.44/vision_agent/agent/easytool.py` & `vision_agent-0.0.45/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.0.45/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/vision_agent/agent/reflexion.py` & `vision_agent-0.0.45/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.0.45/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/vision_agent/agent/vision_agent.py` & `vision_agent-0.0.45/vision_agent/agent/vision_agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.0.45/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/vision_agent/data/data.py` & `vision_agent-0.0.45/vision_agent/data/data.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/vision_agent/emb/emb.py` & `vision_agent-0.0.45/vision_agent/emb/emb.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/vision_agent/image_utils.py` & `vision_agent-0.0.45/vision_agent/image_utils.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/vision_agent/llm/llm.py` & `vision_agent-0.0.45/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/vision_agent/lmm/lmm.py` & `vision_agent-0.0.45/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/vision_agent/tools/prompts.py` & `vision_agent-0.0.45/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/vision_agent/tools/tools.py` & `vision_agent-0.0.45/vision_agent/tools/tools.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/vision_agent/tools/video.py` & `vision_agent-0.0.45/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.44/PKG-INFO` & `vision_agent-0.0.45/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.0.44
+Version: 0.0.45
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -67,63 +67,62 @@
 
 ### Vision Agents
 You can interact with the agents as you would with any LLM or LMM model:
 
 ```python
 >>> import vision_agent as va
 >>> agent = VisionAgent()
->>> agent("How many apples are in this image?", image="apples.jpg")
-"There are 2 apples in the image."
+>>> agent("What percentage of the area of this jar is filled with coffee beans?", image="jar.jpg")
+"The percentage of area of the jar filled with coffee beans is 25%."
 ```
 
 To better understand how the model came up with it's answer, you can also run it in
 debug mode by passing in the verbose argument:
 
 ```python
 >>> agent = VisionAgent(verbose=True)
 ```
 
 You can also have it return the workflow it used to complete the task along with all
 the individual steps and tools to get the answer:
 
 ```python
->>> resp, workflow = agent.chat_with_workflow([{"role": "user", "content": "How many apples are in this image?"}], image="apples.jpg")
+>>> resp, workflow = agent.chat_with_workflow([{"role": "user", "content": "What percentage of the area of this jar is filled with coffee beans?"}], image="jar.jpg")
 >>> print(workflow)
-[{"task": "Count the number of apples using 'grounding_dino_'.",
-  "tool": "grounding_dino_",
-  "parameters": {"prompt": "apple", "image": "apples.jpg"},
+[{"task": "Segment the jar using 'grounding_sam_'.",
+  "tool": "grounding_sam_",
+  "parameters": {"prompt": "jar", "image": "jar.jpg"},
   "call_results": [[
     {
-      "labels": ["apple", "apple"],
-      "scores": [0.99, 0.95],
+      "labels": ["jar"],
+      "scores": [0.99],
       "bboxes": [
         [0.58, 0.2, 0.72, 0.45],
-        [0.94, 0.57, 0.98, 0.66],
-      ]
+      ],
+      "masks": "mask.png"
     }
   ]],
-  "answer": "There are 2 apples in the image.",
+  "answer": "The jar is located at [0.58, 0.2, 0.72, 0.45].",
 }]
 ```
 
 ### Tools
 There are a variety of tools for the model or the user to use. Some are executed locally
 while others are hosted for you. You can also ask an LLM directly to build a tool for
 you. For example:
 
 ```python
 >>> import vision_agent as va
 >>> llm = va.llm.OpenAILLM()
->>> detector = llm.generate_detector("Can you build an apple detector for me?")
->>> detector("apples.jpg")
-[{"labels": ["apple", "apple"],
-  "scores": [0.99, 0.95],
+>>> detector = llm.generate_detector("Can you build a jar detector for me?")
+>>> detector("jar.jpg")
+[{"labels": ["jar",],
+  "scores": [0.99],
   "bboxes": [
     [0.58, 0.2, 0.72, 0.45],
-    [0.94, 0.57, 0.98, 0.66],
   ]
 }]
 ```
 
 | Tool | Description |
 | --- | --- |
 | CLIP | CLIP is a tool that can classify or tag any image given a set of input classes or tags. |
```

