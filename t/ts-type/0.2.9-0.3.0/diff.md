# Comparing `tmp/ts_type-0.2.9.tar.gz` & `tmp/ts_type-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts_type-0.2.9.tar", last modified: Fri Aug  4 08:56:04 2023, max compression
+gzip compressed data, was "ts_type-0.3.0.tar", last modified: Tue Apr  2 07:57:43 2024, max compression
```

## Comparing `ts_type-0.2.9.tar` & `ts_type-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:56:04.891854 ts_type-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-04 08:55:54.000000 ts_type-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-08-04 08:56:04.891854 ts_type-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-08-04 08:55:54.000000 ts_type-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 08:55:54.000000 ts_type-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 08:56:04.891854 ts_type-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-04 08:55:54.000000 ts_type-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:56:04.887854 ts_type-0.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-08-04 08:55:54.000000 ts_type-0.2.9/tests/test_ts_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:56:04.891854 ts_type-0.2.9/ts_type/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-08-04 08:55:54.000000 ts_type-0.2.9/ts_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-08-04 08:55:54.000000 ts_type-0.2.9/ts_type/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-04 08:55:54.000000 ts_type-0.2.9/ts_type/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-04 08:55:54.000000 ts_type-0.2.9/ts_type/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    15679 2023-08-04 08:55:54.000000 ts_type-0.2.9/ts_type/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:55:54.000000 ts_type-0.2.9/ts_type/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-08-04 08:55:54.000000 ts_type-0.2.9/ts_type/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 08:55:54.000000 ts_type-0.2.9/ts_type/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:56:04.891854 ts_type-0.2.9/ts_type.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-08-04 08:56:04.000000 ts_type-0.2.9/ts_type.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-04 08:56:04.000000 ts_type-0.2.9/ts_type.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:56:04.000000 ts_type-0.2.9/ts_type.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 08:56:04.000000 ts_type-0.2.9/ts_type.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:57:43.968841 ts_type-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 07:57:40.000000 ts_type-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-04-02 07:57:43.964841 ts_type-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-04-02 07:57:40.000000 ts_type-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 07:57:40.000000 ts_type-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:57:43.968841 ts_type-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-02 07:57:40.000000 ts_type-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:57:43.964841 ts_type-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13147 2024-04-02 07:57:40.000000 ts_type-0.3.0/tests/test_ts_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:57:43.964841 ts_type-0.3.0/ts_type/
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-02 07:57:40.000000 ts_type-0.3.0/ts_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-04-02 07:57:40.000000 ts_type-0.3.0/ts_type/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 07:57:40.000000 ts_type-0.3.0/ts_type/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-02 07:57:40.000000 ts_type-0.3.0/ts_type/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15679 2024-04-02 07:57:40.000000 ts_type-0.3.0/ts_type/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:57:40.000000 ts_type-0.3.0/ts_type/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-02 07:57:40.000000 ts_type-0.3.0/ts_type/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 07:57:40.000000 ts_type-0.3.0/ts_type/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:57:43.964841 ts_type-0.3.0/ts_type.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-04-02 07:57:43.000000 ts_type-0.3.0/ts_type.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-02 07:57:43.000000 ts_type-0.3.0/ts_type.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:57:43.000000 ts_type-0.3.0/ts_type.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 07:57:43.000000 ts_type-0.3.0/ts_type.egg-info/top_level.txt
```

### Comparing `ts_type-0.2.9/LICENSE` & `ts_type-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.9/PKG-INFO` & `ts_type-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts_type
-Version: 0.2.9
+Version: 0.3.0
 Summary: ts_type generates typescript's type from python code
 Home-page: https://github.com/saryou/ts_type
 Author: Ryosuke Sasaki
 Author-email: saryou.ssk@gmail.com
 Project-URL: Bug Tracker, https://github.com/saryou/ts_type/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -129,16 +129,16 @@
 type RequestForApiB = Extract<Apis, {url: "/api/b"}>['request'];
 type ResponseForApiB = Extract<Apis, {url: "/api/b"}>['request'];
 ```
 
 
 ## Basic Usage
 
-1. add types to `TypeDefinitionGenerator`. (you can use `ts_type.generator`, which is an instance of the class)
-2. call `TypeDefinitionGenerator.generate`
+1. Add types to `TypeDefinitionGenerator` with `add` method. (You can use `ts_type.generator`, which is an instance of the class. `ts_type.gen_type` is a shortcut of `ts_type.generator.add`)
+2. Call `TypeDefinitionGenerator.generate`
 
 ```py3
 from dataclasses import dataclass
 from typing import Optional, List, Dict
 
 import ts_type as ts
 
