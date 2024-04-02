# Comparing `tmp/ActivityRelay-0.3.1.tar.gz` & `tmp/ActivityRelay-0.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ActivityRelay-0.3.1.tar", last modified: Tue Apr  2 19:26:06 2024, max compression
+gzip compressed data, was "ActivityRelay-0.3.1rc1.tar", last modified: Mon Apr  1 19:02:23 2024, max compression
```

## Comparing `ActivityRelay-0.3.1.tar` & `ActivityRelay-0.3.1rc1.tar`

### file list

```diff
@@ -1,65 +1,59 @@
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-02 19:26:06.634209 ActivityRelay-0.3.1/
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-02 19:26:06.634209 ActivityRelay-0.3.1/ActivityRelay.egg-info/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2216 2024-04-02 19:26:06.000000 ActivityRelay-0.3.1/ActivityRelay.egg-info/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1478 2024-04-02 19:26:06.000000 ActivityRelay-0.3.1/ActivityRelay.egg-info/SOURCES.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-02 19:26:06.000000 ActivityRelay-0.3.1/ActivityRelay.egg-info/dependency_links.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)       52 2024-04-02 19:26:06.000000 ActivityRelay-0.3.1/ActivityRelay.egg-info/entry_points.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-02 19:25:26.000000 ActivityRelay-0.3.1/ActivityRelay.egg-info/not-zip-safe
--rw-r--r--   0 zoey      (1000) zoey      (1000)      407 2024-04-02 19:26:06.000000 ActivityRelay-0.3.1/ActivityRelay.egg-info/requires.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        6 2024-04-02 19:26:06.000000 ActivityRelay-0.3.1/ActivityRelay.egg-info/top_level.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)    34254 2023-12-09 10:04:09.000000 ActivityRelay-0.3.1/LICENSE
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2216 2024-04-02 19:26:06.634209 ActivityRelay-0.3.1/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      606 2023-12-09 10:04:09.000000 ActivityRelay-0.3.1/README.md
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2221 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/pyproject.toml
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-02 19:26:06.630209 ActivityRelay-0.3.1/relay/
--rw-r--r--   0 zoey      (1000) zoey      (1000)       22 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/__init__.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)      125 2024-03-10 23:03:43.000000 ActivityRelay-0.3.1/relay/__main__.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     8262 2024-04-02 19:13:11.000000 ActivityRelay-0.3.1/relay/application.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     7775 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/cache.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     3579 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/compat.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     4427 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/config.py
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-02 19:26:06.630209 ActivityRelay-0.3.1/relay/data/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     3765 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/data/statements.sql
--rw-r--r--   0 zoey      (1000) zoey      (1000)    20436 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/data/swagger.yaml
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-02 19:26:06.630209 ActivityRelay-0.3.1/relay/database/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1498 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/database/__init__.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     3772 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/database/config.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     9162 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/database/connection.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2329 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/database/schema.py
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-02 19:26:06.630209 ActivityRelay-0.3.1/relay/frontend/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2007 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/base.haml
--rw-r--r--   0 zoey      (1000) zoey      (1000)      369 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/functions.haml
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-02 19:26:06.630209 ActivityRelay-0.3.1/relay/frontend/page/
--rw-r--r--   0 zoey      (1000) zoey      (1000)      916 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/page/admin-config.haml
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1319 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/page/admin-domain_bans.haml
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2006 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/page/admin-instances.haml
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1308 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/page/admin-software_bans.haml
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1279 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/page/admin-users.haml
--rw-r--r--   0 zoey      (1000) zoey      (1000)      790 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/page/admin-whitelist.haml
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1068 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/page/home.haml
--rw-r--r--   0 zoey      (1000) zoey      (1000)      516 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/page/login.haml
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-02 19:26:06.634209 ActivityRelay-0.3.1/relay/frontend/static/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2796 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/static/api.js
--rw-r--r--   0 zoey      (1000) zoey      (1000)      930 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/static/config.js
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2825 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/static/domain_ban.js
--rw-r--r--   0 zoey      (1000) zoey      (1000)     3327 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/static/instance.js
--rw-r--r--   0 zoey      (1000) zoey      (1000)      564 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/static/login.js
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2714 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/static/software_ban.js
--rw-r--r--   0 zoey      (1000) zoey      (1000)     5677 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/static/style.css
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1959 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/static/user.js
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1379 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/frontend/static/whitelist.js
--rw-r--r--   0 zoey      (1000) zoey      (1000)      600 2024-03-11 05:20:44.000000 ActivityRelay-0.3.1/relay/frontend/variables.css
--rw-r--r--   0 zoey      (1000) zoey      (1000)     6557 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/http_client.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2020 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/logger.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)    25639 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/manage.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     6058 2024-04-02 18:56:26.000000 ActivityRelay-0.3.1/relay/misc.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     6168 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/processors.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2280 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/template.py
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-02 19:26:06.634209 ActivityRelay-0.3.1/relay/views/
--rw-r--r--   0 zoey      (1000) zoey      (1000)      113 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/views/__init__.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     4083 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/views/activitypub.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)    13908 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/views/api.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     3547 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/views/base.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     6489 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/views/frontend.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1494 2024-04-02 18:32:30.000000 ActivityRelay-0.3.1/relay/views/misc.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-04-02 19:26:06.634209 ActivityRelay-0.3.1/setup.cfg
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-01 19:02:23.055362 ActivityRelay-0.3.1rc1/
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-01 19:02:23.055362 ActivityRelay-0.3.1rc1/ActivityRelay.egg-info/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2176 2024-04-01 19:02:23.000000 ActivityRelay-0.3.1rc1/ActivityRelay.egg-info/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1251 2024-04-01 19:02:23.000000 ActivityRelay-0.3.1rc1/ActivityRelay.egg-info/SOURCES.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-01 19:02:23.000000 ActivityRelay-0.3.1rc1/ActivityRelay.egg-info/dependency_links.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)       52 2024-04-01 19:02:23.000000 ActivityRelay-0.3.1rc1/ActivityRelay.egg-info/entry_points.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-01 18:56:06.000000 ActivityRelay-0.3.1rc1/ActivityRelay.egg-info/not-zip-safe
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      407 2024-04-01 19:02:23.000000 ActivityRelay-0.3.1rc1/ActivityRelay.egg-info/requires.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        6 2024-04-01 19:02:23.000000 ActivityRelay-0.3.1rc1/ActivityRelay.egg-info/top_level.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    34254 2023-12-09 10:04:09.000000 ActivityRelay-0.3.1rc1/LICENSE
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2176 2024-04-01 19:02:23.055362 ActivityRelay-0.3.1rc1/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      606 2023-12-09 10:04:09.000000 ActivityRelay-0.3.1rc1/README.md
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      125 2024-03-31 15:51:39.000000 ActivityRelay-0.3.1rc1/dev-requirements.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      330 2024-03-13 21:21:29.000000 ActivityRelay-0.3.1rc1/pyproject.toml
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-01 19:02:23.051362 ActivityRelay-0.3.1rc1/relay/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)       26 2024-04-01 18:57:33.000000 ActivityRelay-0.3.1rc1/relay/__init__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      125 2024-03-10 23:03:43.000000 ActivityRelay-0.3.1rc1/relay/__main__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     7900 2024-03-31 15:32:03.000000 ActivityRelay-0.3.1rc1/relay/application.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     7775 2024-03-13 21:20:52.000000 ActivityRelay-0.3.1rc1/relay/cache.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     3579 2024-03-13 20:43:00.000000 ActivityRelay-0.3.1rc1/relay/compat.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     4362 2024-03-31 15:42:13.000000 ActivityRelay-0.3.1rc1/relay/config.py
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-01 19:02:23.051362 ActivityRelay-0.3.1rc1/relay/data/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     3765 2024-03-11 04:10:45.000000 ActivityRelay-0.3.1rc1/relay/data/statements.sql
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    20436 2024-03-15 10:24:19.000000 ActivityRelay-0.3.1rc1/relay/data/swagger.yaml
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-01 19:02:23.055362 ActivityRelay-0.3.1rc1/relay/database/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1498 2024-03-12 14:48:36.000000 ActivityRelay-0.3.1rc1/relay/database/__init__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     3772 2024-03-31 15:42:31.000000 ActivityRelay-0.3.1rc1/relay/database/config.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     9162 2024-03-31 22:21:52.000000 ActivityRelay-0.3.1rc1/relay/database/connection.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2329 2024-03-13 04:26:02.000000 ActivityRelay-0.3.1rc1/relay/database/schema.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     4694 2024-04-01 11:39:40.000000 ActivityRelay-0.3.1rc1/relay/dev.py
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-01 19:02:23.055362 ActivityRelay-0.3.1rc1/relay/frontend/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2007 2024-03-28 15:16:17.000000 ActivityRelay-0.3.1rc1/relay/frontend/base.haml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      369 2024-03-16 02:57:47.000000 ActivityRelay-0.3.1rc1/relay/frontend/functions.haml
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-01 19:02:23.055362 ActivityRelay-0.3.1rc1/relay/frontend/page/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      916 2024-03-16 02:57:24.000000 ActivityRelay-0.3.1rc1/relay/frontend/page/admin-config.haml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1319 2024-03-15 11:22:47.000000 ActivityRelay-0.3.1rc1/relay/frontend/page/admin-domain_bans.haml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2006 2024-03-15 12:10:39.000000 ActivityRelay-0.3.1rc1/relay/frontend/page/admin-instances.haml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1308 2024-03-15 23:23:15.000000 ActivityRelay-0.3.1rc1/relay/frontend/page/admin-software_bans.haml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1279 2024-03-16 01:58:24.000000 ActivityRelay-0.3.1rc1/relay/frontend/page/admin-users.haml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      790 2024-03-15 23:40:32.000000 ActivityRelay-0.3.1rc1/relay/frontend/page/admin-whitelist.haml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1068 2024-03-14 07:36:17.000000 ActivityRelay-0.3.1rc1/relay/frontend/page/home.haml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      516 2024-03-16 02:07:19.000000 ActivityRelay-0.3.1rc1/relay/frontend/page/login.haml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      600 2024-03-11 05:20:44.000000 ActivityRelay-0.3.1rc1/relay/frontend/variables.css
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     6557 2024-03-30 09:27:50.000000 ActivityRelay-0.3.1rc1/relay/http_client.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2020 2024-03-31 15:42:41.000000 ActivityRelay-0.3.1rc1/relay/logger.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    25417 2024-03-13 20:16:40.000000 ActivityRelay-0.3.1rc1/relay/manage.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     5998 2024-03-31 15:41:58.000000 ActivityRelay-0.3.1rc1/relay/misc.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     6168 2024-03-27 13:46:41.000000 ActivityRelay-0.3.1rc1/relay/processors.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2280 2024-03-14 08:56:55.000000 ActivityRelay-0.3.1rc1/relay/template.py
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-01 19:02:23.055362 ActivityRelay-0.3.1rc1/relay/views/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      113 2024-03-12 14:16:55.000000 ActivityRelay-0.3.1rc1/relay/views/__init__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     4083 2024-03-28 16:26:15.000000 ActivityRelay-0.3.1rc1/relay/views/activitypub.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    13908 2024-03-28 15:58:46.000000 ActivityRelay-0.3.1rc1/relay/views/api.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     3547 2024-03-31 15:41:30.000000 ActivityRelay-0.3.1rc1/relay/views/base.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     6489 2024-03-28 16:04:48.000000 ActivityRelay-0.3.1rc1/relay/views/frontend.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1494 2024-03-13 17:44:32.000000 ActivityRelay-0.3.1rc1/relay/views/misc.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      304 2024-04-01 18:49:14.000000 ActivityRelay-0.3.1rc1/requirements.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1307 2024-04-01 19:02:23.055362 ActivityRelay-0.3.1rc1/setup.cfg
+-rw-r--r--   0 zoey      (1000) zoey      (1000)       69 2023-12-09 10:04:09.000000 ActivityRelay-0.3.1rc1/setup.py
```

### Comparing `ActivityRelay-0.3.1/ActivityRelay.egg-info/PKG-INFO` & `ActivityRelay-0.3.1rc1/ActivityRelay.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ActivityRelay
-Version: 0.3.1
+Version: 0.3.1rc1
 Summary: Generic LitePub relay (works with all LitePub consumers and Mastodon)
