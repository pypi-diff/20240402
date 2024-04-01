# Comparing `tmp/xnxx_api-1.2.tar.gz` & `tmp/xnxx_api-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnxx_api-1.2.tar", last modified: Sat Feb  3 17:27:37 2024, max compression
+gzip compressed data, was "xnxx_api-1.3.tar", last modified: Mon Apr  1 23:54:02 2024, max compression
```

## Comparing `xnxx_api-1.2.tar` & `xnxx_api-1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-03 17:27:37.046933 xnxx_api-1.2/
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2510 2024-02-03 17:27:37.046933 xnxx_api-1.2/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-02-03 17:27:37.046933 xnxx_api-1.2/setup.cfg
--rw-r--r--   0 asuna     (1000) asuna     (1000)      889 2024-02-03 17:27:26.000000 xnxx_api-1.2/setup.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-03 17:27:37.046933 xnxx_api-1.2/xnxx_api/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-01-29 17:29:40.000000 xnxx_api-1.2/xnxx_api/__init__.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-03 17:27:37.046933 xnxx_api-1.2/xnxx_api/modules/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-01-29 17:29:40.000000 xnxx_api-1.2/xnxx_api/modules/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      858 2024-02-03 17:01:23.000000 xnxx_api-1.2/xnxx_api/modules/consts.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     3859 2024-02-03 12:14:11.000000 xnxx_api-1.2/xnxx_api/modules/download.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      169 2024-01-29 17:29:40.000000 xnxx_api-1.2/xnxx_api/modules/errors.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      101 2024-01-29 17:58:31.000000 xnxx_api-1.2/xnxx_api/modules/locals.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      643 2024-02-03 12:14:11.000000 xnxx_api-1.2/xnxx_api/modules/progress_bars.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-03 17:27:37.046933 xnxx_api-1.2/xnxx_api/tests/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-03 16:36:00.000000 xnxx_api-1.2/xnxx_api/tests/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2154 2024-02-03 17:05:46.000000 xnxx_api-1.2/xnxx_api/tests/test_video.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     8370 2024-02-03 17:08:56.000000 xnxx_api-1.2/xnxx_api/xnxx_api.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-03 17:27:37.046933 xnxx_api-1.2/xnxx_api.egg-info/
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2510 2024-02-03 17:27:37.000000 xnxx_api-1.2/xnxx_api.egg-info/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)      445 2024-02-03 17:27:37.000000 xnxx_api-1.2/xnxx_api.egg-info/SOURCES.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-02-03 17:27:37.000000 xnxx_api-1.2/xnxx_api.egg-info/dependency_links.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       40 2024-02-03 17:27:37.000000 xnxx_api-1.2/xnxx_api.egg-info/requires.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)        9 2024-02-03 17:27:37.000000 xnxx_api-1.2/xnxx_api.egg-info/top_level.txt
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:54:02.342345 xnxx_api-1.3/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     7369 2024-03-28 01:26:26.000000 xnxx_api-1.3/LICENSE
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2431 2024-04-01 23:54:02.342345 xnxx_api-1.3/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-04-01 23:54:02.342345 xnxx_api-1.3/setup.cfg
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      905 2024-04-01 23:53:44.000000 xnxx_api-1.3/setup.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:54:02.342345 xnxx_api-1.3/xnxx_api/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 19:18:01.000000 xnxx_api-1.3/xnxx_api/__init__.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:54:02.342345 xnxx_api-1.3/xnxx_api/modules/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 19:18:01.000000 xnxx_api-1.3/xnxx_api/modules/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-29 15:52:32.000000 xnxx_api-1.3/xnxx_api/modules/category.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1784 2024-03-02 11:33:38.000000 xnxx_api-1.3/xnxx_api/modules/consts.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      169 2024-02-08 19:18:01.000000 xnxx_api-1.3/xnxx_api/modules/errors.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      267 2024-02-29 15:52:32.000000 xnxx_api-1.3/xnxx_api/modules/search_filters.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:54:02.342345 xnxx_api-1.3/xnxx_api/tests/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 19:18:01.000000 xnxx_api-1.3/xnxx_api/tests/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1982 2024-02-25 15:50:13.000000 xnxx_api-1.3/xnxx_api/tests/test_video.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     8539 2024-03-28 13:13:57.000000 xnxx_api-1.3/xnxx_api/xnxx_api.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:54:02.342345 xnxx_api-1.3/xnxx_api.egg-info/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2431 2024-04-01 23:54:02.000000 xnxx_api-1.3/xnxx_api.egg-info/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      427 2024-04-01 23:54:02.000000 xnxx_api-1.3/xnxx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-04-01 23:54:02.000000 xnxx_api-1.3/xnxx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       53 2024-04-01 23:54:02.000000 xnxx_api-1.3/xnxx_api.egg-info/requires.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        9 2024-04-01 23:54:02.000000 xnxx_api-1.3/xnxx_api.egg-info/top_level.txt
```

### Comparing `xnxx_api-1.2/PKG-INFO` & `xnxx_api-1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: xnxx_api
-Version: 1.2
+Version: 1.3
 Summary: A Python API for the Porn Site xnxx.com
 Home-page: https://github.com/EchterAlsFake/xnxx_api
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
 Requires-Dist: lxml
 Requires-Dist: ffmpeg-progress-yield
