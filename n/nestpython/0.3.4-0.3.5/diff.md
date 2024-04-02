# Comparing `tmp/nestpython-0.3.4.tar.gz` & `tmp/nestpython-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestpython-0.3.4.tar", last modified: Tue Apr  2 11:07:16 2024, max compression
+gzip compressed data, was "nestpython-0.3.5.tar", last modified: Tue Apr  2 19:32:18 2024, max compression
```

## Comparing `nestpython-0.3.4.tar` & `nestpython-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 11:07:16.346132 nestpython-0.3.4/
--rw-rw-rw-   0        0        0     1346 2024-04-02 11:07:16.342166 nestpython-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-02 11:07:15.000000 nestpython-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 11:07:16.334166 nestpython-0.3.4/nestpy/
--rw-rw-rw-   0        0        0       39 2024-04-01 14:53:49.000000 nestpython-0.3.4/nestpy/__init__.py
--rw-rw-rw-   0        0        0     2340 2024-04-01 14:53:49.000000 nestpython-0.3.4/nestpy/files.py
--rw-rw-rw-   0        0        0    14604 2024-04-02 11:06:29.000000 nestpython-0.3.4/nestpy/main.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:07:16.340148 nestpython-0.3.4/nestpython.egg-info/
--rw-rw-rw-   0        0        0     1346 2024-04-02 11:07:16.000000 nestpython-0.3.4/nestpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-02 11:07:16.000000 nestpython-0.3.4/nestpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 11:07:16.000000 nestpython-0.3.4/nestpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 11:07:16.000000 nestpython-0.3.4/nestpython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 11:07:16.346132 nestpython-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1085 2024-04-01 18:32:02.000000 nestpython-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:32:18.099998 nestpython-0.3.5/
+-rw-rw-rw-   0        0        0     1346 2024-04-02 19:32:18.098008 nestpython-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-02 19:32:17.000000 nestpython-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 19:32:18.090026 nestpython-0.3.5/nestpy/
+-rw-rw-rw-   0        0        0       39 2024-04-01 14:53:49.000000 nestpython-0.3.5/nestpy/__init__.py
+-rw-rw-rw-   0        0        0     2340 2024-04-01 14:53:49.000000 nestpython-0.3.5/nestpy/files.py
+-rw-rw-rw-   0        0        0    14122 2024-04-02 19:29:51.000000 nestpython-0.3.5/nestpy/main.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:32:18.096008 nestpython-0.3.5/nestpython.egg-info/
+-rw-rw-rw-   0        0        0     1346 2024-04-02 19:32:17.000000 nestpython-0.3.5/nestpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-02 19:32:17.000000 nestpython-0.3.5/nestpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 19:32:17.000000 nestpython-0.3.5/nestpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 19:32:17.000000 nestpython-0.3.5/nestpython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 19:32:18.099998 nestpython-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2024-04-01 18:32:02.000000 nestpython-0.3.5/setup.py
```

### Comparing `nestpython-0.3.4/PKG-INFO` & `nestpython-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestpython
-Version: 0.3.4
+Version: 0.3.5
 Summary: python with braces.
 Author: slycedf
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 
 ## nestpy
```

### Comparing `nestpython-0.3.4/nestpy/files.py` & `nestpython-0.3.5/nestpy/files.py`

 * *Files identical despite different names*

### Comparing `nestpython-0.3.4/nestpy/main.py` & `nestpython-0.3.5/nestpy/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     indentLeftDouble = Token(r'{{')
     indentSelfClose = Token(r'{\s*}', TokenTypes.INDENTED, TokenTypes.SYNTACTICAL)
     indentLeft = Token(r'{', TokenTypes.INDENTED, TokenTypes.SYNTACTICAL)
     indentRight = Token(r'}', TokenTypes.INDENTED, TokenTypes.SYNTACTICAL)
     newline = Token(r'\n', TokenTypes.INDENTED, TokenTypes.MISS)
     returnShorthand = Token(r'=>', TokenTypes.SHORTHAND)
     nativeSemicolon = Token(r',,', TokenTypes.MAP)
+    nativeAssignment = Token(r'<-', TokenTypes.MAP)
     andShorthand = Token(r'&&', TokenTypes.SHORTHAND)
     orShorthand = Token(r'\|\|', TokenTypes.SHORTHAND)
     isShorthand = Token(r'=&', TokenTypes.SHORTHAND)
     isNotShorthand = Token(r'!=&', TokenTypes.SHORTHAND)
     defShorthand = Token(r':=', TokenTypes.SHORTHAND)
     inShorthand = Token(r'->', TokenTypes.SHORTHAND)
     notInShorthand = Token(r'!>', TokenTypes.SHORTHAND)
