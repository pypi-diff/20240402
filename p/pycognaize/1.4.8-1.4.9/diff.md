# Comparing `tmp/pycognaize-1.4.8.tar.gz` & `tmp/pycognaize-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycognaize-1.4.8.tar", last modified: Sat Jun 24 16:48:31 2023, max compression
+gzip compressed data, was "pycognaize-1.4.9.tar", last modified: Tue Jun 27 15:13:11 2023, max compression
```

## Comparing `pycognaize-1.4.8.tar` & `pycognaize-1.4.9.tar`

### file list

```diff
@@ -1,72 +1,70 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-24 16:48:31.370433 pycognaize-1.4.8/
--rw-rw-r--   0 david     (1000) david     (1000)    32056 2023-06-24 16:44:55.000000 pycognaize-1.4.8/CHANGELOG.md
--rw-rw-r--   0 david     (1000) david     (1000)    35137 2023-01-20 10:59:34.000000 pycognaize-1.4.8/LICENSE.txt
--rw-rw-r--   0 david     (1000) david     (1000)    33824 2023-06-24 16:48:31.370433 pycognaize-1.4.8/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1310 2023-02-10 17:58:58.000000 pycognaize-1.4.8/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-24 16:48:31.370433 pycognaize-1.4.8/pycognaize/
--rw-rw-r--   0 david     (1000) david     (1000)      361 2023-06-24 16:44:55.000000 pycognaize-1.4.8/pycognaize/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      210 2023-04-20 11:39:33.000000 pycognaize-1.4.8/pycognaize/cli.py
--rw-rw-r--   0 david     (1000) david     (1000)     2168 2023-01-20 10:59:34.000000 pycognaize-1.4.8/pycognaize/clidriver.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-24 16:48:31.370433 pycognaize-1.4.8/pycognaize/common/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-05-10 16:19:18.000000 pycognaize-1.4.8/pycognaize/common/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      968 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/common/classification_labels.py
--rw-rw-r--   0 david     (1000) david     (1000)      959 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/common/cloud_service.py
--rw-rw-r--   0 david     (1000) david     (1000)     2359 2023-03-09 16:00:53.000000 pycognaize-1.4.8/pycognaize/common/confidence.py
--rw-rw-r--   0 david     (1000) david     (1000)     2345 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/common/decorators.py
--rw-rw-r--   0 david     (1000) david     (1000)     5138 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/common/enums.py
--rw-rw-r--   0 david     (1000) david     (1000)      394 2023-01-20 10:59:34.000000 pycognaize-1.4.8/pycognaize/common/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)     1750 2023-01-20 10:59:34.000000 pycognaize-1.4.8/pycognaize/common/field_collection.py
--rw-rw-r--   0 david     (1000) david     (1000)     2352 2023-01-20 10:59:34.000000 pycognaize-1.4.8/pycognaize/common/lazy_dict.py
--rw-rw-r--   0 david     (1000) david     (1000)     2096 2023-01-20 10:59:34.000000 pycognaize-1.4.8/pycognaize/common/lazy_group_dict.py
--rw-rw-r--   0 david     (1000) david     (1000)     6826 2023-02-10 17:58:58.000000 pycognaize-1.4.8/pycognaize/common/numeric_parser.py
--rw-rw-r--   0 david     (1000) david     (1000)     3903 2023-05-02 20:13:15.000000 pycognaize-1.4.8/pycognaize/common/table_utils.py
--rw-rw-r--   0 david     (1000) david     (1000)    22922 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/common/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)      285 2023-01-20 10:59:34.000000 pycognaize-1.4.8/pycognaize/common/white_pixel.jpeg
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-24 16:48:31.370433 pycognaize-1.4.8/pycognaize/document/
--rw-rw-r--   0 david     (1000) david     (1000)      129 2023-01-20 10:59:34.000000 pycognaize-1.4.8/pycognaize/document/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    23603 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/document/document.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-24 16:48:31.370433 pycognaize-1.4.8/pycognaize/document/field/
--rw-rw-r--   0 david     (1000) david     (1000)      674 2023-05-10 14:14:12.000000 pycognaize-1.4.8/pycognaize/document/field/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3367 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/document/field/area_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     2818 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/document/field/date_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     3200 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/document/field/field.py
--rw-rw-r--   0 david     (1000) david     (1000)     3988 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/document/field/link_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     3965 2023-06-24 16:44:55.000000 pycognaize-1.4.8/pycognaize/document/field/numeric_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     4437 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/document/field/section_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     2825 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/document/field/span_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     5242 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/document/field/table_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     4051 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/document/field/text_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     2904 2023-05-10 14:14:12.000000 pycognaize-1.4.8/pycognaize/document/html_info.py
--rw-rw-r--   0 david     (1000) david     (1000)    22757 2023-06-21 13:11:18.000000 pycognaize-1.4.8/pycognaize/document/page.py
--rw-rw-r--   0 david     (1000) david     (1000)     3349 2023-05-02 20:13:15.000000 pycognaize-1.4.8/pycognaize/document/snapshot.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-24 16:48:31.370433 pycognaize-1.4.8/pycognaize/document/tag/
--rw-rw-r--   0 david     (1000) david     (1000)      116 2023-01-20 10:59:34.000000 pycognaize-1.4.8/pycognaize/document/tag/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3449 2023-01-20 10:59:34.000000 pycognaize-1.4.8/pycognaize/document/tag/cell.py
--rw-rw-r--   0 david     (1000) david     (1000)     6247 2023-06-21 13:11:18.000000 pycognaize-1.4.8/pycognaize/document/tag/extraction_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)    15408 2023-06-21 13:11:18.000000 pycognaize-1.4.8/pycognaize/document/tag/html_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)     2657 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/document/tag/section_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)     1794 2023-01-20 10:59:34.000000 pycognaize-1.4.8/pycognaize/document/tag/span_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)     8858 2023-01-20 10:59:34.000000 pycognaize-1.4.8/pycognaize/document/tag/table_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)    14977 2023-02-21 11:37:51.000000 pycognaize-1.4.8/pycognaize/document/tag/tag.py
--rw-rw-r--   0 david     (1000) david     (1000)     2863 2023-01-20 10:59:34.000000 pycognaize-1.4.8/pycognaize/index.py
--rw-rw-r--   0 david     (1000) david     (1000)     4004 2023-06-14 08:17:55.000000 pycognaize-1.4.8/pycognaize/login.py
--rw-rw-r--   0 david     (1000) david     (1000)    21992 2023-05-02 20:13:15.000000 pycognaize-1.4.8/pycognaize/model.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-24 16:48:31.370433 pycognaize-1.4.8/pycognaize/model_registry/
--rw-rw-r--   0 david     (1000) david     (1000)      133 2023-04-20 11:39:33.000000 pycognaize-1.4.8/pycognaize/model_registry/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-24 16:48:31.370433 pycognaize-1.4.8/pycognaize/model_registry/db/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-05-10 16:19:18.000000 pycognaize-1.4.8/pycognaize/model_registry/db/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      787 2023-04-20 11:39:33.000000 pycognaize-1.4.8/pycognaize/model_registry/db/models.py
--rw-rw-r--   0 david     (1000) david     (1000)      598 2023-04-20 11:39:33.000000 pycognaize-1.4.8/pycognaize/model_registry/login.py
--rw-rw-r--   0 david     (1000) david     (1000)     4687 2023-04-20 11:39:33.000000 pycognaize-1.4.8/pycognaize/model_registry/submit.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-24 16:48:31.370433 pycognaize-1.4.8/pycognaize.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)    33824 2023-06-24 16:48:31.000000 pycognaize-1.4.8/pycognaize.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1917 2023-06-24 16:48:31.000000 pycognaize-1.4.8/pycognaize.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-24 16:48:31.000000 pycognaize-1.4.8/pycognaize.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       53 2023-06-24 16:48:31.000000 pycognaize-1.4.8/pycognaize.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)      168 2023-06-24 16:48:31.000000 pycognaize-1.4.8/pycognaize.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       16 2023-06-24 16:48:31.000000 pycognaize-1.4.8/pycognaize.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      905 2023-06-24 16:48:31.370433 pycognaize-1.4.8/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     1005 2023-04-20 11:39:33.000000 pycognaize-1.4.8/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-24 16:48:31.370433 pycognaize-1.4.8/temp/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-21 16:35:59.000000 pycognaize-1.4.8/temp/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-21 16:36:11.000000 pycognaize-1.4.8/temp/temp.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-06-27 15:13:11.244490 pycognaize-1.4.9/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    32233 2023-06-27 15:11:14.000000 pycognaize-1.4.9/CHANGELOG.md
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    35137 2022-11-15 12:53:10.000000 pycognaize-1.4.9/LICENSE.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    34027 2023-06-27 15:13:11.244490 pycognaize-1.4.9/PKG-INFO
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1310 2023-06-06 11:32:18.000000 pycognaize-1.4.9/README.md
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-06-27 15:13:11.236490 pycognaize-1.4.9/pycognaize/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      361 2023-06-27 15:11:14.000000 pycognaize-1.4.9/pycognaize/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      210 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/cli.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2168 2023-01-11 08:15:39.000000 pycognaize-1.4.9/pycognaize/clidriver.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-06-27 15:13:11.240490 pycognaize-1.4.9/pycognaize/common/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 12:53:10.000000 pycognaize-1.4.9/pycognaize/common/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      968 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/common/classification_labels.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      959 2023-06-21 08:27:09.000000 pycognaize-1.4.9/pycognaize/common/cloud_service.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2359 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/common/confidence.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2345 2023-06-21 08:27:09.000000 pycognaize-1.4.9/pycognaize/common/decorators.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5671 2023-06-27 15:11:14.000000 pycognaize-1.4.9/pycognaize/common/enums.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      394 2022-12-06 11:01:27.000000 pycognaize-1.4.9/pycognaize/common/exceptions.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1750 2022-12-06 11:01:27.000000 pycognaize-1.4.9/pycognaize/common/field_collection.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     7761 2023-06-27 15:11:14.000000 pycognaize-1.4.9/pycognaize/common/langchain_loader.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2352 2022-12-06 11:01:27.000000 pycognaize-1.4.9/pycognaize/common/lazy_dict.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2096 2022-12-06 11:01:27.000000 pycognaize-1.4.9/pycognaize/common/lazy_group_dict.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6826 2023-06-20 14:23:46.000000 pycognaize-1.4.9/pycognaize/common/numeric_parser.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3903 2023-06-20 14:24:16.000000 pycognaize-1.4.9/pycognaize/common/table_utils.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    22922 2023-06-21 08:27:09.000000 pycognaize-1.4.9/pycognaize/common/utils.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      285 2022-11-15 12:53:10.000000 pycognaize-1.4.9/pycognaize/common/white_pixel.jpeg
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-06-27 15:13:11.240490 pycognaize-1.4.9/pycognaize/document/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      129 2022-11-15 12:53:10.000000 pycognaize-1.4.9/pycognaize/document/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    23603 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/document/document.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-06-27 15:13:11.240490 pycognaize-1.4.9/pycognaize/document/field/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      674 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/document/field/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3367 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/document/field/area_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2818 2023-06-20 14:23:46.000000 pycognaize-1.4.9/pycognaize/document/field/date_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3200 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/document/field/field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3996 2023-06-27 15:12:38.000000 pycognaize-1.4.9/pycognaize/document/field/link_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3965 2023-06-27 11:43:29.000000 pycognaize-1.4.9/pycognaize/document/field/numeric_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4437 2023-06-20 14:23:46.000000 pycognaize-1.4.9/pycognaize/document/field/section_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2825 2023-06-20 14:23:46.000000 pycognaize-1.4.9/pycognaize/document/field/span_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5242 2023-06-20 14:23:46.000000 pycognaize-1.4.9/pycognaize/document/field/table_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4051 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/document/field/text_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2904 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/document/html_info.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    22757 2023-06-27 11:43:17.000000 pycognaize-1.4.9/pycognaize/document/page.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3349 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/document/snapshot.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-06-27 15:13:11.244490 pycognaize-1.4.9/pycognaize/document/tag/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      116 2022-11-15 12:53:10.000000 pycognaize-1.4.9/pycognaize/document/tag/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3449 2022-11-15 12:53:10.000000 pycognaize-1.4.9/pycognaize/document/tag/cell.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6247 2023-06-21 08:27:09.000000 pycognaize-1.4.9/pycognaize/document/tag/extraction_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    15408 2023-06-21 08:27:09.000000 pycognaize-1.4.9/pycognaize/document/tag/html_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2657 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/document/tag/section_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1794 2022-12-06 11:01:27.000000 pycognaize-1.4.9/pycognaize/document/tag/span_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     9115 2023-06-27 15:11:14.000000 pycognaize-1.4.9/pycognaize/document/tag/table_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    14977 2023-05-29 14:03:01.000000 pycognaize-1.4.9/pycognaize/document/tag/tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2863 2022-11-15 12:53:10.000000 pycognaize-1.4.9/pycognaize/index.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4004 2023-06-21 08:27:09.000000 pycognaize-1.4.9/pycognaize/login.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    21992 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/model.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-06-27 15:13:11.244490 pycognaize-1.4.9/pycognaize/model_registry/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      133 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/model_registry/__init__.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-06-27 15:13:11.244490 pycognaize-1.4.9/pycognaize/model_registry/db/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/model_registry/db/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      787 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/model_registry/db/models.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      598 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/model_registry/login.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4687 2023-06-06 11:32:18.000000 pycognaize-1.4.9/pycognaize/model_registry/submit.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-06-27 15:13:11.240490 pycognaize-1.4.9/pycognaize.egg-info/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    34027 2023-06-27 15:13:11.000000 pycognaize-1.4.9/pycognaize.egg-info/PKG-INFO
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1925 2023-06-27 15:13:11.000000 pycognaize-1.4.9/pycognaize.egg-info/SOURCES.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        1 2023-06-27 15:13:11.000000 pycognaize-1.4.9/pycognaize.egg-info/dependency_links.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       53 2023-06-27 15:13:11.000000 pycognaize-1.4.9/pycognaize.egg-info/entry_points.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      213 2023-06-27 15:13:11.000000 pycognaize-1.4.9/pycognaize.egg-info/requires.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       11 2023-06-27 15:13:11.000000 pycognaize-1.4.9/pycognaize.egg-info/top_level.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      915 2023-06-27 15:13:11.244490 pycognaize-1.4.9/setup.cfg
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1095 2023-06-27 15:11:14.000000 pycognaize-1.4.9/setup.py
```

### Comparing `pycognaize-1.4.8/CHANGELOG.md` & `pycognaize-1.4.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Changelog
 
 ## [1.4]
 
