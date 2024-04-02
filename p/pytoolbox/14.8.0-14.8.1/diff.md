# Comparing `tmp/pytoolbox-14.8.0.tar.gz` & `tmp/pytoolbox-14.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytoolbox-14.8.0.tar", last modified: Mon Mar 25 15:38:06 2024, max compression
+gzip compressed data, was "pytoolbox-14.8.1.tar", last modified: Tue Apr  2 11:25:01 2024, max compression
```

## Comparing `pytoolbox-14.8.0.tar` & `pytoolbox-14.8.1.tar`

### file list

```diff
@@ -1,222 +1,222 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.660807 pytoolbox-14.8.0/
--rw-rw-r--   0 david     (1000) david     (1000)      219 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/AUTHORS.md
--rw-rw-r--   0 david     (1000) david     (1000)    32955 2024-03-25 15:37:35.000000 pytoolbox-14.8.0/CHANGELOG.md
--rw-rw-r--   0 david     (1000) david     (1000)     5747 2021-09-17 11:12:53.000000 pytoolbox-14.8.0/LICENSE.rst
--rw-rw-r--   0 david     (1000) david     (1000)       27 2023-06-08 07:35:27.000000 pytoolbox-14.8.0/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)    11167 2024-03-25 15:38:06.660807 pytoolbox-14.8.0/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     6529 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/README.rst
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.648806 pytoolbox-14.8.0/pytoolbox/
--rw-rw-r--   0 david     (1000) david     (1000)       23 2024-03-25 15:37:48.000000 pytoolbox-14.8.0/pytoolbox/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.648806 pytoolbox-14.8.0/pytoolbox/ai/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:53.000000 pytoolbox-14.8.0/pytoolbox/ai/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.648806 pytoolbox-14.8.0/pytoolbox/ai/vision/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/ai/vision/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.648806 pytoolbox-14.8.0/pytoolbox/ai/vision/face/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/ai/vision/face/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.648806 pytoolbox-14.8.0/pytoolbox/ai/vision/face/detect/
--rw-rw-r--   0 david     (1000) david     (1000)       67 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/ai/vision/face/detect/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     8925 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/ai/vision/face/detect/dlib.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.648806 pytoolbox-14.8.0/pytoolbox/ai/vision/face/recognize/
--rw-rw-r--   0 david     (1000) david     (1000)       97 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/ai/vision/face/recognize/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    11412 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/ai/vision/face/recognize/nn4_small2.py
--rw-rw-r--   0 david     (1000) david     (1000)      651 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/ai/vision/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)     3480 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/pytoolbox/argparse.py
--rw-rw-r--   0 david     (1000) david     (1000)     1738 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/atlassian.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.648806 pytoolbox-14.8.0/pytoolbox/aws/
--rw-rw-r--   0 david     (1000) david     (1000)       71 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/aws/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2768 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/aws/s3.py
--rw-rw-r--   0 david     (1000) david     (1000)    10212 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/collections.py
--rw-rw-r--   0 david     (1000) david     (1000)     4209 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/comparison.py
--rw-rw-r--   0 david     (1000) david     (1000)     5662 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/console.py
--rw-rw-r--   0 david     (1000) david     (1000)     6587 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/crypto.py
--rw-rw-r--   0 david     (1000) david     (1000)    12567 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/datetime.py
--rw-rw-r--   0 david     (1000) david     (1000)     5198 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/pytoolbox/decorators.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.648806 pytoolbox-14.8.0/pytoolbox/django/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.648806 pytoolbox-14.8.0/pytoolbox/django/core/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django/core/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      113 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/core/constants.py
--rw-rw-r--   0 david     (1000) david     (1000)     2628 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/core/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)     2586 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/django/core/validators.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django/forms/
--rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-08 07:35:27.000000 pytoolbox-14.8.0/pytoolbox/django/forms/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      728 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/forms/base.py
--rw-rw-r--   0 david     (1000) david     (1000)      563 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/forms/fields.py
--rw-rw-r--   0 david     (1000) david     (1000)     5349 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/forms/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)     3562 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/django/forms/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)      787 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/forms/widgets.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django/models/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django/models/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      412 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/models/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     1658 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/models/decorators.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django/models/fields/
--rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-08 07:35:27.000000 pytoolbox-14.8.0/pytoolbox/django/models/fields/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4157 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/models/fields/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     1299 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/models/fields/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django/models/managers/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django/models/managers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      773 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/models/managers/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      468 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/models/metaclass.py
--rw-rw-r--   0 david     (1000) david     (1000)    15204 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/models/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django/models/query/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django/models/query/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2555 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django/models/query/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)     1519 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/models/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django/signals/
--rw-rw-r--   0 david     (1000) david     (1000)       64 2023-06-08 07:35:27.000000 pytoolbox-14.8.0/pytoolbox/django/signals/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      541 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/signals/dispatch.py
--rw-rw-r--   0 david     (1000) david     (1000)     3780 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/signals/handlers.py
--rw-rw-r--   0 david     (1000) david     (1000)     1431 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/storage.py
--rw-rw-r--   0 david     (1000) david     (1000)    10687 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/templatetags.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django/test/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django/test/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4796 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/test/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django/test/runner/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django/test/runner/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      878 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/test/runner/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      614 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/urls.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django/utils/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django/utils/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2375 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/utils/collections.py
--rw-rw-r--   0 david     (1000) david     (1000)     1660 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/utils/logging.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django/views/
--rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-08 07:35:27.000000 pytoolbox-14.8.0/pytoolbox/django/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      511 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/views/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     4927 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/views/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      317 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django/views/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django_datatable_view/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django_datatable_view/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django_datatable_view/views/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django_datatable_view/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1767 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django_datatable_view/views/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django_filter/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django_filter/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django_filter/filterset/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django_filter/filterset/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      756 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/django_filter/filterset/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django_formtools/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django_formtools/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/django_formtools/views/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/django_formtools/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3091 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/django_formtools/views/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)     1618 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/enum.py
--rw-rw-r--   0 david     (1000) david     (1000)     6216 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/pytoolbox/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)    25670 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/filesystem.py
--rw-rw-r--   0 david     (1000) david     (1000)     3138 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/flask.py
--rw-rw-r--   0 david     (1000) david     (1000)     4195 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/pytoolbox/git.py
--rw-rw-r--   0 david     (1000) david     (1000)    11701 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/humanize.py
--rw-rw-r--   0 david     (1000) david     (1000)     2417 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/itertools.py
--rw-rw-r--   0 david     (1000) david     (1000)    49374 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/pytoolbox/juju.py
--rw-rw-r--   0 david     (1000) david     (1000)     1120 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/linux.py
--rw-rw-r--   0 david     (1000) david     (1000)     4837 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/pytoolbox/logging.py
--rw-rw-r--   0 david     (1000) david     (1000)      424 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/module.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/multimedia/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/multimedia/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/multimedia/exif/
--rw-rw-r--   0 david     (1000) david     (1000)      344 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/multimedia/exif/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1654 2024-03-13 08:15:09.000000 pytoolbox-14.8.0/pytoolbox/multimedia/exif/brand.py
--rw-rw-r--   0 david     (1000) david     (1000)      642 2023-06-21 06:37:24.000000 pytoolbox-14.8.0/pytoolbox/multimedia/exif/camera.py
--rw-rw-r--   0 david     (1000) david     (1000)     1149 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/multimedia/exif/equipment.py
--rw-rw-r--   0 david     (1000) david     (1000)     1914 2023-06-21 06:37:24.000000 pytoolbox-14.8.0/pytoolbox/multimedia/exif/image.py
--rw-rw-r--   0 david     (1000) david     (1000)      907 2024-03-13 08:18:08.000000 pytoolbox-14.8.0/pytoolbox/multimedia/exif/lens.py
--rw-rw-r--   0 david     (1000) david     (1000)     2549 2024-03-13 08:18:10.000000 pytoolbox-14.8.0/pytoolbox/multimedia/exif/metadata.py
--rw-rw-r--   0 david     (1000) david     (1000)     1847 2024-03-13 08:18:12.000000 pytoolbox-14.8.0/pytoolbox/multimedia/exif/photo.py
--rw-rw-r--   0 david     (1000) david     (1000)     3913 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/multimedia/exif/tag.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/multimedia/ffmpeg/
--rw-rw-r--   0 david     (1000) david     (1000)      672 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/multimedia/ffmpeg/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     7270 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/multimedia/ffmpeg/encode.py
--rw-rw-r--   0 david     (1000) david     (1000)     5898 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/multimedia/ffmpeg/ffmpeg.py
--rw-rw-r--   0 david     (1000) david     (1000)     8566 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/multimedia/ffmpeg/ffprobe.py
--rw-rw-r--   0 david     (1000) david     (1000)     9639 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/multimedia/ffmpeg/miscellaneous.py
--rw-rw-r--   0 david     (1000) david     (1000)     1809 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/multimedia/ffmpeg/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/multimedia/image/
--rw-rw-r--   0 david     (1000) david     (1000)     2302 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/multimedia/image/PIL.py
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/multimedia/image/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1699 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/multimedia/x264.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/network/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/network/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    11608 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/network/http.py
--rw-rw-r--   0 david     (1000) david     (1000)     1151 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/network/ip.py
--rw-rw-r--   0 david     (1000) david     (1000)    15654 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/network/rtp.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/network/smpte2022/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/network/smpte2022/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    27737 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/network/smpte2022/base.py
--rw-rw-r--   0 david     (1000) david     (1000)    10420 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/network/smpte2022/generator.py
--rw-rw-r--   0 david     (1000) david     (1000)    27854 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/network/smpte2022/receiver.py
--rw-rw-r--   0 david     (1000) david     (1000)      916 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/network/url.py
--rw-rw-r--   0 david     (1000) david     (1000)      527 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/pandas.py
--rw-rw-r--   0 david     (1000) david     (1000)      466 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/private.py
--rw-rw-r--   0 david     (1000) david     (1000)     5048 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/pytoolbox/regex.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/rest_framework/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/rest_framework/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/rest_framework/metadata/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/rest_framework/metadata/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1110 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/rest_framework/metadata/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      717 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/rest_framework/permissions.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/rest_framework/serializers/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/rest_framework/serializers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      777 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/rest_framework/serializers/fields.py
--rw-rw-r--   0 david     (1000) david     (1000)     2238 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/rest_framework/serializers/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.652807 pytoolbox-14.8.0/pytoolbox/rest_framework/views/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.8.0/pytoolbox/rest_framework/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1571 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/rest_framework/views/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.656807 pytoolbox-14.8.0/pytoolbox/selenium/
--rw-rw-r--   0 david     (1000) david     (1000)      149 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/selenium/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3349 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/selenium/client.py
--rw-rw-r--   0 david     (1000) david     (1000)     1343 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/selenium/common.py
--rw-rw-r--   0 david     (1000) david     (1000)      464 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/selenium/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)      266 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/selenium/select.py
--rw-rw-r--   0 david     (1000) david     (1000)     2643 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/selenium/test.py
--rw-rw-r--   0 david     (1000) david     (1000)      815 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/selenium/webdrivers.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.656807 pytoolbox-14.8.0/pytoolbox/selenium/webelements/
--rw-rw-r--   0 david     (1000) david     (1000)      186 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/selenium/webelements/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1109 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/selenium/webelements/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     1030 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/selenium/webelements/bootstrap_slider.py
--rw-rw-r--   0 david     (1000) david     (1000)      473 2023-06-08 07:35:27.000000 pytoolbox-14.8.0/pytoolbox/selenium/webelements/bootstrap_switch.py
--rw-rw-r--   0 david     (1000) david     (1000)    21142 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/pytoolbox/serialization.py
--rw-rw-r--   0 david     (1000) david     (1000)      452 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/setuptools.py
--rw-rw-r--   0 david     (1000) david     (1000)     1650 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/signals.py
--rw-rw-r--   0 david     (1000) david     (1000)     3407 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/pytoolbox/ssh.py
--rw-rw-r--   0 david     (1000) david     (1000)     2875 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/states.py
--rw-rw-r--   0 david     (1000) david     (1000)     4864 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/string.py
--rw-rw-r--   0 david     (1000) david     (1000)    12862 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/pytoolbox/subprocess.py
--rw-rw-r--   0 david     (1000) david     (1000)     3407 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/throttles.py
--rw-rw-r--   0 david     (1000) david     (1000)     8981 2024-03-25 07:36:04.000000 pytoolbox-14.8.0/pytoolbox/types.py
--rw-rw-r--   0 david     (1000) david     (1000)    10931 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/pytoolbox/unittest.py
--rw-rw-r--   0 david     (1000) david     (1000)     9568 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/validation.py
--rw-rw-r--   0 david     (1000) david     (1000)     1164 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/virtualenv.py
--rw-rw-r--   0 david     (1000) david     (1000)     2160 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/pytoolbox/voluptuous.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.656807 pytoolbox-14.8.0/pytoolbox.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)    11167 2024-03-25 15:38:06.000000 pytoolbox-14.8.0/pytoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     5548 2024-03-25 15:38:06.000000 pytoolbox-14.8.0/pytoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2024-03-25 15:38:06.000000 pytoolbox-14.8.0/pytoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)     1042 2024-03-25 15:38:06.000000 pytoolbox-14.8.0/pytoolbox.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       10 2024-03-25 15:38:06.000000 pytoolbox-14.8.0/pytoolbox.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      144 2024-03-25 15:38:06.660807 pytoolbox-14.8.0/setup.cfg
--rwxrwxr-x   0 david     (1000) david     (1000)     8796 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-25 15:38:06.656807 pytoolbox-14.8.0/tests/
--rw-rw-r--   0 david     (1000) david     (1000)     1067 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_argparse.py
--rw-rw-r--   0 david     (1000) david     (1000)     1237 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_collections.py
--rw-rw-r--   0 david     (1000) david     (1000)     4689 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_comparison.py
--rw-rw-r--   0 david     (1000) david     (1000)      832 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_console.py
--rw-rw-r--   0 david     (1000) david     (1000)      514 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_decorators.py
--rw-rw-r--   0 david     (1000) david     (1000)      668 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_django_utils.py
--rw-rw-r--   0 david     (1000) david     (1000)     1186 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/tests/test_exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)    16098 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_ffmpeg.py
--rw-rw-r--   0 david     (1000) david     (1000)     2555 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_filesystem.py
--rw-rw-r--   0 david     (1000) david     (1000)     4996 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/tests/test_git.py
--rw-rw-r--   0 david     (1000) david     (1000)     2887 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_juju.py
--rw-rw-r--   0 david     (1000) david     (1000)      760 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/tests/test_logging.py
--rw-rw-r--   0 david     (1000) david     (1000)      705 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_module.py
--rw-rw-r--   0 david     (1000) david     (1000)      692 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_private.py
--rw-rw-r--   0 david     (1000) david     (1000)     2068 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/tests/test_regex.py
--rw-rw-r--   0 david     (1000) david     (1000)     1679 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_serialization.py
--rw-rw-r--   0 david     (1000) david     (1000)     2699 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_signals.py
--rw-rw-r--   0 david     (1000) david     (1000)     4525 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/tests/test_ssh.py
--rw-rw-r--   0 david     (1000) david     (1000)     4125 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_states.py
--rw-rw-r--   0 david     (1000) david     (1000)     2873 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_string.py
--rw-rw-r--   0 david     (1000) david     (1000)     4437 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/tests/test_subprocess.py
--rw-rw-r--   0 david     (1000) david     (1000)      338 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_types.py
--rw-rw-r--   0 david     (1000) david     (1000)     5981 2024-03-25 15:20:56.000000 pytoolbox-14.8.0/tests/test_unittest.py
--rw-rw-r--   0 david     (1000) david     (1000)      637 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_validation.py
--rw-rw-r--   0 david     (1000) david     (1000)      433 2024-03-21 16:14:37.000000 pytoolbox-14.8.0/tests/test_x264.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.357379 pytoolbox-14.8.1/
+-rw-rw-r--   0 david     (1000) david     (1000)      219 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/AUTHORS.md
+-rw-rw-r--   0 david     (1000) david     (1000)    35196 2024-04-02 11:17:18.000000 pytoolbox-14.8.1/CHANGELOG.md
+-rw-rw-r--   0 david     (1000) david     (1000)     5747 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/LICENSE.rst
+-rw-rw-r--   0 david     (1000) david     (1000)       27 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)    11167 2024-04-02 11:25:01.357379 pytoolbox-14.8.1/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     6529 2024-03-26 07:35:12.000000 pytoolbox-14.8.1/README.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.257378 pytoolbox-14.8.1/pytoolbox/
+-rw-rw-r--   0 david     (1000) david     (1000)      467 2024-04-02 11:17:33.000000 pytoolbox-14.8.1/pytoolbox/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.257378 pytoolbox-14.8.1/pytoolbox/ai/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.261378 pytoolbox-14.8.1/pytoolbox/ai/vision/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.261378 pytoolbox-14.8.1/pytoolbox/ai/vision/face/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/face/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.261378 pytoolbox-14.8.1/pytoolbox/ai/vision/face/detect/
+-rw-rw-r--   0 david     (1000) david     (1000)       67 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/face/detect/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8925 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/face/detect/dlib.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.261378 pytoolbox-14.8.1/pytoolbox/ai/vision/face/recognize/
+-rw-rw-r--   0 david     (1000) david     (1000)       97 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/face/recognize/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11412 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/face/recognize/nn4_small2.py
+-rw-rw-r--   0 david     (1000) david     (1000)      651 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7959 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/argparse.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1738 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/atlassian.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.261378 pytoolbox-14.8.1/pytoolbox/aws/
+-rw-rw-r--   0 david     (1000) david     (1000)       71 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/aws/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2768 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/aws/s3.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10212 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/collections.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4223 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/comparison.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6412 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/console.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6587 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/crypto.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12567 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/datetime.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5427 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/decorators.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.265378 pytoolbox-14.8.1/pytoolbox/django/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.265378 pytoolbox-14.8.1/pytoolbox/django/core/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/core/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      113 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/core/constants.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2628 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/core/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2582 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/core/validators.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.269378 pytoolbox-14.8.1/pytoolbox/django/forms/
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/forms/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      728 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/forms/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)      563 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/forms/fields.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5345 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/forms/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3562 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/forms/utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)      787 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/forms/widgets.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.273378 pytoolbox-14.8.1/pytoolbox/django/models/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      412 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1658 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/decorators.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.273378 pytoolbox-14.8.1/pytoolbox/django/models/fields/
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/fields/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4157 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/fields/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1299 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/fields/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.273378 pytoolbox-14.8.1/pytoolbox/django/models/managers/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/managers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      773 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/managers/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      468 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/metaclass.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15196 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/models/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.277378 pytoolbox-14.8.1/pytoolbox/django/models/query/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/query/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2555 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/query/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1511 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/models/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.277378 pytoolbox-14.8.1/pytoolbox/django/signals/
+-rw-rw-r--   0 david     (1000) david     (1000)       64 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/signals/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      541 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/signals/dispatch.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3796 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/signals/handlers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1426 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/storage.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10688 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/templatetags.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.277378 pytoolbox-14.8.1/pytoolbox/django/test/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/test/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4796 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/test/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.281378 pytoolbox-14.8.1/pytoolbox/django/test/runner/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/test/runner/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      878 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/test/runner/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      614 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/urls.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.281378 pytoolbox-14.8.1/pytoolbox/django/utils/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/utils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2375 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/utils/collections.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1660 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/utils/logging.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.281378 pytoolbox-14.8.1/pytoolbox/django/views/
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      511 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/views/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4927 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/views/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      317 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/views/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.285378 pytoolbox-14.8.1/pytoolbox/django_datatable_view/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_datatable_view/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.285378 pytoolbox-14.8.1/pytoolbox/django_datatable_view/views/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_datatable_view/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1767 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_datatable_view/views/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.285378 pytoolbox-14.8.1/pytoolbox/django_filter/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_filter/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.285378 pytoolbox-14.8.1/pytoolbox/django_filter/filterset/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_filter/filterset/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      752 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django_filter/filterset/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.285378 pytoolbox-14.8.1/pytoolbox/django_formtools/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_formtools/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.289378 pytoolbox-14.8.1/pytoolbox/django_formtools/views/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_formtools/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3091 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_formtools/views/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1570 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/enum.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6445 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    25984 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/filesystem.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3134 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/flask.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4203 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/git.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11833 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/humanize.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2417 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/itertools.py
+-rw-rw-r--   0 david     (1000) david     (1000)    49307 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/juju.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1120 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/linux.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5533 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/logging.py
+-rw-rw-r--   0 david     (1000) david     (1000)      424 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/module.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.289378 pytoolbox-14.8.1/pytoolbox/multimedia/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.293378 pytoolbox-14.8.1/pytoolbox/multimedia/exif/
+-rw-rw-r--   0 david     (1000) david     (1000)      344 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1654 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/brand.py
+-rw-rw-r--   0 david     (1000) david     (1000)      642 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/camera.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1145 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/equipment.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1914 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/image.py
+-rw-rw-r--   0 david     (1000) david     (1000)      907 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/lens.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2579 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/metadata.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1847 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/photo.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3909 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/tag.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.301378 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/
+-rw-rw-r--   0 david     (1000) david     (1000)      672 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7270 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/encode.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5898 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/ffmpeg.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8566 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/ffprobe.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9639 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/miscellaneous.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1809 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.301378 pytoolbox-14.8.1/pytoolbox/multimedia/image/
+-rw-rw-r--   0 david     (1000) david     (1000)     2302 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/image/PIL.py
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/image/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1699 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/x264.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.305378 pytoolbox-14.8.1/pytoolbox/network/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11608 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/http.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1151 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/ip.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15650 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/network/rtp.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.305378 pytoolbox-14.8.1/pytoolbox/network/smpte2022/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/smpte2022/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    27733 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/network/smpte2022/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10420 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/smpte2022/generator.py
+-rw-rw-r--   0 david     (1000) david     (1000)    27854 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/smpte2022/receiver.py
+-rw-rw-r--   0 david     (1000) david     (1000)      916 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/url.py
+-rw-rw-r--   0 david     (1000) david     (1000)      527 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/pandas.py
+-rw-rw-r--   0 david     (1000) david     (1000)      466 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/private.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5330 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/regex.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.309378 pytoolbox-14.8.1/pytoolbox/rest_framework/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.309378 pytoolbox-14.8.1/pytoolbox/rest_framework/metadata/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/metadata/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1106 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/metadata/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      717 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/permissions.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.309378 pytoolbox-14.8.1/pytoolbox/rest_framework/serializers/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/serializers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      777 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/serializers/fields.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2238 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/serializers/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.313378 pytoolbox-14.8.1/pytoolbox/rest_framework/views/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1571 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/views/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.317378 pytoolbox-14.8.1/pytoolbox/selenium/
+-rw-rw-r--   0 david     (1000) david     (1000)      149 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3349 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/client.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1343 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/common.py
+-rw-rw-r--   0 david     (1000) david     (1000)      464 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)      266 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/select.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2631 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/selenium/test.py
+-rw-rw-r--   0 david     (1000) david     (1000)      815 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/webdrivers.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.317378 pytoolbox-14.8.1/pytoolbox/selenium/webelements/
+-rw-rw-r--   0 david     (1000) david     (1000)      186 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/webelements/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1109 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/webelements/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1030 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/webelements/bootstrap_slider.py
+-rw-rw-r--   0 david     (1000) david     (1000)      473 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/webelements/bootstrap_switch.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21143 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/serialization.py
+-rw-rw-r--   0 david     (1000) david     (1000)      452 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/setuptools.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1650 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/signals.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3402 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/ssh.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2875 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/states.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4864 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/string.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13522 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/subprocess.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3407 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/throttles.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8965 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/types.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10931 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/unittest.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9644 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/validation.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1164 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/virtualenv.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2160 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/voluptuous.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.333378 pytoolbox-14.8.1/pytoolbox.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)    11167 2024-04-02 11:25:01.000000 pytoolbox-14.8.1/pytoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     5548 2024-04-02 11:25:01.000000 pytoolbox-14.8.1/pytoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2024-04-02 11:25:01.000000 pytoolbox-14.8.1/pytoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)     1042 2024-04-02 11:25:01.000000 pytoolbox-14.8.1/pytoolbox.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       10 2024-04-02 11:25:01.000000 pytoolbox-14.8.1/pytoolbox.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      144 2024-04-02 11:25:01.357379 pytoolbox-14.8.1/setup.cfg
+-rwxrwxr-x   0 david     (1000) david     (1000)     8796 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.333378 pytoolbox-14.8.1/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)     2961 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/tests/test_argparse.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1237 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_collections.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4691 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/tests/test_comparison.py
+-rw-rw-r--   0 david     (1000) david     (1000)      832 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_console.py
+-rw-rw-r--   0 david     (1000) david     (1000)      514 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_decorators.py
+-rw-rw-r--   0 david     (1000) david     (1000)      668 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_django_utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2185 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/tests/test_exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16098 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_ffmpeg.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2555 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_filesystem.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5059 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/tests/test_git.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2887 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_juju.py
+-rw-rw-r--   0 david     (1000) david     (1000)      813 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/tests/test_logging.py
+-rw-rw-r--   0 david     (1000) david     (1000)      705 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_module.py
+-rw-rw-r--   0 david     (1000) david     (1000)      692 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_private.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2068 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_regex.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1679 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_serialization.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2699 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_signals.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4525 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_ssh.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4125 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_states.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2873 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_string.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6002 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/tests/test_subprocess.py
+-rw-rw-r--   0 david     (1000) david     (1000)      338 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_types.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5981 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_unittest.py
+-rw-rw-r--   0 david     (1000) david     (1000)      637 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_validation.py
+-rw-rw-r--   0 david     (1000) david     (1000)      433 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_x264.py
```

### Comparing `pytoolbox-14.8.0/CHANGELOG.md` & `pytoolbox-14.8.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,63 @@
 # Changelog
 
 Roadmap ? Not so, but you can check this: https://github.com/davidfischer-ch/pytoolbox/issues
 
