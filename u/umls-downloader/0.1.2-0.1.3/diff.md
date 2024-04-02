# Comparing `tmp/umls_downloader-0.1.2.tar.gz` & `tmp/umls_downloader-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umls_downloader-0.1.2.tar", last modified: Tue Nov  7 14:28:37 2023, max compression
+gzip compressed data, was "umls_downloader-0.1.3.tar", last modified: Tue Apr  2 08:03:27 2024, max compression
```

## Comparing `umls_downloader-0.1.2.tar` & `umls_downloader-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-11-07 14:28:37.639808 umls_downloader-0.1.2/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      347 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)     7487 2023-11-07 14:28:37.639723 umls_downloader-0.1.2/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     5663 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-11-07 14:28:37.634793 umls_downloader-0.1.2/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-11-07 14:28:37.635899 umls_downloader-0.1.2/docs/source/
--rw-r--r--   0 cthoyt     (501) staff       (20)     6926 2023-11-07 14:28:37.000000 umls_downloader-0.1.2/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      484 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      376 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2468 2023-11-07 14:28:37.640184 umls_downloader-0.1.2/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-11-07 14:28:37.634951 umls_downloader-0.1.2/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-11-07 14:28:37.637593 umls_downloader-0.1.2/src/umls_downloader/
--rw-r--r--   0 cthoyt     (501) staff       (20)      656 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/src/umls_downloader/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      332 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/src/umls_downloader/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4447 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/src/umls_downloader/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2641 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/src/umls_downloader/cli.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2352 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/src/umls_downloader/rxnorm.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2388 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/src/umls_downloader/semmeddb.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1263 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/src/umls_downloader/snomed.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3337 2023-11-07 14:28:16.000000 umls_downloader-0.1.2/src/umls_downloader/umls.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1036 2023-11-07 14:28:37.000000 umls_downloader-0.1.2/src/umls_downloader/version.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-11-07 14:28:37.638551 umls_downloader-0.1.2/src/umls_downloader.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)     7487 2023-11-07 14:28:37.000000 umls_downloader-0.1.2/src/umls_downloader.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)      707 2023-11-07 14:28:37.000000 umls_downloader-0.1.2/src/umls_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-11-07 14:28:37.000000 umls_downloader-0.1.2/src/umls_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       61 2023-11-07 14:28:37.000000 umls_downloader-0.1.2/src/umls_downloader.egg-info/entry_points.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-11-07 14:24:09.000000 umls_downloader-0.1.2/src/umls_downloader.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      188 2023-11-07 14:28:37.000000 umls_downloader-0.1.2/src/umls_downloader.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       16 2023-11-07 14:28:37.000000 umls_downloader-0.1.2/src/umls_downloader.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-11-07 14:28:37.638882 umls_downloader-0.1.2/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       65 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      409 2023-11-07 14:18:54.000000 umls_downloader-0.1.2/tests/test_version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-02 08:03:27.386345 umls_downloader-0.1.3/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2023-11-07 14:18:54.000000 umls_downloader-0.1.3/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      347 2023-11-07 14:18:54.000000 umls_downloader-0.1.3/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7487 2024-04-02 08:03:27.386265 umls_downloader-0.1.3/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5663 2023-11-07 14:18:54.000000 umls_downloader-0.1.3/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-02 08:03:27.378442 umls_downloader-0.1.3/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-02 08:03:27.379933 umls_downloader-0.1.3/docs/source/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6937 2024-04-02 08:03:26.000000 umls_downloader-0.1.3/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      484 2023-11-07 14:18:54.000000 umls_downloader-0.1.3/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      376 2023-11-07 14:18:54.000000 umls_downloader-0.1.3/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2396 2024-04-02 08:03:27.386759 umls_downloader-0.1.3/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-02 08:03:27.378584 umls_downloader-0.1.3/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-02 08:03:27.384313 umls_downloader-0.1.3/src/umls_downloader/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      772 2024-03-28 14:20:57.000000 umls_downloader-0.1.3/src/umls_downloader/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      332 2023-11-07 14:18:54.000000 umls_downloader-0.1.3/src/umls_downloader/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4447 2023-11-07 14:18:54.000000 umls_downloader-0.1.3/src/umls_downloader/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2641 2023-11-07 14:18:54.000000 umls_downloader-0.1.3/src/umls_downloader/cli.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2352 2023-11-07 14:18:54.000000 umls_downloader-0.1.3/src/umls_downloader/rxnorm.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2388 2023-11-07 14:18:54.000000 umls_downloader-0.1.3/src/umls_downloader/semmeddb.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1263 2023-11-07 14:18:54.000000 umls_downloader-0.1.3/src/umls_downloader/snomed.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8395 2024-03-28 15:27:45.000000 umls_downloader-0.1.3/src/umls_downloader/umls.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1036 2024-04-02 08:03:26.000000 umls_downloader-0.1.3/src/umls_downloader/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-02 08:03:27.385693 umls_downloader-0.1.3/src/umls_downloader.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7487 2024-04-02 08:03:27.000000 umls_downloader-0.1.3/src/umls_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)      707 2024-04-02 08:03:27.000000 umls_downloader-0.1.3/src/umls_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-04-02 08:03:27.000000 umls_downloader-0.1.3/src/umls_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       61 2024-04-02 08:03:27.000000 umls_downloader-0.1.3/src/umls_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-11-07 14:24:09.000000 umls_downloader-0.1.3/src/umls_downloader.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      188 2024-04-02 08:03:27.000000 umls_downloader-0.1.3/src/umls_downloader.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       16 2024-04-02 08:03:27.000000 umls_downloader-0.1.3/src/umls_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-02 08:03:27.385445 umls_downloader-0.1.3/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       65 2023-11-07 14:18:54.000000 umls_downloader-0.1.3/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      409 2023-11-07 14:18:54.000000 umls_downloader-0.1.3/tests/test_version.py
```

### Comparing `umls_downloader-0.1.2/LICENSE` & `umls_downloader-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `umls_downloader-0.1.2/PKG-INFO` & `umls_downloader-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umls_downloader
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automate downloading UMLS data.
 Home-page: https://github.com/cthoyt/umls_downloader
 Download-URL: https://github.com/cthoyt/umls_downloader/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: umls_downloader Version: 0.1.2 Summary: Automate
+Metadata-Version: 2.1 Name: umls_downloader Version: 0.1.3 Summary: Automate
 downloading UMLS data. Home-page: https://github.com/cthoyt/umls_downloader
 Download-URL: https://github.com/cthoyt/umls_downloader/releases Author:
 Charles Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley
 Hoyt Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/umls_downloader/issues Project-URL: Source Code,
 https://github.com/cthoyt/umls_downloader Keywords:
 snekpack,cookiecutter,UMLS,SNOMED-CT,RxNorm Classifier: Development Status :: 1
```

