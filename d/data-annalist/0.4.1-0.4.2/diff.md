# Comparing `tmp/data-annalist-0.4.1.tar.gz` & `tmp/data-annalist-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-annalist-0.4.1.tar", last modified: Tue Feb 13 03:39:20 2024, max compression
+gzip compressed data, was "data-annalist-0.4.2.tar", last modified: Tue Apr  2 02:03:10 2024, max compression
```

## Comparing `data-annalist-0.4.1.tar` & `data-annalist-0.4.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-02-13 03:39:20.182872 data-annalist-0.4.1/
--rw-r--r--   0 nic       (1000) nic       (1000)      292 2023-09-22 02:26:01.000000 data-annalist-0.4.1/.editorconfig
--rw-r--r--   0 nic       (1000) nic       (1000)     1204 2023-09-22 02:26:01.000000 data-annalist-0.4.1/.gitignore
--rw-r--r--   0 nic       (1000) nic       (1000)      514 2024-02-13 02:37:10.000000 data-annalist-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     1068 2024-02-13 03:24:37.000000 data-annalist-0.4.1/.readthedocs.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)      169 2023-09-22 02:26:01.000000 data-annalist-0.4.1/AUTHORS.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     6708 2024-02-13 02:40:11.000000 data-annalist-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1269 2024-02-13 03:37:19.000000 data-annalist-0.4.1/HISTORY.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1563 2023-09-25 00:32:51.000000 data-annalist-0.4.1/LICENSE
--rw-r--r--   0 nic       (1000) nic       (1000)      262 2023-09-22 02:26:01.000000 data-annalist-0.4.1/MANIFEST.in
--rw-r--r--   0 nic       (1000) nic       (1000)     2495 2024-02-13 03:16:18.000000 data-annalist-0.4.1/Makefile
--rw-r--r--   0 nic       (1000) nic       (1000)    17763 2024-02-13 03:39:20.182872 data-annalist-0.4.1/PKG-INFO
--rw-r--r--   0 nic       (1000) nic       (1000)    16215 2024-02-13 02:40:30.000000 data-annalist-0.4.1/README.rst
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-02-13 03:39:20.182872 data-annalist-0.4.1/annalist/
--rw-r--r--   0 nic       (1000) nic       (1000)      139 2024-02-13 03:35:52.000000 data-annalist-0.4.1/annalist/__init__.py
--rw-r--r--   0 nic       (1000) nic       (1000)    11650 2024-02-13 02:31:50.000000 data-annalist-0.4.1/annalist/annalist.py
--rw-r--r--   0 nic       (1000) nic       (1000)    14103 2024-02-13 02:31:50.000000 data-annalist-0.4.1/annalist/decorators.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-02-13 03:39:20.182872 data-annalist-0.4.1/data_annalist.egg-info/
--rw-r--r--   0 nic       (1000) nic       (1000)    17763 2024-02-13 03:39:20.000000 data-annalist-0.4.1/data_annalist.egg-info/PKG-INFO
--rw-r--r--   0 nic       (1000) nic       (1000)      885 2024-02-13 03:39:20.000000 data-annalist-0.4.1/data_annalist.egg-info/SOURCES.txt
--rw-r--r--   0 nic       (1000) nic       (1000)        1 2024-02-13 03:39:20.000000 data-annalist-0.4.1/data_annalist.egg-info/dependency_links.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      217 2024-02-13 03:39:20.000000 data-annalist-0.4.1/data_annalist.egg-info/requires.txt
--rw-r--r--   0 nic       (1000) nic       (1000)        9 2024-02-13 03:39:20.000000 data-annalist-0.4.1/data_annalist.egg-info/top_level.txt
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-02-13 03:39:20.182872 data-annalist-0.4.1/docs/
--rw-r--r--   0 nic       (1000) nic       (1000)      611 2023-09-22 02:26:01.000000 data-annalist-0.4.1/docs/Makefile
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-02-13 03:39:20.172872 data-annalist-0.4.1/docs/_build/
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-02-13 03:39:20.172872 data-annalist-0.4.1/docs/_build/html/
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-02-13 03:39:20.182872 data-annalist-0.4.1/docs/_build/html/_static/
--rw-r--r--   0 nic       (1000) nic       (1000)      286 2023-09-22 02:32:07.000000 data-annalist-0.4.1/docs/_build/html/_static/file.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-09-22 02:32:07.000000 data-annalist-0.4.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-09-22 02:32:07.000000 data-annalist-0.4.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 nic       (1000) nic       (1000)      310 2023-11-20 20:08:22.000000 data-annalist-0.4.1/docs/annalist.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-22 02:26:01.000000 data-annalist-0.4.1/docs/authors.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     4840 2023-11-20 20:05:59.000000 data-annalist-0.4.1/docs/conf.py
--rw-r--r--   0 nic       (1000) nic       (1000)       33 2023-09-22 02:26:01.000000 data-annalist-0.4.1/docs/contributing.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-22 02:26:01.000000 data-annalist-0.4.1/docs/history.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      305 2023-09-22 03:45:29.000000 data-annalist-0.4.1/docs/index.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1130 2023-09-22 03:46:29.000000 data-annalist-0.4.1/docs/installation.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      770 2023-09-22 03:47:10.000000 data-annalist-0.4.1/docs/make.bat
--rw-r--r--   0 nic       (1000) nic       (1000)       61 2023-11-20 20:08:22.000000 data-annalist-0.4.1/docs/modules.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       27 2023-09-22 02:26:01.000000 data-annalist-0.4.1/docs/readme.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       71 2023-09-22 03:48:02.000000 data-annalist-0.4.1/docs/usage.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1481 2023-11-20 20:07:53.000000 data-annalist-0.4.1/old_requirements_dev.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      384 2023-11-28 22:09:53.000000 data-annalist-0.4.1/old_setup.cfg
--rw-r--r--   0 nic       (1000) nic       (1000)     1212 2024-02-13 01:56:04.000000 data-annalist-0.4.1/old_setup.py
--rw-r--r--   0 nic       (1000) nic       (1000)     2859 2024-02-13 03:35:52.000000 data-annalist-0.4.1/pyproject.toml
--rw-r--r--   0 nic       (1000) nic       (1000)       38 2024-02-13 03:39:20.182872 data-annalist-0.4.1/setup.cfg
--rw-r--r--   0 nic       (1000) nic       (1000)     5198 2024-02-13 02:31:50.000000 data-annalist-0.4.1/temp_file.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-02-13 03:39:20.182872 data-annalist-0.4.1/tests/
--rw-r--r--   0 nic       (1000) nic       (1000)       38 2023-09-22 03:38:37.000000 data-annalist-0.4.1/tests/__init__.py
--rw-r--r--   0 nic       (1000) nic       (1000)     3372 2024-02-13 02:31:45.000000 data-annalist-0.4.1/tests/example_class.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1905 2024-02-13 02:31:50.000000 data-annalist-0.4.1/tests/example_script.py
--rw-r--r--   0 nic       (1000) nic       (1000)    94181 2023-11-19 19:10:48.000000 data-annalist-0.4.1/tests/logfile.txt
--rw-r--r--   0 nic       (1000) nic       (1000)    17593 2024-02-13 03:12:16.000000 data-annalist-0.4.1/tests/test_annalist.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.631655 data-annalist-0.4.2/
+-rw-r--r--   0 nic       (1000) nic       (1000)      292 2023-09-22 02:26:01.000000 data-annalist-0.4.2/.editorconfig
+-rw-r--r--   0 nic       (1000) nic       (1000)     1204 2023-09-22 02:26:01.000000 data-annalist-0.4.2/.gitignore
+-rw-r--r--   0 nic       (1000) nic       (1000)      514 2024-02-13 20:04:40.000000 data-annalist-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)     1068 2024-02-13 03:24:37.000000 data-annalist-0.4.2/.readthedocs.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)      169 2023-09-22 02:26:01.000000 data-annalist-0.4.2/AUTHORS.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     6708 2024-02-13 02:40:11.000000 data-annalist-0.4.2/CONTRIBUTING.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1357 2024-04-02 02:01:16.000000 data-annalist-0.4.2/HISTORY.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1563 2023-09-25 00:32:51.000000 data-annalist-0.4.2/LICENSE
+-rw-r--r--   0 nic       (1000) nic       (1000)      262 2023-09-22 02:26:01.000000 data-annalist-0.4.2/MANIFEST.in
+-rw-r--r--   0 nic       (1000) nic       (1000)     2495 2024-02-13 03:16:18.000000 data-annalist-0.4.2/Makefile
+-rw-r--r--   0 nic       (1000) nic       (1000)    17785 2024-04-02 02:03:10.631655 data-annalist-0.4.2/PKG-INFO
+-rw-r--r--   0 nic       (1000) nic       (1000)    16237 2024-02-13 19:35:12.000000 data-annalist-0.4.2/README.rst
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.571655 data-annalist-0.4.2/annalist/
+-rw-r--r--   0 nic       (1000) nic       (1000)      139 2024-04-02 01:58:24.000000 data-annalist-0.4.2/annalist/__init__.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    11650 2024-02-13 02:31:50.000000 data-annalist-0.4.2/annalist/annalist.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    14103 2024-02-13 02:31:50.000000 data-annalist-0.4.2/annalist/decorators.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.621655 data-annalist-0.4.2/data_annalist.egg-info/
+-rw-r--r--   0 nic       (1000) nic       (1000)    17785 2024-04-02 02:03:10.000000 data-annalist-0.4.2/data_annalist.egg-info/PKG-INFO
+-rw-r--r--   0 nic       (1000) nic       (1000)      885 2024-04-02 02:03:10.000000 data-annalist-0.4.2/data_annalist.egg-info/SOURCES.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)        1 2024-04-02 02:03:10.000000 data-annalist-0.4.2/data_annalist.egg-info/dependency_links.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)      217 2024-04-02 02:03:10.000000 data-annalist-0.4.2/data_annalist.egg-info/requires.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)        9 2024-04-02 02:03:10.000000 data-annalist-0.4.2/data_annalist.egg-info/top_level.txt
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.571655 data-annalist-0.4.2/docs/
+-rw-r--r--   0 nic       (1000) nic       (1000)      611 2023-09-22 02:26:01.000000 data-annalist-0.4.2/docs/Makefile
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.561655 data-annalist-0.4.2/docs/_build/
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.561655 data-annalist-0.4.2/docs/_build/html/
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.611655 data-annalist-0.4.2/docs/_build/html/_static/
+-rw-r--r--   0 nic       (1000) nic       (1000)      286 2023-09-22 02:32:07.000000 data-annalist-0.4.2/docs/_build/html/_static/file.png
+-rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-09-22 02:32:07.000000 data-annalist-0.4.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-09-22 02:32:07.000000 data-annalist-0.4.2/docs/_build/html/_static/plus.png
+-rw-r--r--   0 nic       (1000) nic       (1000)      310 2023-11-20 20:08:22.000000 data-annalist-0.4.2/docs/annalist.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-22 02:26:01.000000 data-annalist-0.4.2/docs/authors.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     4840 2023-11-20 20:05:59.000000 data-annalist-0.4.2/docs/conf.py
+-rw-r--r--   0 nic       (1000) nic       (1000)       33 2023-09-22 02:26:01.000000 data-annalist-0.4.2/docs/contributing.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-22 02:26:01.000000 data-annalist-0.4.2/docs/history.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)      305 2023-09-22 03:45:29.000000 data-annalist-0.4.2/docs/index.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1239 2024-02-13 19:34:51.000000 data-annalist-0.4.2/docs/installation.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)      770 2023-09-22 03:47:10.000000 data-annalist-0.4.2/docs/make.bat
+-rw-r--r--   0 nic       (1000) nic       (1000)       61 2023-11-20 20:08:22.000000 data-annalist-0.4.2/docs/modules.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       27 2023-09-22 02:26:01.000000 data-annalist-0.4.2/docs/readme.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       71 2023-09-22 03:48:02.000000 data-annalist-0.4.2/docs/usage.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1481 2023-11-20 20:07:53.000000 data-annalist-0.4.2/old_requirements_dev.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)      384 2023-11-28 22:09:53.000000 data-annalist-0.4.2/old_setup.cfg
+-rw-r--r--   0 nic       (1000) nic       (1000)     1212 2024-02-13 01:56:04.000000 data-annalist-0.4.2/old_setup.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     2859 2024-04-02 01:59:26.000000 data-annalist-0.4.2/pyproject.toml
+-rw-r--r--   0 nic       (1000) nic       (1000)       38 2024-04-02 02:03:10.631655 data-annalist-0.4.2/setup.cfg
+-rw-r--r--   0 nic       (1000) nic       (1000)     5198 2024-02-13 02:31:50.000000 data-annalist-0.4.2/temp_file.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.621655 data-annalist-0.4.2/tests/
+-rw-r--r--   0 nic       (1000) nic       (1000)       38 2023-09-22 03:38:37.000000 data-annalist-0.4.2/tests/__init__.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     3372 2024-02-13 02:31:45.000000 data-annalist-0.4.2/tests/example_class.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1905 2024-02-13 02:31:50.000000 data-annalist-0.4.2/tests/example_script.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    94181 2023-11-19 19:10:48.000000 data-annalist-0.4.2/tests/logfile.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)    17593 2024-02-13 03:12:16.000000 data-annalist-0.4.2/tests/test_annalist.py
```

### Comparing `data-annalist-0.4.1/.gitignore` & `data-annalist-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/.pre-commit-config.yaml` & `data-annalist-0.4.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.5.0
   hooks:
   - id: check-yaml
   - id: end-of-file-fixer
   - id: trailing-whitespace
 - repo: https://github.com/psf/black
