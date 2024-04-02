# Comparing `tmp/devine-3.2.0.tar.gz` & `tmp/devine-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devine-3.2.0.tar", max compression
+gzip compressed data, was "devine-3.3.0.tar", max compression
```

## Comparing `devine-3.2.0.tar` & `devine-3.3.0.tar`

### file list

```diff
@@ -1,67 +1,69 @@
--rw-r--r--   0        0        0    53046 2024-03-25 03:54:38.351468 devine-3.2.0/CHANGELOG.md
--rw-r--r--   0        0        0    35822 2024-03-25 03:54:38.351468 devine-3.2.0/LICENSE
--rw-r--r--   0        0        0    19888 2024-03-25 03:54:38.351468 devine-3.2.0/README.md
--rw-r--r--   0        0        0       80 2024-03-25 03:54:38.351468 devine-3.2.0/devine/__main__.py
--rw-r--r--   0        0        0        0 2024-03-25 03:54:38.351468 devine-3.2.0/devine/commands/__init__.py
--rw-r--r--   0        0        0     3254 2024-03-25 03:54:38.351468 devine-3.2.0/devine/commands/cfg.py
--rw-r--r--   0        0        0    43024 2024-03-25 03:54:38.351468 devine-3.2.0/devine/commands/dl.py
--rw-r--r--   0        0        0     2247 2024-03-25 03:54:38.351468 devine-3.2.0/devine/commands/env.py
--rw-r--r--   0        0        0     7986 2024-03-25 03:54:38.351468 devine-3.2.0/devine/commands/kv.py
--rw-r--r--   0        0        0     6574 2024-03-25 03:54:38.351468 devine-3.2.0/devine/commands/search.py
--rw-r--r--   0        0        0     1743 2024-03-25 03:54:38.351468 devine-3.2.0/devine/commands/serve.py
--rw-r--r--   0        0        0     9243 2024-03-25 03:54:38.351468 devine-3.2.0/devine/commands/util.py
--rw-r--r--   0        0        0     9320 2024-03-25 03:54:38.351468 devine-3.2.0/devine/commands/wvd.py
--rw-r--r--   0        0        0       22 2024-03-25 03:54:38.351468 devine-3.2.0/devine/core/__init__.py
--rw-r--r--   0        0        0     2857 2024-03-25 03:54:38.351468 devine-3.2.0/devine/core/__main__.py
--rw-r--r--   0        0        0     6195 2024-03-25 03:54:38.351468 devine-3.2.0/devine/core/cacher.py
--rw-r--r--   0        0        0     1215 2024-03-25 03:54:38.351468 devine-3.2.0/devine/core/commands.py
--rw-r--r--   0        0        0     4441 2024-03-25 03:54:38.351468 devine-3.2.0/devine/core/config.py
--rw-r--r--   0        0        0    15343 2024-03-25 03:54:38.351468 devine-3.2.0/devine/core/console.py
--rw-r--r--   0        0        0     1065 2024-03-25 03:54:38.351468 devine-3.2.0/devine/core/constants.py
--rw-r--r--   0        0        0     3380 2024-03-25 03:54:38.351468 devine-3.2.0/devine/core/credential.py
--rw-r--r--   0        0        0      159 2024-03-25 03:54:38.351468 devine-3.2.0/devine/core/downloaders/__init__.py
--rw-r--r--   0        0        0    13339 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/downloaders/aria2c.py
--rw-r--r--   0        0        0    11609 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/downloaders/curl_impersonate.py
--rw-r--r--   0        0        0    11931 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/downloaders/requests.py
--rw-r--r--   0        0        0      199 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/drm/__init__.py
--rw-r--r--   0        0        0     4020 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/drm/clearkey.py
--rw-r--r--   0        0        0    11898 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/drm/widevine.py
--rw-r--r--   0        0        0       71 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/manifests/__init__.py
--rw-r--r--   0        0        0    31115 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/manifests/dash.py
--rw-r--r--   0        0        0    28091 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/manifests/hls.py
--rw-r--r--   0        0        0      117 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/proxies/__init__.py
--rw-r--r--   0        0        0      929 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/proxies/basic.py
--rw-r--r--   0        0        0     2290 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/proxies/hola.py
--rw-r--r--   0        0        0     5565 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/proxies/nordvpn.py
--rw-r--r--   0        0        0     1048 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/proxies/proxy.py
--rw-r--r--   0        0        0     1714 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/search_result.py
--rw-r--r--   0        0        0    11069 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/service.py
--rw-r--r--   0        0        0     3001 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/services.py
--rw-r--r--   0        0        0      298 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/titles/__init__.py
--rw-r--r--   0        0        0     8002 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/titles/episode.py
--rw-r--r--   0        0        0     5538 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/titles/movie.py
--rw-r--r--   0        0        0     4689 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/titles/song.py
--rw-r--r--   0        0        0     2595 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/titles/title.py
--rw-r--r--   0        0        0      277 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/tracks/__init__.py
--rw-r--r--   0        0        0     5001 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/tracks/audio.py
--rw-r--r--   0        0        0     2961 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/tracks/chapter.py
--rw-r--r--   0        0        0     5352 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/tracks/chapters.py
--rw-r--r--   0        0        0    23318 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/tracks/subtitle.py
--rw-r--r--   0        0        0    21903 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/tracks/track.py
--rw-r--r--   0        0        0    16177 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/tracks/tracks.py
--rw-r--r--   0        0        0    13118 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/tracks/video.py
--rw-r--r--   0        0        0    10003 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/utilities.py
--rw-r--r--   0        0        0        0 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/utils/__init__.py
--rw-r--r--   0        0        0     6227 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/utils/click_types.py
--rw-r--r--   0        0        0     1532 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/utils/collections.py
--rw-r--r--   0        0        0     3699 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/utils/sslciphers.py
--rw-r--r--   0        0        0      845 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/utils/subprocess.py
--rw-r--r--   0        0        0      791 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/utils/xml.py
--rw-r--r--   0        0        0     1711 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/vault.py
--rw-r--r--   0        0        0     2518 2024-03-25 03:54:38.355468 devine-3.2.0/devine/core/vaults.py
--rw-r--r--   0        0        0     6414 2024-03-25 03:54:38.359468 devine-3.2.0/devine/vaults/API.py
--rw-r--r--   0        0        0     8485 2024-03-25 03:54:38.359468 devine-3.2.0/devine/vaults/MySQL.py
--rw-r--r--   0        0        0     6076 2024-03-25 03:54:38.359468 devine-3.2.0/devine/vaults/SQLite.py
--rw-r--r--   0        0        0        0 2024-03-25 03:54:38.359468 devine-3.2.0/devine/vaults/__init__.py
--rw-r--r--   0        0        0     2650 2024-03-25 03:54:38.359468 devine-3.2.0/pyproject.toml
--rw-r--r--   0        0        0    22374 1970-01-01 00:00:00.000000 devine-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0    54122 2024-04-02 21:00:25.663346 devine-3.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35822 2024-04-02 21:00:25.663346 devine-3.3.0/LICENSE
+-rw-r--r--   0        0        0    19888 2024-04-02 21:00:25.663346 devine-3.3.0/README.md
+-rw-r--r--   0        0        0       80 2024-04-02 21:00:25.663346 devine-3.3.0/devine/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-02 21:00:25.663346 devine-3.3.0/devine/commands/__init__.py
+-rw-r--r--   0        0        0     3254 2024-04-02 21:00:25.663346 devine-3.3.0/devine/commands/cfg.py
+-rw-r--r--   0        0        0    45664 2024-04-02 21:00:25.663346 devine-3.3.0/devine/commands/dl.py
+-rw-r--r--   0        0        0     2247 2024-04-02 21:00:25.667346 devine-3.3.0/devine/commands/env.py
+-rw-r--r--   0        0        0     7986 2024-04-02 21:00:25.667346 devine-3.3.0/devine/commands/kv.py
+-rw-r--r--   0        0        0     6574 2024-04-02 21:00:25.667346 devine-3.3.0/devine/commands/search.py
+-rw-r--r--   0        0        0     1743 2024-04-02 21:00:25.667346 devine-3.3.0/devine/commands/serve.py
+-rw-r--r--   0        0        0     9243 2024-04-02 21:00:25.667346 devine-3.3.0/devine/commands/util.py
+-rw-r--r--   0        0        0     9920 2024-04-02 21:00:25.667346 devine-3.3.0/devine/commands/wvd.py
+-rw-r--r--   0        0        0       22 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/__init__.py
+-rw-r--r--   0        0        0     2857 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/__main__.py
+-rw-r--r--   0        0        0     6195 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/cacher.py
+-rw-r--r--   0        0        0     1215 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/commands.py
+-rw-r--r--   0        0        0     4481 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/config.py
+-rw-r--r--   0        0        0    15343 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/console.py
+-rw-r--r--   0        0        0     1065 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/constants.py
+-rw-r--r--   0        0        0     3380 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/credential.py
+-rw-r--r--   0        0        0      159 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/downloaders/__init__.py
+-rw-r--r--   0        0        0    13339 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/downloaders/aria2c.py
+-rw-r--r--   0        0        0    11697 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/downloaders/curl_impersonate.py
+-rw-r--r--   0        0        0    11931 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/downloaders/requests.py
+-rw-r--r--   0        0        0      199 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/drm/__init__.py
+-rw-r--r--   0        0        0     4020 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/drm/clearkey.py
+-rw-r--r--   0        0        0    11898 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/drm/widevine.py
+-rw-r--r--   0        0        0     2753 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/events.py
+-rw-r--r--   0        0        0       71 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/manifests/__init__.py
+-rw-r--r--   0        0        0    31228 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/manifests/dash.py
+-rw-r--r--   0        0        0    28214 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/manifests/hls.py
+-rw-r--r--   0        0        0      117 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/proxies/__init__.py
+-rw-r--r--   0        0        0     1958 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/proxies/basic.py
+-rw-r--r--   0        0        0     2290 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/proxies/hola.py
+-rw-r--r--   0        0        0     5565 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/proxies/nordvpn.py
+-rw-r--r--   0        0        0     1048 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/proxies/proxy.py
+-rw-r--r--   0        0        0     1714 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/search_result.py
+-rw-r--r--   0        0        0    12729 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/service.py
+-rw-r--r--   0        0        0     3001 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/services.py
+-rw-r--r--   0        0        0      298 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/titles/__init__.py
+-rw-r--r--   0        0        0     8002 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/titles/episode.py
+-rw-r--r--   0        0        0     5538 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/titles/movie.py
+-rw-r--r--   0        0        0     4689 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/titles/song.py
+-rw-r--r--   0        0        0     2595 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/titles/title.py
+-rw-r--r--   0        0        0      277 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/tracks/__init__.py
+-rw-r--r--   0        0        0     2132 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/tracks/attachment.py
+-rw-r--r--   0        0        0     5001 2024-04-02 21:00:25.667346 devine-3.3.0/devine/core/tracks/audio.py
+-rw-r--r--   0        0        0     2961 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/tracks/chapter.py
+-rw-r--r--   0        0        0     5352 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/tracks/chapters.py
+-rw-r--r--   0        0        0    23318 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/tracks/subtitle.py
+-rw-r--r--   0        0        0    21426 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/tracks/track.py
+-rw-r--r--   0        0        0    17269 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/tracks/tracks.py
+-rw-r--r--   0        0        0    13118 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/tracks/video.py
+-rw-r--r--   0        0        0    10741 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utilities.py
+-rw-r--r--   0        0        0        0 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utils/__init__.py
+-rw-r--r--   0        0        0     6227 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utils/click_types.py
+-rw-r--r--   0        0        0     1532 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utils/collections.py
+-rw-r--r--   0        0        0     3699 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utils/sslciphers.py
+-rw-r--r--   0        0        0      845 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utils/subprocess.py
+-rw-r--r--   0        0        0      791 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/utils/xml.py
+-rw-r--r--   0        0        0     1711 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/vault.py
+-rw-r--r--   0        0        0     2518 2024-04-02 21:00:25.671346 devine-3.3.0/devine/core/vaults.py
+-rw-r--r--   0        0        0     6414 2024-04-02 21:00:25.671346 devine-3.3.0/devine/vaults/API.py
+-rw-r--r--   0        0        0     8485 2024-04-02 21:00:25.671346 devine-3.3.0/devine/vaults/MySQL.py
+-rw-r--r--   0        0        0     6076 2024-04-02 21:00:25.671346 devine-3.3.0/devine/vaults/SQLite.py
+-rw-r--r--   0        0        0        0 2024-04-02 21:00:25.671346 devine-3.3.0/devine/vaults/__init__.py
+-rw-r--r--   0        0        0     2650 2024-04-02 21:00:25.671346 devine-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0    22374 1970-01-01 00:00:00.000000 devine-3.3.0/PKG-INFO
```

### Comparing `devine-3.2.0/CHANGELOG.md` & `devine-3.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,43 @@
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Versions [3.0.0] and older use a format based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 but versions thereafter use a custom changelog format using [git-cliff](https://git-cliff.org).
 
+## [3.3.0] - 2024-04-02
+
+### Features
+
+- Add support for MKV Attachments via Attachment class
+- *dl*: Automatically attach fonts used within SSAv4 subs
+- *dl*: Try find SSAv4 fonts in System OS fonts folder
+- *Basic*: Allow single string URIs for countries
+- *Basic*: Allow proxy selection by index (one-indexed)
+- *Events*: Add new global Event Observer API
+
+### Bug Fixes
+
+- *curl-impersonate*: Set Cert-Authority Bundle for HTTPS Proxies
+- *Basic*: Make query case-insensitive
+- *WVD*: Ensure WVDs dir exists before moving WVD file
+- *WVD*: Fix empty path to WVDs folder check
+- *WVD*: Move log out of loop to save performance
+- *WVD*: Move log with path before Device load
+- *WVD*: Add exists/empty checks to WVD folder dumps
+- *Basic*: Fix variable typo regression
+
+### Changes
+
+- *Basic*: Improve proxy format checks
+- *WVD*: Print error if path to parse doesn't exist
+- *WVD*: Seperate logs in loop for visual clarity
+- *Track*: Move from OnXyz callables to Event observer
+
 ## [3.2.0] - 2024-03-25
 
 ### Features
 
 - *ClearKey*: Pass session not proxy str in from_m3u_key method
 - *Track*: Allow Track to choose downloader to use
 - *search*: New Search command, Service method, SearchResult Class
@@ -715,14 +744,15 @@
 - Fixed crash when adding a Cookie using `auth add` to a Service that has no directory yet.
 - Fixed crash when adding a Credential using `auth add` when it's the first ever credential, or first for the Service.
 
 ## [1.0.0] - 2023-02-06
 
 Initial public release under the name Devine.
 
+[3.3.0]: https://github.com/devine-dl/devine/releases/tag/v3.3.0
 [3.2.0]: https://github.com/devine-dl/devine/releases/tag/v3.2.0
 [3.1.0]: https://github.com/devine-dl/devine/releases/tag/v3.1.0
 [3.0.0]: https://github.com/devine-dl/devine/releases/tag/v3.0.0
 [2.2.0]: https://github.com/devine-dl/devine/releases/tag/v2.2.0
 [2.1.0]: https://github.com/devine-dl/devine/releases/tag/v2.1.0
 [2.0.1]: https://github.com/devine-dl/devine/releases/tag/v2.0.1
 [2.0.0]: https://github.com/devine-dl/devine/releases/tag/v2.0.0
```

### Comparing `devine-3.2.0/LICENSE` & `devine-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/README.md` & `devine-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/commands/cfg.py` & `devine-3.3.0/devine/commands/cfg.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/commands/dl.py` & `devine-3.3.0/devine/commands/dl.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,23 @@
 from rich.tree import Tree
 
 from devine.core.config import config
 from devine.core.console import console
 from devine.core.constants import DOWNLOAD_LICENCE_ONLY, AnyTrack, context_settings
 from devine.core.credential import Credential
 from devine.core.drm import DRM_T, Widevine
+from devine.core.events import events
 from devine.core.proxies import Basic, Hola, NordVPN
 from devine.core.service import Service
 from devine.core.services import Services
 from devine.core.titles import Movie, Song, Title_T
 from devine.core.titles.episode import Episode
 from devine.core.tracks import Audio, Subtitle, Tracks, Video
-from devine.core.utilities import get_binary_path, is_close_match, time_elapsed_since
+from devine.core.tracks.attachment import Attachment
+from devine.core.utilities import get_binary_path, get_system_fonts, is_close_match, time_elapsed_since
 from devine.core.utils.click_types import LANGUAGE_RANGE, QUALITY_LIST, SEASON_RANGE, ContextData, MultipleChoice
 from devine.core.utils.collections import merge_dict
 from devine.core.utils.subprocess import ffprobe
 from devine.core.vaults import Vaults
 
 
 class dl:
@@ -319,14 +321,22 @@
             ))
 
             if slow and i != 0:
                 delay = random.randint(60, 120)
                 with console.status(f"Delaying by {delay} seconds..."):
                     time.sleep(delay)
 