### Comparing `umls_downloader-0.1.2/README.md` & `umls_downloader-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `umls_downloader-0.1.2/docs/source/conf.py` & `umls_downloader-0.1.3/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "umls_downloader"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.1.2"
+release = "0.1.3"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
@@ -222,12 +222,12 @@
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    "https://docs.python.org/3/": None,
+    "python": ("https://docs.python.org/3", None),
 }
 
 autoclass_content = "both"
 autodoc_member_order = "bysource"
```

### Comparing `umls_downloader-0.1.2/setup.cfg` & `umls_downloader-0.1.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = umls_downloader
-version = 0.1.2
+version = 0.1.3
 description = Automate downloading UMLS data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cthoyt/umls_downloader
 download_url = https://github.com/cthoyt/umls_downloader/releases
 project_urls = 
 	Bug Tracker = https://github.com/cthoyt/umls_downloader/issues
@@ -97,19 +97,19 @@
 
 [darglint]
 docstring_style = sphinx
 strictness = short
 
 [flake8]
 ignore = 
-	S301 # pickle
-	S403 # pickle
+	S301
+	S403
 	S404
 	S603
-	W503 # Line break before binary operator (flake8 is wrong)
+	W503
 exclude = 
 	.tox,
 	.git,
 	__pycache__,
 	docs/source/conf.py,
 	build,
 	dist,
```

### Comparing `umls_downloader-0.1.2/src/umls_downloader/__init__.py` & `umls_downloader-0.1.3/src/umls_downloader/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,8 +9,16 @@
     download_semmeddb_concept,
     download_semmeddb_entity,
     download_semmeddb_predication,
     download_semmeddb_predication_aux,
     download_semmeddb_sentence,
 )
 from .snomed import download_snomed_international, download_snomed_us  # noqa:F401
-from .umls import download_umls, download_umls_metathesaurus, open_umls  # noqa:F401
+from .umls import (  # noqa:F401
+    download_umls,
+    download_umls_full,
+    download_umls_metathesaurus,
+    open_umls,
+    open_umls_full,
+    open_umls_hierarchy,
+    open_umls_semantic_types,
+)
```

### Comparing `umls_downloader-0.1.2/src/umls_downloader/api.py` & `umls_downloader-0.1.3/src/umls_downloader/api.py`

 * *Files identical despite different names*

### Comparing `umls_downloader-0.1.2/src/umls_downloader/cli.py` & `umls_downloader-0.1.3/src/umls_downloader/cli.py`

 * *Files identical despite different names*

### Comparing `umls_downloader-0.1.2/src/umls_downloader/rxnorm.py` & `umls_downloader-0.1.3/src/umls_downloader/rxnorm.py`

 * *Files identical despite different names*

### Comparing `umls_downloader-0.1.2/src/umls_downloader/semmeddb.py` & `umls_downloader-0.1.3/src/umls_downloader/semmeddb.py`

 * *Files identical despite different names*

### Comparing `umls_downloader-0.1.2/src/umls_downloader/snomed.py` & `umls_downloader-0.1.3/src/umls_downloader/snomed.py`

 * *Files identical despite different names*

### Comparing `umls_downloader-0.1.2/src/umls_downloader/version.py` & `umls_downloader-0.1.3/src/umls_downloader/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`umls_downloader` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `umls_downloader-0.1.2/src/umls_downloader.egg-info/PKG-INFO` & `umls_downloader-0.1.3/src/umls_downloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: umls-downloader
-Version: 0.1.2
+Name: umls_downloader
+Version: 0.1.3
 Summary: Automate downloading UMLS data.
 Home-page: https://github.com/cthoyt/umls_downloader
 Download-URL: https://github.com/cthoyt/umls_downloader/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: umls-downloader Version: 0.1.2 Summary: Automate
+Metadata-Version: 2.1 Name: umls_downloader Version: 0.1.3 Summary: Automate
 downloading UMLS data. Home-page: https://github.com/cthoyt/umls_downloader
 Download-URL: https://github.com/cthoyt/umls_downloader/releases Author:
 Charles Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley
 Hoyt Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/umls_downloader/issues Project-URL: Source Code,
 https://github.com/cthoyt/umls_downloader Keywords:
 snekpack,cookiecutter,UMLS,SNOMED-CT,RxNorm Classifier: Development Status :: 1
```

### Comparing `umls_downloader-0.1.2/src/umls_downloader.egg-info/SOURCES.txt` & `umls_downloader-0.1.3/src/umls_downloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

