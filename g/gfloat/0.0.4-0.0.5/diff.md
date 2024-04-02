# Comparing `tmp/gfloat-0.0.4.tar.gz` & `tmp/gfloat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfloat-0.0.4.tar", last modified: Fri Mar 22 15:18:53 2024, max compression
+gzip compressed data, was "gfloat-0.0.5.tar", last modified: Tue Apr  2 14:34:02 2024, max compression
```

## Comparing `gfloat-0.0.4.tar` & `gfloat-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-03-22 15:18:53.090849 gfloat-0.0.4/
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-03-22 15:18:53.090849 gfloat-0.0.4/.github/
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-03-22 15:18:53.090849 gfloat-0.0.4/.github/workflows/
--rw-r--r--   0 awf       (1000) awf       (1000)      667 2024-03-21 17:30:20.000000 gfloat-0.0.4/.github/workflows/ci.yaml
--rw-r--r--   0 awf       (1000) awf       (1000)     3099 2024-02-15 18:32:26.000000 gfloat-0.0.4/.gitignore
--rw-r--r--   0 awf       (1000) awf       (1000)      301 2024-01-27 13:52:18.000000 gfloat-0.0.4/.readthedocs.yaml
--rw-r--r--   0 awf       (1000) awf       (1000)     1074 2024-01-27 13:41:22.000000 gfloat-0.0.4/LICENSE
--rw-r--r--   0 awf       (1000) awf       (1000)     1563 2024-03-22 15:18:53.090849 gfloat-0.0.4/PKG-INFO
--rw-r--r--   0 awf       (1000) awf       (1000)      884 2024-03-21 17:36:36.000000 gfloat-0.0.4/README.md
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-03-22 15:18:53.090849 gfloat-0.0.4/docs/
--rw-r--r--   0 awf       (1000) awf       (1000)      638 2024-01-27 16:06:55.000000 gfloat-0.0.4/docs/Makefile
--rw-r--r--   0 awf       (1000) awf       (1000)      799 2024-01-27 13:41:22.000000 gfloat-0.0.4/docs/make.bat
--rw-r--r--   0 awf       (1000) awf       (1000)        8 2024-03-22 15:17:01.000000 gfloat-0.0.4/docs/requirements-rtd.txt
--rw-r--r--   0 awf       (1000) awf       (1000)       41 2024-01-27 13:41:22.000000 gfloat-0.0.4/docs/requirements.txt
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-03-22 15:18:53.090849 gfloat-0.0.4/docs/source/
--rw-r--r--   0 awf       (1000) awf       (1000)      876 2024-03-22 15:17:01.000000 gfloat-0.0.4/docs/source/conf.py
--rw-r--r--   0 awf       (1000) awf       (1000)     1586 2024-03-22 15:17:01.000000 gfloat-0.0.4/docs/source/index.rst
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-03-22 15:18:53.090849 gfloat-0.0.4/notebooks/
--rw-r--r--   0 awf       (1000) awf       (1000)    10166 2024-03-21 14:24:19.000000 gfloat-0.0.4/notebooks/01-decode.ipynb
--rw-r--r--   0 awf       (1000) awf       (1000)      909 2024-03-22 15:17:01.000000 gfloat-0.0.4/pyproject.toml
--rw-r--r--   0 awf       (1000) awf       (1000)       49 2024-03-21 17:23:18.000000 gfloat-0.0.4/requirements-test.txt
--rw-r--r--   0 awf       (1000) awf       (1000)        6 2024-01-27 13:41:22.000000 gfloat-0.0.4/requirements.txt
--rw-r--r--   0 awf       (1000) awf       (1000)       38 2024-03-22 15:18:53.090849 gfloat-0.0.4/setup.cfg
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-03-22 15:18:53.090849 gfloat-0.0.4/src/
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-03-22 15:18:53.090849 gfloat-0.0.4/src/gfloat/
--rw-r--r--   0 awf       (1000) awf       (1000)      351 2024-03-22 15:17:01.000000 gfloat-0.0.4/src/gfloat/__init__.py
--rw-r--r--   0 awf       (1000) awf       (1000)     2488 2024-01-27 17:49:21.000000 gfloat-0.0.4/src/gfloat/decode.py
--rw-r--r--   0 awf       (1000) awf       (1000)     1895 2024-03-22 15:17:01.000000 gfloat-0.0.4/src/gfloat/formats.py
--rw-r--r--   0 awf       (1000) awf       (1000)     3617 2024-03-22 15:17:01.000000 gfloat-0.0.4/src/gfloat/round.py
--rw-r--r--   0 awf       (1000) awf       (1000)     8083 2024-03-22 15:17:01.000000 gfloat-0.0.4/src/gfloat/types.py
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-03-22 15:18:53.090849 gfloat-0.0.4/src/gfloat.egg-info/
--rw-r--r--   0 awf       (1000) awf       (1000)     1563 2024-03-22 15:18:53.000000 gfloat-0.0.4/src/gfloat.egg-info/PKG-INFO
--rw-r--r--   0 awf       (1000) awf       (1000)      603 2024-03-22 15:18:53.000000 gfloat-0.0.4/src/gfloat.egg-info/SOURCES.txt
--rw-r--r--   0 awf       (1000) awf       (1000)        1 2024-03-22 15:18:53.000000 gfloat-0.0.4/src/gfloat.egg-info/dependency_links.txt
--rw-r--r--   0 awf       (1000) awf       (1000)       63 2024-03-22 15:18:53.000000 gfloat-0.0.4/src/gfloat.egg-info/requires.txt
--rw-r--r--   0 awf       (1000) awf       (1000)        7 2024-03-22 15:18:53.000000 gfloat-0.0.4/src/gfloat.egg-info/top_level.txt
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-03-22 15:18:53.090849 gfloat-0.0.4/test/
--rw-r--r--   0 awf       (1000) awf       (1000)     3404 2024-03-20 21:14:57.000000 gfloat-0.0.4/test/test_decode.py
--rw-r--r--   0 awf       (1000) awf       (1000)      756 2024-02-08 12:20:25.000000 gfloat-0.0.4/test/test_finfo.py
--rw-r--r--   0 awf       (1000) awf       (1000)     5470 2024-03-22 15:17:01.000000 gfloat-0.0.4/test/test_round.py
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.490228 gfloat-0.0.5/
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/.github/
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/.github/workflows/
+-rw-r--r--   0 awf       (1000) awf       (1000)      667 2024-03-21 17:30:20.000000 gfloat-0.0.5/.github/workflows/ci.yaml
+-rw-r--r--   0 awf       (1000) awf       (1000)     3099 2024-02-15 18:32:26.000000 gfloat-0.0.5/.gitignore
+-rw-r--r--   0 awf       (1000) awf       (1000)      301 2024-01-27 13:52:18.000000 gfloat-0.0.5/.readthedocs.yaml
+-rw-r--r--   0 awf       (1000) awf       (1000)     1074 2024-01-27 13:41:22.000000 gfloat-0.0.5/LICENSE
+-rw-r--r--   0 awf       (1000) awf       (1000)     1586 2024-04-02 14:34:02.490228 gfloat-0.0.5/PKG-INFO
+-rw-r--r--   0 awf       (1000) awf       (1000)      907 2024-04-02 14:30:00.000000 gfloat-0.0.5/README.md
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/docs/
+-rw-r--r--   0 awf       (1000) awf       (1000)      638 2024-01-27 16:06:55.000000 gfloat-0.0.5/docs/Makefile
+-rw-r--r--   0 awf       (1000) awf       (1000)      799 2024-01-27 13:41:22.000000 gfloat-0.0.5/docs/make.bat
+-rw-r--r--   0 awf       (1000) awf       (1000)        8 2024-03-22 15:17:01.000000 gfloat-0.0.5/docs/requirements-rtd.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)       41 2024-01-27 13:41:22.000000 gfloat-0.0.5/docs/requirements.txt
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/docs/source/
+-rw-r--r--   0 awf       (1000) awf       (1000)      876 2024-04-02 14:33:41.000000 gfloat-0.0.5/docs/source/conf.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     1618 2024-04-02 14:30:00.000000 gfloat-0.0.5/docs/source/index.rst
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/notebooks/
+-rw-r--r--   0 awf       (1000) awf       (1000)    10166 2024-03-21 14:24:19.000000 gfloat-0.0.5/notebooks/01-decode.ipynb
+-rw-r--r--   0 awf       (1000) awf       (1000)      909 2024-04-02 14:33:48.000000 gfloat-0.0.5/pyproject.toml
+-rw-r--r--   0 awf       (1000) awf       (1000)       49 2024-03-21 17:23:18.000000 gfloat-0.0.5/requirements-test.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)        6 2024-03-22 15:19:02.000000 gfloat-0.0.5/requirements.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)       38 2024-04-02 14:34:02.490228 gfloat-0.0.5/setup.cfg
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/src/
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/src/gfloat/
+-rw-r--r--   0 awf       (1000) awf       (1000)      365 2024-04-02 14:30:00.000000 gfloat-0.0.5/src/gfloat/__init__.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     2471 2024-04-02 14:30:00.000000 gfloat-0.0.5/src/gfloat/decode.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     2228 2024-04-02 14:30:00.000000 gfloat-0.0.5/src/gfloat/formats.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     6093 2024-04-02 14:30:00.000000 gfloat-0.0.5/src/gfloat/round.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     9526 2024-04-02 14:30:00.000000 gfloat-0.0.5/src/gfloat/types.py
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.490228 gfloat-0.0.5/src/gfloat.egg-info/
+-rw-r--r--   0 awf       (1000) awf       (1000)     1586 2024-04-02 14:34:02.000000 gfloat-0.0.5/src/gfloat.egg-info/PKG-INFO
+-rw-r--r--   0 awf       (1000) awf       (1000)      623 2024-04-02 14:34:02.000000 gfloat-0.0.5/src/gfloat.egg-info/SOURCES.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)        1 2024-04-02 14:34:02.000000 gfloat-0.0.5/src/gfloat.egg-info/dependency_links.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)       63 2024-04-02 14:34:02.000000 gfloat-0.0.5/src/gfloat.egg-info/requires.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)        7 2024-04-02 14:34:02.000000 gfloat-0.0.5/src/gfloat.egg-info/top_level.txt
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.490228 gfloat-0.0.5/test/
+-rw-r--r--   0 awf       (1000) awf       (1000)     4140 2024-04-02 14:30:00.000000 gfloat-0.0.5/test/test_decode.py
+-rw-r--r--   0 awf       (1000) awf       (1000)      683 2024-04-02 14:30:00.000000 gfloat-0.0.5/test/test_encode.py
+-rw-r--r--   0 awf       (1000) awf       (1000)      968 2024-04-02 14:30:00.000000 gfloat-0.0.5/test/test_finfo.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     5572 2024-04-02 14:30:00.000000 gfloat-0.0.5/test/test_round.py
```

### Comparing `gfloat-0.0.4/.github/workflows/ci.yaml` & `gfloat-0.0.5/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `gfloat-0.0.4/.gitignore` & `gfloat-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `gfloat-0.0.4/LICENSE` & `gfloat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gfloat-0.0.4/PKG-INFO` & `gfloat-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfloat
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generic floating point handling in Python
 Author-email: Andrew Fitzgibbon <awf@fitzgibbon.ie>
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8.1
@@ -37,15 +37,16 @@
 make html
 cd ..
 ```
 
 #### Pushing
 ```
 rm -rf dist
