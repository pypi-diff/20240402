# Comparing `tmp/zibanu-django-1.3.4.tar.gz` & `tmp/zibanu-django-1.3.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibanu-django-1.3.4.tar", last modified: Fri Feb 23 16:33:21 2024, max compression
+gzip compressed data, was "zibanu-django-1.3.5rc0.tar", last modified: Tue Apr  2 16:54:02 2024, max compression
```

## Comparing `zibanu-django-1.3.4.tar` & `zibanu-django-1.3.5rc0.tar`

### file list

```diff
@@ -1,99 +1,102 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.226515 zibanu-django-1.3.4/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.3.4/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      105 2023-08-07 23:22:31.000000 zibanu-django-1.3.4/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    68384 2024-02-23 16:33:21.225515 zibanu-django-1.3.4/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    27020 2023-09-12 12:23:03.000000 zibanu-django-1.3.4/README.md
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      932 2024-02-23 16:32:52.000000 zibanu-django-1.3.4/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2024-02-23 16:33:21.226515 zibanu-django-1.3.4/setup.cfg
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.217515 zibanu-django-1.3.4/zibanu/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      618 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.217515 zibanu-django-1.3.4/zibanu/django/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/django/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.217515 zibanu-django-1.3.4/zibanu/django/api/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      312 2023-07-07 11:33:04.000000 zibanu-django-1.3.4/zibanu/django/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.217515 zibanu-django-1.3.4/zibanu/django/api/services/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      447 2023-08-08 16:47:24.000000 zibanu-django-1.3.4/zibanu/django/api/services/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1301 2023-11-09 21:33:49.000000 zibanu-django-1.3.4/zibanu/django/api/services/language.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1280 2023-11-09 21:33:59.000000 zibanu-django-1.3.4/zibanu/django/api/services/timezone.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1147 2023-11-07 20:39:50.000000 zibanu-django-1.3.4/zibanu/django/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.218515 zibanu-django-1.3.4/zibanu/django/db/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/django/db/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.218515 zibanu-django-1.3.4/zibanu/django/db/backends/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      500 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/django/db/backends/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.218515 zibanu-django-1.3.4/zibanu/django/db/backends/oracle/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      500 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/django/db/backends/oracle/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1572 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/django/db/backends/oracle/base.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.218515 zibanu-django-1.3.4/zibanu/django/db/models/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      761 2023-08-09 14:54:09.000000 zibanu-django-1.3.4/zibanu/django/db/models/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1120 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/django/db/models/dated_model.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1593 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/django/db/models/manager.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2082 2024-02-15 02:14:26.000000 zibanu-django-1.3.4/zibanu/django/db/models/model.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.218515 zibanu-django-1.3.4/zibanu/django/lib/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      536 2024-01-30 16:24:02.000000 zibanu-django-1.3.4/zibanu/django/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.219515 zibanu-django-1.3.4/zibanu/django/lib/classes/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      644 2024-02-01 21:22:22.000000 zibanu-django-1.3.4/zibanu/django/lib/classes/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     5879 2024-02-23 16:24:08.000000 zibanu-django-1.3.4/zibanu/django/lib/classes/code_generator.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1182 2024-01-30 21:26:52.000000 zibanu-django-1.3.4/zibanu/django/lib/classes/extended_json_encoder.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      731 2024-01-30 14:05:23.000000 zibanu-django-1.3.4/zibanu/django/lib/classes/model_name.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.215515 zibanu-django-1.3.4/zibanu/django/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.215515 zibanu-django-1.3.4/zibanu/django/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.219515 zibanu-django-1.3.4/zibanu/django/locale/es/LC_MESSAGES/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2493 2024-02-14 01:42:00.000000 zibanu-django-1.3.4/zibanu/django/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 macercha  (1000) macercha  (1000)     4500 2024-02-14 01:43:43.000000 zibanu-django-1.3.4/zibanu/django/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.220515 zibanu-django-1.3.4/zibanu/django/rest_framework/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2198 2023-08-07 23:25:47.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/decorators.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.220515 zibanu-django-1.3.4/zibanu/django/rest_framework/exceptions/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1151 2023-11-09 16:02:26.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/exceptions/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     3186 2024-02-07 15:44:25.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/exceptions/api_exception.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      873 2023-11-09 16:02:26.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/exceptions/api_not_implemented_exception.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      779 2023-11-08 11:26:40.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/exceptions/multiple_login_error.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.220515 zibanu-django-1.3.4/zibanu/django/rest_framework/fields/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      718 2023-08-12 22:42:09.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/fields/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1343 2023-07-28 21:32:14.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/fields/current_user_default.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     3394 2024-02-12 11:17:08.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/fields/hybrid_image.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.221515 zibanu-django-1.3.4/zibanu/django/rest_framework/permissions/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      652 2023-11-08 21:21:04.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/permissions/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1174 2023-11-08 11:44:33.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/permissions/is_owner_or_read_only.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.221515 zibanu-django-1.3.4/zibanu/django/rest_framework/serializers/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1649 2023-08-12 22:42:51.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/serializers/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      646 2023-08-09 14:54:09.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/serializers/fields.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      863 2023-11-08 11:01:17.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/serializers/model_serializer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.222515 zibanu-django-1.3.4/zibanu/django/rest_framework/viewsets/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      779 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/viewsets/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)    13771 2024-02-23 00:07:48.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/viewsets/model_viewset.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1737 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/django/rest_framework/viewsets/viewset.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.222515 zibanu-django-1.3.4/zibanu/django/template/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      501 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/django/template/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      825 2023-07-29 16:10:50.000000 zibanu-django-1.3.4/zibanu/django/template/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.222515 zibanu-django-1.3.4/zibanu/django/template/context_processors/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      619 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/django/template/context_processors/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1055 2023-07-29 12:19:18.000000 zibanu-django-1.3.4/zibanu/django/template/context_processors/full_static_uri.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      819 2023-07-29 12:19:18.000000 zibanu-django-1.3.4/zibanu/django/template/context_processors/site.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.216515 zibanu-django-1.3.4/zibanu/django/template/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.216515 zibanu-django-1.3.4/zibanu/django/template/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.222515 zibanu-django-1.3.4/zibanu/django/template/locale/es/LC_MESSAGES/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      709 2024-02-14 01:42:00.000000 zibanu-django-1.3.4/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1083 2024-02-14 01:43:43.000000 zibanu-django-1.3.4/zibanu/django/template/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.223515 zibanu-django-1.3.4/zibanu/django/template/templatetags/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      501 2023-07-29 12:07:00.000000 zibanu-django-1.3.4/zibanu/django/template/templatetags/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2317 2023-07-29 12:33:40.000000 zibanu-django-1.3.4/zibanu/django/template/templatetags/static_uri.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      889 2023-07-29 12:34:47.000000 zibanu-django-1.3.4/zibanu/django/template/templatetags/string_concat.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2673 2023-08-10 09:09:24.000000 zibanu-django-1.3.4/zibanu/django/template/templatetags/subtotal_dict.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1549 2023-07-29 12:45:14.000000 zibanu-django-1.3.4/zibanu/django/template/templatetags/sum_dict.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      655 2023-08-08 16:47:24.000000 zibanu-django-1.3.4/zibanu/django/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.224515 zibanu-django-1.3.4/zibanu/django/utils/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1005 2024-02-13 01:57:52.000000 zibanu-django-1.3.4/zibanu/django/utils/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1986 2023-09-13 12:35:19.000000 zibanu-django-1.3.4/zibanu/django/utils/date_time.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1168 2023-07-29 15:01:10.000000 zibanu-django-1.3.4/zibanu/django/utils/error_messages.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     7608 2024-02-07 15:45:27.000000 zibanu-django-1.3.4/zibanu/django/utils/mail.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2423 2024-01-30 14:39:02.000000 zibanu-django-1.3.4/zibanu/django/utils/model_utils.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1263 2023-12-12 00:48:58.000000 zibanu-django-1.3.4/zibanu/django/utils/receivers_utils.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1511 2024-01-30 21:29:36.000000 zibanu-django-1.3.4/zibanu/django/utils/request_utils.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1559 2024-02-07 15:47:04.000000 zibanu-django-1.3.4/zibanu/django/utils/user_utils.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-23 16:33:21.225515 zibanu-django-1.3.4/zibanu_django.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    68384 2024-02-23 16:33:21.000000 zibanu-django-1.3.4/zibanu_django.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2852 2024-02-23 16:33:21.000000 zibanu-django-1.3.4/zibanu_django.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2024-02-23 16:33:21.000000 zibanu-django-1.3.4/zibanu_django.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       91 2024-02-23 16:33:21.000000 zibanu-django-1.3.4/zibanu_django.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2024-02-23 16:33:21.000000 zibanu-django-1.3.4/zibanu_django.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.374563 zibanu-django-1.3.5rc0/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.3.5rc0/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      105 2023-08-07 23:22:31.000000 zibanu-django-1.3.5rc0/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    68387 2024-04-02 16:54:02.374563 zibanu-django-1.3.5rc0/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    27020 2023-09-12 12:23:03.000000 zibanu-django-1.3.5rc0/README.md
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      935 2024-04-02 16:32:39.000000 zibanu-django-1.3.5rc0/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2024-04-02 16:54:02.374563 zibanu-django-1.3.5rc0/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.362563 zibanu-django-1.3.5rc0/zibanu/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      618 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.362563 zibanu-django-1.3.5rc0/zibanu/django/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.363563 zibanu-django-1.3.5rc0/zibanu/django/api/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      312 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.363563 zibanu-django-1.3.5rc0/zibanu/django/api/services/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      447 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/api/services/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1301 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/api/services/language.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1280 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/api/services/timezone.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1147 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.363563 zibanu-django-1.3.5rc0/zibanu/django/db/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/db/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.364563 zibanu-django-1.3.5rc0/zibanu/django/db/backends/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      500 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/db/backends/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.364563 zibanu-django-1.3.5rc0/zibanu/django/db/backends/oracle/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      500 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/db/backends/oracle/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1572 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/db/backends/oracle/base.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.364563 zibanu-django-1.3.5rc0/zibanu/django/db/models/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      761 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/db/models/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1120 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/db/models/dated_model.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1593 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/db/models/manager.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2082 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/db/models/model.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.365563 zibanu-django-1.3.5rc0/zibanu/django/lib/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      536 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.365563 zibanu-django-1.3.5rc0/zibanu/django/lib/classes/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      644 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/lib/classes/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     5879 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/lib/classes/code_generator.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1182 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/lib/classes/extended_json_encoder.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      731 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/lib/classes/model_name.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.359563 zibanu-django-1.3.5rc0/zibanu/django/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.359563 zibanu-django-1.3.5rc0/zibanu/django/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.366563 zibanu-django-1.3.5rc0/zibanu/django/locale/es/LC_MESSAGES/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2493 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     4500 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.366563 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2197 2024-03-13 14:44:10.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/decorators.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.367563 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/exceptions/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1171 2024-03-15 01:58:14.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/exceptions/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     3076 2024-03-15 01:58:14.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/exceptions/api_exception.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      850 2024-03-11 22:02:32.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/exceptions/multiple_login_error.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      957 2024-03-15 01:58:14.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/exceptions/not_implemented_exception.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1058 2024-03-18 23:17:34.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/exceptions/permission_denied.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.368563 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/fields/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      718 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/fields/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1343 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/fields/current_user_default.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     3394 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/fields/hybrid_image.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.368563 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/permissions/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      652 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/permissions/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1174 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/permissions/is_owner_or_read_only.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.368563 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/serializers/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1649 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/serializers/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      646 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/serializers/fields.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      863 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/serializers/model_serializer.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1031 2024-03-19 00:59:35.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/utils.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.369563 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/viewsets/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      779 2024-03-19 00:59:46.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/viewsets/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    15023 2024-03-18 23:38:48.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/viewsets/model_viewset.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1737 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/rest_framework/viewsets/viewset.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.369563 zibanu-django-1.3.5rc0/zibanu/django/template/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      501 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/template/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      825 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/template/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.370563 zibanu-django-1.3.5rc0/zibanu/django/template/context_processors/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      619 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/template/context_processors/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1055 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/template/context_processors/full_static_uri.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      819 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/template/context_processors/site.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.361563 zibanu-django-1.3.5rc0/zibanu/django/template/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.361563 zibanu-django-1.3.5rc0/zibanu/django/template/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.370563 zibanu-django-1.3.5rc0/zibanu/django/template/locale/es/LC_MESSAGES/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      709 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1083 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/template/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.371563 zibanu-django-1.3.5rc0/zibanu/django/template/templatetags/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      501 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/template/templatetags/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2317 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/template/templatetags/static_uri.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      889 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/template/templatetags/string_concat.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2673 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/template/templatetags/subtotal_dict.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1549 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/template/templatetags/sum_dict.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      655 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.372563 zibanu-django-1.3.5rc0/zibanu/django/utils/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1075 2024-03-12 21:02:22.000000 zibanu-django-1.3.5rc0/zibanu/django/utils/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1986 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/utils/date_time.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1168 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/utils/error_messages.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1493 2024-03-12 21:02:08.000000 zibanu-django-1.3.5rc0/zibanu/django/utils/generic_utils.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     7608 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/utils/mail.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2423 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/utils/model_utils.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1263 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/utils/receivers_utils.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1511 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/utils/request_utils.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1559 2024-03-11 02:33:38.000000 zibanu-django-1.3.5rc0/zibanu/django/utils/user_utils.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:54:02.373563 zibanu-django-1.3.5rc0/zibanu_django.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    68387 2024-04-02 16:54:02.000000 zibanu-django-1.3.5rc0/zibanu_django.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2984 2024-04-02 16:54:02.000000 zibanu-django-1.3.5rc0/zibanu_django.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2024-04-02 16:54:02.000000 zibanu-django-1.3.5rc0/zibanu_django.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       91 2024-04-02 16:54:02.000000 zibanu-django-1.3.5rc0/zibanu_django.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2024-04-02 16:54:02.000000 zibanu-django-1.3.5rc0/zibanu_django.egg-info/top_level.txt
```

### Comparing `zibanu-django-1.3.4/LICENSE` & `zibanu-django-1.3.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/PKG-INFO` & `zibanu-django-1.3.5rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.3.4
+Version: 1.3.5rc0
 Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-1.3.4/README.md` & `zibanu-django-1.3.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/pyproject.toml` & `zibanu-django-1.3.5rc0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zibanu-django"
