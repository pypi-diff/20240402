# Comparing `tmp/ailment-9.2.96.tar.gz` & `tmp/ailment-9.2.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailment-9.2.96.tar", last modified: Tue Mar 26 17:01:52 2024, max compression
+gzip compressed data, was "ailment-9.2.97.tar", last modified: Tue Apr  2 17:02:16 2024, max compression
```

## Comparing `ailment-9.2.96.tar` & `ailment-9.2.97.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:52.289903 ailment-9.2.96/
--rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-03-26 17:00:58.000000 ailment-9.2.96/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     1584 2024-03-26 17:01:52.289903 ailment-9.2.96/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-03-26 17:00:58.000000 ailment-9.2.96/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:52.285903 ailment-9.2.96/ailment/
--rw-r--r--   0 vsts      (1001) docker     (127)     2014 2024-03-26 17:01:07.000000 ailment-9.2.96/ailment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2260 2024-03-26 17:00:58.000000 ailment-9.2.96/ailment/block.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19143 2024-03-26 17:00:58.000000 ailment-9.2.96/ailment/block_walker.py
--rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-03-26 17:00:58.000000 ailment-9.2.96/ailment/converter_common.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23721 2024-03-26 17:00:58.000000 ailment-9.2.96/ailment/converter_pcode.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26382 2024-03-26 17:00:58.000000 ailment-9.2.96/ailment/converter_vex.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36404 2024-03-26 17:00:58.000000 ailment-9.2.96/ailment/expression.py
--rw-r--r--   0 vsts      (1001) docker     (127)      704 2024-03-26 17:00:58.000000 ailment-9.2.96/ailment/manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20109 2024-03-26 17:00:58.000000 ailment-9.2.96/ailment/statement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1538 2024-03-26 17:00:58.000000 ailment-9.2.96/ailment/tagged_object.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2665 2024-03-26 17:00:58.000000 ailment-9.2.96/ailment/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:52.289903 ailment-9.2.96/ailment.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1584 2024-03-26 17:01:52.000000 ailment-9.2.96/ailment.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-03-26 17:01:52.000000 ailment-9.2.96/ailment.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-26 17:01:52.000000 ailment-9.2.96/ailment.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-03-26 17:01:52.000000 ailment-9.2.96/ailment.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-03-26 17:01:52.000000 ailment-9.2.96/ailment.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-03-26 17:01:07.000000 ailment-9.2.96/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)      820 2024-03-26 17:01:52.289903 ailment-9.2.96/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:52.289903 ailment-9.2.96/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)     1479 2024-03-26 17:00:58.000000 ailment-9.2.96/tests/test_irsb.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:16.842342 ailment-9.2.97/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-04-02 17:01:35.000000 ailment-9.2.97/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     1584 2024-04-02 17:02:16.842342 ailment-9.2.97/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-02 17:01:35.000000 ailment-9.2.97/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:16.838342 ailment-9.2.97/ailment/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2014 2024-04-02 17:01:43.000000 ailment-9.2.97/ailment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2260 2024-04-02 17:01:35.000000 ailment-9.2.97/ailment/block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19143 2024-04-02 17:01:35.000000 ailment-9.2.97/ailment/block_walker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-04-02 17:01:35.000000 ailment-9.2.97/ailment/converter_common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23721 2024-04-02 17:01:35.000000 ailment-9.2.97/ailment/converter_pcode.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26673 2024-04-02 17:01:35.000000 ailment-9.2.97/ailment/converter_vex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36737 2024-04-02 17:01:35.000000 ailment-9.2.97/ailment/expression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      704 2024-04-02 17:01:35.000000 ailment-9.2.97/ailment/manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20109 2024-04-02 17:01:35.000000 ailment-9.2.97/ailment/statement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1538 2024-04-02 17:01:35.000000 ailment-9.2.97/ailment/tagged_object.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2665 2024-04-02 17:01:35.000000 ailment-9.2.97/ailment/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:16.842342 ailment-9.2.97/ailment.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1584 2024-04-02 17:02:16.000000 ailment-9.2.97/ailment.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-04-02 17:02:16.000000 ailment-9.2.97/ailment.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-02 17:02:16.000000 ailment-9.2.97/ailment.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-04-02 17:02:16.000000 ailment-9.2.97/ailment.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-04-02 17:02:16.000000 ailment-9.2.97/ailment.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-04-02 17:01:43.000000 ailment-9.2.97/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)      820 2024-04-02 17:02:16.842342 ailment-9.2.97/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:16.842342 ailment-9.2.97/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1479 2024-04-02 17:01:35.000000 ailment-9.2.97/tests/test_irsb.py
```

### Comparing `ailment-9.2.96/LICENSE` & `ailment-9.2.97/LICENSE`

 * *Files identical despite different names*

### Comparing `ailment-9.2.96/PKG-INFO` & `ailment-9.2.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ailment
-Version: 9.2.96
+Version: 9.2.97
 Summary: The angr intermediate language.
 Home-page: https://github.com/angr/ailment
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ailment-9.2.96/README.md` & `ailment-9.2.97/README.md`

 * *Files identical despite different names*

### Comparing `ailment-9.2.96/ailment/__init__.py` & `ailment-9.2.97/ailment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "9.2.96"
+__version__ = "9.2.97"
 
 import logging
 from typing import Set
 
 from .block import Block
 from . import statement as Stmt
 from . import expression as Expr
