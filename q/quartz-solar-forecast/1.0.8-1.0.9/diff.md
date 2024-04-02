# Comparing `tmp/quartz_solar_forecast-1.0.8.tar.gz` & `tmp/quartz_solar_forecast-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quartz_solar_forecast-1.0.8.tar", last modified: Sun Feb 25 10:24:41 2024, max compression
+gzip compressed data, was "quartz_solar_forecast-1.0.9.tar", last modified: Sun Feb 25 10:25:58 2024, max compression
```

## Comparing `quartz_solar_forecast-1.0.8.tar` & `quartz_solar_forecast-1.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:24:41.270788 quartz_solar_forecast-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-02-25 10:24:41.270788 quartz_solar_forecast-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   101720 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/predictions.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:24:41.266787 quartz_solar_forecast-1.0.8/quartz_solar_forecast/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:24:41.266787 quartz_solar_forecast-1.0.8/quartz_solar_forecast/eval/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/eval/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/eval/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/eval/nwp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/eval/pv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/eval/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:24:41.270788 quartz_solar_forecast-1.0.8/quartz_solar_forecast/forecasts/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/forecasts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/forecasts/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:24:41.270788 quartz_solar_forecast-1.0.8/quartz_solar_forecast/models/
--rw-r--r--   0 runner    (1001) docker     (127)   366099 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/models/model-0.3.0.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast/pydantic_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:24:41.270788 quartz_solar_forecast-1.0.8/quartz_solar_forecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-02-25 10:24:41.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-25 10:24:41.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 10:24:41.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 10:24:41.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 10:24:41.000000 quartz_solar_forecast-1.0.8/quartz_solar_forecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 10:24:41.270788 quartz_solar_forecast-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:24:41.270788 quartz_solar_forecast-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/tests/test_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-25 10:24:30.000000 quartz_solar_forecast-1.0.8/tests/test_forecast_no_ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:25:58.746709 quartz_solar_forecast-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-02-25 10:25:58.746709 quartz_solar_forecast-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   101720 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/predictions.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:25:58.742709 quartz_solar_forecast-1.0.9/quartz_solar_forecast/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:25:58.742709 quartz_solar_forecast-1.0.9/quartz_solar_forecast/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/eval/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/eval/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/eval/nwp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/eval/pv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/eval/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:25:58.746709 quartz_solar_forecast-1.0.9/quartz_solar_forecast/forecasts/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/forecasts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/forecasts/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:25:58.746709 quartz_solar_forecast-1.0.9/quartz_solar_forecast/models/
+-rw-r--r--   0 runner    (1001) docker     (127)   366099 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/models/model-0.3.0.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast/pydantic_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:25:58.746709 quartz_solar_forecast-1.0.9/quartz_solar_forecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-02-25 10:25:58.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-25 10:25:58.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 10:25:58.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 10:25:58.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 10:25:58.000000 quartz_solar_forecast-1.0.9/quartz_solar_forecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 10:25:58.746709 quartz_solar_forecast-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 10:25:58.746709 quartz_solar_forecast-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/tests/test_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-25 10:25:39.000000 quartz_solar_forecast-1.0.9/tests/test_forecast_no_ts.py
```

### Comparing `quartz_solar_forecast-1.0.8/LICENSE` & `quartz_solar_forecast-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/PKG-INFO` & `quartz_solar_forecast-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartz_solar_forecast
-Version: 1.0.8
+Version: 1.0.9
 Summary: Open Source Solar Forecasting for a Site
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
@@ -12,15 +12,15 @@
 Requires-Dist: pv-site-prediction
 Requires-Dist: pydantic
 Requires-Dist: huggingface_hub
 Requires-Dist: python-dotenv
 
 # Quartz Solar Forecast
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-8-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 The aim of the project is to build an open source PV forecast that is free and easy to use.
 The forecast provides the expected generation in `kw` for 0 to 48 hours for a single PV site.
 
 Open Climate Fix also provides a commercial PV forecast, please get in touch at quartz.support@openclimatefix.org
 
