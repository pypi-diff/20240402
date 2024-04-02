# Comparing `tmp/bare-script-3.0.8.tar.gz` & `tmp/bare-script-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bare-script-3.0.8.tar", last modified: Sat Mar 30 14:54:16 2024, max compression
+gzip compressed data, was "bare-script-3.0.9.tar", last modified: Tue Apr  2 16:20:31 2024, max compression
```

## Comparing `bare-script-3.0.8.tar` & `bare-script-3.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-03-30 14:54:16.721710 bare-script-3.0.8/
--rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-03-14 18:21:45.000000 bare-script-3.0.8/LICENSE
--rw-r--r--   0 craighobbs   (501) staff       (20)     7794 2024-03-30 14:54:16.721648 bare-script-3.0.8/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)     6932 2024-03-14 18:21:45.000000 bare-script-3.0.8/README.rst
--rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-03-14 18:21:45.000000 bare-script-3.0.8/pyproject.toml
--rw-r--r--   0 craighobbs   (501) staff       (20)      981 2024-03-30 14:54:16.722039 bare-script-3.0.8/setup.cfg
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-03-30 14:54:16.718561 bare-script-3.0.8/src/
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-03-30 14:54:16.720539 bare-script-3.0.8/src/bare_script/
--rw-r--r--   0 craighobbs   (501) staff       (20)      696 2024-03-14 18:21:45.000000 bare-script-3.0.8/src/bare_script/__init__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)      232 2024-03-14 18:21:45.000000 bare-script-3.0.8/src/bare_script/__main__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     4970 2024-03-19 20:44:30.000000 bare-script-3.0.8/src/bare_script/bare.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     6608 2024-03-14 18:21:45.000000 bare-script-3.0.8/src/bare_script/baredoc.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    16534 2024-03-19 21:03:53.000000 bare-script-3.0.8/src/bare_script/data.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    65240 2024-03-30 14:44:03.000000 bare-script-3.0.8/src/bare_script/library.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    13024 2024-03-14 18:21:45.000000 bare-script-3.0.8/src/bare_script/model.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     2647 2024-03-14 18:21:45.000000 bare-script-3.0.8/src/bare_script/options.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    29008 2024-03-14 18:21:45.000000 bare-script-3.0.8/src/bare_script/parser.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    14951 2024-03-30 14:44:03.000000 bare-script-3.0.8/src/bare_script/runtime.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    14570 2024-03-30 14:44:03.000000 bare-script-3.0.8/src/bare_script/value.py
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-03-30 14:54:16.721423 bare-script-3.0.8/src/bare_script.egg-info/
--rw-r--r--   0 craighobbs   (501) staff       (20)     7794 2024-03-30 14:54:16.000000 bare-script-3.0.8/src/bare_script.egg-info/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)      567 2024-03-30 14:54:16.000000 bare-script-3.0.8/src/bare_script.egg-info/SOURCES.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-03-30 14:54:16.000000 bare-script-3.0.8/src/bare_script.egg-info/dependency_links.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       82 2024-03-30 14:54:16.000000 bare-script-3.0.8/src/bare_script.egg-info/entry_points.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       23 2024-03-30 14:54:16.000000 bare-script-3.0.8/src/bare_script.egg-info/requires.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-03-30 14:54:16.000000 bare-script-3.0.8/src/bare_script.egg-info/top_level.txt
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-02 16:20:31.370931 bare-script-3.0.9/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-03-30 15:31:56.000000 bare-script-3.0.9/LICENSE
+-rw-r--r--   0 craighobbs   (501) staff       (20)     7794 2024-04-02 16:20:31.370871 bare-script-3.0.9/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)     6932 2024-03-30 15:31:56.000000 bare-script-3.0.9/README.rst
+-rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-03-30 15:31:56.000000 bare-script-3.0.9/pyproject.toml
+-rw-r--r--   0 craighobbs   (501) staff       (20)      981 2024-04-02 16:20:31.371242 bare-script-3.0.9/setup.cfg
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-02 16:20:31.367926 bare-script-3.0.9/src/
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-02 16:20:31.369833 bare-script-3.0.9/src/bare_script/
+-rw-r--r--   0 craighobbs   (501) staff       (20)      696 2024-03-30 15:31:56.000000 bare-script-3.0.9/src/bare_script/__init__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)      232 2024-03-30 15:31:56.000000 bare-script-3.0.9/src/bare_script/__main__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     4970 2024-03-30 15:31:56.000000 bare-script-3.0.9/src/bare_script/bare.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     6608 2024-03-30 15:31:56.000000 bare-script-3.0.9/src/bare_script/baredoc.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    16534 2024-03-30 15:31:56.000000 bare-script-3.0.9/src/bare_script/data.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    65240 2024-03-30 15:31:56.000000 bare-script-3.0.9/src/bare_script/library.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    13196 2024-04-02 16:09:50.000000 bare-script-3.0.9/src/bare_script/model.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2647 2024-03-30 15:31:56.000000 bare-script-3.0.9/src/bare_script/options.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    29008 2024-03-30 15:31:56.000000 bare-script-3.0.9/src/bare_script/parser.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    14951 2024-03-30 15:31:56.000000 bare-script-3.0.9/src/bare_script/runtime.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    14570 2024-03-30 15:31:56.000000 bare-script-3.0.9/src/bare_script/value.py
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-02 16:20:31.370658 bare-script-3.0.9/src/bare_script.egg-info/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     7794 2024-04-02 16:20:31.000000 bare-script-3.0.9/src/bare_script.egg-info/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)      567 2024-04-02 16:20:31.000000 bare-script-3.0.9/src/bare_script.egg-info/SOURCES.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-04-02 16:20:31.000000 bare-script-3.0.9/src/bare_script.egg-info/dependency_links.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       82 2024-04-02 16:20:31.000000 bare-script-3.0.9/src/bare_script.egg-info/entry_points.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       23 2024-04-02 16:20:31.000000 bare-script-3.0.9/src/bare_script.egg-info/requires.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-04-02 16:20:31.000000 bare-script-3.0.9/src/bare_script.egg-info/top_level.txt
```

### Comparing `bare-script-3.0.8/LICENSE` & `bare-script-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bare-script-3.0.8/PKG-INFO` & `bare-script-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bare-script
-Version: 3.0.8
+Version: 3.0.9
 Summary: bare-script
 Home-page: https://github.com/craigahobbs/bare-script
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: bare-script
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bare-script-3.0.8/README.rst` & `bare-script-3.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `bare-script-3.0.8/setup.cfg` & `bare-script-3.0.9/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bare-script
-version = 3.0.8
+version = 3.0.9
 url = https://github.com/craigahobbs/bare-script
 author = Craig A. Hobbs
 author_email = craigahobbs@gmail.com
 license = MIT
 description = bare-script
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```

