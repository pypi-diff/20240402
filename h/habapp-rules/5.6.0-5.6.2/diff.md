# Comparing `tmp/habapp_rules-5.6.0.tar.gz` & `tmp/habapp_rules-5.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habapp_rules-5.6.0.tar", last modified: Sun Mar 24 15:20:35 2024, max compression
+gzip compressed data, was "habapp_rules-5.6.2.tar", last modified: Tue Apr  2 17:59:51 2024, max compression
```

## Comparing `habapp_rules-5.6.0.tar` & `habapp_rules-5.6.2.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.431302 habapp_rules-5.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-24 15:20:35.431302 habapp_rules-5.6.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.419302 habapp_rules-5.6.0/habapp_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.423302 habapp_rules-5.6.0/habapp_rules/actors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.423302 habapp_rules-5.6.0/habapp_rules/actors/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/config/light.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/config/light_hcl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/config/shading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/config/ventilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/irrigation.py
--rw-r--r--   0 runner    (1001) docker     (127)    38658 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/light.py
--rw-r--r--   0 runner    (1001) docker     (127)    16197 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/light_hcl.py
--rw-r--r--   0 runner    (1001) docker     (127)    36944 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/shading.py
--rw-r--r--   0 runner    (1001) docker     (127)    19218 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/state_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)    29831 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/ventilation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.423302 habapp_rules-5.6.0/habapp_rules/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/bridge/knx_mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.427302 habapp_rules-5.6.0/habapp_rules/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/common/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/common/hysteresis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/common/logic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.427302 habapp_rules-5.6.0/habapp_rules/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/state_machine_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/timeout_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/type_of_day.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.427302 habapp_rules-5.6.0/habapp_rules/energy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/energy/donut_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/energy/monthly_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.427302 habapp_rules-5.6.0/habapp_rules/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/sensors/astro.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/sensors/dwd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/sensors/motion.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/sensors/sun.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.431302 habapp_rules-5.6.0/habapp_rules/system/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/system/presence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11767 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/system/sleep.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/system/summer_winter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.431302 habapp_rules-5.6.0/habapp_rules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-24 15:20:35.000000 habapp_rules-5.6.0/habapp_rules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-24 15:20:35.000000 habapp_rules-5.6.0/habapp_rules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 15:20:35.000000 habapp_rules-5.6.0/habapp_rules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-24 15:20:35.000000 habapp_rules-5.6.0/habapp_rules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-24 15:20:35.000000 habapp_rules-5.6.0/habapp_rules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 15:20:35.431302 habapp_rules-5.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:51.901070 habapp_rules-5.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-02 17:59:51.901070 habapp_rules-5.6.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:51.889070 habapp_rules-5.6.2/habapp_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:51.893070 habapp_rules-5.6.2/habapp_rules/actors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/actors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:51.893070 habapp_rules-5.6.2/habapp_rules/actors/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/actors/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/actors/config/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/actors/config/light_hcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/actors/config/shading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/actors/config/ventilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/actors/irrigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38658 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/actors/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16197 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/actors/light_hcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36944 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/actors/shading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19218 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/actors/state_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29962 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/actors/ventilation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:51.893070 habapp_rules-5.6.2/habapp_rules/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/bridge/knx_mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:51.893070 habapp_rules-5.6.2/habapp_rules/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/common/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/common/hysteresis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/common/logic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:51.897070 habapp_rules-5.6.2/habapp_rules/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/core/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/core/state_machine_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/core/timeout_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/core/type_of_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:51.897070 habapp_rules-5.6.2/habapp_rules/energy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/energy/donut_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/energy/monthly_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/energy/monthly_report_template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:51.897070 habapp_rules-5.6.2/habapp_rules/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/sensors/astro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/sensors/dwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/sensors/motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/sensors/sun.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:51.897070 habapp_rules-5.6.2/habapp_rules/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/system/presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11767 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/system/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/habapp_rules/system/summer_winter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:59:51.901070 habapp_rules-5.6.2/habapp_rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-02 17:59:51.000000 habapp_rules-5.6.2/habapp_rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-02 17:59:51.000000 habapp_rules-5.6.2/habapp_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 17:59:51.000000 habapp_rules-5.6.2/habapp_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-02 17:59:51.000000 habapp_rules-5.6.2/habapp_rules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 17:59:51.000000 habapp_rules-5.6.2/habapp_rules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 17:59:51.901070 habapp_rules-5.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 17:59:37.000000 habapp_rules-5.6.2/setup.py
```

### Comparing `habapp_rules-5.6.0/LICENCE` & `habapp_rules-5.6.2/LICENCE`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/actors/config/light.py` & `habapp_rules-5.6.2/habapp_rules/actors/config/light.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/actors/config/light_hcl.py` & `habapp_rules-5.6.2/habapp_rules/actors/config/light_hcl.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/actors/config/shading.py` & `habapp_rules-5.6.2/habapp_rules/actors/config/shading.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/actors/config/ventilation.py` & `habapp_rules-5.6.2/habapp_rules/actors/config/ventilation.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/actors/irrigation.py` & `habapp_rules-5.6.2/habapp_rules/actors/irrigation.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/actors/light.py` & `habapp_rules-5.6.2/habapp_rules/actors/light.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/actors/light_hcl.py` & `habapp_rules-5.6.2/habapp_rules/actors/light_hcl.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/actors/shading.py` & `habapp_rules-5.6.2/habapp_rules/actors/shading.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/actors/state_observer.py` & `habapp_rules-5.6.2/habapp_rules/actors/state_observer.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/actors/ventilation.py` & `habapp_rules-5.6.2/habapp_rules/actors/ventilation.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,19 @@
 
 	def on_enter_Auto_Init(self) -> None:  # pylint: disable=invalid-name
 		"""Is called on entering of Auto_Init state"""
 		self._set_initial_state()
 
 	def on_enter_Auto_LongAbsence_Off(self):  # pylint: disable=invalid-name
 		"""Is called on entering of Auto_LongAbsence_Off state."""
-		self.run.at(self._config.state_long_absence.start_time, self._long_absence_power_on)
+		self.run.at(self._config.state_long_absence.start_time, self._trigger_long_absence_power_on)
+
+	def _trigger_long_absence_power_on(self) -> None:
+		"""Trigger long absence power on."""
+		self._long_absence_power_on()
 
 	def _external_active_and_configured(self) -> bool:
 		"""Check if external request is active and configured.
 
 		:return: True if external request is active and configured
 		"""
 		return self._item_external_request is not None and self._item_external_request.is_on()
```