+            with console.status("Subscribing to events...", spinner="dots"):
+                events.reset()
+                events.subscribe(events.Types.SEGMENT_DOWNLOADED, service.on_segment_downloaded)
+                events.subscribe(events.Types.TRACK_DOWNLOADED, service.on_track_downloaded)
+                events.subscribe(events.Types.TRACK_DECRYPTED, service.on_track_decrypted)
+                events.subscribe(events.Types.TRACK_REPACKED, service.on_track_repacked)
+                events.subscribe(events.Types.TRACK_MULTIPLEX, service.on_track_multiplex)
+
             with console.status("Getting tracks...", spinner="dots"):
                 title.tracks.add(service.get_tracks(title), warn_only=True)
                 title.tracks.chapters = service.get_chapters(title)
 
             # strip SDH subs to non-SDH if no equivalent same-lang non-SDH is available
             # uses a loose check, e.g, wont strip en-US SDH sub if a non-SDH en-GB is available
             for subtitle in title.tracks.subtitles:
@@ -334,16 +344,21 @@
                     is_close_match(subtitle.language, [x.language])
                     for x in title.tracks.subtitles
                     if not x.sdh and not x.forced
                 ):
                     non_sdh_sub = deepcopy(subtitle)
                     non_sdh_sub.id += "_stripped"
                     non_sdh_sub.sdh = False
