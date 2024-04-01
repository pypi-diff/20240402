# Comparing `tmp/ai_characters-1.1.0.tar.gz` & `tmp/ai_characters-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_characters-1.1.0.tar", last modified: Mon Apr  1 00:49:05 2024, max compression
+gzip compressed data, was "ai_characters-1.2.0.tar", last modified: Mon Apr  1 22:36:02 2024, max compression
```

## Comparing `ai_characters-1.1.0.tar` & `ai_characters-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 00:49:05.516207 ai_characters-1.1.0/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1066 2024-03-31 01:22:36.000000 ai_characters-1.1.0/LICENSE
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       36 2024-03-31 01:22:36.000000 ai_characters-1.1.0/MANIFEST.in
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1086 2024-04-01 00:49:05.516022 ai_characters-1.1.0/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      808 2024-03-31 01:22:36.000000 ai_characters-1.1.0/README.md
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 00:49:05.515508 ai_characters-1.1.0/ai_characters.egg-info/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1086 2024-04-01 00:49:05.000000 ai_characters-1.1.0/ai_characters.egg-info/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      260 2024-04-01 00:49:05.000000 ai_characters-1.1.0/ai_characters.egg-info/SOURCES.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-01 00:49:05.000000 ai_characters-1.1.0/ai_characters.egg-info/dependency_links.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       44 2024-04-01 00:49:05.000000 ai_characters-1.1.0/ai_characters.egg-info/requires.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        4 2024-04-01 00:49:05.000000 ai_characters-1.1.0/ai_characters.egg-info/top_level.txt
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 00:49:05.515833 ai_characters-1.1.0/aic/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     2635 2024-04-01 00:48:52.000000 ai_characters-1.1.0/aic/__init__.py
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      614 2024-04-01 00:35:05.000000 ai_characters-1.1.0/aic/agent.schema.json
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-01 00:49:05.516275 ai_characters-1.1.0/setup.cfg
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      861 2024-04-01 00:49:00.000000 ai_characters-1.1.0/setup.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:36:02.277756 ai_characters-1.2.0/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1066 2024-03-31 01:22:36.000000 ai_characters-1.2.0/LICENSE
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       36 2024-03-31 01:22:36.000000 ai_characters-1.2.0/MANIFEST.in
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1086 2024-04-01 22:36:02.277582 ai_characters-1.2.0/PKG-INFO
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      808 2024-03-31 01:22:36.000000 ai_characters-1.2.0/README.md
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:36:02.276349 ai_characters-1.2.0/ai_characters.egg-info/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1086 2024-04-01 22:36:02.000000 ai_characters-1.2.0/ai_characters.egg-info/PKG-INFO
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      296 2024-04-01 22:36:02.000000 ai_characters-1.2.0/ai_characters.egg-info/SOURCES.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-01 22:36:02.000000 ai_characters-1.2.0/ai_characters.egg-info/dependency_links.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       76 2024-04-01 22:36:02.000000 ai_characters-1.2.0/ai_characters.egg-info/requires.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       10 2024-04-01 22:36:02.000000 ai_characters-1.2.0/ai_characters.egg-info/top_level.txt
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:36:02.276881 ai_characters-1.2.0/aic/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     3012 2024-04-01 22:26:49.000000 ai_characters-1.2.0/aic/__init__.py
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      614 2024-04-01 00:35:05.000000 ai_characters-1.2.0/aic/agent.schema.json
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-01 22:36:02.277885 ai_characters-1.2.0/setup.cfg
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      861 2024-04-01 22:24:46.000000 ai_characters-1.2.0/setup.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:36:02.277346 ai_characters-1.2.0/tests/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:28:12.000000 ai_characters-1.2.0/tests/__init__.py
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      992 2024-04-01 22:35:16.000000 ai_characters-1.2.0/tests/test_aic.py
```

### Comparing `ai_characters-1.1.0/LICENSE` & `ai_characters-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_characters-1.1.0/PKG-INFO` & `ai_characters-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai_characters
-Version: 1.1.0
+Version: 1.2.0
 Summary: Client for AI Characters
 Home-page: UNKNOWN
 Author: Viacheslav Kovalevskyi
 Author-email: viacheslav@kovalevskyi.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ai_characters-1.1.0/README.md` & `ai_characters-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_characters-1.1.0/ai_characters.egg-info/PKG-INFO` & `ai_characters-1.2.0/ai_characters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-characters
-Version: 1.1.0
+Version: 1.2.0
 Summary: Client for AI Characters
 Home-page: UNKNOWN
 Author: Viacheslav Kovalevskyi
 Author-email: viacheslav@kovalevskyi.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ai_characters-1.1.0/aic/__init__.py` & `ai_characters-1.2.0/aic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from google.cloud import storage
 from jsonschema import validate
 from typing import List, Any
 from pkg_resources import resource_string, resource_exists
 from crewai import Agent
+from tools.datetime import get_datetime
 
 import json
 
 BUCKET_NAME="ai-characters"
-
+TOOLS = {
+    "DATETIME": get_datetime
+}
 
 class AICharacter:
     def __init__(self, version: str, roleName: str, backstory: str, tools: List[str]):
         self.version = version
         self.roleName = roleName
         self.backstory = backstory
         self.tools = tools
@@ -66,18 +69,27 @@
         backstory=backstory,
         tools=tools
     )
     
     return character
 
 
-def load_agent(character_id: str, llm, goal, tools=[], verbose=True) -> Agent:
+def _load_agent_tools(character: AICharacter) -> List[Any]:
+    tools = []
+    if character.tools is not None:
+        for tool_name in character.tools:
+            tools.append(TOOLS[tool_name])
+    return tools
+
+
+def load_agent(character_id: str, llm, goal, tools=[], allow_delegation=True, verbose=True) -> Agent:
     character = load_character(character_id)
+    tools.append(_load_agent_tools(character))
     return Agent(
         role=character.roleName,
         goal=goal,
         backstory=character.backstory,
         tools=tools,
         llm=llm,
         verbose=verbose,
-        allow_delegation=True
+        allow_delegation=allow_delegation
     )
```

### Comparing `ai_characters-1.1.0/aic/agent.schema.json` & `ai_characters-1.2.0/aic/agent.schema.json`

 * *Files identical despite different names*

### Comparing `ai_characters-1.1.0/setup.py` & `ai_characters-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 
 # Call the function and store the requirements list
 install_requires = read_requirements()
 
 setup(
     name='ai_characters',
-    version='1.1.0',
+    version='1.2.0',
     packages=find_packages(),
     description='Client for AI Characters',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Viacheslav Kovalevskyi',
     author_email='viacheslav@kovalevskyi.com',
     license='MIT',
```