-  rev: 24.1.1
+  rev: 24.2.0
   hooks:
   - id: black
 - repo: https://github.com/PyCQA/bandit
   rev: 1.7.7
   hooks:
   - id: bandit
     args: ["-r", "-lll"]
```

### Comparing `data-annalist-0.4.1/.readthedocs.yaml` & `data-annalist-0.4.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/CONTRIBUTING.rst` & `data-annalist-0.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/HISTORY.rst` & `data-annalist-0.4.2/HISTORY.rst`

 * *Files 19% similar despite different names*

```diff
@@ -55,7 +55,12 @@
 * Fixed bug relating to method identity crisis (decorated functions thought they were their decorators).
 
 0.4.1 (2024-02-13)
 ------------------
 
 * Fixed pyproject.toml package
 * Updated .readthedocs.yaml to reflect changes in pyproject.toml
+
+0.4.2 (2024-04-02)
+------------------
+
+* Relaxed Python dependency from 3.11.6 to 3.11
```

### Comparing `data-annalist-0.4.1/LICENSE` & `data-annalist-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/Makefile` & `data-annalist-0.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/PKG-INFO` & `data-annalist-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: data-annalist
-Version: 0.4.1
+Version: 0.4.2
 Summary: Audit trail generator for data processing scripts.
 Author-email: Nic Mostert <nicolas.mostert@horizons.govt.nz>
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/nicmostert/annalist
 Project-URL: Issues, https://github.com/nicmostert/annalist/issues
 Project-URL: Documentation, https://annalist.readthedocs.io
 Project-URL: Package, https://pypi.org/project/data-annalist
 Keywords: logging, auditing, audit trail, hydrology, automation, hilltop, hydrobot, HorizonsRC
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: ==3.11.6
+Requires-Python: ==3.11.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Provides-Extra: test
 Requires-Dist: pytest>=7.4.2; extra == "test"
 Requires-Dist: pytest-cov>=4.1.0; extra == "test"
 Provides-Extra: dev