-version = "1.3.4"
+version = "1.3.5-rc"
 authors = [
     { name = "Mario Cerón", email = "mario.ceron@cqinversiones.co" }
 ]
 description = "Zibanu library for django projects"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `zibanu-django-1.3.4/zibanu/__init__.py` & `zibanu-django-1.3.5rc0/zibanu/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/api/services/language.py` & `zibanu-django-1.3.5rc0/zibanu/django/api/services/language.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/api/services/timezone.py` & `zibanu-django-1.3.5rc0/zibanu/django/api/services/timezone.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/apps.py` & `zibanu-django-1.3.5rc0/zibanu/django/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/db/backends/oracle/base.py` & `zibanu-django-1.3.5rc0/zibanu/django/db/backends/oracle/base.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/db/models/__init__.py` & `zibanu-django-1.3.5rc0/zibanu/django/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/db/models/dated_model.py` & `zibanu-django-1.3.5rc0/zibanu/django/db/models/dated_model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/db/models/manager.py` & `zibanu-django-1.3.5rc0/zibanu/django/db/models/manager.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/db/models/model.py` & `zibanu-django-1.3.5rc0/zibanu/django/db/models/model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/lib/__init__.py` & `zibanu-django-1.3.5rc0/zibanu/django/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/lib/classes/__init__.py` & `zibanu-django-1.3.5rc0/zibanu/django/lib/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/lib/classes/code_generator.py` & `zibanu-django-1.3.5rc0/zibanu/django/lib/classes/code_generator.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/lib/classes/extended_json_encoder.py` & `zibanu-django-1.3.5rc0/zibanu/django/lib/classes/extended_json_encoder.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/lib/classes/model_name.py` & `zibanu-django-1.3.5rc0/zibanu/django/lib/classes/model_name.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.3.5rc0/zibanu/django/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.3.5rc0/zibanu/django/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/decorators.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 # Developed by: macercha
 # Date:         27/04/23 9:57
 # Project:      Zibanu - Django
 # Module Name:  decorators
 # Description:
 # ****************************************************************
 from django.contrib.auth.decorators import user_passes_test
-from django.core.exceptions import PermissionDenied
 from django.utils.translation import gettext_lazy as _
 from typing import Any
+from zibanu.django.rest_framework.exceptions import PermissionDenied
 from zibanu.django.utils import get_user_object
 
 
 def permission_required(permissions: Any, raise_exception=True):
     """
     Decorator to validate permissions from django auth structure. SimpleJWT compatible.
 
@@ -57,10 +57,10 @@
         if "is_staff" in perms:
             is_staff = True
             perms = tuple([perm for perm in perms if perm != "is_staff"])
 
         if (len(perms) > 0 and local_user.has_perms(perms)) or (is_staff and local_user.is_staff) or local_user.is_superuser:
             b_return = True
         elif raise_exception:
-            raise PermissionDenied(_("You do not have permission to perform this action."), "not_authorized")
+            raise PermissionDenied(_("You do not have permission to perform this action."))
         return b_return
     return user_passes_test(check_perms)
```

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/exceptions/api_exception.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/exceptions/api_exception.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,23 +7,37 @@
 # IDE:          PyCharm
 # Developed by: macercha
 # Date:         14/12/22 4:14 AM
 # Project:      Zibanu Django Project
 # Module Name:  api_exception
 # Description:
 # ****************************************************************
