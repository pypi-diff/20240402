# Comparing `tmp/wagtail-modeltranslation-0.8a1.tar.gz` & `tmp/wagtail-modeltranslation-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtail-modeltranslation-0.8a1.tar", last modified: Mon Jan 15 14:21:51 2018, max compression
+gzip compressed data, was "dist/wagtail-modeltranslation-0.9.0.tar", last modified: Wed May 30 11:28:23 2018, max compression
```

## Comparing `wagtail-modeltranslation-0.8a1.tar` & `wagtail-modeltranslation-0.9.0.tar`

### file list

```diff
@@ -1,58 +1,76 @@
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/docs/
--rw-r--r--   0 diogo     (1000) diogo     (1000)      472 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.8a1/docs/AUTHORS.rst
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/docs/releases/
--rw-r--r--   0 diogo     (1000) diogo     (1000)       68 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.8a1/docs/releases/index.rst
--rw-r--r--   0 diogo     (1000) diogo     (1000)     1634 2018-01-05 18:20:32.000000 wagtail-modeltranslation-0.8a1/docs/releases/0.6.0.rst
--rw-r--r--   0 diogo     (1000) diogo     (1000)     3851 2018-01-09 15:13:20.000000 wagtail-modeltranslation-0.8a1/docs/Installation.rst
--rw-r--r--   0 diogo     (1000) diogo     (1000)     4282 2018-01-05 18:20:32.000000 wagtail-modeltranslation-0.8a1/docs/CHANGELOG.rst
--rw-r--r--   0 diogo     (1000) diogo     (1000)     1243 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/docs/caveats.rst
--rw-r--r--   0 diogo     (1000) diogo     (1000)     1456 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/docs/advanced settings.rst
--rw-r--r--   0 diogo     (1000) diogo     (1000)      731 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.8a1/docs/recommended reading.rst
--rw-r--r--   0 diogo     (1000) diogo     (1000)     6118 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/docs/Registering Models.rst
--rw-r--r--   0 diogo     (1000) diogo     (1000)     1060 2018-01-05 18:24:20.000000 wagtail-modeltranslation-0.8a1/docs/template tags.rst
--rw-r--r--   0 diogo     (1000) diogo     (1000)     4122 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/docs/management commands.rst
--rw-r--r--   0 diogo     (1000) diogo     (1000)     2001 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/docs/index.rst
--rw-r--r--   0 diogo     (1000) diogo     (1000)     2230 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.8a1/docs/Introduction.rst
--rwxr-xr-x   0 diogo     (1000) diogo     (1000)      472 2017-02-20 14:40:41.000000 wagtail-modeltranslation-0.8a1/AUTHORS.rst
--rwxr-xr-x   0 diogo     (1000) diogo     (1000)     3702 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.8a1/CHANGELOG.txt
--rw-r--r--   0 diogo     (1000) diogo     (1000)     1336 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/PKG-INFO
--rwxr-xr-x   0 diogo     (1000) diogo     (1000)     2401 2018-01-15 14:21:43.000000 wagtail-modeltranslation-0.8a1/setup.py
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/static/
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/static/wagtail_modeltranslation/
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/static/wagtail_modeltranslation/css/
--rw-r--r--   0 diogo     (1000) diogo     (1000)      241 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/static/wagtail_modeltranslation/css/page_editor_modeltranslation.css
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/static/wagtail_modeltranslation/js/
--rw-r--r--   0 diogo     (1000) diogo     (1000)      965 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/static/wagtail_modeltranslation/js/wagtail_translated_slugs.js
--rwxr-xr-x   0 diogo     (1000) diogo     (1000)       45 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/static/wagtail_modeltranslation/js/force_jquery.js
--rw-r--r--   0 diogo     (1000) diogo     (1000)     2783 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/static/wagtail_modeltranslation/js/copy_stream_fields.js
--rw-r--r--   0 diogo     (1000) diogo     (1000)      345 2018-01-08 11:16:23.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/translation.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)     4981 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/wagtail_hooks.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)      607 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/settings.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)      533 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/contextlib.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)      486 2018-01-05 18:20:32.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/utils.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)      730 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/apps.py
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/makemigrations/
--rw-r--r--   0 diogo     (1000) diogo     (1000)      243 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/makemigrations/apps.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)      106 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/makemigrations/__init__.py
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/makemigrations/management/
--rw-r--r--   0 diogo     (1000) diogo     (1000)        0 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/makemigrations/management/__init__.py
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/makemigrations/management/commands/
--rwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/makemigrations/management/commands/__init__.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)      141 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/makemigrations/management/commands/makemigrations_original.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)      166 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/makemigrations/management/commands/makemigrations.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)       93 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/__init__.py
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/templatetags/
--rw-r--r--   0 diogo     (1000) diogo     (1000)     3349 2018-01-05 18:35:04.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/templatetags/wagtail_modeltranslation.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)        0 2017-02-20 14:40:41.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/templatetags/__init__.py
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/management/
--rwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2017-02-20 14:40:41.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/management/__init__.py
-drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-15 14:21:51.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/management/commands/
--rwxr--r--   0 diogo     (1000) diogo     (1000)      194 2018-01-05 18:25:28.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/management/commands/update_translation_fields.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)     1048 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/management/commands/set_translation_url_paths.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)     1298 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/management/commands/makemigrations_translation.py
--rwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2017-02-20 14:40:41.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/management/commands/__init__.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)     1004 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/management/commands/sync_page_translation_fields.py
--rw-r--r--   0 diogo     (1000) diogo     (1000)    20066 2018-01-08 11:16:23.000000 wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/patch_wagtailadmin.py
--rwxr-xr-x   0 diogo     (1000) diogo     (1000)     6104 2018-01-09 15:13:20.000000 wagtail-modeltranslation-0.8a1/README.rst
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/docs/
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      472 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.9.0/docs/AUTHORS.rst
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/docs/releases/
+-rw-r--r--   0 diogo     (1000) diogo     (1000)       68 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.9.0/docs/releases/index.rst
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     1634 2018-01-05 18:20:32.000000 wagtail-modeltranslation-0.9.0/docs/releases/0.6.0.rst
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     3851 2018-01-09 15:13:20.000000 wagtail-modeltranslation-0.9.0/docs/Installation.rst
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     4282 2018-01-05 18:20:32.000000 wagtail-modeltranslation-0.9.0/docs/CHANGELOG.rst
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     1243 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.9.0/docs/caveats.rst
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     1456 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.9.0/docs/advanced settings.rst
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      731 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.9.0/docs/recommended reading.rst
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     6118 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.9.0/docs/Registering Models.rst
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     1060 2018-01-05 18:24:20.000000 wagtail-modeltranslation-0.9.0/docs/template tags.rst
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     6275 2018-03-15 11:35:26.000000 wagtail-modeltranslation-0.9.0/docs/management commands.rst
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     2001 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.9.0/docs/index.rst
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     2230 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.9.0/docs/Introduction.rst
+-rwxr-xr-x   0 diogo     (1000) diogo     (1000)      472 2017-02-20 14:40:41.000000 wagtail-modeltranslation-0.9.0/AUTHORS.rst
+-rwxr-xr-x   0 diogo     (1000) diogo     (1000)     3702 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.9.0/CHANGELOG.txt
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      159 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/setup.cfg
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     1409 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/PKG-INFO
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation.egg-info/
+-rw-r--r--   0 diogo     (1000) diogo     (1000)       56 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation.egg-info/requires.txt
+-rw-r--r--   0 diogo     (1000) diogo     (1000)        1 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation.egg-info/dependency_links.txt
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     1409 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation.egg-info/PKG-INFO
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     2584 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation.egg-info/SOURCES.txt
+-rw-r--r--   0 diogo     (1000) diogo     (1000)       25 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation.egg-info/top_level.txt
+-rwxr-xr-x   0 diogo     (1000) diogo     (1000)     2888 2018-04-24 10:36:38.000000 wagtail-modeltranslation-0.9.0/setup.py
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/static/
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/static/wagtail_modeltranslation/
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/static/wagtail_modeltranslation/css/
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      241 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/static/wagtail_modeltranslation/css/page_editor_modeltranslation.css
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/static/wagtail_modeltranslation/js/
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     1019 2018-03-15 11:35:26.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/static/wagtail_modeltranslation/js/wagtail_translated_slugs.js
+-rwxr-xr-x   0 diogo     (1000) diogo     (1000)       45 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/static/wagtail_modeltranslation/js/force_jquery.js
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     2783 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/static/wagtail_modeltranslation/js/copy_stream_fields.js
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      414 2018-03-15 11:35:26.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/translation.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     5178 2018-04-24 10:36:38.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/wagtail_hooks.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      607 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/settings.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      533 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/contextlib.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      486 2018-01-05 18:20:32.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/utils.py
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/migrate/
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      215 2018-03-15 11:35:26.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/migrate/apps.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)       92 2018-03-15 11:35:26.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/migrate/__init__.py
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/migrate/management/
+-rw-r--r--   0 diogo     (1000) diogo     (1000)        0 2018-03-15 11:35:26.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/migrate/management/__init__.py
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/migrate/management/commands/
+-rwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-03-15 11:35:26.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/migrate/management/commands/__init__.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      145 2018-03-15 11:35:26.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/migrate/management/commands/migrate.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      120 2018-03-15 11:35:26.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/migrate/management/commands/migrate_original.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      730 2017-05-05 09:27:37.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/apps.py
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/makemigrations/
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      243 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/makemigrations/apps.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      106 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/makemigrations/__init__.py
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/makemigrations/management/
+-rw-r--r--   0 diogo     (1000) diogo     (1000)        0 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/makemigrations/management/__init__.py
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/makemigrations/management/commands/
+-rwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/makemigrations/management/commands/__init__.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      141 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/makemigrations/management/commands/makemigrations_original.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      166 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/makemigrations/management/commands/makemigrations.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)      114 2018-04-24 10:39:45.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/__init__.py
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/templatetags/
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     3768 2018-03-15 11:35:26.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/templatetags/wagtail_modeltranslation.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)        0 2017-02-20 14:40:41.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/templatetags/__init__.py
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/management/
+-rwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2017-02-20 14:40:41.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/management/__init__.py
+drwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2018-05-30 11:28:23.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/management/commands/
+-rwxr--r--   0 diogo     (1000) diogo     (1000)      194 2018-01-05 18:25:28.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/management/commands/update_translation_fields.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     1485 2018-03-15 11:35:26.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/management/commands/migrate_translation.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     1118 2018-03-15 11:35:26.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/management/commands/set_translation_url_paths.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     1298 2018-01-05 18:21:00.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/management/commands/makemigrations_translation.py
+-rwxr-xr-x   0 diogo     (1000) diogo     (1000)        0 2017-02-20 14:40:41.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/management/commands/__init__.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)     1074 2018-03-15 11:35:26.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/management/commands/sync_page_translation_fields.py
+-rw-r--r--   0 diogo     (1000) diogo     (1000)    24144 2018-04-24 10:36:38.000000 wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/patch_wagtailadmin.py
+-rwxr-xr-x   0 diogo     (1000) diogo     (1000)      288 2017-02-20 14:40:41.000000 wagtail-modeltranslation-0.9.0/MANIFEST.in
+-rwxr-xr-x   0 diogo     (1000) diogo     (1000)     6104 2018-01-09 15:13:20.000000 wagtail-modeltranslation-0.9.0/README.rst
```

### Comparing `wagtail-modeltranslation-0.8a1/docs/releases/0.6.0.rst` & `wagtail-modeltranslation-0.9.0/docs/releases/0.6.0.rst`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/docs/Installation.rst` & `wagtail-modeltranslation-0.9.0/docs/Installation.rst`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/docs/CHANGELOG.rst` & `wagtail-modeltranslation-0.9.0/docs/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/docs/caveats.rst` & `wagtail-modeltranslation-0.9.0/docs/caveats.rst`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/docs/advanced settings.rst` & `wagtail-modeltranslation-0.9.0/docs/advanced settings.rst`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/docs/recommended reading.rst` & `wagtail-modeltranslation-0.9.0/docs/recommended reading.rst`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/docs/Registering Models.rst` & `wagtail-modeltranslation-0.9.0/docs/Registering Models.rst`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/docs/template tags.rst` & `wagtail-modeltranslation-0.9.0/docs/template tags.rst`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/docs/management commands.rst` & `wagtail-modeltranslation-0.9.0/docs/management commands.rst`

 * *Files 20% similar despite different names*

