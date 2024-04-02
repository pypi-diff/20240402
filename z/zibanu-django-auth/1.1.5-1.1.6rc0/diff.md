# Comparing `tmp/zibanu-django-auth-1.1.5.tar.gz` & `tmp/zibanu-django-auth-1.1.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibanu-django-auth-1.1.5.tar", last modified: Thu Feb 22 11:33:19 2024, max compression
+gzip compressed data, was "zibanu-django-auth-1.1.6rc0.tar", last modified: Tue Apr  2 16:55:03 2024, max compression
```

## Comparing `zibanu-django-auth-1.1.5.tar` & `zibanu-django-auth-1.1.6rc0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.891873 zibanu-django-auth-1.1.5/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-auth-1.1.5/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      109 2023-06-19 16:17:43.000000 zibanu-django-auth-1.1.5/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)   151726 2024-02-22 11:33:19.891873 zibanu-django-auth-1.1.5/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)   110334 2023-11-28 01:08:56.000000 zibanu-django-auth-1.1.5/README.md
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      955 2024-02-22 11:31:33.000000 zibanu-django-auth-1.1.5/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2024-02-22 11:33:19.891873 zibanu-django-auth-1.1.5/setup.cfg
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.880873 zibanu-django-auth-1.1.5/zibanu/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.880873 zibanu-django-auth-1.1.5/zibanu/django/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.883873 zibanu-django-auth-1.1.5/zibanu/django/auth/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:20:31.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      785 2023-11-16 17:04:35.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/admin.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      832 2023-11-16 17:12:07.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/admin_views.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.883873 zibanu-django-auth-1.1.5/zibanu/django/auth/api/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      362 2024-02-08 19:20:16.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.884873 zibanu-django-auth-1.1.5/zibanu/django/auth/api/serializers/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1079 2024-02-13 15:13:24.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/api/serializers/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1017 2023-11-28 01:06:50.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/api/serializers/group.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      661 2023-07-26 21:21:14.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/api/serializers/permission.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1619 2024-02-15 01:04:03.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/api/serializers/profile.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)    10873 2024-02-08 19:20:16.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/api/serializers/token.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     6905 2024-02-15 02:11:29.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/api/serializers/user.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.885873 zibanu-django-auth-1.1.5/zibanu/django/auth/api/services/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      600 2023-08-26 15:54:46.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/api/services/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1494 2024-01-25 01:39:58.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/api/services/auth.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2003 2023-11-28 01:04:13.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/api/services/group.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1355 2023-11-09 21:37:15.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/api/services/permission.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2807 2024-02-01 21:22:22.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/api/services/profile.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)    19922 2024-02-14 00:51:53.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/api/services/user.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     3138 2024-02-08 03:00:23.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.886873 zibanu-django-auth-1.1.5/zibanu/django/auth/lib/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      313 2023-11-11 12:36:53.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/lib/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1244 2023-11-17 15:26:09.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/lib/backends.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      946 2023-11-11 16:08:36.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/lib/enums.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     4497 2023-12-12 01:25:00.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/lib/receivers.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      697 2023-12-12 01:10:06.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/lib/signals.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1450 2023-12-03 13:18:52.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/lib/utils.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.881873 zibanu-django-auth-1.1.5/zibanu/django/auth/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.881873 zibanu-django-auth-1.1.5/zibanu/django/auth/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.886873 zibanu-django-auth-1.1.5/zibanu/django/auth/locale/es/LC_MESSAGES/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     3949 2024-02-14 01:42:00.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 macercha  (1000) macercha  (1000)     6967 2024-02-14 01:43:43.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.888873 zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    24474 2023-04-11 22:39:55.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0001_initial.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)    23351 2023-07-05 13:34:24.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      443 2023-07-19 00:48:43.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0003_userprofile_multiple_login.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      447 2023-07-29 22:41:09.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0004_userprofile_secure_password.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      448 2023-08-12 00:23:05.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0005_alter_userprofile_avatar.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      877 2023-11-07 21:51:38.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0006_alter_userprofile_app_profile_and_more.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      978 2023-11-13 20:07:13.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0007_grouplevel.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      449 2023-11-16 21:21:58.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0008_alter_grouplevel_level.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      703 2023-11-17 18:54:33.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0009_user.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      365 2024-01-25 23:57:56.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0010_rename_app_profile_userprofile_app_settings.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:31:28.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     5079 2024-02-15 02:14:26.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.889873 zibanu-django-auth-1.1.5/zibanu/django/auth/templates/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      487 2023-05-23 16:11:28.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/templates/change_password.html
--rw-r--r--   0 macercha  (1000) macercha  (1000)      324 2023-05-22 17:32:26.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/templates/change_password.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)      615 2024-02-14 01:32:27.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/templates/new_user.html
--rw-r--r--   0 macercha  (1000) macercha  (1000)      395 2023-11-30 19:48:56.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/templates/new_user.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)      123 2023-05-13 16:44:16.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/templates/request-code.html
--rw-r--r--   0 macercha  (1000) macercha  (1000)        0 2023-05-13 16:41:48.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/templates/request-code.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)      559 2023-05-22 17:30:07.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/templates/request_password.html
--rw-r--r--   0 macercha  (1000) macercha  (1000)      346 2023-05-13 16:55:01.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/templates/request_password.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2175 2024-02-12 11:43:33.000000 zibanu-django-auth-1.1.5/zibanu/django/auth/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-02-22 11:33:19.890873 zibanu-django-auth-1.1.5/zibanu_django_auth.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)   151726 2024-02-22 11:33:19.000000 zibanu-django-auth-1.1.5/zibanu_django_auth.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2334 2024-02-22 11:33:19.000000 zibanu-django-auth-1.1.5/zibanu_django_auth.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2024-02-22 11:33:19.000000 zibanu-django-auth-1.1.5/zibanu_django_auth.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)      105 2024-02-22 11:33:19.000000 zibanu-django-auth-1.1.5/zibanu_django_auth.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2024-02-22 11:33:19.000000 zibanu-django-auth-1.1.5/zibanu_django_auth.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.648287 zibanu-django-auth-1.1.6rc0/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-auth-1.1.6rc0/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      109 2023-06-19 16:17:43.000000 zibanu-django-auth-1.1.6rc0/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)   151729 2024-04-02 16:55:03.647287 zibanu-django-auth-1.1.6rc0/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)   110334 2023-11-28 01:08:56.000000 zibanu-django-auth-1.1.6rc0/README.md
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      958 2024-04-02 16:54:37.000000 zibanu-django-auth-1.1.6rc0/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2024-04-02 16:55:03.648287 zibanu-django-auth-1.1.6rc0/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.635287 zibanu-django-auth-1.1.6rc0/zibanu/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.635287 zibanu-django-auth-1.1.6rc0/zibanu/django/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.638287 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      311 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      785 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/admin.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      832 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/admin_views.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.638287 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      362 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.639287 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/serializers/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1079 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/serializers/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1017 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/serializers/group.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      661 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/serializers/permission.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1619 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/serializers/profile.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    11627 2024-03-15 01:58:14.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/serializers/token.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     6654 2024-03-21 21:58:21.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/serializers/user.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.641287 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/services/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      600 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/services/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1513 2024-03-12 22:57:31.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/services/auth.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2003 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/services/group.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1355 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/services/permission.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2807 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/services/profile.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    20765 2024-03-21 21:51:14.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/services/user.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     3323 2024-03-21 22:58:30.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.642287 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/lib/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      313 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/lib/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1244 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/lib/backends.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      947 2024-03-13 14:24:21.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/lib/enums.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     4497 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/lib/receivers.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      697 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/lib/signals.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1450 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/lib/utils.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.636287 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.636287 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.642287 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/locale/es/LC_MESSAGES/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     3949 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     6967 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.644287 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    24474 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0001_initial.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    23351 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      443 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0003_userprofile_multiple_login.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      447 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0004_userprofile_secure_password.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      448 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0005_alter_userprofile_avatar.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      877 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0006_alter_userprofile_app_profile_and_more.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      978 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0007_grouplevel.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      449 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0008_alter_grouplevel_level.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      703 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0009_user.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      365 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0010_rename_app_profile_userprofile_app_settings.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      313 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     5079 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.645287 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/templates/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      487 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/templates/change_password.html
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      324 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/templates/change_password.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      615 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/templates/new_user.html
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      395 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/templates/new_user.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      123 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/templates/request-code.html
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        0 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/templates/request-code.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      559 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/templates/request_password.html
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      346 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/templates/request_password.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2175 2024-03-11 02:33:38.000000 zibanu-django-auth-1.1.6rc0/zibanu/django/auth/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-04-02 16:55:03.646287 zibanu-django-auth-1.1.6rc0/zibanu_django_auth.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)   151729 2024-04-02 16:55:03.000000 zibanu-django-auth-1.1.6rc0/zibanu_django_auth.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2334 2024-04-02 16:55:03.000000 zibanu-django-auth-1.1.6rc0/zibanu_django_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2024-04-02 16:55:03.000000 zibanu-django-auth-1.1.6rc0/zibanu_django_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      105 2024-04-02 16:55:03.000000 zibanu-django-auth-1.1.6rc0/zibanu_django_auth.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2024-04-02 16:55:03.000000 zibanu-django-auth-1.1.6rc0/zibanu_django_auth.egg-info/top_level.txt
```

### Comparing `zibanu-django-auth-1.1.5/LICENSE` & `zibanu-django-auth-1.1.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/PKG-INFO` & `zibanu-django-auth-1.1.6rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django-auth
-Version: 1.1.5
+Version: 1.1.6rc0
 Summary: Zibanu authentication library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-auth-1.1.5/README.md` & `zibanu-django-auth-1.1.6rc0/README.md`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/pyproject.toml` & `zibanu-django-auth-1.1.6rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zibanu-django-auth"
-version = "1.1.5"
+version = "1.1.6-rc"
 authors = [
     { name = "Mario Cerón", email = "mario.ceron@cqinversiones.co" }
 ]
 description = "Zibanu authentication library for django projects"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/admin.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/admin.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/admin_views.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/admin_views.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/api/serializers/__init__.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/api/serializers/group.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/serializers/group.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/api/serializers/permission.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/serializers/permission.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/api/serializers/profile.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/serializers/profile.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/api/serializers/token.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/serializers/token.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,49 +14,38 @@
 
 from django.conf import settings
 from django.contrib.auth import authenticate
 from django.contrib.auth import user_logged_in, user_login_failed
 from django.contrib.auth.models import update_last_login
 from django.core.cache import cache
 from django.core.exceptions import ObjectDoesNotExist
-from django.utils.module_loading import import_string
 from django.utils.translation import gettext_lazy as _
 from rest_framework.exceptions import AuthenticationFailed
+from rest_framework import status
 from rest_framework_simplejwt.serializers import TokenObtainSerializer, TokenRefreshSlidingSerializer
 from rest_framework_simplejwt.settings import api_settings
 from rest_framework_simplejwt.tokens import SlidingToken
-
-from zibanu.django.auth.api.serializers.user import UserTokenSerializer
 from zibanu.django.auth.lib.utils import get_cache_key
 from zibanu.django.auth.models import User
+from zibanu.django.rest_framework.exceptions import APIException
 from zibanu.django.rest_framework.exceptions import MultipleLoginError
-from zibanu.django.utils import get_http_origin, get_ip_address
+from zibanu.django.utils import get_http_origin, get_ip_address, import_class
 
 
 def get_user(token: SlidingToken):
     user_id = token.payload.get("user_id")
     user = None
     try:
         user = User.objects.get(pk=user_id)
     except ObjectDoesNotExist:
         user = None
     finally:
         return user
 
 
-def import_serializer(serializer_class: str = None):
-    try:
-        return import_string(serializer_class)
-    except ImportError:
-        msg = _("Could not load import serializer class: ") + serializer_class
-        logging.critical(msg)
-        logging.debug(traceback.format_exc())
-        raise ImportError(msg)
-
-
 class EmailTokenObtainSerializer(TokenObtainSerializer):
     """
     SimpleJWTToken serializer to get token with full user object payload for email authentication method.
     """
     username_field = User.EMAIL_FIELD
     serializer_class = None
     _serializer_class = settings.ZB_AUTH_USER_TOKEN_SERIALIZER
@@ -82,15 +71,15 @@
         self.user = None
 
     @classmethod
     def get_serializer_class(cls):
         if cls.serializer_class:
             return cls.serializer_class
         else:
-            return import_serializer(cls._serializer_class)
+            return import_class(cls._serializer_class)
 
     @property
     def close_sessions(self):
         """
         Property to view if request has close sessions flag active.
 
         Returns
@@ -127,18 +116,16 @@
                             cache.delete(cache_key)
                         else:
                             if cached_token is not None:
                                 raise MultipleLoginError(self.error_messages["multiple_login"])
                 else:
                     raise AuthenticationFailed(self.error_messages["invalid_profile"])
         except MultipleLoginError as exc:
-            logging.info(exc.detail, log_params)
             raise
         except AuthenticationFailed as exc:
-            logging.info(exc.detail, log_params)
             raise
         except Exception as exc:
             logging.critical(str(exc), log_params)
             logging.debug(traceback.format_exc(), log_params)
             raise
 
     def _save_cache(self, token: Any) -> str:
@@ -187,35 +174,43 @@
         ----------
         attrs: Request dictionary attributes
 
         Returns
         -------
         None: Empty data
         """
-        data = {}
-        user = User.objects.filter(email__iexact=attrs.get(self.username_field)).first()
-
-        if user is None:
-            user_login_failed.send(self.__class__, user=None, request=self.context.get("request"),
-                                   detail=attrs.get(self.username_field))
-            raise AuthenticationFailed(self.error_messages["no_active_account"], "no_active_account")
-        self._validate_sessions(user)
-        authenticate_kwargs = {
-            User.USERNAME_FIELD: user.get_username(),
-            "password": attrs.get("password")
-        }
-
-        self.user = authenticate(**authenticate_kwargs)
-        if not api_settings.USER_AUTHENTICATION_RULE(self.user):
-            raise AuthenticationFailed(
-                self.error_messages["no_active_account"],
-                "no_active_account",
-            )
+        try:
+            data = {}
+            user = User.objects.filter(email__iexact=attrs.get(self.username_field)).first()
 
-        return data
+            if user is None:
+                user_login_failed.send(self.__class__, user=None, request=self.context.get("request"),
+                                       detail=attrs.get(self.username_field))
+                raise AuthenticationFailed(self.error_messages["no_active_account"], "no_active_account")
+            self._validate_sessions(user)
+            authenticate_kwargs = {
+                User.USERNAME_FIELD: user.get_username(),
+                "password": attrs.get("password")
+            }
+
+            self.user = authenticate(**authenticate_kwargs)
+            if not api_settings.USER_AUTHENTICATION_RULE(self.user):
+                raise AuthenticationFailed(
+                    self.error_messages["no_active_account"],
+                    "no_active_account",
+                )
+        except MultipleLoginError as exc:
+            raise APIException(detail=exc.detail.get("errors"), code=exc.detail.get("code"),
+                               status_code=exc.status_code) from exc
+        except AuthenticationFailed as exc:
+            raise APIException(detail=exc.detail, code=exc.default_code, status_code=exc.status_code) from exc
+        except Exception as exc:
+            raise APIException(detail=str(exc), code="not_controlled_exception") from exc
+        else:
+            return data
 
 
 class EmailTokenObtainSlidingSerializer(EmailTokenObtainSerializer):
     """
     TokenSlidingSerializer child class of EmailTokenObtainSerializer
     """
     token_class = SlidingToken
@@ -260,15 +255,15 @@
         **kwargs: Dictionary with key/value of parameters.
         """
         super().__init__(*args, **kwargs)
         self.__request = self.context.get("request")
         self.error_messages["invalid_token"] = _("You're trying to refresh and invalid token.")
 
     def get_serializer_class(self):
-        return import_serializer(serializer_class=self._serializer_class)
+        return import_class(serializer_class=self._serializer_class)
 
     def validate(self, attrs):
         """
         Override method to implement a cached token validation and new token generation.
 
         Parameters
         ----------
@@ -278,30 +273,38 @@
         -------
         Dictionary with "token" key and new token value.
         """
         token = self.token_class(attrs["token"])
         token.check_exp(api_settings.SLIDING_TOKEN_REFRESH_EXP_CLAIM)
         token.blacklist()
 
-        # Load user from token and generate cache key
-        user = get_user(token)
-        if user is None:
-            raise AuthenticationFailed(self.error_messages["invalid_user"])
-        cache_key = get_cache_key(self.__request, user)
-
-        # Validate if multiple login flag is active
-        if not user.is_superuser and not user.profile.multiple_login:
-            cached_token = cache.get(cache_key, None)
-            if cached_token is None:
-                raise AuthenticationFailed(self.error_messages["invalid_token"])
-
-        # Generate new token
-        token = SlidingToken.for_user(user)
-        serializer = self.get_serializer_class()
-        user_serializer = serializer(instance=user)
-        token["user"] = user_serializer.data
-
-        # Set new token in cache if multiple login flag is active
-        if not user.is_superuser and not user.profile.multiple_login:
-            cache.set(cache_key, token, timeout=token.lifetime.total_seconds())
-
-        return {"token": str(token)}
+        try:
+            # Load user from token and generate cache key
+            user = get_user(token)
+            if user is None:
+                raise AuthenticationFailed(self.error_messages["invalid_user"], code="invalid_user")
+            cache_key = get_cache_key(self.__request, user)
+
+            # Validate if multiple login flag is active
+            if not user.is_superuser and not user.profile.multiple_login:
+                cached_token = cache.get(cache_key, None)
+                if cached_token is None:
+                    raise AuthenticationFailed(self.error_messages["invalid_token"], code="invalid_token")
+
+            # Generate new token
+            token = SlidingToken.for_user(user)
+            serializer = self.get_serializer_class()
+            user_serializer = serializer(instance=user)
+            token["user"] = user_serializer.data
+
+            # Set new token in cache if multiple login flag is active
+            if not user.is_superuser and not user.profile.multiple_login:
+                cache.set(cache_key, token, timeout=token.lifetime.total_seconds())
+        except ImportError as exc:
+            raise APIException(detail=exc.msg, code="import_error",
+                               status_code=status.HTTP_500_INTERNAL_SERVER_ERROR) from exc
+        except AuthenticationFailed as exc:
+            raise APIException(detail=exc.detail, code=exc.default_code, status_code=exc.status_code) from exc
+        except Exception as exc:
+            raise APIException(detail=str(exc), code="not_controlled_exception") from exc
+        else:
+            return {"token": str(token)}
```

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/api/serializers/user.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/serializers/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 class UserSerializer(UserListSerializer):
     """
     Serializer class for Django user entity, including user profile, permissions and groups (groups).
     """
     profile = ProfileSerializer(required=True, read_only=False)
