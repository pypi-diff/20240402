# Comparing `tmp/synthetix-0.1.4.tar.gz` & `tmp/synthetix-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthetix-0.1.4.tar", last modified: Thu Mar 28 18:54:38 2024, max compression
+gzip compressed data, was "synthetix-0.1.5.tar", last modified: Tue Apr  2 20:10:32 2024, max compression
```

## Comparing `synthetix-0.1.4.tar` & `synthetix-0.1.5.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.541089 synthetix-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-28 18:54:24.000000 synthetix-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-28 18:54:38.541089 synthetix-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-03-28 18:54:24.000000 synthetix-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 18:54:38.541089 synthetix-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-28 18:54:24.000000 synthetix-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.529089 synthetix-0.1.4/synthetix/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.529089 synthetix-0.1.4/synthetix/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.529089 synthetix-0.1.4/synthetix/contracts/deployments/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.529089 synthetix-0.1.4/synthetix/contracts/deployments/1/
--rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/1/CannonRegistry.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.529089 synthetix-0.1.4/synthetix/contracts/deployments/10/
--rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/10/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/10/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/10/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/10/sUSD.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.533089 synthetix-0.1.4/synthetix/contracts/deployments/420/
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/420/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   113611 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/420/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/420/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    90963 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/420/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    42868 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/420/PerpsV2Market.json
--rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/420/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (127)    86175 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/420/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/420/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/420/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/420/sUSD.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.533089 synthetix-0.1.4/synthetix/contracts/deployments/421614/
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/421614/WETH.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.537089 synthetix-0.1.4/synthetix/contracts/deployments/8453/
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/8453/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/8453/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/8453/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/8453/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json
--rw-r--r--   0 runner    (1001) docker     (127)    88477 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/8453/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    34846 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/8453/USDC.json
--rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/8453/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/8453/WETH.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.537089 synthetix-0.1.4/synthetix/contracts/deployments/84532/
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/84532/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   116830 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/84532/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/84532/MintableToken.json
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/84532/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   102340 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/84532/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    53394 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/84532/Pyth.json
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json
--rw-r--r--   0 runner    (1001) docker     (127)    88477 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/84532/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/84532/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/84532/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/contracts/deployments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.537089 synthetix-0.1.4/synthetix/core/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/core/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.537089 synthetix-0.1.4/synthetix/perps/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/perps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37923 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/perps/perps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.541089 synthetix-0.1.4/synthetix/pyth/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/pyth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/pyth/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/pyth/pyth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.541089 synthetix-0.1.4/synthetix/queries/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/queries/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/queries/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/queries/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.541089 synthetix-0.1.4/synthetix/spot/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/spot/spot.py
--rw-r--r--   0 runner    (1001) docker     (127)    19869 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.541089 synthetix-0.1.4/synthetix/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-28 18:54:24.000000 synthetix-0.1.4/synthetix/utils/wei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.541089 synthetix-0.1.4/synthetix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-28 18:54:38.000000 synthetix-0.1.4/synthetix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-03-28 18:54:38.000000 synthetix-0.1.4/synthetix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:54:38.000000 synthetix-0.1.4/synthetix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-28 18:54:38.000000 synthetix-0.1.4/synthetix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-28 18:54:38.000000 synthetix-0.1.4/synthetix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:54:38.541089 synthetix-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-03-28 18:54:24.000000 synthetix-0.1.4/tests/test_perps_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-28 18:54:24.000000 synthetix-0.1.4/tests/test_spot_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-28 18:54:24.000000 synthetix-0.1.4/tests/test_susd.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-28 18:54:24.000000 synthetix-0.1.4/tests/test_synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.623297 synthetix-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 20:10:19.000000 synthetix-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-02 20:10:32.623297 synthetix-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-02 20:10:19.000000 synthetix-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:10:32.623297 synthetix-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-02 20:10:19.000000 synthetix-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.607297 synthetix-0.1.5/synthetix/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.607297 synthetix-0.1.5/synthetix/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.611297 synthetix-0.1.5/synthetix/contracts/deployments/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.611297 synthetix-0.1.5/synthetix/contracts/deployments/1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/1/CannonRegistry.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.611297 synthetix-0.1.5/synthetix/contracts/deployments/10/
+-rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/10/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/10/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/10/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/10/sUSD.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.611297 synthetix-0.1.5/synthetix/contracts/deployments/420/
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   113611 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90963 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42868 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsV2Market.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (127)    86175 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/sUSD.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.611297 synthetix-0.1.5/synthetix/contracts/deployments/421614/
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/421614/WETH.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.615297 synthetix-0.1.5/synthetix/contracts/deployments/8453/
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)    88477 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34846 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/USDC.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/WETH.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/contracts/deployments/84532/
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   116830 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/MintableToken.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   102340 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    53394 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/Pyth.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)    88477 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/core/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/perps/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/perps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37923 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/perps/perps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/pyth/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/pyth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/pyth/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/pyth/pyth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/queries/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/queries/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/queries/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/spot/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/spot/spot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20714 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/utils/wei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-02 20:10:32.000000 synthetix-0.1.5/synthetix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-02 20:10:32.000000 synthetix-0.1.5/synthetix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:10:32.000000 synthetix-0.1.5/synthetix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 20:10:32.000000 synthetix-0.1.5/synthetix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 20:10:32.000000 synthetix-0.1.5/synthetix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-04-02 20:10:19.000000 synthetix-0.1.5/tests/test_perps_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-02 20:10:19.000000 synthetix-0.1.5/tests/test_spot_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-02 20:10:19.000000 synthetix-0.1.5/tests/test_susd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-02 20:10:19.000000 synthetix-0.1.5/tests/test_synthetix.py
```

### Comparing `synthetix-0.1.4/PKG-INFO` & `synthetix-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetix
-Version: 0.1.4
+Version: 0.1.5
 Summary: Synthetix protocol SDK
 Author: Synthetix DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `synthetix-0.1.4/README.md` & `synthetix-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/setup.py` & `synthetix-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="synthetix",
-    version="0.1.4",
+    version="0.1.5",
     description="Synthetix protocol SDK",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Synthetix DAO",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

### Comparing `synthetix-0.1.4/synthetix/constants.py` & `synthetix-0.1.5/synthetix/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # default
 DEFAULT_NETWORK_ID = 8453
 DEFAULT_TRACKING_CODE = (
     "0x53594e5448455449585f53444b00000000000000000000000000000000000000"
 )
 DEFAULT_REFERRER = "0x0000000000000000000000000000000000000000"
 DEFAULT_SLIPPAGE = 2.0
