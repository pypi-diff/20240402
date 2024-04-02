# Comparing `tmp/pangeo-forge-esgf-0.1.1.tar.gz` & `tmp/pangeo-forge-esgf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangeo-forge-esgf-0.1.1.tar", last modified: Thu Nov 16 19:28:28 2023, max compression
+gzip compressed data, was "pangeo-forge-esgf-0.2.0.tar", last modified: Tue Apr  2 19:14:55 2024, max compression
```

## Comparing `pangeo-forge-esgf-0.1.1.tar` & `pangeo-forge-esgf-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 19:28:28.135117 pangeo-forge-esgf-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 19:28:28.131117 pangeo-forge-esgf-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 19:28:28.131117 pangeo-forge-esgf-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/.github/workflows/pythonpublish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2023-11-16 19:28:28.135117 pangeo-forge-esgf-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 19:28:28.131117 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-16 19:28:27.000000 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16551 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf/recipe_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 19:28:28.135117 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf/tests/test_recipe_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 19:28:28.131117 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2023-11-16 19:28:28.000000 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-11-16 19:28:28.000000 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 19:28:28.000000 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 19:28:28.000000 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-16 19:28:28.000000 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-16 19:28:28.000000 pangeo-forge-esgf-0.1.1/pangeo_forge_esgf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-11-16 19:28:28.135117 pangeo-forge-esgf-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2023-11-16 19:28:18.000000 pangeo-forge-esgf-0.1.1/test_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:14:55.315451 pangeo-forge-esgf-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:14:55.311452 pangeo-forge-esgf-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:14:55.311452 pangeo-forge-esgf-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/.github/workflows/pythonpublish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-02 19:14:55.315451 pangeo-forge-esgf-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:14:55.311452 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 19:14:55.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17813 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/recipe_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:14:55.315451 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/tests/test_recipe_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:14:55.315451 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-02 19:14:55.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 19:14:55.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:14:55.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 19:14:55.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 19:14:55.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:14:55.315451 pangeo-forge-esgf-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/test_script.py
```

### Comparing `pangeo-forge-esgf-0.1.1/.gitignore` & `pangeo-forge-esgf-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pangeo-forge-esgf-0.1.1/.pre-commit-config.yaml` & `pangeo-forge-esgf-0.2.0/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    # Ruff version.
+    rev: v0.3.5
     hooks:
-      - id: isort
-  - repo: https://github.com/psf/black
-    rev: 23.1.0
+      # Run the linter.
+      - id: ruff
+        args: [ --fix ]
+      # Run the formatter.
+      - id: ruff-format
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: 'v1.9.0'  # Use the sha / tag you want to point at
     hooks:
-      - id: black
-  - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
-    hooks:
-      - id: flake8
+    -   id: mypy
+        additional_dependencies: ["types-requests"]
+        exclude: "test_script.py"
```

### Comparing `pangeo-forge-esgf-0.1.1/LICENSE` & `pangeo-forge-esgf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pangeo-forge-esgf-0.1.1/PKG-INFO` & `pangeo-forge-esgf-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,74 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-esgf
-Version: 0.1.1
-Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
-Home-page: https://github.com/jbusecke/pangeo-forge-esgf
-Maintainer: Julius Busecke
-Maintainer-email: julius@ldeo.columbia.edu
-License: Apache
+Version: 0.2.0
+Summary: Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge
+Author-email: Julius Busecke <julius@ldeo.columbia.edu>
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/jbusecke/pangeo-forge-esgf
+Project-URL: Tracker, https://github.com/jbusecke/pangeo-forge-esgf/issues
 Keywords: pangeo,data,esgf
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: tqdm
+Requires-Dist: backoff
+Requires-Dist: requests
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: types-requests; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pangeo-forge-esgf[test]; extra == "dev"
 
 # pangeo-forge-esgf
 
 Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge
 
+## Install
+You can install pangeo-forge-esgf via pip:
+```
+pip install pangeo-forge-esgf
+```
+
+If you want all the required dependencies for testing and development simply do:
+```
+pip install pangeo-forge-esgf[dev]
+```
+
 ## Parsing a list of instance ids using wildcards
 
 Pangeo forge recipes require the user to provide exact instance_id's for the datasets they want to be processed. Discovering these with the [web search](https://esgf-node.llnl.gov/search/cmip6/) can become cumbersome, especially when dealing with a large number of members/models etc.
 
 `pangeo-forge-esgf` provides some functions to query the ESGF API based on instance_id values with wildcards.
 
 For example if you want to find all the zonal (`uo`) and meridonal (`vo`) velocities available for the `lgm` experiment of PMIP, you can do:
 
 ```python
 from pangeo_forge_esgf.parsing import parse_instance_ids
 parse_iids = [
-    "CMIP6.PMIP.*.*.lgm.*.*.uo.*.*",
-    "CMIP6.PMIP.*.*.lgm.*.*.vo.*.*",
+    "CMIP6.PMIP.*.*.lgm.*.*.[uo, vo].*.*",
 ]
+# Comma separated values in square brackets will be expanded and the above is equivalent to:
+# parse_iids = [
+#     "CMIP6.PMIP.*.*.lgm.*.*.[uo, vo].*.*", # this is equivalent to passing
+#     "CMIP6.PMIP.*.*.lgm.*.*.vo.*.*",
+# ]
 iids = []
 for piid in parse_iids:
     iids.extend(parse_instance_ids(piid))
 iids
 ```
 
 and you will get:
@@ -90,10 +116,7 @@
 ```python
 from pangeo_forge_esgf import get_urls_from_esgf, setup_logging
 setup_logging('DEBUG')
 iids = ['CMIP6.CMIP.CSIRO-ARCCSS.ACCESS-CM2.historical.r1i1p1f1.SImon.sifb.gn.v20200817']
 url_dict = await get_urls_from_esgf(iids)
 url_dict['CMIP6.CMIP.CSIRO-ARCCSS.ACCESS-CM2.historical.r1i1p1f1.SImon.sifb.gn.v20200817']
 ```
