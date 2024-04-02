# Comparing `tmp/composio_autogen-0.1.63.tar.gz` & `tmp/composio_autogen-0.1.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.63.tar", last modified: Mon Apr  1 14:15:12 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.64.tar", last modified: Tue Apr  2 17:01:33 2024, max compression
```

## Comparing `composio_autogen-0.1.63.tar` & `composio_autogen-0.1.64.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-01 14:15:12.477454 composio_autogen-0.1.63/
--rw-r--r--   0 utkarsh    (501) staff       (20)      661 2024-04-01 14:15:12.477198 composio_autogen-0.1.63/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      128 2024-03-20 12:04:29.000000 composio_autogen-0.1.63/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-01 14:15:12.475854 composio_autogen-0.1.63/composio_autogen/
--rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.63/composio_autogen/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6977 2024-03-27 14:52:24.000000 composio_autogen-0.1.63/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-01 14:15:12.476917 composio_autogen-0.1.63/composio_autogen.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      661 2024-04-01 14:15:12.000000 composio_autogen-0.1.63/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-01 14:15:12.000000 composio_autogen-0.1.63/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-01 14:15:12.000000 composio_autogen-0.1.63/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       42 2024-04-01 14:15:12.000000 composio_autogen-0.1.63/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-01 14:15:12.000000 composio_autogen-0.1.63/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-01 14:14:25.000000 composio_autogen-0.1.63/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-01 14:15:12.477503 composio_autogen-0.1.63/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-01 14:14:25.000000 composio_autogen-0.1.63/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-02 17:01:33.269773 composio_autogen-0.1.64/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3309 2024-04-02 17:01:33.269556 composio_autogen-0.1.64/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.64/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-02 17:01:33.268249 composio_autogen-0.1.64/composio_autogen/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.64/composio_autogen/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     6977 2024-03-27 14:52:24.000000 composio_autogen-0.1.64/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-02 17:01:33.269334 composio_autogen-0.1.64/composio_autogen.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3309 2024-04-02 17:01:33.000000 composio_autogen-0.1.64/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-02 17:01:33.000000 composio_autogen-0.1.64/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-02 17:01:33.000000 composio_autogen-0.1.64/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       42 2024-04-02 17:01:33.000000 composio_autogen-0.1.64/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-02 17:01:33.000000 composio_autogen-0.1.64/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-02 16:52:07.000000 composio_autogen-0.1.64/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-02 17:01:33.269809 composio_autogen-0.1.64/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-02 16:52:07.000000 composio_autogen-0.1.64/setup.py
```

### Comparing `composio_autogen-0.1.63/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.64/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.63/setup.py` & `composio_autogen-0.1.64/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.63",
+    version="0.1.64",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

