# Comparing `tmp/fastblocks-0.3.7.tar.gz` & `tmp/fastblocks-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastblocks-0.3.7.tar", last modified: Mon Mar  4 15:15:36 2024, max compression
+gzip compressed data, was "fastblocks-0.3.8.tar", last modified: Tue Apr  2 14:42:14 2024, max compression
```

## Comparing `fastblocks-0.3.7.tar` & `fastblocks-0.3.8.tar`

### file list

```diff
@@ -1,34 +1,33 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.3.7/LICENSE
--rw-r--r--   0        0        0     1024 2023-09-28 16:26:56.729322 fastblocks-0.3.7/README.md
--rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.3.7/fastblocks/Dockerfile
--rw-r--r--   0        0        0      149 2024-02-08 11:06:00.249936 fastblocks-0.3.7/fastblocks/__init__.py
--rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.3.7/fastblocks/__main__.py
--rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.3.7/fastblocks/actions/__init__.py
--rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.3.7/fastblocks/actions/minify.py
--rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.3.7/fastblocks/adapters/__init__.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.3.7/fastblocks/adapters/admin/__init__.py
--rw-r--r--   0        0        0       96 2024-02-05 00:13:09.758290 fastblocks-0.3.7/fastblocks/adapters/admin/_base.py
--rw-r--r--   0        0        0     2988 2024-02-09 12:51:23.096080 fastblocks-0.3.7/fastblocks/adapters/admin/sqladmin.py
--rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.3.7/fastblocks/adapters/app/__init__.py
--rw-r--r--   0        0        0      312 2024-02-24 10:37:18.246405 fastblocks-0.3.7/fastblocks/adapters/app/_base.py
--rw-r--r--   0        0        0     2638 2024-02-09 12:50:19.221823 fastblocks-0.3.7/fastblocks/adapters/app/main.py
--rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.3.7/fastblocks/adapters/auth/__init__.py
--rw-r--r--   0        0        0     1682 2024-02-08 21:44:35.522977 fastblocks-0.3.7/fastblocks/adapters/auth/_base.py
--rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.3.7/fastblocks/adapters/auth/basic.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.3.7/fastblocks/adapters/fonts/__init__.py
--rw-r--r--   0        0        0      222 2024-02-05 00:13:09.776789 fastblocks-0.3.7/fastblocks/adapters/fonts/_base.py
--rw-r--r--   0        0        0     1230 2024-02-05 00:13:09.786522 fastblocks-0.3.7/fastblocks/adapters/fonts/google.py
--rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.3.7/fastblocks/adapters/sitemap/__init__.py
--rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.3.7/fastblocks/adapters/sitemap/sitemap.py
--rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.3.7/fastblocks/adapters/style/__init__.py
--rw-r--r--   0        0        0     3923 2024-02-09 17:43:28.021037 fastblocks-0.3.7/fastblocks/adapters/style/_base.py
--rw-r--r--   0        0        0      118 2023-10-09 12:04:34.161212 fastblocks-0.3.7/fastblocks/adapters/style/bulma.py
--rw-r--r--   0        0        0       30 2023-11-30 20:15:46.371981 fastblocks-0.3.7/fastblocks/adapters/style/cirrus.py
--rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.3.7/fastblocks/adapters/templates/__init__.py
--rw-r--r--   0        0        0      332 2024-03-03 09:36:13.663071 fastblocks-0.3.7/fastblocks/adapters/templates/_base.py
--rw-r--r--   0        0        0      758 2023-10-13 23:22:41.140320 fastblocks-0.3.7/fastblocks/adapters/templates/_filters.py
--rw-r--r--   0        0        0    14759 2024-03-04 14:04:06.525893 fastblocks-0.3.7/fastblocks/adapters/templates/jinja2.py
--rw-r--r--   0        0        0     3785 2024-02-09 11:38:52.591481 fastblocks-0.3.7/fastblocks/applications.py
--rw-r--r--   0        0        0     3056 2024-03-04 14:52:11.154976 fastblocks-0.3.7/fastblocks/middleware.py
--rw-r--r--   0        0        0     3009 2024-03-04 15:15:36.031132 fastblocks-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 fastblocks-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1024 2023-09-28 16:26:56.729322 fastblocks-0.3.8/README.md
+-rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.3.8/fastblocks/Dockerfile
+-rw-r--r--   0        0        0      149 2024-02-08 11:06:00.249936 fastblocks-0.3.8/fastblocks/__init__.py
+-rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.3.8/fastblocks/__main__.py
+-rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.3.8/fastblocks/actions/__init__.py
+-rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.3.8/fastblocks/actions/minify.py
+-rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.3.8/fastblocks/adapters/__init__.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.3.8/fastblocks/adapters/admin/__init__.py
+-rw-r--r--   0        0        0       96 2024-02-05 00:13:09.758290 fastblocks-0.3.8/fastblocks/adapters/admin/_base.py
+-rw-r--r--   0        0        0     2988 2024-02-09 12:51:23.096080 fastblocks-0.3.8/fastblocks/adapters/admin/sqladmin.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.3.8/fastblocks/adapters/app/__init__.py
+-rw-r--r--   0        0        0      312 2024-02-24 10:37:18.246405 fastblocks-0.3.8/fastblocks/adapters/app/_base.py
+-rw-r--r--   0        0        0     2669 2024-03-31 09:28:05.032996 fastblocks-0.3.8/fastblocks/adapters/app/main.py
+-rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.3.8/fastblocks/adapters/auth/__init__.py
+-rw-r--r--   0        0        0     1682 2024-02-08 21:44:35.522977 fastblocks-0.3.8/fastblocks/adapters/auth/_base.py
+-rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.3.8/fastblocks/adapters/auth/basic.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.3.8/fastblocks/adapters/fonts/__init__.py
+-rw-r--r--   0        0        0      222 2024-02-05 00:13:09.776789 fastblocks-0.3.8/fastblocks/adapters/fonts/_base.py
+-rw-r--r--   0        0        0     1230 2024-02-05 00:13:09.786522 fastblocks-0.3.8/fastblocks/adapters/fonts/google.py
+-rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.3.8/fastblocks/adapters/sitemap/__init__.py
+-rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.3.8/fastblocks/adapters/sitemap/sitemap.py
+-rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.3.8/fastblocks/adapters/style/__init__.py
+-rw-r--r--   0        0        0     3812 2024-03-09 09:26:05.815486 fastblocks-0.3.8/fastblocks/adapters/style/_base.py
+-rw-r--r--   0        0        0      118 2024-03-09 09:10:00.894074 fastblocks-0.3.8/fastblocks/adapters/style/bulma.py
+-rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.3.8/fastblocks/adapters/templates/__init__.py
+-rw-r--r--   0        0        0      332 2024-03-03 09:36:13.663071 fastblocks-0.3.8/fastblocks/adapters/templates/_base.py
+-rw-r--r--   0        0        0      758 2023-10-13 23:22:41.140320 fastblocks-0.3.8/fastblocks/adapters/templates/_filters.py
+-rw-r--r--   0        0        0    14759 2024-03-04 14:04:06.525893 fastblocks-0.3.8/fastblocks/adapters/templates/jinja2.py
+-rw-r--r--   0        0        0     3848 2024-03-29 16:08:40.512632 fastblocks-0.3.8/fastblocks/applications.py
+-rw-r--r--   0        0        0     3056 2024-03-04 14:52:11.154976 fastblocks-0.3.8/fastblocks/middleware.py
+-rw-r--r--   0        0        0     3052 2024-04-02 14:42:14.906140 fastblocks-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 fastblocks-0.3.8/PKG-INFO
```

### Comparing `fastblocks-0.3.7/LICENSE` & `fastblocks-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.7/README.md` & `fastblocks-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.7/fastblocks/adapters/admin/sqladmin.py` & `fastblocks-0.3.8/fastblocks/adapters/admin/sqladmin.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.7/fastblocks/adapters/app/main.py` & `fastblocks-0.3.8/fastblocks/adapters/app/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,11 +73,12 @@
 
         await post_startup()
         main_start_time = perf_counter() - main_start
         self.logger.info(f"App started in {main_start_time} s")
         yield
         await cache.close()
         self.logger.error("Application shut down")
