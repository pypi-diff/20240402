# Comparing `tmp/crackerjack-0.7.8.tar.gz` & `tmp/crackerjack-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.7.8.tar", last modified: Sat Oct 14 21:27:06 2023, max compression
+gzip compressed data, was "crackerjack-0.7.9.tar", last modified: Sat Nov  4 14:26:39 2023, max compression
```

## Comparing `crackerjack-0.7.8.tar` & `crackerjack-0.7.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.7.8/LICENSE
--rw-r--r--   0        0        0     5853 2023-09-28 08:22:56.721114 crackerjack-0.7.8/README.md
--rw-r--r--   0        0        0      197 2023-10-14 21:26:31.722152 crackerjack-0.7.8/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-10-14 21:26:31.726264 crackerjack-0.7.8/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2453 2023-10-14 21:26:31.723960 crackerjack-0.7.8/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.7.8/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.7.8/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.7.8/crackerjack/__init__.py
--rw-r--r--   0        0        0     1567 2023-10-13 04:57:56.888743 crackerjack-0.7.8/crackerjack/__main__.py
--rw-r--r--   0        0        0     8478 2023-10-14 21:24:40.335058 crackerjack-0.7.8/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     2565 2023-10-14 21:26:32.792977 crackerjack-0.7.8/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     2565 2023-10-14 21:27:06.939565 crackerjack-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     7325 1970-01-01 00:00:00.000000 crackerjack-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.7.9/LICENSE
+-rw-r--r--   0        0        0     5853 2023-09-28 08:22:56.721114 crackerjack-0.7.9/README.md
+-rw-r--r--   0        0        0      197 2023-11-04 14:26:23.730744 crackerjack-0.7.9/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-11-04 14:26:23.732926 crackerjack-0.7.9/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2452 2023-11-04 14:26:23.731823 crackerjack-0.7.9/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.7.9/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      248 2023-11-04 14:25:36.771278 crackerjack-0.7.9/crackerjack/.ruff_cache/0.1.4/10355199064880463147
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.7.9/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.7.9/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1567 2023-10-13 04:57:56.888743 crackerjack-0.7.9/crackerjack/__main__.py
+-rw-r--r--   0        0        0     8152 2023-10-17 08:39:56.127703 crackerjack-0.7.9/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     2565 2023-11-04 14:26:24.821869 crackerjack-0.7.9/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     2565 2023-11-04 14:26:39.922172 crackerjack-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     7325 1970-01-01 00:00:00.000000 crackerjack-0.7.9/PKG-INFO
```

### Comparing `crackerjack-0.7.8/LICENSE` & `crackerjack-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.7.8/README.md` & `crackerjack-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.7.8/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.7.9/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.7.8/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.7.9/crackerjack/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/pdm-project/pdm
-    rev: 2.9.3  # a PDM release exposing the hook
+    rev: 2.10.0  # a PDM release exposing the hook
     hooks:
       - id: pdm-lock-check
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.5.0
     hooks:
       - id: trailing-whitespace
         name: trailing-whitspace
@@ -13,19 +13,19 @@
       - id: check-yaml
         name: check-yaml
       - id: check-toml
         name: check-toml
       - id: check-added-large-files
         name: check-added-large-files
   - repo: https://github.com/psf/black
-    rev: '23.9.1'
+    rev: '23.10.1'
     hooks:
       - id: black
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.292
+    rev: v0.1.4
     hooks:
       - id: ruff
   - repo: https://github.com/fredrikaverpil/creosote
     rev: v3.0.0
     hooks:
       - id: creosote
   - repo: https://github.com/ikamensh/flynt/
@@ -54,37 +54,37 @@
         types_or: [ python, pyi ]
         language: python
         files: \.py$
         additional_dependencies:
           - autotyping>=23.3.0
           - libcst>=0.4.9
   - repo: https://github.com/dosisod/refurb
-    rev: v1.21.0
+    rev: v1.22.1
     hooks:
       - id: refurb
   - repo: https://github.com/PyCQA/bandit
     rev: '1.7.5'
     hooks:
       - id: bandit
         args: ["-c", "pyproject.toml"]
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.331
+    rev: v1.1.334
     hooks:
       - id: pyright
   #  - repo: https://github.com/pdoc3/pdoc
   #    rev: master
   #    hooks:
   #      - id: pdoc
   #        name: pdoc
   #        entry: pdoc --html -f -o docs module1 module2 module3
   #        language_version: python3.11
   #        require_serial: true
   #        types: [ python ]
   #        always_run: true
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.292
+    rev: v0.1.4
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
-    rev: '23.9.1'
+    rev: '23.10.1'
     hooks:
       - id: black
```

### Comparing `crackerjack-0.7.8/crackerjack/__main__.py` & `crackerjack-0.7.9/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.7.8/crackerjack/crackerjack.py` & `crackerjack-0.7.9/crackerjack/crackerjack.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,17 +86,18 @@
             config_path = self.our_path / config
             pkg_config_path = self.pkg_path / config
             await pkg_config_path.touch(exist_ok=True)
             if self.pkg_path.stem == "crackerjack":
                 await config_path.write_text(await pkg_config_path.read_text())
                 continue
             config_text = await config_path.read_text()
