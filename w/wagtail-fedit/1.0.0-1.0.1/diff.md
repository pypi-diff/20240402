# Comparing `tmp/wagtail_fedit-1.0.0.tar.gz` & `tmp/wagtail_fedit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.0.0.tar", last modified: Mon Apr  1 21:27:05 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.0.1.tar", last modified: Mon Apr  1 21:35:07 2024, max compression
```

## Comparing `wagtail_fedit-1.0.0.tar` & `wagtail_fedit-1.0.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.534991 wagtail_fedit-1.0.0/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1273 2024-04-01 21:27:05.534991 wagtail_fedit-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-01 21:27:05.552923 wagtail_fedit-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.211053 wagtail_fedit-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.213081 wagtail_fedit-1.0.0/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.214995 wagtail_fedit-1.0.0/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.215532 wagtail_fedit-1.0.0/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.219809 wagtail_fedit-1.0.0/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.0/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.288211 wagtail_fedit-1.0.0/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.0/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.0/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.0/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.335649 wagtail_fedit-1.0.0/wagtail_fedit/block_forms/
--rw-rw-rw-   0        0        0      334 2024-03-30 17:06:54.000000 wagtail_fedit-1.0.0/wagtail_fedit/block_forms/__init__.py
--rw-rw-rw-   0        0        0     1471 2024-03-30 18:10:34.000000 wagtail_fedit-1.0.0/wagtail_fedit/block_forms/field_conversions.py
--rw-rw-rw-   0        0        0     7932 2024-04-01 21:09:37.000000 wagtail_fedit-1.0.0/wagtail_fedit/block_forms/forms.py
--rw-rw-rw-   0        0        0     2298 2024-04-01 21:02:12.000000 wagtail_fedit-1.0.0/wagtail_fedit/block_forms/subform_field.py
--rw-rw-rw-   0        0        0     4397 2024-04-01 20:14:21.000000 wagtail_fedit-1.0.0/wagtail_fedit/block_forms/utils.py
--rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.0.0/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.336813 wagtail_fedit-1.0.0/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.0/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.337375 wagtail_fedit-1.0.0/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.0/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.0/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.202615 wagtail_fedit-1.0.0/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.203143 wagtail_fedit-1.0.0/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.351042 wagtail_fedit-1.0.0/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.0.0/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.0.0/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.0.0/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.363881 wagtail_fedit-1.0.0/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    10317 2024-04-01 16:03:33.000000 wagtail_fedit-1.0.0/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.204242 wagtail_fedit-1.0.0/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.205273 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.374027 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.393264 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.408402 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      570 2024-04-01 16:14:23.000000 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     3851 2024-04-01 14:37:48.000000 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/editor/iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.430651 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-01 14:29:21.000000 wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.450267 wagtail_fedit-1.0.0/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.0.0/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.455188 wagtail_fedit-1.0.0/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.0/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16748 2024-04-01 17:25:24.000000 wagtail_fedit-1.0.0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13455 2024-04-01 17:25:22.000000 wagtail_fedit-1.0.0/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.455188 wagtail_fedit-1.0.0/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.0.0/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     9934 2024-04-01 21:23:20.000000 wagtail_fedit-1.0.0/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0       63 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.0/wagtail_fedit/tests.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.0.0/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.0.0/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     1236 2024-04-01 18:06:46.000000 wagtail_fedit-1.0.0/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.502712 wagtail_fedit-1.0.0/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.0.0/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8544 2024-04-01 18:38:00.000000 wagtail_fedit-1.0.0/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5329 2024-04-01 18:17:22.000000 wagtail_fedit-1.0.0/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    10807 2024-04-01 18:29:15.000000 wagtail_fedit-1.0.0/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.534991 wagtail_fedit-1.0.0/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      131 2024-04-01 18:07:12.000000 wagtail_fedit-1.0.0/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      394 2024-03-31 07:07:45.000000 wagtail_fedit-1.0.0/wagtail_fedit/wagtail_hooks/editorjs.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.0.0/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.0.0/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.0.0/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     2544 2024-04-01 20:53:54.000000 wagtail_fedit-1.0.0/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:27:05.534991 wagtail_fedit-1.0.0/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     1273 2024-04-01 21:27:04.000000 wagtail_fedit-1.0.0/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2511 2024-04-01 21:27:05.000000 wagtail_fedit-1.0.0/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 21:27:04.000000 wagtail_fedit-1.0.0/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-01 21:27:04.000000 wagtail_fedit-1.0.0/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-01 21:27:04.000000 wagtail_fedit-1.0.0/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.219655 wagtail_fedit-1.0.1/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1318 2024-04-01 21:35:07.219655 wagtail_fedit-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-04-01 21:34:47.000000 wagtail_fedit-1.0.1/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-01 21:35:07.230887 wagtail_fedit-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.164771 wagtail_fedit-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.165774 wagtail_fedit-1.0.1/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.167771 wagtail_fedit-1.0.1/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.167927 wagtail_fedit-1.0.1/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.171928 wagtail_fedit-1.0.1/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.1/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.178461 wagtail_fedit-1.0.1/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.1/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.1/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.1/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.192047 wagtail_fedit-1.0.1/wagtail_fedit/block_forms/
+-rw-rw-rw-   0        0        0      334 2024-03-30 17:06:54.000000 wagtail_fedit-1.0.1/wagtail_fedit/block_forms/__init__.py
+-rw-rw-rw-   0        0        0     1471 2024-03-30 18:10:34.000000 wagtail_fedit-1.0.1/wagtail_fedit/block_forms/field_conversions.py
+-rw-rw-rw-   0        0        0     7932 2024-04-01 21:09:37.000000 wagtail_fedit-1.0.1/wagtail_fedit/block_forms/forms.py
+-rw-rw-rw-   0        0        0     2298 2024-04-01 21:02:12.000000 wagtail_fedit-1.0.1/wagtail_fedit/block_forms/subform_field.py
+-rw-rw-rw-   0        0        0     4397 2024-04-01 20:14:21.000000 wagtail_fedit-1.0.1/wagtail_fedit/block_forms/utils.py
+-rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.0.1/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.193044 wagtail_fedit-1.0.1/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.1/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.193044 wagtail_fedit-1.0.1/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.1/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.1/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.154690 wagtail_fedit-1.0.1/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.154690 wagtail_fedit-1.0.1/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.197044 wagtail_fedit-1.0.1/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.0.1/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.0.1/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.0.1/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.198192 wagtail_fedit-1.0.1/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    10317 2024-04-01 16:03:33.000000 wagtail_fedit-1.0.1/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.155696 wagtail_fedit-1.0.1/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.156695 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.199203 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.201202 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.203201 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      570 2024-04-01 16:14:23.000000 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     3851 2024-04-01 14:37:48.000000 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/editor/iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.204200 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-01 14:29:21.000000 wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.206200 wagtail_fedit-1.0.1/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.0.1/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.207200 wagtail_fedit-1.0.1/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.1/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16748 2024-04-01 17:25:24.000000 wagtail_fedit-1.0.1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13455 2024-04-01 17:25:22.000000 wagtail_fedit-1.0.1/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.209317 wagtail_fedit-1.0.1/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.0.1/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     9934 2024-04-01 21:23:20.000000 wagtail_fedit-1.0.1/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0       63 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.1/wagtail_fedit/tests.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.0.1/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.0.1/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     1236 2024-04-01 18:06:46.000000 wagtail_fedit-1.0.1/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.211506 wagtail_fedit-1.0.1/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.0.1/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8544 2024-04-01 18:38:00.000000 wagtail_fedit-1.0.1/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5329 2024-04-01 18:17:22.000000 wagtail_fedit-1.0.1/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    10807 2024-04-01 18:29:15.000000 wagtail_fedit-1.0.1/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.217527 wagtail_fedit-1.0.1/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      131 2024-04-01 18:07:12.000000 wagtail_fedit-1.0.1/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      394 2024-03-31 07:07:45.000000 wagtail_fedit-1.0.1/wagtail_fedit/wagtail_hooks/editorjs.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.0.1/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.0.1/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.0.1/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     2544 2024-04-01 20:53:54.000000 wagtail_fedit-1.0.1/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:35:07.218529 wagtail_fedit-1.0.1/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     1318 2024-04-01 21:35:06.000000 wagtail_fedit-1.0.1/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2511 2024-04-01 21:35:07.000000 wagtail_fedit-1.0.1/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 21:35:06.000000 wagtail_fedit-1.0.1/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-01 21:35:06.000000 wagtail_fedit-1.0.1/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-01 21:35:06.000000 wagtail_fedit-1.0.1/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.0.0/LICENSE` & `wagtail_fedit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/PKG-INFO` & `wagtail_fedit-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.0.0
+Version: 1.0.1
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -22,24 +22,29 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=4.2
 Requires-Dist: Wagtail>=4.2
 
 wagtail_fedit
