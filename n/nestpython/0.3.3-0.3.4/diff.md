# Comparing `tmp/nestpython-0.3.3.tar.gz` & `tmp/nestpython-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestpython-0.3.3.tar", last modified: Mon Apr  1 19:57:42 2024, max compression
+gzip compressed data, was "nestpython-0.3.4.tar", last modified: Tue Apr  2 11:07:16 2024, max compression
```

## Comparing `nestpython-0.3.3.tar` & `nestpython-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 19:57:42.525471 nestpython-0.3.3/
--rw-rw-rw-   0        0        0     1346 2024-04-01 19:57:42.524471 nestpython-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-01 19:57:41.000000 nestpython-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 19:57:42.517901 nestpython-0.3.3/nestpy/
--rw-rw-rw-   0        0        0       39 2024-04-01 14:53:49.000000 nestpython-0.3.3/nestpy/__init__.py
--rw-rw-rw-   0        0        0     2340 2024-04-01 14:53:49.000000 nestpython-0.3.3/nestpy/files.py
--rw-rw-rw-   0        0        0    14129 2024-04-01 19:56:44.000000 nestpython-0.3.3/nestpy/main.py
-drwxrwxrwx   0        0        0        0 2024-04-01 19:57:42.522889 nestpython-0.3.3/nestpython.egg-info/
--rw-rw-rw-   0        0        0     1346 2024-04-01 19:57:42.000000 nestpython-0.3.3/nestpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-01 19:57:42.000000 nestpython-0.3.3/nestpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 19:57:42.000000 nestpython-0.3.3/nestpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 19:57:42.000000 nestpython-0.3.3/nestpython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 19:57:42.525471 nestpython-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1085 2024-04-01 18:32:02.000000 nestpython-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:07:16.346132 nestpython-0.3.4/
+-rw-rw-rw-   0        0        0     1346 2024-04-02 11:07:16.342166 nestpython-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-02 11:07:15.000000 nestpython-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 11:07:16.334166 nestpython-0.3.4/nestpy/
+-rw-rw-rw-   0        0        0       39 2024-04-01 14:53:49.000000 nestpython-0.3.4/nestpy/__init__.py
+-rw-rw-rw-   0        0        0     2340 2024-04-01 14:53:49.000000 nestpython-0.3.4/nestpy/files.py
+-rw-rw-rw-   0        0        0    14604 2024-04-02 11:06:29.000000 nestpython-0.3.4/nestpy/main.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:07:16.340148 nestpython-0.3.4/nestpython.egg-info/
+-rw-rw-rw-   0        0        0     1346 2024-04-02 11:07:16.000000 nestpython-0.3.4/nestpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-02 11:07:16.000000 nestpython-0.3.4/nestpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 11:07:16.000000 nestpython-0.3.4/nestpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 11:07:16.000000 nestpython-0.3.4/nestpython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 11:07:16.346132 nestpython-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2024-04-01 18:32:02.000000 nestpython-0.3.4/setup.py
```

### Comparing `nestpython-0.3.3/PKG-INFO` & `nestpython-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestpython
-Version: 0.3.3
+Version: 0.3.4
 Summary: python with braces.
 Author: slycedf
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 
 ## nestpy
```

### Comparing `nestpython-0.3.3/nestpy/files.py` & `nestpython-0.3.4/nestpy/files.py`

 * *Files identical despite different names*

### Comparing `nestpython-0.3.3/nestpy/main.py` & `nestpython-0.3.4/nestpy/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,17 +67,14 @@
       j += 1
     if i < len(string):
       tokenized.append(anonToken(string[i:]))
     return tokenized
 
   # TOKEN DECLARATIONS
 
-  def sclude(regex):
-    return r'(?<![\w0-9])' + regex + r'(?![\w0-9])'
-
   def sclund(regex):
     return r'(?<![\w0-9])' + regex + r'_*(?![\w0-9])'
 
   macros = {}
 
   class Tokens(Enum):
     escape = Token(r'\\', TokenTypes.ESCAPEMENT)
@@ -181,56 +178,57 @@
   in_multilineStringDouble = False
   in_stringSingle = False
   in_stringDouble = False
   in_fstring = False
   in_rstring = False
   fstring_indent_level = None
   in_fstringComp = False
+  in_fstringCompString = False
   in_multilineString = lambda: (in_multilineStringSingle or
                                 in_multilineStringDouble)
   in_string = lambda: (in_multilineString() or in_stringDouble or
                        in_stringSingle)
