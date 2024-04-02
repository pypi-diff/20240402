# Comparing `tmp/spotify_web_downloader-1.5.5.tar.gz` & `tmp/spotify_web_downloader-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_web_downloader-1.5.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "spotify_web_downloader-1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spotify_web_downloader-1.5.5.tar` & `spotify_web_downloader-1.6.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0     1137 2024-03-19 23:40:41.926834 spotify_web_downloader-1.5.5/.github/workflows/main.yml
--rw-r--r--   0        0        0       96 2024-03-19 23:40:41.926834 spotify_web_downloader-1.5.5/.gitignore
--rw-r--r--   0        0        0     6842 2024-03-19 23:40:41.926834 spotify_web_downloader-1.5.5/README.md
--rw-r--r--   0        0        0      533 2024-03-19 23:40:41.926834 spotify_web_downloader-1.5.5/pyproject.toml
--rw-r--r--   0        0        0       40 2024-03-19 23:40:41.926834 spotify_web_downloader-1.5.5/requirements.txt
--rw-r--r--   0        0        0       22 2024-03-19 23:40:41.926834 spotify_web_downloader-1.5.5/spotify_web_downloader/__init__.py
--rw-r--r--   0        0        0       30 2024-03-19 23:40:41.926834 spotify_web_downloader-1.5.5/spotify_web_downloader/__main__.py
--rw-r--r--   0        0        0    11641 2024-03-19 23:40:41.926834 spotify_web_downloader-1.5.5/spotify_web_downloader/cli.py
--rw-r--r--   0        0        0      440 2024-03-19 23:40:41.926834 spotify_web_downloader-1.5.5/spotify_web_downloader/constants.py
--rw-r--r--   0        0        0    16708 2024-03-19 23:40:41.926834 spotify_web_downloader-1.5.5/spotify_web_downloader/downloader.py
--rw-r--r--   0        0        0     4015 2024-03-19 23:40:41.926834 spotify_web_downloader-1.5.5/spotify_web_downloader/hardcoded_wvd.py
--rw-r--r--   0        0        0     7253 1970-01-01 00:00:00.000000 spotify_web_downloader-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1137 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/.github/workflows/main.yml
+-rw-r--r--   0        0        0       96 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/.gitignore
+-rw-r--r--   0        0        0     8410 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/README.md
+-rw-r--r--   0        0        0      533 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/requirements.txt
+-rw-r--r--   0        0        0       20 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/__main__.py
+-rw-r--r--   0        0        0    21135 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/cli.py
+-rw-r--r--   0        0        0      457 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/constants.py
+-rw-r--r--   0        0        0     8459 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/downloader.py
+-rw-r--r--   0        0        0    11132 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/downloader_music_video.py
+-rw-r--r--   0        0        0     8729 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/downloader_song.py
+-rw-r--r--   0        0        0      175 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/hardcoded_wvd.py
+-rw-r--r--   0        0        0      707 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/models.py
+-rw-r--r--   0        0        0     7367 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/spotify_api.py
+-rw-r--r--   0        0        0     8819 1970-01-01 00:00:00.000000 spotify_web_downloader-1.6/PKG-INFO
```

### Comparing `spotify_web_downloader-1.5.5/.github/workflows/main.yml` & `spotify_web_downloader-1.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.5.5/README.md` & `spotify_web_downloader-1.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,73 @@
 # Spotify Web Downloader
-A Python script to download songs/albums/playlists directly from Spotify in 256kbps/128kbps AAC.
+A Python script to download songs/music videos/albums/playlists directly from Spotify.
 
 ## Features
-* Download songs in 128kbps AAC or 256kbps AAC with a premium account
+* Download songs in 128kbps AAC or in 256kbps AAC with a premium account
+* Download music videos with a premium account
 * Download synced lyrics
-* Highly customizable
+* Highly configurable
+
+## Pre-requisites
+* The cookies file of your Spotify account (free or premium)
+    * You can get your cookies by using this Google Chrome extension on Spotify website: https://chrome.google.com/webstore/detail/open-cookiestxt/gdocmgbfkjnnpapoeobnolbbkoibbcif. Make sure to be logged in.
+* FFmpeg on your system PATH
+    * Older versions of FFmpeg may not work.
+* Python 3.7 or higher
 
 ## Installation
