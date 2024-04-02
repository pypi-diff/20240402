# Comparing `tmp/smartboiler-0.0.3.0.0.5.8.7.tar.gz` & `tmp/smartboiler-0.0.3.0.0.5.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.0.3.0.0.5.8.7.tar", last modified: Mon Apr  1 06:29:38 2024, max compression
+gzip compressed data, was "smartboiler-0.0.3.0.0.5.8.9.tar", last modified: Tue Apr  2 20:16:27 2024, max compression
```

## Comparing `smartboiler-0.0.3.0.0.5.8.7.tar` & `smartboiler-0.0.3.0.0.5.8.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:29:38.714288 smartboiler-0.0.3.0.0.5.8.7/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-01 06:29:38.714288 smartboiler-0.0.3.0.0.5.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 06:29:38.714288 smartboiler-0.0.3.0.0.5.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-01 06:29:36.000000 smartboiler-0.0.3.0.0.5.8.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:29:38.710288 smartboiler-0.0.3.0.0.5.8.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:29:38.710288 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    36881 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    36915 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/retrieve_hass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:29:38.714288 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:29:38.714288 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/time_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    42745 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/web_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-01 06:29:32.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/week_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:29:38.714288 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-01 06:29:38.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-01 06:29:38.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 06:29:38.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 06:29:38.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-01 06:29:38.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 06:29:38.000000 smartboiler-0.0.3.0.0.5.8.7/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-02 20:16:25.000000 smartboiler-0.0.3.0.0.5.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:16:27.192939 smartboiler-0.0.3.0.0.5.8.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36881 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21278 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36915 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/retrieve_hass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/time_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42745 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/web_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-02 20:16:21.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/week_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:16:27.196939 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-02 20:16:27.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-02 20:16:27.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:16:27.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 20:16:27.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-02 20:16:27.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 20:16:27.000000 smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.0.3.0.0.5.8.7/PKG-INFO` & `smartboiler-0.0.3.0.0.5.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.5.8.7
+Version: 0.0.3.0.0.5.8.9
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.5.8.7/README.md` & `smartboiler-0.0.3.0.0.5.8.9/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/setup.py` & `smartboiler-0.0.3.0.0.5.8.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='smartboiler',  # Required
-    version='0.0.3.0.0.5.8.7',  # Required
+    version='0.0.3.0.0.5.8.9',  # Required
     description='Smart boiling of household',  # Optional
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/grinwi/smartboiler',  # Optional
     author='Adam GRUNWALD',  # Optional
     author_email='grunwald.adam24@gmail.com',  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/boiler.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/boiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         """
         Calculates the time needed for heating water in boiler by temperature delta.
             time = (m * c) * d'(tmp) / P * effectivity_coef
 
             https://vytapeni.tzb-info.cz/tabulky-a-vypocty/97-vypocet-doby-ohrevu-teple-vody
         """
 
-        return ( consumption_kWh / (self.real_wattage / 1000)) * 60
+        return (( consumption_kWh / (self.real_wattage / 1000)) * 60)
     
     def get_kWh_delta_from_temperatures(self, tmp_act: int, tmp_goal: int):
         return ( 4.186 * self.capacity * (tmp_goal - tmp_act) / 3600 )
 
     def is_needed_to_heat(self, tmp_act: int, prediction_of_consumption)->tuple[bool, int]:
         """Conciders if it is needed to heat.
```

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/command_line.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/command_line.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/controller.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/data_handler.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/data_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,15 @@
 
     # Data Processing
 
     def extract_features_from_longitude_latitude(self, df_old):
         home_coords = (self.home_latitude, self.home_longitude)
         #drop na in columns mean_latitude and mean_longitude
         df = df_old.copy()
+        
         df = df.dropna(subset=["mean_latitude", "mean_longitude"])
         df.loc[:,"distance_from_home"] = np.vectorize(self.haversine_dist)(
             df["mean_latitude"],
             df["mean_longitude"],
             self.home_latitude,
             self.home_longitude,
         )
```

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/event_checker.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/forecast.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/forecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,14 +314,18 @@
         if left_time_interval is None:
             left_time_interval = datetime.now() - timedelta(days=5)
         if right_time_interval is None:
             right_time_interval = datetime.now()
             
         
         forecast_future = pd.DataFrame()
+        
+        #set minutes to 0
+        left_time_interval = left_time_interval.replace(minute=0)
+        right_time_interval = right_time_interval.replace(minute=0)
 
 
         df_all = self.dataHandler.get_data_for_prediction(
             left_time_interval=left_time_interval,
             right_time_interval=right_time_interval,
         )
         num_targets = len(self.predicted_columns)
```

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/machine_learning_forecaster.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/machine_learning_forecaster.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/main.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/main.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/optimization.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/optimization.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/retrieve_hass.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/retrieve_hass.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/static/style.css` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/static/style.css`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/switch.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/templates/index.html` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/templates/index.html`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/time_handler.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/utils.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/utils.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/web_server.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/web_server.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler/week_planner.py` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler/week_planner.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.5.8.7
+Version: 0.0.3.0.0.5.8.9
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.5.8.7/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.0.3.0.0.5.8.9/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

