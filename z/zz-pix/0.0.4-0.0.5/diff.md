# Comparing `tmp/zz-pix-0.0.4.tar.gz` & `tmp/zz-pix-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zz-pix-0.0.4.tar", last modified: Mon Apr  1 22:08:32 2024, max compression
+gzip compressed data, was "zz-pix-0.0.5.tar", last modified: Mon Apr  1 22:28:00 2024, max compression
```

## Comparing `zz-pix-0.0.4.tar` & `zz-pix-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 22:08:32.113780 zz-pix-0.0.4/
--rw-rw-rw-   0        0        0    11541 2024-03-29 15:51:16.000000 zz-pix-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3601 2024-04-01 22:08:32.112278 zz-pix-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-01 22:08:32.102768 zz-pix-0.0.4/pix/
--rw-rw-rw-   0        0        0        0 2024-03-29 15:51:16.000000 zz-pix-0.0.4/pix/__init__.py
--rw-rw-rw-   0        0        0     2661 2024-04-01 21:55:37.000000 zz-pix-0.0.4/pix/blip.py
--rw-rw-rw-   0        0        0     4579 2024-04-01 21:55:54.000000 zz-pix-0.0.4/pix/cli_parser.py
--rw-rw-rw-   0        0        0     2856 2024-03-29 15:51:16.000000 zz-pix-0.0.4/pix/converter.py
--rw-rw-rw-   0        0        0     3852 2024-03-29 15:51:16.000000 zz-pix-0.0.4/pix/croper.py
--rw-rw-rw-   0        0        0     4431 2024-04-01 22:03:29.000000 zz-pix-0.0.4/pix/main.py
--rw-rw-rw-   0        0        0      182 2024-04-01 16:45:01.000000 zz-pix-0.0.4/pix/manifest.json
--rw-rw-rw-   0        0        0      588 2024-03-30 18:15:25.000000 zz-pix-0.0.4/pix/prune.py
--rw-rw-rw-   0        0        0     1580 2024-03-29 15:51:16.000000 zz-pix-0.0.4/pix/resizer.py
--rw-rw-rw-   0        0        0      706 2024-03-29 18:51:50.000000 zz-pix-0.0.4/pix/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-01 22:08:32.113780 zz-pix-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1789 2024-04-01 18:25:17.000000 zz-pix-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:08:32.112278 zz-pix-0.0.4/zz_pix.egg-info/
--rw-rw-rw-   0        0        0     3601 2024-04-01 22:08:32.000000 zz-pix-0.0.4/zz_pix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-04-01 22:08:32.000000 zz-pix-0.0.4/zz_pix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 22:08:32.000000 zz-pix-0.0.4/zz_pix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-01 22:08:32.000000 zz-pix-0.0.4/zz_pix.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       90 2024-04-01 22:08:32.000000 zz-pix-0.0.4/zz_pix.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-01 22:08:32.000000 zz-pix-0.0.4/zz_pix.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 22:28:00.835146 zz-pix-0.0.5/
+-rw-rw-rw-   0        0        0    11541 2024-03-29 15:51:16.000000 zz-pix-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3601 2024-04-01 22:28:00.834147 zz-pix-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-01 22:28:00.822374 zz-pix-0.0.5/pix/
+-rw-rw-rw-   0        0        0        0 2024-03-29 15:51:16.000000 zz-pix-0.0.5/pix/__init__.py
+-rw-rw-rw-   0        0        0     2837 2024-04-01 22:27:14.000000 zz-pix-0.0.5/pix/blip.py
+-rw-rw-rw-   0        0        0     4579 2024-04-01 21:55:54.000000 zz-pix-0.0.5/pix/cli_parser.py
+-rw-rw-rw-   0        0        0     2856 2024-03-29 15:51:16.000000 zz-pix-0.0.5/pix/converter.py
+-rw-rw-rw-   0        0        0     3852 2024-03-29 15:51:16.000000 zz-pix-0.0.5/pix/croper.py
+-rw-rw-rw-   0        0        0     4431 2024-04-01 22:03:29.000000 zz-pix-0.0.5/pix/main.py
+-rw-rw-rw-   0        0        0      182 2024-04-01 22:27:53.000000 zz-pix-0.0.5/pix/manifest.json
+-rw-rw-rw-   0        0        0      588 2024-03-30 18:15:25.000000 zz-pix-0.0.5/pix/prune.py
+-rw-rw-rw-   0        0        0     1580 2024-03-29 15:51:16.000000 zz-pix-0.0.5/pix/resizer.py
+-rw-rw-rw-   0        0        0      706 2024-03-29 18:51:50.000000 zz-pix-0.0.5/pix/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 22:28:00.835146 zz-pix-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1789 2024-04-01 18:25:17.000000 zz-pix-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 22:28:00.834147 zz-pix-0.0.5/zz_pix.egg-info/
+-rw-rw-rw-   0        0        0     3601 2024-04-01 22:28:00.000000 zz-pix-0.0.5/zz_pix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-04-01 22:28:00.000000 zz-pix-0.0.5/zz_pix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 22:28:00.000000 zz-pix-0.0.5/zz_pix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-01 22:28:00.000000 zz-pix-0.0.5/zz_pix.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       90 2024-04-01 22:28:00.000000 zz-pix-0.0.5/zz_pix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-01 22:28:00.000000 zz-pix-0.0.5/zz_pix.egg-info/top_level.txt
```

### Comparing `zz-pix-0.0.4/LICENSE` & `zz-pix-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.4/PKG-INFO` & `zz-pix-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zz-pix
-Version: 0.0.4
+Version: 0.0.5
 Summary: CLI tool for image manipulation
 Home-page: https://github.com/sean1832/pix
 Author: Zeke Zhang
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `zz-pix-0.0.4/pix/blip.py` & `zz-pix-0.0.5/pix/blip.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import logging
 from typing import List, Union
 
 import PIL
 import torch
 from termcolor import colored
+from transformers import logging as transformers_logging
 from transformers import pipeline
 
 
 class Blip:
     def __init__(self, large=False, cpu=False, blip2=False):
+        logging.basicConfig(level=logging.ERROR)
+        transformers_logging.set_verbosity_error()
         self.model_type = "blip"
         model_name = "Salesforce/blip-image-captioning-base"
         if large:
             model_name = "Salesforce/blip-image-captioning-large"
         if blip2:
             self.model_type = "blip2"
             print("Using Blip2 model")
```

### Comparing `zz-pix-0.0.4/pix/cli_parser.py` & `zz-pix-0.0.5/pix/cli_parser.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.4/pix/converter.py` & `zz-pix-0.0.5/pix/converter.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.4/pix/croper.py` & `zz-pix-0.0.5/pix/croper.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.4/pix/main.py` & `zz-pix-0.0.5/pix/main.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.4/pix/prune.py` & `zz-pix-0.0.5/pix/prune.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.4/pix/resizer.py` & `zz-pix-0.0.5/pix/resizer.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.4/pix/utils.py` & `zz-pix-0.0.5/pix/utils.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.4/setup.py` & `zz-pix-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.4/zz_pix.egg-info/PKG-INFO` & `zz-pix-0.0.5/zz_pix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zz-pix
-Version: 0.0.4
+Version: 0.0.5
 Summary: CLI tool for image manipulation
 Home-page: https://github.com/sean1832/pix
 Author: Zeke Zhang
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
```

