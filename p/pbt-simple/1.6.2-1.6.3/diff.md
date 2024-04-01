# Comparing `tmp/pbt_simple-1.6.2.tar.gz` & `tmp/pbt_simple-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbt_simple-1.6.2.tar", max compression
+gzip compressed data, was "pbt_simple-1.6.3.tar", max compression
```

## Comparing `pbt_simple-1.6.2.tar` & `pbt_simple-1.6.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2024-01-19 10:41:39.974282 pbt_simple-1.6.2/LICENSE
--rw-r--r--   0        0        0      178 2024-01-19 10:41:39.974282 pbt_simple-1.6.2/README.md
--rw-r--r--   0        0        0      931 2024-01-19 10:41:39.974282 pbt_simple-1.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/__init__.py
--rw-r--r--   0        0        0     1224 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/__main__.py
--rw-r--r--   0        0        0        0 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/commands/__init__.py
--rw-r--r--   0        0        0     2684 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/commands/build.py
--rw-r--r--   0        0        0     1550 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/commands/git.py
--rw-r--r--   0        0        0    15862 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/commands/install.py
--rw-r--r--   0        0        0     1740 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/commands/list.py
--rw-r--r--   0        0        0     6328 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/config.py
--rw-r--r--   0        0        0     5622 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/misc.py
--rw-r--r--   0        0        0        0 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/package/__init__.py
--rw-r--r--   0        0        0    11788 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/package/discovery.py
--rw-r--r--   0        0        0     3452 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/package/graph.py
--rw-r--r--   0        0        0     6853 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/package/package.py
--rw-r--r--   0        0        0        0 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/registry/__init__.py
--rw-r--r--   0        0        0     2834 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/registry/pypi.py
--rw-r--r--   0        0        0      434 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/registry/registry.py
--rw-r--r--   0        0        0        0 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/vcs/__init__.py
--rw-r--r--   0        0        0    10514 2024-01-19 10:41:39.978283 pbt_simple-1.6.2/sbt/vcs/git.py
--rw-r--r--   0        0        0     1415 1970-01-01 00:00:00.000000 pbt_simple-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-02-12 18:31:11.055159 pbt_simple-1.6.3/LICENSE
+-rw-r--r--   0        0        0      178 2024-02-12 18:31:11.055159 pbt_simple-1.6.3/README.md
+-rw-r--r--   0        0        0      931 2024-02-12 18:31:11.055159 pbt_simple-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-12 18:31:11.055159 pbt_simple-1.6.3/sbt/__init__.py
+-rw-r--r--   0        0        0     1224 2024-02-12 18:31:11.055159 pbt_simple-1.6.3/sbt/__main__.py
+-rw-r--r--   0        0        0        0 2024-02-12 18:31:11.055159 pbt_simple-1.6.3/sbt/commands/__init__.py
+-rw-r--r--   0        0        0     2684 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/commands/build.py
+-rw-r--r--   0        0        0     1550 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/commands/git.py
+-rw-r--r--   0        0        0    16123 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/commands/install.py
+-rw-r--r--   0        0        0     1740 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/commands/list.py
+-rw-r--r--   0        0        0     6328 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/config.py
+-rw-r--r--   0        0        0     5622 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/misc.py
+-rw-r--r--   0        0        0        0 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/package/__init__.py
+-rw-r--r--   0        0        0    11788 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/package/discovery.py
+-rw-r--r--   0        0        0     3452 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/package/graph.py
+-rw-r--r--   0        0        0     6853 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/package/package.py
+-rw-r--r--   0        0        0        0 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/registry/__init__.py
+-rw-r--r--   0        0        0     2834 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/registry/pypi.py
+-rw-r--r--   0        0        0      434 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/registry/registry.py
+-rw-r--r--   0        0        0        0 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/vcs/__init__.py
+-rw-r--r--   0        0        0    10514 2024-02-12 18:31:11.059159 pbt_simple-1.6.3/sbt/vcs/git.py
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 pbt_simple-1.6.3/PKG-INFO
```

### Comparing `pbt_simple-1.6.2/LICENSE` & `pbt_simple-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.6.2/pyproject.toml` & `pbt_simple-1.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "pbt-simple"
-version = "1.6.2"
+version = "1.6.3"
 description = "A simpler version of [PBT](https://github.com/binh-vu/pbt) for installing a package (and its local dependencies in editable mode) and build extension modules written in PYO3."
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "sbt" }]
 homepage = "https://github.com/binh-vu/pbt-simple"
 repository = "https://github.com/binh-vu/pbt-simple"
 
 [tool.poetry.scripts]
 sbt = 'sbt.__main__:cli'
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 orjson = "^3.9.9"
 click = "^8.1.7"
 tomlkit = "^0.12.1"
 loguru = "^0.7.2"
 semver = "^3.0.2"
 typing-extensions = "^4.8.0"
 requests = "^2.31.0"
```

### Comparing `pbt_simple-1.6.2/sbt/__main__.py` & `pbt_simple-1.6.3/sbt/__main__.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.6.2/sbt/commands/build.py` & `pbt_simple-1.6.3/sbt/commands/build.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.6.2/sbt/commands/git.py` & `pbt_simple-1.6.3/sbt/commands/git.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.6.2/sbt/commands/install.py` & `pbt_simple-1.6.3/sbt/commands/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,20 +417,29 @@
             exec(
                 "poetry lock --no-update" + (" -q" if quiet else ""),
                 cwd=pkg.location,
                 capture_stdout=False,
                 env=env,
             )
 
-    exec(
-        f"poetry install" + (" -q" if quiet else ""),
-        cwd=pkg.location,
-        capture_stdout=False,
-        env=env,
-    )
+    try:
+        exec(
+            f"poetry install" + (" -q" if quiet else ""),
+            cwd=pkg.location,
+            capture_stdout=False,
+            env=env,
+        )
+    except ExecProcessError:
+        # retry without quiet mode to print out the error.
+        exec(
+            f"poetry install",
+            cwd=pkg.location,
+            capture_stdout=False,
+            env=env,
+        )
 
 
 def get_virtualenv_environment_variables(virtualenv: Path) -> dict:
     return {
         "VIRTUAL_ENV": str(virtualenv),
         "PATH": str(virtualenv / "bin") + os.pathsep + os.environ.get("PATH", ""),
     }
```

### Comparing `pbt_simple-1.6.2/sbt/commands/list.py` & `pbt_simple-1.6.3/sbt/commands/list.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.6.2/sbt/config.py` & `pbt_simple-1.6.3/sbt/config.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.6.2/sbt/misc.py` & `pbt_simple-1.6.3/sbt/misc.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.6.2/sbt/package/discovery.py` & `pbt_simple-1.6.3/sbt/package/discovery.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.6.2/sbt/package/graph.py` & `pbt_simple-1.6.3/sbt/package/graph.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.6.2/sbt/package/package.py` & `pbt_simple-1.6.3/sbt/package/package.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.6.2/sbt/registry/pypi.py` & `pbt_simple-1.6.3/sbt/registry/pypi.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.6.2/sbt/vcs/git.py` & `pbt_simple-1.6.3/sbt/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.6.2/PKG-INFO` & `pbt_simple-1.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: pbt-simple
-Version: 1.6.2
+Version: 1.6.3
 Summary: A simpler version of [PBT](https://github.com/binh-vu/pbt) for installing a package (and its local dependencies in editable mode) and build extension modules written in PYO3.
 Home-page: https://github.com/binh-vu/pbt-simple
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
```