+Home-page: https://git.pleroma.social/pleroma/relay
 License: AGPLv3
-Project-URL: Documentation, https://git.pleroma.social/pleroma/relay/-/blob/main/docs/index.md
 Project-URL: Source, https://git.pleroma.social/pleroma/relay
 Project-URL: Tracker, https://git.pleroma.social/pleroma/relay/-/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ActivityRelay-0.3.1/ActivityRelay.egg-info/SOURCES.txt` & `ActivityRelay-0.3.1rc1/ActivityRelay.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 LICENSE
 README.md
+dev-requirements.txt
 pyproject.toml
+requirements.txt
+setup.cfg
+setup.py
 ActivityRelay.egg-info/PKG-INFO
 ActivityRelay.egg-info/SOURCES.txt
 ActivityRelay.egg-info/dependency_links.txt
 ActivityRelay.egg-info/entry_points.txt
 ActivityRelay.egg-info/not-zip-safe
 ActivityRelay.egg-info/requires.txt
 ActivityRelay.egg-info/top_level.txt
 relay/__init__.py
 relay/__main__.py
 relay/application.py
 relay/cache.py
 relay/compat.py
 relay/config.py
+relay/dev.py
 relay/http_client.py
 relay/logger.py
 relay/manage.py
 relay/misc.py
 relay/processors.py
 relay/template.py
 relay/data/statements.sql
