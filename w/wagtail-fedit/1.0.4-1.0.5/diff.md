# Comparing `tmp/wagtail_fedit-1.0.4.tar.gz` & `tmp/wagtail_fedit-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.0.4.tar", last modified: Tue Apr  2 20:07:23 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.0.5.tar", last modified: Tue Apr  2 20:40:13 2024, max compression
```

## Comparing `wagtail_fedit-1.0.4.tar` & `wagtail_fedit-1.0.5.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.361981 wagtail_fedit-1.0.4/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1326 2024-04-02 20:07:23.360979 wagtail_fedit-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-04-01 21:38:14.000000 wagtail_fedit-1.0.4/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-02 20:07:23.369983 wagtail_fedit-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.008841 wagtail_fedit-1.0.4/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.014858 wagtail_fedit-1.0.4/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.021218 wagtail_fedit-1.0.4/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.022208 wagtail_fedit-1.0.4/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.054585 wagtail_fedit-1.0.4/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.110451 wagtail_fedit-1.0.4/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.4/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.4/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.4/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.143581 wagtail_fedit-1.0.4/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.0.4/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2403 2024-04-02 20:00:51.000000 wagtail_fedit-1.0.4/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.0.4/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.0.4/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.145578 wagtail_fedit-1.0.4/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.4/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.146577 wagtail_fedit-1.0.4/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.4/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.4/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:22.986078 wagtail_fedit-1.0.4/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:22.987078 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.164795 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.179795 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    10561 2024-04-02 19:44:50.000000 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:22.987078 wagtail_fedit-1.0.4/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:22.989045 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.193980 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.210175 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.238937 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
--rw-rw-rw-   0        0        0     1959 2024-04-02 19:17:17.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.255280 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-01 14:29:21.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.267279 wagtail_fedit-1.0.4/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.0.4/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.268338 wagtail_fedit-1.0.4/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.4/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16610 2024-04-02 18:36:53.000000 wagtail_fedit-1.0.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13337 2024-04-02 18:34:03.000000 wagtail_fedit-1.0.4/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.280012 wagtail_fedit-1.0.4/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.0.4/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.0.4/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.0.4/wagtail_fedit/tests.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.0.4/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.0.4/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     3806 2024-04-02 18:36:29.000000 wagtail_fedit-1.0.4/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.308603 wagtail_fedit-1.0.4/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.0.4/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8655 2024-04-02 19:18:27.000000 wagtail_fedit-1.0.4/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.0.4/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     9474 2024-04-02 20:03:35.000000 wagtail_fedit-1.0.4/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.357982 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      106 2024-04-02 18:12:22.000000 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/editorjs.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     2544 2024-04-01 20:53:54.000000 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.359979 wagtail_fedit-1.0.4/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     1326 2024-04-02 20:07:22.000000 wagtail_fedit-1.0.4/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2598 2024-04-02 20:07:22.000000 wagtail_fedit-1.0.4/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 20:07:22.000000 wagtail_fedit-1.0.4/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-02 20:07:22.000000 wagtail_fedit-1.0.4/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-02 20:07:22.000000 wagtail_fedit-1.0.4/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.743497 wagtail_fedit-1.0.5/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4439 2024-04-02 20:40:13.743497 wagtail_fedit-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3389 2024-04-02 20:39:49.000000 wagtail_fedit-1.0.5/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-02 20:40:13.748843 wagtail_fedit-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.593319 wagtail_fedit-1.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.594326 wagtail_fedit-1.0.5/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.595326 wagtail_fedit-1.0.5/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.596555 wagtail_fedit-1.0.5/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.600294 wagtail_fedit-1.0.5/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.5/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.619384 wagtail_fedit-1.0.5/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.5/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.5/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.5/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.636353 wagtail_fedit-1.0.5/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.0.5/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2403 2024-04-02 20:00:51.000000 wagtail_fedit-1.0.5/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.0.5/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.0.5/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.637360 wagtail_fedit-1.0.5/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.5/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.637360 wagtail_fedit-1.0.5/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.5/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.5/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.585132 wagtail_fedit-1.0.5/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.585132 wagtail_fedit-1.0.5/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.642599 wagtail_fedit-1.0.5/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.0.5/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.0.5/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.0.5/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.652599 wagtail_fedit-1.0.5/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    10561 2024-04-02 19:44:50.000000 wagtail_fedit-1.0.5/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.586137 wagtail_fedit-1.0.5/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.587132 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.654600 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.658752 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.666917 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
+-rw-rw-rw-   0        0        0     1959 2024-04-02 19:17:17.000000 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.677982 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-02 20:15:18.000000 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+-rw-rw-rw-   0        0        0      845 2024-04-02 20:15:27.000000 wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.684526 wagtail_fedit-1.0.5/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.0.5/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.686427 wagtail_fedit-1.0.5/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.5/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16610 2024-04-02 18:36:53.000000 wagtail_fedit-1.0.5/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13337 2024-04-02 18:34:03.000000 wagtail_fedit-1.0.5/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.700437 wagtail_fedit-1.0.5/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.0.5/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.0.5/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.0.5/wagtail_fedit/tests.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.0.5/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.0.5/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     3806 2024-04-02 18:36:29.000000 wagtail_fedit-1.0.5/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.729248 wagtail_fedit-1.0.5/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.0.5/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8655 2024-04-02 19:18:27.000000 wagtail_fedit-1.0.5/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.0.5/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     9474 2024-04-02 20:03:35.000000 wagtail_fedit-1.0.5/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.741476 wagtail_fedit-1.0.5/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      106 2024-04-02 18:12:22.000000 wagtail_fedit-1.0.5/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.0.5/wagtail_fedit/wagtail_hooks/editorjs.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.0.5/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.0.5/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.0.5/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.0.5/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:40:13.742503 wagtail_fedit-1.0.5/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     4439 2024-04-02 20:40:13.000000 wagtail_fedit-1.0.5/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2670 2024-04-02 20:40:13.000000 wagtail_fedit-1.0.5/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 20:40:13.000000 wagtail_fedit-1.0.5/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-02 20:40:13.000000 wagtail_fedit-1.0.5/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-02 20:40:13.000000 wagtail_fedit-1.0.5/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.0.4/LICENSE` & `wagtail_fedit-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/setup.cfg` & `wagtail_fedit-1.0.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
-00000030: 340d 0a64 6573 6372 6970 7469 6f6e 203d  4..description =
+00000030: 350d 0a64 6573 6372 6970 7469 6f6e 203d  5..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.0.4/tests/testapp/manage.py` & `wagtail_fedit-1.0.5/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.0.5/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.0.5/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.0.5/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.0.5/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.0.5/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.0.5/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.0.5/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.0.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.0.5/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.0.5/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.0.5/wagtail_fedit/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.0.5/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/urls.py` & `wagtail_fedit-1.0.5/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/utils.py` & `wagtail_fedit-1.0.5/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.0.5/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.0.5/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.0.5/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.0.5/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.0.5/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,26 @@
 
         return super().render(request)
 
 
 class WagtailFeditItem(BaseWagtailFeditItem):
     template = "wagtail_fedit/userbar/item_fedit.html"
 