+## v14.8.1 (2024-04-02)
+
+Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.8.0...14.8.1
+
+### Deprecations
+
+* Replace your calls to `argparse.set_columns` by `console.set_columns`
+* Replace your calls to `argparse.HelpArgumentParser` by `argparse.ArgumentParser`
+* Replace your calls to `filesystem.recursive_copy` by `filesystem.copy_recursive`
+* Replace your calls to `subprocess.git_clone_or_pull` by `git.clone_or_pull`
+* Replace your calls to `subprocess.ssh` by `ssh.ssh`
+
+### Features
+
+* Prevent `pytoolbox` logged events being output to `sys.stderr` by registering a `NullHandler`
+* Add class `argparse.ChainAction` (argument parsing action)
+* Add function `argparse.separator` (argument parsing type)
+* Add function `arpgarse.env_default` (utility function)
+* Add convenient constants `DIRECTORY_ARGS`, `FILE_ARG`, `REMAINDER_ARG` and `MULTI_ARG()` (`arpgarse` module)
+* Add class `argparse.ArgumentParser` (renamed from `argparse.HelpArgumentParser`)
+* Add class `argparse.ActionArgumentParser`
+* Add TypeAlias `Color`
+* Expose `arpgarse.{ArgumentTypeError,Namespace}` to be convenient (`import argparse` not required)
+* Decorator `decorators.deprecated` now accept a `guideline` argument (default to `''`)
+* Expose `logging.{CRITICAL, ..., NOTSET}`, `logging.{Logger, LogRecord}` to be convenient (`import logging` not required)
+* Add TypedDict `subprocess.CallResult` and use it to type hint functions response (added `exception` key)
+* Function `subprocess.cmd`: Now logging to `pytoolbox.subprocess.cmd.<binary>` unless log is defined
+* Function `subprocess.cmd`: Log can be a function, a `Logger` or a `str`. `None` will be mapped to default behavior
+
+### Fix and enhancements
+
+* Favor `type(obj)` over `obj.__class__`
+* Class `exceptions.MessageMixin`: Now show missing attributes (attributes can be properties too)
+* Class `exceptions.CalledProcessError`: Add property `cmd_short` and prevent exposing sensitive data in `__str__` or `__repr__`
+* Fix calls to `yaml.dump` (as its now `ruamel.yaml`)
+* Various improvements such as type hints, documentation, tests
+
 ## v14.8.0 (2024-03-25)
 
 Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.7.0...14.8.0
 
 ### Minor compatibility breaks
 
 * Replace `subprocess.CalledProcessError` by `exceptions.CalledProcessError` (keep a deprecated alias)
