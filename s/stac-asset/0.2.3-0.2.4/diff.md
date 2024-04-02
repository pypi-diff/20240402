# Comparing `tmp/stac-asset-0.2.3.tar.gz` & `tmp/stac-asset-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-asset-0.2.3.tar", last modified: Fri Oct 20 12:42:00 2023, max compression
+gzip compressed data, was "stac-asset-0.2.4.tar", last modified: Tue Apr  2 18:37:36 2024, max compression
```

## Comparing `stac-asset-0.2.3.tar` & `stac-asset-0.2.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:42:00.808427 stac-asset-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-20 12:41:46.000000 stac-asset-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-20 12:41:46.000000 stac-asset-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      643 2023-10-20 12:41:46.000000 stac-asset-0.2.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2023-10-20 12:42:00.808427 stac-asset-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2023-10-20 12:41:46.000000 stac-asset-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2023-10-20 12:41:46.000000 stac-asset-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-20 12:42:00.808427 stac-asset-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:42:00.792427 stac-asset-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:42:00.800427 stac-asset-0.2.3/src/stac_asset/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15367 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    18360 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-10-20 12:41:46.000000 stac-asset-0.2.3/src/stac_asset/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:42:00.800427 stac-asset-0.2.3/src/stac_asset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2023-10-20 12:42:00.000000 stac-asset-0.2.3/src/stac_asset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-10-20 12:42:00.000000 stac-asset-0.2.3/src/stac_asset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 12:42:00.000000 stac-asset-0.2.3/src/stac_asset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-10-20 12:42:00.000000 stac-asset-0.2.3/src/stac_asset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-10-20 12:42:00.000000 stac-asset-0.2.3/src/stac_asset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-20 12:42:00.000000 stac-asset-0.2.3/src/stac_asset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:42:00.804427 stac-asset-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-10-20 12:41:46.000000 stac-asset-0.2.3/tests/test_blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2023-10-20 12:41:46.000000 stac-asset-0.2.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-10-20 12:41:46.000000 stac-asset-0.2.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-10-20 12:41:46.000000 stac-asset-0.2.3/tests/test_earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-10-20 12:41:46.000000 stac-asset-0.2.3/tests/test_filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2023-10-20 12:41:46.000000 stac-asset-0.2.3/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-10-20 12:41:46.000000 stac-asset-0.2.3/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-10-20 12:41:46.000000 stac-asset-0.2.3/tests/test_planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2023-10-20 12:41:46.000000 stac-asset-0.2.3/tests/test_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-10-20 12:41:46.000000 stac-asset-0.2.3/tests/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:37:36.578661 stac-asset-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 18:37:27.000000 stac-asset-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 18:37:27.000000 stac-asset-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-02 18:37:27.000000 stac-asset-0.2.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-04-02 18:37:36.578661 stac-asset-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-02 18:37:27.000000 stac-asset-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-02 18:37:27.000000 stac-asset-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:37:36.578661 stac-asset-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:37:36.570661 stac-asset-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:37:36.574661 stac-asset-0.2.4/src/stac_asset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18913 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:37:36.574661 stac-asset-0.2.4/src/stac_asset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-04-02 18:37:36.000000 stac-asset-0.2.4/src/stac_asset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-02 18:37:36.000000 stac-asset-0.2.4/src/stac_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:37:36.000000 stac-asset-0.2.4/src/stac_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 18:37:36.000000 stac-asset-0.2.4/src/stac_asset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-02 18:37:36.000000 stac-asset-0.2.4/src/stac_asset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 18:37:36.000000 stac-asset-0.2.4/src/stac_asset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:37:36.574661 stac-asset-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_validate.py
```

### Comparing `stac-asset-0.2.3/LICENSE` & `stac-asset-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/NOTICE` & `stac-asset-0.2.4/NOTICE`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/PKG-INFO` & `stac-asset-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.2.3
+Version: 0.2.4
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Github, https://github.com/stac-utils/stac-asset
 Project-URL: CHANGELOG, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/stac-utils/stac-asset/issues
 Keywords: stac,async
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: aiofiles>=23.1.0
 Requires-Dist: aiobotocore>=2.5.0
@@ -27,24 +28,23 @@
 Requires-Dist: yarl>=1.9.2
 Provides-Extra: cli
 Requires-Dist: click~=8.1.5; extra == "cli"
 Requires-Dist: click-logging~=1.0.1; extra == "cli"
 Requires-Dist: tabulate~=0.9.0; extra == "cli"
 Requires-Dist: tqdm~=4.66.1; extra == "cli"
 Provides-Extra: dev
-Requires-Dist: black~=23.3; extra == "dev"
 Requires-Dist: mypy~=1.3; extra == "dev"
 Requires-Dist: pre-commit~=3.3; extra == "dev"
 Requires-Dist: pystac[validation]>=1.8.4; extra == "dev"
 Requires-Dist: pytest~=7.3; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.21; extra == "dev"
-Requires-Dist: pytest-cov~=4.1; extra == "dev"
-Requires-Dist: ruff==0.0.292; extra == "dev"
+Requires-Dist: pytest-cov>=5.0; extra == "dev"
+Requires-Dist: ruff==0.3.4; extra == "dev"
 Requires-Dist: types-aiofiles~=23.1; extra == "dev"
-Requires-Dist: types-python-dateutil~=2.8.19; extra == "dev"
+Requires-Dist: types-python-dateutil~=2.9; extra == "dev"
 Requires-Dist: types-tqdm~=4.66.0; extra == "dev"
 Requires-Dist: types-tabulate~=0.9.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
 Requires-Dist: sphinx~=7.2.2; extra == "docs"
 Requires-Dist: sphinx-click~=5.0; extra == "docs"
```

