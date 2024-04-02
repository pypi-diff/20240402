# Comparing `tmp/automython-1.1.1.tar.gz` & `tmp/automython-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automython-1.1.1.tar", last modified: Sun Mar 10 04:21:38 2024, max compression
+gzip compressed data, was "automython-1.1.2.tar", last modified: Tue Apr  2 02:29:53 2024, max compression
```

## Comparing `automython-1.1.1.tar` & `automython-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 04:21:38.751300 automython-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-10 04:20:58.000000 automython-1.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-03-10 04:21:38.751300 automython-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-03-10 04:20:58.000000 automython-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-10 04:20:58.000000 automython-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-10 04:21:38.751300 automython-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-03-10 04:20:58.000000 automython-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 04:21:38.747300 automython-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 04:21:38.751300 automython-1.1.1/src/automython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-03-10 04:21:38.000000 automython-1.1.1/src/automython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-10 04:21:38.000000 automython-1.1.1/src/automython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 04:21:38.000000 automython-1.1.1/src/automython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-10 04:21:38.000000 automython-1.1.1/src/automython.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-10 04:21:38.000000 automython-1.1.1/src/automython.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-10 04:21:38.000000 automython-1.1.1/src/automython.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 04:21:38.751300 automython-1.1.1/src/interpret/
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-10 04:20:58.000000 automython-1.1.1/src/interpret/Buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-03-10 04:20:58.000000 automython-1.1.1/src/interpret/Lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14383 2024-03-10 04:20:58.000000 automython-1.1.1/src/interpret/Parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-10 04:20:58.000000 automython-1.1.1/src/interpret/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-03-10 04:20:58.000000 automython-1.1.1/src/interpret/Visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 04:20:58.000000 automython-1.1.1/src/interpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-10 04:20:58.000000 automython-1.1.1/src/interpret/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-10 04:20:58.000000 automython-1.1.1/src/interpret/file_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    18876 2024-03-10 04:20:58.000000 automython-1.1.1/src/interpret/helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      791 2024-03-10 04:20:58.000000 automython-1.1.1/src/interpret/interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:29:53.604455 automython-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-02 02:28:41.000000 automython-1.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-04-02 02:29:53.604455 automython-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-04-02 02:28:41.000000 automython-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-02 02:28:41.000000 automython-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 02:29:53.604455 automython-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-02 02:28:41.000000 automython-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:29:53.600455 automython-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:29:53.600455 automython-1.1.2/src/automython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-04-02 02:29:53.000000 automython-1.1.2/src/automython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-02 02:29:53.000000 automython-1.1.2/src/automython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:29:53.000000 automython-1.1.2/src/automython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 02:29:53.000000 automython-1.1.2/src/automython.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 02:29:53.000000 automython-1.1.2/src/automython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 02:29:53.000000 automython-1.1.2/src/automython.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:29:53.600455 automython-1.1.2/src/interpret/
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/Buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/Lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/Parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/Visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/file_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18876 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      791 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/interpreter.py
```

### Comparing `automython-1.1.1/LICENSE.txt` & `automython-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automython-1.1.1/PKG-INFO` & `automython-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automython
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simplistic programming language interpreter to Python to help students grasp finite automata theory programmatically and with a computed graph through visualization libraries.
 Home-page: https://github.com/mkantrr/automython
 Author: Matthew Kanter
 Author-email: Matthew Kanter <matt@matutu.dev>
 Maintainer-email: Matthew Kanter <matt@matutu.dev>
 License: The MIT License (MIT)
         
