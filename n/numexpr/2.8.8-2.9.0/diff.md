# Comparing `tmp/numexpr-2.8.8.tar.gz` & `tmp/numexpr-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numexpr-2.8.8.tar", last modified: Mon Dec 11 13:06:59 2023, max compression
+gzip compressed data, was "numexpr-2.9.0.tar", last modified: Fri Jan 26 12:52:10 2024, max compression
```

## Comparing `numexpr-2.8.8.tar` & `numexpr-2.9.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-12-11 13:06:59.466662 numexpr-2.8.8/
--rw-rw-rw-   0        0        0     2218 2023-12-11 12:56:26.000000 numexpr-2.8.8/ANNOUNCE.rst
--rw-rw-rw-   0        0        0      942 2023-12-11 12:56:26.000000 numexpr-2.8.8/AUTHORS.txt
--rw-rw-rw-   0        0        0     1214 2023-12-11 12:56:26.000000 numexpr-2.8.8/LICENSE.txt
--rw-rw-rw-   0        0        0      240 2023-12-11 12:56:26.000000 numexpr-2.8.8/MANIFEST.in
--rw-rw-rw-   0        0        0     8104 2023-12-11 13:06:59.466662 numexpr-2.8.8/PKG-INFO
--rw-rw-rw-   0        0        0     7060 2023-12-11 12:56:26.000000 numexpr-2.8.8/README.rst
--rw-rw-rw-   0        0        0    30008 2023-12-11 12:56:26.000000 numexpr-2.8.8/RELEASE_NOTES.rst
-drwxrwxrwx   0        0        0        0 2023-12-11 13:06:59.451043 numexpr-2.8.8/bench/
--rw-rw-rw-   0        0        0     5665 2023-12-11 12:56:26.000000 numexpr-2.8.8/bench/boolean_timing.py
--rw-rw-rw-   0        0        0      929 2023-12-11 12:56:26.000000 numexpr-2.8.8/bench/issue-36.py
--rw-rw-rw-   0        0        0      202 2023-12-11 12:56:26.000000 numexpr-2.8.8/bench/issue-47.py
--rw-rw-rw-   0        0        0     2801 2023-12-11 12:56:26.000000 numexpr-2.8.8/bench/multidim.py
--rw-rw-rw-   0        0        0     1960 2023-12-11 12:56:26.000000 numexpr-2.8.8/bench/poly.py
--rw-rw-rw-   0        0        0     4119 2023-12-11 12:56:26.000000 numexpr-2.8.8/bench/timing.py
--rw-rw-rw-   0        0        0     1489 2023-12-11 12:56:26.000000 numexpr-2.8.8/bench/unaligned-simple.py
--rw-rw-rw-   0        0        0     1679 2023-12-11 12:56:26.000000 numexpr-2.8.8/bench/varying-expr.py
--rw-rw-rw-   0        0        0     6040 2023-12-11 12:56:26.000000 numexpr-2.8.8/bench/vml_timing.py
--rw-rw-rw-   0        0        0     1526 2023-12-11 12:56:26.000000 numexpr-2.8.8/bench/vml_timing2.py
--rw-rw-rw-   0        0        0      324 2023-12-11 12:56:26.000000 numexpr-2.8.8/bench/vml_timing3.py
-drwxrwxrwx   0        0        0        0 2023-12-11 13:06:59.466662 numexpr-2.8.8/numexpr/
--rw-rw-rw-   0        0        0     2346 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/__init__.py
--rw-rw-rw-   0        0        0    10092 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/complex_functions.hpp
--rw-rw-rw-   0        0        0    26023 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/cpuinfo.py
--rw-rw-rw-   0        0        0    16661 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/expressions.py
--rw-rw-rw-   0        0        0     5863 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/functions.hpp
--rw-rw-rw-   0        0        0    21811 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/interp_body.cpp
--rw-rw-rw-   0        0        0    49781 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/interpreter.cpp
--rw-rw-rw-   0        0        0     2708 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/interpreter.hpp
--rw-rw-rw-   0        0        0     2052 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/missing_posix_functions.hpp
--rw-rw-rw-   0        0        0    16870 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/module.cpp
--rw-rw-rw-   0        0        0     2261 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/module.hpp
--rw-rw-rw-   0        0        0     3620 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/msvc_function_stubs.hpp
--rw-rw-rw-   0        0        0    35788 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/necompiler.py
--rw-rw-rw-   0        0        0     1380 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/numexpr_config.hpp
--rw-rw-rw-   0        0        0    15041 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/numexpr_object.cpp
--rw-rw-rw-   0        0        0     1069 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/numexpr_object.hpp
--rw-rw-rw-   0        0        0     7489 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/opcodes.hpp
--rw-rw-rw-   0        0        0    14863 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/str-two-way.hpp
-drwxrwxrwx   0        0        0        0 2023-12-11 13:06:59.466662 numexpr-2.8.8/numexpr/tests/
--rw-rw-rw-   0        0        0      461 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/tests/__init__.py
--rw-rw-rw-   0        0        0    51290 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/tests/test_numexpr.py
--rw-rw-rw-   0        0        0     7693 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/utils.py
--rw-rw-rw-   0        0        0      119 2023-12-11 13:06:59.000000 numexpr-2.8.8/numexpr/version.py
-drwxrwxrwx   0        0        0        0 2023-12-11 13:06:59.466662 numexpr-2.8.8/numexpr/win32/
--rw-rw-rw-   0        0        0     7303 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/win32/pthread.c
--rw-rw-rw-   0        0        0     4155 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/win32/pthread.h
--rw-rw-rw-   0        0        0     7565 2023-12-11 12:56:26.000000 numexpr-2.8.8/numexpr/win32/stdint.h
-drwxrwxrwx   0        0        0        0 2023-12-11 13:06:59.466662 numexpr-2.8.8/numexpr.egg-info/
--rw-rw-rw-   0        0        0     8104 2023-12-11 13:06:59.000000 numexpr-2.8.8/numexpr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1173 2023-12-11 13:06:59.000000 numexpr-2.8.8/numexpr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-11 13:06:59.000000 numexpr-2.8.8/numexpr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-12-11 12:57:41.000000 numexpr-2.8.8/numexpr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-12-11 13:06:59.000000 numexpr-2.8.8/numexpr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-12-11 13:06:59.000000 numexpr-2.8.8/numexpr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2023-12-11 12:56:26.000000 numexpr-2.8.8/pyproject.toml
--rw-rw-rw-   0        0        0       17 2023-12-11 12:56:26.000000 numexpr-2.8.8/requirements.txt
--rw-rw-rw-   0        0        0      974 2023-12-11 13:06:59.466662 numexpr-2.8.8/setup.cfg
--rw-rw-rw-   0        0        0     3239 2023-12-11 12:56:26.000000 numexpr-2.8.8/setup.py
--rw-rw-rw-   0        0        0      700 2023-12-11 12:56:26.000000 numexpr-2.8.8/site.cfg.example
+drwxrwxrwx   0        0        0        0 2024-01-26 12:52:10.854595 numexpr-2.9.0/
+-rw-rw-rw-   0        0        0     2261 2024-01-26 12:44:10.000000 numexpr-2.9.0/ANNOUNCE.rst
+-rw-rw-rw-   0        0        0      942 2024-01-26 12:44:10.000000 numexpr-2.9.0/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1214 2024-01-26 12:44:10.000000 numexpr-2.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      240 2024-01-26 12:44:10.000000 numexpr-2.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8098 2024-01-26 12:52:10.854595 numexpr-2.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7060 2024-01-26 12:44:10.000000 numexpr-2.9.0/README.rst
+-rw-rw-rw-   0        0        0    30444 2024-01-26 12:44:10.000000 numexpr-2.9.0/RELEASE_NOTES.rst
+drwxrwxrwx   0        0        0        0 2024-01-26 12:52:10.838930 numexpr-2.9.0/bench/
+-rw-rw-rw-   0        0        0     5665 2024-01-26 12:44:10.000000 numexpr-2.9.0/bench/boolean_timing.py
+-rw-rw-rw-   0        0        0      929 2024-01-26 12:44:10.000000 numexpr-2.9.0/bench/issue-36.py
+-rw-rw-rw-   0        0        0      202 2024-01-26 12:44:10.000000 numexpr-2.9.0/bench/issue-47.py
+-rw-rw-rw-   0        0        0     2801 2024-01-26 12:44:10.000000 numexpr-2.9.0/bench/multidim.py
+-rw-rw-rw-   0        0        0     1960 2024-01-26 12:44:10.000000 numexpr-2.9.0/bench/poly.py
+-rw-rw-rw-   0        0        0     4119 2024-01-26 12:44:10.000000 numexpr-2.9.0/bench/timing.py
+-rw-rw-rw-   0        0        0     1489 2024-01-26 12:44:10.000000 numexpr-2.9.0/bench/unaligned-simple.py
+-rw-rw-rw-   0        0        0     1679 2024-01-26 12:44:10.000000 numexpr-2.9.0/bench/varying-expr.py
+-rw-rw-rw-   0        0        0     6040 2024-01-26 12:44:10.000000 numexpr-2.9.0/bench/vml_timing.py
+-rw-rw-rw-   0        0        0     1526 2024-01-26 12:44:10.000000 numexpr-2.9.0/bench/vml_timing2.py
+-rw-rw-rw-   0        0        0      324 2024-01-26 12:44:10.000000 numexpr-2.9.0/bench/vml_timing3.py
+drwxrwxrwx   0        0        0        0 2024-01-26 12:52:10.838930 numexpr-2.9.0/numexpr/
+-rw-rw-rw-   0        0        0     2346 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/__init__.py
+-rw-rw-rw-   0        0        0    10092 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/complex_functions.hpp
+-rw-rw-rw-   0        0        0    26023 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/cpuinfo.py
+-rw-rw-rw-   0        0        0    16661 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/expressions.py
+-rw-rw-rw-   0        0        0     5863 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/functions.hpp
+-rw-rw-rw-   0        0        0    21811 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/interp_body.cpp
+-rw-rw-rw-   0        0        0    49806 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/interpreter.cpp
+-rw-rw-rw-   0        0        0     2708 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/interpreter.hpp
+-rw-rw-rw-   0        0        0     2052 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/missing_posix_functions.hpp
+-rw-rw-rw-   0        0        0    16870 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/module.cpp
+-rw-rw-rw-   0        0        0     2261 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/module.hpp
+-rw-rw-rw-   0        0        0     3620 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/msvc_function_stubs.hpp
+-rw-rw-rw-   0        0        0    35852 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/necompiler.py
+-rw-rw-rw-   0        0        0     1380 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/numexpr_config.hpp
+-rw-rw-rw-   0        0        0    15041 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/numexpr_object.cpp
+-rw-rw-rw-   0        0        0     1069 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/numexpr_object.hpp
+-rw-rw-rw-   0        0        0     7489 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/opcodes.hpp
+-rw-rw-rw-   0        0        0    14863 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/str-two-way.hpp
+drwxrwxrwx   0        0        0        0 2024-01-26 12:52:10.854595 numexpr-2.9.0/numexpr/tests/
+-rw-rw-rw-   0        0        0      461 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/tests/__init__.py
+-rw-rw-rw-   0        0        0    51610 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/tests/test_numexpr.py
+-rw-rw-rw-   0        0        0     7693 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/utils.py
+-rw-rw-rw-   0        0        0      119 2024-01-26 12:52:10.000000 numexpr-2.9.0/numexpr/version.py
+drwxrwxrwx   0        0        0        0 2024-01-26 12:52:10.854595 numexpr-2.9.0/numexpr/win32/
+-rw-rw-rw-   0        0        0     7303 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/win32/pthread.c
+-rw-rw-rw-   0        0        0     4155 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/win32/pthread.h
+-rw-rw-rw-   0        0        0     7565 2024-01-26 12:44:10.000000 numexpr-2.9.0/numexpr/win32/stdint.h
+drwxrwxrwx   0        0        0        0 2024-01-26 12:52:10.854595 numexpr-2.9.0/numexpr.egg-info/
+-rw-rw-rw-   0        0        0     8098 2024-01-26 12:52:10.000000 numexpr-2.9.0/numexpr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1173 2024-01-26 12:52:10.000000 numexpr-2.9.0/numexpr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-26 12:52:10.000000 numexpr-2.9.0/numexpr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-26 12:45:02.000000 numexpr-2.9.0/numexpr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2024-01-26 12:52:10.000000 numexpr-2.9.0/numexpr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-01-26 12:52:10.000000 numexpr-2.9.0/numexpr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2024-01-26 12:44:10.000000 numexpr-2.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       17 2024-01-26 12:44:10.000000 numexpr-2.9.0/requirements.txt
+-rw-rw-rw-   0        0        0      968 2024-01-26 12:52:10.854595 numexpr-2.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     3239 2024-01-26 12:44:10.000000 numexpr-2.9.0/setup.py
+-rw-rw-rw-   0        0        0      700 2024-01-26 12:44:10.000000 numexpr-2.9.0/site.cfg.example
```

### Comparing `numexpr-2.8.8/ANNOUNCE.rst` & `numexpr-2.9.0/ANNOUNCE.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 ========================
-Announcing NumExpr 2.8.8
+Announcing NumExpr 2.9.0
 ========================
 
 Hi everyone,
 