@@ -151,14 +151,17 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/zakwatts"><img src="https://avatars.githubusercontent.com/u/47150349?v=4?s=100" width="100px;" alt="Megawattz"/><br /><sub><b>Megawattz</b></sub></a><br /><a href="#ideas-zakwatts" title="Ideas, Planning, & Feedback">🤔</a> <a href="#talk-zakwatts" title="Talks">📢</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/EdFage"><img src="https://avatars.githubusercontent.com/u/87755165?v=4?s=100" width="100px;" alt="EdFage"/><br /><sub><b>EdFage</b></sub></a><br /><a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=EdFage" title="Documentation">📖</a> <a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=EdFage" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/chloepilonv"><img src="https://avatars.githubusercontent.com/u/136987461?v=4?s=100" width="100px;" alt="Chloe Pilon Vaillancourt"/><br /><sub><b>Chloe Pilon Vaillancourt</b></sub></a><br /><a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=chloepilonv" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://racheltipton.dev"><img src="https://avatars.githubusercontent.com/u/86949265?v=4?s=100" width="100px;" alt="rachel tipton"/><br /><sub><b>rachel tipton</b></sub></a><br /><a href="#talk-rachel-labri-tipton" title="Talks">📢</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/armenbod"><img src="https://avatars.githubusercontent.com/u/84937223?v=4?s=100" width="100px;" alt="armenbod"/><br /><sub><b>armenbod</b></sub></a><br /><a href="#content-armenbod" title="Content">🖋</a> <a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=armenbod" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/shreyasudaya"><img src="https://avatars.githubusercontent.com/u/94735680?v=4?s=100" width="100px;" alt="Shreyas Udaya"/><br /><sub><b>Shreyas Udaya</b></sub></a><br /><a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=shreyasudaya" title="Documentation">📖</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="http://github.com/aryanbhosale"><img src="https://avatars.githubusercontent.com/u/36108149?v=4?s=100" width="100px;" alt="Aryan Bhosale"/><br /><sub><b>Aryan Bhosale</b></sub></a><br /><a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=aryanbhosale" title="Documentation">📖</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `quartz_solar_forecast-1.0.8/README.md` & `quartz_solar_forecast-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Quartz Solar Forecast
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-8-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 The aim of the project is to build an open source PV forecast that is free and easy to use.
 The forecast provides the expected generation in `kw` for 0 to 48 hours for a single PV site.
 
 Open Climate Fix also provides a commercial PV forecast, please get in touch at quartz.support@openclimatefix.org
 
@@ -135,14 +135,17 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/zakwatts"><img src="https://avatars.githubusercontent.com/u/47150349?v=4?s=100" width="100px;" alt="Megawattz"/><br /><sub><b>Megawattz</b></sub></a><br /><a href="#ideas-zakwatts" title="Ideas, Planning, & Feedback">🤔</a> <a href="#talk-zakwatts" title="Talks">📢</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/EdFage"><img src="https://avatars.githubusercontent.com/u/87755165?v=4?s=100" width="100px;" alt="EdFage"/><br /><sub><b>EdFage</b></sub></a><br /><a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=EdFage" title="Documentation">📖</a> <a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=EdFage" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/chloepilonv"><img src="https://avatars.githubusercontent.com/u/136987461?v=4?s=100" width="100px;" alt="Chloe Pilon Vaillancourt"/><br /><sub><b>Chloe Pilon Vaillancourt</b></sub></a><br /><a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=chloepilonv" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://racheltipton.dev"><img src="https://avatars.githubusercontent.com/u/86949265?v=4?s=100" width="100px;" alt="rachel tipton"/><br /><sub><b>rachel tipton</b></sub></a><br /><a href="#talk-rachel-labri-tipton" title="Talks">📢</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/armenbod"><img src="https://avatars.githubusercontent.com/u/84937223?v=4?s=100" width="100px;" alt="armenbod"/><br /><sub><b>armenbod</b></sub></a><br /><a href="#content-armenbod" title="Content">🖋</a> <a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=armenbod" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/shreyasudaya"><img src="https://avatars.githubusercontent.com/u/94735680?v=4?s=100" width="100px;" alt="Shreyas Udaya"/><br /><sub><b>Shreyas Udaya</b></sub></a><br /><a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=shreyasudaya" title="Documentation">📖</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="http://github.com/aryanbhosale"><img src="https://avatars.githubusercontent.com/u/36108149?v=4?s=100" width="100px;" alt="Aryan Bhosale"/><br /><sub><b>Aryan Bhosale</b></sub></a><br /><a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=aryanbhosale" title="Documentation">📖</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `quartz_solar_forecast-1.0.8/predictions.png` & `quartz_solar_forecast-1.0.9/predictions.png`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/quartz_solar_forecast/data.py` & `quartz_solar_forecast-1.0.9/quartz_solar_forecast/data.py`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/quartz_solar_forecast/eval/forecast.py` & `quartz_solar_forecast-1.0.9/quartz_solar_forecast/eval/forecast.py`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/quartz_solar_forecast/eval/metrics.py` & `quartz_solar_forecast-1.0.9/quartz_solar_forecast/eval/metrics.py`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/quartz_solar_forecast/eval/nwp.py` & `quartz_solar_forecast-1.0.9/quartz_solar_forecast/eval/nwp.py`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/quartz_solar_forecast/eval/pv.py` & `quartz_solar_forecast-1.0.9/quartz_solar_forecast/eval/pv.py`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/quartz_solar_forecast/eval/utils.py` & `quartz_solar_forecast-1.0.9/quartz_solar_forecast/eval/utils.py`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/quartz_solar_forecast/evaluation.py` & `quartz_solar_forecast-1.0.9/quartz_solar_forecast/evaluation.py`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/quartz_solar_forecast/forecast.py` & `quartz_solar_forecast-1.0.9/quartz_solar_forecast/forecast.py`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/quartz_solar_forecast/forecasts/v1.py` & `quartz_solar_forecast-1.0.9/quartz_solar_forecast/forecasts/v1.py`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/quartz_solar_forecast/models/model-0.3.0.pkl` & `quartz_solar_forecast-1.0.9/quartz_solar_forecast/models/model-0.3.0.pkl`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/quartz_solar_forecast/pydantic_models.py` & `quartz_solar_forecast-1.0.9/quartz_solar_forecast/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/quartz_solar_forecast.egg-info/PKG-INFO` & `quartz_solar_forecast-1.0.9/quartz_solar_forecast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartz_solar_forecast
-Version: 1.0.8
+Version: 1.0.9
 Summary: Open Source Solar Forecasting for a Site
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
@@ -12,15 +12,15 @@
 Requires-Dist: pv-site-prediction
 Requires-Dist: pydantic
 Requires-Dist: huggingface_hub
 Requires-Dist: python-dotenv
 
 # Quartz Solar Forecast
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-8-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 The aim of the project is to build an open source PV forecast that is free and easy to use.
 The forecast provides the expected generation in `kw` for 0 to 48 hours for a single PV site.
 
 Open Climate Fix also provides a commercial PV forecast, please get in touch at quartz.support@openclimatefix.org
 