@@ -163,15 +163,15 @@
 
 The NFA object in Automython must resemble this syntax:
 ```python
 NFA(states, input_symbols, transitions, initial_state, final_states)
 ```
 It must **also** be assigned to a variable; it cannot be treated as an expression, i.e.:
 ```python
-nfa = NFA(states, input_symbols, transitions, initial_state, final_states, allow_partial[optional]: bool)
+nfa = NFA(states, input_symbols, transitions, initial_state, final_states)
 ```
 
 - The `states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 - The `input_symbols` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 - The `transitions` argument is a Dictionary. This can be either a Dictionary in the argument, or a variable that stores a Dictionary. The values of each key maps to an input symbol as a key to a Set of states.
 - The `initial_state` argument is a String. This can be either a String in the argument, or a variable that stores a String.
 - The `final_states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
```

### Comparing `automython-1.1.1/README.md` & `automython-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
 The NFA object in Automython must resemble this syntax:
 ```python
 NFA(states, input_symbols, transitions, initial_state, final_states)
 ```
 It must **also** be assigned to a variable; it cannot be treated as an expression, i.e.:
 ```python
-nfa = NFA(states, input_symbols, transitions, initial_state, final_states, allow_partial[optional]: bool)
+nfa = NFA(states, input_symbols, transitions, initial_state, final_states)
 ```
 
 - The `states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 - The `input_symbols` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 - The `transitions` argument is a Dictionary. This can be either a Dictionary in the argument, or a variable that stores a Dictionary. The values of each key maps to an input symbol as a key to a Set of states.
 - The `initial_state` argument is a String. This can be either a String in the argument, or a variable that stores a String.
 - The `final_states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
