# Comparing `tmp/vite_to_flask-0.1.0.tar.gz` & `tmp/vite_to_flask-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vite_to_flask-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vite_to_flask-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vite_to_flask-0.1.0.tar` & `vite_to_flask-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,28 @@
--rw-r--r--   0        0        0     5165 2024-04-01 18:22:01.196818 vite_to_flask-0.1.0/.gitignore
--rw-r--r--   0        0        0      239 2024-03-30 20:33:17.290703 vite_to_flask-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0     5449 2024-03-30 20:33:16.318189 vite_to_flask-0.1.0/.idea/copilot/chatSessions/00000000000.xd
--rw-r--r--   0        0        0        4 2024-03-30 20:33:15.306027 vite_to_flask-0.1.0/.idea/copilot/chatSessions/blobs/version
--rw-r--r--   0        0        0    18014 2024-03-30 20:33:15.298186 vite_to_flask-0.1.0/.idea/copilot/chatSessions/xd.lck
--rw-r--r--   0        0        0     1170 2024-03-30 20:33:16.417920 vite_to_flask-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2024-03-30 20:33:16.531904 vite_to_flask-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      310 2024-03-30 20:42:06.566945 vite_to_flask-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      278 2024-03-30 20:33:16.465951 vite_to_flask-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      180 2024-03-30 20:33:16.525195 vite_to_flask-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0      690 2024-04-01 19:20:16.111160 vite_to_flask-0.1.0/.idea/vite-to-flask.iml
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_to_flask-0.1.0/LICENSE
--rw-r--r--   0        0        0     2485 2024-04-01 21:07:42.721942 vite_to_flask-0.1.0/README.md
--rw-r--r--   0        0        0      298 2024-04-01 19:22:45.362507 vite_to_flask-0.1.0/app_flask_demo/__init__.py
--rw-r--r--   0        0        0       69 2024-04-01 10:28:05.818282 vite_to_flask-0.1.0/app_flask_demo/extensions/__init__.py
--rw-r--r--   0        0        0    39139 2024-04-01 20:19:37.795932 vite_to_flask-0.1.0/app_flask_demo/vtf/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    32826 2024-04-01 20:19:37.796632 vite_to_flask-0.1.0/app_flask_demo/vtf/app_vite_demo/index-9511eedb.css
--rw-r--r--   0        0        0    20114 2024-04-01 20:19:37.797165 vite_to_flask-0.1.0/app_flask_demo/vtf/app_vite_demo/index-9a82b860.js
--rw-r--r--   0        0        0      203 2024-04-01 19:32:58.177827 vite_to_flask-0.1.0/app_flask_demo/www/__init__.py
--rw-r--r--   0        0        0      174 2024-04-01 19:35:46.379933 vite_to_flask-0.1.0/app_flask_demo/www/templates/www/index.html
--rw-r--r--   0        0        0      194 2024-04-01 20:19:30.615319 vite_to_flask-0.1.0/app_vite_demo/Index.jsx
--rw-r--r--   0        0        0      536 2024-03-13 09:34:18.030126 vite_to_flask-0.1.0/app_vite_demo/__router__.jsx
--rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_to_flask-0.1.0/app_vite_demo/assets/ili.gif
--rw-r--r--   0        0        0      262 2024-03-31 09:43:57.345376 vite_to_flask-0.1.0/app_vite_demo/index.css
--rw-r--r--   0        0        0      413 2024-03-13 08:00:10.035867 vite_to_flask-0.1.0/app_vite_demo/index.html
--rw-r--r--   0        0        0   105659 2024-03-31 10:00:53.866729 vite_to_flask-0.1.0/app_vite_demo/package-lock.json
--rw-r--r--   0        0        0      570 2024-03-31 09:46:57.981095 vite_to_flask-0.1.0/app_vite_demo/package.json
--rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_to_flask-0.1.0/app_vite_demo/postcss.config.js
--rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_to_flask-0.1.0/app_vite_demo/tailwind.config.js
--rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_to_flask-0.1.0/app_vite_demo/vite.config.js
--rw-r--r--   0        0        0      858 2024-04-01 20:10:00.689094 vite_to_flask-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        5 2024-03-30 22:14:07.892357 vite_to_flask-0.1.0/requirements/dev.txt
--rw-r--r--   0        0        0       23 2024-03-30 22:47:24.808244 vite_to_flask-0.1.0/requirements/needed.txt
--rw-r--r--   0        0        0     1741 2024-04-01 20:39:06.293991 vite_to_flask-0.1.0/vite_to_flask/__init__.py
--rw-r--r--   0        0        0     4943 2024-04-01 19:39:45.691324 vite_to_flask-0.1.0/vite_to_flask/_html_tags.py
--rw-r--r--   0        0        0     3617 2024-04-01 20:07:27.744032 vite_to_flask-0.1.0/vite_to_flask/flask_extension.py
--rw-r--r--   0        0        0     3703 2024-04-01 20:17:48.087356 vite_to_flask-0.1.0/vite_to_flask/helpers.py
--rw-r--r--   0        0        0      788 2024-04-01 20:39:57.723948 vite_to_flask-0.1.0/vite_to_flask/parser.py
--rw-r--r--   0        0        0     3089 1970-01-01 00:00:00.000000 vite_to_flask-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5173 2024-04-01 21:09:14.191229 vite_to_flask-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_to_flask-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2485 2024-04-01 21:07:42.721942 vite_to_flask-0.2.0/README.md
+-rw-r--r--   0        0        0      298 2024-04-01 19:22:45.362507 vite_to_flask-0.2.0/app_flask_demo/__init__.py
+-rw-r--r--   0        0        0       69 2024-04-01 10:28:05.818282 vite_to_flask-0.2.0/app_flask_demo/extensions/__init__.py
+-rw-r--r--   0        0        0    39139 2024-04-01 20:19:37.795932 vite_to_flask-0.2.0/app_flask_demo/vtf/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    32826 2024-04-01 20:19:37.796632 vite_to_flask-0.2.0/app_flask_demo/vtf/app_vite_demo/index-9511eedb.css
+-rw-r--r--   0        0        0    20114 2024-04-01 20:19:37.797165 vite_to_flask-0.2.0/app_flask_demo/vtf/app_vite_demo/index-9a82b860.js
+-rw-r--r--   0        0        0      203 2024-04-01 19:32:58.177827 vite_to_flask-0.2.0/app_flask_demo/www/__init__.py
+-rw-r--r--   0        0        0      174 2024-04-01 19:35:46.379933 vite_to_flask-0.2.0/app_flask_demo/www/templates/www/index.html
+-rw-r--r--   0        0        0      194 2024-04-01 20:19:30.615319 vite_to_flask-0.2.0/app_vite_demo/Index.jsx
+-rw-r--r--   0        0        0      536 2024-03-13 09:34:18.030126 vite_to_flask-0.2.0/app_vite_demo/__router__.jsx
+-rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_to_flask-0.2.0/app_vite_demo/assets/ili.gif
+-rw-r--r--   0        0        0      262 2024-03-31 09:43:57.345376 vite_to_flask-0.2.0/app_vite_demo/index.css
+-rw-r--r--   0        0        0      413 2024-03-13 08:00:10.035867 vite_to_flask-0.2.0/app_vite_demo/index.html
+-rw-r--r--   0        0        0   105659 2024-03-31 10:00:53.866729 vite_to_flask-0.2.0/app_vite_demo/package-lock.json
+-rw-r--r--   0        0        0      570 2024-03-31 09:46:57.981095 vite_to_flask-0.2.0/app_vite_demo/package.json
+-rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_to_flask-0.2.0/app_vite_demo/postcss.config.js
+-rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_to_flask-0.2.0/app_vite_demo/tailwind.config.js
+-rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_to_flask-0.2.0/app_vite_demo/vite.config.js
+-rw-r--r--   0        0        0      961 2024-04-02 13:04:07.177829 vite_to_flask-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        5 2024-04-01 21:13:09.994976 vite_to_flask-0.2.0/requirements/needed.txt
+-rw-r--r--   0        0        0     1741 2024-04-02 13:00:25.910329 vite_to_flask-0.2.0/vite_to_flask/__init__.py
+-rw-r--r--   0        0        0     4943 2024-04-01 19:39:45.691324 vite_to_flask-0.2.0/vite_to_flask/_html_tags.py
+-rw-r--r--   0        0        0     3607 2024-04-02 13:00:13.553886 vite_to_flask-0.2.0/vite_to_flask/flask_extension.py
+-rw-r--r--   0        0        0     3703 2024-04-01 20:17:48.087356 vite_to_flask-0.2.0/vite_to_flask/helpers.py
+-rw-r--r--   0        0        0      788 2024-04-01 20:39:57.723948 vite_to_flask-0.2.0/vite_to_flask/parser.py
+-rw-r--r--   0        0        0     3089 1970-01-01 00:00:00.000000 vite_to_flask-0.2.0/PKG-INFO
```

### Comparing `vite_to_flask-0.1.0/.gitignore` & `vite_to_flask-0.2.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.idea/
+
 ### Node template
 # Logs
 logs
 *.log
 npm-debug.log*
 yarn-debug.log*
 yarn-error.log*