-import json
+import logging
+import traceback
+from typing import Any
+
 from django.utils.translation import gettext_lazy as _
+from rest_framework import status
 from rest_framework.exceptions import APIException as SourceException
+from zibanu.django.utils import object_to_list
+
+
+class ApiError:
+    errors = list
+    code = "api_exception"
 
 
 class APIException(SourceException):
     """
     Inherited class from rest_framework.exceptions.ApiException
     """
+    default_detail = _("API Exception")
+    default_code = "api_exception"
+    status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
+
     __default_messages = {
         "304": _("Object has not been created."),
         "400": _("Generic error."),
         "401": _("You are not authorized for this resource."),
         "403": _("You do not have permission to perform this action."),
         "404": _("Object does not exists."),
         "406": _("Data validation error."),
@@ -38,51 +52,43 @@
         "403": "forbidden",
         "404": "not_found",
         "406": "validation_error",
         "412": "precondition_failed",
         "500": "not_controlled_exception"
     }
 
-    def __init__(self, detail: str = None, code: str = None, status_code: int = None, **kwargs) -> None:
+    def __init__(self, detail: Any = None, code: str = None, status_code: int = None, **kwargs) -> None:
         """
-        Constructor method
+        Overwrite constructor method
 
         Parameters
         ----------
         detail : str: String message to be sent through exception.
         code : str: String exception code to be sent through exception.
         http_status: int: HTTP Status code
         msg: Message to send trough exception. (Legacy)
         error: Error code or long description. (Legacy)
         """
         if status_code is not None:
             self.status_code = status_code
         else:
-            self.status_code = kwargs.get("http_status", 500)
+            self.status_code = kwargs.get("http_status", self.status_code)
 
-        str_status_code = str(self.status_code)
+        # Set detail from msg if exists and detail is None
+        if detail is None:
+            detail = kwargs.get("msg", self.default_detail)
 
-        # Set default detail
-        # TODO: Optimize procedure
-        if detail is not None:
-            if isinstance(detail, (list, tuple)):
-                self.default_detail = "".join(map(str, detail))
-            elif isinstance(detail, dict):
-                self.default_detail = json.dumps(detail)
-            else:
-                self.default_detail = detail
-        elif "msg" in kwargs:
-            self.default_detail = kwargs.get("msg")
-        else:
-            if str_status_code in self.__default_messages:
-                self.default_detail = self.__default_messages.get(str_status_code)
+        # Set default detail based on detail object
+        detail = object_to_list(detail)
 
         # Set default code
-        if code is not None:
-            self.default_code = code
-        elif "error" in kwargs:
-            self.default_code = kwargs.get("error")
-        else:
-            if str_status_code in self.__default_codes:
-                self.default_code = self.__default_codes.get(str_status_code)
+        if code is None:
+            code = kwargs.get("error", self.default_code)
 
-        super().__init__()
+        self.detail = {
+            "errors": detail.copy(),
+            "code": code
+        }
+
+        # Save Logging
+        logging.error(self.default_detail)
+        logging.debug(traceback.format_exc())
```

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/exceptions/api_not_implemented_exception.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/exceptions/not_implemented_exception.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,11 +14,14 @@
 # Default imports
 import logging
 import traceback
 from django.utils.translation import gettext_lazy as _
 from .api_exception import APIException
 from rest_framework import status
 
-class APINotImplementedException(APIException):
-    status_code = status.HTTP_405_METHOD_NOT_ALLOWED
-    default_detail = _("Service not implemented")
-    default_code = "not_implemented"
+
+class NotImplementedException(APIException):
+    """
+    Class to raise error for not implemented method
+    """
+    def __init__(self):
+        super().__init__(detail=_("Service not implemented"), code="not_implemented", status_code=status.HTTP_405_METHOD_NOT_ALLOWED)
```

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/exceptions/multiple_login_error.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/exceptions/multiple_login_error.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,13 @@
 # Description:
 # ****************************************************************
 # Default imports
 from .api_exception import APIException
 from rest_framework import status
 
 
