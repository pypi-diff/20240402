# Comparing `tmp/starlette_async_jinja-1.7.1.tar.gz` & `tmp/starlette_async_jinja-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_async_jinja-1.7.1.tar", last modified: Sun Mar  3 14:17:40 2024, max compression
+gzip compressed data, was "starlette_async_jinja-1.7.2.tar", last modified: Tue Apr  2 10:36:31 2024, max compression
```

## Comparing `starlette_async_jinja-1.7.1.tar` & `starlette_async_jinja-1.7.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 starlette_async_jinja-1.7.1/LICENSE
--rw-r--r--   0        0        0     1535 2024-02-26 07:33:43.485098 starlette_async_jinja-1.7.1/README.md
--rw-r--r--   0        0        0     2310 2024-03-03 14:17:40.166289 starlette_async_jinja-1.7.1/pyproject.toml
--rw-r--r--   0        0        0      211 2023-06-11 12:03:37.580220 starlette_async_jinja-1.7.1/starlette_async_jinja/__init__.py
--rw-r--r--   0        0        0     6318 2024-03-03 08:02:56.844340 starlette_async_jinja-1.7.1/starlette_async_jinja/responses.py
--rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 starlette_async_jinja-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 starlette_async_jinja-1.7.2/LICENSE
+-rw-r--r--   0        0        0     1535 2024-02-26 07:33:43.485098 starlette_async_jinja-1.7.2/README.md
+-rw-r--r--   0        0        0     2353 2024-04-02 10:36:31.651802 starlette_async_jinja-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0      211 2023-06-11 12:03:37.580220 starlette_async_jinja-1.7.2/starlette_async_jinja/__init__.py
+-rw-r--r--   0        0        0     6344 2024-03-18 08:09:07.321729 starlette_async_jinja-1.7.2/starlette_async_jinja/responses.py
+-rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 starlette_async_jinja-1.7.2/PKG-INFO
```

### Comparing `starlette_async_jinja-1.7.1/LICENSE` & `starlette_async_jinja-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_async_jinja-1.7.1/README.md` & `starlette_async_jinja-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `starlette_async_jinja-1.7.1/pyproject.toml` & `starlette_async_jinja-1.7.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 [tool.ruff]
 line-length = 88
 target-version = "py312"
 fix = true
 show-fixes = true
 output-format = "full"
 
+[tool.ruff.lint]
+ignore = [
+    "F821",
+]
+
 [tool.ruff.lint.isort]
 force-single-line = true
 
 [tool.ruff.lint.mccabe]
 max-complexity = 10
 
 [tool.ruff.lint.pydocstyle]
@@ -32,34 +37,34 @@
 
 [tool.creosote]
 paths = [
     "starlette_async_jinja",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
+    "python-ulid",
+    "autotyping",
     "pytest",
     "pdm",
-    "autotyping",
-    "python-ulid",
-    "pdm-bump",
     "pre-commit",
+    "pdm-bump",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "starlette_async_jinja",
 ]
 skips = [
-    "B113",
+    "B403",
     "B603",
+    "B113",
     "B404",
-    "B403",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "starlette_async_jinja",
 ]
@@ -80,15 +85,15 @@
 [tool.codespell]
 skip = "*/data/*"
 quiet-level = 3
 ignore-words-list = "crate,uptodate"
 
 [project]
 name = "starlette-async-jinja"
-version = "1.7.1"
+version = "1.7.2"
 description = ""
 dependencies = [
     "starlette>=0.34.0",
     "jinja2>=3.1.2",
     "jinja2-async-environment>=0.4.2",
 ]
 requires-python = ">=3.12"
```

### Comparing `starlette_async_jinja-1.7.1/starlette_async_jinja/responses.py` & `starlette_async_jinja-1.7.2/starlette_async_jinja/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,16 @@
         renderer = renderer or self.renderer
         return Markup(await renderer(template_name, **data))
 
     def generate_render_partial(self, renderer: t.Any) -> t.Any:
         return partial(self.render_block, renderer=renderer)
 
     async def renderer(self, template_name: str, **data: t.Any) -> t.Any:
-        return await (await self.get_template(template_name)).render_async(**data)
+        template = await self.get_template(template_name)
+        return await template.render_async(**data)
 
     # Fragments - https://github.com/sponsfreixes/jinja2-fragments
 
     async def render_fragment(
         self,
         template_name: str,
         block_name: str,
```

### Comparing `starlette_async_jinja-1.7.1/PKG-INFO` & `starlette_async_jinja-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette-async-jinja
-Version: 1.7.1
+Version: 1.7.2
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: FastAPI
```