-    groups = serializers.SerializerMethodField(default=[])
+    roles = serializers.SerializerMethodField(default=[])
     permissions = serializers.SerializerMethodField(default=[])
 
     def get_permissions(self, instance) -> list:
         """
         Method to get permission list from User object.
 
         Parameters
@@ -71,43 +71,38 @@
         """
         permissions = []
         if self.context.get("load_permissions", settings.ZB_AUTH_INCLUDE_PERMISSIONS):
             for permission in instance.user_permissions.all():
                 permissions.append(permission.name)
         return permissions
 
-    def get_groups(self, instance) -> list:
+    def get_roles(self, instance) -> list:
         """
         Method to get groups list from User object
 
         Parameters
         ----------
         instance: User object instance
 
         Returns
         -------
         groups: Group list
 
         """
         roles = []
-        if self.context.get("load_roles", settings.ZB_AUTH_INCLUDE_GROUPS):
-            for group in instance.groups.all():
+        if self.context.get("load_roles", settings.ZB_AUTH_INCLUDE_ROLES):
+            for group in instance.roles.all():
                 roles.append(
                     {
                         "id": group.id,
                         "name": group.name
                     }
                 )
         return roles
 
-    def save_profile(self, instance: UserProfile, data: dict):
-        profile_serializer = ProfileExtendedSerializer(instance=instance, data=data)
-        if profile_serializer.is_valid(raise_exception=True):
-            profile_serializer.save()
-
     def validate(self, attrs: dict) -> dict:
         """
         Method to validate if email is already registered in the user model
         Parameters
         ----------
         attrs : dictionary with user attributes to be validated
 
@@ -186,20 +181,22 @@
         """
         UserSerializer metaclass
         """
         model = User
         fields = ("email", "full_name", "last_login", "is_staff", "is_superuser", "is_active", "profile", "groups",
                   "first_name", "last_name", "permissions", "username", "password")
 
+
 class UserExtendedSerializer(UserSerializer):
     """
     Class to be used to update full user information
     """
     profile = ProfileExtendedSerializer(required=True, read_only=False)
 
+
 class UserTokenSerializer(UserSerializer):
     """
     Class inherited from UserSerializer to only use in the TokenSerializer for the authentication process.
     """
 
     class Meta:
         model = User
```

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/api/services/__init__.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/api/services/auth.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/services/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         user = get_user(request.user)
 
         if isinstance(request.user, TokenUser) and hasattr(request.user, "token"):
             token = request.user.token
             token.blacklist()
 
         try:
-            if not user.profile.multiple_login:
+            if not user.is_superuser and hasattr(user, "profile"):
                 cache_key = get_cache_key(request, user)
                 cache.delete(cache_key)
         except Exception as exc:
             logging.error(str(exc))
             logging.debug(traceback.format_exc())
             raise APIException() from exc
         finally:
```

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/api/services/group.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/services/group.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/api/services/permission.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/services/permission.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/api/services/profile.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/services/profile.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/api/services/user.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/api/services/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,49 +43,46 @@
     Set of REST Services for django User model
     """
     model = User
     serializer_class = serializers.UserListSerializer
     request_password_template = settings.ZB_AUTH_REQUEST_PASSWORD_TEMPLATE
     change_password_template = settings.ZB_AUTH_CHANGE_PASSWORD_TEMPLATE
     new_user_template = settings.ZB_AUTH_NEW_USER_TEMPLATE