-
 class MultipleLoginError(APIException):
     """
     Override class for ValidationError
     """
-    status_code = status.HTTP_412_PRECONDITION_FAILED
-    default_code = "multiple_login"
+    def __init__(self, detail: str = None):
+        super().__init__(detail=detail, status_code=status.HTTP_412_PRECONDITION_FAILED, code="multiple_login_error")
```

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/fields/__init__.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/fields/current_user_default.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/fields/current_user_default.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/fields/hybrid_image.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/fields/hybrid_image.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/permissions/__init__.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/permissions/is_owner_or_read_only.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/permissions/is_owner_or_read_only.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/serializers/__init__.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/serializers/fields.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/serializers/model_serializer.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/serializers/model_serializer.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/viewsets/__init__.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/viewsets/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/viewsets/model_viewset.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/viewsets/model_viewset.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,76 @@
 # IDE:          PyCharm
 # Developed by: macercha
 # Date:         19/12/22 3:18 PM
 # Project:      Zibanu Django Project
 # Module Name:  model_viewset
 # Description:
 # ****************************************************************
-import logging
-import traceback
 from typing import Any
 
 from django.db import DatabaseError
 from django.conf import settings
+from django.utils.translation import gettext_lazy as _
 from django.core.exceptions import ObjectDoesNotExist
+from django.core.exceptions import ValidationError as CoreValidationError
 from rest_framework import authentication
 from rest_framework import permissions
 from rest_framework import status
+from rest_framework.request import Request
 from rest_framework.generics import QuerySet
 from rest_framework.viewsets import ModelViewSet as RestModelViewSet
 from rest_framework.response import Response
+from rest_framework_simplejwt.exceptions import InvalidToken
 from rest_framework_simplejwt.authentication import JWTTokenUserAuthentication
 
 from zibanu.django.rest_framework.exceptions import APIException
-from zibanu.django.rest_framework.exceptions import APINotImplementedException
+from zibanu.django.rest_framework.exceptions import NotImplementedException
 from zibanu.django.rest_framework.exceptions import ValidationError
 from zibanu.django.utils import ErrorMessages
 
 
 class ModelViewSet(RestModelViewSet):
     """
     Inherited class from rest_framework.viewsets.ModelViewSet to override
     """
-    logger = logging.getLogger(__name__)
     model = None
     http_method_names = ["post"]
     permission_classes = [permissions.IsAuthenticated]
     authentication_classes = [JWTTokenUserAuthentication]
 
     if settings.DEBUG:
         authentication_classes.append(authentication.TokenAuthentication)
 
+    def perform_authentication(self, request: Request):
+        """
+        Override method to intercept InvalidToken exception.
+
+        Parameters
+        ----------
+        request: Request
+            Request object from HTTP
+
+        Returns
+        -------
+        None
+        """
+        try:
+            super().perform_authentication(request)
+        except InvalidToken as exc:
+            detail = []
+            if isinstance(exc.detail, dict) and "messages" in exc.detail and isinstance(exc.detail["messages"], list):
+                for message in exc.detail.get("messages", []):
+                    if "message" in message:
+                        detail.append(message.get("message"))
+            if len(detail) == 0:
+                detail.append(_("Invalid Token"))
+            raise APIException(detail=detail, code="invalid_token", status_code=exc.status_code) from exc
+        except Exception as exc:
+            raise APIException(str(exc), status_code=status.HTTP_500_INTERNAL_SERVER_ERROR) from exc
+
     @staticmethod
     def _get_pk(request) -> Any:
         """
         Get PK value from received request data dictionary.
 
         Parameters
         ----------
@@ -60,17 +88,17 @@
         """
         if request.data:
             if "pk" in request.data.keys():
                 pk_value = request.data.get("pk", None)
             elif "id" in request.data.keys():
                 pk_value = request.data.get("id", None)
             else:
-                raise APIException(ErrorMessages.DATA_REQUIRED, "get_pk", status.HTTP_406_NOT_ACCEPTABLE)
+                raise APIException(ErrorMessages.DATA_REQUIRED, "pk_required", status.HTTP_406_NOT_ACCEPTABLE)
         else:
-            raise APIException(ErrorMessages.DATA_REQUIRED, "get_pk", status.HTTP_406_NOT_ACCEPTABLE)
+            raise APIException(ErrorMessages.DATA_REQUIRED, "pk_required", status.HTTP_406_NOT_ACCEPTABLE)
         return pk_value
 
     def get_queryset(self, **kwargs) -> QuerySet:
         """
         Get a queryset from model from **kwargs parameters. If you want queryset pk based on, send "pk" key in kwargs.
         Parameters
         ----------
@@ -121,21 +149,21 @@
             if order_by is not None:
                 qs = qs.order_by(*order_by)
 
             serializer = self.get_serializer(instance=qs, many=True, context=context)
             data_return = serializer.data
             status_return = status.HTTP_200_OK if len(data_return) > 0 else status.HTTP_204_NO_CONTENT
             data_return = data_return
-        except APIException as exc:
-            logging.warning(str(exc))
-            raise APIException(detail=exc.detail, error=exc.detail.code, status_code=exc.status_code) from exc
+        except APIException:
+            raise
+        except CoreValidationError as exc:
+            raise APIException(detail=exc.messages, status_code=status.HTTP_406_NOT_ACCEPTABLE) from exc
         except Exception as exc:
-            logging.error(str(exc))
-            logging.debug(traceback.format_exc())
-            raise APIException() from exc
+            raise APIException(detail=str(exc), code="not_controlled_exception",
+                               status_code=status.HTTP_500_INTERNAL_SERVER_ERROR) from exc
         else:
             return Response(data=data_return, status=status_return)
 
     def list(self, request, *args, **kwargs):
         """
         Overridden class method to disallow access
 
@@ -145,15 +173,15 @@
         args :      Tuple of parameters
         kwargs :    Dictionary of key, value parameters
 
         Returns
         -------
         response: Response error with HTTP 405 status code
         """
-        raise APINotImplementedException()
+        raise NotImplementedException()
 
     def _retrieve(self, request, *args, **kwargs) -> Response:
         """
         REST service to get a record filtered by pk.
 
         Parameters
         ----------
@@ -167,22 +195,22 @@
         an exception is launched.
         """
         try:
             pk = self._get_pk(request)
             data_record = self.get_queryset(pk=pk).get()
             data_return = self.get_serializer(data_record).data
             status_return = status.HTTP_200_OK
-        except APIException as exc:
-            raise APIException(exc.detail, exc.detail.code, exc.status_code) from exc
+        except APIException:
+            raise
         except ObjectDoesNotExist as exc:
-            logging.warning(str(exc))
-            raise APIException(detail=ErrorMessages.NOT_FOUND, status_code=status.HTTP_404_NOT_FOUND) from exc
+            raise APIException(detail=ErrorMessages.NOT_FOUND, code="doest_not_exists",
+                               status_code=status.HTTP_404_NOT_FOUND) from exc
+        except CoreValidationError as exc:
+            raise APIException(detail=exc.messages, status_code=status.HTTP_406_NOT_ACCEPTABLE) from exc
         except Exception as exc:
-            logging.error(str(exc))
-            logging.debug(traceback.format_exc())
             raise APIException(error=str(exc), status_code=status.HTTP_500_INTERNAL_SERVER_ERROR) from exc
         else:
             return Response(status=status_return, data=data_return)
 
     def retrieve(self, request, *args, **kwargs):
         """
         Overridden class method to disallow access
@@ -193,15 +221,15 @@
         args :      Tuple of parameters
         kwargs :    Dictionary of key, value parameters
 
         Returns
         -------
         response: Response error with HTTP 405 status code
         """
-        raise APINotImplementedException()
+        raise NotImplementedException()
 
     def _create(self, request, *args, **kwargs) -> Response:
         """
         REST service for create a model record.
 
         Parameters
         ----------
@@ -225,23 +253,24 @@
                         data_return = self.get_serializer(created_record).data
                         status_return = status.HTTP_201_CREATED
                     else:
                         raise ValidationError(ErrorMessages.CREATE_ERROR, "create_object")
             else:
                 raise APIException(ErrorMessages.DATA_REQUIRED, "data_required")
         except DatabaseError as exc:
-            raise APIException(ErrorMessages.DATABASE_ERROR, str(exc)) from exc
+            raise APIException(detail=str(exc), code="database_error",
+                               status_code=status.HTTP_500_INTERNAL_SERVER_ERROR) from exc
         except ValidationError as exc:
-            raise APIException(error=exc.detail, status_code=status.HTTP_406_NOT_ACCEPTABLE) from exc
-        except APIException as exc:
-            raise APIException(exc.detail, exc.detail.code, exc.status_code) from exc
+            raise APIException(detail=exc.detail, status_code=status.HTTP_406_NOT_ACCEPTABLE) from exc
+        except CoreValidationError as exc:
+            raise APIException(detail=exc.messages, status_code=status.HTTP_406_NOT_ACCEPTABLE) from exc
+        except APIException:
+            raise
         except Exception as exc:
-            logging.error(str(exc))
-            logging.debug(traceback.format_exc())
-            raise APIException(error=str(exc), status_code=status.HTTP_500_INTERNAL_SERVER_ERROR)
+            raise APIException(detail=str(exc), status_code=status.HTTP_500_INTERNAL_SERVER_ERROR)
         else:
             return Response(status=status_return, data=data_return)
 
     def create(self, request, *args, **kwargs):
         """
         Overridden class method to disallow access
 
@@ -251,15 +280,15 @@
         args :      Tuple of parameters
         kwargs :    Dictionary of key, value parameters
 
         Returns
         -------
         response: Response error with HTTP 405 status code
         """
-        raise APINotImplementedException()
+        raise NotImplementedException()
 
     def _update(self, request, *args, **kwargs) -> Response:
         """
         REST service to update an existent record from model.
 
         Parameters
         ----------
@@ -285,21 +314,21 @@
             else:
                 raise APIException(ErrorMessages.NOT_FOUND, "update", status.HTTP_404_NOT_FOUND)
         except ObjectDoesNotExist as exc:
             raise APIException(ErrorMessages.NOT_FOUND, "update", status.HTTP_404_NOT_FOUND) from exc
         except DatabaseError as exc:
             raise APIException(ErrorMessages.UPDATE_ERROR, str(exc)) from exc
         except ValidationError as exc:
-            raise APIException(error=str(exc.detail), status_code=status.HTTP_406_NOT_ACCEPTABLE) from exc
-        except APIException as exc:
-            raise APIException(exc.detail, exc.detail.code, exc.status_code) from exc
+            raise APIException(detail=exc.detail, status_code=status.HTTP_406_NOT_ACCEPTABLE) from exc
+        except CoreValidationError as exc:
+            raise APIException(detail=exc.messages, status_code=status.HTTP_406_NOT_ACCEPTABLE) from exc
+        except APIException:
+            raise
         except Exception as exc:
-            logging.error(str(exc))
-            logging.debug(traceback.format_exc())
-            raise APIException(error=str(exc), status_code=status.HTTP_500_INTERNAL_SERVER_ERROR) from exc
+            raise APIException(detail=str(exc), status_code=status.HTTP_500_INTERNAL_SERVER_ERROR) from exc
         else:
             return Response(data=data_return, status=status_return)
 
     def update(self, request, *args, **kwargs):
         """
         Overridden class method to disallow access
 
@@ -309,15 +338,15 @@
         args :      Tuple of parameters
         kwargs :    Dictionary of key, value parameters
 
         Returns
         -------
         response: Response error with HTTP 405 status code
         """
-        raise APINotImplementedException()
+        raise NotImplementedException()
 
     def _destroy(self, request, *args, **kwargs) -> Response:
         """
         REST service to delete a record from model.
 
         Parameters
         ----------
@@ -332,24 +361,24 @@
         try:
             pk = self._get_pk(request)
             data_record = self.get_queryset(pk=pk)
             if data_record:
                 data_record.delete()
                 status_return = status.HTTP_200_OK
             else:
-                raise APIException(ErrorMessages.DELETE_ERROR, "delete", status.HTTP_404_NOT_FOUND)
+                raise APIException(ErrorMessages.NOT_FOUND, "delete", status.HTTP_404_NOT_FOUND)
         except DatabaseError as exc:
-            raise APIException(ErrorMessages.UPDATE_ERROR, str(exc)) from exc
+            raise APIException(ErrorMessages.DELETE_ERROR, str(exc)) from exc
         except ValidationError as exc:
             raise APIException(error=str(exc.detail), status_code=status.HTTP_406_NOT_ACCEPTABLE) from exc
-        except APIException as exc:
-            raise APIException(detail=exc.detail, code=exc.detail.code, status_code=exc.status_code) from exc
+        except CoreValidationError as exc:
+            raise APIException(detail=exc.messages, status_code=status.HTTP_406_NOT_ACCEPTABLE) from exc
+        except APIException:
+            raise
         except Exception as exc:
-            logging.error(str(exc))
-            logging.debug(traceback.format_exc())
             raise APIException(error=str(exc), status_code=status.HTTP_500_INTERNAL_SERVER_ERROR) from exc
         else:
             return Response(status=status_return)
 
     def destroy(self, request, *args, **kwargs):
         """
         Overridden class method to disallow access
@@ -361,8 +390,8 @@
         kwargs :    Dictionary of key, value parameters
 
         Returns
         -------
         response: Response error with HTTP 405 status code
         """
 
-        raise APINotImplementedException()
+        raise NotImplementedException()
```

