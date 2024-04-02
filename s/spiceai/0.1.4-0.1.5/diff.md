# Comparing `tmp/spiceai-0.1.4.tar.gz` & `tmp/spiceai-0.1.5.tar.gz`

## Comparing `spiceai-0.1.4.tar` & `spiceai-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 spiceai-0.1.4/README.md
--rw-r--r--   0        0        0    11218 2020-02-02 00:00:00.000000 spiceai-0.1.4/tags
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 spiceai-0.1.4/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 spiceai-0.1.4/.ropeproject/globalnames
--rw-r--r--   0        0        0    33445 2020-02-02 00:00:00.000000 spiceai-0.1.4/.ropeproject/history
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 spiceai-0.1.4/scripts/run.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 spiceai-0.1.4/spice/__init__.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 spiceai-0.1.4/spice/client_manager.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 spiceai-0.1.4/spice/embeddings.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 spiceai-0.1.4/spice/errors.py
--rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 spiceai-0.1.4/spice/spice.py
--rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 spiceai-0.1.4/spice/utils.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 spiceai-0.1.4/spice/whisper.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 spiceai-0.1.4/spice/wrapped_clients.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 spiceai-0.1.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.1.4/LICENSE
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 spiceai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 spiceai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 spiceai-0.1.5/README.md
+-rw-r--r--   0        0        0    11218 2020-02-02 00:00:00.000000 spiceai-0.1.5/tags
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 spiceai-0.1.5/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 spiceai-0.1.5/.ropeproject/globalnames
+-rw-r--r--   0        0        0    33445 2020-02-02 00:00:00.000000 spiceai-0.1.5/.ropeproject/history
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 spiceai-0.1.5/scripts/run.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 spiceai-0.1.5/spice/__init__.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 spiceai-0.1.5/spice/client_manager.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 spiceai-0.1.5/spice/embeddings.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 spiceai-0.1.5/spice/errors.py
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 spiceai-0.1.5/spice/spice.py
+-rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 spiceai-0.1.5/spice/utils.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 spiceai-0.1.5/spice/whisper.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 spiceai-0.1.5/spice/wrapped_clients.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 spiceai-0.1.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.1.5/LICENSE
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 spiceai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 spiceai-0.1.5/PKG-INFO
```

### Comparing `spiceai-0.1.4/README.md` & `spiceai-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.4/tags` & `spiceai-0.1.5/tags`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.4/.github/workflows/ruff.yml` & `spiceai-0.1.5/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.4/.ropeproject/history` & `spiceai-0.1.5/.ropeproject/history`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.4/scripts/run.py` & `spiceai-0.1.5/scripts/run.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.4/spice/client_manager.py` & `spiceai-0.1.5/spice/client_manager.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.4/spice/embeddings.py` & `spiceai-0.1.5/spice/embeddings.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.4/spice/spice.py` & `spiceai-0.1.5/spice/spice.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.4/spice/utils.py` & `spiceai-0.1.5/spice/utils.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.4/spice/whisper.py` & `spiceai-0.1.5/spice/whisper.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.4/spice/wrapped_clients.py` & `spiceai-0.1.5/spice/wrapped_clients.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.4/LICENSE` & `spiceai-0.1.5/LICENSE`

 * *Files identical despite different names*