```

### Comparing `ailment-9.2.96/ailment/block.py` & `ailment-9.2.97/ailment/block.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.96/ailment/block_walker.py` & `ailment-9.2.97/ailment/block_walker.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.96/ailment/converter_pcode.py` & `ailment-9.2.97/ailment/converter_pcode.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.96/ailment/converter_vex.py` & `ailment-9.2.97/ailment/converter_vex.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,23 +291,29 @@
                     ins_addr=manager.ins_addr,
                     vex_block_addr=manager.block_addr,
                     vex_stmt_idx=manager.vex_stmt_idx,
                 )
 
         bits = op._output_size_bits
 
+        extra_kwargs = {}
+        if op_name == "DivMod":
+            extra_kwargs["from_bits"] = op._from_size if op._from_size is not None else operands[1].bits
+            extra_kwargs["to_bits"] = op._to_size if op._to_size is not None else operands[1].bits
+
         return BinaryOp(
             manager.next_atom(),
             op_name,
             operands,
             signed,
             ins_addr=manager.ins_addr,
             vex_block_addr=manager.block_addr,
             vex_stmt_idx=manager.vex_stmt_idx,
             bits=bits,
+            **extra_kwargs,
         )
 
     @staticmethod
     def Triop(expr, manager):
         op = VEXExprConverter.simop_from_vexop(expr.op)
         op_name = op._generic_name
         operands = VEXExprConverter.convert_list(expr.args, manager)
```

### Comparing `ailment-9.2.96/ailment/expression.py` & `ailment-9.2.97/ailment/expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,14 +459,16 @@
         "operands",
         "bits",
         "signed",
         "variable",
         "variable_offset",
         "floating_point",
         "rounding_mode",
+        "from_bits",  # for divmod
+        "to_bits",  # for divmod
     )
 
     OPSTR_MAP = {
         "Add": "+",
         "AddF": "+",
         "AddV": "+",
         "Sub": "-",
@@ -525,14 +527,16 @@
         operands,
         signed,
         variable=None,
         variable_offset=None,
         bits=None,
         floating_point=False,
         rounding_mode=None,
+        from_bits=None,
+        to_bits=None,
         **kwargs,
     ):
         depth = (
             max(
                 operands[0].depth if isinstance(operands[0], Expression) else 0,
                 operands[1].depth if isinstance(operands[1], Expression) else 0,
             )
@@ -573,14 +577,17 @@
             self.bits = get_bits(operands[0]) if not isinstance(operands[0], int) else get_bits(operands[1])
         self.signed = signed
         self.variable = variable
         self.variable_offset = variable_offset
         self.floating_point = floating_point
         self.rounding_mode = rounding_mode
 
+        self.from_bits = from_bits
+        self.to_bits = to_bits
+
         # TODO: sanity check of operands' sizes for some ops
         # assert self.bits == operands[1].bits
 
     def __str__(self):
         op_str = self.OPSTR_MAP.get(self.verbose_op, self.verbose_op)
         return f"({str(self.operands[0])} {op_str} {str(self.operands[1])})"
 
@@ -658,14 +665,16 @@
                 self.idx,
                 self.op,
                 [replaced_operand_0, replaced_operand_1],
                 self.signed,
                 bits=self.bits,
                 floating_point=self.floating_point,
                 rounding_mode=self.rounding_mode,
+                from_bits=self.from_bits,
+                to_bits=self.to_bits,
                 **self.tags,
             )
         else:
             return False, self
 
     @property
     def verbose_op(self):
@@ -688,14 +697,16 @@
             self.operands[::],
             self.signed,
             variable=self.variable,
             variable_offset=self.variable_offset,
             bits=self.bits,
             floating_point=self.floating_point,
             rounding_mode=self.rounding_mode,
+            from_bits=self.from_bits,
+            to_bits=self.to_bits,
             **self.tags,
         )
 
 
 class TernaryOp(Op):
     OPSTR_MAP = {}
```

### Comparing `ailment-9.2.96/ailment/manager.py` & `ailment-9.2.97/ailment/manager.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.96/ailment/statement.py` & `ailment-9.2.97/ailment/statement.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.96/ailment/tagged_object.py` & `ailment-9.2.97/ailment/tagged_object.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.96/ailment/utils.py` & `ailment-9.2.97/ailment/utils.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.96/ailment.egg-info/PKG-INFO` & `ailment-9.2.97/ailment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ailment
-Version: 9.2.96
+Version: 9.2.97
 Summary: The angr intermediate language.
 Home-page: https://github.com/angr/ailment
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ailment-9.2.96/setup.cfg` & `ailment-9.2.97/setup.cfg`

 * *Files identical despite different names*

### Comparing `ailment-9.2.96/tests/test_irsb.py` & `ailment-9.2.97/tests/test_irsb.py`

 * *Files identical despite different names*

