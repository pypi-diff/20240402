# Comparing `tmp/wagtail_fedit-1.0.7.tar.gz` & `tmp/wagtail_fedit-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.0.7.tar", last modified: Tue Apr  2 20:47:15 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.0.8.tar", last modified: Tue Apr  2 20:57:07 2024, max compression
```

## Comparing `wagtail_fedit-1.0.7.tar` & `wagtail_fedit-1.0.8.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.766210 wagtail_fedit-1.0.7/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5010 2024-04-02 20:47:15.765200 wagtail_fedit-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3960 2024-04-02 20:46:59.000000 wagtail_fedit-1.0.7/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-02 20:47:15.777330 wagtail_fedit-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.719404 wagtail_fedit-1.0.7/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.720400 wagtail_fedit-1.0.7/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.721396 wagtail_fedit-1.0.7/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.722394 wagtail_fedit-1.0.7/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.725272 wagtail_fedit-1.0.7/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.7/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.730841 wagtail_fedit-1.0.7/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.7/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.7/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.7/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.737252 wagtail_fedit-1.0.7/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.0.7/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2403 2024-04-02 20:00:51.000000 wagtail_fedit-1.0.7/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.0.7/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.0.7/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.738254 wagtail_fedit-1.0.7/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.7/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.739461 wagtail_fedit-1.0.7/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.7/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.7/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.711044 wagtail_fedit-1.0.7/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.712355 wagtail_fedit-1.0.7/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.741859 wagtail_fedit-1.0.7/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.0.7/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.0.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.0.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.741859 wagtail_fedit-1.0.7/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    10561 2024-04-02 19:44:50.000000 wagtail_fedit-1.0.7/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.712355 wagtail_fedit-1.0.7/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.713737 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.743863 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.744863 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.748860 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
--rw-rw-rw-   0        0        0     1959 2024-04-02 19:17:17.000000 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.751349 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-02 20:15:18.000000 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
--rw-rw-rw-   0        0        0      845 2024-04-02 20:15:27.000000 wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.752353 wagtail_fedit-1.0.7/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.0.7/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.754805 wagtail_fedit-1.0.7/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.7/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16610 2024-04-02 18:36:53.000000 wagtail_fedit-1.0.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13337 2024-04-02 18:34:03.000000 wagtail_fedit-1.0.7/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.756150 wagtail_fedit-1.0.7/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.0.7/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.0.7/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.0.7/wagtail_fedit/tests.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.0.7/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.0.7/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     3806 2024-04-02 18:36:29.000000 wagtail_fedit-1.0.7/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.758390 wagtail_fedit-1.0.7/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.0.7/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8655 2024-04-02 19:18:27.000000 wagtail_fedit-1.0.7/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.0.7/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     9474 2024-04-02 20:03:35.000000 wagtail_fedit-1.0.7/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.763839 wagtail_fedit-1.0.7/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      106 2024-04-02 18:12:22.000000 wagtail_fedit-1.0.7/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.0.7/wagtail_fedit/wagtail_hooks/editorjs.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.0.7/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.0.7/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.0.7/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.0.7/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:47:15.765200 wagtail_fedit-1.0.7/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     5010 2024-04-02 20:47:15.000000 wagtail_fedit-1.0.7/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2670 2024-04-02 20:47:15.000000 wagtail_fedit-1.0.7/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 20:47:15.000000 wagtail_fedit-1.0.7/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-02 20:47:15.000000 wagtail_fedit-1.0.7/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-02 20:47:15.000000 wagtail_fedit-1.0.7/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.984141 wagtail_fedit-1.0.8/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5476 2024-04-02 20:57:07.984141 wagtail_fedit-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4426 2024-04-02 20:57:00.000000 wagtail_fedit-1.0.8/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-02 20:57:07.984141 wagtail_fedit-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.935346 wagtail_fedit-1.0.8/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.936770 wagtail_fedit-1.0.8/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.939125 wagtail_fedit-1.0.8/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.939866 wagtail_fedit-1.0.8/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.943065 wagtail_fedit-1.0.8/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.8/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.949198 wagtail_fedit-1.0.8/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.8/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.8/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.8/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.961668 wagtail_fedit-1.0.8/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.0.8/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2403 2024-04-02 20:00:51.000000 wagtail_fedit-1.0.8/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.0.8/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.0.8/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.962173 wagtail_fedit-1.0.8/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.8/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.963068 wagtail_fedit-1.0.8/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.8/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.8/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.919508 wagtail_fedit-1.0.8/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.919508 wagtail_fedit-1.0.8/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.963068 wagtail_fedit-1.0.8/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.0.8/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.0.8/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.0.8/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.963068 wagtail_fedit-1.0.8/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    10561 2024-04-02 19:44:50.000000 wagtail_fedit-1.0.8/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.919508 wagtail_fedit-1.0.8/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.919508 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.968156 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.968156 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.968156 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
+-rw-rw-rw-   0        0        0     1959 2024-04-02 19:17:17.000000 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.968156 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-02 20:15:18.000000 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+-rw-rw-rw-   0        0        0      845 2024-04-02 20:15:27.000000 wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.968156 wagtail_fedit-1.0.8/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.0.8/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.980502 wagtail_fedit-1.0.8/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.8/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16610 2024-04-02 18:36:53.000000 wagtail_fedit-1.0.8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13337 2024-04-02 18:34:03.000000 wagtail_fedit-1.0.8/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.980502 wagtail_fedit-1.0.8/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.0.8/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.0.8/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.0.8/wagtail_fedit/tests.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.0.8/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.0.8/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     3806 2024-04-02 18:36:29.000000 wagtail_fedit-1.0.8/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.984141 wagtail_fedit-1.0.8/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.0.8/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8655 2024-04-02 19:18:27.000000 wagtail_fedit-1.0.8/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.0.8/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     9474 2024-04-02 20:03:35.000000 wagtail_fedit-1.0.8/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.984141 wagtail_fedit-1.0.8/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      106 2024-04-02 18:12:22.000000 wagtail_fedit-1.0.8/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.0.8/wagtail_fedit/wagtail_hooks/editorjs.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.0.8/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.0.8/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.0.8/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.0.8/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:57:07.984141 wagtail_fedit-1.0.8/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     5476 2024-04-02 20:57:07.000000 wagtail_fedit-1.0.8/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2670 2024-04-02 20:57:07.000000 wagtail_fedit-1.0.8/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 20:57:07.000000 wagtail_fedit-1.0.8/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-02 20:57:07.000000 wagtail_fedit-1.0.8/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-02 20:57:07.000000 wagtail_fedit-1.0.8/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.0.7/LICENSE` & `wagtail_fedit-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/PKG-INFO` & `wagtail_fedit-1.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.0.7
+Version: 1.0.8
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -49,15 +49,15 @@
 
    **This is a requirement.**
 2. Define a template for your model.
 
    Example:
 
    ```django-html
-   {% load fedit static %} {# Load the required template tag libraries #}
+   {% load fedit static wagtailuserbar %} {# Load the required template tag libraries #}
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
        <link rel="stylesheet" href="{% static 'wagtail_fedit/css/frontend.css' %}">
@@ -67,14 +67,16 @@
        <h1>{% fedit_field "title" self %}</h1>
 
        {# Pass in the field_name and the model instance on which that field resides. #}
        <main class="my-streamfield-content">
            {% fedit_field "content" self %}
        </main>
 
+       {% wagtailuserbar %}
+
        <script src="{% static 'wagtail_fedit/js/frontend.js' %}"></script>
    </body>
    </html>
 
 
    ```
 3. If your needs some special form of rendering; we allow your model to define a custom render method.
