# Comparing `tmp/forfloatrange-1.2.0.tar.gz` & `tmp/forfloatrange-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forfloatrange-1.2.0.tar", max compression
+gzip compressed data, was "forfloatrange-1.2.1.tar", max compression
```

## Comparing `forfloatrange-1.2.0.tar` & `forfloatrange-1.2.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1750 2024-02-21 01:45:21.694177 forfloatrange-1.2.0/README.md
--rw-r--r--   0        0        0      786 2024-02-21 09:54:21.605044 forfloatrange-1.2.0/forfloatrange.py
--rw-r--r--   0        0        0      294 2024-02-21 09:54:21.609651 forfloatrange-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2365 1970-01-01 00:00:00.000000 forfloatrange-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1704 2024-02-27 11:20:54.338671 forfloatrange-1.2.1/README.md
+-rw-r--r--   0        0        0      710 2024-04-02 11:33:08.533275 forfloatrange-1.2.1/forfloatrange.py
+-rw-r--r--   0        0        0      294 2024-04-02 11:33:24.733047 forfloatrange-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 forfloatrange-1.2.1/PKG-INFO
```

### Comparing `forfloatrange-1.2.0/README.md` & `forfloatrange-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # English
 
 `forfloatrange` is a Python library that provides a function called `ffrange` for generating a sequence of floating-point numbers within a specified range with a given step. The function verifies that the step is not zero to prevent errors and utilizes a generator expression for efficient handling of large value ranges.
 
-
-The speed of ffrange 1.1.0 is taken as 100%.
 ### Installation
 
 You can install the library using pip:
 
 ```bash
 pip install forfloatrange
 ```
```

### Comparing `forfloatrange-1.2.0/forfloatrange.py` & `forfloatrange-1.2.1/forfloatrange.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     step_val = Decimal(str(args[2])) if length > 2 else Decimal(1)
 
     if step_val == 0:
         raise ValueError("Error: Step cannot be 0.")
 
     results = []
 
-    def calculate_range(start, end, step):
-        current_val = start
-        while (step > 0 and current_val < end+step) or (step < 0 and current_val > end+step):
-            results.append(current_val)
-            current_val += step
+    current_val = min_val
+    while (step_val > 0 and current_val < max_val+step_val) or (step_val < 0 and current_val > max_val+step_val):
+        results.append(current_val)
+        current_val += step_val
 
-    calculate_range(min_val, max_val, step_val)
 
-    return results
+    return results
```

### Comparing `forfloatrange-1.2.0/PKG-INFO` & `forfloatrange-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forfloatrange
-Version: 1.2.0
+Version: 1.2.1
 Summary: Range with float
 Author: Nova D Andrew
 Author-email: andrew.d.nova@icloud.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -15,16 +15,14 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # English
 
 `forfloatrange` is a Python library that provides a function called `ffrange` for generating a sequence of floating-point numbers within a specified range with a given step. The function verifies that the step is not zero to prevent errors and utilizes a generator expression for efficient handling of large value ranges.
 
-
-The speed of ffrange 1.1.0 is taken as 100%.
 ### Installation
 
 You can install the library using pip:
 
 ```bash
 pip install forfloatrange
 ```
```