+Requires-Dist: eaf_base_api
 
 <h1 align="center">XNXX API</h1> 
 
 <div align="center">
     <a href="https://pepy.tech/project/xnxx_api"><img src="https://static.pepy.tech/badge/xnxx_api" alt="Downloads"></a>
     <a href="https://github.com/EchterAlsFake/xnxx_api/workflows/"><img src="https://github.com/EchterAlsFake/xnxx_api/workflows/CodeQL/badge.svg" alt="CodeQL Analysis"/></a>
     <a href="https://github.com/EchterAlsFake/xnxx_api/workflows/"><img src="https://github.com/EchterAlsFake/xnxx_api/actions/workflows/tests.yml/badge.svg" alt="API Tests"/></a>
@@ -24,19 +26,17 @@
 
 # Description
  
 XNXX API is an API for xnxx.com. It allows you to fetch information from videos using regexes and requests.
 
 # Disclaimer
 
-[!IMPORTANT] The xxnx API is in violation to xnxx's ToS!
-
-Copyright Information: I have no intention of stealing copyright protected content or slowing down
-a website. Contact me at my E-Mail, and I'll take this Repository immediately offline.
-
+> [!IMPORTANT] 
+> XNXX API is in violation to the ToS of xnxx.com!
+> If you are the website owner of xnxx.com, contact me at my E-Mail, and I'll take this repository immediately offline.
 > EchterAlsFake@proton.me
 
 # Quickstart
 
 ### Have a look at the [Documentation](https://github.com/EchterAlsFake/xnxx_api/blob/master/README/Documentation.md) for more details
 
 - Install the library with `pip install xnxx_api`
@@ -51,15 +51,15 @@
 video_object = client.get_video("<insert_url_here>")
 
 # Information from Video objects
 print(video_object.title)
 print(video_object.likes)
 # Download the video
 
