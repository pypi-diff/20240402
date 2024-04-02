# Comparing `tmp/flask-variable-manager-0.0.1.tar.gz` & `tmp/flask-variable-manager-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-variable-manager-0.0.1.tar", last modified: Tue Apr  2 03:15:52 2024, max compression
+gzip compressed data, was "flask-variable-manager-0.1.0.tar", last modified: Tue Apr  2 10:32:45 2024, max compression
```

## Comparing `flask-variable-manager-0.0.1.tar` & `flask-variable-manager-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2024-04-02 03:15:52.240143 flask-variable-manager-0.0.1/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1064 2024-04-01 03:40:38.000000 flask-variable-manager-0.0.1/LICENSE
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2480 2024-04-02 03:15:52.239804 flask-variable-manager-0.0.1/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1643 2024-04-01 12:20:31.000000 flask-variable-manager-0.0.1/README.md
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2024-04-02 03:15:52.235854 flask-variable-manager-0.0.1/flask_variable_manager/
--rw-r--r--   0 minwook-shin   (501) staff       (20)      127 2024-04-01 03:44:48.000000 flask-variable-manager-0.0.1/flask_variable_manager/__init__.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2024-04-02 03:15:52.237944 flask-variable-manager-0.0.1/flask_variable_manager/extension/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2024-04-01 03:41:38.000000 flask-variable-manager-0.0.1/flask_variable_manager/extension/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     3656 2024-04-01 08:28:31.000000 flask-variable-manager-0.0.1/flask_variable_manager/extension/variable_manager.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2024-04-02 03:15:52.238415 flask-variable-manager-0.0.1/flask_variable_manager/tests/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2024-04-01 08:14:27.000000 flask-variable-manager-0.0.1/flask_variable_manager/tests/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)      754 2024-04-01 08:19:49.000000 flask-variable-manager-0.0.1/flask_variable_manager/tests/test_vm.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2024-04-02 03:15:52.238752 flask-variable-manager-0.0.1/flask_variable_manager.egg-info/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2480 2024-04-02 03:15:52.000000 flask-variable-manager-0.0.1/flask_variable_manager.egg-info/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)      475 2024-04-02 03:15:52.000000 flask-variable-manager-0.0.1/flask_variable_manager.egg-info/SOURCES.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2024-04-02 03:15:52.000000 flask-variable-manager-0.0.1/flask_variable_manager.egg-info/dependency_links.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       78 2024-04-02 03:15:52.000000 flask-variable-manager-0.0.1/flask_variable_manager.egg-info/requires.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       23 2024-04-02 03:15:52.000000 flask-variable-manager-0.0.1/flask_variable_manager.egg-info/top_level.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1061 2024-04-01 12:21:32.000000 flask-variable-manager-0.0.1/pyproject.toml
--rw-r--r--   0 minwook-shin   (501) staff       (20)       38 2024-04-02 03:15:52.240224 flask-variable-manager-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:32:45.324519 flask-variable-manager-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-02 10:32:38.000000 flask-variable-manager-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-02 10:32:45.324519 flask-variable-manager-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-02 10:32:38.000000 flask-variable-manager-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:32:45.320520 flask-variable-manager-0.1.0/flask_variable_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 10:32:38.000000 flask-variable-manager-0.1.0/flask_variable_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:32:45.320520 flask-variable-manager-0.1.0/flask_variable_manager/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:32:38.000000 flask-variable-manager-0.1.0/flask_variable_manager/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-02 10:32:38.000000 flask-variable-manager-0.1.0/flask_variable_manager/extension/variable_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:32:45.320520 flask-variable-manager-0.1.0/flask_variable_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:32:38.000000 flask-variable-manager-0.1.0/flask_variable_manager/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 10:32:38.000000 flask-variable-manager-0.1.0/flask_variable_manager/tests/test_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:32:45.320520 flask-variable-manager-0.1.0/flask_variable_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-02 10:32:45.000000 flask-variable-manager-0.1.0/flask_variable_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-02 10:32:45.000000 flask-variable-manager-0.1.0/flask_variable_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:32:45.000000 flask-variable-manager-0.1.0/flask_variable_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 10:32:45.000000 flask-variable-manager-0.1.0/flask_variable_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 10:32:45.000000 flask-variable-manager-0.1.0/flask_variable_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-02 10:32:38.000000 flask-variable-manager-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:32:45.324519 flask-variable-manager-0.1.0/setup.cfg
```

### Comparing `flask-variable-manager-0.0.1/LICENSE` & `flask-variable-manager-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-variable-manager-0.0.1/PKG-INFO` & `flask-variable-manager-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: flask-variable-manager
-Version: 0.0.1
+Version: 0.1.0
 Summary: Create a variable manager in flask, enter values in python, and use values on the jinja template.
 Author-email: minwook-shin <minwook0106@gmail.com>
 Project-URL: Homepage, https://github.com/minwook-shin/flask-variable-manager
 Project-URL: Bug Tracker, https://github.com/minwook-shin/flask-variable-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Framework :: Flask
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask==2.3.3
 Requires-Dist: Jinja2==3.1.3
 Provides-Extra: dev
 Requires-Dist: flasgger==0.9.7b2; extra == "dev"