+    extended_serializer_class = serializers.UserExtendedSerializer
+    roles_key = settings.ZB_AUTH_ROLES_KEY
+    permissions_key = settings.ZB_AUTH_PERMISSIONS_KEY
 
-    def __send_mail(self, subject: str, to: list, template: str, context: dict) -> None:
+    def _send_mail(self, subject: str, to: list, template: str, context: dict) -> None:
         """
-        Private method to send mail
+        Protected method to send mail
 
         Parameters
         ----------
-        subject
-        to
-        template
-        context
+        subject: str
+            Subject for email
+        to: list[str...]
+            List of email targets
+        template: str
+            Name of the email body template
+        context: dic[str, Any]
+            Context data required for email template
 
         Returns
         -------
-
+        None
         """
         try:
             # TODO: Reformat to use class directly
             email = Email(subject=subject, to=to, context=context)
             email.set_text_template(template=template)
             email.set_html_template(template=template)
             email.send()
         except smtplib.SMTPException:
             pass
 
-    def get_serializer(self, *args, **kwargs):
-        if self.action == "retrieve":
-            return serializers.UserSerializer(*args)
-        elif self.action == "get_avatar":
-            return serializers.ProfileExtendedSerializer(*args, **kwargs)
-        elif self.action == "get_profile":
-            return serializers.UserProfileSerializer(*args, **kwargs)
-        else:
-            return super().get_serializer()
-
     def get_permissions(self):
         """
         Override method to get permissions for allow on_request_password action.
 
         Returns
         -------
         response: Response object with HTTP status (200 if success) and list of permissions dataset.
@@ -122,15 +119,65 @@
             data = [x for x in response.data if x["level"] >= user.level]
         else:
             data = response.data
         return Response(data=data, status=response.status_code)
 
     @method_decorator(permission_required("auth.view_user"))
     def retrieve(self, request, *args, **kwargs):
-        return super()._retrieve(request, *args, **kwargs)
+        self.serializer_class = serializers.UserSerializer
+        response = super()._retrieve(request, *args, **kwargs)
+        # Drop password field from data
+        response.data.pop("password", None)
+        return response
+
+    def _create_user(self, request) -> User:
+        """
+        Create a new user from request data and return user object created
+
+        Parameters
+        ----------
+        request : Request
+            HTTP request object
+
+        Returns
+        -------
+        User:
+            User object created if success
+        """
+        try:
+            roles_data = request.data.pop(self.roles_key, [])
+            permissions_data = request.data.pop(self.permissions_key, [])
+            # Set default values and automatic options
+            if settings.ZB_AUTH_AUTO_PASSWORD:
+                code_generator = CodeGenerator("create_user", is_safe=True, code_length=10)
+                request.data["password"] = code_generator.get_alpha_numeric_code()
+            if settings.ZB_AUTH_AUTO_USERNAME:
+                request.data["username"] = uuid.uuid4().hex
+            if "profile" not in request.data:
+                request.data["profile"] = {}
+            # Create an atomic transaction
+            with transaction.atomic():
+                serializer = self.extended_serializer_class(data=request.data)
+                if serializer.is_valid(raise_exception=True):
+                    created_user = serializer.create(validated_data=serializer.validated_data)
+                    if created_user is not None:
+                        if len(roles_data) > 0:
+                            # If user has groups to add
+                            created_user.groups.set(roles_data)
+                        if len(permissions_data) > 0:
+                            # If user has permissions to add
+                            created_user.user_permissions.set(permissions_data)
+                    else:
+                        raise ValidationError(_("Error creating user"))
+        except ValidationError:
+            raise
+        except Exception:
+            raise
+        else:
+            return created_user
 
     @method_decorator(permission_required(["auth.add_user", "zb_auth.add_userprofile"]))
     def create(self, request, *args, **kwargs) -> Response:
         """
         REST service to create user with its profile.
 
         Parameters