-                    non_sdh_sub.OnMultiplex = lambda: non_sdh_sub.strip_hearing_impaired()
                     title.tracks.add(non_sdh_sub)
+                    events.subscribe(
+                        events.Types.TRACK_MULTIPLEX,
+                        lambda track: (
+                            track.strip_hearing_impaired()
+                        ) if track.id == non_sdh_sub.id else None
+                    )
 
             with console.status("Sorting tracks by language and bitrate...", spinner="dots"):
                 title.tracks.sort_videos(by_language=v_lang or lang)
                 title.tracks.sort_audio(by_language=lang)
                 title.tracks.sort_subtitles(by_language=s_lang)
 
             if list_:
@@ -593,22 +608,53 @@
 
                 if sub_format:
                     with console.status(f"Converting Subtitles to {sub_format.name}..."):
                         for subtitle in title.tracks.subtitles:
                             if subtitle.codec != sub_format:
                                 subtitle.convert(sub_format)
 
+                with console.status("Checking Subtitles for Fonts..."):
+                    font_names = []
+                    for subtitle in title.tracks.subtitles:
+                        if subtitle.codec == Subtitle.Codec.SubStationAlphav4:
+                            for line in subtitle.path.read_text("utf8").splitlines():
+                                if line.startswith("Style: "):
+                                    font_names.append(line.removesuffix("Style: ").split(",")[1])
+
+                    font_count = 0
+                    system_fonts = get_system_fonts()
+                    for font_name in set(font_names):
+                        family_dir = Path(config.directories.fonts, font_name)
+                        fonts_from_system = [
+                            file
+                            for name, file in system_fonts.items()
+                            if name.startswith(font_name)
+                        ]
+                        if family_dir.exists():
+                            fonts = family_dir.glob("*.*tf")
+                            for font in fonts:
+                                title.tracks.add(Attachment(font, f"{font_name} ({font.stem})"))
+                                font_count += 1
+                        elif fonts_from_system:
+                            for font in fonts_from_system:
+                                title.tracks.add(Attachment(font, f"{font_name} ({font.stem})"))
+                                font_count += 1
+                        else:
+                            self.log.warning(f"Subtitle uses font [text2]{font_name}[/] but it could not be found...")
+
+                    if font_count:
+                        self.log.info(f"Attached {font_count} fonts for the Subtitles")
+
                 with console.status("Repackaging tracks with FFMPEG..."):
                     has_repacked = False
                     for track in title.tracks:
                         if track.needs_repack:
                             track.repackage()
                             has_repacked = True
-                            if callable(track.OnRepacked):
-                                track.OnRepacked()
+                            events.emit(events.Types.TRACK_REPACKED, track=track)
                     if has_repacked:
                         # we don't want to fill up the log with "Repacked x track"
                         self.log.info("Repacked one or more tracks with FFMPEG")
 
                 muxed_paths = []
 
                 if isinstance(title, (Movie, Episode)):
@@ -628,15 +674,15 @@
                             if len(quality) > 1:
                                 task_description += f" {video_track.height}p"
                             if len(range_) > 1:
                                 task_description += f" {video_track.range.name}"
 
                         task_id = progress.add_task(f"{task_description}...", total=None, start=False)
 
