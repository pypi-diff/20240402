# Comparing `tmp/senpwai-2.1.6.tar.gz` & `tmp/senpwai-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "senpwai-2.1.6.tar", max compression
+gzip compressed data, was "senpwai-2.1.7.tar", max compression
```

## Comparing `senpwai-2.1.6.tar` & `senpwai-2.1.7.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    35823 2024-02-27 02:54:57.469943 senpwai-2.1.6/LICENSE
--rw-r--r--   0        0        0     4435 2024-03-11 19:11:21.833735 senpwai-2.1.6/pyproject.toml
--rw-r--r--   0        0        0     6465 2024-02-27 02:54:57.471939 senpwai-2.1.6/README.md
--rw-r--r--   0        0        0        0 2024-02-27 02:54:57.615906 senpwai-2.1.6/senpwai/__init__.py
--rw-r--r--   0        0        0       73 2024-02-27 02:54:57.616904 senpwai-2.1.6/senpwai/__main__.py
--rw-r--r--   0        0        0   167773 2024-02-27 02:54:57.620926 senpwai-2.1.6/senpwai/assets/audio/aqua-crying.mp3
--rw-r--r--   0        0        0    28037 2024-02-27 02:54:57.621905 senpwai-2.1.6/senpwai/assets/audio/bunshin-poof.mp3
--rw-r--r--   0        0        0   257620 2024-02-27 02:54:57.625930 senpwai-2.1.6/senpwai/assets/audio/gigachad.mp3
--rw-r--r--   0        0        0    45701 2024-02-27 02:54:57.628908 senpwai-2.1.6/senpwai/assets/audio/kage-bunshin-no-jutsu.mp3
--rw-r--r--   0        0        0    38481 2024-02-27 02:54:57.630908 senpwai-2.1.6/senpwai/assets/audio/merry-chrismasu.mp3
--rw-r--r--   0        0        0    91267 2024-02-27 02:54:57.632906 senpwai-2.1.6/senpwai/assets/audio/morbin-time.mp3
--rw-r--r--   0        0        0   230876 2024-02-27 02:54:57.636908 senpwai-2.1.6/senpwai/assets/audio/one-piece-real-1.mp3
--rw-r--r--   0        0        0   184032 2024-02-27 02:54:57.639940 senpwai-2.1.6/senpwai/assets/audio/one-piece-real-2.mp3
--rw-r--r--   0        0        0   132304 2024-02-27 02:54:57.642941 senpwai-2.1.6/senpwai/assets/audio/sen-favourite.wav
--rw-r--r--   0        0        0    48659 2024-02-27 02:54:57.645909 senpwai-2.1.6/senpwai/assets/audio/toki-wa-ugoki-dasu.mp3
--rw-r--r--   0        0        0   348653 2024-02-27 02:54:57.653909 senpwai-2.1.6/senpwai/assets/audio/what-da-hell.mp3
--rw-r--r--   0        0        0   463516 2024-02-27 02:54:57.664911 senpwai-2.1.6/senpwai/assets/audio/za-warudo.mp3
--rw-r--r--   0        0        0   348902 2024-02-27 02:54:57.671911 senpwai-2.1.6/senpwai/assets/background-images/about.jpg
--rw-r--r--   0        0        0   617045 2024-02-27 02:54:57.681432 senpwai-2.1.6/senpwai/assets/background-images/chopper-crying.png
--rw-r--r--   0        0        0   392654 2024-02-27 02:54:57.688431 senpwai-2.1.6/senpwai/assets/background-images/chosen-anime.jpg
--rw-r--r--   0        0        0   172353 2024-02-27 02:54:57.692430 senpwai-2.1.6/senpwai/assets/background-images/christmas.jpg
--rw-r--r--   0        0        0   884962 2024-02-27 02:54:57.703431 senpwai-2.1.6/senpwai/assets/background-images/downloads.png
--rw-r--r--   0        0        0   357703 2024-02-27 02:54:57.709432 senpwai-2.1.6/senpwai/assets/background-images/search.jpg
--rw-r--r--   0        0        0   247094 2024-02-27 02:54:57.714432 senpwai-2.1.6/senpwai/assets/background-images/settings.jpg
--rw-r--r--   0        0        0   405642 2024-02-27 02:54:57.721432 senpwai-2.1.6/senpwai/assets/background-images/update.jpg
--rw-r--r--   0        0        0     1227 2024-02-27 02:54:57.722432 senpwai-2.1.6/senpwai/assets/download-icons/cancel.png
--rw-r--r--   0        0        0      757 2024-02-27 02:54:57.723432 senpwai-2.1.6/senpwai/assets/download-icons/down.png
--rw-r--r--   0        0        0      694 2024-02-27 02:54:57.724431 senpwai-2.1.6/senpwai/assets/download-icons/pause.png
--rw-r--r--   0        0        0      920 2024-02-27 02:54:57.725432 senpwai-2.1.6/senpwai/assets/download-icons/resume.png
--rw-r--r--   0        0        0      781 2024-02-27 02:54:57.726437 senpwai-2.1.6/senpwai/assets/download-icons/trash.png
--rw-r--r--   0        0        0      641 2024-02-27 02:54:57.727433 senpwai-2.1.6/senpwai/assets/download-icons/up.png
--rw-r--r--   0        0        0    27409 2024-02-27 02:54:57.729464 senpwai-2.1.6/senpwai/assets/link-icons/discord.png
--rw-r--r--   0        0        0    16226 2024-02-27 02:54:57.730425 senpwai-2.1.6/senpwai/assets/link-icons/github-sponsors.svg
--rw-r--r--   0        0        0    22763 2024-02-27 02:54:57.731426 senpwai-2.1.6/senpwai/assets/link-icons/github.png
--rw-r--r--   0        0        0    17064 2024-02-27 02:54:57.732430 senpwai-2.1.6/senpwai/assets/link-icons/patreon.png
--rw-r--r--   0        0        0    35215 2024-02-27 02:54:57.734432 senpwai-2.1.6/senpwai/assets/link-icons/reddit.png
--rw-r--r--   0        0        0    49259 2024-02-27 02:54:57.736432 senpwai-2.1.6/senpwai/assets/mascots/1.png
--rw-r--r--   0        0        0    69802 2024-02-27 02:54:57.739434 senpwai-2.1.6/senpwai/assets/mascots/2.png
--rw-r--r--   0        0        0     4258 2024-02-27 02:54:57.740433 senpwai-2.1.6/senpwai/assets/misc/folder.png
--rw-r--r--   0        0        0   625301 2024-02-27 02:54:57.754464 senpwai-2.1.6/senpwai/assets/misc/loading.gif
--rw-r--r--   0        0        0    89481 2024-02-27 02:54:57.757459 senpwai-2.1.6/senpwai/assets/misc/sadge-piece.gif
--rw-r--r--   0        0        0    99300 2024-02-27 02:54:57.760429 senpwai-2.1.6/senpwai/assets/misc/senpwai-icon.ico
--rw-r--r--   0        0        0     8044 2024-02-27 02:54:57.761438 senpwai-2.1.6/senpwai/assets/misc/task-complete.png
--rw-r--r--   0        0        0    16336 2024-02-27 02:54:57.763436 senpwai-2.1.6/senpwai/assets/navigation-bar-icons/about.png
--rw-r--r--   0        0        0     7749 2024-02-27 02:54:57.764436 senpwai-2.1.6/senpwai/assets/navigation-bar-icons/downloads.png
--rw-r--r--   0        0        0    19245 2024-02-27 02:54:57.765437 senpwai-2.1.6/senpwai/assets/navigation-bar-icons/search.png
--rw-r--r--   0        0        0    10851 2024-02-27 02:54:57.767439 senpwai-2.1.6/senpwai/assets/navigation-bar-icons/settings.png
--rw-r--r--   0        0        0     6454 2024-02-27 02:54:57.768437 senpwai-2.1.6/senpwai/assets/navigation-bar-icons/update.png
--rw-r--r--   0        0        0    96597 2024-02-27 02:54:57.772439 senpwai-2.1.6/senpwai/assets/reviewer-profile-pics/hentai-addict.png
--rw-r--r--   0        0        0    19936 2024-02-27 02:54:57.773439 senpwai-2.1.6/senpwai/assets/reviewer-profile-pics/morbius-is-peak.png
--rw-r--r--   0        0        0    52908 2024-02-27 02:54:57.774438 senpwai-2.1.6/senpwai/assets/reviewer-profile-pics/sen.png
--rw-r--r--   0        0        0     1710 2024-03-05 08:24:06.852246 senpwai-2.1.6/senpwai/main.py
--rw-r--r--   0        0        0        0 2024-02-27 02:54:57.777958 senpwai-2.1.6/senpwai/scrapers/__init__.py
--rw-r--r--   0        0        0      109 2024-03-05 08:24:06.852246 senpwai-2.1.6/senpwai/scrapers/gogo/__init__.py
--rw-r--r--   0        0        0     1112 2024-03-05 08:24:06.852246 senpwai-2.1.6/senpwai/scrapers/gogo/constants.py
--rw-r--r--   0        0        0     5196 2024-02-27 02:54:57.781957 senpwai-2.1.6/senpwai/scrapers/gogo/hls.py
--rw-r--r--   0        0        0     7747 2024-03-11 02:40:02.199646 senpwai-2.1.6/senpwai/scrapers/gogo/main.py
--rw-r--r--   0        0        0       78 2024-03-05 08:24:06.852246 senpwai-2.1.6/senpwai/scrapers/pahe/__init__.py
--rw-r--r--   0        0        0     1204 2024-03-05 08:24:06.852246 senpwai-2.1.6/senpwai/scrapers/pahe/constants.py
--rw-r--r--   0        0        0    13680 2024-03-11 02:37:37.564977 senpwai-2.1.6/senpwai/scrapers/pahe/main.py
--rw-r--r--   0        0        0    29624 2024-03-05 08:24:06.852246 senpwai-2.1.6/senpwai/scrapers/test.py
--rw-r--r--   0        0        0       81 2024-02-27 02:54:57.788962 senpwai-2.1.6/senpwai/senpcli/__main__.py
--rw-r--r--   0        0        0    23020 2024-03-11 02:01:35.564503 senpwai-2.1.6/senpwai/senpcli/main.py
--rw-r--r--   0        0        0        0 2024-02-27 02:54:57.791960 senpwai-2.1.6/senpwai/utils/__init__.py
--rw-r--r--   0        0        0    14833 2024-03-05 08:24:06.852246 senpwai-2.1.6/senpwai/utils/classes.py
--rw-r--r--   0        0        0    22335 2024-03-11 03:43:58.187207 senpwai-2.1.6/senpwai/utils/scraper.py
--rw-r--r--   0        0        0     9500 2024-03-11 19:11:21.843784 senpwai-2.1.6/senpwai/utils/static.py
--rw-r--r--   0        0        0    25727 2024-03-05 08:24:06.867880 senpwai-2.1.6/senpwai/utils/widgets.py
--rw-r--r--   0        0        0        0 2024-02-27 02:54:57.800965 senpwai-2.1.6/senpwai/windows/__init__.py
--rw-r--r--   0        0        0     8097 2024-03-05 08:24:06.867880 senpwai-2.1.6/senpwai/windows/about.py
--rw-r--r--   0        0        0     2670 2024-03-05 08:24:06.867880 senpwai-2.1.6/senpwai/windows/abstracts.py
--rw-r--r--   0        0        0    20740 2024-03-05 08:24:06.867880 senpwai-2.1.6/senpwai/windows/chosen_anime.py
--rw-r--r--   0        0        0    54375 2024-03-05 08:24:06.867880 senpwai-2.1.6/senpwai/windows/download.py
--rw-r--r--   0        0        0    10393 2024-02-27 02:54:57.808959 senpwai-2.1.6/senpwai/windows/main.py
--rw-r--r--   0        0        0    11995 2024-03-05 08:24:06.867880 senpwai-2.1.6/senpwai/windows/misc.py
--rw-r--r--   0        0        0    18032 2024-03-05 08:24:06.867880 senpwai-2.1.6/senpwai/windows/search.py
--rw-r--r--   0        0        0    27126 2024-03-05 08:24:06.867880 senpwai-2.1.6/senpwai/windows/settings.py
--rw-r--r--   0        0        0     7722 1970-01-01 00:00:00.000000 senpwai-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-02-27 02:54:57.469943 senpwai-2.1.7/LICENSE
+-rw-r--r--   0        0        0     4435 2024-04-02 19:10:28.650268 senpwai-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6465 2024-02-27 02:54:57.471939 senpwai-2.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-02-27 02:54:57.615906 senpwai-2.1.7/senpwai/__init__.py
+-rw-r--r--   0        0        0       73 2024-02-27 02:54:57.616904 senpwai-2.1.7/senpwai/__main__.py
+-rw-r--r--   0        0        0   167773 2024-02-27 02:54:57.620926 senpwai-2.1.7/senpwai/assets/audio/aqua-crying.mp3
+-rw-r--r--   0        0        0    28037 2024-02-27 02:54:57.621905 senpwai-2.1.7/senpwai/assets/audio/bunshin-poof.mp3
+-rw-r--r--   0        0        0   257620 2024-02-27 02:54:57.625930 senpwai-2.1.7/senpwai/assets/audio/gigachad.mp3
+-rw-r--r--   0        0        0    45701 2024-02-27 02:54:57.628908 senpwai-2.1.7/senpwai/assets/audio/kage-bunshin-no-jutsu.mp3
+-rw-r--r--   0        0        0    38481 2024-02-27 02:54:57.630908 senpwai-2.1.7/senpwai/assets/audio/merry-chrismasu.mp3
+-rw-r--r--   0        0        0    91267 2024-02-27 02:54:57.632906 senpwai-2.1.7/senpwai/assets/audio/morbin-time.mp3
+-rw-r--r--   0        0        0   230876 2024-02-27 02:54:57.636908 senpwai-2.1.7/senpwai/assets/audio/one-piece-real-1.mp3
+-rw-r--r--   0        0        0   184032 2024-02-27 02:54:57.639940 senpwai-2.1.7/senpwai/assets/audio/one-piece-real-2.mp3
+-rw-r--r--   0        0        0   132304 2024-02-27 02:54:57.642941 senpwai-2.1.7/senpwai/assets/audio/sen-favourite.wav
+-rw-r--r--   0        0        0    48659 2024-02-27 02:54:57.645909 senpwai-2.1.7/senpwai/assets/audio/toki-wa-ugoki-dasu.mp3
+-rw-r--r--   0        0        0   348653 2024-02-27 02:54:57.653909 senpwai-2.1.7/senpwai/assets/audio/what-da-hell.mp3
+-rw-r--r--   0        0        0   463516 2024-02-27 02:54:57.664911 senpwai-2.1.7/senpwai/assets/audio/za-warudo.mp3
+-rw-r--r--   0        0        0   348902 2024-02-27 02:54:57.671911 senpwai-2.1.7/senpwai/assets/background-images/about.jpg
+-rw-r--r--   0        0        0   617045 2024-02-27 02:54:57.681432 senpwai-2.1.7/senpwai/assets/background-images/chopper-crying.png
+-rw-r--r--   0        0        0   392654 2024-02-27 02:54:57.688431 senpwai-2.1.7/senpwai/assets/background-images/chosen-anime.jpg
+-rw-r--r--   0        0        0   172353 2024-02-27 02:54:57.692430 senpwai-2.1.7/senpwai/assets/background-images/christmas.jpg
+-rw-r--r--   0        0        0   884962 2024-02-27 02:54:57.703431 senpwai-2.1.7/senpwai/assets/background-images/downloads.png
+-rw-r--r--   0        0        0   357703 2024-02-27 02:54:57.709432 senpwai-2.1.7/senpwai/assets/background-images/search.jpg
+-rw-r--r--   0        0        0   247094 2024-02-27 02:54:57.714432 senpwai-2.1.7/senpwai/assets/background-images/settings.jpg
+-rw-r--r--   0        0        0   405642 2024-02-27 02:54:57.721432 senpwai-2.1.7/senpwai/assets/background-images/update.jpg
+-rw-r--r--   0        0        0     1227 2024-02-27 02:54:57.722432 senpwai-2.1.7/senpwai/assets/download-icons/cancel.png
+-rw-r--r--   0        0        0      757 2024-02-27 02:54:57.723432 senpwai-2.1.7/senpwai/assets/download-icons/down.png
+-rw-r--r--   0        0        0      694 2024-02-27 02:54:57.724431 senpwai-2.1.7/senpwai/assets/download-icons/pause.png
+-rw-r--r--   0        0        0      920 2024-02-27 02:54:57.725432 senpwai-2.1.7/senpwai/assets/download-icons/resume.png
+-rw-r--r--   0        0        0      781 2024-02-27 02:54:57.726437 senpwai-2.1.7/senpwai/assets/download-icons/trash.png
+-rw-r--r--   0        0        0      641 2024-02-27 02:54:57.727433 senpwai-2.1.7/senpwai/assets/download-icons/up.png
+-rw-r--r--   0        0        0    27409 2024-02-27 02:54:57.729464 senpwai-2.1.7/senpwai/assets/link-icons/discord.png
+-rw-r--r--   0        0        0    16226 2024-02-27 02:54:57.730425 senpwai-2.1.7/senpwai/assets/link-icons/github-sponsors.svg
+-rw-r--r--   0        0        0    22763 2024-02-27 02:54:57.731426 senpwai-2.1.7/senpwai/assets/link-icons/github.png
+-rw-r--r--   0        0        0    17064 2024-02-27 02:54:57.732430 senpwai-2.1.7/senpwai/assets/link-icons/patreon.png
+-rw-r--r--   0        0        0    35215 2024-02-27 02:54:57.734432 senpwai-2.1.7/senpwai/assets/link-icons/reddit.png
+-rw-r--r--   0        0        0    49259 2024-02-27 02:54:57.736432 senpwai-2.1.7/senpwai/assets/mascots/1.png
+-rw-r--r--   0        0        0    69802 2024-02-27 02:54:57.739434 senpwai-2.1.7/senpwai/assets/mascots/2.png
+-rw-r--r--   0        0        0     4258 2024-02-27 02:54:57.740433 senpwai-2.1.7/senpwai/assets/misc/folder.png
+-rw-r--r--   0        0        0   625301 2024-02-27 02:54:57.754464 senpwai-2.1.7/senpwai/assets/misc/loading.gif
+-rw-r--r--   0        0        0    89481 2024-02-27 02:54:57.757459 senpwai-2.1.7/senpwai/assets/misc/sadge-piece.gif
+-rw-r--r--   0        0        0    99300 2024-02-27 02:54:57.760429 senpwai-2.1.7/senpwai/assets/misc/senpwai-icon.ico
+-rw-r--r--   0        0        0     8044 2024-02-27 02:54:57.761438 senpwai-2.1.7/senpwai/assets/misc/task-complete.png
+-rw-r--r--   0        0        0    16336 2024-02-27 02:54:57.763436 senpwai-2.1.7/senpwai/assets/navigation-bar-icons/about.png
+-rw-r--r--   0        0        0     7749 2024-02-27 02:54:57.764436 senpwai-2.1.7/senpwai/assets/navigation-bar-icons/downloads.png
+-rw-r--r--   0        0        0    19245 2024-02-27 02:54:57.765437 senpwai-2.1.7/senpwai/assets/navigation-bar-icons/search.png
+-rw-r--r--   0        0        0    10851 2024-02-27 02:54:57.767439 senpwai-2.1.7/senpwai/assets/navigation-bar-icons/settings.png
+-rw-r--r--   0        0        0     6454 2024-02-27 02:54:57.768437 senpwai-2.1.7/senpwai/assets/navigation-bar-icons/update.png
+-rw-r--r--   0        0        0    96597 2024-02-27 02:54:57.772439 senpwai-2.1.7/senpwai/assets/reviewer-profile-pics/hentai-addict.png
+-rw-r--r--   0        0        0    19936 2024-02-27 02:54:57.773439 senpwai-2.1.7/senpwai/assets/reviewer-profile-pics/morbius-is-peak.png
+-rw-r--r--   0        0        0    52908 2024-02-27 02:54:57.774438 senpwai-2.1.7/senpwai/assets/reviewer-profile-pics/sen.png
+-rw-r--r--   0        0        0     1710 2024-03-13 02:52:36.375376 senpwai-2.1.7/senpwai/main.py
+-rw-r--r--   0        0        0        0 2024-02-27 02:54:57.777958 senpwai-2.1.7/senpwai/scrapers/__init__.py
+-rw-r--r--   0        0        0      109 2024-03-05 08:24:06.852246 senpwai-2.1.7/senpwai/scrapers/gogo/__init__.py
+-rw-r--r--   0        0        0     1112 2024-03-05 08:24:06.852246 senpwai-2.1.7/senpwai/scrapers/gogo/constants.py
+-rw-r--r--   0        0        0     5196 2024-02-27 02:54:57.781957 senpwai-2.1.7/senpwai/scrapers/gogo/hls.py
+-rw-r--r--   0        0        0     7747 2024-03-11 19:14:50.991450 senpwai-2.1.7/senpwai/scrapers/gogo/main.py
+-rw-r--r--   0        0        0       78 2024-03-05 08:24:06.852246 senpwai-2.1.7/senpwai/scrapers/pahe/__init__.py
+-rw-r--r--   0        0        0     1204 2024-03-05 08:24:06.852246 senpwai-2.1.7/senpwai/scrapers/pahe/constants.py
+-rw-r--r--   0        0        0    13680 2024-04-02 19:03:05.659479 senpwai-2.1.7/senpwai/scrapers/pahe/main.py
+-rw-r--r--   0        0        0    29624 2024-04-02 18:25:35.009961 senpwai-2.1.7/senpwai/scrapers/test.py
+-rw-r--r--   0        0        0       81 2024-02-27 02:54:57.788962 senpwai-2.1.7/senpwai/senpcli/__main__.py
+-rw-r--r--   0        0        0    23020 2024-03-11 19:14:50.992450 senpwai-2.1.7/senpwai/senpcli/main.py
+-rw-r--r--   0        0        0        0 2024-02-27 02:54:57.791960 senpwai-2.1.7/senpwai/utils/__init__.py
+-rw-r--r--   0        0        0    14833 2024-03-05 08:24:06.852246 senpwai-2.1.7/senpwai/utils/classes.py
+-rw-r--r--   0        0        0    22603 2024-04-02 19:03:15.489710 senpwai-2.1.7/senpwai/utils/scraper.py
+-rw-r--r--   0        0        0     9500 2024-04-02 19:10:28.652272 senpwai-2.1.7/senpwai/utils/static.py
+-rw-r--r--   0        0        0    25727 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/utils/widgets.py
+-rw-r--r--   0        0        0        0 2024-02-27 02:54:57.800965 senpwai-2.1.7/senpwai/windows/__init__.py
+-rw-r--r--   0        0        0     8097 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/about.py
+-rw-r--r--   0        0        0     2670 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/abstracts.py
+-rw-r--r--   0        0        0    20740 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/chosen_anime.py
+-rw-r--r--   0        0        0    54375 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/download.py
+-rw-r--r--   0        0        0    10393 2024-02-27 02:54:57.808959 senpwai-2.1.7/senpwai/windows/main.py
+-rw-r--r--   0        0        0    11995 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/misc.py
+-rw-r--r--   0        0        0    18032 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/search.py
+-rw-r--r--   0        0        0    27126 2024-03-05 08:24:06.867880 senpwai-2.1.7/senpwai/windows/settings.py
+-rw-r--r--   0        0        0     7722 1970-01-01 00:00:00.000000 senpwai-2.1.7/PKG-INFO
```

### Comparing `senpwai-2.1.6/LICENSE` & `senpwai-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/pyproject.toml` & `senpwai-2.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "senpwai"
-version = "2.1.6"
+version = "2.1.7"
 description = "A desktop app for tracking and batch downloading anime"
 authors = ["SenZmaKi <senzmaki@gmail.com>"]
 license = "GPL v3"
 readme = "README.md"
 include = ["senpwai/assets"]
 packages = [{ include = "senpwai" }, { include = "senpcli", from = "senpwai" }]
 exclude = ["src/**/test.py"]
