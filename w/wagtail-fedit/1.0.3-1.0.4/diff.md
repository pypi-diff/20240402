# Comparing `tmp/wagtail_fedit-1.0.3.tar.gz` & `tmp/wagtail_fedit-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.0.3.tar", last modified: Tue Apr  2 07:15:22 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.0.4.tar", last modified: Tue Apr  2 20:07:23 2024, max compression
```

## Comparing `wagtail_fedit-1.0.3.tar` & `wagtail_fedit-1.0.4.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.478103 wagtail_fedit-1.0.3/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1326 2024-04-02 07:15:22.478103 wagtail_fedit-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-04-01 21:38:14.000000 wagtail_fedit-1.0.3/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-02 07:15:22.486410 wagtail_fedit-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.072783 wagtail_fedit-1.0.3/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.081958 wagtail_fedit-1.0.3/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.093043 wagtail_fedit-1.0.3/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.094025 wagtail_fedit-1.0.3/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.130842 wagtail_fedit-1.0.3/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.195253 wagtail_fedit-1.0.3/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.3/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.3/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.3/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.252001 wagtail_fedit-1.0.3/wagtail_fedit/block_forms/
--rw-rw-rw-   0        0        0      334 2024-03-30 17:06:54.000000 wagtail_fedit-1.0.3/wagtail_fedit/block_forms/__init__.py
--rw-rw-rw-   0        0        0     1471 2024-03-30 18:10:34.000000 wagtail_fedit-1.0.3/wagtail_fedit/block_forms/field_conversions.py
--rw-rw-rw-   0        0        0     7932 2024-04-01 21:09:37.000000 wagtail_fedit-1.0.3/wagtail_fedit/block_forms/forms.py
--rw-rw-rw-   0        0        0     2369 2024-04-01 22:35:55.000000 wagtail_fedit-1.0.3/wagtail_fedit/block_forms/subform_field.py
--rw-rw-rw-   0        0        0     4397 2024-04-01 20:14:21.000000 wagtail_fedit-1.0.3/wagtail_fedit/block_forms/utils.py
--rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.0.3/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.254163 wagtail_fedit-1.0.3/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.3/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.257162 wagtail_fedit-1.0.3/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.3/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.059292 wagtail_fedit-1.0.3/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.060805 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.275092 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.289250 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    10317 2024-04-01 16:03:33.000000 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.060805 wagtail_fedit-1.0.3/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.062267 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.301273 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.316065 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.335774 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      570 2024-04-01 16:14:23.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     3381 2024-04-02 06:48:17.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/editor/iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.352080 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-01 14:29:21.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.362945 wagtail_fedit-1.0.3/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.0.3/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.366946 wagtail_fedit-1.0.3/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16748 2024-04-02 07:08:47.000000 wagtail_fedit-1.0.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13455 2024-04-02 07:08:45.000000 wagtail_fedit-1.0.3/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.380686 wagtail_fedit-1.0.3/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.0.3/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     9934 2024-04-01 21:23:20.000000 wagtail_fedit-1.0.3/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0       63 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.3/wagtail_fedit/tests.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.0.3/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.0.3/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     1236 2024-04-01 18:06:46.000000 wagtail_fedit-1.0.3/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.412934 wagtail_fedit-1.0.3/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.0.3/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8713 2024-04-02 07:11:24.000000 wagtail_fedit-1.0.3/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5329 2024-04-02 07:10:16.000000 wagtail_fedit-1.0.3/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    10807 2024-04-01 18:29:15.000000 wagtail_fedit-1.0.3/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.475946 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      131 2024-04-01 18:07:12.000000 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      394 2024-03-31 07:07:45.000000 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/editorjs.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     2544 2024-04-01 20:53:54.000000 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.476876 wagtail_fedit-1.0.3/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     1326 2024-04-02 07:15:21.000000 wagtail_fedit-1.0.3/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2511 2024-04-02 07:15:22.000000 wagtail_fedit-1.0.3/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 07:15:21.000000 wagtail_fedit-1.0.3/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-02 07:15:21.000000 wagtail_fedit-1.0.3/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-02 07:15:21.000000 wagtail_fedit-1.0.3/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.361981 wagtail_fedit-1.0.4/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1326 2024-04-02 20:07:23.360979 wagtail_fedit-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-04-01 21:38:14.000000 wagtail_fedit-1.0.4/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-02 20:07:23.369983 wagtail_fedit-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.008841 wagtail_fedit-1.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.014858 wagtail_fedit-1.0.4/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.021218 wagtail_fedit-1.0.4/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.022208 wagtail_fedit-1.0.4/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.054585 wagtail_fedit-1.0.4/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.4/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.110451 wagtail_fedit-1.0.4/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.4/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.4/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.4/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.143581 wagtail_fedit-1.0.4/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.0.4/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2403 2024-04-02 20:00:51.000000 wagtail_fedit-1.0.4/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.0.4/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.0.4/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.145578 wagtail_fedit-1.0.4/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.4/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.146577 wagtail_fedit-1.0.4/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.4/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.4/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:22.986078 wagtail_fedit-1.0.4/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:22.987078 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.164795 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.179795 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    10561 2024-04-02 19:44:50.000000 wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:22.987078 wagtail_fedit-1.0.4/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:22.989045 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.193980 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.210175 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.238937 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
+-rw-rw-rw-   0        0        0     1959 2024-04-02 19:17:17.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.255280 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-01 14:29:21.000000 wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.267279 wagtail_fedit-1.0.4/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.0.4/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.268338 wagtail_fedit-1.0.4/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.4/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16610 2024-04-02 18:36:53.000000 wagtail_fedit-1.0.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13337 2024-04-02 18:34:03.000000 wagtail_fedit-1.0.4/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.280012 wagtail_fedit-1.0.4/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.0.4/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.0.4/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.0.4/wagtail_fedit/tests.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.0.4/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.0.4/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     3806 2024-04-02 18:36:29.000000 wagtail_fedit-1.0.4/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.308603 wagtail_fedit-1.0.4/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.0.4/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8655 2024-04-02 19:18:27.000000 wagtail_fedit-1.0.4/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.0.4/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     9474 2024-04-02 20:03:35.000000 wagtail_fedit-1.0.4/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.357982 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      106 2024-04-02 18:12:22.000000 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/editorjs.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     2544 2024-04-01 20:53:54.000000 wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:07:23.359979 wagtail_fedit-1.0.4/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     1326 2024-04-02 20:07:22.000000 wagtail_fedit-1.0.4/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2598 2024-04-02 20:07:22.000000 wagtail_fedit-1.0.4/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 20:07:22.000000 wagtail_fedit-1.0.4/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-02 20:07:22.000000 wagtail_fedit-1.0.4/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-02 20:07:22.000000 wagtail_fedit-1.0.4/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.0.3/LICENSE` & `wagtail_fedit-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/PKG-INFO` & `wagtail_fedit-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.0.3
+Version: 1.0.4
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.0.3/setup.cfg` & `wagtail_fedit-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
-00000030: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
+00000030: 340d 0a64 6573 6372 6970 7469 6f6e 203d  4..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.0.3/tests/testapp/manage.py` & `wagtail_fedit-1.0.4/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.0.4/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.0.4/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/block_forms/subform_field.py` & `wagtail_fedit-1.0.4/wagtail_fedit/forms/blocks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,75 @@
-from typing import Any, Type
 from django import forms
-from django.http import (
-    HttpRequest,
+from django.db import models
+from wagtail.models import RevisionMixin
+from wagtail.blocks.base import (
+    BlockField,
+    BlockWidget,
+    BoundBlock,
 )
 from wagtail import blocks
-from .utils import get_block_name
 
-class SubformValidationError(forms.ValidationError):
-    def __init__(self, message, code=None, params=None):
-        if isinstance(message, dict):
-            self.subform_errors = message
-            message = list(message.values())
-        else:
-            self.subform_errors = {}
-        super().__init__(message, code, params)
+import warnings
 
-    def __repr__(self):
-        return str(self.subform_errors)
 
 
-class SubFormWidget(forms.Widget):
-    def __init__(self,
-            block:   blocks.BoundBlock,
-            form:    forms.Form,
-            request: HttpRequest,
-            attrs=None,
-        ):
-        self.block = block
-        self.form = form
-        self.request = request
-        super().__init__(attrs)
+class BlockWidgetWithErrors(BlockWidget):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.form_errors = None
 
     def render(self, name, value, attrs=None, renderer=None):
-        return self.form.as_p()
-    
-    def value_from_datadict(self, data, files, name):
-        return self.form.__class__(data=data, files=files, prefix=name, block=self.block, request=self.request)
-
-    def format_value(self, value: Any):
-        return value
-
-    @property
-    def media(self):
-        return self.form.media
-    
-
-class BlockEditSubFormField(forms.Field):
-    def __init__(self,
-            block: blocks.BoundBlock,
-            form: Type[forms.Form],
-            request: HttpRequest, 
-            *args,
-            **kwargs
-        ):
-        self.block:   blocks.BoundBlock = block
-        self.request: HttpRequest = request
+        if not self.form_errors:
+            return super().render(name, value, attrs, renderer)
+        
+        return self.render_with_errors(name, value, attrs, self.form_errors, renderer)
 
-        if self.request.method == "POST":
-            self.form = form(prefix=self.block_name, data=request.POST, block=block, request=request)
-        else:
-            self.form = form(prefix=self.block_name, block=block, request=request)
 
-        super().__init__(*args, **kwargs)
-        self.widget = SubFormWidget(block, self.form, request)
+def get_block_form_class(block: blocks.Block):
+
+    if isinstance(block, blocks.BoundBlock):
+        block = block.block
+
+    class BlockForm(BlockEditForm):
+        value = BlockField(block=block, widget=BlockWidgetWithErrors(block))
 
-    @property
-    def block_name(self):
-        return get_block_name(self.block)
+    return BlockForm
 
-    def validate(self, value: Any):
-        super().validate(value)
 
-        if not value.is_valid():
-            raise SubformValidationError(value.errors)
+class BlockEditForm(forms.Form):
+    def __init__(self, *args, block: BoundBlock, parent_instance: models.Model, request = None, **kwargs):
+        self.block = block
+        self.request = request
+        self.parent_instance = parent_instance
+
+        if "initial" not in kwargs:
+            kwargs["initial"] = {
+                "value": block.block.get_prep_value(block.value),
+            }
+
+        super().__init__(*args, **kwargs)
+
+    def full_clean(self):
+        super().full_clean()
+        if self.errors:
+            self.fields["value"].widget.form_errors = self.errors["value"]
+
+    def save(self):
+        block = self.cleaned_data["value"]
+        self.block.value = block
+        self.parent_instance.full_clean()
+
+        if isinstance(self.parent_instance, RevisionMixin) and self.request:
+            self.parent_instance = self.parent_instance.save_revision(
+                user=self.request.user,
+                log_action=False,
+            )
+        elif isinstance(self.parent_instance, RevisionMixin) and not self.request:
+            warnings.warn((
+                "RevisionMixin instance (%(model_type)s) provided without request," 
+                "skipping revision creation and saving model instance instead."
+            ) % {"model_type": type(self.parent_instance)})
+            self.parent_instance.save()
+        else:
+            self.parent_instance.save()
 
-    def clean(self, value: Any) -> Any:
-        value = super().clean(value)
-        return value.save()
+        return self.block
```

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.0.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -24,14 +24,18 @@
         return this.iframe;
     }
 
     get document() {
         return this.element.contentWindow.document;
     }
 
+    get window() {
+        return this.element.contentWindow;
+    }
+
     get mainElement() {
         return this.document.querySelector("#main");
     }
 
     get formElement() {
         return this.document.querySelector("#wagtail-fedit-form");
     }
@@ -163,14 +167,20 @@
                     }).then((response) => {
                         if (!response.success) {
                             console.error("Errors rendering response", response);
                             let newElement = document.createElement("div");
                             newElement.innerHTML = response.html;
                             this.iframe.mainElement.innerHTML = newElement.querySelector("#main").innerHTML;
                             this.iframe.formElement.onsubmit = onSubmit;
+
+                            const uninitializedBlock = this.iframe.mainElement.querySelector("#value[data-block]");
+                            if (uninitializedBlock) {
+                                this.iframe.window.initBlockWidget(uninitializedBlock.id);
+                            }
+
                             const cancelButton = this.iframe.document.querySelector("button.wagtail-fedit-cancel-button");
                             cancelButton.addEventListener("click", this.closeModal.bind(this));
                             return;
                         }
                         this.wrapperElement.style.display = "none";
                         this.setWrapperHtml(response.html);
                         this.initNewEditors();
@@ -191,18 +201,16 @@
                     )) ||
                     (formHeight > window.innerHeight)
                 ) {
                     this.modal.classList.add("fedit-full");
                 }
 
                 // Check if we should adjust the modal height to the height of the iframe form.
-                const modalheight = this.modal.getBoundingClientRect().height;
-                const formHeightDiff = modalheight - formHeight;
-                if (formHeightDiff > 0) {
-                    this.modal.style.height = `${modalheight + formHeightDiff}px`;
+                if (formHeight > this.modal.getBoundingClientRect().height) {
+                    this.modal.style.height = `${formHeight}px`;
                 }
 
                 const url = window.location.href.split("#")[0];
                 window.history.pushState(null, this.iframe.document.title, url + `#${this.wrapperElement.id}`);
                 document.title = this.iframe.document.title;
             },
         });
```

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/editor/iframe.html` & `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files 22% similar despite different names*

```diff
@@ -21,41 +21,15 @@
     <main class="content-wrapper w-overflow-x-hidden" id="main">
         {% block header %}
             <header class="nice-padding" id="modal-header">
                 <h1 id="modal-title">{{ view.get_header_title }}</h1>
             </header>
         {% endblock %}
         <div class="nice-padding">
-            <div class="wagtail-fedit-form-wrapper{% if form.block.block.meta.fedit_full %} fedit-full{% endif %}">
-                {% block errors %}
-                    {% if form.errors or form.non_field_errors %}
-                        <div class="error-message">
-                            <h2>{% translate "Validation errors" %}</h2>
-                            <ul>
-                                {% for error in form.non_field_errors %}
-                                    <li>{{ error }}</li>
-                                {% endfor %}
-                                {% for field, errors in form.errors.items %}
-                                    {% for error in errors %}
-                                        <li>{{ field }}: {{ error }}</li>
-                                    {% endfor %}
-                                {% endfor %}
-                            </ul>
-                        </div>
-                    {% endif %}
-                {% endblock %}
-                <form id="wagtail-fedit-form" action="{{ edit_url }}" method="post" {% for k, v in form_attrs.items %}{{ k }}="{{ v|safe }}" {% endfor %}>
-                    {% csrf_token %}
-                    <div class="wagtail-fedit-form">
-                        {% for field in form %}
-                            {% include "./field.html" %}
-                        {% endfor %}
-                    </div>
-                </form>
-            </div>
+            {% block content %}{% endblock %}
         </div>
     </main>
     <aside>
         <div class="fedit-sidebar-logo">
             {% block sidebar_logo %}{% endblock %}
         </div>
         <div class="fedit-sidebar">
```

#### html2text {}

```diff
@@ -2,24 +2,13 @@
 static %} {% block titletag %}{{view.get_header_title}}{% endblock %} {% block
 extra_css %} {{ block.super }} {{ form.media.css }}
 {% endblock %} {% block extra_js %}
 {% include "wagtailadmin/pages/_editor_js.html" %} {{ block.super }} {
 { form.media.js }} {% endblock %} {% block furniture %} {% block header %}
 ************ {{{{ vviieeww..ggeett__hheeaaddeerr__ttiittllee }}}} ************
 {% endblock %}
-{% block errors %} {% if form.errors or form.non_field_errors %}
-********** {{%% ttrraannssllaattee ""VVaalliiddaattiioonn eerrrroorrss"" %%}} **********
-    * {% for error in form.non_field_errors %}
-    * {{ error }}
-    * {% endfor %} {% for field, errors in form.errors.items %} {% for error in
-      errors %}
-    * {{ field }}: {{ error }}
-    * {% endfor %} {% endfor %}
-{% endif %} {% endblock %}
-% for k, v in form_attrs.items %}{{ k }}="{{ v|safe }}" {% endfor %}> {%
-csrf_token %}
-{% for field in form %} {% include "./field.html" %} {% endfor %}
+{% block content %}{% endblock %}
 {% block sidebar_logo %}{% endblock %}
 {% block sidebar %} {% if admin_edit_url %} _{_%_ _i_c_o_n_ _n_a_m_e_=_"_l_i_n_k_-_e_x_t_e_r_n_a_l_"_ _%_}_ {%
 endif %} {% icon name="circle-check" %} {% translate "Close" as close_title %}
 {% icon name="logout" title=close_title %} {% endblock %}
 {% endblock %}
