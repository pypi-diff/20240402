# Comparing `tmp/eaf_base_api-1.3.tar.gz` & `tmp/eaf_base_api-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eaf_base_api-1.3.tar", last modified: Thu Mar 28 15:20:20 2024, max compression
+gzip compressed data, was "eaf_base_api-1.5.tar", last modified: Mon Apr  1 23:41:06 2024, max compression
```

## Comparing `eaf_base_api-1.3.tar` & `eaf_base_api-1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-03-28 15:20:20.416161 eaf_base_api-1.3/
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1603 2024-03-28 15:20:20.416161 eaf_base_api-1.3/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1134 2024-02-25 13:36:08.000000 eaf_base_api-1.3/README.md
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-03-28 15:20:20.416161 eaf_base_api-1.3/base_api/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-17 20:06:14.000000 eaf_base_api-1.3/base_api/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     5666 2024-03-28 15:20:09.000000 eaf_base_api-1.3/base_api/base.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-03-28 15:20:20.416161 eaf_base_api-1.3/base_api/modules/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-17 23:21:34.000000 eaf_base_api-1.3/base_api/modules/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)       15 2024-03-02 11:31:49.000000 eaf_base_api-1.3/base_api/modules/consts.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     4845 2024-02-29 14:57:59.000000 eaf_base_api-1.3/base_api/modules/download.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1559 2024-02-17 21:49:48.000000 eaf_base_api-1.3/base_api/modules/progress_bars.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      101 2024-02-17 21:30:46.000000 eaf_base_api-1.3/base_api/modules/quality.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-03-28 15:20:20.416161 eaf_base_api-1.3/eaf_base_api.egg-info/
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1603 2024-03-28 15:20:20.000000 eaf_base_api-1.3/eaf_base_api.egg-info/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)      382 2024-03-28 15:20:20.000000 eaf_base_api-1.3/eaf_base_api.egg-info/SOURCES.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-03-28 15:20:20.000000 eaf_base_api-1.3/eaf_base_api.egg-info/dependency_links.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       31 2024-03-28 15:20:20.000000 eaf_base_api-1.3/eaf_base_api.egg-info/requires.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)        9 2024-03-28 15:20:20.000000 eaf_base_api-1.3/eaf_base_api.egg-info/top_level.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-03-28 15:20:20.416161 eaf_base_api-1.3/setup.cfg
--rw-r--r--   0 asuna     (1000) asuna     (1000)      846 2024-03-28 15:20:09.000000 eaf_base_api-1.3/setup.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:41:06.810887 eaf_base_api-1.5/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1603 2024-04-01 23:41:06.810887 eaf_base_api-1.5/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1134 2024-02-25 13:36:08.000000 eaf_base_api-1.5/README.md
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:41:06.807554 eaf_base_api-1.5/base_api/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-17 20:06:14.000000 eaf_base_api-1.5/base_api/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     5695 2024-03-29 12:15:28.000000 eaf_base_api-1.5/base_api/base.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:41:06.810887 eaf_base_api-1.5/base_api/modules/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-17 23:21:34.000000 eaf_base_api-1.5/base_api/modules/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-03-29 13:01:59.000000 eaf_base_api-1.5/base_api/modules/consts.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     5868 2024-03-29 13:09:26.000000 eaf_base_api-1.5/base_api/modules/download.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1559 2024-02-17 21:49:48.000000 eaf_base_api-1.5/base_api/modules/progress_bars.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      101 2024-02-17 21:30:46.000000 eaf_base_api-1.5/base_api/modules/quality.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:41:06.810887 eaf_base_api-1.5/eaf_base_api.egg-info/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1603 2024-04-01 23:41:06.000000 eaf_base_api-1.5/eaf_base_api.egg-info/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      382 2024-04-01 23:41:06.000000 eaf_base_api-1.5/eaf_base_api.egg-info/SOURCES.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-04-01 23:41:06.000000 eaf_base_api-1.5/eaf_base_api.egg-info/dependency_links.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       31 2024-04-01 23:41:06.000000 eaf_base_api-1.5/eaf_base_api.egg-info/requires.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        9 2024-04-01 23:41:06.000000 eaf_base_api-1.5/eaf_base_api.egg-info/top_level.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-04-01 23:41:06.810887 eaf_base_api-1.5/setup.cfg
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      846 2024-04-01 23:40:24.000000 eaf_base_api-1.5/setup.py
```

### Comparing `eaf_base_api-1.3/PKG-INFO` & `eaf_base_api-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eaf_base_api
-Version: 1.3
+Version: 1.5
 Summary: A base API for EchterAlsFake's Porn APIs
 Home-page: https://github.com/EchterAlsFake/eaf_base_api
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `eaf_base_api-1.3/README.md` & `eaf_base_api-1.5/README.md`

 * *Files identical despite different names*

