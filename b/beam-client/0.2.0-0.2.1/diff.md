# Comparing `tmp/beam_client-0.2.0.tar.gz` & `tmp/beam_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beam_client-0.2.0.tar", max compression
+gzip compressed data, was "beam_client-0.2.1.tar", max compression
```

## Comparing `beam_client-0.2.0.tar` & `beam_client-0.2.1.tar`

### file list

```diff
@@ -1,3 +1,6 @@
--rw-r--r--   0        0        0     1260 2024-03-28 17:43:21.189134 beam_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-28 17:42:56.392633 beam_client-0.2.0/src/beam/__init__.py
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 beam_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1254 2024-04-02 19:22:26.042006 beam_client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      637 2024-03-30 13:01:39.670148 beam_client-0.2.1/src/beam/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 02:07:20.445321 beam_client-0.2.1/src/beam/cli/__init__.py
+-rw-r--r--   0        0        0      461 2024-03-29 14:37:29.406725 beam_client-0.2.1/src/beam/cli/logs.py
+-rw-r--r--   0        0        0       83 2024-03-29 14:38:33.741973 beam_client-0.2.1/src/beam/cli/main.py
+-rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 beam_client-0.2.1/PKG-INFO
```

### Comparing `beam_client-0.2.0/pyproject.toml` & `beam_client-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beam-client"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["beam.cloud <support@beam.cloud>"]
 packages = [
     { include = "beam/**/*.py", from = "src" },
     { include = "beam", from = "src" },
 ]
 
@@ -25,34 +25,35 @@
 cloudpickle = "^3.0.0"
 rich = "^13.7.0"
 click = "^8.1.7"
 betterproto = {version = "^1.2.5", extras = ["compiler"]}
 protobuf = "^4.25.1"
 fastapi = "^0.109.0"
 uvicorn = "^0.27.0.post1"
+beta9 = "0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 pytest-env = "^1.1.3"
 attrs = "^22.1.0"
 docstring-parser = "^0.15"
 ruff = "^0.1.11"
 pydantic = "^2.5.3"
 
 [tool.poetry.scripts]
-beta9 = "beta9.cli.main:cli"
+beam = "beam.cli.main:cli"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 
 [tool.ruff]
 line-length = 100
 ignore-init-module-imports = true
-exclude = ["src/beta9/clients"]
+exclude = []
 src = ["src", "test", "bin"]
 
 [tool.ruff.per-file-ignores]
-"src/beta9/__init__.py" = ["F403"]
+"src/beam/__init__.py" = ["F403"]
```

### Comparing `beam_client-0.2.0/PKG-INFO` & `beam_client-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: beam-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: beam.cloud
 Author-email: support@beam.cloud
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: asgiref (>=3.7.2,<4.0.0)
 Requires-Dist: astor (>=0.8.1,<0.9.0)
+Requires-Dist: beta9 (==0.1.1)
 Requires-Dist: betterproto[compiler] (>=1.2.5,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cloudpickle (>=3.0.0,<4.0.0)
 Requires-Dist: croniter (>=1.3.7,<2.0.0)
 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: grpcio (>=1.60.0,<2.0.0)
 Requires-Dist: grpclib (>=0.4.7,<0.5.0)
```