@@ -33,22 +38,13 @@
 relay/frontend/page/admin-domain_bans.haml
 relay/frontend/page/admin-instances.haml
 relay/frontend/page/admin-software_bans.haml
 relay/frontend/page/admin-users.haml
 relay/frontend/page/admin-whitelist.haml
 relay/frontend/page/home.haml
 relay/frontend/page/login.haml
-relay/frontend/static/api.js
-relay/frontend/static/config.js
-relay/frontend/static/domain_ban.js
-relay/frontend/static/instance.js
-relay/frontend/static/login.js
-relay/frontend/static/software_ban.js
-relay/frontend/static/style.css
-relay/frontend/static/user.js
-relay/frontend/static/whitelist.js
 relay/views/__init__.py
 relay/views/activitypub.py
 relay/views/api.py
 relay/views/base.py
 relay/views/frontend.py
 relay/views/misc.py
```

### Comparing `ActivityRelay-0.3.1/LICENSE` & `ActivityRelay-0.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/PKG-INFO` & `ActivityRelay-0.3.1rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ActivityRelay
-Version: 0.3.1
+Version: 0.3.1rc1
 Summary: Generic LitePub relay (works with all LitePub consumers and Mastodon)
+Home-page: https://git.pleroma.social/pleroma/relay
 License: AGPLv3