-================
+=============
 
 ...
 
 Quick start
 -----------
 
 1. Add 'wagtail_fedit' to your INSTALLED_APPS setting like this:
 
    ```
    INSTALLED_APPS = [
    ...,
    'wagtail_fedit',
    ]
    ```
-
 2. ...
+
+## Caveats
+
+## Settings
+
+## Models/Methods
```

### Comparing `wagtail_fedit-1.0.0/setup.cfg` & `wagtail_fedit-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
-00000030: 300d 0a64 6573 6372 6970 7469 6f6e 203d  0..description =
+00000030: 310d 0a64 6573 6372 6970 7469 6f6e 203d  1..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.0.0/tests/testapp/manage.py` & `wagtail_fedit-1.0.1/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.0.1/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.0.1/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/block_forms/field_conversions.py` & `wagtail_fedit-1.0.1/wagtail_fedit/block_forms/field_conversions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/block_forms/forms.py` & `wagtail_fedit-1.0.1/wagtail_fedit/block_forms/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/block_forms/subform_field.py` & `wagtail_fedit-1.0.1/wagtail_fedit/block_forms/subform_field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/block_forms/utils.py` & `wagtail_fedit-1.0.1/wagtail_fedit/block_forms/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.0.1/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.0.1/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.0.1/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/editor/field.html` & `wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/editor/field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/editor/iframe.html` & `wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/editor/iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.0.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.0.1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.0.1/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.0.1/wagtail_fedit/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.0.1/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/urls.py` & `wagtail_fedit-1.0.1/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/utils.py` & `wagtail_fedit-1.0.1/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.0.1/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.0.1/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.0.1/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.0.1/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.0.1/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.0.1/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.0.0
+Version: 1.0.1
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -22,24 +22,29 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=4.2
 Requires-Dist: Wagtail>=4.2
 
 wagtail_fedit
-================
+=============
 
 ...
 
 Quick start
 -----------
 
 1. Add 'wagtail_fedit' to your INSTALLED_APPS setting like this:
 
    ```
    INSTALLED_APPS = [
    ...,
    'wagtail_fedit',
    ]
    ```
-
 2. ...
+
+## Caveats
+
+## Settings
+
+## Models/Methods
```

### Comparing `wagtail_fedit-1.0.0/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.0.1/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