-
-
-
```

### Comparing `pangeo-forge-esgf-0.1.1/README.md` & `pangeo-forge-esgf-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 # pangeo-forge-esgf
 
 Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge
 
+## Install
+You can install pangeo-forge-esgf via pip:
+```
+pip install pangeo-forge-esgf
+```
+
+If you want all the required dependencies for testing and development simply do:
+```
+pip install pangeo-forge-esgf[dev]
+```
+
 ## Parsing a list of instance ids using wildcards
 
 Pangeo forge recipes require the user to provide exact instance_id's for the datasets they want to be processed. Discovering these with the [web search](https://esgf-node.llnl.gov/search/cmip6/) can become cumbersome, especially when dealing with a large number of members/models etc.
 
 `pangeo-forge-esgf` provides some functions to query the ESGF API based on instance_id values with wildcards.
 
 For example if you want to find all the zonal (`uo`) and meridonal (`vo`) velocities available for the `lgm` experiment of PMIP, you can do:
 
 ```python
 from pangeo_forge_esgf.parsing import parse_instance_ids
 parse_iids = [
-    "CMIP6.PMIP.*.*.lgm.*.*.uo.*.*",
-    "CMIP6.PMIP.*.*.lgm.*.*.vo.*.*",
+    "CMIP6.PMIP.*.*.lgm.*.*.[uo, vo].*.*",
 ]
+# Comma separated values in square brackets will be expanded and the above is equivalent to:
+# parse_iids = [
+#     "CMIP6.PMIP.*.*.lgm.*.*.[uo, vo].*.*", # this is equivalent to passing
+#     "CMIP6.PMIP.*.*.lgm.*.*.vo.*.*",
+# ]
 iids = []
 for piid in parse_iids:
     iids.extend(parse_instance_ids(piid))
 iids
 ```
 
 and you will get:
@@ -67,8 +82,7 @@
 ```python
 from pangeo_forge_esgf import get_urls_from_esgf, setup_logging
 setup_logging('DEBUG')
 iids = ['CMIP6.CMIP.CSIRO-ARCCSS.ACCESS-CM2.historical.r1i1p1f1.SImon.sifb.gn.v20200817']
 url_dict = await get_urls_from_esgf(iids)
 url_dict['CMIP6.CMIP.CSIRO-ARCCSS.ACCESS-CM2.historical.r1i1p1f1.SImon.sifb.gn.v20200817']
 ```
-
```

### Comparing `pangeo-forge-esgf-0.1.1/pangeo_forge_esgf/__init__.py` & `pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from .recipe_inputs import get_urls_from_esgf
 import logging
-import backoff #noqa #https://github.com/litl/backoff/issues/71
+import backoff  # noqa #https://github.com/litl/backoff/issues/71
 
-logging.getLogger('backoff').setLevel(logging.FATAL) 
+try:
+    from ._version import __version__
+except ImportError:
+    __version__ = "unknown"
+
+logging.getLogger("backoff").setLevel(logging.FATAL)
 # not sure if this is needed, but I want to avoid the many backoff messages
 
+
 def setup_logging(level: str = "INFO"):
     """A convenience function that sets up logging for developing and debugging recipes in Jupyter,
     iPython, or another interactive context.
 
     :param level: One of (in decreasing level of detail) ``"DEBUG"``, ``"INFO"``, or ``"WARNING"``.
       Defaults to ``"INFO"``.
     """
@@ -19,14 +25,16 @@
 
         handler = RichHandler()
         handler.setFormatter(logging.Formatter("%(message)s"))
     except ImportError:
         import sys
 
         handler = logging.StreamHandler(stream=sys.stdout)
-        handler.setFormatter(logging.Formatter("%(name)s - %(levelname)s - %(message)s"))
+        handler.setFormatter(
+            logging.Formatter("%(name)s - %(levelname)s - %(message)s")
+        )
 
     logger = logging.getLogger("pangeo_forge_esgf")
     if logger.hasHandlers():
         logger.handlers.clear()
     logger.setLevel(getattr(logging, level))
     logger.addHandler(handler)
```

### Comparing `pangeo-forge-esgf-0.1.1/pangeo_forge_esgf/recipe_inputs.py` & `pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/recipe_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,60 @@
 import aiohttp
 import asyncio
 import logging
 import backoff
 
 from .utils import facets_from_iid
-from typing import Dict, List, Tuple, Any, Optional
+from typing import Dict, List, Tuple, Any, Optional, Union
+
 # import backoff #might still be using the backoff stuff later
 from tqdm.asyncio import tqdm
 
 logger = logging.getLogger(__name__)
 
 
 ## async steps
 def backoff_hdlr(details):
-    logger.debug("Backing off {wait:0.1f} seconds after {tries} tries "
-           "calling function {target} with args {args} and kwargs "
-           "{kwargs}".format(**details))
+    logger.debug(
+        "Backing off {wait:0.1f} seconds after {tries} tries "
+        "calling function {target} with args {args} and kwargs "
+        "{kwargs}".format(**details)
+    )
+
 
 @backoff.on_predicate(
     backoff.constant,
     lambda x: x is None,
     on_backoff=backoff_hdlr,
-    interval = 5, # in seconds
-    max_tries = 2, 
+    interval=5,  # in seconds
+    max_tries=2,
 )
 async def url_responsive(
-        session: aiohttp.ClientSession,
-        semaphore: asyncio.BoundedSemaphore,
-        url: str,  
-        timeout: int
-        ) -> bool:
+    session: aiohttp.ClientSession,
+    semaphore: asyncio.BoundedSemaphore,
+    url: str,
+    timeout: int,
+) -> Union[None, str]:
     async with semaphore:
         try:
             async with session.get(url, timeout=timeout) as resp:
