# Comparing `tmp/jaraco.postgres-5.1.0.tar.gz` & `tmp/jaraco.postgres-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.postgres-5.1.0.tar", last modified: Tue Feb  2 02:13:21 2021, max compression
+gzip compressed data, was "jaraco.postgres-5.2.0.tar", last modified: Mon Apr  1 22:22:17 2024, max compression
```

## Comparing `jaraco.postgres-5.1.0.tar` & `jaraco.postgres-5.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 02:13:21.090892 jaraco.postgres-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (117)       50 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (117)      136 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 02:13:21.086892 jaraco.postgres-5.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 02:13:21.090892 jaraco.postgres-5.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (117)      497 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/.github/workflows/automerge.yml
--rw-r--r--   0 runner    (1001) docker     (117)     1030 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (117)      175 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (117)       79 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (117)     1887 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (117)     1050 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (117)     2081 2021-02-02 02:13:21.090892 jaraco.postgres-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)     1182 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 02:13:21.090892 jaraco.postgres-5.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (117)      756 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (117)       81 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (117)      397 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 02:13:21.086892 jaraco.postgres-5.1.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 02:13:21.090892 jaraco.postgres-5.1.0/jaraco/postgres/
--rw-r--r--   0 runner    (1001) docker     (117)    21846 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/jaraco/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (117)      439 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/jaraco/postgres/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 02:13:21.090892 jaraco.postgres-5.1.0/jaraco.postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (117)     2081 2021-02-02 02:13:20.000000 jaraco.postgres-5.1.0/jaraco.postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)      607 2021-02-02 02:13:21.000000 jaraco.postgres-5.1.0/jaraco.postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (117)        1 2021-02-02 02:13:20.000000 jaraco.postgres-5.1.0/jaraco.postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (117)       50 2021-02-02 02:13:20.000000 jaraco.postgres-5.1.0/jaraco.postgres.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (117)      282 2021-02-02 02:13:20.000000 jaraco.postgres-5.1.0/jaraco.postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (117)       12 2021-02-02 02:13:20.000000 jaraco.postgres-5.1.0/jaraco.postgres.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (117)       37 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (117)      367 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (117)      333 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (117)     1160 2021-02-02 02:13:21.090892 jaraco.postgres-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (117)       92 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (117)    10139 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/skeleton.md
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 02:13:21.090892 jaraco.postgres-5.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (117)       87 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (117)    15168 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/tests/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (117)      719 2021-02-02 02:13:05.000000 jaraco.postgres-5.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:22:17.912880 jaraco.postgres-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:22:17.908880 jaraco.postgres-5.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:22:17.908880 jaraco.postgres-5.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-01 22:22:17.912880 jaraco.postgres-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:22:17.908880 jaraco.postgres-5.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:22:17.904880 jaraco.postgres-5.2.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:22:17.912880 jaraco.postgres-5.2.0/jaraco/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)    22005 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/jaraco/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/jaraco/postgres/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:22:17.912880 jaraco.postgres-5.2.0/jaraco.postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-01 22:22:17.000000 jaraco.postgres-5.2.0/jaraco.postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-01 22:22:17.000000 jaraco.postgres-5.2.0/jaraco.postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:22:17.000000 jaraco.postgres-5.2.0/jaraco.postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 22:22:17.000000 jaraco.postgres-5.2.0/jaraco.postgres.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-01 22:22:17.000000 jaraco.postgres-5.2.0/jaraco.postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 22:22:17.000000 jaraco.postgres-5.2.0/jaraco.postgres.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-01 22:22:17.912880 jaraco.postgres-5.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:22:17.912880 jaraco.postgres-5.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14969 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/tests/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-01 22:21:59.000000 jaraco.postgres-5.2.0/tox.ini
```

### Comparing `jaraco.postgres-5.1.0/CHANGES.rst` & `jaraco.postgres-5.2.0/NEWS.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v5.2.0
+======
+
+Features
+--------
+
+- Packaging refresh.
+
+
 v5.1.0
 ======
 
 #7: Allow ``encoding`` parameter to ``initdb``.
 
 Package now uses PEP 420 for namespace package.