@@ -164,33 +164,35 @@
 
 ```python3
 class Builder(ts.NodeBuilder):
     def handle_unknown_type(self, t: Any) -> ts.TypeNode:
         if isinstance(t, type):
             if issubclass(t, cl.Cleaned):
                 return self.define_cleaned(t)
+            if issubclass(t, cl.Undefined):
+                return ts.Undefined()
         return super().handle_unknown_type(t)
 
     def define_cleaned(self,
-                       t: Type[cl.Cleaned],
+                       t: type[cl.Cleaned],
                        exclude: set[str] = set()) -> ts.TypeNode:
         ret: ts.TypeNode = self.define_ref_node(t, lambda: ts.Object(
             attrs={
                 k: self.type_to_node(self.field_to_type(f))
                 for k, f in t._meta.fields.items()
             },
             omissible={k for k, f in t._meta.fields.items() if f.has_default}))
 
         if (exclude := exclude & set(t._meta.fields)):
             ret = ts.Omit(ret, ts.Union(
                 [self.literal_to_node(k) for k in sorted(exclude)]))
 
         return ret
 
-    def field_to_type(self, t: cl.Field) -> Type:
+    def field_to_type(self, t: cl.Field) -> type:
         if isinstance(t, cl.OptionalField):
             vt = self.field_to_type(t.field)
             return Union[None, cl.Undefined, vt]
         elif isinstance(t, cl.ListField):
             vt = self.field_to_type(t.value)
             return list[vt]
         elif isinstance(t, cl.SetField):
```

### Comparing `ts_type-0.2.9/README.md` & `ts_type-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -114,16 +114,16 @@
 type RequestForApiB = Extract<Apis, {url: "/api/b"}>['request'];
 type ResponseForApiB = Extract<Apis, {url: "/api/b"}>['request'];
 ```
 
 
 ## Basic Usage
 
-1. add types to `TypeDefinitionGenerator`. (you can use `ts_type.generator`, which is an instance of the class)
-2. call `TypeDefinitionGenerator.generate`
+1. Add types to `TypeDefinitionGenerator` with `add` method. (You can use `ts_type.generator`, which is an instance of the class. `ts_type.gen_type` is a shortcut of `ts_type.generator.add`)
+2. Call `TypeDefinitionGenerator.generate`
 
 ```py3
 from dataclasses import dataclass
 from typing import Optional, List, Dict
 
 import ts_type as ts
 
@@ -149,33 +149,35 @@
 
 ```python3
 class Builder(ts.NodeBuilder):
     def handle_unknown_type(self, t: Any) -> ts.TypeNode:
         if isinstance(t, type):
             if issubclass(t, cl.Cleaned):
                 return self.define_cleaned(t)
+            if issubclass(t, cl.Undefined):
+                return ts.Undefined()
         return super().handle_unknown_type(t)
 
     def define_cleaned(self,
-                       t: Type[cl.Cleaned],
+                       t: type[cl.Cleaned],
                        exclude: set[str] = set()) -> ts.TypeNode:
         ret: ts.TypeNode = self.define_ref_node(t, lambda: ts.Object(
             attrs={
                 k: self.type_to_node(self.field_to_type(f))
                 for k, f in t._meta.fields.items()
             },
             omissible={k for k, f in t._meta.fields.items() if f.has_default}))
 
         if (exclude := exclude & set(t._meta.fields)):
             ret = ts.Omit(ret, ts.Union(
                 [self.literal_to_node(k) for k in sorted(exclude)]))
 
         return ret
 
-    def field_to_type(self, t: cl.Field) -> Type:
+    def field_to_type(self, t: cl.Field) -> type:
         if isinstance(t, cl.OptionalField):
             vt = self.field_to_type(t.field)
             return Union[None, cl.Undefined, vt]
         elif isinstance(t, cl.ListField):
             vt = self.field_to_type(t.value)
             return list[vt]
         elif isinstance(t, cl.SetField):
```

