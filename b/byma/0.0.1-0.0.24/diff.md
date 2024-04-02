# Comparing `tmp/byma-0.0.1.tar.gz` & `tmp/byma-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byma-0.0.1.tar", last modified: Mon Apr  1 22:06:42 2024, max compression
+gzip compressed data, was "byma-0.0.24.tar", last modified: Tue Apr  2 20:20:16 2024, max compression
```

## Comparing `byma-0.0.1.tar` & `byma-0.0.24.tar`

### file list

```diff
@@ -1,38 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 22:06:42.556965 byma-0.0.1/
--rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-01 22:06:31.000000 byma-0.0.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      585 2024-04-01 22:06:42.555965 byma-0.0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       55 2024-04-01 22:06:31.000000 byma-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 22:06:42.550966 byma-0.0.1/byma/
--rw-rw-rw-   0 root         (0) root         (0)     1151 2024-04-01 22:06:31.000000 byma-0.0.1/byma/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 22:06:42.552965 byma-0.0.1/byma/interface/
--rw-rw-rw-   0 root         (0) root         (0)     1022 2024-04-01 22:06:31.000000 byma-0.0.1/byma/interface/BaseInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     2676 2024-04-01 22:06:31.000000 byma-0.0.1/byma/interface/NonlinearHeat.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-01 22:06:31.000000 byma-0.0.1/byma/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 22:06:42.552965 byma-0.0.1/byma/iteral/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-01 22:06:31.000000 byma-0.0.1/byma/iteral/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 22:06:42.553965 byma-0.0.1/byma/iteral/nonstationary/
--rw-rw-rw-   0 root         (0) root         (0)     1773 2024-04-01 22:06:31.000000 byma-0.0.1/byma/iteral/nonstationary/Newton.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-01 22:06:31.000000 byma-0.0.1/byma/iteral/nonstationary/NonStationary.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-01 22:06:31.000000 byma-0.0.1/byma/iteral/nonstationary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2024-04-01 22:06:31.000000 byma-0.0.1/byma/iteral/part_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 22:06:42.553965 byma-0.0.1/byma/iteral/stationary/
--rw-rw-rw-   0 root         (0) root         (0)     5142 2024-04-01 22:06:31.000000 byma-0.0.1/byma/iteral/stationary/OrthogonalSubspace.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-04-01 22:06:31.000000 byma-0.0.1/byma/iteral/stationary/Stationary.py
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-01 22:06:31.000000 byma-0.0.1/byma/iteral/stationary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 22:06:42.554965 byma-0.0.1/byma/nuby/
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-04-01 22:06:31.000000 byma-0.0.1/byma/nuby/Bifurcation.py
--rw-rw-rw-   0 root         (0) root         (0)     4811 2024-04-01 22:06:31.000000 byma-0.0.1/byma/nuby/Continuation.py
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-04-01 22:06:31.000000 byma-0.0.1/byma/nuby/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 22:06:42.555965 byma-0.0.1/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-01 22:06:31.000000 byma-0.0.1/byma/pyplot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6594 2024-04-01 22:06:31.000000 byma-0.0.1/byma/pyplot/plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 22:06:42.555965 byma-0.0.1/byma.egg-info/
--rw-r--r--   0 root         (0) root         (0)      585 2024-04-01 22:06:42.000000 byma-0.0.1/byma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      680 2024-04-01 22:06:42.000000 byma-0.0.1/byma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 22:06:42.000000 byma-0.0.1/byma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-01 22:06:42.000000 byma-0.0.1/byma.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      568 2024-04-01 22:06:31.000000 byma-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 22:06:42.556965 byma-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      924 2024-04-01 22:06:31.000000 byma-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 22:06:42.555965 byma-0.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 22:06:31.000000 byma-0.0.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.484999 byma-0.0.24/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-02 20:20:03.000000 byma-0.0.24/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-04-02 20:20:03.000000 byma-0.0.24/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-02 20:20:03.000000 byma-0.0.24/CHANGELOG.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-02 20:20:03.000000 byma-0.0.24/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-02 20:20:03.000000 byma-0.0.24/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-02 20:20:16.483999 byma-0.0.24/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1387 2024-04-02 20:20:03.000000 byma-0.0.24/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.478999 byma-0.0.24/byma/
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2024-04-02 20:20:03.000000 byma-0.0.24/byma/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      413 2024-04-02 20:20:16.000000 byma-0.0.24/byma/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.479999 byma-0.0.24/byma/interface/
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2024-04-02 20:20:03.000000 byma-0.0.24/byma/interface/BaseInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2676 2024-04-02 20:20:03.000000 byma-0.0.24/byma/interface/NonlinearHeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-02 20:20:03.000000 byma-0.0.24/byma/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.480999 byma-0.0.24/byma/iteral/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.481999 byma-0.0.24/byma/iteral/nonstationary/
+-rw-rw-rw-   0 root         (0) root         (0)     4104 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/nonstationary/Newton.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/nonstationary/NonStationary.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/nonstationary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/part_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.481999 byma-0.0.24/byma/iteral/stationary/
+-rw-rw-rw-   0 root         (0) root         (0)     5142 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/stationary/OrthogonalSubspace.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/stationary/Stationary.py
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/stationary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.482999 byma-0.0.24/byma/nuby/
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-04-02 20:20:03.000000 byma-0.0.24/byma/nuby/Bifurcation.py
+-rw-rw-rw-   0 root         (0) root         (0)     6412 2024-04-02 20:20:03.000000 byma-0.0.24/byma/nuby/Continuation.py
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-04-02 20:20:03.000000 byma-0.0.24/byma/nuby/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.482999 byma-0.0.24/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-02 20:20:03.000000 byma-0.0.24/byma/pyplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6594 2024-04-02 20:20:03.000000 byma-0.0.24/byma/pyplot/plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.483999 byma-0.0.24/byma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-02 20:20:16.000000 byma-0.0.24/byma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      791 2024-04-02 20:20:16.000000 byma-0.0.24/byma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 20:20:16.000000 byma-0.0.24/byma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-02 20:20:16.000000 byma-0.0.24/byma.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.483999 byma-0.0.24/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      877 2024-04-02 20:20:03.000000 byma-0.0.24/examples/assignment_4.py
+-rwxrwxrwx   0 root         (0) root         (0)      724 2024-04-02 20:20:03.000000 byma-0.0.24/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-02 20:20:03.000000 byma-0.0.24/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 20:20:16.484999 byma-0.0.24/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-02 20:20:03.000000 byma-0.0.24/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.483999 byma-0.0.24/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 20:20:03.000000 byma-0.0.24/tests/__init__.py
```

### Comparing `byma-0.0.1/LICENSE.md` & `byma-0.0.24/LICENSE.md`

 * *Files identical despite different names*

### Comparing `byma-0.0.1/byma/__init__.py` & `byma-0.0.24/byma/__init__.py`

 * *Files identical despite different names*

### Comparing `byma-0.0.1/byma/interface/BaseInterface.py` & `byma-0.0.24/byma/interface/BaseInterface.py`

 * *Files identical despite different names*

### Comparing `byma-0.0.1/byma/interface/NonlinearHeat.py` & `byma-0.0.24/byma/interface/NonlinearHeat.py`

 * *Files identical despite different names*

### Comparing `byma-0.0.1/byma/iteral/stationary/OrthogonalSubspace.py` & `byma-0.0.24/byma/iteral/stationary/OrthogonalSubspace.py`

 * *Files identical despite different names*

### Comparing `byma-0.0.1/byma/pyplot/plots.py` & `byma-0.0.24/byma/pyplot/plots.py`

 * *Files identical despite different names*

### Comparing `byma-0.0.1/byma.egg-info/SOURCES.txt` & `byma-0.0.24/byma.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+.gitignore
+.gitlab-ci.yml
+CHANGELOG.txt
 LICENSE.md
+MANIFEST.in
 README.md
 pyproject.toml
+requirements.txt
 setup.py
 byma/__init__.py
+byma/_version.py
 byma.egg-info/PKG-INFO
 byma.egg-info/SOURCES.txt
 byma.egg-info/dependency_links.txt
 byma.egg-info/top_level.txt
 byma/interface/BaseInterface.py
 byma/interface/NonlinearHeat.py
 byma/interface/__init__.py
@@ -19,8 +25,9 @@
 byma/iteral/stationary/Stationary.py
 byma/iteral/stationary/__init__.py
 byma/nuby/Bifurcation.py
 byma/nuby/Continuation.py
 byma/nuby/__init__.py
 byma/pyplot/__init__.py
 byma/pyplot/plots.py
+examples/assignment_4.py
 tests/__init__.py
```