@@ -129,14 +130,15 @@
 
     # CONVERSION TOKEN MAPPING
 
   tokenMap = {
       Tokens.dictIndentLeft.value.id: '{',
       Tokens.dictIndentRight.value.id: '}',
       Tokens.nativeSemicolon.value.id: ';',
+      Tokens.nativeAssignment.value.id: '<-',
       Tokens.andShorthand.value.id: 'and',
       Tokens.orShorthand.value.id: 'or',
       Tokens.notShorthand.value.id: 'not',
       Tokens.isShorthand.value.id: 'is',
       Tokens.isNotShorthand.value.id: 'is not',
       Tokens.defShorthand.value.id: 'def',
       Tokens.inShorthand.value.id: 'in',
@@ -170,47 +172,66 @@
     return isEscape(token) and not in_rstring
 
   def isNRawEscapedEscape(token):
     return isEscapedEscape(token) and not in_rstring
 
   compiled_code = ''
   indent_level = 0
-  in_multilineStringSingle = False
-  in_multilineStringDouble = False
-  in_stringSingle = False
-  in_stringDouble = False
+  string_nesting = []
+  def getStringType():
+    return anonToken('') if len(string_nesting) == 0 else string_nesting[~0]
+  fstring_nesting = 0
+  in_multilineStringSingle = lambda: getStringType().id == Tokens.multilineStringSingle.value.id and in_string
+  in_multilineStringDouble = lambda: getStringType().id == Tokens.multilineStringDouble.value.id and in_string
+  in_stringSingle = lambda: getStringType().id == Tokens.stringSingle.value.id and in_string
+  in_stringDouble = lambda: getStringType().id == Tokens.stringDouble.value.id and in_string
   in_fstring = False
   in_rstring = False
-  fstring_indent_level = None
-  in_fstringComp = False
-  in_fstringCompString = False
-  in_multilineString = lambda: (in_multilineStringSingle or
-                                in_multilineStringDouble)
-  in_string = lambda: (in_multilineString() or in_stringDouble or
-                       in_stringSingle)
-  compilable = lambda: ((not in_string()) or (in_fstringComp and not in_fstringCompString))
+  in_multilineString = lambda: (in_multilineStringSingle() or
+                                in_multilineStringDouble())
+  in_string = False
+  compilable = lambda: not in_string
+
+  def string_compilable(token):
+    match token.id:
+      case Tokens.multilineStringSingle.value.id:
+        return not in_multilineStringDouble()
+      case Tokens.multilineStringDouble.value.id:
+        return not in_multilineStringSingle()
+      case Tokens.stringSingle.value.id:
+        return not (in_multilineString() or in_stringDouble())
+      case Tokens.stringDouble.value.id:
+        return not (in_multilineString() or in_stringSingle())
+
   indent = ' ' * indent_amount
   buffer = 1
   tokens = tokenize(modified_code, [t.value for t in Tokens], buffer)
   compiling = True
   ptoken = Token()
   class breakout(Exception):
     pass
+
+  def string_compile(token):
+    nonlocal in_string
+    if getStringType().id == token.id:
+      string_nesting.pop()
+    else:
+      string_nesting.append(token)
+    in_string = not in_string
+
   def compile(bufferToken):
     nonlocal compiled_code
     nonlocal indent_level 
     nonlocal in_multilineStringSingle
     nonlocal in_multilineStringDouble
     nonlocal in_stringSingle
     nonlocal in_stringDouble
     nonlocal in_fstring
     nonlocal in_rstring
-    nonlocal fstring_indent_level
-    nonlocal in_fstringComp
-    nonlocal in_fstringCompString
+    nonlocal fstring_nesting
     nonlocal in_multilineString
     nonlocal in_string
     nonlocal compilable
     nonlocal indent
     nonlocal tokens
     nonlocal buffer
     nonlocal compiling
@@ -224,16 +245,15 @@
             continue
           case Tokens.lineStatement.value.id:
             compiled_code += '#' + token.symb[2:-2].rstrip() + '\n' + indent * indent_level
             continue
       if isNRawEscapedEscape(token):
         compiled_code += '\\'
       if (token.id == Tokens.indentLeftDouble.value.id 
-          and (not in_fstring 
-          or in_fstringComp)):
+          and not in_fstring):
         tokens = [Tokens.indentLeft.value]*2 + tokens[n + 1:]
         raise breakout
       if token.id == Tokens.indentSelfClose.value.id:
         if compilable():
           compiled_code = (compiled_code.rstrip()
                            + f':\n{indent * (indent_level+1)}\
 pass\n{indent * indent_level}')
