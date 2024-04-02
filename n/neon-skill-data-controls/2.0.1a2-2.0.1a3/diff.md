# Comparing `tmp/neon-skill-data_controls-2.0.1a2.tar.gz` & `tmp/neon-skill-data_controls-2.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-data_controls-2.0.1a2.tar", last modified: Tue Feb  6 00:42:53 2024, max compression
+gzip compressed data, was "neon-skill-data_controls-2.0.1a3.tar", last modified: Tue Apr  2 18:42:34 2024, max compression
```

## Comparing `neon-skill-data_controls-2.0.1a2.tar` & `neon-skill-data_controls-2.0.1a3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:42:53.536476 neon-skill-data_controls-2.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-06 00:42:53.536476 neon-skill-data_controls-2.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:42:53.532476 neon-skill-data_controls-2.0.1a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:42:53.532476 neon-skill-data_controls-2.0.1a2/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:42:53.536476 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/ask_clear_data.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/confirm_clear_all.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/confirm_clear_data.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/confirm_no_action.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/word_all_brands.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/word_all_data.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/word_caches.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/word_disliked_brands.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/word_language.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/word_liked_brands.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/word_media.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/word_profile_data.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/word_transcriptions.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/dialog/word_units.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:42:53.536476 neon-skill-data_controls-2.0.1a2/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/intent/clear_data.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:42:53.536476 neon-skill-data_controls-2.0.1a2/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/vocab/brands.voc
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/vocab/cache.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/vocab/cancel.voc
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/vocab/data.voc
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/vocab/dislikes.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/vocab/language.voc
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/vocab/likes.voc
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/vocab/media.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/vocab/profile.voc
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/vocab/transcription.voc
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/locale/en-us/vocab/units.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:42:53.536476 neon-skill-data_controls-2.0.1a2/neon_skill_data_controls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-06 00:42:53.000000 neon-skill-data_controls-2.0.1a2/neon_skill_data_controls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-06 00:42:53.000000 neon-skill-data_controls-2.0.1a2/neon_skill_data_controls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 00:42:53.000000 neon-skill-data_controls-2.0.1a2/neon_skill_data_controls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-06 00:42:53.000000 neon-skill-data_controls-2.0.1a2/neon_skill_data_controls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-06 00:42:53.000000 neon-skill-data_controls-2.0.1a2/neon_skill_data_controls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-06 00:42:53.000000 neon-skill-data_controls-2.0.1a2/neon_skill_data_controls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 00:42:53.536476 neon-skill-data_controls-2.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 00:42:53.536476 neon-skill-data_controls-2.0.1a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)    13677 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-06 00:42:41.000000 neon-skill-data_controls-2.0.1a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:42:34.111537 neon-skill-data_controls-2.0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-02 18:42:34.111537 neon-skill-data_controls-2.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:42:34.107537 neon-skill-data_controls-2.0.1a3/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:42:34.107537 neon-skill-data_controls-2.0.1a3/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:42:34.107537 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/ask_clear_data.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/confirm_clear_all.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/confirm_clear_data.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/confirm_no_action.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/word_all_brands.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/word_all_data.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/word_caches.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/word_disliked_brands.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/word_language.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/word_liked_brands.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/word_media.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/word_profile_data.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/word_transcriptions.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/dialog/word_units.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:42:34.107537 neon-skill-data_controls-2.0.1a3/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/intent/clear_data.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:42:34.111537 neon-skill-data_controls-2.0.1a3/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/vocab/brands.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/vocab/cache.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/vocab/cancel.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/vocab/data.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/vocab/dislikes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/vocab/language.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/vocab/likes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/vocab/media.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/vocab/profile.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/vocab/transcription.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/locale/en-us/vocab/units.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:42:34.111537 neon-skill-data_controls-2.0.1a3/neon_skill_data_controls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-02 18:42:34.000000 neon-skill-data_controls-2.0.1a3/neon_skill_data_controls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-02 18:42:34.000000 neon-skill-data_controls-2.0.1a3/neon_skill_data_controls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:42:34.000000 neon-skill-data_controls-2.0.1a3/neon_skill_data_controls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-02 18:42:34.000000 neon-skill-data_controls-2.0.1a3/neon_skill_data_controls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-02 18:42:34.000000 neon-skill-data_controls-2.0.1a3/neon_skill_data_controls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 18:42:34.000000 neon-skill-data_controls-2.0.1a3/neon_skill_data_controls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:42:34.111537 neon-skill-data_controls-2.0.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:42:34.111537 neon-skill-data_controls-2.0.1a3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    13677 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 18:42:30.000000 neon-skill-data_controls-2.0.1a3/version.py
```

### Comparing `neon-skill-data_controls-2.0.1a2/LICENSE.md` & `neon-skill-data_controls-2.0.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-data_controls-2.0.1a2/PKG-INFO` & `neon-skill-data_controls-2.0.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-data_controls
-Version: 2.0.1a2
+Version: 2.0.1a3
 Home-page: https://github.com/NeonGeckoCom/skill-data_controls
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-data_controls-2.0.1a2/README.md` & `neon-skill-data_controls-2.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-data_controls-2.0.1a2/__init__.py` & `neon-skill-data_controls-2.0.1a3/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-data_controls-2.0.1a2/neon_skill_data_controls.egg-info/PKG-INFO` & `neon-skill-data_controls-2.0.1a3/neon_skill_data_controls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-data-controls
-Version: 2.0.1a2
+Version: 2.0.1a3
 Home-page: https://github.com/NeonGeckoCom/skill-data_controls
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-data_controls-2.0.1a2/neon_skill_data_controls.egg-info/SOURCES.txt` & `neon-skill-data_controls-2.0.1a3/neon_skill_data_controls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-data_controls-2.0.1a2/setup.py` & `neon-skill-data_controls-2.0.1a3/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-data_controls-2.0.1a2/skill.json` & `neon-skill-data_controls-2.0.1a3/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-data_controls-2.0.1a2/test/test_skill.py` & `neon-skill-data_controls-2.0.1a3/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-data_controls-2.0.1a2/version.py` & `neon-skill-data_controls-2.0.1a3/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.0.1a2"
+__version__ = "2.0.1a3"
```