```

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.0.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.0.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,33 +1,33 @@
 magic:    0xa70d0d0a
-moddate:  0xfdae0b66 (Tue Apr  2 07:08:45 2024 UTC)
-files sz: 13455
+moddate:  0x9b4f0c66 (Tue Apr  2 18:34:03 2024 UTC)
+files sz: 13337
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
       055a050100640064036c066d075a076d085a086d095a090100640064046c
       066d0a5a0a0100640064056c0b6d0c5a0c0100640064066c0d6d0e5a0e01
       00640064076c0f6d105a100100640064086c116d125a120100640064096c
       136d145a1401006400640a6c156d165a1601006400640b6c176d185a1801
       006400640c6c196d1a5a1a0100640d640e6c1b6d1c5a1c6d1d5a1d010064
-      0d640f6c1e6d1f5a1f0100640d64106c206d215a210100640d64116c186d
-      225a226d235a230100020065016a240000000000000000a6000000ab0000
-      000000000000005a25020065106a260000000000000000a6000000ab0000
-      000000000000005a27020047006412840064136502a6030000ab03000000
-      00000000005a286525a02900000000000000000000000000000000000000
-      006414ac15a6010000ab0100000000000000006416650764176508660464
-      188404a6000000ab0000000000000000005a2a6525a02b00000000000000
-      000000000000000000000000006419641aac1ba6020000ab020000000000
-      0000006424641d8401a6000000ab0000000000000000005a2c641e84005a
-      2d64166507641f652e652f190000000000000000006420652e652f190000
-      00000000000000642165306608642284045a31642384005a32641c5300
+      0d640f6c1e6d1f5a1f0100640d64106c186d205a206d215a210100020065
+      016a220000000000000000a6000000ab0000000000000000005a23020065
+      106a240000000000000000a6000000ab0000000000000000005a25020047
+      006411840064126502a6030000ab0300000000000000005a266523a02700
+      000000000000000000000000000000000000006413ac14a6010000ab0100
+      000000000000006415650764166508660464178404a6000000ab00000000
+      00000000005a286523a02900000000000000000000000000000000000000
+      0064186419ac1aa6020000ab0200000000000000006423641c8401a60000
+      00ab0000000000000000005a2a641d84005a2b64156507641e652c652d19
+      000000000000000000641f652c652d190000000000000000006420652e66
+      08642184045a2f642284005a30641b5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('library', 'Node', 'NodeList'))
                  6 IMPORT_NAME              0 (django.template)
                  8 IMPORT_FROM              1 (library)
                 10 STORE_NAME               1 (library)
@@ -124,123 +124,116 @@
                168 IMPORT_FROM             28 (FeditBlockEditButton)
                170 STORE_NAME              28 (FeditBlockEditButton)
                172 IMPORT_FROM             29 (FeditFieldEditButton)
                174 STORE_NAME              29 (FeditFieldEditButton)
                176 POP_TOP
    
     19         178 LOAD_CONST              13 (2)
-               180 LOAD_CONST              15 (('can_fedit',))
-               182 IMPORT_NAME             30 (block_forms.utils)
-               184 IMPORT_FROM             31 (can_fedit)
-               186 STORE_NAME              31 (can_fedit)
+               180 LOAD_CONST              15 (('FEDIT_PREVIEW_VAR',))
+               182 IMPORT_NAME             30 (utils)
+               184 IMPORT_FROM             31 (FEDIT_PREVIEW_VAR)
+               186 STORE_NAME              31 (FEDIT_PREVIEW_VAR)
                188 POP_TOP
    
     20         190 LOAD_CONST              13 (2)
-               192 LOAD_CONST              16 (('FEDIT_PREVIEW_VAR',))
-               194 IMPORT_NAME             32 (utils)
-               196 IMPORT_FROM             33 (FEDIT_PREVIEW_VAR)
-               198 STORE_NAME              33 (FEDIT_PREVIEW_VAR)
-               200 POP_TOP
-   
-    21         202 LOAD_CONST              13 (2)
-               204 LOAD_CONST              17 (('CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR'))
-               206 IMPORT_NAME             24 (hooks)
-               208 IMPORT_FROM             34 (CONSTRUCT_BLOCK_TOOLBAR)
-               210 STORE_NAME              34 (CONSTRUCT_BLOCK_TOOLBAR)
-               212 IMPORT_FROM             35 (CONSTRUCT_FIELD_TOOLBAR)
-               214 STORE_NAME              35 (CONSTRUCT_FIELD_TOOLBAR)
-               216 POP_TOP
-   
-    27         218 PUSH_NULL
-               220 LOAD_NAME                1 (library)
-               222 LOAD_ATTR               36 (Library)
-               232 PRECALL                  0
-               236 CALL                     0
-               246 STORE_NAME              37 (register)
-   
-    29         248 PUSH_NULL
-               250 LOAD_NAME               16 (signing)
-               252 LOAD_ATTR               38 (TimestampSigner)
-               262 PRECALL                  0
-               266 CALL                     0
-               276 STORE_NAME              39 (url_value_signer)
-   
-    32         278 PUSH_NULL
-               280 LOAD_BUILD_CLASS
-               282 LOAD_CONST              18 (<code object BlockEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 32>)
-               284 MAKE_FUNCTION            0
-               286 LOAD_CONST              19 ('BlockEditNode')
-               288 LOAD_NAME                2 (Node)
-               290 PRECALL                  3
-               294 CALL                     3
-               304 STORE_NAME              40 (BlockEditNode)
-   
-   220         306 LOAD_NAME               37 (register)
-               308 LOAD_METHOD             41 (tag)
-               330 LOAD_CONST              20 ('fedit_block')
-               332 KW_NAMES                21
-               334 PRECALL                  1
-               338 CALL                     1
-   
-   221         348 LOAD_CONST              22 ('parser')
-               350 LOAD_NAME                7 (Parser)
-               352 LOAD_CONST              23 ('token')
-               354 LOAD_NAME                8 (Token)
-               356 BUILD_TUPLE              4
-               358 LOAD_CONST              24 (<code object do_render_fedit_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 220>)
-               360 MAKE_FUNCTION            4 (annotations)
-   
-   220         362 PRECALL                  0
-               366 CALL                     0
-   
-   221         376 STORE_NAME              42 (do_render_fedit_block)
-   
-   282         378 LOAD_NAME               37 (register)
-               380 LOAD_METHOD             43 (simple_tag)
-               402 LOAD_CONST              25 (True)
-               404 LOAD_CONST              26 ('fedit_field')
-               406 KW_NAMES                27
-               408 PRECALL                  2
-               412 CALL                     2
-   
-   283         422 LOAD_CONST              36 ((None,))
-               424 LOAD_CONST              29 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 282>)
-               426 MAKE_FUNCTION            1 (defaults)
-   
-   282         428 PRECALL                  0
-               432 CALL                     0
-   
-   283         442 STORE_NAME              44 (do_render_fedit_field)
-   
-   338         444 LOAD_CONST              30 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 338>)
-               446 MAKE_FUNCTION            0
-               448 STORE_NAME              45 (render_editable_field)
-   
-   374         450 LOAD_CONST              22 ('parser')
-               452 LOAD_NAME                7 (Parser)
-               454 LOAD_CONST              31 ('kwarg_list')
-               456 LOAD_NAME               46 (list)
-               458 LOAD_NAME               47 (str)
-               460 BINARY_SUBSCR
-               470 LOAD_CONST              32 ('tokens')
-               472 LOAD_NAME               46 (list)
-               474 LOAD_NAME               47 (str)
-               476 BINARY_SUBSCR
-               486 LOAD_CONST              33 ('return')
-               488 LOAD_NAME               48 (dict)
-               490 BUILD_TUPLE              8
-               492 LOAD_CONST              34 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 374>)
-               494 MAKE_FUNCTION            4 (annotations)
-               496 STORE_NAME              49 (get_kwargs)
-   
-   401         498 LOAD_CONST              35 (<code object _get_from_context_or_set, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 401>)
-               500 MAKE_FUNCTION            0
-               502 STORE_NAME              50 (_get_from_context_or_set)
-               504 LOAD_CONST              28 (None)
-               506 RETURN_VALUE
+               192 LOAD_CONST              16 (('CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR'))
+               194 IMPORT_NAME             24 (hooks)
+               196 IMPORT_FROM             32 (CONSTRUCT_BLOCK_TOOLBAR)
+               198 STORE_NAME              32 (CONSTRUCT_BLOCK_TOOLBAR)
+               200 IMPORT_FROM             33 (CONSTRUCT_FIELD_TOOLBAR)
+               202 STORE_NAME              33 (CONSTRUCT_FIELD_TOOLBAR)
+               204 POP_TOP
+   
+    26         206 PUSH_NULL
+               208 LOAD_NAME                1 (library)
+               210 LOAD_ATTR               34 (Library)
+               220 PRECALL                  0
+               224 CALL                     0
+               234 STORE_NAME              35 (register)
+   
+    28         236 PUSH_NULL
+               238 LOAD_NAME               16 (signing)
+               240 LOAD_ATTR               36 (TimestampSigner)
+               250 PRECALL                  0
+               254 CALL                     0
+               264 STORE_NAME              37 (url_value_signer)
+   
+    31         266 PUSH_NULL
+               268 LOAD_BUILD_CLASS
+               270 LOAD_CONST              17 (<code object BlockEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 31>)
+               272 MAKE_FUNCTION            0
+               274 LOAD_CONST              18 ('BlockEditNode')
+               276 LOAD_NAME                2 (Node)
+               278 PRECALL                  3
+               282 CALL                     3
+               292 STORE_NAME              38 (BlockEditNode)
+   
+   216         294 LOAD_NAME               35 (register)
+               296 LOAD_METHOD             39 (tag)
+               318 LOAD_CONST              19 ('fedit_block')
+               320 KW_NAMES                20
+               322 PRECALL                  1
+               326 CALL                     1
+   
+   217         336 LOAD_CONST              21 ('parser')
+               338 LOAD_NAME                7 (Parser)
+               340 LOAD_CONST              22 ('token')
+               342 LOAD_NAME                8 (Token)
+               344 BUILD_TUPLE              4
+               346 LOAD_CONST              23 (<code object do_render_fedit_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 216>)
+               348 MAKE_FUNCTION            4 (annotations)
+   
+   216         350 PRECALL                  0
+               354 CALL                     0
+   
+   217         364 STORE_NAME              40 (do_render_fedit_block)
+   
+   278         366 LOAD_NAME               35 (register)
+               368 LOAD_METHOD             41 (simple_tag)
+               390 LOAD_CONST              24 (True)
+               392 LOAD_CONST              25 ('fedit_field')
+               394 KW_NAMES                26
+               396 PRECALL                  2
+               400 CALL                     2
+   
+   279         410 LOAD_CONST              35 ((None,))
+               412 LOAD_CONST              28 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 278>)
+               414 MAKE_FUNCTION            1 (defaults)
+   
+   278         416 PRECALL                  0
+               420 CALL                     0
+   
+   279         430 STORE_NAME              42 (do_render_fedit_field)
+   
+   334         432 LOAD_CONST              29 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 334>)
+               434 MAKE_FUNCTION            0
+               436 STORE_NAME              43 (render_editable_field)
+   
+   370         438 LOAD_CONST              21 ('parser')
+               440 LOAD_NAME                7 (Parser)
+               442 LOAD_CONST              30 ('kwarg_list')
+               444 LOAD_NAME               44 (list)
+               446 LOAD_NAME               45 (str)
+               448 BINARY_SUBSCR
+               458 LOAD_CONST              31 ('tokens')
+               460 LOAD_NAME               44 (list)
+               462 LOAD_NAME               45 (str)
+               464 BINARY_SUBSCR
+               474 LOAD_CONST              32 ('return')
+               476 LOAD_NAME               46 (dict)
+               478 BUILD_TUPLE              8
+               480 LOAD_CONST              33 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 370>)
+               482 MAKE_FUNCTION            4 (annotations)
+               484 STORE_NAME              47 (get_kwargs)
+   
+   397         486 LOAD_CONST              34 (<code object _get_from_context_or_set, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 397>)
+               488 MAKE_FUNCTION            0
+               490 STORE_NAME              48 (_get_from_context_or_set)
+               492 LOAD_CONST              27 (None)
+               494 RETURN_VALUE
    consts
       0
       ('library', 'Node', 'NodeList')
       ('render_to_string',)
       ('Parser', 'Token', 'TokenType')
       ('FilterExpression',)
       ('mark_safe',)
@@ -249,15 +242,14 @@
       ('models',)
       ('BoundBlock',)
       ('Page',)
       ('hooks',)
       ('urlencode',)
       2
       ('FeditBlockEditButton', 'FeditFieldEditButton')
-      ('can_fedit',)
       ('FEDIT_PREVIEW_VAR',)
       ('CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
          flags     : 0
@@ -266,149 +258,149 @@
             000000000000005a04090009000900090009006412640465056405650664
             06650764076507640865086a090000000000000000660a640984055a0a64
             0a84005a0b650c640b650d6602640c8404a6000000ab0000000000000000
             005a0e650f6403640d9c01640e6507640b650d6604640f8406a6000000ab
             0000000000000000005a10650c6406650764076507641065086a09000000
             0000000000640b6507660864118404a6000000ab0000000000000000005a
             1164035300
-          32           0 RESUME                   0
+          31           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BlockEditNode')
                        8 STORE_NAME               2 (__qualname__)
          
-          33          10 PUSH_NULL
+          32          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object UnpackError, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 33>)
+                      14 LOAD_CONST               1 (<code object UnpackError, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 32>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('UnpackError')
                       20 LOAD_NAME                3 (Exception)
                       22 PRECALL                  3
                       26 CALL                     3
                       36 STORE_NAME               4 (UnpackError)
          
-          37          38 NOP
+          36          38 NOP
          
-          38          40 NOP
+          37          40 NOP
          
-          39          42 NOP
+          38          42 NOP
          
-          40          44 NOP
+          39          44 NOP
          
-          41          46 NOP
+          40          46 NOP
          
-          36          48 LOAD_CONST              18 ((None, None, None, None, None))
+          35          48 LOAD_CONST              18 ((None, None, None, None, None))
                       50 LOAD_CONST               4 ('nodelist')
          
-          37          52 LOAD_NAME                5 (NodeList)
+          36          52 LOAD_NAME                5 (NodeList)
          
-          36          54 LOAD_CONST               5 ('block')
+          35          54 LOAD_CONST               5 ('block')
          
-          38          56 LOAD_NAME                6 (BoundBlock)
+          37          56 LOAD_NAME                6 (BoundBlock)
          
-          36          58 LOAD_CONST               6 ('block_id')
+          35          58 LOAD_CONST               6 ('block_id')
          
-          39          60 LOAD_NAME                7 (str)
+          38          60 LOAD_NAME                7 (str)
          
-          36          62 LOAD_CONST               7 ('field_name')
+          35          62 LOAD_CONST               7 ('field_name')
          
-          40          64 LOAD_NAME                7 (str)
+          39          64 LOAD_NAME                7 (str)
          
-          36          66 LOAD_CONST               8 ('model')
+          35          66 LOAD_CONST               8 ('model')
          
-          41          68 LOAD_NAME                8 (models)
+          40          68 LOAD_NAME                8 (models)
                       70 LOAD_ATTR                9 (Model)
          
-          36          80 BUILD_TUPLE             10
-                      82 LOAD_CONST               9 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 36>)
+          35          80 BUILD_TUPLE             10
+                      82 LOAD_CONST               9 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 35>)
                       84 MAKE_FUNCTION            5 (defaults, annotations)
                       86 STORE_NAME              10 (__init__)
          
-          52          88 LOAD_CONST              10 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 52>)
+          51          88 LOAD_CONST              10 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 51>)
                       90 MAKE_FUNCTION            0
                       92 STORE_NAME              11 (render)
          
-         171          94 LOAD_NAME               12 (staticmethod)
+         167          94 LOAD_NAME               12 (staticmethod)
          
-         172          96 LOAD_CONST              11 ('return')
+         168          96 LOAD_CONST              11 ('return')
                       98 LOAD_NAME               13 (dict)
                      100 BUILD_TUPLE              2
-                     102 LOAD_CONST              12 (<code object pack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 171>)
+                     102 LOAD_CONST              12 (<code object pack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 167>)
                      104 MAKE_FUNCTION            4 (annotations)
          
-         171         106 PRECALL                  0
+         167         106 PRECALL                  0
                      110 CALL                     0
          
-         172         120 STORE_NAME              14 (pack)
+         168         120 STORE_NAME              14 (pack)
          
-         180         122 LOAD_NAME               15 (classmethod)
+         176         122 LOAD_NAME               15 (classmethod)
          
-         181         124 LOAD_CONST               3 (None)
+         177         124 LOAD_CONST               3 (None)
                      126 LOAD_CONST              13 (('request',))
                      128 BUILD_CONST_KEY_MAP      1
                      130 LOAD_CONST              14 ('expected')
                      132 LOAD_NAME                7 (str)
                      134 LOAD_CONST              11 ('return')
                      136 LOAD_NAME               13 (dict)
                      138 BUILD_TUPLE              4
-                     140 LOAD_CONST              15 (<code object unpack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 180>)
+                     140 LOAD_CONST              15 (<code object unpack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 176>)
                      142 MAKE_FUNCTION            6 (kwdefaults, annotations)
          
-         180         144 PRECALL                  0
+         176         144 PRECALL                  0
                      148 CALL                     0
          
-         181         158 STORE_NAME              16 (unpack)
+         177         158 STORE_NAME              16 (unpack)
          
-         203         160 LOAD_NAME               12 (staticmethod)
+         199         160 LOAD_NAME               12 (staticmethod)
          
-         204         162 LOAD_CONST               6 ('block_id')
+         200         162 LOAD_CONST               6 ('block_id')
                      164 LOAD_NAME                7 (str)
                      166 LOAD_CONST               7 ('field_name')
                      168 LOAD_NAME                7 (str)
                      170 LOAD_CONST              16 ('instance')
                      172 LOAD_NAME                8 (models)
                      174 LOAD_ATTR                9 (Model)
                      184 LOAD_CONST              11 ('return')
                      186 LOAD_NAME                7 (str)
                      188 BUILD_TUPLE              8
-                     190 LOAD_CONST              17 (<code object get_edit_url, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 203>)
+                     190 LOAD_CONST              17 (<code object get_edit_url, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 199>)
                      192 MAKE_FUNCTION            4 (annotations)
          
-         203         194 PRECALL                  0
+         199         194 PRECALL                  0
                      198 CALL                     0
          
-         204         208 STORE_NAME              17 (get_edit_url)
+         200         208 STORE_NAME              17 (get_edit_url)
                      210 LOAD_CONST               3 (None)
                      212 RETURN_VALUE
          consts
             'BlockEditNode'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015300
-                33           0 RESUME                   0
+                32           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('BlockEditNode.UnpackError')
                              8 STORE_NAME               2 (__qualname__)
                
-                34          10 LOAD_CONST               1 (None)
+                33          10 LOAD_CONST               1 (None)
                             12 RETURN_VALUE
                consts
                   'BlockEditNode.UnpackError'
                   None
                names      ('__name__', '__module__', '__qualname__')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'UnpackError'
-               firstlineno 33
+               firstlineno 32
                lnotab 0x0a01
             'UnpackError'
             None
             'nodelist'
             'block'
             'block_id'
             'field_name'
@@ -419,50 +411,50 @@
                stacksize : 2
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   007c037c005f0200000000000000007c047c005f0300000000000000007c
                   057c005f0400000000000000007c067c005f050000000000000000640053
                   00
-                36           0 RESUME                   0
+                35           0 RESUME                   0
                
-                45           2 LOAD_FAST                1 (nodelist)
+                44           2 LOAD_FAST                1 (nodelist)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (nl)
                
-                46          16 LOAD_FAST                2 (block)
+                45          16 LOAD_FAST                2 (block)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (block)
                
-                47          30 LOAD_FAST                3 (block_id)
+                46          30 LOAD_FAST                3 (block_id)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (block_id)
                
-                48          44 LOAD_FAST                4 (field_name)
+                47          44 LOAD_FAST                4 (field_name)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (field_name)
                
-                49          58 LOAD_FAST                5 (model)
+                48          58 LOAD_FAST                5 (model)
                             60 LOAD_FAST                0 (self)
                             62 STORE_ATTR               4 (model)
                
-                50          72 LOAD_FAST                6 (extra)
+                49          72 LOAD_FAST                6 (extra)
                             74 LOAD_FAST                0 (self)
                             76 STORE_ATTR               5 (extra)
                             86 LOAD_CONST               0 (None)
                             88 RETURN_VALUE
                consts
                   None
                names      ('nl', 'block', 'block_id', 'field_name', 'model', 'extra')
                varnames   ('self', 'nodelist', 'block', 'block_id', 'field_name', 'model', 'extra')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 36
+               firstlineno 35
                lnotab 0x02090e010e010e010e010e01
             code
                argcount  : 2
                nlocals   : 12
                stacksize : 12
                flags     : 3
                code
@@ -495,509 +487,497 @@
                   007c05a6010000ab01000000000000000001007c02a00d00000000000000
                   000000000000000000000000007c01a6010000ab0100000000000000007d
                   0864067c005f0e00000000000000006e4c7c006a0f000000000000000072
                   367c006a0f0000000000000000a010000000000000000000000000000000
                   00000000007c01a6010000ab0100000000000000007d087c01a011000000
                   000000000000000000000000000000000064076408a6020000ab02000000
                   00000000007c005f0e00000000000000006e0f7413000000000000000000
-                  006409a6010000ab01000000000000000082017c02721174250000000000
-                  00000000007c02a6010000ab01000000000000000073027c0853007c0373
-                  0d64027c01760072097c016402190000000000000000007d036e2d7c0373
-                  1a7c0272187427000000000000000000007c02640aa6020000ab02000000
-                  000000000072087c026a1400000000000000007d036e117c03730f741300
-                  0000000000000000006403a6010000ab0100000000000000008201890c70
-                  077c016404190000000000000000008a0c7c01a011000000000000000000
-                  0000000000000000000000640ba6010000ab0100000000000000008a0d89
-                  0d7271890d6a1500000000000000006a1600000000000000007263890d6a
-                  150000000000000000a01700000000000000000000000000000000000000
-                  00640ca6010000ab0100000000000000007249890d6a1500000000000000
-                  00a0170000000000000000000000000000000000000000890c6a18000000
-                  00000000006a1900000000000000009b00640d890c6a1800000000000000
-                  006a1a00000000000000009b009d03a6010000ab01000000000000000072
-                  16743700000000000000000000890d7438000000000000000000006408a6
-                  030000ab03000000000000000073027c085300740d000000000000000000
-                  00890c743a00000000000000000000a6020000ab02000000000000000072
-                  1d743d000000000000000000007c01640e880c6601640f8408a6030000ab
-                  0300000000000000007d097c099b0064107c039b0064119d047d096e0264
-                  007d097c05a01f000000000000000000000000000000000000000064127c
-                  006a0e0000000000000000a6020000ab0200000000000000000100744100
-                  000000000000000000a6000000ab00000000000000000067017d0a744300
-                  0000000000000000006a2200000000000000007446000000000000000000
-                  00a6010000ab01000000000000000044005d127d0b02007c0b890d7c0a89
-                  0c7c037c04ac13a6050000ab05000000000000000001008c13880d660164
-                  1484087c0a4400a6000000ab0000000000000000007d0a74490000000000
-                  0000000000744b0000000000000000000064007c0aa6020000ab02000000
-                  0000000000a6010000ab0100000000000000007d0a744d00000000000000
-                  000000641502007c006a2700000000000000007c037c0466026416890c69
-                  017c05a4018e017c097c03890c7c087c047c017c0a64179c08a6020000ab
-                  0200000000000000005300
+                  006409a6010000ab01000000000000000082017c03730d64027c01760072
+                  097c016402190000000000000000007d036e2d7c03731a7c027218742500
+                  0000000000000000007c02640aa6020000ab02000000000000000072087c
+                  026a1300000000000000007d036e117c03730f7413000000000000000000
+                  006403a6010000ab0100000000000000008201890c70077c016404190000
+                  000000000000008a0c7c01a0110000000000000000000000000000000000
+                  000000640ba6010000ab0100000000000000008a0d890d7271890d6a1400
+                  000000000000006a1500000000000000007263890d6a1400000000000000
+                  00a0160000000000000000000000000000000000000000640ca6010000ab
+                  0100000000000000007249890d6a140000000000000000a0160000000000
+                  000000000000000000000000000000890c6a1700000000000000006a1800
+                  000000000000009b00640d890c6a1700000000000000006a190000000000
+                  0000009b009d03a6010000ab010000000000000000721674350000000000
+                  0000000000890d7436000000000000000000006408a6030000ab03000000
+                  000000000073027c085300740d00000000000000000000890c7438000000
+                  00000000000000a6020000ab020000000000000000721d743b0000000000
+                  00000000007c01640e880c6601640f8408a6030000ab0300000000000000
+                  007d097c099b0064107c039b0064119d047d096e0264007d097c05a01e00
+                  0000000000000000000000000000000000000064127c006a0e0000000000
+                  000000a6020000ab0200000000000000000100743f000000000000000000
+                  00a6000000ab00000000000000000067017d0a7441000000000000000000
+                  006a210000000000000000744400000000000000000000a6010000ab0100
+                  0000000000000044005d127d0b02007c0b890d7c0a890c7c037c04ac13a6
+                  050000ab05000000000000000001008c13880d6601641484087c0a4400a6
+                  000000ab0000000000000000007d0a744700000000000000000000744900
+                  00000000000000000064007c0aa6020000ab020000000000000000a60100
+                  00ab0100000000000000007d0a744b00000000000000000000641502007c
+                  006a2600000000000000007c037c0466026416890c69017c05a4018e017c
+                  097c03890c7c087c047c017c0a64179c08a6020000ab0200000000000000
+                  005300
                              0 MAKE_CELL               12 (model)
                              2 MAKE_CELL               13 (request)
                
-                52           4 RESUME                   0
+                51           4 RESUME                   0
                
-                53           6 LOAD_FAST                0 (self)
+                52           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (block)
                             18 STORE_FAST               2 (block)
                
-                54          20 LOAD_FAST                0 (self)
+                53          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                1 (block_id)
                             32 STORE_FAST               3 (block_id)
                
-                55          34 LOAD_FAST                0 (self)
+                54          34 LOAD_FAST                0 (self)
                             36 LOAD_ATTR                2 (field_name)
                             46 STORE_FAST               4 (field_name)
                
-                56          48 LOAD_FAST                0 (self)
+                55          48 LOAD_FAST                0 (self)
                             50 LOAD_ATTR                3 (model)
                             60 STORE_DEREF             12 (model)
                
-                57          62 LOAD_FAST                0 (self)
+                56          62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                4 (extra)
                             74 STORE_FAST               5 (extra)
                
-                60          76 LOAD_FAST                5 (extra)
+                59          76 LOAD_FAST                5 (extra)
                             78 LOAD_METHOD              5 (items)
                            100 PRECALL                  0
                            104 CALL                     0
                            114 GET_ITER
                        >>  116 FOR_ITER                50 (to 218)
                            118 UNPACK_SEQUENCE          2
                            122 STORE_FAST               6 (k)
                            124 STORE_FAST               7 (e)
                
-                61         126 LOAD_GLOBAL             13 (NULL + isinstance)
+                60         126 LOAD_GLOBAL             13 (NULL + isinstance)
                            138 LOAD_FAST                7 (e)
                            140 LOAD_GLOBAL             14 (FilterExpression)
                            152 PRECALL                  2
                            156 CALL                     2
                            166 POP_JUMP_FORWARD_IF_FALSE    24 (to 216)
                
-                62         168 LOAD_FAST                7 (e)
+                61         168 LOAD_FAST                7 (e)
                            170 LOAD_METHOD              8 (resolve)
                            192 LOAD_FAST                1 (context)
                            194 PRECALL                  1
                            198 CALL                     1
                            208 LOAD_FAST                5 (extra)
                            210 LOAD_FAST                6 (k)
                            212 STORE_SUBSCR
                        >>  216 JUMP_BACKWARD           51 (to 116)
                
-                64     >>  218 LOAD_GLOBAL             13 (NULL + isinstance)
+                63     >>  218 LOAD_GLOBAL             13 (NULL + isinstance)
                            230 LOAD_FAST                2 (block)
                            232 LOAD_GLOBAL             14 (FilterExpression)
                            244 PRECALL                  2
                            248 CALL                     2
                            258 POP_JUMP_FORWARD_IF_FALSE    21 (to 302)
                
-                65         260 LOAD_FAST                2 (block)
+                64         260 LOAD_FAST                2 (block)
                            262 LOAD_METHOD              8 (resolve)
                            284 LOAD_FAST                1 (context)
                            286 PRECALL                  1
                            290 CALL                     1
                            300 STORE_FAST               2 (block)
                
-                66     >>  302 LOAD_GLOBAL             13 (NULL + isinstance)
+                65     >>  302 LOAD_GLOBAL             13 (NULL + isinstance)
                            314 LOAD_FAST                3 (block_id)
                            316 LOAD_GLOBAL             14 (FilterExpression)
                            328 PRECALL                  2
                            332 CALL                     2
                            342 POP_JUMP_FORWARD_IF_FALSE    21 (to 386)
                
-                67         344 LOAD_FAST                3 (block_id)
+                66         344 LOAD_FAST                3 (block_id)
                            346 LOAD_METHOD              8 (resolve)
                            368 LOAD_FAST                1 (context)
                            370 PRECALL                  1
                            374 CALL                     1
                            384 STORE_FAST               3 (block_id)
                
-                68     >>  386 LOAD_GLOBAL             13 (NULL + isinstance)
+                67     >>  386 LOAD_GLOBAL             13 (NULL + isinstance)
                            398 LOAD_FAST                4 (field_name)
                            400 LOAD_GLOBAL             14 (FilterExpression)
                            412 PRECALL                  2
                            416 CALL                     2
                            426 POP_JUMP_FORWARD_IF_FALSE    21 (to 470)
                
-                69         428 LOAD_FAST                4 (field_name)
+                68         428 LOAD_FAST                4 (field_name)
                            430 LOAD_METHOD              8 (resolve)
                            452 LOAD_FAST                1 (context)
                            454 PRECALL                  1
                            458 CALL                     1
                            468 STORE_FAST               4 (field_name)
                
-                70     >>  470 LOAD_GLOBAL             13 (NULL + isinstance)
+                69     >>  470 LOAD_GLOBAL             13 (NULL + isinstance)
                            482 LOAD_DEREF              12 (model)
                            484 LOAD_GLOBAL             14 (FilterExpression)
                            496 PRECALL                  2
                            500 CALL                     2
                            510 POP_JUMP_FORWARD_IF_FALSE    21 (to 554)
                
-                71         512 LOAD_DEREF              12 (model)
+                70         512 LOAD_DEREF              12 (model)
                            514 LOAD_METHOD              8 (resolve)
                            536 LOAD_FAST                1 (context)
                            538 PRECALL                  1
                            542 CALL                     1
                            552 STORE_DEREF             12 (model)
                
-                74     >>  554 LOAD_FAST                4 (field_name)
+                73     >>  554 LOAD_FAST                4 (field_name)
                            556 POP_JUMP_FORWARD_IF_TRUE    15 (to 588)
                
-                75         558 LOAD_GLOBAL             19 (NULL + ValueError)
+                74         558 LOAD_GLOBAL             19 (NULL + ValueError)
                            570 LOAD_CONST               1 ('Field name is required')
                            572 PRECALL                  1
                            576 CALL                     1
                            586 RAISE_VARARGS            1
                
-                77     >>  588 LOAD_FAST                3 (block_id)
+                76     >>  588 LOAD_FAST                3 (block_id)
                            590 POP_JUMP_FORWARD_IF_TRUE    21 (to 634)
                            592 LOAD_CONST               2 ('block_id')
                            594 LOAD_FAST                1 (context)
                            596 CONTAINS_OP              1
                            598 POP_JUMP_FORWARD_IF_FALSE    17 (to 634)
                            600 LOAD_FAST                2 (block)
                            602 POP_JUMP_FORWARD_IF_TRUE    15 (to 634)
                
-                78         604 LOAD_GLOBAL             19 (NULL + ValueError)
+                77         604 LOAD_GLOBAL             19 (NULL + ValueError)
                            616 LOAD_CONST               3 ('Block ID is required')
                            618 PRECALL                  1
                            622 CALL                     1
                            632 RAISE_VARARGS            1
                
-                80     >>  634 LOAD_DEREF              12 (model)
+                79     >>  634 LOAD_DEREF              12 (model)
                            636 POP_JUMP_FORWARD_IF_TRUE    19 (to 676)
                            638 LOAD_CONST               4 ('wagtail_fedit_instance')
                            640 LOAD_FAST                1 (context)
                            642 CONTAINS_OP              1
                            644 POP_JUMP_FORWARD_IF_FALSE    15 (to 676)
                
-                81         646 LOAD_GLOBAL             19 (NULL + ValueError)
+                80         646 LOAD_GLOBAL             19 (NULL + ValueError)
                            658 LOAD_CONST               5 ('Model instance is required')
                            660 PRECALL                  1
                            664 CALL                     1
                            674 RAISE_VARARGS            1
                
-                85     >>  676 LOAD_FAST                2 (block)
+                84     >>  676 LOAD_FAST                2 (block)
                            678 POP_JUMP_FORWARD_IF_FALSE    88 (to 856)
                
-                86         680 NOP
+                85         680 NOP
                
-                87         682 LOAD_FAST                1 (context)
+                86         682 LOAD_FAST                1 (context)
                            684 LOAD_METHOD             10 (flatten)
                            706 PRECALL                  0
                            710 CALL                     0
                            720 STORE_FAST               1 (context)
                            722 JUMP_FORWARD            16 (to 756)
                        >>  724 PUSH_EXC_INFO
                
-                88         726 LOAD_GLOBAL             22 (AttributeError)
+                87         726 LOAD_GLOBAL             22 (AttributeError)
                            738 CHECK_EXC_MATCH
                            740 POP_JUMP_FORWARD_IF_FALSE     3 (to 748)
                            742 POP_TOP
                
-                89         744 POP_EXCEPT
+                88         744 POP_EXCEPT
                            746 JUMP_FORWARD             4 (to 756)
                
-                88     >>  748 RERAISE                  0
+                87     >>  748 RERAISE                  0
                        >>  750 COPY                     3
                            752 POP_EXCEPT
                            754 RERAISE                  1
                
-                90     >>  756 LOAD_FAST                1 (context)
+                89     >>  756 LOAD_FAST                1 (context)
                            758 LOAD_METHOD             12 (update)
                            780 LOAD_FAST                5 (extra)
                            782 PRECALL                  1
                            786 CALL                     1
                            796 POP_TOP
                
-                91         798 LOAD_FAST                2 (block)
+                90         798 LOAD_FAST                2 (block)
                            800 LOAD_METHOD             13 (render_as_block)
                            822 LOAD_FAST                1 (context)
                            824 PRECALL                  1
                            828 CALL                     1
                            838 STORE_FAST               8 (rendered)
                
-                92         840 LOAD_CONST               6 (True)
+                91         840 LOAD_CONST               6 (True)
                            842 LOAD_FAST                0 (self)
                            844 STORE_ATTR              14 (has_block)
                            854 JUMP_FORWARD            76 (to 1008)
                
-                93     >>  856 LOAD_FAST                0 (self)
+                92     >>  856 LOAD_FAST                0 (self)
                            858 LOAD_ATTR               15 (nl)
                            868 POP_JUMP_FORWARD_IF_FALSE    54 (to 978)
                
-                94         870 LOAD_FAST                0 (self)
+                93         870 LOAD_FAST                0 (self)
                            872 LOAD_ATTR               15 (nl)
                            882 LOAD_METHOD             16 (render)
                            904 LOAD_FAST                1 (context)
                            906 PRECALL                  1
                            910 CALL                     1
                            920 STORE_FAST               8 (rendered)
                
-                95         922 LOAD_FAST                1 (context)
+                94         922 LOAD_FAST                1 (context)
                            924 LOAD_METHOD             17 (get)
                            946 LOAD_CONST               7 ('wagtail_fedit_has_block')
                            948 LOAD_CONST               8 (False)
                            950 PRECALL                  2
                            954 CALL                     2
                            964 LOAD_FAST                0 (self)
                            966 STORE_ATTR              14 (has_block)
                            976 JUMP_FORWARD            15 (to 1008)
                
-                97     >>  978 LOAD_GLOBAL             19 (NULL + ValueError)
+                96     >>  978 LOAD_GLOBAL             19 (NULL + ValueError)
                            990 LOAD_CONST               9 ('Block or nodelist is required')
                            992 PRECALL                  1
                            996 CALL                     1
                           1006 RAISE_VARARGS            1
                
-                99     >> 1008 LOAD_FAST                2 (block)
-                          1010 POP_JUMP_FORWARD_IF_FALSE    17 (to 1046)
-                          1012 LOAD_GLOBAL             37 (NULL + can_fedit)
-                          1024 LOAD_FAST                2 (block)
-                          1026 PRECALL                  1
-                          1030 CALL                     1
-                          1040 POP_JUMP_FORWARD_IF_TRUE     2 (to 1046)
-               
-               100        1042 LOAD_FAST                8 (rendered)
-                          1044 RETURN_VALUE
-               
-               103     >> 1046 LOAD_FAST                3 (block_id)
-                          1048 POP_JUMP_FORWARD_IF_TRUE    13 (to 1076)
-                          1050 LOAD_CONST               2 ('block_id')
-                          1052 LOAD_FAST                1 (context)
-                          1054 CONTAINS_OP              0
-                          1056 POP_JUMP_FORWARD_IF_FALSE     9 (to 1076)
-               
-               104        1058 LOAD_FAST                1 (context)
-                          1060 LOAD_CONST               2 ('block_id')
-                          1062 BINARY_SUBSCR
-                          1072 STORE_FAST               3 (block_id)
-                          1074 JUMP_FORWARD            45 (to 1166)
-               
-               105     >> 1076 LOAD_FAST                3 (block_id)
-                          1078 POP_JUMP_FORWARD_IF_TRUE    26 (to 1132)
-                          1080 LOAD_FAST                2 (block)
-                          1082 POP_JUMP_FORWARD_IF_FALSE    24 (to 1132)
-                          1084 LOAD_GLOBAL             39 (NULL + hasattr)
-                          1096 LOAD_FAST                2 (block)
-                          1098 LOAD_CONST              10 ('id')
-                          1100 PRECALL                  2
-                          1104 CALL                     2
-                          1114 POP_JUMP_FORWARD_IF_FALSE     8 (to 1132)
-               
-               106        1116 LOAD_FAST                2 (block)
-                          1118 LOAD_ATTR               20 (id)
-                          1128 STORE_FAST               3 (block_id)
-                          1130 JUMP_FORWARD            17 (to 1166)
-               
-               107     >> 1132 LOAD_FAST                3 (block_id)
-                          1134 POP_JUMP_FORWARD_IF_TRUE    15 (to 1166)
-               
-               108        1136 LOAD_GLOBAL             19 (NULL + ValueError)
-                          1148 LOAD_CONST               3 ('Block ID is required')
-                          1150 PRECALL                  1
-                          1154 CALL                     1
-                          1164 RAISE_VARARGS            1
-               
-               113     >> 1166 LOAD_DEREF              12 (model)
-                          1168 JUMP_IF_TRUE_OR_POP      7 (to 1184)
-                          1170 LOAD_FAST                1 (context)
-                          1172 LOAD_CONST               4 ('wagtail_fedit_instance')
-                          1174 BINARY_SUBSCR
-                       >> 1184 STORE_DEREF             12 (model)
-               
-               116        1186 LOAD_FAST                1 (context)
-                          1188 LOAD_METHOD             17 (get)
-                          1210 LOAD_CONST              11 ('request')
-                          1212 PRECALL                  1
-                          1216 CALL                     1
-                          1226 STORE_DEREF             13 (request)
-               
-               117        1228 LOAD_DEREF              13 (request)
-                          1230 POP_JUMP_FORWARD_IF_FALSE   113 (to 1458)
-               
-               119        1232 LOAD_DEREF              13 (request)
-                          1234 LOAD_ATTR               21 (user)
-                          1244 LOAD_ATTR               22 (is_authenticated)
-               
-               118        1254 POP_JUMP_FORWARD_IF_FALSE    99 (to 1454)
-               
-               120        1256 LOAD_DEREF              13 (request)
-                          1258 LOAD_ATTR               21 (user)
-                          1268 LOAD_METHOD             23 (has_perm)
-                          1290 LOAD_CONST              12 ('wagtailadmin.access_admin')
-                          1292 PRECALL                  1
-                          1296 CALL                     1
-               
-               118        1306 POP_JUMP_FORWARD_IF_FALSE    73 (to 1454)
-               
-               121        1308 LOAD_DEREF              13 (request)
-                          1310 LOAD_ATTR               21 (user)
-                          1320 LOAD_METHOD             23 (has_perm)
-                          1342 LOAD_DEREF              12 (model)
-                          1344 LOAD_ATTR               24 (_meta)
-                          1354 LOAD_ATTR               25 (app_label)
-                          1364 FORMAT_VALUE             0
-                          1366 LOAD_CONST              13 ('.change_')
-                          1368 LOAD_DEREF              12 (model)
-                          1370 LOAD_ATTR               24 (_meta)
-                          1380 LOAD_ATTR               26 (model_name)
-                          1390 FORMAT_VALUE             0
-                          1392 BUILD_STRING             3
-                          1394 PRECALL                  1
-                          1398 CALL                     1
-               
-               118        1408 POP_JUMP_FORWARD_IF_FALSE    22 (to 1454)
-               
-               122        1410 LOAD_GLOBAL             55 (NULL + getattr)
-                          1422 LOAD_DEREF              13 (request)
-                          1424 LOAD_GLOBAL             56 (FEDIT_PREVIEW_VAR)
-                          1436 LOAD_CONST               8 (False)
-                          1438 PRECALL                  3
-                          1442 CALL                     3
-               
-               118        1452 POP_JUMP_FORWARD_IF_TRUE     2 (to 1458)
-               
-               125     >> 1454 LOAD_FAST                8 (rendered)
-                          1456 RETURN_VALUE
-               
-               129     >> 1458 LOAD_GLOBAL             13 (NULL + isinstance)
-                          1470 LOAD_DEREF              12 (model)
-                          1472 LOAD_GLOBAL             58 (Page)
-                          1484 PRECALL                  2
-                          1488 CALL                     2
-                          1498 POP_JUMP_FORWARD_IF_FALSE    29 (to 1558)
-               
-               130        1500 LOAD_GLOBAL             61 (NULL + _get_from_context_or_set)
-               
-               131        1512 LOAD_FAST                1 (context)
-                          1514 LOAD_CONST              14 ('page_base_edit_url')
-               
-               132        1516 LOAD_CLOSURE            12 (model)
-                          1518 BUILD_TUPLE              1
-                          1520 LOAD_CONST              15 (<code object <lambda>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 132>)
-                          1522 MAKE_FUNCTION            8 (closure)
-               
-               130        1524 PRECALL                  3
-                          1528 CALL                     3
-                          1538 STORE_FAST               9 (admin_edit_url)
-               
-               137        1540 LOAD_FAST                9 (admin_edit_url)
-                          1542 FORMAT_VALUE             0
-                          1544 LOAD_CONST              16 ('#block-')
-                          1546 LOAD_FAST                3 (block_id)
-                          1548 FORMAT_VALUE             0
-                          1550 LOAD_CONST              17 ('-section')
-                          1552 BUILD_STRING             4
-                          1554 STORE_FAST               9 (admin_edit_url)
-                          1556 JUMP_FORWARD             2 (to 1562)
-               
-               139     >> 1558 LOAD_CONST               0 (None)
-                          1560 STORE_FAST               9 (admin_edit_url)
-               
-               141     >> 1562 LOAD_FAST                5 (extra)
-                          1564 LOAD_METHOD             31 (setdefault)
-                          1586 LOAD_CONST              18 ('has_block')
-                          1588 LOAD_FAST                0 (self)
-                          1590 LOAD_ATTR               14 (has_block)
-                          1600 PRECALL                  2
-                          1604 CALL                     2
-                          1614 POP_TOP
-               
-               144        1616 LOAD_GLOBAL             65 (NULL + FeditBlockEditButton)
-                          1628 PRECALL                  0
-                          1632 CALL                     0
-               
-               143        1642 BUILD_LIST               1
-                          1644 STORE_FAST              10 (items)
-               
-               147        1646 LOAD_GLOBAL             67 (NULL + hooks)
-                          1658 LOAD_ATTR               34 (get_hooks)
-                          1668 LOAD_GLOBAL             70 (CONSTRUCT_BLOCK_TOOLBAR)
-                          1680 PRECALL                  1
-                          1684 CALL                     1
-                          1694 GET_ITER
-                       >> 1696 FOR_ITER                18 (to 1734)
-                          1698 STORE_FAST              11 (hook)
-               
-               148        1700 PUSH_NULL
-                          1702 LOAD_FAST               11 (hook)
-                          1704 LOAD_DEREF              13 (request)
-                          1706 LOAD_FAST               10 (items)
-                          1708 LOAD_DEREF              12 (model)
-                          1710 LOAD_FAST                3 (block_id)
-                          1712 LOAD_FAST                4 (field_name)
-                          1714 KW_NAMES                19
-                          1716 PRECALL                  5
-                          1720 CALL                     5
-                          1730 POP_TOP
-                          1732 JUMP_BACKWARD           19 (to 1696)
-               
-               150     >> 1734 LOAD_CLOSURE            13 (request)
-                          1736 BUILD_TUPLE              1
-                          1738 LOAD_CONST              20 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 150>)
-                          1740 MAKE_FUNCTION            8 (closure)
-                          1742 LOAD_FAST               10 (items)
-                          1744 GET_ITER
-                          1746 PRECALL                  0
-                          1750 CALL                     0
-                          1760 STORE_FAST              10 (items)
-               
-               151        1762 LOAD_GLOBAL             73 (NULL + list)
-                          1774 LOAD_GLOBAL             75 (NULL + filter)
-                          1786 LOAD_CONST               0 (None)
-                          1788 LOAD_FAST               10 (items)
-                          1790 PRECALL                  2
-                          1794 CALL                     2
-                          1804 PRECALL                  1
-                          1808 CALL                     1
-                          1818 STORE_FAST              10 (items)
-               
-               153        1820 LOAD_GLOBAL             77 (NULL + render_to_string)
-               
-               154        1832 LOAD_CONST              21 ('wagtail_fedit/content/editable_block.html')
-               
-               156        1834 PUSH_NULL
-                          1836 LOAD_FAST                0 (self)
-                          1838 LOAD_ATTR               39 (get_edit_url)
-               
-               157        1848 LOAD_FAST                3 (block_id)
-                          1850 LOAD_FAST                4 (field_name)
-               
-               156        1852 BUILD_TUPLE              2
-                          1854 LOAD_CONST              22 ('instance')
-               
-               158        1856 LOAD_DEREF              12 (model)
-               
-               156        1858 BUILD_MAP                1
-               
-               159        1860 LOAD_FAST                5 (extra)
-               
-               156        1862 DICT_MERGE               1
-                          1864 CALL_FUNCTION_EX         1
-               
-               161        1866 LOAD_FAST                9 (admin_edit_url)
-               
-               162        1868 LOAD_FAST                3 (block_id)
-               
-               163        1870 LOAD_DEREF              12 (model)
-               
-               164        1872 LOAD_FAST                8 (rendered)
-               
-               165        1874 LOAD_FAST                4 (field_name)
-               
-               166        1876 LOAD_FAST                1 (context)
-               
-               167        1878 LOAD_FAST               10 (items)
-               
-               155        1880 LOAD_CONST              23 (('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'toolbar_items'))
-                          1882 BUILD_CONST_KEY_MAP      8
-               
-               153        1884 PRECALL                  2
-                          1888 CALL                     2
-                          1898 RETURN_VALUE
+                99     >> 1008 LOAD_FAST                3 (block_id)
+                          1010 POP_JUMP_FORWARD_IF_TRUE    13 (to 1038)
+                          1012 LOAD_CONST               2 ('block_id')
+                          1014 LOAD_FAST                1 (context)
+                          1016 CONTAINS_OP              0
+                          1018 POP_JUMP_FORWARD_IF_FALSE     9 (to 1038)
+               
+               100        1020 LOAD_FAST                1 (context)
+                          1022 LOAD_CONST               2 ('block_id')
+                          1024 BINARY_SUBSCR
+                          1034 STORE_FAST               3 (block_id)
+                          1036 JUMP_FORWARD            45 (to 1128)
+               
+               101     >> 1038 LOAD_FAST                3 (block_id)
+                          1040 POP_JUMP_FORWARD_IF_TRUE    26 (to 1094)
+                          1042 LOAD_FAST                2 (block)
+                          1044 POP_JUMP_FORWARD_IF_FALSE    24 (to 1094)
+                          1046 LOAD_GLOBAL             37 (NULL + hasattr)
+                          1058 LOAD_FAST                2 (block)
+                          1060 LOAD_CONST              10 ('id')
+                          1062 PRECALL                  2
+                          1066 CALL                     2
+                          1076 POP_JUMP_FORWARD_IF_FALSE     8 (to 1094)
+               
+               102        1078 LOAD_FAST                2 (block)
+                          1080 LOAD_ATTR               19 (id)
+                          1090 STORE_FAST               3 (block_id)
+                          1092 JUMP_FORWARD            17 (to 1128)
+               
+               103     >> 1094 LOAD_FAST                3 (block_id)
+                          1096 POP_JUMP_FORWARD_IF_TRUE    15 (to 1128)
+               
+               104        1098 LOAD_GLOBAL             19 (NULL + ValueError)
+                          1110 LOAD_CONST               3 ('Block ID is required')
+                          1112 PRECALL                  1
+                          1116 CALL                     1
+                          1126 RAISE_VARARGS            1
+               
+               109     >> 1128 LOAD_DEREF              12 (model)
+                          1130 JUMP_IF_TRUE_OR_POP      7 (to 1146)
+                          1132 LOAD_FAST                1 (context)
+                          1134 LOAD_CONST               4 ('wagtail_fedit_instance')
+                          1136 BINARY_SUBSCR
+                       >> 1146 STORE_DEREF             12 (model)
+               
+               112        1148 LOAD_FAST                1 (context)
+                          1150 LOAD_METHOD             17 (get)
+                          1172 LOAD_CONST              11 ('request')
+                          1174 PRECALL                  1
+                          1178 CALL                     1
+                          1188 STORE_DEREF             13 (request)
+               
+               113        1190 LOAD_DEREF              13 (request)
+                          1192 POP_JUMP_FORWARD_IF_FALSE   113 (to 1420)
+               
+               115        1194 LOAD_DEREF              13 (request)
+                          1196 LOAD_ATTR               20 (user)
+                          1206 LOAD_ATTR               21 (is_authenticated)
+               
+               114        1216 POP_JUMP_FORWARD_IF_FALSE    99 (to 1416)
+               
+               116        1218 LOAD_DEREF              13 (request)
+                          1220 LOAD_ATTR               20 (user)
+                          1230 LOAD_METHOD             22 (has_perm)
+                          1252 LOAD_CONST              12 ('wagtailadmin.access_admin')
+                          1254 PRECALL                  1
+                          1258 CALL                     1
+               
+               114        1268 POP_JUMP_FORWARD_IF_FALSE    73 (to 1416)
+               
+               117        1270 LOAD_DEREF              13 (request)
+                          1272 LOAD_ATTR               20 (user)
+                          1282 LOAD_METHOD             22 (has_perm)
+                          1304 LOAD_DEREF              12 (model)
+                          1306 LOAD_ATTR               23 (_meta)
+                          1316 LOAD_ATTR               24 (app_label)
+                          1326 FORMAT_VALUE             0
+                          1328 LOAD_CONST              13 ('.change_')
+                          1330 LOAD_DEREF              12 (model)
+                          1332 LOAD_ATTR               23 (_meta)
+                          1342 LOAD_ATTR               25 (model_name)
+                          1352 FORMAT_VALUE             0
+                          1354 BUILD_STRING             3
+                          1356 PRECALL                  1
+                          1360 CALL                     1
+               
+               114        1370 POP_JUMP_FORWARD_IF_FALSE    22 (to 1416)
+               
+               118        1372 LOAD_GLOBAL             53 (NULL + getattr)
+                          1384 LOAD_DEREF              13 (request)
+                          1386 LOAD_GLOBAL             54 (FEDIT_PREVIEW_VAR)
+                          1398 LOAD_CONST               8 (False)
+                          1400 PRECALL                  3
+                          1404 CALL                     3
+               
+               114        1414 POP_JUMP_FORWARD_IF_TRUE     2 (to 1420)
+               
+               121     >> 1416 LOAD_FAST                8 (rendered)
+                          1418 RETURN_VALUE
+               
+               125     >> 1420 LOAD_GLOBAL             13 (NULL + isinstance)
+                          1432 LOAD_DEREF              12 (model)
+                          1434 LOAD_GLOBAL             56 (Page)
+                          1446 PRECALL                  2
+                          1450 CALL                     2
+                          1460 POP_JUMP_FORWARD_IF_FALSE    29 (to 1520)
+               
+               126        1462 LOAD_GLOBAL             59 (NULL + _get_from_context_or_set)
+               
+               127        1474 LOAD_FAST                1 (context)
+                          1476 LOAD_CONST              14 ('page_base_edit_url')
+               
+               128        1478 LOAD_CLOSURE            12 (model)
+                          1480 BUILD_TUPLE              1
+                          1482 LOAD_CONST              15 (<code object <lambda>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 128>)
+                          1484 MAKE_FUNCTION            8 (closure)
+               
+               126        1486 PRECALL                  3
+                          1490 CALL                     3
+                          1500 STORE_FAST               9 (admin_edit_url)
+               
+               133        1502 LOAD_FAST                9 (admin_edit_url)
+                          1504 FORMAT_VALUE             0
+                          1506 LOAD_CONST              16 ('#block-')
+                          1508 LOAD_FAST                3 (block_id)
+                          1510 FORMAT_VALUE             0
+                          1512 LOAD_CONST              17 ('-section')
+                          1514 BUILD_STRING             4
+                          1516 STORE_FAST               9 (admin_edit_url)
+                          1518 JUMP_FORWARD             2 (to 1524)
+               
+               135     >> 1520 LOAD_CONST               0 (None)
+                          1522 STORE_FAST               9 (admin_edit_url)
+               
+               137     >> 1524 LOAD_FAST                5 (extra)
+                          1526 LOAD_METHOD             30 (setdefault)
+                          1548 LOAD_CONST              18 ('has_block')
+                          1550 LOAD_FAST                0 (self)
+                          1552 LOAD_ATTR               14 (has_block)
+                          1562 PRECALL                  2
+                          1566 CALL                     2
+                          1576 POP_TOP
+               
+               140        1578 LOAD_GLOBAL             63 (NULL + FeditBlockEditButton)
+                          1590 PRECALL                  0
+                          1594 CALL                     0
+               
+               139        1604 BUILD_LIST               1
+                          1606 STORE_FAST              10 (items)
+               
+               143        1608 LOAD_GLOBAL             65 (NULL + hooks)
+                          1620 LOAD_ATTR               33 (get_hooks)
+                          1630 LOAD_GLOBAL             68 (CONSTRUCT_BLOCK_TOOLBAR)
+                          1642 PRECALL                  1
+                          1646 CALL                     1
+                          1656 GET_ITER
+                       >> 1658 FOR_ITER                18 (to 1696)
+                          1660 STORE_FAST              11 (hook)
+               
+               144        1662 PUSH_NULL
+                          1664 LOAD_FAST               11 (hook)
+                          1666 LOAD_DEREF              13 (request)
+                          1668 LOAD_FAST               10 (items)
+                          1670 LOAD_DEREF              12 (model)
+                          1672 LOAD_FAST                3 (block_id)
+                          1674 LOAD_FAST                4 (field_name)
+                          1676 KW_NAMES                19
+                          1678 PRECALL                  5
+                          1682 CALL                     5
+                          1692 POP_TOP
+                          1694 JUMP_BACKWARD           19 (to 1658)
+               
+               146     >> 1696 LOAD_CLOSURE            13 (request)
+                          1698 BUILD_TUPLE              1
+                          1700 LOAD_CONST              20 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 146>)
+                          1702 MAKE_FUNCTION            8 (closure)
+                          1704 LOAD_FAST               10 (items)
+                          1706 GET_ITER
+                          1708 PRECALL                  0
+                          1712 CALL                     0
+                          1722 STORE_FAST              10 (items)
+               
+               147        1724 LOAD_GLOBAL             71 (NULL + list)
+                          1736 LOAD_GLOBAL             73 (NULL + filter)
+                          1748 LOAD_CONST               0 (None)
+                          1750 LOAD_FAST               10 (items)
+                          1752 PRECALL                  2
+                          1756 CALL                     2
+                          1766 PRECALL                  1
+                          1770 CALL                     1
+                          1780 STORE_FAST              10 (items)
+               
+               149        1782 LOAD_GLOBAL             75 (NULL + render_to_string)
+               
+               150        1794 LOAD_CONST              21 ('wagtail_fedit/content/editable_block.html')
+               
+               152        1796 PUSH_NULL
+                          1798 LOAD_FAST                0 (self)
+                          1800 LOAD_ATTR               38 (get_edit_url)
+               
+               153        1810 LOAD_FAST                3 (block_id)
+                          1812 LOAD_FAST                4 (field_name)
+               
+               152        1814 BUILD_TUPLE              2
+                          1816 LOAD_CONST              22 ('instance')
+               
+               154        1818 LOAD_DEREF              12 (model)
+               
+               152        1820 BUILD_MAP                1
+               
+               155        1822 LOAD_FAST                5 (extra)
+               
+               152        1824 DICT_MERGE               1
+                          1826 CALL_FUNCTION_EX         1
+               
+               157        1828 LOAD_FAST                9 (admin_edit_url)
+               
+               158        1830 LOAD_FAST                3 (block_id)
+               
+               159        1832 LOAD_DEREF              12 (model)
+               
+               160        1834 LOAD_FAST                8 (rendered)
+               
+               161        1836 LOAD_FAST                4 (field_name)
+               
+               162        1838 LOAD_FAST                1 (context)
+               
+               163        1840 LOAD_FAST               10 (items)
+               
+               151        1842 LOAD_CONST              23 (('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'toolbar_items'))
+                          1844 BUILD_CONST_KEY_MAP      8
+               
+               149        1846 PRECALL                  2
+                          1850 CALL                     2
+                          1860 RETURN_VALUE
                ExceptionTable:
                  682 to 720 -> 724 [0]
                  724 to 742 -> 750 [1] lasti
                  748 to 748 -> 750 [1] lasti
                consts
                   None
                   'Field name is required'
@@ -1020,38 +1000,38 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x95019700740100000000000000000000640189006a0100000000000000
                         006701ac02a6020000ab0200000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     132           2 RESUME                   0
+                     128           2 RESUME                   0
                                    4 LOAD_GLOBAL              1 (NULL + reverse)
                      
-                     133          16 LOAD_CONST               1 ('wagtailadmin_pages:edit')
+                     129          16 LOAD_CONST               1 ('wagtailadmin_pages:edit')
                      
-                     134          18 LOAD_DEREF               0 (model)
+                     130          18 LOAD_DEREF               0 (model)
                                   20 LOAD_ATTR                1 (id)
                                   30 BUILD_LIST               1
                      
-                     132          32 KW_NAMES                 2
+                     128          32 KW_NAMES                 2
                                   34 PRECALL                  2
                                   38 CALL                     2
                                   48 RETURN_VALUE
                      consts
                         None
                         'wagtailadmin_pages:edit'
                         ('args',)
                      names      ('reverse', 'id')
                      varnames   ()
                      freevars   ('model',)
                      cellvars   ()
                      filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<lambda>'
-                     firstlineno 132
+                     firstlineno 128
                      lnotab 0x100102010efe
                   '#block-'
                   '-section'
                   'has_block'
                   ('request', 'items', 'model', 'block_id', 'field_name')
                   code
                      argcount  : 1
@@ -1059,15 +1039,15 @@
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d177d017c01a00000000000000000000000000000
                         000000000000008902a6010000ab01000000000000000091028c185300
                                    0 COPY_FREE_VARS           1
                      
-                     150           2 RESUME                   0
+                     146           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                23 (to 56)
                                   10 STORE_FAST               1 (item)
                                   12 LOAD_FAST                1 (item)
                                   14 LOAD_METHOD              0 (render)
                                   36 LOAD_DEREF               2 (request)
@@ -1079,84 +1059,84 @@
                      consts
                      names      ('render',)
                      varnames   ('.0', 'item')
                      freevars   ('request',)
                      cellvars   ()
                      filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<listcomp>'
-                     firstlineno 150
+                     firstlineno 146
                      lnotab 0x
                   'wagtail_fedit/content/editable_block.html'
                   'instance'
                   ('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'toolbar_items')
-               names      ('block', 'block_id', 'field_name', 'model', 'extra', 'items', 'isinstance', 'FilterExpression', 'resolve', 'ValueError', 'flatten', 'AttributeError', 'update', 'render_as_block', 'has_block', 'nl', 'render', 'get', 'can_fedit', 'hasattr', 'id', 'user', 'is_authenticated', 'has_perm', '_meta', 'app_label', 'model_name', 'getattr', 'FEDIT_PREVIEW_VAR', 'Page', '_get_from_context_or_set', 'setdefault', 'FeditBlockEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_BLOCK_TOOLBAR', 'list', 'filter', 'render_to_string', 'get_edit_url')
+               names      ('block', 'block_id', 'field_name', 'model', 'extra', 'items', 'isinstance', 'FilterExpression', 'resolve', 'ValueError', 'flatten', 'AttributeError', 'update', 'render_as_block', 'has_block', 'nl', 'render', 'get', 'hasattr', 'id', 'user', 'is_authenticated', 'has_perm', '_meta', 'app_label', 'model_name', 'getattr', 'FEDIT_PREVIEW_VAR', 'Page', '_get_from_context_or_set', 'setdefault', 'FeditBlockEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_BLOCK_TOOLBAR', 'list', 'filter', 'render_to_string', 'get_edit_url')
                varnames   ('self', 'context', 'block', 'block_id', 'field_name', 'extra', 'k', 'e', 'rendered', 'admin_edit_url', 'items', 'hook')
                freevars   ()
                cellvars   ('model', 'request')
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 52
+               firstlineno 51
                lnotab
                   0x06010e010e010e010e010e0332012a0132022a012a012a012a012a012a
                   012a012a0304011e0210011e020c011e04040102012c01120104ff08022a
-                  012a0110010e01340138021e02220104030c0112012801100104011e0514
-                  032a01040216ff020232fe020364fd02042afc020704042a010c01040108
-                  fe10071202040236031aff0404360122021c013a020c0102020e0104ff04
-                  0202fe020302fd040502010201020102010201020102f404fe
+                  012a0110010e01340138021e030c0112012801100104011e0514032a0104
+                  0216ff020232fe020364fd02042afc020704042a010c01040108fe100712
+                  02040236031aff0404360122021c013a020c0102020e0104ff040202fe02
+                  0302fd040502010201020102010201020102f404fe
             'return'
             code
                argcount  : 0
                nlocals   : 4
                stacksize : 6
                flags     : 11
                code
                   0x970069007d017c00a00000000000000000000000000000000000000000
                   00a6000000ab00000000000000000044005d2f5c0200007d027d03740200
                   000000000000000000a00200000000000000000000000000000000000000
                   007407000000000000000000007c03a6010000ab010000000000000000a6
                   010000ab0100000000000000007c017c023c0000008c307c015300
-               171           0 RESUME                   0
+               167           0 RESUME                   0
                
-               174           2 BUILD_MAP                0
+               170           2 BUILD_MAP                0
                              4 STORE_FAST               1 (packed)
                
-               175           6 LOAD_FAST                0 (kwargs)
+               171           6 LOAD_FAST                0 (kwargs)
                              8 LOAD_METHOD              0 (items)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 GET_ITER
                        >>   46 FOR_ITER                47 (to 142)
                             48 UNPACK_SEQUENCE          2
                             52 STORE_FAST               2 (k)
                             54 STORE_FAST               3 (v)
                
-               176          56 LOAD_GLOBAL              2 (url_value_signer)
+               172          56 LOAD_GLOBAL              2 (url_value_signer)
                             68 LOAD_METHOD              2 (sign)
                             90 LOAD_GLOBAL              7 (NULL + str)
                            102 LOAD_FAST                3 (v)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 PRECALL                  1
                            122 CALL                     1
                            132 LOAD_FAST                1 (packed)
                            134 LOAD_FAST                2 (k)
                            136 STORE_SUBSCR
                            140 JUMP_BACKWARD           48 (to 46)
                
-               178     >>  142 LOAD_FAST                1 (packed)
+               174     >>  142 LOAD_FAST                1 (packed)
                            144 RETURN_VALUE
                consts
                   None
                names      ('items', 'url_value_signer', 'sign', 'str')
                varnames   ('kwargs', 'packed', 'k', 'v')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'pack'
-               firstlineno 171
+               firstlineno 167
                lnotab 0x0203040132015602
             ('request',)
             'expected'
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 7
@@ -1177,130 +1157,130 @@
                   057c039b009d02a6010000ab010000000000000000820177007803590077
                   0174150000000000000000000088046601640684087c024400a6000000ab
                   000000000000000000a6010000ab01000000000000000073187c00a00700
                   0000000000000000000000000000000000000064057c039b009d02a60100
                   00ab010000000000000000820189045300
                              0 MAKE_CELL                4 (unpacked)
                
-               180           2 RESUME                   0
+               176           2 RESUME                   0
                
-               182           4 LOAD_FAST                1 (request)
+               178           4 LOAD_FAST                1 (request)
                              6 POP_JUMP_FORWARD_IF_TRUE    15 (to 38)
                
-               183           8 LOAD_GLOBAL              1 (NULL + ValueError)
+               179           8 LOAD_GLOBAL              1 (NULL + ValueError)
                             20 LOAD_CONST               1 ('Request is required')
                             22 PRECALL                  1
                             26 CALL                     1
                             36 RAISE_VARARGS            1
                
-               185     >>   38 BUILD_MAP                0
+               181     >>   38 BUILD_MAP                0
                             40 STORE_DEREF              4 (unpacked)
                
-               186          42 LOAD_FAST                2 (expected)
+               182          42 LOAD_FAST                2 (expected)
                             44 GET_ITER
                        >>   46 FOR_ITER               171 (to 390)
                             48 STORE_FAST               3 (key)
                
-               187          50 NOP
+               183          50 NOP
                
-               188          52 LOAD_GLOBAL              2 (url_value_signer)
+               184          52 LOAD_GLOBAL              2 (url_value_signer)
                             64 LOAD_METHOD              2 (unsign)
                
-               189          86 LOAD_FAST                1 (request)
+               185          86 LOAD_FAST                1 (request)
                             88 LOAD_ATTR                3 (GET)
                             98 LOAD_METHOD              4 (get)
                            120 LOAD_FAST                3 (key)
                            122 PRECALL                  1
                            126 CALL                     1
                
-               188         136 PRECALL                  1
+               184         136 PRECALL                  1
                            140 CALL                     1
                            150 LOAD_DEREF               4 (unpacked)
                            152 LOAD_FAST                3 (key)
                            154 STORE_SUBSCR
                            158 JUMP_BACKWARD           57 (to 46)
                        >>  160 PUSH_EXC_INFO
                
-               191         162 LOAD_GLOBAL             10 (signing)
+               187         162 LOAD_GLOBAL             10 (signing)
                            174 LOAD_ATTR                6 (SignatureExpired)
                            184 CHECK_EXC_MATCH
                            186 POP_JUMP_FORWARD_IF_FALSE    26 (to 240)
                            188 POP_TOP
                
-               192         190 LOAD_FAST                0 (cls)
+               188         190 LOAD_FAST                0 (cls)
                            192 LOAD_METHOD              7 (UnpackError)
                            214 LOAD_CONST               2 ('Value for ')
                            216 LOAD_FAST                3 (key)
                            218 FORMAT_VALUE             0
                            220 LOAD_CONST               3 (' has expired')
                            222 BUILD_STRING             3
                            224 PRECALL                  1
                            228 CALL                     1
                            238 RAISE_VARARGS            1
                
-               193     >>  240 LOAD_GLOBAL             10 (signing)
+               189     >>  240 LOAD_GLOBAL             10 (signing)
                            252 LOAD_ATTR                8 (BadSignature)
                            262 CHECK_EXC_MATCH
                            264 POP_JUMP_FORWARD_IF_FALSE    25 (to 316)
                            266 POP_TOP
                
-               194         268 LOAD_FAST                0 (cls)
+               190         268 LOAD_FAST                0 (cls)
                            270 LOAD_METHOD              7 (UnpackError)
                            292 LOAD_CONST               4 ('Invalid value for ')
                            294 LOAD_FAST                3 (key)
                            296 FORMAT_VALUE             0
                            298 BUILD_STRING             2
                            300 PRECALL                  1
                            304 CALL                     1
                            314 RAISE_VARARGS            1
                
-               195     >>  316 LOAD_GLOBAL             18 (TypeError)
+               191     >>  316 LOAD_GLOBAL             18 (TypeError)
                            328 CHECK_EXC_MATCH
                            330 POP_JUMP_FORWARD_IF_FALSE    25 (to 382)
                            332 POP_TOP
                
-               196         334 LOAD_FAST                0 (cls)
+               192         334 LOAD_FAST                0 (cls)
                            336 LOAD_METHOD              7 (UnpackError)
                            358 LOAD_CONST               5 ('Missing value for ')
                            360 LOAD_FAST                3 (key)
                            362 FORMAT_VALUE             0
                            364 BUILD_STRING             2
                            366 PRECALL                  1
                            370 CALL                     1
                            380 RAISE_VARARGS            1
                
-               195     >>  382 RERAISE                  0
+               191     >>  382 RERAISE                  0
                        >>  384 COPY                     3
                            386 POP_EXCEPT
                            388 RERAISE                  1
                
-               198     >>  390 LOAD_GLOBAL             21 (NULL + all)
+               194     >>  390 LOAD_GLOBAL             21 (NULL + all)
                            402 LOAD_CLOSURE             4 (unpacked)
                            404 BUILD_TUPLE              1
-                           406 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 198>)
+                           406 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 194>)
                            408 MAKE_FUNCTION            8 (closure)
                            410 LOAD_FAST                2 (expected)
                            412 GET_ITER
                            414 PRECALL                  0
                            418 CALL                     0
                            428 PRECALL                  1
                            432 CALL                     1
                            442 POP_JUMP_FORWARD_IF_TRUE    24 (to 492)
                
-               199         444 LOAD_FAST                0 (cls)
+               195         444 LOAD_FAST                0 (cls)
                            446 LOAD_METHOD              7 (UnpackError)
                            468 LOAD_CONST               5 ('Missing value for ')
                            470 LOAD_FAST                3 (key)
                            472 FORMAT_VALUE             0
                            474 BUILD_STRING             2
                            476 PRECALL                  1
                            480 CALL                     1
                            490 RAISE_VARARGS            1
                
-               201     >>  492 LOAD_DEREF               4 (unpacked)
+               197     >>  492 LOAD_DEREF               4 (unpacked)
                            494 RETURN_VALUE
                ExceptionTable:
                  52 to 156 -> 160 [1]
                  160 to 382 -> 384 [2] lasti
                consts
                   None
                   'Request is required'
@@ -1314,15 +1294,15 @@
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d177d018902a00000000000000000000000000000
                         000000000000007c01a6010000ab01000000000000000091028c185300
                                    0 COPY_FREE_VARS           1
                      
-                     198           2 RESUME                   0
+                     194           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                23 (to 56)
                                   10 STORE_FAST               1 (key)
                                   12 LOAD_DEREF               2 (unpacked)
                                   14 LOAD_METHOD              0 (get)
                                   36 LOAD_FAST                1 (key)
@@ -1334,23 +1314,23 @@
                      consts
                      names      ('get',)
                      varnames   ('.0', 'key')
                      freevars   ('unpacked',)
                      cellvars   ()
                      filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<listcomp>'
-                     firstlineno 198
+                     firstlineno 194
                      lnotab 0x
                names      ('ValueError', 'url_value_signer', 'unsign', 'GET', 'get', 'signing', 'SignatureExpired', 'UnpackError', 'BadSignature', 'TypeError', 'all')
                varnames   ('cls', 'request', 'expected', 'key')
                freevars   ()
                cellvars   ('unpacked',)
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'unpack'
-               firstlineno 180
+               firstlineno 176
                lnotab
                   0x040204011e02040108010201220132ff1a031c0132011c013001120130
                   ff080336013002
             'instance'
             code
                argcount  : 3
                nlocals   : 6
@@ -1359,58 +1339,58 @@
                code
                   0x970074010000000000000000000064017c007c017c026a010000000000
                   0000006a0200000000000000007c026a0100000000000000006a03000000
                   00000000007c026a0400000000000000006705ac02a6020000ab02000000
                   00000000007d047c0373027c045300740b00000000000000000000740d00
                   0000000000000000006a070000000000000000640469007c03a4018e01a6
                   010000ab0100000000000000007d057c049b0064037c059b009d035300
-               203           0 RESUME                   0
+               199           0 RESUME                   0
                
-               205           2 LOAD_GLOBAL              1 (NULL + reverse)
+               201           2 LOAD_GLOBAL              1 (NULL + reverse)
                
-               206          14 LOAD_CONST               1 ('wagtail_fedit:edit_block')
+               202          14 LOAD_CONST               1 ('wagtail_fedit:edit_block')
                
-               207          16 LOAD_FAST                0 (block_id)
+               203          16 LOAD_FAST                0 (block_id)
                             18 LOAD_FAST                1 (field_name)
                             20 LOAD_FAST                2 (instance)
                             22 LOAD_ATTR                1 (_meta)
                             32 LOAD_ATTR                2 (app_label)
                             42 LOAD_FAST                2 (instance)
                             44 LOAD_ATTR                1 (_meta)
                             54 LOAD_ATTR                3 (model_name)
                             64 LOAD_FAST                2 (instance)
                             66 LOAD_ATTR                4 (pk)
                             76 BUILD_LIST               5
                
-               205          78 KW_NAMES                 2
+               201          78 KW_NAMES                 2
                             80 PRECALL                  2
                             84 CALL                     2
                             94 STORE_FAST               4 (base_url)
                
-               210          96 LOAD_FAST                3 (kwargs)
+               206          96 LOAD_FAST                3 (kwargs)
                             98 POP_JUMP_FORWARD_IF_TRUE     2 (to 104)
                
-               211         100 LOAD_FAST                4 (base_url)
+               207         100 LOAD_FAST                4 (base_url)
                            102 RETURN_VALUE
                
-               213     >>  104 LOAD_GLOBAL             11 (NULL + urlencode)
+               209     >>  104 LOAD_GLOBAL             11 (NULL + urlencode)
                
-               214         116 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+               210         116 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                            128 LOAD_ATTR                7 (pack)
                            138 LOAD_CONST               4 (())
                            140 BUILD_MAP                0
                            142 LOAD_FAST                3 (kwargs)
                            144 DICT_MERGE               1
                            146 CALL_FUNCTION_EX         1
                
-               213         148 PRECALL                  1
+               209         148 PRECALL                  1
                            152 CALL                     1
                            162 STORE_FAST               5 (packed)
                
-               216         164 LOAD_FAST                4 (base_url)
+               212         164 LOAD_FAST                4 (base_url)
                            166 FORMAT_VALUE             0
                            168 LOAD_CONST               3 ('?')
                            170 LOAD_FAST                5 (packed)
                            172 FORMAT_VALUE             0
                            174 BUILD_STRING             3
                            176 RETURN_VALUE
                consts
@@ -1421,27 +1401,27 @@
                   ()
                names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack')
                varnames   ('block_id', 'field_name', 'instance', 'kwargs', 'base_url', 'packed')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'get_edit_url'
-               firstlineno 203
+               firstlineno 199
                lnotab 0x02020c0102013efe1205040104020c0120ff1003
             (None, None, None, None, None)
          names      ('__name__', '__module__', '__qualname__', 'Exception', 'UnpackError', 'NodeList', 'BoundBlock', 'str', 'models', 'Model', '__init__', 'render', 'staticmethod', 'dict', 'pack', 'classmethod', 'unpack', 'get_edit_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'BlockEditNode'
-         firstlineno 32
+         firstlineno 31
          lnotab
             0x0a011c04020102010201020102fb040102ff020202fe020302fd020402
-            fc02050cfb0810067702010aff0e010208020114ff0e010216020120ff0e
+            fc02050cfb0810067402010aff0e010208020114ff0e010216020120ff0e
             01
       'BlockEditNode'
       'fedit_block'
       ('name',)
       'parser'
       'token'
       code
@@ -1464,134 +1444,134 @@
             0000008c0f740f00000000000000000000640b7c067c05a0080000000000
             0000000000000000000000000000006405a6010000ab0100000000000000
             007c05a00800000000000000000000000000000000000000006408a60100
             00ab0100000000000000007c05a008000000000000000000000000000000
             00000000006403a6010000ab0100000000000000007c05a0080000000000
             0000000000000000000000000000006409a6010000ab0100000000000000
             00640a9c057c07a4018e015300
-         220           0 RESUME                   0
+         216           0 RESUME                   0
          
-         250           2 LOAD_FAST                1 (token)
+         246           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         251          42 LOAD_FAST                2 (tokens)
+         247          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         252          84 BUILD_LIST               0
+         248          84 BUILD_LIST               0
                       86 LOAD_CONST               2 (('block', 'block_id', 'field_name', 'model'))
                       88 LIST_EXTEND              1
                       90 STORE_FAST               4 (kwargs_names)
          
-         257          92 LOAD_GLOBAL              5 (NULL + get_kwargs)
+         253          92 LOAD_GLOBAL              5 (NULL + get_kwargs)
                      104 LOAD_FAST                0 (parser)
                      106 LOAD_FAST                4 (kwargs_names)
                      108 LOAD_FAST                2 (tokens)
                      110 PRECALL                  3
                      114 CALL                     3
                      124 STORE_FAST               5 (kwargs)
          
-         258         126 LOAD_CONST               3 ('field_name')
+         254         126 LOAD_CONST               3 ('field_name')
                      128 LOAD_FAST                5 (kwargs)
                      130 CONTAINS_OP              1
                      132 POP_JUMP_FORWARD_IF_FALSE    15 (to 164)
          
-         259         134 LOAD_GLOBAL              7 (NULL + ValueError)
+         255         134 LOAD_GLOBAL              7 (NULL + ValueError)
                      146 LOAD_CONST               4 ('Field name is required')
                      148 PRECALL                  1
                      152 CALL                     1
                      162 RAISE_VARARGS            1
          
-         261     >>  164 LOAD_CONST               5 ('block')
+         257     >>  164 LOAD_CONST               5 ('block')
                      166 LOAD_FAST                5 (kwargs)
                      168 CONTAINS_OP              1
                      170 POP_JUMP_FORWARD_IF_FALSE    42 (to 256)
          
-         262         172 LOAD_FAST                0 (parser)
+         258         172 LOAD_FAST                0 (parser)
                      174 LOAD_METHOD              4 (parse)
                      196 LOAD_CONST               6 (('unfedit_block',))
                      198 PRECALL                  1
                      202 CALL                     1
                      212 STORE_FAST               6 (nodelist)
          
-         263         214 LOAD_FAST                0 (parser)
+         259         214 LOAD_FAST                0 (parser)
                      216 LOAD_METHOD              5 (delete_first_token)
                      238 PRECALL                  0
                      242 CALL                     0
                      252 POP_TOP
                      254 JUMP_FORWARD             2 (to 260)
          
-         265     >>  256 LOAD_CONST               7 (None)
+         261     >>  256 LOAD_CONST               7 (None)
                      258 STORE_FAST               6 (nodelist)
          
-         267     >>  260 BUILD_MAP                0
+         263     >>  260 BUILD_MAP                0
                      262 STORE_FAST               7 (extra)
          
-         268         264 LOAD_FAST                5 (kwargs)
+         264         264 LOAD_FAST                5 (kwargs)
                      266 LOAD_METHOD              6 (items)
                      288 PRECALL                  0
                      292 CALL                     0
                      302 GET_ITER
                  >>  304 FOR_ITER                14 (to 334)
                      306 UNPACK_SEQUENCE          2
                      310 STORE_FAST               8 (key)
                      312 STORE_FAST               9 (value)
          
-         269         314 LOAD_FAST                8 (key)
+         265         314 LOAD_FAST                8 (key)
                      316 LOAD_FAST                4 (kwargs_names)
                      318 CONTAINS_OP              1
                      320 POP_JUMP_FORWARD_IF_FALSE     5 (to 332)
          
-         270         322 LOAD_FAST                9 (value)
+         266         322 LOAD_FAST                9 (value)
                      324 LOAD_FAST                7 (extra)
                      326 LOAD_FAST                8 (key)
                      328 STORE_SUBSCR
                  >>  332 JUMP_BACKWARD           15 (to 304)
          
-         272     >>  334 LOAD_GLOBAL             15 (NULL + BlockEditNode)
+         268     >>  334 LOAD_GLOBAL             15 (NULL + BlockEditNode)
                      346 LOAD_CONST              11 (())
          
-         273         348 LOAD_FAST                6 (nodelist)
+         269         348 LOAD_FAST                6 (nodelist)
          
-         274         350 LOAD_FAST                5 (kwargs)
+         270         350 LOAD_FAST                5 (kwargs)
                      352 LOAD_METHOD              8 (get)
                      374 LOAD_CONST               5 ('block')
                      376 PRECALL                  1
                      380 CALL                     1
          
-         275         390 LOAD_FAST                5 (kwargs)
+         271         390 LOAD_FAST                5 (kwargs)
                      392 LOAD_METHOD              8 (get)
                      414 LOAD_CONST               8 ('block_id')
                      416 PRECALL                  1
                      420 CALL                     1
          
-         276         430 LOAD_FAST                5 (kwargs)
+         272         430 LOAD_FAST                5 (kwargs)
                      432 LOAD_METHOD              8 (get)
                      454 LOAD_CONST               3 ('field_name')
                      456 PRECALL                  1
                      460 CALL                     1
          
-         277         470 LOAD_FAST                5 (kwargs)
+         273         470 LOAD_FAST                5 (kwargs)
                      472 LOAD_METHOD              8 (get)
                      494 LOAD_CONST               9 ('model')
                      496 PRECALL                  1
                      500 CALL                     1
          
-         272         510 LOAD_CONST              10 (('nodelist', 'block', 'block_id', 'field_name', 'model'))
+         268         510 LOAD_CONST              10 (('nodelist', 'block', 'block_id', 'field_name', 'model'))
                      512 BUILD_CONST_KEY_MAP      5
          
-         278         514 LOAD_FAST                7 (extra)
+         274         514 LOAD_FAST                7 (extra)
          
-         272         516 DICT_MERGE               1
+         268         516 DICT_MERGE               1
                      518 CALL_FUNCTION_EX         1
                      520 RETURN_VALUE
          consts
             '\n    This tag is used to render an editable block.\n\n    This block will be wrapped and is able to be edited by the user on the frontend.\n\n    We will require the block_id and field_name of the streamfield this block belongs to.\n\n    You could omit needing to pass a block ID by passing in the StreamChild instance as opposed to the StructValue instance.\n    \n    Usage example 1:\n        ```python\n        {% fedit_block my_structvalue_instance block_id my_streamfield_attribute_name page_instance %}\n        ```\n\n    Optionally you can omit the block and pass in the block_id and field_name as keyword arguments.\n\n    This will allow you to use the block as a block tag.\n\n    Usage example 2:\n        ```python\n        {% fedit_block block_id=my_structvalue_instance field_name=my_streamfield_attribute_name model=page_instance %}\n            <p>Some content before block</p>\n            {% include_block my_block %}\n            <p>Some content after block</p>\n        {% unfedit_block %}\n        ```\n    '
             0
             ('block', 'block_id', 'field_name', 'model')
             'field_name'
@@ -1605,15 +1585,15 @@
             ()
          names      ('split_contents', 'pop', 'get_kwargs', 'ValueError', 'parse', 'delete_first_token', 'items', 'BlockEditNode', 'get')
          varnames   ('parser', 'token', 'tokens', '_', 'kwargs_names', 'kwargs', 'nodelist', 'extra', 'key', 'value')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit_block'
-         firstlineno 220
+         firstlineno 216
          lnotab
             0x021e28012a010805220108011e0208012a012a0204020401320108010c
             020e01020128012801280128fb040602fa
       True
       'fedit_field'
       ('takes_context', 'name')
       None
@@ -1645,144 +1625,144 @@
             00000072497c086a090000000000000000a00b0000000000000000000000
             0000000000000000007c026a0c00000000000000006a0d00000000000000
             009b0064077c026a0c00000000000000006a0e00000000000000009b009d
             03a6010000ab0100000000000000007216740b000000000000000000007c
             08741e000000000000000000006408a6030000ab03000000000000000073
             027c0353007421000000000000000000007c087c037c017c027c00660569
             007c05a4018e015300
-         282           0 RESUME                   0
+         278           0 RESUME                   0
          
-         300           2 LOAD_GLOBAL              1 (NULL + all)
+         296           2 LOAD_GLOBAL              1 (NULL + all)
                       14 LOAD_FAST                1 (field_name)
                       16 LOAD_FAST                2 (model)
                       18 BUILD_LIST               2
                       20 PRECALL                  1
                       24 CALL                     1
                       34 POP_JUMP_FORWARD_IF_TRUE    15 (to 66)
          
-         301          36 LOAD_GLOBAL              3 (NULL + ValueError)
+         297          36 LOAD_GLOBAL              3 (NULL + ValueError)
                       48 LOAD_CONST               1 ('Field name, and model are required')
                       50 PRECALL                  1
                       54 CALL                     1
                       64 RAISE_VARARGS            1
          
-         303     >>   66 BUILD_MAP                0
+         299     >>   66 BUILD_MAP                0
                       68 STORE_FAST               5 (extra)
          
-         304          70 LOAD_FAST                4 (kwargs)
+         300          70 LOAD_FAST                4 (kwargs)
                       72 LOAD_METHOD              2 (items)
                       94 PRECALL                  0
                       98 CALL                     0
                      108 GET_ITER
                  >>  110 FOR_ITER                10 (to 132)
                      112 UNPACK_SEQUENCE          2
                      116 STORE_FAST               6 (key)
                      118 STORE_FAST               7 (value)
          
-         305         120 LOAD_FAST                7 (value)
+         301         120 LOAD_FAST                7 (value)
                      122 LOAD_FAST                5 (extra)
                      124 LOAD_FAST                6 (key)
                      126 STORE_SUBSCR
                      130 JUMP_BACKWARD           11 (to 110)
          
-         308     >>  132 LOAD_FAST                0 (context)
+         304     >>  132 LOAD_FAST                0 (context)
                      134 LOAD_METHOD              3 (get)
                      156 LOAD_CONST               2 ('request')
                      158 PRECALL                  1
                      162 CALL                     1
                      172 STORE_FAST               8 (request)
          
-         309         174 LOAD_FAST                3 (content)
+         305         174 LOAD_FAST                3 (content)
                      176 POP_JUMP_FORWARD_IF_TRUE    64 (to 306)
          
-         310         178 LOAD_GLOBAL              9 (NULL + hasattr)
+         306         178 LOAD_GLOBAL              9 (NULL + hasattr)
                      190 LOAD_FAST                2 (model)
                      192 LOAD_CONST               3 ('render_fedit_')
                      194 LOAD_FAST                1 (field_name)
                      196 FORMAT_VALUE             0
                      198 BUILD_STRING             2
                      200 PRECALL                  2
                      204 CALL                     2
                      214 POP_JUMP_FORWARD_IF_FALSE    29 (to 274)
          
-         311         216 PUSH_NULL
+         307         216 PUSH_NULL
                      218 LOAD_GLOBAL             11 (NULL + getattr)
                      230 LOAD_FAST                2 (model)
                      232 LOAD_CONST               3 ('render_fedit_')
                      234 LOAD_FAST                1 (field_name)
                      236 FORMAT_VALUE             0
                      238 BUILD_STRING             2
                      240 PRECALL                  2
                      244 CALL                     2
                      254 LOAD_FAST                8 (request)
                      256 PRECALL                  1
                      260 CALL                     1
                      270 STORE_FAST               3 (content)
                      272 JUMP_FORWARD            16 (to 306)
          
-         313     >>  274 LOAD_GLOBAL             11 (NULL + getattr)
+         309     >>  274 LOAD_GLOBAL             11 (NULL + getattr)
                      286 LOAD_FAST                2 (model)
                      288 LOAD_FAST                1 (field_name)
                      290 PRECALL                  2
                      294 CALL                     2
                      304 STORE_FAST               3 (content)
          
-         315     >>  306 LOAD_GLOBAL              9 (NULL + hasattr)
+         311     >>  306 LOAD_GLOBAL              9 (NULL + hasattr)
                      318 LOAD_FAST                0 (context)
                      320 LOAD_CONST               4 ('flatten')
                      322 PRECALL                  2
                      326 CALL                     2
                      336 POP_JUMP_FORWARD_IF_FALSE    20 (to 378)
          
-         316         338 LOAD_FAST                0 (context)
+         312         338 LOAD_FAST                0 (context)
                      340 LOAD_METHOD              6 (flatten)
                      362 PRECALL                  0
                      366 CALL                     0
                      376 STORE_FAST               0 (context)
          
-         318     >>  378 LOAD_GLOBAL              9 (NULL + hasattr)
+         314     >>  378 LOAD_GLOBAL              9 (NULL + hasattr)
                      390 LOAD_FAST                3 (content)
                      392 LOAD_CONST               5 ('render_as_block')
                      394 PRECALL                  2
                      398 CALL                     2
                      408 POP_JUMP_FORWARD_IF_FALSE    42 (to 494)
          
-         319         410 LOAD_FAST                0 (context)
+         315         410 LOAD_FAST                0 (context)
                      412 LOAD_METHOD              7 (update)
                      434 LOAD_FAST                4 (kwargs)
                      436 PRECALL                  1
                      440 CALL                     1
                      450 POP_TOP
          
-         320         452 LOAD_FAST                3 (content)
+         316         452 LOAD_FAST                3 (content)
                      454 LOAD_METHOD              8 (render_as_block)
                      476 LOAD_FAST                0 (context)
                      478 PRECALL                  1
                      482 CALL                     1
                      492 STORE_FAST               3 (content)
          
-         322     >>  494 LOAD_FAST                8 (request)
+         318     >>  494 LOAD_FAST                8 (request)
                      496 POP_JUMP_FORWARD_IF_FALSE   113 (to 724)
          
-         324         498 LOAD_FAST                8 (request)
+         320         498 LOAD_FAST                8 (request)
                      500 LOAD_ATTR                9 (user)
                      510 LOAD_ATTR               10 (is_authenticated)
          
-         323         520 POP_JUMP_FORWARD_IF_FALSE    99 (to 720)
+         319         520 POP_JUMP_FORWARD_IF_FALSE    99 (to 720)
          
-         325         522 LOAD_FAST                8 (request)
+         321         522 LOAD_FAST                8 (request)
                      524 LOAD_ATTR                9 (user)
                      534 LOAD_METHOD             11 (has_perm)
                      556 LOAD_CONST               6 ('wagtailadmin.access_admin')
                      558 PRECALL                  1
                      562 CALL                     1
          
-         323         572 POP_JUMP_FORWARD_IF_FALSE    73 (to 720)
+         319         572 POP_JUMP_FORWARD_IF_FALSE    73 (to 720)
          
-         326         574 LOAD_FAST                8 (request)
+         322         574 LOAD_FAST                8 (request)
                      576 LOAD_ATTR                9 (user)
                      586 LOAD_METHOD             11 (has_perm)
                      608 LOAD_FAST                2 (model)
                      610 LOAD_ATTR               12 (_meta)
                      620 LOAD_ATTR               13 (app_label)
                      630 FORMAT_VALUE             0
                      632 LOAD_CONST               7 ('.change_')
@@ -1790,44 +1770,44 @@
                      636 LOAD_ATTR               12 (_meta)
                      646 LOAD_ATTR               14 (model_name)
                      656 FORMAT_VALUE             0
                      658 BUILD_STRING             3
                      660 PRECALL                  1
                      664 CALL                     1
          
-         323         674 POP_JUMP_FORWARD_IF_FALSE    22 (to 720)
+         319         674 POP_JUMP_FORWARD_IF_FALSE    22 (to 720)
          
-         327         676 LOAD_GLOBAL             11 (NULL + getattr)
+         323         676 LOAD_GLOBAL             11 (NULL + getattr)
                      688 LOAD_FAST                8 (request)
                      690 LOAD_GLOBAL             30 (FEDIT_PREVIEW_VAR)
                      702 LOAD_CONST               8 (False)
                      704 PRECALL                  3
                      708 CALL                     3
          
-         323         718 POP_JUMP_FORWARD_IF_TRUE     2 (to 724)
+         319         718 POP_JUMP_FORWARD_IF_TRUE     2 (to 724)
          
-         329     >>  720 LOAD_FAST                3 (content)
+         325     >>  720 LOAD_FAST                3 (content)
                      722 RETURN_VALUE
          
-         331     >>  724 LOAD_GLOBAL             33 (NULL + render_editable_field)
+         327     >>  724 LOAD_GLOBAL             33 (NULL + render_editable_field)
          
-         332         736 LOAD_FAST                8 (request)
+         328         736 LOAD_FAST                8 (request)
                      738 LOAD_FAST                3 (content)
          
-         333         740 LOAD_FAST                1 (field_name)
+         329         740 LOAD_FAST                1 (field_name)
                      742 LOAD_FAST                2 (model)
          
-         334         744 LOAD_FAST                0 (context)
+         330         744 LOAD_FAST                0 (context)
          
-         331         746 BUILD_TUPLE              5
+         327         746 BUILD_TUPLE              5
                      748 BUILD_MAP                0
          
-         335         750 LOAD_FAST                5 (extra)
+         331         750 LOAD_FAST                5 (extra)
          
-         331         752 DICT_MERGE               1
+         327         752 DICT_MERGE               1
                      754 CALL_FUNCTION_EX         1
                      756 RETURN_VALUE
          consts
             '\n    This tag is used to render an editable field.\n\n    This field will be wrapped and is able to be edited by the user on the frontend.\n\n    We will require the field_name of the field and the model instance.\n\n    Usage example:\n        ```python\n        {% fedit_field my_field_name page_instance %}\n        ```\n\n    Optionally your model can define a `render_fedit_{field_name}` method that will be used to render the field.\n    This will allow you to use custom rendering logic if need be.\n    '
             'Field name, and model are required'
             'request'
             'render_fedit_'
@@ -1838,15 +1818,15 @@
             False
          names      ('all', 'ValueError', 'items', 'get', 'hasattr', 'getattr', 'flatten', 'update', 'render_as_block', 'user', 'is_authenticated', 'has_perm', '_meta', 'app_label', 'model_name', 'FEDIT_PREVIEW_VAR', 'render_editable_field')
          varnames   ('context', 'field_name', 'model', 'content', 'kwargs', 'extra', 'key', 'value', 'request')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit_field'
-         firstlineno 282
+         firstlineno 278
          lnotab
             0x021222011e02040132010c032a01040126013a0220022001280220012a
             012a02040216ff020232fe020364fd02042afc020604020c010401040102
             fd040402fc
       code
          argcount  : 5
          nlocals   : 10
@@ -1866,135 +1846,135 @@
             084400a6000000ab0000000000000000007d087419000000000000000000
             00741b0000000000000000000064007c08a6020000ab0200000000000000
             00a6010000ab0100000000000000007d08741d0000000000000000000064
             067c067c027c037c017c047c0864079c067c05a5018900ac08a6030000ab
             0300000000000000005300
                        0 MAKE_CELL                0 (request)
          
-         338           2 RESUME                   0
+         334           2 RESUME                   0
          
-         339           4 LOAD_GLOBAL              1 (NULL + reverse)
+         335           4 LOAD_GLOBAL              1 (NULL + reverse)
          
-         340          16 LOAD_CONST               1 ('wagtail_fedit:edit_field')
+         336          16 LOAD_CONST               1 ('wagtail_fedit:edit_field')
          
-         341          18 LOAD_FAST                2 (field_name)
+         337          18 LOAD_FAST                2 (field_name)
                       20 LOAD_FAST                3 (model)
                       22 LOAD_ATTR                1 (_meta)
                       32 LOAD_ATTR                2 (app_label)
                       42 LOAD_FAST                3 (model)
                       44 LOAD_ATTR                1 (_meta)
                       54 LOAD_ATTR                3 (model_name)
                       64 LOAD_FAST                3 (model)
                       66 LOAD_ATTR                4 (pk)
                       76 BUILD_LIST               4
          
-         339          78 KW_NAMES                 2
+         335          78 KW_NAMES                 2
                       80 PRECALL                  2
                       84 CALL                     2
                       94 STORE_FAST               6 (edit_url)
          
-         344          96 LOAD_FAST                5 (kwargs)
+         340          96 LOAD_FAST                5 (kwargs)
                       98 POP_JUMP_FORWARD_IF_FALSE    37 (to 174)
          
-         345         100 LOAD_GLOBAL             11 (NULL + urlencode)
+         341         100 LOAD_GLOBAL             11 (NULL + urlencode)
          
-         346         112 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+         342         112 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                      124 LOAD_ATTR                7 (pack)
                      134 LOAD_CONST               9 (())
                      136 BUILD_MAP                0
                      138 LOAD_FAST                5 (kwargs)
                      140 DICT_MERGE               1
                      142 CALL_FUNCTION_EX         1
          
-         345         144 PRECALL                  1
+         341         144 PRECALL                  1
                      148 CALL                     1
                      158 STORE_FAST               7 (packed)
          
-         348         160 LOAD_FAST                6 (edit_url)
+         344         160 LOAD_FAST                6 (edit_url)
                      162 FORMAT_VALUE             0
                      164 LOAD_CONST               3 ('?')
                      166 LOAD_FAST                7 (packed)
                      168 FORMAT_VALUE             0
                      170 BUILD_STRING             3
                      172 STORE_FAST               6 (edit_url)
          
-         351     >>  174 LOAD_GLOBAL             17 (NULL + FeditFieldEditButton)
+         347     >>  174 LOAD_GLOBAL             17 (NULL + FeditFieldEditButton)
                      186 PRECALL                  0
                      190 CALL                     0
          
-         350         200 BUILD_LIST               1
+         346         200 BUILD_LIST               1
                      202 STORE_FAST               8 (items)
          
-         354         204 LOAD_GLOBAL             19 (NULL + hooks)
+         350         204 LOAD_GLOBAL             19 (NULL + hooks)
                      216 LOAD_ATTR               10 (get_hooks)
                      226 LOAD_GLOBAL             22 (CONSTRUCT_FIELD_TOOLBAR)
                      238 PRECALL                  1
                      242 CALL                     1
                      252 GET_ITER
                  >>  254 FOR_ITER                17 (to 290)
                      256 STORE_FAST               9 (hook)
          
-         355         258 PUSH_NULL
+         351         258 PUSH_NULL
                      260 LOAD_FAST                9 (hook)
                      262 LOAD_DEREF               0 (request)
                      264 LOAD_FAST                8 (items)
                      266 LOAD_FAST                3 (model)
                      268 LOAD_FAST                2 (field_name)
                      270 KW_NAMES                 4
                      272 PRECALL                  4
                      276 CALL                     4
                      286 POP_TOP
                      288 JUMP_BACKWARD           18 (to 254)
          
-         357     >>  290 LOAD_CLOSURE             0 (request)
+         353     >>  290 LOAD_CLOSURE             0 (request)
                      292 BUILD_TUPLE              1
-                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 357>)
+                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 353>)
                      296 MAKE_FUNCTION            8 (closure)
                      298 LOAD_FAST                8 (items)
                      300 GET_ITER
                      302 PRECALL                  0
                      306 CALL                     0
                      316 STORE_FAST               8 (items)
          
-         358         318 LOAD_GLOBAL             25 (NULL + list)
+         354         318 LOAD_GLOBAL             25 (NULL + list)
                      330 LOAD_GLOBAL             27 (NULL + filter)
                      342 LOAD_CONST               0 (None)
                      344 LOAD_FAST                8 (items)
                      346 PRECALL                  2
                      350 CALL                     2
                      360 PRECALL                  1
                      364 CALL                     1
                      374 STORE_FAST               8 (items)
          
-         360         376 LOAD_GLOBAL             29 (NULL + render_to_string)
+         356         376 LOAD_GLOBAL             29 (NULL + render_to_string)
          
-         361         388 LOAD_CONST               6 ('wagtail_fedit/content/editable_field.html')
+         357         388 LOAD_CONST               6 ('wagtail_fedit/content/editable_field.html')
          
-         363         390 LOAD_FAST                6 (edit_url)
+         359         390 LOAD_FAST                6 (edit_url)
          
-         364         392 LOAD_FAST                2 (field_name)
+         360         392 LOAD_FAST                2 (field_name)
          
-         365         394 LOAD_FAST                3 (model)
+         361         394 LOAD_FAST                3 (model)
          
-         366         396 LOAD_FAST                1 (content)
+         362         396 LOAD_FAST                1 (content)
          
-         367         398 LOAD_FAST                4 (context)
+         363         398 LOAD_FAST                4 (context)
          
-         368         400 LOAD_FAST                8 (items)
+         364         400 LOAD_FAST                8 (items)
          
-         362         402 LOAD_CONST               7 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items'))
+         358         402 LOAD_CONST               7 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items'))
                      404 BUILD_CONST_KEY_MAP      6
          
-         369         406 LOAD_FAST                5 (kwargs)
+         365         406 LOAD_FAST                5 (kwargs)
          
-         362         408 DICT_UPDATE              1
+         358         408 DICT_UPDATE              1
          
-         371         410 LOAD_DEREF               0 (request)
+         367         410 LOAD_DEREF               0 (request)
          
-         360         412 KW_NAMES                 8
+         356         412 KW_NAMES                 8
                      414 PRECALL                  3
                      418 CALL                     3
                      428 RETURN_VALUE
          consts
             None
             'wagtail_fedit:edit_field'
             ('args',)
@@ -2006,15 +1986,15 @@
                stacksize : 5
                flags     : 19
                code
                   0x9501970067007c005d177d017c01a00000000000000000000000000000
                   000000000000008902a6010000ab01000000000000000091028c185300
                              0 COPY_FREE_VARS           1
                
-               357           2 RESUME                   0
+               353           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                23 (to 56)
                             10 STORE_FAST               1 (item)
                             12 LOAD_FAST                1 (item)
                             14 LOAD_METHOD              0 (render)
                             36 LOAD_DEREF               2 (request)
@@ -2026,27 +2006,27 @@
                consts
                names      ('render',)
                varnames   ('.0', 'item')
                freevars   ('request',)
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '<listcomp>'
-               firstlineno 357
+               firstlineno 353
                lnotab 0x
             'wagtail_fedit/content/editable_field.html'
             ('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items')
             ('request',)
             ()
          names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack', 'FeditFieldEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_FIELD_TOOLBAR', 'list', 'filter', 'render_to_string')
          varnames   ('request', 'content', 'field_name', 'model', 'context', 'kwargs', 'edit_url', 'packed', 'items', 'hook')
          freevars   ()
          cellvars   ('request',)
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_editable_field'
-         firstlineno 338
+         firstlineno 334
          lnotab
             0x04010c0102013cfe120504010c0120ff10030e031aff0404360120021c
             013a020c0102020201020102010201020102fa040702f9020902f5
       'kwarg_list'
       'tokens'
       'return'
       code
@@ -2062,89 +2042,89 @@
             0064036b020000000072307c03720f7407000000000000000000006404a6
             010000ab01000000000000000082017c00a0040000000000000000000000
             0000000000000000007c06a6010000ab0100000000000000007c047c017c
             05190000000000000000003c0000008c5d7c076405190000000000000000
             007d087c00a00400000000000000000000000000000000000000007c0764
             0319000000000000000000a6010000ab0100000000000000007c047c083c
             00000064067d038c867c045300
-         374           0 RESUME                   0
+         370           0 RESUME                   0
          
-         375           2 LOAD_CONST               1 (False)
+         371           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               3 (had_kwargs)
          
-         376           6 BUILD_MAP                0
+         372           6 BUILD_MAP                0
                        8 STORE_FAST               4 (kwargs)
          
-         381          10 LOAD_GLOBAL              1 (NULL + enumerate)
+         377          10 LOAD_GLOBAL              1 (NULL + enumerate)
                       22 LOAD_FAST                2 (tokens)
                       24 PRECALL                  1
                       28 CALL                     1
                       38 GET_ITER
                  >>   40 FOR_ITER               133 (to 308)
                       42 UNPACK_SEQUENCE          2
                       46 STORE_FAST               5 (i)
                       48 STORE_FAST               6 (token)
          
-         382          50 LOAD_FAST                6 (token)
+         378          50 LOAD_FAST                6 (token)
                       52 LOAD_METHOD              1 (split)
                       74 LOAD_CONST               2 ('=')
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               7 (split)
          
-         383          92 LOAD_GLOBAL              5 (NULL + len)
+         379          92 LOAD_GLOBAL              5 (NULL + len)
                      104 LOAD_FAST                7 (split)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               3 (1)
                      122 COMPARE_OP               2 (==)
                      128 POP_JUMP_FORWARD_IF_FALSE    48 (to 226)
          
-         384         130 LOAD_FAST                3 (had_kwargs)
+         380         130 LOAD_FAST                3 (had_kwargs)
                      132 POP_JUMP_FORWARD_IF_FALSE    15 (to 164)
          
-         385         134 LOAD_GLOBAL              7 (NULL + ValueError)
+         381         134 LOAD_GLOBAL              7 (NULL + ValueError)
                      146 LOAD_CONST               4 ('Unexpected positional argument after keyword argument')
                      148 PRECALL                  1
                      152 CALL                     1
                      162 RAISE_VARARGS            1
          
-         387     >>  164 LOAD_FAST                0 (parser)
+         383     >>  164 LOAD_FAST                0 (parser)
                      166 LOAD_METHOD              4 (compile_filter)
                      188 LOAD_FAST                6 (token)
                      190 PRECALL                  1
                      194 CALL                     1
                      204 LOAD_FAST                4 (kwargs)
                      206 LOAD_FAST                1 (kwarg_list)
                      208 LOAD_FAST                5 (i)
                      210 BINARY_SUBSCR
                      220 STORE_SUBSCR
                      224 JUMP_BACKWARD           93 (to 40)
          
-         389     >>  226 LOAD_FAST                7 (split)
+         385     >>  226 LOAD_FAST                7 (split)
                      228 LOAD_CONST               5 (0)
                      230 BINARY_SUBSCR
                      240 STORE_FAST               8 (key)
          
-         393         242 LOAD_FAST                0 (parser)
+         389         242 LOAD_FAST                0 (parser)
                      244 LOAD_METHOD              4 (compile_filter)
                      266 LOAD_FAST                7 (split)
                      268 LOAD_CONST               3 (1)
                      270 BINARY_SUBSCR
                      280 PRECALL                  1
                      284 CALL                     1
                      294 LOAD_FAST                4 (kwargs)
                      296 LOAD_FAST                8 (key)
                      298 STORE_SUBSCR
          
-         394         302 LOAD_CONST               6 (True)
+         390         302 LOAD_CONST               6 (True)
                      304 STORE_FAST               3 (had_kwargs)
                      306 JUMP_BACKWARD          134 (to 40)
          
-         396     >>  308 LOAD_FAST                4 (kwargs)
+         392     >>  308 LOAD_FAST                4 (kwargs)
                      310 RETURN_VALUE
          consts
             None
             False
             '='
             1
             'Unexpected positional argument after keyword argument'
@@ -2152,74 +2132,74 @@
             True
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter')
          varnames   ('parser', 'kwarg_list', 'tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 374
+         firstlineno 370
          lnotab 0x02010401040528012a01260104011e023e0210043c010602
       code
          argcount  : 3
          nlocals   : 5
          stacksize : 5
          flags     : 15
          code
             0x97007c017c00760072087c007c01190000000000000000005300740100
             0000000000000000007c02a6010000ab010000000000000000720802007c
             027c0369007c04a4018e017d027c027c007c013c0000007c025300
-         401           0 RESUME                   0
+         397           0 RESUME                   0
          
-         402           2 LOAD_FAST                1 (key)
+         398           2 LOAD_FAST                1 (key)
                        4 LOAD_FAST                0 (context)
                        6 CONTAINS_OP              0
                        8 POP_JUMP_FORWARD_IF_FALSE     8 (to 26)
          
-         403          10 LOAD_FAST                0 (context)
+         399          10 LOAD_FAST                0 (context)
                       12 LOAD_FAST                1 (key)
                       14 BINARY_SUBSCR
                       24 RETURN_VALUE
          
-         405     >>   26 LOAD_GLOBAL              1 (NULL + callable)
+         401     >>   26 LOAD_GLOBAL              1 (NULL + callable)
                       38 LOAD_FAST                2 (value)
                       40 PRECALL                  1
                       44 CALL                     1
                       54 POP_JUMP_FORWARD_IF_FALSE     8 (to 72)
          
-         406          56 PUSH_NULL
+         402          56 PUSH_NULL
                       58 LOAD_FAST                2 (value)
                       60 LOAD_FAST                3 (args)
                       62 BUILD_MAP                0
                       64 LOAD_FAST                4 (kwargs)
                       66 DICT_MERGE               1
                       68 CALL_FUNCTION_EX         1
                       70 STORE_FAST               2 (value)
          
-         408     >>   72 LOAD_FAST                2 (value)
+         404     >>   72 LOAD_FAST                2 (value)
                       74 LOAD_FAST                0 (context)
                       76 LOAD_FAST                1 (key)
                       78 STORE_SUBSCR
          
-         409          82 LOAD_FAST                2 (value)
+         405          82 LOAD_FAST                2 (value)
                       84 RETURN_VALUE
          consts
             None
          names      ('callable',)
          varnames   ('context', 'key', 'value', 'args', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       '_get_from_context_or_set'
-         firstlineno 401
+         firstlineno 397
          lnotab 0x0201080110021e0110020a01
       (None,)
-   names      ('django.template', 'library', 'Node', 'NodeList', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'TokenType', 'FilterExpression', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'django.db', 'models', 'wagtail.blocks', 'BoundBlock', 'wagtail.models', 'Page', 'wagtail', 'hooks', 'urllib.parse', 'urlencode', 'toolbar', 'FeditBlockEditButton', 'FeditFieldEditButton', 'block_forms.utils', 'can_fedit', 'utils', 'FEDIT_PREVIEW_VAR', 'CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR', 'Library', 'register', 'TimestampSigner', 'url_value_signer', 'BlockEditNode', 'tag', 'do_render_fedit_block', 'simple_tag', 'do_render_fedit_field', 'render_editable_field', 'list', 'str', 'dict', 'get_kwargs', '_get_from_context_or_set')
+   names      ('django.template', 'library', 'Node', 'NodeList', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'TokenType', 'FilterExpression', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'django.db', 'models', 'wagtail.blocks', 'BoundBlock', 'wagtail.models', 'Page', 'wagtail', 'hooks', 'urllib.parse', 'urlencode', 'toolbar', 'FeditBlockEditButton', 'FeditFieldEditButton', 'utils', 'FEDIT_PREVIEW_VAR', 'CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR', 'Library', 'register', 'TimestampSigner', 'url_value_signer', 'BlockEditNode', 'tag', 'do_render_fedit_block', 'simple_tag', 'do_render_fedit_field', 'render_editable_field', 'list', 'str', 'dict', 'get_kwargs', '_get_from_context_or_set')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020114010c0114010c010c010c010c010c020c010c010c010c0210
-      040c010c0110061e021e031c7f003d2a010eff0e01023d2c0106ff0e0102
-      370624301b
+      040c0110061e021e031c7f003a2a010eff0e01023d2c0106ff0e01023706
+      24301b
```

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.0.4/wagtail_fedit/templatetags/fedit.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from wagtail import hooks
 from urllib.parse import urlencode
 
 from ..toolbar import (
     FeditBlockEditButton,
     FeditFieldEditButton,
 )