-* Rename function `subprocess.git_clone_or_pull` to `ssh.clone_or_pull`
+* Rename function `subprocess.git_clone_or_pull` to `ssh.clone_or_pull` (keep a deprecated alias)
+* Rename function `subprocess.ssh` to `ssh.ssh` (keep a deprecated alias)
 * Rename TypeAlias `subprocess.LoggerType` to `logging.LoggerType`
 
 ### Deprecations
 
-* Replace your call to `subprocess.git_clone_or_pull` by `ssh.clone_or_pull`
+* Replace your calls to `subprocess.git_clone_or_pull` by `ssh.clone_or_pull`
+* Rename function `subprocess.ssh` by `ssh.ssh`
 
 ### Features
 
 * Add module `git`
 * Add module `ssh`
 * Add class `exceptions.CalledProcessError`
 * Add class `exceptions.DuplicateGitTagError`
@@ -65,15 +104,15 @@
 * Method `module.All.diff`: Drop argument `to_type`
 * Function `network.http.download_ext_multi`: Argument `resources` must now be an iterable of `Resource`
 * Functions `validation.valid_*`: Do not accept `None` anymore
 * Rename function `filesystem.recursive_copy` to `filesystem.copy_recursive` (keep a deprecated alias)
 
 ### Deprecations
 
-* Replace your call to `filesystem.copy_recursive` by `filesystem.recursive_copy`
+* Replace your calls to `filesystem.copy_recursive` by `filesystem.recursive_copy`
 
 ### Features
 
 * Type hint a massive portion of code (and import annotations from __future__)!
 * Ensure Python 3.11 & 3.12 compatibility
 * Add optional MongoDB feature (`mongodb` extra)
 * Add class `argparse.Namespace`
```

### Comparing `pytoolbox-14.8.0/LICENSE.rst` & `pytoolbox-14.8.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/PKG-INFO` & `pytoolbox-14.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoolbox
-Version: 14.8.0
+Version: 14.8.1
 Summary: Toolbox for Python scripts
 Home-page: https://github.com/davidfischer-ch/pytoolbox
 Author: David Fischer
 Author-email: david@fisch3r.net
 License: EUPL 1.1
 Keywords: celery,ffmpeg,django,flask,json,juju,mock,pillow,rsync,rtp,selenium,smpte 2022-1,screen,subprocess
 Classifier: Development Status :: 5 - Production/Stable
@@ -290,8 +290,8 @@
 		  packages=['my_cool_project'])
 
 
 See `pip vcs support <http://www.pip-installer.org/en/latest/logic.html#vcs-support>`_ to get further details about this.
 
 You also need to install ``git-core``, but it is probably already the case, at least on your development computer ;-)
 
-2014 - 2022 David Fischer
+2012 - 2024 David Fischer
```

### Comparing `pytoolbox-14.8.0/README.rst` & `pytoolbox-14.8.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -174,8 +174,8 @@
 		  packages=['my_cool_project'])
 
 
 See `pip vcs support <http://www.pip-installer.org/en/latest/logic.html#vcs-support>`_ to get further details about this.
 
 You also need to install ``git-core``, but it is probably already the case, at least on your development computer ;-)
 
-2014 - 2022 David Fischer
+2012 - 2024 David Fischer
```

### Comparing `pytoolbox-14.8.0/pytoolbox/ai/vision/face/detect/dlib.py` & `pytoolbox-14.8.1/pytoolbox/ai/vision/face/detect/dlib.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/ai/vision/face/recognize/nn4_small2.py` & `pytoolbox-14.8.1/pytoolbox/ai/vision/face/recognize/nn4_small2.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/ai/vision/utils.py` & `pytoolbox-14.8.1/pytoolbox/ai/vision/utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/atlassian.py` & `pytoolbox-14.8.1/pytoolbox/atlassian.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/aws/s3.py` & `pytoolbox-14.8.1/pytoolbox/aws/s3.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/collections.py` & `pytoolbox-14.8.1/pytoolbox/collections.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/comparison.py` & `pytoolbox-14.8.1/pytoolbox/comparison.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from collections.abc import Iterator
+from collections.abc import Iterable, Iterator
 from typing import TypeAlias
 import difflib
 import operator as op
 import os
 
 from packaging.version import (  # pylint:disable=ungrouped-imports
     parse as _parse_version,
@@ -40,37 +40,39 @@
 
     def __ne__(self, other) -> bool:
         return not self.__eq__(other)
 
 
 # Content ------------------------------------------------------------------------------------------
 
+
 def unified_diff(before: str, after: str, *, colorize: bool = True, **kwargs) -> str:
     """
     Colorization is not guaranteed (your environment may disable it).
     Use `pytoolbox.console.toggle_colors` appropriately to ensure it.
     """
     diff = difflib.unified_diff(before.splitlines(), after.splitlines(), **kwargs)
     return os.linesep.join(_colorize(diff) if colorize else diff)
 
 
-def _colorize(diff: Iterator[str]) -> Iterator[str]:
+def _colorize(diff: Iterable[str]) -> Iterator[str]:
     for line in diff:
         if line.startswith('+'):
             yield termcolor.colored(line, 'green')
         elif line.startswith('-'):
             yield termcolor.colored(line, 'red')
         elif line.startswith('^'):
             yield termcolor.colored(line, 'blue')
         else:
             yield line
 
 
 # Versions -----------------------------------------------------------------------------------------
 
+
 def _eqn(a, b) -> bool | None:  # pylint:disable=invalid-name
     return True if a == b else None
 
 
 def _nen(a, b) -> bool | None:  # pylint:disable=invalid-name
     return False if a == b else None
 
@@ -100,15 +102,16 @@
         operation = VERSION_OPERATIONS[type(version_a)][operator]
         return operation(version_a, version_b) if operation else None
     return None  # Will not try to compare Version to LegacyVersion
 
 
 def satisfy_version_constraints(
     version: str | None,
-    constraints: tuple[str, ...], *,
+    constraints: Iterable[str],
+    *,
     default: str = '<undefined>',
 ) -> bool:
     """
     Ensure given version fulfill the constraints (if any).
 
     Constraints are given in the form '<operator> <version>', Exemple:
```

### Comparing `pytoolbox-14.8.0/pytoolbox/crypto.py` & `pytoolbox-14.8.1/pytoolbox/crypto.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/datetime.py` & `pytoolbox-14.8.1/pytoolbox/datetime.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/decorators.py` & `pytoolbox-14.8.1/pytoolbox/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,29 +37,32 @@
     def __get__(self, instance, type=None):  # pylint:disable=redefined-builtin
         if instance is None:
             return self
         res = instance.__dict__[self.name] = self.func(instance)
         return res
 
 
-def deprecated(func: Callable) -> Callable:
-    """
-    Decorator that can be used to mark functions as deprecated.
-    It will result in a warning being emitted when the function is used.
-
-    Credits: https://wiki.python.org/moin/PythonDecoratorLibrary.
-    """
-    @functools.wraps(func)
-    def _deprecated(*args, **kwargs) -> Any:
-        warnings.warn_explicit(
-            f'Call to deprecated function {func.__name__}.',
-            category=DeprecationWarning,
-            filename=func.__code__.co_filename,
-            lineno=func.__code__.co_firstlineno + 1)
-        return func(*args, **kwargs)
+def deprecated(guidelines: str = '') -> Callable:
+    def _deprecated(func: Callable) -> Callable:
+        """
+        Decorator that can be used to mark functions as deprecated.
+        It will result in a warning being emitted when the function is used.
+
+        Credits: https://wiki.python.org/moin/PythonDecoratorLibrary.
+        """
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs) -> Any:
+            guidelines_str = f': {guidelines}' if guidelines else ''
+            warnings.warn_explicit(
+                f'Call to deprecated function {func.__module__}.{func.__name__}{guidelines_str}.',
+                category=DeprecationWarning,
+                filename=func.__code__.co_filename,
+                lineno=func.__code__.co_firstlineno + 1)
+            return func(*args, **kwargs)
+        return wrapper
     return _deprecated
 
 
 class hybridmethod(object):  # pylint:disable=invalid-name,too-few-public-methods
     """
     Decorator that allows a method to be both used as a class method and an instance method.
```

### Comparing `pytoolbox-14.8.0/pytoolbox/django/core/exceptions.py` & `pytoolbox-14.8.1/pytoolbox/django/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/core/validators.py` & `pytoolbox-14.8.1/pytoolbox/django/core/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 raise ValidationError(
                     self.messages['extra_keys'],
                     code='extra_keys',
                     params={'keys': ', '.join(extra_keys)})
 
     def __eq__(self, other):
         return (
-            isinstance(other, self.__class__)
+            isinstance(other, type(self))
             and self.required_keys == other.required_keys
             and self.optional_keys == other.optional_keys
             and self.messages == other.messages
             and self.strict == other.strict
         )
 
     def __ne__(self, other):
```

### Comparing `pytoolbox-14.8.0/pytoolbox/django/forms/base.py` & `pytoolbox-14.8.1/pytoolbox/django/forms/base.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/forms/fields.py` & `pytoolbox-14.8.1/pytoolbox/django/forms/fields.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/forms/mixins.py` & `pytoolbox-14.8.1/pytoolbox/django/forms/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     }
     #: Attributes that are applied to all widgets of the form
     widgets_common_attrs = {}
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         for field in self.fields.values():
-            updates = self.widgets_rules.get(field.__class__)
+            updates = self.widgets_rules.get(type(field))
             # May Update widget class with rules-based replacement class
             if updates and updates[0]:
                 field.widget = updates[0]()
             # May update widget attributes with common attributes
             if self.widgets_common_attrs:
                 utils.update_widget_attributes(field.widget, self.widgets_common_attrs)
             # May update widget attributes with rules-based attributes
```

### Comparing `pytoolbox-14.8.0/pytoolbox/django/forms/utils.py` & `pytoolbox-14.8.1/pytoolbox/django/forms/utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/forms/widgets.py` & `pytoolbox-14.8.1/pytoolbox/django/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/models/decorators.py` & `pytoolbox-14.8.1/pytoolbox/django/models/decorators.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/models/fields/base.py` & `pytoolbox-14.8.1/pytoolbox/django/models/fields/base.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/models/fields/mixins.py` & `pytoolbox-14.8.1/pytoolbox/django/models/fields/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/models/managers/mixins.py` & `pytoolbox-14.8.1/pytoolbox/django/models/managers/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/models/mixins.py` & `pytoolbox-14.8.1/pytoolbox/django/models/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
                     fields = {
                         f.strip().replace('_id', '')
                         for f in match.groupdict()['fields'].split(',')
                     }
                     if fields in (set(u) for u in self._meta.unique_together):
                         fields = sorted(fields - set(self.unique_together_hide_fields))
                         if fields:
-                            error = self.unique_error_message(self.__class__, fields)
+                            error = self.unique_error_message(type(self), fields)
                             raise ValidationError({fields[0]: error}) if len(fields) == 1 else error
                         return self._handle_hidden_duplicate_key_error(ex)
             raise
 
     def _handle_hidden_duplicate_key_error(self, ex):
         raise ex
 
@@ -186,15 +186,15 @@
         filtered_errors_by_field = collections.defaultdict(list)
         for field, errors in errors_by_field.items():
             for error in errors:
                 # only process the uniqueness errors related to multiple fields
                 if len(error.params.get('unique_check', [])) > 1:
                     fields = [f for f in error.params['unique_check'] if f not in hidden_fields]
                     if fields:
-                        error = self.unique_error_message(self.__class__, fields)
+                        error = self.unique_error_message(type(self), fields)
                         filtered_errors_by_field[
                             fields[0] if len(fields) == 1 else field
                         ].append(error)
                 else:
                     filtered_errors_by_field[field].append(error)
         return filtered_errors_by_field
```

### Comparing `pytoolbox-14.8.0/pytoolbox/django/models/query/mixins.py` & `pytoolbox-14.8.1/pytoolbox/django/models/query/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/models/utils.py` & `pytoolbox-14.8.1/pytoolbox/django/models/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,27 @@
         field = cls_or_instance._meta.pk.attname.rstrip('_id')
     return cls_or_instance._meta.get_field(field).related_model
 
 
 def get_content_type_dict(instance):
     """Return a dictionary with the serialized content type and private key of given instance."""
     from django.contrib.contenttypes import models as ct_models
-    content_type = ct_models.ContentType.objects.get_for_model(instance.__class__)
+    content_type = ct_models.ContentType.objects.get_for_model(type(instance))
     return {'app_label': content_type.app_label, 'model': content_type.model, 'pk': instance.pk}
 
 
 def get_instance(app_label, model, pk):
     """Return an instance given its app_label, model name and private key."""
     from django.contrib.contenttypes import models as ct_models
     model = ct_models.ContentType.objects.get(app_label=app_label, model=model)
     return model.get_object_for_this_type(pk=pk)
 
 
 def try_get_field(instance, field_name):
     try:
         return getattr(instance, field_name)
     except Exception as ex:
-        if ex.__class__.__name__ != 'RelatedObjectDoesNotExist':
+        if type(ex).__name__ != 'RelatedObjectDoesNotExist':
             raise
 
 
 __all__ = _all.diff(globals())
```

### Comparing `pytoolbox-14.8.0/pytoolbox/django/signals/dispatch.py` & `pytoolbox-14.8.1/pytoolbox/django/signals/dispatch.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/signals/handlers.py` & `pytoolbox-14.8.1/pytoolbox/django/signals/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,29 +31,29 @@
             dj_db_signals.connection_created.connect(setup_postgresql_hstore_extension)
             dj_signals.post_migrate.connect(create_site, sender=config)
             dj_signals.pre_save.connect(
                 strip_strings_and_validate_model, sender=settings.AUTH_USER_MODEL)
 """
 from __future__ import annotations
 
-import logging
-
 from django.conf import settings
 from django.db.models import fields
 from django.db.models.fields.files import FileField
 
+from pytoolbox import logging
+
 __all__ = [
     'logger',
     'clean_files_delete_handler',
     'create_site',
     'setup_postgresql_hstore_extension',
     'strip_strings_and_validate_model'
 ]
 
-logger = logging.getLogger(__name__)
+logger = logging.get_logger(__name__)
 
 
 def clean_files_delete_handler(instance, signal, **kwargs):
     """
     Remove the files of the instance's file fields when it is removed from the database.
 
     Simply use ``post_delete.connect(clean_files_delete_handler, sender=<your_model_class>)``
