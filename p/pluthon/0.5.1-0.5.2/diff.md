# Comparing `tmp/pluthon-0.5.1.tar.gz` & `tmp/pluthon-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluthon-0.5.1.tar", last modified: Sun Mar  3 21:44:55 2024, max compression
+gzip compressed data, was "pluthon-0.5.2.tar", last modified: Tue Apr  2 13:49:10 2024, max compression
```

## Comparing `pluthon-0.5.1.tar` & `pluthon-0.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-03-03 21:44:55.667839 pluthon-0.5.1/
--rw-r--r--   0 travis    (1000) travis    (1000)     1953 2024-03-03 21:44:55.667839 pluthon-0.5.1/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     1001 2024-03-03 21:43:51.000000 pluthon-0.5.1/README.md
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-03-03 21:44:55.663838 pluthon-0.5.1/pluthon/
--rw-r--r--   0 travis    (1000) travis    (1000)      647 2024-03-03 21:43:51.000000 pluthon-0.5.1/pluthon/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1937 2024-03-03 21:43:51.000000 pluthon-0.5.1/pluthon/compiler_config.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-03-03 21:44:55.667839 pluthon-0.5.1/pluthon/optimize/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2024-03-03 21:43:51.000000 pluthon-0.5.1/pluthon/optimize/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1147 2024-03-03 21:43:51.000000 pluthon-0.5.1/pluthon/optimize/constant_index_access_list.py
--rw-r--r--   0 travis    (1000) travis    (1000)     9675 2024-03-03 21:43:51.000000 pluthon-0.5.1/pluthon/optimize/patterns.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5398 2024-03-03 21:43:51.000000 pluthon-0.5.1/pluthon/pluthon_ast.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2694 2024-03-03 21:43:51.000000 pluthon-0.5.1/pluthon/pluthon_functional_data.py
--rw-r--r--   0 travis    (1000) travis    (1000)    29811 2024-03-03 21:43:51.000000 pluthon-0.5.1/pluthon/pluthon_sugar.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1215 2024-03-03 21:43:51.000000 pluthon-0.5.1/pluthon/tools.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5041 2024-03-03 21:43:51.000000 pluthon-0.5.1/pluthon/util.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-03-03 21:44:55.667839 pluthon-0.5.1/pluthon.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     1953 2024-03-03 21:44:55.000000 pluthon-0.5.1/pluthon.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      440 2024-03-03 21:44:55.000000 pluthon-0.5.1/pluthon.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2024-03-03 21:44:55.000000 pluthon-0.5.1/pluthon.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      112 2024-03-03 21:44:55.000000 pluthon-0.5.1/pluthon.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       13 2024-03-03 21:44:55.000000 pluthon-0.5.1/pluthon.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2024-03-03 21:44:55.667839 pluthon-0.5.1/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     1842 2024-03-03 21:43:51.000000 pluthon-0.5.1/setup.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-04-02 13:49:10.779774 pluthon-0.5.2/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1953 2024-04-02 13:49:10.779774 pluthon-0.5.2/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)     1001 2024-04-02 13:48:05.000000 pluthon-0.5.2/README.md
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-04-02 13:49:10.775774 pluthon-0.5.2/pluthon/
+-rw-r--r--   0 travis    (1000) travis    (1000)      647 2024-04-02 13:48:05.000000 pluthon-0.5.2/pluthon/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1937 2024-04-02 13:48:05.000000 pluthon-0.5.2/pluthon/compiler_config.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-04-02 13:49:10.779774 pluthon-0.5.2/pluthon/optimize/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2024-04-02 13:48:05.000000 pluthon-0.5.2/pluthon/optimize/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1147 2024-04-02 13:48:05.000000 pluthon-0.5.2/pluthon/optimize/constant_index_access_list.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     9675 2024-04-02 13:48:05.000000 pluthon-0.5.2/pluthon/optimize/patterns.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5398 2024-04-02 13:48:05.000000 pluthon-0.5.2/pluthon/pluthon_ast.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2694 2024-04-02 13:48:05.000000 pluthon-0.5.2/pluthon/pluthon_functional_data.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    31801 2024-04-02 13:48:05.000000 pluthon-0.5.2/pluthon/pluthon_sugar.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1215 2024-04-02 13:48:05.000000 pluthon-0.5.2/pluthon/tools.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5041 2024-04-02 13:48:05.000000 pluthon-0.5.2/pluthon/util.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2024-04-02 13:49:10.779774 pluthon-0.5.2/pluthon.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1953 2024-04-02 13:49:10.000000 pluthon-0.5.2/pluthon.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      440 2024-04-02 13:49:10.000000 pluthon-0.5.2/pluthon.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2024-04-02 13:49:10.000000 pluthon-0.5.2/pluthon.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      112 2024-04-02 13:49:10.000000 pluthon-0.5.2/pluthon.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       13 2024-04-02 13:49:10.000000 pluthon-0.5.2/pluthon.egg-info/top_level.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       38 2024-04-02 13:49:10.779774 pluthon-0.5.2/setup.cfg
+-rw-r--r--   0 travis    (1000) travis    (1000)     1842 2024-04-02 13:48:05.000000 pluthon-0.5.2/setup.py
```

### Comparing `pluthon-0.5.1/PKG-INFO` & `pluthon-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluthon
-Version: 0.5.1
+Version: 0.5.2
 Summary: Pluto-like programming language for Cardano Smart Contracts in Python
 Home-page: https://github.com/opshin/pluthon
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pluthon-0.5.1/README.md` & `pluthon-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.1/pluthon/__init__.py` & `pluthon-0.5.2/pluthon/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     from .compiler_config import *
 except ImportError as e:
     logging.error(
         "Error, trying to import dependencies. Should only occur upon package installation",
         exc_info=e,
     )
 