@@ -104,17 +104,15 @@
         # DO NOT put it on the __repr__ either.
         # Same as before, this creates infinite recursion.
         def __repr__(self):
             return f"{str(arg1)}: {str(arg2)}"
 
 In the main script, the Annalist object must be called again. This will point to the singleton object initialized in the dependency. The annalist must be configured before usage.
 
-    .. note:: MyPy issues
-
-    Note the `# type: ignore` inline comments. These are only necessary when using `mypy`, which doesn't really seem to like decorators. They need to be supplied when decorating an `__init__` constructor method, or when adding multiple decorators to a method.
+.. note:: Note the `# type: ignore` inline comments. These are only necessary when using static type checkers like MyPy and Pyright. They don't really seem to like decorators very much. They need to be supplied when decorating an `__init__` constructor method, or when adding multiple decorators to a method.
 
 >>> ann = Annalist()
 >>> ann.configure(logger_name="Example Logger", analyst_name="Speve")
 
 Now the annalized code can be run like normal, and will be audited.
 
 >>> example_function()
```

### Comparing `data-annalist-0.4.1/README.rst` & `data-annalist-0.4.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -68,17 +68,15 @@
         # DO NOT put it on the __repr__ either.
         # Same as before, this creates infinite recursion.
         def __repr__(self):
             return f"{str(arg1)}: {str(arg2)}"
 
 In the main script, the Annalist object must be called again. This will point to the singleton object initialized in the dependency. The annalist must be configured before usage.
 