-Project-URL: Documentation, https://git.pleroma.social/pleroma/relay/-/blob/main/docs/index.md
 Project-URL: Source, https://git.pleroma.social/pleroma/relay
 Project-URL: Tracker, https://git.pleroma.social/pleroma/relay/-/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ActivityRelay-0.3.1/README.md` & `ActivityRelay-0.3.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/application.py` & `ActivityRelay-0.3.1rc1/relay/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from threading import Event, Thread
 
 from . import logger as logging
 from .cache import get_cache
 from .config import Config
 from .database import get_database
 from .http_client import HttpClient
-from .misc import IS_WINDOWS, check_open_port, get_resource
+from .misc import check_open_port, get_resource
 from .template import Template
 from .views import VIEWS
 from .views.api import handle_api_path
 from .views.frontend import handle_frontend_path
 
 if typing.TYPE_CHECKING:
 	from collections.abc import Callable
@@ -51,15 +51,15 @@
 	return '; '.join(data) + ';'
 
 
 class Application(web.Application):
 	DEFAULT: Application | None = None
 
 
-	def __init__(self, cfgpath: Path | None, dev: bool = False):
+	def __init__(self, cfgpath: str | None, dev: bool = False):
 		web.Application.__init__(self,
 			middlewares = [
 				handle_api_path,
 				handle_frontend_path,
 				handle_response_headers
 			]
 		)
@@ -292,61 +292,43 @@
 
 	def stop(self) -> None:
 		self.running.clear()
 
 
 class PushWorker(multiprocessing.Process):
 	def __init__(self, queue: multiprocessing.Queue):
-		if Application.DEFAULT is None:
-			raise RuntimeError('Application not setup yet')
-
 		multiprocessing.Process.__init__(self)
-
 		self.queue = queue
 		self.shutdown = multiprocessing.Event()
-		self.path = Application.DEFAULT.config.path
 
 
 	def stop(self) -> None:
 		self.shutdown.set()
 
 
 	def run(self) -> None:
 		asyncio.run(self.handle_queue())
 
 
 	async def handle_queue(self) -> None:
-		if IS_WINDOWS:
-			app = Application(self.path)
-			client = app.client
-
-			client.open()
-			app.database.connect()
-			app.cache.setup()
-
-		else:
-			client = HttpClient()
-			client.open()
+		client = HttpClient()
+		client.open()
 
 		while not self.shutdown.is_set():
 			try:
 				inbox, message, instance = self.queue.get(block=True, timeout=0.1)
 				asyncio.create_task(client.post(inbox, message, instance))
 
 			except Empty:
 				await asyncio.sleep(0)
 
 			# make sure an exception doesn't bring down the worker
 			except Exception:
 				traceback.print_exc()
 
