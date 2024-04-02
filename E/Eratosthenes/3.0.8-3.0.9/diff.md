# Comparing `tmp/Eratosthenes-3.0.8.tar.gz` & `tmp/Eratosthenes-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Eratosthenes-3.0.8.tar", last modified: Mon Apr  1 15:33:19 2024, max compression
+gzip compressed data, was "Eratosthenes-3.0.9.tar", last modified: Tue Apr  2 11:58:40 2024, max compression
```

## Comparing `Eratosthenes-3.0.8.tar` & `Eratosthenes-3.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 15:33:19.440287 Eratosthenes-3.0.8/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 15:33:19.440287 Eratosthenes-3.0.8/Eratosthenes.egg-info/
--rw-r--r--   0 iamu      (1000) iamu      (1000)     1550 2024-04-01 15:33:19.000000 Eratosthenes-3.0.8/Eratosthenes.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      305 2024-04-01 15:33:19.000000 Eratosthenes-3.0.8/Eratosthenes.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2024-04-01 15:33:19.000000 Eratosthenes-3.0.8/Eratosthenes.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       13 2024-04-01 15:33:19.000000 Eratosthenes-3.0.8/Eratosthenes.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2024-03-26 16:40:08.000000 Eratosthenes-3.0.8/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       19 2024-03-26 17:27:20.000000 Eratosthenes-3.0.8/MANIFEST.in
--rw-r--r--   0 iamu      (1000) iamu      (1000)     1550 2024-04-01 15:33:19.440287 Eratosthenes-3.0.8/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      814 2024-03-29 23:46:05.000000 Eratosthenes-3.0.8/README.md
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2024-04-01 15:33:19.440287 Eratosthenes-3.0.8/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1318 2024-04-01 15:32:22.000000 Eratosthenes-3.0.8/setup.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 15:33:19.440287 Eratosthenes-3.0.8/src/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2895 2024-04-01 14:02:53.000000 Eratosthenes-3.0.8/src/dispatchqueue.cpp
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 15:33:19.440287 Eratosthenes-3.0.8/src/include/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      767 2024-03-26 15:47:52.000000 Eratosthenes-3.0.8/src/include/config.h
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1941 2024-03-30 14:18:47.000000 Eratosthenes-3.0.8/src/include/dispatchqueue.hpp
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3460 2024-04-01 15:30:54.000000 Eratosthenes-3.0.8/src/include/prime_generator.hpp
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    15188 2024-04-01 15:29:56.000000 Eratosthenes-3.0.8/src/prime_gen.cpp
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-02 11:58:40.260204 Eratosthenes-3.0.9/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-02 11:58:40.260204 Eratosthenes-3.0.9/Eratosthenes.egg-info/
+-rw-r--r--   0 iamu      (1000) iamu      (1000)     1550 2024-04-02 11:58:40.000000 Eratosthenes-3.0.9/Eratosthenes.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      305 2024-04-02 11:58:40.000000 Eratosthenes-3.0.9/Eratosthenes.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2024-04-02 11:58:40.000000 Eratosthenes-3.0.9/Eratosthenes.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       13 2024-04-02 11:58:40.000000 Eratosthenes-3.0.9/Eratosthenes.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2024-03-26 16:40:08.000000 Eratosthenes-3.0.9/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       19 2024-03-26 17:27:20.000000 Eratosthenes-3.0.9/MANIFEST.in
+-rw-r--r--   0 iamu      (1000) iamu      (1000)     1550 2024-04-02 11:58:40.260204 Eratosthenes-3.0.9/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      814 2024-03-29 23:46:05.000000 Eratosthenes-3.0.9/README.md
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2024-04-02 11:58:40.260204 Eratosthenes-3.0.9/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1318 2024-04-02 11:57:45.000000 Eratosthenes-3.0.9/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-02 11:58:40.256204 Eratosthenes-3.0.9/src/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2895 2024-04-01 14:02:53.000000 Eratosthenes-3.0.9/src/dispatchqueue.cpp
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-02 11:58:40.260204 Eratosthenes-3.0.9/src/include/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      767 2024-03-26 15:47:52.000000 Eratosthenes-3.0.9/src/include/config.h
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1941 2024-03-30 14:18:47.000000 Eratosthenes-3.0.9/src/include/dispatchqueue.hpp
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3460 2024-04-01 15:30:54.000000 Eratosthenes-3.0.9/src/include/prime_generator.hpp
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    15186 2024-04-02 11:56:11.000000 Eratosthenes-3.0.9/src/prime_gen.cpp
```

### Comparing `Eratosthenes-3.0.8/Eratosthenes.egg-info/PKG-INFO` & `Eratosthenes-3.0.9/Eratosthenes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eratosthenes
-Version: 3.0.8
+Version: 3.0.9
 Summary: Fast prime generation for Python based on Sieve of Eratosthenes and Trial Division
 Home-page: https://github.com/vm6502q/Eratosthenes
 Author: Dan Strano
 Author-email: dan@unitary.fund
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `Eratosthenes-3.0.8/LICENSE` & `Eratosthenes-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.8/PKG-INFO` & `Eratosthenes-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eratosthenes
-Version: 3.0.8
+Version: 3.0.9
 Summary: Fast prime generation for Python based on Sieve of Eratosthenes and Trial Division
 Home-page: https://github.com/vm6502q/Eratosthenes
 Author: Dan Strano
 Author-email: dan@unitary.fund
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `Eratosthenes-3.0.8/README.md` & `Eratosthenes-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.8/setup.py` & `Eratosthenes-3.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         language='c++',
         extra_compile_args = cpp_args,
     ),
 ]
 
 setup(
     name='Eratosthenes',
-    version='3.0.8',
+    version='3.0.9',
     author='Dan Strano',
     author_email='dan@unitary.fund',
     description='Fast prime generation for Python based on Sieve of Eratosthenes and Trial Division',
     long_description=README,
     long_description_content_type='text/markdown',
     url="https://github.com/vm6502q/Eratosthenes",
     license="MIT",
```

### Comparing `Eratosthenes-3.0.8/src/dispatchqueue.cpp` & `Eratosthenes-3.0.9/src/dispatchqueue.cpp`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.8/src/include/config.h` & `Eratosthenes-3.0.9/src/include/config.h`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.8/src/include/dispatchqueue.hpp` & `Eratosthenes-3.0.9/src/include/dispatchqueue.hpp`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.8/src/include/prime_generator.hpp` & `Eratosthenes-3.0.9/src/include/prime_generator.hpp`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.8/src/prime_gen.cpp` & `Eratosthenes-3.0.9/src/prime_gen.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,15 @@
     // We save half our necessary bytes by
     // removing multiples of 2.
     // The simple sieve removes multiples of 2, 3, and 5.
     // limit = 2048 KB = 2097152 B,
     // limit_segmented = limit * 2
     // limit_simple = ((((limit * 2) * 3) / 2) * 5) / 4
     constexpr size_t limit = 6291456ULL;
-    constexpr size_t limit_simple = 31457281ULL;
+    constexpr size_t limit_simple = 7864321ULL;
 
     if (!(n & 1U)) {
         --n;
     }
     if ((n % 3U) == 0) {
         n -= 2U;
     }
@@ -368,15 +368,15 @@
     // We save half our necessary bytes by
     // removing multiples of 2.
     // The simple sieve removes multiples of 2, 3, and 5.
     // limit = 2048 KB = 2097152 B,
     // limit_segmented = ((limit * 2) * 3) / 2
     // limit_simple = ((((limit * 2) * 3) / 2) * 5) / 4
     constexpr size_t limit = 6291456ULL;
-    constexpr size_t limit_simple = 31457281ULL;
+    constexpr size_t limit_simple = 7864321ULL;
 
     if (!(n & 1U)) {
         --n;
     }
     if ((n % 3U) == 0) {
         n -= 2U;
     }
```

