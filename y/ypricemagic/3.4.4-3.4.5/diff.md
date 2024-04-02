# Comparing `tmp/ypricemagic-3.4.4.tar.gz` & `tmp/ypricemagic-3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-3.4.4.tar", last modified: Sun Mar 31 07:02:51 2024, max compression
+gzip compressed data, was "ypricemagic-3.4.5.tar", last modified: Tue Apr  2 08:01:15 2024, max compression
```

## Comparing `ypricemagic-3.4.4.tar` & `ypricemagic-3.4.5.tar`

### file list

```diff
@@ -1,205 +1,205 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.783913 ypricemagic-3.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.755912 ypricemagic-3.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.759912 ypricemagic-3.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/.github/workflows/deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-31 07:02:51.783913 ypricemagic-3.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.763913 ypricemagic-3.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.755912 ypricemagic-3.4.4/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.755912 ypricemagic-3.4.4/docs/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.763913 ypricemagic-3.4.4/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/_build/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.763913 ypricemagic-3.4.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/scripts/debug-curve.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/scripts/debug-price.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-31 07:02:51.783913 ypricemagic-3.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.763913 ypricemagic-3.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.763913 ypricemagic-3.4.4/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.767912 ypricemagic-3.4.4/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.767912 ypricemagic-3.4.4/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/dex/test_uniswap.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/dex/test_velodrome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.767912 ypricemagic-3.4.4/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.767912 ypricemagic-3.4.4/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.767912 ypricemagic-3.4.4/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.767912 ypricemagic-3.4.4/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.767912 ypricemagic-3.4.4/y/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.771912 ypricemagic-3.4.4/y/_db/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14129 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.771912 ypricemagic-3.4.4/y/_db/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/utils/_ep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/utils/bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/utils/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/utils/price.py
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/utils/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/utils/traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/_db/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.771912 ypricemagic-3.4.4/y/classes/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24370 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.771912 ypricemagic-3.4.4/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.771912 ypricemagic-3.4.4/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (127)    23102 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.771912 ypricemagic-3.4.4/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32517 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.775912 ypricemagic-3.4.4/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.775912 ypricemagic-3.4.4/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/interfaces/uniswap/velov2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.775912 ypricemagic-3.4.4/y/prices/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (127)    20384 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.775912 ypricemagic-3.4.4/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.779913 ypricemagic-3.4.4/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13900 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/mooniswap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/solidly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.779913 ypricemagic-3.4.4/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    28621 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/uniswap/v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/dex/velodrome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.779913 ypricemagic-3.4.4/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.779913 ypricemagic-3.4.4/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14526 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/popsicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/rkp3r.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/solidex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.779913 ypricemagic-3.4.4/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24089 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.779913 ypricemagic-3.4.4/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.783913 ypricemagic-3.4.4/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.783913 ypricemagic-3.4.4/y/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/utils/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.783913 ypricemagic-3.4.4/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-31 07:02:42.000000 ypricemagic-3.4.4/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:02:51.783913 ypricemagic-3.4.4/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-31 07:02:51.000000 ypricemagic-3.4.4/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-03-31 07:02:51.000000 ypricemagic-3.4.4/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 07:02:51.000000 ypricemagic-3.4.4/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-31 07:02:51.000000 ypricemagic-3.4.4/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-31 07:02:51.000000 ypricemagic-3.4.4/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.417708 ypricemagic-3.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.385708 ypricemagic-3.4.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.393709 ypricemagic-3.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-02 08:01:15.417708 ypricemagic-3.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.393709 ypricemagic-3.4.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.385708 ypricemagic-3.4.5/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.385708 ypricemagic-3.4.5/docs/_build/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.393709 ypricemagic-3.4.5/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/scripts/debug-curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/scripts/debug-price.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 08:01:15.417708 ypricemagic-3.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/dex/test_uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/dex/test_velodrome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.397709 ypricemagic-3.4.5/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.401708 ypricemagic-3.4.5/y/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.401708 ypricemagic-3.4.5/y/_db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/_db/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/_ep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/_db/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24529 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (127)    23102 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32517 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.405708 ypricemagic-3.4.5/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/interfaces/uniswap/velov2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.409709 ypricemagic-3.4.5/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20384 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.409709 ypricemagic-3.4.5/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.409709 ypricemagic-3.4.5/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13900 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/mooniswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/solidly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.409709 ypricemagic-3.4.5/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31130 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/uniswap/v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/dex/velodrome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.409709 ypricemagic-3.4.5/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.413709 ypricemagic-3.4.5/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14526 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/rkp3r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/solidex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.413709 ypricemagic-3.4.5/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24089 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.413709 ypricemagic-3.4.5/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.413709 ypricemagic-3.4.5/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.417708 ypricemagic-3.4.5/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.417708 ypricemagic-3.4.5/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-02 08:01:06.000000 ypricemagic-3.4.5/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:01:15.417708 ypricemagic-3.4.5/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-02 08:01:15.000000 ypricemagic-3.4.5/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-02 08:01:15.000000 ypricemagic-3.4.5/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:01:15.000000 ypricemagic-3.4.5/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 08:01:15.000000 ypricemagic-3.4.5/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 08:01:15.000000 ypricemagic-3.4.5/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-3.4.4/.github/workflows/codeql-analysis.yml` & `ypricemagic-3.4.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/.github/workflows/deploy-docs.yml` & `ypricemagic-3.4.5/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/.github/workflows/pytest.yaml` & `ypricemagic-3.4.5/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/.github/workflows/release.yaml` & `ypricemagic-3.4.5/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/CONTRIBUTING.md` & `ypricemagic-3.4.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/LICENSE.txt` & `ypricemagic-3.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/Makefile` & `ypricemagic-3.4.5/Makefile`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/README.md` & `ypricemagic-3.4.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from y import get_prices
 get_prices(tokens, block)
 ```
 
 You can also use ypricemagic asynchronously
 ```
 get_price(token, block, sync=False)
-
+```
 You can also import protocol specific modules. For example:
 ```
 from ypricemagic import uniswap
 uniswap.get_price(token, block)
 ```
 ```
 from ypricemagic.compound import get_price
```

