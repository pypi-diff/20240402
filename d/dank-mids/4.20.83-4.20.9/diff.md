# Comparing `tmp/dank_mids-4.20.83.tar.gz` & `tmp/dank_mids-4.20.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dank_mids-4.20.83.tar", last modified: Tue Apr  2 01:18:29 2024, max compression
+gzip compressed data, was "dank_mids-4.20.9.tar", last modified: Wed Oct 19 17:56:40 2022, max compression
```

## Comparing `dank_mids-4.20.83.tar` & `dank_mids-4.20.9.tar`

### file list

```diff
@@ -1,60 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:18:29.070956 dank_mids-4.20.83/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:18:29.058956 dank_mids-4.20.83/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:18:29.062955 dank_mids-4.20.83/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-02 01:18:14.000000 dank_mids-4.20.83/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-02 01:18:14.000000 dank_mids-4.20.83/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-02 01:18:14.000000 dank_mids-4.20.83/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 01:18:14.000000 dank_mids-4.20.83/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 01:18:14.000000 dank_mids-4.20.83/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-02 01:18:29.070956 dank_mids-4.20.83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-02 01:18:14.000000 dank_mids-4.20.83/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:18:29.066955 dank_mids-4.20.83/dank_mids/
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/_demo_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/_envs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:18:29.066955 dank_mids-4.20.83/dank_mids/brownie_patch/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/brownie_patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/brownie_patch/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/brownie_patch/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/brownie_patch/overloaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/brownie_patch/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10597 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:18:29.066955 dank_mids-4.20.83/dank_mids/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/helpers/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/helpers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/helpers/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    39786 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/semaphores.py
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-02 01:18:14.000000 dank_mids-4.20.83/dank_mids/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:18:29.066955 dank_mids-4.20.83/dank_mids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-02 01:18:29.000000 dank_mids-4.20.83/dank_mids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-02 01:18:29.000000 dank_mids-4.20.83/dank_mids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:18:29.000000 dank_mids-4.20.83/dank_mids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-02 01:18:29.000000 dank_mids-4.20.83/dank_mids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 01:18:29.000000 dank_mids-4.20.83/dank_mids.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:18:29.066955 dank_mids-4.20.83/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-02 01:18:14.000000 dank_mids-4.20.83/examples/dank_brownie_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 01:18:14.000000 dank_mids-4.20.83/license
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 01:18:14.000000 dank_mids-4.20.83/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 01:18:14.000000 dank_mids-4.20.83/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-02 01:18:14.000000 dank_mids-4.20.83/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 01:18:29.070956 dank_mids-4.20.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-02 01:18:14.000000 dank_mids-4.20.83/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:18:29.066955 dank_mids-4.20.83/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:18:14.000000 dank_mids-4.20.83/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 01:18:14.000000 dank_mids-4.20.83/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-02 01:18:14.000000 dank_mids-4.20.83/tests/test_brownie_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-02 01:18:14.000000 dank_mids-4.20.83/tests/test_dank_mids.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.676519 dank_mids-4.20.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.676519 dank_mids-4.20.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-10-19 17:56:26.000000 dank_mids-4.20.9/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-10-19 17:56:26.000000 dank_mids-4.20.9/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2022-10-19 17:56:26.000000 dank_mids-4.20.9/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-19 17:56:26.000000 dank_mids-4.20.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-19 17:56:40.680519 dank_mids-4.20.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-10-19 17:56:26.000000 dank_mids-4.20.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/dank_mids/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/_demo_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/dank_mids/brownie_patch/
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/brownie_patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/brownie_patch/call.py
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/brownie_patch/contract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/brownie_patch/overloaded.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4784 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/call.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)      793 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/uid.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11199 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/dank_mids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-19 17:56:26.000000 dank_mids-4.20.9/license
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-19 17:56:26.000000 dank_mids-4.20.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-19 17:56:26.000000 dank_mids-4.20.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-19 17:56:26.000000 dank_mids-4.20.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-19 17:56:40.680519 dank_mids-4.20.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2022-10-19 17:56:26.000000 dank_mids-4.20.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/test_brownie_patch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2310 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/test_dank_mids.py
```

### Comparing `dank_mids-4.20.83/.github/workflows/mypy.yaml` & `dank_mids-4.20.9/.github/workflows/mypy.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
     - name: Install MyPy
       run: |
         python -m pip install --upgrade pip
         pip install mypy types-requests
 
     - name: Run MyPy