-    .. note:: MyPy issues
-
-    Note the `# type: ignore` inline comments. These are only necessary when using `mypy`, which doesn't really seem to like decorators. They need to be supplied when decorating an `__init__` constructor method, or when adding multiple decorators to a method.
+.. note:: Note the `# type: ignore` inline comments. These are only necessary when using static type checkers like MyPy and Pyright. They don't really seem to like decorators very much. They need to be supplied when decorating an `__init__` constructor method, or when adding multiple decorators to a method.
 
 >>> ann = Annalist()
 >>> ann.configure(logger_name="Example Logger", analyst_name="Speve")
 
 Now the annalized code can be run like normal, and will be audited.
 
 >>> example_function()
```

### Comparing `data-annalist-0.4.1/annalist/annalist.py` & `data-annalist-0.4.2/annalist/annalist.py`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/annalist/decorators.py` & `data-annalist-0.4.2/annalist/decorators.py`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/data_annalist.egg-info/PKG-INFO` & `data-annalist-0.4.2/data_annalist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: data-annalist
-Version: 0.4.1
+Version: 0.4.2
 Summary: Audit trail generator for data processing scripts.
 Author-email: Nic Mostert <nicolas.mostert@horizons.govt.nz>
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/nicmostert/annalist
 Project-URL: Issues, https://github.com/nicmostert/annalist/issues
 Project-URL: Documentation, https://annalist.readthedocs.io
 Project-URL: Package, https://pypi.org/project/data-annalist
 Keywords: logging, auditing, audit trail, hydrology, automation, hilltop, hydrobot, HorizonsRC
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: ==3.11.6
+Requires-Python: ==3.11.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Provides-Extra: test
 Requires-Dist: pytest>=7.4.2; extra == "test"
 Requires-Dist: pytest-cov>=4.1.0; extra == "test"
 Provides-Extra: dev