-  compilable = lambda: ((not in_string()) or in_fstringComp)
+  compilable = lambda: ((not in_string()) or (in_fstringComp and not in_fstringCompString))
   indent = ' ' * indent_amount
   buffer = 1
   tokens = tokenize(modified_code, [t.value for t in Tokens], buffer)
   compiling = True
   ptoken = Token()
-
   class breakout(Exception):
     pass
   def compile(bufferToken):
     nonlocal compiled_code
     nonlocal indent_level 
     nonlocal in_multilineStringSingle
     nonlocal in_multilineStringDouble
     nonlocal in_stringSingle
     nonlocal in_stringDouble
     nonlocal in_fstring
     nonlocal in_rstring
     nonlocal fstring_indent_level
     nonlocal in_fstringComp
+    nonlocal in_fstringCompString
     nonlocal in_multilineString
     nonlocal in_string
     nonlocal compilable
     nonlocal indent
     nonlocal tokens
     nonlocal buffer
     nonlocal compiling
     nonlocal ptoken
     try:
      for n, token in enumerate(tokens):
       ptoken = tokens[n - 1] if n > 0 else bufferToken
-      match token.id:       
-        case Tokens.comment.value.id | Tokens.lineComment.value.id:
-          print(token.symb)
-          continue
-        case Tokens.lineStatement.value.id:
-          compiled_code += '#' + token.symb[2:-2].rstrip() + '\n' + indent * indent_level
-          continue
+      if compilable():
+        match token.id:
+          case Tokens.comment.value.id | Tokens.lineComment.value.id:
+            continue
+          case Tokens.lineStatement.value.id:
+            compiled_code += '#' + token.symb[2:-2].rstrip() + '\n' + indent * indent_level
+            continue
       if isNRawEscapedEscape(token):
         compiled_code += '\\'
       if (token.id == Tokens.indentLeftDouble.value.id 
           and (not in_fstring 
           or in_fstringComp)):
         tokens = [Tokens.indentLeft.value]*2 + tokens[n + 1:]
         raise breakout
@@ -278,28 +276,36 @@
             tokens = tokenize(macro, [t.value for t in Tokens], buffer) + tokens[n + 1:]
             raise breakout
           else:
             compiled_code += (token.symb if in_multilineString() 
                               else token.symb.replace('\n', ''))
       if TokenTypes.STRING in token.types:
         match token.id:
-          case Tokens.multilineStringSingle.value.id if not in_multilineStringDouble:
+          case Tokens.multilineStringSingle.value.id if not in_multilineStringDouble or in_fstringComp:
             in_multilineStringSingle = not in_multilineStringSingle
-          case Tokens.multilineStringDouble.value.id if not in_multilineStringSingle:
+            if in_fstringComp:
+              in_fstringCompString = not in_fstringCompString
+          case Tokens.multilineStringDouble.value.id if not in_multilineStringSingle or in_fstringComp:
             in_multilineStringDouble = not in_multilineStringDouble
-          case Tokens.stringDouble.value.id if not (in_multilineString()
-                                                    or in_stringSingle):
+            if in_fstringComp:
+              in_fstringCompString = not in_fstringCompString
+          case Tokens.stringDouble.value.id if (not (in_multilineString()
+                                                    or in_stringSingle) or in_fstringComp):
             if not isNRawEscape(ptoken):
              in_stringDouble = not in_stringDouble
+             if in_fstringComp:
+               in_fstringCompString = not in_fstringCompString
             else:
              compiled_code += token.symb
              continue
-          case Tokens.stringSingle.value.id if not (in_multilineString()
-                                                    or in_stringDouble):
+          case Tokens.stringSingle.value.id if (not (in_multilineString()
+                                                    or in_stringDouble or in_fstringComp)):
             if not isNRawEscape(ptoken):
+              if in_fstringComp:
+                in_fstringCompString = not in_fstringCompString
               in_stringSingle = not in_stringSingle
             else:
               compiled_code += token.symb
               continue
         in_fstring = in_string() and isF(token, ptoken)
         in_rstring = in_string() and isR(token, ptoken)
       if compilable():
```

### Comparing `nestpython-0.3.3/nestpython.egg-info/PKG-INFO` & `nestpython-0.3.4/nestpython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestpython
-Version: 0.3.3
+Version: 0.3.4
 Summary: python with braces.
 Author: slycedf
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 
 ## nestpy
```

### Comparing `nestpython-0.3.3/setup.py` & `nestpython-0.3.4/setup.py`

 * *Files identical despite different names*

