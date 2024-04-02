# Comparing `tmp/saphira-0.0.2.tar.gz` & `tmp/saphira-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saphira-0.0.2.tar", last modified: Mon Apr  1 23:41:15 2024, max compression
+gzip compressed data, was "saphira-0.0.3.tar", last modified: Mon Apr  1 23:45:07 2024, max compression
```

## Comparing `saphira-0.0.2.tar` & `saphira-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:41:15.736207 saphira-0.0.2/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1063 2023-12-22 05:35:11.000000 saphira-0.0.2/LICENSE
--rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-01 23:41:15.735187 saphira-0.0.2/PKG-INFO
--rw-r--r--   0 akshaychalana   (501) staff       (20)       71 2023-12-19 02:46:29.000000 saphira-0.0.2/README.md
--rw-r--r--   0 akshaychalana   (501) staff       (20)      718 2024-04-01 23:39:54.000000 saphira-0.0.2/pyproject.toml
--rw-r--r--   0 akshaychalana   (501) staff       (20)       38 2024-04-01 23:41:15.736683 saphira-0.0.2/setup.cfg
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:41:15.699806 saphira-0.0.2/src/
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:41:15.709811 saphira-0.0.2/src/saphira/
--rw-r--r--   0 akshaychalana   (501) staff       (20)       45 2024-04-01 23:39:46.000000 saphira-0.0.2/src/saphira/__init__.py
--rw-r--r--   0 akshaychalana   (501) staff       (20)     2087 2024-01-22 05:10:51.000000 saphira-0.0.2/src/saphira/saphira.py
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:41:15.733828 saphira-0.0.2/src/saphira.egg-info/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-01 23:41:15.000000 saphira-0.0.2/src/saphira.egg-info/PKG-INFO
--rw-r--r--   0 akshaychalana   (501) staff       (20)      310 2024-04-01 23:41:15.000000 saphira-0.0.2/src/saphira.egg-info/SOURCES.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)        1 2024-04-01 23:41:15.000000 saphira-0.0.2/src/saphira.egg-info/dependency_links.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)       53 2024-04-01 23:41:15.000000 saphira-0.0.2/src/saphira.egg-info/requires.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)        8 2024-04-01 23:41:15.000000 saphira-0.0.2/src/saphira.egg-info/top_level.txt
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:41:15.725960 saphira-0.0.2/tests/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1712 2024-03-12 21:02:28.000000 saphira-0.0.2/tests/test_battery_capacity.py
--rw-r--r--   0 akshaychalana   (501) staff       (20)      596 2023-11-18 02:00:44.000000 saphira-0.0.2/tests/test_jama_server.py
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:45:07.496147 saphira-0.0.3/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     1063 2023-12-22 05:35:11.000000 saphira-0.0.3/LICENSE
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-01 23:45:07.495434 saphira-0.0.3/PKG-INFO
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       71 2023-12-19 02:46:29.000000 saphira-0.0.3/README.md
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      718 2024-04-01 23:44:50.000000 saphira-0.0.3/pyproject.toml
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       38 2024-04-01 23:45:07.496289 saphira-0.0.3/setup.cfg
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:45:07.478994 saphira-0.0.3/src/
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:45:07.482500 saphira-0.0.3/src/saphira/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       45 2024-04-01 23:44:58.000000 saphira-0.0.3/src/saphira/__init__.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2123 2024-04-01 23:42:53.000000 saphira-0.0.3/src/saphira/saphira.py
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:45:07.492992 saphira-0.0.3/src/saphira.egg-info/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-01 23:45:07.000000 saphira-0.0.3/src/saphira.egg-info/PKG-INFO
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      310 2024-04-01 23:45:07.000000 saphira-0.0.3/src/saphira.egg-info/SOURCES.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)        1 2024-04-01 23:45:07.000000 saphira-0.0.3/src/saphira.egg-info/dependency_links.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       53 2024-04-01 23:45:07.000000 saphira-0.0.3/src/saphira.egg-info/requires.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)        8 2024-04-01 23:45:07.000000 saphira-0.0.3/src/saphira.egg-info/top_level.txt
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-01 23:45:07.492305 saphira-0.0.3/tests/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     1712 2024-03-12 21:02:28.000000 saphira-0.0.3/tests/test_battery_capacity.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      596 2023-11-18 02:00:44.000000 saphira-0.0.3/tests/test_jama_server.py
```

### Comparing `saphira-0.0.2/LICENSE` & `saphira-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `saphira-0.0.2/PKG-INFO` & `saphira-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saphira
-Version: 0.0.2
+Version: 0.0.3
 Summary: Access parameters from the Saphira.ai SysEng SSoT
 Author-email: Saphira AI <contact@saphira.ai>
 License: MIT License
         
         Copyright (c) 2023 Saphira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `saphira-0.0.2/pyproject.toml` & `saphira-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saphira"
