# Comparing `tmp/xvideos_api-1.1.tar.gz` & `tmp/xvideos_api-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xvideos_api-1.1.tar", last modified: Tue Feb  6 00:04:45 2024, max compression
+gzip compressed data, was "xvideos_api-1.2.tar", last modified: Mon Apr  1 23:50:48 2024, max compression
```

## Comparing `xvideos_api-1.1.tar` & `xvideos_api-1.2.tar`

### file list

```diff
@@ -1,26 +1,23 @@
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-06 00:04:45.272338 xvideos_api-1.1/
--rw-r--r--   0 asuna     (1000) asuna     (1000)    31941 2024-02-05 21:16:20.000000 xvideos_api-1.1/LICENSE
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2589 2024-02-06 00:04:45.269004 xvideos_api-1.1/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-02-06 00:04:45.272338 xvideos_api-1.1/setup.cfg
--rw-r--r--   0 asuna     (1000) asuna     (1000)      902 2024-02-06 00:04:41.000000 xvideos_api-1.1/setup.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-06 00:04:45.269004 xvideos_api-1.1/xvideos_api/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-05 21:16:20.000000 xvideos_api-1.1/xvideos_api/__init__.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-06 00:04:45.269004 xvideos_api-1.1/xvideos_api/modules/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-05 21:16:20.000000 xvideos_api-1.1/xvideos_api/modules/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      971 2024-02-05 23:36:27.000000 xvideos_api-1.1/xvideos_api/modules/consts.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     3836 2024-02-05 21:16:20.000000 xvideos_api-1.1/xvideos_api/modules/download.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)       81 2024-02-05 21:16:20.000000 xvideos_api-1.1/xvideos_api/modules/exceptions.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      101 2024-02-05 21:16:20.000000 xvideos_api-1.1/xvideos_api/modules/locals.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      644 2024-02-05 21:16:20.000000 xvideos_api-1.1/xvideos_api/modules/progress_bars.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      672 2024-02-05 22:39:20.000000 xvideos_api-1.1/xvideos_api/modules/sorting.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-06 00:04:45.269004 xvideos_api-1.1/xvideos_api/tests/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-05 21:16:20.000000 xvideos_api-1.1/xvideos_api/tests/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2981 2024-02-05 23:55:02.000000 xvideos_api-1.1/xvideos_api/tests/test_search.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1563 2024-02-05 21:16:20.000000 xvideos_api-1.1/xvideos_api/tests/test_video.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)    10572 2024-02-05 23:56:21.000000 xvideos_api-1.1/xvideos_api/xvideos_api.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-02-06 00:04:45.269004 xvideos_api-1.1/xvideos_api.egg-info/
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2589 2024-02-06 00:04:45.000000 xvideos_api-1.1/xvideos_api.egg-info/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)      569 2024-02-06 00:04:45.000000 xvideos_api-1.1/xvideos_api.egg-info/SOURCES.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-02-06 00:04:45.000000 xvideos_api-1.1/xvideos_api.egg-info/dependency_links.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       40 2024-02-06 00:04:45.000000 xvideos_api-1.1/xvideos_api.egg-info/requires.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       12 2024-02-06 00:04:45.000000 xvideos_api-1.1/xvideos_api.egg-info/top_level.txt
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:50:48.342865 xvideos_api-1.2/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     7369 2024-03-28 01:24:01.000000 xvideos_api-1.2/LICENSE
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2542 2024-04-01 23:50:48.342865 xvideos_api-1.2/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-04-01 23:50:48.342865 xvideos_api-1.2/setup.cfg
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      918 2024-04-01 23:49:55.000000 xvideos_api-1.2/setup.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:50:48.339532 xvideos_api-1.2/xvideos_api/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/__init__.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:50:48.339532 xvideos_api-1.2/xvideos_api/modules/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/modules/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1204 2024-03-29 11:49:46.000000 xvideos_api-1.2/xvideos_api/modules/consts.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       81 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/modules/exceptions.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      672 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/modules/sorting.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:50:48.342865 xvideos_api-1.2/xvideos_api/tests/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/tests/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2981 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/tests/test_search.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1550 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/tests/test_video.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)    10191 2024-03-29 12:19:12.000000 xvideos_api-1.2/xvideos_api/xvideos_api.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:50:48.342865 xvideos_api-1.2/xvideos_api.egg-info/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2542 2024-04-01 23:50:48.000000 xvideos_api-1.2/xvideos_api.egg-info/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      470 2024-04-01 23:50:48.000000 xvideos_api-1.2/xvideos_api.egg-info/SOURCES.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-04-01 23:50:48.000000 xvideos_api-1.2/xvideos_api.egg-info/dependency_links.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       53 2024-04-01 23:50:48.000000 xvideos_api-1.2/xvideos_api.egg-info/requires.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       12 2024-04-01 23:50:48.000000 xvideos_api-1.2/xvideos_api.egg-info/top_level.txt
```

### Comparing `xvideos_api-1.1/PKG-INFO` & `xvideos_api-1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 Metadata-Version: 2.1
 Name: xvideos_api
