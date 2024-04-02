# Comparing `tmp/prediction_market_agent_tooling-0.6.0.tar.gz` & `tmp/prediction_market_agent_tooling-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prediction_market_agent_tooling-0.6.0.tar", max compression
+gzip compressed data, was "prediction_market_agent_tooling-0.7.0.tar", max compression
```

## Comparing `prediction_market_agent_tooling-0.6.0.tar` & `prediction_market_agent_tooling-0.7.0.tar`

### file list

```diff
@@ -1,55 +1,64 @@
--rw-r--r--   0        0        0     7650 2024-03-20 13:46:31.067683 prediction_market_agent_tooling-0.6.0/LICENSE
--rw-r--r--   0        0        0     2985 2024-03-20 13:46:31.067683 prediction_market_agent_tooling-0.6.0/README.md
--rw-r--r--   0        0        0     9578 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_dxdao.abi.json
--rw-r--r--   0        0        0    11406 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_fpmm.abi.json
--rw-r--r--   0        0        0     9841 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json
--rw-r--r--   0        0        0     4777 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json
--rw-r--r--   0        0        0     7315 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_kleros.abi.json
--rw-r--r--   0        0        0     1775 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_oracle.abi.json
--rw-r--r--   0        0        0    15953 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_realitio.abi.json
--rw-r--r--   0        0        0     6055 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/wxdai.abi.json
--rw-r--r--   0        0        0        0 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/benchmark/__init__.py
--rw-r--r--   0        0        0     3737 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/benchmark/agents.py
--rw-r--r--   0        0        0    21237 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/benchmark/benchmark.py
--rw-r--r--   0        0        0     2748 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/benchmark/utils.py
--rw-r--r--   0        0        0     2053 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/config.py
--rw-r--r--   0        0        0     6780 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/deploy/agent.py
--rw-r--r--   0        0        0      607 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/deploy/agent_example.py
--rw-r--r--   0        0        0       82 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/deploy/constants.py
--rw-r--r--   0        0        0     3739 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/deploy/gcp/deploy.py
--rw-r--r--   0        0        0     5255 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/deploy/gcp/utils.py
--rw-r--r--   0        0        0     2290 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/gtypes.py
--rw-r--r--   0        0        0     4458 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/agent_market.py
--rw-r--r--   0        0        0      422 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/betting_strategies.py
--rw-r--r--   0        0        0      961 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/categorize.py
--rw-r--r--   0        0        0      763 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/data_models.py
--rw-r--r--   0        0        0        0 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/manifold/__init__.py
--rw-r--r--   0        0        0     6670 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/manifold/api.py
--rw-r--r--   0        0        0     5309 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/manifold/data_models.py
--rw-r--r--   0        0        0     3303 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/manifold/manifold.py
--rw-r--r--   0        0        0     1324 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/markets.py
--rw-r--r--   0        0        0        0 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/omen/__init__.py
--rw-r--r--   0        0        0     7992 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/omen/data_models.py
--rw-r--r--   0        0        0    26610 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/omen/omen.py
--rw-r--r--   0        0        0    13803 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/omen/omen_contracts.py
--rw-r--r--   0        0        0     5043 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/omen/omen_replicate.py
--rw-r--r--   0        0        0     4188 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/polymarket/api.py
--rw-r--r--   0        0        0     3909 2024-03-20 13:46:31.071683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/polymarket/data_models.py
--rw-r--r--   0        0        0     2494 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/polymarket/polymarket.py
--rw-r--r--   0        0        0     2503 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/monitor/markets/manifold.py
--rw-r--r--   0        0        0     2335 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/monitor/markets/omen.py
--rw-r--r--   0        0        0     2413 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/monitor/markets/polymarket.py
--rw-r--r--   0        0        0    11392 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/monitor/monitor.py
--rw-r--r--   0        0        0     4124 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/monitor/monitor_app.py
--rw-r--r--   0        0        0        0 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/py.typed
--rw-r--r--   0        0        0     3520 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py
--rw-r--r--   0        0        0     4334 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py
--rw-r--r--   0        0        0      499 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/cache.py
--rw-r--r--   0        0        0     5879 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/contract.py
--rw-r--r--   0        0        0      641 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/gnosis_rpc.py
--rw-r--r--   0        0        0     2530 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/is_predictable.py
--rw-r--r--   0        0        0      733 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/parallelism.py
--rw-r--r--   0        0        0     3656 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/utils.py
--rw-r--r--   0        0        0     4873 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/web3_utils.py
--rw-r--r--   0        0        0     1211 2024-03-20 13:46:31.075683 prediction_market_agent_tooling-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4477 1970-01-01 00:00:00.000000 prediction_market_agent_tooling-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     7650 2024-04-02 07:54:21.061069 prediction_market_agent_tooling-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2985 2024-04-02 07:54:21.061069 prediction_market_agent_tooling-0.7.0/README.md
+-rw-r--r--   0        0        0     9578 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_dxdao.abi.json
+-rw-r--r--   0        0        0    11406 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_fpmm.abi.json
+-rw-r--r--   0        0        0     9841 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json
+-rw-r--r--   0        0        0     4777 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json
+-rw-r--r--   0        0        0     7315 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_kleros.abi.json
+-rw-r--r--   0        0        0     1775 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_oracle.abi.json
+-rw-r--r--   0        0        0    15953 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_realitio.abi.json
+-rw-r--r--   0        0        0     6055 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/wxdai.abi.json
+-rw-r--r--   0        0        0        0 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/benchmark/__init__.py
+-rw-r--r--   0        0        0     3737 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/benchmark/agents.py
+-rw-r--r--   0        0        0    21237 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/benchmark/benchmark.py
+-rw-r--r--   0        0        0     2748 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/benchmark/utils.py
+-rw-r--r--   0        0        0     2596 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/config.py
+-rw-r--r--   0        0        0     7627 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/deploy/agent.py
+-rw-r--r--   0        0        0      607 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/deploy/agent_example.py
+-rw-r--r--   0        0        0       82 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/deploy/constants.py
+-rw-r--r--   0        0        0     3739 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/deploy/gcp/deploy.py
+-rw-r--r--   0        0        0     5255 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/deploy/gcp/utils.py
+-rw-r--r--   0        0        0     2526 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/gtypes.py
+-rw-r--r--   0        0        0     4488 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/agent_market.py
+-rw-r--r--   0        0        0     1026 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/categorize.py
+-rw-r--r--   0        0        0      763 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/data_models.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/manifold/__init__.py
+-rw-r--r--   0        0        0     6670 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/manifold/api.py
+-rw-r--r--   0        0        0     5357 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/manifold/data_models.py
+-rw-r--r--   0        0        0     3402 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/manifold/manifold.py
+-rw-r--r--   0        0        0      513 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/manifold/utils.py
+-rw-r--r--   0        0        0     1550 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/markets.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/omen/__init__.py
+-rw-r--r--   0        0        0    10343 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/omen/data_models.py
+-rw-r--r--   0        0        0    23821 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/omen/omen.py
+-rw-r--r--   0        0        0    18800 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/omen/omen_contracts.py
+-rw-r--r--   0        0        0     5508 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/omen/omen_replicate.py
+-rw-r--r--   0        0        0    11340 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/omen/omen_resolve_replicated.py
+-rw-r--r--   0        0        0    13738 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/omen/omen_subgraph_handler.py
+-rw-r--r--   0        0        0     4188 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/polymarket/api.py
+-rw-r--r--   0        0        0     4199 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/polymarket/data_models.py
+-rw-r--r--   0        0        0    10863 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/polymarket/data_models_web.py
+-rw-r--r--   0        0        0     2652 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/polymarket/polymarket.py
+-rw-r--r--   0        0        0     1960 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/polymarket/utils.py
+-rw-r--r--   0        0        0     2503 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/monitor/markets/manifold.py
+-rw-r--r--   0        0        0     2419 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/monitor/markets/omen.py
+-rw-r--r--   0        0        0     2413 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/monitor/markets/polymarket.py
+-rw-r--r--   0        0        0    11465 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/monitor/monitor.py
+-rw-r--r--   0        0        0     4045 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/monitor/monitor_app.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/py.typed
+-rw-r--r--   0        0        0      625 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/balances.py
+-rw-r--r--   0        0        0     3520 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py
+-rw-r--r--   0        0        0     4367 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py
+-rw-r--r--   0        0        0      422 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/betting_strategies/minimum_bet_to_win.py
+-rw-r--r--   0        0        0      429 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/betting_strategies/stretch_bet_between.py
+-rw-r--r--   0        0        0      499 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/cache.py
+-rw-r--r--   0        0        0     5879 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/contract.py
+-rw-r--r--   0        0        0      660 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/gnosis_rpc.py
+-rw-r--r--   0        0        0     1728 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/google.py
+-rw-r--r--   0        0        0     2037 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/hexbytes_custom.py
+-rw-r--r--   0        0        0     2613 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/is_predictable.py
+-rw-r--r--   0        0        0      733 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/parallelism.py
+-rw-r--r--   0        0        0     4022 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/utils.py
+-rw-r--r--   0        0        0     5246 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/web3_utils.py
+-rw-r--r--   0        0        0     1355 2024-04-02 07:54:21.069069 prediction_market_agent_tooling-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4653 1970-01-01 00:00:00.000000 prediction_market_agent_tooling-0.7.0/PKG-INFO
```

### Comparing `prediction_market_agent_tooling-0.6.0/LICENSE` & `prediction_market_agent_tooling-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/README.md` & `prediction_market_agent_tooling-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_dxdao.abi.json` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_dxdao.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_fpmm.abi.json` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_fpmm.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_kleros.abi.json` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_kleros.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_oracle.abi.json` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_oracle.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/omen_realitio.abi.json` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/omen_realitio.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/abis/wxdai.abi.json` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/abis/wxdai.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/benchmark/agents.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/benchmark/agents.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/benchmark/benchmark.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/benchmark/utils.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/config.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,17 @@
         env_file=".env", env_file_encoding="utf-8", extra="ignore"
     )
 
     MANIFOLD_API_KEY: t.Optional[SecretStr] = None
     BET_FROM_PRIVATE_KEY: t.Optional[PrivateKey] = None
     OPENAI_API_KEY: t.Optional[SecretStr] = None
 