-                if resp.status <= 300: # TODO: Is this a good way to check if the search node and data_url is responsive?
+                if (
+                    resp.status <= 300
+                ):  # TODO: Is this a good way to check if the search node and data_url is responsive?
                     return url
+                else:
+                    resp.raise_for_status()
+                    return None  # mypy did not like the missing return, but this smells to me.
+                    # maybe I should overthink this design. In the end I want to backoff on None, but also get the actual exception back.
+                    # There might be a better way to achive this.
         except Exception as e:
             logger.debug(f"Responsivness check for {url=} failed with: {e}")
             return None
 
+
 # @backoff.on_exception(
 #     backoff.expo,
 #     (aiohttp.ClientError, asyncio.TimeoutError),
 #     max_time = 60, # in seconds
 #     base=5, # prevent the backoff from being too short in the first tries
 #     on_backoff=backoff_hdlr,
 #     jitter=backoff.full_jitter,
@@ -50,125 +62,146 @@
 # NOTE: I am going to use a predicate backoff as above here. This will more broadly back off on anything that returns a None here.
 # Might consider wrapping the pure request in a backoff.on_exception separately. Worried that the Timeouts here would accumulate.
 # but for now this should be fine.
 @backoff.on_predicate(
     backoff.expo,
     lambda x: x is None,
     on_backoff=backoff_hdlr,
-    max_time = 30, # in seconds
+    max_time=30,  # in seconds
     base=4,
 )
 async def get_response_data(
     session: aiohttp.ClientSession,
     semaphore: asyncio.BoundedSemaphore,
     url: str,
     params: Dict[str, str],
-    timeout: int
-    ) -> str:
+    timeout: int,
+) -> Union[None, str]:
     async with semaphore:
         try:
-            async with session.get(url, params=params, timeout=timeout, raise_for_status=True) as response:
+            async with session.get(
+                url, params=params, timeout=timeout, raise_for_status=True
+            ) as response:
                 response_data = await response.json(
                     content_type="text/json"
                 )  # https://stackoverflow.com/questions/48840378/python-attempt-to-decode-json-with-unexpected-mimetype
             return response_data
         # except asyncio.TimeoutError:
         #     logger.debug(f"Timeout for {url}")
-        #     return None 
+        #     return None
         # except aiohttp.ClientError:
         #     logger.debug(f"ClientError for {url}")
         #     return None
         except Exception as e:
             logger.debug(f"Getting response data for {url=} failed with: {e}")
-            return None # should trigger a backoff 
+            return None  # should trigger a backoff
+
 
 ## mid-level steps (not directly making requests)
-async def filter_responsive_urls(session: aiohttp.ClientSession, semaphore: asyncio.BoundedSemaphore, node_list: List[str]) -> List[str]:
+async def filter_responsive_urls(
+    session: aiohttp.ClientSession,
+    semaphore: asyncio.BoundedSemaphore,
+    node_list: List[str],
+) -> List[str]:
     """Filters a list of search nodes for those that are responsive."""
     tasks = []
     for url in node_list:
-        tasks.append(asyncio.ensure_future(url_responsive(session, semaphore, url, timeout=10)))
+        tasks.append(
+            asyncio.ensure_future(url_responsive(session, semaphore, url, timeout=10))
+        )
 
     unfiltered_urls = await asyncio.gather(*tasks)
     return [url for url in unfiltered_urls if url is not None]
 
+
 async def get_first_responsive_url(
-        session: aiohttp.ClientSession,
-        semaphore: asyncio.BoundedSemaphore,
-        iid_url_tuple: Tuple[str, List[str]]) -> Tuple[str, str]:
+    session: aiohttp.ClientSession,
+    semaphore: asyncio.BoundedSemaphore,
+    iid_url_tuple: Tuple[str, List[str]],
+) -> Union[Tuple[str, str], Tuple[str, None]]:
     """Filters a list of search nodes for those that are responsive."""
     label, url_list = iid_url_tuple
-    try: 
+    try:
         tasks = []
         for url in url_list:
-            tasks.append(asyncio.ensure_future(url_responsive(session, semaphore, url, timeout=30)))
+            tasks.append(
+                asyncio.ensure_future(
+                    url_responsive(session, semaphore, url, timeout=30)
+                )
+            )
 
         done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
         for p in pending:
-            p.cancel()    
+            p.cancel()
         return (label, done.pop().result())
     except Exception as e:
         logger.warn(f"Error for {label=}: {e}")
         return (label, None)
 
+
 async def get_urls_for_iid(
-        session: aiohttp.ClientSession,
-        semaphore: asyncio.BoundedSemaphore,
-        iid: str,
-        node_url: str,
-        timeout: int,
-        ) -> str:
+    session: aiohttp.ClientSession,
+    semaphore: asyncio.BoundedSemaphore,
+    iid: str,
+    node_url: str,
+    timeout: int,
+) -> Union[None, Dict[str, List[Dict[str, str]]]]:
     params = esgf_params_from_iid({}, iid)
     logger.debug(f"{iid=} Requesting from {node_url=} {params =}")
-    iid_response = await get_response_data(session, semaphore, node_url, params=params, timeout=timeout)
+    iid_response = await get_response_data(
+        session, semaphore, node_url, params=params, timeout=timeout
+    )
     # check validity of response
     if iid_response is None:
         logger.debug(f"{iid =}: Got no response  {node_url=}")
         return None
-    elif iid_response['response']['numFound'] == 0:
+    elif iid_response["response"]["numFound"] == 0:
         logger.debug(f"{iid =}: No files found on {node_url=}")
         return None
     else:
         # return only the payload
-        return {iid: iid_response['response']["docs"]}
-    
+        return {iid: iid_response["response"]["docs"]}
+
 
 ## utility processing functions (working on response output)