-VERSION = (0, 5, 1)
+VERSION = (0, 5, 2)
 
 __version__ = ".".join([str(i) for i in VERSION])
 __author__ = "nielstron"
 __author_email__ = "n.muendler@web.de"
 __copyright__ = "Copyright (C) 2023 nielstron"
 __license__ = "MIT"
 __url__ = "https://github.com/opshin/pluthon"
```

### Comparing `pluthon-0.5.1/pluthon/compiler_config.py` & `pluthon-0.5.2/pluthon/compiler_config.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.1/pluthon/optimize/constant_index_access_list.py` & `pluthon-0.5.2/pluthon/optimize/constant_index_access_list.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.1/pluthon/optimize/patterns.py` & `pluthon-0.5.2/pluthon/optimize/patterns.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.1/pluthon/pluthon_ast.py` & `pluthon-0.5.2/pluthon/pluthon_ast.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.1/pluthon/pluthon_functional_data.py` & `pluthon-0.5.2/pluthon/pluthon_functional_data.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.1/pluthon/pluthon_sugar.py` & `pluthon-0.5.2/pluthon/pluthon_sugar.py`

 * *Files 2% similar despite different names*

```diff
@@ -705,14 +705,86 @@
             ),
             self.key,
             self.l,
         )
 
 
 @dataclass
+class AnyList(Pattern):
+    """Returns whether the key evaluates to true anywhere in the list"""
+
+    l: AST
+    key: AST
+    default: AST
+
+    def compose(self):
+        return Apply(
+            PLambda(
+                ["op"],
+                RecFun(
+                    PLambda(
+                        ["f", "xs"],
+                        IteNullList(
+                            PVar("xs"),
+                            Bool(False),
+                            Ite(
+                                Apply(PVar("op"), HeadList(PVar("xs"))),
+                                Bool(True),
+                                Apply(
+                                    PVar("f"),
+                                    PVar("f"),
+                                    TailList(PVar("xs")),
+                                ),
+                            ),
+                        ),
+                    ),
+                ),
+            ),
+            self.key,
+            self.l,
+        )
+
+
+@dataclass
+class AllList(Pattern):
+    """Returns whether the key evaluates to true everywhere in the list"""
+
+    l: AST
+    key: AST
+    default: AST
+
+    def compose(self):
+        return Apply(
+            PLambda(
+                ["op"],
+                RecFun(
+                    PLambda(
+                        ["f", "xs"],
+                        IteNullList(
+                            PVar("xs"),
+                            Bool(True),
+                            Ite(
+                                Apply(PVar("op"), HeadList(PVar("xs"))),
+                                Apply(
+                                    PVar("f"),
+                                    PVar("f"),
+                                    TailList(PVar("xs")),
+                                ),
+                                Bool(False),
+                            ),
+                        ),
+                    ),
+                ),
+            ),
+            self.key,
+            self.l,
+        )
+
+
+@dataclass
 class FilterList(Pattern):
     """Apply a filter function on each element in a list (throws out all that evaluate to false)"""
 
     l: AST
     k: AST
     empty_list: AST = field(default_factory=EmptyDataList)
```

### Comparing `pluthon-0.5.1/pluthon/tools.py` & `pluthon-0.5.2/pluthon/tools.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.1/pluthon/util.py` & `pluthon-0.5.2/pluthon/util.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.5.1/pluthon.egg-info/PKG-INFO` & `pluthon-0.5.2/pluthon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluthon
-Version: 0.5.1
+Version: 0.5.2
 Summary: Pluto-like programming language for Cardano Smart Contracts in Python
 Home-page: https://github.com/opshin/pluthon
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pluthon-0.5.1/setup.py` & `pluthon-0.5.2/setup.py`

 * *Files identical despite different names*

