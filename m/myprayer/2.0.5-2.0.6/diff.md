# Comparing `tmp/myprayer-2.0.5.tar.gz` & `tmp/myprayer-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myprayer-2.0.5.tar", max compression
+gzip compressed data, was "myprayer-2.0.6.tar", max compression
```

## Comparing `myprayer-2.0.5.tar` & `myprayer-2.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-01-12 21:15:48.289422 myprayer-2.0.5/LICENSE
--rw-r--r--   0        0        0     5375 2024-01-12 21:45:32.208715 myprayer-2.0.5/README.md
--rw-r--r--   0        0        0        0 2023-10-07 02:42:05.360576 myprayer-2.0.5/myprayer/__init__.py
--rw-r--r--   0        0        0     8656 2024-01-06 21:11:40.149244 myprayer-2.0.5/myprayer/api/client.py
--rw-r--r--   0        0        0     2672 2023-12-31 14:42:40.793978 myprayer-2.0.5/myprayer/api/day.py
--rw-r--r--   0        0        0      732 2023-10-14 01:43:01.057210 myprayer-2.0.5/myprayer/api/exceptions.py
--rw-r--r--   0        0        0      571 2023-10-17 21:43:15.204557 myprayer-2.0.5/myprayer/api/location_types.py
--rw-r--r--   0        0        0      669 2023-11-11 17:45:03.278715 myprayer-2.0.5/myprayer/api/method.py
--rw-r--r--   0        0        0     1983 2023-10-18 20:42:45.215200 myprayer-2.0.5/myprayer/api/month.py
--rw-r--r--   0        0        0      416 2023-11-26 16:42:45.935655 myprayer-2.0.5/myprayer/api/prayer.py
--rw-r--r--   0        0        0     5387 2024-03-22 21:23:48.888843 myprayer-2.0.5/myprayer/cli/config.py
--rw-r--r--   0        0        0     2689 2024-01-13 20:29:26.231274 myprayer-2.0.5/myprayer/cli/constants.py
--rw-r--r--   0        0        0      770 2024-01-12 20:59:39.011876 myprayer-2.0.5/myprayer/cli/enums.py
--rwxr-xr-x   0        0        0    11574 2024-03-22 21:30:17.083002 myprayer-2.0.5/myprayer/cli/main.py
--rw-r--r--   0        0        0     3420 2024-01-07 14:51:48.788896 myprayer-2.0.5/myprayer/cli/output.py
--rw-r--r--   0        0        0      634 2024-01-06 22:19:10.669762 myprayer-2.0.5/myprayer/cli/utils.py
--rw-r--r--   0        0        0      527 2024-03-22 21:30:53.119143 myprayer-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     6281 1970-01-01 00:00:00.000000 myprayer-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-12 21:15:48.289422 myprayer-2.0.6/LICENSE
+-rw-r--r--   0        0        0     5975 2024-03-23 05:28:17.103974 myprayer-2.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-10-07 02:42:05.360576 myprayer-2.0.6/myprayer/__init__.py
+-rw-r--r--   0        0        0     8662 2024-04-02 02:10:18.540660 myprayer-2.0.6/myprayer/api/client.py
+-rw-r--r--   0        0        0     2672 2023-12-31 14:42:40.793978 myprayer-2.0.6/myprayer/api/day.py
+-rw-r--r--   0        0        0      732 2023-10-14 01:43:01.057210 myprayer-2.0.6/myprayer/api/exceptions.py
+-rw-r--r--   0        0        0      571 2023-10-17 21:43:15.204557 myprayer-2.0.6/myprayer/api/location_types.py
+-rw-r--r--   0        0        0      669 2023-11-11 17:45:03.278715 myprayer-2.0.6/myprayer/api/method.py
+-rw-r--r--   0        0        0     1983 2023-10-18 20:42:45.215200 myprayer-2.0.6/myprayer/api/month.py
+-rw-r--r--   0        0        0      416 2023-11-26 16:42:45.935655 myprayer-2.0.6/myprayer/api/prayer.py
+-rw-r--r--   0        0        0     5387 2024-03-22 21:23:48.888843 myprayer-2.0.6/myprayer/cli/config.py
+-rw-r--r--   0        0        0     2689 2024-01-13 20:29:26.231274 myprayer-2.0.6/myprayer/cli/constants.py
+-rw-r--r--   0        0        0      770 2024-01-12 20:59:39.011876 myprayer-2.0.6/myprayer/cli/enums.py
+-rwxr-xr-x   0        0        0    11756 2024-04-02 01:55:35.084447 myprayer-2.0.6/myprayer/cli/main.py
+-rw-r--r--   0        0        0     3420 2024-01-07 14:51:48.788896 myprayer-2.0.6/myprayer/cli/output.py
+-rw-r--r--   0        0        0      634 2024-01-06 22:19:10.669762 myprayer-2.0.6/myprayer/cli/utils.py
+-rw-r--r--   0        0        0      527 2024-04-02 02:12:18.170257 myprayer-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6881 1970-01-01 00:00:00.000000 myprayer-2.0.6/PKG-INFO
```

### Comparing `myprayer-2.0.5/LICENSE` & `myprayer-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.5/README.md` & `myprayer-2.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -90,15 +90,39 @@
  --force        -f                                     Force update cache.       
  --help                                                Configure default settings
 ```
 
 
 ## Configuration
 
-Default settings like location, calculation method, and output format can be configured in `~/.myprayer/config.json` using `myprayer config`.
+Default settings like location, calculation method, and output format can be configured in `$XDG_CONFIG_HOME/myprayer/config.json` or `$HOME/.config/myprayer/config.json` using `myprayer config`.
+
+### Example configuration
+
+```jsonc
+{
+    "time_format": "12", // 12 or 24
+    "print_type": "table", // pretty, machine, table, json
+    "method": 5, // Calculation method
+    "show_next": true, // Highlight next prayer in list
+    "prayers": [ // Prayer to show
+        "Fajr",
+        "Dhuhr",
+        "Asr",
+        "Maghrib",
+        "Isha"
+    ],
+    "location": { // Default location used if no location is provided in command
+        "type": "city",
+        "city": "Cairo",
+        "country": "Egypt",
+        "state": null
+    }
+}
+```
 
 
 ## Credits
 - [Aladhan API](https://aladhan.com/) - for prayer time data
 - [aladhan-api](https://pypi.org/project/aladhan-api/) - i drew inspiration from this project
```

