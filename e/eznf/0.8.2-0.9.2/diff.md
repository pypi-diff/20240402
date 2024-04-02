# Comparing `tmp/eznf-0.8.2.tar.gz` & `tmp/eznf-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eznf-0.8.2.tar", last modified: Mon Nov  6 17:01:35 2023, max compression
+gzip compressed data, was "eznf-0.9.2.tar", last modified: Tue Nov  7 18:35:38 2023, max compression
```

## Comparing `eznf-0.8.2.tar` & `eznf-0.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bsuberca   (504) staff       (20)        0 2023-11-06 17:01:35.231498 eznf-0.8.2/
--rw-r--r--   0 bsuberca   (504) staff       (20)     1074 2023-10-16 01:09:11.000000 eznf-0.8.2/LICENSE
--rw-r--r--   0 bsuberca   (504) staff       (20)      940 2023-11-06 17:01:35.231323 eznf-0.8.2/PKG-INFO
--rw-r--r--   0 bsuberca   (504) staff       (20)      444 2023-10-16 00:48:10.000000 eznf-0.8.2/README.md
-drwxr-xr-x   0 bsuberca   (504) staff       (20)        0 2023-11-06 17:01:35.230069 eznf-0.8.2/eznf/
--rw-r--r--   0 bsuberca   (504) staff       (20)        0 2023-10-16 00:44:14.000000 eznf-0.8.2/eznf/__init__.py
--rw-r--r--   0 bsuberca   (504) staff       (20)    23414 2023-11-06 17:01:01.000000 eznf-0.8.2/eznf/modeler.py
-drwxr-xr-x   0 bsuberca   (504) staff       (20)        0 2023-11-06 17:01:35.230903 eznf-0.8.2/eznf.egg-info/
--rw-r--r--   0 bsuberca   (504) staff       (20)      940 2023-11-06 17:01:35.000000 eznf-0.8.2/eznf.egg-info/PKG-INFO
--rw-r--r--   0 bsuberca   (504) staff       (20)      208 2023-11-06 17:01:35.000000 eznf-0.8.2/eznf.egg-info/SOURCES.txt
--rw-r--r--   0 bsuberca   (504) staff       (20)        1 2023-11-06 17:01:35.000000 eznf-0.8.2/eznf.egg-info/dependency_links.txt
--rw-r--r--   0 bsuberca   (504) staff       (20)        5 2023-11-06 17:01:35.000000 eznf-0.8.2/eznf.egg-info/top_level.txt
--rw-r--r--   0 bsuberca   (504) staff       (20)      548 2023-11-06 17:01:25.000000 eznf-0.8.2/pyproject.toml
--rw-r--r--   0 bsuberca   (504) staff       (20)       38 2023-11-06 17:01:35.231537 eznf-0.8.2/setup.cfg
--rw-r--r--   0 bsuberca   (504) staff       (20)      358 2023-11-06 17:01:25.000000 eznf-0.8.2/setup.py
-drwxr-xr-x   0 bsuberca   (504) staff       (20)        0 2023-11-06 17:01:35.231024 eznf-0.8.2/tests/
--rw-r--r--   0 bsuberca   (504) staff       (20)      131 2023-10-16 00:48:32.000000 eznf-0.8.2/tests/test_modeler.py
+drwxr-xr-x   0 bsuberca   (504) staff       (20)        0 2023-11-07 18:35:38.723858 eznf-0.9.2/
+-rw-r--r--   0 bsuberca   (504) staff       (20)     1074 2023-10-16 01:09:11.000000 eznf-0.9.2/LICENSE
+-rw-r--r--   0 bsuberca   (504) staff       (20)      940 2023-11-07 18:35:38.723577 eznf-0.9.2/PKG-INFO
+-rw-r--r--   0 bsuberca   (504) staff       (20)      444 2023-10-16 00:48:10.000000 eznf-0.9.2/README.md
+drwxr-xr-x   0 bsuberca   (504) staff       (20)        0 2023-11-07 18:35:38.722405 eznf-0.9.2/eznf/
+-rw-r--r--   0 bsuberca   (504) staff       (20)        0 2023-10-16 00:44:14.000000 eznf-0.9.2/eznf/__init__.py
+-rw-r--r--   0 bsuberca   (504) staff       (20)    23433 2023-11-07 18:35:14.000000 eznf-0.9.2/eznf/modeler.py
+drwxr-xr-x   0 bsuberca   (504) staff       (20)        0 2023-11-07 18:35:38.723058 eznf-0.9.2/eznf.egg-info/
+-rw-r--r--   0 bsuberca   (504) staff       (20)      940 2023-11-07 18:35:38.000000 eznf-0.9.2/eznf.egg-info/PKG-INFO
+-rw-r--r--   0 bsuberca   (504) staff       (20)      208 2023-11-07 18:35:38.000000 eznf-0.9.2/eznf.egg-info/SOURCES.txt
+-rw-r--r--   0 bsuberca   (504) staff       (20)        1 2023-11-07 18:35:38.000000 eznf-0.9.2/eznf.egg-info/dependency_links.txt
+-rw-r--r--   0 bsuberca   (504) staff       (20)        5 2023-11-07 18:35:38.000000 eznf-0.9.2/eznf.egg-info/top_level.txt
+-rw-r--r--   0 bsuberca   (504) staff       (20)      548 2023-11-07 18:35:27.000000 eznf-0.9.2/pyproject.toml
+-rw-r--r--   0 bsuberca   (504) staff       (20)       38 2023-11-07 18:35:38.723919 eznf-0.9.2/setup.cfg
+-rw-r--r--   0 bsuberca   (504) staff       (20)      358 2023-11-07 18:35:27.000000 eznf-0.9.2/setup.py
+drwxr-xr-x   0 bsuberca   (504) staff       (20)        0 2023-11-07 18:35:38.723252 eznf-0.9.2/tests/
+-rw-r--r--   0 bsuberca   (504) staff       (20)      131 2023-10-16 00:48:32.000000 eznf-0.9.2/tests/test_modeler.py
```

### Comparing `eznf-0.8.2/LICENSE` & `eznf-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eznf-0.8.2/PKG-INFO` & `eznf-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eznf
-Version: 0.8.2
+Version: 0.9.2
 Summary: A prototype library to prototype SAT encodings
 Author: Bernardo Subercaseaux
 Author-email: Bernardo Subercaseaux <bernardosubercaseaux@gmail.com>
 Project-URL: Homepage, https://github.com/bsubercaseaux/eznf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eznf-0.8.2/eznf/modeler.py` & `eznf-0.9.2/eznf/modeler.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                 file.write("p cnf {} {}\n".format(len(self._varmap), len(clauses)))
                 for clause in clauses:
                     file.write(" ".join(map(str, clause)) + " 0\n")
     
     def serialize_decoder(self, filename) -> None:
         pass
            