### Comparing `stac-asset-0.2.3/README.md` & `stac-asset-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/pyproject.toml` & `stac-asset-0.2.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "stac-asset"
-version = "0.2.3"
+version = "0.2.4"
 description = "Read and download STAC assets across platforms and providers"
 authors = [{ name = "Pete Gadomski", email = "pete.gadomski@gmail.com" }]
 readme = "README.md"
 keywords = ["stac", "async"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Development Status :: 4 - Beta",
 ]
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 dependencies = [
     "aiofiles>=23.1.0",
     "aiobotocore>=2.5.0",
@@ -29,24 +30,23 @@
 cli = [
     "click~=8.1.5",
     "click-logging~=1.0.1",
     "tabulate~=0.9.0",
     "tqdm~=4.66.1",
 ]
 dev = [
-    "black~=23.3",
     "mypy~=1.3",
     "pre-commit~=3.3",
     "pystac[validation]>=1.8.4",
     "pytest~=7.3",
     "pytest-asyncio~=0.21",
-    "pytest-cov~=4.1",
-    "ruff==0.0.292",
+    "pytest-cov>=5.0",
+    "ruff==0.3.4",
     "types-aiofiles~=23.1",
-    "types-python-dateutil~=2.8.19",
+    "types-python-dateutil~=2.9",
     "types-tqdm~=4.66.0",
     "types-tabulate~=0.9.0",
 ]
 docs = ["pydata-sphinx-theme~=0.13", "sphinx~=7.2.2", "sphinx-click~=5.0"]
 
 [project.scripts]
 stac-asset = "stac_asset._cli:cli"
@@ -66,18 +66,18 @@
     "botocore",
     "botocore.config",
     "click_logging",
 ]
 ignore_missing_imports = true
 
 