### Comparing `habapp_rules-5.6.0/habapp_rules/bridge/knx_mqtt.py` & `habapp_rules-5.6.2/habapp_rules/bridge/knx_mqtt.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/common/filter.py` & `habapp_rules-5.6.2/habapp_rules/common/filter.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/common/hysteresis.py` & `habapp_rules-5.6.2/habapp_rules/common/hysteresis.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/common/logic.py` & `habapp_rules-5.6.2/habapp_rules/common/logic.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/core/helper.py` & `habapp_rules-5.6.2/habapp_rules/core/helper.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/core/logger.py` & `habapp_rules-5.6.2/habapp_rules/core/logger.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/core/state_machine_rule.py` & `habapp_rules-5.6.2/habapp_rules/core/state_machine_rule.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/core/timeout_list.py` & `habapp_rules-5.6.2/habapp_rules/core/timeout_list.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/core/type_of_day.py` & `habapp_rules-5.6.2/habapp_rules/core/type_of_day.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/core/version.py` & `habapp_rules-5.6.2/habapp_rules/core/version.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/energy/donut_chart.py` & `habapp_rules-5.6.2/habapp_rules/energy/donut_chart.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/energy/monthly_report.py` & `habapp_rules-5.6.2/habapp_rules/energy/monthly_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import tempfile
 
 import HABApp
 import HABApp.core.internals
 import dateutil.relativedelta
 import jinja2
 import multi_notifier.connectors.connector_mail
+import pkg_resources
 
 import habapp_rules.__version__
 import habapp_rules.core.exceptions
 import habapp_rules.core.logger
 import habapp_rules.energy.donut_chart
 
 LOGGER = logging.getLogger(__name__)
@@ -106,22 +107,24 @@
 
 	def __init__(
 			self,
 			name_energy_sum: str,
 			known_energy_share: list[EnergyShare],
 			persistence_group_name: str | None,
 			config_mail: multi_notifier.connectors.connector_mail.MailConfig | None,
-			recipients: str | list[str]) -> None:
+			recipients: str | list[str],
+			debug: bool = False) -> None:
 		"""Initialize the rule.
 
 		:param name_energy_sum: name of OpenHAB Number item, which holds the total energy consumption (NumberItem)
 		:param known_energy_share: list of EnergyShare objects
 		:param persistence_group_name: OpenHAB group name which holds all items which are persisted. If the group name is given it will be checked if all energy items are in the group
 		:param config_mail: config for sending mails
 		:param recipients: list of recipients who get the mail
+		:param debug: if debug mode is active
 		:raises habapp_rules.core.exceptions.HabAppRulesConfigurationException: if config is not valid
 		"""
 		HABApp.Rule.__init__(self)
 		self._instance_logger = habapp_rules.core.logger.InstanceLogger(LOGGER, name_energy_sum)
 		self._recipients = recipients
 
 		self._item_energy_sum = HABApp.openhab.items.NumberItem.get_item(name_energy_sum)