@@ -141,58 +188,82 @@
 
         Returns
         -------
         response: Response object with HTTP status (200 if success).
         """
         try:
             if request.data is not None and len(request.data) > 0:
-                roles_data = request.data.pop("groups", [])
-                permissions_data = request.data.pop("permissions", [])
-                # Set default values and automatic options
-                if settings.ZB_AUTH_AUTO_PASSWORD:
-                    code_generator = CodeGenerator("create_user", is_safe=True, code_length=10)
-                    request.data["password"] = code_generator.get_alpha_numeric_code()
-                if settings.ZB_AUTH_AUTO_USERNAME:
-                    request.data["username"] = uuid.uuid4().hex
-                if "profile" not in request.data:
-                    request.data["profile"] = {}
-                # Create an atomic transaction
-                with transaction.atomic():
-                    serializer = serializers.UserExtendedSerializer(data=request.data)
-                    if serializer.is_valid(raise_exception=True):
-                        created_user = serializer.create(validated_data=serializer.validated_data)
-                        if created_user is not None:
-                            if len(roles_data) > 0:
-                                # If user has groups to add
-                                created_user.groups.set(roles_data)
-                            if len(permissions_data) > 0:
-                                # If user has permissions to add
-                                created_user.user_permissions.set(permissions_data)
-                            data_return = self.get_serializer(created_user).data
-                            on_user_created.send(sender=self, user=data_return, request=request)
-                            context = {
-                                "user": created_user,
-                                "new_password": request.data.get("password")
-                            }
-                            self.__send_mail(subject=_("New User"), to=[created_user.email],
-                                             template=self.new_user_template, context=context)
+                created_user = self._create_user(request)
+                data_return = self.get_serializer(created_user).data
+                on_user_created.send(sender=self, user=data_return, request=request)
+                context = {
+                    "user": created_user,
+                    "new_password": request.data.get("password")
+                }
+                self._send_mail(subject=_("New User"), to=[created_user.email],
+                                template=self.new_user_template, context=context)
             else:
                 raise ValidationError(ErrorMessages.DATA_REQUEST_NOT_FOUND)
         except ValidationError as exc:
-            logging.warning(str(exc))
             raise APIException(detail=exc.detail, http_status=status.HTTP_406_NOT_ACCEPTABLE) from exc
         except CoreValidationError as exc:
-            logging.warning(str(exc))
             raise APIException(detail=exc.message, code=exc.code, http_status=status.HTTP_406_NOT_ACCEPTABLE) from exc
         except Exception as exc:
-            logging.critical(str(exc))
-            logging.debug(traceback.format_exc())
             raise APIException(detail=str(exc)) from exc
         else:
-            return Response(status=status.HTTP_201_CREATED)
+            return Response(status=status.HTTP_201_CREATED, data=data_return)
+
+    def _update_user(self, request) -> User:
+        """
+        Update one record of the user entity
+
+        Parameters
+        ----------
+        request : Request
+            HTTP request object received
+
+        Returns
+        -------
+        User:
+            User object updated with the request
+        """
+        user = get_user(request.user)
+        try:
+            if "email" in request.data or "id" in request.data:
+                # Add profile key if it does not exist
+                if "profile" not in request.data:
+                    request.data["profile"] = dict()
+                # Remove password key
+                request.data.pop("password", None)
+                groups_data = request.data.pop(self.roles_key, None)
+                permissions_data = request.data.pop(self.permissions_key, None)
+                with transaction.atomic():
+                    if user.id != request.data.get("id", None) or user.email != request.data.get("email", None):
+                        # If authenticated user is different from user to change.
+                        if "id" in request.data:
+                            user = self.model.objects.get(pk=request.data.pop("id"))
+                        else:
+                            user = self.model.objects.get(email__exact=request.data.pop("email"))
+                    # Save user groups and permissions
+                    if groups_data is not None:
+                        user.groups.set(groups_data)
+                    if permissions_data is not None:
+                        user.user_permissions.set(permissions_data)
+                    # Save user data
+                    serializer = serializers.UserExtendedSerializer(instance=user, data=request.data, partial=True)
+                    if serializer.is_valid(raise_exception=True):
+                        user_return = serializer.update(serializer.instance, serializer.validated_data)
+            else:
+                raise ValidationError(_("'email' or 'id' not found in request data"))
+        except self.model.DoesNotExist:
+            raise ValidationError(_("User does not exist."))
+        except Exception:
+            raise
+        else:
+            return user_return
 
     @method_decorator(permission_required(["auth.change_user", "zb_auth.change_userprofile"]))
     def update(self, request, *args, **kwargs) -> Response:
         """
         REST service to update user, including profile, groups and permissions.
 
         Parameters