-from ..block_forms.utils import can_fedit
 from ..utils import FEDIT_PREVIEW_VAR
 from ..hooks import (
     CONSTRUCT_BLOCK_TOOLBAR,
     CONSTRUCT_FIELD_TOOLBAR,
 )
 
 
@@ -92,17 +91,14 @@
             self.has_block = True
         elif self.nl:
             rendered = self.nl.render(context)
             self.has_block = context.get("wagtail_fedit_has_block", False)
         else:
             raise ValueError("Block or nodelist is required")
         
-        if block and not can_fedit(block):
-            return rendered
-
         # Get block id from block if bound or context.
         if not block_id and "block_id" in context:
             block_id = context["block_id"]
         elif not block_id and block and hasattr(block, "id"):
             block_id = block.id
         elif not block_id:
             raise ValueError("Block ID is required")
```

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.0.4/wagtail_fedit/tests/test_blocks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.test import TestCase
 from django import forms
 from wagtail import blocks
-from .. import block_forms
+from .. import forms as block_forms
+from .. import utils
 
 TEST_BLOCK_DATA = [
     {
         "type": "heading_component",
         "value": {
             "heading": "This is pretty cool!!!",
             "subheading": "RIGHT?! FUCK YES!"
@@ -154,132 +155,104 @@
         self.stream_block = blocks.StreamBlock([
             ("heading_component", HeadingComponent()),
             ("flat_menu_component", FlatMenuComponent())
         ])
         self.stream_value = self.stream_block.to_python(TEST_BLOCK_DATA)
 
     def test_find_block(self):
-        block, contentpath = block_forms.find_block("d543a6bf-34dc-4365-a3fa-d302561930ae", self.stream_value)
+        block, contentpath = utils.find_block("d543a6bf-34dc-4365-a3fa-d302561930ae", self.stream_value)
         self.assertEqual(block.value["heading"], "AWESOME!!")
         self.assertEqual(block.value["subheading"], "RIGHT?!")
 
-        block, contentpath = block_forms.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)
+        block, contentpath = utils.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)
         self.assertEqual(block.value["link"]["text"], "Test Item 3")
         self.assertEqual(contentpath, ["3e9144fd-5fa5-47f8-917e-8fe87c15da01", "items", "a98a19c6-2ead-4e69-9ea2-3158c7e82976"])
 
         item = self.stream_block.get_block_by_content_path(self.stream_value, contentpath)
         self.assertEqual(item.value["link"]["text"], "Test Item 3")
 
-        block, contentpath = block_forms.find_block("invalid-id", self.stream_value)
+        block, contentpath = utils.find_block("invalid-id", self.stream_value)
         self.assertIsNone(block)
         self.assertEqual(contentpath, [])
 
     def test_get_form_class(self):
-        block = block_forms.find_block("d543a6bf-34dc-4365-a3fa-d302561930ae", self.stream_value)[0]
-        form_class = block_forms.get_form_class(block, block.block, request=FakeRequest())
+        block = utils.find_block("d543a6bf-34dc-4365-a3fa-d302561930ae", self.stream_value)[0]
+        form_class = block_forms.get_block_form_class(block.block)
         self.assertIsNotNone(form_class)
 
-        fields = {
-            "heading": forms.CharField(max_length=25),
-            "subheading": forms.CharField(max_length=40)
-        }
-
-        for name, field in form_class.base_fields.items():
-            self.assertIsInstance(field, fields[name].__class__)
-
         VALID_DATA = {
-            "heading": "New Heading",
-            "subheading": "New Subheading"
+            "value-heading": "New Heading",
+            "value-subheading": "New Subheading"
         }
 
         INVALID_DATA = {
-            "heading": "New Heading",
-            "subheading": "New Subheading" * 10
+            "value-heading": "New Heading",
+            "value-subheading": "New Subheading" * 10
         }
 
-        valid_form = form_class(data=VALID_DATA, block=block, parent_instance=FakeModel(), request=FakeRequest(method="POST", POST=VALID_DATA))
+        valid_form = form_class(data=VALID_DATA, block=block, parent_instance=FakeModel())
         self.assertTrue(valid_form.is_valid())
 
-        invalid_form = form_class(data=INVALID_DATA, block=block, parent_instance=FakeModel(), request=FakeRequest(method="POST", POST=INVALID_DATA))
+        invalid_form = form_class(data=INVALID_DATA, block=block, parent_instance=FakeModel())
         self.assertFalse(invalid_form.is_valid())
 
     def test_get_subblock_form_class(self):
-        block = block_forms.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)[0]
-        form_class = block_forms.get_form_class(block, block.block, request=FakeRequest())
+        block = utils.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)[0]
+        form_class = block_forms.get_block_form_class(block.block)
         self.assertIsNotNone(form_class)
 
-        fields = {
-            "link": block_forms.BlockEditSubFormField
-        }
-
-        subfields = {
-            "text": forms.CharField(max_length=25)
-        }
-
-        for name, field in form_class.base_fields.items():
-            self.assertIsInstance(field, fields[name])
-
-        field = form_class.declared_fields["link"]
-        self.assertIsInstance(field, block_forms.BlockEditSubFormField)
-        self.assertIsInstance(field.form, block_forms.BaseBlockEditForm)
-
-        for name, field in field.form.base_fields.items():
-            self.assertIsInstance(field, subfields[name].__class__)
-
         VALID_DATA = {
-            "link-text": "New Link Text"
+            "value-link-text": "New Link Text"
         }
 
         INVALID_DATA = {
-            "link-text": ["New Link Text" * 10]
+            "value-link-text": ["New Link Text" * 10]
         }
 
 
-        valid_form = form_class(data=VALID_DATA, block=block, parent_instance=FakeModel(), request=FakeRequest(method="POST"))
+        valid_form = form_class(data=VALID_DATA, block=block, parent_instance=FakeModel())
         if not valid_form.is_valid():
             self.fail((
                 valid_form.errors.items(),
                 valid_form.non_field_errors()
             ))
 
         valid_form.save()
         self.assertEqual(block.value["link"]["text"], "New Link Text")
 
-        invalid_form = form_class(data=INVALID_DATA, block=block, parent_instance=FakeModel(), request=FakeRequest(method="POST"))
+        invalid_form = form_class(data=INVALID_DATA, block=block, parent_instance=FakeModel())
         self.assertFalse(invalid_form.is_valid())
 
 
     def test_block_form_save(self):
-        block = block_forms.find_block("d543a6bf-34dc-4365-a3fa-d302561930ae", self.stream_value)[0]
-        form_class = block_forms.get_form_class(block, block.block, request=FakeRequest())
+        block = utils.find_block("d543a6bf-34dc-4365-a3fa-d302561930ae", self.stream_value)[0]
+        form_class = block_forms.get_block_form_class(block.block)
 
         VALID_DATA = {
-            "heading": "New Heading",
-            "subheading": "New Subheading"
+            "value-heading": "New Heading",
+            "value-subheading": "New Subheading"
         }
 
-        valid_form = form_class(data=VALID_DATA, block=block, parent_instance=FakeModel(), request=FakeRequest(method="POST"))
+        valid_form = form_class(data=VALID_DATA, block=block, parent_instance=FakeModel())
         if not valid_form.is_valid():
             self.fail((valid_form.errors.items(), valid_form.non_field_errors()))
 
         valid_form.save()
         self.assertEqual(block.value["heading"], "New Heading")
         self.assertEqual(block.value["subheading"], "New Subheading")
 
 
     def test_subblock_form_save(self):
-        block = block_forms.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)[0]
-        form_class = block_forms.get_form_class(block, block.block, request=FakeRequest())
+        block = utils.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)[0]
+        form_class = block_forms.get_block_form_class(block.block)
 
         VALID_DATA = {
-            "link-text": "New Link Text"
+            "value-link-text": "New Link Text"
         }
 
-        valid_form = form_class(data=VALID_DATA, block=block, parent_instance=FakeModel(), request=FakeRequest(method="POST"))
+        valid_form = form_class(data=VALID_DATA, block=block, parent_instance=FakeModel())
         if not valid_form.is_valid():
-            self.fail((
-                valid_form.errors.items(),
-                valid_form.non_field_errors()
-            ))
+            errors = valid_form.errors.as_data()["value"][0].as_json_data()
+            self.fail((errors, valid_form.non_field_errors()))
 
         valid_form.save()
         self.assertEqual(block.value["link"]["text"], "New Link Text")
```

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.0.4/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/urls.py` & `wagtail_fedit-1.0.4/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.0.4/wagtail_fedit/views/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,22 @@
 from django.apps import apps
 
 from wagtail.fields import StreamValue
 from wagtail.models import RevisionMixin, Page
 from wagtail.admin.views.generic import WagtailAdminTemplateMixin
 from wagtail.log_actions import log
 from ..templatetags.fedit import BlockEditNode
