# Comparing `tmp/spacestar-0.3.0.tar.gz` & `tmp/spacestar-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacestar-0.3.0.tar", max compression
+gzip compressed data, was "spacestar-0.3.1.tar", max compression
```

## Comparing `spacestar-0.3.0.tar` & `spacestar-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      805 2024-02-11 02:25:18.130249 spacestar-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1482 2024-01-26 02:10:23.228942 spacestar-0.3.0/spacestar/__init__.py
--rw-r--r--   0        0        0     9004 2024-02-11 02:22:39.234576 spacestar-0.3.0/spacestar/app.py
--rw-r--r--   0        0        0      328 2024-01-03 03:25:33.886746 spacestar-0.3.0/spacestar/context.py
--rw-r--r--   0        0        0      221 2024-02-11 02:22:39.238779 spacestar-0.3.0/spacestar/model.py
--rw-r--r--   0        0        0     1168 2024-02-11 02:26:20.320470 spacestar-0.3.0/setup.py
--rw-r--r--   0        0        0      709 2024-02-11 02:26:20.320674 spacestar-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      805 2024-04-02 14:15:51.306460 spacestar-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1482 2024-01-26 02:10:23.228942 spacestar-0.3.1/spacestar/__init__.py
+-rw-r--r--   0        0        0     9010 2024-04-02 14:15:51.301768 spacestar-0.3.1/spacestar/app.py
+-rw-r--r--   0        0        0      328 2024-01-03 03:25:33.886746 spacestar-0.3.1/spacestar/context.py
+-rw-r--r--   0        0        0      322 2024-02-21 00:08:41.808781 spacestar-0.3.1/spacestar/model.py
+-rw-r--r--   0        0        0     1168 2024-04-02 14:16:29.306799 spacestar-0.3.1/setup.py
+-rw-r--r--   0        0        0      709 2024-04-02 14:16:29.307039 spacestar-0.3.1/PKG-INFO
```

### Comparing `spacestar-0.3.0/pyproject.toml` & `spacestar-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spacestar"
-version = "0.3.0"
+version = "0.3.1"
 description = "Framework for building web based apps with the power of Starlette, Pydantic and Deta Space."
 authors = ["Daniel Arantes <arantesdv@me.com>"]
 license = "MIT"
 exclude = ["templates", "dev.py", ".env", "exclude", "dev.css", "dev.html", "dev.js"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `spacestar-0.3.0/spacestar/__init__.py` & `spacestar-0.3.1/spacestar/__init__.py`

 * *Files identical despite different names*

### Comparing `spacestar-0.3.0/spacestar/app.py` & `spacestar-0.3.1/spacestar/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     def insert(self, index: int, app: Route | Mount) -> None:
         self.routes.insert(index, app)
         
     @staticmethod
     async def process_form_data(request: Request) -> dict:
         form_data: FormData = await request.form()
         data, result = defaultdict(list), {}
-        for key, value in form_data.items():
+        for key, value in form_data.multi_items():
             data[key].append(value)
         for key in data:
             if not key == 'search':
                 value = data[key]
                 if len(value) == 0:
                     result[key] = None
                 elif len(value) == 1:
```

### Comparing `spacestar-0.3.0/setup.py` & `spacestar-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                      'spacestar.initfolders:create_static_directory',
                      'init-templates = '
                      'spacestar.initfolders:create_templates_directory',
                      'initfolders = spacestar.initfolders:main']}
 
 setup_kwargs = {
     'name': 'spacestar',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Framework for building web based apps with the power of Starlette, Pydantic and Deta Space.',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `spacestar-0.3.0/PKG-INFO` & `spacestar-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacestar
-Version: 0.3.0
+Version: 0.3.1
 Summary: Framework for building web based apps with the power of Starlette, Pydantic and Deta Space.
 License: MIT
 Author: Daniel Arantes
 Author-email: arantesdv@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

