# Comparing `tmp/pyshared-1.4.0-py3-none-any.whl.zip` & `tmp/pyshared-1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 10593 bytes, number of entries: 15
+Zip file size: 11020 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      390 b- defN 24-Mar-31 21:28 pyshared/__init__.py
 -rw-r--r--  2.0 unx      124 b- defN 24-Jan-11 01:53 pyshared/consts.py
 -rw-r--r--  2.0 unx     1293 b- defN 24-Jan-12 03:28 pyshared/crypto.py
--rw-r--r--  2.0 unx     1630 b- defN 24-Jan-11 05:55 pyshared/env.py
+-rw-r--r--  2.0 unx     1938 b- defN 24-Apr-02 21:41 pyshared/env.py
 -rw-r--r--  2.0 unx      943 b- defN 24-Mar-31 21:02 pyshared/exceptions.py
 -rw-r--r--  2.0 unx      914 b- defN 24-Mar-31 21:30 pyshared/pytest.py
 -rw-r--r--  2.0 unx     4740 b- defN 24-Mar-31 21:11 pyshared/python.py
 -rw-r--r--  2.0 unx      790 b- defN 24-Jan-11 05:57 pyshared/shell.py
 -rw-r--r--  2.0 unx     2083 b- defN 24-Jan-12 03:45 pyshared/terminal.py
--rw-r--r--  2.0 unx       22 b- defN 24-Mar-31 21:20 pyshared/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Mar-31 21:32 pyshared-1.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5371 b- defN 24-Mar-31 21:32 pyshared-1.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-31 21:32 pyshared-1.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Mar-31 21:32 pyshared-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1138 b- defN 24-Mar-31 21:32 pyshared-1.4.0.dist-info/RECORD
-15 files, 20607 bytes uncompressed, 8733 bytes compressed:  57.6%
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-02 21:44 pyshared/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-02 21:48 pyshared-1.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6307 b- defN 24-Apr-02 21:48 pyshared-1.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 21:48 pyshared-1.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-02 21:48 pyshared-1.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1138 b- defN 24-Apr-02 21:48 pyshared-1.5.0.dist-info/RECORD
+15 files, 21851 bytes uncompressed, 9160 bytes compressed:  58.1%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pyshared/terminal.py
 Comment: 
 
 Filename: pyshared/version.py
 Comment: 
 
-Filename: pyshared-1.4.0.dist-info/LICENSE
+Filename: pyshared-1.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: pyshared-1.4.0.dist-info/METADATA
+Filename: pyshared-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: pyshared-1.4.0.dist-info/WHEEL
+Filename: pyshared-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyshared-1.4.0.dist-info/top_level.txt
+Filename: pyshared-1.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyshared-1.4.0.dist-info/RECORD
+Filename: pyshared-1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyshared/env.py

