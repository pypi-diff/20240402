# Comparing `tmp/metapensiero_sqlalchemy_proxy-6.0.dev7.tar.gz` & `tmp/metapensiero_sqlalchemy_proxy-6.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metapensiero_sqlalchemy_proxy-6.0.dev7.tar", last modified: Mon Feb 19 09:20:12 2024, max compression
+gzip compressed data, was "metapensiero_sqlalchemy_proxy-6.0.dev8.tar", last modified: Tue Apr  2 19:01:35 2024, max compression
```

## Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7.tar` & `metapensiero_sqlalchemy_proxy-6.0.dev8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1860 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/CHANGES.rst
--rw-r--r--   0        0        0     2656 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/Justfile
--rw-r--r--   0        0        0    10407 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/OLDERCHANGES.rst
--rw-r--r--   0        0        0     1197 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/README.rst
--rw-r--r--   0        0        0     1197 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/README.rst
--rw-r--r--   0        0        0      561 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/Makefile
--rw-r--r--   0        0        0      434 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/api.rst
--rw-r--r--   0        0        0      457 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/base.rst
-lrwxr-xr-x   0        0        0        0 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/changes.rst -> ../CHANGES.rst
--rw-r--r--   0        0        0     1023 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/conf.py
--rw-r--r--   0        0        0      450 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/core.rst
--rw-r--r--   0        0        0      399 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/filters.rst
--rw-r--r--   0        0        0      810 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/index.rst
--rw-r--r--   0        0        0      398 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/json.rst
--rw-r--r--   0        0        0      441 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/orm.rst
--rw-r--r--   0        0        0    12493 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/pyramid.rst
--rw-r--r--   0        0        0      393 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/sorters.rst
--rw-r--r--   0        0        0      406 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/types.rst
--rw-r--r--   0        0        0      350 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/usage.rst
--rw-r--r--   0        0        0      385 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/doc/utils.rst
--rw-r--r--   0        0        0     2006 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/flake.lock
--rw-r--r--   0        0        0     5105 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/flake.nix
--rw-r--r--   0        0        0     1818 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/pyproject.toml
--rw-r--r--   0        0        0      680 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/__init__.py
--rw-r--r--   0        0        0    20297 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/base.py
--rw-r--r--   0        0        0     7222 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/core.py
--rw-r--r--   0        0        0    14381 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/filters.py
--rw-r--r--   0        0        0     2219 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/json.py
--rw-r--r--   0        0        0     5193 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/orm.py
--rw-r--r--   0        0        0    10945 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/pyramid.py
--rw-r--r--   0        0        0     6839 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/sorters.py
--rw-r--r--   0        0        0     4845 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/types.py
--rw-r--r--   0        0        0     7446 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/utils.py
--rw-r--r--   0        0        0     1631 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/tests/conftest.py
--rw-r--r--   0        0        0     3648 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/tests/fixture.py
--rwxr-xr-x   0        0        0     1629 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/tests/postgresql
--rw-r--r--   0        0        0    22885 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_core.py
--rw-r--r--   0        0        0     9123 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_filters.py
--rw-r--r--   0        0        0     1941 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_json.py
--rw-r--r--   0        0        0    10613 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_orm.py
--rw-r--r--   0        0        0     9858 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_postgresql.py
--rw-r--r--   0        0        0     2423 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_sorters.py
--rw-r--r--   0        0        0     3640 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_types.py
--rw-r--r--   0        0        0     2542 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev7/PKG-INFO
+-rw-r--r--   0        0        0     1968 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/CHANGES.rst
+-rw-r--r--   0        0        0     2697 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/Justfile
+-rw-r--r--   0        0        0    10407 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/OLDERCHANGES.rst
+-rw-r--r--   0        0        0     1197 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/README.rst
+-rw-r--r--   0        0        0     1197 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/README.rst
+-rw-r--r--   0        0        0      561 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/Makefile
+-rw-r--r--   0        0        0      434 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/api.rst
+-rw-r--r--   0        0        0      457 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/base.rst
+lrwxr-xr-x   0        0        0        0 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/changes.rst -> ../CHANGES.rst
+-rw-r--r--   0        0        0     1023 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/conf.py
+-rw-r--r--   0        0        0      450 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/core.rst
+-rw-r--r--   0        0        0      399 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/filters.rst
+-rw-r--r--   0        0        0      810 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/index.rst
+-rw-r--r--   0        0        0      398 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/json.rst
+-rw-r--r--   0        0        0      441 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/orm.rst
+-rw-r--r--   0        0        0    12493 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/pyramid.rst
+-rw-r--r--   0        0        0      393 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/sorters.rst
+-rw-r--r--   0        0        0      406 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/types.rst
+-rw-r--r--   0        0        0      350 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/usage.rst
+-rw-r--r--   0        0        0      385 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/utils.rst
+-rw-r--r--   0        0        0     2006 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/flake.lock
+-rw-r--r--   0        0        0     5105 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/flake.nix
+-rw-r--r--   0        0        0     1843 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/pyproject.toml
+-rw-r--r--   0        0        0      680 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/__init__.py
+-rw-r--r--   0        0        0    20274 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/base.py
+-rw-r--r--   0        0        0     7222 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/core.py
+-rw-r--r--   0        0        0    14744 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/filters.py
+-rw-r--r--   0        0        0     2219 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/json.py
+-rw-r--r--   0        0        0     5193 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/orm.py
+-rw-r--r--   0        0        0    10998 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/pyramid.py
+-rw-r--r--   0        0        0     7086 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/sorters.py
+-rw-r--r--   0        0        0     4845 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/types.py
+-rw-r--r--   0        0        0     7440 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/utils.py
+-rw-r--r--   0        0        0     1631 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/conftest.py
+-rw-r--r--   0        0        0     3648 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/fixture.py
+-rwxr-xr-x   0        0        0     1629 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/postgresql
+-rw-r--r--   0        0        0    22885 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_core.py
+-rw-r--r--   0        0        0     9123 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_filters.py
+-rw-r--r--   0        0        0     1941 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_json.py
+-rw-r--r--   0        0        0    10613 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_orm.py
+-rw-r--r--   0        0        0     9858 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_postgresql.py
+-rw-r--r--   0        0        0     2423 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_sorters.py
+-rw-r--r--   0        0        0     3640 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_types.py
+-rw-r--r--   0        0        0     2575 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/PKG-INFO
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/CHANGES.rst` & `metapensiero_sqlalchemy_proxy-6.0.dev8/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changes
 -------
 
+6.0.dev8 (2024-04-02)
+~~~~~~~~~~~~~~~~~~~~~
+
+* Fix signature of abstract ``save_changes()`` static method
+
+
 6.0.dev7 (2024-02-19)
 ~~~~~~~~~~~~~~~~~~~~~
 
 * Improve handling of ``ARRAY``\ s in the filter operator ``CONTAINS``, differentiating the
   *scalar* value from the *sub-array* containment
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/Justfile` & `metapensiero_sqlalchemy_proxy-6.0.dev8/Justfile`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
   set -euo pipefail
 
   function pg-stop {
     just _pg-stop
   }
   trap pg-stop EXIT
   pytest {{pytest-flags}}