-    def decode(self, sol_filename, output_builder) -> str:
+    def decode_from_sol(self, sol_filename, output_builder) -> str:
         lit_valuation = {}
         with open(sol_filename, 'r') as sol:
             for line in sol:
                 if line[0] == 'v':
                     tokens = line[:-1].split(' ') # skip newline
                     relevant_tokens = tokens[1:]
                     for token in relevant_tokens:
@@ -127,15 +127,15 @@
         for lit_name, (lit, _) in self._varmap.items():
             sem_valuation[lit_name] = lit_valuation[lit]
             
         # for sem_name, sem_var in self._semvars.items():
         #     sem_valuation[sem_name] = OrderIntervalValuation(sem_var, lit_valuation)
         return output_builder(sem_valuation)
         
-    def decode(self, output_builder) -> None:
+    def solve_and_decode(self, output_builder) -> None:
         lit_valuation = {}
         self.serialize("tmp")
         output, return_code = system_call(["cadical", f"tmp.cnf"])
         if return_code != 10:
             print(f"return code = {return_code}, UNSAT formula does not allow decoding.")
             return
```

### Comparing `eznf-0.8.2/eznf.egg-info/PKG-INFO` & `eznf-0.9.2/eznf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eznf
-Version: 0.8.2
+Version: 0.9.2
 Summary: A prototype library to prototype SAT encodings
 Author: Bernardo Subercaseaux
 Author-email: Bernardo Subercaseaux <bernardosubercaseaux@gmail.com>
 Project-URL: Homepage, https://github.com/bsubercaseaux/eznf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eznf-0.8.2/pyproject.toml` & `eznf-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eznf"
-version = "0.8.2"
+version = "0.9.2"
 authors = [
   { name="Bernardo Subercaseaux", email="bernardosubercaseaux@gmail.com" },
 ]
 description = "A prototype library to prototype SAT encodings"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

