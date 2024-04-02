# Comparing `tmp/pyaffalddk-2.0.19.tar.gz` & `tmp/pyaffalddk-2.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaffalddk-2.0.19.tar", last modified: Fri Mar 29 13:35:59 2024, max compression
+gzip compressed data, was "pyaffalddk-2.0.20.tar", last modified: Tue Apr  2 13:53:34 2024, max compression
```

## Comparing `pyaffalddk-2.0.19.tar` & `pyaffalddk-2.0.20.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:35:59.481880 pyaffalddk-2.0.19/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-29 13:35:55.000000 pyaffalddk-2.0.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-29 13:35:59.481880 pyaffalddk-2.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-29 13:35:55.000000 pyaffalddk-2.0.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:35:59.481880 pyaffalddk-2.0.19/pyaffalddk/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-29 13:35:55.000000 pyaffalddk-2.0.19/pyaffalddk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-03-29 13:35:55.000000 pyaffalddk-2.0.19/pyaffalddk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-03-29 13:35:55.000000 pyaffalddk-2.0.19/pyaffalddk/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-29 13:35:55.000000 pyaffalddk-2.0.19/pyaffalddk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-29 13:35:55.000000 pyaffalddk-2.0.19/pyaffalddk/images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:35:59.481880 pyaffalddk-2.0.19/pyaffalddk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-29 13:35:59.000000 pyaffalddk-2.0.19/pyaffalddk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-29 13:35:59.000000 pyaffalddk-2.0.19/pyaffalddk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 13:35:59.000000 pyaffalddk-2.0.19/pyaffalddk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 13:35:59.000000 pyaffalddk-2.0.19/pyaffalddk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 13:35:59.481880 pyaffalddk-2.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-29 13:35:55.000000 pyaffalddk-2.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:53:34.019479 pyaffalddk-2.0.20/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 13:53:34.019479 pyaffalddk-2.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:53:34.019479 pyaffalddk-2.0.20/pyaffalddk/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/pyaffalddk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/pyaffalddk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/pyaffalddk/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/pyaffalddk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/pyaffalddk/images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:53:34.019479 pyaffalddk-2.0.20/pyaffalddk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 13:53:34.000000 pyaffalddk-2.0.20/pyaffalddk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 13:53:34.000000 pyaffalddk-2.0.20/pyaffalddk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:53:34.000000 pyaffalddk-2.0.20/pyaffalddk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 13:53:34.000000 pyaffalddk-2.0.20/pyaffalddk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:53:34.019479 pyaffalddk-2.0.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/setup.py
```

### Comparing `pyaffalddk-2.0.19/LICENSE` & `pyaffalddk-2.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.19/PKG-INFO` & `pyaffalddk-2.0.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.19
+Version: 2.0.20
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.19/pyaffalddk/__init__.py` & `pyaffalddk-2.0.20/pyaffalddk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     AffaldDKNoConnection,
 )
 from pyaffalddk.data import PickupEvents, PickupType, AffaldDKAddressInfo
 
 from pyaffalddk.const import ICON_LIST, MUNICIPALITIES_ARRAY, NAME_ARRAY, NAME_LIST
 
 __title__ = "pyaffalddk"
-__version__ = "2.0.19"
+__version__ = "2.0.20"
 __author__ = "briis"
 __license__ = "MIT"