### Comparing `ts_type-0.2.9/setup.py` & `ts_type-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.9/tests/test_ts_type.py` & `ts_type-0.3.0/tests/test_ts_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from datetime import datetime, date, time
 from enum import Enum
-from typing import Union, Literal, List, Set, Tuple, Dict, Optional, TypeVar,\
+from typing import Union, Literal, List, Set, Tuple, Dict, Optional, TypeVar, \
     Generic
 from unittest import TestCase
 
 import ts_type as ts
 
 
 T = TypeVar('T')
```

### Comparing `ts_type-0.2.9/ts_type/__init__.py` & `ts_type-0.3.0/ts_type/__init__.py`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.9/ts_type/builders.py` & `ts_type-0.3.0/ts_type/builders.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import json
 import re
 from datetime import datetime, date, time
 from enum import Enum
 from contextlib import contextmanager
 from dataclasses import fields as dc_fields, is_dataclass
 from importlib import import_module
-from typing import Optional, Any, Type, Callable, Union, ForwardRef, TypeVar,\
-    Literal, List, Dict, Set, Tuple, cast, Generic, Sequence
+from typing import Optional, Any, Type, Callable, Union, ForwardRef, TypeVar, \
+    Literal, List, Dict, Set, Tuple, cast, Generic
+from typing import _TypedDictMeta  # type: ignore
+from collections.abc import Sequence, MutableSequence, Mapping, \
+    MutableMapping, Set as AbstractSet, MutableSet
 
 from .exceptions import UnknownTypeError
 from .utils import resolve_typevar
 from . import nodes
 
 
 T = TypeVar('T')
@@ -22,14 +25,27 @@
     def _is_union_type(t: Any) -> bool:
         return isinstance(t, UnionType)
 except ImportError:
     def _is_union_type(t: Any) -> bool:
         return False
 
 
+try:
+    from typing import TypeAliasType  # type: ignore
+
+    def _resolve_type_alias_type(t: Any) -> Any:
+        if isinstance(t, TypeAliasType):
+            return _resolve_type_alias_type(t.__value__)
+        else:
+            return t
+except ImportError:
+    def _resolve_type_alias_type(t: Any) -> Any:
+        return t
+
+
 class NodeBuilder:
     """NodeBuilder converts python objects to typescript's types."""
 
     def __init__(self) -> None:
         self._modules: Dict[str, Any] = {}
         self._definitions: Dict[str, nodes.TypeNode] = {}
         self._stack: List[Tuple[str, str, Any]] = []
@@ -57,14 +73,16 @@
                 lhs = f'{export}type {ref.render(ctx)}'
             rhs = f'{node.render(ctx)};'
             return f'{lhs} = {rhs}'
 
         return '\n\n'.join([render(k) for k in ref_names])
 
     def type_to_node(self, t: Any) -> nodes.TypeNode:
+        t = _resolve_type_alias_type(t)
+
         if t in [None, type(None)]:
             return nodes.Null()
 
         origin = getattr(t, '__origin__', None)
         args: tuple[Any, ...] = getattr(t, '__args__', tuple())
 
         if origin is Union or _is_union_type(t):
@@ -73,35 +91,33 @@
                 return self.type_to_node(args[0])
             return nodes.Union(
                 of=[self.type_to_node(a) for a in args])
         elif origin is tuple:
             assert args
             return nodes.Tuple(
                 [self.type_to_node(a) for a in args])
-        elif origin is list or origin is set:
+        elif origin in [list, set, Sequence, MutableSequence,
+                        AbstractSet, MutableSet]:
             assert args
             return nodes.Array(self.type_to_node(args[0]))
-        elif origin is dict:
+        elif origin in [dict, Mapping, MutableMapping]:
             assert len(args) > 1
             key = self.type_to_node(args[0])
             assert isinstance(key, nodes.DictKeyType)
             return nodes.Dict(
                 key=key,
                 value=self.type_to_node(args[1]))
         elif origin is Literal:
             assert args
             literals = [self.literal_to_node(a) for a in args]
             if len(literals) > 1:
                 return nodes.Union(of=cast(List[nodes.TypeNode], literals))
             return literals[0]
         elif origin:
-            node = self.type_to_node(origin)
-            if isinstance(node, nodes.Reference):
-                node.typevars = [self.type_to_node(t) for t in args]
-            return node
+            return self.handle_generic_type(t, origin, args)
         elif isinstance(t, str):
             return self.type_to_node(self._resolve_annotation(t))
         elif isinstance(t, TypeVar):
             try:
                 _t = self._resolve_typevar(t)
             except AssertionError:
                 return nodes.TypeVariable(typevar=t)
@@ -121,17 +137,28 @@
                 return nodes.Boolean()
             elif issubclass(t, (int, float)):
                 return nodes.Number()
             elif issubclass(t, Enum):
                 return self.enum_to_node(t)
             elif is_dataclass(t):
                 return self.dataclass_to_node(t)
+            elif isinstance(t, _TypedDictMeta):
+                return self.typeddict_to_node(t)
 
         return self.handle_unknown_type(t)
 
+    def handle_generic_type(self,
+                            t: Any,
+                            origin: type,
+                            args: tuple[Any, ...]) -> nodes.TypeNode:
+        node = self.type_to_node(origin)
+        if isinstance(node, nodes.Reference):
+            node.typevars = [self.type_to_node(t) for t in args]
+        return node
+
     def handle_unknown_type(self, t: Any) -> nodes.TypeNode:
         raise UnknownTypeError(f'Type `{t}` is not supported.')
 
     class RefSource:
         def __init__(self,
                      type: Union[type, None],
                      identifier: str):
@@ -199,14 +226,20 @@
         return self.define_ref_node(
             dc,
             lambda: nodes.Object(
                 attrs={f.name: self.type_to_node(f.type)
                        for f in dc_fields(dc)},
                 omissible=set()))
 
+    def typeddict_to_node(self, t: _TypedDictMeta) -> nodes.TypeNode:
+        return self.define_ref_node(t, lambda: nodes.Object(
+            attrs={k: self.type_to_node(v)
+                   for k, v in t.__annotations__.items()},
+            omissible=t.__optional_keys__))
+
     @contextmanager
     def _begin_module_context(self, t: Optional[Type]):
         if t is None:
             yield
             return
 
         self._import_module(t.__module__)
```