-NumExpr 2.8.8 is a release to deal mainly with issues appearing with
-upcoming `NumPy` 2.0.  Also, some small fixes (support for simple complex
-expressions like `ne.evaluate('1.5j')`) and improvements are included.
+NumExpr 2.9.0 is a release offering support for latest versions of PyPy.
+The full test suite should pass now, at least for the Python 3.10 version.
+Thanks to @27rabbitlt for most of the work and @mgorny and @mattip for
+providing help and additional fixes.
 
 Project documentation is available at:
 
 http://numexpr.readthedocs.io/
 
 Changes from 2.8.7 to 2.8.8
 ---------------------------
```

### Comparing `numexpr-2.8.8/AUTHORS.txt` & `numexpr-2.9.0/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/LICENSE.txt` & `numexpr-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/PKG-INFO` & `numexpr-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: numexpr
-Version: 2.8.8
+Version: 2.9.0
 Summary: Fast numerical expression evaluator for NumPy
 Home-page: https://github.com/pydata/numexpr
 Author: David M. Cooke, Francesc Alted, and others
-Maintainer: Robert A. McLeod
-Maintainer-email: robbmcleod@gmail.com
+Maintainer: Francesc Alted
+Maintainer-email: faltet@gmail.com
 License: MIT
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `numexpr-2.8.8/README.rst` & `numexpr-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/RELEASE_NOTES.rst` & `numexpr-2.9.0/RELEASE_NOTES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 ====================================
-Release notes for NumExpr 2.8 series
+Release notes for NumExpr 2.9 series
 ====================================
 
+Changes from 2.8.8 to 2.9.0
+---------------------------
+
+* Support for PyPy (see PRs #467 and #740).  The full test suite
+  should pass now, at least for the 3.10 version.  Thanks to
+  @27rabbitlt for most of the work and @mgorny and @mattip for
+  providing help and additional fixes.  Fixes #463.
+
+* Fixed more sanitizer issues (see PR #469).  Thanks to @27rabbitlt.
+
+* Modernized the test suite to avoid some warnings.
+
+
 Changes from 2.8.7 to 2.8.8
 ---------------------------
 
 * Fix re_evaluate not taking global_dict as argument. Thanks to Teng Liu
   (@27rabbitlt).
 
 * Fix parsing of simple complex numbers.  Now, `ne.evaluate('1.5j')` works.
```

