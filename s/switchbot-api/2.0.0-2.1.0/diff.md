# Comparing `tmp/switchbot_api-2.0.0.tar.gz` & `tmp/switchbot_api-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switchbot_api-2.0.0.tar", max compression
+gzip compressed data, was "switchbot_api-2.1.0.tar", max compression
```

## Comparing `switchbot_api-2.0.0.tar` & `switchbot_api-2.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2024-01-12 09:23:39.929936 switchbot_api-2.0.0/LICENSE
--rw-r--r--   0        0        0      464 2024-01-12 09:23:39.929936 switchbot_api-2.0.0/README.md
--rw-r--r--   0        0        0      941 2024-01-12 09:23:39.929936 switchbot_api-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     7718 2024-01-12 09:23:39.929936 switchbot_api-2.0.0/switchbot_api/__init__.py
--rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 switchbot_api-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-02 04:13:04.332311 switchbot_api-2.1.0/LICENSE
+-rw-r--r--   0        0        0      464 2024-04-02 04:13:04.332311 switchbot_api-2.1.0/README.md
+-rw-r--r--   0        0        0      946 2024-04-02 04:13:04.332311 switchbot_api-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7816 2024-04-02 04:13:04.332311 switchbot_api-2.1.0/switchbot_api/__init__.py
+-rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 switchbot_api-2.1.0/PKG-INFO
```

### Comparing `switchbot_api-2.0.0/LICENSE` & `switchbot_api-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `switchbot_api-2.0.0/switchbot_api/__init__.py` & `switchbot_api-2.1.0/switchbot_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tools to query the SwitchBot API."""
+
 import base64
 from dataclasses import dataclass
 from enum import Enum
 import hashlib
 import hmac
 import logging
 import time
@@ -142,14 +143,21 @@
 class LightCommands(Commands):
     """Light commands."""
 
     BRIGHTNESS_UP = "brightnessUp"
     BRIGHTNESS_DOWN = "brightnessDown"
 
 
+class LockCommands(Commands):
+    """Lock commands"""
+
+    LOCK = "lock"
+    UNLOCK = "unlock"
+
+
 class CeilingLightCommands(Commands):
     """Ceiling light commands."""
 
     # 1-100
     SET_BRIGHTNESS = "setBrightness"
     # 2700-6500
     SET_COLOR_TEMPERATURE = "setColorTemperature"
```

### Comparing `switchbot_api-2.0.0/PKG-INFO` & `switchbot_api-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switchbot_api
-Version: 2.0.0
+Version: 2.1.0
 Summary: An asynchronous library to use Switchbot API
 Home-page: https://github.com/SeraphicCorp/py-switchbot-api
 License: MIT
 Author: Ravaka Razafimanantsoa
 Author-email: contact@ravaka.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

