# Comparing `tmp/ubiquerg-0.7.0.tar.gz` & `tmp/ubiquerg-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubiquerg-0.7.0.tar", last modified: Thu Feb  1 21:09:10 2024, max compression
+gzip compressed data, was "ubiquerg-0.8.0.tar", last modified: Tue Apr  2 21:03:06 2024, max compression
```

## Comparing `ubiquerg-0.7.0.tar` & `ubiquerg-0.8.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:09:10.586997 ubiquerg-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-01 21:09:10.586997 ubiquerg-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:09:10.582996 ubiquerg-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:09:10.582996 ubiquerg-0.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-01 21:09:10.586997 ubiquerg-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:09:10.582996 ubiquerg-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/tests/test_cli_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/tests/test_packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/tests/test_query_yes_no.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/tests/test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:09:10.586997 ubiquerg-0.7.0/ubiquerg/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/ubiquerg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/ubiquerg/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/ubiquerg/cli_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/ubiquerg/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/ubiquerg/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/ubiquerg/file_locking.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/ubiquerg/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/ubiquerg/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/ubiquerg/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-01 21:09:03.000000 ubiquerg-0.7.0/ubiquerg/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:09:10.586997 ubiquerg-0.7.0/ubiquerg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-01 21:09:10.000000 ubiquerg-0.7.0/ubiquerg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-02-01 21:09:10.000000 ubiquerg-0.7.0/ubiquerg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 21:09:10.000000 ubiquerg-0.7.0/ubiquerg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-01 21:09:10.000000 ubiquerg-0.7.0/ubiquerg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:03:06.521865 ubiquerg-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-02 21:03:06.521865 ubiquerg-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:03:06.513864 ubiquerg-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:03:06.517864 ubiquerg-0.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-02 21:03:06.521865 ubiquerg-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:03:06.517864 ubiquerg-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/tests/test_cli_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/tests/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/tests/test_query_yes_no.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:03:06.517864 ubiquerg-0.8.0/ubiquerg/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/ubiquerg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/ubiquerg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/ubiquerg/cli_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/ubiquerg/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/ubiquerg/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/ubiquerg/file_locking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/ubiquerg/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/ubiquerg/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/ubiquerg/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-02 21:02:58.000000 ubiquerg-0.8.0/ubiquerg/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:03:06.521865 ubiquerg-0.8.0/ubiquerg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-02 21:03:06.000000 ubiquerg-0.8.0/ubiquerg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-02 21:03:06.000000 ubiquerg-0.8.0/ubiquerg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:03:06.000000 ubiquerg-0.8.0/ubiquerg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 21:03:06.000000 ubiquerg-0.8.0/ubiquerg.egg-info/top_level.txt
```

### Comparing `ubiquerg-0.7.0/LICENSE.txt` & `ubiquerg-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/PKG-INFO` & `ubiquerg-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiquerg
-Version: 0.7.0
+Version: 0.8.0
 Summary: Various utility functions
 Home-page: https://github.com/pepkit/ubiquerg/
 Author: Vince Reuter
 License: BSD-2-Clause
 Keywords: utility,utilities,tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ubiquerg-0.7.0/README.md` & `ubiquerg-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/docs/README.md` & `ubiquerg-0.8.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/docs/changelog.md` & `ubiquerg-0.8.0/docs/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 # Changelog
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) and [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) format. 
 
+## [0.8.0] - 2024-04-02
+### Changed
+- Expanded `mkabs` function to handle more cases
+- Allow `is_url` to work on Path objects
+- Remove `mock` test requirement in favor of importing `unittest.mock as mock`
+
 ## [0.7.0] - 2024-01-02
 
 ### Added
 - Experimental support for three-locking.
 