@@ -202,59 +273,26 @@
         **kwargs: Dictionary of parameters
 
         Returns
         -------
         response: Response object with HTTP status (200 if success).
         """
         try:
-            user = get_user(request.user)
-            if "email" in request.data or "id" in request.data:
-                try:
-                    # Add profile key if it does not exist
-                    if "profile" not in request.data:
-                        request.data["profile"] = dict()
-                    # Remove password key
-                    request.data.pop("password", None)
-                    groups_data = request.data.pop("groups", None)
-                    permissions_data = request.data.pop("permissions", None)
-                    with transaction.atomic():
-                        if user.id != request.data.get("id", None) or user.email != request.data.get("email", None):
-                            # If authenticated user is different from user to change.
-                            if "id" in request.data:
-                                user = self.model.objects.get(pk=request.data.pop("id"))
-                            else:
-                                user = self.model.objects.get(email__exact=request.data.pop("email"))
-                        # Save user groups and permissions
-                        if groups_data is not None:
-                            user.groups.set(groups_data)
-                        if permissions_data is not None:
-                            user.user_permissions.set(permissions_data)
-                        # Save user data
-                        serializer = serializers.UserExtendedSerializer(instance=user, data=request.data, partial=True)
-                        if serializer.is_valid(raise_exception=True):
-                            serializer.update(serializer.instance, serializer.validated_data)
-                            user = serializer.data
-                            on_user_updated.send(sender=self, user=user, request=request)
-                except self.model.DoesNotExist:
-                    raise ValidationError(_("User does not exists."))
-            else:
-                logging.error("'email' or 'id' not found in request data")
-                raise ValidationError(ErrorMessages.DATA_REQUEST_NOT_FOUND)
+            user = self._update_user(request)
+            serializer = serializers.UserExtendedSerializer(instance=user)
+            user_data = serializer.data
+            on_user_updated.send(sender=self, user=user_data, request=request)
         except ValidationError as exc:
-            logging.warning(str(exc))
             raise APIException(detail=exc.detail, http_status=status.HTTP_406_NOT_ACCEPTABLE) from exc
         except ObjectDoesNotExist as exc:
-            logging.warning(str(exc))
             raise APIException(ErrorMessages.NOT_FOUND, http_status=status.HTTP_404_NOT_FOUND) from exc
         except Exception as exc:
-            logging.critical(str(exc))
-            logging.debug(traceback.format_exc())
-            raise APIException() from exc
+            raise APIException(detail=str(exc), status_code=status.HTTP_500_INTERNAL_SERVER_ERROR) from exc
         else:
-            return Response(status=status.HTTP_200_OK)
+            return Response(status=status.HTTP_200_OK, data=user_data)
 
     @method_decorator(permission_required(["auth.delete_user", "zb_auth.delete_userprofile"]))
     def destroy(self, request, *args, **kwargs) -> Response:
         """
         REST service to delete one user object.
 
         Parameters