-Version: 1.1
+Version: 1.2
 Summary: A Python API for the Porn Site xvideos.com
 Home-page: https://github.com/EchterAlsFake/xvideos_api
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
 Requires-Dist: ffmpeg-progress-yield
+Requires-Dist: eaf_base_api
 
 <h1 align="center">XVIDEOS API</h1> 
 
 <div align="center">
     <a href="https://pepy.tech/project/xvideos_api"><img src="https://static.pepy.tech/badge/xvideos_api" alt="Downloads"></a>
     <a href="https://github.com/EchterAlsFake/xvideos_api/workflows/"><img src="https://github.com/EchterAlsFake/xvideos_api/workflows/CodeQL/badge.svg" alt="CodeQL Analysis"/></a>
     <a href="https://github.com/EchterAlsFake/xvideos_api/workflows/"><img src="https://github.com/EchterAlsFake/xvideos_api/actions/workflows/tests.yml/badge.svg" alt="API Tests"/></a>
 </div>
 
 # Description
- 
-xvideos API is an API for xvideos.com. It allows you to fetch information from videos using regexes and requests.
+XVideos API is an API for xvideos.com. It allows you to fetch information from videos using regexes and requests.
 
 # Disclaimer
-
-[!IMPORTANT] The xvideos API is in violation to xvideos's ToS!
-
-Copyright Information: I have no intention of stealing copyright protected content or slowing down
-a website. Contact me at my E-Mail, and I'll take this Repository immediately offline.
-
+> [!IMPORTANT] 
+> XVideos API is in violation to the ToS of xvideos.com!
+> If you are the website owner of xvideos.com, contact me at my E-Mail, and I'll take this repository immediately offline.
 > EchterAlsFake@proton.me
 
 # Quickstart
 
 ### Have a look at the [Documentation](https://github.com/EchterAlsFake/xvideos_api/blob/master/README/Documentation.md) for more details
 
 - Install the library with `pip install xvideos_api`
 
 
 ```python
-from xvideos_api.xvideos_api import Client, Quality, threaded
+from xvideos_api.xvideos_api import Client, Quality
+from base_api.modules.download import threaded, default, FFMPEG
 # Initialize a Client object
 client = Client()
 
 # Fetch a video
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
 See [Changelog](https://github.com/EchterAlsFake/xvideos_api/blob/master/README/Changelog.md) for more details.
 
@@ -70,13 +68,7 @@
 
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
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: xvideos_api Version: 1.1 Summary: A Python API for
+Metadata-Version: 2.1 Name: xvideos_api Version: 1.2 Summary: A Python API for
 the Porn Site xvideos.com Home-page: https://github.com/EchterAlsFake/
 xvideos_api Author: Johannes Habel Author-email: EchterAlsFake@proton.me
 License: LGPLv3 Classifier: License :: OSI Approved :: GNU Lesser General
 Public License v3 (LGPLv3) Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: bs4 Requires-Dist: lxml Requires-Dist: ffmpeg-progress-
-yield
+yield Requires-Dist: eaf_base_api
                            ************ XXVVIIDDEEOOSS AAPPII ************
                     _[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_Q_L_ _A_n_a_l_y_s_i_s_]_[_A_P_I_ _T_e_s_t_s_]
-# Description xvideos API is an API for xvideos.com. It allows you to fetch
-information from videos using regexes and requests. # Disclaimer [!IMPORTANT]
-The xvideos API is in violation to xvideos's ToS! Copyright Information: I have
-no intention of stealing copyright protected content or slowing down a website.
-Contact me at my E-Mail, and I'll take this Repository immediately offline. >
-EchterAlsFake@proton.me # Quickstart ### Have a look at the [Documentation]
-(https://github.com/EchterAlsFake/xvideos_api/blob/master/README/
-Documentation.md) for more details - Install the library with `pip install
-xvideos_api` ```python from xvideos_api.xvideos_api import Client, Quality,
-threaded # Initialize a Client object client = Client() # Fetch a video
-video_object = client.get_video("") # Information from Video objects print
-(video_object.title) print(video_object.likes) # Download the video
-video_object.download(downloader=threaded, quality=Quality.BEST,
-output_path="your_output_path + filename") # SEE DOCUMENTATION FOR MORE ``` #
-Changelog See [Changelog](https://github.com/EchterAlsFake/xvideos_api/blob/
-master/README/Changelog.md) for more details. # Contribution Do you see any
-issues or having some feature requests? Simply open an Issue or talk in the
-discussions. Pull requests are also welcome. # License Licensed under the
-LGPLv3 License Copyright (C) 2023â2024 Johannes Habel # Support Leave a star
-on the repository. That's enough :)
+# Description XVideos API is an API for xvideos.com. It allows you to fetch
+information from videos using regexes and requests. # Disclaimer > [!IMPORTANT]
+> XVideos API is in violation to the ToS of xvideos.com! > If you are the
+website owner of xvideos.com, contact me at my E-Mail, and I'll take this
+repository immediately offline. > EchterAlsFake@proton.me # Quickstart ### Have
+a look at the [Documentation](https://github.com/EchterAlsFake/xvideos_api/
+blob/master/README/Documentation.md) for more details - Install the library
+with `pip install xvideos_api` ```python from xvideos_api.xvideos_api import
+Client, Quality from base_api.modules.download import threaded, default, FFMPEG
+# Initialize a Client object client = Client() # Fetch a video video_object =
+client.get_video("") # Information from Video objects print(video_object.title)
+print(video_object.likes) # Download the video video_object.download
+(downloader=threaded, quality=Quality.BEST, path="your_output_path + filename")
+# SEE DOCUMENTATION FOR MORE ``` # Changelog See [Changelog](https://
+github.com/EchterAlsFake/xvideos_api/blob/master/README/Changelog.md) for more
+details. # Contribution Do you see any issues or having some feature requests?
+Simply open an Issue or talk in the discussions. Pull requests are also
+welcome. # License Licensed under the LGPLv3 License Copyright (C) 2023â2024
+Johannes Habel
```

### Comparing `xvideos_api-1.1/setup.py` & `xvideos_api-1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="xvideos_api",
-    version="1.1",
+    version="1.2",
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

