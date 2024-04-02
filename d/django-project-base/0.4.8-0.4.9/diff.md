# Comparing `tmp/django-project-base-0.4.8.tar.gz` & `tmp/django-project-base-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-project-base-0.4.8.tar", last modified: Thu Nov 16 12:13:05 2023, max compression
+gzip compressed data, was "django-project-base-0.4.9.tar", last modified: Fri Nov 17 14:52:23 2023, max compression
```

## Comparing `django-project-base-0.4.8.tar` & `django-project-base-0.4.9.tar`

### file list

```diff
@@ -1,219 +1,219 @@
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.887628 django-project-base-0.4.8/
--rw-rw-r--   0 jure      (1000) jure      (1000)      116 2021-10-28 06:34:59.000000 django-project-base-0.4.8/MANIFEST.in
--rw-rw-r--   0 jure      (1000) jure      (1000)     1585 2023-11-16 12:13:05.887628 django-project-base-0.4.8/PKG-INFO
--rw-rw-r--   0 jure      (1000) jure      (1000)     1006 2023-10-16 12:26:59.000000 django-project-base-0.4.8/README.md
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.787626 django-project-base-0.4.8/django_project_base/
--rw-rw-r--   0 jure      (1000) jure      (1000)      307 2023-11-16 12:12:53.000000 django-project-base-0.4.8/django_project_base/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.787626 django-project-base-0.4.8/django_project_base/account/
--rw-rw-r--   0 jure      (1000) jure      (1000)      161 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/account/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      420 2021-12-10 13:37:27.000000 django-project-base-0.4.8/django_project_base/account/apps.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      182 2023-07-18 11:29:41.000000 django-project-base-0.4.8/django_project_base/account/constants.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.787626 django-project-base-0.4.8/django_project_base/account/management/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.4.8/django_project_base/account/management/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.787626 django-project-base-0.4.8/django_project_base/account/management/commands/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.4.8/django_project_base/account/management/commands/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1832 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/account/management/commands/allauth_to_social_core.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      663 2023-06-20 12:42:50.000000 django-project-base-0.4.8/django_project_base/account/management/commands/delete_users.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3601 2023-09-11 08:57:16.000000 django-project-base-0.4.8/django_project_base/account/middleware.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.791626 django-project-base-0.4.8/django_project_base/account/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-08-05 09:26:32.000000 django-project-base-0.4.8/django_project_base/account/rest/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    13141 2023-10-26 13:44:43.000000 django-project-base-0.4.8/django_project_base/account/rest/account.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     4541 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/account/rest/impersonate.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     6838 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/account/rest/invite.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5682 2023-10-13 11:01:30.000000 django-project-base-0.4.8/django_project_base/account/rest/login.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    26708 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/account/rest/profile.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5932 2023-11-16 12:12:19.000000 django-project-base-0.4.8/django_project_base/account/rest/profile_merge.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    11354 2023-10-13 11:01:30.000000 django-project-base-0.4.8/django_project_base/account/rest/project_profiles.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     6741 2023-10-13 11:01:30.000000 django-project-base-0.4.8/django_project_base/account/rest/project_profiles_utils.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     6528 2023-08-02 10:50:11.000000 django-project-base-0.4.8/django_project_base/account/rest/reset_password.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2293 2023-10-13 11:01:30.000000 django-project-base-0.4.8/django_project_base/account/router.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.791626 django-project-base-0.4.8/django_project_base/account/service/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:41.000000 django-project-base-0.4.8/django_project_base/account/service/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5837 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/account/service/merge_users_service.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1392 2023-10-13 11:01:30.000000 django-project-base-0.4.8/django_project_base/account/service/register_user_service.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2432 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/account/service/reset_password_email_service.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      216 2021-06-29 12:16:02.000000 django-project-base-0.4.8/django_project_base/account/settings.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.791626 django-project-base-0.4.8/django_project_base/account/social_auth/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.4.8/django_project_base/account/social_auth/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1580 2023-03-29 13:29:13.000000 django-project-base-0.4.8/django_project_base/account/social_auth/providers.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2244 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/account/social_auth/settings.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      226 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/account/urls.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      355 2023-07-18 11:29:41.000000 django-project-base-0.4.8/django_project_base/apps.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.791626 django-project-base-0.4.8/django_project_base/auth/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:44.000000 django-project-base-0.4.8/django_project_base/auth/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       77 2023-07-18 12:51:25.000000 django-project-base-0.4.8/django_project_base/auth/admin.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      160 2023-07-18 11:29:44.000000 django-project-base-0.4.8/django_project_base/auth/apps.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.791626 django-project-base-0.4.8/django_project_base/auth/migrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:44.000000 django-project-base-0.4.8/django_project_base/auth/migrations/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      737 2023-08-18 11:58:37.000000 django-project-base-0.4.8/django_project_base/auth/models.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       74 2023-07-18 12:51:25.000000 django-project-base-0.4.8/django_project_base/auth/tests.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       77 2023-07-18 12:51:25.000000 django-project-base-0.4.8/django_project_base/auth/views.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.791626 django-project-base-0.4.8/django_project_base/aws/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-26 14:22:46.000000 django-project-base-0.4.8/django_project_base/aws/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1726 2023-10-17 13:39:09.000000 django-project-base-0.4.8/django_project_base/aws/ses.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.791626 django-project-base-0.4.8/django_project_base/base/
--rw-rw-r--   0 jure      (1000) jure      (1000)       42 2021-06-29 12:16:02.000000 django-project-base-0.4.8/django_project_base/base/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1814 2023-06-16 10:27:37.000000 django-project-base-0.4.8/django_project_base/base/auth_backends.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     9024 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/base/event.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      304 2023-10-13 11:01:30.000000 django-project-base-0.4.8/django_project_base/base/exceptions.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1794 2023-11-16 12:12:19.000000 django-project-base-0.4.8/django_project_base/base/fields.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1730 2023-09-29 09:40:18.000000 django-project-base-0.4.8/django_project_base/base/middleware.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    12876 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/base/models.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      481 2023-09-04 09:23:53.000000 django-project-base-0.4.8/django_project_base/base/permissions.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1990 2023-07-18 11:29:41.000000 django-project-base-0.4.8/django_project_base/base/queryset_with_cache.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      494 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/base/signals.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.795626 django-project-base-0.4.8/django_project_base/celery/
--rw-rw-r--   0 jure      (1000) jure      (1000)       85 2023-08-01 07:02:58.000000 django-project-base-0.4.8/django_project_base/celery/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      187 2023-08-01 07:02:58.000000 django-project-base-0.4.8/django_project_base/celery/apps.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.795626 django-project-base-0.4.8/django_project_base/celery/background_tasks/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.4.8/django_project_base/celery/background_tasks/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1619 2023-08-30 15:18:55.000000 django-project-base-0.4.8/django_project_base/celery/background_tasks/notification_tasks.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2097 2023-08-28 11:05:17.000000 django-project-base-0.4.8/django_project_base/celery/celery.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      327 2023-08-30 15:18:55.000000 django-project-base-0.4.8/django_project_base/celery/settings.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      447 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/constants.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1335 2023-08-01 07:02:58.000000 django-project-base-0.4.8/django_project_base/country_holidays.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.795626 django-project-base-0.4.8/django_project_base/licensing/
--rw-rw-r--   0 jure      (1000) jure      (1000)       98 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/licensing/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      190 2023-08-20 09:37:15.000000 django-project-base-0.4.8/django_project_base/licensing/apps.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     4327 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/licensing/logic.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.795626 django-project-base-0.4.8/django_project_base/licensing/migrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)     1767 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/licensing/migrations/0001_initial.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2065 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      550 2023-09-04 09:23:53.000000 django-project-base-0.4.8/django_project_base/licensing/migrations/0005_auto_20230901_0613.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-20 09:37:15.000000 django-project-base-0.4.8/django_project_base/licensing/migrations/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      940 2023-08-30 15:18:55.000000 django-project-base-0.4.8/django_project_base/licensing/models.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.795626 django-project-base-0.4.8/django_project_base/licensing/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-30 15:18:55.000000 django-project-base-0.4.8/django_project_base/licensing/rest/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      944 2023-10-13 11:01:30.000000 django-project-base-0.4.8/django_project_base/licensing/rest/rest.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      243 2023-08-30 15:18:55.000000 django-project-base-0.4.8/django_project_base/licensing/rest/router.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      175 2023-08-30 15:18:55.000000 django-project-base-0.4.8/django_project_base/licensing/urls.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.783626 django-project-base-0.4.8/django_project_base/locale/
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.783626 django-project-base-0.4.8/django_project_base/locale/en/
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.795626 django-project-base-0.4.8/django_project_base/locale/en/LC_MESSAGES/
--rw-rw-r--   0 jure      (1000) jure      (1000)      380 2023-08-04 14:40:02.000000 django-project-base-0.4.8/django_project_base/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 jure      (1000) jure      (1000)     7468 2023-08-11 11:07:25.000000 django-project-base-0.4.8/django_project_base/locale/en/LC_MESSAGES/django.po
--rw-rw-r--   0 jure      (1000) jure      (1000)       84 2023-08-04 14:40:02.000000 django-project-base-0.4.8/django_project_base/locale/en/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 jure      (1000) jure      (1000)     4562 2023-08-04 14:39:40.000000 django-project-base-0.4.8/django_project_base/locale/en/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.783626 django-project-base-0.4.8/django_project_base/locale/sl/
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.795626 django-project-base-0.4.8/django_project_base/locale/sl/LC_MESSAGES/
--rw-rw-r--   0 jure      (1000) jure      (1000)     4385 2023-08-04 14:40:02.000000 django-project-base-0.4.8/django_project_base/locale/sl/LC_MESSAGES/django.mo
--rw-rw-r--   0 jure      (1000) jure      (1000)     8756 2023-08-11 11:07:25.000000 django-project-base-0.4.8/django_project_base/locale/sl/LC_MESSAGES/django.po
--rw-rw-r--   0 jure      (1000) jure      (1000)     3731 2023-08-04 14:40:02.000000 django-project-base-0.4.8/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 jure      (1000) jure      (1000)     6150 2023-08-04 14:39:32.000000 django-project-base-0.4.8/django_project_base/locale/sl/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.795626 django-project-base-0.4.8/django_project_base/management/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-10-13 11:01:30.000000 django-project-base-0.4.8/django_project_base/management/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.795626 django-project-base-0.4.8/django_project_base/management/commands/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-10-13 11:01:30.000000 django-project-base-0.4.8/django_project_base/management/commands/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1790 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/management/commands/confirm_setting.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1657 2023-10-17 07:56:43.000000 django-project-base-0.4.8/django_project_base/management/commands/list_pending_settings.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-20 09:46:16.000000 django-project-base-0.4.8/django_project_base/models.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.799626 django-project-base-0.4.8/django_project_base/notifications/
--rw-rw-r--   0 jure      (1000) jure      (1000)      162 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/notifications/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      449 2021-09-30 06:36:03.000000 django-project-base-0.4.8/django_project_base/notifications/apps.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.799626 django-project-base-0.4.8/django_project_base/notifications/base/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.8/django_project_base/notifications/base/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.799626 django-project-base-0.4.8/django_project_base/notifications/base/channels/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.8/django_project_base/notifications/base/channels/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    10772 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/base/channels/channel.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.799626 django-project-base-0.4.8/django_project_base/notifications/base/channels/integrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.8/django_project_base/notifications/base/channels/integrations/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3550 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/base/channels/integrations/aws_ses.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3070 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2815 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/base/channels/integrations/nexmo_sms.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2914 2023-10-13 11:01:30.000000 django-project-base-0.4.8/django_project_base/notifications/base/channels/integrations/provider_integration.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    10461 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/base/channels/integrations/t2.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1759 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/base/channels/mail_channel.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1034 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/base/channels/sms_channel.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.8/django_project_base/notifications/base/channels/websocket_channel.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1613 2023-08-01 07:02:58.000000 django-project-base-0.4.8/django_project_base/notifications/base/duplicate_notification_mixin.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1417 2023-09-20 12:31:19.000000 django-project-base-0.4.8/django_project_base/notifications/base/enums.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    11382 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/base/notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1687 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/base/phone_number_parser.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1407 2023-08-02 06:59:12.000000 django-project-base-0.4.8/django_project_base/notifications/base/queable_notification_mixin.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5936 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/base/send_notification_mixin.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       59 2023-08-01 07:02:58.000000 django-project-base-0.4.8/django_project_base/notifications/constants.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5799 2023-10-17 07:56:43.000000 django-project-base-0.4.8/django_project_base/notifications/email_notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      974 2023-08-18 11:58:37.000000 django-project-base-0.4.8/django_project_base/notifications/maintenance_notification.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.799626 django-project-base-0.4.8/django_project_base/notifications/management/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-11 08:57:16.000000 django-project-base-0.4.8/django_project_base/notifications/management/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.799626 django-project-base-0.4.8/django_project_base/notifications/management/commands/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-11 08:57:16.000000 django-project-base-0.4.8/django_project_base/notifications/management/commands/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      889 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/notifications/management/commands/resend_notification.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.803627 django-project-base-0.4.8/django_project_base/notifications/migrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)     6404 2023-08-30 15:18:55.000000 django-project-base-0.4.8/django_project_base/notifications/migrations/0001_initial.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1086 2023-09-11 08:57:16.000000 django-project-base-0.4.8/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      413 2023-09-04 09:23:53.000000 django-project-base-0.4.8/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      393 2023-09-04 09:23:53.000000 django-project-base-0.4.8/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options_and_more.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      412 2023-09-11 08:57:16.000000 django-project-base-0.4.8/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2533 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1501 2023-09-20 12:31:19.000000 django-project-base-0.4.8/django_project_base/notifications/migrations/0005_merge_20230906_1213.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1458 2023-10-13 11:01:30.000000 django-project-base-0.4.8/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1056 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/migrations/0007_auto_20231026_0555.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      448 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/migrations/0008_deliveryreport_auxiliary_notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1410 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/migrations/0009_auto_20231108_0658.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.8/django_project_base/notifications/migrations/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     9480 2023-11-16 12:12:19.000000 django-project-base-0.4.8/django_project_base/notifications/models.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1200 2023-08-01 07:02:58.000000 django-project-base-0.4.8/django_project_base/notifications/notification_queryset.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.803627 django-project-base-0.4.8/django_project_base/notifications/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.8/django_project_base/notifications/rest/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3172 2023-10-13 11:01:30.000000 django-project-base-0.4.8/django_project_base/notifications/rest/delivery_report.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     9089 2023-08-28 11:05:17.000000 django-project-base-0.4.8/django_project_base/notifications/rest/maintenance_notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    21913 2023-11-16 12:12:19.000000 django-project-base-0.4.8/django_project_base/notifications/rest/notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      988 2023-09-11 08:57:16.000000 django-project-base-0.4.8/django_project_base/notifications/rest/router.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      943 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/notifications/settings.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.803627 django-project-base-0.4.8/django_project_base/notifications/templates/
--rw-rw-r--   0 jure      (1000) jure      (1000)      368 2023-09-11 08:57:16.000000 django-project-base-0.4.8/django_project_base/notifications/templates/account_created.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     4339 2023-09-21 07:55:00.000000 django-project-base-0.4.8/django_project_base/notifications/templates/notification.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     2614 2023-09-21 07:55:00.000000 django-project-base-0.4.8/django_project_base/notifications/templates/notification_login.html
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.803627 django-project-base-0.4.8/django_project_base/notifications/tests/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.4.8/django_project_base/notifications/tests/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.807627 django-project-base-0.4.8/django_project_base/notifications/tests/api/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.4.8/django_project_base/notifications/tests/api/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2427 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/tests/api/test_create_mail.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2196 2023-08-28 11:05:17.000000 django-project-base-0.4.8/django_project_base/notifications/tests/api/test_list_mail.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      789 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/tests/api/test_remainig_license.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1485 2023-08-28 11:05:17.000000 django-project-base-0.4.8/django_project_base/notifications/tests/api/test_retrieve_mail.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3332 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/tests/notifications_transaction_test_case.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.883628 django-project-base-0.4.8/django_project_base/notifications/tests/unit/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.4.8/django_project_base/notifications/tests/unit/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2866 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/tests/unit/test_is_mail_sent.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      543 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      177 2023-08-02 05:31:11.000000 django-project-base-0.4.8/django_project_base/notifications/utils.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.883628 django-project-base-0.4.8/django_project_base/permissions/
--rw-rw-r--   0 jure      (1000) jure      (1000)      450 2023-08-01 07:02:58.000000 django-project-base-0.4.8/django_project_base/permissions/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.883628 django-project-base-0.4.8/django_project_base/profiling/
--rw-rw-r--   0 jure      (1000) jure      (1000)       77 2021-06-29 12:16:02.000000 django-project-base-0.4.8/django_project_base/profiling/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     9788 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/profiling/middleware.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1040 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/profiling/performance_base_command.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3480 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/profiling/views.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.883628 django-project-base-0.4.8/django_project_base/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-03-10 04:17:51.000000 django-project-base-0.4.8/django_project_base/rest/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    18069 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/rest/project.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3999 2023-09-12 11:16:30.000000 django-project-base-0.4.8/django_project_base/rest/project_role.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     4094 2023-09-11 08:57:16.000000 django-project-base-0.4.8/django_project_base/router.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3881 2023-11-14 06:52:55.000000 django-project-base-0.4.8/django_project_base/settings.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1673 2023-09-20 12:31:19.000000 django-project-base-0.4.8/django_project_base/settings_parser.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.783626 django-project-base-0.4.8/django_project_base/static/
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.887628 django-project-base-0.4.8/django_project_base/static/browser-update/
--rw-rw-r--   0 jure      (1000) jure      (1000)      421 2023-07-14 12:32:29.000000 django-project-base-0.4.8/django_project_base/static/browser-update/browser-update.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     9484 2023-07-14 12:32:29.000000 django-project-base-0.4.8/django_project_base/static/browser-update/update.min.js
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.783626 django-project-base-0.4.8/django_project_base/templates/
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.887628 django-project-base-0.4.8/django_project_base/templates/app-debug/
--rw-rw-r--   0 jure      (1000) jure      (1000)     2169 2021-05-19 11:48:39.000000 django-project-base-0.4.8/django_project_base/templates/app-debug/main.html
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.887628 django-project-base-0.4.8/django_project_base/templates/email/
--rw-rw-r--   0 jure      (1000) jure      (1000)      169 2023-06-20 12:45:01.000000 django-project-base-0.4.8/django_project_base/templates/email/base.html
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.887628 django-project-base-0.4.8/django_project_base/templatetags/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2022-01-12 07:10:33.000000 django-project-base-0.4.8/django_project_base/templatetags/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      200 2022-01-12 07:10:33.000000 django-project-base-0.4.8/django_project_base/templatetags/dpb_tags.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      907 2023-10-19 07:08:41.000000 django-project-base-0.4.8/django_project_base/urls.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5636 2023-10-13 11:01:30.000000 django-project-base-0.4.8/django_project_base/utils.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      912 2023-04-14 14:01:54.000000 django-project-base-0.4.8/django_project_base/views.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-16 12:13:05.787626 django-project-base-0.4.8/django_project_base.egg-info/
--rw-rw-r--   0 jure      (1000) jure      (1000)     1585 2023-11-16 12:13:05.000000 django-project-base-0.4.8/django_project_base.egg-info/PKG-INFO
--rw-rw-r--   0 jure      (1000) jure      (1000)     8905 2023-11-16 12:13:05.000000 django-project-base-0.4.8/django_project_base.egg-info/SOURCES.txt
--rw-rw-r--   0 jure      (1000) jure      (1000)        1 2023-11-16 12:13:05.000000 django-project-base-0.4.8/django_project_base.egg-info/dependency_links.txt
--rw-rw-r--   0 jure      (1000) jure      (1000)      297 2023-11-16 12:13:05.000000 django-project-base-0.4.8/django_project_base.egg-info/requires.txt
--rw-rw-r--   0 jure      (1000) jure      (1000)       20 2023-11-16 12:13:05.000000 django-project-base-0.4.8/django_project_base.egg-info/top_level.txt
--rw-rw-r--   0 jure      (1000) jure      (1000)      302 2023-11-14 06:52:55.000000 django-project-base-0.4.8/requirements.txt
--rw-rw-r--   0 jure      (1000) jure      (1000)       38 2023-11-16 12:13:05.887628 django-project-base-0.4.8/setup.cfg
--rwxrwxr-x   0 jure      (1000) jure      (1000)     3354 2023-10-17 07:56:43.000000 django-project-base-0.4.8/setup.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.973523 django-project-base-0.4.9/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      116 2021-10-28 06:34:59.000000 django-project-base-0.4.9/MANIFEST.in
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1585 2023-11-17 14:52:23.973523 django-project-base-0.4.9/PKG-INFO
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1006 2023-10-16 12:26:59.000000 django-project-base-0.4.9/README.md
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.949523 django-project-base-0.4.9/django_project_base/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      307 2023-11-17 14:52:10.000000 django-project-base-0.4.9/django_project_base/__init__.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.949523 django-project-base-0.4.9/django_project_base/account/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      161 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/account/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      420 2021-12-10 13:37:27.000000 django-project-base-0.4.9/django_project_base/account/apps.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      182 2023-07-18 11:29:41.000000 django-project-base-0.4.9/django_project_base/account/constants.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.949523 django-project-base-0.4.9/django_project_base/account/management/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.4.9/django_project_base/account/management/__init__.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.953523 django-project-base-0.4.9/django_project_base/account/management/commands/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.4.9/django_project_base/account/management/commands/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1832 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/account/management/commands/allauth_to_social_core.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      663 2023-06-20 12:42:50.000000 django-project-base-0.4.9/django_project_base/account/management/commands/delete_users.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3601 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/account/middleware.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.953523 django-project-base-0.4.9/django_project_base/account/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-08-05 09:26:32.000000 django-project-base-0.4.9/django_project_base/account/rest/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    13141 2023-10-26 13:44:43.000000 django-project-base-0.4.9/django_project_base/account/rest/account.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4541 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/account/rest/impersonate.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6838 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/account/rest/invite.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     5682 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/account/rest/login.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    26708 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/account/rest/profile.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     5932 2023-11-16 12:12:19.000000 django-project-base-0.4.9/django_project_base/account/rest/profile_merge.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    11354 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/account/rest/project_profiles.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6741 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/account/rest/project_profiles_utils.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6528 2023-08-02 10:50:11.000000 django-project-base-0.4.9/django_project_base/account/rest/reset_password.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2293 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/account/router.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.953523 django-project-base-0.4.9/django_project_base/account/service/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:41.000000 django-project-base-0.4.9/django_project_base/account/service/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     5837 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/account/service/merge_users_service.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1392 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/account/service/register_user_service.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2432 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/account/service/reset_password_email_service.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      216 2021-06-29 12:16:02.000000 django-project-base-0.4.9/django_project_base/account/settings.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.953523 django-project-base-0.4.9/django_project_base/account/social_auth/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.4.9/django_project_base/account/social_auth/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1580 2023-03-29 13:29:13.000000 django-project-base-0.4.9/django_project_base/account/social_auth/providers.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2244 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/account/social_auth/settings.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      226 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/account/urls.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      355 2023-07-18 11:29:41.000000 django-project-base-0.4.9/django_project_base/apps.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.953523 django-project-base-0.4.9/django_project_base/auth/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:44.000000 django-project-base-0.4.9/django_project_base/auth/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)       77 2023-07-18 12:51:25.000000 django-project-base-0.4.9/django_project_base/auth/admin.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      160 2023-07-18 11:29:44.000000 django-project-base-0.4.9/django_project_base/auth/apps.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.953523 django-project-base-0.4.9/django_project_base/auth/migrations/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:44.000000 django-project-base-0.4.9/django_project_base/auth/migrations/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      737 2023-08-18 11:58:37.000000 django-project-base-0.4.9/django_project_base/auth/models.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)       74 2023-07-18 12:51:25.000000 django-project-base-0.4.9/django_project_base/auth/tests.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)       77 2023-07-18 12:51:25.000000 django-project-base-0.4.9/django_project_base/auth/views.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.957523 django-project-base-0.4.9/django_project_base/aws/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-26 14:22:46.000000 django-project-base-0.4.9/django_project_base/aws/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1726 2023-10-17 13:39:09.000000 django-project-base-0.4.9/django_project_base/aws/ses.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.957523 django-project-base-0.4.9/django_project_base/base/
+-rw-rw-r--   0 jure      (1000) jure      (1000)       42 2021-06-29 12:16:02.000000 django-project-base-0.4.9/django_project_base/base/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1814 2023-06-16 10:27:37.000000 django-project-base-0.4.9/django_project_base/base/auth_backends.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     9024 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/base/event.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      304 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/base/exceptions.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1794 2023-11-16 12:12:19.000000 django-project-base-0.4.9/django_project_base/base/fields.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1730 2023-09-29 09:40:18.000000 django-project-base-0.4.9/django_project_base/base/middleware.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    12876 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/base/models.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      481 2023-09-04 09:23:53.000000 django-project-base-0.4.9/django_project_base/base/permissions.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1990 2023-07-18 11:29:41.000000 django-project-base-0.4.9/django_project_base/base/queryset_with_cache.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      494 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/base/signals.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.957523 django-project-base-0.4.9/django_project_base/celery/
+-rw-rw-r--   0 jure      (1000) jure      (1000)       85 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/celery/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      187 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/celery/apps.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.957523 django-project-base-0.4.9/django_project_base/celery/background_tasks/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/celery/background_tasks/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1619 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/celery/background_tasks/notification_tasks.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2097 2023-08-28 11:05:17.000000 django-project-base-0.4.9/django_project_base/celery/celery.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      327 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/celery/settings.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      447 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/constants.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1335 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/country_holidays.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.957523 django-project-base-0.4.9/django_project_base/licensing/
+-rw-rw-r--   0 jure      (1000) jure      (1000)       98 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/licensing/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      190 2023-08-20 09:37:15.000000 django-project-base-0.4.9/django_project_base/licensing/apps.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4327 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/licensing/logic.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.957523 django-project-base-0.4.9/django_project_base/licensing/migrations/
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1767 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/licensing/migrations/0001_initial.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2065 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      550 2023-09-04 09:23:53.000000 django-project-base-0.4.9/django_project_base/licensing/migrations/0005_auto_20230901_0613.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-20 09:37:15.000000 django-project-base-0.4.9/django_project_base/licensing/migrations/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      940 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/licensing/models.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.961523 django-project-base-0.4.9/django_project_base/licensing/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/licensing/rest/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      944 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/licensing/rest/rest.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      243 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/licensing/rest/router.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      175 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/licensing/urls.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.945523 django-project-base-0.4.9/django_project_base/locale/
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.945523 django-project-base-0.4.9/django_project_base/locale/en/
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.961523 django-project-base-0.4.9/django_project_base/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      380 2023-08-04 14:40:02.000000 django-project-base-0.4.9/django_project_base/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jure      (1000) jure      (1000)     7468 2023-08-11 11:07:25.000000 django-project-base-0.4.9/django_project_base/locale/en/LC_MESSAGES/django.po
+-rw-rw-r--   0 jure      (1000) jure      (1000)       84 2023-08-04 14:40:02.000000 django-project-base-0.4.9/django_project_base/locale/en/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4562 2023-08-04 14:39:40.000000 django-project-base-0.4.9/django_project_base/locale/en/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.945523 django-project-base-0.4.9/django_project_base/locale/sl/
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.961523 django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4385 2023-08-04 14:40:02.000000 django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jure      (1000) jure      (1000)     8756 2023-08-11 11:07:25.000000 django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/django.po
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3731 2023-08-04 14:40:02.000000 django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6150 2023-08-04 14:39:32.000000 django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.961523 django-project-base-0.4.9/django_project_base/management/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/management/__init__.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.961523 django-project-base-0.4.9/django_project_base/management/commands/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/management/commands/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1790 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/management/commands/confirm_setting.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1657 2023-10-17 07:56:43.000000 django-project-base-0.4.9/django_project_base/management/commands/list_pending_settings.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-20 09:46:16.000000 django-project-base-0.4.9/django_project_base/models.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.961523 django-project-base-0.4.9/django_project_base/notifications/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      162 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/notifications/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      449 2021-09-30 06:36:03.000000 django-project-base-0.4.9/django_project_base/notifications/apps.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.965523 django-project-base-0.4.9/django_project_base/notifications/base/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/notifications/base/__init__.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.965523 django-project-base-0.4.9/django_project_base/notifications/base/channels/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    10772 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/channel.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.965523 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3550 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/aws_ses.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3070 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2815 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/nexmo_sms.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2914 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/provider_integration.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    10461 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/t2.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1759 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/mail_channel.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1034 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/sms_channel.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/websocket_channel.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1613 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/notifications/base/duplicate_notification_mixin.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1417 2023-09-20 12:31:19.000000 django-project-base-0.4.9/django_project_base/notifications/base/enums.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    11382 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/notification.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1687 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/phone_number_parser.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1407 2023-08-02 06:59:12.000000 django-project-base-0.4.9/django_project_base/notifications/base/queable_notification_mixin.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     5936 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/send_notification_mixin.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)       59 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/notifications/constants.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     5799 2023-10-17 07:56:43.000000 django-project-base-0.4.9/django_project_base/notifications/email_notification.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      974 2023-08-18 11:58:37.000000 django-project-base-0.4.9/django_project_base/notifications/maintenance_notification.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.965523 django-project-base-0.4.9/django_project_base/notifications/management/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/notifications/management/__init__.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.965523 django-project-base-0.4.9/django_project_base/notifications/management/commands/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/notifications/management/commands/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      889 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/notifications/management/commands/resend_notification.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/notifications/migrations/
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6404 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0001_initial.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1086 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      413 2023-09-04 09:23:53.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      393 2023-09-04 09:23:53.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options_and_more.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      412 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2533 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1501 2023-09-20 12:31:19.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0005_merge_20230906_1213.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1458 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1056 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0007_auto_20231026_0555.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      448 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0008_deliveryreport_auxiliary_notification.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1410 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0009_auto_20231108_0658.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     9480 2023-11-16 12:12:19.000000 django-project-base-0.4.9/django_project_base/notifications/models.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1200 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/notifications/notification_queryset.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/notifications/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/notifications/rest/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3172 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/notifications/rest/delivery_report.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     9089 2023-08-28 11:05:17.000000 django-project-base-0.4.9/django_project_base/notifications/rest/maintenance_notification.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    21913 2023-11-16 12:12:19.000000 django-project-base-0.4.9/django_project_base/notifications/rest/notification.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      988 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/notifications/rest/router.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      943 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/notifications/settings.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/notifications/templates/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      368 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/notifications/templates/account_created.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4339 2023-09-21 07:55:00.000000 django-project-base-0.4.9/django_project_base/notifications/templates/notification.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2614 2023-09-21 07:55:00.000000 django-project-base-0.4.9/django_project_base/notifications/templates/notification_login.html
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/notifications/tests/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/notifications/tests/__init__.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/notifications/tests/api/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/notifications/tests/api/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2427 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/tests/api/test_create_mail.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2196 2023-08-28 11:05:17.000000 django-project-base-0.4.9/django_project_base/notifications/tests/api/test_list_mail.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      789 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/tests/api/test_remainig_license.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1485 2023-08-28 11:05:17.000000 django-project-base-0.4.9/django_project_base/notifications/tests/api/test_retrieve_mail.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3332 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/tests/notifications_transaction_test_case.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/notifications/tests/unit/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/notifications/tests/unit/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2866 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/tests/unit/test_is_mail_sent.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      543 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      177 2023-08-02 05:31:11.000000 django-project-base-0.4.9/django_project_base/notifications/utils.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/permissions/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      450 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/permissions/__init__.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/profiling/
+-rw-rw-r--   0 jure      (1000) jure      (1000)       77 2021-06-29 12:16:02.000000 django-project-base-0.4.9/django_project_base/profiling/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     9788 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/profiling/middleware.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1040 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/profiling/performance_base_command.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3480 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/profiling/views.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.973523 django-project-base-0.4.9/django_project_base/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-03-10 04:17:51.000000 django-project-base-0.4.9/django_project_base/rest/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    18069 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/rest/project.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3999 2023-09-12 11:16:30.000000 django-project-base-0.4.9/django_project_base/rest/project_role.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4094 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/router.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3881 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/settings.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1677 2023-11-17 14:51:19.000000 django-project-base-0.4.9/django_project_base/settings_parser.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.945523 django-project-base-0.4.9/django_project_base/static/
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.973523 django-project-base-0.4.9/django_project_base/static/browser-update/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      421 2023-07-14 12:32:29.000000 django-project-base-0.4.9/django_project_base/static/browser-update/browser-update.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     9484 2023-07-14 12:32:29.000000 django-project-base-0.4.9/django_project_base/static/browser-update/update.min.js
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.945523 django-project-base-0.4.9/django_project_base/templates/
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.973523 django-project-base-0.4.9/django_project_base/templates/app-debug/
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2169 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/templates/app-debug/main.html
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.973523 django-project-base-0.4.9/django_project_base/templates/email/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      169 2023-06-20 12:45:01.000000 django-project-base-0.4.9/django_project_base/templates/email/base.html
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.973523 django-project-base-0.4.9/django_project_base/templatetags/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2022-01-12 07:10:33.000000 django-project-base-0.4.9/django_project_base/templatetags/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      200 2022-01-12 07:10:33.000000 django-project-base-0.4.9/django_project_base/templatetags/dpb_tags.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      907 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/urls.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     5636 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/utils.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      912 2023-04-14 14:01:54.000000 django-project-base-0.4.9/django_project_base/views.py
+drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.949523 django-project-base-0.4.9/django_project_base.egg-info/
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1585 2023-11-17 14:52:23.000000 django-project-base-0.4.9/django_project_base.egg-info/PKG-INFO
+-rw-rw-r--   0 jure      (1000) jure      (1000)     8905 2023-11-17 14:52:23.000000 django-project-base-0.4.9/django_project_base.egg-info/SOURCES.txt
+-rw-rw-r--   0 jure      (1000) jure      (1000)        1 2023-11-17 14:52:23.000000 django-project-base-0.4.9/django_project_base.egg-info/dependency_links.txt
+-rw-rw-r--   0 jure      (1000) jure      (1000)      297 2023-11-17 14:52:23.000000 django-project-base-0.4.9/django_project_base.egg-info/requires.txt
+-rw-rw-r--   0 jure      (1000) jure      (1000)       20 2023-11-17 14:52:23.000000 django-project-base-0.4.9/django_project_base.egg-info/top_level.txt
+-rw-rw-r--   0 jure      (1000) jure      (1000)      302 2023-11-14 06:52:55.000000 django-project-base-0.4.9/requirements.txt
+-rw-rw-r--   0 jure      (1000) jure      (1000)       38 2023-11-17 14:52:23.973523 django-project-base-0.4.9/setup.cfg
+-rwxrwxr-x   0 jure      (1000) jure      (1000)     3354 2023-10-17 07:56:43.000000 django-project-base-0.4.9/setup.py
```

### Comparing `django-project-base-0.4.8/PKG-INFO` & `django-project-base-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-project-base
-Version: 0.4.8
+Version: 0.4.9
 Summary: Everything revolves around it: users, roles, permissions, tags, etc.
 Home-page: https://github.com/velis74/django-project-base
 Author: Jure Erznožnik
 Author-email: jure@velis.si
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-project-base-0.4.8/README.md` & `django-project-base-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/management/commands/allauth_to_social_core.py` & `django-project-base-0.4.9/django_project_base/account/management/commands/allauth_to_social_core.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/management/commands/delete_users.py` & `django-project-base-0.4.9/django_project_base/account/management/commands/delete_users.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/middleware.py` & `django-project-base-0.4.9/django_project_base/account/middleware.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/rest/account.py` & `django-project-base-0.4.9/django_project_base/account/rest/account.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/rest/impersonate.py` & `django-project-base-0.4.9/django_project_base/account/rest/impersonate.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/rest/invite.py` & `django-project-base-0.4.9/django_project_base/account/rest/invite.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/rest/login.py` & `django-project-base-0.4.9/django_project_base/account/rest/login.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/rest/profile.py` & `django-project-base-0.4.9/django_project_base/account/rest/profile.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/rest/profile_merge.py` & `django-project-base-0.4.9/django_project_base/account/rest/profile_merge.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/rest/project_profiles.py` & `django-project-base-0.4.9/django_project_base/account/rest/project_profiles.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/rest/project_profiles_utils.py` & `django-project-base-0.4.9/django_project_base/account/rest/project_profiles_utils.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/rest/reset_password.py` & `django-project-base-0.4.9/django_project_base/account/rest/reset_password.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/router.py` & `django-project-base-0.4.9/django_project_base/account/router.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/service/merge_users_service.py` & `django-project-base-0.4.9/django_project_base/account/service/merge_users_service.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/service/register_user_service.py` & `django-project-base-0.4.9/django_project_base/account/service/register_user_service.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/service/reset_password_email_service.py` & `django-project-base-0.4.9/django_project_base/account/service/reset_password_email_service.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/social_auth/providers.py` & `django-project-base-0.4.9/django_project_base/account/social_auth/providers.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/account/social_auth/settings.py` & `django-project-base-0.4.9/django_project_base/account/social_auth/settings.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/auth/models.py` & `django-project-base-0.4.9/django_project_base/auth/models.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/aws/ses.py` & `django-project-base-0.4.9/django_project_base/aws/ses.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/base/auth_backends.py` & `django-project-base-0.4.9/django_project_base/base/auth_backends.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/base/event.py` & `django-project-base-0.4.9/django_project_base/base/event.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/base/fields.py` & `django-project-base-0.4.9/django_project_base/base/fields.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/base/middleware.py` & `django-project-base-0.4.9/django_project_base/base/middleware.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/base/models.py` & `django-project-base-0.4.9/django_project_base/base/models.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/base/queryset_with_cache.py` & `django-project-base-0.4.9/django_project_base/base/queryset_with_cache.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/celery/background_tasks/notification_tasks.py` & `django-project-base-0.4.9/django_project_base/celery/background_tasks/notification_tasks.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/celery/celery.py` & `django-project-base-0.4.9/django_project_base/celery/celery.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/country_holidays.py` & `django-project-base-0.4.9/django_project_base/country_holidays.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/licensing/logic.py` & `django-project-base-0.4.9/django_project_base/licensing/logic.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/licensing/migrations/0001_initial.py` & `django-project-base-0.4.9/django_project_base/licensing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py` & `django-project-base-0.4.9/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/licensing/migrations/0005_auto_20230901_0613.py` & `django-project-base-0.4.9/django_project_base/licensing/migrations/0005_auto_20230901_0613.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/licensing/models.py` & `django-project-base-0.4.9/django_project_base/licensing/models.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/licensing/rest/rest.py` & `django-project-base-0.4.9/django_project_base/licensing/rest/rest.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/locale/en/LC_MESSAGES/django.po` & `django-project-base-0.4.9/django_project_base/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/locale/en/LC_MESSAGES/djangojs.po` & `django-project-base-0.4.9/django_project_base/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/locale/sl/LC_MESSAGES/django.mo` & `django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/locale/sl/LC_MESSAGES/django.po` & `django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo` & `django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/locale/sl/LC_MESSAGES/djangojs.po` & `django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/management/commands/confirm_setting.py` & `django-project-base-0.4.9/django_project_base/management/commands/confirm_setting.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/management/commands/list_pending_settings.py` & `django-project-base-0.4.9/django_project_base/management/commands/list_pending_settings.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/channels/channel.py` & `django-project-base-0.4.9/django_project_base/notifications/base/channels/channel.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/channels/integrations/aws_ses.py` & `django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/aws_ses.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py` & `django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/channels/integrations/nexmo_sms.py` & `django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/nexmo_sms.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/channels/integrations/provider_integration.py` & `django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/provider_integration.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/channels/integrations/t2.py` & `django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/t2.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/channels/mail_channel.py` & `django-project-base-0.4.9/django_project_base/notifications/base/channels/mail_channel.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/channels/sms_channel.py` & `django-project-base-0.4.9/django_project_base/notifications/base/channels/sms_channel.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/duplicate_notification_mixin.py` & `django-project-base-0.4.9/django_project_base/notifications/base/duplicate_notification_mixin.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/enums.py` & `django-project-base-0.4.9/django_project_base/notifications/base/enums.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/notification.py` & `django-project-base-0.4.9/django_project_base/notifications/base/notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/phone_number_parser.py` & `django-project-base-0.4.9/django_project_base/notifications/base/phone_number_parser.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/queable_notification_mixin.py` & `django-project-base-0.4.9/django_project_base/notifications/base/queable_notification_mixin.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/base/send_notification_mixin.py` & `django-project-base-0.4.9/django_project_base/notifications/base/send_notification_mixin.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/email_notification.py` & `django-project-base-0.4.9/django_project_base/notifications/email_notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/maintenance_notification.py` & `django-project-base-0.4.9/django_project_base/notifications/maintenance_notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/management/commands/resend_notification.py` & `django-project-base-0.4.9/django_project_base/notifications/management/commands/resend_notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/migrations/0001_initial.py` & `django-project-base-0.4.9/django_project_base/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py` & `django-project-base-0.4.9/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py` & `django-project-base-0.4.9/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/migrations/0005_merge_20230906_1213.py` & `django-project-base-0.4.9/django_project_base/notifications/migrations/0005_merge_20230906_1213.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py` & `django-project-base-0.4.9/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/migrations/0007_auto_20231026_0555.py` & `django-project-base-0.4.9/django_project_base/notifications/migrations/0007_auto_20231026_0555.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/migrations/0009_auto_20231108_0658.py` & `django-project-base-0.4.9/django_project_base/notifications/migrations/0009_auto_20231108_0658.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/models.py` & `django-project-base-0.4.9/django_project_base/notifications/models.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/notification_queryset.py` & `django-project-base-0.4.9/django_project_base/notifications/notification_queryset.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/rest/delivery_report.py` & `django-project-base-0.4.9/django_project_base/notifications/rest/delivery_report.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/rest/maintenance_notification.py` & `django-project-base-0.4.9/django_project_base/notifications/rest/maintenance_notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/rest/notification.py` & `django-project-base-0.4.9/django_project_base/notifications/rest/notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/rest/router.py` & `django-project-base-0.4.9/django_project_base/notifications/rest/router.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/settings.py` & `django-project-base-0.4.9/django_project_base/notifications/settings.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/templates/notification.html` & `django-project-base-0.4.9/django_project_base/notifications/templates/notification.html`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/templates/notification_login.html` & `django-project-base-0.4.9/django_project_base/notifications/templates/notification_login.html`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/tests/api/test_create_mail.py` & `django-project-base-0.4.9/django_project_base/notifications/tests/api/test_create_mail.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/tests/api/test_list_mail.py` & `django-project-base-0.4.9/django_project_base/notifications/tests/api/test_list_mail.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/tests/api/test_remainig_license.py` & `django-project-base-0.4.9/django_project_base/notifications/tests/api/test_remainig_license.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/tests/api/test_retrieve_mail.py` & `django-project-base-0.4.9/django_project_base/notifications/tests/api/test_retrieve_mail.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/tests/notifications_transaction_test_case.py` & `django-project-base-0.4.9/django_project_base/notifications/tests/notifications_transaction_test_case.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/tests/unit/test_is_mail_sent.py` & `django-project-base-0.4.9/django_project_base/notifications/tests/unit/test_is_mail_sent.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py` & `django-project-base-0.4.9/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/profiling/middleware.py` & `django-project-base-0.4.9/django_project_base/profiling/middleware.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/profiling/performance_base_command.py` & `django-project-base-0.4.9/django_project_base/profiling/performance_base_command.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/profiling/views.py` & `django-project-base-0.4.9/django_project_base/profiling/views.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/rest/project.py` & `django-project-base-0.4.9/django_project_base/rest/project.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/rest/project_role.py` & `django-project-base-0.4.9/django_project_base/rest/project_role.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/router.py` & `django-project-base-0.4.9/django_project_base/router.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/settings.py` & `django-project-base-0.4.9/django_project_base/settings.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/settings_parser.py` & `django-project-base-0.4.9/django_project_base/settings_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections import Iterable
+from collections.abc import Iterable
 from typing import Any
 
 
 def parse_settings(input_settings: tuple) -> None:
     from django.conf import settings
 
     for _setting in input_settings:
```

### Comparing `django-project-base-0.4.8/django_project_base/static/browser-update/update.min.js` & `django-project-base-0.4.9/django_project_base/static/browser-update/update.min.js`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/templates/app-debug/main.html` & `django-project-base-0.4.9/django_project_base/templates/app-debug/main.html`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/urls.py` & `django-project-base-0.4.9/django_project_base/urls.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/utils.py` & `django-project-base-0.4.9/django_project_base/utils.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base/views.py` & `django-project-base-0.4.9/django_project_base/views.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/django_project_base.egg-info/PKG-INFO` & `django-project-base-0.4.9/django_project_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-project-base
-Version: 0.4.8
+Version: 0.4.9
 Summary: Everything revolves around it: users, roles, permissions, tags, etc.
 Home-page: https://github.com/velis74/django-project-base
 Author: Jure Erznožnik
 Author-email: jure@velis.si
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-project-base-0.4.8/django_project_base.egg-info/SOURCES.txt` & `django-project-base-0.4.9/django_project_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.8/setup.py` & `django-project-base-0.4.9/setup.py`

 * *Files identical despite different names*