```diff
@@ -1,56 +1,60 @@
 import os
-import typing as TYPE
+from typing import Union as U, Optional as Opt, Any as A
 
 
-def typed_evar(name: str, default: TYPE.Optional[TYPE.Any] = None):
+def typed_evar(
+    name: str, default: Opt[A] = None, vartype: U[type, A] = None
+) -> A:
     """Return an environment variable with an assumed type. Type from
     the default value, if provided, will be prioritized, otherwise
     the type will be inferred in order of: bool, int, float, str.
+    ~name (str): the environment variable name
+    ?default (Any): the default value if the environment variable is not set
+    ?vartype (type): override type assumption to attempt to cast to this type
 
     (CURDAY, 25) -> 25
     (CURDAY, 25.0) -> 25.0
     (CURDAY, '25.0') -> '25.0'
     (CURDAY, None) -> '25'
+    (CURDAY, None, int) -> 25
+    (CURDAY, None, float) -> 25.0
+    (CURDAY, None, bool) -> True
+    (CURDAY, None, Decimal) -> Decimal('25')
 
-    Args:
-        name (str): The name of the environment variable.
-        default (Optional[Any]): The default value of the environment variable.
-            Defaults to None.
-    Returns:
-        Any: The env var value with the assumed type.
     """
     varval = os.environ.get(name)
     if varval is None:
         return default
 
-    # use default's type
-    if default is not None:
-        vartype = type(default)
-
-        # bool gets special treatment
-        if vartype is bool:
-            if varval.lower() in ('1', 'true'):
+    if vartype is not None:
+        return vartype(varval)
+
+    _true = ('1', 'true', 'yes', 'on')
+    _false = ('0', 'false', 'no', 'off')
+
+    deftype = type(default) if default is not None else None
+    if deftype is not None:
+        if deftype is bool:
+            if varval.lower() in _true:
                 return True
-            elif varval.lower() in ('0', 'false', '-1'):
+            elif varval.lower() in _false:
                 return False
-            else:
-                raise ValueError(
-                    "Invalid boolean value for environment variable %s: %s"
-                    % (name, varval)
-                )
-        try:
-            return vartype(varval)
-        except Exception:
-            pass
+            raise ValueError('Invalid boolean value: %s' % varval)
+        return deftype(varval)
 
-    # otherwise assume type using a few simple types
-    if varval.casefold() in ('true', 'false'):
-        return varval.casefold() == 'true'
+    casevar = varval.casefold()
 
-    for vartype in (int, float):
-        try:
-            return vartype(varval)
-        except ValueError:
-            continue
+    # otherwise assume type using a few simple types
+    if casevar in ('1', 'true', 'false', '0'):
+        return True if casevar in _true else False
+    elif varval.isdigit():
+        return int(varval)
+    elif '.' in varval:
+        spval = varval.split('.')
+        if len(spval) == 2:
+            if spval[0].isdigit() and spval[1].isdigit():
+                return float(varval)
+            elif spval[0] == '' and spval[1].isdigit():
+                return float(varval)
 
-    return varval
+    return str(varval)
```

## pyshared/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.4.0'
+__version__ = '1.5.0'
```

## Comparing `pyshared-1.4.0.dist-info/LICENSE` & `pyshared-1.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyshared-1.4.0.dist-info/METADATA` & `pyshared-1.5.0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshared
-Version: 1.4.0
+Version: 1.5.0
 Summary: A Python library containing common utility functions for use across multiple codebases, filling gaps not covered by the standard Python libraries.
 Author-email: Cary Carter <ccarterdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Cary Carter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -80,48 +80,78 @@
 ### `consts.py`
 
 - `ALPHANUMERIC_CHARS`: A string of alphanumeric characters.
 - `ALPHANUMERIC_EXT_CHARS`: Alphanumeric characters, including underscores and hyphens.
 
 ### `crypto.py`
 
-- `is_jwt`: Verifies if a string is a valid JSON Web Token (JWT).
+- `is_jwt`: Simply verifies if a string looks like a JSON Web Token (JWT)
 
 ### `env.py`
 
 - `typed_evar`: Retrieves and type-casts environment variables.
 
+Examples: (input, default, type, expected_output)
+
+```
+(None, 1, None, 1),
+(None, 1.0, None, 1.0),
+(None, '1', None, '1'),
+(None, None, int, None),
+(None, None, float, None),
+(None, '20.1', int, '20.1'),
+('0', None, None, 0),
+('0', True, None, False),
+('0', False, None, False),
+('0', 0, None, 0),
+('0', None, bool, True),
+('0', None, int, 0),
+('0', 1.0, float, 0.0),
+('0', None, float, 0.0),
+('0.0', None, None, 0.0),
+('0.', None, None, '0.'),
+('.0', None, None, 0.0),
+('True', None, None, True),
+('tRuE', None, None, True),
+('false', None, None, False),
+('fAlSe', None, None, False),
+('true', None, str, 'true'),
+('test', True, None, ValueError),
+('test', None, int, ValueError),
+('test', 1, None, ValueError),
+```
+
 ### `exceptions.py`
 
-- `NotPrintableError`: Indicates failures in object string representation.
+- `NotPrintableError`: Both str and repr methods raised exceptions.
 
 ### `python.py`
 
 - `ranstr`: Creates random strings of specified length and character set.