### Comparing `ypricemagic-3.4.4/docs/Makefile` & `ypricemagic-3.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/docs/_build/html/_static/alabaster.css` & `ypricemagic-3.4.5/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/docs/_build/html/_static/basic.css` & `ypricemagic-3.4.5/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/docs/_build/html/_static/doctools.js` & `ypricemagic-3.4.5/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/docs/_build/html/_static/language_data.js` & `ypricemagic-3.4.5/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/docs/_build/html/_static/pygments.css` & `ypricemagic-3.4.5/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/docs/_build/html/_static/searchtools.js` & `ypricemagic-3.4.5/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/docs/_build/html/_static/sphinx_highlight.js` & `ypricemagic-3.4.5/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/docs/conf.py` & `ypricemagic-3.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/docs/make.bat` & `ypricemagic-3.4.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/scripts/debug-curve.py` & `ypricemagic-3.4.5/scripts/debug-curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/scripts/debug-price.py` & `ypricemagic-3.4.5/scripts/debug-price.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/setup.py` & `ypricemagic-3.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/tests/classes/test_erc20.py` & `ypricemagic-3.4.5/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/tests/classes/test_singleton.py` & `ypricemagic-3.4.5/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/tests/fixtures.py` & `ypricemagic-3.4.5/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/tests/prices/dex/test_balancer.py` & `ypricemagic-3.4.5/tests/prices/dex/test_balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/tests/prices/dex/test_uniswap.py` & `ypricemagic-3.4.5/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/tests/prices/lending/test_aave.py` & `ypricemagic-3.4.5/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/tests/prices/lending/test_compound.py` & `ypricemagic-3.4.5/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/tests/prices/test_chainlink.py` & `ypricemagic-3.4.5/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/tests/prices/test_magic.py` & `ypricemagic-3.4.5/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/tests/prices/test_popsicle.py` & `ypricemagic-3.4.5/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/tests/prices/test_synthetix.py` & `ypricemagic-3.4.5/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/tests/prices/test_yearn.py` & `ypricemagic-3.4.5/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/tests/prices/utils/test_buckets.py` & `ypricemagic-3.4.5/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/ENVIRONMENT_VARIABLES.py` & `ypricemagic-3.4.5/y/ENVIRONMENT_VARIABLES.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/__init__.py` & `ypricemagic-3.4.5/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/__init__.py` & `ypricemagic-3.4.5/y/_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/common.py` & `ypricemagic-3.4.5/y/_db/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             logger.debug('%s loaded %s objects thru block %s from disk', self, len(self._objects), cached_thru)
             return cached_thru
         return None
 
 _E = TypeVar("_E", bound=_AsyncExecutorMixin)
     
 class Filter(_DiskCachedMixin[T, C]):