-                        task_tracks = Tracks(title.tracks) + title.tracks.chapters
+                        task_tracks = Tracks(title.tracks) + title.tracks.chapters + title.tracks.attachments
                         if video_track:
                             task_tracks.videos = [video_track]
 
                         multiplex_tasks.append((task_id, task_tracks))
 
                     with Live(
                         Padding(progress, (0, 5, 1, 5)),
```

### Comparing `devine-3.2.0/devine/commands/env.py` & `devine-3.3.0/devine/commands/env.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/commands/kv.py` & `devine-3.3.0/devine/commands/kv.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/commands/search.py` & `devine-3.3.0/devine/commands/search.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/commands/serve.py` & `devine-3.3.0/devine/commands/serve.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/commands/util.py` & `devine-3.3.0/devine/commands/util.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/commands/wvd.py` & `devine-3.3.0/devine/commands/wvd.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         if not path.exists():
             log.error(f"The WVD path '{path}' does not exist...")
         elif dst_path.exists():
             log.error(f"WVD named '{path.stem}' already exists...")
         else:
             # TODO: Check for and log errors
             _ = Device.load(path)  # test if WVD is valid
+            dst_path.parent.mkdir(parents=True, exist_ok=True)
             shutil.move(path, dst_path)
             log.info(f"Added {path.stem}")
 
 
 @wvd.command()
 @click.argument("names", type=str, nargs=-1)
 def delete(names: list[str]) -> None:
@@ -79,14 +80,18 @@
     except ValueError:
         named = False
     if named:
         path = config.directories.wvds / f"{path.name}.wvd"
 
     log = logging.getLogger("wvd")
 
+    if not path.exists():
+        console.log(f"[bright_blue]{path.absolute()}[/] does not exist...")
+        return
+
     device = Device.load(path)
 
     log.info(f"System ID: {device.system_id}")
     log.info(f"Security Level: {device.security_level}")
     log.info(f"Type: {device.type}")
     log.info(f"Flags: {device.flags}")
     log.info(f"Private Key: {bool(device.private_key)}")
@@ -111,29 +116,42 @@
 def dump(wvd_paths: list[Path], out_dir: Path) -> None:
     """
     Extract data from a .WVD Widevine Device file to a folder structure.
 
     If the path is relative, with no file extension, it will dump the WVD in the WVDs
     directory.
     """
-    if wvd_paths == (Path(""),):
-        wvd_paths = list(config.directories.wvds.iterdir())
-    for wvd_path, out_path in zip(wvd_paths, (out_dir / x.stem for x in wvd_paths)):
+    log = logging.getLogger("wvd")
+
+    if wvd_paths == ():
+        if not config.directories.wvds.exists():
+            console.log(f"[bright_blue]{config.directories.wvds.absolute()}[/] does not exist...")
+        wvd_paths = list(
+            x
+            for x in config.directories.wvds.iterdir()
+            if x.is_file() and x.suffix.lower() == ".wvd"
+        )
+        if not wvd_paths:
+            console.log(f"[bright_blue]{config.directories.wvds.absolute()}[/] is empty...")
+
+    for i, (wvd_path, out_path) in enumerate(zip(wvd_paths, (out_dir / x.stem for x in wvd_paths))):
+        if i > 0:
+            log.info("")
+
         try:
             named = not wvd_path.suffix and wvd_path.relative_to(Path(""))
         except ValueError:
             named = False
         if named:
             wvd_path = config.directories.wvds / f"{wvd_path.stem}.wvd"
         out_path.mkdir(parents=True, exist_ok=True)
 
+        log.info(f"Dumping: {wvd_path}")
         device = Device.load(wvd_path)
 
-        log = logging.getLogger("wvd")
-        log.info(f"Dumping: {wvd_path}")
         log.info(f"L{device.security_level} {device.system_id} {device.type.name}")
         log.info(f"Saving to: {out_path}")
 
         device_meta = {
             "wvd": {
                 "device_type": device.type.name,
                 "security_level": device.security_level,
```

### Comparing `devine-3.2.0/devine/core/__main__.py` & `devine-3.3.0/devine/core/__main__.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/cacher.py` & `devine-3.3.0/devine/core/cacher.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/commands.py` & `devine-3.3.0/devine/core/commands.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/config.py` & `devine-3.3.0/devine/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         # default directories, do not modify here, set via config
         app_dirs = AppDirs("devine", False)
         core_dir = Path(__file__).resolve().parent
         namespace_dir = core_dir.parent
         commands = namespace_dir / "commands"
         services = namespace_dir / "services"
         vaults = namespace_dir / "vaults"
+        fonts = namespace_dir / "fonts"
         user_configs = Path(app_dirs.user_config_dir)
         data = Path(app_dirs.user_data_dir)
         downloads = Path.home() / "Downloads" / "devine"
         temp = Path(tempfile.gettempdir()) / "devine"
         cache = Path(app_dirs.user_cache_dir)
         cookies = data / "Cookies"
         logs = Path(app_dirs.user_log_dir)
```

### Comparing `devine-3.2.0/devine/core/console.py` & `devine-3.3.0/devine/core/console.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/constants.py` & `devine-3.3.0/devine/core/constants.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/credential.py` & `devine-3.3.0/devine/core/credential.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/downloaders/aria2c.py` & `devine-3.3.0/devine/core/downloaders/aria2c.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/downloaders/curl_impersonate.py` & `devine-3.3.0/devine/core/downloaders/curl_impersonate.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import time
 from concurrent import futures
 from concurrent.futures.thread import ThreadPoolExecutor
 from http.cookiejar import CookieJar
 from pathlib import Path
 from typing import Any, Generator, MutableMapping, Optional, Union
 
+from curl_cffi import CurlOpt
 from curl_cffi.requests import Session
 from rich import filesize
 
 from devine.core.config import config
 from devine.core.constants import DOWNLOAD_CANCELLED
 from devine.core.utilities import get_extension
 
@@ -19,15 +20,15 @@
 PROGRESS_WINDOW = 5
 BROWSER = config.curl_impersonate.get("browser", "chrome120")
 
 
 def download(
     url: str,
     save_path: Path,
-    session: Optional[Session] = None,
+    session: Session,
     **kwargs: Any
 ) -> Generator[dict[str, Any], None, None]:
     """
     Download files using Curl Impersonate.
     https://github.com/lwthiker/curl-impersonate
 
     Yields the following download status updates while chunks are downloading:
@@ -48,16 +49,18 @@
         session: The Requests or Curl-Impersonate Session to make HTTP requests with.
             Useful to set Header, Cookie, and Proxy data. Connections are saved and
             re-used with the session so long as the server keeps the connection alive.
         kwargs: Any extra keyword arguments to pass to the session.get() call. Use this
             for one-time request changes like a header, cookie, or proxy. For example,
             to request Byte-ranges use e.g., `headers={"Range": "bytes=0-128"}`.
     """
-    if not session:
-        session = Session(impersonate=BROWSER)
+    # https://github.com/yifeikong/curl_cffi/issues/6#issuecomment-2028518677
+    # must be applied here since the `session.curl` is thread-localized
+    # noinspection PyProtectedMember
+    session.curl.setopt(CurlOpt.PROXY_CAINFO, session.curl._cacert)
 
     save_dir = save_path.parent
     control_file = save_path.with_name(f"{save_path.name}.!dev")
 
     save_dir.mkdir(parents=True, exist_ok=True)
 
     if control_file.exists():
@@ -220,18 +223,15 @@
             for k, v in headers.items()
             if k.lower() != "accept-encoding"
         }
         session.headers.update(headers)
     if cookies:
         session.cookies.update(cookies)
     if proxy:
-        session.proxies.update({
-            "http": proxy.replace("https://", "http://"),
-            "https": proxy.replace("https://", "http://")
-        })
+        session.proxies.update({"all": proxy})
 
     yield dict(total=len(urls))
 
     download_sizes = []
     last_speed_refresh = time.time()
 
     with ThreadPoolExecutor(max_workers=max_workers) as pool:
```

### Comparing `devine-3.2.0/devine/core/downloaders/requests.py` & `devine-3.3.0/devine/core/downloaders/requests.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/drm/clearkey.py` & `devine-3.3.0/devine/core/drm/clearkey.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/drm/widevine.py` & `devine-3.3.0/devine/core/drm/widevine.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/manifests/dash.py` & `devine-3.3.0/devine/core/manifests/dash.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from pywidevine.cdm import Cdm as WidevineCdm
 from pywidevine.pssh import PSSH
 from requests import Session
 
 from devine.core.constants import DOWNLOAD_CANCELLED, DOWNLOAD_LICENCE_ONLY, AnyTrack
 from devine.core.downloaders import requests as requests_downloader
 from devine.core.drm import Widevine
+from devine.core.events import events
 from devine.core.tracks import Audio, Subtitle, Tracks, Video
 from devine.core.utilities import is_close_match, try_ensure_utf8
 from devine.core.utils.xml import load_xml
 
 
 class DASH:
     def __init__(self, manifest, url: str):
@@ -470,16 +471,16 @@
             filename="{i:0%d}.mp4" % (len(str(len(segments)))),
             headers=session.headers,
             cookies=session.cookies,
             proxy=proxy,
             max_workers=16
         ):
             file_downloaded = status_update.get("file_downloaded")
-            if file_downloaded and callable(track.OnSegmentDownloaded):
-                track.OnSegmentDownloaded(file_downloaded)
+            if file_downloaded:
+                events.emit(events.Types.SEGMENT_DOWNLOADED, track=track, segment=file_downloaded)
             else:
                 downloaded = status_update.get("downloaded")
                 if downloaded and downloaded.endswith("/s"):
                     status_update["downloaded"] = f"DASH {downloaded}"
                 progress(**status_update)
 
         # see https://github.com/devine-dl/devine/issues/71
@@ -510,23 +511,26 @@
                         encode("utf8")
                 f.write(segment_data)
                 f.flush()
                 segment_file.unlink()
                 progress(advance=1)
 
         track.path = save_path
-        if callable(track.OnDownloaded):
-            track.OnDownloaded()
+        events.emit(events.Types.TRACK_DOWNLOADED, track=track)
 
         if drm:
             progress(downloaded="Decrypting", completed=0, total=100)
             drm.decrypt(save_path)
             track.drm = None
-            if callable(track.OnDecrypted):
-                track.OnDecrypted(drm)
+            events.emit(
+                events.Types.TRACK_DECRYPTED,
+                track=track,
+                drm=drm,
+                segment=None
+            )
             progress(downloaded="Decrypting", advance=100)
 
         save_dir.rmdir()
 
         progress(downloaded="Downloaded")
 
     @staticmethod
```

### Comparing `devine-3.2.0/devine/core/manifests/hls.py` & `devine-3.3.0/devine/core/manifests/hls.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pywidevine.cdm import Cdm as WidevineCdm
 from pywidevine.pssh import PSSH
 from requests import Session
 
 from devine.core.constants import DOWNLOAD_CANCELLED, DOWNLOAD_LICENCE_ONLY, AnyTrack
 from devine.core.downloaders import requests as requests_downloader
 from devine.core.drm import DRM_T, ClearKey, Widevine
+from devine.core.events import events
 from devine.core.tracks import Audio, Subtitle, Tracks, Video
 from devine.core.utilities import get_binary_path, get_extension, is_close_match, try_ensure_utf8
 
 
 class HLS:
     def __init__(self, manifest: M3U8, session: Optional[Session] = None):
         if not manifest:
@@ -278,16 +279,16 @@
             filename="{i:0%d}{ext}" % len(str(len(urls))),
             headers=session.headers,
             cookies=session.cookies,
             proxy=proxy,
             max_workers=16
         ):
             file_downloaded = status_update.get("file_downloaded")