```

### Comparing `automython-1.1.1/pyproject.toml` & `automython-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "automython"
-version = "1.1.1"
+version = "1.1.2"
 description = "A simplistic programming language interpreter to Python to help students grasp finite automata theory programmatically and with a computed graph through visualization libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ['automata', "finite", 'compiler', 'interpreter', 'theory', 'computational theory', "non-deterministic", "turing", "machine", "state"]
 license = {file = 'LICENSE.txt'}
 authors = [
     {name = 'Matthew Kanter', email = 'matt@matutu.dev'}
```

### Comparing `automython-1.1.1/setup.py` & `automython-1.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name='automython',
-    version='1.1.1',
+    version='1.1.2',
     description='A simplistic programming language interpreter to Python to help students grasp finite automata theory programmatically and with a computed graph through visualization libraries.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/mkantrr/automython',
     author='Matthew Kanter',
     author_email='matt@matutu.dev',
     license='MIT',
```

### Comparing `automython-1.1.1/src/automython.egg-info/PKG-INFO` & `automython-1.1.2/src/automython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automython
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simplistic programming language interpreter to Python to help students grasp finite automata theory programmatically and with a computed graph through visualization libraries.
 Home-page: https://github.com/mkantrr/automython
 Author: Matthew Kanter
 Author-email: Matthew Kanter <matt@matutu.dev>
 Maintainer-email: Matthew Kanter <matt@matutu.dev>
 License: The MIT License (MIT)
         
@@ -163,15 +163,15 @@
 
 The NFA object in Automython must resemble this syntax:
 ```python
 NFA(states, input_symbols, transitions, initial_state, final_states)
 ```
 It must **also** be assigned to a variable; it cannot be treated as an expression, i.e.:
 ```python
-nfa = NFA(states, input_symbols, transitions, initial_state, final_states, allow_partial[optional]: bool)
+nfa = NFA(states, input_symbols, transitions, initial_state, final_states)
 ```
 
 - The `states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 - The `input_symbols` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 - The `transitions` argument is a Dictionary. This can be either a Dictionary in the argument, or a variable that stores a Dictionary. The values of each key maps to an input symbol as a key to a Set of states.
 - The `initial_state` argument is a String. This can be either a String in the argument, or a variable that stores a String.
 - The `final_states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
```

### Comparing `automython-1.1.1/src/automython.egg-info/SOURCES.txt` & `automython-1.1.2/src/automython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automython-1.1.1/src/interpret/Buffer.py` & `automython-1.1.2/src/interpret/Buffer.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,36 +22,36 @@
 
     @property
     def current_line(self):
         try:
             return self.lines[self.line]
         except IndexError:
             raise EOFError(
-                "EOF reading line {}".format(self.line)
+                "EOF reading line {}".format(self.line + 1)
             )
 
     @property
     def current_char(self):
         try:
             return self.current_line[self.column]
         except IndexError:
             raise EOLError(
                 "EOL reading column {} at line {}".format(
-                    self.column, self.line
+                    self.column + 1, self.line + 1
                 )
             )
             
     @property
     def next_char(self):
         try:
             return self.current_line[self.column + 1]
         except IndexError:
             raise EOLError(
                 "EOL reading column {} at line {}".format(
-                    self.column, self.line
+                    self.column + 1, self.line + 1
                 )
             )
 
     @property
     def tail(self):
         return self.current_line[self.column:]
```

### Comparing `automython-1.1.1/src/interpret/Lexer.py` & `automython-1.1.2/src/interpret/Lexer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,40 @@
 FUNCTION_CALL = 'FUNCTION_CALL'
 
 class TokenError(ValueError):
     """ The expected token cannot be found """
     def __init__(self, msg=""):
         self.msg = msg
         super().__init__(self.msg)
-    
+
+class SyntaxError(SyntaxError):
+    """ The expected token is not the received token and the parsing cannot continue """
+    def __init__(self, msg=""):
+        self.msg = msg
+        super().__init__(self.msg)
+        
+class UnknownError(SyntaxError):
+    """ When all code has run and something has not worked correctly. Mainly used for debugging """
+    def __init__(self, msg=""):
+        self.msg = msg
+        super().__init__(self.msg)
 class Lexer:
     def __init__(self, text=''):
         self._text_storage = buffer.Buffer(text)
         self._status = []
         self._current_token = None
         
     def __enter__(self):
         self.stash()
 
     def __exit__(self, etype, evalue, etrace):
         if etype:
             self.pop()
 
-        if etype in [TokenError]:
+        if etype in [TokenError, SyntaxError]:
             return True
 
     def load(self, text):
         self._text_storage.load(text)
 
     def get_token(self):
         eof = self._process_eof()
@@ -120,19 +131,19 @@
             token = self.get_token()
         self.pop()
 
         return token
      
     @property
     def line(self):
-        return self._text_storage.line 
+        return self._text_storage.line + 1
     
     @property
     def column(self):
-        return self._text_storage.column
+        return self._text_storage.column + 1
     
     @property
     def _current_char(self):
         return self._text_storage.current_char
 
     @property
     def _current_line(self):
```

### Comparing `automython-1.1.1/src/interpret/Parser.py` & `automython-1.1.2/src/interpret/Parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -201,15 +201,19 @@
             
         return t
     
     def parse_print(self):
         t = self.lexer.get_token()
         
         if t.type != fa_lex.PRINT:
-            raise fa_lex.TokenError
+            raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\' at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
        
         return_node = None 
         with self.lexer:
             self._parse_literal(['('])
             node = PrintNode("print_func", self.parse_standalone_func())
             self._parse_literal([')'])
             return_node = node
@@ -235,53 +239,69 @@
         with self.lexer:
             self._parse_literal(['('])
             self._parse_literal([')'])
             node = PrintNode("print_func", ParametersNode([]))
             return_node = node
             
         if not return_node:
-            exception = fa_lex.TokenError(
-                'SyntaxError: Unclosed \'()\' at line {}'.format(
+            exception = fa_lex.SyntaxError(
+                'Incorrect syntax for print() call at line {}'.format(
                     self.lexer.line
                 )
             )
             return exception
         return return_node
     
     def parse_string(self):
         t = self.lexer.get_token()
         
         if t.type != fa_lex.STRING:
-            raise fa_lex.TokenError 
+            raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\' at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
         
         return StringNode(t.value[1:len(t.value)-1])
     
     def parse_number(self):
         t = self.lexer.get_token()
         
         if t.type != fa_lex.INTEGER:
-            raise fa_lex.TokenError
+            raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\' at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
 
         if t.type == fa_lex.INTEGER:
             return IntegerNode(int(t.value))
         
     def parse_boolean(self):
         t = self.lexer.get_token()
         
         if t.type != fa_lex.BOOLEAN:
-            raise fa_lex.TokenError
+            raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\' at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
 
         if t.type == fa_lex.BOOLEAN:
             return BooleanNode(t.value)
     
     def _parse_variable(self):
         t = self.lexer.get_token()
 
         if t.type != fa_lex.VAR:
-            raise fa_lex.TokenError
+            raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\' at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
 
         return VariableNode(t.value)
     
     def parse_assignment(self):
         variable = self._parse_variable()
         self.lexer.discard(token.Token(fa_lex.LITERAL, '='))
        
@@ -291,29 +311,44 @@
             value = self.parse_function()
         elif t.type == fa_lex.DFA or t.type == fa_lex.NFA:
             value = self.parse_fa()
         elif t.type == fa_lex.LITERAL and t.value == '{':
             value = self.parse_collection()
         else:
             value = self.parse_expression()
+            
+        if not value or t == token.Token(fa_lex.EOL) or t == token.Token(fa_lex.EOF):
+            raise fa_lex.SyntaxError(
+                'Assignment has undefined value at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
            
         return AssignmentNode(variable, value)
     
     def _parse_func_name(self):
         t = self.lexer.get_token()
         
         if t.type != fa_lex.FUNCTION_CALL:
-            raise fa_lex.TokenError
+           raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\' at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
         
         return StringNode(t.value)
     
     def _parse_func_parameters(self):
         t = self.lexer.peek_token() 
         if t.type != fa_lex.LITERAL and t.value != '(':
-            raise fa_lex.TokenError
+            raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\' at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
         
         with self.lexer:
             self._parse_literal(['('])
             self._allow_whitespace()
             parameters = self.parse_parameters()
             self._allow_whitespace()
             self._parse_literal([')'])
@@ -332,14 +367,20 @@
             if parameters:
                     return FunctionCallNode(variable, function_name, parameters)
             else:
                 with self.lexer:
                     self._parse_literal(['('])
                     self._parse_literal([')']) 
                     return FunctionCallNode(variable, function_name, ParametersNode([]))
+        else:
+            raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\' at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
                 
     def parse_standalone_func(self):
         t = self.lexer.peek_token()
         if t.type == fa_lex.FUNCTION_CALL:
             with self.lexer:
                 function_name = self._parse_func_name()
             parameters = self._parse_func_parameters()
@@ -348,24 +389,36 @@
                     return FunctionCallNode(StringNode("M"), function_name, parameters)
             else:
                 with self.lexer:
                     self._parse_literal(['('])
                     self._parse_literal([')']) 
                     return FunctionCallNode(StringNode("M"), function_name, ParametersNode([]))
         else:
-            raise fa_lex.TokenError
+            raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\' at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
     
     def _parse_literal(self, values=None):
         t = self.lexer.get_token()
 
         if t.type != fa_lex.LITERAL:
-            raise fa_lex.TokenError
+            raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\' at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
 
         if values and t.value not in values:
-            raise fa_lex.TokenError
+            raise fa_lex.TokenError(
+                'line {}, internal parsing failed, literal value not in parsable array'.format(
+                    self.lexer.line
+                )
+            )
 
         return LiteralNode(t.value)
     
     def parse_factor(self):
         with self.lexer:
             self._parse_literal(['('])
             expression = self.parse_expression()
@@ -388,15 +441,24 @@
         left = self.parse_factor()
 
         with self.lexer:
             operator = self._parse_literal(['+'])
             right = self.parse_expression()
 
             left = BinaryNode(left, operator, right)
-            
+        
+        if isinstance(left, fa_lex.TokenError) \
+            or isinstance(left, fa_lex.SyntaxError):
+                t = self.lexer.get_token()
+                raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\' at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
+                
         return left 
     
     def parse_dictionary(self):
         key = self.parse_expression()
         
         with self.lexer:
             self.lexer.discard(token.Token(fa_lex.LITERAL, ':'))
@@ -431,15 +493,19 @@
                 self._parse_literal(['{'])
                 self._allow_whitespace()
                 collection = self.parse_elements()
                 self._allow_whitespace()
                 self._parse_literal(['}'])
                 return CollectionNode(collection)
         else:
-            raise fa_lex.TokenError
+            raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\' at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
        
     def parse_parameters(self, parameters=None):
         t = self.lexer.peek_token()
         if t.type == fa_lex.LITERAL and t.value == '{':
             left = self.parse_collection()
         else:
             left = self.parse_expression()
@@ -454,15 +520,19 @@
            
         return parameters   
         
     def parse_fa(self):
         t = self.lexer.get_token() 
         
         if t.type not in [fa_lex.DFA, fa_lex.NFA]:
-            raise fa_lex.TokenError
+            raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\', not a supported Automython FA at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
         
         if t.type == fa_lex.DFA:
             with self.lexer:
                 self._parse_literal(['('])
                 self._allow_whitespace()
                 parameters = self.parse_parameters()
                 self._allow_whitespace()
@@ -485,18 +555,28 @@
             
         with self.lexer:
             node = self.parse_print()
         
         with self.lexer:
             node = self.parse_assignment()
             
+        if isinstance(node, fa_lex.TokenError) \
+            or isinstance(node, fa_lex.SyntaxError):
+            raise node
+            
         with self.lexer:
             node = self.parse_function()
             
-        if isinstance(node, fa_lex.TokenError):
+        with self.lexer:
+            node = self.parse_expression()
+            
+        if isinstance(node, fa_lex.TokenError) \
+            or isinstance(node, fa_lex.SyntaxError):
             raise node
         elif node:
             return node
         else:
-            with self.lexer:
-                node = self.parse_expression()
-            return node
+            raise fa_lex.UnknownError(
+                'line {}, the parsed node returned None'.format(
+                    self.lexer.line
+                )
+            )
```

### Comparing `automython-1.1.1/src/interpret/Token.py` & `automython-1.1.2/src/interpret/Token.py`

 * *Files identical despite different names*

### Comparing `automython-1.1.1/src/interpret/Visitor.py` & `automython-1.1.2/src/interpret/Visitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,42 +6,57 @@
       self.printables = []
       self.DFAs = {}
       self.NFAs = {}
       self.DTMs = {}
       self.NTMs = {}
       self.MNTMs = {}
       
+  def visit(self, node):
+      self.visit_helper(node) 
+      
+      for key, value in self.variables.items():
+        if value == None:
+            self.variables.pop(key)
+        
+      for key, value in self.DFAs.items():
+        if value == None:
+            self.DFAs.pop(key)
+            
+      for key, value in self.NFAs.items():
+        if value == None:
+            self.NFAs.pop(key)
+ 
   def isvariable(self, name):
       return name in self.variables
 
   def valueof(self, name):
       if not self.isvariable(name):
           raise KeyError('SyntaxError: ' + name)
       return self.variables[name]['value']
 
   def typeof(self, name):
       if not self.isvariable(name):
           raise KeyError('SyntaxError: ' + name)
       return self.variables[name]['type']
   
-  def visit(self, node):
+  def visit_helper(self, node):
     if node['type'] == 'integer':
         return node['value'], node['type']
     if node['type'] == 'boolean':
         return node['value'], node['type']
     if node['type'] == 'string':
         return node['value'], node['type']
     
     if node['type'] == 'variable':
         return self.valueof(node['value']), self.typeof(node['value'])
 
        
     if node['type'] == 'binary':
-        lvalue, ltype = self.visit(node['left'])
-        rvalue, rtype = self.visit(node['right'])
+        lvalue, ltype = self.visit_helper(node['left'])
+        rvalue, rtype = self.visit_helper(node['right'])
 
         operator = node['operator']['value']
 
         if operator == '+':
             return lvalue + rvalue, rtype
         
     if node['type'] == 'collection':
@@ -49,55 +64,55 @@
         for element in node['value']:
             if element['type'] == 'dictionary':
                 is_dict = True
         if is_dict:
             collection = dict()
             for element in node['value']:
                 if element['type'] == 'variable':
-                    right_value, right_type = self.visit(element)
+                    right_value, right_type = self.visit_helper(element)
                     for key in right_value:
                          collection[key] = right_value[key]
                 else:
-                    right_key, right_value, right_type = self.visit(element)
+                    right_key, right_value, right_type = self.visit_helper(element)
                     collection[right_key] = right_value
             return collection, 'dictionary'
         else:
             collection = set()
             for element in node['value']:
-                right_value, right_type = self.visit(element)
+                right_value, right_type = self.visit_helper(element)
                 collection.add(right_value)
             return collection, node['type']
     
     if node['type'] == 'parameters':
         collection = list()
         for element in node['value']:
-            right_value, right_type = self.visit(element)
+            right_value, right_type = self.visit_helper(element)
             collection.append(right_value)
         return collection, node['type']
   
     if node['type'] == 'dictionary':
-        key_value, key_type = self.visit(node['key'])
-        value_value, value_type = self.visit(node['value'])
+        key_value, key_type = self.visit_helper(node['key'])
+        value_value, value_type = self.visit_helper(node['value'])
         return key_value, value_value, node['type']
     
     if node['type'] == 'print_func':
-        right_value, right_type = self.visit(node['value'])
+        right_value, right_type = self.visit_helper(node['value'])
         if type(right_value) == list and len(right_value) == 0:
             right_value = '' 
         self.printables.append(
             {node['to_print']: {
                 'value': right_value,
                 'type': right_type
             }
         })
 
         return None, None
     
     if node['type'] == 'function_call':
-        right_parameters_value, right_parameters_type = self.visit(node['parameters'])
+        right_parameters_value, right_parameters_type = self.visit_helper(node['parameters'])
         function_name = node['function_name'].asdict()['value']
         default_file = node['variable'] + ".png"
         
         parameters = []
         if function_name not in ['open']:
             parameters.append(self.variables[node['variable']]['value'])
         if function_name in ['open', 'save']:
@@ -111,15 +126,15 @@
             parameters.append(i) 
             
         return getattr(helpers, function_name)(*parameters), node['type']
     
     if node['type'] == 'dfa':
         parameters = list()
         for element in node['value']:
-            right_value, right_type = self.visit(element)
+            right_value, right_type = self.visit_helper(element)
             parameters.append(right_value)
            
         try: 
             if len(parameters) == 6:
                 parameters = helpers.make_DFA(
                                 parameters[0],
                                 parameters[1],
@@ -132,25 +147,30 @@
                 parameters = helpers.make_DFA(
                                 parameters[0],
                                 parameters[1],
                                 parameters[2],
                                 parameters[3],
                                 parameters[4],
                             )
-        except Exception as e:
-            print()
-            print(str(e))
+        except Exception as ex:
+            if isinstance(ex, IndexError):
+                template = "Invalid parameter size for FA\n"
+                print(template)
+            else:
+                template = "An exception of type {0} occurred:\n{1!r}"
+                message = template.format(type(ex).__name__, ex.args[0])
+                print(message)
             return None, None
         
         return parameters, node['type']
     
     if node['type'] == 'nfa':
         parameters = list()
         for element in node['value']:
-            right_value, right_type = self.visit(element)
+            right_value, right_type = self.visit_helper(element)
             parameters.append(right_value)
            
         try: 
             parameters = helpers.make_NFA(
                 parameters[0],
                 parameters[1],
                 parameters[2],
@@ -161,24 +181,25 @@
             print()
             print(str(e))
             return None, None
         
         return parameters, node['type']
         
     if node['type'] == 'assignment':
-        right_value, right_type = self.visit(node['value'])
-        if right_type == 'dfa':
-            self.DFAs[node['variable']] = {
+        right_value, right_type = self.visit_helper(node['value'])
+        if right_value != None and right_type != None:
+            if right_type == 'dfa':
+                self.DFAs[node['variable']] = {
+                    'value': right_value,
+                    'type': right_type
+                }
+            if right_type == 'nfa':
+                self.NFAs[node['variable']] = {
+                    'value': right_value,
+                    'type': right_type
+                } 
+            self.variables[node['variable']] = {
                 'value': right_value,
                 'type': right_type
             }
-        if right_type == 'nfa':
-            self.NFAs[node['variable']] = {
-                'value': right_value,
-                'type': right_type
-            } 
-        self.variables[node['variable']] = {
-            'value': right_value,
-            'type': right_type
-        }
 
         return None, None
```

### Comparing `automython-1.1.1/src/interpret/cli.py` & `automython-1.1.2/src/interpret/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 from IPython.display import display
 
 def cli():
     parser = fa_parse.Parser()
     visitor = fa_visitor.Visitor()
    
-    print('Automython 1.0.3 on ' + str(helpers.system_type())) 
+    print('Automython 1.1.2 on ' + str(helpers.system_type())) 
     print('Enter/Paste your content. Ctrl-D (i.e. EOF) to end input block.')
     while True:
         text = ''
         while True:
             try:
                 line = input('>>> ')
                 if (line in ['exit', 'quit']):
                     print('Use exit() or quit() to exit.')
                     continue
                 if (line in ['exit()', 'quit()']):
                     return
             except EOFError:
-                print(end='')
+                print()
                 break
             except KeyboardInterrupt:
                 print('\n'+'KeyboardInterrupt')
                 continue
             
             text += line + '\n'
             
@@ -41,17 +41,18 @@
         while (t.type != fa_lex.EOF):
             try:
                 node = parser.parse_line()
                 if node:
                     visitor.visit(node.asdict())
             except Exception as ex:
                 template = "An exception of type {0} occurred:\n{1!r}"
-                message = template.format(type(ex).__name__, ex.args)
+                message = template.format(type(ex).__name__, ex.args[0])
                 print(message)
                 break
+            
             t = parser.lexer.peek_token()
             if (t.type == fa_lex.EOL):
                 t = parser.lexer.get_token()
                 t = parser.lexer.peek_token()
                 while (t.type == fa_lex.EOL):
                     if t.type == fa_lex.EOL:
                         t = parser.lexer.get_token()
```

### Comparing `automython-1.1.1/src/interpret/file_interface.py` & `automython-1.1.2/src/interpret/file_interface.py`

 * *Files 17% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     
   except EOFError:
     sys.exit(0)
   
   except Exception as ex:
     print()
     template = "An exception of type {0} occurred:\n{1!r}"
-    message = template.format(type(ex).__name__, ex.args)
+    message = template.format(type(ex).__name__, ex.args[0])
     print(message)
     
   if error_flag:
     sys.exit(1)
     
 if __name__ == '__main__':
   if len(sys.argv) == 2 and sys.argv[1].lower().endswith('.theory'):
```

### Comparing `automython-1.1.1/src/interpret/helpers.py` & `automython-1.1.2/src/interpret/helpers.py`

 * *Files identical despite different names*

### Comparing `automython-1.1.1/src/interpret/interpreter.py` & `automython-1.1.2/src/interpret/interpreter.py`

 * *Files identical despite different names*