-		if IS_WINDOWS:
-			app.database.disconnect()
-			app.cache.close()
-
 		await client.close()
 
 
 @web.middleware
 async def handle_response_headers(request: web.Request, handler: Callable) -> Response:
 	resp = await handler(request)
 	resp.headers['Server'] = 'ActivityRelay'
```

### Comparing `ActivityRelay-0.3.1/relay/cache.py` & `ActivityRelay-0.3.1rc1/relay/cache.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/compat.py` & `ActivityRelay-0.3.1rc1/relay/compat.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/config.py` & `ActivityRelay-0.3.1rc1/relay/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 else:
 	CORE_COUNT = len(os.sched_getaffinity(0))
 
 
 DOCKER_VALUES = {
 	'listen': '0.0.0.0',
 	'port': 8080,
-	'sq_path': '/data/relay.sqlite3'
+	'sq_path': '/data/relay.jsonld'
 }
 
 
 class NOVALUE:
 	pass
 
 
@@ -61,15 +61,15 @@
 	rd_port: int = 6470
 	rd_user: str | None = None
 	rd_pass: str | None = None
 	rd_database: int = 0
 	rd_prefix: str = 'activityrelay'
 
 
-	def __init__(self, path: Path | None = None, load: bool = False):
+	def __init__(self, path: str | None = None, load: bool = False):
 		self.path = Config.get_config_dir(path)
 		self.reset()
 
 		if load:
 			try:
 				self.load()
 
@@ -88,20 +88,17 @@
 			if field.name == key:
 				return field.default # type: ignore
 
 		raise KeyError(key)
 
 
 	@staticmethod
-	def get_config_dir(path: Path | str | None = None) -> Path:
-		if isinstance(path, str):
-			path = Path(path)
-
-		if path is not None:
-			return path.expanduser().resolve()
+	def get_config_dir(path: str | None = None) -> Path:
+		if path:
+			return Path(path).expanduser().resolve()
 
 		paths = (
 			Path("relay.yaml").resolve(),
 			Path(user_config_dir("activityrelay"), "relay.yaml"),
 			Path("/etc/activityrelay/relay.yaml")
 		)
```

### Comparing `ActivityRelay-0.3.1/relay/data/statements.sql` & `ActivityRelay-0.3.1rc1/relay/data/statements.sql`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/data/swagger.yaml` & `ActivityRelay-0.3.1rc1/relay/data/swagger.yaml`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/database/__init__.py` & `ActivityRelay-0.3.1rc1/relay/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/database/config.py` & `ActivityRelay-0.3.1rc1/relay/database/config.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/database/connection.py` & `ActivityRelay-0.3.1rc1/relay/database/connection.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/database/schema.py` & `ActivityRelay-0.3.1rc1/relay/database/schema.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/frontend/base.haml` & `ActivityRelay-0.3.1rc1/relay/frontend/base.haml`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/frontend/page/admin-config.haml` & `ActivityRelay-0.3.1rc1/relay/frontend/page/admin-config.haml`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/frontend/page/admin-domain_bans.haml` & `ActivityRelay-0.3.1rc1/relay/frontend/page/admin-domain_bans.haml`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/frontend/page/admin-instances.haml` & `ActivityRelay-0.3.1rc1/relay/frontend/page/admin-instances.haml`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/frontend/page/admin-software_bans.haml` & `ActivityRelay-0.3.1rc1/relay/frontend/page/admin-software_bans.haml`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/frontend/page/admin-users.haml` & `ActivityRelay-0.3.1rc1/relay/frontend/page/admin-users.haml`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/frontend/page/admin-whitelist.haml` & `ActivityRelay-0.3.1rc1/relay/frontend/page/admin-whitelist.haml`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/frontend/page/home.haml` & `ActivityRelay-0.3.1rc1/relay/frontend/page/home.haml`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/frontend/page/login.haml` & `ActivityRelay-0.3.1rc1/relay/frontend/page/login.haml`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/frontend/variables.css` & `ActivityRelay-0.3.1rc1/relay/frontend/variables.css`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/http_client.py` & `ActivityRelay-0.3.1rc1/relay/http_client.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/logger.py` & `ActivityRelay-0.3.1rc1/relay/logger.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/manage.py` & `ActivityRelay-0.3.1rc1/relay/manage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
+import Crypto
 import aputils
 import asyncio
 import click