```

### Comparing `pytoolbox-14.8.0/pytoolbox/django/storage.py` & `pytoolbox-14.8.1/pytoolbox/django/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
 Extra storages and mix-ins for building your own storages.
 """
 from __future__ import annotations
 
-import logging
 import time
 
 from django.core.files.storage import FileSystemStorage
 
-from pytoolbox import module
+from pytoolbox import logging, module
 
 _all = module.All(globals())
 
-logger = logging.getLogger(__name__)
+logger = logging.get_logger(__name__)
 
 
 class ExpressTemporaryFileMixin(object):
 
     def _save(self, name, content):
         """
         Save the temporary file to the storage.
```

### Comparing `pytoolbox-14.8.0/pytoolbox/django/templatetags.py` & `pytoolbox-14.8.1/pytoolbox/django/templatetags.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,16 @@
 def verbose_name_plural(instance):
     """Return the verbose name (plural) of a model."""
     if instance in (None, string_if_invalid):
         return string_if_invalid
     return constants.DEFFERED_REGEX.sub('', force_str(instance._meta.verbose_name))
 
 
-# TAGS ---------------------------------------------------------------------------------------------
+# Tags ---------------------------------------------------------------------------------------------
+
 
 class StaticPathNode(StaticNode):
 
     @classmethod
     def handle_simple(cls, path):
         return os.path.join(PrefixNode.handle_simple('STATIC_ROOT'), path)
```

### Comparing `pytoolbox-14.8.0/pytoolbox/django/test/mixins.py` & `pytoolbox-14.8.1/pytoolbox/django/test/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/test/runner/mixins.py` & `pytoolbox-14.8.1/pytoolbox/django/test/runner/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/urls.py` & `pytoolbox-14.8.1/pytoolbox/django/urls.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/utils/collections.py` & `pytoolbox-14.8.1/pytoolbox/django/utils/collections.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/utils/logging.py` & `pytoolbox-14.8.1/pytoolbox/django/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django/views/mixins.py` & `pytoolbox-14.8.1/pytoolbox/django/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django_datatable_view/views/mixins.py` & `pytoolbox-14.8.1/pytoolbox/django_datatable_view/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/django_filter/filterset/mixins.py` & `pytoolbox-14.8.1/pytoolbox/django_filter/filterset/mixins.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,10 +14,10 @@
     """
 
     @classmethod
     def filter_for_field(cls, f, name, *, lookup_type='exact'):
         value = super().filter_for_field(f, name, lookup_type)
         if not value:
             raise NotImplementedError(
-                f"Unable to find a suitable filter for field '{name}' of class {f.__class__} "
+                f"Unable to find a suitable filter for field '{name}' of class {type(f)} "
                 f"with lookup type '{lookup_type}'")
         return value
```

### Comparing `pytoolbox-14.8.0/pytoolbox/django_formtools/views/mixins.py` & `pytoolbox-14.8.1/pytoolbox/django_formtools/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/exceptions.py` & `pytoolbox-14.8.1/pytoolbox/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 
 
 class MessageMixin(Exception):
     attrs: Annotated[tuple[str, ...], 'Attributes to expose to the __repr__'] = tuple()
     message: str
 
     def __init__(self, message: str | None = None, **kwargs) -> None:
-        assert hasattr(self, 'message'), type(self)          # TODO metaclass to check this
-        assert set(self.attrs).issubset(set(kwargs.keys()))  # TODO metaclass to check this
         if message is not None:
             self.message = message
         for key, value in kwargs.items():
             setattr(self, key, value)
         super().__init__()
+        if missing := [attr for attr in self.attrs if not hasattr(self, attr)]:
+            missing = ', '.join(missing)  # type: ignore[assignment]
+            raise AttributeError(f'{type(self)} is missing attributes or properties: {missing}')
 
     def __repr__(self) -> str:
         args = [] if self.message == type(self).message else [f'{repr(self.message)}']
         args.extend(f'{a}={repr(getattr(self, a))}' for a in self.attrs)
-        return f"{self.__class__.__name__}({', '.join(args)})"
+        return f"{type(self).__name__}({', '.join(args)})"
 
     def __str__(self) -> str:
         attributes = inspect.getmembers(self, lambda a: not inspect.isroutine(a))
         return self.message.format(**{a: v for a, v in attributes if a[0] != '_'})
 
 
 class BadHTTPResponseCodeError(MessageMixin, Exception):
@@ -42,21 +43,28 @@
     message: str = 'Download request {url} code {r_code} expected {code}.'
     url: str
     r_code: int
     code: int
 
 
 class CalledProcessError(MessageMixin, Exception):
-    attrs: tuple[str, ...] = ('returncode', 'cmd', 'stdout', 'stderr')
-    message: str = 'Process {cmd!r} failed with return code {returncode}'
+    attrs: tuple[str, ...] = ('cmd_short', 'returncode')
+    message: str = 'Process {cmd_short} failed with return code {returncode}'
+    cmd: list[str]
     returncode: int
-    cmd: str
     stdout: bytes | None
     stderr: bytes | None
 
+    @property
+    def cmd_short(self) -> list[str]:
+        short_cmd = self.cmd[:4]
+        if len(self.cmd) > 4:
+            short_cmd.append('(…)')
+        return short_cmd
+
 
 class CorruptedFileError(MessageMixin, Exception):
     attrs: tuple[str, ...] = ('path', 'file_hash', 'expected_hash')
     message: str = 'File {path} is corrupted checksum {file_hash} expected {expected_hash}.'
     path: Path
     file_hash: str
     expected_hash: str
@@ -171,15 +179,15 @@
         elif value is None:
             something[index]  # pylint:disable=pointless-statement
         else:
             something[index] = value
     except Exception as ex:  # pylint:disable=broad-except
         if not isinstance(ex, exception_cls):
             raise ValueError(
-                f'Exception {ex.__class__.__name__} is not '
+                f'Exception {type(ex).__name__} is not '
                 f'an instance of {exception_cls.__name__}.') from ex
         return
     raise AssertionError(f'Exception {exception_cls.__name__} not raised.')
 
 
 def get_exception_with_traceback(exception: Exception) -> str:
     """
```

### Comparing `pytoolbox-14.8.0/pytoolbox/filesystem.py` & `pytoolbox-14.8.1/pytoolbox/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 from . import module
 from .datetime import datetime_now
 from .decorators import deprecated
 from .regex import from_path_patterns
 
 _all = module.All(globals())
 
-FindPatterns: TypeAlias = re.Pattern | str | list[re.Pattern] | list[str] | list[re.Pattern | str]
+FindPatterns: TypeAlias = (
+    re.Pattern | str |  # noqa: W504
+    list[re.Pattern] | list[str] | list[re.Pattern | str] |  # noqa: W504
+    tuple[re.Pattern, ...] | tuple[str, ...] | tuple[re.Pattern | str, ...]
+)
 
 
 class CopyProgressCallback(Protocol):  # pylint:disable=too-few-public-methods
     def __call__(
         self,
         start_date: datetime.datetime,
         elapsed_time: float,
@@ -476,19 +480,14 @@
     except OSError as ex:
         # Directory exists
         if ex.errno == errno.EEXIST and path.is_dir():
             return False
         raise  # Re-raise exception if a different error occurred
 
 
-@deprecated
-def recursive_copy(*args, **kwargs):
-    return copy_recursive(*args, **kwargs)
-
-
 def remove(path: Path | str, *, recursive: bool = False):
     """
     Remove a file/directory (which may not exists) without throwing an exception.
     Returns True if operation is successful, False if file/directory not found and re-raise any
     other type of exception.
 
     **Example usage**
@@ -838,7 +837,15 @@
         >>> assert not f1.is_file()
         """
         for key in self._paths_by_key.copy().keys():
             self.remove_by_key(key)
 
 
 __all__ = _all.diff(globals())
+
+
+# Deprecated ---------------------------------------------------------------------------------------
+
+
+@deprecated('Use pytoolbox.filesystem.copy_recursive instead (drop-in replacement)')
+def recursive_copy(*args, **kwargs):  # pragma: no cover
+    return copy_recursive(*args, **kwargs)
```

### Comparing `pytoolbox-14.8.0/pytoolbox/flask.py` & `pytoolbox-14.8.1/pytoolbox/flask.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,9 +77,9 @@
     elif isinstance(exception, IndexError):
         abort(404, str(exception))
     elif isinstance(exception, ValueError):
         abort(415, str(exception))
     elif isinstance(exception, NotImplementedError):
         abort(501, str(exception))
     else:
-        abort(500, f'{exception.__class__.__name__} {repr(exception)} {str(exception)}')
+        abort(500, f'{type(exception).__name__} {repr(exception)} {str(exception)}')
     return None
```

### Comparing `pytoolbox-14.8.0/pytoolbox/git.py` & `pytoolbox-14.8.1/pytoolbox/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
-from collections.abc import Iterator
+from collections.abc import Iterable, Iterator
 from pathlib import Path
 import contextlib
-import logging
 import os
 import stat
 import tempfile
 
-from . import exceptions, humanize, subprocess
+from . import exceptions, humanize, logging, subprocess
 from .subprocess import CallArgType
 
-log = logging.getLogger(__name__)
+log = logging.get_logger(__name__)
 
 __all__ = ['blame', 'clone_or_pull', 'create_tag', 'get_ref', 'get_tags', 'scoped_ssh_key']
 
 
 def blame(file_path: Path) -> list[str]:
     lines = subprocess.cmd(
         ['git', 'blame', file_path],
@@ -87,15 +86,15 @@
 
 
 @contextlib.contextmanager
 def scoped_ssh_key(
     directory: Path,
     content: str,
     *,
-    options: tuple[str] = tuple(),  # type: ignore[assignment]
+    options: Iterable[str] = tuple(),  # type: ignore[assignment]
 ) -> Iterator[str]:
     """Load an SSH key (content is the private key)."""
     with tempfile.NamedTemporaryFile('w') as key_file:
         os.chmod(key_file.name, stat.S_IRUSR)
         key_file.write(content + os.linesep)
         key_file.flush()
         try:
```

### Comparing `pytoolbox-14.8.0/pytoolbox/humanize.py` & `pytoolbox-14.8.1/pytoolbox/humanize.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 _all = module.All(globals())
 
 DEFAULT_BITRATE_UNITS: Final[tuple[str, ...]] = (
     'bit/s', 'kb/s', 'Mb/s', 'Gb/s', 'Tb/s', 'Pb/s', 'Eb/s', 'Zb/s', 'Yb/s'
 )
 # pylint:disable=consider-using-namedtuple-or-dataclass)
-DEFAULT_FILESIZE_ARGS: Final[dict[str, dict[str, int | tuple[str, ...]]]] = {
+DEFAULT_FILESIZE_ARGS: Final[dict[str, dict[str, int | list[str] | tuple[str, ...]]]] = {
     'gnu': {'base': 1000, 'units': ('B', 'K', 'M', 'G', 'T', 'P', 'E', 'Z', 'Y')},
     'nist': {'base': 1024, 'units': ('B', 'kB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB')},
     'si': {'base': 1000, 'units': ('B', 'KiB', 'MiB', 'GiB', 'TiB', 'PiB', 'EiB', 'ZiB', 'YiB')}
 }
 DEFAULT_FREQUENCY_UNITS: Final[tuple[str, ...]] = (
     'Hz', 'kHz', 'MHz', 'GHz', 'THz', 'PHz', 'EHz', 'ZHz', 'YHz'
 )
@@ -36,15 +36,15 @@
     r'(?P<number>[\+-]?\d*\.?\d+([eE]\+\d+)?)\s*(?P<unit>[a-zA-Z]+)')
 
 
 def naturalbitrate(
     bps: int | float,
     fmt: str = '{sign}{value:.3g} {unit}',
     scale: int | None = None,
-    units: tuple[str, ...] = DEFAULT_BITRATE_UNITS
+    units: list[str] | tuple[str, ...] = DEFAULT_BITRATE_UNITS
 ) -> str:
     """
     Return a human readable representation of a bit rate taking `bps` as the rate in bits/s.
 
     The unit is taken from:
 
     * The `scale` if not None (0=bit/s, 1=kb/s, 2=Mb/s, ...).
@@ -73,15 +73,15 @@
 
 
 def naturalfilesize(  # pylint:disable=dangerous-default-value
     size_bytes: int | float,
     system: str = 'nist',
     fmt: str = '{sign}{value:.3g} {unit}',
     scale: int | None = None,
-    args: dict[str, dict[str, int | tuple[str, ...]]] = DEFAULT_FILESIZE_ARGS
+    args: dict[str, dict[str, int | list[str] | tuple[str, ...]]] = DEFAULT_FILESIZE_ARGS
 ) -> str:
     """
     Return a human readable representation of a *file* size taking `bytes` as the size in bytes.
 
     The base and units taken from:
 
     * The value in `args` with key `system` if not None.
@@ -124,15 +124,15 @@
         **(args[system] if system else args))
 
 
 def naturalfrequency(
     hertz: int | float,
     fmt: str = '{sign}{value:.3g} {unit}',
     scale: int | None = None,
-    units: tuple[str, ...] = DEFAULT_FREQUENCY_UNITS
+    units: list[str] | tuple[str, ...] = DEFAULT_FREQUENCY_UNITS
 ) -> str:  # pylint:disable=dangerous-default-value
     """
     Return a human readable representation of a frequency taking `hertz` as the frequency in Hz.
 
     The unit is taken from:
 
     * The `scale` if not None (0=bit/s, 1=kb/s, 2=Mb/s, ...).
@@ -160,15 +160,15 @@
     return _natural_number(hertz, base=1000, fmt=fmt, scale=scale, units=units)
 
 
 def naturalweight(
     grams: int | float,
     fmt: str = '{sign}{value:.3g} {unit}',
     scale: int | None = None,
-    units: tuple[str, ...] = DEFAULT_WEIGHT_UNITS
+    units: list[str] | tuple[str, ...] = DEFAULT_WEIGHT_UNITS
 ) -> str:  # pylint:disable=dangerous-default-value
     """
     Return a human readable representation of a weight in `grams`.
 
     The unit is taken from:
 
     * The `scale` if not None (0=g, 1=Kg, 2=T, ...).
@@ -209,15 +209,15 @@
     ['a1', 'a3', 'a4', 'a10', 'a19', 'a26', 'b2', 'b12']
     """
     return [int(c) if c.isdigit() else c for c in DIGIT_REGEX.split(text)]
 
 
 def parse_bitrate(
     bitrate: str,
-    units: tuple[str, ...] = DEFAULT_BITRATE_UNITS,
+    units: list[str] | tuple[str, ...] = DEFAULT_BITRATE_UNITS,
     pattern: re.Pattern = BITRATE_PATTERN
 ) -> float:
     """
     Parse a human readable representation of a `bitrate` to its numeric value in bits/s.
 
     Returned as a natural number you can round if desired.
 
@@ -247,15 +247,15 @@
         units=units,
         pattern=pattern)
 
 
 def parse_filesize(  # pylint:disable=dangerous-default-value
     size: str,
     system: str = 'nist',
-    args: dict[str, dict[str, int | tuple[str, ...]]] = DEFAULT_FILESIZE_ARGS,
+    args: dict[str, dict[str, int | list[str] | tuple[str, ...]]] = DEFAULT_FILESIZE_ARGS,
     pattern: re.Pattern = FILESIZE_PATTERN
 ) -> float:
     """
     Parse a human readable representation of a *file* `size` to its numeric value in bytes.
 
     Returned as a natural number you can round if desired.
 
@@ -289,15 +289,15 @@
         kind='file size',
         pattern=pattern,
         **(args[system] if system else args))
 
 
 def parse_frequency(
     frequency: str,
-    units: tuple[str, ...] = DEFAULT_FREQUENCY_UNITS,
+    units: list[str] | tuple[str, ...] = DEFAULT_FREQUENCY_UNITS,
     pattern: re.Pattern = FREQUENCY_PATTERN
 ) -> float:
     """
     Parse a human readable representation of a `frequency` to its numeric value in Hertz.
 
     Returned as a natural number you can round if desired.
 