### Comparing `bare-script-3.0.8/src/bare_script/__init__.py` & `bare-script-3.0.9/src/bare_script/__init__.py`

 * *Files identical despite different names*

### Comparing `bare-script-3.0.8/src/bare_script/bare.py` & `bare-script-3.0.9/src/bare_script/bare.py`

 * *Files identical despite different names*

### Comparing `bare-script-3.0.8/src/bare_script/baredoc.py` & `bare-script-3.0.9/src/bare_script/baredoc.py`

 * *Files identical despite different names*

### Comparing `bare-script-3.0.8/src/bare_script/data.py` & `bare-script-3.0.9/src/bare_script/data.py`

 * *Files identical despite different names*

### Comparing `bare-script-3.0.8/src/bare_script/library.py` & `bare-script-3.0.9/src/bare_script/library.py`

 * *Files identical despite different names*

### Comparing `bare-script-3.0.8/src/bare_script/model.py` & `bare-script-3.0.9/src/bare_script/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,32 +409,35 @@
 
 # Helper function to set variable assignments/uses for a statements array
 def _get_variable_assignments_and_uses(statements, assigns, uses):
     for ix_statement, statement in enumerate(statements):
         statement_key = next(iter(statement.keys()))
         if statement_key == 'expr':
             if 'name' in statement['expr']:
