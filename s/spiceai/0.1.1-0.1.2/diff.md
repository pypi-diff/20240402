# Comparing `tmp/spiceai-0.1.1.tar.gz` & `tmp/spiceai-0.1.2.tar.gz`

## Comparing `spiceai-0.1.1.tar` & `spiceai-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 spiceai-0.1.1/README.md
--rw-r--r--   0        0        0    11218 2020-02-02 00:00:00.000000 spiceai-0.1.1/tags
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 spiceai-0.1.1/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 spiceai-0.1.1/.ropeproject/globalnames
--rw-r--r--   0        0        0    33445 2020-02-02 00:00:00.000000 spiceai-0.1.1/.ropeproject/history
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 spiceai-0.1.1/scripts/run.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/__init__.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/client_manager.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/embeddings.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/errors.py
--rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/spice.py
--rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/utils.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/whisper.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/wrapped_clients.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 spiceai-0.1.1/.gitignore
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 spiceai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 spiceai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 spiceai-0.1.2/README.md
+-rw-r--r--   0        0        0    11218 2020-02-02 00:00:00.000000 spiceai-0.1.2/tags
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 spiceai-0.1.2/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 spiceai-0.1.2/.ropeproject/globalnames
+-rw-r--r--   0        0        0    33445 2020-02-02 00:00:00.000000 spiceai-0.1.2/.ropeproject/history
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 spiceai-0.1.2/scripts/run.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 spiceai-0.1.2/spice/__init__.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 spiceai-0.1.2/spice/client_manager.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 spiceai-0.1.2/spice/embeddings.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 spiceai-0.1.2/spice/errors.py
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 spiceai-0.1.2/spice/spice.py
+-rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 spiceai-0.1.2/spice/utils.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 spiceai-0.1.2/spice/whisper.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 spiceai-0.1.2/spice/wrapped_clients.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 spiceai-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.1.2/LICENSE
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 spiceai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 spiceai-0.1.2/PKG-INFO
```

### Comparing `spiceai-0.1.1/README.md` & `spiceai-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.1/tags` & `spiceai-0.1.2/tags`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.1/.github/workflows/ruff.yml` & `spiceai-0.1.2/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.1/.ropeproject/history` & `spiceai-0.1.2/.ropeproject/history`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.1/scripts/run.py` & `spiceai-0.1.2/scripts/run.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.1/spice/client_manager.py` & `spiceai-0.1.2/spice/client_manager.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.1/spice/embeddings.py` & `spiceai-0.1.2/spice/embeddings.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.1/spice/spice.py` & `spiceai-0.1.2/spice/spice.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.1/spice/utils.py` & `spiceai-0.1.2/spice/utils.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.1/spice/whisper.py` & `spiceai-0.1.2/spice/whisper.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.1/spice/wrapped_clients.py` & `spiceai-0.1.2/spice/wrapped_clients.py`

 * *Files identical despite different names*

