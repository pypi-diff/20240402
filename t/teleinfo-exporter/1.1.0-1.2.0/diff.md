# Comparing `tmp/teleinfo-exporter-1.1.0.tar.gz` & `tmp/teleinfo-exporter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teleinfo-exporter-1.1.0.tar", last modified: Fri Feb 16 17:38:13 2024, max compression
+gzip compressed data, was "teleinfo-exporter-1.2.0.tar", last modified: Tue Apr  2 18:08:05 2024, max compression
```

## Comparing `teleinfo-exporter-1.1.0.tar` & `teleinfo-exporter-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 17:38:13.322998 teleinfo-exporter-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-16 17:37:58.000000 teleinfo-exporter-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-02-16 17:38:13.322998 teleinfo-exporter-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-02-16 17:37:58.000000 teleinfo-exporter-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-02-16 17:37:58.000000 teleinfo-exporter-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 17:38:13.322998 teleinfo-exporter-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 17:38:13.322998 teleinfo-exporter-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 17:38:13.322998 teleinfo-exporter-1.1.0/src/teleinfo_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 17:37:58.000000 teleinfo-exporter-1.1.0/src/teleinfo_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-16 17:37:58.000000 teleinfo-exporter-1.1.0/src/teleinfo_exporter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-02-16 17:37:58.000000 teleinfo-exporter-1.1.0/src/teleinfo_exporter/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 17:38:13.322998 teleinfo-exporter-1.1.0/src/teleinfo_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-02-16 17:38:13.000000 teleinfo-exporter-1.1.0/src/teleinfo_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-16 17:38:13.000000 teleinfo-exporter-1.1.0/src/teleinfo_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 17:38:13.000000 teleinfo-exporter-1.1.0/src/teleinfo_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-16 17:38:13.000000 teleinfo-exporter-1.1.0/src/teleinfo_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-16 17:38:13.000000 teleinfo-exporter-1.1.0/src/teleinfo_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-16 17:38:13.000000 teleinfo-exporter-1.1.0/src/teleinfo_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:08:05.742968 teleinfo-exporter-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 18:07:55.000000 teleinfo-exporter-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-02 18:08:05.742968 teleinfo-exporter-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-02 18:07:55.000000 teleinfo-exporter-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-02 18:07:55.000000 teleinfo-exporter-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:08:05.742968 teleinfo-exporter-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:08:05.742968 teleinfo-exporter-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:08:05.742968 teleinfo-exporter-1.2.0/src/teleinfo_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:07:55.000000 teleinfo-exporter-1.2.0/src/teleinfo_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 18:07:55.000000 teleinfo-exporter-1.2.0/src/teleinfo_exporter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-04-02 18:07:55.000000 teleinfo-exporter-1.2.0/src/teleinfo_exporter/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:08:05.742968 teleinfo-exporter-1.2.0/src/teleinfo_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-02 18:08:05.000000 teleinfo-exporter-1.2.0/src/teleinfo_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-02 18:08:05.000000 teleinfo-exporter-1.2.0/src/teleinfo_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:08:05.000000 teleinfo-exporter-1.2.0/src/teleinfo_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 18:08:05.000000 teleinfo-exporter-1.2.0/src/teleinfo_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 18:08:05.000000 teleinfo-exporter-1.2.0/src/teleinfo_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 18:08:05.000000 teleinfo-exporter-1.2.0/src/teleinfo_exporter.egg-info/top_level.txt
```

### Comparing `teleinfo-exporter-1.1.0/LICENSE` & `teleinfo-exporter-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `teleinfo-exporter-1.1.0/PKG-INFO` & `teleinfo-exporter-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teleinfo-exporter
-Version: 1.1.0
+Version: 1.2.0
 Summary: Simple prometheus exporter for Linky teleinfo.
 Author-email: d3vyce <contact@d3vyce.fr>
 License: MIT License
         
         Copyright (c) 2023 d3vyce
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,18 +44,18 @@
 Requires-Dist: prometheus-client~=0.19
 
 # Teleinfo Exporter
 
 ![Grafana Dashboard](https://grafana.com/api/dashboards/20182/images/15332/image)
 
 Simple prometheus exporter for Linky teleinfo.
-Teleinfo Tasmota project :
-https://github.com/NicolasBernaerts/tasmota/tree/master/teleinfo
-Grafana Dashboard:
-https://grafana.com/grafana/dashboards/20182-linky-teleinfo/
+
+[Teleinfo Tasmota project](https://github.com/NicolasBernaerts/tasmota/tree/master/teleinfo)
+
+[Grafana Dashboard](https://grafana.com/grafana/dashboards/20182-linky-teleinfo/)
 
 ## Installation
 ### Pip
 ```
 python3 -m pip install teleinfo-exporter
 teleinfo-exporter --help
 ```
```

