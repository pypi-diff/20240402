# Comparing `tmp/fast_html-1.0.8.tar.gz` & `tmp/fast_html-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_html-1.0.8.tar", max compression
+gzip compressed data, was "fast_html-1.0.9.tar", max compression
```

## Comparing `fast_html-1.0.8.tar` & `fast_html-1.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7636 2023-05-08 16:52:22.164958 fast_html-1.0.8/LICENSE
--rw-r--r--   0        0        0     4516 2024-04-01 15:35:40.352251 fast_html-1.0.8/README.md
--rw-r--r--   0        0        0    13549 2024-04-01 15:35:30.688085 fast_html-1.0.8/fast_html/__init__.py
--rw-r--r--   0        0        0        0 2024-01-01 20:10:19.913231 fast_html-1.0.8/fast_html/py.typed
--rw-r--r--   0        0        0     2577 2024-01-24 14:05:55.939255 fast_html-1.0.8/fast_html/utils.py
--rw-r--r--   0        0        0      608 2024-04-01 15:39:06.427501 fast_html-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 fast_html-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     7636 2023-05-08 16:52:22.164958 fast_html-1.0.9/LICENSE
+-rw-r--r--   0        0        0     4516 2024-04-01 15:35:40.352251 fast_html-1.0.9/README.md
+-rw-r--r--   0        0        0    13495 2024-04-02 05:47:39.251704 fast_html-1.0.9/fast_html/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-01 20:10:19.913231 fast_html-1.0.9/fast_html/py.typed
+-rw-r--r--   0        0        0     2577 2024-01-24 14:05:55.939255 fast_html-1.0.9/fast_html/utils.py
+-rw-r--r--   0        0        0      608 2024-04-02 05:48:48.827003 fast_html-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 fast_html-1.0.9/PKG-INFO
```

### Comparing `fast_html-1.0.8/LICENSE` & `fast_html-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_html-1.0.8/README.md` & `fast_html-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fast_html-1.0.8/fast_html/__init__.py` & `fast_html-1.0.9/fast_html/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,21 +53,21 @@
         for k, v in kwargs.items()
     )
     yield f"<{tag_name}{attrs}>{_cr if indent else ''}"
 
 
 def _inner(inner: Inner, with_cr = False):
     """unfold the inner iterators"""
-    if isinstance(inner, Iterable) and not isinstance(inner, str):
-        for i in inner:
-            yield from _inner(i)
-    else:  # inner is a str
+    if isinstance(inner, str):
         yield ((f'{_tab}{inner}{_cr}' if indent and with_cr else
                 f'{_tab}{inner}' if indent else
                 inner))
+    else:
+        for i in inner:
+            yield from _inner(i)
 
 
 def tag(tag_name: str, inner: Optional[Inner] = None, **kwargs) -> Tag:
     """returns a generator of strings, to be rendered as a HTML tag of type `name`
 
     Args:
         tag_name : name of the tag
```

### Comparing `fast_html-1.0.8/fast_html/utils.py` & `fast_html-1.0.9/fast_html/utils.py`

 * *Files identical despite different names*

### Comparing `fast_html-1.0.8/pyproject.toml` & `fast_html-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast_html"
-version = "1.0.8"
+version = "1.0.9"
 description = "A fast, minimalist HTML generator"
 authors = ["Pierre <pierre.carbonnelle@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/pcarbonn/fast_html"
 license = "LGPL-3.0-or-later"
 keywords = ["HTML", "HTMX"]
 classifiers = [
```

### Comparing `fast_html-1.0.8/PKG-INFO` & `fast_html-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-html
-Version: 1.0.8
+Version: 1.0.9
 Summary: A fast, minimalist HTML generator
 Home-page: https://github.com/pcarbonn/fast_html
 License: LGPL-3.0-or-later
 Keywords: HTML,HTMX
 Author: Pierre
 Author-email: pierre.carbonnelle@gmail.com
 Requires-Python: >=3.7,<4.0
```