@@ -104,17 +104,15 @@
         # DO NOT put it on the __repr__ either.
         # Same as before, this creates infinite recursion.
         def __repr__(self):
             return f"{str(arg1)}: {str(arg2)}"
 
 In the main script, the Annalist object must be called again. This will point to the singleton object initialized in the dependency. The annalist must be configured before usage.
 
-    .. note:: MyPy issues
-
-    Note the `# type: ignore` inline comments. These are only necessary when using `mypy`, which doesn't really seem to like decorators. They need to be supplied when decorating an `__init__` constructor method, or when adding multiple decorators to a method.
+.. note:: Note the `# type: ignore` inline comments. These are only necessary when using static type checkers like MyPy and Pyright. They don't really seem to like decorators very much. They need to be supplied when decorating an `__init__` constructor method, or when adding multiple decorators to a method.
 
 >>> ann = Annalist()
 >>> ann.configure(logger_name="Example Logger", analyst_name="Speve")
 
 Now the annalized code can be run like normal, and will be audited.
 
 >>> example_function()
```

### Comparing `data-annalist-0.4.1/data_annalist.egg-info/SOURCES.txt` & `data-annalist-0.4.2/data_annalist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/docs/Makefile` & `data-annalist-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/docs/conf.py` & `data-annalist-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/docs/installation.rst` & `data-annalist-0.4.2/docs/installation.rst`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 Stable release
 --------------
 
 To install Annalist, run this command in your terminal:
 
 .. code-block:: console
 
-    $ pip install annalist
+    $ pip install data-annalist
+
+.. note:: Make sure you install `data-annalist`. The PyPI package called `annalist` is something else.
 
 This is the preferred method to install Annalist, as it will always install the most recent stable release.
 
 If you don't have `pip`_ installed, this `Python installation guide`_ can guide
 you through the process.
 
 .. _pip: https://pip.pypa.io
```

### Comparing `data-annalist-0.4.1/docs/make.bat` & `data-annalist-0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/old_requirements_dev.txt` & `data-annalist-0.4.2/old_requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/old_setup.py` & `data-annalist-0.4.2/old_setup.py`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/pyproject.toml` & `data-annalist-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "data-annalist"
 description = "Audit trail generator for data processing scripts."
-version = "0.4.1"
+version = "0.4.2"
 authors = [
     { name = "Nic Mostert", email = "nicolas.mostert@horizons.govt.nz" },
 ]
-requires-python = "==3.11.6"
+requires-python = "==3.11.*"
 dependencies = []
 classifiers=[
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.11"
@@ -84,15 +84,15 @@
 convention = "numpy"
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S311", "S101", "F841"]
 "docs/*" = ["I001"]
 
 [tool.bumpversion]
-current_version = "0.4.1"
+current_version = "0.4.2"
 commit = true
 tag = true
 tag_name = "{new_version}"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = "{current_version}"
```

### Comparing `data-annalist-0.4.1/temp_file.py` & `data-annalist-0.4.2/temp_file.py`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/tests/example_class.py` & `data-annalist-0.4.2/tests/example_class.py`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/tests/example_script.py` & `data-annalist-0.4.2/tests/example_script.py`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/tests/logfile.txt` & `data-annalist-0.4.2/tests/logfile.txt`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.1/tests/test_annalist.py` & `data-annalist-0.4.2/tests/test_annalist.py`

 * *Files identical despite different names*