### Comparing `zibanu-django-1.3.4/zibanu/django/rest_framework/viewsets/viewset.py` & `zibanu-django-1.3.5rc0/zibanu/django/rest_framework/viewsets/viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/template/apps.py` & `zibanu-django-1.3.5rc0/zibanu/django/template/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/template/context_processors/__init__.py` & `zibanu-django-1.3.5rc0/zibanu/django/template/context_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/template/context_processors/full_static_uri.py` & `zibanu-django-1.3.5rc0/zibanu/django/template/context_processors/full_static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/template/context_processors/site.py` & `zibanu-django-1.3.5rc0/zibanu/django/template/context_processors/site.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/template/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.3.5rc0/zibanu/django/template/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/template/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.3.5rc0/zibanu/django/template/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/template/templatetags/static_uri.py` & `zibanu-django-1.3.5rc0/zibanu/django/template/templatetags/static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/template/templatetags/string_concat.py` & `zibanu-django-1.3.5rc0/zibanu/django/template/templatetags/string_concat.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/template/templatetags/subtotal_dict.py` & `zibanu-django-1.3.5rc0/zibanu/django/template/templatetags/subtotal_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/template/templatetags/sum_dict.py` & `zibanu-django-1.3.5rc0/zibanu/django/template/templatetags/sum_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/urls.py` & `zibanu-django-1.3.5rc0/zibanu/django/urls.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/utils/__init__.py` & `zibanu-django-1.3.5rc0/zibanu/django/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Module Name:  __init__.py
 # Description:
 # ****************************************************************
 from .date_time import *
 from .error_messages import ErrorMessages
 from .mail import Email
 from .model_utils import *