```diff
@@ -53,21 +53,38 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. versionadded:: 0.8
 
 ``wagtail-modeltranslation`` patches Wagtail's ``Page`` model and as consequence Django's original 
 ``makemigrations`` commmand will create migrations for ``Page`` which may create conflicts with 
 other migrations. To circumvent this issue ``makemigrations_translation`` hides any ``Page`` model changes 
-and creates all other migrations as usual. Use this command as an alterntive to Django's own 
+and creates all other migrations as usual. Use this command as an alternative to Django's own 
 ``makemigrations`` or consider using :ref:`management_commands-makemigrations`.
 
 .. code-block:: console
 
     $ python manage.py makemigrations_translation
 
+.. _management_commands-migrate_translation:
+
+The ``migrate_translation`` Command
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. versionadded:: 0.8
+
+Since :ref:`management_commands-makemigrations_translation` hides any ``Page`` model changes, Django's own
+``migrate`` command won't be able to update ``wagtailcore_page`` table with new translation fields. In order to
+correctly update the database schema a combination of ``migrate`` followed by :ref:`sync_page_translation_fields` 
+is usually required. ``migrate_translation`` provides a shortcut to running these two commands. Use this 
+as an alternative to Django's own ``migrate`` or consider using :ref:`management_commands-migrate`.
+
+.. code-block:: console
+
+    $ python manage.py migrate_translation
+
 .. _management_commands-set_translation_url_paths:
 
 The ``set_translation_url_paths`` Command
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Updates url_path translation fields for all pages.
 
@@ -105,7 +122,45 @@
 Since Django's ``makemigrations`` is overriden by ``wagtail-modeltranslation``'s version use 
 ``makemigrations_original`` to run the Django's original ``makemigrations`` command. Please note 
 this will likely create invalid ``Page`` migrations, do this only if you know what you're doing.
 
 .. code-block:: console
 
     $ python manage.py makemigrations_original
+
+
+.. _management_commands-wagtail_modeltranslation.migrate:
+
+wagtail_modeltranslation.migrate
+---------------------------------
+
+To use ``wagtail_modeltranslation.migrate`` module commands add ``'wagtail_modeltranslation.migrate,'`` 
+to ``INSTALLED_APPS``. This module adds the following management commands.
+
+.. _management_commands-migrate:
+
+The ``migrate`` Command
+~~~~~~~~~~~~~~~~~~~~~~~
+
+This command is a proxy for :ref:`management_commands-migrate_translation`. It has the added benefit of 
+overriding Django's own ``migrate`` saving the need to additionally run :ref:`sync_page_translation_fields`. 
+See `issue #175
+<https://github.com/infoportugal/wagtail-modeltranslation/issues/175#issuecomment-368046055>`_ to understand 
+how this command can be used to create translation fields in a test database.
+
+.. code-block:: console
+
+    $ python manage.py migrate
+
+.. _management_commands-migrate_original:
+
+The ``migrate_original`` Command
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Since Django's ``migrate`` is overriden by ``wagtail-modeltranslation``'s version use 
+``migrate_original`` to run the Django's original ``migrate`` command. Please note 
+this will not update ``wagtailcore_page`` table with new translation fields, use 
+:ref:`sync_page_translation_fields` for that.
+
+.. code-block:: console
+
+    $ python manage.py migrate_original
```

### Comparing `wagtail-modeltranslation-0.8a1/docs/index.rst` & `wagtail-modeltranslation-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/docs/Introduction.rst` & `wagtail-modeltranslation-0.9.0/docs/Introduction.rst`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/CHANGELOG.txt` & `wagtail-modeltranslation-0.9.0/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/PKG-INFO` & `wagtail-modeltranslation-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: wagtail-modeltranslation
-Version: 0.8a1
+Version: 0.9.0
 Summary: Translates Wagtail CMS models using a registration approach.
 Home-page: https://github.com/infoportugal/wagtail-modeltranslation
 Author: InfoPortugal, S.A.
 Author-email: suporte24@infoportugal.pt
+Maintainer: InfoPortugal, S.A.
+Maintainer-email: suporte24@infoportugal.pt
 License: New BSD
-Download-URL: https://github.com/infoportugal/wagtail-modeltranslation/archive/v0.8a1.tar.gz
+Download-URL: https://github.com/infoportugal/wagtail-modeltranslation/archive/v0.8.tar.gz
 Description: The modeltranslation application can be used to translate dynamic content of existing models to an arbitrary number of languages without having to change the original model classes. It uses a registration approach (comparable to Django's admin app) to be able to add translations to existing or new projects and is fully integrated into the Wagtail admin backend.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
```