+### [1.4.9] - 2023-06-27
+- Add `to_string()` functionality to `table_tags`
+- Add langchain_loader util to convert Pycognaize `Document` objects to Langchain `Document` objects
+
 ### [1.4.8] - 2023-06-24
 - Add field value and tag value to numeric field
 
 ### [1.4.7] - 2023-06-15
 - Add `ocr_tags()` and `line_tags()` to `Page`
 
-### [1.4.6] - 2023-06-15
+### [1.4.6] - 2023-06-27
 - Add replace_nans_with_empty_html_tags functionality in HTMLTableTag build df
 
 ### [1.4.5] - 2023-06-12
 - Add relogin when AWS token is expired
 
 ### [1.4.4] - 2023-05-31
 - Add `anytree` to setup-requires in `setup.cfg`
```

### Comparing `pycognaize-1.4.8/LICENSE.txt` & `pycognaize-1.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/PKG-INFO` & `pycognaize-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pycognaize
-Version: 1.4.8
+Version: 1.4.9
 Home-page: https://github.com/cognaize/pycognaize
 Author: Cognaize
 License: Apache License 2.0
 Project-URL: Source, https://github.com/cognaize/pycognaize
 Project-URL: Reference, https://pycognaize.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/cognaize/pycognaize/blob/master/CHANGELOG.md
 Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