### Comparing `teleinfo-exporter-1.1.0/README.md` & `teleinfo-exporter-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Teleinfo Exporter
 
 ![Grafana Dashboard](https://grafana.com/api/dashboards/20182/images/15332/image)
 
 Simple prometheus exporter for Linky teleinfo.
-Teleinfo Tasmota project :
-https://github.com/NicolasBernaerts/tasmota/tree/master/teleinfo
-Grafana Dashboard:
-https://grafana.com/grafana/dashboards/20182-linky-teleinfo/
+
+[Teleinfo Tasmota project](https://github.com/NicolasBernaerts/tasmota/tree/master/teleinfo)
+
+[Grafana Dashboard](https://grafana.com/grafana/dashboards/20182-linky-teleinfo/)
 
 ## Installation
 ### Pip
 ```
 python3 -m pip install teleinfo-exporter
 teleinfo-exporter --help
 ```
```

### Comparing `teleinfo-exporter-1.1.0/pyproject.toml` & `teleinfo-exporter-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "teleinfo-exporter"
-version = "1.1.0"
+version = "1.2.0"
 dependencies = [
   "bcrypt ~= 4.1",
   "configargparse ~= 1.7",
   "flask ~= 3.0",
   "flask-httpauth ~= 4.8",
   "paho-mqtt ~= 1.6",
   "prometheus-client ~= 0.19",
```

### Comparing `teleinfo-exporter-1.1.0/src/teleinfo_exporter/app.py` & `teleinfo-exporter-1.2.0/src/teleinfo_exporter/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -97,59 +97,69 @@
     if rc == 0:
         print("Connected to broker")
     else:
         print("Connection failed")
 
 
 def on_message(client, userdata, message):  # pylint: disable=unused-argument
-    message = json.loads(message.payload.decode("utf-8"))
+    try:
+        message = json.loads(message.payload.decode("utf-8"))
+    except UnicodeDecodeError:
+        pass
+
     if "ENERGY" in message:
-        teleinfo_total.set(message["ENERGY"]["Total"])
-        teleinfo_yesterday.set(message["ENERGY"]["Yesterday"])
-        teleinfo_today.set(message["ENERGY"]["Today"])
-        teleinfo_power.set(message["ENERGY"]["Power"])
-        teleinfo_apparent_power.set(message["ENERGY"]["ApparentPower"])
-        teleinfo_reactive_power.set(message["ENERGY"]["ReactivePower"])
-        teleinfo_power_factor.set(message["ENERGY"]["Factor"])
-        teleinfo_voltage.set(message["ENERGY"]["Voltage"])
-        teleinfo_current.set(message["ENERGY"]["Current"])
+        teleinfo_total.set(message.get("ENERGY", {}).get("Total", 0))
+        teleinfo_yesterday.set(message.get("ENERGY", {}).get("Yesterday", 0))
+        teleinfo_today.set(message.get("ENERGY", {}).get("Today", 0))
+        teleinfo_power.set(message.get("ENERGY", {}).get("Power", 0))
+        teleinfo_apparent_power.set(message.get("ENERGY", {}).get("ApparentPower", 0))
+        teleinfo_reactive_power.set(message.get("ENERGY", {}).get("ReactivePower", 0))
+        teleinfo_power_factor.set(message.get("ENERGY", {}).get("Factor", 0))
+        teleinfo_voltage.set(message.get("ENERGY", {}).get("Voltage", 0))
+        teleinfo_current.set(message.get("ENERGY", {}).get("Current", 0))
     elif "METER" in message:
-        teleinfo_phases_count.set(message["METER"]["PH"])
-        teleinfo_max_current_per_phase.set(message["METER"]["ISUB"])
-        teleinfo_max_power_per_phase.set(message["METER"]["PSUB"])
-        teleinfo_max_power_per_phase_with_overload.set(message["METER"]["PMAX"])
-        teleinfo_total_apparent_power.set(message["METER"]["P"])
-        teleinfo_total_active_power.set(message["METER"]["W"])
-        teleinfo_total_current.set(message["METER"]["I"])
+        teleinfo_phases_count.set(message.get("METER", {}).get("PH", 0))
+        teleinfo_max_current_per_phase.set(message.get("METER", {}).get("ISUB", 0))
+        teleinfo_max_power_per_phase.set(message.get("METER", {}).get("PSUB", 0))
+        teleinfo_max_power_per_phase_with_overload.set(
+            message.get("METER", {}).get("PMAX", 0)
+        )
+        teleinfo_total_apparent_power.set(message.get("METER", {}).get("P", 0))
+        teleinfo_total_active_power.set(message.get("METER", {}).get("W", 0))
+        teleinfo_total_current.set(message.get("METER", {}).get("I", 0))
         for i in range(1, 4):
-            if not message["METER"].get(f"U{i}"):
+            if not message.get("METER", {}).get(f"U{i}"):
                 break
             teleinfo_instant_voltage_per_phase.labels(f"U{i}").set(
-                message["METER"][f"U{i}"]
+                message.get("METER", {}).get(f"U{i}", 0)
             )
             teleinfo_instant_apparent_power_per_phase.labels(f"P{i}").set(
-                message["METER"][f"P{i}"]
+                message.get("METER", {}).get(f"P{i}", 0)
             )
             teleinfo_instant_active_power_per_phase.labels(f"W{i}").set(
-                message["METER"][f"W{i}"]
+                message.get("METER", {}).get(f"W{i}", 0)
             )
             teleinfo_instant_current_per_phase.labels(f"I{i}").set(
-                message["METER"][f"I{i}"]
+                message.get("METER", {}).get(f"I{i}", 0)
             )
             teleinfo_power_factor_per_phase.labels(f"C{i}").set(
-                message["METER"][f"C{i}"]
+                message.get("METER", {}).get(f"C{i}", 0)
             )
 
     elif "PROD" in message:
-        teleinfo_production_instant_apparent_power.set(message["PROD"]["VA"])
-        teleinfo_production_instant_active_power.set(message["PROD"]["W"])
-        teleinfo_production_power_factor.set(message["PROD"]["COS"])
+        teleinfo_production_instant_apparent_power.set(
+            message.get("PROD", {}).get("VA", 0)
+        )
+        teleinfo_production_instant_active_power.set(
+            message.get("PROD", {}).get("W", 0)
+        )
+        teleinfo_production_power_factor.set(message.get("PROD", {}).get("COS", 0))
     elif "TIC" in message:
-        teleinfo_contract_number.labels(message["TIC"]["ADCO"]).set(0)
-        teleinfo_contract_type.labels(message["TIC"]["OPTARIF"]).set(0)
+        teleinfo_contract_number.labels(message.get("TIC", {}).get("ADCO", 0)).set(0)
+        teleinfo_contract_type.labels(message.get("TIC", {}).get("OPTARIF", 0)).set(0)
 
 
 def on_disconnect(client, userdata, rc):  # pylint: disable=unused-argument
     print("Diconnected from broker, reconnecting...")
     while True:
         try:
             if not client.reconnect():
```

### Comparing `teleinfo-exporter-1.1.0/src/teleinfo_exporter.egg-info/PKG-INFO` & `teleinfo-exporter-1.2.0/src/teleinfo_exporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teleinfo-exporter
-Version: 1.1.0
+Version: 1.2.0
 Summary: Simple prometheus exporter for Linky teleinfo.
 Author-email: d3vyce <contact@d3vyce.fr>
 License: MIT License
         
         Copyright (c) 2023 d3vyce
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,18 +44,18 @@
 Requires-Dist: prometheus-client~=0.19
 
 # Teleinfo Exporter
 
 ![Grafana Dashboard](https://grafana.com/api/dashboards/20182/images/15332/image)
 
 Simple prometheus exporter for Linky teleinfo.
-Teleinfo Tasmota project :
-https://github.com/NicolasBernaerts/tasmota/tree/master/teleinfo
-Grafana Dashboard:
-https://grafana.com/grafana/dashboards/20182-linky-teleinfo/
+
+[Teleinfo Tasmota project](https://github.com/NicolasBernaerts/tasmota/tree/master/teleinfo)
+
+[Grafana Dashboard](https://grafana.com/grafana/dashboards/20182-linky-teleinfo/)
 
 ## Installation
 ### Pip
 ```
 python3 -m pip install teleinfo-exporter
 teleinfo-exporter --help
 ```
```