-video_object.download(downloader=threaded, quality=Quality.BEST, output_path="your_output_path + filename")
+video_object.download(downloader=threaded, quality=Quality.BEST, path="your_output_path + filename")
 
 # SEE DOCUMENTATION FOR MORE
 ```
 
 # Changelog
 See [Changelog](https://github.com/EchterAlsFake/xnxx_api/blob/master/README/Changelog.md) for more details.
 
@@ -69,13 +69,7 @@
 
 Pull requests are also welcome.
 
 # License
 Licensed under the LGPLv3 License
 
 Copyright (C) 2023–2024 Johannes Habel
-
-# Support
-
-Leave a star on the repository. That's enough :) 
-
-
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: xnxx_api Version: 1.2 Summary: A Python API for the
+Metadata-Version: 2.1 Name: xnxx_api Version: 1.3 Summary: A Python API for the
 Porn Site xnxx.com Home-page: https://github.com/EchterAlsFake/xnxx_api Author:
 Johannes Habel Author-email: EchterAlsFake@proton.me License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
 (LGPLv3) Classifier: Programming Language :: Python Description-Content-Type:
-text/markdown Requires-Dist: requests Requires-Dist: bs4 Requires-Dist: lxml
-Requires-Dist: ffmpeg-progress-yield
+text/markdown License-File: LICENSE Requires-Dist: requests Requires-Dist: bs4
+Requires-Dist: lxml Requires-Dist: ffmpeg-progress-yield Requires-Dist:
+eaf_base_api
                             ************ XXNNXXXX AAPPII ************
                     _[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_Q_L_ _A_n_a_l_y_s_i_s_]_[_A_P_I_ _T_e_s_t_s_]
 # Description XNXX API is an API for xnxx.com. It allows you to fetch
-information from videos using regexes and requests. # Disclaimer [!IMPORTANT]
-The xxnx API is in violation to xnxx's ToS! Copyright Information: I have no
-intention of stealing copyright protected content or slowing down a website.
-Contact me at my E-Mail, and I'll take this Repository immediately offline. >
-EchterAlsFake@proton.me # Quickstart ### Have a look at the [Documentation]
-(https://github.com/EchterAlsFake/xnxx_api/blob/master/README/Documentation.md)
-for more details - Install the library with `pip install xnxx_api` ```python
-from xnxx_api.xnxx_api import Client, Quality, threaded # Initialize a Client
-object client = Client() # Fetch a video video_object = client.get_video("") #
-Information from Video objects print(video_object.title) print
-(video_object.likes) # Download the video video_object.download
-(downloader=threaded, quality=Quality.BEST, output_path="your_output_path +
-filename") # SEE DOCUMENTATION FOR MORE ``` # Changelog See [Changelog](https:/
-/github.com/EchterAlsFake/xnxx_api/blob/master/README/Changelog.md) for more
-details. # Contribution Do you see any issues or having some feature requests?
-Simply open an Issue or talk in the discussions. Pull requests are also
-welcome. # License Licensed under the LGPLv3 License Copyright (C) 2023â2024
-Johannes Habel # Support Leave a star on the repository. That's enough :)
+information from videos using regexes and requests. # Disclaimer > [!IMPORTANT]
+> XNXX API is in violation to the ToS of xnxx.com! > If you are the website
+owner of xnxx.com, contact me at my E-Mail, and I'll take this repository
+immediately offline. > EchterAlsFake@proton.me # Quickstart ### Have a look at
+the [Documentation](https://github.com/EchterAlsFake/xnxx_api/blob/master/
+README/Documentation.md) for more details - Install the library with `pip
+install xnxx_api` ```python from xnxx_api.xnxx_api import Client, Quality,
+threaded # Initialize a Client object client = Client() # Fetch a video
+video_object = client.get_video("") # Information from Video objects print
+(video_object.title) print(video_object.likes) # Download the video
+video_object.download(downloader=threaded, quality=Quality.BEST,
+path="your_output_path + filename") # SEE DOCUMENTATION FOR MORE ``` #
+Changelog See [Changelog](https://github.com/EchterAlsFake/xnxx_api/blob/
+master/README/Changelog.md) for more details. # Contribution Do you see any
+issues or having some feature requests? Simply open an Issue or talk in the
+discussions. Pull requests are also welcome. # License Licensed under the
+LGPLv3 License Copyright (C) 2023â2024 Johannes Habel
```

### Comparing `xnxx_api-1.2/setup.py` & `xnxx_api-1.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="xnxx_api",
-    version="1.2",
+    version="1.3",
     packages=find_packages(),
     install_requires=[
-        "requests", "bs4", "lxml", "ffmpeg-progress-yield"
+        "requests", "bs4", "lxml", "ffmpeg-progress-yield", "eaf_base_api"
     ],
     entry_points={
         'console_scripts': [
             # If you want to create any executable scripts
         ],
     },
     author="Johannes Habel",
