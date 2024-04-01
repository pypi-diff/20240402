# Comparing `tmp/ai_characters-1.3.0.tar.gz` & `tmp/ai_characters-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_characters-1.3.0.tar", last modified: Mon Apr  1 22:44:57 2024, max compression
+gzip compressed data, was "ai_characters-1.4.0.tar", last modified: Mon Apr  1 23:51:28 2024, max compression
```

## Comparing `ai_characters-1.3.0.tar` & `ai_characters-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:44:57.617547 ai_characters-1.3.0/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1066 2024-03-31 01:22:36.000000 ai_characters-1.3.0/LICENSE
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       36 2024-03-31 01:22:36.000000 ai_characters-1.3.0/MANIFEST.in
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1086 2024-04-01 22:44:57.617425 ai_characters-1.3.0/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      808 2024-03-31 01:22:36.000000 ai_characters-1.3.0/README.md
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:44:57.616797 ai_characters-1.3.0/ai_characters.egg-info/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1086 2024-04-01 22:44:57.000000 ai_characters-1.3.0/ai_characters.egg-info/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      296 2024-04-01 22:44:57.000000 ai_characters-1.3.0/ai_characters.egg-info/SOURCES.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-01 22:44:57.000000 ai_characters-1.3.0/ai_characters.egg-info/dependency_links.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       74 2024-04-01 22:44:57.000000 ai_characters-1.3.0/ai_characters.egg-info/requires.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       10 2024-04-01 22:44:57.000000 ai_characters-1.3.0/ai_characters.egg-info/top_level.txt
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:44:57.617034 ai_characters-1.3.0/aic/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     3016 2024-04-01 22:43:34.000000 ai_characters-1.3.0/aic/__init__.py
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      614 2024-04-01 00:35:05.000000 ai_characters-1.3.0/aic/agent.schema.json
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-01 22:44:57.617592 ai_characters-1.3.0/setup.cfg
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      861 2024-04-01 22:44:55.000000 ai_characters-1.3.0/setup.py
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:44:57.617259 ai_characters-1.3.0/tests/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:28:12.000000 ai_characters-1.3.0/tests/__init__.py
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      992 2024-04-01 22:35:16.000000 ai_characters-1.3.0/tests/test_aic.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 23:51:28.954839 ai_characters-1.4.0/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1066 2024-03-31 01:22:36.000000 ai_characters-1.4.0/LICENSE
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       36 2024-03-31 01:22:36.000000 ai_characters-1.4.0/MANIFEST.in
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1181 2024-04-01 23:51:28.954370 ai_characters-1.4.0/PKG-INFO
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      808 2024-03-31 01:22:36.000000 ai_characters-1.4.0/README.md
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 23:51:28.953983 ai_characters-1.4.0/ai_characters.egg-info/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1181 2024-04-01 23:51:28.000000 ai_characters-1.4.0/ai_characters.egg-info/PKG-INFO
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      296 2024-04-01 23:51:28.000000 ai_characters-1.4.0/ai_characters.egg-info/SOURCES.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-01 23:51:28.000000 ai_characters-1.4.0/ai_characters.egg-info/dependency_links.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       74 2024-04-01 23:51:28.000000 ai_characters-1.4.0/ai_characters.egg-info/requires.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       10 2024-04-01 23:51:28.000000 ai_characters-1.4.0/ai_characters.egg-info/top_level.txt
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 23:51:28.953267 ai_characters-1.4.0/aic/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     3018 2024-04-01 23:49:50.000000 ai_characters-1.4.0/aic/__init__.py
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      614 2024-04-01 00:35:05.000000 ai_characters-1.4.0/aic/agent.schema.json
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-01 23:51:28.954892 ai_characters-1.4.0/setup.cfg
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      861 2024-04-01 23:51:13.000000 ai_characters-1.4.0/setup.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 23:51:28.953698 ai_characters-1.4.0/tests/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:28:12.000000 ai_characters-1.4.0/tests/__init__.py
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      992 2024-04-01 22:35:16.000000 ai_characters-1.4.0/tests/test_aic.py
```

### Comparing `ai_characters-1.3.0/LICENSE` & `ai_characters-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_characters-1.3.0/PKG-INFO` & `ai_characters-1.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: ai_characters
-Version: 1.3.0
+Version: 1.4.0
 Summary: Client for AI Characters
-Home-page: UNKNOWN
 Author: Viacheslav Kovalevskyi
 Author-email: viacheslav@kovalevskyi.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: google-cloud-storage==2.16
+Requires-Dist: jsonschema==4.21
+Requires-Dist: aic_tools==1.0.0
+Requires-Dist: crewai==0.22
 
 # YourPackageName
 
 AICharacters (AIC) is a Python client library for service AICharacters that stores different AI characters, mostly tailored for use with Crew AI. It includes functionality to download character configurations from the service, validate them against a predefined schema, and utilize these characters in various contexts.
 
 ## Features
 
@@ -39,9 +41,7 @@
 
 character = load_character(character_id)
 
 print(character.backstory)
 ```
 
 
-
-
```

### Comparing `ai_characters-1.3.0/README.md` & `ai_characters-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_characters-1.3.0/ai_characters.egg-info/PKG-INFO` & `ai_characters-1.4.0/ai_characters.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
-Name: ai-characters
-Version: 1.3.0
+Name: ai_characters
+Version: 1.4.0
 Summary: Client for AI Characters
-Home-page: UNKNOWN
 Author: Viacheslav Kovalevskyi
 Author-email: viacheslav@kovalevskyi.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: google-cloud-storage==2.16
+Requires-Dist: jsonschema==4.21
+Requires-Dist: aic_tools==1.0.0
+Requires-Dist: crewai==0.22
 
 # YourPackageName
 
 AICharacters (AIC) is a Python client library for service AICharacters that stores different AI characters, mostly tailored for use with Crew AI. It includes functionality to download character configurations from the service, validate them against a predefined schema, and utilize these characters in various contexts.
 
 ## Features
 
@@ -39,9 +41,7 @@
 
 character = load_character(character_id)
 
 print(character.backstory)
 ```
 
 
-
-
```

### Comparing `ai_characters-1.3.0/aic/__init__.py` & `ai_characters-1.4.0/aic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         for tool_name in character.tools:
             tools.append(TOOLS[tool_name])
     return tools
 
 
 def load_agent(character_id: str, llm, goal, tools=[], allow_delegation=True, verbose=True) -> Agent:
     character = load_character(character_id)
-    tools.append(_load_agent_tools(character))
+    tools.append(**_load_agent_tools(character))
     return Agent(
         role=character.roleName,
         goal=goal,
         backstory=character.backstory,
         tools=tools,
         llm=llm,
         verbose=verbose,
```

### Comparing `ai_characters-1.3.0/aic/agent.schema.json` & `ai_characters-1.4.0/aic/agent.schema.json`

 * *Files identical despite different names*

### Comparing `ai_characters-1.3.0/setup.py` & `ai_characters-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 
 # Call the function and store the requirements list
 install_requires = read_requirements()
 
 setup(
     name='ai_characters',
-    version='1.3.0',
+    version='1.4.0',
     packages=find_packages(),
     description='Client for AI Characters',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Viacheslav Kovalevskyi',
     author_email='viacheslav@kovalevskyi.com',
     license='MIT',
```

### Comparing `ai_characters-1.3.0/tests/test_aic.py` & `ai_characters-1.4.0/tests/test_aic.py`

 * *Files identical despite different names*

