# Comparing `tmp/psrqpy-1.2.8.tar.gz` & `tmp/psrqpy-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/psrqpy/psrqpy/dist/.tmp-0bzdpusq/psrqpy-1.2.8.tar", last modified: Fri Feb 16 21:11:02 2024, max compression
+gzip compressed data, was "/home/runner/work/psrqpy/psrqpy/dist/.tmp-n5qd70ga/psrqpy-1.2.9.tar", last modified: Tue Apr  2 15:10:25 2024, max compression
```

## Comparing `psrqpy-1.2.8.tar` & `psrqpy-1.2.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:11:02.000000 psrqpy-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-16 21:10:50.000000 psrqpy-1.2.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:11:02.000000 psrqpy-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:11:02.000000 psrqpy-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-02-16 21:10:50.000000 psrqpy-1.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-16 21:10:50.000000 psrqpy-1.2.8/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-16 21:10:50.000000 psrqpy-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-16 21:10:50.000000 psrqpy-1.2.8/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-16 21:10:50.000000 psrqpy-1.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-02-16 21:10:50.000000 psrqpy-1.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-16 21:10:50.000000 psrqpy-1.2.8/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-16 21:10:50.000000 psrqpy-1.2.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-16 21:10:50.000000 psrqpy-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-02-16 21:11:02.000000 psrqpy-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-02-16 21:10:50.000000 psrqpy-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:11:02.000000 psrqpy-1.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-02-16 21:10:50.000000 psrqpy-1.2.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:11:02.000000 psrqpy-1.2.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-02-16 21:10:50.000000 psrqpy-1.2.8/docs/source/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-02-16 21:10:50.000000 psrqpy-1.2.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-16 21:10:50.000000 psrqpy-1.2.8/docs/source/config.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:11:02.000000 psrqpy-1.2.8/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (127)   187239 2024-02-16 21:10:50.000000 psrqpy-1.2.8/docs/source/images/PvsPdot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   141497 2024-02-16 21:10:50.000000 psrqpy-1.2.8/docs/source/images/ppdot.png
--rw-r--r--   0 runner    (1001) docker     (127)    18282 2024-02-16 21:10:50.000000 psrqpy-1.2.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-16 21:10:50.000000 psrqpy-1.2.8/docs/source/pulsar.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-16 21:10:50.000000 psrqpy-1.2.8/docs/source/query.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-16 21:10:50.000000 psrqpy-1.2.8/docs/source/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:11:02.000000 psrqpy-1.2.8/paper/
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-16 21:10:50.000000 psrqpy-1.2.8/paper/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-02-16 21:10:50.000000 psrqpy-1.2.8/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-16 21:10:50.000000 psrqpy-1.2.8/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-02-16 21:10:50.000000 psrqpy-1.2.8/paper/paper.tex
--rw-r--r--   0 runner    (1001) docker     (127)   141497 2024-02-16 21:10:50.000000 psrqpy-1.2.8/paper/ppdot.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:11:02.000000 psrqpy-1.2.8/psrqpy/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-16 21:10:50.000000 psrqpy-1.2.8/psrqpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-16 21:11:02.000000 psrqpy-1.2.8/psrqpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    21298 2024-02-16 21:10:50.000000 psrqpy-1.2.8/psrqpy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-02-16 21:10:50.000000 psrqpy-1.2.8/psrqpy/pulsar.py
--rw-r--r--   0 runner    (1001) docker     (127)   122264 2024-02-16 21:10:50.000000 psrqpy-1.2.8/psrqpy/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:11:02.000000 psrqpy-1.2.8/psrqpy/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 21:10:50.000000 psrqpy-1.2.8/psrqpy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-16 21:10:50.000000 psrqpy-1.2.8/psrqpy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-02-16 21:10:50.000000 psrqpy-1.2.8/psrqpy/tests/derived_catalogue.db
--rw-r--r--   0 runner    (1001) docker     (127)    28441 2024-02-16 21:10:50.000000 psrqpy-1.2.8/psrqpy/tests/query_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-02-16 21:10:50.000000 psrqpy-1.2.8/psrqpy/tests/test_catalogue.db
--rw-r--r--   0 runner    (1001) docker     (127)    76523 2024-02-16 21:10:50.000000 psrqpy-1.2.8/psrqpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:11:02.000000 psrqpy-1.2.8/psrqpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-02-16 21:11:02.000000 psrqpy-1.2.8/psrqpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-16 21:11:02.000000 psrqpy-1.2.8/psrqpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 21:11:02.000000 psrqpy-1.2.8/psrqpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-16 21:11:02.000000 psrqpy-1.2.8/psrqpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-16 21:11:02.000000 psrqpy-1.2.8/psrqpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-16 21:10:50.000000 psrqpy-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-16 21:10:50.000000 psrqpy-1.2.8/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-02-16 21:11:02.000000 psrqpy-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-16 21:10:50.000000 psrqpy-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:10:25.000000 psrqpy-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 15:10:16.000000 psrqpy-1.2.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:10:25.000000 psrqpy-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:10:25.000000 psrqpy-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-02 15:10:16.000000 psrqpy-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-02 15:10:16.000000 psrqpy-1.2.9/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 15:10:16.000000 psrqpy-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 15:10:16.000000 psrqpy-1.2.9/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-02 15:10:16.000000 psrqpy-1.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-02 15:10:16.000000 psrqpy-1.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-02 15:10:16.000000 psrqpy-1.2.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-02 15:10:16.000000 psrqpy-1.2.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 15:10:16.000000 psrqpy-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-04-02 15:10:25.000000 psrqpy-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-02 15:10:16.000000 psrqpy-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:10:25.000000 psrqpy-1.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-04-02 15:10:16.000000 psrqpy-1.2.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:10:25.000000 psrqpy-1.2.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-02 15:10:16.000000 psrqpy-1.2.9/docs/source/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-02 15:10:16.000000 psrqpy-1.2.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-02 15:10:16.000000 psrqpy-1.2.9/docs/source/config.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:10:25.000000 psrqpy-1.2.9/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   187239 2024-04-02 15:10:16.000000 psrqpy-1.2.9/docs/source/images/PvsPdot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   141497 2024-04-02 15:10:16.000000 psrqpy-1.2.9/docs/source/images/ppdot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18282 2024-04-02 15:10:16.000000 psrqpy-1.2.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 15:10:16.000000 psrqpy-1.2.9/docs/source/pulsar.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 15:10:16.000000 psrqpy-1.2.9/docs/source/query.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-02 15:10:16.000000 psrqpy-1.2.9/docs/source/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:10:25.000000 psrqpy-1.2.9/paper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-02 15:10:16.000000 psrqpy-1.2.9/paper/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-02 15:10:16.000000 psrqpy-1.2.9/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-02 15:10:16.000000 psrqpy-1.2.9/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-02 15:10:16.000000 psrqpy-1.2.9/paper/paper.tex
+-rw-r--r--   0 runner    (1001) docker     (127)   141497 2024-04-02 15:10:16.000000 psrqpy-1.2.9/paper/ppdot.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:10:25.000000 psrqpy-1.2.9/psrqpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-02 15:10:16.000000 psrqpy-1.2.9/psrqpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 15:10:25.000000 psrqpy-1.2.9/psrqpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-04-02 15:10:16.000000 psrqpy-1.2.9/psrqpy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-02 15:10:16.000000 psrqpy-1.2.9/psrqpy/pulsar.py
+-rw-r--r--   0 runner    (1001) docker     (127)   122264 2024-04-02 15:10:16.000000 psrqpy-1.2.9/psrqpy/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:10:25.000000 psrqpy-1.2.9/psrqpy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:10:16.000000 psrqpy-1.2.9/psrqpy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-02 15:10:16.000000 psrqpy-1.2.9/psrqpy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-02 15:10:16.000000 psrqpy-1.2.9/psrqpy/tests/derived_catalogue.db
+-rw-r--r--   0 runner    (1001) docker     (127)    28588 2024-04-02 15:10:16.000000 psrqpy-1.2.9/psrqpy/tests/query_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-02 15:10:16.000000 psrqpy-1.2.9/psrqpy/tests/test_catalogue.db
+-rw-r--r--   0 runner    (1001) docker     (127)    76523 2024-04-02 15:10:16.000000 psrqpy-1.2.9/psrqpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:10:25.000000 psrqpy-1.2.9/psrqpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-04-02 15:10:25.000000 psrqpy-1.2.9/psrqpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 15:10:25.000000 psrqpy-1.2.9/psrqpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:10:25.000000 psrqpy-1.2.9/psrqpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-02 15:10:25.000000 psrqpy-1.2.9/psrqpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 15:10:25.000000 psrqpy-1.2.9/psrqpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-02 15:10:16.000000 psrqpy-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 15:10:16.000000 psrqpy-1.2.9/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-02 15:10:25.000000 psrqpy-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 15:10:16.000000 psrqpy-1.2.9/setup.py
```

### Comparing `psrqpy-1.2.8/.github/workflows/build.yml` & `psrqpy-1.2.9/.github/workflows/build.yml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     - cron: "0 0 * * *"
 
 jobs:
   build:
     strategy:
       matrix:
         os: [ubuntu-20.04]