+        self.logger.complete()
 
 
 depends.set(App)
 app = depends.get(App)
```

### Comparing `fastblocks-0.3.7/fastblocks/adapters/auth/_base.py` & `fastblocks-0.3.8/fastblocks/adapters/auth/_base.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.7/fastblocks/adapters/fonts/google.py` & `fastblocks-0.3.8/fastblocks/adapters/fonts/google.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.7/fastblocks/adapters/sitemap/sitemap.py` & `fastblocks-0.3.8/fastblocks/adapters/sitemap/sitemap.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.7/fastblocks/adapters/style/_base.py` & `fastblocks-0.3.8/fastblocks/adapters/style/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from contextlib import closing
 from io import StringIO
 from string import hexdigits
 
-from acb import depends
+from acb.depends import depends
 from acb.actions.encode import load
+from acb.adapters import AdapterBase
 from acb.adapters import import_adapter
-from acb.config import Config
 from acb.config import Settings
 from acb.debug import debug
 from colour import web2hex  # type: ignore
 
 from aiopath import AsyncPath
 from asgi_htmx import HtmxRequest
 from fastblocks.actions.minify import minify
 
 
-Logger = import_adapter()
 Cache = import_adapter()
 Templates = import_adapter()
 
 
 class StyleBaseSettings(Settings): ...
 
 