```

### Comparing `xnxx_api-1.2/xnxx_api/tests/test_video.py` & `xnxx_api-1.3/xnxx_api/tests/test_video.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from ..xnxx_api import Video, Quality
-
-url = "https://www.xnxx.com/video-16vi44cb/besorg_dir_jetzt_ein_sex-date_auf_fuckmatch.fun_-_deutsch_fuck"
+from ..xnxx_api import Video
+from base_api.modules.quality import Quality
+url = "https://www.xnxx.com/video-1b9bufc9/die_zierliche_stieftochter_passt_kaum_in_den_mund_ihres_stiefvaters"
 # This will be the URL for all tests
 
 video = Video(url)
 
 
 def test_video_title():
     title = video.title
     assert isinstance(title, str) and len(title) > 0
 
 
-def test_uploader():
-    uploader = video.uploader
-    assert isinstance(uploader, str) and len(uploader) > 0
+def test_author():
+    author = video.author
+    assert isinstance(author, str) and len(author) > 0
 
 
 def test_length():
     length = video.length
     assert isinstance(length, str) and len(length) > 0
 
 
@@ -53,40 +53,29 @@
 
 def test_description():
     description = video.description
     assert isinstance(description, str) and len(description) > 0
 
 
 def test_keywords():
-    keywords = video.keywords
-    assert isinstance(keywords, list) and len(keywords) > 0
+    tags = video.tags
+    assert isinstance(tags, list) and len(tags) > 0
 
 
 def test_thumbnail_url():
     thumbnail_url = video.thumbnail_url
     assert isinstance(thumbnail_url, list) and len(thumbnail_url) > 0
 
 
-def test_upload_date():
-    upload_date = video.upload_date
-    assert isinstance(upload_date, str) and len(upload_date) > 0
+def test_publish_date():
+    publish_date = video.publish_date
+    assert isinstance(publish_date, str) and len(publish_date) > 0
 
 
 def test_content_url():
     content_url = video.content_url
     assert isinstance(content_url, str) and len(content_url) > 0
 
 
-def test_quality():
-    quality = video.fix_quality("best")
-    assert isinstance(quality, Quality)
-
-
 def test_get_segments():
-    segments = video.get_segments(quality=Quality.BEST)
-    segment_list = []
-
-    for segment in segments:
-        segment_list.append(segment)
-
-    assert len(segment_list) > 10
-
+    segments = list(video.get_segments(quality=Quality.BEST))
+    assert len(segments) > 10
```

### Comparing `xnxx_api-1.2/xnxx_api/xnxx_api.py` & `xnxx_api-1.3/xnxx_api/xnxx_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,62 @@
 try:
     from modules.consts import *
-    from modules.locals import *
     from modules.errors import *
-    from modules.download import *
-    from modules.progress_bars import *
+    from modules.search_filters import *
 
 except (ModuleNotFoundError, ImportError):
     from .modules.consts import *
-    from .modules.locals import *
     from .modules.errors import *
-    from .modules.download import *
-    from .modules.progress_bars import *
+    from .modules.search_filters import *
 
-import requests
 import json
 import html
 
 from bs4 import BeautifulSoup
 from functools import cached_property
+from base_api.base import Core
+from base_api.modules.progress_bars import Callback
 
 
 class Video:
     def __init__(self, url):
         self.url = url
         self.available_m3u8_urls = None
         self.available_qualities = None
         self.script_content = None
         self.html_content = None
         self.metadata_matches = None
         self.json_content = None
-        self.session = requests.Session()
 
         if not REGEX_VIDEO_CHECK.search(self.url):
             raise InvalidUrl("The video URL is invalid!")
 
         else:
             self.get_base_html()
             self.get_script_content()
             self.get_metadata_matches()
             self.extract_json_from_html()
 
     def get_base_html(self):
-        self.html_content = requests.get(self.url).content.decode("utf-8")
+        self.html_content = Core.get_content(url=self.url, headers=None, cookies=None).decode("utf-8")
 
     @classmethod
     def is_desired_script(cls, tag):
         if tag.name != "script":
             return False
         script_contents = ['html5player', 'setVideoTitle', 'setVideoUrlLow', 'setVideoUrlHigh']
         return all(content in tag.text for content in script_contents)
 
     def get_metadata_matches(self):
         soup = BeautifulSoup(self.html_content, 'html.parser')
         metadata_span = soup.find('span', class_='metadata')
         metadata_text = metadata_span.get_text(separator=' ', strip=True)
 
         # Use a regex to extract the desired strings