-            if file_downloaded and callable(track.OnSegmentDownloaded):
-                track.OnSegmentDownloaded(file_downloaded)
+            if file_downloaded:
+                events.emit(events.Types.SEGMENT_DOWNLOADED, track=track, segment=file_downloaded)
             else:
                 downloaded = status_update.get("downloaded")
                 if downloaded and downloaded.endswith("/s"):
                     status_update["downloaded"] = f"HLS {downloaded}"
                 progress(**status_update)
 
         # see https://github.com/devine-dl/devine/issues/71
@@ -377,16 +378,20 @@
                     delete=True,
                     include_map_data=True
                 )
 
                 drm.decrypt(merged_path)
                 merged_path.rename(decrypted_path)
 
-                if callable(track.OnDecrypted):
-                    track.OnDecrypted(drm, decrypted_path)
+                events.emit(
+                    events.Types.TRACK_DECRYPTED,
+                    track=track,
+                    drm=drm,
+                    segment=decrypted_path
+                )
 
                 return decrypted_path
 
             def merge_discontinuity(include_this_segment: bool, include_map_data: bool = True):
                 """
                 Merge all segments of the discontinuity.
 
@@ -533,16 +538,15 @@
                         discontinuity_file.unlink()
 
         save_dir.rmdir()
 
         progress(downloaded="Downloaded")
 
         track.path = save_path
-        if callable(track.OnDownloaded):
-            track.OnDownloaded()
+        events.emit(events.Types.TRACK_DOWNLOADED, track=track)
 
     @staticmethod
     def merge_segments(segments: list[Path], save_path: Path) -> int:
         """
         Concatenate Segments by first demuxing with FFmpeg.
 
         Returns the file size of the merged file.
```

### Comparing `devine-3.2.0/devine/core/proxies/hola.py` & `devine-3.3.0/devine/core/proxies/hola.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/proxies/nordvpn.py` & `devine-3.3.0/devine/core/proxies/nordvpn.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/proxies/proxy.py` & `devine-3.3.0/devine/core/proxies/proxy.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/search_result.py` & `devine-3.3.0/devine/core/search_result.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/service.py` & `devine-3.3.0/devine/core/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import base64
 import logging
 from abc import ABCMeta, abstractmethod
 from collections.abc import Generator
 from http.cookiejar import CookieJar
+from pathlib import Path
 from typing import Optional, Union
 from urllib.parse import urlparse
 
 import click
+import m3u8
 import requests
 from requests.adapters import HTTPAdapter, Retry
 from rich.padding import Padding
 from rich.rule import Rule
 
 from devine.core.cacher import Cacher
 from devine.core.config import config
 from devine.core.console import console
 from devine.core.constants import AnyTrack
 from devine.core.credential import Credential
+from devine.core.drm import DRM_T
 from devine.core.search_result import SearchResult
 from devine.core.titles import Title_T, Titles_T
 from devine.core.tracks import Chapters, Tracks
 from devine.core.utilities import get_ip_info
 
 
 class Service(metaclass=ABCMeta):