-def get_http(urls:list[str]) -> str:
+def get_http(urls: list[str]) -> str:
     """Filter for http urls"""
-    [url] = [url.split('|')[0] for url in urls if url.endswith('HTTPServer')]
+    [url] = [url.split("|")[0] for url in urls if url.endswith("HTTPServer")]
     return url
 
-def nest_dict_from_keyed_list(keyed_list:List[Tuple[str, Any]], sep:str = '|'):
+
+def nest_dict_from_keyed_list(
+    keyed_list: List[Tuple[str, Any]], sep: str = "|"
+) -> Dict[str, Dict[str, str]]:
     """
-    Creates nested dict from a flat list of tuples (key, value) 
+    Creates nested dict from a flat list of tuples (key, value)
     where key is a string with a separator indicating the levels of the dict.
     This is not general(only works on two levels), but works for the specific case of the ESGF search API
     """
-    new_dict = {}
+    new_dict: Dict[str, Any] = {}
 
     for label, url in keyed_list:
         # split label
-        iid, filename = label.split('|')
+        iid, filename = label.split("|")
         if iid not in new_dict.keys():
             new_dict[iid] = {}
         if filename not in new_dict[iid].keys():
             new_dict[iid][filename] = url
     return new_dict
 
-def sort_urls_by_time(urls:List[str]) -> List[str]:
+
+def sort_urls_by_time(urls: List[str]) -> List[str]:
     """Sorts a list of urls by the time stamp in the filename."""
-    sorted_urls = sorted(urls, key=lambda x: x.split('/')[-1])
+    sorted_urls = sorted(urls, key=lambda x: x.split("/")[-1])
     return sorted_urls
 
+
 def url_result_processing(
-    flat_urls_per_file:List[Tuple[str, str]],
-    expected_files: Dict[str, List[str]]
-    ):
-    
+    flat_urls_per_file: List[Tuple[str, str]], expected_files: Dict[str, List[str]]
+) -> Dict[str, List[str]]:
     filtered_dict = nest_dict_from_keyed_list(flat_urls_per_file)
 
     # now check which files are missing per iid
     files_found_per_iid = {}
     for iid in filtered_dict.keys():
         required_files = len(expected_files[iid])
         if iid in filtered_dict.keys():
@@ -178,207 +211,258 @@
         files_found_per_iid[iid] = (found_files, required_files)
 
     # iid_results_combined is the ground truth about which files should be present
     # create final dict with urls if all files are found
     url_dict = {}
     for iid, counts in files_found_per_iid.items():
         if counts[0] != counts[1]:
-            logger.debug(f"Skipping {iid} because not all files were found. Found {counts[0]} out of {counts[1]}")
-            logger.debug(f'Found files: {list(filtered_dict[iid].keys())}')
+            logger.debug(
+                f"Skipping {iid} because not all files were found. Found {counts[0]} out of {counts[1]}"
+            )
+            logger.debug(f"Found files: {list(filtered_dict[iid].keys())}")
             logger.debug(f"Expected files: {list(expected_files[iid])}")
         else:
             # sort urls by filname only
             urls = [url for filename, url in filtered_dict[iid].items()]
             url_dict[iid] = sort_urls_by_time(urls)
     return url_dict
 
+
 def flatten_iid_filename(iid, r):
     return f"{iid}|{r['id'].split('|')[0]}"
 
-def get_unique_filenames(iid_results: List[Dict[str, List[Dict[str, str]]]]) -> Dict[str, List[str]]:
+
+def get_unique_filenames(
+    iid_results: List[Dict[str, List[Dict[str, str]]]],
+) -> Dict[str, List[str]]:
     """Extract unique filenames from results"""
     filename_dict = {}
     for result in iid_results:
         for iid, res in result.items():
             filenames = []
             for r in res:
-                filename = r['id'].split("|")[0]
+                filename = r["id"].split("|")[0]
                 filenames.append(filename)
             sorted_unique_filenames = sort_urls_by_time(list(set(filenames)))
 
             # check for duplicate timesteps
-            unique_timesteps = set([f.split('_')[-1] for f in sorted_unique_filenames])
+            unique_timesteps = set([f.split("_")[-1] for f in sorted_unique_filenames])
             if len(unique_timesteps) != len(sorted_unique_filenames):
                 raise ValueError(
                     "Duplicate files found. This sometimes happens when the "
                     f"API returns multiple versions. Got {sorted_unique_filenames}."
-                    )
-            
-            filename_dict[iid] = sorted_unique_filenames        
+                )
+
+            filename_dict[iid] = sorted_unique_filenames
     return filename_dict
 
-def esgf_params_from_iid(params: Dict[str, str], iid: str):
+
+def esgf_params_from_iid(params: Dict[str, str], iid: str) -> Dict[str, str]:
     """Generates parameters for a GET request to the ESGF API based on the instance id."""
     # set default search parameters
-    default_params = {
+    default_params: Dict[str, str] = {
         "type": "File",
         "retracted": "false",
         "format": "application/solr+json",
         "fields": "id, url, title, latest, replica, data_node",
         "distrib": "true",
-        "limit": 500,  # This determines the number of urls/files that are returned. I dont expect this to be ever more than 500?
+        "limit": "500",  # This determines the number of urls/files that are returned. I dont expect this to be ever more than 500?
     }
     params = default_params | params
     facets = facets_from_iid(iid)
     # `v` has to be removed from version
     if "version" in facets:
         facets["version"] = facets["version"].replace("v", "")
 
     # combine params and facets
     params = params | facets
     return params
 
 
-preferred_data_nodes = ['a']
+preferred_data_nodes = ["a"]
+
+
 def filter_urls_preferred_node(a):
     pass
 
+
 def filter_urls_first(iid_url_tuple_list: List[Tuple[str, List[str]]]):
     """Just get the first url for each file
     iid_url_tuple_list looks something like this: [('some.iid.you.like|some.filename.pattern', [url1, url2])]
     """
     filtered_list = []
     for iid, urls in iid_url_tuple_list:
         assert len(urls) > 0
         url = urls[0]
         filtered_list.append((iid, url))
     return filtered_list
 
+
 async def filter_urls_first_responsive(
     session: aiohttp.ClientSession,
     semaphore: asyncio.BoundedSemaphore,
-    iid_url_tuple_list: List[Tuple[str, List[str]]]
-    ) -> List[Tuple[str, List[str]]]:
+    iid_url_tuple_list: List[Tuple[str, List[str]]],
+) -> List[Tuple[str, List[str]]]:
     tasks = []
     for iid_url_tuple in iid_url_tuple_list:
-        tasks.append(asyncio.ensure_future(get_first_responsive_url(session, semaphore, iid_url_tuple)))
+        tasks.append(
+            asyncio.ensure_future(
+                get_first_responsive_url(session, semaphore, iid_url_tuple)
+            )
+        )
     results = await tqdm.gather(
         *tasks,
         position=0,
-        leave=True, #https://stackoverflow.com/questions/41707229/why-is-tqdm-printing-to-a-newline-instead-of-updating-the-same-line
-        miniters= int(len(tasks)/10), #https://stackoverflow.com/questions/47995958/python-tqdm-package-how-to-configure-for-less-frequent-status-bar-updates
-        maxinterval=float("inf")
-        ) 
+        leave=True,  # https://stackoverflow.com/questions/41707229/why-is-tqdm-printing-to-a-newline-instead-of-updating-the-same-line
+        miniters=int(
+            len(tasks) / 10
+        ),  # https://stackoverflow.com/questions/47995958/python-tqdm-package-how-to-configure-for-less-frequent-status-bar-updates
+        maxinterval=float("inf"),
+    )
     filtered_results = [r for r in results if r[1] is not None]
     return filtered_results
 
 
 async def get_urls_from_esgf(
-        iids: List[str],
-        limit_per_host: int = 50,
-        max_concurrency: int = 50,
-        max_concurrency_response: int = 50,
-        search_nodes: Optional[List[str]] = None,
-        choose_url: str = 'first',
-        
+    iids: List[str],
+    limit_per_host: int = 50,
+    max_concurrency: int = 50,
+    max_concurrency_response: int = 50,
+    search_nodes: Optional[List[str]] = None,
+    choose_url: str = "first",
 ):
     if search_nodes is None:
         search_nodes = [
             "http://esgf-node.llnl.gov/esg-search/search",
             "http://esgf-data.dkrz.de/esg-search/search",
             "http://esgf-node.ipsl.upmc.fr/esg-search/search",
             "http://esgf-index1.ceda.ac.uk/esg-search/search",
             "http://esg-dn1.nsc.liu.se/esg-search/search",
             "http://esgf.nci.org.au/esg-search/search",
         ]
-    
-    semaphore = asyncio.BoundedSemaphore(max_concurrency) #https://quentin.pradet.me/blog/how-do-you-limit-memory-usage-with-asyncio.html
+
+    semaphore = asyncio.BoundedSemaphore(
+        max_concurrency
+    )  # https://quentin.pradet.me/blog/how-do-you-limit-memory-usage-with-asyncio.html
     semaphore_responsive = asyncio.BoundedSemaphore(max_concurrency_response)
-    connector = aiohttp.TCPConnector(
-        limit_per_host=limit_per_host
-    )
+    connector = aiohttp.TCPConnector(limit_per_host=limit_per_host)
     async with aiohttp.ClientSession(connector=connector) as session:
         logger.info(f"Checking responsiveness of {search_nodes=}")
-        responsive_search_nodes = await filter_responsive_urls(session, semaphore_responsive, search_nodes)
+        responsive_search_nodes = await filter_responsive_urls(
+            session, semaphore_responsive, search_nodes
+        )
         if len(responsive_search_nodes) == 0:
             raise RuntimeError(f"None of the {search_nodes=} are responsive")
         logger.info(f"{responsive_search_nodes=}")
 
-        # We are now basically making requests to all search nodes fore each iid. This will return 
+        # We are now basically making requests to all search nodes fore each iid. This will return
         # results on a *file* basis. While this is rather redundant, I have seen cases where there are
         # inconsistencies between search nodes, and I just want to make super sure that we get every single
         # file/url combo that might be available. To speed this up, just trim the list of search nodes!
 
         logger.info("Requesting urls")
         logger.debug(f"for {iids=}")
         tasks = []
         for iid in iids:
             for search_node in responsive_search_nodes:
-                tasks.append(asyncio.ensure_future(get_urls_for_iid(session, semaphore, iid, search_node, timeout=10)))
-        
+                tasks.append(
+                    asyncio.ensure_future(
+                        get_urls_for_iid(
+                            session, semaphore, iid, search_node, timeout=10
+                        )
+                    )
+                )
+
         # trying with a progressbar
         iid_results = await tqdm.gather(
             *tasks,
-            position=0, 
-            leave=True,# https://stackoverflow.com/questions/41707229/why-is-tqdm-printing-to-a-newline-instead-of-updating-the-same-line
-            miniters= int(len(tasks)/10), #https://stackoverflow.com/questions/47995958/python-tqdm-package-how-to-configure-for-less-frequent-status-bar-updates
+            position=0,
+            leave=True,  # https://stackoverflow.com/questions/41707229/why-is-tqdm-printing-to-a-newline-instead-of-updating-the-same-line
+            miniters=int(
+                len(tasks) / 10
+            ),  # https://stackoverflow.com/questions/47995958/python-tqdm-package-how-to-configure-for-less-frequent-status-bar-updates
             maxinterval=float("inf"),
-            ) 
+        )
         logger.info("Processing responses")
 
         # filter out None values
         iid_results_filtered = [result for result in iid_results if result is not None]
         logger.debug(f"{iid_results_filtered =} ")
 