-class StyleBase:
+class StyleBase(AdapterBase):
     cache: Cache = depends()  # type: ignore
-    logger: Logger = depends()  # type: ignore
-    config: Config = depends()  # type: ignore
     templates: Templates = depends()  # type: ignore
 
     @staticmethod
     def get_hex_color(color: str | int | None) -> str:
         if not color:
             return ""
         if str(color) == "0":
@@ -65,15 +62,15 @@
                 remove.append(k)
                 self.logger.debug(f"\tremoving old sass variable {k!r}")
         # pprint(remove)
         for r in remove:
             del new_sass[r]
         return new_sass
 
-    @cache(expire=config.cache.default_timeout)  # type: ignore
+    @cache()  # type: ignore
     async def render_inline(self, path: AsyncPath, request: HtmxRequest) -> str:
         with closing(StringIO()) as res:
             if self.config.deployed:
                 default_yml = await self.templates.render_template(
                     path.name, request["context"]
                 )
             else:
@@ -97,10 +94,10 @@
                     [self.config.style.scss_path / self.config.style.theme_path]
                 )
             for sass in scss:
                 res.write(f"\n@import {sass!r};\n")
             res = res.getvalue()
         if self.config.debug.css:
             self.logger.debug(f"Style for {path.parent.parent}:\n{res}")
-        # if not site.is_deployed or debug.production:
+        # if not self.config.deployed or self.config.debug.production:
         res = minify.scss(res)
         return res
```

### Comparing `fastblocks-0.3.7/fastblocks/adapters/templates/_filters.py` & `fastblocks-0.3.8/fastblocks/adapters/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.7/fastblocks/adapters/templates/jinja2.py` & `fastblocks-0.3.8/fastblocks/adapters/templates/jinja2.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.7/fastblocks/applications.py` & `fastblocks-0.3.8/fastblocks/applications.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from platform import system
 
 from acb.adapters import import_adapter
 from acb.adapters import register_adapters
 from acb.adapters.logger.loguru import InterceptHandler
 from acb.config import Config
 from acb.depends import depends
-
 from asgi_htmx import HtmxRequest
 from starception import add_link_template
 from starception import install_error_handler
 from starception import set_editor
 from starlette.applications import Starlette
 from starlette.authentication import UnauthenticatedUser
 from starlette.middleware import Middleware
@@ -24,18 +23,23 @@
 from starlette.types import Lifespan
 from .middleware import middlewares
 
 register_adapters()
 
 Logger = import_adapter()
 
-current_user: ContextVar[t.Any] = ContextVar(
+_current_user: ContextVar[t.Any] = ContextVar(
     "current_user", default=UnauthenticatedUser()
 )
 
+
+def current_user() -> t.Any:
+    return _current_user.get()
+
+
 AppType = t.TypeVar("AppType", bound="FastBlocks")
 
 match system():
     case "Windows":
         add_link_template("pycharm", "pycharm64.exe --line {lineno} {path}")
     case "Darwin":
         add_link_template("pycharm", "pycharm --line {lineno} {path}")
```

### Comparing `fastblocks-0.3.7/fastblocks/middleware.py` & `fastblocks-0.3.8/fastblocks/middleware.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.7/pyproject.toml` & `fastblocks-0.3.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fastblocks"
-version = "0.3.7"
+version = "0.3.8"
 description = "Starlette based app for the rapid delivery HTMX/Jinja template blocks"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
@@ -82,14 +82,19 @@
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
@@ -102,37 +107,37 @@
 
 [tool.creosote]
 paths = [
     "fastblocks",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
-    "libsass",
-    "phonenumbers",
-    "pre-commit",
-    "pdm",
-    "aiohttp",
     "autotyping",
     "pdm-bump",
-    "pyfiglet",
+    "pre-commit",
+    "aiohttp",
+    "pdm",
+    "libsass",
     "pytest",
+    "pyfiglet",
+    "phonenumbers",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "fastblocks",
 ]
 skips = [
-    "B403",
+    "B113",
     "B404",
+    "B403",
     "B603",
-    "B113",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "fastblocks",
 ]
```

### Comparing `fastblocks-0.3.7/PKG-INFO` & `fastblocks-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastblocks
-Version: 0.3.7
+Version: 0.3.8
 Summary: Starlette based app for the rapid delivery HTMX/Jinja template blocks
 Keywords: starlette htmx jinja httpx fastapi sqladmin sqlmodel pydantic sqlalchemy redis
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
```

