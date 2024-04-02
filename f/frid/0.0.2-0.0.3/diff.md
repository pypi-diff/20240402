# Comparing `tmp/frid-0.0.2.tar.gz` & `tmp/frid-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frid-0.0.2.tar", last modified: Fri Mar 29 22:43:17 2024, max compression
+gzip compressed data, was "frid-0.0.3.tar", last modified: Tue Apr  2 02:20:18 2024, max compression
```

## Comparing `frid-0.0.2.tar` & `frid-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-03-29 22:43:17.152907 frid-0.0.2/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.2/LICENSE
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      603 2024-03-29 22:43:17.152907 frid-0.0.2/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)       74 2024-03-21 15:01:03.000000 frid-0.0.2/README.md
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-03-29 22:43:17.152907 frid-0.0.2/frid/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      474 2024-03-29 15:03:28.000000 frid-0.0.2/frid/__init__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    23981 2024-03-29 18:12:06.000000 frid-0.0.2/frid/__main__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3828 2024-03-25 13:54:20.000000 frid-0.0.2/frid/chrono.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    12841 2024-03-29 14:57:08.000000 frid-0.0.2/frid/dumper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2597 2024-03-27 14:11:35.000000 frid-0.0.2/frid/errors.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     5657 2024-03-26 04:05:50.000000 frid-0.0.2/frid/guards.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     4061 2024-03-29 18:07:49.000000 frid-0.0.2/frid/helper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    21302 2024-03-28 01:02:08.000000 frid-0.0.2/frid/loader.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-25 20:04:53.000000 frid-0.0.2/frid/pretty.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    10833 2024-03-27 21:55:04.000000 frid-0.0.2/frid/strops.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2082 2024-03-27 14:03:55.000000 frid-0.0.2/frid/typing.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11113 2024-03-28 15:30:47.000000 frid-0.0.2/frid/webapp.py
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-03-29 22:43:17.152907 frid-0.0.2/frid.egg-info/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      603 2024-03-29 22:43:17.000000 frid-0.0.2/frid.egg-info/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      328 2024-03-29 22:43:17.000000 frid-0.0.2/frid.egg-info/SOURCES.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-03-29 22:43:17.000000 frid-0.0.2/frid.egg-info/dependency_links.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-03-29 22:43:17.000000 frid-0.0.2/frid.egg-info/top_level.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-03-29 22:42:29.000000 frid-0.0.2/pyproject.toml
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-03-29 22:43:17.152907 frid-0.0.2/setup.cfg
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-02 02:20:18.445206 frid-0.0.3/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.3/LICENSE
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-02 02:20:18.445206 frid-0.0.3/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1235 2024-03-30 02:09:52.000000 frid-0.0.3/README.md
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-02 02:20:18.445206 frid-0.0.3/frid/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      347 2024-04-02 02:16:36.000000 frid-0.0.3/frid/__init__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    23981 2024-03-29 23:28:02.000000 frid-0.0.3/frid/__main__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3828 2024-03-29 23:28:02.000000 frid-0.0.3/frid/chrono.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    12841 2024-03-29 23:28:02.000000 frid-0.0.3/frid/dumper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2597 2024-03-29 23:28:02.000000 frid-0.0.3/frid/errors.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     6504 2024-04-01 22:27:27.000000 frid-0.0.3/frid/guards.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     4061 2024-03-29 23:28:02.000000 frid-0.0.3/frid/helper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    21302 2024-04-01 15:36:11.000000 frid-0.0.3/frid/loader.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-29 23:28:02.000000 frid-0.0.3/frid/pretty.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    10833 2024-03-29 23:28:02.000000 frid-0.0.3/frid/strops.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2082 2024-04-01 15:53:05.000000 frid-0.0.3/frid/typing.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11113 2024-03-29 23:28:02.000000 frid-0.0.3/frid/webapp.py
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-02 02:20:18.445206 frid-0.0.3/frid.egg-info/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-02 02:20:18.000000 frid-0.0.3/frid.egg-info/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      328 2024-04-02 02:20:18.000000 frid-0.0.3/frid.egg-info/SOURCES.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-04-02 02:20:18.000000 frid-0.0.3/frid.egg-info/dependency_links.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-04-02 02:20:18.000000 frid-0.0.3/frid.egg-info/top_level.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-04-02 02:18:11.000000 frid-0.0.3/pyproject.toml
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-04-02 02:20:18.445206 frid-0.0.3/setup.cfg
```

### Comparing `frid-0.0.2/LICENSE` & `frid-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `frid-0.0.2/frid/__main__.py` & `frid-0.0.3/frid/__main__.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.2/frid/chrono.py` & `frid-0.0.3/frid/chrono.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.2/frid/dumper.py` & `frid-0.0.3/frid/dumper.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.2/frid/errors.py` & `frid-0.0.3/frid/errors.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.2/frid/guards.py` & `frid-0.0.3/frid/guards.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,34 @@
 from collections.abc import Iterable, Mapping, Sequence
 from typing import Literal, TypeGuard, TypeVar, overload
 
-from .typing import BlobTypes
+from .typing import BlobTypes, StrKeyMap
 
 K = TypeVar('K')
 V = TypeVar('V')
 
+@overload
+def as_type(dtype: type[V], data, /, allow_none: Literal[False]=False) -> V: ...
+@overload
+def as_type(dtype: type[V], data, /, allow_none: Literal[True]) -> V|None: ...
+def as_type(dtype: type[V], data, /, allow_none: bool=False) -> V|None:
+    if data is None and allow_none:
+        return None
+    if not isinstance(data, dtype):
+        raise ValueError(f"Expecting type {dtype}, got {type(data).__name__}")
+    return data
+@overload
+def get_as_type(dtype: type[V], map: StrKeyMap, key: str,
+                /, allow_none: Literal[False]=False) -> V: ...
+@overload
+def get_as_type(dtype: type[V], map: StrKeyMap, key: str,
+                /, allow_none: Literal[True]) -> V|None: ...
+def get_as_type(dtype: type[V], map: StrKeyMap, key: str, /, allow_none: bool=False) -> V|None:
+    return as_type(dtype, map.get(key))
+
 def is_text_list_like(data, /) -> TypeGuard[Sequence[str]]:
     """Type guard for a sequence of string elements."""
     if not isinstance(data, Sequence) or isinstance(data, str|BlobTypes):
         return False
     return all(isinstance(x, str) for x in data)
 
 def is_blob_list_like(data, /) -> TypeGuard[Sequence[BlobTypes]]:
```

