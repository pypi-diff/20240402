# Comparing `tmp/FSRS-Optimizer-4.9.0.tar.gz` & `tmp/FSRS-Optimizer-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FSRS-Optimizer-4.9.0.tar", last modified: Thu Aug 10 03:03:03 2023, max compression
+gzip compressed data, was "FSRS-Optimizer-4.9.1.tar", last modified: Sun Aug 13 08:36:12 2023, max compression
```

## Comparing `FSRS-Optimizer-4.9.0.tar` & `FSRS-Optimizer-4.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 03:03:03.654940 FSRS-Optimizer-4.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-10 03:02:49.000000 FSRS-Optimizer-4.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-10 03:03:03.654940 FSRS-Optimizer-4.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-08-10 03:02:49.000000 FSRS-Optimizer-4.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-10 03:02:49.000000 FSRS-Optimizer-4.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-10 03:03:03.654940 FSRS-Optimizer-4.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-10 03:02:49.000000 FSRS-Optimizer-4.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 03:03:03.646940 FSRS-Optimizer-4.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 03:03:03.650940 FSRS-Optimizer-4.9.0/src/FSRS_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-10 03:03:03.000000 FSRS-Optimizer-4.9.0/src/FSRS_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-10 03:03:03.000000 FSRS-Optimizer-4.9.0/src/FSRS_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-10 03:03:03.000000 FSRS-Optimizer-4.9.0/src/FSRS_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-10 03:03:03.000000 FSRS-Optimizer-4.9.0/src/FSRS_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-10 03:03:03.000000 FSRS-Optimizer-4.9.0/src/FSRS_Optimizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 03:03:03.654940 FSRS-Optimizer-4.9.0/src/fsrs_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-10 03:02:49.000000 FSRS-Optimizer-4.9.0/src/fsrs_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-08-10 03:02:49.000000 FSRS-Optimizer-4.9.0/src/fsrs_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53593 2023-08-10 03:02:49.000000 FSRS-Optimizer-4.9.0/src/fsrs_optimizer/fsrs_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 08:36:12.176931 FSRS-Optimizer-4.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-13 08:35:59.000000 FSRS-Optimizer-4.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-13 08:36:12.176931 FSRS-Optimizer-4.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-08-13 08:35:59.000000 FSRS-Optimizer-4.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-13 08:35:59.000000 FSRS-Optimizer-4.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-13 08:36:12.176931 FSRS-Optimizer-4.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-13 08:35:59.000000 FSRS-Optimizer-4.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 08:36:12.176931 FSRS-Optimizer-4.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 08:36:12.176931 FSRS-Optimizer-4.9.1/src/FSRS_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-13 08:36:12.000000 FSRS-Optimizer-4.9.1/src/FSRS_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-13 08:36:12.000000 FSRS-Optimizer-4.9.1/src/FSRS_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-13 08:36:12.000000 FSRS-Optimizer-4.9.1/src/FSRS_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-13 08:36:12.000000 FSRS-Optimizer-4.9.1/src/FSRS_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-13 08:36:12.000000 FSRS-Optimizer-4.9.1/src/FSRS_Optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 08:36:12.176931 FSRS-Optimizer-4.9.1/src/fsrs_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-13 08:35:59.000000 FSRS-Optimizer-4.9.1/src/fsrs_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-08-13 08:35:59.000000 FSRS-Optimizer-4.9.1/src/fsrs_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53593 2023-08-13 08:35:59.000000 FSRS-Optimizer-4.9.1/src/fsrs_optimizer/fsrs_optimizer.py
```

### Comparing `FSRS-Optimizer-4.9.0/LICENSE` & `FSRS-Optimizer-4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.9.0/PKG-INFO` & `FSRS-Optimizer-4.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.9.0
+Version: 4.9.1
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.9.0/README.md` & `FSRS-Optimizer-4.9.1/README.md`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.9.0/src/FSRS_Optimizer.egg-info/PKG-INFO` & `FSRS-Optimizer-4.9.1/src/FSRS_Optimizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.9.0
+Version: 4.9.1
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.9.0/src/fsrs_optimizer/__main__.py` & `FSRS-Optimizer-4.9.1/src/fsrs_optimizer/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,9 +170,18 @@
                     print(e)
                     print(f"Failed to process {file_path}")
                 finally:
                     plt.close('all')
                     os.chdir(curdir)
                     continue
         else:
-            process(filename)
+            try:
+                print(f"Processing {filename}")
+                process(filename)
+            except Exception as e:
+                print(e)
+                print(f"Failed to process {filename}")
+            finally:
+                plt.close('all')
+                os.chdir(curdir)
+                continue
```

### Comparing `FSRS-Optimizer-4.9.0/src/fsrs_optimizer/fsrs_optimizer.py` & `FSRS-Optimizer-4.9.1/src/fsrs_optimizer/fsrs_optimizer.py`

 * *Files identical despite different names*