### Comparing `numexpr-2.8.8/bench/boolean_timing.py` & `numexpr-2.9.0/bench/boolean_timing.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/bench/issue-36.py` & `numexpr-2.9.0/bench/issue-36.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/bench/multidim.py` & `numexpr-2.9.0/bench/multidim.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/bench/poly.py` & `numexpr-2.9.0/bench/poly.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/bench/timing.py` & `numexpr-2.9.0/bench/timing.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/bench/unaligned-simple.py` & `numexpr-2.9.0/bench/unaligned-simple.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/bench/varying-expr.py` & `numexpr-2.9.0/bench/varying-expr.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/bench/vml_timing.py` & `numexpr-2.9.0/bench/vml_timing.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/bench/vml_timing2.py` & `numexpr-2.9.0/bench/vml_timing2.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/__init__.py` & `numexpr-2.9.0/numexpr/__init__.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/complex_functions.hpp` & `numexpr-2.9.0/numexpr/complex_functions.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/cpuinfo.py` & `numexpr-2.9.0/numexpr/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/expressions.py` & `numexpr-2.9.0/numexpr/expressions.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/functions.hpp` & `numexpr-2.9.0/numexpr/functions.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/interp_body.cpp` & `numexpr-2.9.0/numexpr/interp_body.cpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/interpreter.cpp` & `numexpr-2.9.0/numexpr/interpreter.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1025,15 +1025,15 @@
         return PyErr_Format(PyExc_ValueError,
                             "too many inputs");
     }
 
     memset(operands, 0, sizeof(operands));
     memset(dtypes, 0, sizeof(dtypes));
 