### Comparing `xvideos_api-1.1/xvideos_api/modules/sorting.py` & `xvideos_api-1.2/xvideos_api/modules/sorting.py`

 * *Files identical despite different names*

### Comparing `xvideos_api-1.1/xvideos_api/tests/test_search.py` & `xvideos_api-1.2/xvideos_api/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `xvideos_api-1.1/xvideos_api/tests/test_video.py` & `xvideos_api-1.2/xvideos_api/tests/test_video.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def test_title():
     assert isinstance(video.title, str) and len(video.title) > 0
 
 
 def test_uploader():
-    assert isinstance(video.uploader, str) and len(video.uploader) > 0
+    assert isinstance(video.author, str) and len(video.author) > 0
 
 
 def test_length():
     assert isinstance(video.length, str) and len(video.length) > 0
 
 
 def test_views():
@@ -39,24 +39,24 @@
     assert isinstance(video.rating_votes, str) and len(video.rating_votes) > 0
 
 
 def test_description():
     assert isinstance(video.description, str) and len(video.description) > 0
 
 
-def test_keywords():
-    assert isinstance(video.keywords, list) and len(video.keywords) > 0
+def test_tags():
+    assert isinstance(video.tags, list) and len(video.tags) > 0
 
 
 def test_thumbnail_url():
     assert isinstance(video.thumbnail_url, str) and len(video.thumbnail_url) > 0
 
 