-        #TODO: Check if the versions submitted were latest. If not, suggest for the user to run the query again.
+        # TODO: Check if the versions submitted were latest. If not, suggest for the user to run the query again.
 
         logger.info("Processing responses: Expected files per iid")
         # split out the expected number of files per iid
         expected_files_per_iid = get_unique_filenames(iid_results_filtered)
         logger.debug(f"{expected_files_per_iid =}")
 
         logger.info("Processing responses: Check for missing iids")
         # Status message about which iids were not even found on any of the search nodes.
-        remaining_iids = [iid for iid in iids if iid in [list(r.keys())[0] for r in iid_results_filtered]]
+        remaining_iids = [
+            iid
+            for iid in iids
+            if iid in [list(r.keys())[0] for r in iid_results_filtered]
+        ]
         missing_iids = list(set(iids) - set(remaining_iids))
         if len(missing_iids) > 0:
-            logger.warn(f"Not able to find results for the following {len(missing_iids)} iids: {missing_iids}")
-        
+            logger.warn(
+                f"Not able to find results for the following {len(missing_iids)} iids: {missing_iids}"
+            )
+
         # convert flat list of results to dictionary(iid: dict(filename:[unique_urls]))
         logger.info("Processing responses: Flatten results")
-        keyed_results = [(flatten_iid_filename(iid, r), get_http(r['url'])) for r_dict in iid_results_filtered for iid,r_list in r_dict.items() for r in r_list]
+        keyed_results = [
+            (flatten_iid_filename(iid, r), get_http(r["url"]))
+            for r_dict in iid_results_filtered
+            for iid, r_list in r_dict.items()
+            for r in r_list
+        ]
         logger.debug(f"{keyed_results =} ")
 
         logger.info("Processing responses: Group results")
         # aggregate urls of results per iid and filename
-        group_dict = {}
+        group_dict: Dict[str, List[str]] = {}
         for r in keyed_results:
             if r[0] not in group_dict:
                 group_dict[r[0]] = []
             group_dict[r[0]].append(r[1])
-            
-        iid_results_grouped = [(k,list(set(v))) for k,v in group_dict.items()]
+
+        iid_results_grouped = [(k, list(set(v))) for k, v in group_dict.items()]
         logger.debug(f"{iid_results_grouped =} ")
         logger.info("Choosing one url per file")
-        if choose_url == 'preferred':
-            raise NotImplementedError("Preferred data node filtering not implemented yet")
+        if choose_url == "preferred":
+            raise NotImplementedError(
+                "Preferred data node filtering not implemented yet"
+            )
             logger.info("Find preferred data node url for each file")
-            filtered_urls_per_file = filter_urls_preferred_node(iid_results_grouped, preferred_data_nodes)
-        elif choose_url == 'first':
+            filtered_urls_per_file = filter_urls_preferred_node(
+                iid_results_grouped, preferred_data_nodes
+            )
+        elif choose_url == "first":
             logger.info("Find first url for each file")
             filtered_urls_per_file = filter_urls_first(iid_results_grouped)
-        elif choose_url == 'first_responsive':
-            logger.warn("This method seems to be unreliable for getting many urls. \nIf you are getting less datasets than you expect, try 'first' instead.")
+        elif choose_url == "first_responsive":
+            logger.warn(
+                "This method seems to be unreliable for getting many urls. \nIf you are getting less datasets than you expect, try 'first' instead."
+            )
             logger.info("Find first responsive url for each file")
-            filtered_urls_per_file = await filter_urls_first_responsive(session, semaphore_responsive, iid_results_grouped)
+            filtered_urls_per_file = await filter_urls_first_responsive(
+                session, semaphore_responsive, iid_results_grouped
+            )
             logger.debug(f"{filtered_urls_per_file =} ")
         else:
-            raise ValueError(f"Unknown value for {choose_url=}. Must be one of ['preferred', 'first', 'first_responsive']")
+            raise ValueError(
+                f"Unknown value for {choose_url=}. Must be one of ['preferred', 'first', 'first_responsive']"
+            )
 
-    final_url_dict = url_result_processing(filtered_urls_per_file, expected_files_per_iid)
+    final_url_dict = url_result_processing(
+        filtered_urls_per_file, expected_files_per_iid
+    )
 
-    missing_iids = set(iids) - set(final_url_dict.keys())
+    missing_iids = list(set(iids) - set(final_url_dict.keys()))
     if len(missing_iids) > 0:
-        logger.warn(f"Was not able to construct url list for ({len(missing_iids)}/{len(iids)}) iids")
+        logger.warn(
+            f"Was not able to construct url list for ({len(missing_iids)}/{len(iids)}) iids"
+        )
         logger.info("Was not able to construct url list for the following iids:")
         logger.info(missing_iids)
-    return final_url_dict
+    return final_url_dict
```

### Comparing `pangeo-forge-esgf-0.1.1/pangeo_forge_esgf/tests/test_parsing.py` & `pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/tests/test_parsing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pangeo_forge_esgf.parsing import parse_instance_ids
+import pytest
 
 
 def test_readme_example():
     # This is possibly flaky (due to the dependence on the ESGF API)
     parse_iids = [
-        "CMIP6.PMIP.*.*.lgm.*.*.uo.*.*",
-        "CMIP6.PMIP.*.*.lgm.*.*.vo.*.*",
+        "CMIP6.PMIP.*.*.lgm.*.*.[uo,vo].*.*",
     ]
     iids = []
     for piid in parse_iids:
         iids.extend(parse_instance_ids(piid))
     iids
 
     # I expect at least these iids to be parsed
