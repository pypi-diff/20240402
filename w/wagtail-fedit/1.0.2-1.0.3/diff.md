# Comparing `tmp/wagtail_fedit-1.0.2.tar.gz` & `tmp/wagtail_fedit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.0.2.tar", last modified: Mon Apr  1 22:43:52 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.0.3.tar", last modified: Tue Apr  2 07:15:22 2024, max compression
```

## Comparing `wagtail_fedit-1.0.2.tar` & `wagtail_fedit-1.0.3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.453600 wagtail_fedit-1.0.2/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1326 2024-04-01 22:43:52.453600 wagtail_fedit-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-04-01 21:38:14.000000 wagtail_fedit-1.0.2/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-01 22:43:52.462546 wagtail_fedit-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.033976 wagtail_fedit-1.0.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.050473 wagtail_fedit-1.0.2/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.050981 wagtail_fedit-1.0.2/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.050981 wagtail_fedit-1.0.2/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.081209 wagtail_fedit-1.0.2/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.2/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.150096 wagtail_fedit-1.0.2/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.2/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.2/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.2/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.224842 wagtail_fedit-1.0.2/wagtail_fedit/block_forms/
--rw-rw-rw-   0        0        0      334 2024-03-30 17:06:54.000000 wagtail_fedit-1.0.2/wagtail_fedit/block_forms/__init__.py
--rw-rw-rw-   0        0        0     1471 2024-03-30 18:10:34.000000 wagtail_fedit-1.0.2/wagtail_fedit/block_forms/field_conversions.py
--rw-rw-rw-   0        0        0     7932 2024-04-01 21:09:37.000000 wagtail_fedit-1.0.2/wagtail_fedit/block_forms/forms.py
--rw-rw-rw-   0        0        0     2369 2024-04-01 22:35:55.000000 wagtail_fedit-1.0.2/wagtail_fedit/block_forms/subform_field.py
--rw-rw-rw-   0        0        0     4397 2024-04-01 20:14:21.000000 wagtail_fedit-1.0.2/wagtail_fedit/block_forms/utils.py
--rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.0.2/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.224842 wagtail_fedit-1.0.2/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.2/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.224842 wagtail_fedit-1.0.2/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.2/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.017845 wagtail_fedit-1.0.2/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.017845 wagtail_fedit-1.0.2/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.239606 wagtail_fedit-1.0.2/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.0.2/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.0.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.0.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.262201 wagtail_fedit-1.0.2/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    10317 2024-04-01 16:03:33.000000 wagtail_fedit-1.0.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.017845 wagtail_fedit-1.0.2/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.017845 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.274772 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.287494 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.303544 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      570 2024-04-01 16:14:23.000000 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     3381 2024-04-01 22:42:04.000000 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/editor/iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.335009 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-01 14:29:21.000000 wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.335009 wagtail_fedit-1.0.2/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.0.2/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.335009 wagtail_fedit-1.0.2/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16748 2024-04-01 17:25:24.000000 wagtail_fedit-1.0.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13455 2024-04-01 17:25:22.000000 wagtail_fedit-1.0.2/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.350876 wagtail_fedit-1.0.2/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.0.2/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     9934 2024-04-01 21:23:20.000000 wagtail_fedit-1.0.2/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0       63 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.2/wagtail_fedit/tests.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.0.2/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.0.2/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     1236 2024-04-01 18:06:46.000000 wagtail_fedit-1.0.2/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.382547 wagtail_fedit-1.0.2/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.0.2/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8544 2024-04-01 18:38:00.000000 wagtail_fedit-1.0.2/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5329 2024-04-01 18:17:22.000000 wagtail_fedit-1.0.2/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    10807 2024-04-01 18:29:15.000000 wagtail_fedit-1.0.2/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.448557 wagtail_fedit-1.0.2/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      131 2024-04-01 18:07:12.000000 wagtail_fedit-1.0.2/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      394 2024-03-31 07:07:45.000000 wagtail_fedit-1.0.2/wagtail_fedit/wagtail_hooks/editorjs.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.0.2/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.0.2/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.0.2/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     2544 2024-04-01 20:53:54.000000 wagtail_fedit-1.0.2/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:43:52.449913 wagtail_fedit-1.0.2/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     1326 2024-04-01 22:43:51.000000 wagtail_fedit-1.0.2/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2511 2024-04-01 22:43:51.000000 wagtail_fedit-1.0.2/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 22:43:51.000000 wagtail_fedit-1.0.2/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-01 22:43:51.000000 wagtail_fedit-1.0.2/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-01 22:43:51.000000 wagtail_fedit-1.0.2/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.478103 wagtail_fedit-1.0.3/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1326 2024-04-02 07:15:22.478103 wagtail_fedit-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-04-01 21:38:14.000000 wagtail_fedit-1.0.3/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-02 07:15:22.486410 wagtail_fedit-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.072783 wagtail_fedit-1.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.081958 wagtail_fedit-1.0.3/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.093043 wagtail_fedit-1.0.3/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.094025 wagtail_fedit-1.0.3/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.130842 wagtail_fedit-1.0.3/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.0.3/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.195253 wagtail_fedit-1.0.3/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.3/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.3/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.3/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.252001 wagtail_fedit-1.0.3/wagtail_fedit/block_forms/
+-rw-rw-rw-   0        0        0      334 2024-03-30 17:06:54.000000 wagtail_fedit-1.0.3/wagtail_fedit/block_forms/__init__.py
+-rw-rw-rw-   0        0        0     1471 2024-03-30 18:10:34.000000 wagtail_fedit-1.0.3/wagtail_fedit/block_forms/field_conversions.py
+-rw-rw-rw-   0        0        0     7932 2024-04-01 21:09:37.000000 wagtail_fedit-1.0.3/wagtail_fedit/block_forms/forms.py
+-rw-rw-rw-   0        0        0     2369 2024-04-01 22:35:55.000000 wagtail_fedit-1.0.3/wagtail_fedit/block_forms/subform_field.py
+-rw-rw-rw-   0        0        0     4397 2024-04-01 20:14:21.000000 wagtail_fedit-1.0.3/wagtail_fedit/block_forms/utils.py
+-rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.0.3/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.254163 wagtail_fedit-1.0.3/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.3/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.257162 wagtail_fedit-1.0.3/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.3/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.059292 wagtail_fedit-1.0.3/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.060805 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.275092 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.289250 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    10317 2024-04-01 16:03:33.000000 wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.060805 wagtail_fedit-1.0.3/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.062267 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.301273 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.316065 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.335774 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      570 2024-04-01 16:14:23.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     3381 2024-04-02 06:48:17.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/editor/iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.352080 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-01 14:29:21.000000 wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.362945 wagtail_fedit-1.0.3/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.0.3/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.366946 wagtail_fedit-1.0.3/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.0.3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16748 2024-04-02 07:08:47.000000 wagtail_fedit-1.0.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13455 2024-04-02 07:08:45.000000 wagtail_fedit-1.0.3/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.380686 wagtail_fedit-1.0.3/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.0.3/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     9934 2024-04-01 21:23:20.000000 wagtail_fedit-1.0.3/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0       63 2024-03-29 20:13:25.000000 wagtail_fedit-1.0.3/wagtail_fedit/tests.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.0.3/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.0.3/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     1236 2024-04-01 18:06:46.000000 wagtail_fedit-1.0.3/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.412934 wagtail_fedit-1.0.3/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.0.3/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8713 2024-04-02 07:11:24.000000 wagtail_fedit-1.0.3/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5329 2024-04-02 07:10:16.000000 wagtail_fedit-1.0.3/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    10807 2024-04-01 18:29:15.000000 wagtail_fedit-1.0.3/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.475946 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      131 2024-04-01 18:07:12.000000 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      394 2024-03-31 07:07:45.000000 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/editorjs.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     2544 2024-04-01 20:53:54.000000 wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:15:22.476876 wagtail_fedit-1.0.3/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     1326 2024-04-02 07:15:21.000000 wagtail_fedit-1.0.3/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2511 2024-04-02 07:15:22.000000 wagtail_fedit-1.0.3/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 07:15:21.000000 wagtail_fedit-1.0.3/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-02 07:15:21.000000 wagtail_fedit-1.0.3/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-02 07:15:21.000000 wagtail_fedit-1.0.3/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.0.2/LICENSE` & `wagtail_fedit-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/PKG-INFO` & `wagtail_fedit-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.0.2
+Version: 1.0.3
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.0.2/setup.cfg` & `wagtail_fedit-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
-00000030: 320d 0a64 6573 6372 6970 7469 6f6e 203d  2..description =
+00000030: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.0.2/tests/testapp/manage.py` & `wagtail_fedit-1.0.3/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.0.3/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.0.3/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/block_forms/field_conversions.py` & `wagtail_fedit-1.0.3/wagtail_fedit/block_forms/field_conversions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/block_forms/forms.py` & `wagtail_fedit-1.0.3/wagtail_fedit/block_forms/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/block_forms/subform_field.py` & `wagtail_fedit-1.0.3/wagtail_fedit/block_forms/subform_field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/block_forms/utils.py` & `wagtail_fedit-1.0.3/wagtail_fedit/block_forms/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.0.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/editor/field.html` & `wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/editor/field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/editor/iframe.html` & `wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/editor/iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.0.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.0.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x02ee0a66 (Mon Apr  1 17:25:22 2024 UTC)
+moddate:  0xfdae0b66 (Tue Apr  2 07:08:45 2024 UTC)
 files sz: 13455
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.0.3/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.0.3/wagtail_fedit/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.0.3/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/urls.py` & `wagtail_fedit-1.0.3/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/utils.py` & `wagtail_fedit-1.0.3/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.0.3/wagtail_fedit/views/blocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 
 from wagtail.fields import StreamValue
 from wagtail.models import RevisionMixin, Page
 from wagtail.admin.views.generic import WagtailAdminTemplateMixin
 from wagtail.log_actions import log
 from ..templatetags.fedit import BlockEditNode
 from .. import block_forms as block_forms