+DEFAULT_GAS_MULTIPLIER = 2.0
 
 DEFAULT_GQL_ENDPOINT_PERPS = {
     10: "https://api.thegraph.com/subgraphs/name/kwenta/optimism-perps",
 }
 
 DEFAULT_GQL_ENDPOINT_RATES = {
     10: "https://api.thegraph.com/subgraphs/name/kwenta/optimism-latest-rates",
```

### Comparing `synthetix-0.1.4/synthetix/contracts/contracts.py` & `synthetix-0.1.5/synthetix/contracts/contracts.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/1/CannonRegistry.json` & `synthetix-0.1.5/synthetix/contracts/deployments/1/CannonRegistry.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/10/PerpsV2MarketData.json` & `synthetix-0.1.5/synthetix/contracts/deployments/10/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/10/USDProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/10/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/10/WETH.json` & `synthetix-0.1.5/synthetix/contracts/deployments/10/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/10/sUSD.json` & `synthetix-0.1.5/synthetix/contracts/deployments/10/sUSD.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/420/AccountProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/420/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/420/CoreProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/420/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/420/PerpsAccountProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/420/PerpsMarketProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/420/PerpsV2Market.json` & `synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsV2Market.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/420/PerpsV2MarketData.json` & `synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/420/SpotMarketProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/420/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json` & `synthetix-0.1.5/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/420/USDProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/420/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/420/WETH.json` & `synthetix-0.1.5/synthetix/contracts/deployments/420/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/420/sUSD.json` & `synthetix-0.1.5/synthetix/contracts/deployments/420/sUSD.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/421614/WETH.json` & `synthetix-0.1.5/synthetix/contracts/deployments/421614/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/8453/AccountProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/8453/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/8453/CoreProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/8453/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/8453/PerpsAccountProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/8453/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/8453/PerpsMarketProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/8453/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json` & `synthetix-0.1.5/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/8453/SpotMarketProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/8453/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json` & `synthetix-0.1.5/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/8453/USDC.json` & `synthetix-0.1.5/synthetix/contracts/deployments/8453/USDC.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/8453/USDProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/8453/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/8453/WETH.json` & `synthetix-0.1.5/synthetix/contracts/deployments/8453/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/84532/AccountProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/84532/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/84532/CoreProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/84532/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/84532/MintableToken.json` & `synthetix-0.1.5/synthetix/contracts/deployments/84532/MintableToken.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/84532/PerpsAccountProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/84532/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/84532/PerpsMarketProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/84532/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/84532/Pyth.json` & `synthetix-0.1.5/synthetix/contracts/deployments/84532/Pyth.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json` & `synthetix-0.1.5/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/84532/SpotMarketProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/84532/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json` & `synthetix-0.1.5/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/84532/USDProxy.json` & `synthetix-0.1.5/synthetix/contracts/deployments/84532/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/contracts/deployments/84532/WETH.json` & `synthetix-0.1.5/synthetix/contracts/deployments/84532/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/core/core.py` & `synthetix-0.1.5/synthetix/core/core.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/perps/perps.py` & `synthetix-0.1.5/synthetix/perps/perps.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/pyth/constants.py` & `synthetix-0.1.5/synthetix/pyth/constants.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/pyth/pyth.py` & `synthetix-0.1.5/synthetix/pyth/pyth.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/queries/config.py` & `synthetix-0.1.5/synthetix/queries/config.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/queries/gql.py` & `synthetix-0.1.5/synthetix/queries/gql.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/queries/queries.py` & `synthetix-0.1.5/synthetix/queries/queries.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/spot/spot.py` & `synthetix-0.1.5/synthetix/spot/spot.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/synthetix.py` & `synthetix-0.1.5/synthetix/synthetix.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-import asyncio
-import time
 import logging
 import warnings
-import web3
 from web3 import Web3
 from web3.constants import ADDRESS_ZERO
 from web3.types import TxParams
 from .constants import (
     DEFAULT_NETWORK_ID,
     DEFAULT_TRACKING_CODE,
     DEFAULT_SLIPPAGE,
+    DEFAULT_GAS_MULTIPLIER,
     DEFAULT_GQL_ENDPOINT_PERPS,
     DEFAULT_GQL_ENDPOINT_RATES,
     DEFAULT_PRICE_SERVICE_ENDPOINTS,
     DEFAULT_REFERRER,
     DEFAULT_TRACKING_CODE,
 )
 from .utils import wei_to_ether, ether_to_wei
 from .contracts import load_contracts
 from .pyth import Pyth
 from .core import Core
 from .perps import Perps
 from .spot import Spot
 
-# from .alerts import Alerts
 from .queries import Queries
 
 warnings.filterwarnings("ignore")
 
 
 class Synthetix:
     """
@@ -89,25 +86,24 @@
         mainnet_rpc: str = "https://eth.llamarpc.com",
         ipfs_gateway: str = "https://ipfs.synthetix.io/ipfs/",
         address: str = ADDRESS_ZERO,
         private_key: str = None,
         network_id: int = None,
         core_account_id: int = None,
         perps_account_id: int = None,
-        tracking_code: str = None,
-        referrer: str = None,
+        tracking_code: str = DEFAULT_TRACKING_CODE,
+        referrer: str = DEFAULT_REFERRER,
         max_price_impact: float = DEFAULT_SLIPPAGE,
         use_estimate_gas: bool = True,
         cannon_config: dict = None,
         gql_endpoint_perps: str = None,
         gql_endpoint_rates: str = None,
         satsuma_api_key: str = None,
         price_service_endpoint: str = None,
-        telegram_token: str = None,
-        telegram_channel_name: str = None,
+        gas_multiplier: float = DEFAULT_GAS_MULTIPLIER,
     ):
         # set up logging
         self.logger = logging.getLogger(self.__class__.__name__)
         self.logger.setLevel(logging.INFO)
 
         handler = logging.StreamHandler()
         handler.setFormatter(
@@ -117,36 +113,25 @@
 
         # set default values
         if network_id is None:
             network_id = DEFAULT_NETWORK_ID
         else:
             network_id = int(network_id)
 
-        if tracking_code:
-            self.tracking_code = tracking_code
-        else:
-            self.tracking_code = DEFAULT_TRACKING_CODE
-
-        if referrer:
-            self.referrer = referrer
-        else:
-            self.referrer = DEFAULT_REFERRER
-
-        if max_price_impact:
-            self.max_price_impact = max_price_impact
-        else:
-            self.max_price_impact = DEFAULT_SLIPPAGE
-
         # init account variables
         self.private_key = private_key
         self.use_estimate_gas = use_estimate_gas
         self.cannon_config = cannon_config
         self.provider_rpc = provider_rpc
         self.mainnet_rpc = mainnet_rpc
         self.ipfs_gateway = ipfs_gateway
+        self.gas_multiplier = gas_multiplier
+        self.max_price_impact = max_price_impact
+        self.tracking_code = tracking_code
+        self.referrer = referrer
 
         # init chain provider
         if provider_rpc.startswith("http"):
             web3 = Web3(Web3.HTTPProvider(self.provider_rpc))
         elif provider_rpc.startswith("wss"):
             web3 = Web3(Web3.WebsocketProvider(self.provider_rpc))
         elif provider_rpc.endswith("ipc"):
@@ -176,18 +161,14 @@
         (
             self.v2_markets,
             self.susd_legacy_token,
             self.susd_token,
             self.multicall,
         ) = self._load_contracts()
 
-        # init alerts
-        # if telegram_token and telegram_channel_name:
-        #     self.alerts = Alerts(telegram_token, telegram_channel_name)
-
         # init queries
         if not gql_endpoint_perps and self.network_id in DEFAULT_GQL_ENDPOINT_PERPS:
             gql_endpoint_perps = DEFAULT_GQL_ENDPOINT_PERPS[self.network_id]
 
         if not gql_endpoint_rates and self.network_id in DEFAULT_GQL_ENDPOINT_RATES:
             gql_endpoint_rates = DEFAULT_GQL_ENDPOINT_RATES[self.network_id]
 
@@ -334,47 +315,76 @@
         :param int timeout: timeout in seconds
         :return: A transaction receipt
         :rtype: dict
         """
         receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=timeout)
         return receipt
 
