# Comparing `tmp/pyqwe-1.0.3.tar.gz` & `tmp/pyqwe-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqwe-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyqwe-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyqwe-1.0.3.tar` & `pyqwe-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       28 2024-03-30 13:38:11.669595 pyqwe-1.0.3/.env.example
--rw-r--r--   0        0        0     1160 2024-03-30 13:38:11.669728 pyqwe-1.0.3/.gitignore
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 pyqwe-1.0.3/LICENSE
--rw-r--r--   0        0        0     2382 2024-03-30 20:08:00.862609 pyqwe-1.0.3/README.md
--rw-r--r--   0        0        0      204 2024-03-29 08:35:21.325325 pyqwe-1.0.3/flask_example/module.py
--rw-r--r--   0        0        0      204 2024-03-29 08:42:03.877337 pyqwe-1.0.3/flask_example/package/__init__.py
--rw-r--r--   0        0        0      936 2024-03-30 13:38:11.669969 pyqwe-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1111 2024-03-30 20:08:27.265821 pyqwe-1.0.3/pyqwe/__init__.py
--rw-r--r--   0        0        0      179 2024-03-30 13:38:11.670188 pyqwe-1.0.3/pyqwe/exceptions.py
--rw-r--r--   0        0        0     3619 2024-03-30 13:38:11.670300 pyqwe-1.0.3/pyqwe/helpers.py
--rw-r--r--   0        0        0      963 2024-03-30 13:38:11.670411 pyqwe-1.0.3/pyqwe/parser.py
--rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 pyqwe-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       28 2024-03-30 13:38:11.669595 pyqwe-1.1.3/.env.example
+-rw-r--r--   0        0        0     1160 2024-03-30 13:38:11.669728 pyqwe-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 pyqwe-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2897 2024-04-02 10:17:48.240855 pyqwe-1.1.3/README.md
+-rw-r--r--   0        0        0      204 2024-03-29 08:35:21.325325 pyqwe-1.1.3/flask_example/module.py
+-rw-r--r--   0        0        0      204 2024-03-29 08:42:03.877337 pyqwe-1.1.3/flask_example/package/__init__.py
+-rw-r--r--   0        0        0      936 2024-03-30 13:38:11.669969 pyqwe-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1111 2024-04-02 10:19:09.776543 pyqwe-1.1.3/pyqwe/__init__.py
+-rw-r--r--   0        0        0      179 2024-03-30 13:38:11.670188 pyqwe-1.1.3/pyqwe/exceptions.py
+-rw-r--r--   0        0        0     3876 2024-04-02 10:10:43.435476 pyqwe-1.1.3/pyqwe/helpers.py
+-rw-r--r--   0        0        0      963 2024-04-01 15:43:06.466385 pyqwe-1.1.3/pyqwe/parser.py
+-rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 pyqwe-1.1.3/PKG-INFO
```

### Comparing `pyqwe-1.0.3/.gitignore` & `pyqwe-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqwe-1.0.3/LICENSE` & `pyqwe-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqwe-1.0.3/README.md` & `pyqwe-1.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -95,14 +95,37 @@
 To run the command as a subprocess shell command, add the `shell` key to the command.
 
 ```toml
 [tool.pyqwe]
 say_hello = "*shell:echo Hello World"
 ```
 
+### Change the working directory
+
+You can change the working directory of a subprocess by adding the folder 
+within parentheses to the command, `(node_app)` for example.
+
+**The folder must be relative** to the pyproject.toml file. 
+
+**Absolute paths are not supported**.
+
+**Moving up directories is not supported**, `../node_app` for example.
+
+```toml
+[tool.pyqwe]
+npm_install = "*(node_app):npm install"
+```
+
+This can be used with the `shell` key.
+
+```toml
+[tool.pyqwe]
+npm_install = "*shell(node_app):npm i"
+```
+
 ### Using environment variables
 
 To use environment variables in the command, use the `{{ }}` syntax.
 
 ```toml
 [tool.pyqwe]
 talk = "*shell:echo {{MESSAGE}}"
```

### Comparing `pyqwe-1.0.3/pyproject.toml` & `pyqwe-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyqwe-1.0.3/pyqwe/__init__.py` & `pyqwe-1.1.3/pyqwe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tomllib
 from pathlib import Path
 
 from .helpers import _run, _split_runner
 from .parser import ArgumentParser
 
-__version__ = "1.0.3"
+__version__ = "1.1.3"
 
 # sr = start of runner
 # er = end of runner
 # runner = sr:er
 # flask = app:run
 # will invoke the run function in the app module
```

### Comparing `pyqwe-1.0.3/pyqwe/helpers.py` & `pyqwe-1.1.3/pyqwe/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,18 +121,26 @@
         rev = _replace_env_vars
 
     sr = rev(sr)
     er = rev(er)
 
     try:
         if "*" in sr:
+            if "(" in sr:
+                _cwd_tack = sr[sr.find("(") + 1: sr.find(")")]
+
+                if sys.platform == "win32":
+                    _cwd_tack = _cwd_tack.replace("/", "\\")
+
+                _cwd = _cwd / _cwd_tack
+
             if "shell" in sr:
-                subprocess.run(er, shell=True)
+                subprocess.run(er, shell=True, cwd=_cwd)
             else:
-                subprocess.run(shlex.split(er))
+                subprocess.run(shlex.split(er), cwd=_cwd)
 
         else:
             sr_path, sr_type = _identify_sr(sr, _cwd)
 
             if sr_type == "package":
                 sys.path.append(str(sr_path))
                 module = importlib.import_module("__init__")
```

### Comparing `pyqwe-1.0.3/pyqwe/parser.py` & `pyqwe-1.1.3/pyqwe/parser.py`

 * *Files identical despite different names*

### Comparing `pyqwe-1.0.3/PKG-INFO` & `pyqwe-1.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqwe
-Version: 1.0.3
+Version: 1.1.3
 Summary: Run commands set in the pyproject.toml file
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pyqwe-extra-dotenv ; extra == "dotenv"
 Project-URL: Source, https://github.com/CheeseCake87/pyqwe
@@ -107,14 +107,37 @@
 To run the command as a subprocess shell command, add the `shell` key to the command.
 
 ```toml
 [tool.pyqwe]
 say_hello = "*shell:echo Hello World"
 ```
 
+### Change the working directory
+
+You can change the working directory of a subprocess by adding the folder 
+within parentheses to the command, `(node_app)` for example.
+
+**The folder must be relative** to the pyproject.toml file. 
+
+**Absolute paths are not supported**.
+
+**Moving up directories is not supported**, `../node_app` for example.
+
+```toml
+[tool.pyqwe]
+npm_install = "*(node_app):npm install"
+```
+
+This can be used with the `shell` key.
+
+```toml
+[tool.pyqwe]
+npm_install = "*shell(node_app):npm i"
+```
+
 ### Using environment variables
 
 To use environment variables in the command, use the `{{ }}` syntax.
 
 ```toml
 [tool.pyqwe]
 talk = "*shell:echo {{MESSAGE}}"
```

