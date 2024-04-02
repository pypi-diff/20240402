# Comparing `tmp/geopic_tag_reader-1.0.5.tar.gz` & `tmp/geopic_tag_reader-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopic_tag_reader-1.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geopic_tag_reader-1.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geopic_tag_reader-1.0.5.tar` & `geopic_tag_reader-1.0.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0       56 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/.gitignore
--rw-r--r--   0        0        0     1009 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/.gitlab-ci.yml
--rw-r--r--   0        0        0       91 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5952 2024-03-06 15:09:24.623622 geopic_tag_reader-1.0.5/CHANGELOG.md
--rw-r--r--   0        0        0     5468 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1070 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/LICENSE
--rw-r--r--   0        0        0      680 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/Makefile
--rw-r--r--   0        0        0     5243 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/README.md
--rw-r--r--   0        0        0       65 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/docs/.pages
--rw-r--r--   0        0        0     3393 2024-03-06 15:09:24.623622 geopic_tag_reader-1.0.5/docs/API_USAGE.md
--rw-r--r--   0        0        0     1835 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/docs/CLI_USAGE.md
--rw-r--r--   0        0        0      999 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/docs/Develop.md
--rw-r--r--   0        0        0     2015 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/docs/Install.md
--rw-r--r--   0        0        0     1066 2024-03-06 15:09:24.623622 geopic_tag_reader-1.0.5/docs/camera.md
--rw-r--r--   0        0        0      529 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/docs/model.md
--rw-r--r--   0        0        0     8772 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/docs/reader.md
--rw-r--r--   0        0        0     4301 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/docs/writer.md
--rw-r--r--   0        0        0       46 2024-03-06 15:09:24.623622 geopic_tag_reader-1.0.5/geopic_tag_reader/__init__.py
--rw-r--r--   0        0        0     1643 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/geopic_tag_reader/camera.py
--rw-r--r--   0        0        0     3129 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/geopic_tag_reader/main.py
--rw-r--r--   0        0        0      129 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/geopic_tag_reader/model.py
--rw-r--r--   0        0        0        0 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/geopic_tag_reader/py.typed
--rw-r--r--   0        0        0    21325 2024-03-06 15:06:48.384484 geopic_tag_reader-1.0.5/geopic_tag_reader/reader.py
--rw-r--r--   0        0        0     8680 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/geopic_tag_reader/writer.py
--rw-r--r--   0        0        0     1304 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/pyproject.toml
--rw-r--r--   0        0        0       37 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/pytest.ini
--rw-r--r--   0        0        0        0 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/tests/__init__.py
--rw-r--r--   0        0        0      195 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/tests/conftest.py
--rw-r--r--   0        0        0    79729 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.5/tests/fixtures/1.jpg
--rw-r--r--   0        0        0    24664 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/IMG_20210720_144918.jpg
--rw-r--r--   0        0        0    38766 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/IMG_20210720_161352.jpg
--rw-r--r--   0        0        0    75709 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/a1.jpg
--rw-r--r--   0        0        0    29130 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/b1.jpg
--rw-r--r--   0        0        0    39810 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/broken_makernotes.jpg
--rw-r--r--   0        0        0    69903 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/c1.jpg
--rw-r--r--   0        0        0    30503 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/cropped.jpg
--rw-r--r--   0        0        0    33446 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/d1.jpg
--rw-r--r--   0        0        0     5415 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/datetime_ms_float.jpg
--rw-r--r--   0        0        0    35109 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/datetime_offset.jpg
--rw-r--r--   0        0        0    51474 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/e1.jpg
--rw-r--r--   0        0        0    29141 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/flat.jpg
--rw-r--r--   0        0        0    70264 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/gopromax_flat.jpg
--rw-r--r--   0        0        0     4174 2024-03-06 15:06:48.384484 geopic_tag_reader-1.0.5/tests/fixtures/gps_date_slash.jpg
--rw-r--r--   0        0        0     5237 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/gps_date_time_stamp.jpg
--rw-r--r--   0        0        0    66264 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/img_Ricoh_Theta.jpg
--rw-r--r--   0        0        0     5360 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/img_V4MPack.jpg
--rw-r--r--   0        0        0    66961 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/img_categorisee.jpg
--rw-r--r--   0        0        0   135574 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/img_datetimeoriginal.jpg
--rw-r--r--   0        0        0    29503 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/img_gps_date_string.jpg
--rw-r--r--   0        0        0    35282 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/img_gps_datestamp.jpg
--rw-r--r--   0        0        0    43696 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.5/tests/fixtures/img_gps_sotm.jpg
--rw-r--r--   0        0        0    33170 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.5/tests/fixtures/img_invalid_gps_date.jpg
--rw-r--r--   0        0        0    34454 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.5/tests/fixtures/img_without_coord.jpg
--rw-r--r--   0        0        0    34518 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.5/tests/fixtures/img_without_dt.jpg
--rw-r--r--   0        0        0    12643 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.5/tests/fixtures/img_without_exif_tags.jpg
--rw-r--r--   0        0        0    11646 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.5/tests/fixtures/insta360_date.jpg
--rw-r--r--   0        0        0    55140 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.5/tests/fixtures/int_long_tag.jpg
--rw-r--r--   0        0        0    39169 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.5/tests/fixtures/out_of_bounds_lat.jpg
--rw-r--r--   0        0        0    39169 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.5/tests/fixtures/out_of_bounds_lon.jpg
--rw-r--r--   0        0        0     9665 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.5/tests/fixtures/pic_with_float_lat.jpg
--rw-r--r--   0        0        0     3130 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.5/tests/fixtures/ricoh_theta_no_projection.jpg
--rw-r--r--   0        0        0      612 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.5/tests/test_main.py
--rw-r--r--   0        0        0    21456 2024-03-06 15:06:48.384484 geopic_tag_reader-1.0.5/tests/test_reader.py
--rw-r--r--   0        0        0    11476 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.5/tests/test_writer.py
--rw-r--r--   0        0        0     6445 1970-01-01 00:00:00.000000 geopic_tag_reader-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0       56 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1009 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/.gitlab-ci.yml
+-rw-r--r--   0        0        0       91 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6218 2024-04-02 12:42:42.379304 geopic_tag_reader-1.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0     5468 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1070 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/LICENSE
+-rw-r--r--   0        0        0      676 2024-04-02 11:56:01.308379 geopic_tag_reader-1.0.6/Makefile
+-rw-r--r--   0        0        0     5243 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/README.md
+-rw-r--r--   0        0        0       65 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/docs/.pages
+-rw-r--r--   0        0        0     3410 2024-04-02 11:56:01.308379 geopic_tag_reader-1.0.6/docs/API_USAGE.md
+-rw-r--r--   0        0        0     1835 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/docs/CLI_USAGE.md
+-rw-r--r--   0        0        0      999 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/docs/Develop.md
+-rw-r--r--   0        0        0     2015 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/docs/Install.md
+-rw-r--r--   0        0        0     1066 2024-03-06 15:09:24.623622 geopic_tag_reader-1.0.6/docs/camera.md
+-rw-r--r--   0        0        0      543 2024-04-02 11:56:01.308379 geopic_tag_reader-1.0.6/docs/model.md
+-rw-r--r--   0        0        0     8772 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/docs/reader.md
+-rw-r--r--   0        0        0     4301 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/docs/writer.md
+-rw-r--r--   0        0        0       47 2024-04-02 12:42:42.379304 geopic_tag_reader-1.0.6/geopic_tag_reader/__init__.py
+-rw-r--r--   0        0        0     1643 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/geopic_tag_reader/camera.py
+-rw-r--r--   0        0        0     3129 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/geopic_tag_reader/main.py
+-rw-r--r--   0        0        0      129 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/geopic_tag_reader/model.py
+-rw-r--r--   0        0        0        0 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/geopic_tag_reader/py.typed
+-rw-r--r--   0        0        0    21325 2024-03-06 15:06:48.384484 geopic_tag_reader-1.0.6/geopic_tag_reader/reader.py
+-rw-r--r--   0        0        0     8680 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/geopic_tag_reader/writer.py
+-rw-r--r--   0        0        0     1142 2024-04-02 11:56:01.308379 geopic_tag_reader-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/pytest.ini
+-rw-r--r--   0        0        0        0 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      195 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/tests/conftest.py
+-rw-r--r--   0        0        0    79729 2024-02-20 08:18:06.536632 geopic_tag_reader-1.0.6/tests/fixtures/1.jpg
+-rw-r--r--   0        0        0    24664 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/IMG_20210720_144918.jpg
+-rw-r--r--   0        0        0    38766 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/IMG_20210720_161352.jpg
+-rw-r--r--   0        0        0    75709 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/a1.jpg
+-rw-r--r--   0        0        0    29130 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/b1.jpg
+-rw-r--r--   0        0        0    39810 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/broken_makernotes.jpg
+-rw-r--r--   0        0        0    69903 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/c1.jpg
+-rw-r--r--   0        0        0    30503 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/cropped.jpg
+-rw-r--r--   0        0        0    33446 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/d1.jpg
+-rw-r--r--   0        0        0     5415 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/datetime_ms_float.jpg
+-rw-r--r--   0        0        0    35109 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/datetime_offset.jpg
+-rw-r--r--   0        0        0    51474 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/e1.jpg
+-rw-r--r--   0        0        0    29141 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/flat.jpg
+-rw-r--r--   0        0        0    70264 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/gopromax_flat.jpg
+-rw-r--r--   0        0        0     4174 2024-03-06 15:06:48.384484 geopic_tag_reader-1.0.6/tests/fixtures/gps_date_slash.jpg
+-rw-r--r--   0        0        0     5237 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/gps_date_time_stamp.jpg
+-rw-r--r--   0        0        0    66264 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_Ricoh_Theta.jpg
+-rw-r--r--   0        0        0     5360 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_V4MPack.jpg
+-rw-r--r--   0        0        0    66961 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_categorisee.jpg
+-rw-r--r--   0        0        0   135574 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_datetimeoriginal.jpg
+-rw-r--r--   0        0        0    29503 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_gps_date_string.jpg
+-rw-r--r--   0        0        0    35282 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_gps_datestamp.jpg
+-rw-r--r--   0        0        0    43696 2024-02-20 08:18:06.540632 geopic_tag_reader-1.0.6/tests/fixtures/img_gps_sotm.jpg
+-rw-r--r--   0        0        0    33170 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/img_invalid_gps_date.jpg
+-rw-r--r--   0        0        0    34454 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/img_without_coord.jpg
+-rw-r--r--   0        0        0    34518 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/img_without_dt.jpg
+-rw-r--r--   0        0        0    12643 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/img_without_exif_tags.jpg
+-rw-r--r--   0        0        0    11646 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/insta360_date.jpg
+-rw-r--r--   0        0        0    55140 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/int_long_tag.jpg
+-rw-r--r--   0        0        0    39169 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/out_of_bounds_lat.jpg
+-rw-r--r--   0        0        0    39169 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/out_of_bounds_lon.jpg
+-rw-r--r--   0        0        0     9665 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/pic_with_float_lat.jpg
+-rw-r--r--   0        0        0     3130 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/fixtures/ricoh_theta_no_projection.jpg
+-rw-r--r--   0        0        0      612 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/test_main.py
+-rw-r--r--   0        0        0    21456 2024-04-02 11:56:01.308379 geopic_tag_reader-1.0.6/tests/test_reader.py
+-rw-r--r--   0        0        0    11476 2024-02-20 08:18:06.544632 geopic_tag_reader-1.0.6/tests/test_writer.py
+-rw-r--r--   0        0        0     6375 1970-01-01 00:00:00.000000 geopic_tag_reader-1.0.6/PKG-INFO
```

### Comparing `geopic_tag_reader-1.0.5/.gitlab-ci.yml` & `geopic_tag_reader-1.0.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/CHANGELOG.md` & `geopic_tag_reader-1.0.6/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,146 +1,163 @@
 # Changelog