```

### Comparing `vite_to_flask-0.1.0/LICENSE` & `vite_to_flask-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.1.0/README.md` & `vite_to_flask-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.1.0/app_flask_demo/vtf/app_vite_demo/ili-85e34484.gif` & `vite_to_flask-0.2.0/app_flask_demo/vtf/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.1.0/app_flask_demo/vtf/app_vite_demo/index-9511eedb.css` & `vite_to_flask-0.2.0/app_flask_demo/vtf/app_vite_demo/index-9511eedb.css`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.1.0/app_flask_demo/vtf/app_vite_demo/index-9a82b860.js` & `vite_to_flask-0.2.0/app_flask_demo/vtf/app_vite_demo/index-9a82b860.js`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.1.0/app_vite_demo/__router__.jsx` & `vite_to_flask-0.2.0/app_vite_demo/__router__.jsx`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.1.0/app_vite_demo/assets/ili.gif` & `vite_to_flask-0.2.0/app_vite_demo/assets/ili.gif`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.1.0/app_vite_demo/package-lock.json` & `vite_to_flask-0.2.0/app_vite_demo/package-lock.json`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.1.0/app_vite_demo/package.json` & `vite_to_flask-0.2.0/app_vite_demo/package.json`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.1.0/pyproject.toml` & `vite_to_flask-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -20,11 +20,15 @@
 requires-python = ">=3.8"
 dynamic = ["version"]
 dependencies = ['flask']
 
 [project.scripts]
 vtf = "vite_to_flask:_cli"
 
