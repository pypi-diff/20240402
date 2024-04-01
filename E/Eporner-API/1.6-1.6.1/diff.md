# Comparing `tmp/Eporner_API-1.6.tar.gz` & `tmp/Eporner_API-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Eporner_API-1.6.tar", last modified: Fri Feb 16 13:00:56 2024, max compression
+gzip compressed data, was "Eporner_API-1.6.1.tar", last modified: Mon Apr  1 23:46:21 2024, max compression
```

## Comparing `Eporner_API-1.6.tar` & `Eporner_API-1.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-16 13:00:56.644260 Eporner_API-1.6/
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-16 13:00:56.644260 Eporner_API-1.6/Eporner_API.egg-info/
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2945 2024-02-16 13:00:56.000000 Eporner_API-1.6/Eporner_API.egg-info/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)      601 2024-02-16 13:00:56.000000 Eporner_API-1.6/Eporner_API.egg-info/SOURCES.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-02-16 13:00:56.000000 Eporner_API-1.6/Eporner_API.egg-info/dependency_links.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       18 2024-02-16 13:00:56.000000 Eporner_API-1.6/Eporner_API.egg-info/requires.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       12 2024-02-16 13:00:56.000000 Eporner_API-1.6/Eporner_API.egg-info/top_level.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)     7369 2024-02-08 15:55:11.000000 Eporner_API-1.6/LICENSE
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2945 2024-02-16 13:00:56.644260 Eporner_API-1.6/PKG-INFO
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-16 13:00:56.640926 Eporner_API-1.6/eporner_api/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 15:55:11.000000 Eporner_API-1.6/eporner_api/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)    17215 2024-02-16 12:52:56.000000 Eporner_API-1.6/eporner_api/eporner_api.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-16 13:00:56.640926 Eporner_API-1.6/eporner_api/modules/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 15:55:11.000000 Eporner_API-1.6/eporner_api/modules/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2687 2024-02-16 12:41:34.000000 Eporner_API-1.6/eporner_api/modules/consts.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      255 2024-02-08 15:55:11.000000 Eporner_API-1.6/eporner_api/modules/errors.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2109 2024-02-10 12:18:31.000000 Eporner_API-1.6/eporner_api/modules/locals.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      643 2024-02-08 15:55:11.000000 Eporner_API-1.6/eporner_api/modules/progressbar.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      492 2024-02-08 15:55:11.000000 Eporner_API-1.6/eporner_api/modules/sorting.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-16 13:00:56.644260 Eporner_API-1.6/eporner_api/tests/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 15:55:11.000000 Eporner_API-1.6/eporner_api/tests/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      796 2024-02-10 12:39:15.000000 Eporner_API-1.6/eporner_api/tests/test_category.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1756 2024-02-16 12:52:56.000000 Eporner_API-1.6/eporner_api/tests/test_pornstar.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2098 2024-02-08 15:55:11.000000 Eporner_API-1.6/eporner_api/tests/test_search.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2302 2024-02-10 12:42:57.000000 Eporner_API-1.6/eporner_api/tests/test_video.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-02-16 13:00:56.644260 Eporner_API-1.6/setup.cfg
--rw-r--r--   0 asuna     (1000) asuna     (1000)      877 2024-02-16 13:00:49.000000 Eporner_API-1.6/setup.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:46:21.060204 Eporner_API-1.6.1/
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:46:21.060204 Eporner_API-1.6.1/Eporner_API.egg-info/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2975 2024-04-01 23:46:21.000000 Eporner_API-1.6.1/Eporner_API.egg-info/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      601 2024-04-01 23:46:21.000000 Eporner_API-1.6.1/Eporner_API.egg-info/SOURCES.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-04-01 23:46:21.000000 Eporner_API-1.6.1/Eporner_API.egg-info/dependency_links.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       31 2024-04-01 23:46:21.000000 Eporner_API-1.6.1/Eporner_API.egg-info/requires.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       12 2024-04-01 23:46:21.000000 Eporner_API-1.6.1/Eporner_API.egg-info/top_level.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     7369 2024-02-08 15:55:11.000000 Eporner_API-1.6.1/LICENSE
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2975 2024-04-01 23:46:21.060204 Eporner_API-1.6.1/PKG-INFO
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:46:21.060204 Eporner_API-1.6.1/eporner_api/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 15:55:11.000000 Eporner_API-1.6.1/eporner_api/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)    16086 2024-03-29 12:24:14.000000 Eporner_API-1.6.1/eporner_api/eporner_api.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:46:21.060204 Eporner_API-1.6.1/eporner_api/modules/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 15:55:11.000000 Eporner_API-1.6.1/eporner_api/modules/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2687 2024-02-16 12:41:34.000000 Eporner_API-1.6.1/eporner_api/modules/consts.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      255 2024-02-08 15:55:11.000000 Eporner_API-1.6.1/eporner_api/modules/errors.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2030 2024-02-29 15:50:16.000000 Eporner_API-1.6.1/eporner_api/modules/locals.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      643 2024-02-08 15:55:11.000000 Eporner_API-1.6.1/eporner_api/modules/progressbar.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      492 2024-02-08 15:55:11.000000 Eporner_API-1.6.1/eporner_api/modules/sorting.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:46:21.060204 Eporner_API-1.6.1/eporner_api/tests/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 15:55:11.000000 Eporner_API-1.6.1/eporner_api/tests/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      796 2024-02-10 12:39:15.000000 Eporner_API-1.6.1/eporner_api/tests/test_category.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1756 2024-02-16 12:52:56.000000 Eporner_API-1.6.1/eporner_api/tests/test_pornstar.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2098 2024-02-08 15:55:11.000000 Eporner_API-1.6.1/eporner_api/tests/test_search.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2302 2024-02-10 12:42:57.000000 Eporner_API-1.6.1/eporner_api/tests/test_video.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-04-01 23:46:21.060204 Eporner_API-1.6.1/setup.cfg
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      895 2024-04-01 23:46:15.000000 Eporner_API-1.6.1/setup.py
```

### Comparing `Eporner_API-1.6/Eporner_API.egg-info/PKG-INFO` & `Eporner_API-1.6.1/Eporner_API.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: Eporner_API
-Version: 1.6
+Version: 1.6.1
 Summary: A Python API for the Porn Site Eporner.com
 Home-page: https://github.com/EchterAlsFake/EPorner_API
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
 Requires-Dist: lxml