### Comparing `ts_type-0.2.9/ts_type/generators.py` & `ts_type-0.3.0/ts_type/generators.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         if output_filepath is None:
             output_filepath = target.__module__.replace('.', '/')
             output_name = target.__name__
         else:
             assert output_filepath
             output_name = output_name or target.__name__
         _types = self.types[output_filepath]
-        assert output_name not in _types,\
+        assert output_name not in _types, \
             f'{target} {output_filepath} {output_name}'
         _types[output_name] = target
 
         return target
 
     def generate(self,
                  output_dir: Union[str, Path],
```

### Comparing `ts_type-0.2.9/ts_type/nodes.py` & `ts_type-0.3.0/ts_type/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
         ret: typing.List[TypeNode] = []
         for node in of:
             if all(n != node for n in ret):
                 ret.append(node)
         return ret
 
     def render(self, context: RenderContext):
-        return ' | '.join([
+        return ' & '.join([
             _render_with_parenthesis(node, context) for node in self.of
         ])
 
     def __eq__(self, other):
         return isinstance(other, Intersection)\
             and self.of == other.of
```

### Comparing `ts_type-0.2.9/ts_type/utils.py` & `ts_type-0.3.0/ts_type/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         arg_index = found[1]
 
         for m in mro[mro_index:]:
             for b in getattr(m, '__orig_bases__', []):
                 args = getattr(b, '__args__', [])
                 if args and len(args) > arg_index:
                     arg = args[arg_index]
-                    assert t not in getattr(arg, '__parameters__', []),\
+                    assert t not in getattr(arg, '__parameters__', []), \
                         'Unsupported usage of generic parameters. '\
                         f'`{t}` has represented other generic type which '\
                         f'contains `{t}` itself (`{arg}` in `{m}`). '\
                         'So we can not determine which use is '\
                         'appropriate in this context. You should substitute '\
                         'generic type parameter which has different name '\
                         f'such as `OtherNameT` for `{t}`.'
```

### Comparing `ts_type-0.2.9/ts_type.egg-info/PKG-INFO` & `ts_type-0.3.0/ts_type.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ts-type
-Version: 0.2.9
+Name: ts_type
+Version: 0.3.0
 Summary: ts_type generates typescript's type from python code
 Home-page: https://github.com/saryou/ts_type
 Author: Ryosuke Sasaki
 Author-email: saryou.ssk@gmail.com
 Project-URL: Bug Tracker, https://github.com/saryou/ts_type/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -129,16 +129,16 @@
 type RequestForApiB = Extract<Apis, {url: "/api/b"}>['request'];
 type ResponseForApiB = Extract<Apis, {url: "/api/b"}>['request'];
 ```
 
 
 ## Basic Usage
 
-1. add types to `TypeDefinitionGenerator`. (you can use `ts_type.generator`, which is an instance of the class)
-2. call `TypeDefinitionGenerator.generate`
+1. Add types to `TypeDefinitionGenerator` with `add` method. (You can use `ts_type.generator`, which is an instance of the class. `ts_type.gen_type` is a shortcut of `ts_type.generator.add`)
+2. Call `TypeDefinitionGenerator.generate`
 
 ```py3
 from dataclasses import dataclass
 from typing import Optional, List, Dict
 
 import ts_type as ts
 
@@ -164,33 +164,35 @@
 
 ```python3
 class Builder(ts.NodeBuilder):
     def handle_unknown_type(self, t: Any) -> ts.TypeNode:
         if isinstance(t, type):
             if issubclass(t, cl.Cleaned):
                 return self.define_cleaned(t)
+            if issubclass(t, cl.Undefined):
+                return ts.Undefined()
         return super().handle_unknown_type(t)
 
     def define_cleaned(self,
-                       t: Type[cl.Cleaned],
+                       t: type[cl.Cleaned],
                        exclude: set[str] = set()) -> ts.TypeNode:
         ret: ts.TypeNode = self.define_ref_node(t, lambda: ts.Object(
             attrs={
                 k: self.type_to_node(self.field_to_type(f))
                 for k, f in t._meta.fields.items()
             },
             omissible={k for k, f in t._meta.fields.items() if f.has_default}))
 
         if (exclude := exclude & set(t._meta.fields)):
             ret = ts.Omit(ret, ts.Union(
                 [self.literal_to_node(k) for k in sorted(exclude)]))
 
         return ret
 
-    def field_to_type(self, t: cl.Field) -> Type:
+    def field_to_type(self, t: cl.Field) -> type:
         if isinstance(t, cl.OptionalField):
             vt = self.field_to_type(t.field)
             return Union[None, cl.Undefined, vt]
         elif isinstance(t, cl.ListField):
             vt = self.field_to_type(t.value)
             return list[vt]
         elif isinstance(t, cl.SetField):
```