-        # This regex looks for patterns of text that could represent the data you're interested in
-        self.metadata_matches = re.findall(r'(\d+min|\d+p|\d[\d\.,]*\s*[views]*)', metadata_text)
+        self.metadata_matches = re.findall(r'(\d+min|\d+p|\d[\d.,]*\s*[views]*)', metadata_text)
 
     def get_script_content(self):
         soup = BeautifulSoup(self.html_content, 'lxml')
         target_script = soup.find(self.is_desired_script)
         if target_script:
             self.script_content = target_script.text
 
@@ -76,80 +71,35 @@
         if script_tag:
             json_text = script_tag.string.strip()  # Get the content of the tag as a string
             data = json.loads(json_text)
             self.json_content = data
 
     @cached_property
     def m3u8_base_url(self):
+        """
+        The m3u8 base URL is a file that contains the list of segments (.ts files) for the different resolutions.
+        This is basically the whole magic for all my APIs :)
+        :return: (str) The m3u8 base URL
+        """
         return REGEX_VIDEO_M3U8.search(self.script_content).group(1)
 
-    def get_available_qualities(self):
-        response = self.session.get(self.m3u8_base_url)
-        content = response.content.decode("utf-8")
-        lines = content.splitlines()
-
-        quality_url_map = {}
-        base_qualities = ["250p", "360p", "480p", "720p", "1080p"]
-
-        for line in lines:
-            for quality in base_qualities:
-                if f"hls-{quality}" in line:
-                    quality_url_map[quality] = line
-
-        self.quality_url_map = quality_url_map
-        self.available_qualities = list(quality_url_map.keys())
-        return self.available_qualities
-
-    def get_m3u8_by_quality(self, quality):
-        quality = self.fix_quality(quality)
-
-        self.get_available_qualities()
-        base_qualities = ["250p", "360p", "480p", "720p", "1080p"]
-        if quality == Quality.BEST:
-            selected_quality = max(self.available_qualities, key=lambda q: base_qualities.index(q))
-        elif quality == Quality.WORST:
-            selected_quality = min(self.available_qualities, key=lambda q: base_qualities.index(q))
-        elif quality == Quality.HALF:
-            sorted_qualities = sorted(self.available_qualities, key=lambda q: base_qualities.index(q))
-            middle_index = len(sorted_qualities) // 2
-            selected_quality = sorted_qualities[middle_index]
-
-        return self.quality_url_map.get(selected_quality)
-
     def get_segments(self, quality):
+        quality = Core().fix_quality(quality)
+        segments = Core().get_segments(quality=quality, m3u8_base_url=self.m3u8_base_url)
+        return segments
 
-        quality = self.fix_quality(quality)
-
-        # Some inspiration from PHUB (xD)
-        base_url = self.m3u8_base_url
-        new_segment = self.get_m3u8_by_quality(quality)
-        # Split the base URL into components
-        url_components = base_url.split('/')
-
-        # Replace the last component with the new segment
-        url_components[-1] = new_segment
-
-        # Rejoin the components into the new full URL
-        new_url = '/'.join(url_components)
-        master_src = self.session.get(url=new_url).text
-
-        urls = [l for l in master_src.splitlines()
-                if l and not l.startswith('#')]
-
-        for url in urls:
-            url_components[-1] = url
-            new_url = '/'.join(url_components)
-            yield new_url
+    def download(self, quality, path, downloader, callback=Callback.text_progress_bar):
+        Core().download(video=self, quality=quality, path=path, callback=callback, downloader=downloader)
 
     @cached_property
     def title(self) -> str:
         return html.unescape(REGEX_VIDEO_TITLE.search(self.script_content).group(1))
 
     @cached_property
-    def uploader(self) -> str:
+    def author(self) -> str:
         return REGEX_VIDEO_UPLOADER.search(self.script_content).group(1)
 
     @cached_property
     def length(self) -> str:
         return self.metadata_matches[0]
 
     @cached_property
