# Comparing `tmp/pyutube-1.1.7.tar.gz` & `tmp/pyutube-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutube-1.1.7.tar", last modified: Thu Mar 28 14:14:59 2024, max compression
+gzip compressed data, was "pyutube-1.1.8.tar", last modified: Tue Apr  2 18:32:14 2024, max compression
```

## Comparing `pyutube-1.1.7.tar` & `pyutube-1.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-03-28 14:14:59.866584 pyutube-1.1.7/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1078 2024-03-05 00:46:11.000000 pyutube-1.1.7/LICENSE.md
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     5362 2024-03-28 14:14:59.865184 pyutube-1.1.7/PKG-INFO
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     4932 2024-03-28 13:55:45.000000 pyutube-1.1.7/README.md
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-03-28 14:14:59.850079 pyutube-1.1.7/pyutube/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       21 2024-03-23 02:52:27.000000 pyutube-1.1.7/pyutube/__init__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       36 2024-03-23 02:53:08.000000 pyutube-1.1.7/pyutube/__main__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     3392 2024-03-28 14:13:55.000000 pyutube-1.1.7/pyutube/cli.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    12542 2024-03-28 04:52:30.000000 pyutube-1.1.7/pyutube/downloader.py
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-03-28 14:14:59.863091 pyutube-1.1.7/pyutube/tests/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       30 2024-02-14 23:03:00.000000 pyutube-1.1.7/pyutube/tests/__init__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1273 2024-03-12 00:06:32.000000 pyutube-1.1.7/pyutube/tests/test_is_youtube_link.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     3298 2024-03-12 00:06:32.000000 pyutube-1.1.7/pyutube/tests/test_is_youtube_video.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     9764 2024-03-28 14:12:36.000000 pyutube-1.1.7/pyutube/utils.py
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-03-28 14:14:59.864264 pyutube-1.1.7/pyutube.egg-info/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     5362 2024-03-28 14:14:59.000000 pyutube-1.1.7/pyutube.egg-info/PKG-INFO
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      414 2024-03-28 14:14:59.000000 pyutube-1.1.7/pyutube.egg-info/SOURCES.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        1 2024-03-28 14:14:59.000000 pyutube-1.1.7/pyutube.egg-info/dependency_links.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       44 2024-03-28 14:14:59.000000 pyutube-1.1.7/pyutube.egg-info/entry_points.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       62 2024-03-28 14:14:59.000000 pyutube-1.1.7/pyutube.egg-info/requires.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        8 2024-03-28 14:14:59.000000 pyutube-1.1.7/pyutube.egg-info/top_level.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       38 2024-03-28 14:14:59.867579 pyutube-1.1.7/setup.cfg
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1160 2024-03-28 14:14:37.000000 pyutube-1.1.7/setup.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-02 18:32:14.782551 pyutube-1.1.8/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1078 2024-03-05 00:46:11.000000 pyutube-1.1.8/LICENSE.md
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6854 2024-04-02 18:32:14.781430 pyutube-1.1.8/PKG-INFO
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6027 2024-04-02 18:27:42.000000 pyutube-1.1.8/README.md
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-02 18:32:14.767544 pyutube-1.1.8/pyutube/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      397 2024-04-02 18:18:47.000000 pyutube-1.1.8/pyutube/__init__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      184 2024-03-31 03:14:16.000000 pyutube-1.1.8/pyutube/__main__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     5451 2024-04-02 18:28:48.000000 pyutube-1.1.8/pyutube/cli.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    13979 2024-04-02 18:28:32.000000 pyutube-1.1.8/pyutube/downloader.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-02 18:32:14.778849 pyutube-1.1.8/pyutube/tests/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       30 2024-02-14 23:03:00.000000 pyutube-1.1.8/pyutube/tests/__init__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1273 2024-03-12 00:06:32.000000 pyutube-1.1.8/pyutube/tests/test_is_youtube_link.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     3298 2024-03-12 00:06:32.000000 pyutube-1.1.8/pyutube/tests/test_is_youtube_video.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     9449 2024-04-02 18:28:23.000000 pyutube-1.1.8/pyutube/utils.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-02 18:32:14.780244 pyutube-1.1.8/pyutube.egg-info/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6854 2024-04-02 18:32:14.000000 pyutube-1.1.8/pyutube.egg-info/PKG-INFO
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      414 2024-04-02 18:32:14.000000 pyutube-1.1.8/pyutube.egg-info/SOURCES.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        1 2024-04-02 18:32:14.000000 pyutube-1.1.8/pyutube.egg-info/dependency_links.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       44 2024-04-02 18:32:14.000000 pyutube-1.1.8/pyutube.egg-info/entry_points.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       76 2024-04-02 18:32:14.000000 pyutube-1.1.8/pyutube.egg-info/requires.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        8 2024-04-02 18:32:14.000000 pyutube-1.1.8/pyutube.egg-info/top_level.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       38 2024-04-02 18:32:14.782726 pyutube-1.1.8/setup.cfg
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1398 2024-04-02 18:14:54.000000 pyutube-1.1.8/setup.py
```

### Comparing `pyutube-1.1.7/LICENSE.md` & `pyutube-1.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyutube-1.1.7/PKG-INFO` & `pyutube-1.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: pyutube
-Version: 1.1.7
-Project-URL: Homepage, https://github.com/Hetari/pyutube
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: pytube
-Requires-Dist: inquirer
-Requires-Dist: yaspin
-Requires-Dist: typer
-Requires-Dist: requests
-Requires-Dist: rich
-Requires-Dist: inquirer
-Requires-Dist: termcolor
-
 # YouTube Downloader CLI
 
 Enjoying my project? Please show your appreciation by starring it on GitHub! ⭐
 
 ## Description
 
 This command-line tool downloads YouTube videos from the `Terminal`, written under [Pytube](https://pytube.io/).
@@ -30,49 +13,49 @@
 ## Inspiration
 
 This project was inspired by [Utube](https://github.com/omer73364/uTube/) by [omer73364](https://github.com/omer73364) 🤩
 
 ## Features
 
 - User-friendly CLI interface.
-- Download a single YouTube in video format or audio.
+- Download a single YouTube video format or audio.
 - Download YouTube shorts.
 - Download YouTube playlists.
 
 ## TODO
 
 - [x] Publish on PyPI.
 - [x] Support downloading sounds (mp3 format).
 - [x] Supports all available video resolutions.
 - [x] Support shorts.
 - [x] Supports downloading playlists.
-- [ ] Playlists organized into folders by their names.
+- [ ] Playlists are organized into folders by their names.
 - [ ] GUI app (not yet).
-- [ ] Any features that you/I can think of.
+- [ ] Are there any features that you/I can think of?
 
 ## Upgrade
 
 All the latest updates will be posted on [GitHub](https://github.com/Hetari/pyutube), you can also upgrade the tool via [PyPI](https://pypi.org/project/pyutube/) with this command:
 
 ```bash
 pip install --upgrade pyutube
 ```
 
 ## Installation
 
-Make suer that you have [Python](https://www.python.org) installed. To check if you have it installed, type `python --version` in your terminal. You should see something like `Python 3.x.x`.
+Make sure that you have [Python](https://www.python.org) installed. To check if you have it installed, type `python --version` in your terminal. You should see something like `Python 3. x `
 
 ### Method 1: Using Pip
 
 ```bash
 pip install --upgrade pip
 pip install pyutube
 ```
 
-### Method 2: Building the project from source
+### Method 2: Building the project from the source
 
 Clone the repository:
 
 ```bash
 git clone https://github.com/Hetari/pyutube.git
 ```
 
@@ -135,48 +118,88 @@
 
 ### **- Show version:**
 
 ```bash
 pyutube -v
 ```
 
+### **- Download playlists:**
+
+1. `pyutube <YOUTUBE_PLAYLIST_LINK | PLAYLIST_ID> [the_download_path*]`
+
+   > Don't forget, the path is optional.
+
+2. Then choose the format of the download, video or audio.
+3. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it all immediately 🔥.
+   > It will check all resolutions available in the first video in the playlist, then it will download all of them in the same resolution 👍.
+
 ### **- Download shorts, videos, or audio:**
 
 1. `pyutube <YOUTUBE_LINK | VIDEO_ID | SHORT_LINK> [the_download_path*]`
 
    > Don't forget, the path is optional.
 
 2. Then choose the format of the download, video or audio.
-3. Choose the resolution if it is a video you want to download, otherwise choose audio and it will download it immediately 🔥.
+3. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it immediately 🔥.
 
-### **- Download audios immediately:**
+```bash
+pyutube cMPnY7EuZvo
+pyutube youtu.be/cMPnY7EuZvo
+pyutube https://youtube.com/watch?v=cMPnY7EuZvo
+```
+
+### **- Download audio immediately:**
 
 1. `pyutube <YOUTUBE_LINK | VIDEO_ID | SHORT_LINK> [the_download_path*] -a`
 
+```bash
+pyutube cMPnY7EuZvo -a
+```
+
+or
+
+```bash
+pyutube -a youtu.be/cMPnY7EuZvo
+```
+
 and that's it 🎉.
 
 ### **- Download videos immediately:**
 
 1. `pyutube <YOUTUBE_LINK | VIDEO_ID | SHORT_LINK> [the_download_path*] -f`
 2. Choose the resolution.
 
+```bash
+pyutube cMPnY7EuZvo -f
+```
+
+or
+
+```bash
+pyutube -f youtu.be/cMPnY7EuZvo
+```
+
 see the video and relax 🎉.
 
 <div style="text-align: center;">
-    <img src="pyutube/images/image1.png" />
-    <br />
-    <br />
-    <img src="pyutube/images/image2.png" />
-    <br />
-    <br />
-    <img src="pyutube/images/image3.png" />
-    <br />
-    <br />
-    <img src="pyutube/images/image4.png" />
-
+   <a href="https://ibb.co/LhT6r3r">
+      <img src="https://i.ibb.co/WprF0L0/image5.png" alt="image5">
+   </a>
+   <a href="https://ibb.co/7ymCS79">
+      <img src="https://i.ibb.co/h8z9gpq/image4.png" alt="image4">
+   </a>
+   <a href="https://ibb.co/9sVDxbh">
+      <img src="https://i.ibb.co/pJR7HfQ/image3.png" alt="image3">
+   </a>
+   <a href="https://ibb.co/Kb6qjmg">
+      <img src="https://i.ibb.co/sbjwvt4/image2.png" alt="image2">
+   </a>
+   <a href="https://ibb.co/0JkdkQy">
+      <img src="https://i.ibb.co/7yH6Hbt/image1.png" alt="image1">
+   </a>
 </div>
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you want to change.
 please follow the [contributing guidelines](https://github.com/Hetari/pyutube/blob/main/CONTRIBUTING.md)
```

### Comparing `pyutube-1.1.7/pyutube/downloader.py` & `pyutube-1.1.8/pyutube/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,68 @@
+"""
+This module contains the Downloader class which provides functionality 
+for downloading videos from YouTube.
+"""
+import os
+import subprocess
+import sys
+
+
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 from pytube import YouTube, Playlist
 from pytube.cli import on_progress
 from termcolor import colored
 import ffmpeg
 
-import os
-import subprocess
-
 from .utils import (
-    clear,
     console,
     error_console,
     sanitize_filename,
     ask_rename_file,
     ask_resolution,
     rename_file,
     is_file_exists,
 )
 
 
 class Downloader:
-    def __init__(self, url: str, path: str, quality: None = None, is_audio: bool = False, is_playlist: bool = False, is_short: bool = False):
+    """
+    This class provides functionality for downloading videos from YouTube.
+    """
+
+    def __init__(
+            self,
+            url: str,
+            path: str,
+            quality: None = None,
+            is_audio: bool = False,
+            is_playlist: bool = False,
+    ):
+        """
+            Initializes a Downloader object.
+
+            Args:
+                url: The URL of the video or playlist to download.
+                path: The path where the downloaded file(s) will be saved.
+                quality: The desired quality of the video, default is None.
+                is_audio: Flag indicating if the video should be downloaded 
+                    as audio, default is False.
+                is_playlist: Flag indicating if the URL is for a playlist, default is False.
+        """
         self.url = url
         self.path = path
         self.quality = quality
         self.is_audio = is_audio
         self.is_playlist = is_playlist
-        self.is_short = is_short
 
-    @yaspin(text=colored("Searching for the video", "green"), color="green", spinner=Spinners.point)
+    @yaspin(
+        text=colored("Searching for the video", "green"),
+        color="green", spinner=Spinners.point
+    )
     def video_search(self, url: str) -> YouTube:
         """
         This function searches for a video using the provided URL and returns an
         instance of the YouTube class representing the searched video.
 
         Args:
             url: The URL of the video to search for.
@@ -45,15 +74,19 @@
         return YouTube(
             url,
             use_oauth=False,
             allow_oauth_cache=True,
             on_progress_callback=on_progress,
         )
 
-    @yaspin(text=colored("getting video headers ", "green") + colored("(means the video won't be fully downloaded)", "yellow"), spinner=Spinners.point)
+    @yaspin(
+        text=colored("getting video headers ", "green") +
+        colored("(means the video won't be fully downloaded)", "yellow"),
+        spinner=Spinners.point
+    )
     def get_available_resolutions(self, video: YouTube) -> set:
         """
         Get a set of all available resolutions for the video.
 
         Args:
             video: The video to retrieve available resolutions from.
 
@@ -80,43 +113,54 @@
         # Separate resolutions and sizes without using two loops
         resolutions, sizes = zip(*resolutions_with_sizes)
         resolutions = list(resolutions)
         sizes = list(sizes)
 
         return resolutions, sizes, available_streams, audio_stream
 
-    @yaspin(text=colored("Downloading the video...", "green"), color="green", spinner=Spinners.dots13)
+    @yaspin(
+        text=colored("Downloading the video...", "green"),
+        color="green", spinner=Spinners.dots13
+    )
     def get_video_streams(self, quality: str, streams: YouTube.streams) -> YouTube:
         """
         Downloads the video streams based on the specified quality.
         If the specified quality is not available, it selects the nearest quality.
 
         Args:
             video: The video to retrieve streams from.
             quality: The desired quality of the video streams.
 
         Returns:
-            The video stream with the specified quality, or the best available stream if no match is found.
+            The video stream with the specified quality, 
+            or the best available stream if no match is found.
         """
         return streams.filter(res=quality).first()
 
-    @yaspin(text=colored("Downloading the audio...", "green"), color="green", spinner=Spinners.dots13)
+    @yaspin(
+        text=colored("Downloading the audio...", "green"),
+        color="green",
+        spinner=Spinners.dots13
+    )
     def get_audio_streams(self, video: YouTube) -> YouTube:
         """
         Function to get audio streams from a video.
 
         Args:
             video: The video for which audio streams are to be obtained.
 
         Returns:
             The first audio stream found in the video.
         """
         return video.streams.filter(only_audio=True).order_by('mime_type').first()
 
-    @yaspin(text=colored("Saving the file...", "cyan"), spinner=Spinners.smiley)
+    @yaspin(
+        text=colored("Saving the file...", "cyan"),
+        spinner=Spinners.smiley
+    )
     def save_file(self, video: YouTube, path: str, filename: str) -> None:
         """
         Save the file to the specified path with the given filename.
 
         Args:
             video: The video to be saved.
             path: The path where the video will be saved.
@@ -125,14 +169,20 @@
         Returns:
             None
         """
         video.download(output_path=path, filename=filename)
 
     # Helper functions for the Downloader class
     def search_process(self) -> YouTube:
+        """
+        Performs the video search process.
+
+        Returns:
+            YouTube: An instance of the YouTube class representing the searched video.
+        """
         try:
             video = self.video_search(self.url)
         except Exception as error:
             error_console.print(f"Error: {error}")
             return False
 
         # If video is not found
@@ -163,15 +213,17 @@
         Generate a filename for the downloaded video.
 
         Returns:
             str: The generated filename.
         """
         quality = 'audio' if self.is_audio else video.resolution
         title = sanitize_filename(video.title)
-        return f"{title} - {quality}_-_{video_id}.{'mp3' if self.is_audio else video.mime_type.split('/')[1]}"
+        extension = 'mp3' if self.is_audio else video.mime_type.split('/')[1]
+
+        return f"{title} - {quality}_-_{video_id}.{extension}"
 
     def handle_existing_file(self, filename):
         """
         Handle the case where a file with the same name already exists.
 
         Returns:
             str: The user's choice.
@@ -179,15 +231,15 @@
         choice = ask_rename_file(filename).lower()
         if choice.startswith('rename'):
             filename = self.prompt_new_filename(filename)
             if not filename:
                 error_console.print("Invalid filename")
                 return False
             return filename
-        elif choice.startswith('cancel'):
+        if choice.startswith('cancel'):
             console.print("Download canceled", style="info")
             return False
         return True
 
     def prompt_new_filename(self, filename):
         """
         Prompt the user for a new filename.
@@ -195,47 +247,63 @@
         Returns:
             str: The new filename.
         """
         text = colored(filename, 'yellow')
         new_name = input(f"Rename {text} to: ")
         return rename_file(filename, new_name)
 
-    def merging(self, video_name: str, audio_name: str, video_id: str):
+    def merging(self, video_name: str, audio_name: str):
+        """
+        Merges the video and audio files into a single file.
+
+        Args:
+            video_name: The name of the video file.
+            audio_name: The name of the audio file.
+            video_id: The ID of the video.
+
+        Returns:
+            None
+        """
+
         output_directory = "output"
         os.makedirs(output_directory, exist_ok=True)
 
         # Merge video and audio using ffmpeg-python
         input_video = ffmpeg.input(video_name)
         input_audio = ffmpeg.input(audio_name)
 
         # Build FFmpeg command string
         ffmpeg_command = ffmpeg.output(
             ffmpeg.concat(input_video, input_audio, v=1, a=1),
             f'{output_directory}/{video_name}').compile()
 
+        # Error: module 'ffmpeg' has no attribute 'input'
         # Run FFmpeg command using subprocess
         try:
             subprocess.run(ffmpeg_command, stdout=subprocess.PIPE,
                            stderr=subprocess.PIPE, check=True)
         except subprocess.CalledProcessError as e:
-            print('An error occurred:', e.stderr)
+            error_console.print('An error occurred:', e.stderr)
         else:
             os.remove(video_name)
             os.remove(audio_name)
 
             output_file = os.path.join(output_directory, video_name)
 
             if os.path.exists(output_file):
                 os.replace(output_file, os.path.join(os.getcwd(), video_name))
                 os.rmdir(output_directory)
             else:
                 print("Merged video file not found in the output directory.")
 
     @staticmethod
-    def get_video_resolutions_sizes(available_streams: list[YouTube], audio_stream: YouTube) -> list:
+    def get_video_resolutions_sizes(
+            available_streams: list[YouTube],
+            audio_stream: YouTube
+    ) -> list:
         """
         Get the available video resolutions.
 
         Args:
             available_streams: The available video streams.
             audio_stream: The audio stream.
 
@@ -244,17 +312,14 @@
         """
         if not available_streams:
             return []
 
         # Calculate the total audio file size in bytes
         audio_filesize_bytes = audio_stream.filesize_approx
 
-        # Convert the audio file size to KB
-        audio_filesize_kb = audio_filesize_bytes / 1000
-
         resolutions_with_sizes = []
         for stream in available_streams:
             if stream.resolution:
                 # Calculate the total video file size including audio in bytes
                 video_filesize_bytes = stream.filesize_approx + \
                     (2 * audio_filesize_bytes)
                 # Convert the video file size to KB or MB dynamically
@@ -266,15 +331,15 @@
                     video_filesize = f"{video_filesize_bytes / 1024:.2f} KB"
 
                 resolutions_with_sizes.append(
                     (stream.resolution, video_filesize))
 
         return resolutions_with_sizes
 
-    def download_video(self):
+    def download_video(self) -> bool:
         """
         Download a video from a given URL to a specified path.
 
         Args:
             url: The URL of the video.
             path: The path to save the downloaded video.
             quality: The quality of the video, default is '720p'.
@@ -282,56 +347,58 @@
 
         Returns:
             bool: True if the video is downloaded successfully, False otherwise.
         """
         video = self.search_process()
 
         if not video:
-            return False
+            error_console.print("❗ The video could not be found.")
+            sys.exit()
 
         video_id = video.video_id
 
         if self.is_audio:
             footage = self.get_audio_streams(video)
 
         else:
             # shorts and videos
             streams, video_audio = self.get_selected_stream(video)
 
             if not streams:
                 error_console.print("❗ Cancel the download...")
-                return
+                sys.exit()
+
             footage = self.get_video_streams(self.quality, streams)
 
             # Generate filename with title, quality, and file extension
             self.is_audio = True
             audio_filename = self.generate_filename(video_audio, video_id)
             self.is_audio = False
 
         if not footage:
             error_console.print(
                 "Something went wrong while downloading the video.")
-            return False
+            sys.exit()
 
         video_filename = self.generate_filename(footage, video_id)
 
         # If file with the same name already exists in the path
         if is_file_exists(self.path, video_filename):
             video_filename = self.handle_existing_file(video_filename)
             if not video_filename:
-                return False
+                sys.exit()
         try:
             self.save_file(footage, self.path, video_filename)
             if not self.is_audio:
                 self.save_file(video_audio, self.path, audio_filename)
-                self.merging(video_filename, audio_filename, video_id)
+                self.merging(video_filename, audio_filename)
 
         except Exception as error:
             error_console.print(f"Error: {error}")
-            return False
+            sys.exit()
 
         console.print("✅ Download completed", style="info")
         return True
 
     def get_playlist_links(self):
         """
         Get the playlist links from the URL.
@@ -341,15 +408,21 @@
 
         Returns:
             list: A list of playlist links.
         """
         return Playlist(self.url)
 
 
-def download(url: str, path: str, is_audio: bool, is_playlist: bool = False, quality_choice: str = None) -> None:
+def download(
+    url: str,
+    path: str,
+    is_audio: bool,
+    is_playlist: bool = False,
+    quality_choice: str = None
+) -> None:
     """
     Downloads the YouTube video based on the provided parameters.
 
     Args:
         url (str): The URL of the YouTube video.
         path (str): The path to save the video.
         quality_choice (str): The chosen quality for the video.
@@ -359,13 +432,12 @@
         None
     """
     downloader = Downloader(
         url=url, path=path, quality=quality_choice, is_audio=is_audio, is_playlist=is_playlist
     )
 
     if is_playlist:
-
         return downloader.get_playlist_links()
-    else:
-        downloader.download_video()
+
+    downloader.download_video()
 
     return downloader.quality
```

### Comparing `pyutube-1.1.7/pyutube/tests/test_is_youtube_link.py` & `pyutube-1.1.8/pyutube/tests/test_is_youtube_link.py`

 * *Files identical despite different names*

### Comparing `pyutube-1.1.7/pyutube/tests/test_is_youtube_video.py` & `pyutube-1.1.8/pyutube/tests/test_is_youtube_video.py`

 * *Files identical despite different names*

### Comparing `pyutube-1.1.7/pyutube/utils.py` & `pyutube-1.1.8/pyutube/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+"""
+This module contains the utils functions for the pyutube package.
+"""
+
+import sys
+import re
+import os
+
 import inquirer
 import requests
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 from rich.console import Console
 from rich.theme import Theme
 
-import re
-import os
-
 
-__version__ = "1.1.7"
+__version__ = "1.1.8"
 ABORTED_PREFIX = "aborted"
 CANCEL_PREFIX = "cancel"
 
 # Set up the console
 custom_theme = Theme({
     "info": "#64b0f2",
     "warning": "color(3)",
@@ -41,32 +46,23 @@
         # For Unix/Linux/MacOS
         os.system("clear")
 
 
 @yaspin(text="Checking internet connection", color="blue", spinner=Spinners.earth)
 def is_internet_available() -> bool:
     """
-    Checks if internet connection is available by making a simple request to http://www.google.com with a timeout of 5 seconds.
+    Checks if internet connection is available by making a simple request
+    to http://www.google.com with a timeout of 5 seconds.
 
     Returns:
         bool: the request status (True if available, False if not).
     """
     try:
         requests.get("https://www.google.com", timeout=5)
         return True
-    except requests.ConnectionError:
-        return False
-    except requests.ReadTimeout:
-        return False
-    except requests.HTTPError:
-        return False
-    except requests.TooManyRedirects:
-        return False
-    except requests.RequestException:
-        return False
     except Exception as error:
         error_console.print(f"Error: {error}")
         return False
 
 
 def is_youtube_link(link: str) -> tuple[bool, str]:
     """
@@ -80,15 +76,18 @@
         False otherwise. The second item of the tuple indicates the type of link found:
         'video', 'playlist', or 'shorts'.
     """
     is_video = is_youtube_video(link)
     is_short = is_youtube_shorts(link)
     is_playlist = is_youtube_playlist(link)
 
-    return (is_video, "video") if is_video else (is_short, "short") if is_short else (True, "playlist") if is_playlist else (False, "unknown")
+    return (is_video, "video") if is_video \
+        else (is_short, "short") if is_short \
+        else (True, "playlist") if is_playlist\
+        else (False, "unknown")
 
 
 def is_youtube_shorts(link: str) -> bool:
     """
     Check if the given link is a YouTube shorts link.
 
     Args:
@@ -109,17 +108,14 @@
 
     Args:
         link: The link to be checked.
 
     Returns:
         bool: True if the link is a YouTube video, False otherwise.
     """
-    # video_pattern = re.compile(
-    #     r'(?:https?://)?(?:www\.)?(?:youtube\.com/(?:(?:watch\?v=)|(?:embed/))|youtu\.be/)([a-zA-Z0-9_-]{11})')
-
     video_pattern = re.compile(
         r'(?:https?://)?(?:www\.)?(?:youtube\.com/(?:(?:watch\?v=)|(?:embed/))|youtu\.be/|youtube.com/share\?v=)([a-zA-Z0-9_-]{11})')
 
     return bool(video_pattern.match(link))
 
 
 def is_youtube_playlist(link: str) -> bool:
@@ -143,20 +139,23 @@
 
     Args:
         video_id: The string to be checked.
 
     Returns:
         bool: True if the string is a valid YouTube video ID, False otherwise.
     """
-    return len(video_id) == 11 and all(c in "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_-" for c in video_id)
+    return len(video_id) == 11 and all(
+        c in "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_-" for c in video_id
+    )
 
 
 def file_type() -> str:
     """
-    Prompts the user to choose a file type for download and returns the chosen file type as a string.
+    Prompts the user to choose a file type for download and returns 
+    the chosen file type as a string.
 
     Args:
         None
 
     Returns:
         str: The chosen file type as a string.
     """
@@ -170,26 +169,28 @@
     ]
 
     try:
         answer = inquirer.prompt(questions)["file_type"]
 
     # TypeError: 'NoneType' object is not subscriptable
 
-    except TypeError as error:
+    except TypeError:
         return ABORTED_PREFIX
 
     except Exception as error:
         error_console.print(f"Error: {error}")
+        sys.exit()
 
     return answer
 
 
 def ask_resolution(resolutions: set, sizes) -> str:
     """
-    Prompts the user to choose a resolution for download and returns the chosen resolution as a string.
+    Prompts the user to choose a resolution for download
+    and returns the chosen resolution as a string.
 
     Args:
         resolutions (set): The set of available resolutions.
 
     Returns:
         str: The chosen resolution as a string.
     """
@@ -208,19 +209,20 @@
             choices=resolution_choices,
         ),
     ]
 
     try:
         answer = inquirer.prompt(questions)["resolution"]
 
-    except TypeError as error:
+    except TypeError:
         return ABORTED_PREFIX
 
     except Exception as error:
         error_console.print(f"Error: {error}")
+        sys.exit()
 
      # Extract the resolution part from the user's choice
     return answer.split(" ~= ")[0]
 
 
 def ask_rename_file(filename: str) -> str:
     """
@@ -273,14 +275,15 @@
         str: The new filename after the renaming operation.
     """
     try:
         if not new_filename.endswith(os.path.splitext(filename)[1]):
             new_filename += f".{filename.split('.')[-1]}"
     except IndexError as error:
         error_console.print(f"Error: {error}")
+        sys.exit()
     return new_filename
 
 
 def is_file_exists(path: str, filename: str) -> bool:
     """
     Check if a file exists at the specified path and filename.
 
@@ -301,18 +304,18 @@
 
     Returns:
         bool: True if internet connection is available, False otherwise.
     """
     if not is_internet_available():
         error_console.print("❗ No internet connection")
         return False
-    else:
-        console.print("✅ There is internet connection", style="info")
-        console.print()
-        return True
+
+    console.print("✅ There is internet connection", style="info")
+    console.print()
+    return True
 
 
 def validate_link(url: str) -> tuple[bool, str]:
     """
     Validates the given YouTube video URL.
 
     Args:
@@ -325,28 +328,27 @@
     is_valid_link, link_type = is_youtube_link(url)
     if not is_valid_link:
         console.print("❌ Invalid link", style="danger")
 
     return is_valid_link, link_type.lower()
 
 
-def handle_video_link(url: str, path: str) -> None:
+def handle_video_link() -> bool:
     """
     Handles video link scenario.
 
     Args:
-        url (str): The URL of the YouTube video.
-        path (str): The path to save the video.
+        None
 
     Returns:
-        None
+        bool: True if the video link is valid, False otherwise.
     """
     file_type_choice = file_type().lower()
     is_audio = file_type_choice.startswith("audio")
 
     if file_type_choice.startswith(CANCEL_PREFIX):
         error_console.print("❗ Cancel the download...")
-        return
+        sys.exit()
     elif file_type_choice.startswith(ABORTED_PREFIX):
-        return
+        sys.exit()
 
     return is_audio
```

### Comparing `pyutube-1.1.7/pyutube.egg-info/PKG-INFO` & `pyutube-1.1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 Metadata-Version: 2.1
 Name: pyutube
-Version: 1.1.7
+Version: 1.1.8
+Summary: Awesome CLI to download YouTube videos (as video or audio)/shorts/playlists from the terminal
+Author: Ebraheem Alhetari
+Author-email: hetari4all@gmail.com
+License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube
+Keywords: youtube,download,cli,pyutube,pytube
+Platform: Windows
+Platform: MacOS
+Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pytube
 Requires-Dist: inquirer
 Requires-Dist: yaspin
 Requires-Dist: typer
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: inquirer
 Requires-Dist: termcolor
+Requires-Dist: ffmpeg-python
 
 # YouTube Downloader CLI
 
 Enjoying my project? Please show your appreciation by starring it on GitHub! ⭐
 
 ## Description
 
@@ -30,49 +41,49 @@
 ## Inspiration
 
 This project was inspired by [Utube](https://github.com/omer73364/uTube/) by [omer73364](https://github.com/omer73364) 🤩
 
 ## Features
 
 - User-friendly CLI interface.
-- Download a single YouTube in video format or audio.
+- Download a single YouTube video format or audio.
 - Download YouTube shorts.
 - Download YouTube playlists.
 
 ## TODO
 
 - [x] Publish on PyPI.
 - [x] Support downloading sounds (mp3 format).
 - [x] Supports all available video resolutions.
 - [x] Support shorts.
 - [x] Supports downloading playlists.
-- [ ] Playlists organized into folders by their names.
+- [ ] Playlists are organized into folders by their names.
 - [ ] GUI app (not yet).
-- [ ] Any features that you/I can think of.
+- [ ] Are there any features that you/I can think of?
 
 ## Upgrade
 
 All the latest updates will be posted on [GitHub](https://github.com/Hetari/pyutube), you can also upgrade the tool via [PyPI](https://pypi.org/project/pyutube/) with this command:
 
 ```bash
 pip install --upgrade pyutube
 ```
 
 ## Installation
 
-Make suer that you have [Python](https://www.python.org) installed. To check if you have it installed, type `python --version` in your terminal. You should see something like `Python 3.x.x`.
+Make sure that you have [Python](https://www.python.org) installed. To check if you have it installed, type `python --version` in your terminal. You should see something like `Python 3. x `
 
 ### Method 1: Using Pip
 
 ```bash
 pip install --upgrade pip
 pip install pyutube
 ```
 
-### Method 2: Building the project from source
+### Method 2: Building the project from the source
 
 Clone the repository:
 
 ```bash
 git clone https://github.com/Hetari/pyutube.git
 ```
 
@@ -135,48 +146,88 @@
 
 ### **- Show version:**
 
 ```bash
 pyutube -v
 ```
 
+### **- Download playlists:**
+
+1. `pyutube <YOUTUBE_PLAYLIST_LINK | PLAYLIST_ID> [the_download_path*]`
+
+   > Don't forget, the path is optional.
+
+2. Then choose the format of the download, video or audio.
+3. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it all immediately 🔥.
+   > It will check all resolutions available in the first video in the playlist, then it will download all of them in the same resolution 👍.
+
 ### **- Download shorts, videos, or audio:**
 
 1. `pyutube <YOUTUBE_LINK | VIDEO_ID | SHORT_LINK> [the_download_path*]`
 
    > Don't forget, the path is optional.
 
 2. Then choose the format of the download, video or audio.
-3. Choose the resolution if it is a video you want to download, otherwise choose audio and it will download it immediately 🔥.
+3. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it immediately 🔥.
 
-### **- Download audios immediately:**
+```bash
+pyutube cMPnY7EuZvo
+pyutube youtu.be/cMPnY7EuZvo
+pyutube https://youtube.com/watch?v=cMPnY7EuZvo
+```
+
+### **- Download audio immediately:**
 
 1. `pyutube <YOUTUBE_LINK | VIDEO_ID | SHORT_LINK> [the_download_path*] -a`
 
+```bash
+pyutube cMPnY7EuZvo -a
+```
+
+or
+
+```bash
+pyutube -a youtu.be/cMPnY7EuZvo
+```
+
 and that's it 🎉.
 
 ### **- Download videos immediately:**
 
 1. `pyutube <YOUTUBE_LINK | VIDEO_ID | SHORT_LINK> [the_download_path*] -f`
 2. Choose the resolution.
 
+```bash
+pyutube cMPnY7EuZvo -f
+```
+
+or
+
+```bash
+pyutube -f youtu.be/cMPnY7EuZvo
+```
+
 see the video and relax 🎉.
 
 <div style="text-align: center;">
-    <img src="pyutube/images/image1.png" />
-    <br />
-    <br />
-    <img src="pyutube/images/image2.png" />
-    <br />
-    <br />
-    <img src="pyutube/images/image3.png" />
-    <br />
-    <br />
-    <img src="pyutube/images/image4.png" />
-
+   <a href="https://ibb.co/LhT6r3r">
+      <img src="https://i.ibb.co/WprF0L0/image5.png" alt="image5">
+   </a>
+   <a href="https://ibb.co/7ymCS79">
+      <img src="https://i.ibb.co/h8z9gpq/image4.png" alt="image4">
+   </a>
+   <a href="https://ibb.co/9sVDxbh">
+      <img src="https://i.ibb.co/pJR7HfQ/image3.png" alt="image3">
+   </a>
+   <a href="https://ibb.co/Kb6qjmg">
+      <img src="https://i.ibb.co/sbjwvt4/image2.png" alt="image2">
+   </a>
+   <a href="https://ibb.co/0JkdkQy">
+      <img src="https://i.ibb.co/7yH6Hbt/image1.png" alt="image1">
+   </a>
 </div>
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you want to change.
 please follow the [contributing guidelines](https://github.com/Hetari/pyutube/blob/main/CONTRIBUTING.md)
```

### Comparing `pyutube-1.1.7/setup.py` & `pyutube-1.1.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,70 @@
+"""
+This module contains the setup configuration for the pyutube package.
+"""
+
+
+from setuptools import setup
 from pyutube.utils import __version__
-from setuptools import setup, find_packages
 
 
 # Read the README file to use as the long description
-with open("README.md", "r") as f:
+with open("README.md", "r", encoding="utf-8") as f:
     description = f.read()
 
 # Setup configuration
 setup(
-    # Name of the package
     name="pyutube",
 
-    # Version of the package
     version=__version__,
 
-    # Required dependencies
+    author="Ebraheem Alhetari",
+
+    author_email="hetari4all@gmail.com",
+
+    description="Awesome CLI to download YouTube videos (as video or audio)/shorts/playlists from the terminal",
+
+    long_description=description,
+
+    long_description_content_type="text/markdown",
+
+    keywords=["youtube", "download", "cli", "pyutube", "pytube"],
+
+    license="MIT",
+
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+    ],
+
+
+    include_package_data=True,
+
+    python_requires=">=3.6",
+
     install_requires=[
         "pytube",
         "inquirer",
         "yaspin",
         "typer",
         "requests",
         "rich",
         "inquirer",
-        "termcolor"
+        "termcolor",
+        "ffmpeg-python"
     ],
 
-    # Classifiers to categorize the package
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-    ],
 
-    # Entry points for console scripts
     entry_points={
         "console_scripts": [
-            "pyutube=pyutube:cli.app",  # Command to run the application
+            "pyutube=pyutube:cli.app",
         ],
     },
 
-    # Python version requirement
-    python_requires=">=3.6",
-
-    # Long description of the package
-    long_description=description,
 
-    # Description content type
-    long_description_content_type="text/markdown",
-
-    # Project URLs
     project_urls={
         "Homepage": "https://github.com/Hetari/pyutube",
-    }
+    },
+
+    platforms=["Windows", "MacOS", "Linux"],
 )
```