+Requires-Dist: eaf_base_api
 
 <h1 align="center">EPorner API</h1> 
 
 <div align="center">
     <a href="https://pepy.tech/project/Eporner-API"><img src="https://static.pepy.tech/badge/Eporner-API" alt="Downloads"></a>
     <a href="https://github.com/EchterAlsFake/EPorner_API/workflows/"><img src="https://github.com/EchterAlsFake/EPorner_API/workflows/CodeQL/badge.svg" alt="CodeQL Analysis"/></a>
     <a href="https://github.com/EchterAlsFake/EPorner_API/workflows/"><img src="https://github.com/EchterAlsFake/EPorner_API/actions/workflows/tests.yml/badge.svg" alt="API Tests"/></a>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: Eporner_API Version: 1.6 Summary: A Python API for
-the Porn Site Eporner.com Home-page: https://github.com/EchterAlsFake/
+Metadata-Version: 2.1 Name: Eporner_API Version: 1.6.1 Summary: A Python API
+for the Porn Site Eporner.com Home-page: https://github.com/EchterAlsFake/
 EPorner_API Author: Johannes Habel Author-email: EchterAlsFake@proton.me
 License: LGPLv3 Classifier: License :: OSI Approved :: GNU Lesser General
 Public License v3 (LGPLv3) Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests Requires-Dist: bs4 Requires-Dist: lxml
+requests Requires-Dist: bs4 Requires-Dist: lxml Requires-Dist: eaf_base_api
                            ************ EEPPoorrnneerr AAPPII ************
                     _[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_Q_L_ _A_n_a_l_y_s_i_s_]_[_A_P_I_ _T_e_s_t_s_]
 # Description EPorner API is an API for EPorner, which allows you to fetch
 information from videos using the official V2 API. # Disclaimer > Some modules
 of this API are in violence to the ToS from Eporner.com > See Documentation for
 details about this! Copyright Information: I have no intention of stealing
 copyright protected content or slowing down a website. Contact me at my E-Mail,