+Provides-Extra: langchain
 License-File: LICENSE.txt
 
 <h1 align="center">
 <img src="https://github.com/cognaize/pycognaize/blob/master/media/logo/logo.png?raw=true" width="300">
 </h1><br>
 
 ![Package Version](https://github.com/cognaize/pycognaize/blob/master/media/badges/package_version.svg?raw=true)
@@ -45,21 +46,25 @@
 Have a look at the [quick tutorial](http://pycognaize-docs.com.s3-website.us-east-2.amazonaws.com/tutorials/quick_tutorial.html) 
 for understanding main concepts of the SDK.
 
 # Changelog
 
 ## [1.4]
 
+### [1.4.9] - 2023-06-27
+- Add `to_string()` functionality to `table_tags`
+- Add langchain_loader util to convert Pycognaize `Document` objects to Langchain `Document` objects
+
 ### [1.4.8] - 2023-06-24
 - Add field value and tag value to numeric field
 
 ### [1.4.7] - 2023-06-15
 - Add `ocr_tags()` and `line_tags()` to `Page`
 
-### [1.4.6] - 2023-06-15
+### [1.4.6] - 2023-06-27
 - Add replace_nans_with_empty_html_tags functionality in HTMLTableTag build df
 
 ### [1.4.5] - 2023-06-12
 - Add relogin when AWS token is expired
 
 ### [1.4.4] - 2023-05-31
 - Add `anytree` to setup-requires in `setup.cfg`
```

### Comparing `pycognaize-1.4.8/README.md` & `pycognaize-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/clidriver.py` & `pycognaize-1.4.9/pycognaize/clidriver.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/common/classification_labels.py` & `pycognaize-1.4.9/pycognaize/common/classification_labels.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/common/cloud_service.py` & `pycognaize-1.4.9/pycognaize/common/cloud_service.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/common/confidence.py` & `pycognaize-1.4.9/pycognaize/common/confidence.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/common/decorators.py` & `pycognaize-1.4.9/pycognaize/common/decorators.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/common/enums.py` & `pycognaize-1.4.9/pycognaize/common/enums.py`

 * *Files 20% similar despite different names*

```diff
@@ -220,7 +220,23 @@
     left_indentation = 'leftIndentation'
     anchor_id = 'anchorId'
     xpath = 'xpath'
     table = 'table'
     cells = 'cells'
     title = 'title'
     _id = '_id'
+
+
+class PageLayoutEnum(enum.Enum):
+    """Enum of page layout blocks, including tables"""
+    TEXT = 'page_layout__text'
+    # 'page_layout__picture'
+    CAPTION = 'page_layout__caption'
+    SECTION_HEADER = 'page_layout__section_header'
+    FOOTNOTE = 'page_layout__footnote'
+    FORMULA = 'page_layout__formula'
+    # 'page_layout__table'
+    LIST_ITEM = 'page_layout__list_item'
+    PAGE_HEADER = 'page_layout__page_header'
+    PAGE_FOOTER = 'page_layout__page_footer'
+    TITLE = 'page_layout__title'
+    TABLE = 'tables__table'
```

### Comparing `pycognaize-1.4.8/pycognaize/common/field_collection.py` & `pycognaize-1.4.9/pycognaize/common/field_collection.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/common/lazy_dict.py` & `pycognaize-1.4.9/pycognaize/common/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/common/lazy_group_dict.py` & `pycognaize-1.4.9/pycognaize/common/lazy_group_dict.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/common/numeric_parser.py` & `pycognaize-1.4.9/pycognaize/common/numeric_parser.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/common/table_utils.py` & `pycognaize-1.4.9/pycognaize/common/table_utils.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/common/utils.py` & `pycognaize-1.4.9/pycognaize/common/utils.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/document.py` & `pycognaize-1.4.9/pycognaize/document/document.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/field/__init__.py` & `pycognaize-1.4.9/pycognaize/document/field/__init__.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/field/area_field.py` & `pycognaize-1.4.9/pycognaize/document/field/area_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/field/date_field.py` & `pycognaize-1.4.9/pycognaize/document/field/date_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/field/field.py` & `pycognaize-1.4.9/pycognaize/document/field/field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/field/link_field.py` & `pycognaize-1.4.9/pycognaize/document/field/link_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 | The latter can have no tags, a single tag or multiple tags.
 
 >>> from pycognaize.document.field.link_field import LinkField
 >>> link_field = LinkField(name='URL', value='https://LinkField')
 >>> link_field.name
 'URL'
 >>> link_field.value
-'LinkField'
+'https://LinkField'
 >>> link_field.tags
 []
 """
 import logging
 from typing import List, Optional, Dict, Type
 
 from pycognaize.common.classification_labels import ClassificationLabels
```

### Comparing `pycognaize-1.4.8/pycognaize/document/field/numeric_field.py` & `pycognaize-1.4.9/pycognaize/document/field/numeric_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/field/section_field.py` & `pycognaize-1.4.9/pycognaize/document/field/section_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/field/span_field.py` & `pycognaize-1.4.9/pycognaize/document/field/span_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/field/table_field.py` & `pycognaize-1.4.9/pycognaize/document/field/table_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/field/text_field.py` & `pycognaize-1.4.9/pycognaize/document/field/text_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/html_info.py` & `pycognaize-1.4.9/pycognaize/document/html_info.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/page.py` & `pycognaize-1.4.9/pycognaize/document/page.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/snapshot.py` & `pycognaize-1.4.9/pycognaize/document/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/tag/cell.py` & `pycognaize-1.4.9/pycognaize/document/tag/cell.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/tag/extraction_tag.py` & `pycognaize-1.4.9/pycognaize/document/tag/extraction_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/tag/html_tag.py` & `pycognaize-1.4.9/pycognaize/document/tag/html_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/tag/section_tag.py` & `pycognaize-1.4.9/pycognaize/document/tag/section_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/tag/span_tag.py` & `pycognaize-1.4.9/pycognaize/document/tag/span_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/document/tag/table_tag.py` & `pycognaize-1.4.9/pycognaize/document/tag/table_tag.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import bson
 import string
 
 import pandas as pd
 from typing import Optional, Tuple
 
+from tabulate import tabulate
+
 from pycognaize.common.enums import (
     IqCellKeyEnum,
     IqTableTagEnum,
     IqTagKeyEnum,
     ID
 )
 from pycognaize.document.tag import ExtractionTag
@@ -114,14 +116,22 @@
             IqTagKeyEnum.value.value:
                 f"table on page {self.page.page_number}",
             IqTagKeyEnum.is_table.value: True,
             IqTableTagEnum.table.value: table_dict
         }
         return output_dict
 
+    def to_string(self) -> str:
+        """
+        Returns a string representation of the table
+        """
+        if self.df is None:
+            return ''
+        return tabulate(self.df, headers='keys', tablefmt='psql')
+
     def _populate_cells(self):
         for left_col_top_row, cell_dict in self.cell_data.items():
             keys = tuple((int(i) for i in left_col_top_row.split(':')))
             self._cells[keys] = (
                 self._populate_cell(keys=keys, cell_dict=cell_dict))
 
     @staticmethod
```

### Comparing `pycognaize-1.4.8/pycognaize/document/tag/tag.py` & `pycognaize-1.4.9/pycognaize/document/tag/tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/index.py` & `pycognaize-1.4.9/pycognaize/index.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/login.py` & `pycognaize-1.4.9/pycognaize/login.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/model.py` & `pycognaize-1.4.9/pycognaize/model.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/model_registry/db/models.py` & `pycognaize-1.4.9/pycognaize/model_registry/db/models.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/model_registry/login.py` & `pycognaize-1.4.9/pycognaize/model_registry/login.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize/model_registry/submit.py` & `pycognaize-1.4.9/pycognaize/model_registry/submit.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.8/pycognaize.egg-info/PKG-INFO` & `pycognaize-1.4.9/pycognaize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pycognaize
-Version: 1.4.8
+Version: 1.4.9
 Home-page: https://github.com/cognaize/pycognaize
 Author: Cognaize
 License: Apache License 2.0
 Project-URL: Source, https://github.com/cognaize/pycognaize
 Project-URL: Reference, https://pycognaize.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/cognaize/pycognaize/blob/master/CHANGELOG.md
 Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
+Provides-Extra: langchain
 License-File: LICENSE.txt
 
 <h1 align="center">
 <img src="https://github.com/cognaize/pycognaize/blob/master/media/logo/logo.png?raw=true" width="300">
 </h1><br>
 
 ![Package Version](https://github.com/cognaize/pycognaize/blob/master/media/badges/package_version.svg?raw=true)
@@ -45,21 +46,25 @@
 Have a look at the [quick tutorial](http://pycognaize-docs.com.s3-website.us-east-2.amazonaws.com/tutorials/quick_tutorial.html) 
 for understanding main concepts of the SDK.
 
 # Changelog
 
 ## [1.4]
 
+### [1.4.9] - 2023-06-27
+- Add `to_string()` functionality to `table_tags`
+- Add langchain_loader util to convert Pycognaize `Document` objects to Langchain `Document` objects
+
 ### [1.4.8] - 2023-06-24
 - Add field value and tag value to numeric field
 
 ### [1.4.7] - 2023-06-15
 - Add `ocr_tags()` and `line_tags()` to `Page`
 
-### [1.4.6] - 2023-06-15
+### [1.4.6] - 2023-06-27
 - Add replace_nans_with_empty_html_tags functionality in HTMLTableTag build df
 
 ### [1.4.5] - 2023-06-12
 - Add relogin when AWS token is expired
 
 ### [1.4.4] - 2023-05-31
 - Add `anytree` to setup-requires in `setup.cfg`
```

### Comparing `pycognaize-1.4.8/pycognaize.egg-info/SOURCES.txt` & `pycognaize-1.4.9/pycognaize.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 pycognaize/common/classification_labels.py
 pycognaize/common/cloud_service.py
 pycognaize/common/confidence.py
 pycognaize/common/decorators.py
 pycognaize/common/enums.py
 pycognaize/common/exceptions.py
 pycognaize/common/field_collection.py
+pycognaize/common/langchain_loader.py
 pycognaize/common/lazy_dict.py
 pycognaize/common/lazy_group_dict.py
 pycognaize/common/numeric_parser.py
 pycognaize/common/table_utils.py
 pycognaize/common/utils.py
 pycognaize/common/white_pixel.jpeg
 pycognaize/document/__init__.py
@@ -52,10 +53,8 @@
 pycognaize/document/tag/span_tag.py
 pycognaize/document/tag/table_tag.py
 pycognaize/document/tag/tag.py
 pycognaize/model_registry/__init__.py
 pycognaize/model_registry/login.py
 pycognaize/model_registry/submit.py
 pycognaize/model_registry/db/__init__.py
-pycognaize/model_registry/db/models.py
-temp/__init__.py
-temp/temp.py
+pycognaize/model_registry/db/models.py
```

### Comparing `pycognaize-1.4.8/setup.cfg` & `pycognaize-1.4.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 	urllib3
 	lxml
 	beautifulsoup4
 	dataclasses; python_version <= '3.6'
 	PyYAML
 	click
 	anytree
+	tabulate
 
 [options.packages.find]
 exclude = 
 	pycognaize.temp.*
 	pycognaize.temp
 	pycognaize.tests.*
 	pycognaize.tests
```

### Comparing `pycognaize-1.4.8/setup.py` & `pycognaize-1.4.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,13 +28,18 @@
         [console_scripts]
         cognaize=pycognaize.cli:cognaize''',
     project_urls={
         'Source': 'https://github.com/cognaize/pycognaize',
         'Reference': 'https://pycognaize.readthedocs.io/en/latest/',
         'Changelog': 'https://github.com/cognaize/pycognaize/blob/master/CHANGELOG.md',
     },
+    extras_require={
+            'langchain': ['langchain', 'transformers'],
+        },
 )
 
+
+
 setup_options['console'] = ['bin/cognaize']
 
 
 setup(**setup_options)
```