+[tool.pyqwe]
+build = "*:flit build"
+publish = "*shell:export FLIT_USERNAME=__token__ && flit publish"
+
 [tool.vtf]
 npx_exec = "npx"
 flask_app_dir = "app_flask_demo"
 vite_app_dirs = ["app_vite_demo"]
```

### Comparing `vite_to_flask-0.1.0/vite_to_flask/__init__.py` & `vite_to_flask-0.2.0/vite_to_flask/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 
 from .flask_extension import ViteToFlask
 from .helpers import PyProjectConfig, _compile, Colr
 from .parser import ArgumentParser
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __all__ = ["ViteToFlask"]
 
 
 def _cli():
     pars = ArgumentParser(prog="vtf", add_help=False)
     pars.add_argument(
         "--version", "-v", action="version", version=f"vite-to-flask {__version__}"
```

### Comparing `vite_to_flask-0.1.0/vite_to_flask/_html_tags.py` & `vite_to_flask-0.2.0/vite_to_flask/_html_tags.py`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.1.0/vite_to_flask/flask_extension.py` & `vite_to_flask-0.2.0/vite_to_flask/flask_extension.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,28 +37,29 @@
                 "vtf directory not found in the flask app root directory."
             )
 
         for folder in self.vtf_root_path.iterdir():
             if folder.is_dir():
                 self.app.config["VTF_APPS"].update({folder.name: folder})
 
-        self._load_routes()
-        self._load_context_processor()
-        self._load_cors_headers()
+        self._load_routes(app)
+        self._load_context_processor(app)
+        self._load_cors_headers(app)
 
-    def _load_routes(self) -> None:
-        @self.app.route("/__vtf/<vite_app>/<filename>")
+    def _load_routes(self, app: Flask) -> None:
+        @app.route("/__vtf/<vite_app>/<filename>")
         def __vtf(vite_app: str, filename: str):
             return send_from_directory(self.vtf_root_path / vite_app, filename)
 
-    def _load_context_processor(self) -> None:
-        @self.app.context_processor
+    @staticmethod
+    def _load_context_processor(app: Flask) -> None:
+        @app.context_processor
         def vtf_head_processor():
             def vtf_head(vite_app: str) -> t.Any:
-                vite_assets = Path(self.app.root_path) / "vtf" / vite_app
+                vite_assets = Path(app.root_path) / "vtf" / vite_app
                 find_vite_js = vite_assets.glob("*.js")
                 find_vite_css = vite_assets.glob("*.css")
 
                 tags = []
 
                 for file in find_vite_js:
                     tags.append(
@@ -80,25 +81,25 @@
                         )
                     )
 
                 return Markup("".join([tag.raw() for tag in tags]))
 
             return dict(vtf_head=vtf_head)
 
-        @self.app.context_processor
+        @app.context_processor
         def vtf_body_processor():
             def vtf_body(
                     root_id: str = "root",
                     noscript_message: str = "You need to enable JavaScript to run this app.",
             ) -> t.Any:
                 return BodyContent(root_id, noscript_message)()
 
             return dict(vtf_body=vtf_body)
 
-    def _load_cors_headers(self) -> None:
-        if self.app.debug:
-            @self.app.after_request
-            def add_cors_headers(response):
-                response.headers["Access-Control-Allow-Origin"] = "*"
-                response.headers["Access-Control-Allow-Headers"] = "*"
-                response.headers["Access-Control-Allow-Methods"] = "*"
-                return response
+    @staticmethod
+    def _load_cors_headers(app: Flask) -> None:
+        @app.after_request
+        def after_request(response):
+            response.headers["Access-Control-Allow-Origin"] = "*"
+            response.headers["Access-Control-Allow-Headers"] = "*"
+            response.headers["Access-Control-Allow-Methods"] = "*"
+            return response
```

### Comparing `vite_to_flask-0.1.0/vite_to_flask/helpers.py` & `vite_to_flask-0.2.0/vite_to_flask/helpers.py`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.1.0/vite_to_flask/parser.py` & `vite_to_flask-0.2.0/vite_to_flask/parser.py`

 * *Files identical despite different names*

### Comparing `vite_to_flask-0.1.0/PKG-INFO` & `vite_to_flask-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vite-to-flask
-Version: 0.1.0
+Version: 0.2.0
 Summary: Transport Vite apps to Flask / Flask blueprints.
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