@@ -314,14 +352,15 @@
         kwargs : dict: dict of parameters or arguments
 
         Returns
         -------
         Original representation of field.
         """
         try:
+            self.serializer_class = serializers.ProfileExtendedSerializer
             user = get_user(request.user)
             data_return = None
             status_return = status.HTTP_200_OK
             if hasattr(user, "profile"):
                 serializer = self.get_serializer(instance=user.profile)
                 data_return = serializer.data.get("avatar", None)
                 if not data_return:
@@ -331,14 +370,15 @@
             logging.debug(traceback.format_exc())
             raise APIException() from exc
         else:
             return Response(data=data_return, status=status_return)
 
     def get_profile(self, request, *args, **kwargs):
         try:
+            self.serializer_class = serializers.UserProfileSerializer
             user = get_user(request.user)
             data_return = None
             status_return = status.HTTP_200_OK
             if hasattr(user, "profile"):
                 serializer = self.get_serializer(instance=user)
                 data_return = serializer.data
                 if not data_return:
@@ -372,16 +412,16 @@
                 if user.check_password(request.data.get("old_password")):
                     user.set_password(request.data.get("new_password"))
                     user.save()
                     context = {
                         "user": user
                     }
                     if apps.is_installed("zibanu.django"):
-                        self.__send_mail(subject=_("Password change"), to=[user.email],
-                                         template=self.change_password_template, context=context)
+                        self._send_mail(subject=_("Password change"), to=[user.email],
+                                        template=self.change_password_template, context=context)
                     on_change_password.send(sender=self.__class__, user=user, request=request)
                 else:
                     raise ValidationError(_("Old password does not match."))
             else:
                 logging.error("'old_password'/'new_password' not found in request")
                 raise ValidationError(_("Old/New password are required."))
         except ValidationError as exc:
@@ -425,16 +465,16 @@
                     user.set_password(new_password)
                     user.save()
                     context = {
                         "user": user,
                         "new_password": new_password
                     }
                     if apps.is_installed("zibanu.django"):
-                        self.__send_mail(subject=_("Request password."), to=[user.email],
-                                         template=self.request_password_template, context=context)
+                        self._send_mail(subject=_("Request password."), to=[user.email],
+                                        template=self.request_password_template, context=context)
                     on_request_password.send(sender=self.__class__, user=user, request=request)
                 else:
                     raise ValidationError(_("Email is not registered or user is not active."))
             else:
                 logging.error("'email' not found in request data")
                 raise ValidationError(ErrorMessages.DATA_REQUEST_NOT_FOUND)
         except ValidationError as exc:
```

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/apps.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/apps.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,35 +28,37 @@
 
         Returns
         -------
         None
 
         Settings
         -------
-        ZB_AUTH_INCLUDE_GROUPS: If True, includes the set of groups to which the user belongs, False ignores them.
+        ZB_AUTH_INCLUDE_ROLES: If True, includes the set of groups to which the user belongs, False ignores them.
             Default: True
         ZB_AUTH_INCLUDE_PERMISSIONS: If True, includes the set of permissions the user has, False ignores them.
             Default: False
         ZB_AUTH_CHANGE_PASSWORD_TEMPLATE: Template used to generate password change confirmation email.
             Default: "on_change_password"
         ZB_AUTH_REQUEST_PASSWORD_TEMPLATE: Template used to generate request password email.
             Default: "on_request_password"
         ZB_AUTH_ALLOW_MULTIPLE_LOGIN: If True, allows a user to have multiple access from the same type of application,
         False only allows one access.
             Default is FALSE
         """
         # Import signals
         # Set default settings for Simple JWT Module