@@ -75,14 +76,16 @@
 
 ### Get all user-defined variables
 
 This route allows you to get all user-defined variables. 
 
 It accepts a GET request at the `/vm/var` endpoint. 
 
+(or `vm/vars` for the multiple count of the variable)
+
 ## License
 
 This project is licensed under the terms of the MIT license.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

### Comparing `flask-variable-manager-0.0.1/README.md` & `flask-variable-manager-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 
 ### Get all user-defined variables
 
 This route allows you to get all user-defined variables. 
 
 It accepts a GET request at the `/vm/var` endpoint. 
 
+(or `vm/vars` for the multiple count of the variable)
+
 ## License
 
 This project is licensed under the terms of the MIT license.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

### Comparing `flask-variable-manager-0.0.1/flask_variable_manager/extension/variable_manager.py` & `flask-variable-manager-0.1.0/flask_variable_manager/extension/variable_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -54,14 +54,41 @@
         """
         key = request.form.get('key')
         value = request.form.get('value')
 
         g.local[key] = value
         return jsonify({'message': 'The variable has been set successfully.'})
 
+    @app.route('/vm/vars', methods=['POST'])
+    def set_variables():
+        """
+        ---
+        tags:
+          - Variables
+        summary: Set multiple user-defined variables
+        description: This endpoint allows you to set multiple user-defined variables.
+        parameters:
+          - in: body
+            name: variables
+            description: The variables to set.
+            schema:
+              type: object
+              additionalProperties:
+                type: string
+        responses:
+          200:
+            description: The variables have been set successfully.
+        """
+        variables = request.get_json()
+
+        for key, value in variables.items():
+            g.local[key] = value
+
+        return jsonify({'message': 'The variables have been set successfully.'})
+
     @app.route('/vm/var', methods=['GET'])
     def get_variables():
         """
         ---
         tags:
           - Variables
         summary: Get all user-defined variables
```

### Comparing `flask-variable-manager-0.0.1/flask_variable_manager/tests/test_vm.py` & `flask-variable-manager-0.1.0/flask_variable_manager/tests/test_vm.py`

 * *Files identical despite different names*

### Comparing `flask-variable-manager-0.0.1/flask_variable_manager.egg-info/PKG-INFO` & `flask-variable-manager-0.1.0/flask_variable_manager.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: flask-variable-manager
-Version: 0.0.1
+Version: 0.1.0
 Summary: Create a variable manager in flask, enter values in python, and use values on the jinja template.
 Author-email: minwook-shin <minwook0106@gmail.com>
 Project-URL: Homepage, https://github.com/minwook-shin/flask-variable-manager
 Project-URL: Bug Tracker, https://github.com/minwook-shin/flask-variable-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Framework :: Flask
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask==2.3.3
 Requires-Dist: Jinja2==3.1.3
 Provides-Extra: dev
 Requires-Dist: flasgger==0.9.7b2; extra == "dev"
@@ -75,14 +76,16 @@
 
 ### Get all user-defined variables
 
 This route allows you to get all user-defined variables. 
 
 It accepts a GET request at the `/vm/var` endpoint. 
 
+(or `vm/vars` for the multiple count of the variable)
+
 ## License
 
 This project is licensed under the terms of the MIT license.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

### Comparing `flask-variable-manager-0.0.1/pyproject.toml` & `flask-variable-manager-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 include-package-data = false
 
 [tool.setuptools.packages.find]
 include = ['flask_variable_manager*']
 
 [project]
 name = "flask-variable-manager"
-version = "0.0.1"
+version = "0.1.0"
 description = "Create a variable manager in flask, enter values in python, and use values on the jinja template."
 authors = [
     { name = "minwook-shin", email = "minwook0106@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Framework :: Flask"
 ]
 dependencies = [
     "flask==2.3.3",
     "Jinja2==3.1.3"
 ]
 
 [project.optional-dependencies]
```