@@ -132,14 +135,17 @@
 			# check if all energy items are in the given persistence group
 			items_to_check = [self._item_energy_sum] + [share.openhab_item for share in self._known_energy_share]
 			not_in_persistence_group = [item.name for item in items_to_check if persistence_group_name not in item.groups]
 			if not_in_persistence_group:
 				raise habapp_rules.core.exceptions.HabAppRulesConfigurationException(f"The following OpenHAB items are not in the persistence group '{persistence_group_name}': {not_in_persistence_group}")
 
 		self.run.at(next_trigger_time := _get_next_trigger(), self._cb_send_energy)
+		if debug:
+			self._instance_logger.warning("Debug mode is active!")
+			self.run.soon(self._cb_send_energy)
 		self._instance_logger.info(f"Successfully initiated monthly consumption rule for {name_energy_sum}. Triggered first execution to {next_trigger_time.isoformat()}")
 
 	def _get_historic_value(self, item: HABApp.openhab.items.NumberItem, start_time: datetime.datetime) -> float:
 		"""Get historic value of given Number item
 
 		:param item: item instance
 		:param start_time: start time to search for the interested value
@@ -184,18 +190,15 @@
 		           <p style="font-size: 0.6em">Generated with habapp_rules version = 20.0.3</p>
 		        </div>
 		      </div>
 		    </div>
 		  </body>
 		</html>
 		"""
-		html_template_path = pathlib.Path(__file__).parent / "monthly_report_template.html"
-
-		with html_template_path.open() as html_template_file:
-			html_template = html_template_file.read()
+		html_template = pkg_resources.resource_string("habapp_rules.energy", "monthly_report_template.html").decode("utf-8")
 
 		return jinja2.Template(html_template).render(
 			month=_get_previous_month_name(),
 			energy_now=f"{self._item_energy_sum.value:.1f}",
 			energy_last_month=f"{energy_sum_month:.1f}",
 			habapp_version=habapp_rules.__version__.__version__,
 			chart="{{ chart }}"  # this is needed to not replace the chart from the mail-template
```

### Comparing `habapp_rules-5.6.0/habapp_rules/sensors/astro.py` & `habapp_rules-5.6.2/habapp_rules/sensors/astro.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/sensors/dwd.py` & `habapp_rules-5.6.2/habapp_rules/sensors/dwd.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/sensors/motion.py` & `habapp_rules-5.6.2/habapp_rules/sensors/motion.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/sensors/sun.py` & `habapp_rules-5.6.2/habapp_rules/sensors/sun.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/system/presence.py` & `habapp_rules-5.6.2/habapp_rules/system/presence.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/system/sleep.py` & `habapp_rules-5.6.2/habapp_rules/system/sleep.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules/system/summer_winter.py` & `habapp_rules-5.6.2/habapp_rules/system/summer_winter.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.6.0/habapp_rules.egg-info/SOURCES.txt` & `habapp_rules-5.6.2/habapp_rules.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 habapp_rules/core/state_machine_rule.py
 habapp_rules/core/timeout_list.py
 habapp_rules/core/type_of_day.py
 habapp_rules/core/version.py
 habapp_rules/energy/__init__.py
 habapp_rules/energy/donut_chart.py
 habapp_rules/energy/monthly_report.py
+habapp_rules/energy/monthly_report_template.html
 habapp_rules/sensors/__init__.py
 habapp_rules/sensors/astro.py
 habapp_rules/sensors/dwd.py
 habapp_rules/sensors/motion.py
 habapp_rules/sensors/sun.py
 habapp_rules/system/__init__.py
 habapp_rules/system/presence.py
```

### Comparing `habapp_rules-5.6.0/setup.py` & `habapp_rules-5.6.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,9 +18,8 @@
 	author="Seuling N.",
 	description="Basic rules for HABApp",
 	long_description="Basic rules for HABApp",
 	packages=setuptools.find_packages(exclude=["tests*", "rules*"]),
 	install_requires=load_req(),
 	python_requires=">=3.10",
 	license="Apache License 2.0",
-	include_package_data=True
-)
+	package_data={'': ['*.html']})
```