```

### Comparing `jaraco.postgres-5.1.0/LICENSE` & `jaraco.postgres-5.2.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.postgres-5.1.0/PKG-INFO` & `jaraco.postgres-5.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,71 @@
 Metadata-Version: 2.1
 Name: jaraco.postgres
-Version: 5.1.0
+Version: 5.2.0
 Summary: PostgreSQL services by jaraco
 Home-page: https://github.com/jaraco/jaraco.postgres
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/pypi/v/jaraco.postgres.svg
-           :target: `PyPI link`_
-        
-        .. image:: https://img.shields.io/pypi/pyversions/jaraco.postgres.svg
-           :target: `PyPI link`_
-        
-        .. _PyPI link: https://pypi.org/project/jaraco.postgres
-        
-        .. image:: https://github.com/jaraco/jaraco.postgres/workflows/tests/badge.svg
-           :target: https://github.com/jaraco/jaraco.postgres/actions?query=workflow%3A%22tests%22
-           :alt: tests
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: Black
-        
-        .. image:: https://readthedocs.org/projects/jaracopostgres/badge/?version=latest
-           :target: https://jaracopostgres.readthedocs.io/en/latest/?badge=latest
-        
-        Routines and fixtures for launching and managing
-        `PostgreSQL <https://postgresql.org>`_ instances.
-        
-        Pytest Plugin
-        =============
-        
-        This library includes a pytest plugin. To enable it, simply
-        include this library in your test requirements.
-        
-        Then, in your tests, simply add a ``postgresql_instance``
-        parameter to your functions.
-        
-        Instance
-        --------
-        
-        The ``postgresql_instance`` is a ``jaraco.postgres.PostgresServer``
-        instance with ``host`` and ``port`` properties.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Pytest
-Requires-Python: >=3.6
+Requires-Python: >=3.8
+License-File: LICENSE
+Requires-Dist: jaraco.services
+Requires-Dist: portend
+Requires-Dist: packaging
+Requires-Dist: jaraco.functools
+Requires-Dist: jaraco.context
 Provides-Extra: testing
+Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
+Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-mypy; extra == "testing"
+Requires-Dist: pytest-enabler>=2.2; extra == "testing"
+Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
+Requires-Dist: psycopg2-binary; extra == "testing"
 Provides-Extra: docs
+Requires-Dist: sphinx>=3.5; extra == "docs"
+Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
+Requires-Dist: rst.linker>=1.9; extra == "docs"
+Requires-Dist: furo; extra == "docs"
+Requires-Dist: sphinx-lint; extra == "docs"
+
+.. image:: https://img.shields.io/pypi/v/jaraco.postgres.svg
+   :target: https://pypi.org/project/jaraco.postgres
+
+.. image:: https://img.shields.io/pypi/pyversions/jaraco.postgres.svg
+
+.. image:: https://github.com/jaraco/jaraco.postgres/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/jaraco/jaraco.postgres/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. image:: https://readthedocs.org/projects/jaracopostgres/badge/?version=latest
+   :target: https://jaracopostgres.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
+   :target: https://blog.jaraco.com/skeleton
+
+Routines and fixtures for launching and managing
+`PostgreSQL <https://postgresql.org>`_ instances.
+
+Pytest Plugin
+=============
+
+This library includes a pytest plugin. To enable it, simply
+include this library in your test requirements.
+
+Then, in your tests, simply add a ``postgresql_instance``
+parameter to your functions.
+
+Instance
+--------
+
+The ``postgresql_instance`` is a ``jaraco.postgres.PostgresServer``
+instance with ``host`` and ``port`` properties.
```

### Comparing `jaraco.postgres-5.1.0/README.rst` & `jaraco.postgres-5.2.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 .. image:: https://img.shields.io/pypi/v/jaraco.postgres.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.postgres
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.postgres.svg
-   :target: `PyPI link`_
 
