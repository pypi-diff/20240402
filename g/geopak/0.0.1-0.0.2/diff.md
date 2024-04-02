# Comparing `tmp/geopak-0.0.1.tar.gz` & `tmp/geopak-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopak-0.0.1.tar", last modified: Wed Feb 14 21:56:18 2024, max compression
+gzip compressed data, was "geopak-0.0.2.tar", last modified: Tue Apr  2 19:09:44 2024, max compression
```

## Comparing `geopak-0.0.1.tar` & `geopak-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:56:18.717038 geopak-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-14 21:56:03.000000 geopak-0.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:56:18.709038 geopak-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:56:18.713038 geopak-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-14 21:56:03.000000 geopak-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-14 21:56:03.000000 geopak-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-14 21:56:03.000000 geopak-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:56:18.713038 geopak-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-02-14 21:56:03.000000 geopak-0.0.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-14 21:56:03.000000 geopak-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-14 21:56:03.000000 geopak-0.0.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-14 21:56:03.000000 geopak-0.0.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-02-14 21:56:03.000000 geopak-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-02-14 21:56:03.000000 geopak-0.0.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-14 21:56:03.000000 geopak-0.0.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-14 21:56:03.000000 geopak-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 21:56:03.000000 geopak-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-14 21:56:03.000000 geopak-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-14 21:56:18.717038 geopak-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-14 21:56:03.000000 geopak-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:56:18.713038 geopak-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-14 21:56:03.000000 geopak-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-14 21:56:03.000000 geopak-0.0.1/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-02-14 21:56:03.000000 geopak-0.0.1/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:56:18.713038 geopak-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-14 21:56:03.000000 geopak-0.0.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-14 21:56:03.000000 geopak-0.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-14 21:56:03.000000 geopak-0.0.1/docs/geopak.md
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-14 21:56:03.000000 geopak-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-14 21:56:03.000000 geopak-0.0.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:56:18.713038 geopak-0.0.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-14 21:56:03.000000 geopak-0.0.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-14 21:56:03.000000 geopak-0.0.1/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:56:18.713038 geopak-0.0.1/geopak/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-14 21:56:03.000000 geopak-0.0.1/geopak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-14 21:56:03.000000 geopak-0.0.1/geopak/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-14 21:56:03.000000 geopak-0.0.1/geopak/geopak.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:56:18.717038 geopak-0.0.1/geopak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-14 21:56:18.000000 geopak-0.0.1/geopak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-14 21:56:18.000000 geopak-0.0.1/geopak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 21:56:18.000000 geopak-0.0.1/geopak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-14 21:56:18.000000 geopak-0.0.1/geopak.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-14 21:56:18.000000 geopak-0.0.1/geopak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-14 21:56:18.000000 geopak-0.0.1/geopak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-14 21:56:03.000000 geopak-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-02-14 21:56:03.000000 geopak-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-14 21:56:03.000000 geopak-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-14 21:56:03.000000 geopak-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 21:56:18.717038 geopak-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:56:18.717038 geopak-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-14 21:56:03.000000 geopak-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-14 21:56:03.000000 geopak-0.0.1/tests/test_geopak.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.898041 geopak-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-02 19:09:30.000000 geopak-0.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.890041 geopak-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.894041 geopak-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.894041 geopak-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-02 19:09:30.000000 geopak-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:09:30.000000 geopak-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:09:30.000000 geopak-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-02 19:09:44.898041 geopak-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-02 19:09:30.000000 geopak-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.894041 geopak-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.898041 geopak-0.0.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/examples/csv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/examples/ipyleaflet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/examples/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/examples/sample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/examples/vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/geopak.md
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.898041 geopak-0.0.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.898041 geopak-0.0.2/geopak/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 19:09:30.000000 geopak-0.0.2/geopak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-02 19:09:30.000000 geopak-0.0.2/geopak/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-02 19:09:30.000000 geopak-0.0.2/geopak/geopak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-02 19:09:30.000000 geopak-0.0.2/geopak/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.898041 geopak-0.0.2/geopak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-02 19:09:44.000000 geopak-0.0.2/geopak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-02 19:09:44.000000 geopak-0.0.2/geopak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:09:44.000000 geopak-0.0.2/geopak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 19:09:44.000000 geopak-0.0.2/geopak.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:09:44.000000 geopak-0.0.2/geopak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 19:09:44.000000 geopak-0.0.2/geopak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-02 19:09:30.000000 geopak-0.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-02 19:09:30.000000 geopak-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 19:09:30.000000 geopak-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-02 19:09:30.000000 geopak-0.0.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:09:44.898041 geopak-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.898041 geopak-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 19:09:30.000000 geopak-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-02 19:09:30.000000 geopak-0.0.2/tests/test_geopak.py
```

### Comparing `geopak-0.0.1/.github/workflows/docs-build.yml` & `geopak-0.0.2/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.1/.github/workflows/docs.yml` & `geopak-0.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.1/.github/workflows/installation.yml` & `geopak-0.0.2/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.1/.github/workflows/macos.yml` & `geopak-0.0.2/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.1/.github/workflows/pypi.yml` & `geopak-0.0.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.1/.github/workflows/ubuntu.yml` & `geopak-0.0.2/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.1/.github/workflows/windows.yml` & `geopak-0.0.2/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.1/.gitignore` & `geopak-0.0.2/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 private/
 *.py[cod]
 *$py.class