@@ -334,15 +334,15 @@
         base=1000,
         units=units,
         pattern=pattern)
 
 
 def parse_weight(
     weight: str,
-    units: tuple[str, ...] = DEFAULT_WEIGHT_UNITS,
+    units: list[str] | tuple[str, ...] = DEFAULT_WEIGHT_UNITS,
     pattern: re.Pattern = WEIGHT_PATTERN
 ) -> float:
     """
     Parse a human readable representation of a `weight` to its numeric value in grams.
 
     Returned as a natural number you can round if desired.
 
@@ -370,15 +370,15 @@
         units=units,
         pattern=pattern)
 
 
 def _natural_number(
     number: int | float,
     base: int,
-    units: tuple[str, ...],
+    units: list[str] | tuple[str, ...],
     fmt: str = '{sign}{value:.3g} {unit}',
     scale: int | None = None
 ) -> str:
     sign, number = '' if number >= 0 else '-', abs(number)
     if scale is None:
         scale = min(int(math.log(max(1, number), base)), len(units) - 1)
     unit = units[scale]
@@ -386,15 +386,15 @@
     return fmt.format(sign=sign, value=value, unit=unit)
 
 
 def _parse_natural_number(
     value: str,
     kind: str,
     base: int,
-    units: tuple[str, ...],
+    units: list[str] | tuple[str, ...],
     pattern: re.Pattern
 ) -> float:
     if match := pattern.match(value.strip()):
         data = match.groupdict()
         number = float(data['number'])
         unit = data['unit']
         try:
```

### Comparing `pytoolbox-14.8.0/pytoolbox/itertools.py` & `pytoolbox-14.8.1/pytoolbox/itertools.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/juju.py` & `pytoolbox-14.8.1/pytoolbox/juju.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # pylint:disable=too-many-lines
 from __future__ import annotations
 
-import argparse
 import json
 import os
-import socket
 import random
-import subprocess
+import socket
+import subprocess as _subprocess
 import sys
 import time
 import uuid
 
 from . import (  # pylint:disable=reimported
+    argparse,
     console,
+    exceptions,
     filesystem,
     module,
-    subprocess as py_subprocess,
+    subprocess,
     serialization
 )
 from .argparse import FullPaths, is_dir
 
 yaml = serialization.get_yaml()
 
 _all = module.All(globals())
@@ -97,17 +98,17 @@
 
     env = os.environ.copy()
     env['HOME'] = os.path.expanduser('~/')
     env['JUJU_HOME'] = os.path.expanduser('~/.juju')
 
     if is_destroy:
         # TODO Automate yes answer to destroy-environment
-        method = subprocess.check_call if fail else subprocess.call
+        method = _subprocess.check_call if fail else _subprocess.call
         return method(arguments)
-    result = py_subprocess.cmd(arguments, fail=False, log=log, env=env, **kwargs)
+    result = subprocess.cmd(arguments, fail=False, log=log, env=env, **kwargs)
 
     if result['returncode'] != 0 and fail:
         raise RuntimeError(f"Subprocess failed {' '.join(arguments)} : {result['stderr']}.")
 
     return yaml.load(result['stdout'])
 
 
@@ -142,19 +143,20 @@
 
 def save_unit_config(path, service, config):
     with open(path, 'w', encoding='utf-8') as f:
         for option, value in config.items():
             if isinstance(value, bool):
                 config[option] = str(value)
         config = {service: config}
-        f.write(yaml.dump(config))
+        yaml.dump(config, f)
 
 
 # Environments -------------------------------------------------------------------------------------
 
+
 def add_environment(
     environment,
     kind,
     region,
     access_key,
     secret_key,
     control_bucket,
@@ -184,23 +186,23 @@
         }
     else:
         raise NotImplementedError(f'Registration of {kind} type of environment.')
 
     environments_dict['environments'][environment] = environment_dict
 
     with open(environments, 'w', encoding='utf-8') as f:
-        f.write(yaml.dump(environments_dict))
+        yaml.dump(environments_dict, f)
 
     try:
         return juju_do('bootstrap', environment)
     except RuntimeError as ex:
         if 'configuration error' in str(ex):
             del environments_dict['environments'][environment]
             with open(environments, 'w', encoding='utf-8') as f:
-                f.write(yaml.dump(environments_dict))
+                yaml.dump(environments_dict, f)
             raise ValueError(f'Cannot add environment {environment} ({ex}).') from ex
         raise
 
 
 def get_environment(environment, environments=None, get_status=False, status_timeout=None):
     with open(environments or DEFAULT_ENVIRONMENTS_FILE, encoding='utf-8') as f:
         environments_dict = yaml.load(f)
@@ -238,20 +240,22 @@
 def get_environments_count(environments=None):
     with open(environments or DEFAULT_ENVIRONMENTS_FILE, encoding='utf-8') as f:
         return len(yaml.load(f)['environments'])
 
 
 # Units --------------------------------------------------------------------------------------------
 
+
 def get_unit_path(service, number, *args):
     return os.path.join(f'/var/lib/juju/agents/unit-{service}-{number}/charm', *args)
 
 
 # Helpers ------------------------------------------------------------------------------------------
 
+
 __get_ip = None  # pylint:disable=invalid-name
 
 
 def get_ip():
     global __get_ip  # pylint:disable=global-statement,invalid-name
     if __get_ip is None:
         host = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
@@ -343,15 +347,15 @@
                 raise OSError('Disabled by user.')
             self.juju_ok = True
             self.load_config(json.loads(self.cmd(['config-get', '--format=json'])['stdout']))
             self.env_uuid = os.environ.get('JUJU_ENV_UUID')
             self.name = os.environ['JUJU_UNIT_NAME']
             self.private_address = socket.getfqdn(self.unit_get('private-address'))
             self.public_address = socket.getfqdn(self.unit_get('public-address'))
-        except (subprocess.CalledProcessError, OSError) as ex:
+        except (exceptions.CalledProcessError, OSError) as ex:
             reason = ex
             self.juju_ok = False
             if default_config is not None:
                 self.load_config(default_config)
             self.env_uuid = default_os_env['JUJU_ENV_UUID']
             self.name = default_os_env['JUJU_UNIT_NAME']
             self.private_address = self.public_address = socket.getfqdn(get_ip())
@@ -545,15 +549,15 @@
 
     # ----------------------------------------------------------------------------------------------
 
     def cmd(self, command, logging=True, **kwargs):
         """
         Calls the `command` and returns a dictionary with `stdout`, `stderr`, and the `returncode`.
         """
-        return py_subprocess.cmd(command, log=self.debug if logging else None, **kwargs)
+        return subprocess.cmd(command, log=self.debug if logging else None, **kwargs)
 
     def template_to_config(self, template, config, values):
         filesystem.from_template(template, config, values)
         self.remark(f'File {config} successfully generated')
 
     # ----------------------------------------------------------------------------------------------
 
@@ -568,23 +572,23 @@
         """
         if hook_name is None:
             if len(sys.argv) != 2:
                 raise ValueError(f'Usage {sys.argv[0]} hook_name (e.g. config-changed)')
             hook_name = sys.argv[1]
 
         try:  # Call the function hooks_...
-            self.hook(f'Execute {self.__class__.__name__} hook {hook_name}')
+            self.hook(f'Execute {type(self).__name__} hook {hook_name}')
             getattr(self, f"hook_{hook_name.replace('-', '_')}")()
             self.save_local_config()
-        except subprocess.CalledProcessError as ex:
+        except (_subprocess.CalledProcessError, exceptions.CalledProcessError) as ex:
             self.log('Exception caught:')
             self.log(ex.output)
             raise
         finally:
-            self.hook(f'Exiting {self.__class__.__name__} hook {hook_name}')
+            self.hook(f'Exiting {type(self).__name__} hook {hook_name}')
 
 
 class Environment(object):  # pylint:disable=too-many-instance-attributes,too-many-public-methods
 
     def __init__(
         self,
         name='default',
@@ -738,15 +742,15 @@
         if remove:
             # Check if environment destroyed otherwise a lot of trouble with $/€ !
             if self.is_bootstrapped(timeout=timeout):
                 raise RuntimeError(f'Environment {name} not removed, it is still alive.')
 
             del environments_dict['environments'][name]
             with open(environments, 'w', encoding='utf-8') as f:
-                f.write(yaml.dump(environments_dict))
+                yaml.dump(environments_dict, f)
         return result
 
     # Services
 
     def get_service_config(self, service, fail=True):
         return juju_do('get', self.name, options=[service], fail=fail)
 
@@ -1141,17 +1145,15 @@
         charms_path='charms',
         release='raring',
         auto=False
     ):  # pylint:disable=invalid-name
         HELP_A = 'Toggle automatic confirmation of the actions, WARNING: Use it with care.'
         HELP_M = 'Directory (repository) of any local charm.'
         HELP_R = 'Ubuntu serie to deploy by JuJu.'
-        parser = argparse.ArgumentParser(
-            formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-            epilog=epilog)
+        parser = argparse.ArgumentParser(epilog=epilog)
         arg = parser.add_argument
         arg('-a', '--auto', action='store_true', default=auto, help=HELP_A)
         arg('-m', '--charms_path', action=FullPaths, default=charms_path, type=is_dir, help=HELP_M)
         arg('-r', '--release', action='store', default=release, help=HELP_R)
         return parser
 
     def run(self):
@@ -1160,14 +1162,15 @@
 
 # Simulation ---------------------------------------------------------------------------------------
 
 # DISCLAIMER: Ideally this module will implement a simulated juju_do to make it possible to use the
 # same methods to drive a real or a simulated juju process ... The following code is a partial/light
 # implementation of ... Do not use it for your own purposes !!!
 
+
 class SimulatedUnit(object):
     """A simulated unit with a really simple state machine having a latency to start and stop."""
 
     def __init__(self, start_latency_range, stop_latency_range, state=PENDING):
         self.counter = self.next_state = None
         self.state = state
         self.start_latency_range = start_latency_range
```

### Comparing `pytoolbox-14.8.0/pytoolbox/linux.py` & `pytoolbox-14.8.1/pytoolbox/linux.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/logging.py` & `pytoolbox-14.8.1/pytoolbox/logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,52 +3,98 @@
 from pathlib import Path
 from typing import Literal, Protocol, TypeAlias
 import logging
 import sys
 
 from .collections import merge_dicts
 
-__all__ = ['LoggerType', 'setup_logging', 'ColorizeFilter']
+__all__ = [
+    'CRITICAL',
+    'FATAL',
+    'ERROR',
+    'WARN',
+    'WARNING',
+    'INFO',
+    'DEBUG',
+    'NOTSET',
+    'Color',
+    'BasicLoggerFunc',
+    'BasicFuncLogger',
+    'LoggerType',
+    'Logger',
+    'LogRecord',
+    'get_logger',
+    'setup_logging',
+    'ColorizeFilter'
+]
+
+CRITICAL: int = logging.CRITICAL
+FATAL: int = logging.FATAL
+ERROR: int = logging.ERROR
+WARN: int = logging.WARNING
+WARNING: int = logging.WARNING
+INFO: int = logging.INFO
+DEBUG: int = logging.DEBUG
+NOTSET: int = logging.NOTSET
+
+# Terminal colors (termcolor)
+Color: TypeAlias = Literal[
+    'black',
+    'grey',
+    'red',
+    'green',
+    'yellow',
+    'blue',
+    'magenta',
+    'cyan',
+    'light_grey',
+    'dark_grey',
+    'light_red',
+    'light_green',
+    'light_yellow',
+    'light_blue',
+    'light_magenta',
+    'light_cyan',
+    'white'
+]
 
 
 class BasicLoggerFunc(Protocol):  # pylint:disable=too-few-public-methods
     def __call__(self, messsage: str) -> None:
         ...
 
 
 class BasicFuncLogger(logging.Logger):
 
     def __init__(self, log_func) -> None:
         self._log_func = log_func
-        super().__init__(name=log_func.__name__)
+        super().__init__(name=f'{log_func.__module__}.{log_func.__name__}')
 
     def _log(self, level, msg, *args, **kwargs) -> None:  # pylint:disable=unused-argument
         self._log_func(msg)
 
 