### Comparing `eaf_base_api-1.3/base_api/base.py` & `eaf_base_api-1.5/base_api/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 
 
 base_qualities = ["250p", "360p", "480p", "720p", "1080p", "1440p", "2160p"]
 
 
 class Core:
     @classmethod
-    def get_content(cls, url, headers=None, cookies=None):
+    def get_content(cls, url, headers=None, cookies=None, stream=False):
         for i in range(MAX_RETRIES):
             try:
                 logging.debug(f"Trying to fetch {url} / Attempt: [{i+1}]")
-                response = requests.get(url, headers=headers, cookies=cookies)
+                response = requests.get(url, headers=headers, cookies=cookies, stream=stream)
                 if response.status_code == 200:
                     logging.info(f"Successfully fetched {url} on attempt [{i+1}]")
                     return response.content
                 else:
                     logging.warning(f"Failed to fetch {url} with status code {response.status_code} on attempt [{i+1}]")
             except requests.exceptions.RequestException as e:
                 logging.error(f"Exception occurred when trying to fetch {url} on attempt [{i+1}]: {e}")
```

### Comparing `eaf_base_api-1.3/base_api/modules/download.py` & `eaf_base_api-1.5/base_api/modules/download.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 import logging
 import time
 import requests
 import os
 from ffmpeg_progress_yield import FfmpegProgress
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from typing import Callable, List
+from base_api.modules.progress_bars import Callback
+
+try:
+    from base_api.modules.consts import FFMPEG_PATH
+
+except (ModuleNotFoundError, ImportError):
+    from .consts import FFMPEG_PATH
 
 CallbackType = Callable[[int, int], None]
 
 """
 Important: The title of the video isn't applied to the output path. You need to manually append it to 
 the output path. This has good reasons, to make this library more adaptable into other applications.
 """
@@ -105,15 +112,15 @@
     new_segment = video.get_m3u8_by_quality(quality)
     url_components = base_url.split('/')
     url_components[-1] = new_segment
     new_url = '/'.join(url_components)
 
     # Build the command for FFMPEG as a list directly
     command = [
-        "ffmpeg",
+        FFMPEG_PATH,
         "-i", new_url,  # Input URL
         "-bsf:a", "aac_adtstoasc",
         "-y",  # Overwrite output files without asking
         "-c", "copy",  # Copy streams without reencoding
         path  # Output file path
     ]
 
@@ -122,8 +129,38 @@
     for progress in ff.run_command_with_progress():
         # Update the callback with the current progress
         callback(int(round(progress)), 100)
 
         if progress == 100:
             return True
 
-    return False
+    return False
+
+
+def legacy_download(stream, path, url, callback=None):
+    response = requests.get(url, stream=stream)
+    file_size = int(response.headers.get('content-length', 0))
+
+    if callback is None:
+        progress_bar = Callback()
+
+    downloaded_so_far = 0
+
+    if not os.path.exists(path):
+        with open(path, 'wb') as file:
+            for chunk in response.iter_content(chunk_size=1024):
+                file.write(chunk)
+                downloaded_so_far += len(chunk)
+
+                if callback:
+                    callback(downloaded_so_far, file_size)
+
+                else:
+                    progress_bar.text_progress_bar(downloaded=downloaded_so_far, total=file_size)
+
+        if not callback:
+            del progress_bar
+
+        return True
+
+    else:
+        raise FileExistsError("The file already exists.")
```

### Comparing `eaf_base_api-1.3/base_api/modules/progress_bars.py` & `eaf_base_api-1.5/base_api/modules/progress_bars.py`

 * *Files identical despite different names*

### Comparing `eaf_base_api-1.3/eaf_base_api.egg-info/PKG-INFO` & `eaf_base_api-1.5/eaf_base_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eaf_base_api
-Version: 1.3
+Version: 1.5
 Summary: A base API for EchterAlsFake's Porn APIs
 Home-page: https://github.com/EchterAlsFake/eaf_base_api
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `eaf_base_api-1.3/setup.py` & `eaf_base_api-1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="eaf_base_api",
-    version="1.3",
+    version="1.5",
     packages=find_packages(),
     install_requires=[
         "requests", "ffmpeg-progress-yield"
     ],
     entry_points={
         'console_scripts': [
             # If you want to create any executable scripts
```