+
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.0.6] - 2024-04-02
+
+### Changed
+
+- Bump some dependencies, the most important one being [typer](https://typer.tiangolo.com/) since it removes the need for typer-cli.
 
 ## [1.0.5] - 2024-03-06
 
 ### Fixed
+
 - Automatic detection of 360° pictures based on make and model also checks for image dimensions (to avoid false positive, when 360° camera can also take flat pictures).
 - Slash character in GPS date stamp was not correctly interpreted.
 
-
 ## [1.0.4] - 2024-02-12
 
 ### Changed
-- When using date/time not coming from GPS, offset time EXIF field are also read (`Exif.Photo.OffsetTimeOriginal` or `Exif.Photo.OffsetTime` depending on used date/time EXIF tag).
 
+- When using date/time not coming from GPS, offset time EXIF field are also read (`Exif.Photo.OffsetTimeOriginal` or `Exif.Photo.OffsetTime` depending on used date/time EXIF tag).
 
 ## [1.0.3] - 2023-12-18
 
 ### Added
+
 - Support reading date from EXIF fields `Exif.Image.DateTime` and `Xmp.GPano.SourceImageCreateTime`.
 - Auto-detect if a picture is 360° based on make and model.
 
 ### Fixed
-- Avoid failures for pictures with invalid offset for maker notes (due to PyExiv2 log level).
 
+- Avoid failures for pictures with invalid offset for maker notes (due to PyExiv2 log level).
 
 ## [1.0.2] - 2023-11-20
 
 ### Added
+
 - A warning is thrown when microseconds values between decimal seconds and sub-second time fields are not matching.
 
 ### Changed
-- Fraction values for date, time and GPS coordinates are supported.
 
+- Fraction values for date, time and GPS coordinates are supported.
 
 ## [1.0.1] - 2023-11-17
 
 ### Fixed
-- `DateTimeOriginal` field wasn't correctly read when seconds value was decimal.
 
+- `DateTimeOriginal` field wasn't correctly read when seconds value was decimal.
 
 ## [1.0.0] - 2023-10-18
 
 ### Added
+
 - Add subseconds to written metadata
 - Read altitude in metadata
 - Write direction and altitude metadata
 - Add `additional_exif` tags in `writePictureMetadata`
 
 ### Changed
-- EXIF list of tags now uses the [Exiv2](https://exiv2.org/metadata.html) notation (example `Exif.Image.Artist`) in returned data. To do this, pyexiv2 dependency is always necessary, and Pillow dependency has been removed. As a consequence, `readPictureMetadata` function __now takes in input `bytes`__ read from picture file instead of Pillow image. This is a breaking change.
-- Use overriden metadata is available to localize overriden capture_time
 
+- EXIF list of tags now uses the [Exiv2](https://exiv2.org/metadata.html) notation (example `Exif.Image.Artist`) in returned data. To do this, pyexiv2 dependency is always necessary, and Pillow dependency has been removed. As a consequence, `readPictureMetadata` function **now takes in input `bytes`** read from picture file instead of Pillow image. This is a breaking change.
+- Use overriden metadata is available to localize overriden capture_time
 
 ## [0.4.1] - 2023-09-08
 
 ### Added
-- Latitude and longitude values are checked to verify they fit into WGS84 projection bounds (-180, -90, 180, 90).
 
+- Latitude and longitude values are checked to verify they fit into WGS84 projection bounds (-180, -90, 180, 90).
 
 ## [0.4.0] - 2023-09-01
 
 ### Added
+
 - When a picture does not contain a mandatory exif tag (coordinates or datetime), a `PartialExifException` is thrown containing some information about what has been parsed and what is missing.
 
 ## [0.3.1] - 2023-07-31
 
 ### Added
+
 - A way to write exif lon/lat and type tags.
 
 ## [0.3.0] - 2023-07-31
 
 ### Added
+
 - Support of any date/time separator for EXIF tag `DateTimeOriginal`
 - A way to write exif tags. To use this, you need to install this library with the extra `[write-exif]`.
 
-
 ## [0.2.0] - 2023-07-13
 
 ### Added
+
 - Support of cropped equirectangular panoramas
 
 ### Changed
+
 - Support python 3.8
 
 ## [0.1.3]
 
 ### Changed
+
 - Bump [Typer](typer.tiangolo.com/) version, and use fork of [Typer-cli](https://gitlab.com/geovisio/infra/typer-cli)
 
 ## [0.1.2]
 
 ### Added
-- Full typing support ([PEP 484](https://peps.python.org/pep-0484/) and [PEP 561](https://peps.python.org/pep-0561/))
 
+- Full typing support ([PEP 484](https://peps.python.org/pep-0484/) and [PEP 561](https://peps.python.org/pep-0561/))
 
 ## [0.1.1]
 
 ### Added
-- Support of Mapillary tags stored in EXIF tag `ImageDescription`
 
+- Support of Mapillary tags stored in EXIF tag `ImageDescription`
 
 ## [0.1.0]
 
 ### Added
+
 - If GPS Date or time can't be read, fallbacks to Original Date EXIF tag associated with a reader warning
 - New EXIF tags are supported: `GPSDateTime`
 
 ### Changed
+
 - `tag_reader:warning` property has been moved from EXIF, and is now available as a direct property named `tagreader_warnings` of `GeoPicTags` class
 - Reader now supports `GPSLatitude` and `GPSLongitude` stored as decimal values instead of tuple
 - Reader now supports reading `FocalLength` written in `NUMBER/NUMBER` format
 - If EXIF tags for heading `PoseHeadingDegrees` and `GPSImgDirection` have contradicting values, we use by default `GPSImgDirection` value and issue a warning, instead of raising an error
 
 ### Fixed
-- EXIF tag `SubsecTimeOriginal` was not correctly read due to a typo
 
+- EXIF tag `SubsecTimeOriginal` was not correctly read due to a typo
 
 ## [0.0.2] - 2023-05-10
 
 ### Added
+
 - EXIF tag `UserComment` is now read and available in raw `exif` tags
 - If not set, `GPSLatitudeRef` defaults to North and `GPSLongitudeRef` defaults to East
 - A new `tag_reader:warning` property lists non-blocking warnings raised while reading EXIF tags
 
-
 ## [0.0.1] - 2023-03-31
 
 ### Added
-- EXIF tag reading methods extracted from [GeoVisio API](https://gitlab.com/geovisio/api)
 
+- EXIF tag reading methods extracted from [GeoVisio API](https://gitlab.com/geovisio/api)
 
-[Unreleased]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.5...main
+[Unreleased]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.6...main
+[1.0.6]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.5...1.0.6
 [1.0.5]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.4...1.0.5
 [1.0.4]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.3...1.0.4
 [1.0.3]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.2...1.0.3
 [1.0.2]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.1...1.0.2
 [1.0.1]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.0...1.0.1
 [1.0.0]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/0.4.1...1.0.0
 [0.4.1]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/0.4.0...0.4.1
```

### Comparing `geopic_tag_reader-1.0.5/CODE_OF_CONDUCT.md` & `geopic_tag_reader-1.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/LICENSE` & `geopic_tag_reader-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/Makefile` & `geopic_tag_reader-1.0.6/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 fmt: ## Format code
 	black --fast .
 
 ci: type-check fmt test ## Run all check like the ci
 
 docs:  ## Generates documentation from Typer embedded docs
-	python -m typer_cli ./geopic_tag_reader/main.py utils docs --name geopic-tag-reader --output docs/CLI_USAGE.md
+	python -m typer ./geopic_tag_reader/main.py utils docs --name geopic-tag-reader --output docs/CLI_USAGE.md
 	lazydocs --overview-file API_USAGE.md --ignored-modules main --output-path docs/ geopic_tag_reader/
 
 help: ## Print this help message
 	@grep -E '^[a-zA-Z_-]+:.*## .*$$' $(MAKEFILE_LIST) | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
```

### Comparing `geopic_tag_reader-1.0.5/README.md` & `geopic_tag_reader-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/docs/API_USAGE.md` & `geopic_tag_reader-1.0.6/docs/API_USAGE.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - [`camera`](./camera.md#module-camera)
 - [`model`](./model.md#module-model)
 - [`reader`](./reader.md#module-reader)
 - [`writer`](./writer.md#module-writer)
 
 ## Classes
 
-- [`model.PictureType`](./model.md#class-picturetype)
+- [`model.PictureType`](./model.md#class-picturetype): An enumeration.
 - [`reader.CropValues`](./reader.md#class-cropvalues): Cropped equirectangular pictures metadata
 - [`reader.GeoPicTags`](./reader.md#class-geopictags): Tags associated to a geolocated picture
 - [`reader.InvalidExifException`](./reader.md#class-invalidexifexception): Exception for invalid EXIF information from image
 - [`reader.PartialExifException`](./reader.md#class-partialexifexception): Exception for partial / missing EXIF information from image
 - [`reader.PartialGeoPicTags`](./reader.md#class-partialgeopictags): Tags associated to a geolocated picture when not all tags have been found
 - [`writer.Direction`](./writer.md#class-direction): Direction(value: float, ref: writer.DirectionRef = <DirectionRef.true_north: 'T'>)
 - [`writer.DirectionRef`](./writer.md#class-directionref): Indicates the reference for giving the direction of the image when it is captured.
```

### Comparing `geopic_tag_reader-1.0.5/docs/CLI_USAGE.md` & `geopic_tag_reader-1.0.6/docs/CLI_USAGE.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/docs/Develop.md` & `geopic_tag_reader-1.0.6/docs/Develop.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/docs/Install.md` & `geopic_tag_reader-1.0.6/docs/Install.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/docs/camera.md` & `geopic_tag_reader-1.0.6/docs/camera.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/docs/reader.md` & `geopic_tag_reader-1.0.6/docs/reader.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/docs/writer.md` & `geopic_tag_reader-1.0.6/docs/writer.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/geopic_tag_reader/camera.py` & `geopic_tag_reader-1.0.6/geopic_tag_reader/camera.py`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/geopic_tag_reader/main.py` & `geopic_tag_reader-1.0.6/geopic_tag_reader/main.py`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/geopic_tag_reader/reader.py` & `geopic_tag_reader-1.0.6/geopic_tag_reader/reader.py`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/geopic_tag_reader/writer.py` & `geopic_tag_reader-1.0.6/geopic_tag_reader/writer.py`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/pyproject.toml` & `geopic_tag_reader-1.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,36 +4,34 @@
     {name = "Adrien PAVIE", email = "panieravide@riseup.net"},
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 dependencies = [
-    "typer ~= 0.9.0",
-    "xmltodict ~= 0.13.0",
+    "typer ~= 0.12",
+    "xmltodict ~= 0.13",
     "pyexiv2 == 2.8.3",
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 Home = "https://gitlab.com/geovisio/geo-picture-tag-reader"
 
 [project.scripts]
 geopic-tag-reader="geopic_tag_reader.main:app"
 
 [project.optional-dependencies]
 dev = [
-    "black ~= 22.8.0",
-    "mypy ~= 1.0.0",
+    "black ~= 24.3",
+    "mypy ~= 1.9",
     "pytest ~= 7.2.0",
-    "pytest-datafiles ~= 2.0.1",
-    "typer-cli-forked ~= 0.0.14", # fork dependency needed until https://github.com/tiangolo/typer-cli/pull/120 is merged.
-    #"typer-cli ~= 0.0.13",
+    "pytest-datafiles ~= 3.0",
     "lazydocs ~= 0.4.8",
-    "types-xmltodict ~= 0.13.0",
+    "types-xmltodict ~= 0.13",
     "pre-commit ~= 3.3.3",
 ]
 build = ["flit ~= 3.8.0"]
 # optional dependencies to be able to write exif tags
 write-exif = [
     "timezonefinder == 6.2.0",
     "pytz ~= 2023.3",
```

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/1.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/IMG_20210720_144918.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/IMG_20210720_144918.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/IMG_20210720_161352.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/IMG_20210720_161352.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/a1.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/a1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/b1.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/b1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/broken_makernotes.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/broken_makernotes.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/c1.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/c1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/cropped.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/cropped.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/d1.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/d1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/datetime_ms_float.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/datetime_ms_float.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/datetime_offset.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/datetime_offset.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/e1.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/e1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/flat.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/flat.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/gopromax_flat.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/gopromax_flat.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/gps_date_slash.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/gps_date_slash.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/gps_date_time_stamp.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/gps_date_time_stamp.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/img_Ricoh_Theta.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/img_Ricoh_Theta.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/img_V4MPack.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/img_V4MPack.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/img_categorisee.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/img_categorisee.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/img_datetimeoriginal.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/img_datetimeoriginal.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/img_gps_date_string.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/img_gps_date_string.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/img_gps_datestamp.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/img_gps_datestamp.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/img_gps_sotm.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/img_gps_sotm.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/img_invalid_gps_date.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/img_invalid_gps_date.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/img_without_coord.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/img_without_coord.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/img_without_dt.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/img_without_dt.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/img_without_exif_tags.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/img_without_exif_tags.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/insta360_date.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/insta360_date.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/int_long_tag.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/int_long_tag.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/out_of_bounds_lat.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/out_of_bounds_lat.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/out_of_bounds_lon.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/out_of_bounds_lon.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/pic_with_float_lat.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/pic_with_float_lat.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/fixtures/ricoh_theta_no_projection.jpg` & `geopic_tag_reader-1.0.6/tests/fixtures/ricoh_theta_no_projection.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/test_main.py` & `geopic_tag_reader-1.0.6/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/tests/test_reader.py` & `geopic_tag_reader-1.0.6/tests/test_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
             "altitude": 34,
         },
     )
 
 
 @pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "img_Ricoh_Theta.jpg"))
 def test_readPictureMetadata_ricoh_theta(datafiles):
-    for f in datafiles.listdir():
+    for f in datafiles.iterdir():
         result = reader.readPictureMetadata(openImg(str(f)))
         assertGeoPicTagsEquals(
             result,
             {
                 "focal_length": 0.75,
                 "heading": 270,
                 "lat": 48.83930905577957,
@@ -158,15 +158,15 @@
                 "type": "equirectangular",
             },
         )
 
 
 @pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "img_V4MPack.jpg"))
 def test_readPictureMetadata_v4mpack(datafiles):
-    for f in datafiles.listdir():
+    for f in datafiles.iterdir():
         result = reader.readPictureMetadata(openImg(str(f)))
         assertGeoPicTagsEquals(
             result,
             {
                 "focal_length": None,
                 "heading": 64,
                 "lat": 47.08506017299737,
```

### Comparing `geopic_tag_reader-1.0.5/tests/test_writer.py` & `geopic_tag_reader-1.0.6/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.0.5/PKG-INFO` & `geopic_tag_reader-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: geopic-tag-reader
-Version: 1.0.5
+Version: 1.0.6
 Summary: GeoPicTagReader
 Author-email: Adrien PAVIE <panieravide@riseup.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: typer ~= 0.9.0
-Requires-Dist: xmltodict ~= 0.13.0
+Requires-Dist: typer ~= 0.12
+Requires-Dist: xmltodict ~= 0.13
 Requires-Dist: pyexiv2 == 2.8.3
 Requires-Dist: flit ~= 3.8.0 ; extra == "build"
-Requires-Dist: black ~= 22.8.0 ; extra == "dev"
-Requires-Dist: mypy ~= 1.0.0 ; extra == "dev"
+Requires-Dist: black ~= 24.3 ; extra == "dev"
+Requires-Dist: mypy ~= 1.9 ; extra == "dev"
 Requires-Dist: pytest ~= 7.2.0 ; extra == "dev"
-Requires-Dist: pytest-datafiles ~= 2.0.1 ; extra == "dev"
-Requires-Dist: typer-cli-forked ~= 0.0.14 ; extra == "dev"
+Requires-Dist: pytest-datafiles ~= 3.0 ; extra == "dev"
 Requires-Dist: lazydocs ~= 0.4.8 ; extra == "dev"
-Requires-Dist: types-xmltodict ~= 0.13.0 ; extra == "dev"
+Requires-Dist: types-xmltodict ~= 0.13 ; extra == "dev"
 Requires-Dist: pre-commit ~= 3.3.3 ; extra == "dev"
 Requires-Dist: timezonefinder == 6.2.0 ; extra == "write-exif"
 Requires-Dist: pytz ~= 2023.3 ; extra == "write-exif"
 Requires-Dist: types-pytz ~= 2023.3.0.1 ; extra == "write-exif"
 Requires-Dist: python-dateutil ~= 2.8.2 ; extra == "write-exif"
 Project-URL: Home, https://gitlab.com/geovisio/geo-picture-tag-reader
 Provides-Extra: build
```