-LoggerType: TypeAlias = BasicLoggerFunc | logging.Logger | None
+LoggerType: TypeAlias = BasicLoggerFunc | logging.Logger | str | None
+Logger = logging.Logger
+LogRecord = logging.LogRecord
 
 
 def get_logger(log: LoggerType) -> logging.Logger:
     """Convenient function returning an instance of logger for various use cases."""
     if isinstance(log, logging.Logger):
         return log
-    if log is None:
-        log = logging.getLogger('noop')
-        log.setLevel('NOTSET')
-        return log
+    if isinstance(log, str):
+        return logging.getLogger(log)
     if hasattr(log, '__call__'):
-        log = BasicFuncLogger(log_func=log)
-        log.setLevel('NOTSET')
-        return log
+        return BasicFuncLogger(log_func=log)
     raise NotImplementedError(f'Logging with {log!r}')
 
 
 def setup_logging(
-    name_or_log: str | logging.Logger = '',
+    log: LoggerType = '',
     reset: bool = False,
     path: Path | str | None = None,
     console: bool = False,
     level: int | str = logging.DEBUG,
     colorize: bool = False,
     color_by_level: dict[int | str, str] | None = None,
     fmt: str = '%(asctime)s %(levelname)-8s - %(message)s',
@@ -102,15 +148,15 @@
     >>> with tempfile.NamedTemporaryFile('r') as f:
     ...     log = setup_logging('my-logger', path=f.name)
     ...     log.info('Ceci va probablement jamais être lu!')
     ...     lines = f.read().split(os.linesep)
     ...
     >>> assert 'INFO     - Ceci va probablement jamais être lu!' in lines[0]
     """
-    log = logging.getLogger(name_or_log) if isinstance(name_or_log, str) else name_or_log
+    log = get_logger(log)
     if reset:
         log.handlers = []
     log.setLevel(level)
     if colorize:
         log.addFilter(ColorizeFilter(color_by_level=color_by_level))
     if path:
         file_handler = logging.FileHandler(path)
@@ -121,15 +167,15 @@
         console_handler.setFormatter(logging.Formatter(fmt=fmt, datefmt=datefmt))
         log.addHandler(console_handler)
     return log
 
 
 class ColorizeFilter(logging.Filter):  # pylint:disable=too-few-public-methods
 
-    color_by_level: dict[int | str, str] = {
+    color_by_level: dict[int | str, Color] = {
         logging.DEBUG: 'cyan',
         logging.ERROR: 'red',
         logging.INFO: 'white',
         logging.WARNING: 'yellow'
     }
 
     def __init__(self, *args, **kwargs) -> None:
```

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/exif/brand.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/exif/brand.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/exif/camera.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/exif/camera.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/exif/equipment.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/exif/equipment.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         except AttributeError:
             return NotImplemented
 
     def __hash__(self):
         return hash(repr(self))
 
     def __repr__(self):
-        return f'<{self.__class__.__name__} {self.brand} {self.model}>'
+        return f'<{type(self).__name__} {self.brand} {self.model}>'
 
     @property
     @abc.abstractmethod
     def brand(self) -> Brand | None:
         pass
 
     @property
```

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/exif/image.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/exif/image.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/exif/lens.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/exif/lens.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/exif/metadata.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/exif/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
+from collections.abc import Iterable
 from pathlib import Path
 import datetime
 
 from pytoolbox import exceptions
+from pytoolbox.itertools import chain
 
 from . import camera, image, lens, photo, tag
 
 __all__ = ['Metadata']
 
 
 class Metadata(object):
@@ -20,15 +22,15 @@
 
     def __init__(
         self,
         path: Path | None = None,
         buf=None,
         orientation: image.Orientation | int | None = None,
         gexiv2_version: str = '0.10'
-    ):
+    ) -> None:
         import gi
         gi.require_version('GExiv2', gexiv2_version)
         from gi.repository import GExiv2  # type: ignore[attr-defined]
         self.path = path
         self.exiv2 = GExiv2.Metadata()
         if buf:
             self.exiv2.open_buf(buf)
@@ -41,29 +43,26 @@
         self.lens = self.lens_class(self)
         self.photo = self.photo_class(self)
 
     def __getitem__(self, key: str) -> tag.Tag:
         # TODO make it more strict and re-implement less strict self.get(key)
         return self.tag_class(self, key)
 
-    def __setitem__(self, key: str, value):
+    def __setitem__(self, key: str, value) -> None:
         self.exiv2[key] = value  # pylint: disable=unsupported-assignment-operation
 
     @property
     def tags(self) -> dict:
         return {k: self[k] for k in self.exiv2.get_tags()}  # pylint: disable=no-member
 
     def get_date(
         self,
-        keys: tuple[str, ...] | str = ('Exif.Photo.DateTimeOriginal', 'Exif.Image.DateTime')
+        keys: Iterable[str] | str = ('Exif.Photo.DateTimeOriginal', 'Exif.Image.DateTime')
     ) -> datetime.datetime | None:
-
-        if isinstance(keys, str):
-            keys = tuple(keys)
-        for key in keys:
+        for key in chain(keys):
             date = self[key].data
             if isinstance(date, datetime.datetime):
                 return date
         return None
 
     def rewrite(self, path: Path | None = None, save: bool = False) -> None:
         """
```

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/exif/photo.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/exif/photo.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/exif/tag.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/exif/tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     }
 
     def __init__(self, metadata, key):
         self.metadata = metadata
         self.key = key
 
     def __repr__(self):
-        return f'<{self.__class__.__name__} {self.key}: {str(self.data)[:20]}>'
+        return f'<{type(self).__name__} {self.key}: {str(self.data)[:20]}>'
 
     @property
     def data(self):
         if type_hook := self.get_type_hook():
             try:
                 return self.clean(type_hook(self.key))
             except UnicodeDecodeError as ex:
```

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/ffmpeg/__init__.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/ffmpeg/encode.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/encode.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/ffmpeg/ffmpeg.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/ffmpeg/ffprobe.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/ffprobe.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/ffmpeg/miscellaneous.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/ffmpeg/utils.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/image/PIL.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/image/PIL.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/multimedia/x264.py` & `pytoolbox-14.8.1/pytoolbox/multimedia/x264.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/network/http.py` & `pytoolbox-14.8.1/pytoolbox/network/http.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/network/ip.py` & `pytoolbox-14.8.1/pytoolbox/network/ip.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/network/rtp.py` & `pytoolbox-14.8.1/pytoolbox/network/rtp.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,15 +420,15 @@
         Equality test.
 
         .. warning::
 
             Test equality only on some fields (not all) !
         """
         return (
-            isinstance(other, self.__class__)
+            isinstance(other, type(self))
             and self.sequence == other.sequence
             and self.timestamp == other.timestamp
             and self.payload_type == other.payload_type
             and self.payload == other.payload)
 
     def __str__(self):
         """
```

### Comparing `pytoolbox-14.8.0/pytoolbox/network/smpte2022/base.py` & `pytoolbox-14.8.1/pytoolbox/network/smpte2022/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -654,15 +654,15 @@
         return j
 
     def __eq__(self, other):
         """
         Test equality field by field !
         """
         return (
-            isinstance(other, self.__class__)
+            isinstance(other, type(self))
             and self.sequence == other.sequence and self.algorithm == other.algorithm
             and self.direction == other.direction and self.snbase == other.snbase
             and self.offset == other.offset and self.na == other.na
             and self.payload_type_recovery == other.payload_type_recovery
             and self.length_recovery == other.length_recovery
             and self.payload_recovery == other.payload_recovery)
```

### Comparing `pytoolbox-14.8.0/pytoolbox/network/smpte2022/generator.py` & `pytoolbox-14.8.1/pytoolbox/network/smpte2022/generator.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/network/smpte2022/receiver.py` & `pytoolbox-14.8.1/pytoolbox/network/smpte2022/receiver.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/network/url.py` & `pytoolbox-14.8.1/pytoolbox/network/url.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/pandas.py` & `pytoolbox-14.8.1/pytoolbox/pandas.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/regex.py` & `pytoolbox-14.8.1/pytoolbox/regex.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from collections.abc import Iterator
+from collections.abc import Iterable, Iterator
 from typing import Any, Final, Literal, overload
 import fnmatch
 import re
 
 from . import exceptions
 from .itertools import chain
 
@@ -24,50 +24,59 @@
 
 UUID_REGEX: Final[str] = r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}'
 
 
 @overload
 def embed_in_regex(
     string: str,
-    regex_parts: list[str],
+    regex_parts: list[str] | tuple[str, ...],
     index: int,
     *,
     as_string: Literal[True] = True
 ) -> tuple[int, str]:
     ...
 
 
 @overload
 def embed_in_regex(
     string: str,
-    regex_parts: list[str],
+    regex_parts: list[str] | tuple[str, ...],
     index: int,
     *,
     as_string: Literal[False]
 ) -> tuple[int, list[str]]:
     ...
 
 
-def embed_in_regex(string, regex_parts, index, as_string=True):
+def embed_in_regex(
+    string: str,
+    regex_parts: list[str] | tuple[str, ...],
+    index: int,
+    *,
+    as_string: bool = True
+):
     """
     **Example usage**
 
     >>> embed_in_regex('L', ['[a-z]', '[a-z]'], 0)
     (0, 'L[a-z]')
     >>> embed_in_regex('L', ['[a-z]', '[a-z]'], 1)
     (1, '[a-z]L')
     >>> embed_in_regex('L', ['[a-z]', '[a-z]'], 1, as_string=False)
     (1, ['[a-z]', 'L'])
     """
-    regex = regex_parts[:]
+    regex: list[str] = list(regex_parts)
     regex[index:index + len(string)] = string
     return index, ''.join(regex) if as_string else regex
 
 
-def findall_partial(string: str, regex_parts: list[str]) -> Iterator[tuple[str, list[str], int]]:
+def findall_partial(
+    string: str,
+    regex_parts: list[str] | tuple[str, ...]
+) -> Iterator[tuple[str, list[str] | tuple[str, ...], int]]:
     """
     **Example usage**
 
     >>> [i for s, r, i in findall_partial(':', TIME_REGEX_PARTS)]
     [2, 5]
     >>> [embed_in_regex(s, r, i) for s, r, i in findall_partial('12:15:2', TIME_REGEX_PARTS)]
     [(0, '12:15:2[0-9]')]
@@ -79,15 +88,15 @@
     for index in range(0, len(regex_parts) - len(string) + 1):
         regex = regex_parts[index:index + len(string)]
         if re.search(''.join(regex), string):
             yield string, regex_parts, index
 
 
 def from_path_patterns(
-    patterns: re.Pattern | str | list[re.Pattern] | list[str] | list[re.Pattern | str],
+    patterns: re.Pattern | str | Iterable[re.Pattern] | Iterable[str] | Iterable[re.Pattern | str],
     *,
     regex: bool = False
 ) -> list[re.Pattern]:
     """
     Return patterns compiled to regular expressions, if necessary.
 
     If `regex` is set to False, then any string pattern will be converted from the unix-style
@@ -115,25 +124,26 @@
     ]
 
 
 def group_replace(
     string: str,
     match: re.Match, *,
     offset: int = 0,
-    mapping: tuple[tuple[str, str | None], ...]
+    mapping: Iterable[tuple[str, str | None]]
 ) -> str:
     """
     Replace matched groups in `string` by content from given `mapping` (group name -> replacement).
 
     An `exceptions.RegexMatchGroupNotFoundError` can be raised if a group is not found in `match`.
 
     **Example usage**
 
     Please check the code and unit-tests :)
     """
+    # TODO Reorder mapping in reverse(start) to prevent indexing issues while replacing parts
     for group, value in mapping:
         if value is not None:
             try:
                 if (start := match.start(group)) < 0:
                     raise IndexError()
             except IndexError as ex:
                 raise exceptions.RegexMatchGroupNotFoundError(group=group) from ex
```

### Comparing `pytoolbox-14.8.0/pytoolbox/rest_framework/metadata/mixins.py` & `pytoolbox-14.8.1/pytoolbox/rest_framework/metadata/mixins.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class ExcludeRelatedChoicesMixin(object):
     """Do not includes related fields to avoid having choices with hundreds instances."""
 
     related_fields = (serializers.RelatedField, serializers.ManyRelatedField)
 
     def get_field_info(self, field):
         if hasattr(field, 'choices') and isinstance(field, self.related_fields):
-            field_class = field.__class__
+            field_class = type(field)
 
             class HaveNoChoicesProxy(field_class):
 
                 @property
                 def choices(self):
                     raise AttributeError
```

### Comparing `pytoolbox-14.8.0/pytoolbox/rest_framework/permissions.py` & `pytoolbox-14.8.1/pytoolbox/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/rest_framework/serializers/fields.py` & `pytoolbox-14.8.1/pytoolbox/rest_framework/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/rest_framework/serializers/mixins.py` & `pytoolbox-14.8.1/pytoolbox/rest_framework/serializers/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/rest_framework/views/mixins.py` & `pytoolbox-14.8.1/pytoolbox/rest_framework/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/selenium/client.py` & `pytoolbox-14.8.1/pytoolbox/selenium/client.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/selenium/common.py` & `pytoolbox-14.8.1/pytoolbox/selenium/common.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/selenium/test.py` & `pytoolbox-14.8.1/pytoolbox/selenium/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 class LiveTestCaseMixin(object):
 
     live_client_class = client.LiveClient  # pylint:disable=used-before-assignment
 
     def setUp(self):  # pylint:disable=invalid-name
         """Call super's setUp and instantiate a live test client, only once."""
         super().setUp()
-        if not hasattr(self.__class__, 'client'):
-            self.__class__.client = self.live_client_class(self.live_server_url)
-        self.client = self.__class__.client
+        if not hasattr(type(self), 'client'):
+            type(self).client = self.live_client_class(self.live_server_url)
+        self.client = type(self).client
 
     @classmethod
     def tearDownClass(cls):  # pylint:disable=invalid-name
         """Quit the live-test client and call super's tearDownClass."""
         if hasattr(cls, 'client'):
             cls.client.quit()
         super().tearDownClass()
```

### Comparing `pytoolbox-14.8.0/pytoolbox/selenium/webdrivers.py` & `pytoolbox-14.8.1/pytoolbox/selenium/webdrivers.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/selenium/webelements/base.py` & `pytoolbox-14.8.1/pytoolbox/selenium/webelements/base.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/selenium/webelements/bootstrap_slider.py` & `pytoolbox-14.8.1/pytoolbox/selenium/webelements/bootstrap_slider.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/serialization.py` & `pytoolbox-14.8.1/pytoolbox/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .types import get_slots
 
 _all = module.All(globals())
 
 
 # Data -> File -------------------------------------------------------------------------------------
 