@@ -151,14 +151,17 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/zakwatts"><img src="https://avatars.githubusercontent.com/u/47150349?v=4?s=100" width="100px;" alt="Megawattz"/><br /><sub><b>Megawattz</b></sub></a><br /><a href="#ideas-zakwatts" title="Ideas, Planning, & Feedback">🤔</a> <a href="#talk-zakwatts" title="Talks">📢</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/EdFage"><img src="https://avatars.githubusercontent.com/u/87755165?v=4?s=100" width="100px;" alt="EdFage"/><br /><sub><b>EdFage</b></sub></a><br /><a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=EdFage" title="Documentation">📖</a> <a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=EdFage" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/chloepilonv"><img src="https://avatars.githubusercontent.com/u/136987461?v=4?s=100" width="100px;" alt="Chloe Pilon Vaillancourt"/><br /><sub><b>Chloe Pilon Vaillancourt</b></sub></a><br /><a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=chloepilonv" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://racheltipton.dev"><img src="https://avatars.githubusercontent.com/u/86949265?v=4?s=100" width="100px;" alt="rachel tipton"/><br /><sub><b>rachel tipton</b></sub></a><br /><a href="#talk-rachel-labri-tipton" title="Talks">📢</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/armenbod"><img src="https://avatars.githubusercontent.com/u/84937223?v=4?s=100" width="100px;" alt="armenbod"/><br /><sub><b>armenbod</b></sub></a><br /><a href="#content-armenbod" title="Content">🖋</a> <a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=armenbod" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/shreyasudaya"><img src="https://avatars.githubusercontent.com/u/94735680?v=4?s=100" width="100px;" alt="Shreyas Udaya"/><br /><sub><b>Shreyas Udaya</b></sub></a><br /><a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=shreyasudaya" title="Documentation">📖</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="http://github.com/aryanbhosale"><img src="https://avatars.githubusercontent.com/u/36108149?v=4?s=100" width="100px;" alt="Aryan Bhosale"/><br /><sub><b>Aryan Bhosale</b></sub></a><br /><a href="https://github.com/openclimatefix/Open-Source-Quartz-Solar-Forecast/commits?author=aryanbhosale" title="Documentation">📖</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `quartz_solar_forecast-1.0.8/quartz_solar_forecast.egg-info/SOURCES.txt` & `quartz_solar_forecast-1.0.9/quartz_solar_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quartz_solar_forecast-1.0.8/setup.py` & `quartz_solar_forecast-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 
 setup(
     name="quartz_solar_forecast",
-    version="1.0.8",
+    version="1.0.9",
     license="MIT",
     author="Peter Dudfield",
     author_email="info@openclimatefix.org",
     company="Open Climate Fix Ltd",
     install_requires=install_requires,
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `quartz_solar_forecast-1.0.8/tests/test_forecast_no_ts.py` & `quartz_solar_forecast-1.0.9/tests/test_forecast_no_ts.py`

 * *Files identical despite different names*