@@ -274,71 +294,49 @@
           if compilable():
             macro = macros[token.symb[1:].replace('\n', '')][0]
             tokens = tokenize(macro, [t.value for t in Tokens], buffer) + tokens[n + 1:]
             raise breakout
           else:
             compiled_code += (token.symb if in_multilineString() 
                               else token.symb.replace('\n', ''))
-      if TokenTypes.STRING in token.types:
-        match token.id:
-          case Tokens.multilineStringSingle.value.id if not in_multilineStringDouble or in_fstringComp:
-            in_multilineStringSingle = not in_multilineStringSingle
-            if in_fstringComp:
-              in_fstringCompString = not in_fstringCompString
-          case Tokens.multilineStringDouble.value.id if not in_multilineStringSingle or in_fstringComp:
-            in_multilineStringDouble = not in_multilineStringDouble
-            if in_fstringComp:
-              in_fstringCompString = not in_fstringCompString
-          case Tokens.stringDouble.value.id if (not (in_multilineString()
-                                                    or in_stringSingle) or in_fstringComp):
-            if not isNRawEscape(ptoken):
-             in_stringDouble = not in_stringDouble
-             if in_fstringComp:
-               in_fstringCompString = not in_fstringCompString
-            else:
-             compiled_code += token.symb
-             continue
-          case Tokens.stringSingle.value.id if (not (in_multilineString()
-                                                    or in_stringDouble or in_fstringComp)):
-            if not isNRawEscape(ptoken):
-              if in_fstringComp:
-                in_fstringCompString = not in_fstringCompString
-              in_stringSingle = not in_stringSingle
-            else:
-              compiled_code += token.symb
-              continue
-        in_fstring = in_string() and isF(token, ptoken)
-        in_rstring = in_string() and isR(token, ptoken)
+      if TokenTypes.STRING in token.types and string_compilable(token):
+        if not isNRawEscape(ptoken):
+          string_compile(token)
+        in_fstring = in_string and isF(token, ptoken)
+        in_rstring = in_string and isR(token, ptoken)
       if compilable():
+       if fstring_nesting == 0:
         match token.id:
           case Tokens.indentLeft.value.id | Tokens.indentLeftNoColon.value.id:
             indent_level += 1
             compiled_code = compiled_code.rstrip()
             compiled_code += ((':' if token.id == Tokens.indentLeft.value.id 
                               else (
                                 f'\n{indent * (indent_level-1)}if True:'
                               )) + '\n' + indent * indent_level
                              )
           case Tokens.indentRight.value.id:
-            if indent_level == fstring_indent_level:
-              in_fstringComp = False
-              fstring_indent_level = None
-            else:
-              indent_level -= 1
-              for macro in list(macros):
-                if macros[macro][1] > indent_level:
-                  macros.pop(macro)
-              compiled_code += '\n' + indent * indent_level
+            indent_level -= 1
+            for macro in list(macros):
+              if macros[macro][1] > indent_level:
+                macros.pop(macro)
+            compiled_code += '\n' + indent * indent_level
           case Tokens.indentNewline.value.id:
             compiled_code += '\n' + indent * indent_level
-      elif in_fstring and not in_fstringComp:
+       elif token.id == Tokens.indentRight.value.id:
+        fstring_nesting -= 1
+        in_fstring = True
+        in_string = True
+
+      elif in_fstring:
         match token.id:
           case Tokens.indentLeft.value.id:
-            in_fstringComp = True
-            fstring_indent_level = indent_level
+            in_fstring = False
+            in_string = False
+            fstring_nesting += 1
             compiled_code += token.symb
           case Tokens.indentRight.value.id:
             if tokens[n+1].id == token.id:
               compiled_code += token.symb * 2
               tokens = tokens[n+2:]
               raise breakout
       if (not (TokenTypes.SYNTACTICAL in token.types and compilable())
```

### Comparing `nestpython-0.3.4/nestpython.egg-info/PKG-INFO` & `nestpython-0.3.5/nestpython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestpython
-Version: 0.3.4
+Version: 0.3.5
 Summary: python with braces.
 Author: slycedf
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 
 ## nestpy
```

### Comparing `nestpython-0.3.4/setup.py` & `nestpython-0.3.5/setup.py`

 * *Files identical despite different names*