-[tool.ruff]
+[tool.ruff.lint]
 select = ["F", "E", "W", "I", "ERA", "RUF", "D"]
 ignore = ["D100", "D105", "D107"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/**/*.py" = ["D"]
 "docs/conf.py" = ["D"]
 "src/stac_asset/_cli.py" = ["D301"]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
```

### Comparing `stac-asset-0.2.3/src/stac_asset/__init__.py` & `stac-asset-0.2.4/src/stac_asset/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 Use :py:class:`Config` to configure how assets are downloaded.  Every client
 inherits from :py:class:`Client`, which defines a common interface for accessing
 assets.  Writing items, item collections, collections, and assets is currently
 unsupported, but is on the roadmap.
 """
 
-
 from ._functions import (
     assert_asset_exists,
     asset_exists,
     download_asset,
     download_collection,
     download_item,
     download_item_collection,
+    open_href,
     read_href,
 )
 from .client import Client
 from .config import Config
 from .earthdata_client import EarthdataClient
 from .errors import (
     AssetOverwriteError,
@@ -59,9 +59,10 @@
     "S3Client",
     "assert_asset_exists",
     "asset_exists",
     "download_asset",
     "download_collection",
     "download_item",
     "download_item_collection",
+    "open_href",
     "read_href",
 ]
```

### Comparing `stac-asset-0.2.3/src/stac_asset/_cli.py` & `stac-asset-0.2.4/src/stac_asset/_cli.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset/_functions.py` & `stac-asset-0.2.4/src/stac_asset/_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os.path
 import warnings
 from asyncio import Queue, Task
 from dataclasses import dataclass
 from pathlib import Path
 from types import TracebackType
 from typing import (
+    AsyncIterator,
     List,
     Optional,
     Set,
     Type,
     Union,
 )
 
@@ -373,14 +374,15 @@
     )
     if href is None:
         raise ValueError(f"asset '{key}' does not have an absolute href: {asset.href}")
     client = await clients.get_client(href)
 
     if messages:
         if asset.owner:
+            assert isinstance(asset.owner, (Item, Collection))
             owner_id = asset.owner.id
         else:
             owner_id = None
         await messages.put(
             StartAssetDownload(key=key, href=href, path=path, owner_id=owner_id)
         )
     try:
@@ -451,39 +453,56 @@
         await assert_asset_exists(asset, config, clients)
     except Exception:
         return False
     else:
         return True
 
 
-async def read_href(
+async def open_href(
     href: str, config: Optional[Config] = None, clients: Optional[List[Client]] = None
-) -> bytes:
-    """Reads an href and returns its bytes.
+) -> AsyncIterator[bytes]:
+    """Opens an href and yields byte chunks.
 
     Args:
         href: The href to read
         config: The download configuration to use
         clients: Any pre-configured clients to use
 
-    Returns:
+    Yields:
         bytes: The bytes from the href
     """
     if config is None:
         config = Config()
     clients_ = Clients(config, clients=clients)
     async with await clients_.get_client(href) as client:
-        data = b""
         async for chunk in client.open_href(href):
-            data += chunk
-        return data
+            yield chunk
+
+
+async def read_href(
+    href: str, config: Optional[Config] = None, clients: Optional[List[Client]] = None
+) -> bytes:
+    """Reads an href and returns its bytes.
+
+    Args:
+        href: The href to read
+        config: The download configuration to use
+        clients: Any pre-configured clients to use
+
+    Returns:
+        bytes: The bytes from the href
+    """
+    data = b""
+    async for chunk in open_href(href, config=config, clients=clients):
+        data += chunk
+    return data
 
 
 def make_asset_hrefs_relative(
-    stac_object: Union[Item, Collection]
+    stac_object: Union[Item, Collection],
 ) -> Union[Item, Collection]:
     # Copied from
     # https://github.com/stac-utils/pystac/blob/381cf89fc25c15142fb5a187d905e22681de42a2/pystac/item.py#L284C5-L298C20
     # until a fix for https://github.com/stac-utils/pystac/issues/1199 is
     # released.
     self_href = stac_object.get_self_href()
     for asset in stac_object.assets.values():
@@ -493,15 +512,15 @@
                     "Cannot make asset HREFs relative " "if no self_href is set."
                 )
             asset.href = pystac.utils.make_relative_href(asset.href, self_href)
     return stac_object
 
 
 def make_asset_hrefs_absolute(
-    stac_object: Union[Item, Collection]
+    stac_object: Union[Item, Collection],
 ) -> Union[Item, Collection]:
     # Copied from
     # https://github.com/stac-utils/pystac/blob/381cf89fc25c15142fb5a187d905e22681de42a2/pystac/item.py#L309C3-L319C1
     # until a fix for https://github.com/stac-utils/pystac/issues/1199 is
     # released.
     self_href = stac_object.get_self_href()
     for asset in stac_object.assets.values():