@@ -100,25 +102,30 @@
    class MyPage(...): # Can be any type of model.
        content = StreamField(...)
 
        def render_fedit_content(self, request):
            return render_to_string("myapp/render_my_field.html", self.get_context(request))
    ```
 
-   Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %}`
+   Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %} `
 
+4. **But wait?! I go to my template and I do not see a way to edit!**  
+   That is true! We try to protect any styling on your actual page; we do not want to interfere.  
+   Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar.  
+   Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
+   
 ## Revisions
 
 Revision support is included out of the box.
 If your model inherits from a `RevisionMixin`, we will automatically create drafts for you.
 These will not be published (If the model inherits from `DraftStateMixin`) until you choose to do so.
 
 ## Logs
 
-Logs are also included out of the box.  
+Logs are also included out of the box.
 We will automatically update your model's history; including possible revisions.
 This will allow you to backtrack each change made on the frontend.
 This however does mean that a possibly large amount of data will be stored in your database.
 
 ## Caveats
 
 Wagtail does not always make it's `id` attribute available.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.0.7 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.0.8 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
@@ -14,45 +14,51 @@
 Django>=4.2 Requires-Dist: Wagtail>=4.2 wagtail_fedit ============= Wagtail
 FEdit is a library to allow your Wagtail pages and content-blocks to be edited
 on the frontend. Getting Started --------------- 1. Add 'wagtail_fedit' to your
 INSTALLED_APPS setting like this: ``` INSTALLED_APPS = [ ..., 'wagtail_fedit',
 ] ``` 2. Run `py ./manage.py collectstatic`. ## Getting Editing! 1. Make sure
 the models you wish to edit inherit from PreviewableMixin. **This is a
 requirement.** 2. Define a template for your model. Example: ```django-html {%
-load fedit static %} {# Load the required template tag libraries #}
+load fedit static wagtailuserbar %} {# Load the required template tag libraries
+#}
 {# Pass in the field_name and the model instance on which that field resides.
 #}
 ************ {{%% ffeeddiitt__ffiieelldd ""ttiittllee"" sseellff %%}} ************
 {# Pass in the field_name and the model instance on which that field resides.
-#} {% fedit_field "content" self %}
+#} {% fedit_field "content" self %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
 fedit %} {% for block in self.content %} {% fedit_block block=block
 block_id=block.id field_name="content" model=self %} {% endfor %} ``` ```python
 from django.template.loader import render_to_string ... class MyPage(...): #
 Can be any type of model. content = StreamField(...) def render_fedit_content
 (self, request): return render_to_string("myapp/render_my_field.html",
 self.get_context(request)) ``` Your content will then automatically be rendered
-with that method when need be by using `{% fedit_field "content" self %}` ##
-Revisions Revision support is included out of the box. If your model inherits
-from a `RevisionMixin`, we will automatically create drafts for you. These will
-not be published (If the model inherits from `DraftStateMixin`) until you
-choose to do so. ## Logs Logs are also included out of the box. We will
-automatically update your model's history; including possible revisions. This
-will allow you to backtrack each change made on the frontend. This however does
-mean that a possibly large amount of data will be stored in your database. ##
-Caveats Wagtail does not always make it's `id` attribute available. This is
-only available to instances of `StreamChild` and `ListChild`. Consider the
-following regular wagtail list loop where `items` is a `ListBlock`. ```django-
-html {% for item in self.items %} {% include_block item %} {# No access to ID!
-Cannot edit! #} {% endfor %} ``` To make this an editable block instead; we
-would slightly change the loop to make the block's `id` available. This is done
-by accessing the `bound_blocks` of that ListBlock *(`StreamBlock` does this
-automatically for the toplevel block!)* Our new loop would then be: ```django-
-html {% for item in self.items.bound_blocks %} {# Field name and model are the
-same arguments as in the first example! #} {% fedit_block block=item
-block_id=item.id field_name="content" model=self %} {% endfor %} ``` ##
-Settings ## Models/Methods
+with that method when need be by using `{% fedit_field "content" self %} ` 4.
+**But wait?! I go to my template and I do not see a way to edit!** That is
+true! We try to protect any styling on your actual page; we do not want to
+interfere. Instead; we serve the editing interface on a different URL,
+accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye
+on that userbar! It is also used for publishing if your model inherits from
+`DraftStateMixin`. ## Revisions Revision support is included out of the box. If
+your model inherits from a `RevisionMixin`, we will automatically create drafts
+for you. These will not be published (If the model inherits from
+`DraftStateMixin`) until you choose to do so. ## Logs Logs are also included
+out of the box. We will automatically update your model's history; including
+possible revisions. This will allow you to backtrack each change made on the
+frontend. This however does mean that a possibly large amount of data will be
+stored in your database. ## Caveats Wagtail does not always make it's `id`
+attribute available. This is only available to instances of `StreamChild` and
+`ListChild`. Consider the following regular wagtail list loop where `items` is
+a `ListBlock`. ```django-html {% for item in self.items %} {% include_block
+item %} {# No access to ID! Cannot edit! #} {% endfor %} ``` To make this an
+editable block instead; we would slightly change the loop to make the block's
+`id` available. This is done by accessing the `bound_blocks` of that ListBlock
+*(`StreamBlock` does this automatically for the toplevel block!)* Our new loop
+would then be: ```django-html {% for item in self.items.bound_blocks %} {#
+Field name and model are the same arguments as in the first example! #} {%
+fedit_block block=item block_id=item.id field_name="content" model=self %} {%
+endfor %} ``` ## Settings ## Models/Methods
```

### Comparing `wagtail_fedit-1.0.7/README.md` & `wagtail_fedit-1.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
    **This is a requirement.**
 2. Define a template for your model.
 
    Example:
 
    ```django-html
-   {% load fedit static %} {# Load the required template tag libraries #}
+   {% load fedit static wagtailuserbar %} {# Load the required template tag libraries #}
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
        <link rel="stylesheet" href="{% static 'wagtail_fedit/css/frontend.css' %}">
@@ -40,14 +40,16 @@
        <h1>{% fedit_field "title" self %}</h1>
 
        {# Pass in the field_name and the model instance on which that field resides. #}
        <main class="my-streamfield-content">
            {% fedit_field "content" self %}
        </main>
 
+       {% wagtailuserbar %}
+
        <script src="{% static 'wagtail_fedit/js/frontend.js' %}"></script>
    </body>
    </html>
 
 
    ```
 3. If your needs some special form of rendering; we allow your model to define a custom render method.
@@ -73,25 +75,30 @@
    class MyPage(...): # Can be any type of model.
        content = StreamField(...)
 
        def render_fedit_content(self, request):
            return render_to_string("myapp/render_my_field.html", self.get_context(request))
    ```
 
-   Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %}`
+   Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %} `
 
+4. **But wait?! I go to my template and I do not see a way to edit!**  
+   That is true! We try to protect any styling on your actual page; we do not want to interfere.  
+   Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar.  
+   Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
+   
 ## Revisions
 
 Revision support is included out of the box.
 If your model inherits from a `RevisionMixin`, we will automatically create drafts for you.
 These will not be published (If the model inherits from `DraftStateMixin`) until you choose to do so.
 
 ## Logs
 
-Logs are also included out of the box.  
+Logs are also included out of the box.
 We will automatically update your model's history; including possible revisions.
 This will allow you to backtrack each change made on the frontend.
 This however does mean that a possibly large amount of data will be stored in your database.
 
 ## Caveats
 
 Wagtail does not always make it's `id` attribute available.
```

#### html2text {}

```diff
@@ -1,45 +1,50 @@
 wagtail_fedit ============= Wagtail FEdit is a library to allow your Wagtail
 pages and content-blocks to be edited on the frontend. Getting Started --------
 ------- 1. Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
 INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
 collectstatic`. ## Getting Editing! 1. Make sure the models you wish to edit
 inherit from PreviewableMixin. **This is a requirement.** 2. Define a template
-for your model. Example: ```django-html {% load fedit static %} {# Load the
-required template tag libraries #}
+for your model. Example: ```django-html {% load fedit static wagtailuserbar %}
+{# Load the required template tag libraries #}
 {# Pass in the field_name and the model instance on which that field resides.
 #}
 ************ {{%% ffeeddiitt__ffiieelldd ""ttiittllee"" sseellff %%}} ************
 {# Pass in the field_name and the model instance on which that field resides.
-#} {% fedit_field "content" self %}
+#} {% fedit_field "content" self %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
 fedit %} {% for block in self.content %} {% fedit_block block=block
 block_id=block.id field_name="content" model=self %} {% endfor %} ``` ```python
 from django.template.loader import render_to_string ... class MyPage(...): #
 Can be any type of model. content = StreamField(...) def render_fedit_content
 (self, request): return render_to_string("myapp/render_my_field.html",
 self.get_context(request)) ``` Your content will then automatically be rendered
-with that method when need be by using `{% fedit_field "content" self %}` ##
-Revisions Revision support is included out of the box. If your model inherits
-from a `RevisionMixin`, we will automatically create drafts for you. These will
-not be published (If the model inherits from `DraftStateMixin`) until you
-choose to do so. ## Logs Logs are also included out of the box. We will
-automatically update your model's history; including possible revisions. This
-will allow you to backtrack each change made on the frontend. This however does
-mean that a possibly large amount of data will be stored in your database. ##
-Caveats Wagtail does not always make it's `id` attribute available. This is
-only available to instances of `StreamChild` and `ListChild`. Consider the
-following regular wagtail list loop where `items` is a `ListBlock`. ```django-
-html {% for item in self.items %} {% include_block item %} {# No access to ID!
-Cannot edit! #} {% endfor %} ``` To make this an editable block instead; we
-would slightly change the loop to make the block's `id` available. This is done
-by accessing the `bound_blocks` of that ListBlock *(`StreamBlock` does this
-automatically for the toplevel block!)* Our new loop would then be: ```django-
-html {% for item in self.items.bound_blocks %} {# Field name and model are the
-same arguments as in the first example! #} {% fedit_block block=item
-block_id=item.id field_name="content" model=self %} {% endfor %} ``` ##
-Settings ## Models/Methods
+with that method when need be by using `{% fedit_field "content" self %} ` 4.
+**But wait?! I go to my template and I do not see a way to edit!** That is
+true! We try to protect any styling on your actual page; we do not want to
+interfere. Instead; we serve the editing interface on a different URL,
+accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye
+on that userbar! It is also used for publishing if your model inherits from
+`DraftStateMixin`. ## Revisions Revision support is included out of the box. If
+your model inherits from a `RevisionMixin`, we will automatically create drafts
+for you. These will not be published (If the model inherits from
+`DraftStateMixin`) until you choose to do so. ## Logs Logs are also included
+out of the box. We will automatically update your model's history; including
+possible revisions. This will allow you to backtrack each change made on the
+frontend. This however does mean that a possibly large amount of data will be
+stored in your database. ## Caveats Wagtail does not always make it's `id`
+attribute available. This is only available to instances of `StreamChild` and
+`ListChild`. Consider the following regular wagtail list loop where `items` is
+a `ListBlock`. ```django-html {% for item in self.items %} {% include_block
+item %} {# No access to ID! Cannot edit! #} {% endfor %} ``` To make this an
+editable block instead; we would slightly change the loop to make the block's
+`id` available. This is done by accessing the `bound_blocks` of that ListBlock
+*(`StreamBlock` does this automatically for the toplevel block!)* Our new loop
+would then be: ```django-html {% for item in self.items.bound_blocks %} {#
+Field name and model are the same arguments as in the first example! #} {%
+fedit_block block=item block_id=item.id field_name="content" model=self %} {%
+endfor %} ``` ## Settings ## Models/Methods
```

### Comparing `wagtail_fedit-1.0.7/setup.cfg` & `wagtail_fedit-1.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
-00000030: 370d 0a64 6573 6372 6970 7469 6f6e 203d  7..description =
+00000030: 380d 0a64 6573 6372 6970 7469 6f6e 203d  8..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.0.7/tests/testapp/manage.py` & `wagtail_fedit-1.0.8/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.0.8/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.0.8/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.0.8/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.0.8/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.0.8/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.0.8/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.0.8/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.0.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.0.8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.0.8/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.0.8/wagtail_fedit/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.0.8/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/urls.py` & `wagtail_fedit-1.0.8/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/utils.py` & `wagtail_fedit-1.0.8/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.0.8/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.0.8/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.0.8/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.0.8/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.0.8/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.0.8/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.0.7
+Version: 1.0.8
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -49,15 +49,15 @@
 
    **This is a requirement.**
 2. Define a template for your model.
 
    Example:
 
    ```django-html
-   {% load fedit static %} {# Load the required template tag libraries #}
+   {% load fedit static wagtailuserbar %} {# Load the required template tag libraries #}
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
        <link rel="stylesheet" href="{% static 'wagtail_fedit/css/frontend.css' %}">
@@ -67,14 +67,16 @@
        <h1>{% fedit_field "title" self %}</h1>
 
        {# Pass in the field_name and the model instance on which that field resides. #}
        <main class="my-streamfield-content">
            {% fedit_field "content" self %}
        </main>
 
+       {% wagtailuserbar %}
+
        <script src="{% static 'wagtail_fedit/js/frontend.js' %}"></script>
    </body>
    </html>
 
 
    ```
 3. If your needs some special form of rendering; we allow your model to define a custom render method.
@@ -100,25 +102,30 @@
    class MyPage(...): # Can be any type of model.
        content = StreamField(...)
 
        def render_fedit_content(self, request):
            return render_to_string("myapp/render_my_field.html", self.get_context(request))
    ```
 
-   Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %}`
+   Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %} `
 
+4. **But wait?! I go to my template and I do not see a way to edit!**  
+   That is true! We try to protect any styling on your actual page; we do not want to interfere.  
+   Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar.  
+   Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
+   
 ## Revisions
 
 Revision support is included out of the box.
 If your model inherits from a `RevisionMixin`, we will automatically create drafts for you.
 These will not be published (If the model inherits from `DraftStateMixin`) until you choose to do so.
 
 ## Logs
 
-Logs are also included out of the box.  
+Logs are also included out of the box.
 We will automatically update your model's history; including possible revisions.
 This will allow you to backtrack each change made on the frontend.
 This however does mean that a possibly large amount of data will be stored in your database.
 
 ## Caveats
 
 Wagtail does not always make it's `id` attribute available.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.0.7 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.0.8 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
@@ -14,45 +14,51 @@
 Django>=4.2 Requires-Dist: Wagtail>=4.2 wagtail_fedit ============= Wagtail
 FEdit is a library to allow your Wagtail pages and content-blocks to be edited
 on the frontend. Getting Started --------------- 1. Add 'wagtail_fedit' to your
 INSTALLED_APPS setting like this: ``` INSTALLED_APPS = [ ..., 'wagtail_fedit',
 ] ``` 2. Run `py ./manage.py collectstatic`. ## Getting Editing! 1. Make sure
 the models you wish to edit inherit from PreviewableMixin. **This is a
 requirement.** 2. Define a template for your model. Example: ```django-html {%
-load fedit static %} {# Load the required template tag libraries #}
+load fedit static wagtailuserbar %} {# Load the required template tag libraries
+#}
 {# Pass in the field_name and the model instance on which that field resides.
 #}
 ************ {{%% ffeeddiitt__ffiieelldd ""ttiittllee"" sseellff %%}} ************
 {# Pass in the field_name and the model instance on which that field resides.
-#} {% fedit_field "content" self %}
+#} {% fedit_field "content" self %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
 fedit %} {% for block in self.content %} {% fedit_block block=block
 block_id=block.id field_name="content" model=self %} {% endfor %} ``` ```python
 from django.template.loader import render_to_string ... class MyPage(...): #
 Can be any type of model. content = StreamField(...) def render_fedit_content
 (self, request): return render_to_string("myapp/render_my_field.html",
 self.get_context(request)) ``` Your content will then automatically be rendered
-with that method when need be by using `{% fedit_field "content" self %}` ##
-Revisions Revision support is included out of the box. If your model inherits
-from a `RevisionMixin`, we will automatically create drafts for you. These will
-not be published (If the model inherits from `DraftStateMixin`) until you
-choose to do so. ## Logs Logs are also included out of the box. We will
-automatically update your model's history; including possible revisions. This
-will allow you to backtrack each change made on the frontend. This however does
-mean that a possibly large amount of data will be stored in your database. ##
-Caveats Wagtail does not always make it's `id` attribute available. This is
-only available to instances of `StreamChild` and `ListChild`. Consider the
-following regular wagtail list loop where `items` is a `ListBlock`. ```django-
-html {% for item in self.items %} {% include_block item %} {# No access to ID!
-Cannot edit! #} {% endfor %} ``` To make this an editable block instead; we
-would slightly change the loop to make the block's `id` available. This is done
-by accessing the `bound_blocks` of that ListBlock *(`StreamBlock` does this
-automatically for the toplevel block!)* Our new loop would then be: ```django-
-html {% for item in self.items.bound_blocks %} {# Field name and model are the
-same arguments as in the first example! #} {% fedit_block block=item
-block_id=item.id field_name="content" model=self %} {% endfor %} ``` ##
-Settings ## Models/Methods
+with that method when need be by using `{% fedit_field "content" self %} ` 4.
+**But wait?! I go to my template and I do not see a way to edit!** That is
+true! We try to protect any styling on your actual page; we do not want to
+interfere. Instead; we serve the editing interface on a different URL,
+accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye
+on that userbar! It is also used for publishing if your model inherits from
+`DraftStateMixin`. ## Revisions Revision support is included out of the box. If
+your model inherits from a `RevisionMixin`, we will automatically create drafts
+for you. These will not be published (If the model inherits from
+`DraftStateMixin`) until you choose to do so. ## Logs Logs are also included
+out of the box. We will automatically update your model's history; including
+possible revisions. This will allow you to backtrack each change made on the
+frontend. This however does mean that a possibly large amount of data will be
+stored in your database. ## Caveats Wagtail does not always make it's `id`
+attribute available. This is only available to instances of `StreamChild` and
+`ListChild`. Consider the following regular wagtail list loop where `items` is
+a `ListBlock`. ```django-html {% for item in self.items %} {% include_block
+item %} {# No access to ID! Cannot edit! #} {% endfor %} ``` To make this an
+editable block instead; we would slightly change the loop to make the block's
+`id` available. This is done by accessing the `bound_blocks` of that ListBlock
+*(`StreamBlock` does this automatically for the toplevel block!)* Our new loop
+would then be: ```django-html {% for item in self.items.bound_blocks %} {#
+Field name and model are the same arguments as in the first example! #} {%
+fedit_block block=item block_id=item.id field_name="content" model=self %} {%
+endfor %} ``` ## Settings ## Models/Methods
```

### Comparing `wagtail_fedit-1.0.7/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.0.8/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