```

### Comparing `Eporner_API-1.6/Eporner_API.egg-info/SOURCES.txt` & `Eporner_API-1.6.1/Eporner_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Eporner_API-1.6/LICENSE` & `Eporner_API-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Eporner_API-1.6/PKG-INFO` & `Eporner_API-1.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: Eporner_API
-Version: 1.6
+Version: 1.6.1
 Summary: A Python API for the Porn Site Eporner.com
 Home-page: https://github.com/EchterAlsFake/EPorner_API
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
 Requires-Dist: lxml
+Requires-Dist: eaf_base_api
 
 <h1 align="center">EPorner API</h1> 
 
 <div align="center">
     <a href="https://pepy.tech/project/Eporner-API"><img src="https://static.pepy.tech/badge/Eporner-API" alt="Downloads"></a>
     <a href="https://github.com/EchterAlsFake/EPorner_API/workflows/"><img src="https://github.com/EchterAlsFake/EPorner_API/workflows/CodeQL/badge.svg" alt="CodeQL Analysis"/></a>
     <a href="https://github.com/EchterAlsFake/EPorner_API/workflows/"><img src="https://github.com/EchterAlsFake/EPorner_API/actions/workflows/tests.yml/badge.svg" alt="API Tests"/></a>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: Eporner_API Version: 1.6 Summary: A Python API for
-the Porn Site Eporner.com Home-page: https://github.com/EchterAlsFake/
+Metadata-Version: 2.1 Name: Eporner_API Version: 1.6.1 Summary: A Python API
+for the Porn Site Eporner.com Home-page: https://github.com/EchterAlsFake/
 EPorner_API Author: Johannes Habel Author-email: EchterAlsFake@proton.me
 License: LGPLv3 Classifier: License :: OSI Approved :: GNU Lesser General
 Public License v3 (LGPLv3) Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests Requires-Dist: bs4 Requires-Dist: lxml
+requests Requires-Dist: bs4 Requires-Dist: lxml Requires-Dist: eaf_base_api
                            ************ EEPPoorrnneerr AAPPII ************
                     _[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_Q_L_ _A_n_a_l_y_s_i_s_]_[_A_P_I_ _T_e_s_t_s_]
 # Description EPorner API is an API for EPorner, which allows you to fetch
 information from videos using the official V2 API. # Disclaimer > Some modules
 of this API are in violence to the ToS from Eporner.com > See Documentation for
 details about this! Copyright Information: I have no intention of stealing
 copyright protected content or slowing down a website. Contact me at my E-Mail,
```

### Comparing `Eporner_API-1.6/eporner_api/eporner_api.py` & `Eporner_API-1.6.1/eporner_api/eporner_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import re
-
 import requests
 import json
-import os
 
 try:
     from .modules.consts import *
     from .modules.locals import *
     from .modules.errors import *
     from .modules.sorting import *
     from .modules.progressbar import *
@@ -17,14 +14,18 @@
     from modules.errors import *
     from modules.sorting import *
     from modules.progressbar import *
 
 from functools import cached_property
 from bs4 import BeautifulSoup
 from typing import Generator
+from base_api.base import Core
+from base_api.modules.quality import Quality
+from base_api.modules.download import legacy_download
+
 
 """
 Copyright (c) 2024 Johannes Habel
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
@@ -87,16 +88,15 @@
 
     def raw_json_data(self):
         """
         Uses the V2 API to retrieve information from a video
         :return:
         """
 
-        data = (requests.get(f"{ROOT_URL}{API_VIDEO_ID}?id={self.video_id}&thumbsize=medium&format=json")
-                .content.decode("utf-8"))
+        data = Core().get_content(f"{ROOT_URL}{API_VIDEO_ID}?id={self.video_id}&thumbsize=medium&format=json").decode("utf-8")
         parsed_data = json.loads(data)
         return parsed_data
 
     @cached_property
     def tags(self) -> list:
         tags = []
         tags_data = self.json_data["keywords"]
@@ -154,15 +154,15 @@
     The following methods are using HTML scraping. This is against the ToS from EPorner.com!
     """
 
     def request_html_content(self):
         if not self.enable_html:
             raise HTML_IS_DISABLED("HTML content is disabled! See Documentation for more details")
 
