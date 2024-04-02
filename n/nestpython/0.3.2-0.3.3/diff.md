# Comparing `tmp/nestpython-0.3.2.tar.gz` & `tmp/nestpython-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestpython-0.3.2.tar", last modified: Mon Apr  1 18:03:02 2024, max compression
+gzip compressed data, was "nestpython-0.3.3.tar", last modified: Mon Apr  1 19:57:42 2024, max compression
```

## Comparing `nestpython-0.3.2.tar` & `nestpython-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 18:03:02.659628 nestpython-0.3.2/
--rw-rw-rw-   0        0        0     1346 2024-04-01 18:03:02.658607 nestpython-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1141 2024-04-01 17:19:29.000000 nestpython-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 18:03:02.650630 nestpython-0.3.2/nestpy/
--rw-rw-rw-   0        0        0       39 2024-04-01 14:53:49.000000 nestpython-0.3.2/nestpy/__init__.py
--rw-rw-rw-   0        0        0     2340 2024-04-01 14:53:49.000000 nestpython-0.3.2/nestpy/files.py
--rw-rw-rw-   0        0        0    14523 2024-04-01 17:49:57.000000 nestpython-0.3.2/nestpy/main.py
-drwxrwxrwx   0        0        0        0 2024-04-01 18:03:02.656612 nestpython-0.3.2/nestpython.egg-info/
--rw-rw-rw-   0        0        0     1346 2024-04-01 18:03:02.000000 nestpython-0.3.2/nestpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-01 18:03:02.000000 nestpython-0.3.2/nestpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 18:03:02.000000 nestpython-0.3.2/nestpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 18:03:02.000000 nestpython-0.3.2/nestpython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 18:03:02.660606 nestpython-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      856 2024-04-01 17:25:34.000000 nestpython-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:57:42.525471 nestpython-0.3.3/
+-rw-rw-rw-   0        0        0     1346 2024-04-01 19:57:42.524471 nestpython-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:57:41.000000 nestpython-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 19:57:42.517901 nestpython-0.3.3/nestpy/
+-rw-rw-rw-   0        0        0       39 2024-04-01 14:53:49.000000 nestpython-0.3.3/nestpy/__init__.py
+-rw-rw-rw-   0        0        0     2340 2024-04-01 14:53:49.000000 nestpython-0.3.3/nestpy/files.py
+-rw-rw-rw-   0        0        0    14129 2024-04-01 19:56:44.000000 nestpython-0.3.3/nestpy/main.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:57:42.522889 nestpython-0.3.3/nestpython.egg-info/
+-rw-rw-rw-   0        0        0     1346 2024-04-01 19:57:42.000000 nestpython-0.3.3/nestpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-01 19:57:42.000000 nestpython-0.3.3/nestpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 19:57:42.000000 nestpython-0.3.3/nestpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-01 19:57:42.000000 nestpython-0.3.3/nestpython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 19:57:42.525471 nestpython-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2024-04-01 18:32:02.000000 nestpython-0.3.3/setup.py
```

### Comparing `nestpython-0.3.2/PKG-INFO` & `nestpython-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestpython
-Version: 0.3.2
+Version: 0.3.3
 Summary: python with braces.
 Author: slycedf
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 
 ## nestpy
```

### Comparing `nestpython-0.3.2/README.md` & `nestpython-0.3.3/nestpython.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: nestpython
+Version: 0.3.3
+Summary: python with braces.
+Author: slycedf
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Description-Content-Type: text/markdown
+
 ## nestpy
 
 
 *"what if python, with braces, one line?"*
 
 # SETUP
```

### Comparing `nestpython-0.3.2/nestpy/files.py` & `nestpython-0.3.3/nestpy/files.py`

 * *Files identical despite different names*

### Comparing `nestpython-0.3.2/nestpy/main.py` & `nestpython-0.3.3/nestpy/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -115,17 +115,17 @@
     defDeconflict = Token(sclund('def'), TokenTypes.APPENDSUB)
     lambdaDeconflict = Token(sclund('lambda'), TokenTypes.APPENDSUB)
     inDeconflict = Token(sclund('in'), TokenTypes.APPENDSUB)
     returnDeconflict = Token(sclund('return'), TokenTypes.APPENDSUB)
     caseDeconflict = Token(sclund('case'), TokenTypes.APPENDSUB)
     delDeconflict = Token(sclund('del'), TokenTypes.APPENDSUB)
     passDeconflict = Token(sclund('pass'), TokenTypes.APPENDSUB)
-    commentLeft = Token(r'/\*')
-    commentRight = Token(r'\*/', TokenTypes.INDENTED)
-    commentLine = Token(r'//', TokenTypes.MAP)
+    comment = Token(r'\/\*[\s\S]*\*\/', TokenTypes.INDENTED)
+    lineComment = Token(r'\/\/.*', TokenTypes.INDENTED)
+    lineStatement = Token(r'/\|.*\|\\', TokenTypes.INDENTED)
     intDiv = Token(r'~/', TokenTypes.MAP)
     caseShorthand = Token(r'\?', TokenTypes.SHORTHAND)
     macroDefine = Token(r'#\s*[\w\n]+\s*#\s*<[\s\S]*>\s*#', TokenTypes.MACROS)
     macroUndefine = Token(r'#~\s*[\w\n]+\s*~#', TokenTypes.MACROS)
     macroIfdef = Token(r'#\?\s*[\w\n]*\s*\?#', TokenTypes.MACROS)
     macroAccess = Token(r'\$[\w\n]*', TokenTypes.MACROS)
     macro = Token('#', TokenTypes.SYNTACTICAL)
