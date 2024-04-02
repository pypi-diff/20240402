# Comparing `tmp/mkdocstrings_python-1.8.0.tar.gz` & `tmp/mkdocstrings_python-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocstrings_python-1.8.0.tar", last modified: Mon Jan  8 16:15:05 2024, max compression
+gzip compressed data, was "mkdocstrings_python-1.9.0.tar", last modified: Wed Mar 13 19:04:55 2024, max compression
```

## Comparing `mkdocstrings_python-1.8.0.tar` & `mkdocstrings_python-1.9.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0      754 2024-01-08 15:33:26.847628 mkdocstrings_python-1.8.0/LICENSE
--rw-r--r--   0        0        0     4265 2024-01-08 15:33:32.210778 mkdocstrings_python-1.8.0/README.md
--rw-r--r--   0        0        0     2600 2024-01-08 16:15:05.809152 mkdocstrings_python-1.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-08 15:33:32.720761 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/py.typed
--rw-r--r--   0        0        0      326 2024-01-08 15:33:33.840722 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/__init__.py
--rw-r--r--   0        0        0     2764 2024-01-08 15:33:33.107414 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/debug.py
--rw-r--r--   0        0        0    22539 2024-01-08 15:59:07.064308 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/handler.py
--rw-r--r--   0        0        0    16046 2024-01-08 15:59:07.064308 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/rendering.py
--rw-r--r--   0        0        0     2944 2024-01-08 15:59:07.064308 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
--rw-r--r--   0        0        0     5709 2024-01-08 15:33:33.297408 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html
--rw-r--r--   0        0        0     5413 2024-01-08 15:59:07.064308 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html
--rw-r--r--   0        0        0     2163 2024-01-08 15:33:33.354072 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
--rw-r--r--   0        0        0      274 2024-01-08 15:33:33.500734 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
--rw-r--r--   0        0        0     3080 2024-01-08 15:59:07.064308 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
--rw-r--r--   0        0        0     2123 2024-01-08 15:59:07.064308 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/classes.html
--rw-r--r--   0        0        0      460 2024-01-08 15:33:33.444069 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
--rw-r--r--   0        0        0     2646 2024-01-08 15:59:07.064308 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/functions.html
--rw-r--r--   0        0        0     2137 2024-01-08 15:59:07.064308 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/modules.html
--rw-r--r--   0        0        0     2866 2024-01-08 15:33:33.437403 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
--rw-r--r--   0        0        0     3823 2024-01-08 15:33:33.437403 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
--rw-r--r--   0        0        0     2478 2024-01-08 15:33:33.440736 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
--rw-r--r--   0        0        0     3503 2024-01-08 15:33:33.440736 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
--rw-r--r--   0        0        0     3479 2024-01-08 15:33:33.440736 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
--rw-r--r--   0        0        0     2453 2024-01-08 15:33:33.440736 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
--rw-r--r--   0        0        0     3444 2024-01-08 15:33:33.440736 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
--rw-r--r--   0        0        0     2078 2024-01-08 15:33:33.277408 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
--rw-r--r--   0        0        0     3515 2024-01-08 15:59:07.064308 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html
--rw-r--r--   0        0        0      250 2024-01-08 15:33:33.350739 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
--rw-r--r--   0        0        0      966 2024-01-08 15:33:33.317407 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/en.html
--rw-r--r--   0        0        0      984 2024-01-08 15:33:33.320740 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/ja.html
--rw-r--r--   0        0        0      902 2024-01-08 15:33:33.320740 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/zh.html
--rw-r--r--   0        0        0     2480 2024-01-08 15:59:07.064308 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html
--rw-r--r--   0        0        0     2833 2024-01-08 15:33:33.320740 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
--rw-r--r--   0        0        0        0 2024-01-08 15:59:07.064308 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/summary.html
--rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/summary/attributes.html
--rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/summary/classes.html
--rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/summary/functions.html
--rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/summary/modules.html
--rw-r--r--   0        0        0       37 2024-01-08 15:33:33.217410 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/attribute.html
--rw-r--r--   0        0        0       36 2024-01-08 15:33:33.217410 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/children.html
--rw-r--r--   0        0        0       33 2024-01-08 15:33:33.217410 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/class.html
--rw-r--r--   0        0        0       37 2024-01-08 15:33:33.217410 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring.html
--rw-r--r--   0        0        0       48 2024-01-08 15:33:33.517400 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
--rw-r--r--   0        0        0       48 2024-01-08 15:33:33.517400 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
--rw-r--r--   0        0        0       45 2024-01-08 15:33:33.500734 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring/classes.html
--rw-r--r--   0        0        0       46 2024-01-08 15:33:33.517400 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
--rw-r--r--   0        0        0       47 2024-01-08 15:33:33.500734 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring/functions.html
--rw-r--r--   0        0        0       45 2024-01-08 15:33:33.500734 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring/modules.html
--rw-r--r--   0        0        0       54 2024-01-08 15:33:33.520733 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
--rw-r--r--   0        0        0       48 2024-01-08 15:33:33.520733 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
--rw-r--r--   0        0        0       44 2024-01-08 15:33:33.520733 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
--rw-r--r--   0        0        0       46 2024-01-08 15:33:33.517400 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
--rw-r--r--   0        0        0       45 2024-01-08 15:33:33.520733 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
--rw-r--r--   0        0        0       43 2024-01-08 15:33:33.517400 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
--rw-r--r--   0        0        0       44 2024-01-08 15:33:33.520733 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
--rw-r--r--   0        0        0       38 2024-01-08 15:33:33.254076 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/expression.html
--rw-r--r--   0        0        0       36 2024-01-08 15:33:33.230743 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/function.html
--rw-r--r--   0        0        0       34 2024-01-08 15:33:33.230743 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/labels.html
--rw-r--r--   0        0        0      431 2024-01-08 15:33:33.154079 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/language.html
--rw-r--r--   0        0        0       39 2024-01-08 15:33:33.180745 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/languages/en.html
--rw-r--r--   0        0        0       39 2024-01-08 15:33:33.180745 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/languages/ja.html
--rw-r--r--   0        0        0       39 2024-01-08 15:33:33.180745 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/languages/zh.html
--rw-r--r--   0        0        0       34 2024-01-08 15:33:33.250743 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/module.html
--rw-r--r--   0        0        0       37 2024-01-08 15:33:33.250743 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/signature.html
--rw-r--r--   0        0        0     2540 2024-01-08 15:59:07.067641 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/style.css
--rw-r--r--   0        0        0       35 2024-01-08 15:59:07.067641 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/summary.html
--rw-r--r--   0        0        0       46 2024-01-08 15:59:07.067641 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/summary/attributes.html
--rw-r--r--   0        0        0       43 2024-01-08 15:59:07.067641 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/summary/classes.html
--rw-r--r--   0        0        0       45 2024-01-08 15:59:07.067641 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/summary/functions.html
--rw-r--r--   0        0        0       43 2024-01-08 15:59:07.067641 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/summary/modules.html
--rw-r--r--   0        0        0     1001 2024-01-08 15:33:33.610730 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html
--rw-r--r--   0        0        0     1007 2024-01-08 15:33:33.614064 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html
--rw-r--r--   0        0        0     1279 2024-01-08 15:33:33.614064 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html
--rw-r--r--   0        0        0      928 2024-01-08 15:33:33.810723 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html
--rw-r--r--   0        0        0     1131 2024-01-08 15:33:33.837389 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html
--rw-r--r--   0        0        0     1080 2024-01-08 15:33:33.837389 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html
--rw-r--r--   0        0        0      923 2024-01-08 15:33:33.840722 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html
--rw-r--r--   0        0        0     1114 2024-01-08 15:33:33.840722 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html
--rw-r--r--   0        0        0      431 2024-01-08 15:33:33.557399 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/language.html
--rw-r--r--   0        0        0      966 2024-01-08 15:33:33.600731 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/en.html
--rw-r--r--   0        0        0      984 2024-01-08 15:33:33.610730 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/ja.html
--rw-r--r--   0        0        0      902 2024-01-08 15:33:33.610730 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/zh.html
--rw-r--r--   0        0        0      971 2024-01-08 15:33:33.557399 mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
--rw-r--r--   0        0        0      174 2024-01-08 15:33:33.904054 mkdocstrings_python-1.8.0/tests/__init__.py
--rw-r--r--   0        0        0     2976 2024-01-08 15:33:33.857389 mkdocstrings_python-1.8.0/tests/conftest.py
--rw-r--r--   0        0        0     5206 2024-01-08 15:33:33.874055 mkdocstrings_python-1.8.0/tests/test_handler.py
--rw-r--r--   0        0        0     5450 2024-01-08 15:33:33.890721 mkdocstrings_python-1.8.0/tests/test_rendering.py
--rw-r--r--   0        0        0     1332 2024-01-08 15:33:33.907387 mkdocstrings_python-1.8.0/tests/test_themes.py
--rw-r--r--   0        0        0     5770 1970-01-01 00:00:00.000000 mkdocstrings_python-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2024-03-13 18:37:57.897079 mkdocstrings_python-1.9.0/LICENSE
+-rw-r--r--   0        0        0     4043 2024-03-13 18:43:23.554055 mkdocstrings_python-1.9.0/README.md
+-rw-r--r--   0        0        0     1649 2024-03-13 19:04:55.355618 mkdocstrings_python-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-03-13 18:37:58.007075 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/__init__.py
+-rw-r--r--   0        0        0     2764 2024-03-13 18:47:50.869435 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/debug.py
+-rw-r--r--   0        0        0    22925 2024-03-13 19:03:33.684715 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/handler.py
+-rw-r--r--   0        0        0        0 2024-03-13 18:37:58.043741 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/py.typed
+-rw-r--r--   0        0        0    16046 2024-03-13 19:03:45.627693 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/rendering.py
+-rw-r--r--   0        0        0     2944 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
+-rw-r--r--   0        0        0     5709 2024-01-08 15:33:33.297408 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html
+-rw-r--r--   0        0        0     5413 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html
+-rw-r--r--   0        0        0     2163 2024-01-08 15:33:33.354072 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
+-rw-r--r--   0        0        0      274 2024-01-08 15:33:33.500734 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
+-rw-r--r--   0        0        0     3101 2024-01-31 11:17:41.321947 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
+-rw-r--r--   0        0        0     2144 2024-01-31 11:18:21.618366 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/classes.html
+-rw-r--r--   0        0        0      460 2024-01-08 15:33:33.444069 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
+-rw-r--r--   0        0        0     2667 2024-01-31 11:18:34.984950 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/functions.html
+-rw-r--r--   0        0        0     2158 2024-01-31 11:18:43.178233 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/modules.html
+-rw-r--r--   0        0        0     2887 2024-01-31 11:30:21.673669 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
+-rw-r--r--   0        0        0     3844 2024-01-31 11:30:30.813558 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
+-rw-r--r--   0        0        0     2499 2024-01-31 11:30:38.240136 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
+-rw-r--r--   0        0        0     3524 2024-01-31 11:30:44.303396 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
+-rw-r--r--   0        0        0     3500 2024-01-31 11:30:52.079970 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
+-rw-r--r--   0        0        0     2474 2024-01-31 11:30:58.983221 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
+-rw-r--r--   0        0        0     3465 2024-01-31 11:31:06.949793 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
+-rw-r--r--   0        0        0     2078 2024-01-08 15:33:33.277408 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
+-rw-r--r--   0        0        0     3515 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html
+-rw-r--r--   0        0        0      273 2024-03-13 19:03:33.684715 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
+-rw-r--r--   0        0        0      966 2024-01-08 15:33:33.317407 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/en.html
+-rw-r--r--   0        0        0      984 2024-01-08 15:33:33.320740 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/ja.html
+-rw-r--r--   0        0        0      902 2024-01-08 15:33:33.320740 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/zh.html
+-rw-r--r--   0        0        0     2480 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html
+-rw-r--r--   0        0        0     2833 2024-02-20 12:56:18.816418 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
+-rw-r--r--   0        0        0        0 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/summary.html
+-rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/summary/attributes.html
+-rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/summary/classes.html
+-rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/summary/functions.html
+-rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/summary/modules.html
+-rw-r--r--   0        0        0       37 2024-01-08 15:33:33.217410 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/attribute.html
+-rw-r--r--   0        0        0       36 2024-01-08 15:33:33.217410 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/children.html
+-rw-r--r--   0        0        0       33 2024-01-08 15:33:33.217410 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/class.html
+-rw-r--r--   0        0        0       37 2024-01-08 15:33:33.217410 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring.html
+-rw-r--r--   0        0        0       48 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
+-rw-r--r--   0        0        0       48 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
+-rw-r--r--   0        0        0       45 2024-01-08 15:33:33.500734 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/classes.html
+-rw-r--r--   0        0        0       46 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
+-rw-r--r--   0        0        0       47 2024-01-08 15:33:33.500734 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/functions.html
+-rw-r--r--   0        0        0       45 2024-01-08 15:33:33.500734 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/modules.html
+-rw-r--r--   0        0        0       54 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
+-rw-r--r--   0        0        0       48 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
+-rw-r--r--   0        0        0       44 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
+-rw-r--r--   0        0        0       46 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
+-rw-r--r--   0        0        0       45 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
+-rw-r--r--   0        0        0       43 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
+-rw-r--r--   0        0        0       44 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
+-rw-r--r--   0        0        0       38 2024-01-08 15:33:33.254076 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/expression.html
+-rw-r--r--   0        0        0       36 2024-01-08 15:33:33.230743 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/function.html
+-rw-r--r--   0        0        0       34 2024-01-08 15:33:33.230743 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/labels.html
+-rw-r--r--   0        0        0      431 2024-01-08 15:33:33.154079 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/language.html
+-rw-r--r--   0        0        0       39 2024-01-08 15:33:33.180745 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/languages/en.html
+-rw-r--r--   0        0        0       39 2024-01-08 15:33:33.180745 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/languages/ja.html
+-rw-r--r--   0        0        0       39 2024-01-08 15:33:33.180745 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/languages/zh.html
+-rw-r--r--   0        0        0       34 2024-01-08 15:33:33.250743 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/module.html
+-rw-r--r--   0        0        0       37 2024-01-08 15:33:33.250743 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/signature.html
+-rw-r--r--   0        0        0     2540 2024-03-13 19:03:45.627693 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/style.css
+-rw-r--r--   0        0        0       35 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/summary.html
+-rw-r--r--   0        0        0       46 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/summary/attributes.html
+-rw-r--r--   0        0        0       43 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/summary/classes.html
+-rw-r--r--   0        0        0       45 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/summary/functions.html
+-rw-r--r--   0        0        0       43 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/summary/modules.html
+-rw-r--r--   0        0        0     1001 2024-01-08 15:33:33.610730 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html
+-rw-r--r--   0        0        0     1007 2024-01-08 15:33:33.614064 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html
+-rw-r--r--   0        0        0     1279 2024-01-08 15:33:33.614064 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html
+-rw-r--r--   0        0        0      928 2024-01-08 15:33:33.810723 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html
+-rw-r--r--   0        0        0     1131 2024-01-08 15:33:33.837389 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html
+-rw-r--r--   0        0        0     1080 2024-01-08 15:33:33.837389 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html
+-rw-r--r--   0        0        0      923 2024-01-08 15:33:33.840722 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html
+-rw-r--r--   0        0        0     1114 2024-01-08 15:33:33.840722 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html
+-rw-r--r--   0        0        0      431 2024-01-08 15:33:33.557399 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/language.html
+-rw-r--r--   0        0        0      966 2024-01-08 15:33:33.600731 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/en.html
+-rw-r--r--   0        0        0      984 2024-01-08 15:33:33.610730 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/ja.html
+-rw-r--r--   0        0        0      902 2024-01-08 15:33:33.610730 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/zh.html
+-rw-r--r--   0        0        0      971 2024-01-08 15:33:33.557399 mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
+-rw-r--r--   0        0        0      174 2024-03-13 18:38:00.683662 mkdocstrings_python-1.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     2915 2024-03-13 18:52:36.467604 mkdocstrings_python-1.9.0/tests/conftest.py
+-rw-r--r--   0        0        0     5206 2024-01-08 15:33:33.874055 mkdocstrings_python-1.9.0/tests/test_handler.py
+-rw-r--r--   0        0        0     5450 2024-01-08 15:33:33.890721 mkdocstrings_python-1.9.0/tests/test_rendering.py
+-rw-r--r--   0        0        0     1281 2024-03-13 18:54:08.091544 mkdocstrings_python-1.9.0/tests/test_themes.py
+-rw-r--r--   0        0        0     5524 1970-01-01 00:00:00.000000 mkdocstrings_python-1.9.0/PKG-INFO
```

### Comparing `mkdocstrings_python-1.8.0/LICENSE` & `mkdocstrings_python-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/README.md` & `mkdocstrings_python-1.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,16 @@
 <h1 align="center">mkdocstrings-python</h1>
 
 <p align="center">A Python handler for <a href="https://github.com/mkdocstrings/mkdocstrings"><i>mkdocstrings</i></a>.</p>
 
