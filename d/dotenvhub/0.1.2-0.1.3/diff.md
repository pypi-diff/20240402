# Comparing `tmp/dotenvhub-0.1.2.tar.gz` & `tmp/dotenvhub-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotenvhub-0.1.2.tar", last modified: Fri Feb  9 17:23:23 2024, max compression
+gzip compressed data, was "dotenvhub-0.1.3.tar", last modified: Tue Apr  2 20:24:02 2024, max compression
```

## Comparing `dotenvhub-0.1.2.tar` & `dotenvhub-0.1.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:23:23.077403 dotenvhub-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:23:23.065403 dotenvhub-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:23:23.069404 dotenvhub-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-09 17:23:23.077403 dotenvhub-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:23:23.069404 dotenvhub-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:23:23.069404 dotenvhub-0.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:23:23.069404 dotenvhub-0.1.2/images/
--rw-r--r--   0 runner    (1001) docker     (127)   131826 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/images/image_header.PNG
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-02-09 17:23:23.077403 dotenvhub-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:23:23.065403 dotenvhub-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:23:23.073403 dotenvhub-0.1.2/src/dotenvhub/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:23:23.073403 dotenvhub-0.1.2/src/dotenvhub/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/assets/modal_save.css
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/assets/modal_shell.css
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/assets/tui.css
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/tui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:23:23.073403 dotenvhub-0.1.2/src/dotenvhub/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/widgets/filepanel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/widgets/interactionpanel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/widgets/modals.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/src/dotenvhub/widgets/previewpanel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:23:23.073403 dotenvhub-0.1.2/src/dotenvhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-09 17:23:23.000000 dotenvhub-0.1.2/src/dotenvhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-09 17:23:23.000000 dotenvhub-0.1.2/src/dotenvhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 17:23:23.000000 dotenvhub-0.1.2/src/dotenvhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-09 17:23:23.000000 dotenvhub-0.1.2/src/dotenvhub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 17:23:22.000000 dotenvhub-0.1.2/src/dotenvhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-09 17:23:23.000000 dotenvhub-0.1.2/src/dotenvhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-09 17:23:23.000000 dotenvhub-0.1.2/src/dotenvhub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:23:23.073403 dotenvhub-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-02-09 17:22:46.000000 dotenvhub-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.257320 dotenvhub-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.261320 dotenvhub-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.265320 dotenvhub-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.265320 dotenvhub-0.1.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.265320 dotenvhub-0.1.3/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   131826 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/images/image_header.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.261320 dotenvhub-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.265320 dotenvhub-0.1.3/src/dotenvhub/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/src/dotenvhub/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/assets/modal_save.css
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/assets/modal_shell.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/assets/tui.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/tui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/src/dotenvhub/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/widgets/filepanel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/widgets/interactionpanel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/widgets/modals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/widgets/previewpanel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/src/dotenvhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/tox.ini
```

### Comparing `dotenvhub-0.1.2/.coveragerc` & `dotenvhub-0.1.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/.github/workflows/ci.yml` & `dotenvhub-0.1.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/.gitignore` & `dotenvhub-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/.pre-commit-config.yaml` & `dotenvhub-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/.readthedocs.yml` & `dotenvhub-0.1.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/CONTRIBUTING.md` & `dotenvhub-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/LICENSE.txt` & `dotenvhub-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/PKG-INFO` & `dotenvhub-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dotenvhub
-Version: 0.1.2
+Version: 0.1.3
 Summary: Terminal App to manage .env files written in Python powered by Textual
 Home-page: https://github.com/Zaloog/dotenvhub
 Author: Zaloog
 Author-email: gramslars@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/Zaloog/dotenvhub
 Project-URL: Source, https://github.com/Zaloog/dotenvhub
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
-Requires-Dist: textual<=0.50.0
+Requires-Dist: textual<=0.55.1
 Requires-Dist: platformdirs
 Requires-Dist: pyperclip
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `dotenvhub-0.1.2/README.md` & `dotenvhub-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/docs/Makefile` & `dotenvhub-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/docs/conf.py` & `dotenvhub-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/docs/index.md` & `dotenvhub-0.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/images/image_header.PNG` & `dotenvhub-0.1.3/images/image_header.PNG`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/setup.cfg` & `dotenvhub-0.1.3/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.8
 install_requires = 
