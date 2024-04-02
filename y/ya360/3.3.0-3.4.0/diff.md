# Comparing `tmp/ya360-3.3.0.tar.gz` & `tmp/ya360-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ya360-3.3.0.tar", last modified: Fri Mar 29 08:20:47 2024, max compression
+gzip compressed data, was "ya360-3.4.0.tar", last modified: Tue Apr  2 06:42:45 2024, max compression
```

## Comparing `ya360-3.3.0.tar` & `ya360-3.4.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:20:47.323583 ya360-3.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:20:47.315583 ya360-3.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:20:47.315583 ya360-3.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-29 08:20:30.000000 ya360-3.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-29 08:20:30.000000 ya360-3.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-29 08:20:30.000000 ya360-3.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:20:47.315583 ya360-3.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-29 08:20:30.000000 ya360-3.3.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-29 08:20:30.000000 ya360-3.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-29 08:20:30.000000 ya360-3.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-29 08:20:30.000000 ya360-3.3.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:20:47.319583 ya360-3.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-29 08:20:30.000000 ya360-3.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-03-29 08:20:30.000000 ya360-3.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-29 08:20:30.000000 ya360-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-29 08:20:30.000000 ya360-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-29 08:20:47.323583 ya360-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-29 08:20:30.000000 ya360-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-29 08:20:30.000000 ya360-3.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-29 08:20:30.000000 ya360-3.3.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:20:47.319583 ya360-3.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:20:47.319583 ya360-3.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:20:47.319583 ya360-3.3.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    38353 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/source/_static/fig1.png
--rw-r--r--   0 runner    (1001) docker     (127)   127538 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/source/_static/fig2.png
--rw-r--r--   0 runner    (1001) docker     (127)    36447 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/source/_static/fig3.png
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/source/_static/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/source/befo.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/source/cmd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/source/lic.rst
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/source/routing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-03-29 08:20:30.000000 ya360-3.3.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-29 08:20:30.000000 ya360-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 08:20:47.323583 ya360-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-29 08:20:30.000000 ya360-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:20:47.323583 ya360-3.3.0/ya360/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-29 08:20:30.000000 ya360-3.3.0/ya360/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-29 08:20:30.000000 ya360-3.3.0/ya360/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-29 08:20:47.000000 ya360-3.3.0/ya360/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-03-29 08:20:30.000000 ya360-3.3.0/ya360/antispam.py
--rw-r--r--   0 runner    (1001) docker     (127)    20821 2024-03-29 08:20:30.000000 ya360-3.3.0/ya360/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-03-29 08:20:30.000000 ya360-3.3.0/ya360/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-03-29 08:20:30.000000 ya360-3.3.0/ya360/departments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-03-29 08:20:30.000000 ya360-3.3.0/ya360/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-03-29 08:20:30.000000 ya360-3.3.0/ya360/mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-29 08:20:30.000000 ya360-3.3.0/ya360/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-29 08:20:30.000000 ya360-3.3.0/ya360/tid.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-29 08:20:30.000000 ya360-3.3.0/ya360/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-03-29 08:20:30.000000 ya360-3.3.0/ya360/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-03-29 08:20:30.000000 ya360-3.3.0/ya360/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:20:47.323583 ya360-3.3.0/ya360.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-29 08:20:47.000000 ya360-3.3.0/ya360.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-29 08:20:47.000000 ya360-3.3.0/ya360.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 08:20:47.000000 ya360-3.3.0/ya360.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-29 08:20:47.000000 ya360-3.3.0/ya360.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 08:20:47.000000 ya360-3.3.0/ya360.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-29 08:20:47.000000 ya360-3.3.0/ya360.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:42:45.045220 ya360-3.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:42:45.041220 ya360-3.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:42:45.041220 ya360-3.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-02 06:42:40.000000 ya360-3.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-02 06:42:40.000000 ya360-3.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-02 06:42:40.000000 ya360-3.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:42:45.041220 ya360-3.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-02 06:42:40.000000 ya360-3.4.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-02 06:42:40.000000 ya360-3.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-02 06:42:40.000000 ya360-3.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-02 06:42:40.000000 ya360-3.4.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:42:45.041220 ya360-3.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 06:42:40.000000 ya360-3.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-02 06:42:40.000000 ya360-3.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 06:42:40.000000 ya360-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 06:42:40.000000 ya360-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-02 06:42:45.045220 ya360-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-02 06:42:40.000000 ya360-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-02 06:42:40.000000 ya360-3.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 06:42:40.000000 ya360-3.4.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:42:45.041220 ya360-3.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:42:45.041220 ya360-3.4.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:42:45.041220 ya360-3.4.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    38353 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/source/_static/fig1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   127538 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/source/_static/fig2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36447 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/source/_static/fig3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/source/_static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/source/befo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/source/cmd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/source/lic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/source/routing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-04-02 06:42:40.000000 ya360-3.4.0/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-02 06:42:40.000000 ya360-3.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 06:42:45.045220 ya360-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-02 06:42:40.000000 ya360-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:42:45.045220 ya360-3.4.0/ya360/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 06:42:44.000000 ya360-3.4.0/ya360/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/antispam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23533 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/departments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/tid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-02 06:42:40.000000 ya360-3.4.0/ya360/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:42:45.045220 ya360-3.4.0/ya360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-02 06:42:45.000000 ya360-3.4.0/ya360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-02 06:42:45.000000 ya360-3.4.0/ya360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:42:45.000000 ya360-3.4.0/ya360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 06:42:45.000000 ya360-3.4.0/ya360.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 06:42:45.000000 ya360-3.4.0/ya360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 06:42:45.000000 ya360-3.4.0/ya360.egg-info/top_level.txt
```

### Comparing `ya360-3.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ya360-3.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `ya360-3.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/.github/workflows/codeql-analysis.yml` & `ya360-3.4.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/.github/workflows/python-publish.yml` & `ya360-3.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/.gitignore` & `ya360-3.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/.readthedocs.yaml` & `ya360-3.4.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/CODE_OF_CONDUCT.md` & `ya360-3.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/LICENSE` & `ya360-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/PKG-INFO` & `ya360-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ya360
-Version: 3.3.0
+Version: 3.4.0
 Summary: Утилита командной строки для Yandex 360
 Author-email: Купцов Игорь <ya360@uh.net.ru>
 License: MIT
 Project-URL: Homepage, https://ya360.uh.net.ru
 Project-URL: Bug Tracker, https://github.com/imercury13/ya360/issues
 Project-URL: Documentation, https://ya360.readthedocs.io/
 Project-URL: Download, https://github.com/imercury13/ya360
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: yandex-oauth>=1.1.2
-Requires-Dist: yandex-360>=2.2.0
+Requires-Dist: yandex-360>=2.2.1
 
 # ya360
 
 Утилита командной строки для Yandex 360
 
 >Для фанатов автоматизации UNIX/Linux - style или тех, кто устал курлить
```