+from .generic_utils import *
 from .request_utils import *
 from .user_utils import *
 from .receivers_utils import *
 
 __all__ = [
     "add_timezone",
     "change_timezone",
@@ -29,8 +30,10 @@
     "get_model_list",
     "get_model_fields",
     "get_receiver_id",
     "get_request_from_stack",
     "get_sender_name",
     "get_user",
     "get_user_object",
+    "import_class",
+    "object_to_list"
 ]
```

### Comparing `zibanu-django-1.3.4/zibanu/django/utils/date_time.py` & `zibanu-django-1.3.5rc0/zibanu/django/utils/date_time.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/utils/error_messages.py` & `zibanu-django-1.3.5rc0/zibanu/django/utils/error_messages.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/utils/mail.py` & `zibanu-django-1.3.5rc0/zibanu/django/utils/mail.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/utils/model_utils.py` & `zibanu-django-1.3.5rc0/zibanu/django/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/utils/receivers_utils.py` & `zibanu-django-1.3.5rc0/zibanu/django/utils/receivers_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/utils/request_utils.py` & `zibanu-django-1.3.5rc0/zibanu/django/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu/django/utils/user_utils.py` & `zibanu-django-1.3.5rc0/zibanu/django/utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.3.4/zibanu_django.egg-info/PKG-INFO` & `zibanu-django-1.3.5rc0/zibanu_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.3.4
+Version: 1.3.5rc0
 Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-1.3.4/zibanu_django.egg-info/SOURCES.txt` & `zibanu-django-1.3.5rc0/zibanu_django.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,20 @@
 zibanu/django/lib/classes/code_generator.py
 zibanu/django/lib/classes/extended_json_encoder.py
 zibanu/django/lib/classes/model_name.py
 zibanu/django/locale/es/LC_MESSAGES/django.mo
 zibanu/django/locale/es/LC_MESSAGES/django.po
 zibanu/django/rest_framework/__init__.py
 zibanu/django/rest_framework/decorators.py