-        self.html_content = requests.get(self.url).content.decode("utf-8")
+        self.html_content = Core().get_content(self.url).decode("utf-8")
 
     def extract_json_from_html(self):
         if not self.enable_html:
             raise HTML_IS_DISABLED("HTML content is disabled! See Documentation for more details")
 
         soup = BeautifulSoup(self.html_content, 'lxml')
         script_tags = soup.find_all('script', {'type': 'application/ld+json'})
@@ -280,15 +280,15 @@
         :param quality:
         :param mode:
         :return: str
         """
         if not self.enable_html:
             raise HTML_IS_DISABLED("HTML content is disabled! See Documentation for more details")
 
-        quality = self.fix_quality(quality)
+        quality = Core().fix_quality(quality)
         soup = BeautifulSoup(self.html_content, 'html.parser')
         available_links = []
 
         # Define the quality preferences in descending order
         quality_preferences = ['2160p', '1440p', '1080p', '720p', '480p', '360p', '240p']
 
         # Search for all <a> tags and collect links for the specified mode
@@ -319,77 +319,38 @@
 
         # If no specific match is found, return None or the lowest available quality
         if len(available_links) <= 0:
             raise NotAvailable("No available links for given quality / mode found. Not all videos support AV1")
 
         return "https://eporner.com" + available_links[-1][1] if available_links else None
 
-    @classmethod
-    def fix_quality(cls, quality):
-
-        if isinstance(quality, Quality):
-            return quality
-
-        else:
-            if str(quality) == "best":
-                return Quality.BEST
-
-            elif str(quality) == "half":
-                return Quality.HALF
-
-            elif str(quality) == "worst":
-                return Quality.WORST
-
-    def download_video(self, quality, output_path, callback=None, mode=Encoding.mp4_h264):
+    def download(self, quality, path, callback=None, mode=Encoding.mp4_h264):
         if not self.enable_html:
             raise HTML_IS_DISABLED("HTML content is disabled! See Documentation for more details")
 
-        quality = self.fix_quality(quality)
-
+        quality = Core().fix_quality(quality)
         session = requests.Session()
         response_redirect_url = session.get(self.direct_download_link(quality, mode),
                                             allow_redirects=False)
 
         if 'Location' in response_redirect_url.headers:
             redirected_url = response_redirect_url.headers['Location']
-            response_download = session.get(redirected_url, stream=True)
-            file_size = int(response_download.headers.get('content-length', 0))
-
-            final_path = output_path
-            if callback is None:
-                progress_bar = Callback()
-
-            downloaded_so_far = 0
-
-            if not os.path.exists(final_path):
-                with open(final_path, 'wb') as file:
-                    for chunk in response_download.iter_content(chunk_size=1024):
-                        file.write(chunk)
-                        downloaded_so_far += len(chunk)
-
-                        if callback:
-                            callback(downloaded_so_far, file_size)
-
-                        else:
-                            progress_bar.text_progress_bar(downloaded=downloaded_so_far, total=file_size)
-
-                if not callback:
-                    del progress_bar
+            legacy_download(stream=True, url=redirected_url, callback=callback, path=path)
 
 
 class Pornstar:
     def __init__(self, url, enable_html_scraping=False):
         self.url = url
         self.enable_html_scraping = enable_html_scraping
         self.html_content = requests.get(self.url).text
 
     def videos(self, pages: int = 2) -> Generator:
         urls = []
         for page in range(pages):
-            response = requests.get(self.url).content.decode("utf-8")
+            response = Core().get_content(self.url).decode("utf-8")
             extraction = REGEX_SCRAPE_VIDEO_URLS.findall(response)
             for url in extraction:
                 url = f"https://www.eporner.com{url}"
                 url = url.replace("EPTHBN/", "")
                 urls.append(url)
 
         for url in urls:
@@ -485,30 +446,29 @@
     def get_video(cls, url, enable_html_scraping=False):
         return Video(url, enable_html_scraping=enable_html_scraping)
 
     @classmethod
     def search_videos(cls, query: str, sorting_gay: Gay, sorting_order: Order, sorting_low_quality: LowQuality,
                       page: int, per_page: int, enable_html_scraping=False):
 
-        response = requests.get(f"{ROOT_URL}{API_SEARCH}?query={query}&per_page={per_page}&%page={page}"
+        response = Core().get_content(f"{ROOT_URL}{API_SEARCH}?query={query}&per_page={per_page}&%page={page}"
                                 f"&thumbsize=medium&order={sorting_order}&gay={sorting_gay}&lq="
-                                f"{sorting_low_quality}&format=json")
+                                f"{sorting_low_quality}&format=json").decode("utf-8")
 
-        content = response.content.decode("utf-8")
-        json_data = json.loads(content)
+        json_data = json.loads(response)
         for video_ in json_data.get("videos", []):  # Don't know why this works lmao
             id_ = video_["url"]
             yield Video(id_, enable_html_scraping)
 
     @classmethod
     def get_videos_by_category(cls, category: Category, pages: int = 2, enable_html_scraping=False):
         urls = []
 
         for page in range(pages):
-            response = requests.get(f"{ROOT_URL}cat/{category}/{page}").content.decode("utf-8")
+            response = Core().get_content(f"{ROOT_URL}cat/{category}/{page}").decode("utf-8")
             extraction = REGEX_SCRAPE_VIDEO_URLS.findall(response)
             for url in extraction:
                 url = f"https://www.eporner.com{url}"
                 url = url.replace("EPTHBN/", "")
                 urls.append(url)
 
         for url in urls:
```

### Comparing `Eporner_API-1.6/eporner_api/modules/consts.py` & `Eporner_API-1.6.1/eporner_api/modules/consts.py`

 * *Files identical despite different names*

### Comparing `Eporner_API-1.6/eporner_api/modules/locals.py` & `Eporner_API-1.6.1/eporner_api/modules/locals.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,14 @@
 class Size:
     # Thumbnail Sizes
     small = "small"    # 190x152
     medium = "medium"  # 427x240
     big = "big"        # 640x360
 
 
-class Quality(Enum):
-    BEST = 'BEST'
-    HALF = 'HALF'
-    WORST = 'WORST'
-
-
 class Encoding:
     mp4_h264 = "h264"  # Same quality, more file size
     av1 = "AV1"  # Same quality, less file size
 
 
 class Category:
     ALL = "all"
```

### Comparing `Eporner_API-1.6/eporner_api/modules/progressbar.py` & `Eporner_API-1.6.1/eporner_api/modules/progressbar.py`

 * *Files identical despite different names*

### Comparing `Eporner_API-1.6/eporner_api/tests/test_category.py` & `Eporner_API-1.6.1/eporner_api/tests/test_category.py`

 * *Files identical despite different names*

### Comparing `Eporner_API-1.6/eporner_api/tests/test_pornstar.py` & `Eporner_API-1.6.1/eporner_api/tests/test_pornstar.py`

 * *Files identical despite different names*

### Comparing `Eporner_API-1.6/eporner_api/tests/test_search.py` & `Eporner_API-1.6.1/eporner_api/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `Eporner_API-1.6/eporner_api/tests/test_video.py` & `Eporner_API-1.6.1/eporner_api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `Eporner_API-1.6/setup.py` & `Eporner_API-1.6.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Eporner_API",
-    version="1.6",
+    version="1.6.1",
     packages=find_packages(),
     install_requires=[
-        "requests", "bs4", "lxml"
+        "requests", "bs4", "lxml", "eaf_base_api"
     ],
     entry_points={
         'console_scripts': [
             # If you want to create any executable scripts
         ],
     },
     author="Johannes Habel",
```