```

### Comparing `stac-asset-0.2.3/src/stac_asset/blocking.py` & `stac-asset-0.2.4/src/stac_asset/blocking.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset/client.py` & `stac-asset-0.2.4/src/stac_asset/client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset/config.py` & `stac-asset-0.2.4/src/stac_asset/config.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset/earthdata_client.py` & `stac-asset-0.2.4/src/stac_asset/earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset/errors.py` & `stac-asset-0.2.4/src/stac_asset/errors.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset/filesystem_client.py` & `stac-asset-0.2.4/src/stac_asset/filesystem_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset/http_client.py` & `stac-asset-0.2.4/src/stac_asset/http_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset/messages.py` & `stac-asset-0.2.4/src/stac_asset/messages.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset/planetary_computer_client.py` & `stac-asset-0.2.4/src/stac_asset/planetary_computer_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset/s3_client.py` & `stac-asset-0.2.4/src/stac_asset/s3_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset/strategy.py` & `stac-asset-0.2.4/src/stac_asset/strategy.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset/types.py` & `stac-asset-0.2.4/src/stac_asset/types.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset/validate.py` & `stac-asset-0.2.4/src/stac_asset/validate.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/src/stac_asset.egg-info/PKG-INFO` & `stac-asset-0.2.4/src/stac_asset.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.2.3
+Version: 0.2.4
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Github, https://github.com/stac-utils/stac-asset
 Project-URL: CHANGELOG, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/stac-utils/stac-asset/issues
 Keywords: stac,async
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: aiofiles>=23.1.0
 Requires-Dist: aiobotocore>=2.5.0
@@ -27,24 +28,23 @@
 Requires-Dist: yarl>=1.9.2
 Provides-Extra: cli
 Requires-Dist: click~=8.1.5; extra == "cli"
 Requires-Dist: click-logging~=1.0.1; extra == "cli"
 Requires-Dist: tabulate~=0.9.0; extra == "cli"
 Requires-Dist: tqdm~=4.66.1; extra == "cli"
 Provides-Extra: dev
-Requires-Dist: black~=23.3; extra == "dev"
 Requires-Dist: mypy~=1.3; extra == "dev"
 Requires-Dist: pre-commit~=3.3; extra == "dev"
 Requires-Dist: pystac[validation]>=1.8.4; extra == "dev"
 Requires-Dist: pytest~=7.3; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.21; extra == "dev"
-Requires-Dist: pytest-cov~=4.1; extra == "dev"
-Requires-Dist: ruff==0.0.292; extra == "dev"
+Requires-Dist: pytest-cov>=5.0; extra == "dev"
+Requires-Dist: ruff==0.3.4; extra == "dev"
 Requires-Dist: types-aiofiles~=23.1; extra == "dev"
-Requires-Dist: types-python-dateutil~=2.8.19; extra == "dev"
+Requires-Dist: types-python-dateutil~=2.9; extra == "dev"
 Requires-Dist: types-tqdm~=4.66.0; extra == "dev"
 Requires-Dist: types-tabulate~=0.9.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
 Requires-Dist: sphinx~=7.2.2; extra == "docs"
 Requires-Dist: sphinx-click~=5.0; extra == "docs"
```

### Comparing `stac-asset-0.2.3/src/stac_asset.egg-info/SOURCES.txt` & `stac-asset-0.2.4/src/stac_asset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/tests/test_blocking.py` & `stac-asset-0.2.4/tests/test_blocking.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/tests/test_cli.py` & `stac-asset-0.2.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/tests/test_earthdata_client.py` & `stac-asset-0.2.4/tests/test_earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/tests/test_filesystem_client.py` & `stac-asset-0.2.4/tests/test_filesystem_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/tests/test_functions.py` & `stac-asset-0.2.4/tests/test_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,21 @@
 
 async def test_assert_asset_exists(item: Item) -> None:
     await stac_asset.assert_asset_exists(item.assets["data"])
     with pytest.raises(ValueError):
         await stac_asset.assert_asset_exists(Asset(href="not-a-file"))
 
 
+async def test_open_href(data_path: Path) -> None:
+    text = b""
+    async for chunk in stac_asset.open_href(str(data_path / "item.json")):
+        text += chunk
+    Item.from_dict(json.loads(text))
+
+
 async def test_read_href(data_path: Path) -> None:
     text = await stac_asset.read_href(str(data_path / "item.json"))
     Item.from_dict(json.loads(text))
 
 
 async def test_keep_non_downloaded(item: Item, tmp_path: Path) -> None:
     item.assets["other-data"] = item.assets["data"].clone()
```

### Comparing `stac-asset-0.2.3/tests/test_planetary_computer_client.py` & `stac-asset-0.2.4/tests/test_planetary_computer_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/tests/test_s3_client.py` & `stac-asset-0.2.4/tests/test_s3_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.3/tests/test_validate.py` & `stac-asset-0.2.4/tests/test_validate.py`

 * *Files identical despite different names*

