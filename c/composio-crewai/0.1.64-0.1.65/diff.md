# Comparing `tmp/composio_crewai-0.1.64.tar.gz` & `tmp/composio_crewai-0.1.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_crewai-0.1.64.tar", last modified: Tue Apr  2 17:01:22 2024, max compression
+gzip compressed data, was "composio_crewai-0.1.65.tar", last modified: Tue Apr  2 17:07:38 2024, max compression
```

## Comparing `composio_crewai-0.1.64.tar` & `composio_crewai-0.1.65.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-02 17:01:22.393541 composio_crewai-0.1.64/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3078 2024-04-02 17:01:22.393360 composio_crewai-0.1.64/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2576 2024-04-02 16:50:40.000000 composio_crewai-0.1.64/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-02 17:01:22.392362 composio_crewai-0.1.64/composio_crewai/
--rw-r--r--   0 utkarsh    (501) staff       (20)       89 2024-03-20 12:04:29.000000 composio_crewai-0.1.64/composio_crewai/__init__.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-02 17:01:22.393205 composio_crewai-0.1.64/composio_crewai.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3078 2024-04-02 17:01:22.000000 composio_crewai-0.1.64/composio_crewai.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      255 2024-04-02 17:01:22.000000 composio_crewai-0.1.64/composio_crewai.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-02 17:01:22.000000 composio_crewai-0.1.64/composio_crewai.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       28 2024-04-02 17:01:22.000000 composio_crewai-0.1.64/composio_crewai.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       16 2024-04-02 17:01:22.000000 composio_crewai-0.1.64/composio_crewai.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      276 2024-04-02 16:52:07.000000 composio_crewai-0.1.64/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-02 17:01:22.393594 composio_crewai-0.1.64/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-02 16:52:07.000000 composio_crewai-0.1.64/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-02 17:07:38.675732 composio_crewai-0.1.65/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3078 2024-04-02 17:07:38.675558 composio_crewai-0.1.65/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2576 2024-04-02 16:50:40.000000 composio_crewai-0.1.65/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-02 17:07:38.674488 composio_crewai-0.1.65/composio_crewai/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       89 2024-03-20 12:04:29.000000 composio_crewai-0.1.65/composio_crewai/__init__.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-02 17:07:38.675388 composio_crewai-0.1.65/composio_crewai.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3078 2024-04-02 17:07:38.000000 composio_crewai-0.1.65/composio_crewai.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      255 2024-04-02 17:07:38.000000 composio_crewai-0.1.65/composio_crewai.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-02 17:07:38.000000 composio_crewai-0.1.65/composio_crewai.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       28 2024-04-02 17:07:38.000000 composio_crewai-0.1.65/composio_crewai.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       16 2024-04-02 17:07:38.000000 composio_crewai-0.1.65/composio_crewai.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      276 2024-04-02 17:07:07.000000 composio_crewai-0.1.65/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-02 17:07:38.675768 composio_crewai-0.1.65/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-02 17:07:07.000000 composio_crewai-0.1.65/setup.py
```

### Comparing `composio_crewai-0.1.64/PKG-INFO` & `composio_crewai-0.1.65/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.1.64
+Version: 0.1.65
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.1.64
+Requires-Dist: composio_langchain===0.1.65
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.1.64/README.md` & `composio_crewai-0.1.65/README.md`

 * *Files identical despite different names*

### Comparing `composio_crewai-0.1.64/composio_crewai.egg-info/PKG-INFO` & `composio_crewai-0.1.65/composio_crewai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.1.64
+Version: 0.1.65
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.1.64
+Requires-Dist: composio_langchain===0.1.65
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.1.64/setup.py` & `composio_crewai-0.1.65/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_crewai",
-    version="0.1.64",
+    version="0.1.65",
     author="Himanshu",
     author_email="himanshu@composio.dev",
     description="Use Composio to get an array of tools with your CrewAI agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