-version = "0.0.2"
+version = "0.0.3"
 description = "Access parameters from the Saphira.ai SysEng SSoT"
 readme = "README.md"
 authors = [{ name = "Saphira AI", email = "contact@saphira.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `saphira-0.0.2/src/saphira/saphira.py` & `saphira-0.0.3/src/saphira/saphira.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,38 +2,40 @@
 import os
 import requests
 import subprocess
 from typing import Any
 import multiprocessing
 from time import sleep
 
-SAPHIRA_URL = os.getenv('SAPHIRA_URL', 'https://saphira.oavatare1.repl.co')
+SAPHIRA_URL = os.getenv('SAPHIRA_URL', 'https://prod.saphira.ai')
 
 # TODO: Integrate this into Matlab
 # This registers as a daemon that will re-run the parent program
 # TODO: Move daemon registration to service
 def get_param(datasource: str, name: str, skip_threading=False, local_runtime=False) -> Any:
     # TODO: Call select_project first before selecting datasource 
     # TODO: Use datasource to route to appropriate multi-tenant (project)
     # Post to service
-    url = f'{SAPHIRA_URL}/check_key_and_get_value'
+    url = f'{SAPHIRA_URL}/get_single_data/' + name
     req = {
         'check_key': name,
         # TODO: Include program name to allow automatic execution
         # 'consumingApplication': inspect.stack()[1].filename
     }
     consuming_application = inspect.stack()[-1].filename
-    resp = requests.post(url, json = req)
+    # resp = requests.post(url, json = req)
+    resp = requests.get(url)
     print(f"{url} responded with status code {resp.status_code}, {resp.json()}")
-    split_result = resp.json().get('result', "").split("value ")
-    result = None
-    if len(split_result) > 1:
-        result = float(split_result[1])
-    else:
-        raise Exception("bad response")
+    split_result = resp.json().get('value')
+    # result = None
+    result = split_result
+    # if len(split_result) > 1:
+    #     result = float(split_result[1])
+    # else:
+    #     raise Exception("bad response")
     
     if not skip_threading:
         if local_runtime:
             def loop():
                 while True:
                     if get_param(datasource, name, skip_threading=True) != result:
                         subprocess.call(['python', consuming_application])
```

### Comparing `saphira-0.0.2/src/saphira.egg-info/PKG-INFO` & `saphira-0.0.3/src/saphira.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saphira
-Version: 0.0.2
+Version: 0.0.3
 Summary: Access parameters from the Saphira.ai SysEng SSoT
 Author-email: Saphira AI <contact@saphira.ai>
 License: MIT License
         
         Copyright (c) 2023 Saphira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `saphira-0.0.2/tests/test_battery_capacity.py` & `saphira-0.0.3/tests/test_battery_capacity.py`

 * *Files identical despite different names*

### Comparing `saphira-0.0.2/tests/test_jama_server.py` & `saphira-0.0.3/tests/test_jama_server.py`

 * *Files identical despite different names*