-        settings.ZB_AUTH_INCLUDE_GROUPS = getattr(settings, "ZB_AUTH_INCLUDE_GROUPS", True)
+        settings.ZB_AUTH_INCLUDE_ROLES = getattr(settings, "ZB_AUTH_INCLUDE_ROLES", True)
         settings.ZB_AUTH_INCLUDE_PERMISSIONS = getattr(settings, "ZB_AUTH_INCLUDE_PERMISSIONS", False)
         settings.ZB_AUTH_AUTO_PASSWORD = getattr(settings, "ZB_AUTH_AUTO_PASSWORD", True)
         settings.ZB_AUTH_AUTO_USERNAME = getattr(settings, "ZB_AUTH_AUTO_USERNAME", True)
         settings.ZB_AUTH_CHANGE_PASSWORD_TEMPLATE = getattr(settings, "ZB_AUTH_CHANGE_PASSWORD_TEMPLATE",
                                                             "change_password")
         settings.ZB_AUTH_REQUEST_PASSWORD_TEMPLATE = getattr(settings, "ZB_AUTH_REQUEST_PASSWORD_TEMPLATE",
                                                              "request_password")
         settings.ZB_AUTH_NEW_USER_TEMPLATE = getattr(settings, "ZB_AUTH_NEW_USER_TEMPLATE", "new_user")
         settings.ZB_AUTH_ALLOW_MULTIPLE_LOGIN = getattr(settings, "ZB_AUTH_ALLOW_MULTIPLE_LOGIN", False)
         settings.ZB_AUTH_AVATAR_BASE64 = getattr(settings, "ZB_AUTH_AVATAR_FORMAT", True)
         settings.ZB_AUTH_AVATAR_SIZE = getattr(settings, "ZB_AUTH_AVATAR_SIZE", 0)
         settings.ZB_AUTH_USER_TOKEN_SERIALIZER = getattr(settings, "ZB_AUTH_USER_TOKEN_SERIALIZER",
                                                          "zibanu.django.auth.api.serializers.UserTokenSerializer")