-    def execute_transaction(self, tx_data: dict):
+    def _send_transaction(self, tx_data: dict):
         """
-        Execute a provided transaction. This function will be signed with the provided
-        private key and submitted to the connected RPC. The ``Synthetix`` object tracks
-        the nonce internally, and will handle estimating gas limits if they are not
-        provided.
+        Send a prepared transaction to the connected RPC. If the RPC has a signer for
+        the account in the `from` field, the transaction is sent directly to the RPC.
+        For other addresses, if a private key is provided, the transaction is signed
+        and sent to the RPC. Otherwise, this function will raise an error.
 
         :param dict tx_data: transaction data
         :return: A transaction hash
         :rtype: str
         """
+
         is_rpc_signer = tx_data["from"] in self.web3.eth.accounts
         if not is_rpc_signer and self.private_key is None:
             raise Exception("No private key specified.")
 
-        if "gas" not in tx_data:
-            if self.use_estimate_gas:
-                tx_data["gas"] = int(self.web3.eth.estimate_gas(tx_data) * 1.2)
-            else:
-                tx_data["gas"] = 1500000
-
         if is_rpc_signer:
-            tx_token = self.web3.eth.send_transaction(tx_data)
+            tx_hash = self.web3.eth.send_transaction(tx_data)
         else:
             signed_txn = self.web3.eth.account.sign_transaction(
                 tx_data, private_key=self.private_key
             )
