# Comparing `tmp/jaraco.timing-2.0.tar.gz` & `tmp/jaraco.timing-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmp68r9jzts/jaraco.timing-2.0.tar", last modified: Tue Jan  1 16:07:40 2019, max compression
+gzip compressed data, was "jaraco.timing-3.0.0.tar", last modified: Tue Apr  2 20:43:22 2024, max compression
```

## Comparing `jaraco.timing-2.0.tar` & `jaraco.timing-3.0.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-01 16:07:40.000000 jaraco.timing-2.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      214 2019-01-01 16:07:21.000000 jaraco.timing-2.0/.flake8
--rw-rw-r--   0 travis    (2000) travis    (2000)       74 2019-01-01 16:07:21.000000 jaraco.timing-2.0/.readthedocs.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1299 2019-01-01 16:07:21.000000 jaraco.timing-2.0/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      703 2019-01-01 16:07:21.000000 jaraco.timing-2.0/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2019-01-01 16:07:21.000000 jaraco.timing-2.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1439 2019-01-01 16:07:40.000000 jaraco.timing-2.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      719 2019-01-01 16:07:21.000000 jaraco.timing-2.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      454 2019-01-01 16:07:21.000000 jaraco.timing-2.0/appveyor.yml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-01 16:07:40.000000 jaraco.timing-2.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      755 2019-01-01 16:07:21.000000 jaraco.timing-2.0/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-01-01 16:07:21.000000 jaraco.timing-2.0/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      305 2019-01-01 16:07:21.000000 jaraco.timing-2.0/docs/index.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-01 16:07:40.000000 jaraco.timing-2.0/jaraco/
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2019-01-01 16:07:21.000000 jaraco.timing-2.0/jaraco/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      177 2019-01-01 16:07:21.000000 jaraco.timing-2.0/jaraco/timing.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-01 16:07:40.000000 jaraco.timing-2.0/jaraco.timing.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1439 2019-01-01 16:07:40.000000 jaraco.timing-2.0/jaraco.timing.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      422 2019-01-01 16:07:40.000000 jaraco.timing-2.0/jaraco.timing.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-01-01 16:07:40.000000 jaraco.timing-2.0/jaraco.timing.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2019-01-01 16:07:40.000000 jaraco.timing-2.0/jaraco.timing.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-01-01 16:07:40.000000 jaraco.timing-2.0/jaraco.timing.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2019-01-01 16:07:21.000000 jaraco.timing-2.0/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      456 2019-01-01 16:07:21.000000 jaraco.timing-2.0/pytest.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      903 2019-01-01 16:07:40.000000 jaraco.timing-2.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2019-01-01 16:07:21.000000 jaraco.timing-2.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7408 2019-01-01 16:07:21.000000 jaraco.timing-2.0/skeleton.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2019-01-01 16:07:21.000000 jaraco.timing-2.0/test_all.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      553 2019-01-01 16:07:21.000000 jaraco.timing-2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:43:22.859148 jaraco.timing-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:43:22.855148 jaraco.timing-3.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:43:22.855148 jaraco.timing-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-02 20:43:22.859148 jaraco.timing-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:43:22.855148 jaraco.timing-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:43:22.855148 jaraco.timing-3.0.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/jaraco/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:43:22.855148 jaraco.timing-3.0.0/jaraco.timing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-02 20:43:22.000000 jaraco.timing-3.0.0/jaraco.timing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-02 20:43:22.000000 jaraco.timing-3.0.0/jaraco.timing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:43:22.000000 jaraco.timing-3.0.0/jaraco.timing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-02 20:43:22.000000 jaraco.timing-3.0.0/jaraco.timing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 20:43:22.000000 jaraco.timing-3.0.0/jaraco.timing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-02 20:43:22.859148 jaraco.timing-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-02 20:43:08.000000 jaraco.timing-3.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jaraco.timing-2.0/CHANGES.rst` & `jaraco.timing-3.0.0/NEWS.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v3.0.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
+Deprecations and Removals
+-------------------------
+
+- Removed all functionality.
+
+
 2.0
 ===
 
 Switch to `pkgutil namespace technique
 <https://packaging.python.org/guides/packaging-namespace-packages/#pkgutil-style-namespace-packages>`_
 for the ``jaraco`` namespace.
```

### Comparing `jaraco.timing-2.0/docs/conf.py` & `jaraco.timing-3.0.0/docs/conf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,42 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ["sphinx.ext.autodoc", "jaraco.packaging.sphinx", "rst.linker"]
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    "../CHANGES.rst": dict(
-        using=dict(GH="https://github.com"),
+    '../NEWS.rst': dict(
+        using=dict(GH='https://github.com'),
         replace=[
             dict(
-                pattern=r"(Issue #|\B#)(?P<issue>\d+)",
-                url="{package_url}/issues/{issue}",
+                pattern=r'(Issue #|\B#)(?P<issue>\d+)',
+                url='{package_url}/issues/{issue}',
             ),
             dict(
-                pattern=r"^(?m)((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n",
-                with_scm="{text}\n{rev[timestamp]:%d %b %Y}\n",
+                pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
+                with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
-                pattern=r"PEP[- ](?P<pep_number>\d+)",
-                url="https://www.python.org/dev/peps/pep-{pep_number:0>4}/",
+                pattern=r'PEP[- ](?P<pep_number>\d+)',
+                url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
         ],
     )
 }
+
+# Be strict about any broken references
+nitpicky = True
+
+# Include Python intersphinx mapping to prevent failures
+# jaraco/skeleton#51
+extensions += ['sphinx.ext.intersphinx']
+intersphinx_mapping = {
+    'python': ('https://docs.python.org/3', None),
+}
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
```

### Comparing `jaraco.timing-2.0/setup.cfg` & `jaraco.timing-3.0.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-[bdist_wheel]
-universal = 1
-
 [metadata]
-license_file = LICENSE
 name = jaraco.timing
 author = Jason R. Coombs
 author_email = jaraco@jaraco.com
 description = Routines for quick and dirty profiling and rate limits
 long_description = file:README.rst
 url = https://github.com/jaraco/jaraco.timing
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
-	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
 
 [options]
-packages = find:
 include_package_data = true
-python_requires = >=2.7
+python_requires = >=3.8
 install_requires = 
 	tempora >= 1.5
-setup_requires = setuptools_scm >= 1.15.0
 
 [options.extras_require]
 testing = 
-	pytest >= 3.5, !=3.7.3
-	pytest-checkdocs
-	pytest-flake8
+	pytest >= 6, != 8.1.1
+	pytest-checkdocs >= 2.4
+	pytest-cov
+	pytest-mypy
+	pytest-enabler >= 2.2
+	pytest-ruff >= 0.2.1
 	
 	backports.unittest_mock
 docs = 
-	sphinx
-	jaraco.packaging >= 3.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