-from .. import block_forms as block_forms
-from ..utils import (
-    FeditPermissionCheck,
-    FEDIT_PREVIEW_VAR,
-)
+from .. import forms as block_forms
+from .. import utils
 
 
 
 @method_decorator(xframe_options_sameorigin, name="dispatch")
-class EditBlockView(FeditPermissionCheck, WagtailAdminTemplateMixin, View):
-    template_name = "wagtail_fedit/editor/iframe.html"
+class EditBlockView(utils.FeditPermissionCheck, WagtailAdminTemplateMixin, View):
+    template_name = "wagtail_fedit/editor/block_iframe.html"
 
     def dispatch(self, request: HttpRequest, block_id = None, field_name = None, model_id = None, model_name = None, app_label = None) -> None:
 
         self.edit_args = ["block_id", "field_name", "model_id", "model_name", "app_label"]
         if not all([block_id, field_name, model_id, model_name, app_label]):
             return HttpResponseBadRequest("Missing required parameters")
         
@@ -55,22 +52,22 @@
             self.instance = self.model_instance.latest_revision.as_object()
         else:
             self.instance = self.model._default_manager.get(pk=self.model_id)
             self.model_instance = self.instance
 
 
         self.streamfield: StreamValue = getattr(self.instance, self.field_name)
