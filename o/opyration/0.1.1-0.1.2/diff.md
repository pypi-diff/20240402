# Comparing `tmp/opyration-0.1.1.tar.gz` & `tmp/opyration-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opyration-0.1.1.tar", max compression
+gzip compressed data, was "opyration-0.1.2.tar", max compression
```

## Comparing `opyration-0.1.1.tar` & `opyration-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1167 2023-11-15 21:53:11.099792 opyration-0.1.1/README.md
--rw-r--r--   0        0        0       70 2023-11-15 22:00:29.355063 opyration-0.1.1/opyration/__init__.py
--rw-r--r--   0        0        0       55 2023-11-15 22:08:29.950495 opyration-0.1.1/opyration/interfaces.py
--rw-r--r--   0        0        0     8783 2024-03-11 08:53:20.797315 opyration-0.1.1/opyration/operation.py
--rw-r--r--   0        0        0     1479 2024-03-11 08:56:37.634431 opyration-0.1.1/opyration/results.py
--rw-r--r--   0        0        0      371 2024-01-21 20:31:10.054961 opyration-0.1.1/opyration/symbols.py
--rw-r--r--   0        0        0      675 2024-02-14 11:13:28.461968 opyration-0.1.1/opyration/transaction.py
--rw-r--r--   0        0        0      402 2024-03-11 08:56:52.806176 opyration-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 opyration-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1167 2023-11-15 21:53:11.099792 opyration-0.1.2/README.md
+-rw-r--r--   0        0        0       70 2023-11-15 22:00:29.355063 opyration-0.1.2/opyration/__init__.py
+-rw-r--r--   0        0        0       55 2023-11-15 22:08:29.950495 opyration-0.1.2/opyration/interfaces.py
+-rw-r--r--   0        0        0     8803 2024-03-24 11:25:09.077314 opyration-0.1.2/opyration/operation.py
+-rw-r--r--   0        0        0     1507 2024-03-21 21:25:44.190950 opyration-0.1.2/opyration/results.py
+-rw-r--r--   0        0        0      371 2024-01-21 20:31:10.054961 opyration-0.1.2/opyration/symbols.py
+-rw-r--r--   0        0        0      675 2024-02-14 11:13:28.461968 opyration-0.1.2/opyration/transaction.py
+-rw-r--r--   0        0        0      402 2024-04-02 19:54:41.209784 opyration-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 opyration-0.1.2/PKG-INFO
```

### Comparing `opyration-0.1.1/README.md` & `opyration-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `opyration-0.1.1/opyration/operation.py` & `opyration-0.1.2/opyration/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,15 @@
         return self.__join('LEFT JOIN', **conditions)
     
     def right_join(self, **conditions):
         return self.__join('RIGHT JOIN', **conditions)
 
     def limit(self, limit: int):
         self.__sql = f'{self.__sql} LIMIT {limit}'
+        return self
 
     def or_where(self, **pairs):
         start = len(self.__vals)
         for field_op, value in pairs.items():
             placeholder = f'${start + 1}'
             try: field, op = field_op.split('__')
             except: field, op = field_op, 'eq'
```

### Comparing `opyration-0.1.1/opyration/results.py` & `opyration-0.1.2/opyration/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,13 +50,14 @@
         except IndexError: return None
         else: return Lookup(dict(datum))
 
     def reset(self, index: int = 0):
         self.__count = index
 
     def row(self, n: int):
-        try: return Lookup(dict(self.__queue[n]))
+        if n < 1: n = 1
+        try: return Lookup(dict(self.__queue[n - 1]))
         except: return None
 
     def rows(self, n: int):
         if n > len(self.__queue): n = len(self.__queue)
         return [self.pop() for _ in range(n)]
```

### Comparing `opyration-0.1.1/opyration/transaction.py` & `opyration-0.1.2/opyration/transaction.py`

 * *Files identical despite different names*

### Comparing `opyration-0.1.1/PKG-INFO` & `opyration-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opyration
-Version: 0.1.1
+Version: 0.1.2
 Summary: Execute SQL Statements as a series of pythonic functions.
 License: MIT
 Author: Raymond Ortserga
 Author-email: ortserga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