### Comparing `myprayer-2.0.5/myprayer/api/client.py` & `myprayer-2.0.6/myprayer/api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         month: int,
         year: int,
         location: City | Coordinates | Address,
         method: Optional[int] = None,
     ):
         if method is None:
             method = "auto"  # type: ignore
-        suffix = f"{month}_{year}_{method}.json"
+        suffix = f"{month:02}_{year}_{method:02}.json"
         if isinstance(location, Coordinates):
             return f"coordinates_{location.longitude}_{location.latitude}_{suffix}"
         if isinstance(location, Address):
             return f"address_{location.url_encoded()}_{suffix}"
         if isinstance(location, City):
             return f"city_{location.city.replace(' ','')}_{location.country.replace(' ', '')}_{suffix}"
```

### Comparing `myprayer-2.0.5/myprayer/api/day.py` & `myprayer-2.0.6/myprayer/api/day.py`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.5/myprayer/api/exceptions.py` & `myprayer-2.0.6/myprayer/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.5/myprayer/api/location_types.py` & `myprayer-2.0.6/myprayer/api/location_types.py`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.5/myprayer/api/method.py` & `myprayer-2.0.6/myprayer/api/method.py`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.5/myprayer/api/month.py` & `myprayer-2.0.6/myprayer/api/month.py`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.5/myprayer/cli/config.py` & `myprayer-2.0.6/myprayer/cli/config.py`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.5/myprayer/cli/constants.py` & `myprayer-2.0.6/myprayer/cli/constants.py`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.5/myprayer/cli/enums.py` & `myprayer-2.0.6/myprayer/cli/enums.py`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.5/myprayer/cli/main.py` & `myprayer-2.0.6/myprayer/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env python
 
+__author__ = "Youssef Aswad"
+__version__ = "2.0.5"
+
 import json
 from datetime import datetime
 
 import inquirer
 import typer
 from rich import print as rprint
 from rich.prompt import FloatPrompt, Prompt
@@ -22,17 +25,21 @@
     PRAYERS,
     TIME_FORMATS,
 )
 from myprayer.cli.enums import NextOutType, OutType, TimeFormat
 from myprayer.cli.output import DayOutput
 from myprayer.cli.utils import format_time_left
 
+
 app = typer.Typer(name=APP_NAME, pretty_exceptions_enable=False, help="MyPrayer CLI.")
 
 
+# TODO: Add option to display date in output
+# TODO: Emphasize next prayer in waybar output <span font_weight="bold">...</span>
+
 # Load config
 CONFIG = Config(CONFIG_FILE)
 
 
 def get_client(city, country, address, latitude, longitude, method, force):
     cache = None if force else CACHE_DIR
     skip = [prayer for prayer in PRAYERS if prayer not in CONFIG.prayers]
```

### Comparing `myprayer-2.0.5/myprayer/cli/output.py` & `myprayer-2.0.6/myprayer/cli/output.py`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.5/myprayer/cli/utils.py` & `myprayer-2.0.6/myprayer/cli/utils.py`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.5/pyproject.toml` & `myprayer-2.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "myprayer"
-version = "2.0.5"
+version = "2.0.6"
 description = "A CLI tool to get prayer times"
 authors = ["Youssef Aswad <youssefaswad@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/YoussefAswad/myprayer"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `myprayer-2.0.5/PKG-INFO` & `myprayer-2.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myprayer
-Version: 2.0.5
+Version: 2.0.6
 Summary: A CLI tool to get prayer times
 Home-page: https://github.com/YoussefAswad/myprayer
 License: MIT
 Author: Youssef Aswad
 Author-email: youssefaswad@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -114,15 +114,39 @@
  --force        -f                                     Force update cache.       
  --help                                                Configure default settings
 ```
 
 
 ## Configuration
 
-Default settings like location, calculation method, and output format can be configured in `~/.myprayer/config.json` using `myprayer config`.
+Default settings like location, calculation method, and output format can be configured in `$XDG_CONFIG_HOME/myprayer/config.json` or `$HOME/.config/myprayer/config.json` using `myprayer config`.
+
+### Example configuration
+
+```jsonc
+{
+    "time_format": "12", // 12 or 24
+    "print_type": "table", // pretty, machine, table, json
+    "method": 5, // Calculation method
+    "show_next": true, // Highlight next prayer in list
+    "prayers": [ // Prayer to show
+        "Fajr",
+        "Dhuhr",
+        "Asr",
+        "Maghrib",
+        "Isha"
+    ],
+    "location": { // Default location used if no location is provided in command
+        "type": "city",
+        "city": "Cairo",
+        "country": "Egypt",
+        "state": null
+    }
+}
+```
 
 
 ## Credits
 - [Aladhan API](https://aladhan.com/) - for prayer time data
 - [aladhan-api](https://pypi.org/project/aladhan-api/) - i drew inspiration from this project
```