### Comparing `ya360-3.3.0/README.md` & `ya360-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/README.rst` & `ya360-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/docs/Makefile` & `ya360-3.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/docs/make.bat` & `ya360-3.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/docs/source/_static/fig1.png` & `ya360-3.4.0/docs/source/_static/fig1.png`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/docs/source/_static/fig2.png` & `ya360-3.4.0/docs/source/_static/fig2.png`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/docs/source/_static/fig3.png` & `ya360-3.4.0/docs/source/_static/fig3.png`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/docs/source/befo.rst` & `ya360-3.4.0/docs/source/befo.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/docs/source/cmd.rst` & `ya360-3.4.0/docs/source/cmd.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/docs/source/conf.py` & `ya360-3.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/docs/source/index.rst` & `ya360-3.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/docs/source/lic.rst` & `ya360-3.4.0/docs/source/lic.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/docs/source/usage.rst` & `ya360-3.4.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/pyproject.toml` & `ya360-3.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Operating System :: POSIX",
     "Programming Language :: Python",
     "Environment :: Console",
     "Intended Audience :: System Administrators"
 ]
 dependencies = [
     "yandex-oauth >= 1.1.2",
-    "yandex-360 >= 2.2.0",
+    "yandex-360 >= 2.2.1",
 ]
 authors = [
     {name = "Купцов Игорь", email = "ya360@uh.net.ru"},
 ]
 dynamic = ["version"]
 
 [tool.setuptools_scm]
