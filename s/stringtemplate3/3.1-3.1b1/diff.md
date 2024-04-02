# Comparing `tmp/stringtemplate3-3.1.tar.gz` & `tmp/stringtemplate3-3.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringtemplate3-3.1.tar", last modified: Sun Feb 17 22:32:23 2008, max compression, from Unix
+gzip compressed data, was "stringtemplate3-3.1b1.tar", last modified: Tue Dec  4 06:46:01 2007, max compression, from Unix
```

## Comparing `stringtemplate3-3.1.tar` & `stringtemplate3-3.1b1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 pink      (1000) users      (100)        0 2008-02-17 22:32:23.000000 stringtemplate3-3.1/
--rw-r--r--   0 pink      (1000) users      (100)     1160 2008-02-17 22:32:23.000000 stringtemplate3-3.1/PKG-INFO
--r--r--r--   0 pink      (1000) users      (100)     1685 2008-02-17 22:30:42.000000 stringtemplate3-3.1/README.txt
-drwxr-xr-x   0 pink      (1000) users      (100)        0 2008-02-17 22:32:23.000000 stringtemplate3-3.1/stringtemplate3/
--r--r--r--   0 pink      (1000) users      (100)     6299 2008-02-17 22:30:43.000000 stringtemplate3-3.1/stringtemplate3/interfaces.py
-drwxr-xr-x   0 pink      (1000) users      (100)        0 2008-02-17 22:32:23.000000 stringtemplate3-3.1/stringtemplate3/language/
--r--r--r--   0 pink      (1000) users      (100)    32650 2008-02-17 22:30:43.000000 stringtemplate3-3.1/stringtemplate3/language/ASTExpr.py
--r--r--r--   0 pink      (1000) users      (100)    29889 2008-02-17 22:30:43.000000 stringtemplate3-3.1/stringtemplate3/language/ActionEvaluator.py
--r--r--r--   0 pink      (1000) users      (100)      848 2008-02-17 22:30:43.000000 stringtemplate3-3.1/stringtemplate3/language/ChunkToken.py
--r--r--r--   0 pink      (1000) users      (100)    18411 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/language/GroupParser.py
--r--r--r--   0 pink      (1000) users      (100)    26704 2008-02-17 22:30:43.000000 stringtemplate3-3.1/stringtemplate3/language/ActionLexer.py
--r--r--r--   0 pink      (1000) users      (100)      456 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/language/StringTemplateAST.py
--r--r--r--   0 pink      (1000) users      (100)    42455 2008-02-17 22:30:43.000000 stringtemplate3-3.1/stringtemplate3/language/AngleBracketTemplateLexer.py
--r--r--r--   0 pink      (1000) users      (100)     9848 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/language/TemplateParser.py
--r--r--r--   0 pink      (1000) users      (100)      823 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/language/StringRef.py
--r--r--r--   0 pink      (1000) users      (100)      366 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/language/NewlineRef.py
--r--r--r--   0 pink      (1000) users      (100)     1390 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/language/Expr.py
--r--r--r--   0 pink      (1000) users      (100)    43471 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/language/DefaultTemplateLexer.py
--r--r--r--   0 pink      (1000) users      (100)      845 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/language/__init__.py
--r--r--r--   0 pink      (1000) users      (100)      730 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/language/StringTemplateToken.py
--r--r--r--   0 pink      (1000) users      (100)     1127 2008-02-17 22:30:43.000000 stringtemplate3-3.1/stringtemplate3/language/CatIterator.py
--r--r--r--   0 pink      (1000) users      (100)    13334 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/language/InterfaceLexer.py
--r--r--r--   0 pink      (1000) users      (100)     6925 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/language/InterfaceParser.py
--r--r--r--   0 pink      (1000) users      (100)    22710 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/language/GroupLexer.py
--r--r--r--   0 pink      (1000) users      (100)    49066 2008-02-17 22:30:43.000000 stringtemplate3-3.1/stringtemplate3/language/ActionParser.py
--r--r--r--   0 pink      (1000) users      (100)     4064 2008-02-17 22:30:43.000000 stringtemplate3-3.1/stringtemplate3/language/ConditionalExpr.py
--r--r--r--   0 pink      (1000) users      (100)     2353 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/language/FormalArgument.py
--r--r--r--   0 pink      (1000) users      (100)     9249 2008-02-17 22:30:46.000000 stringtemplate3-3.1/stringtemplate3/writers.py
--r--r--r--   0 pink      (1000) users      (100)    53642 2008-02-17 22:30:44.000000 stringtemplate3-3.1/stringtemplate3/templates.py
--r--r--r--   0 pink      (1000) users      (100)      355 2008-02-17 22:30:46.000000 stringtemplate3-3.1/stringtemplate3/utils.py
--r--r--r--   0 pink      (1000) users      (100)    31347 2008-02-17 22:30:43.000000 stringtemplate3-3.1/stringtemplate3/groups.py
--r--r--r--   0 pink      (1000) users      (100)      559 2008-02-17 22:30:42.000000 stringtemplate3-3.1/stringtemplate3/__init__.py
--r--r--r--   0 pink      (1000) users      (100)     6048 2008-02-17 22:30:42.000000 stringtemplate3-3.1/stringtemplate3/grouploaders.py
--r--r--r--   0 pink      (1000) users      (100)     2205 2008-02-17 22:30:42.000000 stringtemplate3-3.1/stringtemplate3/errors.py
--r--r--r--   0 pink      (1000) users      (100)      473 2008-02-17 22:30:42.000000 stringtemplate3-3.1/CHANGES.txt
--r--r--r--   0 pink      (1000) users      (100)     1436 2008-02-17 22:30:42.000000 stringtemplate3-3.1/setup.py
--r--r--r--   0 pink      (1000) users      (100)     1424 2008-02-17 22:30:42.000000 stringtemplate3-3.1/LICENSE.txt
+drwxr-xr-x   0 ben        (502) ben        (502)        0 2007-12-04 06:46:01.000000 stringtemplate3-3.1b1/
+-r--r--r--   0 ben        (502) ben        (502)      188 2007-12-04 06:44:12.000000 stringtemplate3-3.1b1/CHANGES.txt
+-r--r--r--   0 ben        (502) ben        (502)     1424 2007-12-04 06:44:12.000000 stringtemplate3-3.1b1/LICENSE.txt
+-rw-r--r--   0 ben        (502) ben        (502)     1149 2007-12-04 06:46:01.000000 stringtemplate3-3.1b1/PKG-INFO
+-r--r--r--   0 ben        (502) ben        (502)     1686 2007-12-04 06:44:12.000000 stringtemplate3-3.1b1/README.txt
+-r--r--r--   0 ben        (502) ben        (502)     1425 2007-12-04 06:44:12.000000 stringtemplate3-3.1b1/setup.py
+drwxr-xr-x   0 ben        (502) ben        (502)        0 2007-12-04 06:46:01.000000 stringtemplate3-3.1b1/stringtemplate3/
+-r--r--r--   0 ben        (502) ben        (502)      561 2007-12-04 06:44:12.000000 stringtemplate3-3.1b1/stringtemplate3/__init__.py
+-r--r--r--   0 ben        (502) ben        (502)     2205 2007-12-04 06:44:12.000000 stringtemplate3-3.1b1/stringtemplate3/errors.py
+-r--r--r--   0 ben        (502) ben        (502)     5734 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/grouploaders.py
+-r--r--r--   0 ben        (502) ben        (502)    30405 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/groups.py
+-r--r--r--   0 ben        (502) ben        (502)     6299 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/interfaces.py
+drwxr-xr-x   0 ben        (502) ben        (502)        0 2007-12-04 06:46:01.000000 stringtemplate3-3.1b1/stringtemplate3/language/
+-r--r--r--   0 ben        (502) ben        (502)      845 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/__init__.py
+-r--r--r--   0 ben        (502) ben        (502)    29889 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/ActionEvaluator.py
+-r--r--r--   0 ben        (502) ben        (502)    26704 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/ActionLexer.py
+-r--r--r--   0 ben        (502) ben        (502)    47891 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/ActionParser.py
+-r--r--r--   0 ben        (502) ben        (502)    39730 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/AngleBracketTemplateLexer.py
+-r--r--r--   0 ben        (502) ben        (502)    32650 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/ASTExpr.py
+-r--r--r--   0 ben        (502) ben        (502)     1127 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/CatIterator.py
+-r--r--r--   0 ben        (502) ben        (502)      848 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/ChunkToken.py
+-r--r--r--   0 ben        (502) ben        (502)     4064 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/ConditionalExpr.py
+-r--r--r--   0 ben        (502) ben        (502)    40747 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/DefaultTemplateLexer.py
+-r--r--r--   0 ben        (502) ben        (502)     1390 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/Expr.py
+-r--r--r--   0 ben        (502) ben        (502)     2353 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/FormalArgument.py
+-r--r--r--   0 ben        (502) ben        (502)    22710 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/GroupLexer.py
+-r--r--r--   0 ben        (502) ben        (502)    18411 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/GroupParser.py
+-r--r--r--   0 ben        (502) ben        (502)    13334 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/InterfaceLexer.py
+-r--r--r--   0 ben        (502) ben        (502)     6925 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/InterfaceParser.py
+-r--r--r--   0 ben        (502) ben        (502)      366 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/NewlineRef.py
+-r--r--r--   0 ben        (502) ben        (502)      823 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/StringRef.py
+-r--r--r--   0 ben        (502) ben        (502)      456 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/StringTemplateAST.py
+-r--r--r--   0 ben        (502) ben        (502)      634 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/StringTemplateToken.py
+-r--r--r--   0 ben        (502) ben        (502)     9796 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/language/TemplateParser.py
+-r--r--r--   0 ben        (502) ben        (502)    53630 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/templates.py
+-r--r--r--   0 ben        (502) ben        (502)      355 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/utils.py
+-r--r--r--   0 ben        (502) ben        (502)     9249 2007-12-04 06:44:13.000000 stringtemplate3-3.1b1/stringtemplate3/writers.py
```

### Comparing `stringtemplate3-3.1/PKG-INFO` & `stringtemplate3-3.1b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: stringtemplate3
-Version: 3.1
+Version: 3.1b1
 Summary: A powerful template engine with strict model-view separation
 Home-page: http://www.stringtemplate.org/
 Author: Benjamin Niemann
 Author-email: pink@odahoda.de
 License: BSD
 Description: 
         ST (StringTemplate) is a template engine for generating source code, web
@@ -12,14 +12,14 @@
         good at multi-targeted code generators, multiple site skins, and
         internationalization/localization. It evolved over years of effort
         developing jGuru.com. ST also generates this website and powers the
         ANTLR v3 code generator. Its distinguishing characteristic is that it
         strictly enforces model-view separation unlike other engines.
         
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
```

### Comparing `stringtemplate3-3.1/README.txt` & `stringtemplate3-3.1b1/README.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-StringTemplate 3.1 (Python)
-February 17, 2008
+StringTemplate 3.1b1 (Python)
+December 3, 2007
 
 
 AUTHORS
 =======
 
 Design & Java implementation:
```

### Comparing `stringtemplate3-3.1/stringtemplate3/interfaces.py` & `stringtemplate3-3.1b1/stringtemplate3/interfaces.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/language/ASTExpr.py` & `stringtemplate3-3.1b1/stringtemplate3/language/ASTExpr.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import antlr
 
 from stringtemplate3.utils import deprecated
 from stringtemplate3.language.Expr import Expr
 from stringtemplate3.language import ActionEvaluator
 from stringtemplate3.language.StringTemplateAST import StringTemplateAST
 from stringtemplate3.language.CatIterator import CatList
-from stringtemplate3.language.FormalArgument import UNKNOWN_ARGS
+from stringtemplate3.language.FormalArgument import (
+    FormalArgument, UNKNOWN_ARGS
+    )
 import stringtemplate3
 
 class IllegalStateException(Exception):
 
     def __init__(self, *args):
         Exception.__init__(self, *args)
 
@@ -298,16 +300,16 @@
                 isAnonymous = embedded.name == stringtemplate3.ANONYMOUS_ST_NAME
                 self.setSoleFormalArgumentToIthValue(embedded, argumentContext, ithValue)
                 if isinstance(attributeValue, dict):
                     argumentContext[self.DEFAULT_ATTRIBUTE_KEY] = ithValue
                     # formalArgs might be UNKNOWN, which is non-empty but treated
                     # like 'no formal args'. FIXME: Is this correct
                     if not (isAnonymous and formalArgs is not None and len(formalArgs) > 0 and formalArgs != UNKNOWN_ARGS):
-                        argumentContext[self.DEFAULT_ATTRIBUTE_NAME] = { ithValue: attributeValue[ithValue] }
-                        argumentContext[self.DEFAULT_ATTRIBUTE_NAME_DEPRECATED] = { ithValue: attributeValue[ithValue] }
+                        argumentContext[self.DEFAULT_ATTRIBUTE_NAME] = attributeValue[ithValue]
+                        argumentContext[self.DEFAULT_ATTRIBUTE_NAME_DEPRECATED] = attributeValue[ithValue]
                 else:
                     argumentContext[self.DEFAULT_ATTRIBUTE_KEY] = None
                     # formalArgs might be UNKNOWN, which is non-empty but treated
                     # like 'no formal args'. FIXME: Is this correct
                     if not (isAnonymous and formalArgs is not None and len(formalArgs) > 0 and formalArgs != UNKNOWN_ARGS):
                         argumentContext[self.DEFAULT_ATTRIBUTE_NAME] = ithValue
                         argumentContext[self.DEFAULT_ATTRIBUTE_NAME_DEPRECATED] = ithValue