-1. Install Python 3.7 or higher
-2. Add [FFmpeg](https://ffmpeg.org/download.html) to PATH
-    * Older versions of FFmpeg may not work
-3. Place your cookies in the same folder that you will run spotify-web-downloader as `cookies.txt`
-    * You can export your cookies by using this Google Chrome extension on Spotify website: https://chrome.google.com/webstore/detail/open-cookiestxt/gdocmgbfkjnnpapoeobnolbbkoibbcif. Make sure to be logged in.
-4. Install spotify-web-downloader using pip
+1. Install the package `spotify-web-downloader` using pip
     ```bash
     pip install spotify-web-downloader
     ```
+2. Place your cookies in the same directory you will run the script from and name it `cookies.txt`
 
-## Examples
+## Usage
 * Download a song
     ```bash
     spotify-web-downloader "https://open.spotify.com/track/18gqCQzqYb0zvurQPlRkpo"
     ```
 * Download an album
     ```bash
     spotify-web-downloader "https://open.spotify.com/album/0r8D5N674HbTXlR3zNxeU1"
     ```
 
 ## Configuration
 spotify-web-downloader can be configured using the command line arguments or the config file. The config file is created automatically when you run spotify-web-downloader for the first time at `~/.spotify-web-downloader/config.json` on Linux and `%USERPROFILE%\.spotify-web-downloader\config.json` on Windows. Config file values can be overridden using command line arguments.
-| Command line argument / Config file key                         | Description                                                           | Default value                                       |
-| --------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------- |
-| `-f`, `--final-path` / `final_path`                             | Path where the downloaded files will be saved.                        | `./Spotify`                                         |
-| `-t`, `--temp-path` / `temp_path`                               | Path where the temporary files will be saved.                         | `./temp`                                            |
-| `-c`, `--cookies-location` / `cookies_location`                 | Location of the cookies file.                                         | `./cookies.txt`                                     |
-| `-w`, `--wvd-location` / `wvd_location`                         | Location of the .wvd file.                                            | `null`                                              |
-| `--config-location` / -                                         | Location of the config file.                                          | `<home_folder>/.spotify-web-downloader/config.json` |
-| `--ffmpeg-location` / `ffmpeg_location`                         | Location of the FFmpeg binary.                                        | `ffmpeg`                                            |
-| `--aria2c-location` / `aria2c_location`                         | Location of the aria2c binary.                                        | `aria2c`                                            |
-| `--template-folder-album` / `template_folder_album`             | Template of the album folders as a format string.                     | `{album_artist}/{album}`                            |
-| `--template-folder-compilation` / `template_folder_compilation` | Template of the compilation album folders as a format string.         | `Compilations/{album}`                              |
-| `--template-file-single-disc` / `template_file_single_disc`     | Template of the song files for single-disc albums as a format string. | `{track:02d} {title}`                               |
-| `--template-file-multi-disc` / `template_file_multi_disc`       | Template of the song files for multi-disc albums as a format string.  | `{disc}-{track:02d} {title}`                        |
-| `--download-mode` / `download_mode`                             | Download mode.                                                        | `ytdlp`                                             |
-| `-e`, `--exclude-tags` / `exclude_tags`                         | List of tags to exclude from file tagging separated by commas.        | `null`                                              |
-| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                              | `40`                                                |
-| `-l`, `--log-level` / `log_level`                               | Log level.                                                            | `INFO`                                              |
-| `-p`, `--premium-quality` / `premium_quality`                   | Download in 256kbps AAC instead of 128kbps AAC.                       | `false`                                             |
-| `-l`, `--lrc-only` / `lrc_only`                                 | Download only the synced lyrics.                                      | `false`                                             |
-| `-n`, `--no-lrc` / `no_lrc`                                     | Don't download the synced lyrics.                                     | `false`                                             |
-| `-s`, `--save-cover` / `save_cover`                             | Save cover as a separate file.                                        | `false`                                             |
-| `-o`, `--overwrite` / `overwrite`                               | Overwrite existing files.                                             | `false`                                             |
-| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                     | `false`                                             |
-| `-u`, `--url-txt` / -                                           | Read URLs as location of text files containing URLs.                  | `false`                                             |
-| `-n`, `--no-config-file` / -                                    | Don't use the config file.                                            | `false`                                             |
+| Command line argument / Config file key                         | Description                                                                  | Default value                                |
+| --------------------------------------------------------------- | ---------------------------------------------------------------------------- | -------------------------------------------- |
+| `--download-music-video` / `download_music_video`               | Attempt to download music videos from songs (can lead to incorrect results). | `false`                                      |
+| `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                               | `false`                                      |
+| `--overwrite` / `overwrite`                                     | Overwrite existing files.                                                    | `false`                                      |
+| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs.                       | `false`                                      |
+| `--lrc-only`, `-l` / `lrc_only`                                 | Download only the synced lyrics.                                             | `false`                                      |
+| `--no-lrc` / `no_lrc`                                           | Don't download the synced lyrics.                                            | `false`                                      |
+| `--config-path` / -                                             | Path to config file.                                                         | `<home>/.spotify-web-downloader/config.json` |
+| `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                                       |
+| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                                      |
+| `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`                              |
+| `--output-path`, `-o` / `output_path`                           | Path to output directory.                                                    | `./Spotify`                                  |
+| `--temp-path` / `temp_path`                                     | Path to temporary directory.                                                 | `./temp`                                     |
+| `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                           | `null`                                       |
+| `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                                       | `ffmpeg`                                     |
+| `--aria2c-path` / `aria2c_path`                                 | Path to aria2c binary.                                                       | `aria2c`                                     |
+| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8DL-RE`                                |
+| `--date-tag-template` / `date_tag_template`                     | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`                         |
+| `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                                       |
+| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                                         |
+| `--template-folder-album` / `template_folder_album`             | Template of the album folders as a format string.                            | `{album_artist}/{album}`                     |
+| `--template-folder-compilation` / `template_folder_compilation` | Template of the compilation album folders as a format string.                | `Compilations/{album}`                       |
+| `--template-file-single-disc` / `template_file_single_disc`     | Template of the song files for single-disc albums as a format string.        | `{track:02d} {title}`                        |
+| `--template-file-multi-disc` / `template_file_multi_disc`       | Template of the song files for multi-disc albums as a format string.         | `{disc}-{track:02d} {title}`                 |
+| `--download-mode-song` / `download_mode_song`                   | Download mode for songs.                                                     | `ydlp`                                       |
+| `--premium-quality`, `-p` / `premium_quality`                   | Download songs in premium quality.                                           | `false`                                      |
+| `--template-folder-music-video` / `template_folder_music_video` | Template of the music video folders as a format string.                      | `{artist}/Unknown Album`                     |
+| `--template-file-music-video` / `template_file_music_video`     | Template of the music video files as a format string.                        | `{title}`                                    |
+| `--download-mode-video` / `download_mode_video`                 | Download mode for videos.                                                    | `ydlp`                                       |
+| `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
 
 ### Tag variables
 The following variables can be used in the template folder/file and/or in the `exclude_tags` list:
 - `album`
 - `album_artist`
 - `artist`
 - `comment`
@@ -68,17 +78,27 @@
 - `disc_total`
 - `isrc`
 - `label`
 - `lyrics`
 - `media_type`
 - `rating`
 - `release_date`
+- `release_year`
 - `title`
 - `track`
 - `track_total`
 
+### Music videos quality
+Music videos will be downloaded in the highest quality available in H.254/AAC, up to 1080p.
+
 ### Download mode
-The following download modes are available:
+The following modes are available for songs:
 * `ytdlp`
 * `aria2c`
     * Faster than `ytdlp`
     * Can be obtained from here: https://github.com/aria2/aria2/releases
+
+The following modes are available for videos:
+* `ytdlp`
+* `nm38dlre`
+    * Faster than `ytdlp`
+    * Can be obtained from here: https://github.com/nilaoda/N_m3u8DL-RE/releases
```

### Comparing `spotify_web_downloader-1.5.5/pyproject.toml` & `spotify_web_downloader-1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.5.5/spotify_web_downloader/hardcoded_wvd.py` & `spotify_web_downloader-1.6/spotify_web_downloader/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.5.5/PKG-INFO` & `spotify_web_downloader-1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,87 @@
 Metadata-Version: 2.1
 Name: spotify-web-downloader
-Version: 1.5.5
+Version: 1.6
 Summary: Download songs/albums/playlists directly from Spotify in AAC
 Author: glomatico
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: pybase62
 Requires-Dist: pywidevine
 Requires-Dist: pyyaml
 Requires-Dist: yt-dlp
 Project-URL: repository, https://github.com/glomatico/spotify-web-downloader
 
 # Spotify Web Downloader
-A Python script to download songs/albums/playlists directly from Spotify in 256kbps/128kbps AAC.
+A Python script to download songs/music videos/albums/playlists directly from Spotify.
 
 ## Features
-* Download songs in 128kbps AAC or 256kbps AAC with a premium account
+* Download songs in 128kbps AAC or in 256kbps AAC with a premium account
+* Download music videos with a premium account
 * Download synced lyrics
-* Highly customizable
+* Highly configurable
+
+## Pre-requisites
+* The cookies file of your Spotify account (free or premium)
+    * You can get your cookies by using this Google Chrome extension on Spotify website: https://chrome.google.com/webstore/detail/open-cookiestxt/gdocmgbfkjnnpapoeobnolbbkoibbcif. Make sure to be logged in.
+* FFmpeg on your system PATH
+    * Older versions of FFmpeg may not work.
+* Python 3.7 or higher
 
 ## Installation
-1. Install Python 3.7 or higher
-2. Add [FFmpeg](https://ffmpeg.org/download.html) to PATH
-    * Older versions of FFmpeg may not work
-3. Place your cookies in the same folder that you will run spotify-web-downloader as `cookies.txt`
-    * You can export your cookies by using this Google Chrome extension on Spotify website: https://chrome.google.com/webstore/detail/open-cookiestxt/gdocmgbfkjnnpapoeobnolbbkoibbcif. Make sure to be logged in.
-4. Install spotify-web-downloader using pip
+1. Install the package `spotify-web-downloader` using pip
     ```bash
     pip install spotify-web-downloader
     ```
+2. Place your cookies in the same directory you will run the script from and name it `cookies.txt`
 
-## Examples
+## Usage
 * Download a song
     ```bash
     spotify-web-downloader "https://open.spotify.com/track/18gqCQzqYb0zvurQPlRkpo"
     ```
 * Download an album
     ```bash
     spotify-web-downloader "https://open.spotify.com/album/0r8D5N674HbTXlR3zNxeU1"
     ```
 
 ## Configuration
 spotify-web-downloader can be configured using the command line arguments or the config file. The config file is created automatically when you run spotify-web-downloader for the first time at `~/.spotify-web-downloader/config.json` on Linux and `%USERPROFILE%\.spotify-web-downloader\config.json` on Windows. Config file values can be overridden using command line arguments.
-| Command line argument / Config file key                         | Description                                                           | Default value                                       |
-| --------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------- |
-| `-f`, `--final-path` / `final_path`                             | Path where the downloaded files will be saved.                        | `./Spotify`                                         |
-| `-t`, `--temp-path` / `temp_path`                               | Path where the temporary files will be saved.                         | `./temp`                                            |
-| `-c`, `--cookies-location` / `cookies_location`                 | Location of the cookies file.                                         | `./cookies.txt`                                     |
-| `-w`, `--wvd-location` / `wvd_location`                         | Location of the .wvd file.                                            | `null`                                              |
-| `--config-location` / -                                         | Location of the config file.                                          | `<home_folder>/.spotify-web-downloader/config.json` |
-| `--ffmpeg-location` / `ffmpeg_location`                         | Location of the FFmpeg binary.                                        | `ffmpeg`                                            |
-| `--aria2c-location` / `aria2c_location`                         | Location of the aria2c binary.                                        | `aria2c`                                            |
-| `--template-folder-album` / `template_folder_album`             | Template of the album folders as a format string.                     | `{album_artist}/{album}`                            |
-| `--template-folder-compilation` / `template_folder_compilation` | Template of the compilation album folders as a format string.         | `Compilations/{album}`                              |
-| `--template-file-single-disc` / `template_file_single_disc`     | Template of the song files for single-disc albums as a format string. | `{track:02d} {title}`                               |
-| `--template-file-multi-disc` / `template_file_multi_disc`       | Template of the song files for multi-disc albums as a format string.  | `{disc}-{track:02d} {title}`                        |
-| `--download-mode` / `download_mode`                             | Download mode.                                                        | `ytdlp`                                             |
-| `-e`, `--exclude-tags` / `exclude_tags`                         | List of tags to exclude from file tagging separated by commas.        | `null`                                              |
-| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                              | `40`                                                |
-| `-l`, `--log-level` / `log_level`                               | Log level.                                                            | `INFO`                                              |
-| `-p`, `--premium-quality` / `premium_quality`                   | Download in 256kbps AAC instead of 128kbps AAC.                       | `false`                                             |
-| `-l`, `--lrc-only` / `lrc_only`                                 | Download only the synced lyrics.                                      | `false`                                             |
-| `-n`, `--no-lrc` / `no_lrc`                                     | Don't download the synced lyrics.                                     | `false`                                             |
-| `-s`, `--save-cover` / `save_cover`                             | Save cover as a separate file.                                        | `false`                                             |
-| `-o`, `--overwrite` / `overwrite`                               | Overwrite existing files.                                             | `false`                                             |
-| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                     | `false`                                             |
-| `-u`, `--url-txt` / -                                           | Read URLs as location of text files containing URLs.                  | `false`                                             |
-| `-n`, `--no-config-file` / -                                    | Don't use the config file.                                            | `false`                                             |
+| Command line argument / Config file key                         | Description                                                                  | Default value                                |
+| --------------------------------------------------------------- | ---------------------------------------------------------------------------- | -------------------------------------------- |
+| `--download-music-video` / `download_music_video`               | Attempt to download music videos from songs (can lead to incorrect results). | `false`                                      |
+| `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                               | `false`                                      |
+| `--overwrite` / `overwrite`                                     | Overwrite existing files.                                                    | `false`                                      |
+| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs.                       | `false`                                      |
+| `--lrc-only`, `-l` / `lrc_only`                                 | Download only the synced lyrics.                                             | `false`                                      |
+| `--no-lrc` / `no_lrc`                                           | Don't download the synced lyrics.                                            | `false`                                      |
+| `--config-path` / -                                             | Path to config file.                                                         | `<home>/.spotify-web-downloader/config.json` |
+| `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                                       |
+| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                                      |
+| `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`                              |
+| `--output-path`, `-o` / `output_path`                           | Path to output directory.                                                    | `./Spotify`                                  |
+| `--temp-path` / `temp_path`                                     | Path to temporary directory.                                                 | `./temp`                                     |
+| `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                           | `null`                                       |
+| `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                                       | `ffmpeg`                                     |
+| `--aria2c-path` / `aria2c_path`                                 | Path to aria2c binary.                                                       | `aria2c`                                     |
+| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8DL-RE`                                |
+| `--date-tag-template` / `date_tag_template`                     | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`                         |
+| `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                                       |
+| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                                         |
+| `--template-folder-album` / `template_folder_album`             | Template of the album folders as a format string.                            | `{album_artist}/{album}`                     |
+| `--template-folder-compilation` / `template_folder_compilation` | Template of the compilation album folders as a format string.                | `Compilations/{album}`                       |
+| `--template-file-single-disc` / `template_file_single_disc`     | Template of the song files for single-disc albums as a format string.        | `{track:02d} {title}`                        |
+| `--template-file-multi-disc` / `template_file_multi_disc`       | Template of the song files for multi-disc albums as a format string.         | `{disc}-{track:02d} {title}`                 |
+| `--download-mode-song` / `download_mode_song`                   | Download mode for songs.                                                     | `ydlp`                                       |
+| `--premium-quality`, `-p` / `premium_quality`                   | Download songs in premium quality.                                           | `false`                                      |
+| `--template-folder-music-video` / `template_folder_music_video` | Template of the music video folders as a format string.                      | `{artist}/Unknown Album`                     |
+| `--template-file-music-video` / `template_file_music_video`     | Template of the music video files as a format string.                        | `{title}`                                    |
+| `--download-mode-video` / `download_mode_video`                 | Download mode for videos.                                                    | `ydlp`                                       |
+| `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
 
 ### Tag variables
 The following variables can be used in the template folder/file and/or in the `exclude_tags` list:
 - `album`
 - `album_artist`
 - `artist`
 - `comment`
@@ -82,18 +92,28 @@
 - `disc_total`
 - `isrc`
 - `label`
 - `lyrics`
 - `media_type`
 - `rating`
 - `release_date`
+- `release_year`
 - `title`
 - `track`
 - `track_total`
 
+### Music videos quality
+Music videos will be downloaded in the highest quality available in H.254/AAC, up to 1080p.
+
 ### Download mode
-The following download modes are available:
+The following modes are available for songs:
 * `ytdlp`
 * `aria2c`
     * Faster than `ytdlp`
     * Can be obtained from here: https://github.com/aria2/aria2/releases
 
+The following modes are available for videos:
+* `ytdlp`
+* `nm38dlre`
+    * Faster than `ytdlp`
+    * Can be obtained from here: https://github.com/nilaoda/N_m3u8DL-RE/releases
+
```