@@ -179,77 +129,136 @@
         for pornstar in pornstar_list:
             pornstar = str(pornstar).replace("+", " ")
             pornstar_list_filtered.append(pornstar)
 
         return pornstar_list_filtered
 
     @cached_property
-    def keywords(self) -> list:
-        keyword_list = REGEX_VIDEO_KEYWORDS.findall(self.html_content)
-        keyword_list_filtered = []
-        for keyword in keyword_list:
-            keyword = str(keyword).replace("+", " ")
-            keyword_list_filtered.append(keyword)
+    def tags(self) -> list:
+        tags_list = REGEX_VIDEO_KEYWORDS.findall(self.html_content)
+        tags_list_filtered = []
+        for tag in tags_list:
+            tag = str(tag).replace("+", " ")
+            tags_list_filtered.append(tag)
 
-        return keyword_list_filtered
+        return tags_list_filtered
 
     @cached_property
     def description(self) -> str:
         return html.unescape(self.json_content["description"])
 
     @cached_property
     def thumbnail_url(self) -> list:
         return self.json_content["thumbnailUrl"]
 
     @cached_property
-    def upload_date(self) -> str:
+    def publish_date(self) -> str:
         return self.json_content["uploadDate"]
 
     @cached_property
     def content_url(self) -> str:
         return self.json_content["contentUrl"]
 
+
+class Search:
+    def __init__(self, query: str, upload_time: UploadTime, length: Length, searching_quality: SearchingQuality):
+        self.query = self.validate_query(query)
+        self.upload_time = upload_time
+        self.length = length
+        self.searching_quality = searching_quality
+
     @classmethod
-    def fix_quality(cls, quality):
-        # Needed for Porn Fetch
+    def validate_query(cls, query):
+        return query.replace(" ", "+")
 
-        if isinstance(quality, Quality):
-            return quality
+    @cached_property
+    def html_content(self):
+        # Now this is going to be weird, just don't ask
+        return Core().get_content(f"https://www.xnxx.com/search{self.upload_time}{self.length}{self.searching_quality}/{self.query}", headers=HEADERS).decode("utf-8")
 
-        else:
-            if str(quality) == "best":
-                return Quality.BEST
+    @cached_property
+    def total_pages(self):
+        return REGEX_SEARCH_TOTAL_PAGES.search(self.html_content).group(1)
 
-            elif str(quality) == "half":
-                return Quality.HALF
+    @cached_property
+    def videos(self):
+        page = 0
+        while True:
 
-            elif str(quality) == "worst":
-                return Quality.WORST
+            if page == 0:
+                url = f"https://www.xnxx.com/search{self.upload_time}{self.length}{self.searching_quality}/{self.query}"
 
-    def download(self, downloader, quality, output_path, callback=None):
-        """
-        :param callback:
-        :param downloader:
-        :param quality:
-        :param output_path:
-        :return:
-        """
-        quality = self.fix_quality(quality)
+            else:
+                url = f"https://www.xnxx.com/search{self.upload_time}{self.length}{self.searching_quality}/{self.query}/{page}"
 
-        if callback is None:
-            callback = Callback.text_progress_bar
+            content = Core().get_content(url, headers=HEADERS).decode("utf-8")
+            urls = REGEX_SCRAPE_VIDEOS.findall(content)
+            for url_ in urls:
+                yield Video(f"https://www.xnxx.com/video-{url_}")
 
-        if downloader == default or str(downloader) == "default":
-            default(video=self, quality=quality, path=output_path, callback=callback)
+            if int(page) >= int(self.total_pages):
+                break
 
-        elif downloader == threaded or str(downloader) == "threaded":
-            threaded(video=self, quality=quality, path=output_path, callback=callback)
+            page += 1
 