-.. _PyPI link: https://pypi.org/project/jaraco.postgres
-
-.. image:: https://github.com/jaraco/jaraco.postgres/workflows/tests/badge.svg
+.. image:: https://github.com/jaraco/jaraco.postgres/actions/workflows/main.yml/badge.svg
    :target: https://github.com/jaraco/jaraco.postgres/actions?query=workflow%3A%22tests%22
    :alt: tests
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
 
 .. image:: https://readthedocs.org/projects/jaracopostgres/badge/?version=latest
    :target: https://jaracopostgres.readthedocs.io/en/latest/?badge=latest
 
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
+   :target: https://blog.jaraco.com/skeleton
+
 Routines and fixtures for launching and managing
 `PostgreSQL <https://postgresql.org>`_ instances.
 
 Pytest Plugin
 =============
 
 This library includes a pytest plugin. To enable it, simply
```

### Comparing `jaraco.postgres-5.1.0/jaraco/postgres/__init__.py` & `jaraco.postgres-5.2.0/jaraco/postgres/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,34 @@
 etc.
 
 Warning: These methods are inconsistent about the exceptions that they raise.
 Some errors provoke OSError, whereas other similar errors might provoke
 CalledProcessError or RuntimeError.  This should be made consistent.
 '''
 
+import functools
 import glob
+import importlib
+import itertools
 import logging
 import os
+import re
 import shutil
 import signal
 import subprocess
 import tempfile
 import time
-import importlib
-import itertools
-import re
 
 import packaging.version
-from jaraco.services import paths
 
+from jaraco.context import ExceptionTrap
+from jaraco.functools import retry
+from jaraco.services import paths
 
-DEV_NULL = open(os.path.devnull, 'r+')
+DEV_NULL = open(os.path.devnull, 'r+', encoding='utf-8')
 
 log = logging.getLogger('jaraco.postgres')
 
 
 class NotInitializedError(Exception):
     "An exception raised when an uninitialized DBMS is asked to do something"
 
@@ -193,31 +196,30 @@
     # For legacy compatibility.
     drop_if_exists = drop
 
     def drop_user(self):
         """DROP this USER, if it exists."""
         self.super_psql(['-c', "DROP USER IF EXISTS %s" % self.user])
 
-    def psql(self, args):
+    def psql(self, args) -> None:
         r"""Invoke psql, passing the given command-line arguments.
 
         Typical <args> values: ['-c', <sql_string>] or ['-f', <pathname>].
 
-        Connection parameters are taken from self.  STDIN, STDOUT,
+        Connection parameters are taken from self. STDIN, STDOUT,
         and STDERR are inherited from the parent.
 
         WARNING: This method uses the psql(1) program, which ignores SQL
-        errors
-        by default.  That hides many real errors, making our software less
-        reliable.  To overcome this flaw, add this line to the head of your
-        SQL:
+        errors by default. That approach masks real errors and degrades
+        reliability. To overcome this weakness, add the following line to
+        the head of the SQL definition::
+
             "\set ON_ERROR_STOP TRUE"
 
-        @return: None. Raises an exception upon error, but *ignores SQL
-        errors* unless "\set ON_ERROR_STOP TRUE" is used.
+        Raises an exception upon error.
         """
         argv = (
             [
                 PostgresFinder.find_root() / 'psql',
                 '--quiet',
                 '-U',
                 self.user,
@@ -300,14 +302,19 @@
             self.host,
             '-p',
             self.port,
         ] + args
         subprocess.check_call(argv)
 
 
+def first_line(filepath):
+    with open(filepath, encoding='utf-8') as strm:
+        return next(strm)
+
+
 class PostgresServer:
     def __init__(
         self, host='localhost', port=5432, base_pathname=None, superuser='postgres'
     ):
         """This class represents a DBMS server.
 
         This class can represent either
@@ -364,15 +371,15 @@
         succeeds.
         """
         tries = itertools.count()
         max_tries = 50
         while os.path.isdir(path):
             try:
                 shutil.rmtree(path)
-            except WindowsError:
+            except OSError:
                 if next(tries) >= max_tries:
                     raise
                 time.sleep(0.2)
 
     def initdb(self, quiet=True, locale='en_US.UTF-8', encoding=None):
         """Bootstrap this DBMS from nothing.
 
@@ -430,21 +437,22 @@
         return subprocess.check_output(cmd)
 
     def is_running(self, tries=10):
         """
         Return True if this server is currently running and reachable.
 
         The postgres tools have critical windows during which they give
-        misbehave
-        or give the wrong answer.  If postgres was just launched:
-            - it might not yet appear to be running, or
-            - pg_ctl might think that it's running, but psql might not yet
-              be able to connect to it, or
-            - it might be about to abort because of a configuration problem,
-            - or all three!  It might be starting up, but about to abort.
+        misbehave or give the wrong answer. If postgres was just launched:
+
+        - it might not yet appear to be running, or
+        - pg_ctl might think that it's running, but psql might not yet
+          be able to connect to it, or
+        - it might be about to abort because of a configuration problem,
+        - or all three!  It might be starting up, but about to abort.
+
         Sadly, it's not easy to make a declaration about state if the server
         just started
         or stopped.  To increase confidence, makes repeated checks,
         and declares a decision only after <tries> consecutive measurements
         agree.
         """
         return self._is_running(tries) and (self._assert_ready() or True)
@@ -493,38 +501,43 @@
             self.host,
             '-p',
             self.port,
             '-U',
             self.superuser,
         ]
 
+    # Python 3.8 compat
+    passes_CalledProcessError = ExceptionTrap(subprocess.CalledProcessError).passes
+
+    @passes_CalledProcessError
+    @retry(
+        retries=49,
+        trap=subprocess.CalledProcessError,
+        cleanup=functools.partial(time.sleep, 0.2),
+    )
     def ready(self):
         """
         Assumes postgres now talks to pg_ctl, but might not yet be listening
-        or connections from psql.  Test that psql is able to connect, as
+        for connections from psql. Test that psql is able to connect, as
         it occasionally takes 5-10 seconds for postgresql to start listening.
         """
-        cmd = self._psql_cmd()
-        for i in range(50, -1, -1):
-            res = subprocess.call(cmd, stdin=DEV_NULL, stdout=DEV_NULL, stderr=DEV_NULL)
-            if res == 0:
-                break
-            time.sleep(0.2)
-        return i != 0
+        subprocess.check_call(
+            self._psql_cmd(), stdin=DEV_NULL, stdout=DEV_NULL, stderr=DEV_NULL
+        )
 
     @property
     def pid(self):
         """The server's PID (None if not running)."""
         # We can't possibly be running if our base_pathname isn't defined.
         if not self.base_pathname:
             return None
         try:
             pidfile = os.path.join(self.base_pathname, 'postmaster.pid')
-            return int(open(pidfile).readline())
-        except (IOError, OSError):
+            return int(first_line(pidfile))
+        except OSError:
             return None
 
     @staticmethod
     def get_version():
         """Returns the Postgres version in tuple form, e.g: (9, 1)"""
         cmd = [PostgresFinder.find_root() / 'pg_ctl', '--version']
         results = subprocess.check_output(cmd).decode('utf-8')
@@ -560,33 +573,31 @@
             else:
                 socketop = 'unix_socket_directory'
             postgres_options = [
                 # When running not as root, postgres might try to put files
                 #  where they're not writable (see
                 #  https://paste.yougov.net/YKdgi). So set the socket_dir.
                 '-c',
-                '{}={}'.format(socketop, self.base_pathname),
+                f'{socketop}={self.base_pathname}',
                 '-h',
                 self.host,
                 '-i',  # enable TCP/IP connections
                 '-p',
                 self.port,
             ]
-            subprocess.check_call(
-                [
-                    PostgresFinder.find_root() / 'pg_ctl',
-                    'start',
-                    '-D',
-                    self.base_pathname,
-                    '-l',
-                    os.path.join(self.base_pathname, 'postgresql.log'),
-                    '-o',
-                    subprocess.list2cmdline(postgres_options),
-                ]
-            )
+            subprocess.check_call([
+                PostgresFinder.find_root() / 'pg_ctl',
+                'start',
+                '-D',
+                self.base_pathname,
+                '-l',
+                os.path.join(self.base_pathname, 'postgresql.log'),
+                '-o',
+                subprocess.list2cmdline(postgres_options),
+            ])
 
         # Postgres may launch, then abort if it's unhappy with some parameter.
         # This post-launch test helps us decide.
         if not self.is_running():
             tmpl = (
                 '%s aborted immediately after launch, check '
                 'postgresql.log in storage dir'
```

### Comparing `jaraco.postgres-5.1.0/jaraco.postgres.egg-info/PKG-INFO` & `jaraco.postgres-5.2.0/jaraco.postgres.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,71 @@
 Metadata-Version: 2.1
 Name: jaraco.postgres
-Version: 5.1.0
+Version: 5.2.0
 Summary: PostgreSQL services by jaraco
 Home-page: https://github.com/jaraco/jaraco.postgres
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/pypi/v/jaraco.postgres.svg
-           :target: `PyPI link`_
-        
-        .. image:: https://img.shields.io/pypi/pyversions/jaraco.postgres.svg
-           :target: `PyPI link`_
-        
-        .. _PyPI link: https://pypi.org/project/jaraco.postgres
-        
-        .. image:: https://github.com/jaraco/jaraco.postgres/workflows/tests/badge.svg
-           :target: https://github.com/jaraco/jaraco.postgres/actions?query=workflow%3A%22tests%22
-           :alt: tests
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: Black
-        
-        .. image:: https://readthedocs.org/projects/jaracopostgres/badge/?version=latest
-           :target: https://jaracopostgres.readthedocs.io/en/latest/?badge=latest
-        
-        Routines and fixtures for launching and managing
-        `PostgreSQL <https://postgresql.org>`_ instances.
-        
-        Pytest Plugin
-        =============
-        
-        This library includes a pytest plugin. To enable it, simply
-        include this library in your test requirements.
-        
-        Then, in your tests, simply add a ``postgresql_instance``
-        parameter to your functions.
-        
-        Instance
-        --------
-        
-        The ``postgresql_instance`` is a ``jaraco.postgres.PostgresServer``
-        instance with ``host`` and ``port`` properties.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Pytest
-Requires-Python: >=3.6
+Requires-Python: >=3.8
+License-File: LICENSE
+Requires-Dist: jaraco.services
+Requires-Dist: portend
+Requires-Dist: packaging
+Requires-Dist: jaraco.functools
+Requires-Dist: jaraco.context
 Provides-Extra: testing
+Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
+Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-mypy; extra == "testing"
+Requires-Dist: pytest-enabler>=2.2; extra == "testing"
+Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
+Requires-Dist: psycopg2-binary; extra == "testing"
 Provides-Extra: docs
+Requires-Dist: sphinx>=3.5; extra == "docs"
+Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
+Requires-Dist: rst.linker>=1.9; extra == "docs"
+Requires-Dist: furo; extra == "docs"
+Requires-Dist: sphinx-lint; extra == "docs"
+
+.. image:: https://img.shields.io/pypi/v/jaraco.postgres.svg
+   :target: https://pypi.org/project/jaraco.postgres
+
+.. image:: https://img.shields.io/pypi/pyversions/jaraco.postgres.svg
+
+.. image:: https://github.com/jaraco/jaraco.postgres/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/jaraco/jaraco.postgres/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. image:: https://readthedocs.org/projects/jaracopostgres/badge/?version=latest
+   :target: https://jaracopostgres.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
+   :target: https://blog.jaraco.com/skeleton
+
+Routines and fixtures for launching and managing
+`PostgreSQL <https://postgresql.org>`_ instances.
+
+Pytest Plugin
+=============
+
+This library includes a pytest plugin. To enable it, simply
+include this library in your test requirements.
+
+Then, in your tests, simply add a ``postgresql_instance``
+parameter to your functions.
+
+Instance
+--------
+
+The ``postgresql_instance`` is a ``jaraco.postgres.PostgresServer``
+instance with ``host`` and ``port`` properties.
```

### Comparing `jaraco.postgres-5.1.0/jaraco.postgres.egg-info/SOURCES.txt` & `jaraco.postgres-5.2.0/jaraco.postgres.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 .coveragerc
-.flake8
+.editorconfig
 .pre-commit-config.yaml
-.readthedocs.yml
-CHANGES.rst
+.readthedocs.yaml
 LICENSE
+NEWS.rst
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
+ruff.toml
 setup.cfg
-setup.py
-skeleton.md
+towncrier.toml
 tox.ini
-.github/workflows/automerge.yml
+.github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 jaraco.postgres.egg-info/PKG-INFO
 jaraco.postgres.egg-info/SOURCES.txt
 jaraco.postgres.egg-info/dependency_links.txt
```

### Comparing `jaraco.postgres-5.1.0/setup.cfg` & `jaraco.postgres-5.2.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 [metadata]
-license_files = 
-	LICENSE
 name = jaraco.postgres
 author = Jason R. Coombs
 author_email = jaraco@jaraco.com
 description = PostgreSQL services by jaraco
 long_description = file:README.rst
 url = https://github.com/jaraco/jaraco.postgres
 classifiers = 
@@ -12,44 +10,39 @@
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Framework :: Pytest
 
 [options]
-packages = find_namespace:
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
 	jaraco.services
 	portend
 	packaging
-setup_requires = setuptools_scm[toml] >= 3.4.1
-
-[options.packages.find]
-exclude = 
-	build*
-	docs*
-	tests*
+	jaraco.functools
+	jaraco.context
 
 [options.extras_require]
 testing = 
-	pytest >= 3.5, !=3.7.3
-	pytest-checkdocs >= 1.2.3
-	pytest-flake8
-	pytest-black >= 0.3.7; python_implementation != "PyPy"
+	pytest >= 6, != 8.1.1
+	pytest-checkdocs >= 2.4
 	pytest-cov
-	pytest-mypy; python_implementation != "PyPy"
-	pytest-enabler
+	pytest-mypy
+	pytest-enabler >= 2.2
+	pytest-ruff >= 0.2.1
 	
 	psycopg2-binary
 docs = 
-	sphinx
-	jaraco.packaging >= 8.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [options.entry_points]
 pytest11 = 
 	PostgreSQL = jaraco.postgres.fixtures
 
 [egg_info]
 tag_build =
```

### Comparing `jaraco.postgres-5.1.0/tests/test_postgres.py` & `jaraco.postgres-5.2.0/tests/test_postgres.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-# coding: utf-8
-
 '''
 Functional tests for the jaraco.postgres module.
 
 Intended to be run using py.test.
 '''
 
-import io
 import os
 import shutil
 from subprocess import CalledProcessError
 
-import psycopg2
 import portend
+import psycopg2
 import pytest
 
 import jaraco.postgres as pgtools
 from jaraco.postgres import PostgresDatabase, PostgresServer
 
-
 HOST = os.environ.get('HOST', 'localhost')
 
 
 @pytest.fixture(autouse=True)
 def needs_postgresql(postgresql_instance):
     pass
 
@@ -49,15 +45,15 @@
         server.initdb(locale=locale)
 
         try:
             server.start()
             server.get_version()  # To check we're able to talk to it.
 
             config = os.path.join(server.base_pathname, 'postgresql.conf')
-            with io.open(config, encoding='utf-8') as strm:
+            with open(config, encoding='utf-8') as strm:
                 expect = "lc_messages = 'C'"
                 assert any(expect in line for line in strm)
         finally:
             server.destroy()
 
     def test_unicode_value(self, monkeypatch):
         port = portend.find_available_local_port()
@@ -70,39 +66,18 @@
             db = server.create('test_unicode')
             db.sql('CREATE TABLE records(name varchar(80))')
             db.sql("INSERT INTO records (name) VALUES (U&'\\2609')")
         finally:
             server.destroy()
 
 
-class TestPostgresDatabase:
-    def setup(self):
-        self.port = portend.find_available_local_port()
-        self.server = PostgresServer(HOST, self.port)
-        self.server.initdb()
-        self.server.start()
-
-    def teardown(self):
-        self.server.destroy()
-
-    def test_creates_user_and_database(self):
-        database = PostgresDatabase('tests', user='john', host=HOST, port=self.port)
-
-        database.create_user()
-        database.create()
-
-        rows = database.sql('SELECT 1')
-
-        assert rows == [(1,)]
-
-
 UNUSED_PORT = portend.find_available_local_port()
 
 
-class Test_PostgresDatabase:
+class TestPostgresDatabase:
     @pytest.fixture(scope='class', autouse=True)
     def dbms(self, request):
         cls = request.cls
         cls.port = UNUSED_PORT
         cls.dbms = pgtools.PostgresServer(port=cls.port)
         cls.dbms.initdb()
         cls.dbms.start()
@@ -113,14 +88,29 @@
     @pytest.fixture(scope='function', autouse=True)
     def cleanup_database(self):
         yield
         if hasattr(self, 'database'):
             self.database.drop_if_exists()
             self.database.drop_user()
 
+    def test_creates_user_and_database(self, postgresql_instance):
+        database = self.database = PostgresDatabase(
+            'tests',
+            user='john',
+            host=postgresql_instance.host,
+            port=postgresql_instance.port,
+        )
+
+        database.create_user()
+        database.create()
+
+        rows = database.sql('SELECT 1')
+
+        assert rows == [(1,)]
+
     def test___init__can_create_multiple_databases(self):
         database_1 = None
         database_2 = None
         try:
             database_1 = pgtools.PostgresDatabase(
                 db_name='test_pgtools_1', port=self.port
             )
@@ -278,15 +268,15 @@
         exists
         """
         self.database = pgtools.PostgresDatabase(
             db_name='test_pgtools',
             port=self.port,
         )
         self.database.create_user()
-        with pytest.raises(Exception):
+        with pytest.raises(Exception):  # noqa: B017
             self.database.create_user()
 
     def test_ensure_user_exists(self):
         """
         ensure_user should not fail if user already exists
         """
         self.database = pgtools.PostgresDatabase(
@@ -307,24 +297,22 @@
 
     def test___init__ok(self):
         self.dbms = pgtools.PostgresServer(host='localhost', port=UNUSED_PORT)
 
     def test___repr__(self):
         self.dbms = pgtools.PostgresServer(host='localhost', port=UNUSED_PORT)
         assert repr(self.dbms) == (
-            'PostgresServer(host=localhost, port=%s, '
-            'base_pathname=%s, superuser=%s)'
-            % (self.dbms.port, self.dbms.base_pathname, self.dbms.superuser)
+            f'PostgresServer(host=localhost, port={self.dbms.port}, '
+            f'base_pathname={self.dbms.base_pathname}, superuser={self.dbms.superuser})'
         )
 
     def test___str__(self):
         self.dbms = pgtools.PostgresServer(host='localhost', port=UNUSED_PORT)
         assert str(self.dbms) == (
-            'PostgreSQL server at %s:%s (with storage at %s)'
-            % (self.dbms.host, self.dbms.port, self.dbms.base_pathname)
+            f'PostgreSQL server at {self.dbms.host}:{self.dbms.port} (with storage at {self.dbms.base_pathname})'
         )
 
     def test_destroy_handles_deleted_directory(self):
         self.dbms = pgtools.PostgresServer(host='localhost', port=UNUSED_PORT)
         self.dbms.initdb()
         # Reach under the covers and pre-emptively delete the directory.
         # (But first, some checking to prevent hideously
```