### Comparing `wagtail-modeltranslation-0.8a1/setup.py` & `wagtail-modeltranslation-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 #!/usr/bin/env python
-from distutils.core import setup
+import re
+
+import os
+from setuptools import setup
+
+
+def get_version(*file_paths):
+    filename = os.path.join(os.path.dirname(__file__), *file_paths)
+    version_file = open(filename).read()
+    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M)
+    if version_match:
+        return version_match.group(1)
+    raise RuntimeError('Please assure that the package version is defined as "__version__ = x.x.x" in ' + filename)
+
+
+version = get_version("wagtail_modeltranslation", "__init__.py")
 
 setup(
     name='wagtail-modeltranslation',
-    version='0.8a1',
+    version=version,
     description='Translates Wagtail CMS models using a registration approach.',
     long_description=(
         'The modeltranslation application can be used to translate dynamic '
         'content of existing models to an arbitrary number of languages '
         'without having to change the original model classes. It uses a '
         'registration approach (comparable to Django\'s admin app) to be able '
         'to add translations to existing or new projects and is fully '
@@ -20,22 +35,22 @@
     packages=[
         'wagtail_modeltranslation',
         'wagtail_modeltranslation.management',
         'wagtail_modeltranslation.management.commands',
         'wagtail_modeltranslation.templatetags',
         'wagtail_modeltranslation.makemigrations',
         'wagtail_modeltranslation.makemigrations.management',
-        'wagtail_modeltranslation.makemigrations.management.commands'],
+        'wagtail_modeltranslation.makemigrations.management.commands',
+        'wagtail_modeltranslation.migrate',
+        'wagtail_modeltranslation.migrate.management',
+        'wagtail_modeltranslation.migrate.management.commands'],
     package_data={'wagtail_modeltranslation': ['static/wagtail_modeltranslation/css/*.css',
                                                'static/wagtail_modeltranslation/js/*.js']},
-    install_requires=['wagtail(>=1.4)', 'django-modeltranslation(>0.12.1)'],
-    dependency_links=[
-        "http://github.com/deschler/django-modeltranslation/tarball/00fc7f1804aaa1b1e37af48e67871080851e14b0#egg=django-modeltranslation-0.12.2"
-    ],
-    download_url='https://github.com/infoportugal/wagtail-modeltranslation/archive/v0.8a1.tar.gz',
+    install_requires=['Django<2.0', 'wagtail>=1.4', 'django-modeltranslation>=0.12.2'],
+    download_url='https://github.com/infoportugal/wagtail-modeltranslation/archive/v0.8.tar.gz',
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.2',
         'Programming Language :: Python :: 3.3',
```

### Comparing `wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/static/wagtail_modeltranslation/js/copy_stream_fields.js` & `wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/static/wagtail_modeltranslation/js/copy_stream_fields.js`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/wagtail_hooks.py` & `wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/wagtail_hooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,22 @@
 from django.conf import settings
 from django.conf.urls import url
 from django.http import HttpResponse
 from django.http import QueryDict
 from django.utils.html import format_html, format_html_join, escape
 from django.views.decorators.csrf import csrf_exempt
 from six import iteritems
-from wagtail.wagtailcore import hooks
-from wagtail.wagtailcore.models import Page
-from wagtail.wagtailcore.rich_text import PageLinkHandler
+try:
+    from wagtail.core import hooks
+    from wagtail.core.models import Page
+    from wagtail.core.rich_text.pages import PageLinkHandler
+except ImportError:
+    from wagtail.wagtailcore import hooks
+    from wagtail.wagtailcore.models import Page
+    from wagtail.wagtailcore.rich_text import PageLinkHandler
 
 
 @hooks.register('insert_editor_js')
 def translated_slugs():
     js_files = [
         'wagtail_modeltranslation/js/wagtail_translated_slugs.js',
     ]
@@ -50,21 +55,21 @@
         target_field_name = request.POST.get('target_field_name')
         origin_field_serialized = json.loads(
             request.POST.get('serializedOriginField'))
 
         # Patch field prefixes from origin field to target field
         target_field_patched = []
         for item in origin_field_serialized:
-            patched_item = None
+            patched_item = {'name': None, 'value': None}
             for att in iteritems(item):
                 target_value = att[1]
                 if att[0] == 'name':
                     target_value = att[1].replace(
                         origin_field_name, target_field_name)
-                    patched_item = {"name": target_value}
+                    patched_item["name"] = target_value
                 else:
                     patched_item["value"] = att[1]
 
             target_field_patched.append(patched_item)
 
         # convert to QueryDict
         q_data = QueryDict('', mutable=True)
```

### Comparing `wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/settings.py` & `wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/contextlib.py` & `wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/contextlib.py`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/apps.py` & `wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/apps.py`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/templatetags/wagtail_modeltranslation.py` & `wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/templatetags/wagtail_modeltranslation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 # coding: utf-8
 
 import re
 
 from django import template
-from django.core.urlresolvers import resolve
 from django.utils.translation import activate, get_language
 
+try:
+    from django.core.urlresolvers import resolve
+except ImportError:
+    from django.urls import resolve
+
 from six import iteritems
 
-from wagtail.wagtailcore.models import Page
-from modeltranslation import settings as mt_settings
+try:
+    from wagtail.core.models import Page
+    from wagtail.core.templatetags.wagtailcore_tags import pageurl
+except ImportError:
+    from wagtail.wagtailcore.models import Page
+    from wagtail.wagtailcore.templatetags.wagtailcore_tags import pageurl
 
+from modeltranslation import settings as mt_settings
 from modeltranslation.settings import DEFAULT_LANGUAGE
 
 from ..contextlib import use_language
 
 register = template.Library()
 
 
@@ -42,15 +51,17 @@
             return translated_url
         elif match.url_name == 'wagtailsearch_search':
             path_components = [component for component in non_prefixed_path.split('/') if component]
 
             translated_url = '/' + lang + '/' + path_components[0] + '/'
             if request.GET:
                 translated_url += '?'
-                for key, value in iteritems(request.GET):
+                for count, (key, value) in enumerate(iteritems(request.GET)):
+                    if count != 0:
+                        translated_url += "&"
                     translated_url += key + '=' + value
             return translated_url
 
     return ''
 
 
 class GetAvailableLanguagesNode(template.Node):
@@ -76,19 +87,18 @@
     """
     language = language or DEFAULT_LANGUAGE
 
     with use_language(language):
         page = Page.objects.filter(slug=slug).first()
 
     if page:
-        return page.relative_url(context['request'].site)
-    else:
-        return None
+        # call pageurl() instead of page.relative_url() here so we get the ``accepts_kwarg`` logic
+        return pageurl(context, page)
+
 
-        
 @register.tag('get_available_languages_wmt')
 def do_get_available_languages(unused_parser, token):
     """
     Store a list of available languages in the context.
 
     Usage::
```

### Comparing `wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/management/commands/set_translation_url_paths.py` & `wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/management/commands/set_translation_url_paths.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # coding: utf-8
 
 from django.core.management.base import BaseCommand
 from modeltranslation import settings as mt_settings
 from modeltranslation.utils import build_localized_fieldname
-from wagtail.wagtailcore.models import Page
 from wagtail_modeltranslation.contextlib import use_language
+try:
+    from wagtail.core.models import Page
+except ImportError:
+    from wagtail.wagtailcore.models import Page
 
 
 class Command(BaseCommand):
     def __init__(self):
         super(Command, self).__init__()
         update_fields = ['url_path']
         for language in mt_settings.AVAILABLE_LANGUAGES:
```

### Comparing `wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/management/commands/makemigrations_translation.py` & `wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/management/commands/makemigrations_translation.py`

 * *Files identical despite different names*

### Comparing `wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/management/commands/sync_page_translation_fields.py` & `wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/management/commands/sync_page_translation_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from modeltranslation.management.commands.sync_translation_fields import Command as SyncTranslationsFieldsCommand
 from modeltranslation.translator import translator
-from wagtail.wagtailcore.models import Page
+try:
+    from wagtail.core.models import Page
+except ImportError:
+    from wagtail.wagtailcore.models import Page
 
 
 old_get_registered_models = translator.get_registered_models
 
 # Monkey patching, only return a model if it's Page
 def get_page_model(self, abstract=True):
     models = old_get_registered_models(abstract)
```

### Comparing `wagtail-modeltranslation-0.8a1/wagtail_modeltranslation/patch_wagtailadmin.py` & `wagtail-modeltranslation-0.9.0/wagtail_modeltranslation/patch_wagtailadmin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,55 @@
 # coding: utf-8
 import copy
 import logging
 import types
 
+from django.core.cache import cache
 from django.core.exceptions import ValidationError
+from django.core.urlresolvers import reverse
 from django.db import transaction, connection
 from django.db.models import Q, Value
 from django.db.models.functions import Concat, Substr
 from django.http import Http404
 from django.utils.translation import trans_real
 from django.utils.translation import ugettext_lazy as _
 from modeltranslation import settings as mt_settings
 from modeltranslation.translator import translator, NotRegistered
 from modeltranslation.utils import build_localized_fieldname, get_language
 from wagtail.contrib.settings.models import BaseSetting
 from wagtail.contrib.settings.views import get_setting_edit_handler
-from wagtail.contrib.wagtailroutablepage.models import RoutablePageMixin
-from wagtail.wagtailadmin.edit_handlers import FieldPanel, \
-    MultiFieldPanel, FieldRowPanel, InlinePanel, StreamFieldPanel, RichTextFieldPanel
-from wagtail.wagtailcore.models import Page
-from wagtail.wagtailcore.fields import StreamField, StreamValue
-from wagtail.wagtailcore.url_routing import RouteResult
-from wagtail.wagtailimages.edit_handlers import ImageChooserPanel
-from wagtail.wagtailsearch.index import SearchField
-from wagtail.wagtailsnippets.models import get_snippet_models
-from wagtail.wagtailsnippets.views.snippets import SNIPPET_EDIT_HANDLERS
-
+try:
+    from wagtail.contrib.routable_page.models import RoutablePageMixin
+    from wagtail.admin.edit_handlers import FieldPanel, \
+        MultiFieldPanel, FieldRowPanel, InlinePanel, StreamFieldPanel, RichTextFieldPanel
+    from wagtail.core.models import Page, Site
+    from wagtail.core.fields import StreamField, StreamValue
+    from wagtail.core.url_routing import RouteResult
+    from wagtail.images.edit_handlers import ImageChooserPanel
+    from wagtail.search.index import SearchField
+    from wagtail.snippets.models import get_snippet_models
+    from wagtail.snippets.views.snippets import SNIPPET_EDIT_HANDLERS
+except ImportError:
+    from wagtail.contrib.wagtailroutablepage.models import RoutablePageMixin
+    from wagtail.wagtailadmin.edit_handlers import FieldPanel, \
+        MultiFieldPanel, FieldRowPanel, InlinePanel, StreamFieldPanel, RichTextFieldPanel
+    from wagtail.wagtailcore.models import Page, Site
+    from wagtail.wagtailcore.fields import StreamField, StreamValue
+    from wagtail.wagtailcore.url_routing import RouteResult
+    from wagtail.wagtailimages.edit_handlers import ImageChooserPanel
+    from wagtail.wagtailsearch.index import SearchField
+    from wagtail.wagtailsnippets.models import get_snippet_models
+    from wagtail.wagtailsnippets.views.snippets import SNIPPET_EDIT_HANDLERS
+try:
+    from wagtail.core.utils import WAGTAIL_APPEND_SLASH
+except ImportError:
+    try:
+        from wagtail.wagtailcore.utils import WAGTAIL_APPEND_SLASH
+    except ImportError:
+        WAGTAIL_APPEND_SLASH = True  # Wagtail<1.5
 from wagtail_modeltranslation.settings import CUSTOM_SIMPLE_PANELS, CUSTOM_COMPOSED_PANELS
 from wagtail_modeltranslation.utils import compare_class_tree_depth
 
 logger = logging.getLogger('wagtail.core')
 
 SIMPLE_PANEL_CLASSES = [FieldPanel, ImageChooserPanel, StreamFieldPanel, RichTextFieldPanel] + CUSTOM_SIMPLE_PANELS
 COMPOSED_PANEL_CLASSES = [MultiFieldPanel, FieldRowPanel] + CUSTOM_COMPOSED_PANELS
@@ -98,14 +118,17 @@
                 descriptor = getattr(model, field.name)
                 _patch_stream_field_meaningful_value(descriptor)
 
         # OVERRIDE PAGE METHODS
         model.set_url_path = _new_set_url_path
         model.route = _new_route
         model._update_descendant_url_paths = _new_update_descendant_url_paths
+        if not hasattr(model, '_get_site_root_paths'):
+            model.get_url_parts = _new_get_url_parts  # Wagtail<1.11
+        model._get_site_root_paths = _new_get_site_root_paths
         _patch_clean(model)
 
         if not model.save.__name__.startswith('localized'):
             setattr(model, 'save', LocalizedSaveDescriptor(model.save))
 
     def _patch_other_models(self, model):
         if hasattr(model, 'edit_handler'):
@@ -155,14 +178,22 @@
             localized_field_name = build_localized_fieldname(original_panel.field_name, language)
 
             # if the original field is required and the current language is the default one
             # this field's blank property is set to False
             if not original_field.blank and language == mt_settings.DEFAULT_LANGUAGE:
                 localized_field = model._meta.get_field(localized_field_name)
                 localized_field.blank = False
+            elif isinstance(original_field, StreamField):
+                # otherwise the field is optional and
+                # if it's a StreamField the stream_block need to be changed to non required
+                localized_field = model._meta.get_field(localized_field_name)
+                new_stream_block = copy.copy(localized_field.stream_block)
+                new_stream_block.meta = copy.copy(localized_field.stream_block.meta)
+                new_stream_block.meta.required = False
+                localized_field.stream_block = new_stream_block
 
             localized_panel = panel_class(localized_field_name)
 
             # Pass the original panel extra attributes to the localized
             if hasattr(original_panel, 'classname'):
                 localized_panel.classname = original_panel.classname
             if hasattr(original_panel, 'widget'):
@@ -363,14 +394,65 @@
             .exclude(**{localized_url_path: None})  # url_path_xx may not be set yet
             .exclude(pk=page.pk)
             .update(**{localized_url_path: Concat(
                 Value(new_url_path),
                 Substr(localized_url_path, len(old_url_path) + 1))}))
 
 