-def test_upload_date():
-    assert isinstance(video.upload_date, str) and len(video.upload_date) > 0
+def test_publish_date():
+    assert isinstance(video.publish_date, str) and len(video.publish_date) > 0
 
 
 def test_content_url():
     assert isinstance(video.content_url, str) and len(video.content_url) > 0
 
 
 def test_pornstars():
```

### Comparing `xvideos_api-1.1/xvideos_api/xvideos_api.py` & `xvideos_api-1.2/xvideos_api/xvideos_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,73 +11,74 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-import requests
 import json
 import html
+import logging
 
 from bs4 import BeautifulSoup
 from functools import cached_property
+from base_api.base import Core, threaded, default, FFMPEG
+from base_api.modules.download import legacy_download
+from base_api.modules.quality import Quality
 
 try:
     from modules.consts import *
     from modules.exceptions import *
-    from modules.locals import *
-    from modules.progress_bars import *
-    from modules.download import *
     from modules.sorting import *
 
 except (ModuleNotFoundError, ImportError):
     from .modules.consts import *
     from .modules.exceptions import *
-    from .modules.locals import *
-    from .modules.progress_bars import *
-    from .modules.download import *
     from .modules.sorting import *
 
 
 class Video:
     def __init__(self, url):
+        """
+        :param url: (str) The URL of the video
+        """
         self.url = self.check_url(url)
-        self.session = requests.Session()
-        headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/121.0.0.0 Safari/537.36'}
-
-        self.session.headers.update(headers)
-
         self.html_content = self.get_html_content()
         self.json_data = self.flatten_json(nested_json=self.extract_json_from_html())
         self.script_content = self.get_script_content()
+        self.quality_url_map = None
+        self.available_qualities = None
 
     @classmethod
-    def check_url(cls, url):
+    def check_url(cls, url) -> str:
+        """
+        :param url: (str) The URL of the video
+        :return: (str) The URL of the video, if valid, otherwise raises InvalidUrl Exception
+        """
         match = REGEX_VIDEO_CHECK_URL.match(url)
         if match:
             return url
 
         else:
             raise InvalidUrl
 
     @classmethod
     def is_desired_script(cls, tag):
         if tag.name != "script":
             return False
-        script_contents = ['html5player', 'setVideoTitle', 'setVideoUrlLow', 'setVideoUrlHigh']
+        script_contents = ['html5player', 'setVideoTitle', 'setVideoUrlLow']
         return all(content in tag.text for content in script_contents)
 
     def get_script_content(self):
         soup = BeautifulSoup(self.html_content, 'lxml')
         target_script = soup.find(self.is_desired_script)
         return target_script.text
 
     def get_html_content(self):
-        return self.session.get(self.url).content.decode("utf-8")
+        return Core().get_content(self.url, headers=headers).decode("utf-8")
 
     def extract_json_from_html(self):
         soup = BeautifulSoup(self.html_content, 'lxml')
         script_tags = soup.find_all('script', {'type': 'application/ld+json'})
 
         combined_data = {}
 
@@ -102,110 +103,77 @@
             new_key = f"{parent_key}{sep}{k}" if parent_key else k
             if isinstance(v, dict):
                 items.extend(self.flatten_json(v, new_key, sep=sep).items())
             else:
                 items.append((new_key, v))
         return dict(items)
 
-    def get_available_qualities(self):
-        response = self.session.get(self.m3u8_base_url)
-        content = response.content.decode("utf-8")
-        lines = content.splitlines()
+    def get_available_qualities(self) -> list:
+        """
+        :return: (list) List of available qualities
+        """
+        response = Core().get_content(self.m3u8_base_url, headers=headers).decode("utf-8")
+        lines = response.splitlines()
 
         quality_url_map = {}
         base_qualities = ["250p", "360p", "480p", "720p", "1080p"]
 
         for line in lines:
             for quality in base_qualities:
                 if f"hls-{quality}" in line:
                     quality_url_map[quality] = line
 
         self.quality_url_map = quality_url_map
         self.available_qualities = list(quality_url_map.keys())
         return self.available_qualities
 
     def get_m3u8_by_quality(self, quality):
