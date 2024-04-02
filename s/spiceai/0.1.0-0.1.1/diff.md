# Comparing `tmp/spiceai-0.1.0.tar.gz` & `tmp/spiceai-0.1.1.tar.gz`

## Comparing `spiceai-0.1.0.tar` & `spiceai-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,17 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 spiceai-0.1.0/README.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 spiceai-0.1.0/dev-requirements.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 spiceai-0.1.0/requirements.txt
--rw-r--r--   0        0        0    11218 2020-02-02 00:00:00.000000 spiceai-0.1.0/tags
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 spiceai-0.1.0/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 spiceai-0.1.0/.ropeproject/globalnames
--rw-r--r--   0        0        0    33445 2020-02-02 00:00:00.000000 spiceai-0.1.0/.ropeproject/history
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 spiceai-0.1.0/scripts/run.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 spiceai-0.1.0/spice/__init__.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 spiceai-0.1.0/spice/client_manager.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 spiceai-0.1.0/spice/embeddings.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 spiceai-0.1.0/spice/errors.py
--rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 spiceai-0.1.0/spice/spice.py
--rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 spiceai-0.1.0/spice/utils.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 spiceai-0.1.0/spice/whisper.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 spiceai-0.1.0/spice/wrapped_clients.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 spiceai-0.1.0/.gitignore
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 spiceai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 spiceai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 spiceai-0.1.1/README.md
+-rw-r--r--   0        0        0    11218 2020-02-02 00:00:00.000000 spiceai-0.1.1/tags
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 spiceai-0.1.1/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 spiceai-0.1.1/.ropeproject/globalnames
+-rw-r--r--   0        0        0    33445 2020-02-02 00:00:00.000000 spiceai-0.1.1/.ropeproject/history
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 spiceai-0.1.1/scripts/run.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/__init__.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/client_manager.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/embeddings.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/errors.py
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/spice.py
+-rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/utils.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/whisper.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 spiceai-0.1.1/spice/wrapped_clients.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 spiceai-0.1.1/.gitignore
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 spiceai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 spiceai-0.1.1/PKG-INFO
```

### Comparing `spiceai-0.1.0/README.md` & `spiceai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.0/tags` & `spiceai-0.1.1/tags`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.0/.github/workflows/ruff.yml` & `spiceai-0.1.1/.github/workflows/ruff.yml`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: install reqs
         run: |
           curl -LsSf https://astral.sh/uv/install.sh | sh
           uv venv
-          uv pip install -r requirements.txt
-          uv pip install -r dev-requirements.txt
+          uv pip install .
+          uv pip install .[dev]
       - name: activate venv
         run: |
           . .venv/bin/activate
           echo PATH=$PATH >> $GITHUB_ENV
       - name: ruff (linter)
         run: ruff check .
       - name: ruff (formatter)
```

### Comparing `spiceai-0.1.0/.ropeproject/history` & `spiceai-0.1.1/.ropeproject/history`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.0/scripts/run.py` & `spiceai-0.1.1/scripts/run.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.0/spice/client_manager.py` & `spiceai-0.1.1/spice/client_manager.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.0/spice/embeddings.py` & `spiceai-0.1.1/spice/embeddings.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.0/spice/spice.py` & `spiceai-0.1.1/spice/spice.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.0/spice/utils.py` & `spiceai-0.1.1/spice/utils.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.0/spice/whisper.py` & `spiceai-0.1.1/spice/whisper.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.0/spice/wrapped_clients.py` & `spiceai-0.1.1/spice/wrapped_clients.py`

 * *Files identical despite different names*

