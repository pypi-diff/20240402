# Comparing `tmp/example_package_samreynoldsmath-0.1.16.tar.gz` & `tmp/example_package_samreynoldsmath-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example_package_samreynoldsmath-0.1.16.tar", max compression
+gzip compressed data, was "example_package_samreynoldsmath-0.2.1.tar", max compression
```

## Comparing `example_package_samreynoldsmath-0.1.16.tar` & `example_package_samreynoldsmath-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-03-19 23:49:11.896510 example_package_samreynoldsmath-0.1.16/LICENSE
--rw-r--r--   0        0        0      287 2024-03-21 00:06:32.407808 example_package_samreynoldsmath-0.1.16/README.md
--rw-r--r--   0        0        0      309 2024-03-21 00:06:32.407808 example_package_samreynoldsmath-0.1.16/example_package_samreynoldsmath/__init__.py
--rw-r--r--   0        0        0     1171 2024-03-25 23:12:28.907938 example_package_samreynoldsmath-0.1.16/example_package_samreynoldsmath/solver.py
--rw-r--r--   0        0        0      993 2024-03-26 00:49:32.856613 example_package_samreynoldsmath-0.1.16/pyproject.toml
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 example_package_samreynoldsmath-0.1.16/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-19 23:49:11.896510 example_package_samreynoldsmath-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1390 2024-03-26 01:45:46.133496 example_package_samreynoldsmath-0.2.1/README.md
+-rw-r--r--   0        0        0      388 2024-04-01 23:55:35.585652 example_package_samreynoldsmath-0.2.1/example_package_samreynoldsmath/__init__.py
+-rw-r--r--   0        0        0      687 2024-04-01 23:55:35.585652 example_package_samreynoldsmath-0.2.1/example_package_samreynoldsmath/jacobi.py
+-rw-r--r--   0        0        0     1157 2024-04-01 23:55:35.585652 example_package_samreynoldsmath-0.2.1/example_package_samreynoldsmath/solver.py
+-rw-r--r--   0        0        0     1046 2024-04-01 23:55:35.585652 example_package_samreynoldsmath-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1919 1970-01-01 00:00:00.000000 example_package_samreynoldsmath-0.2.1/PKG-INFO
```

### Comparing `example_package_samreynoldsmath-0.1.16/LICENSE` & `example_package_samreynoldsmath-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `example_package_samreynoldsmath-0.1.16/example_package_samreynoldsmath/solver.py` & `example_package_samreynoldsmath-0.2.1/example_package_samreynoldsmath/solver.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 This module contains the Solver class for solving Ax=b, and was mostly written
 Copilot. Good job, Copilot!
 """
 
 import numpy as np
 
+from .jacobi import jacobi_preconditioned_solve
+
 
 class Solver:
     """
     Solver class for solving Ax=b.
     """
 
     n: int
@@ -42,10 +44,8 @@
         """
         return np.linalg.solve(self.A, self.b)
 
     def jacobi_preconditioned_solve(self):
         """
         Solve Ax=b using Jacobi preconditioning.
         """
-        D = np.diag(self.A)
-        D_inv = np.diag(1 / D)
-        return np.linalg.solve(D_inv @ self.A, D_inv @ self.b)
+        return jacobi_preconditioned_solve(self.A, self.b)
```

### Comparing `example_package_samreynoldsmath-0.1.16/pyproject.toml` & `example_package_samreynoldsmath-0.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "example_package_samreynoldsmath"
-version = "0.1.16"
+version = "0.2.1"
 authors = ["Sam Reynolds <sreyn@proton.me>"]
-description = "A small example package with a linear solver"
+description = "A simple demo of how to structure, use, and publish a Python package."
 readme = "README.md"
 license = "MIT"
 packages = [{include = "example_package_samreynoldsmath"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 numpy = "^1.26.4"
@@ -34,10 +34,10 @@
 [tool.pytest.ini_options]
 filterwarnings = ["error"]
 
 [tool.pylint."messages control"]
 max-line-length = 80
 disable = [
   "fixme", # reenable to find TODO comments
-  "invalid-name", # use good-names
 ]
-good-names = ["A",]
+good-names = ["A", "B", "C", "D"]
+good-names-rgx = ["A_.*", "B_.*", "C_.*", "D_.*"]
```