### Comparing `frid-0.0.2/frid/helper.py` & `frid-0.0.3/frid/helper.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.2/frid/loader.py` & `frid-0.0.3/frid/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,20 +373,20 @@
             if c != sep[0]:
                 self.error(index, f"Expect '{sep[0]}' after the value for '{name}': {path=}")
             index = self.skip_fixed_size(index, path, 1)
         return (index, args, kwas)
 
     def construct_mixin(
             self, index: int, path: str, start: int,
-            /, name: str,  args: list[FridValue], kwas: dict[str,FridValue]
+            /, name: str,  args: list[FridValue], kwds: dict[str,FridValue]
     ) -> tuple[int,FridValue]:
         mixin = self.frid_mixin.get(name)
         if mixin is None:
             self.error(start, f"Cannot find constructor called {name}")
-        return (index, mixin.frid_from(name, *args, **kwas))
+        return (index, mixin.frid_from(name, *args, **kwds))
 
     def scan_frid_value(self, index: int, path: str, /, empty: Any='') -> tuple[int,FridValue]:
         """Load the text representation."""
         index = self.skip_whitespace(index, path)
         if index >= self.length:
             return (index, empty)
         c = self.peek_fixed_size(index, path, 1)
```

### Comparing `frid-0.0.2/frid/pretty.py` & `frid-0.0.3/frid/pretty.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.2/frid/strops.py` & `frid-0.0.3/frid/strops.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.2/frid/typing.py` & `frid-0.0.3/frid/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     """
     @classmethod
     def frid_keys(cls) -> Iterable[str]:
         """The list of keys that the class provides; the default containing class name only."""
         return [cls.__name__]
 
     @classmethod
-    def frid_from(cls, name: str, *args: 'FridValue', **kwas: 'FridValue') -> 'FridMixin':
+    def frid_from(cls, name: str, *args: 'FridValue', **kwds: 'FridValue') -> 'FridMixin':
         """Construct an instance with given name and arguments."""
         assert name in cls.frid_keys()
-        return cls(*args, **kwas)
+        return cls(*args, **kwds)
 
     @abstractmethod
     def frid_repr(self) -> tuple[str,Sequence['FridValue'],Mapping[str,'FridValue']]:
         """Converts an instance to a triplet of name, a list of positional values,
         and a dict of keyword values.
         """
         raise NotImplementedError
```

### Comparing `frid-0.0.2/frid/webapp.py` & `frid-0.0.3/frid/webapp.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.2/pyproject.toml` & `frid-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frid"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Hanhua Feng", email="han.hua.feng@askherefirst.com" },
 ]
 description = "Flexibly Represented Interactive Data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