+        settings.ZB_AUTH_ROLES_KEY = getattr(settings, "ZB_AUTH_ROLES_KEY", "roles")
+        settings.ZB_AUTH_PERMISSIONS_KEY = getattr(settings, "ZB_AUTH_PERMISSIONS_KEY", "permissions")
```

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/lib/backends.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/lib/backends.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/lib/enums.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/lib/enums.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
     Allowed levels for django groups
     """
     SUPER_USER = 0, _("Superuser")
     STAFF = 1, _("Staff")
     SUPER_ADMIN = 2, _("Super Administrator")
     ADMIN = 3, _("Administrator")
     SUPERVISOR = 4, _("Supervisor")
-    OPERATOR = 5, _("Operator")
+    OPERATOR = 5, _("Operator")
```

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/lib/receivers.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/lib/receivers.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/lib/signals.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/lib/signals.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/lib/utils.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/lib/utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/locale/es/LC_MESSAGES/django.po` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0001_initial.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0006_alter_userprofile_app_profile_and_more.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0006_alter_userprofile_app_profile_and_more.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0007_grouplevel.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0007_grouplevel.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/migrations/0009_user.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/migrations/0009_user.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/models.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/models.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/templates/new_user.html` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/templates/new_user.html`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/templates/request_password.html` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/templates/request_password.html`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu/django/auth/urls.py` & `zibanu-django-auth-1.1.6rc0/zibanu/django/auth/urls.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.1.5/zibanu_django_auth.egg-info/PKG-INFO` & `zibanu-django-auth-1.1.6rc0/zibanu_django_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django-auth
-Version: 1.1.5
+Version: 1.1.6rc0
 Summary: Zibanu authentication library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-auth-1.1.5/zibanu_django_auth.egg-info/SOURCES.txt` & `zibanu-django-auth-1.1.6rc0/zibanu_django_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