-from ..utils import FeditPermissionCheck
+from ..utils import (
+    FeditPermissionCheck,
+    FEDIT_PREVIEW_VAR,
+)
 
 
 
 @method_decorator(xframe_options_sameorigin, name="dispatch")
 class EditBlockView(FeditPermissionCheck, WagtailAdminTemplateMixin, View):
     template_name = "wagtail_fedit/editor/iframe.html"
 
@@ -153,14 +156,18 @@
         return self.render_to_response(
             self.get_context_data(form=form),
             success=True,
         )
 
     def post(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         form = self.form_class(request.POST, block=self.block, parent_instance=self.instance, request=request)
+
+        # Set the preview flag to mark as editable block when re-rendering.
+        setattr(request, FEDIT_PREVIEW_VAR, True)
+
         valid = form.is_valid()
         if valid:
             self.block = form.save()
         else:
             # We are not rendering the content, so we can omit data from context.
             return JsonResponse({
                 "success": False,
@@ -193,14 +200,15 @@
                 "block_label": str(self.block.block.label),
             },
             content_changed=True,
             **extra_log_kwargs,
         )
 
         # Add the data to the context and render the block.
+
         if self.has_block:
             keys = request.GET.keys()
             data = BlockEditNode.unpack(*keys, request=request)
             for key in self.edit_args:
                 data.pop(key, None)
 
             node = BlockEditNode(
```

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.0.3/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.0.3/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.0.3/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.0.3/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.0.2
+Version: 1.0.3
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.0.2/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.0.3/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