-      run: mypy ./dank_mids --pretty --ignore-missing-imports --show-error-codes --show-error-context --no-warn-no-return
+      run: mypy ./dank_mids --pretty --ignore-missing-imports --show-error-codes --show-error-context
```

### Comparing `dank_mids-4.20.83/.github/workflows/pytest.yaml` & `dank_mids-4.20.9/.github/workflows/pytest.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -7,20 +7,18 @@
     paths:
       - '**.py'
       - '**/pytest.yaml'
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
+    #timeout-minutes: 10
     strategy:
-      fail-fast: false
       matrix:
         os: [ ubuntu-latest, macos-latest, windows-latest ]
-        pyversion: [ "3.8", "3.9", "3.10" ]
-        provider: [ "WEB3_PROVIDER", "LLAMA_ETH_RPC", "INFURA_PROVIDER", "ALCHEMY_PROVIDER" ]
         include:
         - os: ubuntu-latest
           path: ~/.cache/pip
         - os: macos-latest
           path: ~/Library/Caches/pip
         - os: windows-latest
           path: ~\AppData\Local\pip\Cache
@@ -28,24 +26,24 @@
     steps:
       - name: Check out repository code
         uses: actions/checkout@v2
 
       - name: Setup Python (faster than using Python container)
         uses: actions/setup-python@v2
         with:
-          python-version: ${{ matrix.pyversion }}
+          python-version: "3.9"
 
       - name: Install dependencies
         run: |
           pip install -r requirements.txt -r requirements-dev.txt
       
       - name: Setup brownie networks
         run: |
-          brownie networks modify mainnet host=${{ secrets[matrix.provider] }}
+          brownie networks modify mainnet host=${{ secrets.WEB3_PROVIDER }}
         continue-on-error: true
 
       - name: Run test suite
         env:
           PYTEST_NETWORK: mainnet
           ETHERSCAN_TOKEN: ${{ secrets.ETHERSCAN_TOKEN  }}
         run: pytest
-      
+
```

### Comparing `dank_mids-4.20.83/.github/workflows/release.yaml` & `dank_mids-4.20.9/.github/workflows/release.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 on:
   push:
     branches:
       - dev
   release:
     branches:
       - master
-    types: [published]
 
 jobs:
   deploy:
     runs-on: ubuntu-20.04
 
     steps:
     - uses: actions/checkout@v2
```

### Comparing `dank_mids-4.20.83/dank_mids/brownie_patch/overloaded.py` & `dank_mids-4.20.9/dank_mids/brownie_patch/overloaded.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,31 @@
 import functools
 from types import MethodType
-from typing import Any, Dict, Optional, Tuple, Union
+from typing import Any, Coroutine, Dict, Optional, Tuple, Union
 
 from brownie import Contract
 from brownie.network.contract import ContractCall, ContractTx, OverloadedMethod
-from dank_mids.brownie_patch.call import _get_coroutine_fn, _skip_proc_pool
-from dank_mids.brownie_patch.types import ContractMethod
+from dank_mids.brownie_patch.call import _patch_call
 from web3 import Web3
 
 
 def _patch_overloaded_method(call: OverloadedMethod, w3: Web3) -> None:
-    # sourcery skip: avoid-builtin-shadow
     @functools.wraps(call)
     async def coroutine(
         self: Contract,
         *args: Tuple[Any,...],
         block_identifier: Optional[Union[int, str, bytes]] = None,
-        decimals: Optional[int] = None,
-        override: Optional[Dict[str, str]] = None,
+        override: Optional[Dict[str, str]] = None
     ) -> Any:
-        try:
-            fn = self._get_fn_from_args(args)
-        except ValueError as e:
-            if f"Contract has more than one function '.{call._name}" in str(e) and f"You must explicitly declare which function you are calling, e.g. .{call._name}" in str(e):
-                exc_str = str(e)
-                breakpoint = exc_str.find("(*args)")
-                raise ValueError(f"{exc_str[:breakpoint]}.coroutine{exc_str[breakpoint:]}")
-            raise e
-
-        kwargs = {"block_identifier": block_identifier, "decimals": decimals, "override": override}
+        fn = self._get_fn_from_args(args)
+        kwargs = {"block_identifier": block_identifier, "override": override}
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
         return await fn.coroutine(*args, **kwargs)
 
-    for method in call.__dict__['methods'].values():
-        if isinstance(method, (ContractCall, ContractTx)):
-            method._skip_decoder_proc_pool = method._address in _skip_proc_pool
-            method.coroutine = MethodType(_get_coroutine_fn(w3, len(method.abi['inputs'])), method)
+    for args, method in call.__dict__['methods'].items():
+        if isinstance(method, ContractCall) or isinstance(method, ContractTx):
+            _patch_call(method, w3)
     # TODO implement this properly
         #elif isinstance(call, ContractTx):
             #_patch_tx(call, w3)
-
+    
     call.coroutine = MethodType(coroutine, call)
```

### Comparing `dank_mids-4.20.83/dank_mids.egg-info/SOURCES.txt` & `dank_mids-4.20.9/dank_mids.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,38 @@
 .gitignore
-Makefile
 README.md
 license
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/mypy.yaml
 .github/workflows/pytest.yaml
 .github/workflows/release.yaml
-dank_mids/ENVIRONMENT_VARIABLES.py
 dank_mids/__init__.py
+dank_mids/_config.py
 dank_mids/_demo_mode.py
-dank_mids/_envs.py
-dank_mids/_exceptions.py
-dank_mids/_mode.py
-dank_mids/batch.py
+dank_mids/call.py
 dank_mids/constants.py
 dank_mids/controller.py
-dank_mids/exceptions.py
-dank_mids/executor.py
+dank_mids/helpers.py
+dank_mids/loggers.py
 dank_mids/middleware.py
 dank_mids/py.typed
-dank_mids/requests.py
-dank_mids/semaphore.py
-dank_mids/semaphores.py
-dank_mids/stats.py
 dank_mids/types.py
 dank_mids/uid.py
+dank_mids/worker.py
 dank_mids.egg-info/PKG-INFO
 dank_mids.egg-info/SOURCES.txt
 dank_mids.egg-info/dependency_links.txt
 dank_mids.egg-info/requires.txt
 dank_mids.egg-info/top_level.txt
 dank_mids/brownie_patch/__init__.py
 dank_mids/brownie_patch/call.py
 dank_mids/brownie_patch/contract.py
 dank_mids/brownie_patch/overloaded.py
-dank_mids/brownie_patch/types.py
-dank_mids/helpers/__init__.py
-dank_mids/helpers/decode.py
-dank_mids/helpers/helpers.py
-dank_mids/helpers/session.py
-examples/dank_brownie_example.py
 tests/__init__.py
 tests/conftest.py
+tests/fixtures.py
 tests/test_brownie_patch.py
 tests/test_dank_mids.py
```

### Comparing `dank_mids-4.20.83/license` & `dank_mids-4.20.9/license`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.83/setup.py` & `dank_mids-4.20.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # type: ignore
 
 from setuptools import find_packages, setup
 
-with open("requirements.txt", "r") as f:
-    requirements = list(map(str.strip, f.read().split("\n")))[:-1]
-
 setup(
     name='dank_mids',
     packages=find_packages(),
     use_scm_version={
         "root": ".",
         "relative_to": __file__,
         "local_scheme": "no-local-version",
         "version_scheme": "python-simplified-semver",
     },
     description='Multicall batching middleware for asynchronous scripts using web3.py',
     author='BobTheBuidler',
     author_email='bobthebuidlerdefi@gmail.com',
     url='https://github.com/BobTheBuidler/dank_mids',
     license='MIT',
-    install_requires=requirements,
+    install_requires=[
+        "bobs_lazy_logging>=0.0.4",
+        "eth_retry>=0.1.12",
+        "multicall>=0.6.2",
+    ],
     setup_requires=[
         'setuptools_scm',
     ],
     package_data={
         "dank_mids": ["py.typed"],
     },
 )
```