@@ -231,9 +234,57 @@
         descriptive name for a Chapter then do not set a name at all.
 
         You must not set Chapter names to "Chapter {n}" or such. If you (or the user)
         wants "Chapter {n}" style Chapter names (or similar) then they can use the config
         option `chapter_fallback_name`. For example, `"Chapter {i:02}"` for "Chapter 01".
         """
 
+    # Optional Event methods
+
+    def on_segment_downloaded(self, track: AnyTrack, segment: Path) -> None:
+        """
+        Called when one of a Track's Segments has finished downloading.
+
+        Parameters:
+            track: The Track object that had a Segment downloaded.
+            segment: The Path to the Segment that was downloaded.
+        """
+
+    def on_track_downloaded(self, track: AnyTrack) -> None:
+        """
+        Called when a Track has finished downloading.
+
+        Parameters:
+            track: The Track object that was downloaded.
+        """
+
+    def on_track_decrypted(self, track: AnyTrack, drm: DRM_T, segment: Optional[m3u8.Segment] = None) -> None:
+        """
+        Called when a Track has finished decrypting.
+
+        Parameters:
+            track: The Track object that was decrypted.
+            drm: The DRM object it decrypted with.
+            segment: The HLS segment information that was decrypted.
+        """
+
+    def on_track_repacked(self, track: AnyTrack) -> None:
+        """
+        Called when a Track has finished repacking.
+
+        Parameters:
+            track: The Track object that was repacked.
+        """
+
+    def on_track_multiplex(self, track: AnyTrack) -> None:
+        """
+        Called when a Track is about to be Multiplexed into a Container.
+
+        Note: Right now only MKV containers are multiplexed but in the future
+        this may also be called when multiplexing to other containers like
+        MP4 via ffmpeg/mp4box.
+
+        Parameters:
+            track: The Track object that was repacked.
+        """
 
 __all__ = ("Service",)
```

### Comparing `devine-3.2.0/devine/core/services.py` & `devine-3.3.0/devine/core/services.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/titles/episode.py` & `devine-3.3.0/devine/core/titles/episode.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/titles/movie.py` & `devine-3.3.0/devine/core/titles/movie.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/titles/song.py` & `devine-3.3.0/devine/core/titles/song.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/titles/title.py` & `devine-3.3.0/devine/core/titles/title.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/tracks/audio.py` & `devine-3.3.0/devine/core/tracks/audio.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/tracks/chapter.py` & `devine-3.3.0/devine/core/tracks/chapter.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/tracks/chapters.py` & `devine-3.3.0/devine/core/tracks/chapters.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/tracks/subtitle.py` & `devine-3.3.0/devine/core/tracks/subtitle.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/tracks/track.py` & `devine-3.3.0/devine/core/tracks/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from enum import Enum
 from functools import partial
 from pathlib import Path
 from typing import Any, Callable, Iterable, Optional, Union
 from uuid import UUID
 from zlib import crc32
 
-import m3u8
 from langcodes import Language
 from requests import Session
 
 from devine.core.config import config
 from devine.core.constants import DOWNLOAD_CANCELLED, DOWNLOAD_LICENCE_ONLY
 from devine.core.downloaders import aria2c, curl_impersonate, requests
 from devine.core.drm import DRM_T, Widevine
+from devine.core.events import events
 from devine.core.utilities import get_binary_path, get_boxes, try_ensure_utf8
 from devine.core.utils.subprocess import ffprobe
 
 
 class Track:
     class Descriptor(Enum):
         URL = 1  # Direct URL, nothing fancy
@@ -118,25 +118,14 @@
             id_ = hex(checksum)[2:]
 
         self.id = id_
 
         # TODO: Currently using OnFoo event naming, change to just segment_filter
         self.OnSegmentFilter: Optional[Callable] = None
 
-        # Called after one of the Track's segments have downloaded
-        self.OnSegmentDownloaded: Optional[Callable[[Path], None]] = None
-        # Called after the Track has downloaded
-        self.OnDownloaded: Optional[Callable] = None
-        # Called after the Track or one of its segments have been decrypted
-        self.OnDecrypted: Optional[Callable[[DRM_T, Optional[m3u8.Segment]], None]] = None
-        # Called after the Track has been repackaged
-        self.OnRepacked: Optional[Callable] = None
-        # Called before the Track is multiplexed
-        self.OnMultiplex: Optional[Callable] = None
-
     def __repr__(self) -> str:
         return "{name}({items})".format(
             name=self.__class__.__name__,
             items=", ".join([f"{k}={repr(v)}" for k, v in self.__dict__.items()])
         )
 
     def __eq__(self, other: Any) -> bool:
@@ -253,23 +242,26 @@
                             if not file_downloaded:
                                 progress(**status_update)
 
                         # see https://github.com/devine-dl/devine/issues/71
                         save_path.with_suffix(f"{save_path.suffix}.aria2__temp").unlink(missing_ok=True)
 
                         self.path = save_path
-                        if callable(self.OnDownloaded):
-                            self.OnDownloaded()
+                        events.emit(events.Types.TRACK_DOWNLOADED, track=self)
 
                         if drm:
                             progress(downloaded="Decrypting", completed=0, total=100)
                             drm.decrypt(save_path)
                             self.drm = None
-                            if callable(self.OnDecrypted):
-                                self.OnDecrypted(drm)
+                            events.emit(
+                                events.Types.TRACK_DECRYPTED,
+                                track=self,
+                                drm=drm,
+                                segment=None
+                            )
                             progress(downloaded="Decrypted", completed=100)
 
                         if track_type == "Subtitle" and self.codec.name not in ("fVTT", "fTTML"):
                             track_data = self.path.read_bytes()
                             track_data = try_ensure_utf8(track_data)
                             track_data = track_data.decode("utf8"). \
                                 replace("&lrm;", html.unescape("&lrm;")). \
@@ -295,16 +287,15 @@
             # we stopped during the download, let's exit
             return
 
         if not DOWNLOAD_LICENCE_ONLY.is_set():
             if self.path.stat().st_size <= 3:  # Empty UTF-8 BOM == 3 bytes
                 raise IOError("Download failed, the downloaded file is empty.")
 
-        if callable(self.OnDownloaded):
-            self.OnDownloaded(self)
+        events.emit(events.Types.TRACK_DOWNLOADED, track=self)
 
     def delete(self) -> None:
         if self.path:
             self.path.unlink()
             self.path = None
 
     def move(self, target: Union[Path, str]) -> Path:
```

### Comparing `devine-3.2.0/devine/core/tracks/tracks.py` & `devine-3.3.0/devine/core/tracks/tracks.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,54 +10,72 @@
 from rich.progress import BarColumn, Progress, SpinnerColumn, TextColumn, TimeRemainingColumn
 from rich.table import Table
 from rich.tree import Tree
 
 from devine.core.config import config
 from devine.core.console import console
 from devine.core.constants import LANGUAGE_MAX_DISTANCE, AnyTrack, TrackT
+from devine.core.events import events
+from devine.core.tracks.attachment import Attachment
 from devine.core.tracks.audio import Audio
 from devine.core.tracks.chapters import Chapter, Chapters
 from devine.core.tracks.subtitle import Subtitle
 from devine.core.tracks.track import Track
 from devine.core.tracks.video import Video
 from devine.core.utilities import is_close_match, sanitize_filename
 from devine.core.utils.collections import as_list, flatten
 
 
 class Tracks:
     """