-
+*.json
+*vector.ipnb
+*.tif
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 env/
 build/
```

### Comparing `geopak-0.0.1/PKG-INFO` & `geopak-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geopak
-Version: 0.0.1
+Version: 0.0.2
 Summary: python package demo for geodpatial analysis
 Author-email: Albert Tandoh <atandoh004@St.ug.edu.gh>
 License: MIT License
 Project-URL: Homepage, https://github.com/Tandoh004/geopak
 Keywords: geopak
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ipyleaflet
+Requires-Dist: pandas
 Provides-Extra: all
 Requires-Dist: geopak[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # geopak
```

### Comparing `geopak-0.0.1/docs/contributing.md` & `geopak-0.0.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `geopak-0.0.1/docs/installation.md` & `geopak-0.0.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `geopak-0.0.1/geopak.egg-info/PKG-INFO` & `geopak-0.0.2/geopak.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geopak
-Version: 0.0.1
+Version: 0.0.2
 Summary: python package demo for geodpatial analysis
 Author-email: Albert Tandoh <atandoh004@St.ug.edu.gh>
 License: MIT License
 Project-URL: Homepage, https://github.com/Tandoh004/geopak
 Keywords: geopak
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ipyleaflet
+Requires-Dist: pandas
 Provides-Extra: all
 Requires-Dist: geopak[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # geopak
```

### Comparing `geopak-0.0.1/geopak.egg-info/SOURCES.txt` & `geopak-0.0.2/geopak.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -21,19 +21,26 @@
 docs/common.md
 docs/contributing.md
 docs/faq.md
 docs/geopak.md
 docs/index.md
 docs/installation.md
 docs/usage.md
+docs/utils.md
+docs/examples/csv.ipynb
 docs/examples/intro.ipynb
+docs/examples/ipyleaflet.ipynb
+docs/examples/iris.csv
+docs/examples/sample.ipynb
+docs/examples/vector.ipynb
 docs/overrides/main.html
 geopak/__init__.py
 geopak/common.py
 geopak/geopak.py
+geopak/utils.py
 geopak.egg-info/PKG-INFO
 geopak.egg-info/SOURCES.txt
 geopak.egg-info/dependency_links.txt
 geopak.egg-info/entry_points.txt
 geopak.egg-info/requires.txt
 geopak.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `geopak-0.0.1/mkdocs.yml` & `geopak-0.0.2/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 site_name: geopak
-site_description: python package demo for geodpatial analysis
+site_description: python package demo for geospatial analysis
 site_author: Tandoh004
 site_url: https://Tandoh004.github.io/geopak
 repo_url: https://github.com/Tandoh004/geopak
 
 copyright: "Copyright &copy; 2024 - 2024 Albert Tandoh"
 
 theme:
@@ -77,10 +77,15 @@
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/Tandoh004/geopak/issues
     - Examples:
         - examples/intro.ipynb
+        - examples/sample.ipynb
+        - examples/csv.ipynb
+
+
     - API Reference:
           - geopak module: geopak.md
           - common module: common.md
+          - utils module: utils.md
```

### Comparing `geopak-0.0.1/pyproject.toml` & `geopak-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "geopak"
-version = "0.0.1"
+version = "0.0.2"
 dynamic = [
     "dependencies",
 ]
 description = "python package demo for geodpatial analysis"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.0.2"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