-python3 -m build
+pip install build twine
+python -m build
 echo __token__ | twine upload --repository pypi dist/* --verbose
 ```
 
 #### Notes
 
 All NaNs are the same, with no distinction between signalling or quiet, 
 or between differently encoded NaNs.
```

### Comparing `gfloat-0.0.4/README.md` & `gfloat-0.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 make html
 cd ..
 ```
 
 #### Pushing
 ```
 rm -rf dist
-python3 -m build
+pip install build twine
+python -m build
 echo __token__ | twine upload --repository pypi dist/* --verbose
 ```
 
 #### Notes
 
 All NaNs are the same, with no distinction between signalling or quiet, 
 or between differently encoded NaNs.
```

### Comparing `gfloat-0.0.4/docs/Makefile` & `gfloat-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gfloat-0.0.4/docs/make.bat` & `gfloat-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gfloat-0.0.4/docs/source/conf.py` & `gfloat-0.0.5/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # Configuration file for the Sphinx documentation builder.
 
 # -- Project information
 
 project = "GFloat"
 copyright = "2023, Andrew Fitzgibbon"
 author = "Andrew Fitzgibbon"
-release = "0.0.4"
-version = "0.0.4"
+release = "0.0.5"
+version = "0.0.5"
 
 # -- General configuration
 
 extensions = [
     "sphinx.ext.duration",
     "sphinx.ext.doctest",
     "sphinx.ext.autodoc",
```

### Comparing `gfloat-0.0.4/docs/source/index.rst` & `gfloat-0.0.5/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 API
 ===
 
 .. module:: gfloat
 
 .. autofunction:: decode_float
 .. autofunction:: round_float
+.. autofunction:: encode_float
+
 .. autoclass:: FormatInfo()
    :members:
 .. autoclass:: FloatClass()
    :members:
 .. autoclass:: RoundMode()
    :members:
 .. autoclass:: FloatValue()
```

### Comparing `gfloat-0.0.4/notebooks/01-decode.ipynb` & `gfloat-0.0.5/notebooks/01-decode.ipynb`

 * *Files identical despite different names*

### Comparing `gfloat-0.0.4/pyproject.toml` & `gfloat-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools]
 packages = ['gfloat']
 package-dir = {"" = "src"}
 
 [project]
 name =  "gfloat"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     {name = "Andrew Fitzgibbon", email = "awf@fitzgibbon.ie"},
 ]
 description = "Generic floating point handling in Python"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `gfloat-0.0.4/src/gfloat/decode.py` & `gfloat-0.0.5/src/gfloat/decode.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,21 +45,21 @@
         expval = 1 - expBias
         fsignificand = significand * 2**-t
     else:
         expval = exp - expBias
         fsignificand = 1.0 + significand * 2**-t
 
     # val: the raw value excluding specials
-    val = sign * fsignificand * 2**expval
+    val = sign * fsignificand * 2.0**expval
 
     # Now overwrite the raw value with specials: Infs, NaN, -0, NaN_0
     signed_infinity = -np.inf if signbit else np.inf
 
     fval = val
-    # All-bits-one exponent (ABOE)
+    # All-bits-special exponent (ABSE)
     if exp == 2**w - 1:
         min_i_with_nan = 2 ** (p - 1) - fi.num_high_nans
         if significand >= min_i_with_nan:
             fval = np.nan
         if fi.has_infs and significand == min_i_with_nan - 1:
             fval = signed_infinity
 
@@ -80,10 +80,8 @@
         if isnormal:
             fclass = FloatClass.NORMAL
         else:
             fclass = FloatClass.SUBNORMAL
     else:
         fclass = FloatClass.INFINITE
 
-    return FloatValue(
-        i, fval, val, exp, expval, significand, fsignificand, signbit, fclass, fi
-    )
+    return FloatValue(i, fval, exp, expval, significand, fsignificand, signbit, fclass)
```

### Comparing `gfloat-0.0.4/src/gfloat/formats.py` & `gfloat-0.0.5/src/gfloat/formats.py`

 * *Files 16% similar despite different names*

```diff
@@ -87,7 +87,28 @@
         precision=precision,
         emax=emax,
         has_nz=False,
         has_infs=True,
         num_high_nans=0,
         has_subnormals=True,
     )
+
+
+## Collections of formats
+p3109_formats = [format_info_p3109(p) for p in range(1, 7)]
+
+fp8_formats = [
+    format_info_ocp_e4m3,
+    format_info_ocp_e5m2,
+    *p3109_formats,
+]
+
+fp16_formats = [
+    format_info_binary16,
+    format_info_bfloat16,
+]
+
+all_formats = [
+    *fp8_formats,
+    *fp16_formats,
+    format_info_binary32,
+]
```

### Comparing `gfloat-0.0.4/src/gfloat/round.py` & `gfloat-0.0.5/src/gfloat/round.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) 2024 Graphcore Ltd. All rights reserved.
 
 from enum import Enum
 import numpy as np
 import math
 
-from .types import FormatInfo, RoundMode
+from .types import FormatInfo, RoundMode, FloatValue
+from .decode import decode_float
 
 
 def _isodd(v: int):
     return v & 0x1 == 1
 
 
 def round_float(fi: FormatInfo, v: float, rnd=RoundMode.TiesToEven, sat=False) -> float:
@@ -51,27 +52,29 @@
             raise ValueError(f"No NaN in format {fi}")
 
         # Note that this does not preserve the NaN payload
         return np.nan
 
     # Extract sign
     sign = np.signbit(v)
+    vpos = -v if sign else v
 
-    if v == 0:
+    if vpos < fi.smallest_subnormal / 2:
+        # Test against smallest_subnormal to avoid subnormals in frexp below
+        # Note that this restricts us to types narrower than float64
         result = 0
 
-    elif np.isinf(v):
+    elif np.isinf(vpos):
         result = np.inf
 
     else:
         # Extract significand (mantissa) and exponent
-        fsignificand, expval = np.frexp(np.abs(v))
-
+        fsignificand, expval = np.frexp(vpos)
         assert fsignificand >= 0.5 and fsignificand < 1.0
-        # move significand to [1.0, 2.0)
+        # Bring significand into range [1.0, 2.0)
         fsignificand *= 2
         expval -= 1
 
         # Effective precision, accounting for right shift for subnormal values
         biased_exp = expval + bias
         effective_precision = t + min(biased_exp - 1, 0)
 
@@ -96,16 +99,22 @@
                     isignificand += 1
                 elif d == 0.5:
                     # Tie
                     if rnd == RoundMode.TiesToAway:
                         isignificand += 1
                     else:
                         # All other modes tie to even
-                        if _isodd(isignificand):
-                            isignificand += 1
+                        if fi.precision == 1:
+                            # No significand bits
+                            assert (isignificand == 1) or (isignificand == 0)
+                            if _isodd(biased_exp):
+                                expval += 1
+                        else:
+                            if _isodd(isignificand):
+                                isignificand += 1
 
         result = isignificand * (2.0**expval)
 
     if result == 0:
         if sign and fi.has_nz:
             return -0.0
         else:
@@ -124,7 +133,86 @@
                 raise ValueError(f"No Infs or NaNs in format {fi}, and sat=False")
 
     # Set sign
     if sign:
         result = -result
 
     return result
+
+
+def encode_float(fi: FormatInfo, v: float) -> int:
+    """
+    Encode input to the given :py:class:`FormatInfo`.
+
+    Will round toward zero if v is not in the value set.
+    Will saturate to inf, nan, fi.max in order of precedence.
+    Encode -0 to 0 if not fi.has_nz
+    For other roundings, and saturations, call round_float first.
+
+    :return: The integer code point
+    :rtype: int
+    """
+
+    # Format Constants
+    k = fi.bits
+    p = fi.precision
+    t = p - 1
+
+    # Encode
+    if np.isnan(v):
+        return fi.code_of_nan
+
+    # Overflow/underflow
+    if v > fi.max:
+        return (
+            fi.code_of_posinf
+            if fi.has_infs
+            else fi.code_of_nan if fi.num_nans > 0 else fi.max
+        )
+    if v < fi.min:
+        return (
+            fi.code_of_neginf
+            if fi.has_infs
+            else fi.code_of_nan if fi.num_nans > 0 else fi.min
+        )
+
+    # Finite values
+    sign = np.signbit(v)
+    vpos = -v if sign else v
+
+    if vpos <= fi.smallest_subnormal / 2:
+        isig = 0
+        biased_exp = 0
+    else:
+        assert fi.bits < 64  # TODO: check implementation if fi is binary64
+        sig, exp = np.frexp(vpos)
+        # sig in range [0.5, 1)
+        sig *= 2
+        exp -= 1
+        # now sig in range [1, 2)
+
+        biased_exp = exp + fi.expBias
+        if biased_exp < 1:
+            # subnormal
+            sig *= 2.0 ** (biased_exp - 1)
+            biased_exp = 0
+            assert vpos == sig * 2 ** (1 - fi.expBias)
+        else:
+            if sig > 0:
+                sig -= 1.0
+
+        isig = math.floor(sig * 2**t)
+
+    # Zero
+    if isig == 0 and biased_exp == 0:
+        if sign and fi.has_nz:
+            return fi.code_of_negzero
+        else:
+            return fi.code_of_zero
+
+    # Nonzero
+    assert isig < 2**t
+    assert biased_exp < 2**fi.expBits
+
+    ival = (sign << (k - 1)) | (biased_exp << t) | (isig << 0)
+
+    return ival
```

### Comparing `gfloat-0.0.4/src/gfloat/types.py` & `gfloat-0.0.5/src/gfloat/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,46 @@
     TowardZero = 1  #: :math:`\max \{ r ~ s.t. ~ |r| \le |v| \}`
     TowardNegative = 2  #: :math:`\max \{ r ~ s.t. ~ r \le v \}`
     TowardPositive = 3  #: :math:`\min \{ r ~ s.t. ~ r \ge v \}`
     TiesToEven = 4  #: Round to nearest, ties to even
     TiesToAway = 5  #: Round to nearest, ties away from zero
 
 
+class FloatClass(Enum):
+    """
+    Enum for the classification of a FloatValue.
+    """
+
+    NORMAL = 1  #: A positive or negative normalized non-zero value
+    SUBNORMAL = 2  #: A positive or negative subnormal value
+    ZERO = 3  #: A positive or negative zero value
+    INFINITE = 4  #: A positive or negative infinity (+/-Inf)
+    NAN = 5  #: Not a Number (NaN)
+
+
+@dataclass
+class FloatValue:
+    """
+    A floating-point value decoded in great detail.
+    """
+
+    ival: int  #: Integer code point
+
+    #: Value. Assumed to be exactly round-trippable to python float.
+    #: This is true for all <64bit formats known in 2023.
+    fval: float
+
+    exp: int  #: Raw exponent without bias
+    expval: int  #: Exponent, bias subtracted
+    significand: int  #: Significand as an integer
+    fsignificand: float  #: Significand as a float in the range [0,2)
+    signbit: int  #: Sign bit: 1 => negative, 0 => positive
+    fclass: FloatClass  #: See FloatClass
+
+
 @dataclass
 class FormatInfo:
     """
     Class describing a floating-point format, parametrized
     by width, precision, and special value encoding rules.
 
     """
@@ -81,22 +113,14 @@
             self.expBits == 0 and self.has_infs
         )
 
         # Compute exponent bias.
         exp_for_emax = 2**self.expBits - (2 if all_bits_one_full else 1)
         return exp_for_emax - self.emax
 
-    @property
-    def num_nans(self):
-        """The number of code points which decode to NaN"""
-        return (0 if self.has_nz else 1) + 2 * self.num_high_nans
-
-    def __str__(self):
-        return f"{self.name}"
-
     # numpy finfo properties
     @property
     def bits(self) -> int:
         """
         The number of bits occupied by the type.
         """
         return self.k
@@ -171,14 +195,83 @@
     @property
     def min(self) -> float:
         """
         The smallest representable number, typically ``-max``.
         """
         return -self.max
 
+    @property
+    def num_nans(self):
+        """
+        The number of code points which decode to NaN
+        """
+        return (0 if self.has_nz else 1) + 2 * self.num_high_nans
+
+    @property
+    def code_of_nan(self) -> int:
+        """
+        Return a codepoint for a NaN
+        """
+        if self.num_high_nans > 0:
+            return 2 ** (self.k) - 1
+        if not self.has_nz:
+            return 2 ** (self.k - 1)
+        raise ValueError(f"No NaN in {self}")
+
+    @property
+    def code_of_posinf(self) -> int:
+        """
+        Return a codepoint for positive infinity
+        """
+        if not self.has_infs:
+            raise ValueError(f"No Inf in {self}")
+
+        return 2 ** (self.k - 1) - 1 - self.num_high_nans
+
+    @property
+    def code_of_neginf(self) -> int:
+        """
+        Return a codepoint for negative infinity
+        """
+        if not self.has_infs:
+            raise ValueError(f"No Inf in {self}")
+
+        return 2**self.k - 1 - self.num_high_nans
+
+    @property
+    def code_of_zero(self) -> int:
+        """
+        Return a codepoint for (non-negative) zero
+        """
+        return 0
+
+    @property
+    def code_of_negzero(self) -> int:
+        """
+        Return a codepoint for negative zero
+        """
+        if not self.has_nz:
+            raise ValueError(f"No negative zero in {self}")
+
+        return 2 ** (self.k - 1)
+
+    @property
+    def code_of_max(self) -> int:
+        """
+        Return a codepoint for fi.max
+        """
+        return 2 ** (self.k - 1) - self.num_high_nans - self.has_infs - 1
+
+    @property
+    def code_of_min(self) -> int:
+        """
+        Return a codepoint for fi.max
+        """
+        return 2**self.k - self.num_high_nans - self.has_infs - 1
+
     # @property
     # def minexp(self) -> int:
     #     """
     #     The most negative power of the base (2) consistent with there
     #     being no leading 0's in the mantissa.
     #     """
 
@@ -223,52 +316,18 @@
     # @property
     # def smallest_normal(self) -> float:
     #     """
     #     The smallest positive floating point number with 1 as leading bit in
     #     the mantissa following IEEE-754 (see Notes).
     #     """
 
-    # @property
-    # def smallest_subnormal(self) -> float:
-    #     """
-    #     The smallest positive floating point number with 0 as leading bit in
-    #     the mantissa following IEEE-754.
-    #     """
-
-
-class FloatClass(Enum):
-    """
-    Enum for the classification of a FloatValue.
-    """
-
-    NORMAL = 1  #: A positive or negative normalized non-zero value
-    SUBNORMAL = 2  #: A positive or negative subnormal value
-    ZERO = 3  #: A positive or negative zero value
-    INFINITE = 4  #: A positive or negative infinity (+/-Inf)
-    NAN = 5  #: Not a Number (NaN)
-
-
-@dataclass
-class FloatValue:
-    """
-    A floating-point value decoded in great detail.
-    """
-
-    ival: int  #: Integer code point
-
-    #: Value. Assumed to be exactly round-trippable to python float.
-    #: This is true for all <64bit formats known in 2023.
-    fval: float
-
-    val_raw: float  #: Value, assuming all code points finite
-    exp: int  #: Raw exponent without bias
-    expval: int  #: Exponent, bias subtracted
-    significand: int  #: Significand as an integer
-    fsignificand: float  #: Significand as a float in the range [0,2)
-    signbit: int  #: Sign bit: 1 => negative, 0 => positive
-    fclass: FloatClass  #: See FloatClass
-    fi: FormatInfo  # Backlink to FormatInfo
-
     @property
-    def signstr(self):
-        """Return "+" or "-" according to signbit"""
-        return "-" if self.signbit else "+"
+    def smallest_subnormal(self) -> float:
+        """
+        The smallest positive floating point number with 0 as leading bit in
+        the mantissa following IEEE-754.
+        """
+        assert self.has_subnormals, "not implemented"
+        return 2 ** -(self.expBias + self.tSignificandBits - 1)
+
+    def __str__(self):
+        return f"{self.name}"
```

### Comparing `gfloat-0.0.4/src/gfloat.egg-info/PKG-INFO` & `gfloat-0.0.5/src/gfloat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfloat
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generic floating point handling in Python
 Author-email: Andrew Fitzgibbon <awf@fitzgibbon.ie>
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8.1
@@ -37,15 +37,16 @@
 make html
 cd ..
 ```
 
 #### Pushing
 ```
 rm -rf dist
-python3 -m build
+pip install build twine
+python -m build
 echo __token__ | twine upload --repository pypi dist/* --verbose
 ```
 
 #### Notes
 
 All NaNs are the same, with no distinction between signalling or quiet, 
 or between differently encoded NaNs.
```

### Comparing `gfloat-0.0.4/src/gfloat.egg-info/SOURCES.txt` & `gfloat-0.0.5/src/gfloat.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 src/gfloat/types.py
 src/gfloat.egg-info/PKG-INFO
 src/gfloat.egg-info/SOURCES.txt
 src/gfloat.egg-info/dependency_links.txt
 src/gfloat.egg-info/requires.txt
 src/gfloat.egg-info/top_level.txt
 test/test_decode.py
+test/test_encode.py
 test/test_finfo.py
 test/test_round.py
```

### Comparing `gfloat-0.0.4/test/test_decode.py` & `gfloat-0.0.5/test/test_decode.py`

 * *Files 17% similar despite different names*

```diff
@@ -80,14 +80,42 @@
     assert dec(0x0001) == 2**-133
     assert dec(0x4780) == 65536.0
     assert np.isinf(dec(0x7F80))
     assert np.isnan(dec(0x7F81))
     assert np.isnan(dec(0x7FFF))
 
 
+@pytest.mark.parametrize("fi", p3109_formats, ids=str)
+def test_specials(fi):
+    assert fi.code_of_nan == 0x80
+    assert fi.code_of_zero == 0x00
+    assert fi.code_of_posinf == 0x7F
+    assert fi.code_of_neginf == 0xFF
+
+
+@pytest.mark.parametrize("fi", all_formats, ids=str)
+def test_specials_decode(fi):
+    dec = lambda v: decode_float(fi, v).fval
+
+    assert dec(fi.code_of_zero) == 0
+
+    if fi.num_nans > 0:
+        assert np.isnan(dec(fi.code_of_nan))
+
+    if fi.has_infs:
+        assert dec(fi.code_of_posinf) == np.inf
+        assert dec(fi.code_of_neginf) == -np.inf
+
+    assert dec(fi.code_of_max) == fi.max
+    assert dec(fi.code_of_min) == fi.min
+
+    if fi.has_subnormals:
+        assert dec(1) == fi.smallest_subnormal
+
+
 @pytest.mark.parametrize(
     "fmt,npfmt,int_dtype",
     [
         (format_info_binary16, np.float16, np.uint16),
         (format_info_bfloat16, ml_dtypes.bfloat16, np.uint16),
         (format_info_ocp_e4m3, ml_dtypes.float8_e4m3fn, np.uint8),
     ],
```

### Comparing `gfloat-0.0.4/test/test_finfo.py` & `gfloat-0.0.5/test/test_finfo.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,7 +20,13 @@
     ],
 )
 def test_finfo(fmt, npfmt):
     assert fmt.eps == ml_dtypes.finfo(npfmt).eps
     assert fmt.epsneg == ml_dtypes.finfo(npfmt).epsneg
     assert fmt.max == ml_dtypes.finfo(npfmt).max
     assert fmt.maxexp == ml_dtypes.finfo(npfmt).maxexp
+
+
+def test_constants():
+    assert format_info_p3109(1).smallest_subnormal == 2.0**-62
+    assert format_info_p3109(4).smallest_subnormal == 2.0**-10
+    assert format_info_p3109(7).smallest_subnormal == 2.0**-6
```

### Comparing `gfloat-0.0.4/test/test_round.py` & `gfloat-0.0.5/test/test_round.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,18 @@
     Round `v` using ml_dtypes library
     """
     return np.array([v]).astype(dty).astype(float).item()
 
 
 def test_round_p3109():
     fi = format_info_p3109(4)
+    assert round_float(fi, 0.0068359375) == 0.0068359375
     assert round_float(fi, 0.0029296875) == 0.0029296875
+    assert round_float(fi, 0.0078125) == 0.0078125
+    assert round_float(fi, 0.017578125) == 0.017578125
     assert round_float(fi, 224.0) == 224.0
     assert round_float(fi, 240.0) == np.inf
 
     assert round_float(fi, 224.1, RoundMode.TowardPositive) == np.inf
 
     assert round_float(fi, 232.0) == 224.0
     assert round_float(fi, 232.0, RoundMode.TiesToAway) == np.inf
@@ -84,16 +87,14 @@
     assert round_float(fi, 464.0, sat=True) == 448
     assert round_float(fi, 464.01, sat=True) == 448
     assert round_float(fi, np.inf, sat=True) == 448
     assert round_float(fi, -np.inf, sat=True) == -448
     assert np.isnan(round_float(fi, np.nan, sat=True))
 
 
-p3109_formats = [format_info_p3109(p) for p in range(2, 7)]
-
 some_positive_codepoints = (
     0x00,
     0x01,
     0x02,
     0x03,
     0x07,
     0x0F,
```