+    GOOGLE_SEARCH_API_KEY: t.Optional[SecretStr] = None
+    GOOGLE_SEARCH_ENGINE_ID: t.Optional[SecretStr] = None
+
     ENABLE_CACHE: bool = True
     CACHE_DIR: str = "./.cache"
 
     @property
     def manifold_api_key(self) -> SecretStr:
         return check_not_none(
             self.MANIFOLD_API_KEY, "MANIFOLD_API_KEY missing in the environment."
@@ -46,14 +49,28 @@
 
     @property
     def openai_api_key(self) -> SecretStr:
         return check_not_none(
             self.OPENAI_API_KEY, "OPENAI_API_KEY missing in the environment."
         )
 
+    @property
+    def google_search_api_key(self) -> SecretStr:
+        return check_not_none(
+            self.GOOGLE_SEARCH_API_KEY,
+            "GOOGLE_SEARCH_API_KEY missing in the environment.",
+        )
+
+    @property
+    def google_search_engine_id(self) -> SecretStr:
+        return check_not_none(
+            self.GOOGLE_SEARCH_ENGINE_ID,
+            "GOOGLE_SEARCH_ENGINE_ID missing in the environment.",
+        )
+
     def model_dump_public(self) -> dict[str, t.Any]:
         return {
             k: v
             for k, v in self.model_dump().items()
             if APIKeys.model_fields[k].annotation not in SECRET_TYPES and v is not None
         }
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/deploy/agent.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/deploy/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import inspect
 import os
 import tempfile
 import time
 import typing as t
 from datetime import datetime
 
+from loguru import logger
+
 from prediction_market_agent_tooling.config import APIKeys
 from prediction_market_agent_tooling.deploy.constants import (
     MARKET_TYPE_KEY,
     REPOSITORY_KEY,
 )
 from prediction_market_agent_tooling.deploy.gcp.deploy import (
     deploy_to_gcp,
     run_deployed_gcp_function,
     schedule_deployed_gcp_function,
 )
 from prediction_market_agent_tooling.deploy.gcp.utils import (
     gcp_function_is_active,
     gcp_resolve_api_keys_secrets,
 )
-from prediction_market_agent_tooling.markets.agent_market import AgentMarket, SortBy
+from prediction_market_agent_tooling.markets.agent_market import (
+    AgentMarket,
+    FilterBy,
+    SortBy,
+)
 from prediction_market_agent_tooling.markets.data_models import BetAmount
-from prediction_market_agent_tooling.markets.markets import (
-    MARKET_TYPE_TO_AGENT_MARKET,
-    MarketType,
+from prediction_market_agent_tooling.markets.markets import MarketType
+from prediction_market_agent_tooling.markets.omen.omen import (
+    redeem_positions_from_all_omen_markets,
 )
 from prediction_market_agent_tooling.monitor.monitor_app import (
     MARKET_TYPE_TO_DEPLOYED_AGENT,
 )
 from prediction_market_agent_tooling.tools.utils import DatetimeWithTimezone, utcnow
 
 MAX_AVAILABLE_MARKETS = 20
@@ -48,15 +54,15 @@
 
     def pick_markets(self, markets: list[AgentMarket]) -> list[AgentMarket]:
         """
         This method should be implemented by the subclass to pick the markets to bet on. By default, it picks only the first market.
         """
         return markets[:1]
 
-    def answer_binary_market(self, market: AgentMarket) -> bool:
+    def answer_binary_market(self, market: AgentMarket) -> bool | None:
         """
         Answer the binary market. This method must be implemented by the subclass.
         """
         raise NotImplementedError("This method must be implemented by the subclass")
 
     def deploy_local(
         self,
@@ -159,32 +165,55 @@
         return market.get_tiny_bet_amount()
 
     def get_markets(
         self,
         market_type: MarketType,
         limit: int = MAX_AVAILABLE_MARKETS,
         sort_by: SortBy = SortBy.CLOSING_SOONEST,
+        filter_by: FilterBy = FilterBy.OPEN,
     ) -> list[AgentMarket]:
-        cls = MARKET_TYPE_TO_AGENT_MARKET.get(market_type)
-        if not cls:
-            raise ValueError(f"Unknown market type: {market_type}")
+        cls = market_type.market_class
         # Fetch the soonest closing markets to choose from
-        available_markets = cls.get_binary_markets(limit=limit, sort_by=sort_by)
+        available_markets = cls.get_binary_markets(
+            limit=limit, sort_by=sort_by, filter_by=filter_by
+        )
         return available_markets
 
-    def run(self, market_type: MarketType, _place_bet: bool = True) -> None:
+    def before(self, market_type: MarketType) -> None:
+        """
+        Executes actions that occur before bets are placed.
+        """
+
+        if market_type == MarketType.OMEN:
+            redeem_positions_from_all_omen_markets()
+
+    def process_bets(self, market_type: MarketType, _place_bet: bool = True) -> None:
+        """
+        Processes bets placed by agents on a given market.
+        """
         available_markets = self.get_markets(market_type)
         markets = self.pick_markets(available_markets)
         for market in markets:
             result = self.answer_binary_market(market)
+            if result is None:
+                logger.debug(f"Skipping market {market} as no answer was provided")
+                continue
             if _place_bet:
                 amount = self.calculate_bet_amount(result, market)
-                print(
+                logger.debug(
                     f"Placing bet on {market} with result {result} and amount {amount}"
                 )
                 market.place_bet(
                     amount=amount,
                     outcome=result,
                 )
 
+    def after(self, market_type: MarketType) -> None:
+        pass
+
+    def run(self, market_type: MarketType, _place_bet: bool = True) -> None:
+        self.before(market_type)
+        self.process_bets(market_type, _place_bet)
+        self.after(market_type)
+
     def get_gcloud_fname(self, market_type: MarketType) -> str:
         return f"{self.__class__.__name__.lower()}-{market_type}-{datetime.now().strftime('%Y-%m-%d--%H-%M-%S')}"
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/deploy/agent_example.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/deploy/agent_example.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/deploy/gcp/deploy.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/deploy/gcp/deploy.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/deploy/gcp/utils.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/deploy/gcp/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/gtypes.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/gtypes.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 
 from eth_typing.evm import (  # noqa: F401  # Import for the sake of easy importing with others from here.
     Address,
     ChecksumAddress,
     HexAddress,
     HexStr,
 )
-from hexbytes import (  # noqa: F401  # Import for the sake of easy importing with others from here.
-    HexBytes,
-)
 from pydantic.types import SecretStr
 from pydantic.v1.types import SecretStr as SecretStrV1
 from web3.types import (  # noqa: F401  # Import for the sake of easy importing with others from here.
     Nonce,
     TxParams,
     TxReceipt,
     Wei,
 )
 
+from prediction_market_agent_tooling.tools.hexbytes_custom import (  # noqa: F401  # Import for the sake of easy importing with others from here.
+    HexBytes,
+)
+
 Wad = Wei  # Wei tends to be referred to as `wad` variable in contracts.
 USD = NewType(
     "USD", Decimal
 )  # Decimals are more precise than floats, good for finances.
 PrivateKey = NewType("PrivateKey", SecretStr)
 xDai = NewType("xDai", Decimal)
 GNO = NewType("GNO", Decimal)
@@ -74,7 +75,12 @@
 def secretstr_to_v1_secretstr(s: None) -> None:
     ...
 
 
 def secretstr_to_v1_secretstr(s: SecretStr | None) -> SecretStrV1 | None:
     # Another library can be typed with v1, and then we need this ugly conversion.
     return SecretStrV1(s.get_secret_value()) if s is not None else None
+
+
+def int_to_hexbytes(v: int) -> HexBytes:
+    # Example: 1 -> HexBytes("0x0000000000000000000000000000000000000000000000000000000000000001").
+    return HexBytes.fromhex(format(v, "064x"))
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/agent_market.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/agent_market.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 class AgentMarket(BaseModel):
     """
     Common market class that can be created from vendor specific markets.
     Contains everything that is needed for an agent to make a prediction.
     """
 
     currency: t.ClassVar[Currency]
+    base_url: t.ClassVar[str]
 
     id: str
     question: str
     outcomes: list[str]
     resolution: Resolution | None
     created_time: datetime | None
     close_time: datetime | None
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/categorize.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/categorize.py`

 * *Files 25% similar despite different names*

```diff
@@ -27,8 +27,10 @@
         | StrOutputParser()
     )
 
     response: str = research_evaluation_chain.invoke(
         {"question": question, "categories": sorted(categories)}
     )
 
-    return response
+    formatted = response.strip().strip("'").strip('"').strip()
+
+    return formatted
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/data_models.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/data_models.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/manifold/api.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/manifold/api.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/manifold/data_models.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/manifold/data_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from prediction_market_agent_tooling.markets.data_models import (
     Currency,
     ProfitAmount,
     Resolution,
 )
 from prediction_market_agent_tooling.tools.utils import should_not_happen
 
+MANIFOLD_BASE_URL = "https://manifold.markets"
+
 
 class ManifoldPool(BaseModel):
     NO: float
     YES: float
 
 
 class ManifoldMarket(BaseModel):
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/manifold/manifold.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/manifold/manifold.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 
 from prediction_market_agent_tooling.gtypes import Mana, Probability, mana_type
 from prediction_market_agent_tooling.markets.agent_market import (
     AgentMarket,
     FilterBy,
     SortBy,
 )
-from prediction_market_agent_tooling.markets.betting_strategies import (
-    minimum_bet_to_win,
-)
 from prediction_market_agent_tooling.markets.data_models import BetAmount, Currency
 from prediction_market_agent_tooling.markets.manifold.api import (
     get_manifold_binary_markets,
     place_bet,
 )
-from prediction_market_agent_tooling.markets.manifold.data_models import ManifoldMarket
+from prediction_market_agent_tooling.markets.manifold.data_models import (
+    MANIFOLD_BASE_URL,
+    ManifoldMarket,
+)
+from prediction_market_agent_tooling.tools.betting_strategies.minimum_bet_to_win import (
+    minimum_bet_to_win,
+)
 
 
 class ManifoldAgentMarket(AgentMarket):
     """
     Manifold's market class that can be used by agents to make predictions.
     """
 
     currency: t.ClassVar[Currency] = Currency.Mana
+    base_url: t.ClassVar[str] = MANIFOLD_BASE_URL
 
     def get_tiny_bet_amount(self) -> BetAmount:
         return BetAmount(amount=Decimal(1), currency=self.currency)
 
     def get_minimum_bet_to_win(self, answer: bool, amount_to_win: float) -> Mana:
         # Manifold lowest bet is 1 Mana, so we need to ceil the result.
         return mana_type(ceil(minimum_bet_to_win(answer, amount_to_win, self)))
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/markets.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/markets.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,20 @@
 
 
 class MarketType(str, Enum):
     MANIFOLD = "manifold"
     OMEN = "omen"
     POLYMARKET = "polymarket"
 
+    @property
+    def market_class(self) -> type[AgentMarket]:
+        if self not in MARKET_TYPE_TO_AGENT_MARKET:
+            raise ValueError(f"Unknown market type: {self}")
+        return MARKET_TYPE_TO_AGENT_MARKET[self]
+
 
 MARKET_TYPE_TO_AGENT_MARKET: dict[MarketType, type[AgentMarket]] = {
     MarketType.MANIFOLD: ManifoldAgentMarket,
     MarketType.OMEN: OmenAgentMarket,
     MarketType.POLYMARKET: PolymarketAgentMarket,
 }
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/omen/data_models.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/omen/data_models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import typing as t
 from datetime import datetime
 from decimal import Decimal
 
-from eth_typing import ChecksumAddress, HexAddress
 from pydantic import BaseModel
 from web3 import Web3
 
 from prediction_market_agent_tooling.gtypes import (
     USD,
+    ChecksumAddress,
+    HexAddress,
+    HexBytes,
     OmenOutcomeToken,
     Probability,
     Wei,
     xDai,
 )
 from prediction_market_agent_tooling.markets.data_models import (
     BetAmount,
@@ -22,55 +24,88 @@
 )
 from prediction_market_agent_tooling.tools.utils import check_not_none
 from prediction_market_agent_tooling.tools.web3_utils import wei_to_xdai
 
 OMEN_TRUE_OUTCOME = "Yes"
 OMEN_FALSE_OUTCOME = "No"
 INVALID_ANSWER = 0xFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+OMEN_BASE_URL = "https://aiomen.eth.limo"
 
 
 def get_boolean_outcome(outcome_str: str) -> bool:
     if outcome_str == OMEN_TRUE_OUTCOME:
         return True
     if outcome_str == OMEN_FALSE_OUTCOME:
         return False
     raise ValueError(f"Outcome `{outcome_str}` is not a valid boolean outcome.")
 
 
 class Condition(BaseModel):
-    id: HexAddress
+    id: HexBytes
     outcomeSlotCount: int
 
     @property
     def index_sets(self) -> t.List[int]:
         return [i + 1 for i in range(self.outcomeSlotCount)]
 
 
+class Question(BaseModel):
+    id: HexBytes
+    title: str
+    data: str
+    templateId: int
+    outcomes: list[str]
+    isPendingArbitration: bool
+    answerFinalizedTimestamp: t.Optional[datetime] = None
+    currentAnswer: t.Optional[str] = None
+
+    @property
+    def question_raw(self) -> str:
+        # Based on https://github.com/protofire/omen-exchange/blob/2cfdf6bfe37afa8b169731d51fea69d42321d66c/app/src/hooks/graph/useGraphMarketMakerData.tsx#L217.
+        return self.data
+
+    @property
+    def n_outcomes(self) -> int:
+        return len(self.outcomes)
+
+
+class OmenPosition(BaseModel):
+    id: HexBytes
+    conditionIds: t.List[HexBytes]
+
+
+class OmenUserPosition(BaseModel):
+    id: HexBytes
+    position: OmenPosition
+
+
 class OmenMarket(BaseModel):
     """
     https://aiomen.eth.limo
     """
 
     BET_AMOUNT_CURRENCY: t.ClassVar[Currency] = Currency.xDai
 
     id: HexAddress
     title: str
+    creator: HexAddress
     category: str
     collateralVolume: Wei
     usdVolume: USD
     collateralToken: HexAddress
     outcomes: list[str]
     outcomeTokenAmounts: list[OmenOutcomeToken]
     outcomeTokenMarginalPrices: t.Optional[list[xDai]]
     fee: t.Optional[Wei]
     resolutionTimestamp: t.Optional[int] = None
     answerFinalizedTimestamp: t.Optional[int] = None
     currentAnswer: t.Optional[str] = None
     creationTimestamp: t.Optional[int] = None
     condition: Condition
+    question: Question
 
     @property
     def answer_index(self) -> t.Optional[int]:
         return int(self.currentAnswer, 16) if self.currentAnswer else None
 
     @property
     def has_valid_answer(self) -> bool:
@@ -78,18 +113,24 @@
 
     @property
     def is_open(self) -> bool:
         return self.currentAnswer is None
 
     @property
     def is_resolved(self) -> bool:
-        return self.answerFinalizedTimestamp is not None and self.has_valid_answer
+        return (
+            # Finalized on Realitio (e.g. 24h has passed since the last answer was submitted)
+            self.answerFinalizedTimestamp is not None
+            # Resolved on Oracle (e.g. resolved after it was finalized)
+            and self.resolutionTimestamp is not None
+            and self.has_valid_answer
+        )
 
     @property
-    def question(self) -> str:
+    def question_title(self) -> str:
         return self.title
 
     @property
     def creation_datetime(self) -> datetime | None:
         return (
             datetime.fromtimestamp(self.creationTimestamp)
             if self.creationTimestamp is not None
@@ -101,14 +142,18 @@
         return (
             datetime.fromtimestamp(self.answerFinalizedTimestamp)
             if self.answerFinalizedTimestamp is not None
             else None
         )
 
     @property
+    def has_bonded_outcome(self) -> bool:
+        return self.finalized_datetime is not None
+
+    @property
     def market_maker_contract_address(self) -> HexAddress:
         return self.id
 
     @property
     def market_maker_contract_address_checksummed(self) -> ChecksumAddress:
         return Web3.to_checksum_address(self.market_maker_contract_address)
 
@@ -187,15 +232,15 @@
         if self.boolean_outcome:
             return Resolution.YES
         else:
             return Resolution.NO
 
     @property
     def url(self) -> str:
-        return f"https://aiomen.eth.limo/#/{self.id}"
+        return f"{OMEN_BASE_URL}/#/{self.id}"
 
 
 class OmenBetCreator(BaseModel):
     id: HexAddress
 
 
 class OmenBet(BaseModel):
@@ -259,7 +304,42 @@
 
 class FixedProductMarketMakersData(BaseModel):
     fixedProductMarketMakers: list[OmenMarket]
 
 
 class FixedProductMarketMakersResponse(BaseModel):
     data: FixedProductMarketMakersData
+
+
+class RealityQuestion(BaseModel):
+    # This `id` is in form of `0x79e32ae03fb27b07c89c0c568f80287c01ca2e57-0x2d362f435e7b5159794ff0b5457a900283fca41fe6301dc855a647595903db13`,
+    # which I couldn't find how it is created, but based on how it looks like I assume it's composed of `answerId-questionId`.
+    # (Why is answer id as part of the question object? Because this question object is actually received from the answer object below).
+    # And because all the contract methods so far needed bytes32 input, when asked for question id, `questionId` field was the correct one to use so far.
+    id: str
+    user: HexAddress
+    historyHash: HexBytes
+    updatedTimestamp: datetime
+    contentHash: HexBytes
+    questionId: HexBytes
+
+    @property
+    def url(self) -> str:
+        return f"https://reality.eth.limo/app/#!/question/{self.id}"
+
+
+class RealityAnswer(BaseModel):
+    id: str
+    timestamp: datetime
+    answer: HexBytes
+    lastBond: Wei
+    bondAggregate: Wei
+    question: RealityQuestion
+    createdBlock: int
+
+
+class RealityAnswers(BaseModel):
+    answers: list[RealityAnswer]
+
+
+class RealityAnswersResponse(BaseModel):
+    data: RealityAnswers
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/omen/omen.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/omen/omen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,83 @@
 import typing as t
+from collections import defaultdict
 from datetime import datetime
 from decimal import Decimal
 
-import requests
-from eth_typing import HexStr
+from loguru import logger
 from web3 import Web3
 from web3.constants import HASH_ZERO
 
 from prediction_market_agent_tooling.config import APIKeys
 from prediction_market_agent_tooling.gtypes import (
     ChecksumAddress,
     HexAddress,
-    OmenOutcomeToken,
+    HexStr,
     PrivateKey,
-    TxReceipt,
     Wei,
+    wei_type,
     xDai,
+    xdai_type,
 )
 from prediction_market_agent_tooling.markets.agent_market import (
     AgentMarket,
     FilterBy,
     SortBy,
 )
 from prediction_market_agent_tooling.markets.data_models import BetAmount, Currency
 from prediction_market_agent_tooling.markets.omen.data_models import (
+    OMEN_BASE_URL,
     OMEN_FALSE_OUTCOME,
     OMEN_TRUE_OUTCOME,
     Condition,
-    FixedProductMarketMakersResponse,
     OmenBet,
     OmenMarket,
 )
 from prediction_market_agent_tooling.markets.omen.omen_contracts import (
+    OMEN_DEFAULT_MARKET_FEE,
     Arbitrator,
     OmenCollateralTokenContract,
     OmenConditionalTokenContract,
     OmenFixedProductMarketMakerContract,
     OmenFixedProductMarketMakerFactoryContract,
     OmenOracleContract,
     OmenRealitioContract,
 )
-from prediction_market_agent_tooling.tools.utils import response_to_model, utcnow
+from prediction_market_agent_tooling.markets.omen.omen_subgraph_handler import (
+    OmenSubgraphHandler,
+)
 from prediction_market_agent_tooling.tools.web3_utils import (
     add_fraction,
     private_key_to_public_key,
     remove_fraction,
     wei_to_xdai,
     xdai_to_wei,
 )
 
-"""
-Python API for Omen prediction market.
-
-Their API is available as graph on https://thegraph.com/explorer/subgraphs/9V1aHHwkK4uPWgBH6ZLzwqFEkoHTHPS7XHKyjZWe8tEf?view=Overview&chain=mainnet,
-but to not use our own credits, seems we can use their api deployment directly: https://api.thegraph.com/subgraphs/name/protofire/omen-xdai/graphql (link to the online playground)
-"""
-
-OMEN_QUERY_BATCH_SIZE = 1000
-OMEN_DEFAULT_MARKET_FEE = 0.02  # 2% fee from the buying shares amount.
-THEGRAPH_QUERY_URL = "https://api.thegraph.com/subgraphs/name/protofire/omen-xdai"
+MAX_NUMBER_OF_MARKETS_FOR_SUBGRAPH_RETRIEVAL = 1000
+OMEN_DEFAULT_REALITIO_BOND_VALUE = xdai_type(0.01)
 
 
 class OmenAgentMarket(AgentMarket):
     """
     Omen's market class that can be used by agents to make predictions.
     """
 
     currency: t.ClassVar[Currency] = Currency.xDai
+    base_url: t.ClassVar[str] = OMEN_BASE_URL
+    creator: HexAddress
 
     collateral_token_contract_address_checksummed: ChecksumAddress
     market_maker_contract_address_checksummed: ChecksumAddress
     condition: Condition
 
+    INVALID_MARKET_ANSWER: HexStr = HexStr(
+        "0xFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF"
+    )
+
     def get_tiny_bet_amount(self) -> BetAmount:
         return BetAmount(amount=Decimal(0.00001), currency=self.currency)
 
     def place_bet(
         self, outcome: bool, amount: BetAmount, omen_auto_deposit: bool = True
     ) -> None:
         if amount.currency != self.currency:
@@ -86,25 +88,73 @@
             amount=amount_xdai,
             from_private_key=keys.bet_from_private_key,
             market=self,
             binary_outcome=outcome,
             auto_deposit=omen_auto_deposit,
         )
 
-    def redeem_positions(self, from_private_key: PrivateKey) -> None:
+    def was_bet_outcome_correct(self, resolved_omen_bets: t.List[OmenBet]) -> bool:
+        resolved_bets_for_market = [
+            bet for bet in resolved_omen_bets if bet.fpmm.id == self.id
+        ]
+
+        # If there were no bets for this market, we conservatively say that
+        # this method was called incorrectly, hence we raise an Error.
+        if not resolved_bets_for_market:
+            raise ValueError(f"No resolved bets provided for market {self.id}")
+
+        # We iterate through bets since agent could have placed bets on multiple outcomes.
+        # If one of the bets was correct, we return true since there is a redeemable amount to be retrieved.
+        for bet in resolved_bets_for_market:
+            # We only handle markets that are already finalized AND have a final answer
+            if (
+                bet.fpmm.question.answerFinalizedTimestamp is None
+                or bet.fpmm.question.currentAnswer is None
+            ):
+                continue
+
+            # Like Olas, we assert correctness by matching index OR invalid market answer
+            if bet.outcomeIndex == int(
+                bet.fpmm.question.currentAnswer, 16
+            ) or bet.outcomeIndex == int(self.INVALID_MARKET_ANSWER, 16):
+                return True
+
+        return False
+
+    def check_if_position_was_already_redeemed(self) -> bool:
+        """
+        Olas solves this problem (see https://github.com/valory-xyz/trader/blob/033ad88998fe0dc16457cd312b32f9e3b2d9a25f/packages/valory/skills/decision_maker_abci/behaviours/reedem.py#L487) by keeping state of the conditionIDs that were already claimed.
+        Since we currently use stateless functions to redeem positions, it's not possible to query state. Hence we proceed by not tracking the positions already redeemed.
+        Note that this has no major consequences from a gas perspective, it only incurs extra subgraph queries and RPC reads, no writes hence no gas costs.
+        """
+        return False
+
+    def redeem_positions(self, bets_on_market: t.List[OmenBet]) -> None:
+        keys = APIKeys()
+
+        bet_was_correct = self.was_bet_outcome_correct(bets_on_market)
+        if not bet_was_correct:
+            logger.debug(f"Bet placed on market {self.id} was incorrect.")
+            return None
+
+        position_already_redeemed = self.check_if_position_was_already_redeemed()
+        if position_already_redeemed:
+            logger.debug(f"Position on market {self.id} was already redeemed.")
+            return None
+
         return omen_redeem_full_position_tx(
-            market=self,
-            from_private_key=from_private_key,
+            market=self, from_private_key=keys.bet_from_private_key
         )
 
     @staticmethod
     def from_data_model(model: OmenMarket) -> "OmenAgentMarket":
         return OmenAgentMarket(
             id=model.id,
             question=model.title,
+            creator=model.creator,
             outcomes=model.outcomes,
             collateral_token_contract_address_checksummed=model.collateral_token_contract_address_checksummed,
             market_maker_contract_address_checksummed=model.market_maker_contract_address_checksummed,
             resolution=model.get_resolution_enum(),
             created_time=model.creation_datetime,
             close_time=model.finalized_datetime,
             p_yes=model.p_yes,
@@ -134,195 +184,60 @@
 
     def get_contract(self) -> OmenFixedProductMarketMakerContract:
         return OmenFixedProductMarketMakerContract(
             address=self.market_maker_contract_address_checksummed
         )
 
 
-_QUERY_GET_SINGLE_FIXED_PRODUCT_MARKET_MAKER = """
-query getFixedProductMarketMaker($id: String!) {
-    fixedProductMarketMaker(
-        id: $id
-    ) {
-        id
-        title
-        category
-        creationTimestamp
-        collateralVolume
-        usdVolume
-        collateralToken
-        outcomes
-        outcomeTokenAmounts
-        outcomeTokenMarginalPrices
-        fee
-        condition {
-            id
-            outcomeSlotCount
-        }
-        answerFinalizedTimestamp
-        resolutionTimestamp
-        currentAnswer
-    }
-}
-"""
-
-
-def construct_query_get_fixed_product_markets_makers(
-    include_creator: bool, filter_by: FilterBy
-) -> str:
-    query = """
-        query getFixedProductMarketMakers(
-            $first: Int!,
-            $outcomes: [String!],
-            $orderBy: String!,
-            $orderDirection: String!,
-            $creationTimestamp_gt: Int!,
-            $creator: Bytes = null,
-        ) {
-            fixedProductMarketMakers(
-                where: {
-                    isPendingArbitration: false,
-                    outcomes: $outcomes
-                    creationTimestamp_gt: $creationTimestamp_gt
-                    creator: $creator,
-                    answerFinalizedTimestamp: null
-                    resolutionTimestamp_not: null
-                },
-                orderBy: creationTimestamp,
-                orderDirection: desc,
-                first: $first
-            ) {
-                id
-                title
-                collateralVolume
-                usdVolume
-                collateralToken
-                outcomes
-                outcomeTokenAmounts
-                outcomeTokenMarginalPrices
-                fee
-                answerFinalizedTimestamp
-                resolutionTimestamp
-                currentAnswer
-                creationTimestamp
-                category
-                condition {
-                    id
-                    outcomeSlotCount
-                }
-            }
-        }
-    """
-
-    if filter_by == FilterBy.OPEN:
-        query = query.replace("resolutionTimestamp_not: null", "")
-    elif filter_by == FilterBy.RESOLVED:
-        query = query.replace("answerFinalizedTimestamp: null", "")
-    elif filter_by == FilterBy.NONE:
-        query = query.replace("answerFinalizedTimestamp: null", "")
-        query = query.replace("resolutionTimestamp_not: null", "")
-    else:
-        raise ValueError(f"Unknown filter_by: {filter_by}")
-
-    if not include_creator:
-        # If we aren't filtering by query, we need to remove it from where, otherwise "creator: null" will return 0 results.
-        query = query.replace("creator: $creator,", "")
-
-    return query
-
-
 def ordering_from_sort_by(sort_by: SortBy) -> tuple[str, str]:
     """
     Returns 'orderBy' and 'orderDirection' strings for the given SortBy.
     """
     if sort_by == SortBy.CLOSING_SOONEST:
         return "creationTimestamp", "desc"  # TODO make more accurate
     elif sort_by == SortBy.NEWEST:
         return "creationTimestamp", "desc"
     else:
         raise ValueError(f"Unknown sort_by: {sort_by}")
 
 
-def get_omen_markets(
-    first: int,
-    outcomes: list[str],
-    sort_by: SortBy,
-    filter_by: FilterBy,
-    created_after: t.Optional[datetime] = None,
-    creator: t.Optional[HexAddress] = None,
-    excluded_questions: set[str] | None = None,
-) -> list[OmenMarket]:
-    order_by, order_direction = ordering_from_sort_by(sort_by)
-    markets = response_to_model(
-        requests.post(
-            THEGRAPH_QUERY_URL,
-            json={
-                "query": construct_query_get_fixed_product_markets_makers(
-                    include_creator=creator is not None,
-                    filter_by=filter_by,
-                ),
-                "variables": {
-                    "first": first,
-                    "outcomes": outcomes,
-                    "orderBy": order_by,
-                    "orderDirection": order_direction,
-                    "creationTimestamp_gt": (
-                        to_int_timestamp(created_after) if created_after else 0
-                    ),
-                    "creator": creator,
-                },
-            },
-            headers={"Content-Type": "application/json"},
-        ),
-        FixedProductMarketMakersResponse,
-    )
-    return [
-        m
-        for m in markets.data.fixedProductMarketMakers
-        if not excluded_questions or m.question not in excluded_questions
-    ]
-
-
 def get_omen_binary_markets(
-    limit: int,
+    limit: int | None,
     sort_by: SortBy,
     filter_by: FilterBy = FilterBy.OPEN,
     created_after: t.Optional[datetime] = None,
+    opened_before: t.Optional[datetime] = None,
+    finalized_before: t.Optional[datetime] = None,
+    finalized: bool | None = None,
+    resolved: bool | None = None,
     creator: t.Optional[HexAddress] = None,
     excluded_questions: set[str] | None = None,
 ) -> list[OmenMarket]:
-    return get_omen_markets(
-        first=limit,
-        outcomes=[OMEN_TRUE_OUTCOME, OMEN_FALSE_OUTCOME],
+    subgraph_handler = OmenSubgraphHandler()
+    return subgraph_handler.get_omen_binary_markets(
+        limit=limit,
         sort_by=sort_by,
         created_after=created_after,
+        opened_before=opened_before,
+        finalized_before=finalized_before,
+        finalized=finalized,
+        resolved=resolved,
         filter_by=filter_by,
         creator=creator,
         excluded_questions=excluded_questions,
     )
 
 
 def pick_binary_market(
     sort_by: SortBy = SortBy.CLOSING_SOONEST, filter_by: FilterBy = FilterBy.OPEN
 ) -> OmenMarket:
-    return get_omen_binary_markets(limit=1, sort_by=sort_by, filter_by=filter_by)[0]
-
-
-def get_market(market_id: str) -> OmenMarket:
-    market = requests.post(
-        THEGRAPH_QUERY_URL,
-        json={
-            "query": _QUERY_GET_SINGLE_FIXED_PRODUCT_MARKET_MAKER,
-            "variables": {
-                "id": market_id,
-            },
-        },
-        headers={"Content-Type": "application/json"},
-    ).json()["data"]["fixedProductMarketMaker"]
-    return OmenMarket.model_validate(market)
+    subgraph_handler = OmenSubgraphHandler()
+    return subgraph_handler.get_omen_binary_markets(
+        limit=1, sort_by=sort_by, filter_by=filter_by
+    )[0]
 
 
 def omen_buy_outcome_tx(
     amount: xDai,
     from_private_key: PrivateKey,
     market: OmenAgentMarket,
     outcome: str,
@@ -450,136 +365,14 @@
         from_private_key=from_private_key,
         market=market,
         outcome=OMEN_TRUE_OUTCOME if binary_outcome else OMEN_FALSE_OUTCOME,
         auto_withdraw=auto_withdraw,
     )
 
 
-# Order by id, so we can use id_gt for pagination.
-_QUERY_GET_FIXED_PRODUCT_MARKETS_MAKER_TRADES = """
-query getFixedProductMarketMakerTrades(
-    $id_gt: String!,
-    $creator: String!,
-    $creationTimestamp_gte: Int!,
-    $creationTimestamp_lte: Int!,
-    $first: Int!,
-) {
-    fpmmTrades(
-        where: {
-            type: Buy,
-            creator: $creator,
-            creationTimestamp_gte: $creationTimestamp_gte,
-            creationTimestamp_lte: $creationTimestamp_lte,
-            id_gt: $id_gt,
-        }
-        first: $first
-        orderBy: id
-        orderDirection: asc
-    ) {
-        id
-        title
-        collateralToken
-        outcomeTokenMarginalPrice
-        oldOutcomeTokenMarginalPrice
-        type
-        creator {
-            id
-        }
-        creationTimestamp
-        collateralAmount
-        collateralAmountUSD
-        feeAmount
-        outcomeIndex
-        outcomeTokensTraded
-        transactionHash
-        fpmm {
-            id
-            outcomes
-            title
-            answerFinalizedTimestamp
-            resolutionTimestamp
-            currentAnswer
-            isPendingArbitration
-            arbitrationOccurred
-            openingTimestamp
-            condition {
-                id
-                outcomeSlotCount
-            }
-            collateralVolume
-            usdVolume
-            collateralToken
-            outcomeTokenAmounts
-            outcomeTokenMarginalPrices
-            fee
-            category
-        }
-    }
-}
-"""
-
-
-def to_int_timestamp(dt: datetime) -> int:
-    return int(dt.timestamp())
-
-
-def get_omen_bets(
-    better_address: ChecksumAddress,
-    start_time: datetime,
-    end_time: t.Optional[datetime],
-) -> list[OmenBet]:
-    if not end_time:
-        end_time = utcnow()
-
-    # Initialize id_gt for the first batch of bets to zero
-    id_gt: str = "0"
-    all_bets: list[OmenBet] = []
-    while True:
-        query = _QUERY_GET_FIXED_PRODUCT_MARKETS_MAKER_TRADES
-        bets = requests.post(
-            THEGRAPH_QUERY_URL,
-            json={
-                "query": query,
-                "variables": {
-                    "creator": better_address.lower(),
-                    "creationTimestamp_gte": to_int_timestamp(start_time),
-                    "creationTimestamp_lte": to_int_timestamp(end_time),
-                    "id_gt": id_gt,
-                    "first": OMEN_QUERY_BATCH_SIZE,
-                },
-            },
-            headers={"Content-Type": "application/json"},
-        ).json()
-
-        bets = bets.get("data", {}).get("fpmmTrades", [])
-
-        if not bets:
-            break
-
-        # Increment id_gt for the next batch of bets
-        id_gt = bets[-1]["id"]
-
-        all_bets.extend(OmenBet.model_validate(bet) for bet in bets)
-
-    return all_bets
-
-
-def get_resolved_omen_bets(
-    better_address: ChecksumAddress,
-    start_time: datetime,
-    end_time: t.Optional[datetime],
-) -> list[OmenBet]:
-    bets = get_omen_bets(
-        better_address=better_address,
-        start_time=start_time,
-        end_time=end_time,
-    )
-    return [b for b in bets if b.fpmm.is_resolved]
-
-
 def omen_create_market_tx(
     initial_funds: xDai,
     question: str,
     closing_time: datetime,
     category: str,
     language: str,
     from_private_key: PrivateKey,
@@ -672,147 +465,190 @@
         "address"
     ]  # The market address is available in the last emitted log, in the address field.
     return market_address
 
 
 def omen_fund_market_tx(
     market: OmenAgentMarket,
-    funds: xDai,
+    funds: Wei,
     from_private_key: PrivateKey,
     auto_deposit: bool,
 ) -> None:
-    funds_wei = xdai_to_wei(funds)
     from_address = private_key_to_public_key(from_private_key)
     market_contract = market.get_contract()
     collateral_token_contract = OmenCollateralTokenContract()
 
     # Deposit xDai to the collateral token,
     # this can be skipped, if we know we already have enough collateral tokens.
     if (
         auto_deposit
         and collateral_token_contract.balanceOf(
             for_address=from_address,
         )
-        < funds_wei
+        < funds
     ):
-        collateral_token_contract.deposit(funds_wei, from_private_key)
+        collateral_token_contract.deposit(funds, from_private_key)
 
     collateral_token_contract.approve(
         for_address=market_contract.address,
-        amount_wei=funds_wei,
+        amount_wei=funds,
         from_private_key=from_private_key,
     )
 
-    market_contract.addFunding(funds_wei, from_private_key)
+    market_contract.addFunding(funds, from_private_key)
 
 
 def build_parent_collection_id() -> HexStr:
     return HASH_ZERO  # Taken from Olas
 
 
 def omen_redeem_full_position_tx(
     market: OmenAgentMarket,
     from_private_key: PrivateKey,
     web3: Web3 | None = None,
-    unwrap_collateral_after_redeeming_positions: bool = True,
 ) -> None:
     """
-    Redeems position from a given Omen market.
+    Redeems position from a given Omen market. Note that we check if there is a balance
+    to be redeemed before sending the transaction.
     """
+
     from_address = private_key_to_public_key(from_private_key)
 
     market_contract: OmenFixedProductMarketMakerContract = market.get_contract()
     conditional_token_contract = OmenConditionalTokenContract()
 
     # Verify, that markets uses conditional tokens that we expect.
     if market_contract.conditionalTokens() != conditional_token_contract.address:
         raise ValueError(
             f"Market {market.id} uses conditional token that we didn't expect, {market_contract.conditionalTokens()} != {conditional_token_contract.address=}"
         )
 
     parent_collection_id = build_parent_collection_id()
 
     if not market.is_resolved():
-        print("Cannot redeem winnings if market is not yet resolved. Exiting.")
+        logger.debug("Cannot redeem winnings if market is not yet resolved. Exiting.")
         return
 
     amount_wei = get_conditional_tokens_balance_for_market(market, from_address, web3)
     if amount_wei == 0:
-        print("No balance to claim. Exiting.")
+        logger.debug("No balance to claim. Exiting.")
+        return
+
+    # check if condition has already been resolved by oracle
+    payout_for_condition = conditional_token_contract.payoutDenominator(
+        market.condition.id
+    )
+    if not payout_for_condition > 0:
+        # from ConditionalTokens.redeemPositions:
+        # uint den = payoutDenominator[conditionId]; require(den > 0, "result for condition not received yet");
+        logger.debug("Market not yet resolved, not possible to claim")
         return
 
-    conditional_token_contract = OmenConditionalTokenContract()
     conditional_token_contract.redeemPositions(
         from_private_key=from_private_key,
         collateral_token_address=market.collateral_token_contract_address_checksummed,
         condition_id=market.condition.id,
         parent_collection_id=parent_collection_id,
         index_sets=market.condition.index_sets,
         web3=web3,
     )
 
-    if unwrap_collateral_after_redeeming_positions:
-        withdraw_collateral_token(
-            amount_wei=amount_wei,
-            from_private_key=from_private_key,
-            web3=web3,
-        )
-
 
 def get_conditional_tokens_balance_for_market(
     market: OmenAgentMarket,
     from_address: ChecksumAddress,
     web3: Web3 | None = None,
 ) -> Wei:
     """
     We derive the withdrawable balance from the ConditionalTokens contract through CollectionId -> PositionId (which
     also serves as tokenId) -> TokenBalances.
     """
     conditional_token_contract = OmenConditionalTokenContract()
     parent_collection_id = build_parent_collection_id()
-    balance = 0
+    balance = wei_type(0)
 
     for index_set in market.condition.index_sets:
-        collection_id: bytes = conditional_token_contract.call(
-            "getCollectionId",
-            [parent_collection_id, market.condition.id, index_set],
-            web3=web3,
+        collection_id = conditional_token_contract.getCollectionId(
+            parent_collection_id, market.condition.id, index_set, web3=web3
         )
         # Note that collection_id is returned as bytes, which is accepted by the contract calls downstream.
-        position_id: int = conditional_token_contract.call(
-            "getPositionId",
-            [market.collateral_token_contract_address_checksummed, collection_id],
+        position_id: int = conditional_token_contract.getPositionId(
+            market.collateral_token_contract_address_checksummed,
+            collection_id,
             web3=web3,
         )
-        balance_for_position: int = conditional_token_contract.call(
-            "balanceOf", [from_address, position_id], web3=web3
+        balance_for_position = conditional_token_contract.balanceOf(
+            from_address=from_address, position_id=position_id, web3=web3
         )
-        balance += balance_for_position
+        balance = wei_type(balance + balance_for_position)
 
-    return Wei(balance)
+    return balance
 
 
-def withdraw_collateral_token(
-    amount_wei: Wei,
+def omen_remove_fund_market_tx(
+    market: OmenAgentMarket,
+    shares: Wei | None,
     from_private_key: PrivateKey,
     web3: Web3 | None = None,
-) -> TxReceipt:
-    collateral_token = OmenCollateralTokenContract()
-    return collateral_token.withdraw(
-        amount_wei=amount_wei,
+) -> None:
+    """
+    Removes funding from a given OmenMarket (moving the funds from the OmenMarket to the
+    ConditionalTokens contract), and finally calls the `mergePositions` method which transfers collateralToken from the ConditionalTokens contract to the address corresponding to `from_private_key`.
+    """
+    from_address = private_key_to_public_key(from_private_key)
+    market_contract = market.get_contract()
+
+    total_shares = market_contract.balanceOf(from_address, web3=web3)
+    if total_shares == 0:
+        logger.info("No shares to remove.")
+        return
+
+    if shares is None or shares > total_shares:
+        logger.debug(
+            f"shares available to claim {total_shares} - defaulting to a total removal."
+        )
+        shares = total_shares
+
+    market_contract.removeFunding(
+        remove_funding=shares, from_private_key=from_private_key, web3=web3
+    )
+
+    conditional_tokens = OmenConditionalTokenContract()
+    parent_collection_id = build_parent_collection_id()
+    result = conditional_tokens.mergePositions(
         from_private_key=from_private_key,
+        collateral_token_address=market.collateral_token_contract_address_checksummed,
+        parent_collection_id=parent_collection_id,
+        conditionId=market.condition.id,
+        index_sets=market.condition.index_sets,
+        amount=shares,
         web3=web3,
     )
+    logger.debug(f"Result from merge positions {result}")
 
 
-def omen_remove_fund_market_tx(
-    market: OmenAgentMarket,
-    shares: OmenOutcomeToken,
-    from_private_key: PrivateKey,
-    auto_withdraw: bool,
-) -> None:
-    market_contract = market.get_contract()
-    market_contract.removeFunding(shares, from_private_key)
+def redeem_positions_from_all_omen_markets() -> None:
+    """
+    Redeems positions from all resolved Omen markets.
+    """
+    keys = APIKeys()
+    omen_subgraph_handler = OmenSubgraphHandler()
+    resolved_omen_bets = omen_subgraph_handler.get_resolved_bets(
+        better_address=keys.bet_from_address,
+        start_time=datetime(2020, 1, 1),
+    )
 
-    # TODO: How to withdraw remove funding back to our wallet.
-    if auto_withdraw:
-        raise NotImplementedError("TODO")
+    bets_per_market_id: t.Dict[HexAddress, t.List[OmenBet]] = defaultdict(list)
+    market_id_to_market: t.Dict[HexAddress, OmenMarket] = {}
+
+    for bet in resolved_omen_bets:
+        bets_per_market_id[bet.fpmm.id].append(bet)
+        # We keep track of the unique markets
+        if bet.fpmm.id not in market_id_to_market:
+            market_id_to_market[bet.fpmm.id] = bet.fpmm
+
+    # We redeem positions for each unique resolved market where the
+    # agent has placed bets.
+    for market_id, omen_bets in bets_per_market_id.items():
+        market_data_model = market_id_to_market[market_id]
+        market = OmenAgentMarket.from_data_model(market_data_model)
+        market.redeem_positions(omen_bets)
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/omen/omen_contracts.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/omen/omen_contracts.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 from web3 import Web3
 
 from prediction_market_agent_tooling.gtypes import (
     ABI,
     ChecksumAddress,
     HexAddress,
     HexBytes,
+    HexStr,
     OmenOutcomeToken,
     PrivateKey,
     TxParams,
     TxReceipt,
     Wei,
+    int_to_hexbytes,
+    wei_type,
     xdai_type,
 )
 from prediction_market_agent_tooling.tools.contract import (
     ContractERC20OnGnosisChain,
     ContractOnGnosisChain,
     abi_field_validator,
 )
@@ -42,14 +45,33 @@
         realitio_address: ChecksumAddress = self.call("realitio")
         return realitio_address
 
     def conditionalTokens(self) -> ChecksumAddress:
         realitio_address: ChecksumAddress = self.call("conditionalTokens")
         return realitio_address
 
+    def resolve(
+        self,
+        question_id: HexBytes,
+        template_id: int,
+        question_raw: str,
+        n_outcomes: int,
+        from_private_key: PrivateKey,
+    ) -> TxReceipt:
+        return self.send(
+            from_private_key=from_private_key,
+            function_name="resolve",
+            function_params=dict(
+                questionId=question_id,
+                templateId=template_id,
+                question=question_raw,
+                numOutcomes=n_outcomes,
+            ),
+        )
+
 
 class OmenConditionalTokenContract(ContractOnGnosisChain):
     # Contract ABI taken from https://gnosisscan.io/address/0xCeAfDD6bc0bEF976fdCd1112955828E00543c0Ce#code.
     abi: ABI = abi_field_validator(
         os.path.join(
             os.path.dirname(os.path.realpath(__file__)),
             "../../abis/omen_fpmm_conditionaltokens.abi.json",
@@ -61,26 +83,88 @@
 
     def getConditionId(
         self,
         question_id: HexBytes,
         oracle_address: ChecksumAddress,
         outcomes_slot_count: int,
     ) -> HexBytes:
-        id_: HexBytes = self.call(
-            "getConditionId",
-            [oracle_address, question_id, outcomes_slot_count],
+        id_ = HexBytes(
+            self.call(
+                "getConditionId",
+                [oracle_address, question_id, outcomes_slot_count],
+            )
         )
         return id_
 
+    def balanceOf(
+        self, from_address: ChecksumAddress, position_id: int, web3: Web3 | None = None
+    ) -> Wei:
+        balance = wei_type(
+            self.call("balanceOf", [from_address, position_id], web3=web3)
+        )
+        return balance
+
+    def getCollectionId(
+        self,
+        parent_collection_id: HexStr,
+        condition_id: HexBytes,
+        index_set: int,
+        web3: Web3 | None = None,
+    ) -> HexBytes:
+        collection_id = HexBytes(
+            self.call(
+                "getCollectionId",
+                [parent_collection_id, condition_id, index_set],
+                web3=web3,
+            )
+        )
+        return collection_id
+
+    def getPositionId(
+        self,
+        collateral_token_address: ChecksumAddress,
+        collection_id: HexBytes,
+        web3: Web3 | None = None,
+    ) -> int:
+        position_id: int = self.call(
+            "getPositionId",
+            [collateral_token_address, collection_id],
+            web3=web3,
+        )
+        return position_id
+
+    def mergePositions(
+        self,
+        from_private_key: PrivateKey,
+        collateral_token_address: ChecksumAddress,
+        parent_collection_id: HexStr,
+        conditionId: HexBytes,
+        index_sets: t.List[int],
+        amount: Wei,
+        web3: Web3 | None = None,
+    ) -> TxReceipt:
+        return self.send(
+            from_private_key=from_private_key,
+            function_name="mergePositions",
+            function_params=[
+                collateral_token_address,
+                parent_collection_id,
+                conditionId,
+                index_sets,
+                amount,
+            ],
+            web3=web3,
+        )
+
     def redeemPositions(
         self,
         from_private_key: PrivateKey,
-        collateral_token_address: str,
-        condition_id: str,
-        parent_collection_id: str,
+        collateral_token_address: HexAddress,
+        condition_id: HexBytes,
+        parent_collection_id: HexStr,
         index_sets: t.List[int],
         web3: Web3 | None = None,
     ) -> TxReceipt:
         return self.send(
             from_private_key=from_private_key,
             function_name="redeemPositions",
             function_params=[
@@ -104,14 +188,21 @@
 
     def does_condition_exists(
         self,
         condition_id: HexBytes,
     ) -> bool:
         return self.getOutcomeSlotCount(condition_id) > 0
 
+    def payoutDenominator(self, condition_id: HexBytes) -> int:
+        payoutForCondition: int = self.call(
+            "payoutDenominator",
+            [condition_id],
+        )
+        return payoutForCondition
+
     def setApprovalForAll(
         self,
         for_address: ChecksumAddress,
         approve: bool,
         from_private_key: PrivateKey,
         tx_params: t.Optional[TxParams] = None,
     ) -> TxReceipt:
@@ -152,14 +243,18 @@
             os.path.dirname(os.path.realpath(__file__)), "../../abis/omen_fpmm.abi.json"
         )
     )
 
     # ! Note: This doesn't have a fixed contract address, as this is something created by the `OmenFixedProductMarketMakerFactory`.
     # Factory contract at https://gnosisscan.io/address/0x9083a2b699c0a4ad06f63580bde2635d26a3eef0.
 
+    def balanceOf(self, for_address: ChecksumAddress, web3: Web3 | None = None) -> Wei:
+        balance: Wei = self.call("balanceOf", [for_address], web3=web3)
+        return balance
+
     def calcBuyAmount(
         self,
         investment_amount: Wei,
         outcome_index: int,
     ) -> OmenOutcomeToken:
         """
         Returns amount of shares we will get for the given outcome_index for the given investment amount.
@@ -246,26 +341,28 @@
             function_name="addFunding",
             function_params=[add_funding, distribution_hint],
             tx_params=tx_params,
         )
 
     def removeFunding(
         self,
-        remove_funding: OmenOutcomeToken,
+        remove_funding: Wei,
         from_private_key: PrivateKey,
         tx_params: t.Optional[TxParams] = None,
+        web3: Web3 | None = None,
     ) -> TxReceipt:
         """
         Remove funding is done in shares.
         """
         return self.send(
             from_private_key=from_private_key,
             function_name="removeFunding",
             function_params=[remove_funding],
             tx_params=tx_params,
+            web3=web3,
         )
 
 
 class WrappedxDaiContract(ContractERC20OnGnosisChain):
     # File content taken from https://gnosisscan.io/address/0xe91d153e0b41518a2ce8dd3d7944fa863463a97d#code.
     abi: ABI = abi_field_validator(
         os.path.join(
@@ -415,11 +512,75 @@
                 opening_ts=int(opening.timestamp()),
                 nonce=(
                     nonce if nonce is not None else random.randint(0, 1000000)
                 ),  # Two equal questions need to have different nonces.
             ),
             tx_params=tx_params,
         )
-        question_id: HexBytes = receipt_tx["logs"][0]["topics"][
-            1
-        ]  # The question id is available in the first emitted log, in the second topic.
+        question_id = HexBytes(
+            receipt_tx["logs"][0]["topics"][1]
+        )  # The question id is available in the first emitted log, in the second topic.
         return question_id
+
+    def submitAnswer(
+        self,
+        question_id: HexBytes,
+        answer: str,
+        outcomes: list[str],
+        bond: Wei,
+        from_private_key: PrivateKey,
+        max_previous: Wei | None = None,
+    ) -> TxReceipt:
+        if max_previous is None:
+            # If not provided, defaults to 0, which means no checking,
+            # same as on Omen website: https://github.com/protofire/omen-exchange/blob/763d9c9d05ebf9edacbc1dbaa561aa5d08813c0f/app/src/services/realitio.ts#L363.
+            max_previous = Wei(0)
+
+        # Normalise the answer to lowercase, to match Enum values as [YES, NO] against outcomes as ["Yes", "No"].
+        answer = answer.lower()
+        outcomes = [o.lower() for o in outcomes]
+
+        return self.send_with_value(
+            from_private_key=from_private_key,
+            function_name="submitAnswer",
+            function_params=dict(
+                question_id=question_id,
+                answer=int_to_hexbytes(
+                    outcomes.index(answer)
+                ),  # Contract's method expects answer index in bytes.
+                max_previous=max_previous,
+            ),
+            amount_wei=bond,
+        )
+
+    def claimWinnings(
+        self,
+        question_id: HexBytes,
+        history_hashes: list[HexBytes],
+        addresses: list[ChecksumAddress],
+        bonds: list[Wei],
+        answers: list[HexBytes],
+        from_private_key: PrivateKey,
+        tx_params: t.Optional[TxParams] = None,
+    ) -> TxReceipt:
+        return self.send(
+            function_name="claimWinnings",
+            function_params=dict(
+                question_id=question_id,
+                history_hashes=history_hashes,
+                addrs=addresses,
+                bonds=bonds,
+                answers=answers,
+            ),
+            from_private_key=from_private_key,
+            tx_params=tx_params,
+        )
+
+    def balanceOf(self, from_address: ChecksumAddress) -> Wei:
+        balance = wei_type(self.call("balanceOf", [from_address]))
+        return balance
+
+    def withdraw(self, from_private_key: PrivateKey) -> TxReceipt:
+        return self.send(
+            function_name="withdraw",
+            from_private_key=from_private_key,
+        )
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/omen/omen_replicate.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/omen/omen_replicate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from datetime import datetime, timedelta
 
+from loguru import logger
+
 from prediction_market_agent_tooling.gtypes import ChecksumAddress, PrivateKey, xDai
 from prediction_market_agent_tooling.markets.agent_market import FilterBy, SortBy
 from prediction_market_agent_tooling.markets.categorize import infer_category
 from prediction_market_agent_tooling.markets.markets import (
     MarketType,
     get_binary_markets,
 )
@@ -12,15 +14,15 @@
     OMEN_TRUE_OUTCOME,
 )
 from prediction_market_agent_tooling.markets.omen.omen import (
     OMEN_DEFAULT_MARKET_FEE,
     get_omen_binary_markets,
     omen_create_market_tx,
 )
-from prediction_market_agent_tooling.tools.is_predictable import is_predictable
+from prediction_market_agent_tooling.tools.is_predictable import is_predictable_binary
 from prediction_market_agent_tooling.tools.utils import utcnow
 from prediction_market_agent_tooling.tools.web3_utils import private_key_to_public_key
 
 
 def omen_replicate_from_tx(
     market_type: MarketType,
     n_to_replicate: int,
@@ -44,37 +46,33 @@
         )
 
     markets = get_binary_markets(
         # Polymarket is slow to get, so take only 10 candidates for him.
         10 if market_type == MarketType.POLYMARKET else 100,
         market_type,
         filter_by=FilterBy.OPEN,
-        sort_by=(
-            SortBy.CLOSING_SOONEST
-            if market_type == MarketType.MANIFOLD
-            else SortBy.NONE
-        ),
-        excluded_questions=set(m.question for m in already_created_markets),
+        sort_by=SortBy.NONE,
+        excluded_questions=set(m.question_title for m in already_created_markets),
     )
     markets_sorted = sorted(
         markets,
         key=lambda m: m.volume or 0,
         reverse=True,
     )
     markets_to_replicate = [
         m
         for m in markets_sorted
         if close_time_before is None
         or (m.close_time is not None and m.close_time <= close_time_before)
     ]
     if not markets_to_replicate:
-        print(f"No markets found for {market_type}")
+        logger.info(f"No markets found for {market_type}")
         return []
 
-    print(f"Found {len(markets_to_replicate)} markets to replicate.")
+    logger.info(f"Found {len(markets_to_replicate)} markets to replicate.")
 
     # Get a set of possible categories from existing markets (but created by anyone, not just your agent)
     existing_categories = set(
         m.category
         for m in get_omen_binary_markets(
             limit=last_n_omen_markets_to_fetch,
             sort_by=SortBy.NEWEST,
@@ -82,49 +80,61 @@
         )
     )
 
     created_addresses: list[ChecksumAddress] = []
 
     for market in markets_to_replicate:
         if market.close_time is None:
-            print(
+            logger.info(
                 f"Skipping `{market.question}` because it's missing the closing time."
             )
             continue
-        if not is_predictable(market.question):
-            print(
-                f"Skipping `{market.question}` because it seems to not be predictable."
-            )
-            continue
 
         # According to Omen's recommendation, closing time of the market should be at least 6 days after the outcome is known.
         # That is because at the closing time, the question will open on Realitio, and we don't want it to be resolved as unknown/invalid.
         safe_closing_time = market.close_time + timedelta(days=6)
         # Force at least 48 hours of time where the resolution is unknown.
         soonest_allowed_resolution_known_time = utcnow() + timedelta(hours=48)
         if market.close_time <= soonest_allowed_resolution_known_time:
-            print(
+            logger.info(
                 f"Skipping `{market.question}` because it closes sooner than {soonest_allowed_resolution_known_time}."
             )
             continue
+
+        # Do as the last step, becuase it calls OpenAI (costly & slow).
+        if not is_predictable_binary(market.question):
+            logger.info(
+                f"Skipping `{market.question}` because it seems to not be predictable."
+            )
+            continue
+
         category = infer_category(market.question, existing_categories)
+        # Realitio will allow new categories or misformated categories, so double check that the LLM got it right.
+        if category not in existing_categories:
+            logger.info(
+                f"Error: LLM went rouge. Skipping `{market.question}` because the category `{category}` is not in the existing categories {existing_categories}."
+            )
+            continue
+
         market_address = omen_create_market_tx(
             initial_funds=initial_funds,
             fee=OMEN_DEFAULT_MARKET_FEE,
             question=market.question,
             closing_time=safe_closing_time,
             category=category,
             language="en",
             from_private_key=from_private_key,
             outcomes=[OMEN_TRUE_OUTCOME, OMEN_FALSE_OUTCOME],
             auto_deposit=auto_deposit,
         )
         created_addresses.append(market_address)
-        print(
+        logger.info(
             f"Created `https://aiomen.eth.limo/#/{market_address}` for `{market.question}` in category {category} out of {market.url}."
         )
 
         if len(created_addresses) >= n_to_replicate:
-            print(f"Replicated {len(created_addresses)} from {market_type}, breaking.")
+            logger.info(
+                f"Replicated {len(created_addresses)} from {market_type}, breaking."
+            )
             break
 
     return created_addresses
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/polymarket/api.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/polymarket/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 POLYMARKET_FALSE_OUTCOME,
                 POLYMARKET_TRUE_OUTCOME,
             ]:
                 continue
 
             # This is pretty slow to do here, but our safest option at the moment. So keep it as the last filter.
             # TODO: Add support for `description` for `AgentMarket` and if it isn't None, use it in addition to the question in all agents. Then this can be removed.
-            if main_markets_only and not market.check_if_its_a_main_market():
+            if main_markets_only and not market.fetch_if_its_a_main_market():
                 continue
 
             tokens_with_price = get_market_tokens_with_prices(market)
             market_with_prices = PolymarketMarketWithPrices.model_validate(
                 {**market.model_dump(), "tokens": tokens_with_price}
             )
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/polymarket/data_models.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/polymarket/data_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from datetime import datetime
 
-import requests
 from pydantic import BaseModel
 
 from prediction_market_agent_tooling.gtypes import USDC, Probability, usdc_type
 from prediction_market_agent_tooling.markets.data_models import Resolution
-
-POLYMARKET_TRUE_OUTCOME = "Yes"
-POLYMARKET_FALSE_OUTCOME = "No"
+from prediction_market_agent_tooling.markets.polymarket.data_models_web import (
+    POLYMARKET_FALSE_OUTCOME,
+    POLYMARKET_TRUE_OUTCOME,
+    PolymarketFullMarket,
+    construct_polymarket_url,
+)
 
 
 class PolymarketRewards(BaseModel):
     min_size: int
     max_spread: float
     event_start_date: datetime | None
     event_end_date: datetime | None
@@ -58,18 +60,15 @@
 
     @property
     def id(self) -> str:
         return self.condition_id
 
     @property
     def url(self) -> str:
-        """
-        Note: This works only if it's a single main market, not sub-market of some more general question.
-        """
-        return f"https://polymarket.com/event/{self.market_slug}"
+        return construct_polymarket_url(self.market_slug)
 
     @property
     def resolution(self) -> Resolution | None:
         winner_tokens = [token for token in self.tokens if token.winner]
         if len(winner_tokens) == 0:
             return None
         elif (
@@ -83,23 +82,26 @@
         ):
             return Resolution.NO
         else:
             raise ValueError(
                 f"Should not happen, invalid winner tokens: {winner_tokens}"
             )
 
-    def check_if_its_a_main_market(self) -> bool:
+    def fetch_full_market(self) -> PolymarketFullMarket | None:
+        return PolymarketFullMarket.fetch_from_url(self.url)
+
+    def fetch_if_its_a_main_market(self) -> bool:
         # On Polymarket, there are markets that are actually a group of multiple Yes/No markets, for example https://polymarket.com/event/presidential-election-winner-2024.
         # But API returns them individually, and then we receive questions such as "Will any other Republican Politician win the 2024 US Presidential Election?",
         # which are naturally unpredictable without futher details.
         # This is a heuristic to filter them out.
-        headers = {
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3"
-        }
-        return self.question in requests.get(self.url, headers=headers).text
+        # Warning: This is a very slow operation, as it requires fetching the website. Use it only when necessary.
+        full_market = self.fetch_full_market()
+        # `full_market` can be None, if this class come from a multiple Yes/No market, becase then, the constructed URL is invalid (and there is now way to construct an valid one from the data we have).
+        return full_market is not None and full_market.is_main_market
 
 
 class MarketsEndpointResponse(BaseModel):
     limit: int
     count: int
     next_cursor: str
     data: list[PolymarketMarket]
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/markets/polymarket/polymarket.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/markets/polymarket/polymarket.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,26 @@
 from prediction_market_agent_tooling.markets.data_models import BetAmount, Currency
 from prediction_market_agent_tooling.markets.polymarket.api import (
     get_polymarket_binary_markets,
 )
 from prediction_market_agent_tooling.markets.polymarket.data_models import (
     PolymarketMarketWithPrices,
 )
+from prediction_market_agent_tooling.markets.polymarket.data_models_web import (
+    POLYMARKET_BASE_URL,
+)
 
 
 class PolymarketAgentMarket(AgentMarket):
     """
     Polymarket's market class that can be used by agents to make predictions.
     """
 
     currency: t.ClassVar[Currency] = Currency.USDC
+    base_url: t.ClassVar[str] = POLYMARKET_BASE_URL
 
     @staticmethod
     def from_data_model(model: PolymarketMarketWithPrices) -> "PolymarketAgentMarket":
         return PolymarketAgentMarket(
             id=model.id,
             question=model.question,
             outcomes=[x.outcome for x in model.tokens],
@@ -45,15 +49,15 @@
     @staticmethod
     def get_binary_markets(
         limit: int,
         sort_by: SortBy = SortBy.NONE,
         filter_by: FilterBy = FilterBy.OPEN,
         created_after: t.Optional[datetime] = None,
         excluded_questions: set[str] | None = None,
-    ) -> list["AgentMarket"]:
+    ) -> list[AgentMarket]:
         if sort_by != SortBy.NONE:
             raise ValueError(f"Unsuported sort_by {sort_by} for Polymarket.")
 
         if created_after is not None:
             raise ValueError(f"Unsuported created_after for Polymarket.")
 
         closed: bool | None
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/monitor/markets/manifold.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/monitor/markets/manifold.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/monitor/markets/omen.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/monitor/markets/omen.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 from web3 import Web3
 
 from prediction_market_agent_tooling.config import APIKeys
 from prediction_market_agent_tooling.deploy.constants import MARKET_TYPE_KEY
 from prediction_market_agent_tooling.gtypes import ChecksumAddress, DatetimeWithTimezone
 from prediction_market_agent_tooling.markets.data_models import ResolvedBet
 from prediction_market_agent_tooling.markets.markets import MarketType
-from prediction_market_agent_tooling.markets.omen.omen import get_resolved_omen_bets
+from prediction_market_agent_tooling.markets.omen.omen_subgraph_handler import (
+    OmenSubgraphHandler,
+)
 from prediction_market_agent_tooling.monitor.monitor import (
     DeployedAgent,
     MonitorSettings,
 )
 
 
 class DeployedOmenAgent(DeployedAgent):
     omen_public_key: ChecksumAddress
 
     def get_resolved_bets(self) -> list[ResolvedBet]:
-        bets = get_resolved_omen_bets(
+        subgraph_handler = OmenSubgraphHandler()
+        bets = subgraph_handler.get_resolved_bets(
             better_address=self.omen_public_key,
             start_time=self.start_time,
             end_time=self.end_time,
         )
         return [b.to_generic_resolved_bet() for b in bets]
 
     @staticmethod
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/monitor/markets/polymarket.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/monitor/markets/polymarket.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/monitor/monitor.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/monitor/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from itertools import groupby
 
 import altair as alt
 import numpy as np
 import pandas as pd
 import streamlit as st
 from google.cloud.functions_v2.types.functions import Function
+from loguru import logger
 from pydantic import BaseModel, field_validator
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
 from prediction_market_agent_tooling.config import APIKeys
 from prediction_market_agent_tooling.deploy.gcp.utils import (
     get_gcp_function,
     list_gcp_functions,
@@ -138,15 +139,17 @@
         for function in list_gcp_functions():
             if not filter_(function):
                 continue
 
             try:
                 agents.append(cls.from_gcp_function(function))
             except ValueError:
-                print(f"Could not parse `{function.name}` into {cls.__name__}.")
+                logger.warning(
+                    f"Could not parse `{function.name}` into {cls.__name__}."
+                )
 
         return agents
 
 
 def monitor_agent(agent: DeployedAgent) -> None:
     agent_bets = agent.get_resolved_bets()
     if not agent_bets:
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/monitor/monitor_app.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/monitor/monitor_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 import streamlit as st
 
 from prediction_market_agent_tooling.markets.agent_market import (
     AgentMarket,
     FilterBy,
     SortBy,
 )
-from prediction_market_agent_tooling.markets.markets import (
-    MARKET_TYPE_TO_AGENT_MARKET,
-    MarketType,
-)
+from prediction_market_agent_tooling.markets.markets import MarketType
 from prediction_market_agent_tooling.monitor.markets.manifold import (
     DeployedManifoldAgent,
 )
 from prediction_market_agent_tooling.monitor.markets.omen import DeployedOmenAgent
 from prediction_market_agent_tooling.monitor.markets.polymarket import (
     DeployedPolymarketAgent,
 )
@@ -63,16 +60,15 @@
     return agents
 
 
 def get_open_and_resolved_markets(
     start_time: datetime,
     market_type: MarketType,
 ) -> tuple[list[AgentMarket], list[AgentMarket]]:
-    cls = check_not_none(MARKET_TYPE_TO_AGENT_MARKET.get(market_type))
-
+    cls = market_type.market_class
     open_markets = cls.get_binary_markets(
         limit=MAX_MONITOR_MARKETS,
         sort_by=SortBy.NEWEST,
         created_after=start_time,
         filter_by=FilterBy.OPEN,
     )
     resolved_markets = cls.get_binary_markets(
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import typing as t
 from functools import reduce
 
 import numpy as np
+from loguru import logger
 
 from prediction_market_agent_tooling.gtypes import Probability, wei_type, xDai
 from prediction_market_agent_tooling.markets.omen.data_models import OmenMarket
 from prediction_market_agent_tooling.markets.omen.omen import OmenAgentMarket
 from prediction_market_agent_tooling.tools.utils import check_not_none
 from prediction_market_agent_tooling.tools.web3_utils import (
     ONE_XDAI,
@@ -93,15 +94,15 @@
         assert np.isclose(
             reduce(lambda x, y: x * y, new_amounts, 1.0), float(fixed_product)
         )
         new_p_yes = Probability(new_amounts[1] / sum(new_amounts))
         bet_amount_wei = wei_type(bet_amount)
         if verbose:
             outcome = market_agent.get_outcome_str(bet_outcome_index)
-            print(
+            logger.debug(
                 f"Target p_yes: {target_p_yes:.2f}, bet: {wei_to_xdai(bet_amount_wei):.2f}{market_agent.currency} for {outcome}, new p_yes: {new_p_yes:.2f}"
             )
         if abs(target_p_yes - new_p_yes) < 0.01:
             break
         elif new_p_yes > target_p_yes:
             if bet_outcome_index == 0:
                 max_bet_amount = bet_amount
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/contract.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/contract.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/gnosis_rpc.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/gnosis_rpc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 
 import requests
 
-from prediction_market_agent_tooling.gtypes import ChainID, Wei
+from prediction_market_agent_tooling.gtypes import ChainID, HexAddress, Wei
 
 GNOSIS_NETWORK_ID = ChainID(100)  # xDai network.
 GNOSIS_RPC_URL = os.getenv("GNOSIS_RPC_URL", "https://gnosis-rpc.publicnode.com")
 
 
-def get_balance(address: str) -> Wei:
+def get_balance(address: HexAddress) -> Wei:
     response = requests.post(
         GNOSIS_RPC_URL,
         json={
             "jsonrpc": "2.0",
             "method": "eth_getBalance",
             "params": [address, "latest"],
             "id": 1,
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/is_predictable.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/is_predictable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from langchain.prompts import ChatPromptTemplate
 from langchain_openai import ChatOpenAI
 
 from prediction_market_agent_tooling.tools.cache import persistent_inmemory_cache
 
 # I tried to make it return a JSON, but it didn't work well in combo with asking it to do chain of thought.
-QUESTION_EVALUATE_PROMPT = """Main signs about a fully qualified question (sometimes referred to as a "market"):
+QUESTION_IS_PREDICTABLE_BINARY_PROMPT = """Main signs about a fully qualified question (sometimes referred to as a "market"):
 - The market's question needs to be specific, without use of pronouns.
 - The market's question needs to have a clear future event.
 - The market's question needs to have a clear time frame.
 - The event in the market's question doesn't have to be ultra-specific, it will be decided by a crowd later on.
 - If the market's question contains date, but without an year, it's okay.
 - If the market's question contains year, but without an exact date, it's okay.
 - The market's question can not be about itself or refer to itself.
 - The answer is probably Google-able, after the event happened.
+- The potential asnwer can be only "Yes" or "No".
 
 Follow a chain of thought to evaluate if the question is fully qualified:
 
 First, write the parts of the following question:
 
 "{question}"
 
@@ -25,18 +26,18 @@
 Then, explain why do you think it is or isn't fully qualified.
 
 Finally, write your final decision, write `decision: ` followed by either "yes it is fully qualified" or "no it isn't fully qualified" about the question. Don't write anything else after that. You must include "yes" or "no".
 """
 
 
 @persistent_inmemory_cache
-def is_predictable(
+def is_predictable_binary(
     question: str,
     engine: str = "gpt-4-1106-preview",
-    prompt_template: str = QUESTION_EVALUATE_PROMPT,
+    prompt_template: str = QUESTION_IS_PREDICTABLE_BINARY_PROMPT,
 ) -> bool:
     """
     Evaluate if the question is actually answerable.
     """
     llm = ChatOpenAI(model=engine, temperature=0.0)
 
     prompt = ChatPromptTemplate.from_template(template=prompt_template)
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/parallelism.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/parallelism.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/utils.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import typing as t
 from datetime import datetime
 from typing import Any, NoReturn, Optional, Type, TypeVar, cast
 
 import git
 import pytz
 import requests
-from pydantic import BaseModel
+from loguru import logger
+from pydantic import BaseModel, ValidationError
 
 from prediction_market_agent_tooling.gtypes import DatetimeWithTimezone, SecretStr
 
 T = TypeVar("T")
 
 
 def check_not_none(
@@ -64,15 +65,15 @@
         raise ValueError(f"Directory {output_dir} does not exist")
     output_file = f"{output_dir}/requirements.txt"
     subprocess.run(
         f"poetry export -f requirements.txt --without-hashes --output {output_file}",
         shell=True,
         check=True,
     )
-    print(f"Saved requirements to {output_dir}/requirements.txt")
+    logger.debug(f"Saved requirements to {output_dir}/requirements.txt")
 
 
 @t.overload
 def add_utc_timezone_validator(value: datetime) -> DatetimeWithTimezone:
     ...
 
 
@@ -99,14 +100,18 @@
     return add_utc_timezone_validator(datetime.utcnow())
 
 
 def get_current_git_commit_sha() -> str:
     return git.Repo(search_parent_directories=True).head.commit.hexsha
 
 
+def to_int_timestamp(dt: datetime) -> int:
+    return int(dt.timestamp())
+
+
 def get_current_git_branch() -> str:
     return git.Repo(search_parent_directories=True).active_branch.name
 
 
 def get_current_git_url() -> str:
     return git.Repo(search_parent_directories=True).remotes.origin.url
 
@@ -120,20 +125,26 @@
 BaseModelT = TypeVar("BaseModelT", bound=BaseModel)
 
 
 def response_to_model(
     response: requests.models.Response, model: Type[BaseModelT]
 ) -> BaseModelT:
     response_json = response_to_json(response)
-    return model.model_validate(response_json)
+    try:
+        return model.model_validate(response_json)
+    except ValidationError as e:
+        raise ValueError(f"Unable to validate: `{response_json}`") from e
 
 
 def response_list_to_model(
     response: requests.models.Response, model: Type[BaseModelT]
 ) -> list[BaseModelT]:
     response_json = response_to_json(response)
-    return [model.model_validate(x) for x in response_json]
+    try:
+        return [model.model_validate(x) for x in response_json]
+    except ValidationError as e:
+        raise ValueError(f"Unable to validate: `{response_json}`") from e
 
 
 def secret_str_from_env(key: str) -> SecretStr | None:
     value = os.getenv(key)
     return SecretStr(value) if value else None
```

### Comparing `prediction_market_agent_tooling-0.6.0/prediction_market_agent_tooling/tools/web3_utils.py` & `prediction_market_agent_tooling-0.7.0/prediction_market_agent_tooling/tools/web3_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from decimal import Decimal
 from typing import Any, Optional, TypeVar
 
 import tenacity
 from eth_account import Account
 from pydantic.types import SecretStr
 from web3 import Web3
+from web3.constants import HASH_ZERO
 from web3.types import Nonce, TxParams, TxReceipt, Wei
 
 from prediction_market_agent_tooling.gtypes import (
     ABI,
     ChecksumAddress,
     HexAddress,
+    HexBytes,
     HexStr,
     PrivateKey,
     xDai,
     xdai_type,
 )
 
 ONE_NONCE = Nonce(1)
 ONE_XDAI = xdai_type(1)
+ZERO_BYTES = HexBytes(HASH_ZERO)
 
 
 def private_key_to_public_key(private_key: SecretStr) -> ChecksumAddress:
     account = Account.from_key(private_key.get_secret_value())
     return verify_address(account.address)
 
 
@@ -79,33 +82,39 @@
         return params
     if isinstance(params, dict):
         return list(params.values())
     raise ValueError(f"Invalid type for function parameters: {type(params)}")
 
 
 @tenacity.retry(
-    wait=tenacity.wait_chain(*[tenacity.wait_fixed(n) for n in range(1, 6)])
+    wait=tenacity.wait_chain(*[tenacity.wait_fixed(n) for n in range(1, 6)]),
+    stop=tenacity.stop_after_attempt(5),
+    after=lambda x: print(f"call_function_on_contract failed, {x.attempt_number=}."),
 )
 def call_function_on_contract(
     web3: Web3,
     contract_address: ChecksumAddress,
     contract_abi: ABI,
     function_name: str,
     function_params: Optional[list[Any] | dict[str, Any]] = None,
 ) -> Any:
     contract = web3.eth.contract(address=contract_address, abi=contract_abi)
     output = contract.functions[function_name](*parse_function_params(function_params)).call()  # type: ignore # TODO: Fix Mypy, as this works just OK.
     return output
 
 
 @tenacity.retry(
-    # Retry only for the transaction nonce errors (as it can get correct one next time),
+    # Retry only for the transaction errors that match the given patterns,
     # add other retrieable errors gradually to be safe.
-    retry=tenacity.retry_if_exception_message(match=".*wrong transaction nonce.*"),
+    retry=tenacity.retry_if_exception_message(
+        match="(.*wrong transaction nonce.*)|(.*Invalid.*)|(.*OldNonce.*)"
+    ),
     wait=tenacity.wait_chain(*[tenacity.wait_fixed(n) for n in range(1, 10)]),
+    stop=tenacity.stop_after_attempt(9),
+    after=lambda x: print(f"send_function_on_contract_tx failed, {x.attempt_number=}."),
 )
 def send_function_on_contract_tx(
     web3: Web3,
     *,
     contract_address: ChecksumAddress,
     contract_abi: ABI,
     from_private_key: PrivateKey,
```

### Comparing `prediction_market_agent_tooling-0.6.0/pyproject.toml` & `prediction_market_agent_tooling-0.7.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prediction-market-agent-tooling"
-version = "0.6.0"
+version = "0.7.0"
 description = "Tools to benchmark, deploy and monitor prediction market agents."
 authors = ["Gnosis"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 buy_omen = "scripts.bet_omen:buy"
 sell_omen = "scripts.bet_omen:sell"
@@ -29,17 +29,21 @@
 langchain-community = ">=0.0.19"
 scikit-learn = "^1.4.0"
 tabulate = "^0.9.0"
 types-pytz = "^2024.1.0.20240203"
 google-cloud-secret-manager = "^2.18.2"
 langchain = { version = "^0.1.9", optional = true}
 langchain-openai = { version = "^0.0.8", optional = true}
+google-api-python-client = { version = "2.95.0", optional = true}
+subgrounds = "^1.8.1"
+loguru = "^0.7.2"
 
 [tool.poetry.extras]
 langchain = ["langchain", "langchain-openai"]
+google = ["google-api-python-client"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 mypy = "^1.8.0"
 black = "^23.12.1"
 
 [build-system]
```

### Comparing `prediction_market_agent_tooling-0.6.0/PKG-INFO` & `prediction_market_agent_tooling-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: prediction-market-agent-tooling
-Version: 0.6.0
+Version: 0.7.0
 Summary: Tools to benchmark, deploy and monitor prediction market agents.
 Author: Gnosis
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: google
 Provides-Extra: langchain
 Requires-Dist: autoflake (>=2.2.1,<3.0.0)
 Requires-Dist: cron-validator (>=1.0.8,<2.0.0)
 Requires-Dist: eth-typing (>=4.0.0,<5.0.0)
 Requires-Dist: functions-framework (>=3.5.0,<4.0.0)
+Requires-Dist: google-api-python-client (==2.95.0) ; extra == "google"
 Requires-Dist: google-cloud-functions (>=1.16.0,<2.0.0)
 Requires-Dist: google-cloud-resource-manager (>=1.12.0,<2.0.0)
 Requires-Dist: google-cloud-secret-manager (>=2.18.2,<3.0.0)
 Requires-Dist: isort (>=5.13.2,<6.0.0)
 Requires-Dist: langchain (>=0.1.9,<0.2.0) ; extra == "langchain"
 Requires-Dist: langchain-community (>=0.0.19)
 Requires-Dist: langchain-openai (>=0.0.8,<0.0.9) ; extra == "langchain"
+Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.4.0,<2.0.0)
 Requires-Dist: streamlit (>=1.31.0,<2.0.0)
+Requires-Dist: subgrounds (>=1.8.1,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: types-pytz (>=2024.1.0.20240203,<2025.0.0.0)
 Requires-Dist: types-requests (>=2.31.0.20240106,<3.0.0.0)
 Requires-Dist: web3 (>=6.15.1,<7.0.0)
 Description-Content-Type: text/markdown
```