-    Video, Audio, Subtitle, and Chapter Track Store.
+    Video, Audio, Subtitle, Chapter, and Attachment Track Store.
     It provides convenience functions for listing, sorting, and selecting tracks.
     """
 
     TRACK_ORDER_MAP = {
         Video: 0,
         Audio: 1,
         Subtitle: 2,
-        Chapter: 3
+        Chapter: 3,
+        Attachment: 4
     }
 
-    def __init__(self, *args: Union[Tracks, Sequence[Union[AnyTrack, Chapter, Chapters]], Track, Chapter, Chapters]):
+    def __init__(self, *args: Union[
+        Tracks,
+        Sequence[Union[AnyTrack, Chapter, Chapters, Attachment]],
+        Track,
+        Chapter,
+        Chapters,
+        Attachment
+    ]):
         self.videos: list[Video] = []
         self.audio: list[Audio] = []
         self.subtitles: list[Subtitle] = []
         self.chapters = Chapters()
+        self.attachments: list[Attachment] = []
 
         if args:
             self.add(args)
 
     def __iter__(self) -> Iterator[AnyTrack]:
         return iter(as_list(self.videos, self.audio, self.subtitles))
 
     def __len__(self) -> int:
         return len(self.videos) + len(self.audio) + len(self.subtitles)
 
     def __add__(
         self,
-        other: Union[Tracks, Sequence[Union[AnyTrack, Chapter, Chapters]], Track, Chapter, Chapters]
+        other: Union[
+            Tracks,
+            Sequence[Union[AnyTrack, Chapter, Chapters, Attachment]],
+            Track,
+            Chapter,
+            Chapters,
+            Attachment
+        ]
     ) -> Tracks:
         self.add(other)
         return self
 
     def __repr__(self) -> str:
         return "{name}({items})".format(
             name=self.__class__.__name__,
@@ -65,15 +83,16 @@
         )
 
     def __str__(self) -> str:
         rep = {
             Video: [],
             Audio: [],
             Subtitle: [],
-            Chapter: []
+            Chapter: [],
+            Attachment: []
         }
         tracks = [*list(self), *self.chapters]
 
         for track in sorted(tracks, key=lambda t: self.TRACK_ORDER_MAP[type(t)]):
             if not rep[type(track)]:
                 count = sum(type(x) is type(track) for x in tracks)
                 rep[type(track)].append("{count} {type} Track{plural}{colon}".format(
@@ -94,28 +113,28 @@
                 [f"└─ {rep[type_][-1]}"]
             )
         rep = "\n".join(list(rep.values()))
 
         return rep
 
     def tree(self, add_progress: bool = False) -> tuple[Tree, list[partial]]:
-        all_tracks = [*list(self), *self.chapters]
+        all_tracks = [*list(self), *self.chapters, *self.attachments]
 
         progress_callables = []
 
         tree = Tree("", hide_root=True)
         for track_type in self.TRACK_ORDER_MAP:
             tracks = list(x for x in all_tracks if isinstance(x, track_type))
             if not tracks:
                 continue
             num_tracks = len(tracks)
             track_type_plural = track_type.__name__ + ("s" if track_type != Audio and num_tracks != 1 else "")
             tracks_tree = tree.add(f"[repr.number]{num_tracks}[/] {track_type_plural}")
             for track in tracks:
-                if add_progress and track_type != Chapter:
+                if add_progress and track_type not in (Chapter, Attachment):
                     progress = Progress(
                         SpinnerColumn(finished_text=""),
                         BarColumn(),
                         "•",
                         TimeRemainingColumn(compact=True, elapsed_when_finished=True),
                         "•",
                         TextColumn("[progress.data.speed]{task.fields[downloaded]}"),
@@ -139,20 +158,27 @@
             return any(x.id == by_id for x in self)
         if by_url:
             return any(x.url == by_url for x in self)
         return False
 
     def add(
         self,
-        tracks: Union[Tracks, Sequence[Union[AnyTrack, Chapter, Chapters]], Track, Chapter, Chapters],
+        tracks: Union[
+            Tracks,
+            Sequence[Union[AnyTrack, Chapter, Chapters, Attachment]],
+            Track,
+            Chapter,
+            Chapters,
+            Attachment
+        ],
         warn_only: bool = False
     ) -> None:
         """Add a provided track to its appropriate array and ensuring it's not a duplicate."""
         if isinstance(tracks, Tracks):