-    if (kwds) {
+    if (kwds && PyDict_Size(kwds) > 0) {
         tmp = PyDict_GetItemString(kwds, "casting"); // borrowed ref
         if (tmp != NULL && !PyArray_CastingConverter(tmp, &casting)) {
             return NULL;
         }
         tmp = PyDict_GetItemString(kwds, "order"); // borrowed ref
         if (tmp != NULL && !PyArray_OrderConverter(tmp, &order)) {
             return NULL;
```

### Comparing `numexpr-2.8.8/numexpr/interpreter.hpp` & `numexpr-2.9.0/numexpr/interpreter.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/missing_posix_functions.hpp` & `numexpr-2.9.0/numexpr/missing_posix_functions.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/module.cpp` & `numexpr-2.9.0/numexpr/module.cpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/module.hpp` & `numexpr-2.9.0/numexpr/module.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/msvc_function_stubs.hpp` & `numexpr-2.9.0/numexpr/msvc_function_stubs.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/necompiler.py` & `numexpr-2.9.0/numexpr/necompiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,16 @@
     # sanitize the string for obvious attack vectors that NumExpr cannot 
     # parse into its homebrew AST. This is to protect the call to `eval` below.
     # We forbid `;`, `:`. `[` and `__`, and attribute access via '.'.
     # We cannot ban `.real` or `.imag` however...
     # We also cannot ban `.\d*j`, where `\d*` is some digits (or none), e.g. 1.5j, 1.j
     if sanitize:
         no_whitespace = re.sub(r'\s+', '', s)
-        if _blacklist_re.search(no_whitespace) is not None:
+        skip_quotes = re.sub(r'(\'[^\']*\')', '', no_whitespace)
+        if _blacklist_re.search(skip_quotes) is not None:
             raise ValueError(f'Expression {s} has forbidden control characters.')
     
     old_ctx = expressions._context.get_current_context()
     try:
         expressions._context.set_new_context(context)
         # first compile to a code object to determine the names
         if context.get('truediv', False):
```

### Comparing `numexpr-2.8.8/numexpr/numexpr_config.hpp` & `numexpr-2.9.0/numexpr/numexpr_config.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/numexpr_object.cpp` & `numexpr-2.9.0/numexpr/numexpr_object.cpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/numexpr_object.hpp` & `numexpr-2.9.0/numexpr/numexpr_object.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/opcodes.hpp` & `numexpr-2.9.0/numexpr/opcodes.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/str-two-way.hpp` & `numexpr-2.9.0/numexpr/str-two-way.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/tests/test_numexpr.py` & `numexpr-2.9.0/numexpr/tests/test_numexpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import platform
 import warnings
 from contextlib import contextmanager
 import subprocess
 
 import numpy as np
 from numpy import (
-    array, arange, empty, zeros, int32, int64, uint16, complex_, float64, rec,
+    array, arange, empty, zeros, int32, int64, uint16, cdouble, float64, rec,
     copy, ones_like, where, all as alltrue, linspace,
     sum, prod, sqrt, fmod, floor, ceil,
     sin, cos, tan, arcsin, arccos, arctan, arctan2,
     sinh, cosh, tanh, arcsinh, arccosh, arctanh,
     log, log1p, log10, exp, expm1, conj)
 import numpy
 from numpy.testing import (assert_equal, assert_array_equal,
@@ -292,36 +292,37 @@
         assert_equal(res, [True, True, True])
 
     def test_str_contains_long_needle(self):
         a = b'1' + b'a' * 40
         b = b'a' * 40
         res = evaluate('contains(a, b)')
         assert_equal(res, True)
-        
+
     def test_where_scalar_bool(self):
         a = True
         b = array([1, 2])
         c = array([3, 4])
         res = evaluate('where(a, b, c)')
         assert_array_equal(res, b)
         a = False
         res = evaluate('where(a, b, c)')
         assert_array_equal(res, c)
 
-    
+    @unittest.skipIf(hasattr(sys, "pypy_version_info"),
+                     "PyPy does not have sys.getrefcount()")
     def test_refcount(self):
         # Regression test for issue #310
         a = array([1])
         assert sys.getrefcount(a) == 2
         evaluate('1')
         assert sys.getrefcount(a) == 2
 
     def test_locals_clears_globals(self):
         # Check for issue #313, whereby clearing f_locals also clear f_globals
-        # if in the top-frame. This cannot be done inside `unittest` as it is always 
+        # if in the top-frame. This cannot be done inside `unittest` as it is always
         # executing code in a child frame.
         script = r';'.join([
                 r"import numexpr as ne",
                 r"a=10",
                 r"ne.evaluate('1')",
                 r"a += 1",
                 r"ne.evaluate('2', local_dict={})",
@@ -329,15 +330,15 @@
                 r"ne.evaluate('3', global_dict={})",
                 r"a += 1",
                 r"ne.evaluate('4', local_dict={}, global_dict={})",
                 r"a += 1",
             ])
         # Raises CalledProcessError on a non-normal exit
         check = subprocess.check_call([sys.executable, '-c', script])
-        # Ideally this test should also be done against ipython but it's not 
+        # Ideally this test should also be done against ipython but it's not
         # a requirement.
 
 
 
 class test_numexpr2(test_numexpr):
     """Testing with 2 threads"""
     nthreads = 2
@@ -439,15 +440,15 @@
         b = arange(1e6) * 0.1
         x = (a + 2 * b) / (1 + a + 4 * b * b)
         y = evaluate("(a + 2*b) / (1 + a + 4*b*b)")
         assert_array_almost_equal(x, y)
 
     def test_complex_expr(self):
         def complex(a, b):
-            c = zeros(a.shape, dtype=complex_)
+            c = zeros(a.shape, dtype=cdouble)
             c.real = a
             c.imag = b
             return c
 
         a = arange(1e4)
         b = arange(1e4) ** 1e-5
         z = a + 1j * b
@@ -516,15 +517,15 @@
                 evaluate('__builtins__')
             except ValueError:
                 pass
             else:
                 self.fail()
 
             # Forbid colon for lambda funcs
-            try: 
+            try:
                 evaluate('lambda x: x')
             except ValueError:
                 pass
             else:
                 self.fail()
 
             # Forbid indexing
@@ -572,15 +573,23 @@
             evaluate('2.+a')
 
             # pass .real and .imag
             c = 2.5 + 1.5j
             evaluate('c.real')
             evaluate('c.imag')
 
-        
+            # pass imaginary unit j
+            evaluate('1.5j')
+            evaluate('3.j')
+
+            # pass forbidden characters within quotes
+            x = np.array(['a', 'b'], dtype=bytes)
+            evaluate("x == 'b:'")
+
+
     def test_no_sanitize(self):
         try: # Errors on compile() after eval()
             evaluate('import os;', sanitize=False)
         except SyntaxError:
             pass
         else:
             self.fail()
@@ -592,15 +601,15 @@
                 pass
             else:
                 self.fail()
 
     def test_disassemble(self):
         assert_equal(disassemble(NumExpr(
             "where(m, a, -1)", [('m', bool), ('a', float)])),
-            [[b'where_fbff', b'r0', b'r1[m]', b'r2[a]', b'c3[-1.0]'], 
+            [[b'where_fbff', b'r0', b'r1[m]', b'r2[a]', b'c3[-1.0]'],
              [b'noop', None, None, None]])
 
     def test_constant_deduplication(self):
         assert_equal(NumExpr("(a + 1)*(a - 1)", [('a', np.int32)]).constants, (1,))
 
     def test_nan_constant(self):
         assert_equal(str(ConstantNode(float("nan")).value), 'nan')
@@ -611,45 +620,45 @@
         assert_equal(NumExpr(expr, [('a', double), ('b', double)]).constants, (float("nan"),))
 
 
     def test_f32_constant(self):
         assert_equal(ConstantNode(numpy.float32(1)).astKind, "float")
         assert_equal(ConstantNode(numpy.float32("nan")).astKind, "float")
         assert_equal(ConstantNode(numpy.float32(3)).value.dtype, numpy.dtype("float32"))
-        assert_array_equal(NumExpr(ConstantNode(numpy.float32(1))).run(), 
+        assert_array_equal(NumExpr(ConstantNode(numpy.float32(1))).run(),
                            numpy.array(1, dtype="float32"))
 
     def test_unaligned_singleton(self):
-        # Test for issue #397 whether singletons outputs assigned to consts must be 
+        # Test for issue #397 whether singletons outputs assigned to consts must be
         # aligned or not.
         a = np.empty(5, dtype=np.uint8)[1:].view(np.int32)
         evaluate('3', out=a)
         assert_equal(a, 3)
 
     def test_negative_mod(self):
-        # Test for issue #413, modulus of negative integers. C modulus is 
+        # Test for issue #413, modulus of negative integers. C modulus is
         # actually remainder op, and hence different from Python modulus.
         a = np.array([-500, -135, 0, 0, 135, 500], dtype=np.int32)
         n = np.array([-360, -360, -360, 360, 360, 360], dtype=np.int32)
         out_i = evaluate('a % n')
         assert_equal(out_i, np.mod(a, n))
 
         b = a.astype(np.int64)
         m = n.astype(np.int64)
         out_l = evaluate('b % m')
         assert_equal(out_l, np.mod(b, m))
 
     def test_negative_power_scalar(self):
         # Test for issue #428, where the power is negative and the base is an
         # integer. This was running afoul in the precomputation in `expressions.py:pow_op()`
-        base = np.array([-2, -1, 0, 1, 2, 3], dtype=np.int32)
+        base = np.array([-2, -1, 1, 2, 3], dtype=np.int32)
         out_i = evaluate('base ** -1.0')
         assert_equal(out_i, np.power(base, -1.0))
 
-        base = np.array([-2, -1, 0, 1, 2, 3], dtype=np.int64)
+        base = np.array([-2, -1, 1, 2, 3], dtype=np.int64)
         out_l = evaluate('base ** -1.0')
         assert_equal(out_l, np.power(base, -1.0))
 
 
     def test_ex_uses_vml(self):
         vml_funcs = [ "sin", "cos", "tan", "arcsin", "arccos", "arctan",
                       "sinh", "cosh", "tanh", "arcsinh", "arccosh", "arctanh",
@@ -1107,27 +1116,27 @@
             os.environ[key] = old
         else:
             del os.environ[key]
 
 # Test cases for the threading configuration
 class test_threading_config(TestCase):
     def test_max_threads_unset(self):
-        # Has to be done in a subprocess as `importlib.reload` doesn't let us 
+        # Has to be done in a subprocess as `importlib.reload` doesn't let us
         # re-initialize the threadpool
         script = '\n'.join([
                 "import os",
                 "if 'NUMEXPR_MAX_THREADS' in os.environ: os.environ.pop('NUMEXPR_MAX_THREADS')",
                 "if 'OMP_NUM_THREADS' in os.environ: os.environ.pop('OMP_NUM_THREADS')",
                 "import numexpr",
                 "assert(numexpr.nthreads <= 8)",
                 "exit(0)"])
         subprocess.check_call([sys.executable, '-c', script])
 
     def test_max_threads_set(self):
-        # Has to be done in a subprocess as `importlib.reload` doesn't let us 
+        # Has to be done in a subprocess as `importlib.reload` doesn't let us
         # re-initialize the threadpool
         script = '\n'.join([
                 "import os",
                 "os.environ['NUMEXPR_MAX_THREADS'] = '4'",
                 "import numexpr",
                 "assert(numexpr.MAX_THREADS == 4)",
                 "exit(0)"])
@@ -1234,15 +1243,15 @@
     print('-=' * 38)
     print('Numexpr version:   %s' % numexpr.__version__)
     print('NumPy version:     %s' % np.__version__)
     print('Python version:    %s' % sys.version)
     (sysname, nodename, release, os_version, machine, processor) = platform.uname()
     print('Platform:          %s-%s-%s' % (sys.platform, machine, os_version))
     try:
-        # cpuinfo doesn't work on OSX well it seems, so protect these outputs 
+        # cpuinfo doesn't work on OSX well it seems, so protect these outputs
         # with a try block
         cpu_info = cpu.info[0]
         print('CPU vendor:        %s' % cpu_info.get('VendorIdentifier', ''))
         print('CPU model:         %s' % cpu_info.get('ProcessorNameString', ''))
         print('CPU clock speed:   %s MHz' % cpu_info.get('~MHz',''))
     except KeyError:
         pass
```

### Comparing `numexpr-2.8.8/numexpr/utils.py` & `numexpr-2.9.0/numexpr/utils.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/win32/pthread.c` & `numexpr-2.9.0/numexpr/win32/pthread.c`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/win32/pthread.h` & `numexpr-2.9.0/numexpr/win32/pthread.h`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr/win32/stdint.h` & `numexpr-2.9.0/numexpr/win32/stdint.h`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/numexpr.egg-info/PKG-INFO` & `numexpr-2.9.0/numexpr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: numexpr
-Version: 2.8.8
+Version: 2.9.0
 Summary: Fast numerical expression evaluator for NumPy
 Home-page: https://github.com/pydata/numexpr
 Author: David M. Cooke, Francesc Alted, and others
-Maintainer: Robert A. McLeod
-Maintainer-email: robbmcleod@gmail.com
+Maintainer: Francesc Alted
+Maintainer-email: faltet@gmail.com
 License: MIT
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `numexpr-2.8.8/numexpr.egg-info/SOURCES.txt` & `numexpr-2.9.0/numexpr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/setup.cfg` & `numexpr-2.9.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 756d 6578 7072 0d0a 7665 7273   = numexpr..vers
-00000020: 696f 6e20 3d20 322e 382e 380d 0a64 6573  ion = 2.8.8..des
+00000020: 696f 6e20 3d20 322e 392e 300d 0a64 6573  ion = 2.9.0..des
 00000030: 6372 6970 7469 6f6e 203d 2046 6173 7420  cription = Fast 
 00000040: 6e75 6d65 7269 6361 6c20 6578 7072 6573  numerical expres
 00000050: 7369 6f6e 2065 7661 6c75 6174 6f72 2066  sion evaluator f
 00000060: 6f72 204e 756d 5079 0d0a 6175 7468 6f72  or NumPy..author
 00000070: 203d 2044 6176 6964 204d 2e20 436f 6f6b   = David M. Cook
 00000080: 652c 2046 7261 6e63 6573 6320 416c 7465  e, Francesc Alte
 00000090: 642c 2061 6e64 206f 7468 6572 730d 0a6d  d, and others..m
-000000a0: 6169 6e74 6169 6e65 7220 3d20 526f 6265  aintainer = Robe
-000000b0: 7274 2041 2e20 4d63 4c65 6f64 0d0a 6d61  rt A. McLeod..ma
-000000c0: 696e 7461 696e 6572 5f65 6d61 696c 203d  intainer_email =
-000000d0: 2072 6f62 626d 636c 656f 6440 676d 6169   robbmcleod@gmai
-000000e0: 6c2e 636f 6d0d 0a75 726c 203d 2068 7474  l.com..url = htt
-000000f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000100: 7079 6461 7461 2f6e 756d 6578 7072 0d0a  pydata/numexpr..
-00000110: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000120: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-00000130: 7273 740d 0a6c 6f6e 675f 6465 7363 7269  rst..long_descri
-00000140: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
-00000150: 7065 203d 2074 6578 742f 782d 7273 740d  pe = text/x-rst.
-00000160: 0a6c 6963 656e 7365 203d 204d 4954 0d0a  .license = MIT..
-00000170: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-00000180: 0944 6576 656c 6f70 6d65 6e74 2053 7461  .Development Sta
-00000190: 7475 7320 3a3a 2036 202d 204d 6174 7572  tus :: 6 - Matur
-000001a0: 650d 0a09 496e 7465 6e64 6564 2041 7564  e...Intended Aud
-000001b0: 6965 6e63 6520 3a3a 2046 696e 616e 6369  ience :: Financi
-000001c0: 616c 2061 6e64 2049 6e73 7572 616e 6365  al and Insurance
-000001d0: 2049 6e64 7573 7472 790d 0a09 496e 7465   Industry...Inte
-000001e0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-000001f0: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
-00000200: 680d 0a09 4c69 6365 6e73 6520 3a3a 204f  h...License :: O
-00000210: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-00000220: 4954 204c 6963 656e 7365 0d0a 0950 726f  IT License...Pro
-00000230: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000240: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000250: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000260: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000270: 6e20 3a3a 2033 2e39 0d0a 0950 726f 6772  n :: 3.9...Progr
-00000280: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000290: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-000002a0: 300d 0a09 5072 6f67 7261 6d6d 696e 6720  0...Programming 
-000002b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002c0: 6f6e 203a 3a20 332e 3131 0d0a 0950 726f  on :: 3.11...Pro
-000002d0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002e0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002f0: 2e31 320d 0a09 4f70 6572 6174 696e 6720  .12...Operating 
-00000300: 5379 7374 656d 203a 3a20 4d69 6372 6f73  System :: Micros
-00000310: 6f66 7420 3a3a 2057 696e 646f 7773 0d0a  oft :: Windows..
-00000320: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-00000330: 6d20 3a3a 2050 4f53 4958 0d0a 094f 7065  m :: POSIX...Ope
-00000340: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000350: 204d 6163 4f53 0d0a 0d0a 5b6f 7074 696f   MacOS....[optio
-00000360: 6e73 5d0d 0a7a 6970 5f73 6166 6520 3d20  ns]..zip_safe = 
-00000370: 4661 6c73 650d 0a70 6163 6b61 6765 7320  False..packages 
-00000380: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
-00000390: 7265 7175 6972 6573 203d 203e 3d33 2e39  requires = >=3.9
-000003a0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000003b0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-000003c0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+000000a0: 6169 6e74 6169 6e65 7220 3d20 4672 616e  aintainer = Fran
+000000b0: 6365 7363 2041 6c74 6564 0d0a 6d61 696e  cesc Alted..main
+000000c0: 7461 696e 6572 5f65 6d61 696c 203d 2066  tainer_email = f
+000000d0: 616c 7465 7440 676d 6169 6c2e 636f 6d0d  altet@gmail.com.
+000000e0: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
+000000f0: 6974 6875 622e 636f 6d2f 7079 6461 7461  ithub.com/pydata
+00000100: 2f6e 756d 6578 7072 0d0a 6c6f 6e67 5f64  /numexpr..long_d
+00000110: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+00000120: 653a 2052 4541 444d 452e 7273 740d 0a6c  e: README.rst..l
+00000130: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
+00000140: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
+00000150: 6578 742f 782d 7273 740d 0a6c 6963 656e  ext/x-rst..licen
+00000160: 7365 203d 204d 4954 0d0a 636c 6173 7369  se = MIT..classi
+00000170: 6669 6572 7320 3d20 0d0a 0944 6576 656c  fiers = ...Devel
+00000180: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+00000190: 2036 202d 204d 6174 7572 650d 0a09 496e   6 - Mature...In
+000001a0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+000001b0: 3a3a 2046 696e 616e 6369 616c 2061 6e64  :: Financial and
+000001c0: 2049 6e73 7572 616e 6365 2049 6e64 7573   Insurance Indus
+000001d0: 7472 790d 0a09 496e 7465 6e64 6564 2041  try...Intended A
+000001e0: 7564 6965 6e63 6520 3a3a 2053 6369 656e  udience :: Scien
+000001f0: 6365 2f52 6573 6561 7263 680d 0a09 4c69  ce/Research...Li
+00000200: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000210: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+00000220: 656e 7365 0d0a 0950 726f 6772 616d 6d69  ense...Programmi
+00000230: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000240: 7974 686f 6e20 3a3a 2033 0d0a 0950 726f  ython :: 3...Pro
+00000250: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000260: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000270: 2e39 0d0a 0950 726f 6772 616d 6d69 6e67  .9...Programming
+00000280: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000290: 686f 6e20 3a3a 2033 2e31 300d 0a09 5072  hon :: 3.10...Pr
+000002a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000002b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000002c0: 332e 3131 0d0a 0950 726f 6772 616d 6d69  3.11...Programmi
+000002d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002e0: 7974 686f 6e20 3a3a 2033 2e31 320d 0a09  ython :: 3.12...
+000002f0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000300: 203a 3a20 4d69 6372 6f73 6f66 7420 3a3a   :: Microsoft ::
+00000310: 2057 696e 646f 7773 0d0a 094f 7065 7261   Windows...Opera
+00000320: 7469 6e67 2053 7973 7465 6d20 3a3a 2050  ting System :: P
+00000330: 4f53 4958 0d0a 094f 7065 7261 7469 6e67  OSIX...Operating
+00000340: 2053 7973 7465 6d20 3a3a 204d 6163 4f53   System :: MacOS
+00000350: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a7a  ....[options]..z
+00000360: 6970 5f73 6166 6520 3d20 4661 6c73 650d  ip_safe = False.
+00000370: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+00000380: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
+00000390: 6573 203d 203e 3d33 2e39 0d0a 0d0a 5b65  es = >=3.9....[e
+000003a0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+000003b0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+000003c0: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `numexpr-2.8.8/setup.py` & `numexpr-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.8/site.cfg.example` & `numexpr-2.9.0/site.cfg.example`

 * *Files identical despite different names*