+  coverage json --quiet -o coverage.json
 
 # Build documentation
 doc:
     sphinx-build -b html doc doc/_build/html
 
 #################
 # RELEASE TASKS #
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/OLDERCHANGES.rst` & `metapensiero_sqlalchemy_proxy-6.0.dev8/OLDERCHANGES.rst`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/README.rst` & `metapensiero_sqlalchemy_proxy-6.0.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/doc/Makefile` & `metapensiero_sqlalchemy_proxy-6.0.dev8/doc/Makefile`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/doc/conf.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/doc/conf.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/doc/index.rst` & `metapensiero_sqlalchemy_proxy-6.0.dev8/doc/index.rst`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/doc/pyramid.rst` & `metapensiero_sqlalchemy_proxy-6.0.dev8/doc/pyramid.rst`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/flake.lock` & `metapensiero_sqlalchemy_proxy-6.0.dev8/flake.lock`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/flake.nix` & `metapensiero_sqlalchemy_proxy-6.0.dev8/flake.nix`

 * *Files 8% similar despite different names*

```diff
@@ -39,16 +39,16 @@
           "python311"
         ];
 
         # SQLAlchemy versions to try out
         saVersions = [
           { version = "1.4.51";
             hash = "sha256-55CMICXrGDlOMtZd0C0uN+F9czzb59eCMcK21+sgzbk="; }
-          { version = "2.0.25";
-            hash = "sha256-osaadmT7LVS4aC3XdMO1T2f4T6Ejz4TdoqX0DcqgTgg="; }
+          { version = "2.0.29";
+            hash = "sha256-vZVmuOWMq9cAvDZ7YOkNk0nNFvCYSXP5ipoJ+cZOhvA="; }
         ];
 
         py-sa-pairs = cartesianProductOfSets { pyv = pyVersions; sav = saVersions; };
 
         mkSAPkg = python: saVersion:
           python.pkgs.buildPythonPackage rec {
             pname = "SQLAlchemy";
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/pyproject.toml` & `metapensiero_sqlalchemy_proxy-6.0.dev8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "metapensiero.sqlalchemy.proxy"
 description = "Expose SQLAlchemy's queries and their metadata to a webservice"
-version = "6.0.dev7"
+version = "6.0.dev8"
 authors = [
     { name = "Lele Gaifax", email = "lele@metapensiero.it" },
 ]
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
@@ -17,14 +17,15 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Topic :: Database",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "sqlalchemy",
+    "typing-extensions",
 ]
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.urls]
 Changelog = "https://gitlab.com/metapensiero/metapensiero.sqlalchemy.proxy/-/blob/master/CHANGES.rst"
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/__init__.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/base.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,16 +511,15 @@
                 if isinstance(meta['dictionary'], Mapping):
                     meta['dictionary'] = {
                         k: t(v) for k, v in meta['dictionary'].items()}
                 else:
                     meta['dictionary'] = [
                         [k, t(v)] for k, v in meta['dictionary']]
 
-            if 'default' not in meta and getattr(c, 'default', None) is not None:
-                default = c.default
+            if 'default' not in meta and (default := getattr(c, 'default', None)) is not None:
                 if not default.is_clause_element and not default.is_sequence:
                     if default.is_callable:
                         meta['default'] = default.arg(None)
                     else:
                         meta['default'] = default.arg
 
             # Do this last, so it cannot be overridden
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/core.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/core.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/filters.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 # :Copyright: © 2017, 2018, 2020, 2021, 2023, 2024 Lele Gaifax
 #
 
 from collections import namedtuple
 from collections.abc import Mapping, Sequence
 from enum import Enum
 import logging
+from typing import Any
 
 from sqlalchemy import ARRAY, String, and_, not_, or_
-from sqlalchemy.sql.expression import CompoundSelect, any_
+from sqlalchemy.sql.expression import CompoundSelect, Selectable, any_
 from sqlalchemy.orm.query import Query
+from typing_extensions import Self
 
 from .json import JSON
 from .types import get_adaptor_for_sa_type
 from .utils import SQLALCHEMY_VERSION, col_by_name, csv_to_list, get_column_type
 
 
 log = logging.getLogger(__name__)
@@ -146,15 +148,15 @@
     GREATER = ('>', lambda c, t, v, a: c > a(v))
     "The field value must be greater than the specified value."
 
     LESSER = ('<', lambda c, t, v, a: c < a(v))
     "The field value must be less than the specified value."
 
     @classmethod
-    def make(cls, operator):
+    def make(cls, operator: Self | str) -> Self:
         """Helper to create a new instance.
 
         The `operator` argument may be either an instance of the class, the name of one of its
         members (like ``"BETWEEN"``) or the symbolic operator (like ``"><"``).
         """
 
         if isinstance(operator, cls):
@@ -165,30 +167,33 @@
         except KeyError:
             for o in cls:
                 if o.value[0] == operator:
                     return o
 
         raise ValueError('Unrecognized filter operator: %r' % operator)
 
-    def __init__(self, operator, filter_factory):
+    def __init__(self, operator: str, filter_factory):
         self.operator = operator
         self.filter_factory = filter_factory
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__}.{self._name_}>"
 
     def filter(self, column, value):
         "Return a filter expression that compares `column` with `value`."
 
         ctype = get_column_type(column)
         adaptor = get_adaptor_for_sa_type(ctype)
         return self.filter_factory(column, ctype, value, adaptor)
 
 
-def split_operator_and_value(value, default_operator=Operator.EQUAL):
+def split_operator_and_value(
+        value,
+        default_operator: Operator = Operator.EQUAL
+) -> tuple[Operator, Any]:
     """Given a string `value`, recognize possible prefix comparison operator.
 
     If `value` is a string that starts with a known operator, split the value returning a tuple
     like ``(Operator.XXX, remaining-value)``; if it contains the ``><`` operator, return
     ``(Operator.BETWEEN, (start, end))``; otherwise return ``(Operator.EQUAL, value)``.
     """
 
@@ -203,34 +208,34 @@
     return default_operator, value
 
 
 class Filter(namedtuple('Filter', 'property, value, operator')):
     "Represent a single filter condition."
 
     @classmethod
-    def make(cls, property, value, operator=Operator.EQUAL):
+    def make(cls, property: str, value: Any, operator=Operator.EQUAL) -> Self:
         """Helper to create a new instance.
 
         The `operator` gets coerced to an :class:`Operator` instance using its
         :meth:`Operator.make` class method.
         """
 
         return cls(property, value, Operator.make(operator))
 
-    def filter(self, statement):
+    def filter(self, statement: Query | Selectable):
         column = col_by_name(statement, self.property)
         if column is not None:
             try:
                 return self.operator.filter(column, self.value)
             except Exception:  # pragma: no cover
                 log.error('Error filtering on condition %r', self)
                 raise
 
 
-def extract_filters(args):
+def extract_filters(args: dict[str, Any]) -> list[Filter]:
     """Extract filter conditions.
 
     :param args: a dictionary, usually request.params
     :rtype: a list of :class:`Filter` instances
 
     Recognize three possible syntaxes specifying filtering conditions:
 
@@ -309,15 +314,18 @@
             fvalue = args.pop(f, missing)
             if fvalue is not missing:
                 result.append(Filter(fcol, fvalue, Operator.EQUAL))
 
     return result
 
 
-def apply_filters(query, args):
+def apply_filters(
+        query: Query | Selectable,
+        args: dict[str, Any]
+) -> tuple[Selectable, list[str] | None]:
     """Filter a given query.
 
     :param query: an SQLAlchemy ``Query``
     :param args: a dictionary
     :rtype: a tuple
 
     `query` may be either a SQL statement (not necessarily a ``SELECT``) or an ORM query.
@@ -402,14 +410,16 @@
             columns = []
             for f in csv_to_list(qfields):
                 column = col_by_name(stmt, f)
                 if column is not None:
                     columns.append(column)
                 else:
                     log.warning('Ignoring query filter on non-existing column %r', f)
+        else:
+            columns = qfields
 
         conds = []
         for column in columns:
             conds.append(operator.filter(column, value))
 
         if conds:
             if query is not squery:
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/json.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/json.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/orm.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/orm.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/pyramid.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/pyramid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # :Project:   metapensiero.sqlalchemy.proxy -- Pyramid decorator glue
 # :Created:   mer 08 ago 2012 19:07:28 CEST
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2012, 2013, 2016, 2017, 2018, 2020, 2021 Lele Gaifax
+# :Copyright: © 2012, 2013, 2016, 2017, 2018, 2020, 2021, 2024 Lele Gaifax
 #
 
 from collections.abc import Callable
 from functools import wraps
 from inspect import isgeneratorfunction
 
 from sqlalchemy.sql.expression import Selectable
@@ -162,18 +162,19 @@
     @staticmethod
     def extract_parameters(request):
         """Create a dictionary of parameters from the current request."""
 
         return dict(request.params)
 
     @staticmethod
-    def save_changes(sa_session, modified, deleted):
+    def save_changes(session, request, modified, deleted):
         """Save insertions, changes and deletions to the database.
 
-        :param sa_session: the SQLAlchemy session
+        :param session: the SQLAlchemy session
+        :param request: a Pyramid `Request` instance
         :param modified: a sequence of record changes, each represented by
             a tuple of two items, the PK name and a
             dictionary with the modified fields; if the value
             of the PK field is null or 0 then the record is
             considered new and will be inserted instead of updated
         :param deleted: a sequence of deletions, each represented by a tuple
             of two items, the PK name and the ID of the record to
@@ -231,34 +232,34 @@
         self.proxy_kwargs = proxy_kwargs
 
     def __call__(self, method):
         @wraps(method)
         def workhorse(request):
             adapt = method().send if isgeneratorfunction(method) else False
 
-            sa_session = self.create_session(request)
+            session = self.create_session(request)
             options = self.proxy_kwargs.copy()
             options.update(self.extract_parameters(request))
             conditions = ()
 
             with transaction.manager:
                 if adapt:
                     adapt(None)
                     options = adapt((request, options))
                     if isinstance(options, tuple):
                         options, conditions = options
 
                 if request.method == 'GET':
-                    result = self.proxie(sa_session, request, *conditions, **options)
+                    result = self.proxie(session, request, *conditions, **options)
                 else:
                     handler = getattr(self, request.method, None)
                     if handler is None:
                         raise NotImplementedError(
                             'Could not handle %s request' % request.method)
-                    result = handler(sa_session, request, **options)
+                    result = handler(session, request, **options)
 
                 if adapt:
                     result = adapt(result)
                 else:
                     result = method(request, result)
 
                 return result
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/sorters.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/sorters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # -*- coding: utf-8 -*-
 # :Project:   metapensiero.sqlalchemy.proxy -- Sorting capability
 # :Created:   dom 12 feb 2017 12:50:56 CET
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2017, 2018, 2020, 2021 Lele Gaifax
+# :Copyright: © 2017, 2018, 2020, 2021, 2023 Lele Gaifax
 #
 
 from collections import namedtuple
 from collections.abc import Mapping, Sequence
 from enum import Enum
 import logging
+from typing import Any
 
+from sqlalchemy.sql.expression import Selectable
 from sqlalchemy.orm.query import Query
+from typing_extensions import Self
 
 from .json import JSON
 from .utils import col_by_name, csv_to_list
 
 
 log = logging.getLogger(__name__)
 
@@ -26,15 +29,15 @@
     ASC = '<'
     "Ascending order."
 
     DESC = '>'
     "Descending order."
 
     @classmethod
-    def make(cls, direction):
+    def make(cls, direction: Self | str) -> Self:
         """Helper function to create a new instance.
 
         The `direction` argument may be either an instance of the class, the name on one of its
         members (like ``"DESC"``) or the symbolic form (like ``">"``).
         """
 
         if isinstance(direction, cls):
@@ -45,33 +48,33 @@
             except KeyError:
                 for d in cls:
                     if d.value == direction:
                         return d
 
         raise ValueError('Unrecognized sort direction: %r' % direction)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__}.{self._name_}>"
 
 
 class Sorter(namedtuple('Sorter', 'property, direction')):
     "Represent a single field ordering specification."
 
     @classmethod
-    def make(cls, property, direction=Direction.ASC):
+    def make(cls, property: str, direction: Direction | str = Direction.ASC) -> Self:
         """Helper to create a new instance.
 
         The `direction` argument defaults to :data:`Direction.ASC` and gets coerced to a
         :class:`Direction` instance using its :meth:`Direction.make` class method.
         """
 
         return cls(property, Direction.make(direction))
 
 
-def extract_sorters(args):
+def extract_sorters(args: dict[str, Any]) -> list[Sorter]:
     """Extract sort specification.
 
     :param args: a dictionary
     :rtype: a list of :class:`Sorter` instances
 
     Recognize different kinds of specification:
 
@@ -95,17 +98,16 @@
 
     sorters = []
 
     # Old syntax:
     # ?sort_col=fieldname&sort_dir=ASC
 
     sort_col = args.pop('sort_col', missing)
-    sort_dir = Direction.make(args.pop('sort_dir', 'ASC'))
-
     if sort_col is not missing:
+        sort_dir = Direction.make(args.pop('sort_dir', 'ASC'))
         if isinstance(sort_col, str):
             sorters.extend(Sorter(col, sort_dir) for col in csv_to_list(sort_col))
         elif isinstance(sort_col, Sequence):
             for col in sort_col:
                 if not isinstance(col, str):
                     raise ValueError('Unrecognized sort specification: %r' % sort_col)
                 sorters.append(Sorter(col, sort_dir))
@@ -149,15 +151,15 @@
             fvalue = args.pop(f, missing)
             if fvalue is not missing:
                 sorters.append(Sorter(fcol, Direction.make(fvalue or Direction.ASC)))
 
     return sorters
 
 
-def apply_sorters(query, args):
+def apply_sorters(query: Query | Selectable, args: dict) -> Selectable:
     r"""Order a given query.
 
     :param query: an SQLAlchemy ``Query``
     :param args: a dictionary
     :rtype: an SQLAlchemy ``Query``
 
     `query` may be either a SQL statement or an ORM query.
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/types.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/types.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/src/metapensiero/sqlalchemy/proxy/utils.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # :Project:   metapensiero.sqlalchemy.proxy -- Utility functions
 # :Created:   mer 03 feb 2016 10:56:36 CET
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2016, 2017, 2018, 2020, 2021 Lele Gaifax
+# :Copyright: © 2016, 2017, 2018, 2020, 2021, 2024 Lele Gaifax
 #
 
 import logging
 
 from sqlalchemy import Column
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.sql import ColumnCollection
@@ -131,35 +131,35 @@
 
     The `adaptor` function takes four arguments, respectively the SA
     session, the request, a list of added/modified records and a list
     of deleted records; it must return two (possibly modified) lists,
     one containing added/modified records and the other with the
     records to delete, e.g.::
 
-        def adaptor(sa_session, request, modified_recs, deleted_recs):
+        def adaptor(session, request, modified_recs, deleted_recs):
             # do any step to adapt incoming data
             return modified_recs, deleted_recs
     """
 
-    def workhorse(sa_session, request, **args):
+    def workhorse(session, request, **args):
         mr = JSON.decode(args[modified_slot_name])
         dr = JSON.decode(args[deleted_slot_name])
 
         if adaptor is not None:
             try:
-                mr, dr = adaptor(sa_session, request, mr, dr)
+                mr, dr = adaptor(session, request, mr, dr)
             except Exception as e:
                 log.critical('Could not adapt changes: %s', e, exc_info=True)
                 return {
                     success_slot: False,
                     message_slot: 'Internal error, consult application log'
                 }
 
         try:
-            iids, mids, dids = save_changes(sa_session, request, mr, dr)
+            iids, mids, dids = save_changes(session, request, mr, dr)
             status = True
             statusmsg = "Ok"
         except SQLAlchemyError as e:
             msg = str(e)
             log.error('Could not save changes to the database: %s', msg)
             status = False
             statusmsg = msg.split('\n')[0]
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/tests/conftest.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/tests/fixture.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/fixture.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/tests/postgresql` & `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/postgresql`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_core.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_filters.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_json.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_orm.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_postgresql.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_sorters.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_sorters.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/tests/test_types.py` & `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev7/PKG-INFO` & `metapensiero_sqlalchemy_proxy-6.0.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metapensiero.sqlalchemy.proxy
-Version: 6.0.dev7
+Version: 6.0.dev8
 Summary: Expose SQLAlchemy's queries and their metadata to a webservice
 Author-Email: Lele Gaifax <lele@metapensiero.it>
 License: GPL-3.0-or-later
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Database
 Project-URL: Changelog, https://gitlab.com/metapensiero/metapensiero.sqlalchemy.proxy/-/blob/master/CHANGES.rst
 Project-URL: Documentation, https://metapensierosqlalchemyproxy.readthedocs.io/en/latest/
 Project-URL: Source, https://gitlab.com/metapensiero/metapensiero.sqlalchemy.proxy
 Requires-Python: >=3.9
 Requires-Dist: sqlalchemy
+Requires-Dist: typing-extensions
 Requires-Dist: build; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: tomli; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: tomli; extra == "docs"
 Provides-Extra: dev
 Provides-Extra: docs
```