-- `safe_repr`: Safely generates a string representation of any object.
+- `safe_repr`: Safely returns the object's repr/str or an error string without throwing exceptions if the object is not printable.
 - `default_repr`: Generates a default representation for custom objects.
 - `truncstr`: Truncates a string, preserving a portion from the start and/or end.
 
 ### `pytest.py`
 
-- `multiscope_fixture`: Creates a fixture that can be used in multiple scopes.
+- `multiscope_fixture`: Creates multiple scoped pytest fixture and ensures the fixtures are available in the module.
 
 ### `shell.py`
 
 Shell command execution within Python.
 
 - `runcmd`: Executes a command in the system shell.
 
 ### `terminal.py`
 
 Terminal utilities for improved user interaction.
 
-- `get_terminal_width`: Detects the current width of the terminal.
-- `print_middle`: Centers text within the terminal width.
-- `print_columns`: Arranges a list of strings into columns fitted to the terminal width.
+- `get_terminal_width`: Safely retrieves the terminal width, defaulting to 80 columns on failure.
+- `print_middle`: Centers text within left/right padding based on terminal width.
+- `print_columns`: Arranges a list of strings into guestimated $x length strings based on what is approximately optimal for the contents/terminal width.
 
 ## Test Coverage
 
 100% lol
 
 ```
 ---------- coverage: platform darwin, python 3.9.18-final-0 ----------
```

## Comparing `pyshared-1.4.0.dist-info/RECORD` & `pyshared-1.5.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pyshared/__init__.py,sha256=pxcAmxET5NkOaqAGkD9IeVsefpTxdPYuEjj6mHcKp_E,390
 pyshared/consts.py,sha256=vfUhhaxsFGp-DnTP_iJ-ZFT_w_be6frq9VabkLzejuA,124
 pyshared/crypto.py,sha256=Ww3uT2xa7g0ewgZzvJthJQ_BRPeHM0sLZPc5c3tad2E,1293
-pyshared/env.py,sha256=-oZ0FuiCByHn2wwV8mGI5C8LIT2KbzXdStBs7tSAS0I,1630
+pyshared/env.py,sha256=ZkRtypHvFqh6cupGyvPsfPEI-bWChO499c38TqxXLQI,1938
 pyshared/exceptions.py,sha256=j7alpB6QyzZcCt9quCWPIKXmSsUw7dZPvs7fdqbYbO4,943
 pyshared/pytest.py,sha256=Sr62vEHhsVtdD6g5oUtpvW07ciYkVhjnCmMCSK_LLnA,914
 pyshared/python.py,sha256=i7gWixWO8sUNZb45afW8R0QxoMHA5S-e_cRkPmlcL1c,4740
 pyshared/shell.py,sha256=F2EJdaImnnlxeiONPlzdXcE_JZ1HUAdBWR5_i-WLfSA,790
 pyshared/terminal.py,sha256=6BjoRuUoqU7iKuXhEqU091aOiQWJUcVWXTMeUlNE3MA,2083
-pyshared/version.py,sha256=EyMGX1ADFzN6XVXHWbJUtKPONYKeFkvWoKIFPDDB2I8,22
-pyshared-1.4.0.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
-pyshared-1.4.0.dist-info/METADATA,sha256=LsKdMWO_PAvgCL6d74xoQsshrVZ1gwByy_3qxFWVcFs,5371
-pyshared-1.4.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyshared-1.4.0.dist-info/top_level.txt,sha256=ymmYDwmXcInf2QKo-75Is2v41uN5Wg_n5XnONS5UX0o,9
-pyshared-1.4.0.dist-info/RECORD,,
+pyshared/version.py,sha256=wShy9YfBfroz0HjRH_aNNehkEu1_PLsd_GjTU5aCDPk,22
+pyshared-1.5.0.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
+pyshared-1.5.0.dist-info/METADATA,sha256=xAGh0ik36ZLEo4Nu2NJmqy-Wbqs_vq_6sYv4P6kTxag,6307
+pyshared-1.5.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyshared-1.5.0.dist-info/top_level.txt,sha256=ymmYDwmXcInf2QKo-75Is2v41uN5Wg_n5XnONS5UX0o,9
+pyshared-1.5.0.dist-info/RECORD,,
```

