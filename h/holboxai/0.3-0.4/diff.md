# Comparing `tmp/holboxai-0.3.tar.gz` & `tmp/holboxai-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holboxai-0.3.tar", last modified: Thu Mar 14 13:47:20 2024, max compression
+gzip compressed data, was "holboxai-0.4.tar", last modified: Tue Apr  2 11:19:52 2024, max compression
```

## Comparing `holboxai-0.3.tar` & `holboxai-0.4.tar`

### file list

```diff
@@ -1,9 +1,14 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-14 13:47:20.149835 holboxai-0.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      706 2024-03-14 13:47:20.149835 holboxai-0.3/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-14 13:47:20.149835 holboxai-0.3/holboxai/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      108 2024-03-14 13:45:38.461926 holboxai-0.3/holboxai/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2024-03-13 19:08:21.883272 holboxai-0.3/holboxai/file1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      196 2024-03-13 19:08:51.571247 holboxai-0.3/holboxai/file2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      244 2024-03-14 13:45:38.461926 holboxai-0.3/holboxai/file3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2024-03-13 17:29:34.327798 holboxai-0.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1607 2024-03-14 13:46:06.537901 holboxai-0.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 11:19:52.587273 holboxai-0.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2024-04-02 11:19:52.587273 holboxai-0.4/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 11:19:52.587273 holboxai-0.4/holboxai/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      287 2024-04-02 11:16:14.723187 holboxai-0.4/holboxai/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3417 2024-04-02 11:16:14.723187 holboxai-0.4/holboxai/csv_query.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4294 2024-04-02 11:16:14.723187 holboxai-0.4/holboxai/docs_query.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2024-03-13 19:08:21.883272 holboxai-0.4/holboxai/file1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      196 2024-03-13 19:08:51.571247 holboxai-0.4/holboxai/file2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      244 2024-03-14 13:45:38.461926 holboxai-0.4/holboxai/file3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1702 2024-04-02 11:16:14.723187 holboxai-0.4/holboxai/relevant_docs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1875 2024-04-02 11:16:14.723187 holboxai-0.4/holboxai/s3_reader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2024-04-02 11:16:14.723187 holboxai-0.4/holboxai/test1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2024-03-13 17:29:34.327798 holboxai-0.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1915 2024-04-02 11:19:50.727272 holboxai-0.4/setup.py
```

### Comparing `holboxai-0.3/setup.py` & `holboxai-0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from distutils.core import setup
 setup(
   name = 'holboxai',         # How you named your package folder (MyLib)
   packages = ['holboxai'],   # Chose the same as "name"
-  version = '0.3',      # Start with a small number and increase it with every change you make
+  version = '0.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'HolboxAI package',   # Give a short description about your library
+  long_description = 'Welcome to HolboxAI, a comprehensive AI package designed to enhance your data processing and creative capabilities. HolboxAI offers a range of functionalities including text-to-image generation, running textual queries on documents stored in your S3 bucket, and generating insights from natural language queries.',
   author = 'Sahil Khatri',                   # Type in your name
   author_email = 'sahil.khatri@holbox.ai',      # Type in your E-Mail
   url = 'https://github.com/springtownAdmin/holboxai',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/springtownAdmin/holboxai/archive/refs/tags/v_04.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/springtownAdmin/holboxai/archive/refs/tags/v_05.tar.gz',    # I explain this later on
   keywords = ['GenAI', 'Custom', 'holbox'],   # Keywords that define your package best
-  install_requires=[            # I get to this in a second
+  install_requires=[          
           'diffusers',
           'flask',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
```

