# Comparing `tmp/neutron-ai-1.0.0b4.tar.gz` & `tmp/neutron-ai-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutron-ai-1.0.0b4.tar", last modified: Mon Apr  1 20:39:54 2024, max compression
+gzip compressed data, was "neutron-ai-1.0.0b5.tar", last modified: Tue Apr  2 15:34:51 2024, max compression
```

## Comparing `neutron-ai-1.0.0b4.tar` & `neutron-ai-1.0.0b5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:39:54.489673 neutron-ai-1.0.0b4/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-01 20:39:54.489673 neutron-ai-1.0.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:39:54.489673 neutron-ai-1.0.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-01 20:39:47.000000 neutron-ai-1.0.0b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:39:54.485673 neutron-ai-1.0.0b4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:39:54.485673 neutron-ai-1.0.0b4/src/neutron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/src/neutron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/src/neutron/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/src/neutron/interactive_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/src/neutron/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/src/neutron/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:39:54.489673 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-01 20:39:54.000000 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-01 20:39:54.000000 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:39:54.000000 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 20:39:54.000000 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 20:39:54.000000 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 20:39:54.000000 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:34:51.785672 neutron-ai-1.0.0b5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-02 15:34:41.000000 neutron-ai-1.0.0b5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-02 15:34:51.785672 neutron-ai-1.0.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-02 15:34:41.000000 neutron-ai-1.0.0b5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-02 15:34:41.000000 neutron-ai-1.0.0b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 15:34:51.789672 neutron-ai-1.0.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-02 15:34:46.000000 neutron-ai-1.0.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:34:51.785672 neutron-ai-1.0.0b5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:34:51.785672 neutron-ai-1.0.0b5/src/neutron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:34:41.000000 neutron-ai-1.0.0b5/src/neutron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-02 15:34:41.000000 neutron-ai-1.0.0b5/src/neutron/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-02 15:34:41.000000 neutron-ai-1.0.0b5/src/neutron/interactive_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-02 15:34:41.000000 neutron-ai-1.0.0b5/src/neutron/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-02 15:34:41.000000 neutron-ai-1.0.0b5/src/neutron/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:34:51.785672 neutron-ai-1.0.0b5/src/neutron_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-02 15:34:51.000000 neutron-ai-1.0.0b5/src/neutron_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-02 15:34:51.000000 neutron-ai-1.0.0b5/src/neutron_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:34:51.000000 neutron-ai-1.0.0b5/src/neutron_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-02 15:34:51.000000 neutron-ai-1.0.0b5/src/neutron_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 15:34:51.000000 neutron-ai-1.0.0b5/src/neutron_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 15:34:51.000000 neutron-ai-1.0.0b5/src/neutron_ai.egg-info/top_level.txt
```

### Comparing `neutron-ai-1.0.0b4/LICENSE.md` & `neutron-ai-1.0.0b5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b4/PKG-INFO` & `neutron-ai-1.0.0b5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutron-ai
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: AI Powered Ethical Hacking Assistant
 Home-page: https://github.com/berylliumsec/neutron
 Author: David I
 Author-email: david@berylliumsec.com
 License: BSD
 Keywords: AI,Ethical Hacking
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: torch>=1.0.1
 Requires-Dist: transformers>=4.34.0
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
 Requires-Dist: pydantic
+Requires-Dist: langchain
+Requires-Dist: regex
+Requires-Dist: argparse
+Requires-Dist: typing-extensions
 
 # Neutron
 
 Welcome to Neutron.
 
 ![Neutron](/images/neutron.png)
```

### Comparing `neutron-ai-1.0.0b4/README.md` & `neutron-ai-1.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b4/setup.py` & `neutron-ai-1.0.0b5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="neutron-ai",
-    version="1.0.0b4",
+    version="1.0.0b5",
     description="AI Powered Ethical Hacking Assistant",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="David I",
     author_email="david@berylliumsec.com",
     url="https://github.com/berylliumsec/neutron",
     classifiers=[
@@ -29,15 +29,20 @@
     },
     install_requires=[
         "torch>=1.0.1",
         "transformers>=4.34.0",
         "fastapi",
         "uvicorn",
         "pydantic",
-        # Add any other dependencies as necessary
+        "langchain",
+        "regex",
+        "argparse",
+        "typing-extensions"
+    
+
     ],
     entry_points={
         "console_scripts": [
             # Allows users to type 'neutron-client' in the command line to interact with the server
             "neutron-client=neutron.client:main",
             # Allows users to start the server by typing 'neutron-server'
             "neutron-server=neutron.server:main",
```

### Comparing `neutron-ai-1.0.0b4/src/neutron/client.py` & `neutron-ai-1.0.0b5/src/neutron/client.py`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b4/src/neutron/interactive_model.py` & `neutron-ai-1.0.0b5/src/neutron/interactive_model.py`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b4/src/neutron/server.py` & `neutron-ai-1.0.0b5/src/neutron/server.py`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b4/src/neutron/utilities.py` & `neutron-ai-1.0.0b5/src/neutron/utilities.py`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b4/src/neutron_ai.egg-info/PKG-INFO` & `neutron-ai-1.0.0b5/src/neutron_ai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutron-ai
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: AI Powered Ethical Hacking Assistant
 Home-page: https://github.com/berylliumsec/neutron
 Author: David I
 Author-email: david@berylliumsec.com
 License: BSD
 Keywords: AI,Ethical Hacking
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: torch>=1.0.1
 Requires-Dist: transformers>=4.34.0
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
 Requires-Dist: pydantic
+Requires-Dist: langchain
+Requires-Dist: regex
+Requires-Dist: argparse
+Requires-Dist: typing-extensions
 
 # Neutron
 
 Welcome to Neutron.
 
 ![Neutron](/images/neutron.png)
```