### Comparing `dank_mids-4.20.83/tests/test_brownie_patch.py` & `dank_mids-4.20.9/tests/test_brownie_patch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,30 @@
-# sourcery skip: no-loop-in-tests
-import asyncio
 
-from brownie import Contract, web3
-from decimal import Decimal
+from brownie import Contract
+from dank_mids.brownie_patch import patch_contract
+from dank_mids.brownie_patch.call import _patch_call
 from multicall.utils import await_awaitable
 
-from dank_mids import dank_web3, patch_contract, setup_dank_w3_from_sync
-from dank_mids.brownie_patch.call import _patch_call
+from tests.fixtures import dank_w3
 
 
 def test_patch_call():
     # must use from_explorer for gh testing workflow
     weth = Contract.from_explorer('0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2')
-    _patch_call(weth.totalSupply, dank_web3)
+    _patch_call(weth.totalSupply, dank_w3)
     assert hasattr(weth.totalSupply, 'coroutine')
     assert await_awaitable(weth.totalSupply.coroutine(block_identifier=13_000_000)) == 6620041514474872981393155
 
-def test_gather():
-    # must use from_explorer for gh testing workflow
-    weth = Contract.from_explorer('0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2')
-    _patch_call(weth.totalSupply, dank_web3)
-    assert hasattr(weth.totalSupply, 'coroutine')
-    for result in await_awaitable(asyncio.gather(*[weth.totalSupply.coroutine(block_identifier=13_000_000) for _ in range(10_000)])):
-        assert result == 6620041514474872981393155
-    
 def test_patch_contract():
     # ContractCall
     # must use from_explorer for gh testing workflow
-    # specify w3
-    weth = patch_contract(Contract.from_explorer('0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2'), dank_web3)
+    weth = patch_contract(Contract.from_explorer('0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2'), dank_w3)
     assert hasattr(weth.totalSupply, 'coroutine')
     assert await_awaitable(weth.totalSupply.coroutine(block_identifier=13_000_000)) == 6620041514474872981393155
-    assert await_awaitable(weth.totalSupply.coroutine(block_identifier=13_000_000, decimals=18)) == Decimal(6620041.514474872981393155)
-    assert await_awaitable(weth.totalSupply)
 
     # ContractTx
     # must use from_explorer for gh testing workflow
-    # dont specify w3
-    uni_v3_quoter = patch_contract(Contract.from_explorer('0xb27308f9F90D607463bb33eA1BeBb41C27CE5AB6'))
+    uni_v3_quoter = patch_contract(Contract.from_explorer('0xb27308f9F90D607463bb33eA1BeBb41C27CE5AB6'), dank_w3)
     assert hasattr(uni_v3_quoter.quoteExactInput, 'coroutine')
     assert await_awaitable(
         uni_v3_quoter.quoteExactInput.coroutine(b"\xc0*\xaa9\xb2#\xfe\x8d\n\x0e\\O'\xea\xd9\x08<ul\xc2\x00\x01\xf4\xa0\xb8i\x91\xc6!\x8b6\xc1\xd1\x9dJ.\x9e\xb0\xce6\x06\xebH", 1e18, block_identifier=13_000_000)
     ) == 3169438072
-    assert await_awaitable(
-        uni_v3_quoter.quoteExactInput.coroutine(b"\xc0*\xaa9\xb2#\xfe\x8d\n\x0e\\O'\xea\xd9\x08<ul\xc2\x00\x01\xf4\xa0\xb8i\x91\xc6!\x8b6\xc1\xd1\x9dJ.\x9e\xb0\xce6\x06\xebH", 1e18, block_identifier=13_000_000, decimals=8)
-    ) == Decimal(31.69438072)
-
-def test_call_setup_twice_on_same_web3():
-    w3_a = setup_dank_w3_from_sync(web3)
-    w3_a.test = True
-    w3_b = setup_dank_w3_from_sync(web3)
-    assert hasattr(w3_b, 'test')
-
```

