# Comparing `tmp/neon-skill-caffeinewiz-1.0.1a4.tar.gz` & `tmp/neon-skill-caffeinewiz-1.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-caffeinewiz-1.0.1a4.tar", last modified: Mon Feb  5 22:33:58 2024, max compression
+gzip compressed data, was "neon-skill-caffeinewiz-1.0.1a5.tar", last modified: Fri Mar  1 23:49:40 2024, max compression
```

## Comparing `neon-skill-caffeinewiz-1.0.1a4.tar` & `neon-skill-caffeinewiz-1.0.1a5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:33:58.691966 neon-skill-caffeinewiz-1.0.1a4/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-05 22:33:58.691966 neon-skill-caffeinewiz-1.0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    24730 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:33:58.683966 neon-skill-caffeinewiz-1.0.1a4/data/
--rw-r--r--   0 runner    (1001) docker     (127)    31954 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/data/caffeine_wiz_data.pickle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:33:58.683966 neon-skill-caffeinewiz-1.0.1a4/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:33:58.683966 neon-skill-caffeinewiz-1.0.1a4/locale/de-de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:33:58.683966 neon-skill-caffeinewiz-1.0.1a4/locale/de-de/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/de-de/dialog/drink_caffeine.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:33:58.683966 neon-skill-caffeinewiz-1.0.1a4/locale/de-de/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/de-de/regex/drink.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:33:58.683966 neon-skill-caffeinewiz-1.0.1a4/locale/de-de/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/de-de/vocab/goodbye.voc
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/de-de/vocab/query_caffeine.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:33:58.683966 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:33:58.687966 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/drink_caffeine.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/how_about_more.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/more_drinks.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/multiple_drinks.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/no_drink_heard.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/not_found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/one_moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/provided_by_caffeinewiz.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/stay_caffeinated.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/update_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/update_error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/updating.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/word_liter.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/word_milligrams.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/word_milliliters.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/dialog/word_ounces.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:33:58.687966 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/regex/drink.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:33:58.687966 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/vocab/caffeine.voc
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/vocab/goodbye.voc
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/vocab/query_caffeine.voc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/locale/en-us/vocab/update_caffeine.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:33:58.691966 neon-skill-caffeinewiz-1.0.1a4/neon_skill_caffeinewiz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-05 22:33:58.000000 neon-skill-caffeinewiz-1.0.1a4/neon_skill_caffeinewiz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-05 22:33:58.000000 neon-skill-caffeinewiz-1.0.1a4/neon_skill_caffeinewiz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 22:33:58.000000 neon-skill-caffeinewiz-1.0.1a4/neon_skill_caffeinewiz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-05 22:33:58.000000 neon-skill-caffeinewiz-1.0.1a4/neon_skill_caffeinewiz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-05 22:33:58.000000 neon-skill-caffeinewiz-1.0.1a4/neon_skill_caffeinewiz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-05 22:33:58.000000 neon-skill-caffeinewiz-1.0.1a4/neon_skill_caffeinewiz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 22:33:58.691966 neon-skill-caffeinewiz-1.0.1a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:33:58.691966 neon-skill-caffeinewiz-1.0.1a4/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-05 22:33:54.000000 neon-skill-caffeinewiz-1.0.1a4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.758771 neon-skill-caffeinewiz-1.0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-01 23:49:40.758771 neon-skill-caffeinewiz-1.0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    24730 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.750771 neon-skill-caffeinewiz-1.0.1a5/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    31954 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/data/caffeine_wiz_data.pickle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.750771 neon-skill-caffeinewiz-1.0.1a5/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.750771 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.750771 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/dialog/drink_caffeine.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.750771 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/regex/drink.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.754771 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/vocab/goodbye.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/vocab/query_caffeine.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.750771 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.754771 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/drink_caffeine.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/how_about_more.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/more_drinks.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/multiple_drinks.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/no_drink_heard.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/not_found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/one_moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/provided_by_caffeinewiz.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/stay_caffeinated.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/update_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/update_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/updating.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/word_liter.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/word_milligrams.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/word_milliliters.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/word_ounces.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.754771 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/regex/drink.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.754771 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/vocab/caffeine.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/vocab/goodbye.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/vocab/query_caffeine.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/vocab/update_caffeine.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.754771 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-01 23:49:40.000000 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-01 23:49:40.000000 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 23:49:40.000000 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-01 23:49:40.000000 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-01 23:49:40.000000 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-01 23:49:40.000000 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 23:49:40.758771 neon-skill-caffeinewiz-1.0.1a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.754771 neon-skill-caffeinewiz-1.0.1a5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/version.py
```

### Comparing `neon-skill-caffeinewiz-1.0.1a4/LICENSE.md` & `neon-skill-caffeinewiz-1.0.1a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a4/PKG-INFO` & `neon-skill-caffeinewiz-1.0.1a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-caffeinewiz
-Version: 1.0.1a4
+Version: 1.0.1a5
 Home-page: https://github.com/NeonGeckoCom/skill-caffeinewiz
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-caffeinewiz-1.0.1a4/README.md` & `neon-skill-caffeinewiz-1.0.1a5/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a4/__init__.py` & `neon-skill-caffeinewiz-1.0.1a5/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a4/data/caffeine_wiz_data.pickle` & `neon-skill-caffeinewiz-1.0.1a5/data/caffeine_wiz_data.pickle`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a4/neon_skill_caffeinewiz.egg-info/PKG-INFO` & `neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-caffeinewiz
-Version: 1.0.1a4
+Version: 1.0.1a5
 Home-page: https://github.com/NeonGeckoCom/skill-caffeinewiz
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-caffeinewiz-1.0.1a4/neon_skill_caffeinewiz.egg-info/SOURCES.txt` & `neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a4/setup.py` & `neon-skill-caffeinewiz-1.0.1a5/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a4/skill.json` & `neon-skill-caffeinewiz-1.0.1a5/skill.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985507246376812%*

 * *Differences: {"'requirements'": "{'python': {insert: [(1, 'neon-utils~=1.0,!=1.9.0')], delete: [1]}}"}*

```diff
@@ -28,15 +28,15 @@
         "ia64",
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
             "beautifulsoup4~=4.0",
-            "neon-utils~=1.0",
+            "neon-utils~=1.0,!=1.9.0",
             "ovos-bus-client~=0.0.3",
             "ovos-utils~=0.0, >=0.0.28"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "Provides the caffeine content of various drinks on request.",
```

### Comparing `neon-skill-caffeinewiz-1.0.1a4/test/test_skill.py` & `neon-skill-caffeinewiz-1.0.1a5/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a4/version.py` & `neon-skill-caffeinewiz-1.0.1a5/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a4"
+__version__ = "1.0.1a5"
```