-            await pkg_config_path.write_text(
-                config_text.replace("crackerjack", self.pkg_name)
-            )
+            if config == ".gitignore":
+                await pkg_config_path.write_text(
+                    config_text.replace("crackerjack", self.pkg_name)
+                )
             run([str(str(self.config.git_path)), "add", config])
 
     async def run_interactive(self, hook: str) -> None:
         success: bool = False
         while not success:
             fail = run(
                 [str(self.config.pre_commit_path), "run", hook.lower(), "--all-files"]
@@ -113,28 +114,22 @@
         await self.copy_configs()
         installed_pkgs = run(
             [str(str(self.config.pdm_path)), "list", "--freeze"],
             capture_output=True,
             text=True,
         ).stdout.splitlines()
         if not len([pkg for pkg in installed_pkgs if "pre-commit" in pkg]):
-            await asyncio.create_subprocess_shell(
-                f"pdm --pep582 >> {self.config.zshenv_path}"
-            )
-            await asyncio.create_subprocess_shell(f"source {self.config.zshenv_path}")
+            print('Installing "pre-commit"...')
             run([str(self.config.pdm_path), "self", "add", "keyring"])
             run([str(self.config.pdm_path), "config", "python.use_venv", "false"])
             run([str(self.config.git_path), "init"])
             run([str(self.config.git_path), "branch", "-m", "main"])
             run([str(self.config.git_path), "add", "pyproject.toml"])
-            run([str(self.config.pdm_path), "add", "-d", "pre_commit"])
-            run([str(self.config.pdm_path), "add", "-d", "pytest"])
-            run([str(self.config.pdm_path), "add", "-d", "autotyping"])
-            run([str(self.config.pre_commit_path), "install"])
             run([str(self.config.git_path), "add", "pdm.lock"])
+            run([str(self.config.pre_commit_path), "install"])
             run(
                 [
                     str(str(self.config.git_path)),
                     "config",
                     "advice.addIgnoredFile",
                     "false",
                 ]
@@ -151,19 +146,19 @@
             raise SystemExit("\nPlease configure '.crackerjack.yaml' and try again\n")
         imp_dir = self.pkg_path / "__pypackages__" / self.config.python_version / "lib"
         sys.path.append(str(imp_dir))
         self.pkg_name = underscore(self.pkg_path.stem.lower())
         self.pkg_dir = self.pkg_path / self.pkg_name
         await self.pkg_dir.mkdir(exist_ok=True)
         await aprint("\nCrackerjacking...\n")
-        if self.pkg_path.stem == "crackerjack" and options.update_precommit:
-            run([str(self.config.pre_commit_path), "autoupdate"])
         if not options.do_not_update_configs:
             await self.update_pkg_configs()
             run([str(str(self.config.pdm_path)), "install"])
+        if self.pkg_path.stem == "crackerjack" and options.update_precommit:
+            run([str(self.config.pre_commit_path), "autoupdate"])
         if options.interactive:
             for hook in ("refurb", "bandit", "pyright"):
                 await self.run_interactive(hook)
         check_all = run([str(self.config.pre_commit_path), "run", "--all-files"])
         if check_all.returncode > 0:
             check_all = run([str(self.config.pre_commit_path), "run", "--all-files"])
             if check_all.returncode > 0:
```

### Comparing `crackerjack-0.7.8/crackerjack/pyproject.toml` & `crackerjack-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 reportUnknownArgumentType = false
 reportPrivateUsage = "warning"
 pythonVersion = "3.12"
 pythonPlatform = "Darwin"
 
 [project]
 name = "Crackerjack"
-version = "0.7.7"
+version = "0.7.9"
 description = "Crackerjack code style"
 requires-python = ">=3.12"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -98,21 +98,21 @@
     "License :: OSI Approved :: BSD License",
     "Typing :: Typed",
 ]
 dependencies = [
     "click>=8.1.7",
     "aioconsole>=0.6.2",
     "inflection>=0.5.1",
-    "pdm-bump>=0.7.3",
     "autotyping>=23.3.0",
     "pre-commit>=3.4.0",
     "pytest>=7.4.2",
     "pydantic>=2.4.0",
     "aiopath>=0.7.5",
     "acb>=0.3.4",
+    "pdm-bump>=0.7.3",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `crackerjack-0.7.8/pyproject.toml` & `crackerjack-0.7.9/crackerjack/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -98,21 +98,21 @@
     "License :: OSI Approved :: BSD License",
     "Typing :: Typed",
 ]
 dependencies = [
     "click>=8.1.7",
     "aioconsole>=0.6.2",
     "inflection>=0.5.1",
-    "pdm-bump>=0.7.3",
     "autotyping>=23.3.0",
     "pre-commit>=3.4.0",
     "pytest>=7.4.2",
     "pydantic>=2.4.0",
     "aiopath>=0.7.5",
     "acb>=0.3.4",
+    "pdm-bump>=0.7.3",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `crackerjack-0.7.8/PKG-INFO` & `crackerjack-0.7.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Crackerjack
-Version: 0.7.8
+Version: 0.7.9
 Summary: Crackerjack code style
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
@@ -22,21 +22,21 @@
 Project-URL: Homepage, https://github.com/lesleslie/crackerjack
 Project-URL: Documentation, https://github.com/lesleslie/crackerjack
 Project-URL: Repository, https://github.com/lesleslie/crackerjack
 Requires-Python: >=3.12
 Requires-Dist: click>=8.1.7
 Requires-Dist: aioconsole>=0.6.2
 Requires-Dist: inflection>=0.5.1
-Requires-Dist: pdm-bump>=0.7.3
 Requires-Dist: autotyping>=23.3.0
 Requires-Dist: pre-commit>=3.4.0
 Requires-Dist: pytest>=7.4.2
 Requires-Dist: pydantic>=2.4.0
 Requires-Dist: aiopath>=0.7.5
 Requires-Dist: acb>=0.3.4
+Requires-Dist: pdm-bump>=0.7.3
 Description-Content-Type: text/markdown
 
 # Crackerjack Python
 
 [![Python: 3.11](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
```