-	textual<=0.50.0
+	textual<=0.55.1
 	platformdirs
 	pyperclip
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `dotenvhub-0.1.2/setup.py` & `dotenvhub-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/src/dotenvhub/__init__.py` & `dotenvhub-0.1.3/src/dotenvhub/__init__.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/src/dotenvhub/app.py` & `dotenvhub-0.1.3/src/dotenvhub/app.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/src/dotenvhub/assets/modal_shell.css` & `dotenvhub-0.1.3/src/dotenvhub/assets/modal_shell.css`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/src/dotenvhub/assets/tui.css` & `dotenvhub-0.1.3/src/dotenvhub/assets/tui.css`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/src/dotenvhub/cli_parser.py` & `dotenvhub-0.1.3/src/dotenvhub/cli_parser.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/src/dotenvhub/config.py` & `dotenvhub-0.1.3/src/dotenvhub/config.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/src/dotenvhub/constants.py` & `dotenvhub-0.1.3/src/dotenvhub/constants.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/src/dotenvhub/tui.py` & `dotenvhub-0.1.3/src/dotenvhub/tui.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/src/dotenvhub/utils.py` & `dotenvhub-0.1.3/src/dotenvhub/utils.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/src/dotenvhub/widgets/filepanel.py` & `dotenvhub-0.1.3/src/dotenvhub/widgets/filepanel.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
                 yield general_list
             else:
                 folder_list = ListView(
                     *[
                         ListItem(
                             Label(f":page_facing_up: {file}"),
                             Button.warning(
-                                "Edit", id=f"btn-edit-{dirpath}/{file}", classes="edit"
+                                "Edit", id=f"btn-edit-{dirpath}-{file}", classes="edit"
                             ),
                             Button.error(
                                 "Delete",
-                                id=f"btn-del-{dirpath}/{file}",
+                                id=f"btn-del-{dirpath}-{file}",
                                 classes="delete",
                             ),
                             id=f"{dirpath}-{file}",
                         )
                         for file in filenames
                     ],
                     id=f"collaps-{dirpath}",
@@ -99,15 +99,15 @@
         text_widget = self.app.query_one(TextArea)
         text_widget.text = self.app.current_content
         text_widget.action_cursor_page_down()
         text_widget.disabled = True
 
     @on(Button.Pressed, ".delete")
     def delete_env_file(self, event: Button.Pressed):
-        folder_file_path = event.button.id[8:]
+        folder_file_path = event.button.id[8:].replace("-", "/")
 
         # Delete File
         (ENV_FILE_DIR_PATH / folder_file_path).unlink()
         try:
             # If Folder Empty delete Folder
             (ENV_FILE_DIR_PATH / folder_file_path).parent.rmdir()
         except OSError:
```

### Comparing `dotenvhub-0.1.2/src/dotenvhub/widgets/interactionpanel.py` & `dotenvhub-0.1.3/src/dotenvhub/widgets/interactionpanel.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/src/dotenvhub/widgets/modals.py` & `dotenvhub-0.1.3/src/dotenvhub/widgets/modals.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/src/dotenvhub.egg-info/PKG-INFO` & `dotenvhub-0.1.3/src/dotenvhub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dotenvhub
-Version: 0.1.2
+Version: 0.1.3
 Summary: Terminal App to manage .env files written in Python powered by Textual
 Home-page: https://github.com/Zaloog/dotenvhub
 Author: Zaloog
 Author-email: gramslars@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/Zaloog/dotenvhub
 Project-URL: Source, https://github.com/Zaloog/dotenvhub
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
-Requires-Dist: textual<=0.50.0
+Requires-Dist: textual<=0.55.1
 Requires-Dist: platformdirs
 Requires-Dist: pyperclip
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `dotenvhub-0.1.2/src/dotenvhub.egg-info/SOURCES.txt` & `dotenvhub-0.1.3/src/dotenvhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/tests/test_utils.py` & `dotenvhub-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.2/tox.ini` & `dotenvhub-0.1.3/tox.ini`

 * *Files identical despite different names*