-        quality = self.fix_quality(quality)
+        """
+        :param quality: (str, Quality) The video quality
+        :return: (str) The m3u8 URL for the given quality
+        """
+        quality = Core().fix_quality(quality)
 
         self.get_available_qualities()
         base_qualities = ["250p", "360p", "480p", "720p", "1080p"]
         if quality == Quality.BEST:
             selected_quality = max(self.available_qualities, key=lambda q: base_qualities.index(q))
         elif quality == Quality.WORST:
             selected_quality = min(self.available_qualities, key=lambda q: base_qualities.index(q))
         elif quality == Quality.HALF:
             sorted_qualities = sorted(self.available_qualities, key=lambda q: base_qualities.index(q))
             middle_index = len(sorted_qualities) // 2
             selected_quality = sorted_qualities[middle_index]
 
         return self.quality_url_map.get(selected_quality)
 
-    def get_segments(self, quality):
-
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
-
-    @classmethod
-    def fix_quality(cls, quality):
-        # Needed for Porn Fetch
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
+    def get_segments(self, quality) -> list:
+        """
+        :param quality: (str, Quality) The video quality
+        :return: (list) A list of segments (the .ts files)
+        """
+        quality = Core().fix_quality(quality)
+        segments = Core().get_segments(quality=quality, m3u8_base_url=self.m3u8_base_url)
+        return segments
 
-    def download(self, downloader, quality, output_path, callback=None):
+    def download(self, downloader, quality, path, callback=None):
         """
         :param callback:
         :param downloader:
         :param quality:
-        :param output_path:
+        :param path:
         :return:
         """
-        quality = self.fix_quality(quality)
-
-        if callback is None:
-            callback = Callback.text_progress_bar
-
-        if downloader == default or str(downloader) == "default":
-            default(video=self, quality=quality, path=output_path, callback=callback)
-
-        elif downloader == threaded or str(downloader) == "threaded":
-            threaded(video=self, quality=quality, path=output_path, callback=callback)
-
-        elif downloader == FFMPEG or str(downloader) == "FFMPEG":
-            FFMPEG(video=self, quality=quality, path=output_path, callback=callback)
+        quality = Core().fix_quality(quality)
+        try:
+            Core().download(video=self, quality=quality, path=path, callback=callback, downloader=downloader)
+
+        except AttributeError:
+            logging.warning("Video doesn't have an HLS stream. Using legacy downloading instead...")
+            legacy_download(stream=True, path=path, callback=callback, url=self.cdn_url)
 
     @cached_property
     def m3u8_base_url(self) -> str:
         return REGEX_VIDEO_M3U8.search(self.script_content).group(1)
 
     @cached_property
     def title(self) -> str:
@@ -216,23 +184,23 @@
         return html.unescape(self.json_data["description"])
 
     @cached_property
     def thumbnail_url(self) -> str:
         return html.unescape(self.json_data["thumbnailUrl"])[0]
 
     @cached_property
-    def upload_date(self) -> str:
+    def publish_date(self) -> str:
         return html.unescape(self.json_data["uploadDate"])
 
     @cached_property
     def content_url(self) -> str:
         return html.unescape(self.json_data["contentUrl"])
 
     @cached_property
-    def keywords(self) -> list:
+    def tags(self) -> list:
         return REGEX_VIDEO_TAGS.findall(self.html_content)
 
     @cached_property
     def views(self) -> str:
         return REGEX_VIDEO_VIEWS.search(self.html_content).group(1)
 
     @cached_property
@@ -248,30 +216,48 @@
         return REGEX_VIDEO_RATING_VOTES.search(self.html_content).group(1)
 
     @cached_property
     def comment_count(self) -> str:
         return REGEX_VIDEO_COMMENT_COUNT.search(self.html_content).group(1)
 
     @cached_property
-    def uploader(self) -> str:
-        return REGEX_VIDEO_UPLOADER.search(self.html_content).group(1)
+    def author(self) -> str:
+        try:
+            uploader = REGEX_VIDEO_UPLOADER.search(self.html_content).group(1)
+
+        except AttributeError:
+            uploader = "Unknown"
+
+        return uploader
 
     @cached_property
     def length(self) -> str:
         return REGEX_VIDEO_LENGTH.search(self.html_content).group(1)
 
     @cached_property
     def pornstars(self) -> list:
         return REGEX_VIDEO_PORNSTARS.findall(self.html_content)
 