-        elif downloader == FFMPEG or str(downloader) == "FFMPEG":
-            FFMPEG(video=self, quality=quality, path=output_path, callback=callback)
+
+class User:
+    def __init__(self, url):
+        self.url = url
+        self.pages = round(self.total_videos / 50)
+
+    @cached_property
+    def base_json(self):
+        url = f"{self.url}/videos/best/0?from=goldtab"
+        content = Core().get_content(url, headers=HEADERS).decode("utf-8")
+        data = html.unescape(json.loads(content))
+        return data
+
+    @cached_property
+    def videos(self):
+        page = 0
+        while True:
+            page += 1
+            url = f"{self.url}/videos/best/{page}?from=goldtab"
+            content = Core().get_content(url, headers=HEADERS).decode("utf-8")
+            data = html.unescape(json.loads(content))
+            videos = data["videos"]
+            for video in videos:
+                url = video.get("u")
+                yield Video(f"https://www.xnxx.com{url}")
+
+            if int(page) >= int(self.pages):
+                break
+
+    @cached_property
+    def total_videos(self):
+        return self.base_json["nb_videos"]
 
 
 class Client:
 
     @classmethod
     def get_video(cls, url):
+        """
+        :param url: (str) The URL of the video
+        :return: (Video) The video object
+        """
         return Video(url)
+
+    @classmethod
+    def search(cls, query, upload_time: UploadTime = "", length: Length = "", searching_quality: SearchingQuality = ""):
+        """
+        :param query:
+        :param upload_time:
+        :param length:
+        :param searching_quality:
+        :return: (Search) the search object
+        """
+        return Search(query, upload_time, length, searching_quality)
+
+    @classmethod
+    def get_user(cls, url):
+        """
+        :param url: (str) The user URL
+        :return: (User) The User object
+        """
+        return User(url)
```

### Comparing `xnxx_api-1.2/xnxx_api.egg-info/PKG-INFO` & `xnxx_api-1.3/xnxx_api.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: xnxx_api
-Version: 1.2
+Version: 1.3
 Summary: A Python API for the Porn Site xnxx.com
 Home-page: https://github.com/EchterAlsFake/xnxx_api
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
 Requires-Dist: lxml
 Requires-Dist: ffmpeg-progress-yield
+Requires-Dist: eaf_base_api
 
 <h1 align="center">XNXX API</h1> 
 
 <div align="center">
     <a href="https://pepy.tech/project/xnxx_api"><img src="https://static.pepy.tech/badge/xnxx_api" alt="Downloads"></a>
     <a href="https://github.com/EchterAlsFake/xnxx_api/workflows/"><img src="https://github.com/EchterAlsFake/xnxx_api/workflows/CodeQL/badge.svg" alt="CodeQL Analysis"/></a>
     <a href="https://github.com/EchterAlsFake/xnxx_api/workflows/"><img src="https://github.com/EchterAlsFake/xnxx_api/actions/workflows/tests.yml/badge.svg" alt="API Tests"/></a>
@@ -24,19 +26,17 @@
 
 # Description
  
 XNXX API is an API for xnxx.com. It allows you to fetch information from videos using regexes and requests.
 
 # Disclaimer
 
-[!IMPORTANT] The xxnx API is in violation to xnxx's ToS!
-
-Copyright Information: I have no intention of stealing copyright protected content or slowing down
-a website. Contact me at my E-Mail, and I'll take this Repository immediately offline.
-
+> [!IMPORTANT] 
+> XNXX API is in violation to the ToS of xnxx.com!
+> If you are the website owner of xnxx.com, contact me at my E-Mail, and I'll take this repository immediately offline.
 > EchterAlsFake@proton.me
 
 # Quickstart
 
 ### Have a look at the [Documentation](https://github.com/EchterAlsFake/xnxx_api/blob/master/README/Documentation.md) for more details
 
 - Install the library with `pip install xnxx_api`
@@ -51,15 +51,15 @@
 video_object = client.get_video("<insert_url_here>")
 
 # Information from Video objects
 print(video_object.title)
 print(video_object.likes)
 # Download the video
 