```

### Comparing `ya360-3.3.0/ya360/antispam.py` & `ya360-3.4.0/ya360/antispam.py`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/ya360/cmd.py` & `ya360-3.4.0/ya360/cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from . import __version__
 from . import __path__ as path
 from .departments import create_department, update_department, add_alias_department, delete_alias_department, delete_department, show_department, show_departments
 from .users import show_users, show_user, update_user, create_user, add_alias_user, delete_alias_user, delete_user, upload_avatar_user
 from .groups import create_group, delete_group, update_group, add_member_group, delete_member_group, show_group, show_groups
 from .mail import edit_access_mailbox, delete_access_mailbox, show_status_access_mailbox, show_access_mailbox_user, show_users_access_mailbox
 from .whois import whois
+from .logs import show_mail_log, show_disk_log
 from .configure import make_config
 from .antispam import show_whitelist, add_in_whitelist, remove_from_whitelist, delete_whitelist
 from .routing import add_in_routing, show_routing, remove_from_routing
 
 
 def gen_parser():
     """Функция запуска приложения приема аргументов командной строки
@@ -184,14 +185,33 @@
     parser_mailbox_comm.add_argument('nickname', type=str, help='Login пользователя')
 
     parser_mailbox_comm = subparser_mailbox.add_parser('list-users',help='Список сотрудников, у которых есть права доступа к почтовому ящику')
     parser_mailbox_comm.add_argument('nickname', type=str, help='Login пользователя почтового ящика')
 
 
 
+    parser_logs = subparsers.add_parser('logs', help='Аудит-лог событий в организации')
+    subparser_logs = parser_logs.add_subparsers(dest='sub_com_logs')
+
+    parser_logs_comm = subparser_logs.add_parser('mail',help='Аудит-лог почты')
+    parser_logs_comm.add_argument('--beforeDate', type=str, help='Верхняя граница периода выборки в формате ISO 8601')
+    parser_logs_comm.add_argument('--afterDate', type=str, help='Нижняя граница периода выборки в формате ISO 8601')
+    parser_logs_comm.add_argument('--includeUsers', type=str, help='Список пользователей, действия которых должны быть включены в список событий')
+    parser_logs_comm.add_argument('--excludeUsers', type=str, help='Список пользователей, действия которых должны быть исключены из списка событий')
+    parser_logs_comm.add_argument('--types', type=str, help='Типы событий которые должны быть включены в список. По умолчанию включаются все события')
+    parser_logs_comm.add_argument('--csv', type=str, help='Выгрузить в CSV файл')
+
+    parser_logs_comm = subparser_logs.add_parser('disk',help='Аудит-лог диска')
+    parser_logs_comm.add_argument('--beforeDate', type=str, help='Верхняя граница периода выборки в формате ISO 8601')
+    parser_logs_comm.add_argument('--afterDate', type=str, help='Нижняя граница периода выборки в формате ISO 8601')
+    parser_logs_comm.add_argument('--includeUsers', type=str, help='Список пользователей, действия которых должны быть включены в список событий')
+    parser_logs_comm.add_argument('--excludeUsers', type=str, help='Список пользователей, действия которых должны быть исключены из списка событий')
+    parser_logs_comm.add_argument('--types', type=str, help='Типы событий которые должны быть включены в список. По умолчанию включаются все события')
+    parser_logs_comm.add_argument('--csv', type=str, help='Выгрузить в CSV файл')
+
     parser_antispam = subparsers.add_parser('antispam', help='Антиспам')
     subparser_antispam = parser_antispam.add_subparsers(dest='sub_com_antispam')
     parser_antispam_comm = subparser_antispam.add_parser('show', help='Показать содержимое белого списка')
     parser_antispam_comm = subparser_antispam.add_parser('add', help='Добавить в белый список')
     parser_antispam_comm.add_argument('ipcidr', type=str, help='Адрес или CIDR')
     parser_antispam_comm = subparser_antispam.add_parser('remove', help='Удалить из белого списка')
     parser_antispam_comm.add_argument('ipcidr', type=str, help='Адрес или CIDR')
@@ -291,14 +311,20 @@
         if args.sub_com_mailbox == 'status':
             show_status_access_mailbox(args)
         if args.sub_com_mailbox == 'list-mailboxes':
             show_access_mailbox_user(args)
         if args.sub_com_mailbox == 'list-users':
             show_users_access_mailbox(args)
 
+    if args.sub_com == 'logs':
+        if args.sub_com_logs == 'mail':
+            show_mail_log(args)
+        if args.sub_com_logs == 'disk':
+            show_disk_log(args)
+
     if args.sub_com == 'antispam':
         if args.sub_com_antispam == 'show':
             show_whitelist()
         if args.sub_com_antispam == 'add':
             add_in_whitelist(args)
         if args.sub_com_antispam == 'remove':
             remove_from_whitelist(args)
```