+
 def to_file(
     path,
     data=None,
     pickle_data=None,
     *,
     binary=False,
     safe=False,
@@ -97,14 +98,15 @@
     if safe:
         os.rename(write_path, path)
     return backup_path if backup else None
 
 
 # Object <-> Pickle file ---------------------------------------------------------------------------
 
+
 class PickleableObject(object):
     """An :class:`object` serializable/deserializable by :mod:`pickle`."""
     @classmethod
     def read(cls, path, *, store_path=False, create_if_error=False, **kwargs):
         """Return a deserialized instance of a pickleable object loaded from a file."""
         try:
             with open(path, 'rb') as f:
@@ -139,14 +141,15 @@
                 self._pickle_path = path  # pylint:disable=attribute-defined-outside-init
             elif pickle_path:
                 self._pickle_path = pickle_path  # pylint:disable=attribute-defined-outside-init
 
 
 # Object <-> JSON string ---------------------------------------------------------------------------
 
+
 # http://stackoverflow.com/questions/6255387/mongodb-object-serialized-as-json
 class SmartJSONEncoderV1(json.JSONEncoder):
 
     def default(self, obj):  # pylint:disable=arguments-differ
         if ObjectId is not None and isinstance(obj, ObjectId):
             return str(obj)
         if hasattr(obj, '__dict__'):
@@ -364,14 +367,15 @@
     def from_json(cls, json_string, inspect_constructor):
         """Deserialize a JSON string to an instance of `JsoneableObject`."""
         return dict_to_object(cls, json.loads(json_string), inspect_constructor)
 
 
 # Object <-> Dictionary ----------------------------------------------------------------------------
 
+
 def object_to_dict(
     obj,
     schema,
     *,
     depth=0,
     callback=lambda o, s, d: (o, s),
     iterable_callback=lambda o, s, d: list
@@ -611,24 +615,25 @@
 
     extra_slots = None
 
     def to_dict(self, *, extra_slots=True):
         self_dict = {}
         slots = set(s for s in get_slots(self) if s[0] != '_')
         if extra_slots:
-            slots.update(self.__class__.extra_slots or [])
+            slots.update(type(self).extra_slots or [])
         for attribute in slots:
             value = getattr(self, attribute)
             if value is not None:
                 self_dict[attribute] = value
         return self_dict
 
 
 # YAML ---------------------------------------------------------------------------------------------
 
+
 YamlDataTypes: TypeAlias = dict | list | str | None
 
 
 def get_yaml(
     *,
     mapping: int = 2,
     sequence: int = 4,
```

### Comparing `pytoolbox-14.8.0/pytoolbox/signals.py` & `pytoolbox-14.8.1/pytoolbox/signals.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/ssh.py` & `pytoolbox-14.8.1/pytoolbox/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from __future__ import annotations
 
 from collections.abc import Iterator
 from pathlib import Path
 from typing import Final
 import contextlib
-import logging
 import os
 import re
 import signal
 import stat
 import tempfile
 
-from . import exceptions, subprocess
+from . import exceptions, logging, subprocess
 
 __all__ = [
     'AGENT_START_REGEX',
     'add_fingerprint',
     'add_key',
     'is_agent_up',
     'scoped_agent',
     'start_agent',
     'stop_agent',
     'ssh'
 ]
 
-log = logging.getLogger(__name__)
+log = logging.get_logger(__name__)
 
 AGENT_START_REGEX: Final[re.Pattern] = re.compile(
     r'SSH_AUTH_SOCK=(?P<SSH_AUTH_SOCK>[^;]+).*'
     r'SSH_AGENT_PID=(?P<SSH_AGENT_PID>\d+)',
     re.MULTILINE | re.DOTALL)
```

### Comparing `pytoolbox-14.8.0/pytoolbox/states.py` & `pytoolbox-14.8.1/pytoolbox/states.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/string.py` & `pytoolbox-14.8.1/pytoolbox/string.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/subprocess.py` & `pytoolbox-14.8.1/pytoolbox/subprocess.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,33 @@
 from __future__ import annotations
 
-from collections.abc import Iterable
+from collections.abc import Callable, Iterable
 from pathlib import Path
-from typing import Final, TypeAlias
+from typing import TypeAlias, TypedDict
 import errno
 import fcntl
 import grp
-import logging
 import multiprocessing
 import os
 import pwd
 import random
 import re
 import setuptools.archive_util
 import shlex
 import shutil
 import subprocess
 import threading
 import time
 
 from . import exceptions, filesystem, module
-from .logging import LoggerType, get_logger
 from .decorators import deprecated
-
-log = logging.getLogger(__name__)
+from .logging import get_logger, LoggerType
 
 _all = module.All(globals())
 
-EMPTY_CMD_RETURN: Final[dict[str, None]] = {
-    'process': None,
-    'stdout': None,
-    'stderr': None,
-    'returncode': None
-}
-
 # import Popen on steroids if available
 try:
     from psutil import NoSuchProcess, Popen
 except ImportError:
     from subprocess import Popen
     NoSuchProcess = None
 
@@ -49,26 +39,34 @@
 
 # Better to warn user than letting converting to string Any!
 # None will be stripped automatically
 CallArgType: TypeAlias = int | float | str | Path | None
 CallArgsType: TypeAlias = str | Iterable[CallArgType]
 
 
-def kill(process):
+class CallResult(TypedDict):
+    process: Popen | None
+    returncode: int
+    stdout: bytes | None
+    stderr: bytes | None
+    exception: OSError | None
+
+
+def kill(process: Popen) -> None:
     try:
         process.kill()
     except OSError as ex:
         if ex.errno != errno.ESRCH:
             raise
     except Exception as ex:  # pylint:disable=broad-except
         if not NoSuchProcess or not isinstance(ex, NoSuchProcess):
             raise
 
 
-def su(user, group):  # pylint:disable=invalid-name
+def su(user: str | int, group: str | int) -> Callable:  # pylint:disable=invalid-name
     """
     Return a function to change current user/group id.
 
     **Example usage**
 
     >> import subprocess
     >> subprocess.call(['ls', '/'], preexec_fn=su(1000, 1000))
@@ -77,21 +75,21 @@
     def set_ids():
         os.setgid(grp.getgrnam(group).gr_gid if isinstance(group, str) else group)
         os.setuid(pwd.getpwnam(user).pw_uid if isinstance(user, str) else user)
     return set_ids
 
 
 # http://stackoverflow.com/a/7730201/190597
-def make_async(fd):  # pylint:disable=invalid-name
+def make_async(fd) -> None:  # pylint:disable=invalid-name
     """Add the O_NONBLOCK flag to a file descriptor."""
     fcntl.fcntl(fd, fcntl.F_SETFL, fcntl.fcntl(fd, fcntl.F_GETFL) | os.O_NONBLOCK)
 
 
 # http://stackoverflow.com/a/7730201/190597
-def read_async(fd):  # pylint:disable=invalid-name
+def read_async(fd) -> str:  # pylint:disable=invalid-name
     """Read some data from a file descriptor, ignoring EAGAIN errors."""
     try:
         return fd.read()
     except IOError as ex:
         if ex.errno == errno.EAGAIN:
             return ''
         raise
@@ -107,14 +105,15 @@
     if not args:
         return ''
     return args if isinstance(args, str) else ' '.join(quote(str(a)) for a in args if a is not None)
 
 
 # --------------------------------------------------------------------------------------------------
 
+
 def raw_cmd(arguments: CallArgsType, *, shell: bool = False, **kwargs) -> Popen:
     """
     Launch a subprocess.
 
     This function ensure that:
 
     * subprocess arguments will be converted to a string if `shell` is True
@@ -124,88 +123,97 @@
     process = Popen(to_args_string(arguments) if shell else arguments, shell=shell, **kwargs)
     if not hasattr(process, 'args'):
         process.args = arguments
     return process
 
 
 # thanks http://stackoverflow.com/questions/1191374$
-def _communicate_with_timeout(*, data, process, input):  # pylint:disable=redefined-builtin
+def _communicate_with_timeout(*, data, process, input) -> None:  # pylint:disable=redefined-builtin
     data['stdout'], data['stderr'] = process.communicate(input=input)
 
 
+# TODO Refine type hints with overloads
 def cmd(  # pylint:disable=too-many-arguments,too-many-branches,too-many-locals,too-many-statements
     command: CallArgsType,
     *,
     user: str | None = None,
     input: str | None = None,  # pylint:disable=redefined-builtin
     cli_input: str | None = None,
     cli_output: bool = False,
     communicate: bool = True,
     timeout: float | None = None,
     fail: bool = True,
-    log: LoggerType = log,  # pylint:disable=redefined-outer-name
+    log: LoggerType = None,  # pylint:disable=redefined-outer-name
     tries: int = 1,
     delay_min: float = 5,
     delay_max: float = 10,
+    success_codes: Iterable[int] = (0, ),
     **kwargs
-) -> dict:
+):
     """
     Calls the `command` and returns a dictionary with process, stdout, stderr, and the returncode.
 
     Returned returncode, stdout and stderr will be None if `communicate` is set to False.
 
     :param command: The command to execute.
     :param user: If set, this will use ``sudo -u <user> ...`` to execute `command` as `user`.
     :param input: If set, sended to stdin (if `communicate` is True).
     :param cli_input: If set, sended to stdin (no condition).
     :param cli_output: Set to True to output (in real-time) stdout to stdout and stderr to stderr.
     :param fail: Set to False to avoid the exception `exceptions.CalledProcessError`.
-    :param log: A function to log/print details about what is executed/any failure, can be a logger.
+    :param log: If set then override the default logger named `pytoolbox.subprocess.cmd.<binary>`.
     :param communicate: Set to True to communicate with the process, this is a locking call
                         (if timeout is None).
     :param timeout: Time-out for the communication with the process, in seconds.
     :param tries: How many times you want the command to be retried ?
     :param delay_min: Minimum delay to sleep after every attempt communicate must be True.
     :param delay_max: Maximum delay to sleep after every attempt communicate must be True.
+    :param success_codes: Terraform plan may return code 3 for modified, so success_codes=(0, 3).
     :param kwargs: Any argument of the :mod:`subprocess`.Popen constructor
                    excepting stdin, stdout and stderr
 
     The delay will be a random number in range (`delay_min`, `delay_max`).
 
     """
-    log = get_logger(log)
-
     # Process arguments
-    args_list = to_args_list(command)
+    process_cmd: list[str] = to_args_list(command)
+    log = get_logger(log or f'{__name__}.cmd.{Path(process_cmd[0]).name}')
+
     if user is not None:
-        args_list = ['sudo', '-u', user, *command]
-    args_string = to_args_string(args_list)
+        process_cmd = ['sudo', '-u', user, *process_cmd]
 
     # log the execution
     log.debug(''.join([
         'Execute ',
         '' if input is None else f'echo {repr(input)} | ',
-        args_string,
+        to_args_string(process_cmd),
         '' if cli_input is None else f' < {repr(cli_input)}'
     ]))
 
     for trial in range(tries):  # noqa
         # create the sub-process
         try:
             process = Popen(
-                args_list,
+                process_cmd,
                 stdin=subprocess.PIPE,
                 stdout=None if cli_output else subprocess.PIPE,
-                stderr=None if cli_output else subprocess.PIPE, **kwargs)
+                stderr=None if cli_output else subprocess.PIPE,
+                **kwargs)
         except OSError as ex:
             # Unable to execute the program (e.g. does not exist)
             log.exception(ex)
             if fail:
                 raise
-            return {'process': None, 'stdout': '', 'stderr': ex, 'returncode': 2}
+            return {
+                'process': None,
+                'returncode': 2,
+                'stdout': None,
+                'stderr': None,
+                'exception': ex
+            }
 
         # Write to stdin (answer to questions, ...)
         if cli_input is not None:
             process.stdin.write(cli_input)
             process.stdin.flush()
 
         # Interact with the process and wait for the process to terminate
@@ -227,67 +235,61 @@
                         raise
             stdout, stderr = data['stdout'], data['stderr']
         else:
             # get a return code that may be None of course ...
             process.poll()
             stdout = stderr = None
 
-        result = {
+        result: CallResult = {
             'process': process,
+            'returncode': process.returncode,
             'stdout': stdout,
             'stderr': stderr,
-            'returncode': process.returncode
+            'exception': None
         }
 
-        if process.returncode == 0:
+        if process.returncode in success_codes:
             break
 
         # failed attempt, may retry
         do_retry = trial < tries - 1
         delay = random.uniform(delay_min, delay_max)
         log.warning(' '.join([
             f'Attempt {trial + 1} out of {tries}:',
             f'Will retry in {delay} seconds' if do_retry else 'Failed'
         ]))
 
         # raise if this is the last try
         if fail and not do_retry:
             raise exceptions.CalledProcessError(
+                cmd=process_cmd,
                 returncode=process.returncode,
-                cmd=args_string,
                 stdout=stdout,
                 stderr=stderr)
 
         if do_retry:
             time.sleep(delay)
 
     return result
 
 
 # --------------------------------------------------------------------------------------------------
 
-@deprecated
-def git_clone_or_pull(*args, **kwargs) -> None:
-    from pytoolbox.git import clone_or_pull  # pylint:disable=import-outside-toplevel
-    return clone_or_pull(*args, **kwargs)
-
-
-# --------------------------------------------------------------------------------------------------
 
 def make(
     archive: Path,
     directory: Path,
     *,
     with_cmake: bool = False,
     configure_options: str = '',
     install: bool = True,
     remove_temporary: bool = True,
     make_options: str = f'-j{multiprocessing.cpu_count()}',
     **kwargs
-) -> dict[str, dict]:
+) -> dict[str, CallResult]:
     """Build and optionally install a piece of software from source."""
     results = {}
     setuptools.archive_util.unpack_archive(archive, directory)
     with filesystem.chdir(directory):
         if with_cmake:
             filesystem.makedirs(Path('build'))
             os.chdir('build')
@@ -301,14 +303,15 @@
         shutil.rmtree(directory)
 
     return results
 
 
 # --------------------------------------------------------------------------------------------------
 
+
 def rsync(  # pylint:disable=too-many-arguments,too-many-locals
     source: Path,
     destination: Path,
     *,
     source_is_dir: bool = False,
     destination_is_dir: bool = False,
     archive: bool = True,
@@ -318,17 +321,17 @@
     recursive: bool = False,
     simulate: bool = False,
     excludes: Iterable[str] | None = None,
     includes: Iterable[str] | None = None,
     rsync_path: Path | None = None,
     size_only: bool = False,
     extra: str | None = None,
-    extra_args: list[CallArgType] | None = None,
+    extra_args: Iterable[CallArgType] | None = None,
     **kwargs
-) -> dict:
+) -> CallResult:
     """Execute the famous rsync remote (or local) synchronization tool."""
     source_string = str(source)
     if source.is_dir() or source_is_dir:
         source_string += os.sep
 
     destination_string = str(destination)
     if destination.is_dir() or destination_is_dir:
@@ -351,37 +354,46 @@
     if excludes is not None:
         command += [f'--exclude={e}' for e in excludes]
     if includes is not None:
         command += [f'--include={i}' for i in includes]
     if exclude_vcs:
         command += ['--exclude=.svn', '--exclude=.git']
     if extra_args is not None:
-        command += extra_args
+        command.extend(extra_args)
     command += [source_string, destination_string]
 
     return cmd([c for c in command if c], **kwargs)
 
 
 def screen_kill(name: str | None = None, *, fail: bool = True, **kwargs):
     """Kill all screen instances called `name` or all if `name` is None."""
     for instance_name in screen_list(name=name, **kwargs):
         cmd(['screen', '-S', instance_name, '-X', 'quit'], fail=fail, **kwargs)
 
 
-def screen_launch(name: str, command: CallArgsType, **kwargs) -> dict:
+def screen_launch(name: str, command: CallArgsType, **kwargs) -> CallResult:
     """Launch a new named screen instance."""
     return cmd(['screen', '-dmS', name, *to_args_list(command)], **kwargs)
 
 
 def screen_list(name: str | None = None, **kwargs) -> list[str]:
     """Returns a list containing all instances of screen. Can be filtered by `name`."""
     screens = cmd(['screen', '-ls', name], fail=False, **kwargs)['stdout']
-    return re.findall(r'\s+(\d+.\S+)\s+\(.*\).*', screens.decode('utf-8'))
+    return re.findall(r'\s+(\d+.\S+)\s+\(.*\).*', (screens or b'').decode('utf-8'))
 
 
-@deprecated
-def ssh(*args, **kwargs) -> dict:
-    from pytoolbox.ssh import ssh as _ssh
-    return _ssh(*args, **kwargs)
+__all__ = _all.diff(globals())
 
 
-__all__ = _all.diff(globals())
+# Deprecated ---------------------------------------------------------------------------------------
+
+
+@deprecated('Use pytoolbox.git.clone_or_pull instead (drop-in replacement)')
+def git_clone_or_pull(*args, **kwargs) -> None:  # pragma: no cover
+    from pytoolbox.git import clone_or_pull  # pylint:disable=import-outside-toplevel
+    return clone_or_pull(*args, **kwargs)
+
+
+@deprecated('Use pytoolbox.ssh.ssh instead (drop-in replacement)')
+def ssh(*args, **kwargs) -> dict:  # pragma: no cover
+    from pytoolbox.ssh import ssh as _ssh
+    return _ssh(*args, **kwargs)
```

### Comparing `pytoolbox-14.8.0/pytoolbox/throttles.py` & `pytoolbox-14.8.1/pytoolbox/throttles.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/types.py` & `pytoolbox-14.8.1/pytoolbox/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,23 +35,23 @@
     """
     return list(inspect.signature(function).parameters.keys())
 
 
 def get_properties(obj: Any) -> Generator[tuple[str, Any], None, None]:
     return (
         (n, getattr(obj, n))
-        for n, p in inspect.getmembers(obj.__class__, lambda m: isinstance(m, property))
+        for n, p in inspect.getmembers(type(obj), lambda m: isinstance(m, property))
     )
 
 
 def get_slots(obj: Any) -> set[str]:
     """Return a set with the `__slots__` of the `obj` including all parent classes `__slots__`."""
     return set(itertools.chain.from_iterable(
         getattr(cls, '__slots__', ())
-        for cls in obj.__class__.__mro__)
+        for cls in type(obj).__mro__)
     )
 
 
 @overload
 def get_subclasses(obj: Any, *, nested: Literal[True] = True) -> Iterable[type]:
     ...
 
@@ -245,18 +245,18 @@
 
     def __init__(self, name: str, **attrs) -> None:
         assert '_name' not in attrs
         self.__dict__.update(attrs)
         self._name = name
 
     def __getattr__(self, name: str) -> Any:
-        return (self.attr_class or self.__class__)(f'{self._name}.{name}')
+        return (self.attr_class or type(self))(f'{self._name}.{name}')
 
     def __getitem__(self, key: str) -> Any:
-        return (self.attr_class or self.__class__)(f'{self._name}[{repr(key)}]')
+        return (self.attr_class or type(self))(f'{self._name}[{repr(key)}]')
 
     def __str__(self) -> str:
         return self._name
 
 
 class EchoDict(dict):
     """
```

### Comparing `pytoolbox-14.8.0/pytoolbox/unittest.py` & `pytoolbox-14.8.1/pytoolbox/unittest.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/validation.py` & `pytoolbox-14.8.1/pytoolbox/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from collections.abc import Iterable
 from typing import Any, get_type_hints
 from urllib.parse import urlparse
 import errno
 import inspect
 import http.client
 import os
 import re
@@ -207,15 +208,15 @@
 def valid_uri(
     uri: str,
     *,
     check_404: bool,
     scheme_mandatory: bool = False,
     port_mandatory: bool = False,
     default_port: int = 80,
-    excepted_errnos: tuple[int, ...] = (errno.ENOENT, errno.ECONNREFUSED, errno.ENETUNREACH),
+    excepted_errnos: Iterable[int] = (errno.ENOENT, errno.ECONNREFUSED, errno.ENETUNREACH),
     timeout: int | None = None
 ) -> bool:
     """
     Validate an URI.
 
     *Example usage**
 
@@ -306,15 +307,18 @@
         try:
             ObjectId(value)
         except InvalidId:
             return False
     return True
 
 
-def validate_list(the_list: list[Any], regexes: list[re.Pattern | str]) -> bool:
+def validate_list(
+    the_list: list[Any],
+    regexes: list[re.Pattern | str] | tuple[re.Pattern | str, ...]
+) -> None:
     """
     Validate every element of `the_list` with corresponding regular expression picked-in from
     `regexes`.
     """
     if len(the_list) != len(regexes):
         raise IndexError(
             f'{len(the_list)} elements to validate with '
```

### Comparing `pytoolbox-14.8.0/pytoolbox/virtualenv.py` & `pytoolbox-14.8.1/pytoolbox/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox/voluptuous.py` & `pytoolbox-14.8.1/pytoolbox/voluptuous.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox.egg-info/PKG-INFO` & `pytoolbox-14.8.1/pytoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoolbox
-Version: 14.8.0
+Version: 14.8.1
 Summary: Toolbox for Python scripts
 Home-page: https://github.com/davidfischer-ch/pytoolbox
 Author: David Fischer
 Author-email: david@fisch3r.net
 License: EUPL 1.1
 Keywords: celery,ffmpeg,django,flask,json,juju,mock,pillow,rsync,rtp,selenium,smpte 2022-1,screen,subprocess
 Classifier: Development Status :: 5 - Production/Stable
@@ -290,8 +290,8 @@
 		  packages=['my_cool_project'])
 
 
 See `pip vcs support <http://www.pip-installer.org/en/latest/logic.html#vcs-support>`_ to get further details about this.
 
 You also need to install ``git-core``, but it is probably already the case, at least on your development computer ;-)
 
-2014 - 2022 David Fischer
+2012 - 2024 David Fischer
```

### Comparing `pytoolbox-14.8.0/pytoolbox.egg-info/SOURCES.txt` & `pytoolbox-14.8.1/pytoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/pytoolbox.egg-info/requires.txt` & `pytoolbox-14.8.1/pytoolbox.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/setup.py` & `pytoolbox-14.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_collections.py` & `pytoolbox-14.8.1/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_comparison.py` & `pytoolbox-14.8.1/tests/test_comparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     point_3 = Point3D(10, -4, 2, 'dot')
     if point_1 in (point_2, point_3):
         raise AssertionError()
 
 
 # Content ------------------------------------------------------------------------------------------
 
+
 def test_unified_diff() -> None:
     assert comparison.unified_diff(
         'Some T',
         'Other T',
         fromfile='a.py',
         tofile='b.py',
         colorize=False) == ("""
@@ -95,14 +96,15 @@
 \x1b[31m-Some T\x1b[0m
 \x1b[32m+Other T\x1b[0m
 """).strip()
 
 
 # Versions -----------------------------------------------------------------------------------------
 
+
 @mark.parametrize(('version_a', 'version_b', 'operation', 'expected'), [
     ('master', 'master', '<', False),
     ('master', 'master', '<=', True),
     ('master', 'master', '==', True),
     ('master', 'master', '!=', False),
     ('master', 'master', '>=', True),
     ('master', 'master', '>', False),
```

### Comparing `pytoolbox-14.8.0/tests/test_console.py` & `pytoolbox-14.8.1/tests/test_console.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_decorators.py` & `pytoolbox-14.8.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_django_utils.py` & `pytoolbox-14.8.1/tests/test_django_utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_ffmpeg.py` & `pytoolbox-14.8.1/tests/test_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_filesystem.py` & `pytoolbox-14.8.1/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_git.py` & `pytoolbox-14.8.1/tests/test_git.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from pathlib import Path
-from unittest.mock import patch as M
 from typing import Final
+from unittest.mock import patch
 import os
 import tempfile
 
 import pytest
 from pytest import raises
 
 from pytoolbox import exceptions, git, subprocess
@@ -52,24 +52,24 @@
     git.create_tag(pytoolbox_git, 'z2.0')
     tags = git.get_tags(pytoolbox_git)
     assert 'z1.0' in tags and 'z2.0' in tags
 
 
 def test_get_ref(pytoolbox_git: Path) -> None:
     get_ref = git.get_ref
-    with M.dict(os.environ, {}, clear=True):
+    with patch.dict(os.environ, {}, clear=True):
         assert get_ref(pytoolbox_git, kind='branch') == 'main'
         assert get_ref(pytoolbox_git, kind='commit') == '4863c99a97fe358caa24e48b5c477b852b5a6721'
         with raises(exceptions.GitReferenceError):
             get_ref(tempfile.gettempdir())
 
 
 def test_get_ref_from_gitlab_ci(pytoolbox_git: Path) -> None:
     get_ref = git.get_ref
-    with M.dict(os.environ, {'CI_COMMIT_REF_NAME': 'toto'}, clear=True):
+    with patch.dict(os.environ, {'CI_COMMIT_REF_NAME': 'toto'}, clear=True):
         assert get_ref(pytoolbox_git, kind='branch') == 'toto'
         assert get_ref(pytoolbox_git, kind='commit') == 'toto'
         assert get_ref(pytoolbox_git, kind='branch', ci_vars=False) != 'toto'
         assert get_ref(pytoolbox_git, kind='commit', ci_vars=False) != 'toto'
 
 
 def test_get_tags(pytoolbox_git: Path) -> None:  # pylint:disable=redefined-outer-name
@@ -84,15 +84,15 @@
     assert tags(pytoolbox_git, ref='0b87f1b5cf21e18205e334652167c1055d0b4c13') == []
     git.create_tag(pytoolbox_git, 'some-tag')
     git.create_tag(pytoolbox_git, 'other-tag')
     assert tags(pytoolbox_git, ref='HEAD') == ['14.7.0', 'other-tag', 'some-tag']
 
 
 def test_scoped_ssh_key() -> None:
-    with M('pytoolbox.subprocess.cmd') as cmd:
+    with patch('pytoolbox.subprocess.cmd') as cmd:
         cmd.return_value = {'stdout': None, 'stderr': None, 'returncode': 0}
         with git.scoped_ssh_key('.', 'key-data') as name:
             subprocess.cmd(['git', 'push', 'somewhere'])
 
         assert [args for args, kwargs in cmd.call_args_list] == [
             ([
                 'git', 'config', 'core.sshCommand',
@@ -100,17 +100,21 @@
             ], ),
             (['git', 'push', 'somewhere'], ),
             (['git', 'config', '--unset', 'core.sshCommand'], )
         ]
 
 
 def test_scoped_ssh_key_with_options() -> None:
-    with M('pytoolbox.subprocess.cmd') as cmd:
+    with patch('pytoolbox.subprocess.cmd') as cmd:
         cmd.return_value = {'stdout': None, 'stderr': None, 'returncode': 0}
-        with git.scoped_ssh_key('.', 'key-data', options=['StrictHostKeyChecking=no']) as name:
+        with git.scoped_ssh_key(
+            Path('.'),
+            'key-data',
+            options=['StrictHostKeyChecking=no']
+        ) as name:
             subprocess.cmd(['git', 'push', 'somewhere'])
             assert Path(name).read_text(encoding='utf-8') == 'key-data\n'
 
         assert not Path(name).exists()
         assert [args for args, kwargs in cmd.call_args_list] == [
             ([
                 'git', 'config', 'core.sshCommand',
```

### Comparing `pytoolbox-14.8.0/tests/test_juju.py` & `pytoolbox-14.8.1/tests/test_juju.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_module.py` & `pytoolbox-14.8.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_private.py` & `pytoolbox-14.8.1/tests/test_private.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_regex.py` & `pytoolbox-14.8.1/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_serialization.py` & `pytoolbox-14.8.1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_signals.py` & `pytoolbox-14.8.1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_ssh.py` & `pytoolbox-14.8.1/tests/test_ssh.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_states.py` & `pytoolbox-14.8.1/tests/test_states.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_string.py` & `pytoolbox-14.8.1/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_unittest.py` & `pytoolbox-14.8.1/tests/test_unittest.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.0/tests/test_validation.py` & `pytoolbox-14.8.1/tests/test_validation.py`

 * *Files identical despite different names*