```

### Comparing `senpwai-2.1.6/README.md` & `senpwai-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/audio/aqua-crying.mp3` & `senpwai-2.1.7/senpwai/assets/audio/aqua-crying.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/audio/bunshin-poof.mp3` & `senpwai-2.1.7/senpwai/assets/audio/bunshin-poof.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/audio/gigachad.mp3` & `senpwai-2.1.7/senpwai/assets/audio/gigachad.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/audio/kage-bunshin-no-jutsu.mp3` & `senpwai-2.1.7/senpwai/assets/audio/kage-bunshin-no-jutsu.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/audio/merry-chrismasu.mp3` & `senpwai-2.1.7/senpwai/assets/audio/merry-chrismasu.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/audio/morbin-time.mp3` & `senpwai-2.1.7/senpwai/assets/audio/morbin-time.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/audio/one-piece-real-1.mp3` & `senpwai-2.1.7/senpwai/assets/audio/one-piece-real-1.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/audio/one-piece-real-2.mp3` & `senpwai-2.1.7/senpwai/assets/audio/one-piece-real-2.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/audio/sen-favourite.wav` & `senpwai-2.1.7/senpwai/assets/audio/sen-favourite.wav`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/audio/toki-wa-ugoki-dasu.mp3` & `senpwai-2.1.7/senpwai/assets/audio/toki-wa-ugoki-dasu.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/audio/what-da-hell.mp3` & `senpwai-2.1.7/senpwai/assets/audio/what-da-hell.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/audio/za-warudo.mp3` & `senpwai-2.1.7/senpwai/assets/audio/za-warudo.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/background-images/about.jpg` & `senpwai-2.1.7/senpwai/assets/background-images/about.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/background-images/chopper-crying.png` & `senpwai-2.1.7/senpwai/assets/background-images/chopper-crying.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/background-images/chosen-anime.jpg` & `senpwai-2.1.7/senpwai/assets/background-images/chosen-anime.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/background-images/christmas.jpg` & `senpwai-2.1.7/senpwai/assets/background-images/christmas.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/background-images/downloads.png` & `senpwai-2.1.7/senpwai/assets/background-images/downloads.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/background-images/search.jpg` & `senpwai-2.1.7/senpwai/assets/background-images/search.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/background-images/settings.jpg` & `senpwai-2.1.7/senpwai/assets/background-images/settings.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/background-images/update.jpg` & `senpwai-2.1.7/senpwai/assets/background-images/update.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/download-icons/cancel.png` & `senpwai-2.1.7/senpwai/assets/download-icons/cancel.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/download-icons/down.png` & `senpwai-2.1.7/senpwai/assets/download-icons/down.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/download-icons/pause.png` & `senpwai-2.1.7/senpwai/assets/download-icons/pause.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/download-icons/resume.png` & `senpwai-2.1.7/senpwai/assets/download-icons/resume.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/download-icons/trash.png` & `senpwai-2.1.7/senpwai/assets/download-icons/trash.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/download-icons/up.png` & `senpwai-2.1.7/senpwai/assets/download-icons/up.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/link-icons/discord.png` & `senpwai-2.1.7/senpwai/assets/link-icons/discord.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/link-icons/github-sponsors.svg` & `senpwai-2.1.7/senpwai/assets/link-icons/github-sponsors.svg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/link-icons/github.png` & `senpwai-2.1.7/senpwai/assets/link-icons/github.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/link-icons/patreon.png` & `senpwai-2.1.7/senpwai/assets/link-icons/patreon.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/link-icons/reddit.png` & `senpwai-2.1.7/senpwai/assets/link-icons/reddit.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/mascots/1.png` & `senpwai-2.1.7/senpwai/assets/mascots/1.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/mascots/2.png` & `senpwai-2.1.7/senpwai/assets/mascots/2.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/misc/folder.png` & `senpwai-2.1.7/senpwai/assets/misc/folder.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/misc/loading.gif` & `senpwai-2.1.7/senpwai/assets/misc/loading.gif`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/misc/sadge-piece.gif` & `senpwai-2.1.7/senpwai/assets/misc/sadge-piece.gif`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/misc/senpwai-icon.ico` & `senpwai-2.1.7/senpwai/assets/misc/senpwai-icon.ico`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/misc/task-complete.png` & `senpwai-2.1.7/senpwai/assets/misc/task-complete.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/navigation-bar-icons/about.png` & `senpwai-2.1.7/senpwai/assets/navigation-bar-icons/about.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/navigation-bar-icons/downloads.png` & `senpwai-2.1.7/senpwai/assets/navigation-bar-icons/downloads.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/navigation-bar-icons/search.png` & `senpwai-2.1.7/senpwai/assets/navigation-bar-icons/search.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/navigation-bar-icons/settings.png` & `senpwai-2.1.7/senpwai/assets/navigation-bar-icons/settings.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/navigation-bar-icons/update.png` & `senpwai-2.1.7/senpwai/assets/navigation-bar-icons/update.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/reviewer-profile-pics/hentai-addict.png` & `senpwai-2.1.7/senpwai/assets/reviewer-profile-pics/hentai-addict.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/reviewer-profile-pics/morbius-is-peak.png` & `senpwai-2.1.7/senpwai/assets/reviewer-profile-pics/morbius-is-peak.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/assets/reviewer-profile-pics/sen.png` & `senpwai-2.1.7/senpwai/assets/reviewer-profile-pics/sen.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/main.py` & `senpwai-2.1.7/senpwai/main.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/scrapers/gogo/constants.py` & `senpwai-2.1.7/senpwai/scrapers/gogo/constants.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/scrapers/gogo/hls.py` & `senpwai-2.1.7/senpwai/scrapers/gogo/hls.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/scrapers/gogo/main.py` & `senpwai-2.1.7/senpwai/scrapers/gogo/main.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/scrapers/pahe/constants.py` & `senpwai-2.1.7/senpwai/scrapers/pahe/constants.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/scrapers/pahe/main.py` & `senpwai-2.1.7/senpwai/scrapers/pahe/main.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/scrapers/test.py` & `senpwai-2.1.7/senpwai/scrapers/test.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/senpcli/main.py` & `senpwai-2.1.7/senpwai/senpcli/main.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/utils/classes.py` & `senpwai-2.1.7/senpwai/utils/classes.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/utils/scraper.py` & `senpwai-2.1.7/senpwai/utils/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,14 +363,17 @@
 
 def lacked_episodes(
     lacking_episode_numbers: list[int], episode_page_links: list[str]
 ) -> list[str]:
     # Episode count is what is used to generate lacking_episode_numbers, episode count is gotten from anime the page which uses subbed episodes count
     # so for an anime where sub episodes are ahead of dub the missing episodes will be outside the range of the episode_page_links
     first_eps_number = lacking_episode_numbers[0]
