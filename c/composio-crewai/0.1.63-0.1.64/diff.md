# Comparing `tmp/composio_crewai-0.1.63.tar.gz` & `tmp/composio_crewai-0.1.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_crewai-0.1.63.tar", last modified: Mon Apr  1 14:15:01 2024, max compression
+gzip compressed data, was "composio_crewai-0.1.64.tar", last modified: Tue Apr  2 17:01:22 2024, max compression
```

## Comparing `composio_crewai-0.1.63.tar` & `composio_crewai-0.1.64.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-01 14:15:01.297590 composio_crewai-0.1.63/
--rw-r--r--   0 utkarsh    (501) staff       (20)      644 2024-04-01 14:15:01.297311 composio_crewai-0.1.63/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      142 2024-03-18 18:14:40.000000 composio_crewai-0.1.63/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-01 14:15:01.296229 composio_crewai-0.1.63/composio_crewai/
--rw-r--r--   0 utkarsh    (501) staff       (20)       89 2024-03-20 12:04:29.000000 composio_crewai-0.1.63/composio_crewai/__init__.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-01 14:15:01.297093 composio_crewai-0.1.63/composio_crewai.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      644 2024-04-01 14:15:01.000000 composio_crewai-0.1.63/composio_crewai.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      255 2024-04-01 14:15:01.000000 composio_crewai-0.1.63/composio_crewai.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-01 14:15:01.000000 composio_crewai-0.1.63/composio_crewai.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       28 2024-04-01 14:15:01.000000 composio_crewai-0.1.63/composio_crewai.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       16 2024-04-01 14:15:01.000000 composio_crewai-0.1.63/composio_crewai.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      276 2024-04-01 14:14:25.000000 composio_crewai-0.1.63/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-01 14:15:01.297646 composio_crewai-0.1.63/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-01 14:14:25.000000 composio_crewai-0.1.63/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-02 17:01:22.393541 composio_crewai-0.1.64/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3078 2024-04-02 17:01:22.393360 composio_crewai-0.1.64/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2576 2024-04-02 16:50:40.000000 composio_crewai-0.1.64/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-02 17:01:22.392362 composio_crewai-0.1.64/composio_crewai/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       89 2024-03-20 12:04:29.000000 composio_crewai-0.1.64/composio_crewai/__init__.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-02 17:01:22.393205 composio_crewai-0.1.64/composio_crewai.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3078 2024-04-02 17:01:22.000000 composio_crewai-0.1.64/composio_crewai.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      255 2024-04-02 17:01:22.000000 composio_crewai-0.1.64/composio_crewai.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-02 17:01:22.000000 composio_crewai-0.1.64/composio_crewai.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       28 2024-04-02 17:01:22.000000 composio_crewai-0.1.64/composio_crewai.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       16 2024-04-02 17:01:22.000000 composio_crewai-0.1.64/composio_crewai.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      276 2024-04-02 16:52:07.000000 composio_crewai-0.1.64/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-02 17:01:22.393594 composio_crewai-0.1.64/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-02 16:52:07.000000 composio_crewai-0.1.64/setup.py
```

### Comparing `composio_crewai-0.1.63/setup.py` & `composio_crewai-0.1.64/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_crewai",
-    version="0.1.63",
+    version="0.1.64",
     author="Himanshu",
     author_email="himanshu@composio.dev",
     description="Use Composio to get an array of tools with your CrewAI agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