-            tracks = [*list(tracks), *tracks.chapters]
+            tracks = [*list(tracks), *tracks.chapters, *tracks.attachments]
 
         duplicates = 0
         for track in flatten(tracks):
             if self.exists(by_id=track.id):
                 if not warn_only:
                     raise ValueError(
                         "One or more of the provided Tracks is a duplicate. "
@@ -169,14 +195,16 @@
                 self.videos.append(track)
             elif isinstance(track, Audio):
                 self.audio.append(track)
             elif isinstance(track, Subtitle):
                 self.subtitles.append(track)
             elif isinstance(track, Chapter):
                 self.chapters.add(track)
+            elif isinstance(track, Attachment):
+                self.attachments.append(track)
             else:
                 raise ValueError("Track type was not set or is invalid.")
 
         log = logging.getLogger("Tracks")
 
         if duplicates:
             log.warning(f" - Found and skipped {duplicates} duplicate tracks...")
@@ -306,44 +334,41 @@
 
         if config.muxing.get("set_title", True):
             cl.extend(["--title", title])
 
         for i, vt in enumerate(self.videos):
             if not vt.path or not vt.path.exists():
                 raise ValueError("Video Track must be downloaded before muxing...")
-            if callable(vt.OnMultiplex):
-                vt.OnMultiplex()
+            events.emit(events.Types.TRACK_MULTIPLEX, track=vt)
             cl.extend([
                 "--language", f"0:{vt.language}",
                 "--default-track", f"0:{i == 0}",
                 "--original-flag", f"0:{vt.is_original_lang}",
                 "--compression", "0:none",  # disable extra compression
                 "(", str(vt.path), ")"
             ])
 
         for i, at in enumerate(self.audio):
             if not at.path or not at.path.exists():
                 raise ValueError("Audio Track must be downloaded before muxing...")
-            if callable(at.OnMultiplex):
-                at.OnMultiplex()
+            events.emit(events.Types.TRACK_MULTIPLEX, track=at)
             cl.extend([
                 "--track-name", f"0:{at.get_track_name() or ''}",
                 "--language", f"0:{at.language}",
                 "--default-track", f"0:{i == 0}",
                 "--visual-impaired-flag", f"0:{at.descriptive}",
                 "--original-flag", f"0:{at.is_original_lang}",
                 "--compression", "0:none",  # disable extra compression
                 "(", str(at.path), ")"
             ])
 
         for st in self.subtitles:
             if not st.path or not st.path.exists():
                 raise ValueError("Text Track must be downloaded before muxing...")
-            if callable(st.OnMultiplex):
-                st.OnMultiplex()
+            events.emit(events.Types.TRACK_MULTIPLEX, track=st)
             default = bool(self.audio and is_close_match(st.language, [self.audio[0].language]) and st.forced)
             cl.extend([
                 "--track-name", f"0:{st.get_track_name() or ''}",
                 "--language", f"0:{st.language}",
                 "--sub-charset", "0:UTF-8",
                 "--forced-track", f"0:{st.forced}",
                 "--default-track", f"0:{default}",
@@ -359,14 +384,24 @@
                 random=self.chapters.id
             )
             self.chapters.dump(chapters_path, fallback_name=config.chapter_fallback_name)
             cl.extend(["--chapter-charset", "UTF-8", "--chapters", str(chapters_path)])
         else:
             chapters_path = None
 
+        for attachment in self.attachments:
+            if not attachment.path or not attachment.path.exists():
+                raise ValueError("Attachment File was not found...")
+            cl.extend([
+                "--attachment-description", attachment.description or "",
+                "--attachment-mime-type", attachment.mime_type,
+                "--attachment-name", attachment.name,
+                "--attach-file", str(attachment.path.resolve())
+            ])
+
         output_path = (
             self.videos[0].path.with_suffix(".muxed.mkv") if self.videos else
             self.audio[0].path.with_suffix(".muxed.mka") if self.audio else
             self.subtitles[0].path.with_suffix(".muxed.mks") if self.subtitles else
             chapters_path.with_suffix(".muxed.mkv") if self.chapters else
             None
         )
```

### Comparing `devine-3.2.0/devine/core/tracks/video.py` & `devine-3.3.0/devine/core/tracks/video.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/utilities.py` & `devine-3.3.0/devine/core/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -273,14 +273,35 @@
 
     if value_parsed.path:
         ext = os.path.splitext(value_parsed.path)[1]
         if ext and ext != ".":
             return ext
 
 
+def get_system_fonts() -> dict[str, Path]:
+    if sys.platform == "win32":
+        import winreg
+        with winreg.ConnectRegistry(None, winreg.HKEY_LOCAL_MACHINE) as reg:
+            key = winreg.OpenKey(
+                reg,
+                r"SOFTWARE\Microsoft\Windows NT\CurrentVersion\Fonts",
+                0,
+                winreg.KEY_READ
+            )
+            total_fonts = winreg.QueryInfoKey(key)[1]
+            return {
+                name.replace(" (TrueType)", ""): Path(r"C:\Windows\Fonts", filename)
+                for n in range(0, total_fonts)
+                for name, filename, _ in [winreg.EnumValue(key, n)]
+            }
+    else:
+        # TODO: Get System Fonts for Linux and mac OS
+        return {}
+
+
 class FPS(ast.NodeVisitor):
     def visit_BinOp(self, node: ast.BinOp) -> float:
         if isinstance(node.op, ast.Div):
             return self.visit(node.left) / self.visit(node.right)
         raise ValueError(f"Invalid operation: {node.op}")
 
     def visit_Num(self, node: ast.Num) -> complex:
```

### Comparing `devine-3.2.0/devine/core/utils/click_types.py` & `devine-3.3.0/devine/core/utils/click_types.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/utils/collections.py` & `devine-3.3.0/devine/core/utils/collections.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/utils/sslciphers.py` & `devine-3.3.0/devine/core/utils/sslciphers.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/utils/subprocess.py` & `devine-3.3.0/devine/core/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/utils/xml.py` & `devine-3.3.0/devine/core/utils/xml.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/vault.py` & `devine-3.3.0/devine/core/vault.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/core/vaults.py` & `devine-3.3.0/devine/core/vaults.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/vaults/API.py` & `devine-3.3.0/devine/vaults/API.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/vaults/MySQL.py` & `devine-3.3.0/devine/vaults/MySQL.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/devine/vaults/SQLite.py` & `devine-3.3.0/devine/vaults/SQLite.py`

 * *Files identical despite different names*

### Comparing `devine-3.2.0/pyproject.toml` & `devine-3.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "devine"
-version = "3.2.0"
+version = "3.3.0"
 description = "Modular Movie, TV, and Music Archival Software."
 license = "GPL-3.0-only"
 authors = ["rlaphoenix <rlaphoenix@pm.me>"]
 readme = "README.md"
 homepage = "https://github.com/devine-dl/devine"
 repository = "https://github.com/devine-dl/devine"
 keywords = ["python", "downloader", "drm", "widevine"]
@@ -37,15 +37,15 @@
 appdirs = "^1.4.4"
 Brotli = "^1.1.0"
 click = "^8.1.7"
 construct = "^2.8.8"
 crccheck = "^1.3.0"
 jsonpickle = "^3.0.3"
 langcodes = { extras = ["data"], version = "^3.3.0" }
-lxml = "^5.1.0"
+lxml = "^5.2.1"
 pproxy = "^2.7.9"
 protobuf = "^4.25.3"
 pycaption = "^2.2.4"
 pycryptodomex = "^3.20.0"
 pyjwt = "^2.8.0"
 pymediainfo = "^6.1.0"
 pymp4 = "^1.4.0"
@@ -66,20 +66,20 @@
 # uses marisa-trie v0.7.8 which doesn't have Python 3.12 wheels.
 language-data = "^1.2.0.dev3"
 marisa-trie = "^1.1.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^3.7.0"
 mypy = "^1.9.0"
-mypy-protobuf = "^3.5.0"
+mypy-protobuf = "^3.6.0"
 types-protobuf = "^4.24.0.20240311"
 types-PyMySQL = "^1.1.0.1"
-types-requests = "^2.31.0.20240311"
+types-requests = "^2.31.0.20240402"
 isort = "^5.13.2"
-ruff = "~0.3.4"
+ruff = "~0.3.5"
 
 [tool.poetry.scripts]
 devine = "devine.core.__main__:main"
 
 [tool.ruff]
 force-exclude = true
 line-length = 120
```

### Comparing `devine-3.2.0/PKG-INFO` & `devine-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devine
-Version: 3.2.0
+Version: 3.3.0
 Summary: Modular Movie, TV, and Music Archival Software.
 Home-page: https://github.com/devine-dl/devine
 License: GPL-3.0-only
 Keywords: python,downloader,drm,widevine
 Author: rlaphoenix
 Author-email: rlaphoenix@pm.me
 Requires-Python: >=3.9,<4.0
@@ -28,15 +28,15 @@
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: construct (>=2.8.8,<3.0.0)
 Requires-Dist: crccheck (>=1.3.0,<2.0.0)
 Requires-Dist: curl-cffi (>=0.6.2,<0.7.0)
 Requires-Dist: jsonpickle (>=3.0.3,<4.0.0)
 Requires-Dist: langcodes[data] (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.2.0.dev3,<2.0.0)
-Requires-Dist: lxml (>=5.1.0,<6.0.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: marisa-trie (>=1.1.0,<2.0.0)
 Requires-Dist: pproxy (>=2.7.9,<3.0.0)
 Requires-Dist: protobuf (>=4.25.3,<5.0.0)
 Requires-Dist: pycaption (>=2.2.4,<3.0.0)
 Requires-Dist: pycryptodomex (>=3.20.0,<4.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: pymediainfo (>=6.1.0,<7.0.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: devine Version: 3.2.0 Summary: Modular Movie, TV,
+Metadata-Version: 2.1 Name: devine Version: 3.3.0 Summary: Modular Movie, TV,
 and Music Archival Software. Home-page: https://github.com/devine-dl/devine
 License: GPL-3.0-only Keywords: python,downloader,drm,widevine Author:
 rlaphoenix Author-email: rlaphoenix@pm.me Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
@@ -12,15 +12,15 @@
 Classifier: Topic :: Security :: Cryptography Requires-Dist: Brotli
 (>=1.1.0,<2.0.0) Requires-Dist: PyYAML (>=6.0.1,<7.0.0) Requires-Dist:
 Unidecode (>=1.3.8,<2.0.0) Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-
 Dist: chardet (>=5.2.0,<6.0.0) Requires-Dist: click (>=8.1.7,<9.0.0) Requires-
 Dist: construct (>=2.8.8,<3.0.0) Requires-Dist: crccheck (>=1.3.0,<2.0.0)
 Requires-Dist: curl-cffi (>=0.6.2,<0.7.0) Requires-Dist: jsonpickle
 (>=3.0.3,<4.0.0) Requires-Dist: langcodes[data] (>=3.3.0,<4.0.0) Requires-Dist:
-language-data (>=1.2.0.dev3,<2.0.0) Requires-Dist: lxml (>=5.1.0,<6.0.0)
+language-data (>=1.2.0.dev3,<2.0.0) Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: marisa-trie (>=1.1.0,<2.0.0) Requires-Dist: pproxy
 (>=2.7.9,<3.0.0) Requires-Dist: protobuf (>=4.25.3,<5.0.0) Requires-Dist:
 pycaption (>=2.2.4,<3.0.0) Requires-Dist: pycryptodomex (>=3.20.0,<4.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0) Requires-Dist: pymediainfo
 (>=6.1.0,<7.0.0) Requires-Dist: pymp4 (>=1.4.0,<2.0.0) Requires-Dist: pymysql
 (>=1.1.0,<2.0.0) Requires-Dist: pywidevine[serve] (>=1.8.0,<2.0.0) Requires-
 Dist: requests[socks] (>=2.31.0,<3.0.0) Requires-Dist: rich (>=13.7.1,<14.0.0)
```