+    # If the alleged episode count is more than the actual number of episodes the site has e.g., Gintama on animpahe
+    if len(lacking_episode_numbers) > len(episode_page_links):
+        lacking_episode_numbers = lacking_episode_numbers[: len(episode_page_links)]
     return [
         episode_page_links[eps_number - first_eps_number]
         for eps_number in lacking_episode_numbers
     ]
 
 
 def ffmpeg_is_installed() -> bool:
```

### Comparing `senpwai-2.1.6/senpwai/utils/static.py` & `senpwai-2.1.7/senpwai/utils/static.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from random import choice as random_choice
 from subprocess import Popen
 from types import TracebackType
 import logging
 
 APP_NAME = "Senpwai"
 APP_NAME_LOWER = "senpwai"
-VERSION = "2.1.6"
+VERSION = "2.1.7"
 DESCRIPTION = "A desktop app for tracking and batch downloading anime"
 
 IS_PIP_INSTALL = False
 APP_EXE_PATH = ""
 
 
 class OS:
```

### Comparing `senpwai-2.1.6/senpwai/utils/widgets.py` & `senpwai-2.1.7/senpwai/utils/widgets.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/windows/about.py` & `senpwai-2.1.7/senpwai/windows/about.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/windows/abstracts.py` & `senpwai-2.1.7/senpwai/windows/abstracts.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/windows/chosen_anime.py` & `senpwai-2.1.7/senpwai/windows/chosen_anime.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/windows/download.py` & `senpwai-2.1.7/senpwai/windows/download.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/windows/main.py` & `senpwai-2.1.7/senpwai/windows/main.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/windows/misc.py` & `senpwai-2.1.7/senpwai/windows/misc.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/windows/search.py` & `senpwai-2.1.7/senpwai/windows/search.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/senpwai/windows/settings.py` & `senpwai-2.1.7/senpwai/windows/settings.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.6/PKG-INFO` & `senpwai-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senpwai
-Version: 2.1.6
+Version: 2.1.7
 Summary: A desktop app for tracking and batch downloading anime
 Home-page: https://github.com/SenZmaKi/Senpwai
 License: GPL v3
 Keywords: anime,app,cli,desktop app,anime downloader,anime cli,anime app,anime tracker,batch anime downloader,bulk anime  downloader,anime desktop app,anime tracker app
 Author: SenZmaKi
 Author-email: senzmaki@gmail.com
 Requires-Python: >=3.11,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: senpwai Version: 2.1.6 Summary: A desktop app for
+Metadata-Version: 2.1 Name: senpwai Version: 2.1.7 Summary: A desktop app for
 tracking and batch downloading anime Home-page: https://github.com/SenZmaKi/
 Senpwai License: GPL v3 Keywords: anime,app,cli,desktop app,anime
 downloader,anime cli,anime app,anime tracker,batch anime downloader,bulk anime
 downloader,anime desktop app,anime tracker app Author: SenZmaKi Author-email:
 senzmaki@gmail.com Requires-Python: >=3.11,<4.0 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