+class WagtailFeditViewLiveItem(BaseWagtailFeditItem):
+    template = "wagtail_fedit/userbar/item_fedit_view_live.html"
+
+    def get_context_data(self, request):
+        context = super().get_context_data(request)
+        
+        if hasattr(self.model, "get_url"):
+            context["live_url"] = self.model.get_url(request)
+        elif hasattr(self.model, "get_absolute_url"):
+            context["live_url"] = self.model.get_absolute_url()
+
+        return context
     
 class WagtailFeditPublishItem(BaseWagtailFeditItem):
     template = "wagtail_fedit/userbar/item_fedit_publishing.html"
 
     def get_context_data(self, request):
         return super().get_context_data(request) | {
             "edit_url": reverse(
@@ -78,15 +90,19 @@
     
     if getattr(request, FEDIT_PREVIEW_VAR, False):
         if isinstance(model, DraftStateMixin):
             local_items.append(
                 WagtailFeditPublishItem(model),
             )
 
-        
+        if hasattr(model, "get_absolute_url") or hasattr(model, "get_url"):
+            local_items.append(
+                WagtailFeditViewLiveItem(model),
+            )
+
     if model and not getattr(request, FEDIT_PREVIEW_VAR, False):
         local_items.append(
             WagtailFeditItem(model),
         )
 
     items[:] = local_items + items
```

### Comparing `wagtail_fedit-1.0.4/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.0.5/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/field.html
 wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
 wagtail_fedit/templatetags/__init__.py
 wagtail_fedit/templatetags/fedit.py
 wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
 wagtail_fedit/tests/__init__.py
 wagtail_fedit/tests/test_blocks.py
 wagtail_fedit/views/__init__.py
```

