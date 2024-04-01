# Comparing `tmp/gronckle-0.0.2.tar.gz` & `tmp/gronckle-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gronckle-0.0.2.tar", last modified: Mon Apr  1 19:23:24 2024, max compression
+gzip compressed data, was "gronckle-0.0.3.tar", last modified: Mon Apr  1 22:21:58 2024, max compression
```

## Comparing `gronckle-0.0.2.tar` & `gronckle-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:24.320340 gronckle-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 19:23:19.000000 gronckle-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-01 19:23:24.316340 gronckle-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-01 19:23:19.000000 gronckle-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:24.316340 gronckle-0.0.2/gronckle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:19.000000 gronckle-0.0.2/gronckle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:19.000000 gronckle-0.0.2/gronckle/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:24.316340 gronckle-0.0.2/gronckle/rag/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:24.316340 gronckle-0.0.2/gronckle/rag/smart_chunking/
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-01 19:23:19.000000 gronckle-0.0.2/gronckle/rag/smart_chunking/demo_streamlit_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-01 19:23:19.000000 gronckle-0.0.2/gronckle/rag/smart_chunking/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-01 19:23:19.000000 gronckle-0.0.2/gronckle/rag/smart_chunking/split_text_responsibly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-01 19:23:19.000000 gronckle-0.0.2/gronckle/rag/smart_chunking/text_splitter_prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:24.316340 gronckle-0.0.2/gronckle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-01 19:23:24.000000 gronckle-0.0.2/gronckle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-01 19:23:24.000000 gronckle-0.0.2/gronckle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:23:24.000000 gronckle-0.0.2/gronckle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 19:23:24.000000 gronckle-0.0.2/gronckle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-01 19:23:19.000000 gronckle-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:23:24.320340 gronckle-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:58.989254 gronckle-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 22:21:52.000000 gronckle-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-01 22:21:58.989254 gronckle-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-01 22:21:52.000000 gronckle-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:58.989254 gronckle-0.0.3/gronckle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:52.000000 gronckle-0.0.3/gronckle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:52.000000 gronckle-0.0.3/gronckle/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:58.989254 gronckle-0.0.3/gronckle/rag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:58.989254 gronckle-0.0.3/gronckle/rag/smart_chunking/
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-01 22:21:52.000000 gronckle-0.0.3/gronckle/rag/smart_chunking/demo_streamlit_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-01 22:21:52.000000 gronckle-0.0.3/gronckle/rag/smart_chunking/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-01 22:21:52.000000 gronckle-0.0.3/gronckle/rag/smart_chunking/split_text_responsibly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-01 22:21:52.000000 gronckle-0.0.3/gronckle/rag/smart_chunking/text_splitter_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:58.989254 gronckle-0.0.3/gronckle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-01 22:21:58.000000 gronckle-0.0.3/gronckle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-01 22:21:58.000000 gronckle-0.0.3/gronckle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:21:58.000000 gronckle-0.0.3/gronckle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 22:21:58.000000 gronckle-0.0.3/gronckle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-01 22:21:56.000000 gronckle-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:21:58.989254 gronckle-0.0.3/setup.cfg
```

### Comparing `gronckle-0.0.2/LICENSE` & `gronckle-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gronckle-0.0.2/PKG-INFO` & `gronckle-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gronckle
-Version: 0.0.2
+Version: 0.0.3
 Summary: Quality of content LLM application infrastructure
 Author-email: Griffin Clark <griffin@lionsentry.com>
 Project-URL: Homepage, https://pypi.org/project/gronckle/
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gronckle-0.0.2/README.md` & `gronckle-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gronckle-0.0.2/gronckle/rag/smart_chunking/demo_streamlit_app.py` & `gronckle-0.0.3/gronckle/rag/smart_chunking/demo_streamlit_app.py`

 * *Files identical despite different names*

### Comparing `gronckle-0.0.2/gronckle/rag/smart_chunking/main.py` & `gronckle-0.0.3/gronckle/rag/smart_chunking/main.py`

 * *Files identical despite different names*

### Comparing `gronckle-0.0.2/gronckle/rag/smart_chunking/split_text_responsibly.py` & `gronckle-0.0.3/gronckle/rag/smart_chunking/split_text_responsibly.py`

 * *Files identical despite different names*

### Comparing `gronckle-0.0.2/gronckle/rag/smart_chunking/text_splitter_prompt.py` & `gronckle-0.0.3/gronckle/rag/smart_chunking/text_splitter_prompt.py`

 * *Files identical despite different names*

### Comparing `gronckle-0.0.2/gronckle.egg-info/PKG-INFO` & `gronckle-0.0.3/gronckle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gronckle
-Version: 0.0.2
+Version: 0.0.3
 Summary: Quality of content LLM application infrastructure
 Author-email: Griffin Clark <griffin@lionsentry.com>
 Project-URL: Homepage, https://pypi.org/project/gronckle/
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