```

### Comparing `stringtemplate3-3.1/stringtemplate3/language/ActionEvaluator.py` & `stringtemplate3-3.1b1/stringtemplate3/language/ActionEvaluator.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/language/ChunkToken.py` & `stringtemplate3-3.1b1/stringtemplate3/language/ChunkToken.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/language/GroupParser.py` & `stringtemplate3-3.1b1/stringtemplate3/language/GroupParser.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/language/ActionLexer.py` & `stringtemplate3-3.1b1/stringtemplate3/language/ActionLexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,24 +238,24 @@
     def mINT(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
         _ttype = INT
         _saveIndex = 0
         pass
-        _cnt63= 0
+        _cnt60= 0
         while True:
             if ((self.LA(1) >= u'0' and self.LA(1) <= u'9')):
                 pass
                 self.matchRange(u'0', u'9')
             else:
                 break
             
-            _cnt63 += 1
-        if _cnt63 < 1:
+            _cnt60 += 1
+        if _cnt60 < 1:
             self.raise_NoViableAlt(self.LA(1))
         self.set_return_token(_createToken, _token, _ttype, _begin)
     
     def mSTRING(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
@@ -339,27 +339,27 @@
         _saveIndex = 0
         args = None
         t = None
         pass
         _saveIndex = self.text.length()
         self.match('{')
         self.text.setLength(_saveIndex)
-        synPredMatched70 = False
+        synPredMatched67 = False
         if (_tokenSet_1.member(self.LA(1))) and (_tokenSet_2.member(self.LA(2))):
-            _m70 = self.mark()
-            synPredMatched70 = True
+            _m67 = self.mark()
+            synPredMatched67 = True
             self.inputState.guessing += 1
             try:
                 pass
                 self.mTEMPLATE_ARGS(False)
             except antlr.RecognitionException, pe:
-                synPredMatched70 = False
-            self.rewind(_m70)
+                synPredMatched67 = False
+            self.rewind(_m67)
             self.inputState.guessing -= 1
-        if synPredMatched70:
+        if synPredMatched67:
             pass
             args=self.mTEMPLATE_ARGS(False)
             if (_tokenSet_3.member(self.LA(1))) and ((self.LA(2) >= u'\u0003' and self.LA(2) <= u'\ufffe')):
                 pass
                 _saveIndex = self.text.length()
                 self.mWS_CHAR(False)
                 self.text.setLength(_saveIndex)
```

### Comparing `stringtemplate3-3.1/stringtemplate3/language/AngleBracketTemplateLexer.py` & `stringtemplate3-3.1b1/stringtemplate3/language/AngleBracketTemplateLexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,21 +38,19 @@
 ENDIF = 10
 REGION_REF = 11
 REGION_DEF = 12
 NL = 13
 EXPR = 14
 TEMPLATE = 15
 IF_EXPR = 16
-ESC_CHAR = 17
-ESC = 18
-HEX = 19
-SUBTEMPLATE = 20
-NESTED_PARENS = 21
-INDENT = 22
-COMMENT = 23
+ESC = 17
+SUBTEMPLATE = 18
+NESTED_PARENS = 19
+INDENT = 20
+COMMENT = 21
 
 
 ###/** Break up an input text stream into chunks of either plain text
 ### *  or template actions in "<...>".  Treat IF and ENDIF tokens
 ### *  specially.
 ### */
 class Lexer(antlr.CharScanner) :
@@ -254,45 +252,45 @@
     def mACTION(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
         _ttype = ACTION
         _saveIndex = 0
         startCol = self.getColumn()
-        if (self.LA(1)==u'<') and (self.LA(2)==u'\\') and (_tokenSet_2.member(self.LA(3))) and (_tokenSet_3.member(self.LA(4))) and (True) and (True) and (True):
+        if (self.LA(1)==u'<') and (self.LA(2)==u'\\') and (self.LA(3)==u'n') and (self.LA(4)==u'>') and (True) and (True) and (True):
             pass
-            buf = u""
-            uc = u"\000"
             _saveIndex = self.text.length()
-            self.match('<')
+            self.match("<\\n>")
             self.text.setLength(_saveIndex)
-            _cnt13= 0
-            while True:
-                if (self.LA(1)==u'\\'):
-                    pass
-                    uc=self.mESC_CHAR(False)
-                    buf += uc
-                else:
-                    break
-                
-                _cnt13 += 1
-            if _cnt13 < 1:
-                self.raise_NoViableAlt(self.LA(1))
+            self.text.setLength(_begin) ; self.text.append('\n'); _ttype = LITERAL
+        elif (self.LA(1)==u'<') and (self.LA(2)==u'\\') and (self.LA(3)==u'r') and (self.LA(4)==u'>') and (True) and (True) and (True):
+            pass
+            _saveIndex = self.text.length()
+            self.match("<\\r>")
+            self.text.setLength(_saveIndex)
+            self.text.setLength(_begin) ; self.text.append('\r'); _ttype = LITERAL
+        elif (self.LA(1)==u'<') and (self.LA(2)==u'\\') and (self.LA(3)==u't') and (self.LA(4)==u'>') and (True) and (True) and (True):
+            pass
+            _saveIndex = self.text.length()
+            self.match("<\\t>")
+            self.text.setLength(_saveIndex)
+            self.text.setLength(_begin) ; self.text.append('\t'); _ttype = LITERAL
+        elif (self.LA(1)==u'<') and (self.LA(2)==u'\\') and (self.LA(3)==u' ') and (self.LA(4)==u'>') and (True) and (True) and (True):
+            pass
             _saveIndex = self.text.length()
-            self.match('>')
+            self.match("<\\ >")
             self.text.setLength(_saveIndex)
-            self.text.setLength(_begin) ; self.text.append(buf)
-            _ttype = LITERAL
+            self.text.setLength(_begin) ; self.text.append(' '); _ttype = LITERAL
         elif (self.LA(1)==u'<') and (self.LA(2)==u'!') and ((self.LA(3) >= u'\u0001' and self.LA(3) <= u'\ufffe')) and ((self.LA(4) >= u'\u0001' and self.LA(4) <= u'\ufffe')) and (True) and (True) and (True):
             pass
             self.mCOMMENT(False)
             _ttype = SKIP
-        elif (self.LA(1)==u'<') and (_tokenSet_4.member(self.LA(2))) and ((self.LA(3) >= u'\u0001' and self.LA(3) <= u'\ufffe')) and (True) and (True) and (True) and (True):
+        elif (self.LA(1)==u'<') and (_tokenSet_2.member(self.LA(2))) and ((self.LA(3) >= u'\u0001' and self.LA(3) <= u'\ufffe')) and (True) and (True) and (True) and (True):
             pass
-            if (self.LA(1)==u'<') and (self.LA(2)==u'i') and (self.LA(3)==u'f') and (self.LA(4)==u' ' or self.LA(4)==u'(') and (_tokenSet_5.member(self.LA(5))) and ((self.LA(6) >= u'\u0001' and self.LA(6) <= u'\ufffe')) and ((self.LA(7) >= u'\u0001' and self.LA(7) <= u'\ufffe')):
+            if (self.LA(1)==u'<') and (self.LA(2)==u'i') and (self.LA(3)==u'f') and (self.LA(4)==u' ' or self.LA(4)==u'(') and (_tokenSet_3.member(self.LA(5))) and ((self.LA(6) >= u'\u0001' and self.LA(6) <= u'\ufffe')) and ((self.LA(7) >= u'\u0001' and self.LA(7) <= u'\ufffe')):
                 pass
                 _saveIndex = self.text.length()
                 self.match('<')
                 self.text.setLength(_saveIndex)
                 self.match("if")
                 while True:
                     if (self.LA(1)==u' '):
@@ -353,32 +351,32 @@
                     _saveIndex = self.text.length()
                     self.mNL(False)
                     self.text.setLength(_saveIndex)
                     self.newline()
                 else: ## <m4>
                         pass
                     
-            elif (self.LA(1)==u'<') and (self.LA(2)==u'@') and (_tokenSet_6.member(self.LA(3))) and ((self.LA(4) >= u'\u0001' and self.LA(4) <= u'\ufffe')) and ((self.LA(5) >= u'\u0001' and self.LA(5) <= u'\ufffe')) and ((self.LA(6) >= u'\u0001' and self.LA(6) <= u'\ufffe')) and (True):
+            elif (self.LA(1)==u'<') and (self.LA(2)==u'@') and (_tokenSet_4.member(self.LA(3))) and ((self.LA(4) >= u'\u0001' and self.LA(4) <= u'\ufffe')) and ((self.LA(5) >= u'\u0001' and self.LA(5) <= u'\ufffe')) and ((self.LA(6) >= u'\u0001' and self.LA(6) <= u'\ufffe')) and (True):
                 pass
                 _saveIndex = self.text.length()
                 self.match('<')
                 self.text.setLength(_saveIndex)
                 _saveIndex = self.text.length()
                 self.match('@')
                 self.text.setLength(_saveIndex)
-                _cnt22= 0
+                _cnt20= 0
                 while True:
-                    if (_tokenSet_6.member(self.LA(1))):
+                    if (_tokenSet_4.member(self.LA(1))):
                         pass
-                        self.match(_tokenSet_6)
+                        self.match(_tokenSet_4)
                     else:
                         break
                     
-                    _cnt22 += 1
-                if _cnt22 < 1:
+                    _cnt20 += 1
+                if _cnt20 < 1:
                     self.raise_NoViableAlt(self.LA(1))
                 la1 = self.LA(1)
                 if False:
                     pass
                 elif la1 and la1 in u'(':
                     pass
                     _saveIndex = self.text.length()
@@ -417,15 +415,15 @@
                         self.newline()
                     elif ((self.LA(1) >= u'\u0001' and self.LA(1) <= u'\ufffe')) and ((self.LA(2) >= u'\u0001' and self.LA(2) <= u'\ufffe')) and (True) and (True) and (True) and (True) and (True):
                         pass
                     else:
                         self.raise_NoViableAlt(self.LA(1))
                     
                     atLeft = False
-                    _cnt29= 0
+                    _cnt27= 0
                     while True:
                         if (((self.LA(1) >= u'\u0001' and self.LA(1) <= u'\ufffe')) and ((self.LA(2) >= u'\u0001' and self.LA(2) <= u'\ufffe')) and (True) and (True) and (True) and (True) and (True) and (not (self.upcomingAtEND(1) or (self.upcomingNewline(1) and self.upcomingAtEND(2))))):
                             pass
                             if (self.LA(1)==u'\n' or self.LA(1)==u'\r') and ((self.LA(2) >= u'\u0001' and self.LA(2) <= u'\ufffe')) and (True) and (True) and (True) and (True) and (True):
                                 pass
                                 la1 = self.LA(1)
                                 if False:
@@ -447,16 +445,16 @@
                                 atLeft = False
                             else:
                                 self.raise_NoViableAlt(self.LA(1))
                             
                         else:
                             break
                         
-                        _cnt29 += 1
-                    if _cnt29 < 1:
+                        _cnt27 += 1
+                    if _cnt27 < 1:
                         self.raise_NoViableAlt(self.LA(1))
                     if (self.LA(1)==u'\n' or self.LA(1)==u'\r') and ((self.LA(2) >= u'\u0001' and self.LA(2) <= u'\ufffe')) and (True) and (True) and (True) and (True) and (True):
                         pass
                         la1 = self.LA(1)
                         if False:
                             pass
                         elif la1 and la1 in u'\r':
@@ -512,15 +510,15 @@
                         self.newline()
                     else: ## <m4>
                             pass
                         
                 else:
                         self.raise_NoViableAlt(self.LA(1))
                     
-            elif (self.LA(1)==u'<') and (_tokenSet_4.member(self.LA(2))) and ((self.LA(3) >= u'\u0001' and self.LA(3) <= u'\ufffe')) and (True) and (True) and (True) and (True):
+            elif (self.LA(1)==u'<') and (_tokenSet_2.member(self.LA(2))) and ((self.LA(3) >= u'\u0001' and self.LA(3) <= u'\ufffe')) and (True) and (True) and (True) and (True):
                 pass
                 _saveIndex = self.text.length()
                 self.match('<')
                 self.text.setLength(_saveIndex)
                 self.mEXPR(False)
                 _saveIndex = self.text.length()
                 self.match('>')
@@ -531,77 +529,14 @@
             t = ChunkToken(_ttype, self.text.getString(_begin), self.currentIndent)
             _token = t
         else:
             self.raise_NoViableAlt(self.LA(1))
         
         self.set_return_token(_createToken, _token, _ttype, _begin)
     
-    def mESC_CHAR(self, _createToken):    
-        uc='\u0000'
-        _ttype = 0
-        _token = None
-        _begin = self.text.length()
-        _ttype = ESC_CHAR
-        _saveIndex = 0
-        a = None
-        b = None
-        c = None
-        d = None
-        if (self.LA(1)==u'\\') and (self.LA(2)==u'n'):
-            pass
-            _saveIndex = self.text.length()
-            self.match("\\n")
-            self.text.setLength(_saveIndex)
-            uc = '\n'
-        elif (self.LA(1)==u'\\') and (self.LA(2)==u'r'):
-            pass
-            _saveIndex = self.text.length()
-            self.match("\\r")
-            self.text.setLength(_saveIndex)
-            uc = '\r'
-        elif (self.LA(1)==u'\\') and (self.LA(2)==u't'):
-            pass
-            _saveIndex = self.text.length()
-            self.match("\\t")
-            self.text.setLength(_saveIndex)
-            uc = '\t'
-        elif (self.LA(1)==u'\\') and (self.LA(2)==u' '):
-            pass
-            _saveIndex = self.text.length()
-            self.match("\\ ")
-            self.text.setLength(_saveIndex)
-            uc = ' '
-        elif (self.LA(1)==u'\\') and (self.LA(2)==u'u'):
-            pass
-            _saveIndex = self.text.length()
-            self.match("\\u")
-            self.text.setLength(_saveIndex)
-            _saveIndex = self.text.length()
-            self.mHEX(True)
-            self.text.setLength(_saveIndex)
-            a = self._returnToken
-            _saveIndex = self.text.length()
-            self.mHEX(True)
-            self.text.setLength(_saveIndex)
-            b = self._returnToken
-            _saveIndex = self.text.length()
-            self.mHEX(True)
-            self.text.setLength(_saveIndex)
-            c = self._returnToken
-            _saveIndex = self.text.length()
-            self.mHEX(True)
-            self.text.setLength(_saveIndex)
-            d = self._returnToken
-            uc = unichr(int(a.getText()+b.getText()+c.getText()+d.getText(), 16))
-        else:
-            self.raise_NoViableAlt(self.LA(1))
-        
-        self.set_return_token(_createToken, _token, _ttype, _begin)
-        return uc
-    
     def mCOMMENT(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
         _ttype = COMMENT
         _saveIndex = 0
         startCol = self.getColumn()
@@ -634,15 +569,15 @@
     def mIF_EXPR(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
         _ttype = IF_EXPR
         _saveIndex = 0
         pass
-        _cnt54= 0
+        _cnt52= 0
         while True:
             la1 = self.LA(1)
             if False:
                 pass
             elif la1 and la1 in u'\\':
                 pass
                 self.mESC(False)
@@ -664,22 +599,22 @@
             elif la1 and la1 in u'{':
                 pass
                 self.mSUBTEMPLATE(False)
             elif la1 and la1 in u'(':
                 pass
                 self.mNESTED_PARENS(False)
             else:
-                if (_tokenSet_7.member(self.LA(1))):
+                if (_tokenSet_5.member(self.LA(1))):
                     pass
                     self.matchNot(')')
                 else:
                     break
                 
-            _cnt54 += 1
-        if _cnt54 < 1:
+            _cnt52 += 1
+        if _cnt52 < 1:
             self.raise_NoViableAlt(self.LA(1))
         self.set_return_token(_createToken, _token, _ttype, _begin)
     
     def mNL(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
@@ -703,15 +638,15 @@
     def mEXPR(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
         _ttype = EXPR
         _saveIndex = 0
         pass
-        _cnt42= 0
+        _cnt40= 0
         while True:
             la1 = self.LA(1)
             if False:
                 pass
             elif la1 and la1 in u'\\':
                 pass
                 self.mESC(False)
@@ -749,37 +684,37 @@
                     elif la1 and la1 in u'+':
                         pass
                         self.match('+')
                     else:
                             self.raise_NoViableAlt(self.LA(1))
                         
                     self.mSUBTEMPLATE(False)
-                elif (self.LA(1)==u'+' or self.LA(1)==u'=') and (_tokenSet_8.member(self.LA(2))):
+                elif (self.LA(1)==u'+' or self.LA(1)==u'=') and (_tokenSet_6.member(self.LA(2))):
                     pass
                     la1 = self.LA(1)
                     if False:
                         pass
                     elif la1 and la1 in u'=':
                         pass
                         self.match('=')
                     elif la1 and la1 in u'+':
                         pass
                         self.match('+')
                     else:
                             self.raise_NoViableAlt(self.LA(1))
                         
-                    self.match(_tokenSet_8)
-                elif (_tokenSet_9.member(self.LA(1))):
+                    self.match(_tokenSet_6)
+                elif (_tokenSet_7.member(self.LA(1))):
                     pass
                     self.matchNot('>')
                 else:
                     break
                 
-            _cnt42 += 1
-        if _cnt42 < 1:
+            _cnt40 += 1
+        if _cnt40 < 1:
             self.raise_NoViableAlt(self.LA(1))
         self.set_return_token(_createToken, _token, _ttype, _begin)
     
     def mESC(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
@@ -805,15 +740,15 @@
             elif la1 and la1 in u'{':
                 pass
                 self.mSUBTEMPLATE(False)
             elif la1 and la1 in u'\\':
                 pass
                 self.mESC(False)
             else:
-                if (_tokenSet_10.member(self.LA(1))):
+                if (_tokenSet_8.member(self.LA(1))):
                     pass
                     self.matchNot('}')
                 else:
                     break
                 
         self.match('}')
         self.set_return_token(_createToken, _token, _ttype, _begin)
@@ -830,15 +765,15 @@
         elif la1 and la1 in u'"':
             pass
             self.match('"')
             while True:
                 if (self.LA(1)==u'\\'):
                     pass
                     self.mESC(False)
-                elif (_tokenSet_11.member(self.LA(1))):
+                elif (_tokenSet_9.member(self.LA(1))):
                     pass
                     self.matchNot('"')
                 else:
                     break
                 
             self.match('"')
         elif la1 and la1 in u'<':
@@ -918,61 +853,38 @@
         _ttype = 0
         _token = None
         _begin = self.text.length()
         _ttype = NESTED_PARENS
         _saveIndex = 0
         pass
         self.match('(')
-        _cnt63= 0
+        _cnt59= 0
         while True:
             la1 = self.LA(1)
             if False:
                 pass
             elif la1 and la1 in u'(':
                 pass
                 self.mNESTED_PARENS(False)
             elif la1 and la1 in u'\\':
                 pass
                 self.mESC(False)
             else:
-                if (_tokenSet_12.member(self.LA(1))):
+                if (_tokenSet_10.member(self.LA(1))):
                     pass
                     self.matchNot(')')
                 else:
                     break
                 
-            _cnt63 += 1
-        if _cnt63 < 1:
+            _cnt59 += 1
+        if _cnt59 < 1:
             self.raise_NoViableAlt(self.LA(1))
         self.match(')')
         self.set_return_token(_createToken, _token, _ttype, _begin)
     
-    def mHEX(self, _createToken):    
-        _ttype = 0
-        _token = None
-        _begin = self.text.length()
-        _ttype = HEX
-        _saveIndex = 0
-        la1 = self.LA(1)
-        if False:
-            pass
-        elif la1 and la1 in u'0123456789':
-            pass
-            self.matchRange(u'0', u'9')
-        elif la1 and la1 in u'ABCDEF':
-            pass
-            self.matchRange(u'A', u'F')
-        elif la1 and la1 in u'abcdef':
-            pass
-            self.matchRange(u'a', u'f')
-        else:
-                self.raise_NoViableAlt(self.LA(1))
-            
-        self.set_return_token(_createToken, _token, _ttype, _begin)
-    
     
 
 ### generate bit set
 def mk_tokenSet_0(): 
     data = [0L] * 2048 ### init list
     data[0] =-1152921504606856194L
     for x in xrange(1, 1023):
@@ -989,123 +901,107 @@
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
 _tokenSet_1 = antlr.BitSet(mk_tokenSet_1())
 
 ### generate bit set
 def mk_tokenSet_2(): 
-    data = [0L] * 1025 ### init list
-    data[0] =4294967296L
-    data[1] =14707067533131776L
-    return data
-_tokenSet_2 = antlr.BitSet(mk_tokenSet_2())
-
-### generate bit set
-def mk_tokenSet_3(): 
-    data = [0L] * 1025 ### init list
-    data[0] =4899634919602388992L
-    data[1] =541434314878L
-    return data
-_tokenSet_3 = antlr.BitSet(mk_tokenSet_3())
-
-### generate bit set
-def mk_tokenSet_4(): 
     data = [0L] * 2048 ### init list
     data[0] =-4611686018427387906L
     for x in xrange(1, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_4 = antlr.BitSet(mk_tokenSet_4())
+_tokenSet_2 = antlr.BitSet(mk_tokenSet_2())
 
 ### generate bit set
-def mk_tokenSet_5(): 
+def mk_tokenSet_3(): 
     data = [0L] * 2048 ### init list
     data[0] =-2199023255554L
     for x in xrange(1, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_5 = antlr.BitSet(mk_tokenSet_5())
+_tokenSet_3 = antlr.BitSet(mk_tokenSet_3())
 
 ### generate bit set
-def mk_tokenSet_6(): 
+def mk_tokenSet_4(): 
     data = [0L] * 2048 ### init list
     data[0] =-4611687117939015682L
     for x in xrange(1, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_6 = antlr.BitSet(mk_tokenSet_6())
+_tokenSet_4 = antlr.BitSet(mk_tokenSet_4())
 
 ### generate bit set
-def mk_tokenSet_7(): 
+def mk_tokenSet_5(): 
     data = [0L] * 2048 ### init list
     data[0] =-3298534892546L
     data[1] =-576460752571858945L
     for x in xrange(2, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_7 = antlr.BitSet(mk_tokenSet_7())
+_tokenSet_5 = antlr.BitSet(mk_tokenSet_5())
 
 ### generate bit set
-def mk_tokenSet_8(): 
+def mk_tokenSet_6(): 
     data = [0L] * 2048 ### init list
     data[0] =-1152921521786716162L
     data[1] =-576460752303423489L
     for x in xrange(2, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_8 = antlr.BitSet(mk_tokenSet_8())
+_tokenSet_6 = antlr.BitSet(mk_tokenSet_6())
 
 ### generate bit set
-def mk_tokenSet_9(): 
+def mk_tokenSet_7(): 
     data = [0L] * 2048 ### init list
     data[0] =-6917537823734113282L
     data[1] =-576460752571858945L
     for x in xrange(2, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_9 = antlr.BitSet(mk_tokenSet_9())
+_tokenSet_7 = antlr.BitSet(mk_tokenSet_7())
 
 ### generate bit set
-def mk_tokenSet_10(): 
+def mk_tokenSet_8(): 
     data = [0L] * 2048 ### init list
     data[0] =-2L
     data[1] =-2882303761785552897L
     for x in xrange(2, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_10 = antlr.BitSet(mk_tokenSet_10())
+_tokenSet_8 = antlr.BitSet(mk_tokenSet_8())
 
 ### generate bit set
-def mk_tokenSet_11(): 
+def mk_tokenSet_9(): 
     data = [0L] * 2048 ### init list
     data[0] =-17179869186L
     data[1] =-268435457L
     for x in xrange(2, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_11 = antlr.BitSet(mk_tokenSet_11())
+_tokenSet_9 = antlr.BitSet(mk_tokenSet_9())
 
 ### generate bit set
-def mk_tokenSet_12(): 
+def mk_tokenSet_10(): 
     data = [0L] * 2048 ### init list
     data[0] =-3298534883330L
     data[1] =-268435457L
     for x in xrange(2, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_12 = antlr.BitSet(mk_tokenSet_12())
+_tokenSet_10 = antlr.BitSet(mk_tokenSet_10())
     
 ### __main__ header action >>> 
 if __name__ == '__main__' :
     import sys
     import antlr
     import AngleBracketTemplateLexer
```

### Comparing `stringtemplate3-3.1/stringtemplate3/language/TemplateParser.py` & `stringtemplate3-3.1b1/stringtemplate3/language/TemplateParser.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,21 +36,19 @@
 ENDIF = 10
 REGION_REF = 11
 REGION_DEF = 12
 NL = 13
 EXPR = 14
 TEMPLATE = 15
 IF_EXPR = 16
-ESC_CHAR = 17
-ESC = 18
-HEX = 19
-SUBTEMPLATE = 20
-NESTED_PARENS = 21
-INDENT = 22
-COMMENT = 23
+ESC = 17
+SUBTEMPLATE = 18
+NESTED_PARENS = 19
+INDENT = 20
+COMMENT = 21
 
 
 ###/** A parser used to break up a single template into chunks, text literals
 ### *  and attribute expressions.
 ### */
 class Parser(antlr.LLkParser):
     ### user action >>>
@@ -261,17 +259,15 @@
     "ENDIF", 
     "REGION_REF", 
     "REGION_DEF", 
     "NL", 
     "EXPR", 
     "TEMPLATE", 
     "IF_EXPR", 
-    "ESC_CHAR", 
     "ESC", 
-    "HEX", 
     "SUBTEMPLATE", 
     "NESTED_PARENS", 
     "INDENT", 
     "COMMENT"
 ]
```

### Comparing `stringtemplate3-3.1/stringtemplate3/language/StringRef.py` & `stringtemplate3-3.1b1/stringtemplate3/language/StringRef.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/language/Expr.py` & `stringtemplate3-3.1b1/stringtemplate3/language/Expr.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/language/DefaultTemplateLexer.py` & `stringtemplate3-3.1b1/stringtemplate3/language/DefaultTemplateLexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,19 @@
 ENDIF = 10
 REGION_REF = 11
 REGION_DEF = 12
 NL = 13
 EXPR = 14
 TEMPLATE = 15
 IF_EXPR = 16
-ESC_CHAR = 17
-ESC = 18
-HEX = 19
-SUBTEMPLATE = 20
-NESTED_PARENS = 21
-INDENT = 22
-COMMENT = 23
+ESC = 17
+SUBTEMPLATE = 18
+NESTED_PARENS = 19
+INDENT = 20
+COMMENT = 21
 
 
 ###/** Break up an input text stream into chunks of either plain text
 ### *  or template actions in "$...$".  Treat IF and ENDIF tokens
 ### *  specially.
 ### */
 class Lexer(antlr.CharScanner) :
@@ -204,27 +202,27 @@
     def mINDENT(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
         _ttype = INDENT
         _saveIndex = 0
         pass
-        _cnt72= 0
+        _cnt68= 0
         while True:
             if (self.LA(1)==u' ') and (True) and (True) and (True) and (True) and (True) and (True):
                 pass
                 self.match(' ')
             elif (self.LA(1)==u'\t') and (True) and (True) and (True) and (True) and (True) and (True):
                 pass
                 self.match('\t')
             else:
                 break
             
-            _cnt72 += 1
-        if _cnt72 < 1:
+            _cnt68 += 1
+        if _cnt68 < 1:
             self.raise_NoViableAlt(self.LA(1))
         self.set_return_token(_createToken, _token, _ttype, _begin)
     
     def mNEWLINE(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
@@ -260,45 +258,45 @@
     def mACTION(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
         _ttype = ACTION
         _saveIndex = 0
         startCol = self.getColumn()
-        if (self.LA(1)==u'$') and (self.LA(2)==u'\\') and (_tokenSet_2.member(self.LA(3))) and (_tokenSet_3.member(self.LA(4))) and (True) and (True) and (True):
+        if (self.LA(1)==u'$') and (self.LA(2)==u'\\') and (self.LA(3)==u'n') and (self.LA(4)==u'$') and (True) and (True) and (True):
             pass
-            buf = u""
-            uc = u"\000"
             _saveIndex = self.text.length()
-            self.match('$')
+            self.match("$\\n$")
             self.text.setLength(_saveIndex)
-            _cnt15= 0
-            while True:
-                if (self.LA(1)==u'\\'):
-                    pass
-                    uc=self.mESC_CHAR(False)
-                    buf += uc
-                else:
-                    break
-                
-                _cnt15 += 1
-            if _cnt15 < 1:
-                self.raise_NoViableAlt(self.LA(1))
+            self.text.setLength(_begin) ; self.text.append('\n'); _ttype = LITERAL
+        elif (self.LA(1)==u'$') and (self.LA(2)==u'\\') and (self.LA(3)==u'r') and (self.LA(4)==u'$') and (True) and (True) and (True):
+            pass
+            _saveIndex = self.text.length()
+            self.match("$\\r$")
+            self.text.setLength(_saveIndex)
+            self.text.setLength(_begin) ; self.text.append('\r'); _ttype = LITERAL
+        elif (self.LA(1)==u'$') and (self.LA(2)==u'\\') and (self.LA(3)==u't') and (self.LA(4)==u'$') and (True) and (True) and (True):
+            pass
+            _saveIndex = self.text.length()
+            self.match("$\\t$")
+            self.text.setLength(_saveIndex)
+            self.text.setLength(_begin) ; self.text.append('\t'); _ttype = LITERAL
+        elif (self.LA(1)==u'$') and (self.LA(2)==u'\\') and (self.LA(3)==u' ') and (self.LA(4)==u'$') and (True) and (True) and (True):
+            pass
             _saveIndex = self.text.length()
-            self.match('$')
+            self.match("$\\ $")
             self.text.setLength(_saveIndex)
-            self.text.setLength(_begin) ; self.text.append(buf)
-            _ttype = LITERAL
+            self.text.setLength(_begin) ; self.text.append(' '); _ttype = LITERAL
         elif (self.LA(1)==u'$') and (self.LA(2)==u'!') and ((self.LA(3) >= u'\u0001' and self.LA(3) <= u'\ufffe')) and ((self.LA(4) >= u'\u0001' and self.LA(4) <= u'\ufffe')) and (True) and (True) and (True):
             pass
             self.mCOMMENT(False)
             _ttype = SKIP
         elif (self.LA(1)==u'$') and (_tokenSet_1.member(self.LA(2))) and ((self.LA(3) >= u'\u0001' and self.LA(3) <= u'\ufffe')) and (True) and (True) and (True) and (True):
             pass
-            if (self.LA(1)==u'$') and (self.LA(2)==u'i') and (self.LA(3)==u'f') and (self.LA(4)==u' ' or self.LA(4)==u'(') and (_tokenSet_4.member(self.LA(5))) and ((self.LA(6) >= u'\u0001' and self.LA(6) <= u'\ufffe')) and ((self.LA(7) >= u'\u0001' and self.LA(7) <= u'\ufffe')):
+            if (self.LA(1)==u'$') and (self.LA(2)==u'i') and (self.LA(3)==u'f') and (self.LA(4)==u' ' or self.LA(4)==u'(') and (_tokenSet_2.member(self.LA(5))) and ((self.LA(6) >= u'\u0001' and self.LA(6) <= u'\ufffe')) and ((self.LA(7) >= u'\u0001' and self.LA(7) <= u'\ufffe')):
                 pass
                 _saveIndex = self.text.length()
                 self.match('$')
                 self.text.setLength(_saveIndex)
                 self.match("if")
                 while True:
                     if (self.LA(1)==u' '):
@@ -403,32 +401,32 @@
                     _saveIndex = self.text.length()
                     self.mNL(False)
                     self.text.setLength(_saveIndex)
                     self.newline()
                 else: ## <m4>
                         pass
                     
-            elif (self.LA(1)==u'$') and (self.LA(2)==u'@') and (_tokenSet_5.member(self.LA(3))) and ((self.LA(4) >= u'\u0001' and self.LA(4) <= u'\ufffe')) and ((self.LA(5) >= u'\u0001' and self.LA(5) <= u'\ufffe')) and ((self.LA(6) >= u'\u0001' and self.LA(6) <= u'\ufffe')) and (True):
+            elif (self.LA(1)==u'$') and (self.LA(2)==u'@') and (_tokenSet_3.member(self.LA(3))) and ((self.LA(4) >= u'\u0001' and self.LA(4) <= u'\ufffe')) and ((self.LA(5) >= u'\u0001' and self.LA(5) <= u'\ufffe')) and ((self.LA(6) >= u'\u0001' and self.LA(6) <= u'\ufffe')) and (True):
                 pass
                 _saveIndex = self.text.length()
                 self.match('$')
                 self.text.setLength(_saveIndex)
                 _saveIndex = self.text.length()
                 self.match('@')
                 self.text.setLength(_saveIndex)
-                _cnt28= 0
+                _cnt26= 0
                 while True:
-                    if (_tokenSet_5.member(self.LA(1))):
+                    if (_tokenSet_3.member(self.LA(1))):
                         pass
-                        self.match(_tokenSet_5)
+                        self.match(_tokenSet_3)
                     else:
                         break
                     
-                    _cnt28 += 1
-                if _cnt28 < 1:
+                    _cnt26 += 1
+                if _cnt26 < 1:
                     self.raise_NoViableAlt(self.LA(1))
                 la1 = self.LA(1)
                 if False:
                     pass
                 elif la1 and la1 in u'(':
                     pass
                     _saveIndex = self.text.length()
@@ -467,15 +465,15 @@
                         newline();
                     elif ((self.LA(1) >= u'\u0001' and self.LA(1) <= u'\ufffe')) and ((self.LA(2) >= u'\u0001' and self.LA(2) <= u'\ufffe')) and (True) and (True) and (True) and (True) and (True):
                         pass
                     else:
                         self.raise_NoViableAlt(self.LA(1))
                     
                     atLeft = False
-                    _cnt35= 0
+                    _cnt33= 0
                     while True:
                         if (((self.LA(1) >= u'\u0001' and self.LA(1) <= u'\ufffe')) and ((self.LA(2) >= u'\u0001' and self.LA(2) <= u'\ufffe')) and (True) and (True) and (True) and (True) and (True) and (not (self.upcomingAtEND(1) or (self.upcomingNewline(1) and self.upcomingAtEND(2))))):
                             pass
                             if (self.LA(1)==u'\n' or self.LA(1)==u'\r') and ((self.LA(2) >= u'\u0001' and self.LA(2) <= u'\ufffe')) and (True) and (True) and (True) and (True) and (True):
                                 pass
                                 la1 = self.LA(1)
                                 if False:
@@ -497,16 +495,16 @@
                                 atLeft = False
                             else:
                                 self.raise_NoViableAlt(self.LA(1))
                             
                         else:
                             break
                         
-                        _cnt35 += 1
-                    if _cnt35 < 1:
+                        _cnt33 += 1
+                    if _cnt33 < 1:
                         self.raise_NoViableAlt(self.LA(1))
                     if (self.LA(1)==u'\n' or self.LA(1)==u'\r') and ((self.LA(2) >= u'\u0001' and self.LA(2) <= u'\ufffe')) and (True) and (True) and (True) and (True) and (True):
                         pass
                         la1 = self.LA(1)
                         if False:
                             pass
                         elif la1 and la1 in u'\r':
@@ -581,77 +579,14 @@
             t = ChunkToken(_ttype, self.text.getString(_begin), self.currentIndent)
             _token = t;
         else:
             self.raise_NoViableAlt(self.LA(1))
         
         self.set_return_token(_createToken, _token, _ttype, _begin)
     
-    def mESC_CHAR(self, _createToken):    
-        uc='\u0000'
-        _ttype = 0
-        _token = None
-        _begin = self.text.length()
-        _ttype = ESC_CHAR
-        _saveIndex = 0
-        a = None
-        b = None
-        c = None
-        d = None
-        if (self.LA(1)==u'\\') and (self.LA(2)==u'n'):
-            pass
-            _saveIndex = self.text.length()
-            self.match("\\n")
-            self.text.setLength(_saveIndex)
-            uc = '\n'
-        elif (self.LA(1)==u'\\') and (self.LA(2)==u'r'):
-            pass
-            _saveIndex = self.text.length()
-            self.match("\\r")
-            self.text.setLength(_saveIndex)
-            uc = '\r'
-        elif (self.LA(1)==u'\\') and (self.LA(2)==u't'):
-            pass
-            _saveIndex = self.text.length()
-            self.match("\\t")
-            self.text.setLength(_saveIndex)
-            uc = '\t'
-        elif (self.LA(1)==u'\\') and (self.LA(2)==u' '):
-            pass
-            _saveIndex = self.text.length()
-            self.match("\\ ")
-            self.text.setLength(_saveIndex)
-            uc = ' '
-        elif (self.LA(1)==u'\\') and (self.LA(2)==u'u'):
-            pass
-            _saveIndex = self.text.length()
-            self.match("\\u")
-            self.text.setLength(_saveIndex)
-            _saveIndex = self.text.length()
-            self.mHEX(True)
-            self.text.setLength(_saveIndex)
-            a = self._returnToken
-            _saveIndex = self.text.length()
-            self.mHEX(True)
-            self.text.setLength(_saveIndex)
-            b = self._returnToken
-            _saveIndex = self.text.length()
-            self.mHEX(True)
-            self.text.setLength(_saveIndex)
-            c = self._returnToken
-            _saveIndex = self.text.length()
-            self.mHEX(True)
-            self.text.setLength(_saveIndex)
-            d = self._returnToken
-            uc = unichr(int(a.getText()+b.getText()+c.getText()+d.getText(), 16))
-        else:
-            self.raise_NoViableAlt(self.LA(1))
-        
-        self.set_return_token(_createToken, _token, _ttype, _begin)
-        return uc
-    
     def mCOMMENT(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
         _ttype = COMMENT
         _saveIndex = 0
         startCol = self.getColumn()
@@ -684,15 +619,15 @@
     def mIF_EXPR(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
         _ttype = IF_EXPR
         _saveIndex = 0
         pass
-        _cnt60= 0
+        _cnt58= 0
         while True:
             la1 = self.LA(1)
             if False:
                 pass
             elif la1 and la1 in u'\\':
                 pass
                 self.mESC(False)
@@ -714,33 +649,33 @@
             elif la1 and la1 in u'{':
                 pass
                 self.mSUBTEMPLATE(False)
             elif la1 and la1 in u'(':
                 pass
                 self.mNESTED_PARENS(False)
             else:
-                if (_tokenSet_6.member(self.LA(1))):
+                if (_tokenSet_4.member(self.LA(1))):
                     pass
                     self.matchNot(')')
                 else:
                     break
                 
-            _cnt60 += 1
-        if _cnt60 < 1:
+            _cnt58 += 1
+        if _cnt58 < 1:
             self.raise_NoViableAlt(self.LA(1))
         self.set_return_token(_createToken, _token, _ttype, _begin)
     
     def mEXPR(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
         _ttype = EXPR
         _saveIndex = 0
         pass
-        _cnt48= 0
+        _cnt46= 0
         while True:
             la1 = self.LA(1)
             if False:
                 pass
             elif la1 and la1 in u'\\':
                 pass
                 self.mESC(False)
@@ -778,37 +713,37 @@
                     elif la1 and la1 in u'+':
                         pass
                         self.match('+')
                     else:
                             self.raise_NoViableAlt(self.LA(1))
                         
                     self.mSUBTEMPLATE(False)
-                elif (self.LA(1)==u'+' or self.LA(1)==u'=') and (_tokenSet_7.member(self.LA(2))):
+                elif (self.LA(1)==u'+' or self.LA(1)==u'=') and (_tokenSet_5.member(self.LA(2))):
                     pass
                     la1 = self.LA(1)
                     if False:
                         pass
                     elif la1 and la1 in u'=':
                         pass
                         self.match('=')
                     elif la1 and la1 in u'+':
                         pass
                         self.match('+')
                     else:
                             self.raise_NoViableAlt(self.LA(1))
                         
-                    self.match(_tokenSet_7)
-                elif (_tokenSet_8.member(self.LA(1))):
+                    self.match(_tokenSet_5)
+                elif (_tokenSet_6.member(self.LA(1))):
                     pass
                     self.matchNot('$')
                 else:
                     break
                 
-            _cnt48 += 1
-        if _cnt48 < 1:
+            _cnt46 += 1
+        if _cnt46 < 1:
             self.raise_NoViableAlt(self.LA(1))
         self.set_return_token(_createToken, _token, _ttype, _begin)
     
     def mESC(self, _createToken):    
         _ttype = 0
         _token = None
         _begin = self.text.length()
@@ -834,15 +769,15 @@
             elif la1 and la1 in u'{':
                 pass
                 self.mSUBTEMPLATE(False)
             elif la1 and la1 in u'\\':
                 pass
                 self.mESC(False)
             else:
-                if (_tokenSet_9.member(self.LA(1))):
+                if (_tokenSet_7.member(self.LA(1))):
                     pass
                     self.matchNot('}')
                 else:
                     break
                 
         self.match('}')
         self.set_return_token(_createToken, _token, _ttype, _begin)
@@ -859,15 +794,15 @@
         elif la1 and la1 in u'"':
             pass
             self.match('"')
             while True:
                 if (self.LA(1)==u'\\'):
                     pass
                     self.mESC(False)
-                elif (_tokenSet_10.member(self.LA(1))):
+                elif (_tokenSet_8.member(self.LA(1))):
                     pass
                     self.matchNot('"')
                 else:
                     break
                 
             self.match('"')
         elif la1 and la1 in u'<':
@@ -947,61 +882,38 @@
         _ttype = 0
         _token = None
         _begin = self.text.length()
         _ttype = NESTED_PARENS
         _saveIndex = 0
         pass
         self.match('(')
-        _cnt69= 0
+        _cnt65= 0
         while True:
             la1 = self.LA(1)
             if False:
                 pass
             elif la1 and la1 in u'(':
                 pass
                 self.mNESTED_PARENS(False)
             elif la1 and la1 in u'\\':
                 pass
                 self.mESC(False)
             else:
-                if (_tokenSet_11.member(self.LA(1))):
+                if (_tokenSet_9.member(self.LA(1))):
                     pass
                     self.matchNot(')')
                 else:
                     break
                 
-            _cnt69 += 1
-        if _cnt69 < 1:
+            _cnt65 += 1
+        if _cnt65 < 1:
             self.raise_NoViableAlt(self.LA(1))
         self.match(')')
         self.set_return_token(_createToken, _token, _ttype, _begin)
     
-    def mHEX(self, _createToken):    
-        _ttype = 0
-        _token = None
-        _begin = self.text.length()
-        _ttype = HEX
-        _saveIndex = 0
-        la1 = self.LA(1)
-        if False:
-            pass
-        elif la1 and la1 in u'0123456789':
-            pass
-            self.matchRange(u'0', u'9')
-        elif la1 and la1 in u'ABCDEF':
-            pass
-            self.matchRange(u'A', u'F')
-        elif la1 and la1 in u'abcdef':
-            pass
-            self.matchRange(u'a', u'f')
-        else:
-                self.raise_NoViableAlt(self.LA(1))
-            
-        self.set_return_token(_createToken, _token, _ttype, _begin)
-    
     
 
 ### generate bit set
 def mk_tokenSet_0(): 
     data = [0L] * 2048 ### init list
     data[0] =-68719485954L
     for x in xrange(1, 1023):
@@ -1018,113 +930,97 @@
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
 _tokenSet_1 = antlr.BitSet(mk_tokenSet_1())
 
 ### generate bit set
 def mk_tokenSet_2(): 
-    data = [0L] * 1025 ### init list
-    data[0] =4294967296L
-    data[1] =14707067533131776L
-    return data
-_tokenSet_2 = antlr.BitSet(mk_tokenSet_2())
-
-### generate bit set
-def mk_tokenSet_3(): 
-    data = [0L] * 1025 ### init list
-    data[0] =287948969894477824L
-    data[1] =541434314878L
-    return data
-_tokenSet_3 = antlr.BitSet(mk_tokenSet_3())
-
-### generate bit set
-def mk_tokenSet_4(): 
     data = [0L] * 2048 ### init list
     data[0] =-2199023255554L
     for x in xrange(1, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_4 = antlr.BitSet(mk_tokenSet_4())
+_tokenSet_2 = antlr.BitSet(mk_tokenSet_2())
 
 ### generate bit set
-def mk_tokenSet_5(): 
+def mk_tokenSet_3(): 
     data = [0L] * 2048 ### init list
     data[0] =-1168231104514L
     for x in xrange(1, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_5 = antlr.BitSet(mk_tokenSet_5())
+_tokenSet_3 = antlr.BitSet(mk_tokenSet_3())
 
 ### generate bit set
-def mk_tokenSet_6(): 
+def mk_tokenSet_4(): 
     data = [0L] * 2048 ### init list
     data[0] =-3298534892546L
     data[1] =-576460752571858945L
     for x in xrange(2, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_6 = antlr.BitSet(mk_tokenSet_6())
+_tokenSet_4 = antlr.BitSet(mk_tokenSet_4())
 
 ### generate bit set
-def mk_tokenSet_7(): 
+def mk_tokenSet_5(): 
     data = [0L] * 2048 ### init list
     data[0] =-1152921521786716162L
     data[1] =-576460752303423489L
     for x in xrange(2, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_7 = antlr.BitSet(mk_tokenSet_7())
+_tokenSet_5 = antlr.BitSet(mk_tokenSet_5())
 
 ### generate bit set
-def mk_tokenSet_8(): 
+def mk_tokenSet_6(): 
     data = [0L] * 2048 ### init list
     data[0] =-2305851874026202114L
     data[1] =-576460752571858945L
     for x in xrange(2, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_8 = antlr.BitSet(mk_tokenSet_8())
+_tokenSet_6 = antlr.BitSet(mk_tokenSet_6())
 
 ### generate bit set
-def mk_tokenSet_9(): 
+def mk_tokenSet_7(): 
     data = [0L] * 2048 ### init list
     data[0] =-2L
     data[1] =-2882303761785552897L
     for x in xrange(2, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_9 = antlr.BitSet(mk_tokenSet_9())
+_tokenSet_7 = antlr.BitSet(mk_tokenSet_7())
 
 ### generate bit set
-def mk_tokenSet_10(): 
+def mk_tokenSet_8(): 
     data = [0L] * 2048 ### init list
     data[0] =-17179869186L
     data[1] =-268435457L
     for x in xrange(2, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_10 = antlr.BitSet(mk_tokenSet_10())
+_tokenSet_8 = antlr.BitSet(mk_tokenSet_8())
 
 ### generate bit set
-def mk_tokenSet_11(): 
+def mk_tokenSet_9(): 
     data = [0L] * 2048 ### init list
     data[0] =-3298534883330L
     data[1] =-268435457L
     for x in xrange(2, 1023):
         data[x] = -1L
     data[1023] =9223372036854775807L
     return data
-_tokenSet_11 = antlr.BitSet(mk_tokenSet_11())
+_tokenSet_9 = antlr.BitSet(mk_tokenSet_9())
     
 ### __main__ header action >>> 
 if __name__ == '__main__' :
     import sys
     import antlr
     import DefaultTemplateLexer
```

### Comparing `stringtemplate3-3.1/stringtemplate3/language/__init__.py` & `stringtemplate3-3.1b1/stringtemplate3/language/__init__.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/language/StringTemplateToken.py` & `stringtemplate3-3.1b1/stringtemplate3/language/StringTemplateToken.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 
 import antlr
 
 class StringTemplateToken(antlr.CommonToken):
 
-    def __init__(self, type = 0, text = '', args = None):
+    def __init__(self, type = 0, text = '', args = []):
         super(StringTemplateToken, self).__init__(type=type, text=text)
-        ## Track any args for anonymous templates like
-        #  <tokens,rules:{t,r | <t> then <r>}>
-        #  The lexer in action.g returns a single token ANONYMOUS_TEMPLATE
-        #  and so I need to have it parse args in the lexer and make them
-        #  available for when I build the anonymous template.
-
-        if args is None:
-            args = []
-        self.args = args
+	## Track any args for anonymous templates like
+	#  <tokens,rules:{t,r | <t> then <r>}>
+	#  The lexer in action.g returns a single token ANONYMOUS_TEMPLATE
+	#  and so I need to have it parse args in the lexer and make them
+	#  available for when I build the anonymous template.
+	#
+	self.args = args
 
     def __str__(self):
         return super(StringTemplateToken, self).__str__() + \
-               '; args=' + str(self.args)
+	       '; args=' + str(self.args)
 
     __repr__ = __str__
```

### Comparing `stringtemplate3-3.1/stringtemplate3/language/CatIterator.py` & `stringtemplate3-3.1b1/stringtemplate3/language/CatIterator.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/language/InterfaceLexer.py` & `stringtemplate3-3.1b1/stringtemplate3/language/InterfaceLexer.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/language/InterfaceParser.py` & `stringtemplate3-3.1b1/stringtemplate3/language/InterfaceParser.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/language/GroupLexer.py` & `stringtemplate3-3.1b1/stringtemplate3/language/GroupLexer.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/language/ActionParser.py` & `stringtemplate3-3.1b1/stringtemplate3/language/ActionParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -532,40 +532,14 @@
             elif la1 and la1 in [EOF,SEMI,RPAREN,COMMA,COLON,PLUS,RBRACK]:
                 pass
                 primaryExpr_AST = currentAST.root
             elif la1 and la1 in [LITERAL_first,LITERAL_rest,LITERAL_last,LITERAL_length,LITERAL_strip,LITERAL_trunc]:
                 pass
                 self.function()
                 self.addASTChild(currentAST, self.returnAST)
-                while True:
-                    if (self.LA(1)==DOT):
-                        pass
-                        tmp14_AST = None
-                        tmp14_AST = self.astFactory.create(self.LT(1))
-                        self.makeASTRoot(currentAST, tmp14_AST)
-                        self.match(DOT)
-                        la1 = self.LA(1)
-                        if False:
-                            pass
-                        elif la1 and la1 in [ID]:
-                            pass
-                            tmp15_AST = None
-                            tmp15_AST = self.astFactory.create(self.LT(1))
-                            self.addASTChild(currentAST, tmp15_AST)
-                            self.match(ID)
-                        elif la1 and la1 in [LPAREN]:
-                            pass
-                            self.valueExpr()
-                            self.addASTChild(currentAST, self.returnAST)
-                        else:
-                                raise antlr.NoViableAltException(self.LT(1), self.getFilename())
-                            
-                    else:
-                        break
-                    
                 primaryExpr_AST = currentAST.root
             elif la1 and la1 in [LBRACK]:
                 pass
                 self.list_()
                 self.addASTChild(currentAST, self.returnAST)
                 primaryExpr_AST = currentAST.root
             else:
@@ -589,26 +563,26 @@
                 elif (_tokenSet_11.member(self.LA(1))) and (_tokenSet_12.member(self.LA(2))):
                     pass
                     self.atom()
                     self.addASTChild(currentAST, self.returnAST)
                     while True:
                         if (self.LA(1)==DOT):
                             pass
-                            tmp16_AST = None
-                            tmp16_AST = self.astFactory.create(self.LT(1))
-                            self.makeASTRoot(currentAST, tmp16_AST)
+                            tmp14_AST = None
+                            tmp14_AST = self.astFactory.create(self.LT(1))
+                            self.makeASTRoot(currentAST, tmp14_AST)
                             self.match(DOT)
                             la1 = self.LA(1)
                             if False:
                                 pass
                             elif la1 and la1 in [ID]:
                                 pass
-                                tmp17_AST = None
-                                tmp17_AST = self.astFactory.create(self.LT(1))
-                                self.addASTChild(currentAST, tmp17_AST)
+                                tmp15_AST = None
+                                tmp15_AST = self.astFactory.create(self.LT(1))
+                                self.addASTChild(currentAST, tmp15_AST)
                                 self.match(ID)
                             elif la1 and la1 in [LPAREN]:
                                 pass
                                 self.valueExpr()
                                 self.addASTChild(currentAST, self.returnAST)
                             else:
                                     raise antlr.NoViableAltException(self.LT(1), self.getFilename())
@@ -705,38 +679,38 @@
         atom_AST = None
         try:      ## for error handling
             la1 = self.LA(1)
             if False:
                 pass
             elif la1 and la1 in [ID]:
                 pass
-                tmp20_AST = None
-                tmp20_AST = self.astFactory.create(self.LT(1))
-                self.addASTChild(currentAST, tmp20_AST)
+                tmp18_AST = None
+                tmp18_AST = self.astFactory.create(self.LT(1))
+                self.addASTChild(currentAST, tmp18_AST)
                 self.match(ID)
                 atom_AST = currentAST.root
             elif la1 and la1 in [STRING]:
                 pass
-                tmp21_AST = None
-                tmp21_AST = self.astFactory.create(self.LT(1))
-                self.addASTChild(currentAST, tmp21_AST)
+                tmp19_AST = None
+                tmp19_AST = self.astFactory.create(self.LT(1))
+                self.addASTChild(currentAST, tmp19_AST)
                 self.match(STRING)
                 atom_AST = currentAST.root
             elif la1 and la1 in [INT]:
                 pass
-                tmp22_AST = None
-                tmp22_AST = self.astFactory.create(self.LT(1))
-                self.addASTChild(currentAST, tmp22_AST)
+                tmp20_AST = None
+                tmp20_AST = self.astFactory.create(self.LT(1))
+                self.addASTChild(currentAST, tmp20_AST)
                 self.match(INT)
                 atom_AST = currentAST.root
             elif la1 and la1 in [ANONYMOUS_TEMPLATE]:
                 pass
-                tmp23_AST = None
-                tmp23_AST = self.astFactory.create(self.LT(1))
-                self.addASTChild(currentAST, tmp23_AST)
+                tmp21_AST = None
+                tmp21_AST = self.astFactory.create(self.LT(1))
+                self.addASTChild(currentAST, tmp21_AST)
                 self.match(ANONYMOUS_TEMPLATE)
                 atom_AST = currentAST.root
             else:
                     raise antlr.NoViableAltException(self.LT(1), self.getFilename())
                 
         
         except antlr.RecognitionException, ex:
@@ -788,47 +762,47 @@
         try:      ## for error handling
             pass
             la1 = self.LA(1)
             if False:
                 pass
             elif la1 and la1 in [LITERAL_first]:
                 pass
-                tmp25_AST = None
-                tmp25_AST = self.astFactory.create(self.LT(1))
-                self.addASTChild(currentAST, tmp25_AST)
+                tmp23_AST = None
+                tmp23_AST = self.astFactory.create(self.LT(1))
+                self.addASTChild(currentAST, tmp23_AST)
                 self.match(LITERAL_first)
             elif la1 and la1 in [LITERAL_rest]:
                 pass
-                tmp26_AST = None
-                tmp26_AST = self.astFactory.create(self.LT(1))
-                self.addASTChild(currentAST, tmp26_AST)
+                tmp24_AST = None
+                tmp24_AST = self.astFactory.create(self.LT(1))
+                self.addASTChild(currentAST, tmp24_AST)
                 self.match(LITERAL_rest)
             elif la1 and la1 in [LITERAL_last]:
                 pass
-                tmp27_AST = None
-                tmp27_AST = self.astFactory.create(self.LT(1))
-                self.addASTChild(currentAST, tmp27_AST)
+                tmp25_AST = None
+                tmp25_AST = self.astFactory.create(self.LT(1))
+                self.addASTChild(currentAST, tmp25_AST)
                 self.match(LITERAL_last)
             elif la1 and la1 in [LITERAL_length]:
                 pass
-                tmp28_AST = None
-                tmp28_AST = self.astFactory.create(self.LT(1))
-                self.addASTChild(currentAST, tmp28_AST)
+                tmp26_AST = None
+                tmp26_AST = self.astFactory.create(self.LT(1))
+                self.addASTChild(currentAST, tmp26_AST)
                 self.match(LITERAL_length)
             elif la1 and la1 in [LITERAL_strip]:
                 pass
-                tmp29_AST = None
-                tmp29_AST = self.astFactory.create(self.LT(1))
-                self.addASTChild(currentAST, tmp29_AST)
+                tmp27_AST = None
+                tmp27_AST = self.astFactory.create(self.LT(1))
+                self.addASTChild(currentAST, tmp27_AST)
                 self.match(LITERAL_strip)
             elif la1 and la1 in [LITERAL_trunc]:
                 pass
-                tmp30_AST = None
-                tmp30_AST = self.astFactory.create(self.LT(1))
-                self.addASTChild(currentAST, tmp30_AST)
+                tmp28_AST = None
+                tmp28_AST = self.astFactory.create(self.LT(1))
+                self.addASTChild(currentAST, tmp28_AST)
                 self.match(LITERAL_trunc)
             else:
                     raise antlr.NoViableAltException(self.LT(1), self.getFilename())
                 
             self.singleArg()
             self.addASTChild(currentAST, self.returnAST)
             if not self.inputState.guessing:
@@ -842,15 +816,15 @@
                 currentAST.advanceChildToEnd()
             function_AST = currentAST.root
         
         except antlr.RecognitionException, ex:
             if not self.inputState.guessing:
                 self.reportError(ex)
                 self.consume()
-                self.consumeUntil(_tokenSet_12)
+                self.consumeUntil(_tokenSet_14)
             else:
                 raise ex
         
         self.returnAST = function_AST
     
     def list_(self):    
         
@@ -951,15 +925,15 @@
                 currentAST.advanceChildToEnd()
             singleArg_AST = currentAST.root
         
         except antlr.RecognitionException, ex:
             if not self.inputState.guessing:
                 self.reportError(ex)
                 self.consume()
-                self.consumeUntil(_tokenSet_12)
+                self.consumeUntil(_tokenSet_14)
             else:
                 raise ex
         
         self.returnAST = singleArg_AST
     
     def namedTemplate(self):    
         
@@ -970,17 +944,17 @@
         qid_AST = None
         try:      ## for error handling
             la1 = self.LA(1)
             if False:
                 pass
             elif la1 and la1 in [ID]:
                 pass
-                tmp35_AST = None
-                tmp35_AST = self.astFactory.create(self.LT(1))
-                self.addASTChild(currentAST, tmp35_AST)
+                tmp33_AST = None
+                tmp33_AST = self.astFactory.create(self.LT(1))
+                self.addASTChild(currentAST, tmp33_AST)
                 self.match(ID)
                 self.argList()
                 self.addASTChild(currentAST, self.returnAST)
                 namedTemplate_AST = currentAST.root
             elif la1 and la1 in [LITERAL_super]:
                 pass
                 self.match(LITERAL_super)
@@ -1029,27 +1003,27 @@
                     currentAST.root = argList_AST
                     if (argList_AST != None) and (argList_AST.getFirstChild() != None):
                         currentAST.child = argList_AST.getFirstChild()
                     else:
                         currentAST.child = argList_AST
                     currentAST.advanceChildToEnd()
             else:
-                synPredMatched52 = False
+                synPredMatched49 = False
                 if (self.LA(1)==LPAREN) and (_tokenSet_16.member(self.LA(2))):
-                    _m52 = self.mark()
-                    synPredMatched52 = True
+                    _m49 = self.mark()
+                    synPredMatched49 = True
                     self.inputState.guessing += 1
                     try:
                         pass
                         self.singleArg()
                     except antlr.RecognitionException, pe:
-                        synPredMatched52 = False
-                    self.rewind(_m52)
+                        synPredMatched49 = False
+                    self.rewind(_m49)
                     self.inputState.guessing -= 1
-                if synPredMatched52:
+                if synPredMatched49:
                     pass
                     self.singleArg()
                     self.addASTChild(currentAST, self.returnAST)
                     argList_AST = currentAST.root
                 elif (self.LA(1)==LPAREN) and (self.LA(2)==ID or self.LA(2)==DOTDOTDOT):
                     pass
                     self.match(LPAREN)
@@ -1096,21 +1070,21 @@
         self.returnAST = None
         currentAST = antlr.ASTPair()
         indirectTemplate_AST = None
         e_AST = None
         args_AST = None
         try:      ## for error handling
             pass
-            tmp43_AST = None
-            tmp43_AST = self.astFactory.create(self.LT(1))
+            tmp41_AST = None
+            tmp41_AST = self.astFactory.create(self.LT(1))
             self.match(LPAREN)
             self.templatesExpr()
             e_AST = self.returnAST
-            tmp44_AST = None
-            tmp44_AST = self.astFactory.create(self.LT(1))
+            tmp42_AST = None
+            tmp42_AST = self.astFactory.create(self.LT(1))
             self.match(RPAREN)
             self.argList()
             args_AST = self.returnAST
             if not self.inputState.guessing:
                 indirectTemplate_AST = currentAST.root
                 indirectTemplate_AST = antlr.make(self.astFactory.create(VALUE,"value"), e_AST, args_AST)
                 currentAST.root = indirectTemplate_AST
@@ -1174,30 +1148,30 @@
         argumentAssignment_AST = None
         try:      ## for error handling
             la1 = self.LA(1)
             if False:
                 pass
             elif la1 and la1 in [ID]:
                 pass
-                tmp45_AST = None
-                tmp45_AST = self.astFactory.create(self.LT(1))
-                self.addASTChild(currentAST, tmp45_AST)
+                tmp43_AST = None
+                tmp43_AST = self.astFactory.create(self.LT(1))
+                self.addASTChild(currentAST, tmp43_AST)
                 self.match(ID)
-                tmp46_AST = None
-                tmp46_AST = self.astFactory.create(self.LT(1))
-                self.makeASTRoot(currentAST, tmp46_AST)
+                tmp44_AST = None
+                tmp44_AST = self.astFactory.create(self.LT(1))
+                self.makeASTRoot(currentAST, tmp44_AST)
                 self.match(ASSIGN)
                 self.nonAlternatingTemplateExpr()
                 self.addASTChild(currentAST, self.returnAST)
                 argumentAssignment_AST = currentAST.root
             elif la1 and la1 in [DOTDOTDOT]:
                 pass
-                tmp47_AST = None
-                tmp47_AST = self.astFactory.create(self.LT(1))
-                self.addASTChild(currentAST, tmp47_AST)
+                tmp45_AST = None
+                tmp45_AST = self.astFactory.create(self.LT(1))
+                self.addASTChild(currentAST, tmp45_AST)
                 self.match(DOTDOTDOT)
                 argumentAssignment_AST = currentAST.root
             else:
                     raise antlr.NoViableAltException(self.LT(1), self.getFilename())
                 
         
         except antlr.RecognitionException, ex:
```

### Comparing `stringtemplate3-3.1/stringtemplate3/language/ConditionalExpr.py` & `stringtemplate3-3.1b1/stringtemplate3/language/ConditionalExpr.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/language/FormalArgument.py` & `stringtemplate3-3.1b1/stringtemplate3/language/FormalArgument.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/writers.py` & `stringtemplate3-3.1b1/stringtemplate3/writers.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/stringtemplate3/templates.py` & `stringtemplate3-3.1b1/stringtemplate3/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,15 +643,15 @@
         """
         
         if self.formalArguments != UNKNOWN_ARGS and \
            not self.hasFormalArgument(name):
             # a normal call to setAttribute with unknown attribute
             raise KeyError("no such attribute: " + name +
                " in template context " + self.enclosingInstanceStackString)
-        if value is not None:
+        if value:
             attributes[name] = value
         elif isinstance(value, list) or \
              isinstance(value, dict) or \
              isinstance(value, set):
             attributes[name] = value
```

### Comparing `stringtemplate3-3.1/stringtemplate3/groups.py` & `stringtemplate3-3.1b1/stringtemplate3/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,16 +201,14 @@
             else:
                 self.templateLexerClass = AngleBracketTemplateLexer.Lexer
 
             assert superGroup is None or isinstance(superGroup, StringTemplateGroup)
             self.superGroup = superGroup
 
             self.parseGroup(file)
-            assert self.name is not None
-            StringTemplateGroup.nameToGroupMap[self.name] = self
             self.verifyInterfaceImplementations()
 
 
     def getTemplateLexerClass(self):
         """
         What lexer class to use to break up templates.  If not lexer set
         for this group, use static default.
@@ -255,32 +253,25 @@
 
 
     def setSuperGroup(self, superGroup):
         if superGroup is None or isinstance(superGroup, StringTemplateGroup):
             self._superGroup = superGroup
             
         elif isinstance(superGroup, basestring):
-            # Called by group parser when ": supergroupname" is found.
-            # This method forces the supergroup's lexer to be same as lexer
-            # for this (sub) group.
-
-            superGroupName = superGroup
-            superGroup = StringTemplateGroup.nameToGroupMap.get(
-                superGroupName, None)
-            if superGroup is not None:
+            group = StringTemplateGroup.nameToGroupMap.get(superGroup, None)
+            if group is not None:
                 # we've seen before; just use it
-                self.superGroup = superGroup
+                self.superGroup = group
 
             else:
-                # else load it using this group's template lexer
-                superGroup = self.loadGroup(
-                    superGroupName, lexer=self.templateLexerClass)
-                if superGroup is not None:
-                    StringTemplateGroup.nameToGroupMap[superGroup] = superGroup
-                    self._superGroup = superGroup
+                # else load it
+                group = self.loadGroup(superGroup)
+                if group is not None:
+                    StringTemplateGroup.nameToGroupMap[superGroup] = group
+                    self._superGroup = group
 
                 elif self.groupLoader is None:
                     self.listener.error("no group loader registered", None)
 
         else:
             raise TypeError(
                 "Need StringTemplateGroup or string, got %s"
@@ -291,26 +282,14 @@
         return self._superGroup
 
     superGroup = property(getSuperGroup, setSuperGroup)
     getSuperGroup = deprecated(getSuperGroup)
     setSuperGroup = deprecated(setSuperGroup)
     
 
-    def getGroupHierarchyStackString(self):
-        """Walk up group hierarchy and show top down to this group"""
-
-        groupNames = []
-        p = self
-        while p is not None:
-            groupNames.insert(0, p.name)
-            p = p.superGroup
-
-        return '[' + ' '.join(groupNames) + ']'
-
-
     @deprecated
     def getRootDir(self):
         return self.rootDir
 
     @deprecated
     def setRootDir(self, rootDir):
         self.rootDir = rootDir
@@ -438,16 +417,14 @@
                 self.templates[name] = StringTemplateGroup.NOT_FOUND_ST
                 context = ""
                 if enclosingInstance is not None:
                     context = (
                         "; context is "+
                         enclosingInstance.enclosingInstanceStackString
                         )
-                hier = self.getGroupHierarchyStackString()
-                context += "; group hierarchy is "+hier
                 raise ValueError(
                     "Can't load template " +
                     self.getFileNameFromTemplateName(name) +
                     context
                     )
 
         elif st is StringTemplateGroup.NOT_FOUND_ST:
@@ -754,21 +731,19 @@
         if not self.attributeRenderers:
             if not self.superGroup:
                 return None # no renderers and no parent?  Stop.
             # no renderers; consult super group
             return self.superGroup.getAttributeRenderer(attributeClassType)
 
         if self.attributeRenderers.has_key(attributeClassType):
-            return self.attributeRenderers[attributeClassType]
-
-        elif self.superGroup is not None:
+            renderer = self.attributeRenderers[attributeClassType]
+        else:
             # no renderer registered for this class, check super group
-            return self.superGroup.getAttributeRenderer(attributeClassType)
-        
-        return None
+            renderer = self.superGroup.getAttributeRenderer(attributeClassType)
+        return renderer
 
     def getMap(self, name):
         if not self.maps:
             if not self.superGroup:
                 return None
             return self.superGroup.getMap(name)
         m = None
@@ -791,17 +766,17 @@
         cls.groupLoader = loader
 
     @classmethod
     def registerDefaultLexer(cls, lexerClass):
         cls.defaultTemplateLexerClass = lexerClass
 
     @classmethod
-    def loadGroup(cls, name, superGroup=None, lexer=None):
+    def loadGroup(cls, name, superGroup=None):
         if cls.groupLoader is not None:
-            return cls.groupLoader.loadGroup(name, superGroup, lexer)
+            return cls.groupLoader.loadGroup(name, superGroup)
 
         return None
     
     @classmethod
     def loadInterface(cls, name):
         if cls.groupLoader is not None:
             return cls.groupLoader.loadInterface(name)
```

### Comparing `stringtemplate3-3.1/stringtemplate3/__init__.py` & `stringtemplate3-3.1b1/stringtemplate3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 __all__ = ['language']
 
-__version__ = "3.1"
+__version__ = "3.1b1"
 
 ## track probable issues like setting attribute that is not referenced.
 #  Set to true to make StringTemplate check your work as it evaluates
 #  templates.  Problems are sent to error listener.  Currently warns when
 #  you set attributes that are not used.
 lintMode = False
```

### Comparing `stringtemplate3-3.1/stringtemplate3/grouploaders.py` & `stringtemplate3-3.1b1/stringtemplate3/grouploaders.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,32 +30,29 @@
 import os
 import traceback
 import codecs
 
 from stringtemplate3.utils import deprecated
 from stringtemplate3.groups import StringTemplateGroup
 from stringtemplate3.interfaces import StringTemplateGroupInterface
-from stringtemplate3.language import AngleBracketTemplateLexer
 
 
 class StringTemplateGroupLoader(object):
     """
     When group files derive from another group, we have to know how to
     load that group and its supergroups. This interface also knows how
     to load interfaces
     """
 
-    def loadGroup(self, groupName, superGroup=None, lexer=None):
+    def loadGroup(self, groupName, superGroup=None):
         """
         Load the group called groupName from somewhere.  Return null
         if no group is found.
         Groups with region definitions must know their supergroup to find
         templates during parsing.
-        Specify the template lexer to use for parsing templates.  If null,
-        it assumes angle brackets <...>.
         """
         
         raise NotImplementedError
 
 
     def loadInterface(self, interfaceName):
         """
@@ -86,27 +83,24 @@
         self.errors = errors
 
         ## How are the files encoded (ascii, UTF8, ...)?
         #  You might want to read UTF8 for example on an ascii machine.
         self.fileCharEncoding = sys.getdefaultencoding()
         
 
-    def loadGroup(self, groupName, superGroup=None, lexer=None):
-        if lexer is None:
-            lexer = AngleBracketTemplateLexer.Lexer
+    def loadGroup(self, groupName, superGroup=None):
         try:
             fr = self.locate(groupName+".stg")
             if fr is None:
                 self.error("no such group file "+groupName+".stg")
                 return None
 
             try:
                 return StringTemplateGroup(
                     file=fr,
-                    lexer=lexer,
                     errors=self.errors,
                     superGroup=superGroup
                     )
             finally:
                 fr.close()
 
         except IOError, ioe:
```

### Comparing `stringtemplate3-3.1/stringtemplate3/errors.py` & `stringtemplate3-3.1b1/stringtemplate3/errors.py`

 * *Files identical despite different names*

### Comparing `stringtemplate3-3.1/setup.py` & `stringtemplate3-3.1b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
 
 setup(
     name="stringtemplate3",
-    version="3.1",
+    version="3.1b1",
     description="A powerful template engine with strict model-view separation",
     long_description="""
     ST (StringTemplate) is a template engine for generating source code, web
     pages, emails, or any other formatted text output. ST is particularly
     good at multi-targeted code generators, multiple site skins, and
     internationalization/localization. It evolved over years of effort
     developing jGuru.com. ST also generates this website and powers the
     ANTLR v3 code generator. Its distinguishing characteristic is that it
     strictly enforces model-view separation unlike other engines.
     """,
     classifiers=[
-    'Development Status :: 5 - Production/Stable',
+    'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Text Processing',
     ],
```

### Comparing `stringtemplate3-3.1/LICENSE.txt` & `stringtemplate3-3.1b1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [The "BSD licence"]
-Copyright (c) 2003-2008 Terence Parr
+Copyright (c) 2003-2007 Terence Parr
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
  1. Redistributions of source code must retain the above copyright
```