+def _localized_site_get_site_root_paths():
+    """
+    Localized version of ``Site.get_site_root_paths()``
+    """
+    current_language = get_language()
+    cache_key = 'wagtail_site_root_paths_{}'.format(current_language)
+    result = cache.get(cache_key)
+
+    if result is None:
+        result = [
+            (site.id, site.root_page.url_path, site.root_url)
+            for site in Site.objects.select_related('root_page').order_by('-root_page__url_path')
+        ]
+        cache.set(cache_key, result, 3600)
+
+    return result
+
+
+def _new_get_site_root_paths(self, request=None):
+    """
+    Return localized site_root_paths, using the cached copy on the
+    request object if available and if language is the same.
+    """
+    # if we have a request, use that to cache site_root_paths; otherwise, use self
+    current_language = get_language()
+    cache_object = request if request else self
+    if not hasattr(cache_object, '_wagtail_cached_site_root_paths_language') or \
+            cache_object._wagtail_cached_site_root_paths_language != current_language:
+        cache_object._wagtail_cached_site_root_paths_language = current_language
+        cache_object._wagtail_cached_site_root_paths = _localized_site_get_site_root_paths()
+
+    return cache_object._wagtail_cached_site_root_paths
+
+
+def _new_get_url_parts(self, request=None):
+    """
+    For Wagtail<1.11 ``Page.get_url_parts()`` is patched so it uses ``self._get_site_root_paths(request)``
+    """
+    for (site_id, root_path, root_url) in self._get_site_root_paths(request):
+        if self.url_path.startswith(root_path):
+            page_path = reverse('wagtail_serve', args=(self.url_path[len(root_path):],))
+
+            # Remove the trailing slash from the URL reverse generates if
+            # WAGTAIL_APPEND_SLASH is False and we're not trying to serve
+            # the root path
+            if not WAGTAIL_APPEND_SLASH and page_path != '/':
+                page_path = page_path.rstrip('/')
+
+            return (site_id, root_url, page_path)
+
+
 def _update_translation_descendant_url_paths(old_record, page):
     # update children paths, must be done for all languages to ensure fallbacks are applied
     languages_changed = []
     default_localized_url_path = build_localized_fieldname('url_path', mt_settings.DEFAULT_LANGUAGE)
     for language in mt_settings.AVAILABLE_LANGUAGES:
         localized_url_path = build_localized_fieldname('url_path', language)
         old_url_path = getattr(old_record, localized_url_path) or getattr(old_record, default_localized_url_path)
@@ -448,14 +530,19 @@
 
         result = self.func(instance, *args, **kwargs)
 
         # update children localized paths if any language had it slug changed
         if change_descendant_url_path:
             _update_translation_descendant_url_paths(old_record, instance)
 
+        # Check if this is a root page of any sites and clear the 'wagtail_site_root_paths_XX' key if so
+        if Site.objects.filter(root_page=instance).exists():
+            for language in mt_settings.AVAILABLE_LANGUAGES:
+                cache.delete('wagtail_site_root_paths_{}'.format(language))
+
         return result
 
     def __get__(self, instance, owner=None):
         return types.MethodType(self, instance) if instance else self
 
 
 def _patch_stream_field_meaningful_value(field):
```

### Comparing `wagtail-modeltranslation-0.8a1/README.rst` & `wagtail-modeltranslation-0.9.0/README.rst`

 * *Files identical despite different names*