-            tx_token = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
+            tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
 
-        # increase nonce
         self.nonce += 1
+        return self.web3.to_hex(tx_hash)
 
-        return self.web3.to_hex(tx_token)
+    def execute_transaction(self, tx_data: dict, reset_nonce: bool = False):
+        """
+        Execute a provided transaction. This function will be signed with the provided
+        private key and submitted to the connected RPC. The ``Synthetix`` object tracks
+        the nonce internally, and will handle estimating gas limits if they are not
+        provided.
+
+        :param dict tx_data: transaction data
+        :param bool reset_nonce: call the RPC to get the current nonce, otherwise use the
+            stored nonce
+        :return: A transaction hash
+        :rtype: str
+        """
+        if "gas" not in tx_data:
+            if self.use_estimate_gas:
+                tx_data["gas"] = int(
+                    self.web3.eth.estimate_gas(tx_data) * self.gas_multiplier
+                )
+            else:
+                tx_data["gas"] = 1500000
+
+        if reset_nonce:
+            self.nonce = self.web3.eth.get_transaction_count(self.address)
+            tx_data["nonce"] = self.nonce
+
+        try:
+            self.logger.info(f"Tx data: {tx_data}")
+            tx_hash = self._send_transaction(tx_data)
+            return tx_hash
+        except ValueError as e:
+            if "nonce too low" in str(e):
+                self.logger.info("Nonce too low, resetting nonce and retrying.")
+                return self.execute_transaction(tx_data, reset_nonce=True)
+            else:
+                raise Exception(f"Transaction failed: {e}")
 
     def get_susd_balance(self, address: str = None, legacy: bool = False) -> dict:
         """
         Gets current sUSD balance in wallet. Supports both legacy and V3 sUSD.
 
         :param str address: address to check balances for
         :param bool legacy: check legacy sUSD balance
```

### Comparing `synthetix-0.1.4/synthetix/utils/multicall.py` & `synthetix-0.1.5/synthetix/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix/utils/wei.py` & `synthetix-0.1.5/synthetix/utils/wei.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/synthetix.egg-info/PKG-INFO` & `synthetix-0.1.5/synthetix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetix
-Version: 0.1.4
+Version: 0.1.5
 Summary: Synthetix protocol SDK
 Author: Synthetix DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `synthetix-0.1.4/synthetix.egg-info/SOURCES.txt` & `synthetix-0.1.5/synthetix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/tests/test_perps_v3.py` & `synthetix-0.1.5/tests/test_perps_v3.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/tests/test_spot_v3.py` & `synthetix-0.1.5/tests/test_spot_v3.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.4/tests/test_susd.py` & `synthetix-0.1.5/tests/test_susd.py`

 * *Files identical despite different names*

