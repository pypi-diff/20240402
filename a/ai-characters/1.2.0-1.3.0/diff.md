# Comparing `tmp/ai_characters-1.2.0.tar.gz` & `tmp/ai_characters-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_characters-1.2.0.tar", last modified: Mon Apr  1 22:36:02 2024, max compression
+gzip compressed data, was "ai_characters-1.3.0.tar", last modified: Mon Apr  1 22:44:57 2024, max compression
```

## Comparing `ai_characters-1.2.0.tar` & `ai_characters-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:36:02.277756 ai_characters-1.2.0/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1066 2024-03-31 01:22:36.000000 ai_characters-1.2.0/LICENSE
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       36 2024-03-31 01:22:36.000000 ai_characters-1.2.0/MANIFEST.in
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1086 2024-04-01 22:36:02.277582 ai_characters-1.2.0/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      808 2024-03-31 01:22:36.000000 ai_characters-1.2.0/README.md
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:36:02.276349 ai_characters-1.2.0/ai_characters.egg-info/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1086 2024-04-01 22:36:02.000000 ai_characters-1.2.0/ai_characters.egg-info/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      296 2024-04-01 22:36:02.000000 ai_characters-1.2.0/ai_characters.egg-info/SOURCES.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-01 22:36:02.000000 ai_characters-1.2.0/ai_characters.egg-info/dependency_links.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       76 2024-04-01 22:36:02.000000 ai_characters-1.2.0/ai_characters.egg-info/requires.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       10 2024-04-01 22:36:02.000000 ai_characters-1.2.0/ai_characters.egg-info/top_level.txt
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:36:02.276881 ai_characters-1.2.0/aic/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)     3012 2024-04-01 22:26:49.000000 ai_characters-1.2.0/aic/__init__.py
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      614 2024-04-01 00:35:05.000000 ai_characters-1.2.0/aic/agent.schema.json
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-01 22:36:02.277885 ai_characters-1.2.0/setup.cfg
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      861 2024-04-01 22:24:46.000000 ai_characters-1.2.0/setup.py
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:36:02.277346 ai_characters-1.2.0/tests/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:28:12.000000 ai_characters-1.2.0/tests/__init__.py
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      992 2024-04-01 22:35:16.000000 ai_characters-1.2.0/tests/test_aic.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:44:57.617547 ai_characters-1.3.0/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1066 2024-03-31 01:22:36.000000 ai_characters-1.3.0/LICENSE
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       36 2024-03-31 01:22:36.000000 ai_characters-1.3.0/MANIFEST.in
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1086 2024-04-01 22:44:57.617425 ai_characters-1.3.0/PKG-INFO
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      808 2024-03-31 01:22:36.000000 ai_characters-1.3.0/README.md
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:44:57.616797 ai_characters-1.3.0/ai_characters.egg-info/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     1086 2024-04-01 22:44:57.000000 ai_characters-1.3.0/ai_characters.egg-info/PKG-INFO
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      296 2024-04-01 22:44:57.000000 ai_characters-1.3.0/ai_characters.egg-info/SOURCES.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-01 22:44:57.000000 ai_characters-1.3.0/ai_characters.egg-info/dependency_links.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       74 2024-04-01 22:44:57.000000 ai_characters-1.3.0/ai_characters.egg-info/requires.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       10 2024-04-01 22:44:57.000000 ai_characters-1.3.0/ai_characters.egg-info/top_level.txt
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:44:57.617034 ai_characters-1.3.0/aic/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)     3016 2024-04-01 22:43:34.000000 ai_characters-1.3.0/aic/__init__.py
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      614 2024-04-01 00:35:05.000000 ai_characters-1.3.0/aic/agent.schema.json
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-01 22:44:57.617592 ai_characters-1.3.0/setup.cfg
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      861 2024-04-01 22:44:55.000000 ai_characters-1.3.0/setup.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:44:57.617259 ai_characters-1.3.0/tests/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:28:12.000000 ai_characters-1.3.0/tests/__init__.py
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      992 2024-04-01 22:35:16.000000 ai_characters-1.3.0/tests/test_aic.py
```

### Comparing `ai_characters-1.2.0/LICENSE` & `ai_characters-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_characters-1.2.0/PKG-INFO` & `ai_characters-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai_characters
-Version: 1.2.0
+Version: 1.3.0
 Summary: Client for AI Characters
 Home-page: UNKNOWN
 Author: Viacheslav Kovalevskyi
 Author-email: viacheslav@kovalevskyi.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ai_characters-1.2.0/README.md` & `ai_characters-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_characters-1.2.0/ai_characters.egg-info/PKG-INFO` & `ai_characters-1.3.0/ai_characters.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-characters
-Version: 1.2.0
+Version: 1.3.0
 Summary: Client for AI Characters
 Home-page: UNKNOWN
 Author: Viacheslav Kovalevskyi
 Author-email: viacheslav@kovalevskyi.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ai_characters-1.2.0/aic/__init__.py` & `ai_characters-1.3.0/aic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from google.cloud import storage
 from jsonschema import validate
 from typing import List, Any
 from pkg_resources import resource_string, resource_exists
 from crewai import Agent
-from tools.datetime import get_datetime
+from aic_tools.datetime import get_datetime
 
 import json
 
 BUCKET_NAME="ai-characters"
 TOOLS = {
     "DATETIME": get_datetime
 }
```

### Comparing `ai_characters-1.2.0/aic/agent.schema.json` & `ai_characters-1.3.0/aic/agent.schema.json`

 * *Files identical despite different names*

### Comparing `ai_characters-1.2.0/setup.py` & `ai_characters-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 
 # Call the function and store the requirements list
 install_requires = read_requirements()
 
 setup(
     name='ai_characters',
-    version='1.2.0',
+    version='1.3.0',
     packages=find_packages(),
     description='Client for AI Characters',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Viacheslav Kovalevskyi',
     author_email='viacheslav@kovalevskyi.com',
     license='MIT',
```

### Comparing `ai_characters-1.2.0/tests/test_aic.py` & `ai_characters-1.3.0/tests/test_aic.py`

 * *Files identical despite different names*