-    __slots__ = 'from_block', 'to_block', '_chunk_size', '_chunks_per_batch', '_db_task', '_exc', '_interval', '_lock', '_semaphore', '_sleep_fut', '_sleep_time', '_task', '_verbose'
+    __slots__ = 'from_block', 'to_block', '_chunk_size', '_chunks_per_batch', '_db_task', '_exc', '_interval', '_lock', '_semaphore', '_sleep_fut', '_sleep_time', '_task', '_verbose', '__dict__'
     def __init__(
         self, 
         from_block: int,
         *, 
         chunk_size: int = BATCH_SIZE, 
         chunks_per_batch: Optional[int] = None,
         sleep_time: int = 60,
@@ -187,14 +187,15 @@
     def is_asleep(self) -> bool:
         return not self._sleep_fut.done() if self._sleep_fut else False
     
     def _get_block_for_obj(self, obj: T) -> int:
         """Override this as needed for different object types"""
         return obj['blockNumber']
     
+    @a_sync.ASyncIterator.wrap
     async def _objects_thru(self, block: Optional[int]) -> AsyncIterator[T]:
         self._ensure_task()
         yielded = 0
         done_thru = 0
         while True:
             if block is None or done_thru < block:
                 if self.is_asleep:
```

### Comparing `ypricemagic-3.4.4/y/_db/config.py` & `ypricemagic-3.4.5/y/_db/config.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/decorators.py` & `ypricemagic-3.4.5/y/_db/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/entities.py` & `ypricemagic-3.4.5/y/_db/entities.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/exceptions.py` & `ypricemagic-3.4.5/y/_db/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/structs.py` & `ypricemagic-3.4.5/y/_db/structs.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/utils/_ep.py` & `ypricemagic-3.4.5/y/_db/utils/_ep.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/utils/bulk.py` & `ypricemagic-3.4.5/y/_db/utils/bulk.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/utils/contract.py` & `ypricemagic-3.4.5/y/_db/utils/contract.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/utils/logs.py` & `ypricemagic-3.4.5/y/_db/utils/logs.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/utils/price.py` & `ypricemagic-3.4.5/y/_db/utils/price.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/utils/token.py` & `ypricemagic-3.4.5/y/_db/utils/token.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/utils/traces.py` & `ypricemagic-3.4.5/y/_db/utils/traces.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/_db/utils/utils.py` & `ypricemagic-3.4.5/y/_db/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/classes/common.py` & `ypricemagic-3.4.5/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/classes/singleton.py` & `ypricemagic-3.4.5/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/constants.py` & `ypricemagic-3.4.5/y/constants.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/contracts.py` & `ypricemagic-3.4.5/y/contracts.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,14 +181,18 @@
         return hi
     raise ValueError(f"Unable to find deploy block for {address} on {Network.name()}")
 
 
 # this defaultdict prevents congestion in the contracts thread pool
 address_semaphores = defaultdict(lambda: a_sync.ThreadsafeSemaphore(1))
 
+class ContractEvents(ContractEvents):
+    def __getattr__(self, name: str) -> Events:
+        return super().__getattr__(name)
+    
 class Contract(dank_mids.Contract, metaclass=ChecksumAddressSingletonMeta):
     """
     Though it may look complicated, a ypricemagic Contract object is simply a brownie Contract object with a few modifications:
     1. Contracts will not be compiled. This allows you to more quickly fetch contracts from the block explorer and prevents you from having to download and install compilers.
     2. To each contract method, a `coroutine` property has been defined which allows you to make asynchronous calls using the following syntax:
     ```Contract(0xAddress).methodName.coroutine(*args, block_identifier = 123)```
     3. A few attributes were removed in order to minimize the size of a Contract object in memory: 
@@ -197,14 +201,15 @@
         - has_method
         - has_methods
         - has_methods_async
         - build_name
         - build_name_async
         - get_code
     """
+    events: ContractEvents
     _ChecksumAddressSingletonMeta__instances: ChecksumAddressDict["Contract"]
 
     @eth_retry.auto_retry
     def __init__(
         self, 
         address: AnyAddressType, 
         owner: Optional[AccountsType] = None,
```

### Comparing `ypricemagic-3.4.4/y/datatypes.py` & `ypricemagic-3.4.5/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/decorators.py` & `ypricemagic-3.4.5/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/erc20.py` & `ypricemagic-3.4.5/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/exceptions.py` & `ypricemagic-3.4.5/y/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/interfaces/ERC20.py` & `ypricemagic-3.4.5/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-3.4.5/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/interfaces/compound/unitroller.py` & `ypricemagic-3.4.5/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-3.4.5/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/interfaces/multicall2.py` & `ypricemagic-3.4.5/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-3.4.5/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-3.4.5/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/interfaces/uniswap/velov2.py` & `ypricemagic-3.4.5/y/interfaces/uniswap/velov2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/networks.py` & `ypricemagic-3.4.5/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/band.py` & `ypricemagic-3.4.5/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/chainlink.py` & `ypricemagic-3.4.5/y/prices/chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/convex.py` & `ypricemagic-3.4.5/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/dex/balancer/balancer.py` & `ypricemagic-3.4.5/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/dex/balancer/v1.py` & `ypricemagic-3.4.5/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/dex/balancer/v2.py` & `ypricemagic-3.4.5/y/prices/dex/balancer/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/dex/genericamm.py` & `ypricemagic-3.4.5/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/dex/mooniswap.py` & `ypricemagic-3.4.5/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/dex/solidly.py` & `ypricemagic-3.4.5/y/prices/dex/solidly.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-3.4.5/y/prices/dex/uniswap/uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/dex/uniswap/v1.py` & `ypricemagic-3.4.5/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/dex/uniswap/v2.py` & `ypricemagic-3.4.5/y/prices/dex/uniswap/v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import a_sync
 import brownie
 import dank_mids
 from a_sync.property import HiddenMethodDescriptor
 from brownie import chain
 from brownie.network.event import _EventItem
+from dank_mids.exceptions import Revert
 from multicall import Call
 from typing_extensions import Self
 from web3.exceptions import ContractLogicError
 
 from y import ENVIRONMENT_VARIABLES as ENVS
 from y import convert
 from y.classes.common import ERC20, ContractBase, WeiBalance
@@ -379,20 +380,38 @@
         tokens = set(await asyncio.gather(*itertools.chain(*((pool.__token0__, pool.__token1__) for pool in pools))))
         logger.info('Loaded %s pools supporting %s tokens on %s', len(pools), len(tokens), self.label)
         return pools
     __pools__: HiddenMethodDescriptor[Self, List[UniswapV2Pool]]
 
     @stuck_coro_debugger
     @a_sync.a_sync(ram_cache_maxsize=None, ram_cache_ttl=60*60)
-    async def get_pools_for(self, token_in: Address) -> Dict[UniswapV2Pool, Address]:
+    async def get_pools_for(self, token_in: Address, block: Optional[Block] = None) -> Dict[UniswapV2Pool, Address]:
         if self._supports_uniswap_helper:
-            pools = [
-                UniswapV2Pool(pool, asynchronous=self.asynchronous)
-                for pool in await FACTORY_HELPER.getPairsFor.coroutine(self.factory, token_in)
-            ]
+            try:
+                pools = [
+                    UniswapV2Pool(pool, asynchronous=self.asynchronous)
+                    for pool in await FACTORY_HELPER.getPairsFor.coroutine(self.factory, token_in, block_identifier=block)
+                ]
+            except Exception as e:
+                if block is None:
+                    raise e
+                if not call_reverted(e) and "out of gas" not in str(e) and "timeout" not in str(e):
+                    raise e
+                pool_to_token_out = {}
+                async for pool, (token0, token1) in a_sync.map(_get_tokens, await self.__pools__):
+                    if token_in == token0:
+                        pool_to_token_out[pool] = token1
+                    elif token_in == token1:
+                        pool_to_token_out[pool] = token0
+                if not pool_to_token_out:
+                    logger.debug("no data returned and 0 pools when checking the long way!")
+                else:
+                    logger.debug("no data returned but we have pools when checking the long way...")
+                return pool_to_token_out
+
         else:
             pools = await self.__pools__
         pool_to_token_out = {}
         async for pool, (token0, token1) in a_sync.map(_get_tokens, pools):
             if token_in == token0:
                 pool_to_token_out[pool] = token1
             elif token_in == token1:
@@ -403,44 +422,63 @@
     async def pools_for_token(self, token_address: Address, block: Optional[Block] = None, _ignore_pools: Tuple[UniswapV2Pool,...] = ()) -> Dict[UniswapV2Pool, Address]:
         pools: Dict[UniswapV2Pool, Address]
         
         if chain.id == Network.Mainnet and token_address == WRAPPED_GAS_COIN and self.label == "uniswap v2":
             # This will run out of gas if we use the helper so we bypass it with a known liquid pool
             pools = {UniswapV2Pool("0xB4e16d0168e52d35CaCD2c6185b44281Ec28C9Dc", asynchronous=True): "0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48"}
         else:
-            pools = await self.get_pools_for(token_address, sync=False)
+            try:
+                pools = await self.get_pools_for(token_address, sync=False)
+            except Exception as e:
+                if 'out of gas' not in str(e) and not call_reverted(e):
+                    e.args = (*e.args, self, token_address, block)
+                    raise e
+                try:
+                    # if it fails with no block we will try once with a block before we fetch the long way
+                    pools = await self.get_pools_for(token_address, block=block, sync=False)
+                except Exception as e:
+                    e.args = (*e.args, self, token_address, block)
+                    raise e
         pools = {k: v for k, v in pools.items() if k not in _ignore_pools}
         if pools and block is not None:
             deploy_blocks = await asyncio.gather(*[pool.deploy_block(when_no_history_return_0=True, sync=False) for pool in pools])
             pools = {k: v for (k, v), deploy_block in zip(pools.items(), deploy_blocks) if deploy_block <= block}
         return pools
 
     @stuck_coro_debugger
     @a_sync.a_sync(ram_cache_maxsize=500)
     async def deepest_pool(self, token_address: AnyAddressType, block: Optional[Block] = None, _ignore_pools: Tuple[UniswapV2Pool,...] = ()) -> Optional[UniswapV2Pool]:
         """returns the deepest pool for `token_address` at `block`, excluding pools in `_ignore_pools`"""
         token_address = convert.to_address(token_address)
         if token_address == WRAPPED_GAS_COIN or token_address in STABLECOINS:
             return await self.deepest_stable_pool(token_address, block, sync=False)
         if self._supports_uniswap_helper and (block is None or block >= await contract_creation_block_async(FACTORY_HELPER)):
-            deepest_pool, deepest_pool_depth = await self.deepest_pool_for(token_address, block, ignore_pools=_ignore_pools)
-            return None if deepest_pool == brownie.ZERO_ADDRESS else UniswapV2Pool(deepest_pool, asynchronous=self.asynchronous)
-        else:
-            pools: List[UniswapV2Pool] = list((await self.pools_for_token(token_address, block, _ignore_pools=_ignore_pools, sync=False)).keys())
-            if not pools:
-                return None
-            liquidity = await asyncio.gather(*[pool.check_liquidity(token_address, block, sync=False) for pool in pools])
+            try:
+                deepest_pool, deepest_pool_depth = await self.deepest_pool_for(token_address, block, ignore_pools=_ignore_pools)
+                return None if deepest_pool == brownie.ZERO_ADDRESS else UniswapV2Pool(deepest_pool, asynchronous=self.asynchronous)
+            except Revert as e:
+                # TODO: debug me!
+                logger.debug('helper reverted for %s at block %s ignore_pools %s: %s', token_address, block, _ignore_pools, e)
+            except ValueError as e:
+                if "out of gas" not in str(e):
+                    raise e
+                logger.debug('helper out of gas for %s at block %s ignore_pools %s: %s', token_address, block, _ignore_pools, e)
+
+        pools: List[UniswapV2Pool] = list((await self.pools_for_token(token_address, block, _ignore_pools=_ignore_pools, sync=False)).keys())
+        if not pools:
+            return None
+        liquidity = await asyncio.gather(*[pool.check_liquidity(token_address, block, sync=False) for pool in pools])
 
-            deepest_pool = None
-            deepest_pool_balance = 0
-            for pool, depth in zip(pools, liquidity):
-                if depth and depth > deepest_pool_balance:
-                    deepest_pool = pool
-                    deepest_pool_balance = depth
-            return deepest_pool
+        deepest_pool = None
+        deepest_pool_balance = 0
+        for pool, depth in zip(pools, liquidity):
+            if depth and depth > deepest_pool_balance:
+                deepest_pool = pool
+                deepest_pool_balance = depth
+        return deepest_pool
 
     @stuck_coro_debugger
     @a_sync.a_sync(ram_cache_maxsize=500)
     async def deepest_stable_pool(self, token_address: AnyAddressType, block: Optional[Block] = None, _ignore_pools: Tuple[UniswapV2Pool,...] = ()) -> Optional[UniswapV2Pool]:
         """returns the deepest pool for `token_address` at `block` which has `token_address` paired with a stablecoin, excluding pools in `_ignore_pools`"""
         token_address = convert.to_address(token_address)
         stable_pools: Dict[UniswapV2Pool, Address] = {
@@ -512,28 +550,38 @@
     @a_sync.a_sync(ram_cache_maxsize=100_000, ram_cache_ttl=60*60)
     async def check_liquidity(self, token: Address, block: Block, ignore_pools = []) -> int:
         logger.debug("checking %s liquidity for %s at %s", self, token, block)
         if block and block < await contract_creation_block_async(self.factory):
             logger.debug("block %s is before %s deploy block")
             return 0
         if self._supports_uniswap_helper and (block is None or block >= await contract_creation_block_async(FACTORY_HELPER)):
-            deepest_pool, liquidity = await self.deepest_pool_for(token, block, ignore_pools=ignore_pools)
-        else:
-            pools: Dict[UniswapV2Pool, Address] = await self.pools_for_token(token, block=block, _ignore_pools=ignore_pools, sync=False)
-            liquidity = max(await asyncio.gather(*[pool.check_liquidity(token, block) for pool in pools])) if pools else 0
+            try:
+                deepest_pool, liquidity = await self.deepest_pool_for(token, block, ignore_pools=ignore_pools)
+                logger.debug("%s liquidity for %s at %s is %s", self, token, block, liquidity)
+                return liquidity
+            except Revert as e:
+                # TODO: debug me!
+                logger.debug('helper reverted on check_liquidity for %s at block %s: %s',token, block, e)
+            except ValueError as e:
+                if "out of gas" not in str(e):
+                    raise e
+                logger.debug('helper out of gas on check_liquidity for %s at block %s: %s',token, block, e)
+                
+        pools: Dict[UniswapV2Pool, Address] = await self.pools_for_token(token, block=block, _ignore_pools=ignore_pools, sync=False)
+        liquidity = max(await asyncio.gather(*[pool.check_liquidity(token, block) for pool in pools])) if pools else 0
         logger.debug("%s liquidity for %s at %s is %s", self, token, block, liquidity)
         return liquidity
 
     @a_sync.a_sync(ram_cache_maxsize=100_000, ram_cache_ttl=60*60)
     async def deepest_pool_for(self, token: Address, block: Block = None, *, ignore_pools = []) -> Tuple[Address, int]:
         # sourcery skip: default-mutable-arg
         try:
             return await FACTORY_HELPER.deepestPoolFor.coroutine(self.factory, token, ignore_pools, block_identifier=block)
         except Exception as e:
-            e.args = (*e.args, self.__repr__(), self.label, self.address)
+            e.args = (*e.args, self.__repr__(), token, block, ignore_pools)
             raise e
     
     @cached_property
     def _supports_uniswap_helper(self) -> bool:
         """returns True if our uniswap helper contract is supported, False if not"""
         return FACTORY_HELPER and self.label and self.label not in {"zipswap"}
```

### Comparing `ypricemagic-3.4.4/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-3.4.5/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/dex/uniswap/v3.py` & `ypricemagic-3.4.5/y/prices/dex/uniswap/v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,22 +159,22 @@
             ]
         logger.debug("paths: %s", paths)
         
         amount_in = await ERC20(token, asynchronous=True).scale
 
         # TODO make this properly async after extending for brownie ContractTx
         results = await fetch_multicall(
-            *[[quoter, 'quoteExactInput', self._encode_path(path), amount_in] for path in paths],
+            *[[quoter, 'quoteExactInput', _encode_path(path), amount_in] for path in paths],
             block=block,
             sync=False
         )
         logger.debug("results: %s", results)
         # Quoter v2 uses this weird return struct, we must unpack it to get amount out.
         outputs = [
-            (amount if isinstance(amount, int) else amount[0]) / self._undo_fees(path) / 1e6
+            (amount if isinstance(amount, int) else amount[0]) / _undo_fees(path) / 1e6
             for amount, path in zip(results, paths)
             if amount
         ]
         logger.debug("outputs: %s", outputs)
         return UsdPrice(max(outputs)) if outputs else None
 
     @a_sync.aka.cached_property
@@ -195,15 +195,15 @@
         quoter = await self.__quoter__
         if block and block < await contract_creation_block_async(quoter):
             logger.debug("block %s is before %s deploy block", block, quoter)
             return 0
         
         token_in_tasks: Dict[UniswapV3Pool, asyncio.Task] = {}
         token_out_tasks: Dict[UniswapV3Pool, asyncio.Task] = {}
-        async for pool in self._pools_for_token(token, block):
+        async for pool in self.pools_for_token(token, block):
             if pool not in ignore_pools:
                 token_in_tasks[pool] = asyncio.create_task(pool.check_liquidity(token, block, sync=False))
                 token_out_tasks[pool] = asyncio.create_task(pool.check_liquidity(pool._get_token_out(token), block, sync=False))
         
         # Since uni v3 liquidity can be provided asymmetrically, the most liquid pool in terms of `token` might not actually be the most liquid pool in terms of `token_out`
         # We need some spaghetticode here to account for these erroneous liquidity values
         # TODO: Refactor this
@@ -223,27 +223,27 @@
                 logger.debug("insufficient liquidity for %s", pool)
                 token_in_tasks.pop(pool)
 
         liquidity = max(await asyncio.gather(*token_in_tasks.values())) if token_in_tasks else 0
         logger.debug("%s liquidity for %s at %s is %s", self, token, block, liquidity)
         return liquidity
 
-    async def _pools_for_token(self, token: Address, block: Block) -> AsyncIterator[UniswapV3Pool]:
+    async def pools_for_token(self, token: Address, block: Block) -> AsyncIterator[UniswapV3Pool]:
         pools = await self.__pools__
         async for pool in pools.objects(to_block=block):
             if token in pool:
                 yield pool
 
-    def _encode_path(self, path) -> bytes:
-        types = [type for _, type in zip(path, cycle(['address', 'uint24']))]
-        return encode_abi_packed(types, path)
-
-    def _undo_fees(self, path) -> float:
-        fees = [1 - fee / FEE_DENOMINATOR for fee in path if isinstance(fee, int)]
-        return math.prod(fees)
+def _encode_path(path) -> bytes:
+    types = [type for _, type in zip(path, cycle(['address', 'uint24']))]
+    return encode_abi_packed(types, path)
+
+def _undo_fees(path) -> float:
+    fees = [1 - fee / FEE_DENOMINATOR for fee in path if isinstance(fee, int)]
+    return math.prod(fees)
 
 
 class UniV3Pools(ProcessedEvents[UniswapV3Pool]):
     __slots__ = "asynchronous", 
     def __init__(self, factory: Contract, asynchronous: bool = False):
         self.asynchronous = asynchronous
         super().__init__(addresses=[factory.address], topics=[factory.topics["PoolCreated"]])
```

### Comparing `ypricemagic-3.4.4/y/prices/dex/velodrome.py` & `ypricemagic-3.4.5/y/prices/dex/velodrome.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/eth_derivs/creth.py` & `ypricemagic-3.4.5/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/eth_derivs/wsteth.py` & `ypricemagic-3.4.5/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/gearbox.py` & `ypricemagic-3.4.5/y/prices/gearbox.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/lending/aave.py` & `ypricemagic-3.4.5/y/prices/lending/aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/lending/compound.py` & `ypricemagic-3.4.5/y/prices/lending/compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/lending/ib.py` & `ypricemagic-3.4.5/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/magic.py` & `ypricemagic-3.4.5/y/prices/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/one_to_one.py` & `ypricemagic-3.4.5/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/popsicle.py` & `ypricemagic-3.4.5/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/rkp3r.py` & `ypricemagic-3.4.5/y/prices/rkp3r.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/solidex.py` & `ypricemagic-3.4.5/y/prices/solidex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/stable_swap/belt.py` & `ypricemagic-3.4.5/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/stable_swap/curve.py` & `ypricemagic-3.4.5/y/prices/stable_swap/curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/stable_swap/ellipsis.py` & `ypricemagic-3.4.5/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/stable_swap/froyo.py` & `ypricemagic-3.4.5/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-3.4.5/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/stable_swap/saddle.py` & `ypricemagic-3.4.5/y/prices/stable_swap/saddle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/synthetix.py` & `ypricemagic-3.4.5/y/prices/synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-3.4.5/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/tokenized_fund/gelato.py` & `ypricemagic-3.4.5/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/tokenized_fund/piedao.py` & `ypricemagic-3.4.5/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-3.4.5/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/utils/buckets.py` & `ypricemagic-3.4.5/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/utils/sense_check.py` & `ypricemagic-3.4.5/y/prices/utils/sense_check.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/utils/ypriceapi.py` & `ypricemagic-3.4.5/y/prices/utils/ypriceapi.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/prices/yearn.py` & `ypricemagic-3.4.5/y/prices/yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/time.py` & `ypricemagic-3.4.5/y/time.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/utils/client.py` & `ypricemagic-3.4.5/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/utils/events.py` & `ypricemagic-3.4.5/y/utils/events.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/utils/fakes.py` & `ypricemagic-3.4.5/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/utils/gather.py` & `ypricemagic-3.4.5/y/utils/gather.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/utils/logging.py` & `ypricemagic-3.4.5/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/utils/middleware.py` & `ypricemagic-3.4.5/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/utils/multicall.py` & `ypricemagic-3.4.5/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/y/utils/raw_calls.py` & `ypricemagic-3.4.5/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/ypricemagic/magic.py` & `ypricemagic-3.4.5/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.4/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-3.4.5/ypricemagic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