### Comparing `ya360-3.3.0/ya360/configure.py` & `ya360-3.4.0/ya360/configure.py`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/ya360/departments.py` & `ya360-3.4.0/ya360/departments.py`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/ya360/groups.py` & `ya360-3.4.0/ya360/groups.py`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/ya360/mail.py` & `ya360-3.4.0/ya360/mail.py`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/ya360/routing.py` & `ya360-3.4.0/ya360/routing.py`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/ya360/tid.py` & `ya360-3.4.0/ya360/tid.py`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/ya360/users.py` & `ya360-3.4.0/ya360/users.py`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/ya360/whois.py` & `ya360-3.4.0/ya360/whois.py`

 * *Files identical despite different names*

### Comparing `ya360-3.3.0/ya360.egg-info/PKG-INFO` & `ya360-3.4.0/ya360.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ya360
-Version: 3.3.0
+Version: 3.4.0
 Summary: Утилита командной строки для Yandex 360
 Author-email: Купцов Игорь <ya360@uh.net.ru>
 License: MIT
 Project-URL: Homepage, https://ya360.uh.net.ru
 Project-URL: Bug Tracker, https://github.com/imercury13/ya360/issues
 Project-URL: Documentation, https://ya360.readthedocs.io/
 Project-URL: Download, https://github.com/imercury13/ya360
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: yandex-oauth>=1.1.2
-Requires-Dist: yandex-360>=2.2.0
+Requires-Dist: yandex-360>=2.2.1
 
 # ya360
 
 Утилита командной строки для Yandex 360
 
 >Для фанатов автоматизации UNIX/Linux - style или тех, кто устал курлить
```

### Comparing `ya360-3.3.0/ya360.egg-info/SOURCES.txt` & `ya360-3.4.0/ya360.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 ya360/__main__.py
 ya360/_version.py
 ya360/antispam.py
 ya360/cmd.py
 ya360/configure.py
 ya360/departments.py
 ya360/groups.py
+ya360/logs.py
 ya360/mail.py
 ya360/routing.py
 ya360/tid.py
 ya360/tools.py
 ya360/users.py
 ya360/whois.py
 ya360.egg-info/PKG-INFO
```