-        python-version: [3.7, 3.8, 3.9, "3.10", "3.11"]
+        python-version: [3.8, 3.9, "3.10", "3.11"]
     runs-on: ${{ matrix.os }}
     defaults:
       run:
         shell: bash -l {0}
 
     steps:
     - uses: actions/checkout@v3
```

### Comparing `psrqpy-1.2.8/.github/workflows/pypi.yml` & `psrqpy-1.2.9/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/CHANGELOG.md` & `psrqpy-1.2.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Notable changes between versions
 
+## [1.2.9] 2024-04-02
+
+- Update the Galactic MSP table URL. See [#135](https://github.com/mattpitkin/psrqpy/issues/135).
+
 ## [1.2.8] 2024-02-16
 
 - Fix extracting the ATNF catalogue version number from the database file for v2.0.0 of the catalogue. See [#132](https://github.com/mattpitkin/psrqpy/pull/132).
 
 ## [1.2.7] 2023-05-19
 
 - Fix URL for the Globular Cluster pulsar catalogue, which recently moved to [here](https://www3.mpifr-bonn.mpg.de/staff/pfreire/GCpsr.txt). See [#123](https://github.com/mattpitkin/psrqpy/issues/123).
```

### Comparing `psrqpy-1.2.8/CITATION.cff` & `psrqpy-1.2.9/CITATION.cff`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/Dockerfile` & `psrqpy-1.2.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/LICENSE` & `psrqpy-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/PKG-INFO` & `psrqpy-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psrqpy
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Python module for querying the ATNF pulsar catalogue
 Home-page: https://github.com/mattpitkin/psrqpy
 Author: Matthew Pitkin
 Author-email: matthew.pitkin@ligo.org
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `psrqpy-1.2.8/README.md` & `psrqpy-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/docs/Makefile` & `psrqpy-1.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/docs/source/CHANGELOG.md` & `psrqpy-1.2.9/docs/source/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Notable changes between versions
 
+## [1.2.9] 2024-04-02
+
+- Update the Galactic MSP table URL. See [#135](https://github.com/mattpitkin/psrqpy/issues/135).
+
 ## [1.2.8] 2024-02-16
 
 - Fix extracting the ATNF catalogue version number from the database file for v2.0.0 of the catalogue. See [#132](https://github.com/mattpitkin/psrqpy/pull/132).
 
 ## [1.2.7] 2023-05-19
 
 - Fix URL for the Globular Cluster pulsar catalogue, which recently moved to [here](https://www3.mpifr-bonn.mpg.de/staff/pfreire/GCpsr.txt). See [#123](https://github.com/mattpitkin/psrqpy/issues/123).
```

### Comparing `psrqpy-1.2.8/docs/source/conf.py` & `psrqpy-1.2.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/docs/source/images/PvsPdot.ipynb` & `psrqpy-1.2.9/docs/source/images/PvsPdot.ipynb`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/docs/source/images/ppdot.png` & `psrqpy-1.2.9/docs/source/images/ppdot.png`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/docs/source/index.rst` & `psrqpy-1.2.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/paper/Makefile` & `psrqpy-1.2.9/paper/Makefile`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/paper/paper.bib` & `psrqpy-1.2.9/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/paper/paper.md` & `psrqpy-1.2.9/paper/paper.md`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/paper/paper.tex` & `psrqpy-1.2.9/paper/paper.tex`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/paper/ppdot.png` & `psrqpy-1.2.9/paper/ppdot.png`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/psrqpy/__init__.py` & `psrqpy-1.2.9/psrqpy/__init__.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/psrqpy/config.py` & `psrqpy-1.2.9/psrqpy/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 #: The Jodrell Bank glitch catalogue table URL.
 GLITCH_URL = r"https://www.jb.man.ac.uk/pulsar/glitches/gTable.html"
 
 #: Paolo Freire's globular cluster pulsar table URL
 GC_URL = r"https://www3.mpifr-bonn.mpg.de/staff/pfreire/GCpsr.txt"
 
-#: Dunc Lorimer's MSP table URL
-MSP_URL = r"http://astro.phys.wvu.edu/GalacticMSPs/GalacticMSPs.txt"
+#: MSP table URL (maintained by Elizabeth Ferrara)
+MSP_URL = r"https://www.astro.umd.edu/~eferrara/pulsars/GalacticMSPs.txt"
 
 # Pulsar parameters (http://www.atnf.csiro.au/research/pulsar/psrcat/psrcat_help.html) that can be
 # queried. For each parameter there is a dictionary giving:
 #  - 'ref': True if the parameter can have an associated reference in the ATNF catalogue
 #  - 'err': True if the parameter can have an associated error value
 #  - 'unit': a string giving the units for the parameter (to be used if generating an astropy table)
 PSR_GENERAL = dict()
```

### Comparing `psrqpy-1.2.8/psrqpy/pulsar.py` & `psrqpy-1.2.9/psrqpy/pulsar.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/psrqpy/search.py` & `psrqpy-1.2.9/psrqpy/search.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/psrqpy/tests/derived_catalogue.db` & `psrqpy-1.2.9/psrqpy/tests/derived_catalogue.db`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/psrqpy/tests/query_test.py` & `psrqpy-1.2.9/psrqpy/tests/query_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,14 +275,17 @@
 
 
 def test_num_pulsars(query):
     """
     Test that the number of pulsars returned is as expected.
     """
 
+    # store all pulsar names
+    psrs = query["PSRJ"].tolist()
+
     query.psrs = 'J9999+9999'  # bad pulsar
 
     # length should be zero
     with pytest.warns(UserWarning):
         lq = len(query)
 
     assert lq == 0
@@ -292,14 +295,18 @@
     # length should be one
     assert len(query) == 1
 
     query.psrs = ['J0534+2200', 'J0537-6910']
 
     # length should be two
     assert len(query) == 2
+    
+    # reset pulsars
+    query.psrs = psrs
+    assert len(query) == len(psrs)
 
 
 def test_num_columns(query):
     """
     Test that the number of columns if correct.
     """
 
@@ -1010,7 +1017,8 @@
     """
 
     psr = query.get_pulsar("J0034-0721")  # This pulsar has a BName and a JName
     assert psr["NAME"][0] == psr["BNAME"][0]
 
     psr = query.get_pulsar("J1906+1854")  # This pulsar only has a JName
     assert psr["NAME"][0] == psr["JNAME"][0]
+
```

### Comparing `psrqpy-1.2.8/psrqpy/tests/test_catalogue.db` & `psrqpy-1.2.9/psrqpy/tests/test_catalogue.db`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/psrqpy/utils.py` & `psrqpy-1.2.9/psrqpy/utils.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/psrqpy.egg-info/PKG-INFO` & `psrqpy-1.2.9/psrqpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psrqpy
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Python module for querying the ATNF pulsar catalogue
 Home-page: https://github.com/mattpitkin/psrqpy
 Author: Matthew Pitkin
 Author-email: matthew.pitkin@ligo.org
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `psrqpy-1.2.8/psrqpy.egg-info/SOURCES.txt` & `psrqpy-1.2.9/psrqpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.8/setup.cfg` & `psrqpy-1.2.9/setup.cfg`

 * *Files identical despite different names*