+
 ## [0.6.3] - 2023-08-08
 ### Fixed 
 - Incorrect read of registry path.  [Issue 35](https://github.com/pepkit/ubiquerg/issues/35)
 
 ## [0.6.2] - 2021-01-28
 
 ### Fixed
```

### Comparing `ubiquerg-0.7.0/setup.py` & `ubiquerg-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/tests/test_cli_tools.py` & `ubiquerg-0.8.0/tests/test_cli_tools.py`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/tests/test_collection.py` & `ubiquerg-0.8.0/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/tests/test_environment.py` & `ubiquerg-0.8.0/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/tests/test_files.py` & `ubiquerg-0.8.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/tests/test_packaging.py` & `ubiquerg-0.8.0/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/tests/test_paths.py` & `ubiquerg-0.8.0/tests/test_paths.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Tests for filesystem utilities """
 
 import os
 import pytest
-from ubiquerg import expandpath, parse_registry_path
+from ubiquerg import expandpath, parse_registry_path, mkabs
 
 __author__ = "Vince Reuter"
 __email__ = "vreuter@virginia.edu"
 
 
 class PathTestCase(object):
     """Bundle data and expectation with context management for a test case."""
@@ -102,7 +102,16 @@
             },
         )
     ],
 )
 def test_registry_path(registry_path, output):
     pvars = parse_registry_path(registry_path)
     assert pvars == output
+
+
+def test_mkabs():
+    relpath = "abc.txt"
+    abspath = mkabs(relpath)
+    print(f"Abspath: {abspath}")
+    assert abspath == os.path.join(os.getcwd(), relpath)
+    url = "http://example.com"
+    assert mkabs(url) == url
```

### Comparing `ubiquerg-0.7.0/tests/test_query_yes_no.py` & `ubiquerg-0.8.0/tests/test_query_yes_no.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Tests for binary user terminal interaction """
 
 import itertools
-import mock
+import unittest.mock as mock
 
 import pytest
 from ubiquerg import query_yes_no
 
 
 READ_INPUT_PATH = "ubiquerg.cli_tools._read_from_user"
```

### Comparing `ubiquerg-0.7.0/tests/test_system.py` & `ubiquerg-0.8.0/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/ubiquerg/cli_tools.py` & `ubiquerg-0.8.0/ubiquerg/cli_tools.py`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/ubiquerg/collection.py` & `ubiquerg-0.8.0/ubiquerg/collection.py`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/ubiquerg/environment.py` & `ubiquerg-0.8.0/ubiquerg/environment.py`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/ubiquerg/file_locking.py` & `ubiquerg-0.8.0/ubiquerg/file_locking.py`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/ubiquerg/files.py` & `ubiquerg-0.8.0/ubiquerg/files.py`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/ubiquerg/paths.py` & `ubiquerg-0.8.0/ubiquerg/paths.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """ Filesystem utility functions """
 
 import os
 import re
+
 from typing import List, Tuple, Any, Union
 
+from .web import is_url
+
 __author__ = "Vince Reuter"
 __email__ = "vreuter@virginia.edu"
 
 
 def expandpath(path):
     """
     Expand a filesystem path that may or may not contain user/env vars.
@@ -74,30 +77,39 @@
         defaults[2][0]: captures[2] or defaults[2][1],
         defaults[3][0]: captures[3] or defaults[3][1],
         defaults[4][0]: captures[4] or defaults[4][1],
     }
     return parsed_identifier
 
 
-def mkabs(path, reldir=None):
+def mkabs(path: str, reldir: str = None) -> str:
     """
     Makes sure a path is absolute; if not already absolute, it's made absolute
-    relative to a given directory. Also expands ~ and environment variables for
+    relative to a given directory (or file). Also expands ~ and environment variables for
     kicks.
 
     :param str path: Path to make absolute
     :param str reldir: Relative directory to make path absolute from if it's
         not already absolute
 
     :return str: Absolute path
     """
 
     def xpand(path):
         return os.path.expandvars(os.path.expanduser(path))
 
+    if path is None:
+        return path
+
+    if is_url(path):
+        return path
+
     if os.path.isabs(xpand(path)):
         return xpand(path)
 
     if not reldir:
         return os.path.abspath(xpand(path))
 
-    return os.path.join(xpand(reldir), xpand(path))
+    if os.path.isdir(reldir):
+        return os.path.join(xpand(reldir), xpand(path))
+    else:
+        return os.path.join(xpand(os.path.dirname(reldir)), xpand(path))
```

### Comparing `ubiquerg-0.7.0/ubiquerg/system.py` & `ubiquerg-0.8.0/ubiquerg/system.py`

 * *Files identical despite different names*

### Comparing `ubiquerg-0.7.0/ubiquerg/web.py` & `ubiquerg-0.8.0/ubiquerg/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
         r"(?:(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+(?:[A-Z]{2,6}\.?|[A-Z0-9-]{2,}\.?)|"
         r"localhost|"
         r"\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})"
         r"(?::\d+)?"
         r"(?:/?|[/?]\S+)$",
         re.IGNORECASE,
     )
-    return re.match(regex, maybe_url) is not None
+    return re.match(regex, str(maybe_url)) is not None
```

### Comparing `ubiquerg-0.7.0/ubiquerg.egg-info/PKG-INFO` & `ubiquerg-0.8.0/ubiquerg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiquerg
-Version: 0.7.0
+Version: 0.8.0
 Summary: Various utility functions
 Home-page: https://github.com/pepkit/ubiquerg/
 Author: Vince Reuter
 License: BSD-2-Clause
 Keywords: utility,utilities,tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ubiquerg-0.7.0/ubiquerg.egg-info/SOURCES.txt` & `ubiquerg-0.8.0/ubiquerg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