+zibanu/django/rest_framework/utils.py
 zibanu/django/rest_framework/exceptions/__init__.py
 zibanu/django/rest_framework/exceptions/api_exception.py
-zibanu/django/rest_framework/exceptions/api_not_implemented_exception.py
 zibanu/django/rest_framework/exceptions/multiple_login_error.py
+zibanu/django/rest_framework/exceptions/not_implemented_exception.py
+zibanu/django/rest_framework/exceptions/permission_denied.py
 zibanu/django/rest_framework/fields/__init__.py
 zibanu/django/rest_framework/fields/current_user_default.py
 zibanu/django/rest_framework/fields/hybrid_image.py
 zibanu/django/rest_framework/permissions/__init__.py
 zibanu/django/rest_framework/permissions/is_owner_or_read_only.py
 zibanu/django/rest_framework/serializers/__init__.py
 zibanu/django/rest_framework/serializers/fields.py
@@ -53,14 +55,15 @@
 zibanu/django/template/templatetags/static_uri.py
 zibanu/django/template/templatetags/string_concat.py
 zibanu/django/template/templatetags/subtotal_dict.py
 zibanu/django/template/templatetags/sum_dict.py
 zibanu/django/utils/__init__.py
 zibanu/django/utils/date_time.py
 zibanu/django/utils/error_messages.py
+zibanu/django/utils/generic_utils.py
 zibanu/django/utils/mail.py
 zibanu/django/utils/model_utils.py
 zibanu/django/utils/receivers_utils.py
 zibanu/django/utils/request_utils.py
 zibanu/django/utils/user_utils.py
 zibanu_django.egg-info/PKG-INFO
 zibanu_django.egg-info/SOURCES.txt
```