-import json
 import os
+import platform
 import typing
 
 from pathlib import Path
 from shutil import copyfile
 from urllib.parse import urlparse
 
 from . import __version__
@@ -27,190 +28,188 @@
 def check_alphanumeric(text: str) -> str:
 	if not text.isalnum():
 		raise click.BadParameter('String not alphanumeric')
 
 	return text
 
 
-@click.group('cli', context_settings = {'show_default': True})
-@click.option('--config', '-c', type = Path, help = 'path to the relay\'s config')
-@click.version_option(version = __version__, prog_name = 'ActivityRelay')
+@click.group('cli', context_settings={'show_default': True}, invoke_without_command=True)
+@click.option('--config', '-c', help='path to the relay\'s config')
+@click.version_option(version=__version__, prog_name='ActivityRelay')
 @click.pass_context
-def cli(ctx: click.Context, config: Path | None) -> None:
-	if IS_DOCKER:
-		config = Path("/data/relay.yaml")
-
-		# The database was named "relay.jsonld" even though it's an sqlite file. Fix it.
-		db = Path('/data/relay.sqlite3')
-		wrongdb = Path('/data/relay.jsonld')
-
-		if wrongdb.exists() and not db.exists():
-			try:
-				with wrongdb.open('rb') as fd:
-					json.load(fd)
+def cli(ctx: click.Context, config: str | None) -> None:
+	ctx.obj = Application(config)
 
-			except json.JSONDecodeError:
-				wrongdb.rename(db)
+	if not ctx.invoked_subcommand:
+		if ctx.obj.config.domain.endswith('example.com'):
+			cli_setup.callback() # type: ignore
 
-	ctx.obj = Application(config)
+		else:
+			click.echo(
+				'[DEPRECATED] Running the relay without the "run" command will be removed in the ' +
+				'future.'
+			)
+
+			cli_run.callback() # type: ignore
 
 
 @cli.command('setup')
-@click.option('--skip-questions', '-s', is_flag = True, help = 'Just setup the database')
 @click.pass_context
-def cli_setup(ctx: click.Context, skip_questions: bool) -> None:
+def cli_setup(ctx: click.Context) -> None:
 	'Generate a new config and create the database'
 
-	if ctx.obj.signer is not None:
-		if not click.prompt('The database is already setup. Are you sure you want to continue?'):
-			return
-
-	if skip_questions and ctx.obj.config.domain.endswith('example.com'):
-		click.echo('You cannot skip the questions if the relay is not configured yet')
-		return
-
-	if not skip_questions:
-		while True:
-			ctx.obj.config.domain = click.prompt(
-				'What domain will the relay be hosted on?',
-				default = ctx.obj.config.domain
-			)
+	while True:
+		ctx.obj.config.domain = click.prompt(
+			'What domain will the relay be hosted on?',
+			default = ctx.obj.config.domain
+		)
 
-			if not ctx.obj.config.domain.endswith('example.com'):
-				break
+		if not ctx.obj.config.domain.endswith('example.com'):
+			break
 
-			click.echo('The domain must not end with "example.com"')
+		click.echo('The domain must not end with "example.com"')
 
-		if not IS_DOCKER:
-			ctx.obj.config.listen = click.prompt(
-				'Which address should the relay listen on?',
-				default = ctx.obj.config.listen
-			)
-
-			ctx.obj.config.port = click.prompt(
-				'What TCP port should the relay listen on?',
-				default = ctx.obj.config.port,
-				type = int
-			)
+	if not IS_DOCKER:
+		ctx.obj.config.listen = click.prompt(
+			'Which address should the relay listen on?',
+			default = ctx.obj.config.listen
+		)
 