-        result = block_forms.find_block(self.block_id, self.streamfield)
+        result = utils.find_block(self.block_id, self.streamfield)
         if not result:
             # raise ValueError("Block not found; did you provide the correct block ID?")
             return HttpResponseBadRequest("Block not found; did you provide the correct block ID?")
 
 
         self.block, self.contentpath = result
-        self.form_class = block_forms.get_form_class(self.block, self.block.block, request)
+        self.form_class = block_forms.get_block_form_class(self.block.block)
 
 
         if not self.form_class:
             return HttpResponseBadRequest("Invalid block type")
 
         return super().dispatch(request, block_id, field_name, model_id, model_name, app_label)
 
@@ -158,26 +155,26 @@
             success=True,
         )
 
     def post(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         form = self.form_class(request.POST, block=self.block, parent_instance=self.instance, request=request)
 
         # Set the preview flag to mark as editable block when re-rendering.
-        setattr(request, FEDIT_PREVIEW_VAR, True)
+        setattr(request, utils.FEDIT_PREVIEW_VAR, True)
 
         valid = form.is_valid()
         if valid:
             self.block = form.save()
         else:
             # We are not rendering the content, so we can omit data from context.
             return JsonResponse({
                 "success": False,
                 "errors": form.errors,
                 "html": render_to_string(
-                    "wagtail_fedit/editor/iframe.html",
+                    "wagtail_fedit/editor/block_iframe.html",
                     context=self.get_context_data(form=form),
                     request=request,
                 )
             })
         
         extra_log_kwargs = {}
         if isinstance(self.instance, RevisionMixin):
```

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.0.4/wagtail_fedit/views/editable.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from wagtail.admin.views.generic import WagtailAdminTemplateMixin
 from wagtail.models import (
     RevisionMixin,
     PreviewableMixin,
     DraftStateMixin,
 )
-from .. import block_forms as block_forms
+from .. import forms as block_forms
 from ..utils import (
     FEDIT_PREVIEW_VAR,
     USERBAR_MODEL_VAR,
     FeditPermissionCheck,
     with_userbar_model,
 )
```

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.0.4/wagtail_fedit/views/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,80 +15,35 @@
 from django.apps import apps
 
 from wagtail.log_actions import log
 from wagtail.models import (
     RevisionMixin, 
 )
 from wagtail.admin.views.generic import WagtailAdminTemplateMixin
-from wagtail.admin.forms import (
-    WagtailAdminModelForm,
-)
 
 import uuid
 
 from ..templatetags.fedit import (
     BlockEditNode,
     render_editable_field,
 )
-from .. import block_forms as block_forms
+from ..forms import (
+    blocks as block_forms,
+    fields as field_forms,
+)
 from ..utils import (
     FeditPermissionCheck,
     use_related_form,
 )
 
 
-class PossiblePreviewForm(WagtailAdminModelForm):
-    def __init__(self, *args, request = None, **kwargs):
-        self.request = request
-        super().__init__(*args, **kwargs)
-
-    def save(self, commit=True):
-        instance = super().save(commit=False)
-        if commit:
-            instance = save_possible_revision(instance, self.request)
-        return instance
-
-def save_possible_revision(instance: models.Model, request: HttpRequest, **kwargs) -> models.Model:
-    if isinstance(instance, RevisionMixin):
-        instance = instance.save_revision(
-            user=request.user,
-            **kwargs,
-        )
-        instance = instance.as_object()
-    else:
-        instance.save()
-
-    return instance
-
-def get_form_class_for_fields(form_model: models.Model, form_fields: list[str]) -> Type[WagtailAdminModelForm]:
-
-    if hasattr(form_model, "get_fedit_form"):
-        return form_model.get_fedit_form(form_fields)
-
-    class Form(PossiblePreviewForm):
-        class Meta:
-            model = form_model
-            fields = form_fields
-
-    return Form
-
-
-def get_model_string(instance: models.Model) -> str:
-    model_string = getattr(instance, "get_admin_display_title", None)
-    if model_string:
-        model_string = model_string()
-    else:
-        model_string = getattr(instance, "title", str(instance))
-
-    return model_string
-
 
 @method_decorator(xframe_options_sameorigin, name="dispatch")
 class EditFieldView(FeditPermissionCheck, WagtailAdminTemplateMixin, View):
-    template_name = "wagtail_fedit/editor/iframe.html"
+    template_name = "wagtail_fedit/editor/field_iframe.html"
 
     def dispatch(self, request: HttpRequest, field_name = None, app_label = None, model_name = None, model_id = None) -> None:
         if not all([field_name, model_name, app_label, model_id]):
             return HttpResponseBadRequest("Missing required parameters")
 
         self.model = apps.get_model(app_label, model_name)
         if not self.has_perms(request, self.model):
@@ -114,35 +69,35 @@
 
         # Check if the field is a relation and if the value is a model
         # for the field instead of the form for the relation.
         if self.meta_field.is_relation and use_related_form(self.meta_field):
             # If the field is a model, we want to edit the model itself
             # We can do this by getting the fields from the model
             self.instance = self.field_value
-            self.form_class = get_form_class_for_fields(
+            self.form_class = field_forms.get_form_class_for_fields(
                 self.meta_field.related_model,
                 getattr(
                     self.meta_field.related_model,
                     "fedit_fields", "__all__"
                 ),
             )
         else:
-            self.form_class = get_form_class_for_fields(
+            self.form_class = field_forms.get_form_class_for_fields(
                 self.model,
                 [field_name],
             )
 
         return super().dispatch(request, field_name, model_name, app_label, model_id)
 
     def get_page_title(self):
         meta_field: models.Field = self.model._meta.get_field(self.field_name)
 
-        model_string = get_model_string(self.original_instance)
+        model_string = field_forms.get_model_string(self.original_instance)
         if self.original_instance != self.instance:
-            instance_string = get_model_string(self.instance)
+            instance_string = field_forms.get_model_string(self.instance)
             return _("Edit model %(instance_string)s for %(model_name)s %(model_string)s") % {
                 "instance_string": instance_string,
                 "model_name": self.model._meta.verbose_name,
                 "model_string": model_string,
             }
 
         return _("Edit field %(field_name)s for %(model_name)s %(model_string)s") % {
@@ -194,39 +149,39 @@
             
             # add data to context
             context = self.get_context_data(form=form, **self.data)
 
             # Check if we are saving a relation
             if self.instance.pk != self.original_instance.pk:
                 self.meta_field.save_form_data(self.original_instance, self.instance)
-                save_possible_revision(self.original_instance, request)
+                field_forms.save_possible_revision(self.original_instance, request)
 
             extra_log_kwargs = {}
             if isinstance(self.original_instance, RevisionMixin):
                 extra_log_kwargs["revision"] = self.original_instance.latest_revision
 
             data = {
                 "verbose_field_name": self.meta_field.verbose_name,
                 "field_name": self.field_name,
                 "model_id": self.model_id,
                 "model_name": self.model_name,
                 "app_label": self.app_label,
                 "model_verbose": str(self.model._meta.verbose_name),
-                "model_string": str(get_model_string(self.original_instance)),
+                "model_string": str(field_forms.get_model_string(self.original_instance)),
                 "old": str(self.initial_field_value),
                 "new": str(getattr(
                     self.original_instance,
                     self.field_name
                 )),
             }
 
             uid = uuid.uuid4()
             if self.original_instance.pk != self.instance.pk:
                 data.update({
-                    "edited_model_string": str(get_model_string(self.instance)),
+                    "edited_model_string": str(field_forms.get_model_string(self.instance)),
                     "edited_model_verbose": str(self.instance._meta.verbose_name),
                     "edited_model_id": self.instance.pk,
                     "edited_model_name": self.instance._meta.model_name,
                     "edited_app_label": self.instance._meta.app_label,
                 })
 
                 log(
@@ -272,13 +227,13 @@
                 "html": html,
             })
 
         return JsonResponse({
             "success": False,
             "errors": form.errors,
             "html": render_to_string(
-                "wagtail_fedit/editor/iframe.html",
+                "wagtail_fedit/editor/field_iframe.html",
                 context=self.get_context_data(form=form),
                 request=request,
             )
         })
```

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.0.4/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.0.4/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.0.3
+Version: 1.0.4
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.0.3/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.0.4/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,31 +25,32 @@
 wagtail_fedit/urls.py
 wagtail_fedit/utils.py
 wagtail_fedit.egg-info/PKG-INFO
 wagtail_fedit.egg-info/SOURCES.txt
 wagtail_fedit.egg-info/dependency_links.txt
 wagtail_fedit.egg-info/requires.txt
 wagtail_fedit.egg-info/top_level.txt
-wagtail_fedit/block_forms/__init__.py
-wagtail_fedit/block_forms/field_conversions.py
-wagtail_fedit/block_forms/forms.py
-wagtail_fedit/block_forms/subform_field.py
-wagtail_fedit/block_forms/utils.py
+wagtail_fedit/forms/__init__.py
+wagtail_fedit/forms/blocks.py
+wagtail_fedit/forms/fields.py
 wagtail_fedit/migrations/__init__.py
 wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/static/wagtail_fedit/css/admin.css
 wagtail_fedit/static/wagtail_fedit/css/frontend.css
 wagtail_fedit/static/wagtail_fedit/css/furniture.css
 wagtail_fedit/static/wagtail_fedit/js/frontend.js
 wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
+wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/field.html
-wagtail_fedit/templates/wagtail_fedit/editor/iframe.html
+wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
 wagtail_fedit/templatetags/__init__.py
 wagtail_fedit/templatetags/fedit.py
 wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
```