@@ -25,7 +25,22 @@
         "CMIP6.PMIP.AWI.AWI-ESM-1-1-LR.lgm.r1i1p1f1.Odec.vo.gn.v20200212",
         "CMIP6.PMIP.MIROC.MIROC-ES2L.lgm.r1i1p1f2.Omon.vo.gr1.v20200911",
         "CMIP6.PMIP.MPI-M.MPI-ESM1-2-LR.lgm.r1i1p1f1.Omon.vo.gn.v20190710",
     ]
 
     for iid in expected_iids:
         assert iid in iids
+
+
+@pytest.mark.parametrize(
+    "facet_iid, expected",
+    [
+        ("a.b.c.d", ["a.b.c.d"]),
+        ("a.[b1, b2].c.[d1, d2]", ["a.b1.c.d1", "a.b1.c.d2", "a.b2.c.d1", "a.b2.c.d2"]),
+        ("a.[b1, b2].c.d", ["a.b1.c.d", "a.b2.c.d"]),
+        ("a.b.c.[d1, d2]", ["a.b.c.d1", "a.b.c.d2"]),
+    ],
+)
+def test_split_square_brackets(facet_iid, expected):
+    from pangeo_forge_esgf.parsing import split_square_brackets
+
+    assert split_square_brackets(facet_iid) == expected
```

### Comparing `pangeo-forge-esgf-0.1.1/pangeo_forge_esgf/tests/test_recipe_inputs.py` & `pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/tests/test_recipe_inputs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import pytest
-from pangeo_forge_esgf.recipe_inputs import sort_urls_by_time, get_unique_filenames, filter_urls_first, filter_urls_preferred_node
+from pangeo_forge_esgf.recipe_inputs import (
+    sort_urls_by_time,
+    get_unique_filenames,
+    filter_urls_first,
+)
 
 
 @pytest.mark.parametrize(
     "urls_raw, expected_urls",
     [
         (
             [
@@ -24,69 +28,69 @@
     ],
 )
 def test_sort_urls_by_time(urls_raw, expected_urls):
     urls_sorted = sort_urls_by_time(urls_raw)
     for i in range(len(expected_urls)):
         assert expected_urls[i] == urls_sorted[i]
 
+
 def test_get_unique_filenames():
     filenames_w_data_node = [
-     'iid.stuff_20700101-20791231.nc|data.node.a',
-     'iid.stuff_20800101-20891231.nc|data.node.a',
-     'iid.stuff_20800101-20891231.nc|data.node.b',
+        "iid.stuff_20700101-20791231.nc|data.node.a",
+        "iid.stuff_20800101-20891231.nc|data.node.a",
+        "iid.stuff_20800101-20891231.nc|data.node.b",
     ]
     expected_filenames = [
-        'iid.stuff_20700101-20791231.nc',
-        'iid.stuff_20800101-20891231.nc',
+        "iid.stuff_20700101-20791231.nc",
+        "iid.stuff_20800101-20891231.nc",
+    ]
+    iid = "some.iid"
+    iid_results = [
+        {
+            iid: [
+                {"id": f"{filename}|data.node.stuff"}
+                for filename in filenames_w_data_node
+            ]
+        }
     ]
-    iid = 'some.iid'
-    iid_results = [{iid:[{'id':f"{filename}|data.node.stuff"} for filename in filenames_w_data_node]}]
     filename_dict = get_unique_filenames(iid_results)
     filenames = filename_dict[iid]
     for i in range(len(expected_filenames)):
         assert filenames[i] == expected_filenames[i]
-        
+
+
 def test_get_unique_filenames_raise_on_duplicates():
     filenames_w_data_node = [
-     'iid.stuff_20700101-20791231.nc|data.node.a',
-     'iid.stuff_20800101-20891231.nc|data.node.a',
-     'iid.staff_20800101-20891231.nc|data.node.a',
+        "iid.stuff_20700101-20791231.nc|data.node.a",
+        "iid.stuff_20800101-20891231.nc|data.node.a",
+        "iid.staff_20800101-20891231.nc|data.node.a",
+    ]
+    iid = "some.iid"
+    iid_results = [
+        {
+            iid: [
+                {"id": f"{filename}|data.node.stuff"}
+                for filename in filenames_w_data_node
+            ]
+        }
     ]
-    iid = 'some.iid'
-    iid_results = [{iid:[{'id':f"{filename}|data.node.stuff"} for filename in filenames_w_data_node]}]
     with pytest.raises(ValueError):
         get_unique_filenames(iid_results)
 
+
 def test_filter_first_file_urls():
     unfiltered = [
-        ('some.iid.you.like|some.filename.pattern', ['url1', 'url2']),
-        ('some.iid.you.like|some.other_filename.pattern', ['urla', 'urlb']),
-        ('some.other_iid.you.like|some.filename.pattern', ['urlc']),
-        ('some.other_iid.you.like|some.other_filename.pattern', ['urlb', 'urla']),
-        ]
+        ("some.iid.you.like|some.filename.pattern", ["url1", "url2"]),
+        ("some.iid.you.like|some.other_filename.pattern", ["urla", "urlb"]),
+        ("some.other_iid.you.like|some.filename.pattern", ["urlc"]),
+        ("some.other_iid.you.like|some.other_filename.pattern", ["urlb", "urla"]),
+    ]
     expected = [
-        ('some.iid.you.like|some.filename.pattern', 'url1'),
-        ('some.iid.you.like|some.other_filename.pattern', 'urla'),
-        ('some.other_iid.you.like|some.filename.pattern', 'urlc'),
-         ('some.other_iid.you.like|some.other_filename.pattern', 'urlb'),
-        ]
+        ("some.iid.you.like|some.filename.pattern", "url1"),
+        ("some.iid.you.like|some.other_filename.pattern", "urla"),
+        ("some.other_iid.you.like|some.filename.pattern", "urlc"),
+        ("some.other_iid.you.like|some.other_filename.pattern", "urlb"),
+    ]
     filtered = filter_urls_first(unfiltered)
     for i in range(len(expected)):
         for ii in range(2):
             assert filtered[i][ii] == expected[i][ii]
