# Comparing `tmp/architect_py-0.1.0.tar.gz` & `tmp/architect_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "architect_py-0.2.0.tar", max compression
```

## Comparing `architect_py-0.1.0.tar` & `architect_py-0.2.0.tar`

### file list

```diff
@@ -1,84 +1,6 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 architect_py-0.1.0/Makefile
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 architect_py-0.1.0/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 architect_py-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 architect_py-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 architect_py-0.1.0/.idea/python.iml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 architect_py-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 architect_py-0.1.0/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 architect_py-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 architect_py-0.1.0/architect_py/__init__.py
--rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 architect_py-0.1.0/architect_py/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 architect_py-0.1.0/architect_py/examples/__init__.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 architect_py-0.1.0/architect_py/examples/market_making_example.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 architect_py-0.1.0/architect_py/examples/netidx_example.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 architect_py-0.1.0/architect_py/examples/print_book_example.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 architect_py-0.1.0/architect_py/examples/simple_order_example.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/README.md
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/make.bat
--rw-r--r--   0        0        0   113697 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0    43711 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/doctrees/source/architect_py.doctree
--rw-r--r--   0        0        0    14473 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/doctrees/source/architect_py.examples.doctree
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/doctrees/source/modules.doctree
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/.DS_Store
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0    10784 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/genindex.html
--rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/index.html
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/objects.inv
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/py-modindex.html
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/search.html
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_sources/source/architect_py.examples.rst.txt
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_sources/source/architect_py.rst.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_sources/source/modules.rst.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/.DS_Store
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/jquery.js
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0   135235 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/theme.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/_static/js/theme.js
--rw-r--r--   0        0        0    10493 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/source/architect_py.examples.html
--rw-r--r--   0        0        0    24158 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/source/architect_py.html
--rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/_build/html/source/modules.html
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/source/architect_py.examples.rst
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/source/architect_py.rst
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 architect_py-0.1.0/docs/source/modules.rst
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 architect_py-0.1.0/.gitignore
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 architect_py-0.1.0/LICENSE
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 architect_py-0.1.0/README.md
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 architect_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 architect_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11362 2024-04-01 23:48:50.192622 architect_py-0.2.0/LICENSE
+-rw-r--r--   0        0        0      657 2024-04-01 23:49:46.235990 architect_py-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 22:50:17.669839 architect_py-0.2.0/architect_py/__init__.py
+-rw-r--r--   0        0        0     1885 2024-04-01 23:28:44.285736 architect_py-0.2.0/architect_py/client.py
+-rw-r--r--   0        0        0      613 2024-04-01 23:07:17.875026 architect_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 architect_py-0.2.0/PKG-INFO
```

### Comparing `architect_py-0.1.0/LICENSE` & `architect_py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `architect_py-0.1.0/pyproject.toml` & `architect_py-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
+[tool.poetry]
 name = "architect-py"
-version = "0.1.0"
-authors = [
-  { name="Architect Financial Technologies", email="support@architect.xyz" },
-]
+version = "0.2.0"
 description = "Client library for the Architect trading platform."
+authors = ["Architect Financial Technologies, Inc. <hello@architect.xyz>"]
 readme = "README.md"
-requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: Apache Software License",
     "Development Status :: 3 - Alpha"
 ]
-dependencies = [
-    "asyncio>=3.4",
-    "websockets>=11"
-]
 
-[project.urls]
-"Homepage" = "https://verbose-journey-9kzk3z6.pages.github.io/architect-py/"
-# "Bug Tracker" = "mailto:support@architect.xyz"
+[tool.poetry.dependencies]
+python = ">=3.8,<4"
+asyncio = "^3.4.3"
+gql = {extras = ["all"], version = "^3.5.0"}
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