-                assigns[statement['expr']['name']] = ix_statement
-            _get_xpression_variable_uses(statement['expr']['expr'], uses, ix_statement)
+                if statement['expr']['name'] not in assigns:
+                    assigns[statement['expr']['name']] = ix_statement
+            _get_expression_variable_uses(statement['expr']['expr'], uses, ix_statement)
         elif statement_key == 'jump' and 'expr' in statement['jump']:
-            _get_xpression_variable_uses(statement['jump']['expr'], uses, ix_statement)
+            _get_expression_variable_uses(statement['jump']['expr'], uses, ix_statement)
         elif statement_key == 'return' and 'expr' in statement['return']:
-            _get_xpression_variable_uses(statement['return']['expr'], uses, ix_statement)
+            _get_expression_variable_uses(statement['return']['expr'], uses, ix_statement)
 
 
 # Helper function to set variable uses for an expression
-def _get_xpression_variable_uses(expr, uses, ix_statement):
+def _get_expression_variable_uses(expr, uses, ix_statement):
     expr_key = next(iter(expr.keys()))
     if expr_key == 'variable':
-        uses[expr['variable']] = ix_statement
+        if expr['variable'] not in uses:
+            uses[expr['variable']] = ix_statement
     elif expr_key == 'binary':
-        _get_xpression_variable_uses(expr['binary']['left'], uses, ix_statement)
-        _get_xpression_variable_uses(expr['binary']['right'], uses, ix_statement)
+        _get_expression_variable_uses(expr['binary']['left'], uses, ix_statement)
+        _get_expression_variable_uses(expr['binary']['right'], uses, ix_statement)
     elif expr_key == 'unary':
-        _get_xpression_variable_uses(expr['unary']['expr'], uses, ix_statement)
+        _get_expression_variable_uses(expr['unary']['expr'], uses, ix_statement)
     elif expr_key == 'group':
-        _get_xpression_variable_uses(expr['group'], uses, ix_statement)
+        _get_expression_variable_uses(expr['group'], uses, ix_statement)
     elif expr_key == 'function':
-        uses[expr['function']['name']] = ix_statement
+        if expr['function']['name'] not in uses:
+            uses[expr['function']['name']] = ix_statement
         if 'args' in expr['function']:
             for arg_expr in expr['function']['args']:
-                _get_xpression_variable_uses(arg_expr, uses, ix_statement)
+                _get_expression_variable_uses(arg_expr, uses, ix_statement)
```

### Comparing `bare-script-3.0.8/src/bare_script/options.py` & `bare-script-3.0.9/src/bare_script/options.py`

 * *Files identical despite different names*

### Comparing `bare-script-3.0.8/src/bare_script/parser.py` & `bare-script-3.0.9/src/bare_script/parser.py`

 * *Files identical despite different names*

### Comparing `bare-script-3.0.8/src/bare_script/runtime.py` & `bare-script-3.0.9/src/bare_script/runtime.py`

 * *Files identical despite different names*

### Comparing `bare-script-3.0.8/src/bare_script/value.py` & `bare-script-3.0.9/src/bare_script/value.py`

 * *Files identical despite different names*

### Comparing `bare-script-3.0.8/src/bare_script.egg-info/PKG-INFO` & `bare-script-3.0.9/src/bare_script.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bare-script
-Version: 3.0.8
+Version: 3.0.9
 Summary: bare-script
 Home-page: https://github.com/craigahobbs/bare-script
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: bare-script
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bare-script-3.0.8/src/bare_script.egg-info/SOURCES.txt` & `bare-script-3.0.9/src/bare_script.egg-info/SOURCES.txt`

 * *Files identical despite different names*