-		ctx.obj.config.db_type = click.prompt(
-			'Which database backend will be used?',
-			default = ctx.obj.config.db_type,
-			type = click.Choice(['postgres', 'sqlite'], case_sensitive = False)
+		ctx.obj.config.port = click.prompt(
+			'What TCP port should the relay listen on?',
+			default = ctx.obj.config.port,
+			type = int
 		)
 
-		if ctx.obj.config.db_type == 'sqlite' and not IS_DOCKER:
-			ctx.obj.config.sq_path = click.prompt(
-				'Where should the database be stored?',
-				default = ctx.obj.config.sq_path
-			)
+	ctx.obj.config.db_type = click.prompt(
+		'Which database backend will be used?',
+		default = ctx.obj.config.db_type,
+		type = click.Choice(['postgres', 'sqlite'], case_sensitive = False)
+	)
+
+	if ctx.obj.config.db_type == 'sqlite':
+		ctx.obj.config.sq_path = click.prompt(
+			'Where should the database be stored?',
+			default = ctx.obj.config.sq_path
+		)
 
-		elif ctx.obj.config.db_type == 'postgres':
-			ctx.obj.config.pg_name = click.prompt(
-				'What is the name of the database?',
-				default = ctx.obj.config.pg_name
-			)
+	elif ctx.obj.config.db_type == 'postgres':
+		ctx.obj.config.pg_name = click.prompt(
+			'What is the name of the database?',
+			default = ctx.obj.config.pg_name
+		)
 
-			ctx.obj.config.pg_host = click.prompt(
-				'What IP address, hostname, or unix socket does the server listen on?',
-				default = ctx.obj.config.pg_host,
-				type = int
-			)
+		ctx.obj.config.pg_host = click.prompt(
+			'What IP address, hostname, or unix socket does the server listen on?',
+			default = ctx.obj.config.pg_host,
+			type = int
+		)
 
-			ctx.obj.config.pg_port = click.prompt(
-				'What port does the server listen on?',
-				default = ctx.obj.config.pg_port,
-				type = int
-			)
+		ctx.obj.config.pg_port = click.prompt(
+			'What port does the server listen on?',
+			default = ctx.obj.config.pg_port,
+			type = int
+		)
 
-			ctx.obj.config.pg_user = click.prompt(
-				'Which user will authenticate with the server?',
-				default = ctx.obj.config.pg_user
-			)
+		ctx.obj.config.pg_user = click.prompt(
+			'Which user will authenticate with the server?',
+			default = ctx.obj.config.pg_user
+		)
 
-			ctx.obj.config.pg_pass = click.prompt(
-				'User password',
-				hide_input = True,
-				show_default = False,
-				default = ctx.obj.config.pg_pass or ""
-			) or None
-
-		ctx.obj.config.ca_type = click.prompt(
-			'Which caching backend?',
-			default = ctx.obj.config.ca_type,
-			type = click.Choice(['database', 'redis'], case_sensitive = False)
-		)
-
-		if ctx.obj.config.ca_type == 'redis':
-			ctx.obj.config.rd_host = click.prompt(
-				'What IP address, hostname, or unix socket does the server listen on?',
-				default = ctx.obj.config.rd_host
-			)
+		ctx.obj.config.pg_pass = click.prompt(
+			'User password',
+			hide_input = True,
+			show_default = False,
+			default = ctx.obj.config.pg_pass or ""
+		) or None
+
+	ctx.obj.config.ca_type = click.prompt(
+		'Which caching backend?',
+		default = ctx.obj.config.ca_type,
+		type = click.Choice(['database', 'redis'], case_sensitive = False)
+	)
+
+	if ctx.obj.config.ca_type == 'redis':
+		ctx.obj.config.rd_host = click.prompt(
+			'What IP address, hostname, or unix socket does the server listen on?',
+			default = ctx.obj.config.rd_host
+		)
 
-			ctx.obj.config.rd_port = click.prompt(
-				'What port does the server listen on?',
-				default = ctx.obj.config.rd_port,
-				type = int
-			)
+		ctx.obj.config.rd_port = click.prompt(
+			'What port does the server listen on?',
+			default = ctx.obj.config.rd_port,
+			type = int
+		)
 
-			ctx.obj.config.rd_user = click.prompt(
-				'Which user will authenticate with the server',
-				default = ctx.obj.config.rd_user
-			)
+		ctx.obj.config.rd_user = click.prompt(
+			'Which user will authenticate with the server',
+			default = ctx.obj.config.rd_user
+		)
 
-			ctx.obj.config.rd_pass = click.prompt(
-				'User password',
-				hide_input = True,
-				show_default = False,
-				default = ctx.obj.config.rd_pass or ""
-			) or None
-
-			ctx.obj.config.rd_database = click.prompt(
-				'Which database number to use?',
-				default = ctx.obj.config.rd_database,
-				type = int
-			)
+		ctx.obj.config.rd_pass = click.prompt(
+			'User password',
+			hide_input = True,
+			show_default = False,
+			default = ctx.obj.config.rd_pass or ""
+		) or None
+
+		ctx.obj.config.rd_database = click.prompt(
+			'Which database number to use?',
+			default = ctx.obj.config.rd_database,
+			type = int
+		)
 
-			ctx.obj.config.rd_prefix = click.prompt(
-				'What text should each cache key be prefixed with?',
-				default = ctx.obj.config.rd_database,
-				type = check_alphanumeric
-			)
+		ctx.obj.config.rd_prefix = click.prompt(
+			'What text should each cache key be prefixed with?',
+			default = ctx.obj.config.rd_database,
+			type = check_alphanumeric
+		)
 
-		ctx.obj.config.save()
+	ctx.obj.config.save()
 
 	config = {
 		'private-key': aputils.Signer.new('n/a').export()
 	}
 
 	with ctx.obj.database.session() as conn:
 		for key, value in config.items():
 			conn.put_config(key, value)
 
-	if IS_DOCKER:
-		click.echo("Relay all setup! Start the container to run the relay.")
-		return
-
-	if click.confirm('Relay all setup! Would you like to run it now?'):
+	if not IS_DOCKER and click.confirm('Relay all setup! Would you like to run it now?'):
 		cli_run.callback() # type: ignore
 
 
 @cli.command('run')
 @click.option('--dev', '-d', is_flag=True, help='Enable developer mode')
 @click.pass_context
 def cli_run(ctx: click.Context, dev: bool = False) -> None:
 	'Run the relay'
 
-	if ctx.obj.config.domain.endswith('example.com') or ctx.obj.signer is None:
-		if not IS_DOCKER:
-			click.echo('Relay is not set up. Please run "activityrelay setup".')
+	if ctx.obj.config.domain.endswith('example.com') or not ctx.obj.signer:
+		click.echo(
+			'Relay is not set up. Please edit your relay config or run "activityrelay setup".'
+		)
+
+		return
+
+	vers_split = platform.python_version().split('.')
+	pip_command = 'pip3 uninstall pycrypto && pip3 install pycryptodome'
+
+	if Crypto.__version__ == '2.6.1':
+		if int(vers_split[1]) > 7:
+			click.echo(
+				'Error: PyCrypto is broken on Python 3.8+. Please replace it with pycryptodome ' +
+				'before running again. Exiting...'
+			)
 
+			click.echo(pip_command)
 			return
 
-		cli_setup.callback() # type: ignore
+		click.echo('Warning: PyCrypto is old and should be replaced with pycryptodome')
+		click.echo(pip_command)
 		return
 
 	ctx.obj['dev'] = dev
 	ctx.obj.run()
 
 	# todo: figure out why the relay doesn't quit properly without this
 	os._exit(0)
```

### Comparing `ActivityRelay-0.3.1/relay/misc.py` & `ActivityRelay-0.3.1rc1/relay/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import aputils
 import json
 import os
-import platform
 import socket
 import typing
 
 from aiohttp.web import Response as AiohttpResponse
 from datetime import datetime
 from pathlib import Path
 from uuid import uuid4
@@ -35,15 +34,14 @@
 	'headers': dict[str, typing.Any] | None,
 	'content_type': str,
 	'body': bytes | None,
 	'text': str | None
 })
 
 IS_DOCKER = bool(os.environ.get('DOCKER_RUNNING'))
-IS_WINDOWS = platform.system() == 'Windows'
 
 MIMETYPES = {
 	'activity': 'application/activity+json',
 	'css': 'text/css',
 	'html': 'text/html',
 	'json': 'application/json',
 	'text': 'text/plain',
```

### Comparing `ActivityRelay-0.3.1/relay/processors.py` & `ActivityRelay-0.3.1rc1/relay/processors.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/template.py` & `ActivityRelay-0.3.1rc1/relay/template.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/views/activitypub.py` & `ActivityRelay-0.3.1rc1/relay/views/activitypub.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/views/api.py` & `ActivityRelay-0.3.1rc1/relay/views/api.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/views/base.py` & `ActivityRelay-0.3.1rc1/relay/views/base.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/views/frontend.py` & `ActivityRelay-0.3.1rc1/relay/views/frontend.py`

 * *Files identical despite different names*

### Comparing `ActivityRelay-0.3.1/relay/views/misc.py` & `ActivityRelay-0.3.1rc1/relay/views/misc.py`

 * *Files identical despite different names*