```

### Comparing `pyaffalddk-2.0.19/pyaffalddk/api.py` & `pyaffalddk-2.0.20/pyaffalddk/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module contains the code to get garbage data from AffaldDK."""
 from __future__ import annotations
 
 import abc
 import datetime as dt
+from datetime import timezone
 import json
 import logging
 
 from typing import Any
 
 import aiohttp
 
@@ -100,19 +101,21 @@
 
 class GarbageCollection:
     """Class to get garbage collection data."""
 
     def __init__(
         self,
         municipality: str,
+        timezone: str = "Europe/Copenhagen",
         session: aiohttp.ClientSession = None,
         api: AffaldDKAPIBase = AffaldDKAPI(),
     ) -> None:
         """Initialize the class."""
         self._municipality = municipality
+        self._timezone = timezone
         self._street = None
         self._house_number = None
         self._api = api
         self._data = None
         self._municipality_url = None
         self._address_id = None
         if session:
@@ -188,14 +191,17 @@
 
             pickup_events: PickupEvents = {}
             _next_pickup = dt.datetime(2030, 12, 31, 23, 59, 0)
             _next_pickup = _next_pickup.date()
             _next_pickup_event: PickupType = None
             _next_name = []
             _next_description = []
+            _last_update = dt.datetime.now(timezone.utc)
+            _utc_date = _last_update.replace(tzinfo=timezone.utc)
+            _utc_timestamp = _utc_date.timestamp()
 
             for row in garbage_data:
                 if row["ordningnavn"] in NON_SUPPORTED_ITEMS:
                     continue
 
                 _pickup_date = None
                 if row["toemningsdato"] not in NON_SUPPORTED_ITEMS:
@@ -217,24 +223,24 @@
                 if key == row["ordningnavn"] and key != "Bestillerordning":
                     _LOGGER.warning(
                         "Garbage type [%s] is not defined in the system. Please notify the developer",
                         key,
                     )
                     continue
 
-                _last_update = dt.datetime.now()
                 _pickup_event = {
                     key: PickupType(
                         date=_pickup_date,
                         group=row["ordningnavn"],
                         friendly_name=NAME_LIST.get(key),
                         icon=ICON_LIST.get(key),
                         entity_picture=f"{key}.svg",
                         description=row["materielnavn"],
-                        last_updated=_last_update.strftime("%Y-%m-%d %H:%M:%S"),
+                        last_updated=_utc_date,
+                        utc_timestamp=_utc_timestamp,
                     )
                 }
                 pickup_events.update(_pickup_event)
 
                 if _pickup_date is not None:
                     if _pickup_date < dt.date.today():
                         continue
@@ -242,24 +248,24 @@
                         _next_pickup = _pickup_date
                         _next_name = []
                         _next_description = []
                     if _pickup_date == _next_pickup:
                         _next_name.append(NAME_LIST.get(key))
                         _next_description.append(row["materielnavn"])
 
-            _last_update = dt.datetime.now()
             _next_pickup_event = {
                 "next_pickup": PickupType(
                     date=_next_pickup,
                     group="genbrug",
                     friendly_name=list_to_string(_next_name),
                     icon=ICON_LIST.get("genbrug"),
                     entity_picture="genbrug.svg",
                     description=list_to_string(_next_description),
-                    last_updated=_last_update.strftime("%Y-%m-%d %H:%M:%S"),
+                    last_updated=_utc_date,
+                    utc_timestamp=_utc_timestamp,
                 )
             }
 
             pickup_events.update(_next_pickup_event)
             return pickup_events
```

### Comparing `pyaffalddk-2.0.19/pyaffalddk/const.py` & `pyaffalddk-2.0.20/pyaffalddk/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,15 @@
         "240 l PMDK/PP 3 ugers tømning (1 stk.)",
     ],
     "farligtaffald": [
         "",
     ],
     "farligtaffaldmiljoboks": [
         "Miljøkasse (1 stk.)",
+        "Miljøboks",
     ],
     "flis": [""],
     "jern": [""],
     "genbrug": [
         "Tekstiler",
         "Genbrug",
         "Genbrugsøer",
```

### Comparing `pyaffalddk-2.0.19/pyaffalddk/data.py` & `pyaffalddk-2.0.20/pyaffalddk/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
     date: dt.date | None = None
     group: str | None = None
     friendly_name: str | None = None
     icon: str | None = None
     entity_picture: str | None = None
     description: str | None = None
-    last_updated: str | None = None
+    last_updated: dt.datetime | None = None
+    utc_timestamp: int | None = None
 
 
 @dataclass(frozen=True)
 class PickupEvents:
     """Represent AffaldDK collection data."""
 
     batterier: list[PickupType] | None = None
```

### Comparing `pyaffalddk-2.0.19/pyaffalddk/images.py` & `pyaffalddk-2.0.20/pyaffalddk/images.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.19/pyaffalddk.egg-info/PKG-INFO` & `pyaffalddk-2.0.20/pyaffalddk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.19
+Version: 2.0.20
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.19/setup.py` & `pyaffalddk-2.0.20/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyaffalddk",
-    version="2.0.19",
+    version="2.0.20",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets garbage collection data from danish Municipalities",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pyaffalddk",
```