+    @cached_property
+    def embed_url(self) -> str:
+        return REGEX_IFRAME.search(html.unescape(self.html_content)).group(1)
+
+    @cached_property
+    def cdn_url(self) -> str:
+        return self.json_data["contentUrl"]
+
 
 class Client:
 
     @classmethod
     def get_video(cls, url):
+        """
+        :param url: (str) The video URL
+        :return: (Video) The video object
+        """
         return Video(url)
 
     @classmethod
     def extract_video_urls(cls, html_content):
         # Parse the HTML content with BeautifulSoup
         soup = BeautifulSoup(html_content, 'lxml')
         video_urls = []
@@ -290,18 +276,18 @@
     @classmethod
     def search(cls, query, sorting_Sort: Sort = Sort.Sort_relevance, sorting_Date: SortDate = SortDate.Sort_all,
                sorting_Time: SortVideoTime = SortVideoTime.Sort_all, sort_Quality: SortQuality = SortQuality.Sort_all,
                pages=2):
 
         query = query.replace(" ", "+")
 
-        url = f"https://www.xvideos.com/?k={query}&sort={sorting_Sort}%&datef={sorting_Date}&durf={sorting_Time}&quality={sort_Quality}"
+        base_url = f"https://www.xvideos.com/?k={query}&sort={sorting_Sort}%&datef={sorting_Date}&durf={sorting_Time}&quality={sort_Quality}"
         urls = []
         for page in range(pages):
-            response = requests.get(f"{url}&p={page}").content.decode("utf-8")
+            response = Core().get_content(f"{base_url}&p={page}", headers=headers).decode("utf-8")
             urls_ = Client.extract_video_urls(response)
 
             for url in urls_:
                 url = f"https://www.xvideos.com{url}"
 
                 if REGEX_VIDEO_CHECK_URL.match(url):
                     urls.append(url)
```

### Comparing `xvideos_api-1.1/xvideos_api.egg-info/PKG-INFO` & `xvideos_api-1.2/xvideos_api.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 Metadata-Version: 2.1
 Name: xvideos_api
-Version: 1.1
+Version: 1.2
 Summary: A Python API for the Porn Site xvideos.com
 Home-page: https://github.com/EchterAlsFake/xvideos_api
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
 Requires-Dist: ffmpeg-progress-yield
+Requires-Dist: eaf_base_api
 
 <h1 align="center">XVIDEOS API</h1> 
 
 <div align="center">
     <a href="https://pepy.tech/project/xvideos_api"><img src="https://static.pepy.tech/badge/xvideos_api" alt="Downloads"></a>
     <a href="https://github.com/EchterAlsFake/xvideos_api/workflows/"><img src="https://github.com/EchterAlsFake/xvideos_api/workflows/CodeQL/badge.svg" alt="CodeQL Analysis"/></a>
     <a href="https://github.com/EchterAlsFake/xvideos_api/workflows/"><img src="https://github.com/EchterAlsFake/xvideos_api/actions/workflows/tests.yml/badge.svg" alt="API Tests"/></a>
 </div>
 
 # Description
- 
-xvideos API is an API for xvideos.com. It allows you to fetch information from videos using regexes and requests.
+XVideos API is an API for xvideos.com. It allows you to fetch information from videos using regexes and requests.
 
 # Disclaimer