@@ -144,15 +144,14 @@
       Tokens.defShorthand.value.id: 'def',
       Tokens.inShorthand.value.id: 'in',
       Tokens.caseShorthand.value.id: 'case',
       Tokens.notInShorthand.value.id: 'not in',
       Tokens.returnShorthand.value.id: 'return',
       Tokens.lambdaShorthand.value.id: 'lambda',
       Tokens.delShorthand.value.id: 'del',
-      Tokens.commentLine.value.id: '#',
       Tokens.intDiv.value.id: '//'
   }
 
   def isF(token, ptoken):
     with contextlib.suppress(TypeError):
       return (TokenTypes.STRING in token.types) and (ptoken.symb[~0].lower() == 'f' or
                                                      ptoken.symb[~1:].lower() == 'fr')
@@ -178,16 +177,14 @@
 
   compiled_code = ''
   indent_level = 0
   in_multilineStringSingle = False
   in_multilineStringDouble = False
   in_stringSingle = False
   in_stringDouble = False
-  in_comment = False
-  in_line_comment = False
   in_fstring = False
   in_rstring = False
   fstring_indent_level = None
   in_fstringComp = False
   in_multilineString = lambda: (in_multilineStringSingle or
                                 in_multilineStringDouble)
   in_string = lambda: (in_multilineString() or in_stringDouble or
@@ -204,16 +201,14 @@
   def compile(bufferToken):
     nonlocal compiled_code
     nonlocal indent_level 
     nonlocal in_multilineStringSingle
     nonlocal in_multilineStringDouble
     nonlocal in_stringSingle
     nonlocal in_stringDouble
-    nonlocal in_comment
-    nonlocal in_line_comment
     nonlocal in_fstring
     nonlocal in_rstring
     nonlocal fstring_indent_level
     nonlocal in_fstringComp
     nonlocal in_multilineString
     nonlocal in_string
     nonlocal compilable
@@ -222,45 +217,32 @@
     nonlocal buffer
     nonlocal compiling
     nonlocal ptoken
     try:
      for n, token in enumerate(tokens):
       ptoken = tokens[n - 1] if n > 0 else bufferToken
       match token.id:       
-        case Tokens.commentLeft.value.id:
-          in_comment = True
+        case Tokens.comment.value.id | Tokens.lineComment.value.id:
+          print(token.symb)
           continue
-        case Tokens.commentRight.value.id:
-          in_comment = False
+        case Tokens.lineStatement.value.id:
+          compiled_code += '#' + token.symb[2:-2].rstrip() + '\n' + indent * indent_level
           continue
-        case Tokens.commentLine.value.id:
-          in_line_comment = True
-          compiled_code += '#'
-          continue
-        case Tokens.newline.value.id if in_line_comment:
-          in_line_comment = False
-          compiled_code += '\n'
-          continue
-      if in_comment:
-        continue
-      if in_line_comment:
-        compiled_code += token.symb
-        continue
       if isNRawEscapedEscape(token):
         compiled_code += '\\'
       if (token.id == Tokens.indentLeftDouble.value.id 
           and (not in_fstring 
           or in_fstringComp)):
         tokens = [Tokens.indentLeft.value]*2 + tokens[n + 1:]
         raise breakout
       if token.id == Tokens.indentSelfClose.value.id:
         if compilable():
-          compiled_code = (compiled_code.rstrip() 
+          compiled_code = (compiled_code.rstrip()
                            + f':\n{indent * (indent_level+1)}\
-pass\n{indent * (indent_level)}')
+pass\n{indent * indent_level}')
           continue
         else:
           tokens = ([Tokens.indentLeft.value] 
           + tokenize(token.symb[1:-1], [t.value for t in Tokens], buffer) 
           + [Tokens.indentRight.value]
           + tokens[n + 1:])
           raise breakout
```

### Comparing `nestpython-0.3.2/setup.py` & `nestpython-0.3.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from setuptools import find_packages, setup
 from os import path as osp, system as runcmd
 
+def parse(filename):
+    return osp.join(osp.dirname(__file__), filename)
+
 def read(filename):
-    return open(osp.join(osp.dirname(__file__), filename)).read()
+    return open(parse(filename), 'r').read()
 
 
 param = eval(read('param.i'))
 
 version = param['version']
 test = param['test']
-setup(
-    name='nestpython',
-    packages=find_packages(include=['nestpy']),
-    version=version,
-    description='python with braces.',
-    author='slycedf',
-    license='MIT',
-    long_description=read('README.md'),
-    long_description_content_type='text/markdown',
-    classifiers=[
-        "Development Status :: 4 - Beta"
-    ]
-)
+
+with open(parse('../README.md'), 'r') as f, open(parse('README.md'), 'w') as fn:
+    readme = f.read()
+    fn.write(readme)
+
+    setup(
+        name='nestpython',
+        packages=find_packages(include=['nestpy']),
+        version=version,
+        description='python with braces.',
+        author='slycedf',
+        license='MIT',
+        long_description=readme,
+        long_description_content_type='text/markdown',
+        classifiers=[
+            "Development Status :: 4 - Beta"
+        ]
+    )
 
 token = open(f'D:/slycefolder/ins/nsp/{ {True: "tt", False: "tr"}[test]}', 'r').read()
 
 runcmd(
     f'pause & twine upload --repository { {True: "testpypi", False: "pypi"}[test]} dist/*{version}* -u __token__ -p {token} --verbose')
```

