# Comparing `tmp/financetoolkit-1.8.4.tar.gz` & `tmp/financetoolkit-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financetoolkit-1.8.4.tar", max compression
+gzip compressed data, was "financetoolkit-1.8.5.tar", max compression
```

## Comparing `financetoolkit-1.8.4.tar` & `financetoolkit-1.8.5.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0     1069 2023-05-11 17:19:30.665832 financetoolkit-1.8.4/LICENSE.txt
--rw-r--r--   0        0        0   233119 2024-02-11 09:36:03.861472 financetoolkit-1.8.4/README.md
--rw-r--r--   0        0        0      200 2024-01-02 16:19:56.729577 financetoolkit-1.8.4/financetoolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-01-02 16:19:56.729619 financetoolkit-1.8.4/financetoolkit/discovery/__init__.py
--rw-r--r--   0        0        0    52191 2024-01-05 15:16:03.401705 financetoolkit-1.8.4/financetoolkit/discovery/discovery_controller.py
--rw-r--r--   0        0        0    21555 2024-01-02 16:19:56.730152 financetoolkit-1.8.4/financetoolkit/discovery/discovery_model.py
--rw-r--r--   0        0        0        0 2023-12-11 15:16:16.590582 financetoolkit-1.8.4/financetoolkit/economics/__init__.py
--rw-r--r--   0        0        0     2718 2023-12-18 12:15:31.628859 financetoolkit-1.8.4/financetoolkit/economics/ecb_model.py
--rw-r--r--   0        0        0   116795 2024-01-22 16:45:00.544101 financetoolkit-1.8.4/financetoolkit/economics/economics_controller.py
--rw-r--r--   0        0        0     5924 2023-12-18 12:15:31.629485 financetoolkit-1.8.4/financetoolkit/economics/fed_model.py
--rw-r--r--   0        0        0    41430 2023-12-21 12:41:19.719057 financetoolkit-1.8.4/financetoolkit/economics/oecd_model.py
--rw-r--r--   0        0        0    47381 2024-01-26 13:56:45.140582 financetoolkit-1.8.4/financetoolkit/fundamentals_model.py
--rw-r--r--   0        0        0    18368 2024-01-24 22:40:52.936602 financetoolkit-1.8.4/financetoolkit/helpers.py
--rw-r--r--   0        0        0    43662 2024-02-04 11:49:16.648225 financetoolkit-1.8.4/financetoolkit/historical_model.py
--rw-r--r--   0        0        0        0 2023-05-11 14:54:28.954198 financetoolkit-1.8.4/financetoolkit/models/__init__.py
--rw-r--r--   0        0        0     7478 2024-02-11 09:36:03.861799 financetoolkit-1.8.4/financetoolkit/models/altman_model.py
--rw-r--r--   0        0        0     5320 2023-12-05 14:17:55.353456 financetoolkit-1.8.4/financetoolkit/models/dupont_model.py
--rw-r--r--   0        0        0     2859 2023-12-05 14:17:55.353743 financetoolkit-1.8.4/financetoolkit/models/enterprise_model.py
--rw-r--r--   0        0        0     1682 2024-01-09 09:12:45.437621 financetoolkit-1.8.4/financetoolkit/models/growth_model.py
--rw-r--r--   0        0        0     1576 2024-02-04 11:49:16.648377 financetoolkit-1.8.4/financetoolkit/models/helpers.py
--rw-r--r--   0        0        0     5562 2024-02-04 11:49:16.648585 financetoolkit-1.8.4/financetoolkit/models/intrinsic_model.py
--rw-r--r--   0        0        0    54517 2024-02-11 09:36:03.862148 financetoolkit-1.8.4/financetoolkit/models/models_controller.py
--rw-r--r--   0        0        0    21129 2023-12-05 14:17:55.355064 financetoolkit-1.8.4/financetoolkit/models/piotroski_model.py
--rw-r--r--   0        0        0     6891 2024-01-09 09:12:45.439111 financetoolkit-1.8.4/financetoolkit/models/wacc_model.py
--rw-r--r--   0        0        0     1795 2023-12-05 12:12:44.159114 financetoolkit-1.8.4/financetoolkit/normalization/balance.csv
--rw-r--r--   0        0        0     1364 2023-12-05 12:12:44.159234 financetoolkit-1.8.4/financetoolkit/normalization/cash.csv
--rw-r--r--   0        0        0     1119 2023-12-05 12:12:44.159347 financetoolkit-1.8.4/financetoolkit/normalization/income.csv
--rw-r--r--   0        0        0      205 2023-12-05 12:12:44.159428 financetoolkit-1.8.4/financetoolkit/normalization/statistics.csv
--rw-r--r--   0        0        0     6859 2023-12-05 14:17:55.355618 financetoolkit-1.8.4/financetoolkit/normalization_model.py
--rw-r--r--   0        0        0        0 2024-01-17 13:13:01.201305 financetoolkit-1.8.4/financetoolkit/options/__init__.py
--rw-r--r--   0        0        0     9128 2024-02-04 11:49:16.649095 financetoolkit-1.8.4/financetoolkit/options/binomial_trees_model.py
--rw-r--r--   0        0        0     3481 2024-01-17 13:13:01.201463 financetoolkit-1.8.4/financetoolkit/options/black_scholes_model.py
--rw-r--r--   0        0        0    27717 2024-01-17 13:13:01.201597 financetoolkit-1.8.4/financetoolkit/options/greeks_model.py
--rw-r--r--   0        0        0     9093 2024-02-04 11:49:16.649301 financetoolkit-1.8.4/financetoolkit/options/helpers.py
--rw-r--r--   0        0        0   211062 2024-02-11 09:36:03.862962 financetoolkit-1.8.4/financetoolkit/options/options_controller.py
--rw-r--r--   0        0        0     4540 2024-02-11 09:36:03.863368 financetoolkit-1.8.4/financetoolkit/options/options_model.py
--rw-r--r--   0        0        0        0 2023-12-05 12:12:44.159580 financetoolkit-1.8.4/financetoolkit/performance/__init__.py
--rw-r--r--   0        0        0     7028 2024-01-26 13:56:45.141380 financetoolkit-1.8.4/financetoolkit/performance/helpers.py
--rw-r--r--   0        0        0    70539 2024-01-26 13:56:45.141733 financetoolkit-1.8.4/financetoolkit/performance/performance_controller.py
--rw-r--r--   0        0        0    25650 2024-01-26 13:56:45.141950 financetoolkit-1.8.4/financetoolkit/performance/performance_model.py
--rw-r--r--   0        0        0        0 2023-05-11 14:28:40.501711 financetoolkit-1.8.4/financetoolkit/ratios/__init__.py
--rw-r--r--   0        0        0     9837 2024-01-05 15:16:03.403144 financetoolkit-1.8.4/financetoolkit/ratios/efficiency_model.py
--rw-r--r--   0        0        0     5029 2023-12-05 14:17:55.357009 financetoolkit-1.8.4/financetoolkit/ratios/liquidity_model.py
--rw-r--r--   0        0        0    12829 2024-01-05 15:16:03.403517 financetoolkit-1.8.4/financetoolkit/ratios/profitability_model.py
--rw-r--r--   0        0        0   261569 2024-02-04 11:49:16.650933 financetoolkit-1.8.4/financetoolkit/ratios/ratios_controller.py
--rw-r--r--   0        0        0     7011 2023-12-05 14:17:55.357905 financetoolkit-1.8.4/financetoolkit/ratios/solvency_model.py
--rw-r--r--   0        0        0    15318 2024-01-05 15:16:03.404873 financetoolkit-1.8.4/financetoolkit/ratios/valuation_model.py
--rw-r--r--   0        0        0        0 2023-12-05 12:12:44.161409 financetoolkit-1.8.4/financetoolkit/risk/__init__.py
--rw-r--r--   0        0        0     7713 2024-01-05 15:16:03.405414 financetoolkit-1.8.4/financetoolkit/risk/cvar_model.py
--rw-r--r--   0        0        0     1723 2024-01-05 15:16:03.405651 financetoolkit-1.8.4/financetoolkit/risk/evar_model.py
--rw-r--r--   0        0        0     9537 2024-01-05 15:16:03.405900 financetoolkit-1.8.4/financetoolkit/risk/garch_model.py
--rw-r--r--   0        0        0     2531 2024-01-26 13:56:45.142894 financetoolkit-1.8.4/financetoolkit/risk/helpers.py
--rw-r--r--   0        0        0    38389 2024-01-26 13:56:45.143141 financetoolkit-1.8.4/financetoolkit/risk/risk_controller.py
--rw-r--r--   0        0        0     5609 2024-01-05 15:16:03.406914 financetoolkit-1.8.4/financetoolkit/risk/risk_model.py
--rw-r--r--   0        0        0     5471 2024-01-19 13:10:21.010912 financetoolkit-1.8.4/financetoolkit/risk/var_model.py
--rw-r--r--   0        0        0        0 2024-01-17 13:13:01.202491 financetoolkit-1.8.4/financetoolkit/technicals/__init__.py
--rw-r--r--   0        0        0     3620 2024-01-17 13:13:01.202619 financetoolkit-1.8.4/financetoolkit/technicals/breadth_model.py
--rw-r--r--   0        0        0     1993 2024-01-26 13:56:45.143315 financetoolkit-1.8.4/financetoolkit/technicals/helpers.py
--rw-r--r--   0        0        0    16454 2024-01-17 13:13:01.202824 financetoolkit-1.8.4/financetoolkit/technicals/momentum_model.py
--rw-r--r--   0        0        0     2761 2024-01-17 13:13:01.202897 financetoolkit-1.8.4/financetoolkit/technicals/overlap_model.py
--rw-r--r--   0        0        0     3826 2024-01-17 13:13:01.202959 financetoolkit-1.8.4/financetoolkit/technicals/statistic_model.py
--rw-r--r--   0        0        0   134139 2024-01-26 13:56:45.143730 financetoolkit-1.8.4/financetoolkit/technicals/technicals_controller.py
--rw-r--r--   0        0        0     3598 2024-01-17 13:13:01.203383 financetoolkit-1.8.4/financetoolkit/technicals/volatility_model.py
--rw-r--r--   0        0        0   161268 2024-02-05 13:57:08.560738 financetoolkit-1.8.4/financetoolkit/toolkit_controller.py
--rw-r--r--   0        0        0     2492 2024-02-11 09:36:03.863692 financetoolkit-1.8.4/pyproject.toml
--rw-r--r--   0        0        0   234268 1970-01-01 00:00:00.000000 financetoolkit-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 17:19:30.665832 financetoolkit-1.8.5/LICENSE.txt
+-rw-r--r--   0        0        0   235829 2024-04-02 14:55:09.340278 financetoolkit-1.8.5/README.md
+-rw-r--r--   0        0        0      200 2024-04-02 13:53:46.521829 financetoolkit-1.8.5/financetoolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-02 16:19:56.729619 financetoolkit-1.8.5/financetoolkit/discovery/__init__.py
+-rw-r--r--   0        0        0    52191 2024-01-05 15:16:03.401705 financetoolkit-1.8.5/financetoolkit/discovery/discovery_controller.py
+-rw-r--r--   0        0        0    21555 2024-01-02 16:19:56.730152 financetoolkit-1.8.5/financetoolkit/discovery/discovery_model.py
+-rw-r--r--   0        0        0        0 2023-12-11 15:16:16.590582 financetoolkit-1.8.5/financetoolkit/economics/__init__.py
+-rw-r--r--   0        0        0     2718 2023-12-18 12:15:31.628859 financetoolkit-1.8.5/financetoolkit/economics/ecb_model.py
+-rw-r--r--   0        0        0   129829 2024-04-02 14:55:09.341394 financetoolkit-1.8.5/financetoolkit/economics/economics_controller.py
+-rw-r--r--   0        0        0     5924 2023-12-18 12:15:31.629485 financetoolkit-1.8.5/financetoolkit/economics/fed_model.py
+-rw-r--r--   0        0        0     7889 2024-04-02 14:55:09.341765 financetoolkit-1.8.5/financetoolkit/economics/fred_model.py
+-rw-r--r--   0        0        0    41430 2023-12-21 12:41:19.719057 financetoolkit-1.8.5/financetoolkit/economics/oecd_model.py
+-rw-r--r--   0        0        0    47381 2024-01-26 13:56:45.140582 financetoolkit-1.8.5/financetoolkit/fundamentals_model.py
+-rw-r--r--   0        0        0    18368 2024-04-02 15:17:03.310710 financetoolkit-1.8.5/financetoolkit/helpers.py
+-rw-r--r--   0        0        0    43761 2024-04-02 15:19:39.434469 financetoolkit-1.8.5/financetoolkit/historical_model.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:54:28.954198 financetoolkit-1.8.5/financetoolkit/models/__init__.py
+-rw-r--r--   0        0        0     7478 2024-02-11 09:36:03.861799 financetoolkit-1.8.5/financetoolkit/models/altman_model.py
+-rw-r--r--   0        0        0     5320 2023-12-05 14:17:55.353456 financetoolkit-1.8.5/financetoolkit/models/dupont_model.py
+-rw-r--r--   0        0        0     2859 2023-12-05 14:17:55.353743 financetoolkit-1.8.5/financetoolkit/models/enterprise_model.py
+-rw-r--r--   0        0        0     1682 2024-01-09 09:12:45.437621 financetoolkit-1.8.5/financetoolkit/models/growth_model.py
+-rw-r--r--   0        0        0     1576 2024-02-04 11:49:16.648377 financetoolkit-1.8.5/financetoolkit/models/helpers.py
+-rw-r--r--   0        0        0     5562 2024-02-04 11:49:16.648585 financetoolkit-1.8.5/financetoolkit/models/intrinsic_model.py
+-rw-r--r--   0        0        0    54517 2024-02-11 09:36:03.862148 financetoolkit-1.8.5/financetoolkit/models/models_controller.py
+-rw-r--r--   0        0        0    21129 2023-12-05 14:17:55.355064 financetoolkit-1.8.5/financetoolkit/models/piotroski_model.py
+-rw-r--r--   0        0        0     7264 2024-04-02 15:30:42.742540 financetoolkit-1.8.5/financetoolkit/models/wacc_model.py
+-rw-r--r--   0        0        0     1795 2023-12-05 12:12:44.159114 financetoolkit-1.8.5/financetoolkit/normalization/balance.csv
+-rw-r--r--   0        0        0     1364 2023-12-05 12:12:44.159234 financetoolkit-1.8.5/financetoolkit/normalization/cash.csv
+-rw-r--r--   0        0        0     1119 2023-12-05 12:12:44.159347 financetoolkit-1.8.5/financetoolkit/normalization/income.csv
+-rw-r--r--   0        0        0      205 2023-12-05 12:12:44.159428 financetoolkit-1.8.5/financetoolkit/normalization/statistics.csv
+-rw-r--r--   0        0        0     6859 2023-12-05 14:17:55.355618 financetoolkit-1.8.5/financetoolkit/normalization_model.py
+-rw-r--r--   0        0        0        0 2024-01-17 13:13:01.201305 financetoolkit-1.8.5/financetoolkit/options/__init__.py
+-rw-r--r--   0        0        0     9128 2024-02-04 11:49:16.649095 financetoolkit-1.8.5/financetoolkit/options/binomial_trees_model.py
+-rw-r--r--   0        0        0     3481 2024-01-17 13:13:01.201463 financetoolkit-1.8.5/financetoolkit/options/black_scholes_model.py
+-rw-r--r--   0        0        0    27717 2024-01-17 13:13:01.201597 financetoolkit-1.8.5/financetoolkit/options/greeks_model.py
+-rw-r--r--   0        0        0     9093 2024-02-04 11:49:16.649301 financetoolkit-1.8.5/financetoolkit/options/helpers.py
+-rw-r--r--   0        0        0   211062 2024-04-02 14:55:03.298677 financetoolkit-1.8.5/financetoolkit/options/options_controller.py
+-rw-r--r--   0        0        0     4540 2024-02-11 09:36:03.863368 financetoolkit-1.8.5/financetoolkit/options/options_model.py
+-rw-r--r--   0        0        0        0 2023-12-05 12:12:44.159580 financetoolkit-1.8.5/financetoolkit/performance/__init__.py
+-rw-r--r--   0        0        0     7028 2024-01-26 13:56:45.141380 financetoolkit-1.8.5/financetoolkit/performance/helpers.py
+-rw-r--r--   0        0        0    70539 2024-01-26 13:56:45.141733 financetoolkit-1.8.5/financetoolkit/performance/performance_controller.py
+-rw-r--r--   0        0        0    25650 2024-01-26 13:56:45.141950 financetoolkit-1.8.5/financetoolkit/performance/performance_model.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:28:40.501711 financetoolkit-1.8.5/financetoolkit/ratios/__init__.py
+-rw-r--r--   0        0        0     9837 2024-01-05 15:16:03.403144 financetoolkit-1.8.5/financetoolkit/ratios/efficiency_model.py
+-rw-r--r--   0        0        0     5029 2023-12-05 14:17:55.357009 financetoolkit-1.8.5/financetoolkit/ratios/liquidity_model.py
+-rw-r--r--   0        0        0    12829 2024-01-05 15:16:03.403517 financetoolkit-1.8.5/financetoolkit/ratios/profitability_model.py
+-rw-r--r--   0        0        0   261569 2024-02-04 11:49:16.650933 financetoolkit-1.8.5/financetoolkit/ratios/ratios_controller.py
+-rw-r--r--   0        0        0     7011 2023-12-05 14:17:55.357905 financetoolkit-1.8.5/financetoolkit/ratios/solvency_model.py
+-rw-r--r--   0        0        0    15318 2024-01-05 15:16:03.404873 financetoolkit-1.8.5/financetoolkit/ratios/valuation_model.py
+-rw-r--r--   0        0        0        0 2023-12-05 12:12:44.161409 financetoolkit-1.8.5/financetoolkit/risk/__init__.py
+-rw-r--r--   0        0        0     7713 2024-01-05 15:16:03.405414 financetoolkit-1.8.5/financetoolkit/risk/cvar_model.py
+-rw-r--r--   0        0        0     1723 2024-01-05 15:16:03.405651 financetoolkit-1.8.5/financetoolkit/risk/evar_model.py
+-rw-r--r--   0        0        0     9537 2024-01-05 15:16:03.405900 financetoolkit-1.8.5/financetoolkit/risk/garch_model.py
+-rw-r--r--   0        0        0     2531 2024-01-26 13:56:45.142894 financetoolkit-1.8.5/financetoolkit/risk/helpers.py
+-rw-r--r--   0        0        0    38389 2024-01-26 13:56:45.143141 financetoolkit-1.8.5/financetoolkit/risk/risk_controller.py
+-rw-r--r--   0        0        0     5609 2024-01-05 15:16:03.406914 financetoolkit-1.8.5/financetoolkit/risk/risk_model.py
+-rw-r--r--   0        0        0     5471 2024-01-19 13:10:21.010912 financetoolkit-1.8.5/financetoolkit/risk/var_model.py
+-rw-r--r--   0        0        0        0 2024-01-17 13:13:01.202491 financetoolkit-1.8.5/financetoolkit/technicals/__init__.py
+-rw-r--r--   0        0        0     3620 2024-01-17 13:13:01.202619 financetoolkit-1.8.5/financetoolkit/technicals/breadth_model.py
+-rw-r--r--   0        0        0     1993 2024-01-26 13:56:45.143315 financetoolkit-1.8.5/financetoolkit/technicals/helpers.py
+-rw-r--r--   0        0        0    16454 2024-01-17 13:13:01.202824 financetoolkit-1.8.5/financetoolkit/technicals/momentum_model.py
+-rw-r--r--   0        0        0     2761 2024-01-17 13:13:01.202897 financetoolkit-1.8.5/financetoolkit/technicals/overlap_model.py
+-rw-r--r--   0        0        0    14582 2024-04-02 15:45:53.162486 financetoolkit-1.8.5/financetoolkit/technicals/statistic_model.py
+-rw-r--r--   0        0        0   134139 2024-01-26 13:56:45.143730 financetoolkit-1.8.5/financetoolkit/technicals/technicals_controller.py
+-rw-r--r--   0        0        0     3598 2024-01-17 13:13:01.203383 financetoolkit-1.8.5/financetoolkit/technicals/volatility_model.py
+-rw-r--r--   0        0        0   161448 2024-04-02 15:19:40.167959 financetoolkit-1.8.5/financetoolkit/toolkit_controller.py
+-rw-r--r--   0        0        0     2492 2024-04-02 15:46:11.943579 financetoolkit-1.8.5/pyproject.toml
+-rw-r--r--   0        0        0   236978 1970-01-01 00:00:00.000000 financetoolkit-1.8.5/PKG-INFO
```

### Comparing `financetoolkit-1.8.4/LICENSE.txt` & `financetoolkit-1.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/README.md` & `financetoolkit-1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: financetoolkit
+Version: 1.8.5
+Summary: Transparent and Efficient Financial Analysis
+Home-page: https://www.jeroenbouma.com/projects/financetoolkit
+License: MIT
+Keywords: Finance,Toolkit,Financial,Analysis,Fundamental,Technical,Quantitative,Database,Equities,Currencies,Economics,ETFs,Funds,Indices,Moneymarkets,Commodities,Options
+Author: Jeroen Bouma
+Requires-Python: >=3.10,<3.13
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Office/Business :: Financial :: Investment
+Requires-Dist: pandas[computation,performance,plot] (>=2.2,<3.0)
+Requires-Dist: requests (>=2.31,<3.0)
+Requires-Dist: scikit-learn (>=1.3,<2.0)
+Project-URL: Repository, https://github.com/JerBouma/FinanceToolkit
+Description-Content-Type: text/markdown
+
 [![FinanceToolkit](https://github.com/JerBouma/FinanceToolkit/assets/46355364/198d47bd-e1b3-492d-acc4-5d9f02d1d009)](https://github.com/JerBouma/FinanceToolkit)
 
 [![GitHub Sponsors](https://img.shields.io/badge/Sponsor_this_Project-grey?logo=github)](https://github.com/sponsors/JerBouma)
 [![Buy Me a Coffee](https://img.shields.io/badge/Buy_Me_a_Coffee-grey?logo=buymeacoffee)](https://www.buymeacoffee.com/jerbouma)
 [![Twitter](https://img.shields.io/badge/Twitter-grey?logo=x)](https://twitter.com/JerBouma)
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-grey?logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/boumajeroen/)
 [![Documentation](https://img.shields.io/badge/Documentation-grey?logo=readme)](https://www.jeroenbouma.com/projects/financetoolkit/docs)
@@ -2706,14 +2730,48 @@
 > **Secured Overnight Financing Rate**
 
 The SOFR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data and data on bilateral Treasury repo transactions cleared through FICC’s DVP service, which are obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_federal_reserve_rates).
 
 </details>
 
 <details>
+    <summary><b>Fixed Income 📃 </b></summary>
+
+The fixed income metrics revolve around option-adjusted spreads, effective yields and total returns of corporate bonds based on the ICE BofA US Corporate Indices. It is possible to view both the indices of the ratings (AAA, AA, A, BBB, BB, B and CCC) and the maturities (1-3 years, 3-5 years, 5-7 years, 7-10 years, 10-15 years, 15-30 years and 30+ years).
+
+All fixed income metrics can be called by using `get_` to get a single metric. E.g. `get_option_adjusted_spread` or `get_yield_to_worst`. As an example:
+
+```python
+from financetoolkit import Toolkit
+
+toolkit = Toolkit(["AAPL", "TSLA"], api_key="FINANCIAL_MODELING_PREP_KEY")
+
+# Get Fixed Income Results
+toolkit.economics.get_option_adjusted_spread()
+```
+
+> Option-Adjusted Spread (OAS)
+
+The Option-Adjusted Spread (OAS) is the spread relative to a risk-free interest rate, usually measured in basis points (bp), that equates the theoretical present value of a series of uncertain cash flows to the market price of a fixed-income investment. The spread is added to the risk-free rate to compensate for the uncertainty of the cash flows. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_option_adjusted_spread).
+
+> Effective Yield
+
+The Effective Yield is the yield of a bond, calculated by dividing the bond's coupon payments by its market price. The effective yield is not the same as the stated yield, which is the yield on the bond's coupon payments divided by the bond's principal value. The effective yield is a more accurate measure of a bond's return, as it takes into account the fact that the investor will not hold the bond to maturity and will likely sell it before it matures. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_effective_yield).
+
+> Total Return
+
+The total return is the actual rate of return of an investment or a pool of investments over a given evaluation period. Total return includes interest, capital gains, dividends and distributions realized over a given period of time. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_total_return).
+
+> Yield to Worst
+
+Yield to worst is the lowest potential yield that a bond can generate without the issuer defaulting. The standard US convention for this series is to use semi-annual coupon payments, whereas the standard in the foreign markets is to use coupon payments with frequencies of annual, semi-annual, quarterly, and monthly. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_yield_to_worst).
+
+</details>
+
+<details>
     <summary><b>Environment 💚</b></summary>
 
 The environment metrics revolve around renewable energy, environmental tax, greenhouse gas emissions, crude oil production and crude oil prices of countries. This includes the renewable energy as a percentage of total energy, environmental tax as a percentage of GDP, greenhouse gas emissions, crude oil production and crude oil prices.
 
 All environment metrics can be called by using `get_` to get a single metric. E.g. `get_renewable_energy` or `get_crude_oil_prices`. As an example:
 
 ```python
@@ -2970,7 +3028,8 @@
 - **LinkedIn:** https://www.linkedin.com/in/boumajeroen/
 - **Email:** jer.bouma@gmail.com
 - **Discord:** add me on Discord **`JerBouma`**
 
 If you'd like to support my efforts, either help me out by contributing to the package or [Sponsor Me](https://github.com/sponsors/JerBouma).
 
 [![Star History Chart](https://api.star-history.com/svg?repos=JerBouma/FinanceToolkit&type=Date)](https://star-history.com/#JerBouma/FinanceToolkit&Date)
+
```

### Comparing `financetoolkit-1.8.4/financetoolkit/discovery/discovery_controller.py` & `financetoolkit-1.8.5/financetoolkit/discovery/discovery_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/discovery/discovery_model.py` & `financetoolkit-1.8.5/financetoolkit/discovery/discovery_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/economics/ecb_model.py` & `financetoolkit-1.8.5/financetoolkit/economics/ecb_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/economics/economics_controller.py` & `financetoolkit-1.8.5/financetoolkit/economics/economics_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 import re
 from datetime import datetime, timedelta
 
 import pandas as pd
 
-from financetoolkit.economics import ecb_model, fed_model, oecd_model
+from financetoolkit.economics import ecb_model, fed_model, fred_model, oecd_model
 from financetoolkit.helpers import calculate_growth, handle_errors
 
 # pylint: disable=too-many-instance-attributes,too-few-public-methods,too-many-lines,
 # pylint: disable=too-many-locals,line-too-long,too-many-public-methods
 # ruff: noqa: E501
 
 
@@ -1435,14 +1435,290 @@
                 "Rate must be one of 'EFFR', 'OBFR', 'TGCR', 'BGCR' or 'SOFR'."
             )
 
         fed_data = fed_data.loc[self._start_date : self._end_date]
 
         return fed_data
 
+    @handle_errors
+    def get_option_adjusted_spread(
+        self,
+        maturity: bool = True,
+        rounding: int | None = None,
+    ):
+        """
+        The ICE BofA Option-Adjusted Spreads (OASs) are the calculated spreads between a computed OAS index
+        of all bonds in a given maturity and rating category and a spot Treasury curve. An OAS index is constructed
+        using each constituent bond's OAS, weighted by market capitalization.
+
+        The Option-Adjusted Spread (OAS) is the spread relative to a risk-free interest rate, usually measured in
+        basis points (bp), that equates the theoretical present value of a series of uncertain cash flows to the
+        market price of a fixed-income investment. The spread is added to the risk-free rate to compensate for the
+        uncertainty of the cash flows.
+
+        See definitions:
+
+        - Ratings: https://fred.stlouisfed.org/series/BAMLC0A4CBBB
+        - Maturity: https://fred.stlouisfed.org/series/BAMLC1A0C13Y
+
+        Args:
+            maturity (bool, optional): Whether to return the maturity option adjusted spread or the rating option adjusted spread.
+            rounding (int | None, optional): The number of decimals to round the results to. Defaults to None.
+
+        Returns:
+            pd.DataFrame: A DataFrame containing the Option Adjusted Spread
+
+        As an example:
+
+        ```python
+        from financetoolkit import Economics
+
+        economics = Economics(
+            start_date='2024-01-01',
+            end_date='2024-01-15',
+        )
+
+        economics.get_option_adjusted_spread()
+        ```
+
+        Which returns:
+
+        | Date       |   1-3 Years |   3-5 Years |   5-7 Years |   7-10 Years |   10-15 Years |   15+ Years |
+        |:-----------|------------:|------------:|------------:|-------------:|--------------:|------------:|
+        | 2024-01-01 |          77 |          94 |       108.5 |          127 |         131.5 |         118 |
+        | 2024-01-02 |          78 |          95 |       109   |          128 |         133   |         119 |
+        | 2024-01-03 |          80 |          98 |       113   |          133 |         136   |         122 |
+        | 2024-01-04 |          80 |          98 |       112   |          133 |         135   |         122 |
+        | 2024-01-05 |          80 |          98 |       112   |          132 |         134   |         121 |
+        | 2024-01-08 |          79 |          98 |       112   |          132 |         134   |         120 |
+        | 2024-01-09 |          78 |          96 |       110   |          130 |         131   |         117 |
+        | 2024-01-10 |          77 |          94 |       108   |          128 |         128   |         113 |
+        | 2024-01-11 |          75 |          94 |       107   |          128 |         127   |         113 |
+        | 2024-01-12 |          74 |          94 |       107   |          128 |         126   |         112 |
+        | 2024-01-15 |          74 |          94 |       107   |          128 |         125   |         111 |
+        """
+        option_adjusted_spread = (
+            fred_model.get_maturity_option_adjusted_spread()
+            if maturity
+            else fred_model.get_rating_option_adjusted_spread()
+        )
+
+        option_adjusted_spread = option_adjusted_spread.loc[
+            self._start_date : self._end_date
+        ]
+
+        option_adjusted_spread = option_adjusted_spread.round(
+            rounding if rounding else self._rounding
+        )
+
+        return option_adjusted_spread
+
+    @handle_errors
+    def get_effective_yield(
+        self,
+        maturity: bool = True,
+        rounding: int | None = None,
+    ):
+        """
+        This data represents the effective yield of the ICE BofA Indices, When the last calendar day of the month
+        takes place on the weekend, weekend observations will occur as a result of month ending accrued interest adjustments.
+
+        The Effective Yield is the yield of a bond, calculated by dividing the bond's coupon payments by its market price.
+        The effective yield is not the same as the stated yield, which is the yield on the bond's coupon payments divided
+        by the bond's principal value. The effective yield is a more accurate measure of a bond's return, as it takes into
+        account the fact that the investor will not hold the bond to maturity and will likely sell it before it matures.
+
+        See definitions:
+
+        - Ratings: https://fred.stlouisfed.org/series/BAMLC0A4CBBBEY
+        - Maturity: https://fred.stlouisfed.org/series/BAMLC1A0C13YEY
+
+        Args:
+            maturity (bool, optional): Whether to return the maturity effective yield or the rating effective yield.
+            rounding (int | None, optional): The number of decimals to round the results to. Defaults to None.
+
+        Returns:
+            pd.DataFrame: A DataFrame containing the Gross Domestic Product
+
+        As an example:
+
+        ```python
+        from financetoolkit import Economics
+
+        economics = Economics(
+            start_date='2024-01-01',
+            end_date='2024-01-15',
+        )
+
+        economics.get_effective_yield(maturity=False)
+        ```
+
+        Which returns:
+
+        | Date       |    AAA |     AA |      A |    BBB |     BB |      B |    CCC |
+        |:-----------|-------:|-------:|-------:|-------:|-------:|-------:|-------:|
+        | 2024-01-01 | 0.0456 | 0.047  | 0.0505 | 0.054  | 0.0613 | 0.0752 | 0.1319 |
+        | 2024-01-02 | 0.0459 | 0.0473 | 0.0509 | 0.0543 | 0.0622 | 0.0763 | 0.1333 |
+        | 2024-01-03 | 0.0459 | 0.0474 | 0.051  | 0.0544 | 0.0634 | 0.0779 | 0.1358 |
+        | 2024-01-04 | 0.0466 | 0.0481 | 0.0518 | 0.0551 | 0.0639 | 0.0784 | 0.1367 |
+        | 2024-01-05 | 0.047  | 0.0485 | 0.0521 | 0.0554 | 0.0641 | 0.0787 | 0.137  |
+        | 2024-01-08 | 0.0465 | 0.0481 | 0.0517 | 0.055  | 0.0633 | 0.0776 | 0.1365 |
+        | 2024-01-09 | 0.0464 | 0.048  | 0.0516 | 0.0548 | 0.0629 | 0.0771 | 0.1359 |
+        | 2024-01-10 | 0.0464 | 0.048  | 0.0515 | 0.0547 | 0.0622 | 0.0762 | 0.1351 |
+        | 2024-01-11 | 0.0456 | 0.0472 | 0.0507 | 0.054  | 0.0619 | 0.076  | 0.1344 |
+        | 2024-01-12 | 0.0451 | 0.0467 | 0.0502 | 0.0534 | 0.0613 | 0.0753 | 0.1338 |
+        | 2024-01-15 | 0.0451 | 0.0467 | 0.0501 | 0.0533 | 0.0611 | 0.0751 | 0.1328 |
+        """
+        effective_yield = (
+            fred_model.get_maturity_effective_yield()
+            if maturity
+            else fred_model.get_rating_effective_yield()
+        )
+
+        effective_yield = effective_yield.loc[self._start_date : self._end_date]
+
+        effective_yield = effective_yield.round(
+            rounding if rounding else self._rounding
+        )
+
+        return effective_yield
+
+    @handle_errors
+    def get_total_return(
+        self,
+        maturity: bool = True,
+        rounding: int | None = None,
+    ):
+        """
+        This data represents the total return of the ICE BofA Indices, When the last calendar day of the month
+        takes place on the weekend, weekend observations will occur as a result of month ending accrued interest adjustments.
+
+        The total return is the actual rate of return of an investment or a pool of investments over a given evaluation period.
+        Total return includes interest, capital gains, dividends and distributions realized over a given period of time.
+
+        See definitions:
+
+        - Ratings: https://fred.stlouisfed.org/series/BAMLC0A4CBBBEY
+        - Maturity: https://fred.stlouisfed.org/series/BAMLC1A0C13YEY
+
+        Args:
+            maturity (bool, optional): Whether to return the maturity total return or the rating total return.
+            rounding (int | None, optional): The number of decimals to round the results to. Defaults to None.
+
+        Returns:
+            pd.DataFrame: A DataFrame containing the Gross Domestic Product
+
+        As an example:
+
+        ```python
+        from financetoolkit import Economics
+
+        economics = Economics(
+            start_date='2024-01-01',
+            end_date='2024-01-15',
+        )
+
+        economics.get_total_return(maturity=True)
+        ```
+
+        Which returns:
+
+        | Date       |   1-3 Years |   3-5 Years |   5-7 Years |   7-10 Years |   10-15 Years |   15+ Years |
+        |:-----------|------------:|------------:|------------:|-------------:|--------------:|------------:|
+        | 2024-01-01 |     1913.78 |     2487.68 |      809.13 |      585.705 |       4206.25 |     4358.69 |
+        | 2024-01-02 |     1912.73 |     2484.25 |      807.62 |      584.32  |       4193.7  |     4343.71 |
+        | 2024-01-03 |     1912.18 |     2483.95 |      807.54 |      583.84  |       4194.39 |     4339.07 |
+        | 2024-01-04 |     1910.86 |     2477.9  |      804.35 |      580.42  |       4163.24 |     4289.24 |
+        | 2024-01-05 |     1910.86 |     2475.75 |      802.82 |      578.73  |       4148.31 |     4262.52 |
+        | 2024-01-08 |     1912.48 |     2480.39 |      804.97 |      580.71  |       4167.04 |     4302.16 |
+        | 2024-01-09 |     1913.5  |     2482.27 |      805.72 |      581.26  |       4173.04 |     4303.34 |
+        | 2024-01-10 |     1914.12 |     2483.6  |      806.21 |      581.29  |       4175.16 |     4304.82 |
+        | 2024-01-11 |     1918.28 |     2492.25 |      809.94 |      583.92  |       4200.49 |     4330.72 |
+        | 2024-01-12 |     1922.1  |     2498.89 |      812.41 |      585.2   |       4213.47 |     4338.43 |
+        | 2024-01-15 |     1922.67 |     2499.76 |      812.67 |      585.41  |       4215.34 |     4340.24 |
+        """
+        total_return = (
+            fred_model.get_maturity_total_return()
+            if maturity
+            else fred_model.get_rating_total_return()
+        )
+
+        total_return = total_return.loc[self._start_date : self._end_date]
+
+        total_return = total_return.round(rounding if rounding else self._rounding)
+
+        return total_return
+
+    @handle_errors
+    def get_yield_to_worst(
+        self,
+        maturity: bool = True,
+        rounding: int | None = None,
+    ):
+        """
+        This data represents the semi-annual yield to worst of the ICE BofA Indices, When the last calendar day of the month
+        takes place on the weekend, weekend observations will occur as a result of month ending accrued interest adjustments.
+
+        Yield to worst is the lowest potential yield that a bond can generate without the issuer defaulting. The standard US
+        convention for this series is to use semi-annual coupon payments, whereas the standard in the foreign markets is
+        to use coupon payments with frequencies of annual, semi-annual, quarterly, and monthly.
+
+        See definitions:
+
+        - Ratings: https://fred.stlouisfed.org/series/BAMLC0A4CBBBEY
+        - Maturity: https://fred.stlouisfed.org/series/BAMLC1A0C13YEY
+
+        Args:
+            maturity (bool, optional): Whether to return the maturity yield to worst or the rating yield to worst.
+            rounding (int | None, optional): The number of decimals to round the results to. Defaults to None.
+
+        Returns:
+            pd.DataFrame: A DataFrame containing the Gross Domestic Product
+
+        As an example:
+
+        ```python
+        from financetoolkit import Economics
+
+        economics = Economics(
+            start_date='2024-01-01',
+            end_date='2024-01-15',
+        )
+
+        economics.get_yield_to_worst(maturity=False)
+        ```
+
+        Which returns:
+
+        | Date       |    AAA |     AA |      A |    BBB |     BB |      B |    CCC |
+        |:-----------|-------:|-------:|-------:|-------:|-------:|-------:|-------:|
+        | 2024-01-01 | 0.0456 | 0.0472 | 0.0503 | 0.0542 | 0.0645 | 0.0786 | 0.1316 |
+        | 2024-01-02 | 0.046  | 0.0475 | 0.0506 | 0.0546 | 0.0652 | 0.0796 | 0.1329 |
+        | 2024-01-03 | 0.0461 | 0.0475 | 0.0507 | 0.0547 | 0.0662 | 0.081  | 0.1353 |
+        | 2024-01-04 | 0.0468 | 0.0483 | 0.0515 | 0.0554 | 0.0665 | 0.0814 | 0.136  |
+        | 2024-01-05 | 0.0471 | 0.0486 | 0.0518 | 0.0557 | 0.0667 | 0.0816 | 0.1362 |
+        | 2024-01-08 | 0.0466 | 0.0482 | 0.0514 | 0.0553 | 0.066  | 0.0806 | 0.1359 |
+        | 2024-01-09 | 0.0465 | 0.0481 | 0.0513 | 0.0551 | 0.0656 | 0.0803 | 0.1353 |
+        | 2024-01-10 | 0.0465 | 0.0481 | 0.0512 | 0.0551 | 0.065  | 0.0795 | 0.1345 |
+        | 2024-01-11 | 0.0458 | 0.0473 | 0.0504 | 0.0543 | 0.0648 | 0.0793 | 0.134  |
+        | 2024-01-12 | 0.0453 | 0.0468 | 0.0499 | 0.0537 | 0.0642 | 0.0786 | 0.1335 |
+        | 2024-01-15 | 0.0452 | 0.0468 | 0.0498 | 0.0537 | 0.064  | 0.0784 | 0.1325 |
+        """
+        yield_to_worst = (
+            fred_model.get_maturity_yield_to_worst()
+            if maturity
+            else fred_model.get_rating_yield_to_worst()
+        )
+
+        yield_to_worst = yield_to_worst.loc[self._start_date : self._end_date]
+
+        yield_to_worst = yield_to_worst.round(rounding if rounding else self._rounding)
+
+        return yield_to_worst
+
     def get_renewable_energy(
         self,
         growth: bool = False,
         lag: int = 1,
         rounding: int | None = None,
     ):
         """
```

### Comparing `financetoolkit-1.8.4/financetoolkit/economics/fed_model.py` & `financetoolkit-1.8.5/financetoolkit/economics/fed_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/economics/oecd_model.py` & `financetoolkit-1.8.5/financetoolkit/economics/oecd_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/fundamentals_model.py` & `financetoolkit-1.8.5/financetoolkit/fundamentals_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/helpers.py` & `financetoolkit-1.8.5/financetoolkit/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/historical_model.py` & `financetoolkit-1.8.5/financetoolkit/historical_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,14 +230,17 @@
         # even if no data is found. This is mostly applicable when nothing
         # can be found at all.
         for ticker in tickers:
             historical_data_dict[ticker] = empty_historical_data
 
     reorder_tickers = [ticker for ticker in tickers if ticker in historical_data_dict]
 
+    if not historical_data_dict:
+        raise ValueError("No data found for the given tickers.")
+
     historical_data = pd.concat(historical_data_dict).unstack(level=0)
     historical_data = historical_data.reindex(reorder_tickers, level=1, axis=1)
 
     if "Dividends" in historical_data.columns:
         historical_data["Dividends"] = historical_data["Dividends"].fillna(0)
 
     if fill_nan:
```

### Comparing `financetoolkit-1.8.4/financetoolkit/models/altman_model.py` & `financetoolkit-1.8.5/financetoolkit/models/altman_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/models/dupont_model.py` & `financetoolkit-1.8.5/financetoolkit/models/dupont_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/models/enterprise_model.py` & `financetoolkit-1.8.5/financetoolkit/models/enterprise_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/models/growth_model.py` & `financetoolkit-1.8.5/financetoolkit/models/growth_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/models/helpers.py` & `financetoolkit-1.8.5/financetoolkit/models/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/models/intrinsic_model.py` & `financetoolkit-1.8.5/financetoolkit/models/intrinsic_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/models/models_controller.py` & `financetoolkit-1.8.5/financetoolkit/models/models_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/models/piotroski_model.py` & `financetoolkit-1.8.5/financetoolkit/models/piotroski_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/models/wacc_model.py` & `financetoolkit-1.8.5/financetoolkit/models/wacc_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Weighted Average Cost of Capital Module"""
 __docformat__ = "google"
 
+import numpy as np
 import pandas as pd
 
 from financetoolkit.performance import performance_model
 from financetoolkit.ratios import profitability_model, valuation_model
 
 # pylint: disable=too-many-locals
 
@@ -132,14 +133,22 @@
 
     # Calculate the Cost of Equity
     cost_of_equity = get_cost_of_equity(risk_free_rate, beta, benchmark_returns).T
 
     # Calculate the Cost of Debt
     cost_of_debt = get_cost_of_debt(interest_expense, total_debt)
 
+    # If the cost of debt is Inf, change it to 0
+    if np.inf in cost_of_debt.to_numpy():
+        print(
+            "Please note that the Cost of Debt contains Inf. This is due to Total Debt being 0, "
+            "therefore Cost of Debt is adjusted to 0 for those periods."
+        )
+        cost_of_debt = cost_of_debt.replace([np.inf, -np.inf], 0)
+
     # Calculate the Corporate Tax Rate
     corporate_tax_rate = profitability_model.get_effective_tax_rate(
         income_tax_expense, income_before_tax
     )
 
     # Calculate the Weighted Average Cost of Capital
     weighted_average_cost_of_capital = (
```

### Comparing `financetoolkit-1.8.4/financetoolkit/normalization/balance.csv` & `financetoolkit-1.8.5/financetoolkit/normalization/balance.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/normalization/cash.csv` & `financetoolkit-1.8.5/financetoolkit/normalization/cash.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/normalization/income.csv` & `financetoolkit-1.8.5/financetoolkit/normalization/income.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/normalization_model.py` & `financetoolkit-1.8.5/financetoolkit/normalization_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/options/binomial_trees_model.py` & `financetoolkit-1.8.5/financetoolkit/options/binomial_trees_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/options/black_scholes_model.py` & `financetoolkit-1.8.5/financetoolkit/options/black_scholes_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/options/greeks_model.py` & `financetoolkit-1.8.5/financetoolkit/options/greeks_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/options/helpers.py` & `financetoolkit-1.8.5/financetoolkit/options/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/options/options_controller.py` & `financetoolkit-1.8.5/financetoolkit/options/options_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/options/options_model.py` & `financetoolkit-1.8.5/financetoolkit/options/options_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/performance/helpers.py` & `financetoolkit-1.8.5/financetoolkit/performance/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/performance/performance_controller.py` & `financetoolkit-1.8.5/financetoolkit/performance/performance_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/performance/performance_model.py` & `financetoolkit-1.8.5/financetoolkit/performance/performance_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/ratios/efficiency_model.py` & `financetoolkit-1.8.5/financetoolkit/ratios/efficiency_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/ratios/liquidity_model.py` & `financetoolkit-1.8.5/financetoolkit/ratios/liquidity_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/ratios/profitability_model.py` & `financetoolkit-1.8.5/financetoolkit/ratios/profitability_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/ratios/ratios_controller.py` & `financetoolkit-1.8.5/financetoolkit/ratios/ratios_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/ratios/solvency_model.py` & `financetoolkit-1.8.5/financetoolkit/ratios/solvency_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/ratios/valuation_model.py` & `financetoolkit-1.8.5/financetoolkit/ratios/valuation_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/risk/cvar_model.py` & `financetoolkit-1.8.5/financetoolkit/risk/cvar_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/risk/evar_model.py` & `financetoolkit-1.8.5/financetoolkit/risk/evar_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/risk/garch_model.py` & `financetoolkit-1.8.5/financetoolkit/risk/garch_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/risk/helpers.py` & `financetoolkit-1.8.5/financetoolkit/risk/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/risk/risk_controller.py` & `financetoolkit-1.8.5/financetoolkit/risk/risk_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/risk/risk_model.py` & `financetoolkit-1.8.5/financetoolkit/risk/risk_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/risk/var_model.py` & `financetoolkit-1.8.5/financetoolkit/risk/var_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/technicals/breadth_model.py` & `financetoolkit-1.8.5/financetoolkit/technicals/breadth_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/technicals/helpers.py` & `financetoolkit-1.8.5/financetoolkit/technicals/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/technicals/momentum_model.py` & `financetoolkit-1.8.5/financetoolkit/technicals/momentum_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/technicals/overlap_model.py` & `financetoolkit-1.8.5/financetoolkit/technicals/overlap_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/technicals/technicals_controller.py` & `financetoolkit-1.8.5/financetoolkit/technicals/technicals_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/technicals/volatility_model.py` & `financetoolkit-1.8.5/financetoolkit/technicals/volatility_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.4/financetoolkit/toolkit_controller.py` & `financetoolkit-1.8.5/financetoolkit/toolkit_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -2552,20 +2552,24 @@
             if self._statistics_statement.empty:
                 self.get_statistics_statement(
                     progress_bar=progress_bar
                     if progress_bar is not None
                     else self._progress_bar
                 )
 
-            self._statement_currencies, self._currencies = helpers.determine_currencies(
-                statement_currencies=self._statistics_statement.xs(
-                    "Reported Currency", axis=0, level=1
-                ),
-                historical_currencies=self._historical_statistics.loc["Currency"],
-            )
+            if not self._statistics_statement.empty:
+                (
+                    self._statement_currencies,
+                    self._currencies,
+                ) = helpers.determine_currencies(
+                    statement_currencies=self._statistics_statement.xs(
+                        "Reported Currency", axis=0, level=1
+                    ),
+                    historical_currencies=self._historical_statistics.loc["Currency"],
+                )
 
         if self._daily_exchange_rate_data.empty or overwrite:
             self._daily_exchange_rate_data, _ = _get_historical_data(
                 tickers=self._currencies,
                 api_key=self._api_key,
                 source=self._historical_source,
                 start=self._start_date,
@@ -2988,17 +2992,17 @@
                 if progress_bar is not None
                 else self._progress_bar,
             )
 
             income_statement = helpers.convert_currencies(
                 financial_statement_data=income_statement,
                 financial_statement_currencies=self._statement_currencies,
-                exchange_rate_data=self.get_exchange_rates(
-                    period="quarterly" if self._quarterly else "yearly"
-                )["Adj Close"],
+                exchange_rate_data=self._quarterly_exchange_rate_data["Adj Close"]
+                if self._quarterly
+                else self._yearly_exchange_rate_data["Adj Close"],
                 items_not_to_adjust=[
                     "Gross Profit Ratio",
                     "EBITDA Ratio",
                     "Operating Income Ratio",
                     "Income Before Tax Ratio",
                     "Net Income Ratio",
                     "EPS",
@@ -3156,17 +3160,17 @@
                 if progress_bar is not None
                 else self._progress_bar,
             )
 
             cash_flow_statement = helpers.convert_currencies(
                 financial_statement_data=cash_flow_statement,
                 financial_statement_currencies=self._statement_currencies,
-                exchange_rate_data=self.get_exchange_rates(
-                    period="quarterly" if self._quarterly else "yearly"
-                )["Adj Close"],
+                exchange_rate_data=self._quarterly_exchange_rate_data["Adj Close"]
+                if self._quarterly
+                else self._yearly_exchange_rate_data["Adj Close"],
                 financial_statement_name="cash flow statement",
             )
 
         cash_flow_statement = cash_flow_statement.round(
             rounding if rounding else self._rounding
         )
```

### Comparing `financetoolkit-1.8.4/pyproject.toml` & `financetoolkit-1.8.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "financetoolkit"
-version = "1.8.4"
+version = "1.8.5"
 description = "Transparent and Efficient Financial Analysis"
 license = "MIT"
 authors = ["Jeroen Bouma"]
 packages = [
     { include = "financetoolkit" },
 ]
 include = ['normalization/*.csv']
```

### Comparing `financetoolkit-1.8.4/PKG-INFO` & `financetoolkit-1.8.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: financetoolkit
-Version: 1.8.4
-Summary: Transparent and Efficient Financial Analysis
-Home-page: https://www.jeroenbouma.com/projects/financetoolkit
-License: MIT
-Keywords: Finance,Toolkit,Financial,Analysis,Fundamental,Technical,Quantitative,Database,Equities,Currencies,Economics,ETFs,Funds,Indices,Moneymarkets,Commodities,Options
-Author: Jeroen Bouma
-Requires-Python: >=3.10,<3.13
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Dist: pandas[computation,performance,plot] (>=2.2,<3.0)
-Requires-Dist: requests (>=2.31,<3.0)
-Requires-Dist: scikit-learn (>=1.3,<2.0)
-Project-URL: Repository, https://github.com/JerBouma/FinanceToolkit
-Description-Content-Type: text/markdown
-
 [![FinanceToolkit](https://github.com/JerBouma/FinanceToolkit/assets/46355364/198d47bd-e1b3-492d-acc4-5d9f02d1d009)](https://github.com/JerBouma/FinanceToolkit)
 
 [![GitHub Sponsors](https://img.shields.io/badge/Sponsor_this_Project-grey?logo=github)](https://github.com/sponsors/JerBouma)
 [![Buy Me a Coffee](https://img.shields.io/badge/Buy_Me_a_Coffee-grey?logo=buymeacoffee)](https://www.buymeacoffee.com/jerbouma)
 [![Twitter](https://img.shields.io/badge/Twitter-grey?logo=x)](https://twitter.com/JerBouma)
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-grey?logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/boumajeroen/)
 [![Documentation](https://img.shields.io/badge/Documentation-grey?logo=readme)](https://www.jeroenbouma.com/projects/financetoolkit/docs)
@@ -2730,14 +2706,48 @@
 > **Secured Overnight Financing Rate**
 
 The SOFR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data and data on bilateral Treasury repo transactions cleared through FICC’s DVP service, which are obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_federal_reserve_rates).
 
 </details>
 
 <details>
+    <summary><b>Fixed Income 📃 </b></summary>
+
+The fixed income metrics revolve around option-adjusted spreads, effective yields and total returns of corporate bonds based on the ICE BofA US Corporate Indices. It is possible to view both the indices of the ratings (AAA, AA, A, BBB, BB, B and CCC) and the maturities (1-3 years, 3-5 years, 5-7 years, 7-10 years, 10-15 years, 15-30 years and 30+ years).
+
+All fixed income metrics can be called by using `get_` to get a single metric. E.g. `get_option_adjusted_spread` or `get_yield_to_worst`. As an example:
+
+```python
+from financetoolkit import Toolkit
+
+toolkit = Toolkit(["AAPL", "TSLA"], api_key="FINANCIAL_MODELING_PREP_KEY")
+
+# Get Fixed Income Results
+toolkit.economics.get_option_adjusted_spread()
+```
+
+> Option-Adjusted Spread (OAS)
+
+The Option-Adjusted Spread (OAS) is the spread relative to a risk-free interest rate, usually measured in basis points (bp), that equates the theoretical present value of a series of uncertain cash flows to the market price of a fixed-income investment. The spread is added to the risk-free rate to compensate for the uncertainty of the cash flows. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_option_adjusted_spread).
+
+> Effective Yield
+
+The Effective Yield is the yield of a bond, calculated by dividing the bond's coupon payments by its market price. The effective yield is not the same as the stated yield, which is the yield on the bond's coupon payments divided by the bond's principal value. The effective yield is a more accurate measure of a bond's return, as it takes into account the fact that the investor will not hold the bond to maturity and will likely sell it before it matures. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_effective_yield).
+
+> Total Return
+
+The total return is the actual rate of return of an investment or a pool of investments over a given evaluation period. Total return includes interest, capital gains, dividends and distributions realized over a given period of time. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_total_return).
+
+> Yield to Worst
+
+Yield to worst is the lowest potential yield that a bond can generate without the issuer defaulting. The standard US convention for this series is to use semi-annual coupon payments, whereas the standard in the foreign markets is to use coupon payments with frequencies of annual, semi-annual, quarterly, and monthly. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_yield_to_worst).
+
+</details>
+
+<details>
     <summary><b>Environment 💚</b></summary>
 
 The environment metrics revolve around renewable energy, environmental tax, greenhouse gas emissions, crude oil production and crude oil prices of countries. This includes the renewable energy as a percentage of total energy, environmental tax as a percentage of GDP, greenhouse gas emissions, crude oil production and crude oil prices.
 
 All environment metrics can be called by using `get_` to get a single metric. E.g. `get_renewable_energy` or `get_crude_oil_prices`. As an example:
 
 ```python
@@ -2994,8 +3004,7 @@
 - **LinkedIn:** https://www.linkedin.com/in/boumajeroen/
 - **Email:** jer.bouma@gmail.com
 - **Discord:** add me on Discord **`JerBouma`**
 
 If you'd like to support my efforts, either help me out by contributing to the package or [Sponsor Me](https://github.com/sponsors/JerBouma).
 
 [![Star History Chart](https://api.star-history.com/svg?repos=JerBouma/FinanceToolkit&type=Date)](https://star-history.com/#JerBouma/FinanceToolkit&Date)
-
```