-
-# def test_filter_urls_preferred_node():
-#     unfiltered = [
-#         ('some.iid.you.like|some.filename.pattern', ['urlb', 'url2']),
-#         ('some.iid.you.like|some.other_filename.pattern', ['url2', 'urla', 'urlb']),
-#         ('some.other_iid.you.like|some.filename.pattern', ['urlc']),
-#         ('some.other_iid.you.like|some.other_filename.pattern', ['urlb', 'urla']),
-#         ]
-#     expected = [
-#         ('some.iid.you.like|some.filename.pattern', 'url2'),
-#         ('some.iid.you.like|some.other_filename.pattern', 'urla'),
-#         ('some.other_iid.you.like|some.filename.pattern', 'urlc'),
-#          ('some.other_iid.you.like|some.other_filename.pattern', 'urla'),
-#         ]
-#     filtered = filter_urls_preferred_node(unfiltered, preferred_file=['urla', 'url2'])
-#     pass
-
```

### Comparing `pangeo-forge-esgf-0.1.1/pangeo_forge_esgf.egg-info/PKG-INFO` & `pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,74 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-esgf
-Version: 0.1.1
-Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
-Home-page: https://github.com/jbusecke/pangeo-forge-esgf
-Maintainer: Julius Busecke
-Maintainer-email: julius@ldeo.columbia.edu
-License: Apache
+Version: 0.2.0
+Summary: Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge
+Author-email: Julius Busecke <julius@ldeo.columbia.edu>
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/jbusecke/pangeo-forge-esgf
+Project-URL: Tracker, https://github.com/jbusecke/pangeo-forge-esgf/issues
 Keywords: pangeo,data,esgf
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: tqdm
+Requires-Dist: backoff
+Requires-Dist: requests
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: types-requests; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pangeo-forge-esgf[test]; extra == "dev"
 
 # pangeo-forge-esgf
 
 Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge
 
+## Install
+You can install pangeo-forge-esgf via pip:
+```
+pip install pangeo-forge-esgf
+```
+
+If you want all the required dependencies for testing and development simply do:
+```
+pip install pangeo-forge-esgf[dev]
+```
+
 ## Parsing a list of instance ids using wildcards
 
 Pangeo forge recipes require the user to provide exact instance_id's for the datasets they want to be processed. Discovering these with the [web search](https://esgf-node.llnl.gov/search/cmip6/) can become cumbersome, especially when dealing with a large number of members/models etc.
 
 `pangeo-forge-esgf` provides some functions to query the ESGF API based on instance_id values with wildcards.
 
 For example if you want to find all the zonal (`uo`) and meridonal (`vo`) velocities available for the `lgm` experiment of PMIP, you can do:
 
 ```python
 from pangeo_forge_esgf.parsing import parse_instance_ids
 parse_iids = [
-    "CMIP6.PMIP.*.*.lgm.*.*.uo.*.*",
-    "CMIP6.PMIP.*.*.lgm.*.*.vo.*.*",
+    "CMIP6.PMIP.*.*.lgm.*.*.[uo, vo].*.*",
 ]
+# Comma separated values in square brackets will be expanded and the above is equivalent to:
+# parse_iids = [
+#     "CMIP6.PMIP.*.*.lgm.*.*.[uo, vo].*.*", # this is equivalent to passing
+#     "CMIP6.PMIP.*.*.lgm.*.*.vo.*.*",
+# ]
 iids = []
 for piid in parse_iids:
     iids.extend(parse_instance_ids(piid))
 iids
 ```
 
 and you will get:
@@ -90,10 +116,7 @@
 ```python
 from pangeo_forge_esgf import get_urls_from_esgf, setup_logging
 setup_logging('DEBUG')
 iids = ['CMIP6.CMIP.CSIRO-ARCCSS.ACCESS-CM2.historical.r1i1p1f1.SImon.sifb.gn.v20200817']
 url_dict = await get_urls_from_esgf(iids)
 url_dict['CMIP6.CMIP.CSIRO-ARCCSS.ACCESS-CM2.historical.r1i1p1f1.SImon.sifb.gn.v20200817']
 ```
-
-
-
```

### Comparing `pangeo-forge-esgf-0.1.1/pangeo_forge_esgf.egg-info/SOURCES.txt` & `pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-.flake8
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
-environment.yaml
 pyproject.toml
-requirements.txt
-setup.cfg
-setup.py
 test_script.py
+.github/dependabot.yml
 .github/workflows/ci.yaml
 .github/workflows/pythonpublish.yaml
 pangeo_forge_esgf/__init__.py
 pangeo_forge_esgf/_version.py
 pangeo_forge_esgf/parsing.py
 pangeo_forge_esgf/recipe_inputs.py
 pangeo_forge_esgf/utils.py
 pangeo_forge_esgf.egg-info/PKG-INFO
 pangeo_forge_esgf.egg-info/SOURCES.txt
 pangeo_forge_esgf.egg-info/dependency_links.txt
-pangeo_forge_esgf.egg-info/not-zip-safe
 pangeo_forge_esgf.egg-info/requires.txt
 pangeo_forge_esgf.egg-info/top_level.txt
+pangeo_forge_esgf/tests/test_logging.py
 pangeo_forge_esgf/tests/test_parsing.py
 pangeo_forge_esgf/tests/test_recipe_inputs.py
```

### Comparing `pangeo-forge-esgf-0.1.1/test_script.py` & `pangeo-forge-esgf-0.2.0/test_script.py`

 * *Files identical despite different names*

