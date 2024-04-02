# Comparing `tmp/semantic_cache-0.1.0.tar.gz` & `tmp/semantic_cache-0.1.1.tar.gz`

## Comparing `semantic_cache-0.1.0.tar` & `semantic_cache-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 semantic_cache-0.1.0/.python-version
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 semantic_cache-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 semantic_cache-0.1.0/requirements.lock
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 semantic_cache-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 semantic_cache-0.1.0/src/semantic_cache/__init__.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 semantic_cache-0.1.0/src/test/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 semantic_cache-0.1.0/.gitignore
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 semantic_cache-0.1.0/README.md
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 semantic_cache-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 semantic_cache-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/.python-version
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/requirements.lock
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/.vscode/extensions.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/src/semantic_cache/__init__.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/src/test/__init__.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/README.md
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 semantic_cache-0.1.1/PKG-INFO
```

### Comparing `semantic_cache-0.1.0/requirements-dev.lock` & `semantic_cache-0.1.1/requirements-dev.lock`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 h2==4.1.0
     # via httpx
 hpack==4.0.0
     # via h2
 httpcore==1.0.5
     # via httpx
 httpx==0.27.0
+    # via httpx
     # via qdrant-client
 huggingface-hub==0.20.3
     # via fastembed
     # via tokenizers
 humanfriendly==10.0
     # via coloredlogs
 hyperframe==6.0.1
@@ -81,20 +82,19 @@
 pydantic==2.6.4
     # via qdrant-client
 pydantic-core==2.16.3
     # via pydantic
 pyyaml==6.0.1
     # via huggingface-hub
 qdrant-client==1.8.2
+    # via qdrant-client
     # via semantic-cache
 requests==2.31.0
     # via fastembed
     # via huggingface-hub
-setuptools==69.2.0
-    # via grpcio-tools
 sniffio==1.3.1
     # via anyio
     # via httpx
 sympy==1.12
     # via onnxruntime
 tokenizers==0.15.2
     # via fastembed
@@ -105,7 +105,9 @@
     # via anyio
     # via huggingface-hub
     # via pydantic
     # via pydantic-core
 urllib3==2.2.1
     # via qdrant-client
     # via requests
+setuptools==69.2.0
+    # via grpcio-tools
```

### Comparing `semantic_cache-0.1.0/requirements.lock` & `semantic_cache-0.1.1/requirements.lock`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 h2==4.1.0
     # via httpx
 hpack==4.0.0
     # via h2
 httpcore==1.0.5
     # via httpx
 httpx==0.27.0
+    # via httpx
     # via qdrant-client
 huggingface-hub==0.20.3
     # via fastembed
     # via tokenizers
 humanfriendly==10.0
     # via coloredlogs
 hyperframe==6.0.1
@@ -81,20 +82,19 @@
 pydantic==2.6.4
     # via qdrant-client
 pydantic-core==2.16.3
     # via pydantic
 pyyaml==6.0.1
     # via huggingface-hub
 qdrant-client==1.8.2
+    # via qdrant-client
     # via semantic-cache
 requests==2.31.0
     # via fastembed
     # via huggingface-hub
-setuptools==69.2.0
-    # via grpcio-tools
 sniffio==1.3.1
     # via anyio
     # via httpx
 sympy==1.12
     # via onnxruntime
 tokenizers==0.15.2
     # via fastembed
@@ -105,7 +105,9 @@
     # via anyio
     # via huggingface-hub
     # via pydantic
     # via pydantic-core
 urllib3==2.2.1
     # via qdrant-client
     # via requests
+setuptools==69.2.0
+    # via grpcio-tools
```

### Comparing `semantic_cache-0.1.0/src/semantic_cache/__init__.py` & `semantic_cache-0.1.1/src/semantic_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_cache-0.1.0/pyproject.toml` & `semantic_cache-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "semantic-cache"
-version = "0.1.0"
+version = "0.1.1"
 description = "Semantic Caching on python functions"
 authors = [{ name = "Rajaniraiyn R", email = "rajaniraiyn@gmail.com" }]
 readme = "README.md"
 requires-python = ">= 3.8"
 dependencies = ["qdrant-client[fastembed]>=1.8.2"]
 
 [build-system]
```