-<p align="center">
-  <a href="https://github.com/mkdocstrings/python/actions?query=workflow%3Aci">
-    <img alt="ci" src="https://github.com/mkdocstrings/python/workflows/ci/badge.svg" />
-  </a>
-  <a href="https://mkdocstrings.github.io/python/">
-    <img alt="documentation" src="https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat" />
-  </a>
-  <a href="https://pypi.org/project/mkdocstrings-python/">
-    <img alt="pypi version" src="https://img.shields.io/pypi/v/mkdocstrings-python.svg" />
-  </a>
-  <a href="https://gitpod.io/#https://github.com/mkdocstrings/python">
-    <img alt="gitpod" src="https://img.shields.io/badge/gitpod-workspace-blue.svg?style=flat" />
-  </a>
-  <a href="https://app.gitter.im/#/room/#mkdocstrings_python:gitter.im">
-    <img alt="gitter" src="https://badges.gitter.im/join%20chat.svg" />
-  </a>
-</p>
+[![ci](https://github.com/mkdocstrings/python/workflows/ci/badge.svg)](https://github.com/mkdocstrings/python/actions?query=workflow%3Aci)
+[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://mkdocstrings.github.io/python/)
+[![pypi version](https://img.shields.io/pypi/v/mkdocstrings-python.svg)](https://pypi.org/project/mkdocstrings-python/)
+[![gitpod](https://img.shields.io/badge/gitpod-workspace-blue.svg?style=flat)](https://gitpod.io/#https://github.com/mkdocstrings/python)
+[![gitter](https://badges.gitter.im/join%20chat.svg)](https://app.gitter.im/#/room/#python:gitter.im)
 
 ---
 
 <p align="center"><img src="logo.png"></p>
 
 The Python handler uses [Griffe](https://mkdocstrings.github.io/griffe)
 to collect documentation from Python source code.
```

#### html2text {}

```diff
@@ -1,11 +1,18 @@
                        ************ mmkkddooccssttrriinnggss--ppyytthhoonn ************
                       A Python handler for _m_k_d_o_c_s_t_r_i_n_g_s.
-               _[_c_i_]_[_d_o_c_u_m_e_n_t_a_t_i_o_n_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_g_i_t_p_o_d_]_[_g_i_t_t_e_r_]
----
+[![ci](https://github.com/mkdocstrings/python/workflows/ci/badge.svg)](https://
+github.com/mkdocstrings/python/actions?query=workflow%3Aci) [![documentation]
+(https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)]
+(https://mkdocstrings.github.io/python/) [![pypi version](https://
+img.shields.io/pypi/v/mkdocstrings-python.svg)](https://pypi.org/project/
+mkdocstrings-python/) [![gitpod](https://img.shields.io/badge/gitpod-workspace-
+blue.svg?style=flat)](https://gitpod.io/#https://github.com/mkdocstrings/
+python) [![gitter](https://badges.gitter.im/join%20chat.svg)](https://
+app.gitter.im/#/room/#python:gitter.im) ---
                                   [logo.png]
 The Python handler uses [Griffe](https://mkdocstrings.github.io/griffe) to
 collect documentation from Python source code. The word "griffe" can sometimes
 be used instead of "signature" in French. Griffe is able to visit the Abstract
 Syntax Tree (AST) of the source code to extract useful information. It is also
 able to execute the code (by importing it) and introspect objects in memory
 when source code is not available. Finally, it can parse docstrings following
```

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/debug.py` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/debug.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/handler.py` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     enable_inventory: bool = True
     """Whether this handler is interested in enabling the creation of the `objects.inv` Sphinx inventory file."""
     fallback_theme = "material"
     """The fallback theme."""
     fallback_config: ClassVar[dict] = {"fallback": True}
     """The configuration used to collect item during autorefs fallback."""
     default_config: ClassVar[dict] = {
+        "find_stubs_package": False,
         "docstring_style": "google",
         "docstring_options": {},
         "show_symbol_type_heading": False,
         "show_symbol_type_toc": False,
         "show_root_heading": False,
         "show_root_toc_entry": True,
         "show_root_full_path": True,
@@ -101,19 +102,21 @@
         "members": None,
         "inherited_members": False,
         "filters": ["!^_[^_]"],
         "annotations_path": "brief",
         "preload_modules": None,
         "allow_inspection": True,
         "summary": False,
+        "show_labels": True,
         "unwrap_annotated": False,
     }
     """Default handler configuration.
 
     Attributes: General options:
+        find_stubs_package (bool): Whether to load stubs package (package-stubs) when extracting docstrings. Default `False`.
         allow_inspection (bool): Whether to allow inspecting modules when visiting them is not possible. Default: `True`.
         show_bases (bool): Show the base classes of a class. Default: `True`.
         show_source (bool): Show the source code of this object. Default: `True`.
         preload_modules (list[str] | None): Pre-load modules that are
             not specified directly in autodoc instructions (`::: identifier`).
             It is useful when you want to render documentation for a particular member of an object,
             and this member is imported from another package than its parent.
@@ -148,14 +151,15 @@
         filters (list[str] | None): A list of filters applied to filter objects based on their name.
             A filter starting with `!` will exclude matching objects instead of including them.
             The `members` option takes precedence over `filters` (filters will still be applied recursively
             to lower members in the hierarchy). Default: `["!^_[^_]"]`.
         group_by_category (bool): Group the object's children by categories: attributes, classes, functions, and modules. Default: `True`.
         show_submodules (bool): When rendering a module, show its submodules recursively. Default: `False`.
         summary (bool | dict[str, bool]): Whether to render summaries of modules, classes, functions (methods) and attributes.
+        show_labels (bool): Whether to show labels of the members. Default: `True`.
 
     Attributes: Docstrings options:
         docstring_style (str): The docstring style to use: `google`, `numpy`, `sphinx`, or `None`. Default: `"google"`.
         docstring_options (dict): The options for the docstring parser. See parsers under [`griffe.docstrings`][].
         docstring_section_style (str): The style used to render docstring sections. Options: `table`, `list`, `spacy`. Default: `"table"`.
         merge_init_into_class (bool): Whether to merge the `__init__` method into the class' signature and docstring. Default: `False`.
         show_if_no_docstring (bool): Show the object heading even if it has no docstring or children with docstrings. Default: `False`.
@@ -275,16 +279,16 @@
                 modules_collection=self._modules_collection,
                 lines_collection=self._lines_collection,
                 allow_inspection=final_config["allow_inspection"],
             )
             try:
                 for pre_loaded_module in final_config.get("preload_modules") or []:
                     if pre_loaded_module not in self._modules_collection:
-                        loader.load(pre_loaded_module)
-                loader.load(module_name)
+                        loader.load(pre_loaded_module, find_stubs_package=final_config["find_stubs_package"])
+                loader.load(module_name, find_stubs_package=final_config["find_stubs_package"])
             except ImportError as error:
                 raise CollectionError(str(error)) from error
             unresolved, iterations = loader.resolve_aliases(
                 implicit=False,
                 external=self._load_external_modules,
             )
             if unresolved:
```

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/rendering.py` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/rendering.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {{ log.debug("Rendering attributes section") }}
 
 {% import "language.html" as lang with context %}
 
 {% if config.docstring_section_style == "table" %}
-  {% block table_style %}
+  {% block table_style scoped %}
   <p><strong>{{ section.title or lang.t("Attributes:") }}</strong></p>
   <table>
     <thead>
       <tr>
         <th>{{ lang.t("Name") }}</th>
         <th>{{ lang.t("Type") }}</th>
         <th>{{ lang.t("Description") }}</th>
@@ -31,15 +31,15 @@
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
-  {% block list_style %}
+  {% block list_style scoped %}
   <p>{{ section.title or lang.t("Attributes:") }}</p>
   <ul>
     {% for attribute in section.value %}
       <li class="field-body">
         <b><code><span data-autorefs-optional-hover="{{ obj.path }}.{{ attribute.name }}">{{ attribute.name }}</span></code></b>
         {% if attribute.annotation %}
           {% with expression = attribute.annotation %}
@@ -51,15 +51,15 @@
           {{ attribute.description|convert_markdown(heading_level, html_id) }}
         </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
-  {% block spacy_style %}
+  {% block spacy_style scoped %}
   <table>
     <thead>
       <tr>
         <th><b>{{ (section.title or lang.t("ATTRIBUTE")).rstrip(":").upper() }}</b></th>
         <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
 {{ log.debug("Rendering attributes section") }} {% import "language.html" as
 lang with context %} {% if config.docstring_section_style == "table" %} {%
-block table_style %}
+block table_style scoped %}
 {{{{ sseeccttiioonn..ttiittllee oorr llaanngg..tt((""AAttttrriibbuutteess::"")) }}}}
 {{{{ llaanngg..tt((""NNaammee"")) {{{{ llaanngg..tt((""TTyyppee"")) }}}} {{{{ llaanngg..tt((""DDeessccrriippttiioonn"")) }}}}
 }}}}
                   {% if
                   attribute.annotation
                   %} {% with
                   expression =         {
 {{ attribute.name attribute.annotation {
 }}                %} {% include        attribute.description|convert_markdown
                   "expression.html"    (heading_level, html_id) }}
                   with context %} {%
                   endwith %} {% endif
                   %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
-{% block list_style %}
+{% block list_style scoped %}
 {{ section.title or lang.t("Attributes:") }}
     * {% for attribute in section.value %}
     * {{{{ aattttrriibbuuttee..nnaammee }}}} {% if attribute.annotation %} {% with expression =
       attribute.annotation %} ({% include "expression.html" with context %}) {%
       endwith %} {% endif %} â
       {{ attribute.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
-{% block spacy_style %}
+{% block spacy_style scoped %}
 {{{{ ((sseeccttiioonn..ttiittllee oorr llaanngg..tt           {{{{ llaanngg..tt((""DDEESSCCRRIIPPTTIIOONN"")) }}}}
 ((""AATTTTRRIIBBUUTTEE""))))..rrssttrriipp((""::""))..uuppppeerr(()) }}}}
                                       {{ attribute.description|convert_markdown
                                       (heading_level, html_id) }}
 {{ attribute.name }}                  {% if attribute.annotation %} TTYYPPEE:: {%
                                       with expression = attribute.annotation %}
                                       {% include "expression.html" with context
```

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/classes.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/classes.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {{ log.debug("Rendering classes section") }}
 
 {% import "language.html" as lang with context %}
 
 {% if config.docstring_section_style == "table" %}
-  {% block table_style %}
+  {% block table_style scoped %}
   <p><strong>{{ section.title or lang.t("Classes:") }}</strong></p>
   <table>
     <thead>
       <tr>
         <th>{{ lang.t("Name") }}</th>
         <th>{{ lang.t("Description") }}</th>
       </tr>
@@ -23,30 +23,30 @@
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
-  {% block list_style %}
+  {% block list_style scoped %}
   <p>{{ section.title or lang.t("Classes:") }}</p>
   <ul>
     {% for class in section.value %}
       <li class="field-body">
         <b><code><span data-autorefs-optional-hover="{{ obj.path }}.{{ class.name }}">{{ class.name }}</span></code></b>
         –
         <div class="doc-md-description">
           {{ class.description|convert_markdown(heading_level, html_id) }}
         </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
-  {% block spacy_style %}
+  {% block spacy_style scoped %}
   <table>
     <thead>
       <tr>
         <th><b>{{ (section.title or lang.t("CLASS")).rstrip(":").upper() }}</b></th>
         <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 {{ log.debug("Rendering classes section") }} {% import "language.html" as lang
 with context %} {% if config.docstring_section_style == "table" %} {% block
-table_style %}
+table_style scoped %}
 {{{{ sseeccttiioonn..ttiittllee oorr llaanngg..tt((""CCllaasssseess::"")) }}}}
 {{{{ llaanngg..tt((""NNaammee"")) }}}} {{{{ llaanngg..tt((""DDeessccrriippttiioonn"")) }}}}
 {{ class.name }}     {{ class.description|convert_markdown(heading_level,
                      html_id) }}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
-{% block list_style %}
+{% block list_style scoped %}
 {{ section.title or lang.t("Classes:") }}
     * {% for class in section.value %}
     * {{{{ ccllaassss..nnaammee }}}} â
       {{ class.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
-{% block spacy_style %}
+{% block spacy_style scoped %}
 {{{{ ((sseeccttiioonn..ttiittllee oorr llaanngg..tt       {{{{ llaanngg..tt((""DDEESSCCRRIIPPTTIIOONN"")) }}}}
 ((""CCLLAASSSS""))))..rrssttrriipp((""::""))..uuppppeerr(()) }}}}
 {{ class.name }}                  {{ class.description|convert_markdown
                                   (heading_level, html_id) }}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/functions.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/functions.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {{ log.debug("Rendering functions section") }}
 
 {% import "language.html" as lang with context %}
 
 {% if config.docstring_section_style == "table" %}
-  {% block table_style %}
+  {% block table_style scoped %}
   <p><strong>{{ section.title or lang.t("Methods:") if obj.is_class else lang.t("Functions:") }}</strong></p>
   <table>
     <thead>
       <tr>
         <th>{{ lang.t("Name") }}</th>
         <th>{{ lang.t("Description") }}</th>
       </tr>
@@ -25,15 +25,15 @@
           </tr>
         {% endif %}
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
-  {% block list_style %}
+  {% block list_style scoped %}
   <p>{{ section.title or lang.t("Methods:") if obj.is_class else lang.t("Functions:") }}</p>
   <ul>
     {% for function in section.value %}
       {% if not function.name == "__init__" or not config.merge_init_into_class %}
         <li class="field-body">
           <b><code><span data-autorefs-optional-hover="{{ obj.path }}.{{ function.name }}">{{ function.name }}</span></code></b>
           –
@@ -42,15 +42,15 @@
           </div>
         </li>
       {% endif %}
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
-  {% block spacy_style %}
+  {% block spacy_style scoped %}
   <table>
     <thead>
       <tr>
         <th><b>{{ (section.title or lang.t("METHOD") if obj.is_class else lang.t("FUNCTION")).rstrip(":").upper() }}</b></th>
         <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
 {{ log.debug("Rendering functions section") }} {% import "language.html" as
 lang with context %} {% if config.docstring_section_style == "table" %} {%
-block table_style %}
+block table_style scoped %}
 {{{{ sseeccttiioonn..ttiittllee oorr llaanngg..tt((""MMeetthhooddss::"")) iiff oobbjj..iiss__ccllaassss eellssee llaanngg..tt((""FFuunnccttiioonnss::
 "")) }}}}
 {{{{ llaanngg..tt((""NNaammee"")) }}}} {{{{ llaanngg..tt((""DDeessccrriippttiioonn"")) }}}}
 {{ function.name }}  {{ function.description|convert_markdown(heading_level,
                      html_id) }}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
-{% block list_style %}
+{% block list_style scoped %}
 {{ section.title or lang.t("Methods:") if obj.is_class else lang.t("Functions:
 ") }}
     * {% for function in section.value %} {% if not function.name == "__init__"
       or not config.merge_init_into_class %}
     * {{{{ ffuunnccttiioonn..nnaammee }}}} â
       {{ function.description|convert_markdown(heading_level, html_id) }}
     * {% endif %} {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
-{% block spacy_style %}
+{% block spacy_style scoped %}
 {{{{ ((sseeccttiioonn..ttiittllee oorr llaanngg..tt((""MMEETTHHOODD""))
 iiff oobbjj..iiss__ccllaassss eellssee llaanngg..tt           {{{{ llaanngg..tt((""DDEESSCCRRIIPPTTIIOONN"")) }}}}
 ((""FFUUNNCCTTIIOONN""))))..rrssttrriipp((""::""))..uuppppeerr(()) }}}}
 {{ function.name }}                   {{ function.description|convert_markdown
                                       (heading_level, html_id) }}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/modules.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/modules.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {{ log.debug("Rendering modules section") }}
 
 {% import "language.html" as lang with context %}
 
 {% if config.docstring_section_style == "table" %}
-  {% block table_style %}
+  {% block table_style scoped %}
   <p><strong>{{ section.title or lang.t("Modules:") }}</strong></p>
   <table>
     <thead>
       <tr>
         <th>{{ lang.t("Name") }}</th>
         <th>{{ lang.t("Description") }}</th>
       </tr>
@@ -23,30 +23,30 @@
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
-  {% block list_style %}
+  {% block list_style scoped %}
   <p>{{ section.title or lang.t("Modules:") }}</p>
   <ul>
     {% for module in section.value %}
       <li class="field-body">
         <b><code><span data-autorefs-optional-hover="{{ obj.path }}.{{ module.name }}">{{ module.name }}</span></code></b>
         –
         <div class="doc-md-description">
           {{ module.description|convert_markdown(heading_level, html_id) }}
         </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
-  {% block spacy_style %}
+  {% block spacy_style scoped %}
   <table>
     <thead>
       <tr>
         <th><b>{{ (section.title or lang.t("MODULE")).rstrip(":").upper() }}</b></th>
         <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 {{ log.debug("Rendering modules section") }} {% import "language.html" as lang
 with context %} {% if config.docstring_section_style == "table" %} {% block
-table_style %}
+table_style scoped %}
 {{{{ sseeccttiioonn..ttiittllee oorr llaanngg..tt((""MMoodduulleess::"")) }}}}
 {{{{ llaanngg..tt((""NNaammee"")) }}}} {{{{ llaanngg..tt((""DDeessccrriippttiioonn"")) }}}}
 {{ module.name }}    {{ module.description|convert_markdown(heading_level,
                      html_id) }}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
-{% block list_style %}
+{% block list_style scoped %}
 {{ section.title or lang.t("Modules:") }}
     * {% for module in section.value %}
     * {{{{ mmoodduullee..nnaammee }}}} â
       {{ module.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
-{% block spacy_style %}
+{% block spacy_style scoped %}
 {{{{ ((sseeccttiioonn..ttiittllee oorr llaanngg..tt        {{{{ llaanngg..tt((""DDEESSCCRRIIPPTTIIOONN"")) }}}}
 ((""MMOODDUULLEE""))))..rrssttrriipp((""::""))..uuppppeerr(()) }}}}
 {{ module.name }}                  {{ module.description|convert_markdown
                                    (heading_level, html_id) }}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {{ log.debug("Rendering other parameters section") }}
 
 {% import "language.html" as lang with context %}
 
 {% if config.docstring_section_style == "table" %}
-  {% block table_style %}
+  {% block table_style scoped %}
   <p><strong>{{ section.title or lang.t("Other Parameters:") }}</strong></p>
   <table>
     <thead>
       <tr>
         <th>{{ lang.t("Name") }}</th>
         <th>{{ lang.t("Type") }}</th>
         <th>{{ lang.t("Description") }}</th>
@@ -31,15 +31,15 @@
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
-  {% block list_style %}
+  {% block list_style scoped %}
   <p>{{ section.title or lang.t("Other Parameters:") }}</p>
   <ul>
     {% for parameter in section.value %}
       <li class="field-body">
         <b><code>{{ parameter.name }}</code></b>
         {% if parameter.annotation %}
           {% with expression = parameter.annotation %}
@@ -51,15 +51,15 @@
           {{ parameter.description|convert_markdown(heading_level, html_id) }}
         </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
-  {% block spacy_style %}
+  {% block spacy_style scoped %}
   <table>
     <thead>
       <tr>
         <th><b>{{ (section.title or lang.t("PARAMETER")).rstrip(":").upper() }}</b></th>
         <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
 {{ log.debug("Rendering other parameters section") }} {% import "language.html"
 as lang with context %} {% if config.docstring_section_style == "table" %} {%
-block table_style %}
+block table_style scoped %}
 {{{{ sseeccttiioonn..ttiittllee oorr llaanngg..tt((""OOtthheerr PPaarraammeetteerrss::"")) }}}}
 {{{{ llaanngg..tt((""NNaammee"")) {{{{ llaanngg..tt((""TTyyppee"")) }}}} {{{{ llaanngg..tt((""DDeessccrriippttiioonn"")) }}}}
 }}}}
                   {% if
                   parameter.annotation
                   %} {% with
                   expression =         {
 {{ parameter.name parameter.annotation {
 }}                %} {% include        parameter.description|convert_markdown
                   "expression.html"    (heading_level, html_id) }}
                   with context %} {%
                   endwith %} {% endif
                   %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
-{% block list_style %}
+{% block list_style scoped %}
 {{ section.title or lang.t("Other Parameters:") }}
     * {% for parameter in section.value %}
     * {{{{ ppaarraammeetteerr..nnaammee }}}} {% if parameter.annotation %} {% with expression =
       parameter.annotation %} ({% include "expression.html" with context %}) {%
       endwith %} {% endif %} â
       {{ parameter.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
-{% block spacy_style %}
+{% block spacy_style scoped %}
 {{{{ ((sseeccttiioonn..ttiittllee oorr llaanngg..tt           {{{{ llaanngg..tt((""DDEESSCCRRIIPPTTIIOONN"")) }}}}
 ((""PPAARRAAMMEETTEERR""))))..rrssttrriipp((""::""))..uuppppeerr(()) }}}}
                                       {{ parameter.description|convert_markdown
                                       (heading_level, html_id) }}
                                       {% if parameter.annotation %} {{{{ llaanngg..tt
 {{ parameter.name }}                  ((""TTYYPPEE::"")) }}}} {% with expression =
                                       parameter.annotation %} {% include
```

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {{ log.debug("Rendering parameters section") }}
 
 {% import "language.html" as lang with context %}
 
 {% if config.docstring_section_style == "table" %}
-  {% block table_style %}
+  {% block table_style scoped %}
   <p><strong>{{ section.title or lang.t("Parameters:") }}</strong></p>
   <table>
     <thead>
       <tr>
         <th>{{ lang.t("Name") }}</th>
         <th>{{ lang.t("Type") }}</th>
         <th>{{ lang.t("Description") }}</th>
@@ -41,15 +41,15 @@
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
-  {% block list_style %}
+  {% block list_style scoped %}
   <p>{{ section.title or lang.t("Parameters:") }}</p>
   <ul>
     {% for parameter in section.value %}
       <li class="field-body">
         <b><code>{{ parameter.name }}</code></b>
         {% if parameter.annotation %}
           {% with expression = parameter.annotation %}
@@ -66,15 +66,15 @@
           {{ parameter.description|convert_markdown(heading_level, html_id) }}
         </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
-  {% block spacy_style %}
+  {% block spacy_style scoped %}
   <table>
     <thead>
       <tr>
         <th><b>{{ (section.title or lang.t("PARAMETER")).rstrip(":").upper() }}</b></th>
         <th><b> {{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {{ log.debug("Rendering parameters section") }} {% import "language.html" as
 lang with context %} {% if config.docstring_section_style == "table" %} {%
-block table_style %}
+block table_style scoped %}
 {{{{ sseeccttiioonn..ttiittllee oorr llaanngg..tt((""PPaarraammeetteerrss::"")) }}}}
 {{{{ llaanngg..tt      {{{{ llaanngg..tt((""TTyyppee"")) }}}} {{{{ llaanngg..tt((""DDeessccrriippttiioonn"")) }}}}            {{{{ llaanngg..tt
 ((""NNaammee"")) }}}}                                                                ((""DDeeffaauulltt"")) }}}}
                                                                            {% if
                {% if                                                       parameter.default
                parameter.annotation                                        %} {% with
                %} {% with                                                  expression =
@@ -13,26 +13,26 @@
 parameter.name %} {% include        parameter.description|convert_markdown "expression.html"
 }}             "expression.html"    (heading_level, html_id) }}            with context %}
                with context %} {%                                          {% endwith %} {%
                endwith %} {% endif                                         else %} {{{{ llaanngg..tt
                %}                                                          ((""rreeqquuiirreedd"")) }}}}
                                                                            {% endif %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
-{% block list_style %}
+{% block list_style scoped %}
 {{ section.title or lang.t("Parameters:") }}
     * {% for parameter in section.value %}
     * {{{{ ppaarraammeetteerr..nnaammee }}}} {% if parameter.annotation %} {% with expression =
       parameter.annotation %} ({% include "expression.html" with context %} {%-
       if parameter.default %}, {{ lang.t("default:") }} {% with expression =
       parameter.default %} {% include "expression.html" with context %} {%
       endwith %} {% endif %}) {% endwith %} {% endif %} â
       {{ parameter.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
-{% block spacy_style %}
+{% block spacy_style scoped %}
 {{{{ ((sseeccttiioonn..ttiittllee oorr llaanngg..tt           {{{{ llaanngg..tt((""DDEESSCCRRIIPPTTIIOONN"")) }}}}
 ((""PPAARRAAMMEETTEERR""))))..rrssttrriipp((""::""))..uuppppeerr(()) }}}}
                                       {{ parameter.description|convert_markdown
                                       (heading_level, html_id) }}
                                       {% if parameter.annotation %} {{{{ llaanngg..tt
                                       ((""TTYYPPEE::"")) }}}} {% with expression =
                                       parameter.annotation %} {% include
```

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {{ log.debug("Rendering raises section") }}
 
 {% import "language.html" as lang with context %}
 
 {% if config.docstring_section_style == "table" %}
-  {% block table_style %}
+  {% block table_style scoped %}
   <p><strong>{{ section.title or lang.t("Raises:") }}</strong></p>
   <table>
     <thead>
       <tr>
         <th>{{ lang.t("Type") }}</th>
         <th>{{ lang.t("Description") }}</th>
       </tr>
@@ -29,15 +29,15 @@
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
-  {% block list_style %}
+  {% block list_style scoped %}
   <p>{{ lang.t(section.title) or lang.t("Raises:") }}</p>
   <ul>
     {% for raises in section.value %}
       <li class="field-body">
         {% if raises.annotation %}
           {% with expression = raises.annotation %}
             <code>{% include "expression.html" with context %}</code>
@@ -48,15 +48,15 @@
           {{ raises.description|convert_markdown(heading_level, html_id) }}
         </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
-  {% block spacy_style %}
+  {% block spacy_style scoped %}
   <table>
     <thead>
       <tr>
         <th><b>{{ (section.title or lang.t("RAISES")).rstrip(":").upper() }}</b></th>
         <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
 {{ log.debug("Rendering raises section") }} {% import "language.html" as lang
 with context %} {% if config.docstring_section_style == "table" %} {% block
-table_style %}
+table_style scoped %}
 {{{{ sseeccttiioonn..ttiittllee oorr llaanngg..tt((""RRaaiisseess::"")) }}}}
 {{{{ llaanngg..tt((""TTyyppee"")) }}}}                   {{{{ llaanngg..tt((""DDeessccrriippttiioonn"")) }}}}
 {% if raises.annotation %} {% with
 expression = raises.annotation %} {%   {{ raises.description|convert_markdown
 include "expression.html" with context (heading_level, html_id) }}
 %} {% endwith %} {% endif %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
-{% block list_style %}
+{% block list_style scoped %}
 {{ lang.t(section.title) or lang.t("Raises:") }}
     * {% for raises in section.value %}
     * {% if raises.annotation %} {% with expression = raises.annotation %} {%
       include "expression.html" with context %} {% endwith %} â {% endif %}
       {{ raises.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
-{% block spacy_style %}
+{% block spacy_style scoped %}
 {{{{ ((sseeccttiioonn..ttiittllee oorr llaanngg..tt            {{{{ llaanngg..tt((""DDEESSCCRRIIPPTTIIOONN"")) }}}}
 ((""RRAAIISSEESS""))))..rrssttrriipp((""::""))..uuppppeerr(()) }}}}
 {% with expression = raises.annotation {{ raises.description|convert_markdown
 %} {% include "expression.html" with   (heading_level, html_id) }}
 context %} {% endwith %}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {{ log.debug("Rendering receives section") }}
 
 {% import "language.html" as lang with context %}
 
 {% if config.docstring_section_style == "table" %}
-  {% block table_style %}
+  {% block table_style scoped %}
   {% set name_column = section.value|selectattr("name")|any %}
   <p><strong>{{ section.title or lang.t("Receives:") }}</strong></p>
   <table>
     <thead>
       <tr>
         {% if name_column %}<th>{{ lang.t("Name") }}</th>{% endif %}
         <th>{{ lang.t("Type") }}</th>
@@ -32,15 +32,15 @@
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
-  {% block list_style %}
+  {% block list_style scoped %}
   <p>{{ section.title or lang.t("Receives:") }}</p>
   <ul>
     {% for receives in section.value %}
       <li class="field-body">
         {% if receives.name %}<b><code>{{ receives.name }}</code></b>{% endif %}
         {% if receives.annotation %}
           {% with expression = receives.annotation %}
@@ -54,15 +54,15 @@
           {{ receives.description|convert_markdown(heading_level, html_id) }}
         </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
-  {% block spacy_style %}
+  {% block spacy_style scoped %}
   <table>
     <thead>
       <tr>
         <th><b>{{ (section.title or lang.t("RECEIVES")).rstrip(":").upper() }}</b></th>
         <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
 {{ log.debug("Rendering receives section") }} {% import "language.html" as lang
 with context %} {% if config.docstring_section_style == "table" %} {% block
-table_style %} {% set name_column = section.value|selectattr("name")|any %}
+table_style scoped %} {% set name_column = section.value|selectattr("name")|any
+%}
 {{{{ sseeccttiioonn..ttiittllee oorr llaanngg..tt((""RReecceeiivveess::"")) }}}}
 {{{{ llaanngg..tt((""NNaammee"")) }}}} {{{{ llaanngg..tt((""TTyyppee"")) }}}} {{{{ llaanngg..tt((""DDeessccrriippttiioonn"")) }}}}
                      {% if
                      receives.annotation
                      %} {% with
 {% if receives.name  expression =         {
 %}{{ receives.name   receives.annotation  {
 }}{% endif %}        %} {% include        receives.description|convert_markdown
                      "expression.html"    (heading_level, html_id) }}
                      with context %} {%
                      endwith %} {% endif
                      %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
-{% block list_style %}
+{% block list_style scoped %}
 {{ section.title or lang.t("Receives:") }}
     * {% for receives in section.value %}
     * {% if receives.name %}{{{{ rreecceeiivveess..nnaammee }}}}{% endif %} {% if
       receives.annotation %} {% with expression = receives.annotation %} {% if
       receives.name %} ({% endif %} {% include "expression.html" with context
       %} {% if receives.name %}){% endif %} {% endwith %} {% endif %} â
       {{ receives.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
-{% block spacy_style %}
+{% block spacy_style scoped %}
 {{{{ ((sseeccttiioonn..ttiittllee oorr llaanngg..tt             {{{{ llaanngg..tt((""DDEESSCCRRIIPPTTIIOONN"")) }}}}
 ((""RREECCEEIIVVEESS""))))..rrssttrriipp((""::""))..uuppppeerr(()) }}}}
                                         {
                                         { receives.description|convert_markdown
 {% if receives.name %} {{ receives.name (heading_level, html_id) }}
 }} {% elif receives.annotation %} {%    {% if receives.name and
 with expression = receives.annotation   receives.annotation %}
```

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {{ log.debug("Rendering returns section") }}
 
 {% import "language.html" as lang with context %}
 
 {% if config.docstring_section_style == "table" %}
-  {% block table_style %}
+  {% block table_style scoped %}
   {% set name_column = section.value|selectattr("name")|any %}
   <p><strong>{{ section.title or lang.t("Returns:") }}</strong></p>
   <table>
     <thead>
       <tr>
         {% if name_column %}<th>{{ lang.t("Name") }}</th>{% endif %}
         <th>{{ lang.t("Type") }}</th>
@@ -32,15 +32,15 @@
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
-  {% block list_style %}
+  {% block list_style scoped %}
   <p>{{ section.title or lang.t("Returns:") }}</p>
   <ul>
     {% for returns in section.value %}
       <li class="field-body">
         {% if returns.name %}<b><code>{{ returns.name }}</code></b>{% endif %}
         {% if returns.annotation %}
           {% with expression = returns.annotation %}
@@ -54,15 +54,15 @@
           {{ returns.description|convert_markdown(heading_level, html_id) }}
       </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
-  {% block spacy_style %}
+  {% block spacy_style scoped %}
   <table>
     <thead>
       <tr>
         <th><b>{{ (section.title or lang.t("RETURNS")).rstrip(":").upper() }}</b></th>
         <th><b>{{ lang.t("DESCRIPTION").upper() }}</b></th>
       </tr>
     </thead>
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
 {{ log.debug("Rendering returns section") }} {% import "language.html" as lang
 with context %} {% if config.docstring_section_style == "table" %} {% block
-table_style %} {% set name_column = section.value|selectattr("name")|any %}
+table_style scoped %} {% set name_column = section.value|selectattr("name")|any
+%}
 {{{{ sseeccttiioonn..ttiittllee oorr llaanngg..tt((""RReettuurrnnss::"")) }}}}
 {{{{ llaanngg..tt((""NNaammee"")) }}}} {{{{ llaanngg..tt((""TTyyppee"")) }}}}  {{{{ llaanngg..tt((""DDeessccrriippttiioonn"")) }}}}
                      {% if
                      returns.annotation %}
                      {% with expression =  {
 {% if returns.name   returns.annotation %} {
 %}{{ returns.name }} {% include            returns.description|convert_markdown
 {% endif %}          "expression.html"     (heading_level, html_id) }}
                      with context %} {%
                      endwith %} {% endif
                      %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
-{% block list_style %}
+{% block list_style scoped %}
 {{ section.title or lang.t("Returns:") }}
     * {% for returns in section.value %}
     * {% if returns.name %}{{{{ rreettuurrnnss..nnaammee }}}}{% endif %} {% if
       returns.annotation %} {% with expression = returns.annotation %} {% if
       returns.name %} ({% endif %} {% include "expression.html" with context %}
       {% if returns.name %}){% endif %} {% endwith %} {% endif %} â
       {{ returns.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
-{% block spacy_style %}
+{% block spacy_style scoped %}
 {{{{ ((sseeccttiioonn..ttiittllee oorr llaanngg..tt             {{{{ llaanngg..tt((""DDEESSCCRRIIPPTTIIOONN""))..uuppppeerr(()) }}}}
 ((""RREETTUURRNNSS""))))..rrssttrriipp((""::""))..uuppppeerr(()) }}}}
                                         {{ returns.description|convert_markdown
                                         (heading_level, html_id) }}
 {% if returns.name %} {{ returns.name   {% if returns.name and
 }} {% elif returns.annotation %} {%     returns.annotation %}
 with expression = returns.annotation %} {{{{ llaanngg..tt((""TTYYPPEE::"")) }}}} {% with
```

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {{ log.debug("Rendering warns section") }}
 
 {% import "language.html" as lang with context %}
 
 {% if config.docstring_section_style == "table" %}
-  {% block table_style %}
+  {% block table_style scoped %}
   <p><strong>{{ section.title or lang.t("Warns:") }}</strong></p>
   <table>
     <thead>
       <tr>
         <th>{{ lang.t("Type") }}</th>
         <th>{{ lang.t("Description") }}</th>
       </tr>
@@ -29,15 +29,15 @@
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
-  {% block list_style %}
+  {% block list_style scoped %}
   <p>{{ section.title or lang.t("Warns:") }}</p>
   <ul>
     {% for warns in section.value %}
       <li class="field-body">
         {% if warns.annotation %}
           {% with expression = warns.annotation %}
             <code>{% include "expression.html" with context %}</code>
@@ -48,15 +48,15 @@
           {{ warns.description|convert_markdown(heading_level, html_id) }}
         </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
-  {% block spacy_style %}
+  {% block spacy_style scoped %}
   <table>
     <thead>
       <tr>
         <th><b>{{ (section.title or lang.t("WARNS")).rstrip(":").upper() }}</b></th>
         <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
 {{ log.debug("Rendering warns section") }} {% import "language.html" as lang
 with context %} {% if config.docstring_section_style == "table" %} {% block
-table_style %}
+table_style scoped %}
 {{{{ sseeccttiioonn..ttiittllee oorr llaanngg..tt((""WWaarrnnss::"")) }}}}
 {{{{ llaanngg..tt((""TTyyppee"")) }}}}                      {{{{ llaanngg..tt((""DDeessccrriippttiioonn"")) }}}}
 {% if warns.annotation %} {% with
 expression = warns.annotation %} {%       {{ warns.description|convert_markdown
 include "expression.html" with context %} (heading_level, html_id) }}
 {% endwith %} {% endif %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
-{% block list_style %}
+{% block list_style scoped %}
 {{ section.title or lang.t("Warns:") }}
     * {% for warns in section.value %}
     * {% if warns.annotation %} {% with expression = warns.annotation %} {%
       include "expression.html" with context %} {% endwith %} â {% endif %}
       {{ warns.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
-{% block spacy_style %}
+{% block spacy_style scoped %}
 {{{{ ((sseeccttiioonn..ttiittllee oorr llaanngg..tt               {{{{ llaanngg..tt((""DDEESSCCRRIIPPTTIIOONN"")) }}}}
 ((""WWAARRNNSS""))))..rrssttrriipp((""::""))..uuppppeerr(()) }}}}
 {% with expression = warns.annotation %}  {{ warns.description|convert_markdown
 {% include "expression.html" with context (heading_level, html_id) }}
 %} {% endwith %}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {{ log.debug("Rendering yields section") }}
 
 {% import "language.html" as lang with context %}
 
 {% if config.docstring_section_style == "table" %}
-  {% block table_style %}
+  {% block table_style scoped %}
   {% set name_column = section.value|selectattr("name")|any %}
   <p><strong>{{ section.title or lang.t("Yields:") }}</strong></p>
   <table>
     <thead>
       <tr>
         {% if name_column %}<th>{{ lang.t("Name") }}</th>{% endif %}
         <th>{{ lang.t("Type") }}</th>
@@ -32,15 +32,15 @@
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
-  {% block list_style %}
+  {% block list_style scoped %}
   <p>{{ section.title or lang.t("Yields:") }}</p>
   <ul>
     {% for yields in section.value %}
       <li class="field-body">
         {% if yields.name %}<b><code>{{ yields.name }}</code></b>{% endif %}
         {% if yields.annotation %}
           {% with expression = yields.annotation %}
@@ -54,15 +54,15 @@
           {{ yields.description|convert_markdown(heading_level, html_id) }}
         </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
-  {% block spacy_style %}
+  {% block spacy_style scoped %}
   <table>
     <thead>
       <tr>
         <th><b>{{ (section.title or lang.t("YIELDS")).rstrip(":").upper() }}</b></th>
         <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
 {{ log.debug("Rendering yields section") }} {% import "language.html" as lang
 with context %} {% if config.docstring_section_style == "table" %} {% block
-table_style %} {% set name_column = section.value|selectattr("name")|any %}
+table_style scoped %} {% set name_column = section.value|selectattr("name")|any
+%}
 {{{{ sseeccttiioonn..ttiittllee oorr llaanngg..tt((""YYiieellddss::"")) }}}}
 {{{{ llaanngg..tt((""NNaammee"")) }}}}  {{{{ llaanngg..tt((""TTyyppee"")) }}}}  {{{{ llaanngg..tt((""DDeessccrriippttiioonn"")) }}}}
                       {% if
                       yields.annotation %}
                       {% with expression =  {
 {% if yields.name %}{ yields.annotation %}  {
 { yields.name }}{%    {% include            yields.description|convert_markdown
 endif %}              "expression.html"     (heading_level, html_id) }}
                       with context %} {%
                       endwith %} {% endif
                       %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
-{% block list_style %}
+{% block list_style scoped %}
 {{ section.title or lang.t("Yields:") }}
     * {% for yields in section.value %}
     * {% if yields.name %}{{{{ yyiieellddss..nnaammee }}}}{% endif %} {% if yields.annotation
       %} {% with expression = yields.annotation %} {% if yields.name %} ({%
       endif %} {% include "expression.html" with context %} {% if yields.name
       %}){% endif %} {% endwith %} {% endif %} â
       {{ yields.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
-{% block spacy_style %}
+{% block spacy_style scoped %}
 {{{{ ((sseeccttiioonn..ttiittllee oorr llaanngg..tt             {{{{ llaanngg..tt((""DDEESSCCRRIIPPTTIIOONN"")) }}}}
 ((""YYIIEELLDDSS""))))..rrssttrriipp((""::""))..uuppppeerr(()) }}}}
                                         {{ yields.description|convert_markdown
                                         (heading_level, html_id) }}
 {% if yields.name %} {{ yields.name }}  {% if yields.name and yields.annotation
 {% elif yields.annotation %} {% with    %}
 expression = yields.annotation %} {%    {{{{ llaanngg..tt((""TTYYPPEE::"")) }}}}:: {% with
```

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/en.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/en.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/ja.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/ja.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/zh.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/zh.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/material/style.css` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/material/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/en.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/en.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/ja.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/ja.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/zh.html` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/zh.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css` & `mkdocstrings_python-1.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/tests/conftest.py` & `mkdocstrings_python-1.9.0/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,41 +56,41 @@
 
 
 @pytest.fixture(name="plugin")
 def fixture_plugin(mkdocs_conf: config.Config) -> MkdocstringsPlugin:
     """Return a plugin instance.
 
     Parameters:
-        mkdocs_conf: Pytest fixture: [tests.conftest.fixture_mkdocs_conf][].
+        mkdocs_conf: Pytest fixture (see conftest.py).
 
     Returns:
         mkdocstrings plugin instance.
     """
     return mkdocs_conf["plugins"]["mkdocstrings"]
 
 
 @pytest.fixture(name="ext_markdown")
 def fixture_ext_markdown(mkdocs_conf: config.Config) -> Markdown:
     """Return a Markdown instance with MkdocstringsExtension.
 
     Parameters:
-        mkdocs_conf: Pytest fixture: [tests.conftest.fixture_mkdocs_conf][].
+        mkdocs_conf: Pytest fixture (see conftest.py).
 
     Returns:
         A Markdown instance.
     """
     return Markdown(extensions=mkdocs_conf["markdown_extensions"], extension_configs=mkdocs_conf["mdx_configs"])
 
 
 @pytest.fixture(name="handler")
 def fixture_handler(plugin: MkdocstringsPlugin, ext_markdown: Markdown) -> PythonHandler:
     """Return a handler instance.
 
     Parameters:
-        plugin: Pytest fixture: [tests.conftest.fixture_plugin][].
+        plugin: Pytest fixture (see conftest.py).
 
     Returns:
         A handler instance.
     """
     handler = plugin.handlers.get_handler("python")
     handler._update_env(ext_markdown, plugin.handlers._config)
     return handler  # type: ignore[return-value]
```

### Comparing `mkdocstrings_python-1.8.0/tests/test_handler.py` & `mkdocstrings_python-1.9.0/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/tests/test_rendering.py` & `mkdocstrings_python-1.9.0/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.8.0/tests/test_themes.py` & `mkdocstrings_python-1.9.0/tests/test_themes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Tests for the different themes we claim to support."""
 
 from __future__ import annotations
 
-import sys
 from typing import TYPE_CHECKING
 
 import pytest
 
 if TYPE_CHECKING:
     from markdown import Markdown
     from mkdocstrings.plugin import MkdocstringsPlugin
@@ -18,30 +17,30 @@
         {"theme": "mkdocs"},
         {"theme": "readthedocs"},
         {"theme": {"name": "material"}},
     ],
     indirect=["plugin"],
 )
 @pytest.mark.parametrize(
-    "module",
+    "identifier",
     [
         "mkdocstrings.extension",
         "mkdocstrings.inventory",
         "mkdocstrings.loggers",
         "mkdocstrings.plugin",
         "mkdocstrings.handlers.base",
         "mkdocstrings.handlers.rendering",
         "mkdocstrings_handlers.python",
     ],
 )
-@pytest.mark.skipif(sys.version_info < (3, 7), reason="material is not installed on Python 3.6")
-def test_render_themes_templates_python(module: str, plugin: MkdocstringsPlugin, ext_markdown: Markdown) -> None:
+def test_render_themes_templates_python(identifier: str, plugin: MkdocstringsPlugin, ext_markdown: Markdown) -> None:
     """Test rendering of a given theme's templates.
 
     Parameters:
-        module: Parametrized argument.
-        plugin: Pytest fixture: [tests.conftest.fixture_plugin][].
+        identifier: Parametrized identifier.
+        plugin: Pytest fixture (see conftest.py).
+        ext_markdown: Pytest fixture (see conftest.py).
     """
     handler = plugin.handlers.get_handler("python")
     handler._update_env(ext_markdown, plugin.handlers._config)
-    data = handler.collect(module, {})
+    data = handler.collect(identifier, {})
     handler.render(data, {})
```

### Comparing `mkdocstrings_python-1.8.0/PKG-INFO` & `mkdocstrings_python-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,50 @@
 Metadata-Version: 2.1
 Name: mkdocstrings-python
-Version: 1.8.0
+Version: 1.9.0
 Summary: A Python handler for mkdocstrings.
-Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
+Author-Email: Timothée Mazzucotelli <dev@pawamoy.fr>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Project-URL: Homepage, https://mkdocstrings.github.io/python
 Project-URL: Documentation, https://mkdocstrings.github.io/python
 Project-URL: Changelog, https://mkdocstrings.github.io/python/changelog
 Project-URL: Repository, https://github.com/mkdocstrings/python
 Project-URL: Issues, https://github.com/mkdocstrings/python/issues
 Project-URL: Discussions, https://github.com/mkdocstrings/python/discussions
 Project-URL: Gitter, https://gitter.im/mkdocstrings/python
 Project-URL: Funding, https://github.com/sponsors/pawamoy
 Requires-Python: >=3.8
+Requires-Dist: markdown<3.6,>=3.3
 Requires-Dist: mkdocstrings>=0.20
 Requires-Dist: griffe>=0.37
 Description-Content-Type: text/markdown
 
 <h1 align="center">mkdocstrings-python</h1>
 
 <p align="center">A Python handler for <a href="https://github.com/mkdocstrings/mkdocstrings"><i>mkdocstrings</i></a>.</p>
 
-<p align="center">
-  <a href="https://github.com/mkdocstrings/python/actions?query=workflow%3Aci">
-    <img alt="ci" src="https://github.com/mkdocstrings/python/workflows/ci/badge.svg" />
-  </a>
-  <a href="https://mkdocstrings.github.io/python/">
-    <img alt="documentation" src="https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat" />
-  </a>
-  <a href="https://pypi.org/project/mkdocstrings-python/">
-    <img alt="pypi version" src="https://img.shields.io/pypi/v/mkdocstrings-python.svg" />
-  </a>
-  <a href="https://gitpod.io/#https://github.com/mkdocstrings/python">
-    <img alt="gitpod" src="https://img.shields.io/badge/gitpod-workspace-blue.svg?style=flat" />
-  </a>
-  <a href="https://app.gitter.im/#/room/#mkdocstrings_python:gitter.im">
-    <img alt="gitter" src="https://badges.gitter.im/join%20chat.svg" />
-  </a>
-</p>
+[![ci](https://github.com/mkdocstrings/python/workflows/ci/badge.svg)](https://github.com/mkdocstrings/python/actions?query=workflow%3Aci)
+[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://mkdocstrings.github.io/python/)
+[![pypi version](https://img.shields.io/pypi/v/mkdocstrings-python.svg)](https://pypi.org/project/mkdocstrings-python/)
+[![gitpod](https://img.shields.io/badge/gitpod-workspace-blue.svg?style=flat)](https://gitpod.io/#https://github.com/mkdocstrings/python)
+[![gitter](https://badges.gitter.im/join%20chat.svg)](https://app.gitter.im/#/room/#python:gitter.im)
 
 ---
 
 <p align="center"><img src="logo.png"></p>
 
 The Python handler uses [Griffe](https://mkdocstrings.github.io/griffe)
 to collect documentation from Python source code.
```

#### html2text {}

```diff
@@ -1,32 +1,39 @@
-Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.8.0 Summary: A
+Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.9.0 Summary: A
 Python handler for mkdocstrings. Author-Email: TimothÃ©e Mazzucotelli
-pm.me> License: ISC Classifier: Development Status :: 4 - Beta Classifier:
+pawamoy.fr> License: ISC Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Documentation Classifier: Topic :: Software Development Classifier: Topic ::
-Software Development :: Documentation Classifier: Topic :: Utilities
-Classifier: Typing :: Typed Project-URL: Homepage, https://
+Utilities Classifier: Typing :: Typed Project-URL: Homepage, https://
 mkdocstrings.github.io/python Project-URL: Documentation, https://
 mkdocstrings.github.io/python Project-URL: Changelog, https://
 mkdocstrings.github.io/python/changelog Project-URL: Repository, https://
 github.com/mkdocstrings/python Project-URL: Issues, https://github.com/
 mkdocstrings/python/issues Project-URL: Discussions, https://github.com/
 mkdocstrings/python/discussions Project-URL: Gitter, https://gitter.im/
 mkdocstrings/python Project-URL: Funding, https://github.com/sponsors/pawamoy
-Requires-Python: >=3.8 Requires-Dist: mkdocstrings>=0.20 Requires-Dist:
-griffe>=0.37 Description-Content-Type: text/markdown
+Requires-Python: >=3.8 Requires-Dist: markdown<3.6,>=3.3 Requires-Dist:
+mkdocstrings>=0.20 Requires-Dist: griffe>=0.37 Description-Content-Type: text/
+markdown
                        ************ mmkkddooccssttrriinnggss--ppyytthhoonn ************
                       A Python handler for _m_k_d_o_c_s_t_r_i_n_g_s.
-               _[_c_i_]_[_d_o_c_u_m_e_n_t_a_t_i_o_n_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_g_i_t_p_o_d_]_[_g_i_t_t_e_r_]
----
+[![ci](https://github.com/mkdocstrings/python/workflows/ci/badge.svg)](https://
+github.com/mkdocstrings/python/actions?query=workflow%3Aci) [![documentation]
+(https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)]
+(https://mkdocstrings.github.io/python/) [![pypi version](https://
+img.shields.io/pypi/v/mkdocstrings-python.svg)](https://pypi.org/project/
+mkdocstrings-python/) [![gitpod](https://img.shields.io/badge/gitpod-workspace-
+blue.svg?style=flat)](https://gitpod.io/#https://github.com/mkdocstrings/
+python) [![gitter](https://badges.gitter.im/join%20chat.svg)](https://
+app.gitter.im/#/room/#python:gitter.im) ---
                                   [logo.png]
 The Python handler uses [Griffe](https://mkdocstrings.github.io/griffe) to
 collect documentation from Python source code. The word "griffe" can sometimes
 be used instead of "signature" in French. Griffe is able to visit the Abstract
 Syntax Tree (AST) of the source code to extract useful information. It is also
 able to execute the code (by importing it) and introspect objects in memory
 when source code is not available. Finally, it can parse docstrings following
```