-
-[!IMPORTANT] The xvideos API is in violation to xvideos's ToS!
-
-Copyright Information: I have no intention of stealing copyright protected content or slowing down
-a website. Contact me at my E-Mail, and I'll take this Repository immediately offline.
-
+> [!IMPORTANT] 
+> XVideos API is in violation to the ToS of xvideos.com!
+> If you are the website owner of xvideos.com, contact me at my E-Mail, and I'll take this repository immediately offline.
 > EchterAlsFake@proton.me
 
 # Quickstart
 
 ### Have a look at the [Documentation](https://github.com/EchterAlsFake/xvideos_api/blob/master/README/Documentation.md) for more details
 
 - Install the library with `pip install xvideos_api`
 
 
 ```python
-from xvideos_api.xvideos_api import Client, Quality, threaded
+from xvideos_api.xvideos_api import Client, Quality
+from base_api.modules.download import threaded, default, FFMPEG
 # Initialize a Client object
 client = Client()
 
 # Fetch a video
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
 See [Changelog](https://github.com/EchterAlsFake/xvideos_api/blob/master/README/Changelog.md) for more details.
 
@@ -70,13 +68,7 @@
 
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
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: xvideos_api Version: 1.1 Summary: A Python API for
+Metadata-Version: 2.1 Name: xvideos_api Version: 1.2 Summary: A Python API for
 the Porn Site xvideos.com Home-page: https://github.com/EchterAlsFake/
 xvideos_api Author: Johannes Habel Author-email: EchterAlsFake@proton.me
 License: LGPLv3 Classifier: License :: OSI Approved :: GNU Lesser General
 Public License v3 (LGPLv3) Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: bs4 Requires-Dist: lxml Requires-Dist: ffmpeg-progress-
-yield
+yield Requires-Dist: eaf_base_api
                            ************ XXVVIIDDEEOOSS AAPPII ************
                     _[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_Q_L_ _A_n_a_l_y_s_i_s_]_[_A_P_I_ _T_e_s_t_s_]
-# Description xvideos API is an API for xvideos.com. It allows you to fetch
-information from videos using regexes and requests. # Disclaimer [!IMPORTANT]
-The xvideos API is in violation to xvideos's ToS! Copyright Information: I have
-no intention of stealing copyright protected content or slowing down a website.
-Contact me at my E-Mail, and I'll take this Repository immediately offline. >
-EchterAlsFake@proton.me # Quickstart ### Have a look at the [Documentation]
-(https://github.com/EchterAlsFake/xvideos_api/blob/master/README/
-Documentation.md) for more details - Install the library with `pip install
-xvideos_api` ```python from xvideos_api.xvideos_api import Client, Quality,
-threaded # Initialize a Client object client = Client() # Fetch a video
-video_object = client.get_video("") # Information from Video objects print
-(video_object.title) print(video_object.likes) # Download the video
-video_object.download(downloader=threaded, quality=Quality.BEST,
-output_path="your_output_path + filename") # SEE DOCUMENTATION FOR MORE ``` #
-Changelog See [Changelog](https://github.com/EchterAlsFake/xvideos_api/blob/
-master/README/Changelog.md) for more details. # Contribution Do you see any
-issues or having some feature requests? Simply open an Issue or talk in the
-discussions. Pull requests are also welcome. # License Licensed under the
-LGPLv3 License Copyright (C) 2023â2024 Johannes Habel # Support Leave a star
-on the repository. That's enough :)
+# Description XVideos API is an API for xvideos.com. It allows you to fetch
+information from videos using regexes and requests. # Disclaimer > [!IMPORTANT]
+> XVideos API is in violation to the ToS of xvideos.com! > If you are the
+website owner of xvideos.com, contact me at my E-Mail, and I'll take this
+repository immediately offline. > EchterAlsFake@proton.me # Quickstart ### Have
+a look at the [Documentation](https://github.com/EchterAlsFake/xvideos_api/
+blob/master/README/Documentation.md) for more details - Install the library
+with `pip install xvideos_api` ```python from xvideos_api.xvideos_api import
+Client, Quality from base_api.modules.download import threaded, default, FFMPEG
+# Initialize a Client object client = Client() # Fetch a video video_object =
+client.get_video("") # Information from Video objects print(video_object.title)
+print(video_object.likes) # Download the video video_object.download
+(downloader=threaded, quality=Quality.BEST, path="your_output_path + filename")
+# SEE DOCUMENTATION FOR MORE ``` # Changelog See [Changelog](https://
+github.com/EchterAlsFake/xvideos_api/blob/master/README/Changelog.md) for more
+details. # Contribution Do you see any issues or having some feature requests?
+Simply open an Issue or talk in the discussions. Pull requests are also
+welcome. # License Licensed under the LGPLv3 License Copyright (C) 2023â2024
+Johannes Habel
```