-video_object.download(downloader=threaded, quality=Quality.BEST, output_path="your_output_path + filename")
+video_object.download(downloader=threaded, quality=Quality.BEST, path="your_output_path + filename")
 
 # SEE DOCUMENTATION FOR MORE
 ```
 
 # Changelog
 See [Changelog](https://github.com/EchterAlsFake/xnxx_api/blob/master/README/Changelog.md) for more details.
 
@@ -69,13 +69,7 @@
 
 Pull requests are also welcome.
 
 # License
 Licensed under the LGPLv3 License
 
 Copyright (C) 2023–2024 Johannes Habel
-
-# Support
-
-Leave a star on the repository. That's enough :) 
-
-
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: xnxx_api Version: 1.2 Summary: A Python API for the
+Metadata-Version: 2.1 Name: xnxx_api Version: 1.3 Summary: A Python API for the
 Porn Site xnxx.com Home-page: https://github.com/EchterAlsFake/xnxx_api Author:
 Johannes Habel Author-email: EchterAlsFake@proton.me License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
 (LGPLv3) Classifier: Programming Language :: Python Description-Content-Type:
-text/markdown Requires-Dist: requests Requires-Dist: bs4 Requires-Dist: lxml
-Requires-Dist: ffmpeg-progress-yield
+text/markdown License-File: LICENSE Requires-Dist: requests Requires-Dist: bs4
+Requires-Dist: lxml Requires-Dist: ffmpeg-progress-yield Requires-Dist:
+eaf_base_api
                             ************ XXNNXXXX AAPPII ************
                     _[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_Q_L_ _A_n_a_l_y_s_i_s_]_[_A_P_I_ _T_e_s_t_s_]
 # Description XNXX API is an API for xnxx.com. It allows you to fetch
-information from videos using regexes and requests. # Disclaimer [!IMPORTANT]
-The xxnx API is in violation to xnxx's ToS! Copyright Information: I have no
-intention of stealing copyright protected content or slowing down a website.
-Contact me at my E-Mail, and I'll take this Repository immediately offline. >
-EchterAlsFake@proton.me # Quickstart ### Have a look at the [Documentation]
-(https://github.com/EchterAlsFake/xnxx_api/blob/master/README/Documentation.md)
-for more details - Install the library with `pip install xnxx_api` ```python
-from xnxx_api.xnxx_api import Client, Quality, threaded # Initialize a Client
-object client = Client() # Fetch a video video_object = client.get_video("") #
-Information from Video objects print(video_object.title) print
-(video_object.likes) # Download the video video_object.download
-(downloader=threaded, quality=Quality.BEST, output_path="your_output_path +
-filename") # SEE DOCUMENTATION FOR MORE ``` # Changelog See [Changelog](https:/
-/github.com/EchterAlsFake/xnxx_api/blob/master/README/Changelog.md) for more
-details. # Contribution Do you see any issues or having some feature requests?
-Simply open an Issue or talk in the discussions. Pull requests are also
-welcome. # License Licensed under the LGPLv3 License Copyright (C) 2023â2024
-Johannes Habel # Support Leave a star on the repository. That's enough :)
+information from videos using regexes and requests. # Disclaimer > [!IMPORTANT]
+> XNXX API is in violation to the ToS of xnxx.com! > If you are the website
+owner of xnxx.com, contact me at my E-Mail, and I'll take this repository
+immediately offline. > EchterAlsFake@proton.me # Quickstart ### Have a look at
+the [Documentation](https://github.com/EchterAlsFake/xnxx_api/blob/master/
+README/Documentation.md) for more details - Install the library with `pip
+install xnxx_api` ```python from xnxx_api.xnxx_api import Client, Quality,
+threaded # Initialize a Client object client = Client() # Fetch a video
+video_object = client.get_video("") # Information from Video objects print
+(video_object.title) print(video_object.likes) # Download the video
+video_object.download(downloader=threaded, quality=Quality.BEST,
+path="your_output_path + filename") # SEE DOCUMENTATION FOR MORE ``` #
+Changelog See [Changelog](https://github.com/EchterAlsFake/xnxx_api/blob/
+master/README/Changelog.md) for more details. # Contribution Do you see any
+issues or having some feature requests? Simply open an Issue or talk in the
+discussions. Pull requests are also welcome. # License Licensed under the
+LGPLv3 License Copyright (C) 2023â2024 Johannes Habel
```

