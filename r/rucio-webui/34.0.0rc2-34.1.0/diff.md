# Comparing `tmp/rucio-webui-34.0.0rc2.tar.gz` & `tmp/rucio-webui-34.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-webui-34.0.0rc2.tar", last modified: Thu Mar 14 14:43:11 2024, max compression
+gzip compressed data, was "rucio-webui-34.1.0.tar", last modified: Tue Apr  2 13:57:13 2024, max compression
```

## Comparing `rucio-webui-34.0.0rc2.tar` & `rucio-webui-34.1.0.tar`

### file list

```diff
@@ -1,267 +1,267 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.086300 rucio-webui-34.0.0rc2/
--rwxr-xr-x   0 root         (0) root         (0)     4487 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      484 2024-03-14 14:43:07.000000 rucio-webui-34.0.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      869 2024-03-14 14:43:11.086300 rucio-webui-34.0.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.032299 rucio-webui-34.0.0rc2/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.036299 rucio-webui-34.0.0rc2/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      684 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      714 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/lib/rucio/alembicrevision.py
--rw-r--r--   0 root         (0) root         (0)      243 2024-03-14 13:17:06.000000 rucio-webui-34.0.0rc2/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1573 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.037299 rucio-webui-34.0.0rc2/lib/rucio/web/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.037299 rucio-webui-34.0.0rc2/lib/rucio/web/ui/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.038299 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6202 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/bp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.038299 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/common/
--rwxr-xr-x   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.039299 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/common/saml/
--rw-r--r--   0 root         (0) root         (0)      990 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/common/saml/advanced_settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.039299 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/common/saml/certs/
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/common/saml/certs/README
--rw-r--r--   0 root         (0) root         (0)      656 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/common/saml/settings.json
--rw-r--r--   0 root         (0) root         (0)    27924 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/common/utils.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.051299 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/
--rw-r--r--   0 root         (0) root         (0)     3705 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/account.html
--rw-r--r--   0 root         (0) root         (0)     1292 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/account_rse_usage.html
--rw-r--r--   0 root         (0) root         (0)     1825 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/account_usage.html
--rw-r--r--   0 root         (0) root         (0)     1234 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/account_usage_history.html
--rw-r--r--   0 root         (0) root         (0)      857 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/accounting.html
--rw-r--r--   0 root         (0) root         (0)      996 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/accounts.html
--rw-r--r--   0 root         (0) root         (0)     4233 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/add_rse.html
--rw-r--r--   0 root         (0) root         (0)     4109 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/approve_rules.html
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/atlas_index.html
--rw-r--r--   0 root         (0) root         (0)     2880 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/backlog_mon.html
--rw-r--r--   0 root         (0) root         (0)     1207 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/bad_replicas.html
--rw-r--r--   0 root         (0) root         (0)     1678 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html
--rw-r--r--   0 root         (0) root         (0)     8979 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/base.html
--rw-r--r--   0 root         (0) root         (0)     2652 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/cond.html
--rw-r--r--   0 root         (0) root         (0)     2678 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/dbrelease.html
--rw-r--r--   0 root         (0) root         (0)     2628 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/did.html
--rw-r--r--   0 root         (0) root         (0)     4970 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/dumps.html
--rw-r--r--   0 root         (0) root         (0)     1230 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/heartbeats.html
--rw-r--r--   0 root         (0) root         (0)      585 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/index.html
--rw-r--r--   0 root         (0) root         (0)     1789 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/infrastructure.html
--rw-r--r--   0 root         (0) root         (0)     3499 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/lifetime_exception.html
--rw-r--r--   0 root         (0) root         (0)     1270 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html
--rw-r--r--   0 root         (0) root         (0)     6608 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/list_rules.html
--rw-r--r--   0 root         (0) root         (0)     4440 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/login.html
--rw-r--r--   0 root         (0) root         (0)     1276 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/no_certificate.html
--rw-r--r--   0 root         (0) root         (0)      803 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/problem.html
--rw-r--r--   0 root         (0) root         (0)    16321 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/request_rule.html
--rw-r--r--   0 root         (0) root         (0)     4124 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rse.html
--rw-r--r--   0 root         (0) root         (0)     2380 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rse_account_usage.html
--rw-r--r--   0 root         (0) root         (0)     7277 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rse_add_protocol.html
--rw-r--r--   0 root         (0) root         (0)     1547 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rse_locks.html
--rw-r--r--   0 root         (0) root         (0)     1363 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rse_usage.html
--rw-r--r--   0 root         (0) root         (0)     1796 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rses.html
--rw-r--r--   0 root         (0) root         (0)     1919 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rule.html
--rw-r--r--   0 root         (0) root         (0)     2079 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rules.html
--rw-r--r--   0 root         (0) root         (0)     2164 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/search.html
--rw-r--r--   0 root         (0) root         (0)     5125 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/select_login_method.html
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/subscription.html
--rw-r--r--   0 root         (0) root         (0)      956 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/subscriptionrules.html
--rw-r--r--   0 root         (0) root         (0)     1562 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/subscriptions.html
--rw-r--r--   0 root         (0) root         (0)     5327 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/subscriptions_editor.html
--rw-r--r--   0 root         (0) root         (0)     3024 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/suspicious_replicas.html
--rw-r--r--   0 root         (0) root         (0)      741 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.054299 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/
--rwxr-xr-x   0 root         (0) root         (0)   135652 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/RucioUI.png
--rw-r--r--   0 root         (0) root         (0)      686 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/details_close.png
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/details_open.png
--rw-r--r--   0 root         (0) root         (0)    84798 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/error.jpg
--rw-r--r--   0 root         (0) root         (0)    10510 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.055300 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/fonts/
--rwxr-xr-x   0 root         (0) root         (0)     3400 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.eot
--rwxr-xr-x   0 root         (0) root         (0)     9218 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.svg
--rwxr-xr-x   0 root         (0) root         (0)     3236 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.ttf
--rwxr-xr-x   0 root         (0) root         (0)     3312 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.woff
--rw-r--r--   0 root         (0) root         (0)      753 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/get_info.png
--rw-r--r--   0 root         (0) root         (0)    56517 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/logo.png
--rw-r--r--   0 root         (0) root         (0)    19563 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/rucio_logo.png
--rw-r--r--   0 root         (0) root         (0)    32246 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/spinner.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.069300 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/
--rw-r--r--   0 root         (0) root         (0)     6764 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/account.js
--rw-r--r--   0 root         (0) root         (0)     8084 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/account_rse_usage.js
--rw-r--r--   0 root         (0) root         (0)    12181 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/account_usage.js
--rw-r--r--   0 root         (0) root         (0)     7667 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/account_usage_history.js
--rw-r--r--   0 root         (0) root         (0)     4998 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/accounting.js
--rw-r--r--   0 root         (0) root         (0)     1352 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/accounts.js
--rw-r--r--   0 root         (0) root         (0)     2468 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/add_rse.js
--rw-r--r--   0 root         (0) root         (0)    12226 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/approve_rules.js
--rw-r--r--   0 root         (0) root         (0)     2229 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/atlas_index.js
--rw-r--r--   0 root         (0) root         (0)    15169 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/backlog_mon.js
--rw-r--r--   0 root         (0) root         (0)     1054 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/bad_replicas.js
--rw-r--r--   0 root         (0) root         (0)    11540 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/bad_replicas_summary.js
--rw-r--r--   0 root         (0) root         (0)     7366 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/base.js
--rw-r--r--   0 root         (0) root         (0)      538 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen-sprite.png
--rw-r--r--   0 root         (0) root         (0)      738 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen-sprite@2x.png
--rw-r--r--   0 root         (0) root         (0)    13270 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen.css
--rw-r--r--   0 root         (0) root         (0)    44811 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen.jquery.js
--rw-r--r--   0 root         (0) root         (0)    28401 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen.jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    11061 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen.min.css
--rw-r--r--   0 root         (0) root         (0)    45100 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen.proto.js
--rw-r--r--   0 root         (0) root         (0)    28757 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen.proto.min.js
--rw-r--r--   0 root         (0) root         (0)     5641 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/cond.js
--rw-r--r--   0 root         (0) root         (0)     5758 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/dbrelease.js
--rw-r--r--   0 root         (0) root         (0)    43648 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/did.js
--rw-r--r--   0 root         (0) root         (0)     1396 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/filesize.min.js
--rw-r--r--   0 root         (0) root         (0)    19507 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/foundation-icons.css
--rw-r--r--   0 root         (0) root         (0)    54568 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/foundation-icons.eot
--rw-r--r--   0 root         (0) root         (0)   150251 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/foundation-icons.svg
--rw-r--r--   0 root         (0) root         (0)    56976 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/foundation-icons.ttf
--rw-r--r--   0 root         (0) root         (0)    32020 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/foundation-icons.woff
--rw-r--r--   0 root         (0) root         (0)     1359 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/heartbeats.js
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring.css
--rw-r--r--   0 root         (0) root         (0)    12386 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_account_details.js
--rw-r--r--   0 root         (0) root         (0)     3525 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_accounts.js
--rw-r--r--   0 root         (0) root         (0)     5294 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js
--rw-r--r--   0 root         (0) root         (0)     3795 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_apiclasses.js
--rw-r--r--   0 root         (0) root         (0)     3555 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_index.js
--rw-r--r--   0 root         (0) root         (0)     3043 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_resources.js
--rw-r--r--   0 root         (0) root         (0)     8872 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js
--rw-r--r--   0 root         (0) root         (0)     3055 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_scriptids.js
--rw-r--r--   0 root         (0) root         (0)    10028 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_utils.js
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/index.js
--rw-r--r--   0 root         (0) root         (0)    23108 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/jquery.multiple.select.js
--rw-r--r--   0 root         (0) root         (0)    20021 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/jquery.multiple.select2.js
--rw-r--r--   0 root         (0) root         (0)     4151 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/jquery.quicksearch.js
--rw-r--r--   0 root         (0) root         (0)     6966 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/jquery.storageapi.min.js
--rw-r--r--   0 root         (0) root         (0)    11881 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/lifetime_exception.js
--rw-r--r--   0 root         (0) root         (0)     4060 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/list_lifetime_exceptions.js
--rw-r--r--   0 root         (0) root         (0)    13472 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/list_rules.js
--rw-r--r--   0 root         (0) root         (0)      324 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/login.js
--rw-r--r--   0 root         (0) root         (0)     4279 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/multiple-select.css
--rw-r--r--   0 root         (0) root         (0)     3342 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/multiple-select.png
--rw-r--r--   0 root         (0) root         (0)     2233 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/multiple-select2.css
--rw-r--r--   0 root         (0) root         (0)    54419 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/request_rule.js
--rw-r--r--   0 root         (0) root         (0)     7089 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rse.js
--rw-r--r--   0 root         (0) root         (0)    23373 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rse_account_usage.js
--rw-r--r--   0 root         (0) root         (0)     7076 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rse_add_protocol.js
--rw-r--r--   0 root         (0) root         (0)     6559 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rse_locks.js
--rw-r--r--   0 root         (0) root         (0)    10905 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rse_usage.js
--rw-r--r--   0 root         (0) root         (0)     1632 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rses.js
--rw-r--r--   0 root         (0) root         (0)     2598 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rucio.css
--rw-r--r--   0 root         (0) root         (0)    63519 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rucio.js
--rw-r--r--   0 root         (0) root         (0)    23335 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rule.js
--rw-r--r--   0 root         (0) root         (0)     1341 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rules.js
--rw-r--r--   0 root         (0) root         (0)     6323 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/search.js
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/select_login_method.css
--rw-r--r--   0 root         (0) root         (0)     7637 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/subscription.js
--rw-r--r--   0 root         (0) root         (0)     3071 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/subscriptionrules.js
--rw-r--r--   0 root         (0) root         (0)     4946 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/subscriptions.js
--rw-r--r--   0 root         (0) root         (0)    13983 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/subscriptions_editor.js
--rw-r--r--   0 root         (0) root         (0)     9784 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/suspicious_replicas.js
--rw-r--r--   0 root         (0) root         (0)      540 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/switch.png
--rw-r--r--   0 root         (0) root         (0)      599 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/version.js
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-14 13:17:06.000000 rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/webui_version
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.086300 rucio-webui-34.0.0rc2/lib/rucio_webui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8846 2024-03-14 14:43:11.000000 rucio-webui-34.0.0rc2/lib/rucio_webui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/pylintrc
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-27 12:40:37.000000 rucio-webui-34.0.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5048 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2024-03-14 14:43:11.087300 rucio-webui-34.0.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2153 2024-03-14 14:43:07.000000 rucio-webui-34.0.0rc2/setup.py
--rw-r--r--   0 root         (0) root         (0)     4803 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 14:43:11.085300 rucio-webui-34.0.0rc2/tests/
--rw-r--r--   0 root         (0) root         (0)     3708 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10703 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3255 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15944 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9834 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20552 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13376 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4120 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2213 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4225 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    15088 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3488 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23358 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12468 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     6975 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107211 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2089 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     6954 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1889 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6966 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    96530 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    22661 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6971 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7703 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7361 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2642 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28217 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2759 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    55589 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29541 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4209 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35378 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7203 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16658 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10907 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3158 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38325 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7977 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10138 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5843 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18578 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57259 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5281 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22299 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11070 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20482 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12205 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5879 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6323 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2058 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54268 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2911 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11606 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   108519 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4508 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4147 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1165 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7607 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2765 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2053 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27544 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6464 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62616 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    38899 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22764 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    17208 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    13002 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75277 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13230 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8966 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4300 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3845 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3290 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3713 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4822 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     4002 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4678 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3038 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3803 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7770 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    90893 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)    13873 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_schema_cms.py
--rw-r--r--   0 root         (0) root         (0)     7510 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48716 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)    55640 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5064 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3204 2024-03-13 10:19:28.000000 rucio-webui-34.0.0rc2/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    25277 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8949 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_transfer_plugins.py
--rw-r--r--   0 root         (0) root         (0)     8436 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15549 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     7451 2024-03-14 13:07:01.000000 rucio-webui-34.0.0rc2/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.756327 rucio-webui-34.1.0/
+-rwxr-xr-x   0 root         (0) root         (0)     4487 2024-03-19 15:04:29.000000 rucio-webui-34.1.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      484 2024-04-02 13:57:10.000000 rucio-webui-34.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      866 2024-04-02 13:57:13.756327 rucio-webui-34.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-02 11:45:19.000000 rucio-webui-34.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.710326 rucio-webui-34.1.0/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.713326 rucio-webui-34.1.0/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/alembicrevision.py
+-rw-r--r--   0 root         (0) root         (0)      244 2024-04-02 11:50:17.000000 rucio-webui-34.1.0/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1549 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.713326 rucio-webui-34.1.0/lib/rucio/web/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.713326 rucio-webui-34.1.0/lib/rucio/web/ui/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.714326 rucio-webui-34.1.0/lib/rucio/web/ui/flask/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/bp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.714326 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/
+-rwxr-xr-x   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.715326 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/
+-rw-r--r--   0 root         (0) root         (0)      990 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/advanced_settings.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.715326 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/certs/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/certs/README
+-rw-r--r--   0 root         (0) root         (0)      656 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/settings.json
+-rw-r--r--   0 root         (0) root         (0)    27943 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/utils.py
+-rw-r--r--   0 root         (0) root         (0)      893 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.722326 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account.html
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account_rse_usage.html
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account_usage.html
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account_usage_history.html
+-rw-r--r--   0 root         (0) root         (0)      857 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/accounting.html
+-rw-r--r--   0 root         (0) root         (0)      996 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/accounts.html
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/add_rse.html
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/approve_rules.html
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/atlas_index.html
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/backlog_mon.html
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/bad_replicas.html
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html
+-rw-r--r--   0 root         (0) root         (0)     8979 2024-03-13 10:19:28.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)     2652 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/cond.html
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/dbrelease.html
+-rw-r--r--   0 root         (0) root         (0)     2628 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/did.html
+-rw-r--r--   0 root         (0) root         (0)     4970 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/dumps.html
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/heartbeats.html
+-rw-r--r--   0 root         (0) root         (0)      585 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/index.html
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/infrastructure.html
+-rw-r--r--   0 root         (0) root         (0)     3499 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/lifetime_exception.html
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html
+-rw-r--r--   0 root         (0) root         (0)     6608 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/list_rules.html
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/login.html
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/no_certificate.html
+-rw-r--r--   0 root         (0) root         (0)      803 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/problem.html
+-rw-r--r--   0 root         (0) root         (0)    16321 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/request_rule.html
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse.html
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_account_usage.html
+-rw-r--r--   0 root         (0) root         (0)     7277 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_add_protocol.html
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_locks.html
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_usage.html
+-rw-r--r--   0 root         (0) root         (0)     1796 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rses.html
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rule.html
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rules.html
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/search.html
+-rw-r--r--   0 root         (0) root         (0)     5125 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/select_login_method.html
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscription.html
+-rw-r--r--   0 root         (0) root         (0)      956 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscriptionrules.html
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscriptions.html
+-rw-r--r--   0 root         (0) root         (0)     5327 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscriptions_editor.html
+-rw-r--r--   0 root         (0) root         (0)     3024 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/suspicious_replicas.html
+-rw-r--r--   0 root         (0) root         (0)      717 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.724326 rucio-webui-34.1.0/lib/rucio/web/ui/media/
+-rwxr-xr-x   0 root         (0) root         (0)   135652 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/RucioUI.png
+-rw-r--r--   0 root         (0) root         (0)      686 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/details_close.png
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/details_open.png
+-rw-r--r--   0 root         (0) root         (0)    84798 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/error.jpg
+-rw-r--r--   0 root         (0) root         (0)    10510 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.725326 rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/
+-rwxr-xr-x   0 root         (0) root         (0)     3400 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.eot
+-rwxr-xr-x   0 root         (0) root         (0)     9218 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.svg
+-rwxr-xr-x   0 root         (0) root         (0)     3236 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.ttf
+-rwxr-xr-x   0 root         (0) root         (0)     3312 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.woff
+-rw-r--r--   0 root         (0) root         (0)      753 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/get_info.png
+-rw-r--r--   0 root         (0) root         (0)    56517 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/logo.png
+-rw-r--r--   0 root         (0) root         (0)    19563 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/rucio_logo.png
+-rw-r--r--   0 root         (0) root         (0)    32246 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/spinner.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.738326 rucio-webui-34.1.0/lib/rucio/web/ui/static/
+-rw-r--r--   0 root         (0) root         (0)     6764 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/account.js
+-rw-r--r--   0 root         (0) root         (0)     8084 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/account_rse_usage.js
+-rw-r--r--   0 root         (0) root         (0)    12181 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/account_usage.js
+-rw-r--r--   0 root         (0) root         (0)     7667 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/account_usage_history.js
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/accounting.js
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/accounts.js
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/add_rse.js
+-rw-r--r--   0 root         (0) root         (0)    12226 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/approve_rules.js
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/atlas_index.js
+-rw-r--r--   0 root         (0) root         (0)    15169 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/backlog_mon.js
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/bad_replicas.js
+-rw-r--r--   0 root         (0) root         (0)    11540 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/bad_replicas_summary.js
+-rw-r--r--   0 root         (0) root         (0)     7366 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/base.js
+-rw-r--r--   0 root         (0) root         (0)      538 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen-sprite.png
+-rw-r--r--   0 root         (0) root         (0)      738 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen-sprite@2x.png
+-rw-r--r--   0 root         (0) root         (0)    13270 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.css
+-rw-r--r--   0 root         (0) root         (0)    44811 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.jquery.js
+-rw-r--r--   0 root         (0) root         (0)    28401 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    11061 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.min.css
+-rw-r--r--   0 root         (0) root         (0)    45100 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.proto.js
+-rw-r--r--   0 root         (0) root         (0)    28757 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.proto.min.js
+-rw-r--r--   0 root         (0) root         (0)     5641 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/cond.js
+-rw-r--r--   0 root         (0) root         (0)     5758 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/dbrelease.js
+-rw-r--r--   0 root         (0) root         (0)    43648 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/did.js
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/filesize.min.js
+-rw-r--r--   0 root         (0) root         (0)    19507 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.css
+-rw-r--r--   0 root         (0) root         (0)    54568 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.eot
+-rw-r--r--   0 root         (0) root         (0)   150251 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.svg
+-rw-r--r--   0 root         (0) root         (0)    56976 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)    32020 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.woff
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/heartbeats.js
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring.css
+-rw-r--r--   0 root         (0) root         (0)    12386 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_account_details.js
+-rw-r--r--   0 root         (0) root         (0)     3525 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_accounts.js
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js
+-rw-r--r--   0 root         (0) root         (0)     3795 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_apiclasses.js
+-rw-r--r--   0 root         (0) root         (0)     3555 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_index.js
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_resources.js
+-rw-r--r--   0 root         (0) root         (0)     8872 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js
+-rw-r--r--   0 root         (0) root         (0)     3055 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_scriptids.js
+-rw-r--r--   0 root         (0) root         (0)    10028 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_utils.js
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/index.js
+-rw-r--r--   0 root         (0) root         (0)    23108 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.multiple.select.js
+-rw-r--r--   0 root         (0) root         (0)    20021 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.multiple.select2.js
+-rw-r--r--   0 root         (0) root         (0)     4151 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.quicksearch.js
+-rw-r--r--   0 root         (0) root         (0)     6966 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.storageapi.min.js
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/lifetime_exception.js
+-rw-r--r--   0 root         (0) root         (0)     4060 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/list_lifetime_exceptions.js
+-rw-r--r--   0 root         (0) root         (0)    13472 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/list_rules.js
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/login.js
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/multiple-select.css
+-rw-r--r--   0 root         (0) root         (0)     3342 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/multiple-select.png
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/multiple-select2.css
+-rw-r--r--   0 root         (0) root         (0)    54419 2024-03-13 10:19:28.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/request_rule.js
+-rw-r--r--   0 root         (0) root         (0)     7089 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rse.js
+-rw-r--r--   0 root         (0) root         (0)    23373 2024-03-13 10:19:28.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_account_usage.js
+-rw-r--r--   0 root         (0) root         (0)     7076 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_add_protocol.js
+-rw-r--r--   0 root         (0) root         (0)     6559 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_locks.js
+-rw-r--r--   0 root         (0) root         (0)    10905 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_usage.js
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rses.js
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rucio.css
+-rw-r--r--   0 root         (0) root         (0)    63519 2024-03-13 10:19:28.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rucio.js
+-rw-r--r--   0 root         (0) root         (0)    23335 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rule.js
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rules.js
+-rw-r--r--   0 root         (0) root         (0)     6323 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/search.js
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/select_login_method.css
+-rw-r--r--   0 root         (0) root         (0)     7637 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/subscription.js
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/subscriptionrules.js
+-rw-r--r--   0 root         (0) root         (0)     4946 2024-03-13 10:19:28.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/subscriptions.js
+-rw-r--r--   0 root         (0) root         (0)    13983 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/subscriptions_editor.js
+-rw-r--r--   0 root         (0) root         (0)     9784 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/suspicious_replicas.js
+-rw-r--r--   0 root         (0) root         (0)      540 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/switch.png
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/version.js
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-02 11:50:17.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/webui_version
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.756327 rucio-webui-34.1.0/lib/rucio_webui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8846 2024-04-02 13:57:13.000000 rucio-webui-34.1.0/lib/rucio_webui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2024-03-13 10:19:28.000000 rucio-webui-34.1.0/pylintrc
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5048 2024-03-19 15:04:29.000000 rucio-webui-34.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2024-04-02 13:57:13.758327 rucio-webui-34.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2128 2024-04-02 13:57:10.000000 rucio-webui-34.1.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.756327 rucio-webui-34.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10677 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20523 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13352 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    15058 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23264 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12425 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107413 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     6929 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6942 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    96558 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    23797 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7679 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7337 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28187 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    58823 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29517 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16419 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10867 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38301 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10106 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5819 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18584 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57223 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5258 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22277 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20428 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12180 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54264 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11582 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   108356 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7583 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27487 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62385 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    38873 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22741 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    17184 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    12978 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75019 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13184 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8941 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4799 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     3979 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7746 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    91864 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)    13848 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_schema_cms.py
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48328 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    55587 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    25254 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8923 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_transfer_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    15526 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_utils.py
```

### Comparing `rucio-webui-34.0.0rc2/AUTHORS.rst` & `rucio-webui-34.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/LICENSE` & `rucio-webui-34.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/PKG-INFO` & `rucio-webui-34.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio-webui
-Version: 34.0.0rc2
+Version: 34.1.0
 Summary: Rucio WebUI Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rucio-webui-34.0.0rc2/README.rst` & `rucio-webui-34.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/__init__.py` & `rucio-webui-34.1.0/lib/rucio/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/alembicrevision.py` & `rucio-webui-34.1.0/lib/rucio/alembicrevision.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/version.py` & `rucio-webui-34.1.0/lib/rucio/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/__init__.py` & `rucio-webui-34.1.0/lib/rucio/web/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/__init__.py` & `rucio-webui-34.1.0/lib/rucio/web/ui/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/__init__.py` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/bp.py` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/bp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from flask import Blueprint, request, render_template, make_response
+from flask import Blueprint, make_response, render_template, request
 
 from rucio.api.authentication import get_auth_token_x509
 from rucio.common.config import config_get, config_get_bool
 from rucio.web.rest.flaskapi.v1.common import generate_http_error_flask
-from rucio.web.ui.flask.common.utils import get_token, authenticate, userpass_auth, x509token_auth, saml_auth, oidc_auth, finalize_auth, AUTH_ISSUERS, SAML_SUPPORT
+from rucio.web.ui.flask.common.utils import AUTH_ISSUERS, SAML_SUPPORT, authenticate, finalize_auth, get_token, oidc_auth, saml_auth, userpass_auth, x509token_auth
 
 MULTI_VO = config_get_bool('common', 'multi_vo', raise_exception=False, default=False)
 POLICY = config_get('policy', 'permission')
 ATLAS_URLS = ()
 OTHER_URLS = ()
```

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/common/__init__.py` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/common/saml/advanced_settings.json` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/advanced_settings.json`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/common/saml/settings.json` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/settings.json`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/common/utils.py` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -17,22 +16,24 @@
 import html
 import re
 from json import dumps, load
 from os.path import dirname, join
 from time import time
 from urllib.parse import quote, unquote
 
-from flask import request, render_template, redirect, make_response
+from flask import make_response, redirect, render_template, request
 
-from rucio.api import authentication as auth, identity
+from rucio.api import authentication as auth
+from rucio.api import identity
 from rucio.api.account import account_exists, get_account_info, list_account_attributes
 from rucio.common.config import config_get, config_get_bool
 from rucio.common.exception import CannotAuthenticate
 from rucio.common.extra import import_extras
-from rucio.core import identity as identity_core, vo as vo_core
+from rucio.core import identity as identity_core
+from rucio.core import vo as vo_core
 from rucio.db.sqla.constants import AccountType, IdentityType
 
 EXTRA_MODULES = import_extras(['onelogin'])
 
 if EXTRA_MODULES['onelogin']:
     from onelogin.saml2.auth import OneLogin_Saml2_Auth  # pylint: disable=import-error
```

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/main.py` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/account.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/account_rse_usage.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account_rse_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/account_usage.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/account_usage_history.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account_usage_history.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/accounting.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/accounting.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/accounts.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/accounts.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/add_rse.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/add_rse.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/approve_rules.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/approve_rules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/atlas_index.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/atlas_index.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/backlog_mon.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/backlog_mon.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/bad_replicas.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/bad_replicas.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/base.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/base.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/cond.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/cond.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/dbrelease.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/dbrelease.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/did.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/did.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/dumps.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/dumps.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/heartbeats.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/heartbeats.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/index.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/index.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/infrastructure.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/infrastructure.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/lifetime_exception.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/lifetime_exception.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/list_rules.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/list_rules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/login.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/login.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/no_certificate.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/no_certificate.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/problem.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/problem.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/request_rule.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/request_rule.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rse.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rse_account_usage.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_account_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rse_add_protocol.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_add_protocol.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rse_locks.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_locks.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rse_usage.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rses.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rses.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rule.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rule.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/rules.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/search.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/search.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/select_login_method.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/select_login_method.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/subscription.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscription.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/subscriptionrules.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscriptionrules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/subscriptions.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscriptions.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/subscriptions_editor.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscriptions_editor.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/flask/templates/suspicious_replicas.html` & `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/suspicious_replicas.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/main.py` & `rucio-webui-34.1.0/lib/rucio/web/ui/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/RucioUI.png` & `rucio-webui-34.1.0/lib/rucio/web/ui/media/RucioUI.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/details_close.png` & `rucio-webui-34.1.0/lib/rucio/web/ui/media/details_close.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/details_open.png` & `rucio-webui-34.1.0/lib/rucio/web/ui/media/details_open.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/error.jpg` & `rucio-webui-34.1.0/lib/rucio/web/ui/media/error.jpg`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/favicon.ico` & `rucio-webui-34.1.0/lib/rucio/web/ui/media/favicon.ico`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.eot` & `rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.eot`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.svg` & `rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.svg`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.ttf` & `rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.ttf`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.woff` & `rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.woff`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/get_info.png` & `rucio-webui-34.1.0/lib/rucio/web/ui/media/get_info.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/logo.png` & `rucio-webui-34.1.0/lib/rucio/web/ui/media/logo.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/rucio_logo.png` & `rucio-webui-34.1.0/lib/rucio/web/ui/media/rucio_logo.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/media/spinner.gif` & `rucio-webui-34.1.0/lib/rucio/web/ui/media/spinner.gif`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/account.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/account.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/account_rse_usage.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/account_rse_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/account_usage.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/account_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/account_usage_history.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/account_usage_history.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/accounting.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/accounting.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/accounts.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/accounts.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/add_rse.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/add_rse.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/approve_rules.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/approve_rules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/atlas_index.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/atlas_index.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/backlog_mon.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/backlog_mon.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/bad_replicas.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/bad_replicas.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/bad_replicas_summary.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/bad_replicas_summary.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/base.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/base.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen-sprite.png` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen-sprite@2x.png` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen.css` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen.jquery.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.jquery.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen.jquery.min.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen.min.css` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.min.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen.proto.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.proto.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/chosen.proto.min.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.proto.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/cond.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/cond.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/dbrelease.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/dbrelease.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/did.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/did.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/filesize.min.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/filesize.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/foundation-icons.css` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/foundation-icons.eot` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.eot`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/foundation-icons.svg` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.svg`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/foundation-icons.ttf` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.ttf`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/foundation-icons.woff` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.woff`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/heartbeats.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/heartbeats.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring.css` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_account_details.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_account_details.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_accounts.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_accounts.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_apiclasses.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_apiclasses.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_index.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_index.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_resources.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_resources.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_scriptids.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_scriptids.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/http_monitoring_utils.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_utils.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/jquery.multiple.select.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.multiple.select.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/jquery.multiple.select2.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.multiple.select2.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/jquery.quicksearch.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.quicksearch.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/jquery.storageapi.min.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.storageapi.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/lifetime_exception.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/lifetime_exception.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/list_lifetime_exceptions.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/list_lifetime_exceptions.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/list_rules.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/list_rules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/multiple-select.css` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/multiple-select.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/multiple-select.png` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/multiple-select.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/multiple-select2.css` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/multiple-select2.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/request_rule.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/request_rule.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rse.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/rse.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rse_account_usage.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_account_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rse_add_protocol.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_add_protocol.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rse_locks.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_locks.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rse_usage.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rses.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/rses.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rucio.css` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/rucio.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rucio.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/rucio.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rule.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/rule.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/rules.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/rules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/search.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/search.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/select_login_method.css` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/select_login_method.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/subscription.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/subscription.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/subscriptionrules.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/subscriptionrules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/subscriptions.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/subscriptions.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/subscriptions_editor.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/subscriptions_editor.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/suspicious_replicas.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/suspicious_replicas.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/switch.png` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/switch.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio/web/ui/static/version.js` & `rucio-webui-34.1.0/lib/rucio/web/ui/static/version.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/lib/rucio_webui.egg-info/SOURCES.txt` & `rucio-webui-34.1.0/lib/rucio_webui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/pylintrc` & `rucio-webui-34.1.0/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/requirements.txt` & `rucio-webui-34.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.0.0rc2/setup.py` & `rucio-webui-34.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -14,15 +13,14 @@
 # limitations under the License.
 
 import os
 import sys
 
 from setuptools import setup
 
-
 if sys.version_info < (3, 9):
     print('ERROR: Rucio WebUI requires at least Python 3.9 to run.')
     sys.exit(1)
 
 try:
     from setuputil import get_rucio_version
 except ImportError:
```

### Comparing `rucio-webui-34.0.0rc2/setuputil.py` & `rucio-webui-34.1.0/setuputil.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -12,16 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import subprocess
 import sys
 
-from pkg_resources import safe_name, parse_requirements
-
+from pkg_resources import parse_requirements, safe_name
 
 clients_requirements_table = {
     'install_requires': [
         'requests',
         'urllib3',
         'dogpile.cache',
         'tabulate',
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_abacus_account.py` & `rucio-webui-34.1.0/tests/test_abacus_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -24,15 +23,15 @@
 from rucio.daemons.judge import cleaner
 from rucio.daemons.reaper import reaper
 from rucio.db.sqla import models
 from rucio.db.sqla.session import get_session
 
 
 @pytest.mark.noparallel(reason='uses daemon, failing in parallel to other tests, updates account')
-class TestAbacusAccount2():
+class TestAbacusAccount2:
 
     def test_abacus_account(self, vo, root_account, mock_scope, rse_factory, did_factory, rucio_client):
         """ ABACUS (ACCOUNT): Test update of account usage """
         session = get_session()
         session.query(models.UpdatedAccountCounter).delete()  # pylint: disable=no-member
         session.query(models.AccountUsage).delete()  # pylint: disable=no-member
         session.commit()  # pylint: disable=no-member
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_abacus_collection_replica.py` & `rucio-webui-34.1.0/tests/test_abacus_collection_replica.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -26,15 +25,15 @@
 from rucio.daemons.undertaker import undertaker
 from rucio.db.sqla import models, session
 from rucio.db.sqla.constants import DIDType, ReplicaState
 from rucio.tests.common import did_name_generator
 
 
 @pytest.mark.noparallel(reason='uses daemons, fails when run in parallel')
-class TestAbacusCollectionReplica():
+class TestAbacusCollectionReplica:
 
     def test_abacus_collection_replica_cleanup(self, vo, mock_scope, rse_factory, did_client, jdoe_account):
         """ ABACUS (COLLECTION REPLICA): Test if the cleanup procedure works correctly. """
         collection_replica.run(once=True)
         db_session = session.get_session()
         rse1, rse_id1 = rse_factory.make_rse()
         rse2, rse_id2 = rse_factory.make_rse()
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_abacus_rse.py` & `rucio-webui-34.1.0/tests/test_abacus_rse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -21,15 +20,15 @@
 from rucio.daemons.judge import cleaner
 from rucio.daemons.reaper import reaper
 from rucio.db.sqla import models
 from rucio.db.sqla.session import get_session
 
 
 @pytest.mark.noparallel(reason='uses daemon, failing in parallel to other tests')
-class TestAbacusRSE():
+class TestAbacusRSE:
 
     def test_abacus_rse(self, vo, mock_scope, rse_factory, did_factory, rucio_client):
         """ ABACUS (RSE): Test update of RSE usage. """
         # Get RSE usage of all sources
         session = get_session()
         session.query(models.UpdatedRSECounter).delete()  # pylint: disable=no-member
         session.query(models.RSEUsage).delete()  # pylint: disable=no-member
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_account.py` & `rucio-webui-34.1.0/tests/test_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -13,23 +12,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from json import loads
 
 import pytest
 
-from rucio.api.account import add_account, account_exists, del_account, update_account, get_account_info
+from rucio.api.account import account_exists, add_account, del_account, get_account_info, update_account
 from rucio.common.config import config_get
 from rucio.common.exception import AccountNotFound, Duplicate, InvalidObject
 from rucio.common.types import InternalAccount
 from rucio.common.utils import generate_uuid as uuid
-from rucio.core.account import list_identities, add_account_attribute, list_account_attributes, del_account_attribute
+from rucio.core.account import add_account_attribute, del_account_attribute, list_account_attributes, list_identities
 from rucio.core.identity import add_account_identity, add_identity
 from rucio.db.sqla.constants import AccountStatus, IdentityType
-from rucio.tests.common import account_name_generator, headers, auth, vohdr, loginhdr, skip_non_belleii
+from rucio.tests.common import account_name_generator, auth, headers, loginhdr, skip_non_belleii, vohdr
 
 
 class TestAccountCoreApi:
 
     def test_create_and_check_for_user(self, vo):
         """ ACCOUNT (CORE): Test the creation, query, and deletion of an account """
         usr = account_name_generator()
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_account_limits.py` & `rucio-webui-34.1.0/tests/test_account_limits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -10,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
+
 from rucio.core import account_limit
 
 
 @pytest.fixture
 def account(random_account):
     yield random_account
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_api_external_representation.py` & `rucio-webui-34.1.0/tests/test_api_external_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -26,26 +25,25 @@
 from rucio.api.account import add_account, get_account_info, list_accounts
 from rucio.api.did import add_did, add_did_to_followed, attach_dids_to_dids, get_users_following_did, scope_list
 from rucio.api.exporter import export_data
 from rucio.api.identity import add_account_identity, list_accounts_for_identity
 from rucio.api.replica import add_replicas, get_did_from_pfns, list_replicas
 from rucio.api.request import get_request_by_did, list_requests, queue_requests
 from rucio.api.rule import add_replication_rule
-from rucio.api.scope import add_scope, list_scopes, get_scopes
-from rucio.api.subscription import add_subscription, list_subscriptions, list_subscription_rule_states, \
-    get_subscription_by_id
+from rucio.api.scope import add_scope, get_scopes, list_scopes
+from rucio.api.subscription import add_subscription, get_subscription_by_id, list_subscription_rule_states, list_subscriptions
 from rucio.common.config import config_get_bool
 from rucio.common.types import InternalScope
 from rucio.common.utils import api_update_return_dict, generate_uuid
 from rucio.core.vo import add_vo, vo_exists
 from rucio.daemons.abacus import rse as abacus_rse
 from rucio.daemons.judge import cleaner
 from rucio.daemons.reaper import reaper
 from rucio.db.sqla import constants
-from rucio.tests.common import rse_name_generator, did_name_generator
+from rucio.tests.common import did_name_generator, rse_name_generator
 
 
 @pytest.fixture(scope='class')
 def vo2():
     if config_get_bool('common', 'multi_vo', raise_exception=False, default=False):
         vo2 = 'new'
         if not vo_exists(vo=vo2):
@@ -438,15 +436,15 @@
         add_did(new_scope_name, did, 'DATASET', 'root', account=new_acc_name, rse=self.rse3_name, vo=test_vo)
 
         sub_id = add_subscription(sub, new_acc_name, {'account': [new_acc_name], 'scope': [new_scope_name]},
                                   [{'copies': 1, 'rse_expression': self.rse3_name, 'weight': 0, 'activity': 'Functional Test',
                                     'source_replica_expression': self.rse4_name}],
                                   '', False, 0, 0, 3, 'root', vo=test_vo)
         add_replication_rule(dids=[{'scope': new_scope_name, 'name': did}], copies=1, rse_expression=self.rse3_name, weight=None,
-                             lifetime=180, grouping='DATASET', account=new_acc_name, locked=False, subscription_id=sub_id,
+                             lifetime=None, grouping='DATASET', account=new_acc_name, locked=False, subscription_id=sub_id,
                              source_replica_expression=self.rse4_name, activity='Functional Test', notify=None,
                              purge_replicas=False, ignore_availability=False, comment='', ask_approval=False, asynchronous=False,
                              delay_injection=None, priority=0, split_container=False, meta='', issuer='root', vo=test_vo)
 
         out = list_subscriptions(sub, vo=test_vo)
         out = list(out)
         assert 0 != len(out)
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_archive.py` & `rucio-webui-34.1.0/tests/test_archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -10,17 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from rucio.common.utils import generate_uuid
+from rucio.core.did import attach_dids, get_metadata
 from rucio.core.replica import add_replicas, delete_replicas
 from rucio.core.rse import add_protocol, update_rse
-from rucio.core.did import attach_dids, get_metadata
 
 
 def test_add_and_list_archive(rse_factory, replica_client, did_client, mock_scope):
     """  ARCHIVE (CLIENT): Add files to archive and list the content """
     rse, _ = rse_factory.make_mock_rse()
     scope = mock_scope.external
     archive_files = ['file_' + generate_uuid() + '.zip' for _ in range(2)]
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_auditor.py` & `rucio-webui-34.1.0/tests/test_auditor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -14,16 +13,15 @@
 # limitations under the License.
 
 import bz2
 import collections
 import multiprocessing
 import os
 import tempfile
-from datetime import datetime
-from datetime import timedelta
+from datetime import datetime, timedelta
 from unittest import mock
 
 import pytest
 
 from rucio.daemons import auditor
 
 
@@ -105,15 +103,15 @@
     queue.put(('RSE_SHOULD_WORK', 1))
     queue.put(('RSE_WITH_ERROR', 1))
     wr_pipe = collections.namedtuple('FakePipe', ('send', 'close'))(
         lambda _: None,
         lambda: None,
     )
 
-    class MockMultiProcessing():
+    class MockMultiProcessing:
         def is_set(self):
             return queue.empty()
     terminate = MockMultiProcessing()
     auditor.check(queue, retry, terminate, wr_pipe, None, None, 3, False)
 
     assert queue.empty()
     assert retry.get() == ('RSE_WITH_EXCEPTION', 0)
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_auditor_hdfs.py` & `rucio-webui-34.1.0/tests/test_auditor_hdfs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -19,15 +18,15 @@
 from unittest import mock
 
 import pytest
 
 from rucio.daemons.auditor import hdfs
 
 
-class FakeHDFSGet(object):
+class FakeHDFSGet:
     def __init__(self, files=[]):
         self.files = files
 
     def __call__(self, src_path, dst_dir):
         # src_path is ignored, it is assumed a directory is requested
         for content, name in self.files:
             with open(os.path.join(dst_dir, name), 'w') as fichier:
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_auditor_srmdumps.py` & `rucio-webui-34.1.0/tests/test_auditor_srmdumps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_authentication.py` & `rucio-webui-34.1.0/tests/test_authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -10,29 +9,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import base64
-
 import datetime
+import time
+
 import pytest
 from requests import session
-import time
 
-from rucio.api.authentication import get_auth_token_user_pass, get_auth_token_ssh, get_ssh_challenge_token, \
-    get_auth_token_saml
-from rucio.common.exception import Duplicate, AccessDenied, CannotAuthenticate
+from rucio.api.authentication import get_auth_token_saml, get_auth_token_ssh, get_auth_token_user_pass, get_ssh_challenge_token
+from rucio.common.exception import AccessDenied, CannotAuthenticate, Duplicate
 from rucio.common.utils import ssh_sign
-from rucio.core.identity import add_account_identity, del_account_identity
 from rucio.core.authentication import strip_x509_proxy_attributes
+from rucio.core.identity import add_account_identity, del_account_identity
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import IdentityType
-from rucio.tests.common import headers, hdrdict, loginhdr, vohdr
+from rucio.tests.common import hdrdict, headers, loginhdr, vohdr
 
 PUBLIC_KEY = "ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEAq5LySllrQFpPL"\
              "614sulXQ7wnIr1aGhGtl8b+HCB/0FhMSMTHwSjX78UbfqEorZ"\
              "V16rXrWPgUpvcbp2hqctw6eCbxwqcgu3uGWaeS5A0iWRw7oXU"\
              "h6ydnVy89zGzX1FJFFDZ+AgiZ3ytp55tg1bjqqhK1OSC0pJxd"\
              "Ne878TRVVo5MLI0S/rZY2UovCSGFaQG2iLj14wz/YqI7NFMUu"\
              "JFR4e6xmNsOP7fCZ4bGMsmnhR0GmY0dWYTupNiP5WdYXAfKEx"\
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_automatix.py` & `rucio-webui-34.1.0/tests/test_automatix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -11,23 +10,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os
+import tempfile
 from random import choice
 from string import ascii_uppercase
-import tempfile
 
 import pytest
 
-from rucio.common.config import config_add_section, config_has_section, config_set, config_remove_option
+from rucio.common.config import config_add_section, config_has_section, config_remove_option, config_set
 from rucio.common.types import InternalScope
-from rucio.core.did import list_dids, list_files, get_metadata
+from rucio.core.did import get_metadata, list_dids, list_files
 from rucio.core.scope import add_scope
 from rucio.daemons.automatix.automatix import automatix
 from rucio.rse import rsemanager as rsemgr
 from rucio.tests.common import scope_name_generator
 
 
 @pytest.mark.noparallel(reason='changes global configuration value')
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_bad_replica.py` & `rucio-webui-34.1.0/tests/test_bad_replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -14,27 +13,25 @@
 # limitations under the License.
 
 from datetime import datetime, timedelta
 from json import dumps, loads
 
 import pytest
 
-from rucio.common.exception import RucioException, UnsupportedOperation, InvalidType
-from rucio.common.utils import generate_uuid, clean_surls
-from rucio.core.did import delete_dids
-from rucio.core.replica import (add_replicas, get_replicas_state, list_replicas,
-                                declare_bad_file_replicas, list_bad_replicas, get_bad_pfns,
-                                get_bad_replicas_backlog, list_bad_replicas_status, get_pfn_to_rse)
 from rucio.client.rseclient import RSEClient
+from rucio.common.exception import InvalidType, RucioException, UnsupportedOperation
+from rucio.common.utils import clean_surls, generate_uuid
+from rucio.core.did import delete_dids
+from rucio.core.replica import add_replicas, declare_bad_file_replicas, get_bad_pfns, get_bad_replicas_backlog, get_pfn_to_rse, get_replicas_state, list_bad_replicas, list_bad_replicas_status, list_replicas
 from rucio.daemons.badreplicas.minos import run as minos_run
 from rucio.daemons.badreplicas.minos_temporary_expiration import run as minos_temp_run
-from rucio.daemons.badreplicas.necromancer import run as necromancer_run
 from rucio.daemons.badreplicas.necromancer import REGION
-from rucio.db.sqla.constants import DIDType, ReplicaState, BadPFNStatus, BadFilesStatus
-from rucio.tests.common import headers, auth
+from rucio.daemons.badreplicas.necromancer import run as necromancer_run
+from rucio.db.sqla.constants import BadFilesStatus, BadPFNStatus, DIDType, ReplicaState
+from rucio.tests.common import auth, headers
 
 
 @pytest.fixture
 def rse_client():
     return RSEClient()
 
 
@@ -246,15 +243,15 @@
         for badrep in bad_replicas:
             if badrep['rse_id'] == rse3_id:
                 if badrep['scope'].external == rep['scope'] and badrep['name'] == rep['name']:
                     nbbadrep += 1
     assert len(replicas) == nbbadrep
 
     list_rep.extend(['srm://%s.cern.ch/test_%s/%s/%s' % (rse2_id, rse2_id, tmp_scope, generate_uuid()), ])
-    with pytest.raises(InvalidType):    
+    with pytest.raises(InvalidType):
         # this should fail becase the replica list will now contain a mix of PFNs and dictionaries
         replica_client.declare_bad_file_replicas(list_rep, 'This is a good reason')
 
 
 def test_client_add_suspicious_replicas(rse_factory, replica_client):
     """ REPLICA (CLIENT): Add suspicious replicas"""
     tmp_scope = 'mock'
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_bb8.py` & `rucio-webui-34.1.0/tests/test_bb8.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,27 +14,28 @@
 
 from datetime import datetime, timedelta
 
 import pytest
 
 from rucio.common.exception import RuleNotFound, UnsupportedOperation
 from rucio.core.account_limit import set_local_account_limit
-from rucio.core.did import attach_dids, set_status, set_metadata
+from rucio.core.did import attach_dids, set_metadata, set_status
 from rucio.core.lock import successful_transfer
 from rucio.core.replica import add_replicas
 from rucio.core.rse import add_rse_attribute, fill_rse_expired, get_rse_usage, set_rse_usage
-from rucio.core.rule import add_rule, get_rule, delete_rule, update_rule
 from rucio.core.rse_expression_parser import REGION
+from rucio.core.rule import add_rule, delete_rule, get_rule, update_rule
 from rucio.daemons.abacus.rse import run as run_abacus
-from rucio.daemons.bb8.common import rebalance_rule
 from rucio.daemons.bb8.bb8 import run as bb8_run
+from rucio.daemons.bb8.common import rebalance_rule
 from rucio.daemons.judge.cleaner import rule_cleaner
 from rucio.daemons.judge.evaluator import re_evaluator
 from rucio.daemons.undertaker import undertaker
 from rucio.db.sqla.constants import RuleState
+
 from .test_rule import create_files, tag_generator
 
 
 @pytest.mark.noparallel(reason='uses daemons')
 def test_bb8_rebalance_rule(vo, root_account, jdoe_account, rse_factory, mock_scope, did_factory):
     """BB8: Test the rebalance rule method"""
     rse1, rse1_id = rse_factory.make_posix_rse()
@@ -155,18 +155,18 @@
     nb_files3 = 3
     nb_files4 = 2
     file_size = 1 * base_unit
     rule_to_rebalance = None
 
     # Add one secondary file
     files = create_files(1, mock_scope, rse1_id, bytes_=1)
-    add_rule(dids=[{'scope': mock_scope, 'name': files[0]['name']}], account=jdoe_account, copies=1, rse_expression=rse1, grouping='DATASET', weight=None, lifetime=-86400, locked=False, subscription_id=None)[0]
+    add_rule(dids=[{'scope': mock_scope, 'name': files[0]['name']}], account=jdoe_account, copies=1, rse_expression=rse1, grouping='DATASET', weight=None, lifetime=-1, locked=False, subscription_id=None)[0]
     for cnt in range(3, tot_rses):
         add_replicas(rses[cnt][1], files, jdoe_account)
-        add_rule(dids=[{'scope': mock_scope, 'name': files[0]['name']}], account=jdoe_account, copies=1, rse_expression=rses[cnt][0], grouping='DATASET', weight=None, lifetime=-86400, locked=False, subscription_id=None)[0]
+        add_rule(dids=[{'scope': mock_scope, 'name': files[0]['name']}], account=jdoe_account, copies=1, rse_expression=rses[cnt][0], grouping='DATASET', weight=None, lifetime=-1, locked=False, subscription_id=None)[0]
     rule_cleaner(once=True)
 
     # Create dataset 1 of 800 GB and create a rule on RSE 1 and RSE 3
     files = create_files(nb_files1, mock_scope, rse1_id, bytes_=file_size)
     attach_dids(mock_scope, dsn[0], files, jdoe_account)
 
     rule_id = add_rule(dids=[{'scope': mock_scope, 'name': dsn[0]}], account=jdoe_account, copies=1, rse_expression=rse1, grouping='DATASET', weight=None, lifetime=None, locked=False, subscription_id=None)[0]
@@ -192,30 +192,30 @@
     attach_dids(mock_scope, dsn[2], files, jdoe_account)
 
     rule_id = add_rule(dids=[{'scope': mock_scope, 'name': dsn[2]}], account=jdoe_account, copies=1, rse_expression=rse1, grouping='DATASET', weight=None, lifetime=None, locked=False, subscription_id=None)[0]
     rule_to_rebalance = rule_id
     rules.append(rule_id)
 
     add_replicas(rse3_id, files, jdoe_account)
-    rule_id = add_rule(dids=[{'scope': mock_scope, 'name': dsn[2]}], account=jdoe_account, copies=1, rse_expression=rse3, grouping='DATASET', weight=None, lifetime=-86400, locked=False, subscription_id=None)[0]
+    rule_id = add_rule(dids=[{'scope': mock_scope, 'name': dsn[2]}], account=jdoe_account, copies=1, rse_expression=rse3, grouping='DATASET', weight=None, lifetime=-1, locked=False, subscription_id=None)[0]
     rule_cleaner(once=True)
     try:
         rule = get_rule(rule_id)
     except:
         pytest.raises(RuleNotFound, get_rule, rule_id)
 
     # Create dataset 4 of 200 GB and create a rule on RSE 3. The copy on RSE 2 is secondary
     files = create_files(nb_files4, mock_scope, rse3_id, bytes_=file_size)
     attach_dids(mock_scope, dsn[3], files, jdoe_account)
 
     rule_id = add_rule(dids=[{'scope': mock_scope, 'name': dsn[3]}], account=jdoe_account, copies=1, rse_expression=rse3, grouping='DATASET', weight=None, lifetime=None, locked=False, subscription_id=None)[0]
     rules.append(rule_id)
 
     add_replicas(rse2_id, files, jdoe_account)
-    rule_id = add_rule(dids=[{'scope': mock_scope, 'name': dsn[3]}], account=jdoe_account, copies=1, rse_expression=rse2, grouping='DATASET', weight=None, lifetime=-86400, locked=False, subscription_id=None)[0]
+    rule_id = add_rule(dids=[{'scope': mock_scope, 'name': dsn[3]}], account=jdoe_account, copies=1, rse_expression=rse2, grouping='DATASET', weight=None, lifetime=-1, locked=False, subscription_id=None)[0]
     rule_cleaner(once=True)
     try:
         rule = get_rule(rule_id)
     except:
         pytest.raises(RuleNotFound, get_rule, rule_id)
 
     for dataset in dsn:
@@ -258,13 +258,13 @@
         else:
             assert (rule['child_rule_id'] is not None)
             assert (rule['expires_at'] <= datetime.utcnow() + timedelta(seconds=1))  # timedelta needed to prevent failure due to rounding effects
             child_rule_id = rule['child_rule_id']
             child_rule = get_rule(child_rule_id)
             assert (child_rule['rse_expression'] == rse2)
             # For teardown, delete child rule
-            update_rule(child_rule_id, {'lifetime': -86400})
+            update_rule(child_rule_id, {'lifetime': -1})
     rule_cleaner(once=True)
 
     for dataset in dsn:
         set_metadata(mock_scope, dataset, 'lifetime', -86400)
     undertaker.run(once=True)
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_belleii.py` & `rucio-webui-34.1.0/tests/test_belleii.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +14,15 @@
 
 from datetime import datetime
 
 import pytest
 
 from rucio.common.exception import InvalidObject
 from rucio.common.schema.belleii import validate_schema
-from rucio.common.utils import generate_uuid, extract_scope
+from rucio.common.utils import extract_scope, generate_uuid
 from rucio.core.config import set as config_set
 from rucio.tests.common import did_name_generator, skip_non_belleii
 
 
 @skip_non_belleii
 def test_dirac_addfile(rse_factory, did_factory, root_account, did_client, dirac_client, rse_client, replica_client):
     """ DIRAC (CLIENT): Test the functionality of the addfile method """
@@ -102,15 +101,15 @@
     dataset_meta = {'project': 'data13_hip', 'run_number': 300000, 'mykey': 'myvalue'}
     container_meta = {'containerkey': 'containervalue'}
     parents_metadata = {dataset: dataset_meta, container: container_meta}
     dirac_client.add_files(lfns=lfns, ignore_availability=False, parents_metadata=parents_metadata)
     replicas = [rep for rep in replica_client.list_replicas(dids=files)]
     for replica in replicas:
         assert {'scope': replica['scope'], 'name': replica['name'], 'rse': list(replica['rses'].keys())[0]} in reps
-    
+
     # check if metadata if properly created for file and parents
     for lfn in lfns:
         scope, name = extract_scope(lfn['lfn'], [])
         metadata = did_client.get_metadata(scope, name, plugin='ALL')
         assert all(item in metadata.items() for item in lfn_meta.items())
         dsn_scope, dsn_name = extract_scope(dataset, [])
         metadata = did_client.get_metadata(dsn_scope, dsn_name, plugin='ALL')
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_bin_rucio.py` & `rucio-webui-34.1.0/tests/test_bin_rucio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -14,30 +13,30 @@
 # limitations under the License.
 
 import os
 import random
 import re
 import tempfile
 from datetime import datetime, timedelta
-from os import remove, unlink, listdir, rmdir, stat, path, environ
+from os import environ, listdir, path, remove, rmdir, stat, unlink
 
 import pytest
 
 from rucio.client.accountlimitclient import AccountLimitClient
+from rucio.client.configclient import ConfigClient
 from rucio.client.didclient import DIDClient
+from rucio.client.lifetimeclient import LifetimeClient
 from rucio.client.replicaclient import ReplicaClient
 from rucio.client.rseclient import RSEClient
 from rucio.client.ruleclient import RuleClient
-from rucio.client.configclient import ConfigClient
-from rucio.client.lifetimeclient import LifetimeClient
 from rucio.common.config import config_get, config_get_bool
-from rucio.common.types import InternalScope, InternalAccount
+from rucio.common.types import InternalAccount, InternalScope
 from rucio.common.utils import generate_uuid, get_tmp_dir, md5, render_json
 from rucio.rse import rsemanager as rsemgr
-from rucio.tests.common import execute, account_name_generator, rse_name_generator, file_generator, scope_name_generator, get_long_vo
+from rucio.tests.common import account_name_generator, execute, file_generator, get_long_vo, rse_name_generator, scope_name_generator
 
 
 class TestBinRucio:
 
     def conf_vo(self):
         self.vo = {}
         if config_get_bool('common', 'multi_vo', raise_exception=False, default=False):
@@ -358,15 +357,15 @@
         assert upload_string_1 in out or upload_string_1 in err
         assert upload_string_2 in out or upload_string_2 in err
         assert upload_string_3 in out or upload_string_3 in err
 
         # removing replica -> file on RSE should be overwritten
         # (simulating an upload error, where a part of the file is uploaded but the replica is not registered)
         if 'SUITE' not in environ or environ['SUITE'] != 'client':
-            from rucio.db.sqla import session, models
+            from rucio.db.sqla import models, session
             db_session = session.get_session()
             internal_scope = InternalScope(self.user, **self.vo)
             db_session.query(models.RSEFileAssociation).filter_by(name=tmp_file1_name, scope=internal_scope).delete()
             db_session.query(models.ReplicaLock).filter_by(name=tmp_file1_name, scope=internal_scope).delete()
             db_session.query(models.ReplicationRule).filter_by(name=tmp_file1_name, scope=internal_scope).delete()
             db_session.query(models.DidMeta).filter_by(name=tmp_file1_name, scope=internal_scope).delete()
             db_session.query(models.DataIdentifier).filter_by(name=tmp_file1_name, scope=internal_scope).delete()
@@ -681,19 +680,23 @@
         # add files
         cmd = 'rucio upload --rse {0} --scope {1} {2}'.format(self.def_rse, self.user, tmp_file1)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
 
         # download files
+        download_dir = "/temp"
         replica_pfn = list(self.replica_client.list_replicas([{'scope': self.user, 'name': name}]))[0]['rses'][self.def_rse][0]
-        cmd = 'rucio -v download --rse {0} --pfn {1} {2}:{3}'.format(self.def_rse, replica_pfn, self.user, name)
+        cmd = f'rucio -v download  --dir {download_dir} --rse {self.def_rse} --pfn {replica_pfn} {self.user}:{name}'
         exitcode, out, err = execute(cmd)
-        print(out, err)
-        assert re.search('Total files.*1', out) is not None
+
+        if "Access to local destination denied." in err:  # Known issue - see #6506
+            assert False, "test `test_download_pfn` unable to access file {self.user}/{name} in {download_dir}"
+        else:
+            assert re.search('Total files.*1', out) is not None
 
         try:
             for i in listdir('data13_hip'):
                 unlink('data13_hip/%s' % i)
             rmdir('data13_hip')
         except Exception:
             pass
@@ -1828,17 +1831,17 @@
         self.account_client.set_local_account_limit(account, rse, -1)
         self.account_client.set_global_account_limit(account, rse_exp, -1)
 
     @pytest.mark.noparallel(reason='modifies account limit on pre-defined RSE')
     @pytest.mark.skipif('SUITE' in os.environ and os.environ['SUITE'] == 'client', reason='uses abacus daemon and core functions')
     def test_list_account_usage(self):
         """ CLIENT (USER): list account usage. """
-        from rucio.db.sqla import session, models
         from rucio.core.account_counter import increase
         from rucio.daemons.abacus import account as abacus_account
+        from rucio.db.sqla import models, session
 
         db_session = session.get_session()
         db_session.query(models.AccountUsage).delete()
         db_session.query(models.AccountLimit).delete()
         db_session.query(models.AccountGlobalLimit).delete()
         db_session.query(models.UpdatedAccountCounter).delete()
         db_session.commit()
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_boolean.py` & `rucio-webui-34.1.0/tests/test_boolean.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_clients.py` & `rucio-webui-34.1.0/tests/test_clients.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -10,22 +9,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime, timedelta
-
 from os import rename
 
 import pytest
 
 from rucio.client.baseclient import BaseClient
 from rucio.client.client import Client
-from rucio.common.config import config_get, config_set, Config
+from rucio.common.config import Config, config_get, config_set
 from rucio.common.exception import CannotAuthenticate, ClientProtocolNotSupported, RucioException
 from rucio.common.utils import execute
 from tests.mocks.mock_http_server import MockServer
 
 
 @pytest.fixture
 def client_token_path_override(file_config_mock, function_scope_prefix, tmp_path):
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_common_types.py` & `rucio-webui-34.1.0/tests/test_common_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from rucio.common.types import InternalScope, InternalAccount, InternalType
+from rucio.common.types import InternalAccount, InternalScope, InternalType
 
 
 class TestInternalType:
     """ Test the base InternalType class """
 
     def test_equality(self, vo):
         """ INTERNAL TYPES: Equality """
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_config.py` & `rucio-webui-34.1.0/tests/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_conveyor.py` & `rucio-webui-34.1.0/tests/test_conveyor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -14,48 +13,49 @@
 # limitations under the License.
 import logging
 import threading
 import time
 from datetime import datetime, timedelta
 from tempfile import TemporaryDirectory
 from unittest.mock import patch
-from urllib.parse import urlencode, urlparse, parse_qsl, urlunparse
-from sqlalchemy import update
+from urllib.parse import parse_qsl, urlencode, urlparse, urlunparse
 
 import pytest
+from sqlalchemy import update
 
 import rucio.daemons.reaper.reaper
-from rucio.common.types import InternalAccount
-from rucio.common.utils import generate_uuid, adler32
 from rucio.common.exception import ReplicaNotFound, RequestNotFound
+from rucio.common.types import InternalAccount
+from rucio.common.utils import adler32, generate_uuid
 from rucio.core import config as core_config
 from rucio.core import did as did_core
 from rucio.core import distance as distance_core
 from rucio.core import lock as lock_core
 from rucio.core import message as message_core
 from rucio.core import replica as replica_core
 from rucio.core import request as request_core
 from rucio.core import rse as rse_core
 from rucio.core import rule as rule_core
 from rucio.core.account_limit import set_local_account_limit
 from rucio.daemons.conveyor.finisher import finisher
 from rucio.daemons.conveyor.poller import poller
 from rucio.daemons.conveyor.preparer import preparer
-from rucio.daemons.conveyor.submitter import submitter
+from rucio.daemons.conveyor.receiver import GRACEFUL_STOP as receiver_graceful_stop
+from rucio.daemons.conveyor.receiver import Receiver, receiver
 from rucio.daemons.conveyor.stager import stager
+from rucio.daemons.conveyor.submitter import submitter
 from rucio.daemons.conveyor.throttler import throttler
-from rucio.daemons.conveyor.receiver import receiver, GRACEFUL_STOP as receiver_graceful_stop, Receiver
 from rucio.daemons.reaper.reaper import reaper
 from rucio.db.sqla import models
-from rucio.db.sqla.constants import LockState, RequestState, RequestType, ReplicaState, RSEType, RuleState
+from rucio.db.sqla.constants import LockState, ReplicaState, RequestState, RequestType, RSEType, RuleState
 from rucio.db.sqla.session import read_session, transactional_session
 from rucio.tests.common import skip_rse_tests_with_accounts
 from rucio.transfertool.fts3 import FTS3Transfertool
-from tests.ruciopytest import NoParallelGroups
 from tests.mocks.mock_http_server import MockServer
+from tests.ruciopytest import NoParallelGroups
 
 MAX_POLL_WAIT_SECONDS = 100
 TEST_FTS_HOST = 'https://fts:8446'
 
 
 @transactional_session
 def __update_request(request_id, *, session=None, **kwargs):
@@ -125,17 +125,18 @@
         .filter(models.Source.rse_id == src_rse_id) \
         .first()
 
 
 @pytest.fixture
 def scitags_mock(core_config_mock):
     """Run a mock http server which always returns the content of scitags.json from test/inputs"""
-    from tests.inputs import SCITAGS_JSON
     from pathlib import Path
 
+    from tests.inputs import SCITAGS_JSON
+
     class _SendScitagsJson(MockServer.Handler):
         def do_GET(self):
             file_content = Path(SCITAGS_JSON).read_text()
             self.send_code_and_message(200, {'Content-Type': 'application/json'}, file_content)
 
     with MockServer(_SendScitagsJson) as mock_server:
         core_config.set('packet-marking', 'enabled', True)
@@ -171,23 +172,23 @@
     dst_rse_name = 'XRD4'
     dst_rse_id = rse_core.get_rse_id(rse=dst_rse_name, vo=vo)
 
     all_rses = [src_rse1_id, src_rse2_id, jump_rse_id, dst_rse_id]
     did = did_factory.upload_test_file(src_rse1_name)
 
     # Copy replica to a second source. To avoid the special case of having a unique last replica, which could be handled in a special (more careful) way
-    rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=src_rse2_name, grouping='ALL', weight=None, lifetime=3600, locked=False, subscription_id=None)
+    rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=src_rse2_name, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
     submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], partition_wait_time=0, transfertype='single', filter_transfertool=None)
     replica = __wait_for_replica_transfer(dst_rse_id=src_rse2_id, **did)
     assert replica['state'] == ReplicaState.AVAILABLE
 
     rse_core.set_rse_limits(rse_id=jump_rse_id, name='MinFreeSpace', value=1)
     rse_core.set_rse_usage(rse_id=jump_rse_id, source='storage', used=1, free=0)
     try:
-        rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse_name, grouping='ALL', weight=None, lifetime=3600, locked=False, subscription_id=None)
+        rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse_name, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
 
         # Submit transfers to FTS
         # Ensure a replica was created on the intermediary host with epoch tombstone
         submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], partition_wait_time=0, transfertype='single', filter_transfertool=None)
         request = request_core.get_request_by_did(rse_id=jump_rse_id, **did)
         assert request['state'] == RequestState.SUBMITTED
         replica = replica_core.get_replica(rse_id=jump_rse_id, **did)
@@ -570,15 +571,15 @@
         dst_rse = 'XRD4'
         dst_rse_id = rse_core.get_rse_id(rse=dst_rse, vo=vo)
 
         all_rses = [src_rse_id, jump_rse_id, dst_rse_id]
 
         did = did_factory.upload_test_file(src_rse)
         rule_priority = 5
-        rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=3600, locked=False, subscription_id=None, priority=rule_priority)
+        rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None, priority=rule_priority)
         submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=2, partition_wait_time=0, transfertype='single', filter_transfertool=None)
 
         request = __wait_for_state_transition(dst_rse_id=jump_rse_id, run_poller=False, **did)
         assert request['state'] == RequestState.DONE
         request = __wait_for_state_transition(dst_rse_id=dst_rse_id, run_poller=False, **did)
         assert request['state'] == RequestState.DONE
 
@@ -682,16 +683,16 @@
     distance_core.add_distance(src_rse_id, dst_rse_id1, distance=10)
     distance_core.add_distance(src_rse_id, dst_rse_id2, distance=10)
     # Set limits only for one of the RSEs
     request_core.set_transfer_limit(dst_rse1, max_transfers=1, activity='all_activities', strategy='fifo')
 
     did1 = did_factory.upload_test_file(src_rse)
     did2 = did_factory.upload_test_file(src_rse)
-    rule_core.add_rule(dids=[did1], account=root_account, copies=1, rse_expression=dst_rse1, grouping='ALL', weight=None, lifetime=3600, locked=False, subscription_id=None)
-    rule_core.add_rule(dids=[did2], account=root_account, copies=1, rse_expression=dst_rse1, grouping='ALL', weight=None, lifetime=3600, locked=False, subscription_id=None)
+    rule_core.add_rule(dids=[did1], account=root_account, copies=1, rse_expression=dst_rse1, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
+    rule_core.add_rule(dids=[did2], account=root_account, copies=1, rse_expression=dst_rse1, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
     rule_core.add_rule(dids=[did1], account=root_account, copies=1, rse_expression=dst_rse2, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
 
     request = request_core.get_request_by_did(rse_id=dst_rse_id1, **did1)
     assert request['state'] == RequestState.PREPARING
     request = request_core.get_request_by_did(rse_id=dst_rse_id1, **did2)
     assert request['state'] == RequestState.PREPARING
     request = request_core.get_request_by_did(rse_id=dst_rse_id2, **did1)
@@ -752,17 +753,17 @@
     assert request['state'] == RequestState.QUEUED
 
     # Check that resetting stale waiting requests works properly
     request_core.set_transfer_limit(dst_rse2, max_transfers=1, activity='all_activities', strategy='fifo')
     did3 = did_factory.upload_test_file(src_rse)
     did4 = did_factory.upload_test_file(src_rse)
     rule_core.add_rule(dids=[did3], account=root_account, copies=1, rse_expression=dst_rse2, grouping='ALL',
-                       weight=None, lifetime=3600, locked=False, subscription_id=None)
+                       weight=None, lifetime=None, locked=False, subscription_id=None)
     rule_core.add_rule(dids=[did4], account=root_account, copies=1, rse_expression=dst_rse2, grouping='ALL',
-                       weight=None, lifetime=3600, locked=False, subscription_id=None)
+                       weight=None, lifetime=None, locked=False, subscription_id=None)
     request3 = request_core.get_request_by_did(rse_id=dst_rse_id2, **did3)
     request4 = request_core.get_request_by_did(rse_id=dst_rse_id2, **did4)
     assert request3['state'] == RequestState.PREPARING
     assert request4['state'] == RequestState.PREPARING
 
     # Run the preparer so requests are in waiting state
     preparer(once=True, sleep_time=1, bulk=100, partition_wait_time=0, ignore_availability=False)
@@ -886,15 +887,15 @@
 
     distance_core.add_distance(src_rse_id, dst_rse_id, distance=10)
     rse_core.add_rse_attribute(dst_rse_id, 'staging_required', True)
     rse_core.add_rse_attribute(dst_rse_id, 'maximum_pin_lifetime', maximum_pin_lifetime)
 
     did = did_factory.upload_test_file(rse_name=src_rse)
 
-    rule1_id = rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=-1, locked=False, subscription_id=None)[0]
+    rule1_id = rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)[0]
     request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
 
     assert request['request_type'] == RequestType.TRANSFER
 
     submitter(once=True, rses=[{'id': dst_rse_id}], partition_wait_time=0, transfertools=['mock'], transfertype='single', filter_transfertool=None)
 
     assert lock_core.get_replica_locks_for_rule_id(rule_id=rule1_id)[0]['state'] == LockState.REPLICATING
@@ -907,15 +908,15 @@
 
     # assert all replicas available
     for rse_id in all_rses:
         assert replica_core.get_replica(rse_id=rse_id, **did)['state'] == ReplicaState.AVAILABLE
 
     # now test a second rule, different account
     set_local_account_limit(jdoe_account, dst_rse_id, bytes_=-1)
-    rule2_id = rule_core.add_rule(dids=[did], account=jdoe_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=-1, locked=False, subscription_id=None, source_replica_expression=dst_rse)[0]
+    rule2_id = rule_core.add_rule(dids=[did], account=jdoe_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None, source_replica_expression=dst_rse)[0]
     request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
 
     assert request['request_type'] == RequestType.STAGEIN
 
     stager(once=True, rses=[{'id': dst_rse_id}])
 
     assert request['attributes']['lifetime'] == str(maximum_pin_lifetime)
@@ -947,15 +948,15 @@
 
     distance_core.add_distance(src_rse_id, dst_rse_id, distance=10)
     rse_core.add_rse_attribute(dst_rse_id, 'staging_required', True)
     rse_core.add_rse_attribute(dst_rse_id, 'maximum_pin_lifetime', maximum_pin_lifetime)
 
     did = did_factory.upload_test_file(rse_name=src_rse)
 
-    rule1_id = rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=-1, locked=False, subscription_id=None)[0]
+    rule1_id = rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)[0]
     request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
 
     assert request['request_type'] == RequestType.TRANSFER
 
     submitter(once=True, rses=[{'id': dst_rse_id}], partition_wait_time=0, transfertools=['mock'], transfertype='single', filter_transfertool=None)
 
     assert lock_core.get_replica_locks_for_rule_id(rule_id=rule1_id)[0]['state'] == LockState.REPLICATING
@@ -968,15 +969,15 @@
     lock_core.failed_transfer(scope=did['scope'], name=did['name'], rse_id=dst_rse_id)
 
     assert rule_core.get_rule(rule1_id)['state'] == RuleState.STUCK
     assert lock_core.get_replica_locks_for_rule_id(rule_id=rule1_id)[0]['state'] == LockState.STUCK
 
     # now test a second rule, different account
     set_local_account_limit(jdoe_account, dst_rse_id, bytes_=-1)
-    rule2_id = rule_core.add_rule(dids=[did], account=jdoe_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=-1, locked=False, subscription_id=None, source_replica_expression=dst_rse)[0]
+    rule2_id = rule_core.add_rule(dids=[did], account=jdoe_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None, source_replica_expression=dst_rse)[0]
     request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
 
     # since the first rule is STUCK assert a transfer not stagein
     assert request['request_type'] == RequestType.TRANSFER
 
     submitter(once=True, rses=[{'id': dst_rse_id}], partition_wait_time=0, transfertools=['mock'], transfertype='single', filter_transfertool=None)
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_conveyor_submitter.py` & `rucio-webui-34.1.0/tests/test_conveyor_submitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pytest
-
 import itertools
 from datetime import datetime, timedelta
 from random import randint
 from unittest.mock import patch
+
+import pytest
 from sqlalchemy import delete
 
 from rucio.common.exception import RequestNotFound
+from rucio.core import config as core_config
 from rucio.core import distance as distance_core
+from rucio.core import replica as replica_core
 from rucio.core import request as request_core
 from rucio.core import rse as rse_core
-from rucio.core import replica as replica_core
 from rucio.core import rule as rule_core
-from rucio.core import config as core_config
 from rucio.daemons.conveyor.submitter import submitter
 from rucio.daemons.reaper.reaper import reaper
-from rucio.db.sqla.models import Request, Source
 from rucio.db.sqla.constants import RequestState
+from rucio.db.sqla.models import Request, Source
 from rucio.db.sqla.session import read_session, transactional_session
 from tests.ruciopytest import NoParallelGroups
 
 
 @pytest.mark.noparallel(groups=[NoParallelGroups.SUBMITTER])
 def test_request_submitted_in_order(rse_factory, did_factory, root_account):
 
@@ -91,14 +90,35 @@
         assert request_core.get_request(request_id=request['id'])['state'] == RequestState.SUBMITTED
 
     # Requests must be submitted in the order of their creation
     assert requests_id_in_submission_order == [r['id'] for r in requests]
 
 
 @pytest.mark.noparallel(groups=[NoParallelGroups.SUBMITTER])
+def test_skip_requests_from_expired_rules(rse_factory, did_factory, root_account):
+    src_rse_name, src_rse_id = rse_factory.make_posix_rse()
+    dst_rse_name, dst_rse_id = rse_factory.make_posix_rse()
+    distance_core.add_distance(src_rse_id, dst_rse_id, distance=10)
+
+    did = did_factory.upload_test_file(rse_name=src_rse_name)
+    rule = rule_core.add_rule(dids=[did], account=root_account, copies=1,
+                              rse_expression=dst_rse_name, grouping='ALL',
+                              weight=None, lifetime=-1, locked=False,
+                              subscription_id=None)[0]
+    request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
+    assert request_core.get_request(request_id=request['id'])['state'] == RequestState.QUEUED
+
+    submitter(once=True,
+              rses=[{'id': rse_id} for rse_id in (src_rse_id, dst_rse_id)],
+              partition_wait_time=None, transfertools=['mock'],
+              transfertype='single', filter_transfertool=None)
+    assert request_core.get_request(request_id=request['id'])['state'] == RequestState.QUEUED
+
+
+@pytest.mark.noparallel(groups=[NoParallelGroups.SUBMITTER])
 @pytest.mark.parametrize("core_config_mock", [
     # Run test twice: with, and without, temp tables
     {
         "table_content": [
             ('transfers', 'multihop_rse_expression', '*'),
         ]
     }
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_counter.py` & `rucio-webui-34.1.0/tests/test_counter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_credential.py` & `rucio-webui-34.1.0/tests/test_credential.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_curl.py` & `rucio-webui-34.1.0/tests/test_curl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +14,15 @@
 
 import json
 import os
 
 import pytest
 
 from rucio.common.config import config_get, config_get_bool
-from rucio.tests.common import account_name_generator, rse_name_generator, execute, get_long_vo
+from rucio.tests.common import account_name_generator, execute, get_long_vo, rse_name_generator
 
 
 class TestCurlRucio:
     '''
     class TestCurlRucio
     '''
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_daemons.py` & `rucio-webui-34.1.0/tests/test_daemons.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -21,15 +20,15 @@
 from rucio.common import exception
 from rucio.daemons.abacus import account, collection_replica, rse
 from rucio.daemons.atropos import atropos
 from rucio.daemons.automatix import automatix
 from rucio.daemons.badreplicas import minos, minos_temporary_expiration, necromancer
 from rucio.daemons.c3po import c3po
 from rucio.daemons.cache import consumer
-from rucio.daemons.conveyor import finisher, poller, receiver, stager, submitter, throttler, preparer
+from rucio.daemons.conveyor import finisher, poller, preparer, receiver, stager, submitter, throttler
 from rucio.daemons.follower import follower
 from rucio.daemons.hermes import hermes
 from rucio.daemons.judge import cleaner, evaluator, injector, repairer
 from rucio.daemons.oauthmanager import oauthmanager
 from rucio.daemons.reaper import dark_reaper, reaper
 from rucio.daemons.replicarecoverer import suspicious_replica_recoverer
 from rucio.daemons.tracer import kronos
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_dataset_replicas.py` & `rucio-webui-34.1.0/tests/test_dataset_replicas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -17,21 +16,20 @@
 from sqlalchemy.orm.exc import NoResultFound
 
 from rucio.client.didclient import DIDClient
 from rucio.client.replicaclient import ReplicaClient
 from rucio.client.ruleclient import RuleClient
 from rucio.common.exception import InvalidObject
 from rucio.common.schema import get_schema_value
-from rucio.core.did import attach_dids, add_dids
-from rucio.core.replica import list_datasets_per_rse, update_collection_replica, \
-    get_cleaned_updated_collection_replicas, delete_replicas, add_replicas
-from rucio.core.rse import add_rse, del_rse, add_protocol, get_rse_id
-from rucio.db.sqla import models, constants
+from rucio.core.did import add_dids, attach_dids
+from rucio.core.replica import add_replicas, delete_replicas, get_cleaned_updated_collection_replicas, list_datasets_per_rse, update_collection_replica
+from rucio.core.rse import add_protocol, add_rse, del_rse, get_rse_id
+from rucio.db.sqla import constants, models
 from rucio.db.sqla.constants import ReplicaState
-from rucio.tests.common import rse_name_generator, did_name_generator
+from rucio.tests.common import did_name_generator, rse_name_generator
 
 
 class TestDatasetReplicaClient:
 
     @pytest.mark.noparallel(reason='uses pre-defined RSE')
     def test_list_dataset_replicas(self):
         """ REPLICA (CLIENT): List dataset replicas."""
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_db.py` & `rucio-webui-34.1.0/tests/test_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pytest
 from unittest.mock import patch
 
+import pytest
 from sqlalchemy import text
-from rucio.db.sqla.session import get_session, _get_engine_poolclass, NullPool, QueuePool, SingletonThreadPool
+
 from rucio.common.exception import InputValidationError
+from rucio.db.sqla.session import NullPool, QueuePool, SingletonThreadPool, _get_engine_poolclass, get_session
 
 
 def test_db_connection():
     """ DB (CORE): Test db connection """
     session = get_session()
     if session.bind.dialect.name == 'oracle':
         session.execute(text('select 1 from dual'))
@@ -39,16 +39,16 @@
     with pytest.raises(InputValidationError, match='Unknown poolclass: unknown'):
         _get_engine_poolclass('unknown')
 
 
 @pytest.mark.noparallel(reason='Changes an internal method of MethodView.')
 def test_pooloverload():
     """ DB (WEB): Test response to a DatabaseException due to Pool Overflow """
-    from rucio.web.rest.flaskapi.v1.ping import Ping
     from rucio.common.exception import DatabaseException
+    from rucio.web.rest.flaskapi.v1.ping import Ping
 
     # Create a new ErrorHandlingMethodView as_view
     ping_view = Ping.as_view('ping')
 
     # specification for the mock we create to replace flask.request
     # without specifying this, _is_async_obj is run which triggers flask RuntimeError
     class T:
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_did.py` & `rucio-webui-34.1.0/tests/test_did.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -13,30 +12,43 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime, timedelta
 
 import pytest
 
-from rucio.api import did
-from rucio.api import scope
-from rucio.db.sqla.util import json_implemented
+from rucio.api import did, scope
 from rucio.common import exception
-from rucio.common.exception import (DataIdentifierNotFound, DataIdentifierAlreadyExists,
-                                    InvalidPath, UnsupportedOperation,
-                                    UnsupportedStatus, ScopeNotFound, FileAlreadyExists, FileConsistencyMismatch)
+from rucio.common.exception import DataIdentifierAlreadyExists, DataIdentifierNotFound, FileAlreadyExists, FileConsistencyMismatch, InvalidPath, ScopeNotFound, UnsupportedOperation, UnsupportedStatus
 from rucio.common.types import InternalScope
 from rucio.common.utils import generate_uuid
-from rucio.core.did import (list_dids, add_did, delete_dids, get_did_atime, touch_dids, attach_dids, detach_dids,
-                            get_metadata, set_metadata, get_did, get_did_access_cnt, add_did_to_followed,
-                            get_users_following_did, remove_did_from_followed, set_status, list_new_dids,
-                            set_new_dids)
+from rucio.core.did import (
+    add_did,
+    add_did_to_followed,
+    attach_dids,
+    bulk_list_files,
+    delete_dids,
+    detach_dids,
+    get_did,
+    get_did_access_cnt,
+    get_did_atime,
+    get_metadata,
+    get_users_following_did,
+    list_dids,
+    list_new_dids,
+    remove_did_from_followed,
+    set_metadata,
+    set_new_dids,
+    set_status,
+    touch_dids,
+)
 from rucio.core.replica import add_replica, get_replica
 from rucio.db.sqla.constants import DIDType
-from rucio.tests.common import rse_name_generator, scope_name_generator, did_name_generator
+from rucio.db.sqla.util import json_implemented
+from rucio.tests.common import did_name_generator, rse_name_generator, scope_name_generator
 
 
 def skip_without_json():
     if not json_implemented():
         pytest.skip("JSON support is not implemented in this database")
 
 
@@ -249,14 +261,43 @@
         new_dids = [did for did in list_new_dids(did_type=None, thread=None, total_threads=None, chunk_size=100000, session=None)]
         assert {'scope': mock_scope, 'name': dsn, 'did_type': DIDType.DATASET} not in new_dids
 
         set_status(mock_scope, dsn, open=False)
         new_dids = [did for did in list_new_dids(did_type=None, thread=None, total_threads=None, chunk_size=100000, session=None)]
         assert {'scope': mock_scope, 'name': dsn, 'did_type': DIDType.DATASET} in new_dids
 
+    def test_bulk_list_files(self, mock_scope, root_account, rse_factory, did_factory):
+        """ Test the bulk_list_files method"""
+        _, rse_id = rse_factory.make_mock_rse()
+        nb_datasets = 5
+        nb_files = 10
+        # Try listing existing datasets
+        datasets = [did_factory.make_dataset() for _ in range(nb_datasets)]
+        files = []
+        for dataset in datasets:
+            new_files = []
+            for _ in range(nb_files):
+                new_files.append({'scope': mock_scope, 'name': did_name_generator('file'), 'bytes': 1, 'adler32': '0cc737eb', 'events': None, 'guid': None})
+            attach_dids(scope=dataset['scope'], name=dataset['name'], rse_id=rse_id, dids=new_files, account=root_account)
+            for file_ in new_files:
+                file_['parent_scope'] = dataset['scope']
+                file_['parent_name'] = dataset['name']
+            files.extend(new_files)
+        result = [file_ for file_ in bulk_list_files(datasets)]
+        assert len(result) == len(files)
+        for file_ in files:
+            assert file_ in result
+        # Try listing non-existing datasets
+        non_existing_datasets = [{'scope': mock_scope, 'name': did_name_generator('dataset')} for _ in range(nb_datasets)]
+        datasets.extend(non_existing_datasets)
+        parent_datasets = [(dataset['parent_scope'], dataset['parent_name']) for dataset in result]
+        assert len(result) == len(files)
+        for dataset in non_existing_datasets:
+            assert (dataset['scope'], dataset['name']) not in parent_datasets
+
 
 class TestDIDApi:
 
     @pytest.mark.dirty
     def test_list_new_dids(self, vo):
         """ DATA IDENTIFIERS (API): List new identifiers """
         tmp_scope = scope_name_generator()
@@ -1099,14 +1140,44 @@
         assert len(list_meta) == 12
         list_dids = []
         for idx in range(4):
             list_dids.append({'scope': scope, 'name': cnt[idx]})
         list_meta = [_ for _ in did_client.get_metadata_bulk(list_dids)]
         assert len(list_meta) == 0
 
+    def test_bulk_list_files(self, did_client, mock_scope, root_account, rse_factory, did_factory):
+        """ Test the bulk_list_files method"""
+        _, rse_id = rse_factory.make_mock_rse()
+        nb_datasets = 5
+        # Try listing existing datasets
+        datasets = [did_factory.make_dataset() for _ in range(nb_datasets)]
+        external_datasets = [{'scope': dataset['scope'].external, 'name': dataset['name']} for dataset in datasets]
+        files = []
+        for dataset in datasets:
+            new_files = []
+            for _ in range(10):
+                new_files.append({'scope': mock_scope, 'name': did_name_generator('file'), 'bytes': 1, 'adler32': '0cc737eb', 'events': None, 'guid': None})
+            attach_dids(scope=dataset['scope'], name=dataset['name'], rse_id=rse_id, dids=new_files, account=root_account)
+            for file_ in new_files:
+                file_['scope'] = dataset['scope'].external
+                file_['parent_scope'] = dataset['scope'].external
+                file_['parent_name'] = dataset['name']
+            files.extend(new_files)
+        result = [files for files in did_client.bulk_list_files(external_datasets)]
+        assert len(result) == len(files)
+        for file_ in files:
+            assert file_ in result
+        # Try listing non-existing datasets
+        non_existing_datasets = [{'scope': mock_scope.external, 'name': did_name_generator('dataset')} for _ in range(nb_datasets)]
+        datasets.extend(non_existing_datasets)
+        parent_datasets = [(dataset['parent_scope'], dataset['parent_name']) for dataset in result]
+        assert len(result) == len(files)
+        for dataset in non_existing_datasets:
+            assert (dataset['scope'], dataset['name']) not in parent_datasets
+
 
 @pytest.mark.noparallel(reason='uses mock scope')
 def test_bulk_get_meta_inheritance(vo, rse_factory, mock_scope, did_factory, rucio_client):
     """ DATA IDENTIFIERS (CLIENT): Add metadata for a hierarchical list of DIDs and check that the metadata are inherited"""
     skip_without_json()
     key = 'generic_metadata'
     nb_dids = 4
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_did_meta_plugins.py` & `rucio-webui-34.1.0/tests/test_did_meta_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -16,20 +15,20 @@
 from copy import deepcopy
 
 import pytest
 
 from rucio.client.didclient import DIDClient
 from rucio.common.exception import KeyNotFound
 from rucio.common.utils import generate_uuid
-from rucio.core.did import add_did, delete_dids, set_metadata_bulk, set_dids_metadata_bulk
-from rucio.core.did_meta_plugins import list_dids, get_metadata, set_metadata
+from rucio.core.did import add_did, delete_dids, set_dids_metadata_bulk, set_metadata_bulk
+from rucio.core.did_meta_plugins import get_metadata, list_dids, set_metadata
 from rucio.core.did_meta_plugins.mongo_meta import MongoDidMeta
 from rucio.core.did_meta_plugins.postgres_meta import ExternalPostgresJSONDidMeta
 from rucio.db.sqla.util import json_implemented
-from rucio.tests.common import skip_rse_tests_with_accounts, did_name_generator
+from rucio.tests.common import did_name_generator, skip_rse_tests_with_accounts
 
 
 def skip_without_json():
     if not json_implemented():
         pytest.skip("JSON support is not implemented in this database")
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_didtype.py` & `rucio-webui-34.1.0/tests/test_didtype.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_download.py` & `rucio-webui-34.1.0/tests/test_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -19,26 +18,25 @@
 import tarfile
 from tempfile import TemporaryDirectory
 from unittest.mock import ANY, MagicMock, patch
 from zipfile import ZipFile
 
 import pytest
 
-from rucio.client.downloadclient import DownloadClient
+from rucio.client.downloadclient import DownloadClient, FileDownloadState
 from rucio.common.config import config_add_section, config_set
 from rucio.common.exception import InputValidationError, NoFilesDownloaded, RucioException
 from rucio.common.types import InternalScope
 from rucio.common.utils import generate_uuid
 from rucio.core import did as did_core
 from rucio.core import scope as scope_core
 from rucio.core.rse import add_protocol
-from rucio.client.downloadclient import FileDownloadState
 from rucio.rse import rsemanager as rsemgr
 from rucio.rse.protocols.posix import Default as PosixProtocol
-from rucio.tests.common import skip_rse_tests_with_accounts, scope_name_generator, file_generator
+from rucio.tests.common import file_generator, scope_name_generator, skip_rse_tests_with_accounts
 
 
 @pytest.fixture
 def download_client():
     logger = logging.getLogger('dlul_client')
     logger.addHandler(logging.StreamHandler())
     logger.setLevel(logging.DEBUG)
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_dumper.py` & `rucio-webui-34.1.0/tests/test_dumper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -20,18 +19,17 @@
 from datetime import datetime
 from io import StringIO
 from unittest import mock
 
 import pytest
 import requests
 
-from rucio.common import config
-from rucio.common import dumper
-from rucio.tests.common import make_temp_file
-from rucio.tests.common import mock_open
+from rucio.common import config, dumper
+from rucio.tests.common import make_temp_file, mock_open
+
 from .mocks import gfal2
 
 DATE_SECONDS = "2015-03-10 14:00:35"
 DATE_TENTHS = "2015-03-10T14:00:35.5"
 DATE_MILLISECONDS = "2015-03-10T14:00:35.5"
 RSEPROTOCOL = {
     "hostname": "example.com",
@@ -82,15 +80,15 @@
     os.unlink(tmp)
 
 
 def test_smart_open_for_bz2_file():
     fd, path = tempfile.mkstemp()
     comp = bz2.BZ2Compressor()
     with os.fdopen(fd, 'wb') as f:
-        f.write(comp.compress('abcdef'.encode()))
+        f.write(comp.compress(b'abcdef'))
         f.write(comp.flush())
     assert not isinstance(dumper.smart_open(path), bz2.BZ2File)
     os.unlink(path)
 
 
 def test_temp_file_with_final_name_creates_a_tmp_file_and_then_removes_it():
     final_name = tempfile.mktemp()
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_dumper_consistency.py` & `rucio-webui-34.1.0/tests/test_dumper_consistency.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -14,20 +13,15 @@
 # limitations under the License.
 
 import json
 import os
 from datetime import datetime
 from unittest import mock
 
-from rucio.common.dumper.consistency import Consistency
-from rucio.common.dumper.consistency import _try_to_advance
-from rucio.common.dumper.consistency import compare3
-from rucio.common.dumper.consistency import gnu_sort
-from rucio.common.dumper.consistency import min3
-from rucio.common.dumper.consistency import parse_and_filter_file
+from rucio.common.dumper.consistency import Consistency, _try_to_advance, compare3, gnu_sort, min3, parse_and_filter_file
 from rucio.tests.common import make_temp_file
 
 RSEPROTOCOL = {
     "hostname": "example.com",
     "scheme": "root",
     "port": 1094,
     "prefix": "//atlasdatadisk/rucio/",
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_dumper_data_model.py` & `rucio-webui-34.1.0/tests/test_dumper_data_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -212,15 +211,15 @@
             self._DataConcrete.download(
                 'SOMEENDPOINT',
                 date=datetime.strptime('01-01-2015', '%d-%m-%Y'),
                 cache_dir=tmp_path,
             )
 
 
-class TestCompleteDataset(object):
+class TestCompleteDataset:
 
     @staticmethod
     def test_creation_with_7_parameters():
         """ test ceation with 7 parameters """
         complete_dataset = data_models.CompleteDataset(
             'RSE',
             'scope',
@@ -259,15 +258,15 @@
             '2015-01-01 23:00:00',
             '2015-01-01 23:00:00',
             'A',
         )
         assert complete_dataset.size is None  # pylint: disable=no-member
 
 
-class TestReplica(object):
+class TestReplica:
 
     @staticmethod
     def test_replica_with_8_parameters():
         """ test replica with 8 parameters """
         replica = data_models.Replica(
             'RSE',
             'scope',
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_dumper_path_parsing.py` & `rucio-webui-34.1.0/tests/test_dumper_path_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from rucio.common.dumper.path_parsing import components
-from rucio.common.dumper.path_parsing import remove_prefix
+from rucio.common.dumper.path_parsing import components, remove_prefix
 
 
-class TestPathParsing(object):
+class TestPathParsing:
     def test_remove_prefix(self):
         prefix = ['a', 'b', 'c', 'd']
 
         full = ['a', 'b', 'c', 'd', 'e', 'f']  # -> e,f
         relative = ['c', 'd', 'e', 'f']  # -> e,f
         exclusive = ['e', 'f', 'g']  # -> e,f,g
         mixed = ['c', 'a', 'e', 'f']  # -> c,a,e,f
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_filter_engine.py` & `rucio-webui-34.1.0/tests/test_filter_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -10,26 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import operator
-from datetime import datetime, timedelta
 import unittest
+from datetime import datetime, timedelta
 
 import pytest
 
 from rucio.common.exception import DuplicateCriteriaInDIDFilter
 from rucio.common.utils import generate_uuid
 from rucio.core.did import add_did
 from rucio.core.did_meta_plugins import set_metadata
+from rucio.core.did_meta_plugins.filter_engine import FilterEngine
 from rucio.db.sqla import models
 from rucio.db.sqla.util import json_implemented
-from rucio.core.did_meta_plugins.filter_engine import FilterEngine
 
 
 class TestFilterEngineDummy:
     def test_InputSanitisation(self):
         filters = FilterEngine('  TestKeyword1  =  True  ,  TestKeyword2   =   0; 1 < TestKeyword4 <= 2', strict_coerce=False).filters
         filters_expected = [[('TestKeyword1', operator.eq, 1),
                              ('TestKeyword2', operator.eq, 0)],
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_heartbeat.py` & `rucio-webui-34.1.0/tests/test_heartbeat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +14,15 @@
 
 import random
 import threading
 from datetime import datetime, timedelta
 
 import pytest
 
-from rucio.core.heartbeat import live, die, cardiac_arrest, list_payload_counts, list_heartbeats, sanity_check
+from rucio.core.heartbeat import cardiac_arrest, die, list_heartbeats, list_payload_counts, live, sanity_check
 from rucio.db.sqla.models import Heartbeats
 from rucio.db.sqla.session import transactional_session
 
 
 @pytest.fixture
 def executable_factory(function_scope_prefix, db_session):
     executables = []
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_hermes.py` & `rucio-webui-34.1.0/tests/test_hermes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -13,29 +12,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Hermes Test
 """
 
+import time
 from datetime import datetime
 from json import loads
-import requests
-import pytest
 
+import pytest
+import requests
 import stomp
-import time
 
 from rucio.common.config import config_get, config_get_int
 from rucio.core.message import add_message, retrieve_messages, truncate_messages
 from rucio.daemons.hermes import hermes
 from rucio.tests.common import rse_name_generator, skip_missing_elasticsearch_influxdb_in_env
 
 
-class MyListener(object):
+class MyListener:
     def __init__(self, conn):
         self.conn = conn
         self.count = 0
         self.messages = []
 
     def reset(self):
         self.count = 0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_identity.py` & `rucio-webui-34.1.0/tests/test_identity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,22 +14,22 @@
 
 import random
 import string
 
 import pytest
 
 from rucio.common.config import config_get_bool
+from rucio.common.exception import IdentityError, IdentityNotFound
 from rucio.common.types import InternalAccount
 from rucio.common.utils import generate_uuid as uuid
 from rucio.core.account import add_account, del_account
-from rucio.core.identity import add_identity, del_identity, add_account_identity, del_account_identity, list_identities, verify_identity
+from rucio.core.identity import add_account_identity, add_identity, del_account_identity, del_identity, list_identities, verify_identity
 from rucio.db.sqla.constants import AccountType, IdentityType
-from rucio.tests.common import account_name_generator, headers, hdrdict, auth, rfc2253_dn_generator
+from rucio.tests.common import account_name_generator, auth, hdrdict, headers, rfc2253_dn_generator
 from rucio.tests.common_server import get_vo
-from rucio.common.exception import IdentityNotFound, IdentityError
 
 
 @pytest.mark.noparallel(reason='adds/removes entities with non-unique names')
 class TestIdentity:
     """
     Test the Identity abstraction layer
     """
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_impl_upload_download.py` & `rucio-webui-34.1.0/tests/test_impl_upload_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from os import path
 import re
+from os import path
 
 import pytest
 
-from rucio.common.utils import generate_uuid as uuid, execute
+from rucio.common.utils import execute
+from rucio.common.utils import generate_uuid as uuid
 from rucio.tests.common import skip_rse_tests_with_accounts
 
 
 @pytest.fixture(scope='class')
 def scope_and_rse(mock_scope, test_scope):
     """
     Check if xrd containers rses for xrootd are available in the testing environment.
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_import_export.py` & `rucio-webui-34.1.0/tests/test_import_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,29 +14,27 @@
 
 from copy import deepcopy
 
 import pytest
 
 from rucio.client.exportclient import ExportClient
 from rucio.client.importclient import ImportClient
-from rucio.common.config import config_set, config_add_section, config_has_section
+from rucio.common.config import config_add_section, config_has_section, config_set
 from rucio.common.exception import RSENotFound
 from rucio.common.types import InternalAccount
-from rucio.common.utils import render_json, parse_response
+from rucio.common.utils import parse_response, render_json
 from rucio.core.account import add_account, get_account
 from rucio.core.distance import add_distance, get_distances
 from rucio.core.exporter import export_data, export_rses
-from rucio.core.identity import add_identity, list_identities, add_account_identity, list_accounts_for_identity
+from rucio.core.identity import add_account_identity, add_identity, list_accounts_for_identity, list_identities
 from rucio.core.importer import import_data, import_rses
-from rucio.core.rse import get_rse_id, get_rse_name, add_rse, get_rse, add_protocol, get_rse_protocols, \
-    list_rse_attributes, get_rse_limits, set_rse_limits, add_rse_attribute, list_rses, export_rse, del_rse, \
-    get_rse_attribute
-from rucio.db.sqla import session, models
-from rucio.db.sqla.constants import RSEType, AccountType, IdentityType, AccountStatus
-from rucio.tests.common import rse_name_generator, headers, auth, hdrdict
+from rucio.core.rse import add_protocol, add_rse, add_rse_attribute, del_rse, export_rse, get_rse, get_rse_attribute, get_rse_id, get_rse_limits, get_rse_name, get_rse_protocols, list_rse_attributes, list_rses, set_rse_limits
+from rucio.db.sqla import models, session
+from rucio.db.sqla.constants import AccountStatus, AccountType, IdentityType, RSEType
+from rucio.tests.common import auth, hdrdict, headers, rse_name_generator
 
 
 def check_rse(rse_name, test_data, vo='def'):
     rse_id = get_rse_id(rse=rse_name, vo=vo)
     rse = get_rse(rse_id=rse_id)
     assert rse['rse'] == rse_name
     assert rse['vo'] == vo
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_judge_cleaner.py` & `rucio-webui-34.1.0/tests/test_judge_cleaner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -22,14 +21,15 @@
 from rucio.core.did import add_did, attach_dids
 from rucio.core.lock import get_replica_locks
 from rucio.core.rse import add_rse_attribute
 from rucio.core.rule import add_rule, update_rule
 from rucio.daemons.judge.cleaner import rule_cleaner
 from rucio.db.sqla.constants import DIDType
 from rucio.tests.common_server import get_vo
+
 from .test_rule import create_files, tag_generator
 
 
 @pytest.fixture(scope="class")
 def setup_class(request, rse_factory_unittest):
     request.cls.setUpClass()
 
@@ -82,15 +82,15 @@
         """ JUDGE CLEANER: Test the judge when deleting expired rules"""
         scope = InternalScope('mock', **self.vo)
         files = create_files(3, scope, self.rse1_id)
         dataset = 'dataset_' + str(uuid())
         add_did(scope, dataset, DIDType.DATASET, self.jdoe)
         attach_dids(scope, dataset, files, self.jdoe)
 
-        add_rule(dids=[{'scope': scope, 'name': dataset}], account=self.jdoe, copies=1, rse_expression=self.rse1, grouping='NONE', weight='fakeweight', lifetime=-3, locked=False, subscription_id=None)[0]
+        add_rule(dids=[{'scope': scope, 'name': dataset}], account=self.jdoe, copies=1, rse_expression=self.rse1, grouping='NONE', weight='fakeweight', lifetime=-1, locked=False, subscription_id=None)[0]
         add_rule(dids=[{'scope': scope, 'name': dataset}], account=self.jdoe, copies=2, rse_expression=self.T1, grouping='NONE', weight='fakeweight', lifetime=None, locked=False, subscription_id=None)[0]
         add_rule(dids=[{'scope': scope, 'name': dataset}], account=self.jdoe, copies=3, rse_expression=self.T1, grouping='NONE', weight='fakeweight', lifetime=None, locked=False, subscription_id=None)[0]
 
         rule_cleaner(once=True)
 
         for file in files:
             rse_locks = get_replica_locks(scope=file['scope'], name=file['name'])
@@ -101,11 +101,11 @@
         scope = InternalScope('mock', **self.vo)
         files = create_files(3, scope, self.rse1_id)
         dataset = 'dataset_' + str(uuid())
         add_did(scope, dataset, DIDType.DATASET, self.jdoe)
         attach_dids(scope, dataset, files, self.jdoe)
 
         rule_id = add_rule(dids=[{'scope': scope, 'name': dataset}], account=self.jdoe, copies=1, rse_expression=self.rse1, grouping='NONE', weight='fakeweight', lifetime=None, locked=False, subscription_id=None)[0]
-        child_rule = add_rule(dids=[{'scope': scope, 'name': dataset}], account=self.jdoe, copies=1, rse_expression=self.rse3, grouping='NONE', weight='fakeweight', lifetime=-3, locked=False, subscription_id=None)[0]
+        child_rule = add_rule(dids=[{'scope': scope, 'name': dataset}], account=self.jdoe, copies=1, rse_expression=self.rse3, grouping='NONE', weight='fakeweight', lifetime=-1, locked=False, subscription_id=None)[0]
         update_rule(rule_id, {'child_rule_id': child_rule})
 
         rule_cleaner(once=True)
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_judge_evaluator.py` & `rucio-webui-34.1.0/tests/test_judge_evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import TYPE_CHECKING
+
 import pytest
 
 from rucio.common.config import config_get_bool
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.common.utils import generate_uuid as uuid
 from rucio.core.account import get_usage
 from rucio.core.account_limit import set_local_account_limit
@@ -28,17 +29,17 @@
 from rucio.daemons.abacus.account import account_update
 from rucio.daemons.judge.evaluator import re_evaluator
 from rucio.db.sqla.constants import DIDType, LockState
 from rucio.db.sqla.models import UpdatedDID
 from rucio.db.sqla.session import transactional_session
 from rucio.tests.common import RSE_namedtuple
 from rucio.tests.common_server import get_vo
+
 from .test_rule import create_files, tag_generator
 
-from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .temp_factories import TemporaryDidFactory, TemporaryRSEFactory
 
 
 @pytest.fixture(scope="class")
 def setup_class(request, rse_factory_unittest):
     request.cls.setUpClass()
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_judge_injector.py` & `rucio-webui-34.1.0/tests/test_judge_injector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -21,20 +20,21 @@
 from rucio.common.exception import RuleNotFound
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.common.utils import generate_uuid as uuid
 from rucio.core.account_limit import set_local_account_limit
 from rucio.core.did import add_did, attach_dids
 from rucio.core.lock import get_replica_locks
 from rucio.core.rse import add_rse_attribute
-from rucio.core.rule import add_rule, get_rule, approve_rule, deny_rule, list_rules
+from rucio.core.rule import add_rule, approve_rule, deny_rule, get_rule, list_rules
 from rucio.daemons.judge.injector import rule_injector
 from rucio.db.sqla.constants import DIDType, RuleState
 from rucio.db.sqla.models import ReplicationRule
 from rucio.db.sqla.session import transactional_session
 from rucio.tests.common_server import get_vo
+
 from .test_rule import create_files, tag_generator
 
 
 @pytest.fixture(scope="class")
 def setup_class(request, rse_factory_unittest):
     request.cls.setUpClass()
 
@@ -186,15 +186,15 @@
         for i in range(3):
             files = create_files(3, scope, self.rse1_id)
             dataset = 'dataset_' + str(uuid())
             datasets.append(dataset)
             add_did(scope, dataset, DIDType.DATASET, self.jdoe)
             attach_dids(scope, dataset, files, self.jdoe)
             attach_dids(scope, container, [{'scope': scope, 'name': dataset}], self.jdoe)
-        rule_id = add_rule(dids=[{'scope': scope, 'name': container}], account=self.jdoe, copies=1, rse_expression=self.rse1, grouping='DATASET', weight=None, lifetime=900, locked=False, subscription_id=None, ask_approval=True)[0]
+        rule_id = add_rule(dids=[{'scope': scope, 'name': container}], account=self.jdoe, copies=1, rse_expression=self.rse1, grouping='DATASET', weight=None, lifetime=None, locked=False, subscription_id=None, ask_approval=True)[0]
         approve_rule(rule_id, approver=self.jdoe)
         assert (get_rule(rule_id)['state'] == RuleState.INJECT)
         rule_injector(once=True)
         # Check if there is a rule for each file
         with pytest.raises(RuleNotFound):
             get_rule(rule_id)
         for dataset in datasets:
@@ -209,16 +209,16 @@
         for i in range(3):
             files = create_files(3, scope, self.rse1_id)
             dataset = 'dataset_' + str(uuid())
             datasets.append(dataset)
             add_did(scope, dataset, DIDType.DATASET, self.jdoe)
             attach_dids(scope, dataset, files, self.jdoe)
             attach_dids(scope, container, [{'scope': scope, 'name': dataset}], self.jdoe)
-        add_rule(dids=[{'scope': scope, 'name': dataset}], account=self.jdoe, copies=1, rse_expression=self.rse1, grouping='DATASET', weight=None, lifetime=900, locked=False, subscription_id=None, ask_approval=False)
-        rule_id = add_rule(dids=[{'scope': scope, 'name': container}], account=self.jdoe, copies=1, rse_expression=self.rse1, grouping='DATASET', weight=None, lifetime=900, locked=False, subscription_id=None, ask_approval=True)[0]
+        add_rule(dids=[{'scope': scope, 'name': dataset}], account=self.jdoe, copies=1, rse_expression=self.rse1, grouping='DATASET', weight=None, lifetime=None, locked=False, subscription_id=None, ask_approval=False)
+        rule_id = add_rule(dids=[{'scope': scope, 'name': container}], account=self.jdoe, copies=1, rse_expression=self.rse1, grouping='DATASET', weight=None, lifetime=None, locked=False, subscription_id=None, ask_approval=True)[0]
         approve_rule(rule_id, approver=self.jdoe)
         assert (get_rule(rule_id)['state'] == RuleState.INJECT)
         rule_injector(once=True)
         # Check if there is a rule for each file
         with pytest.raises(RuleNotFound):
             get_rule(rule_id)
         for dataset in datasets:
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_judge_repairer.py` & `rucio-webui-34.1.0/tests/test_judge_repairer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,32 +14,32 @@
 
 import itertools
 from hashlib import sha256
 
 import pytest
 from dogpile.cache import make_region
 
-from rucio.common.config import config_get
-from rucio.common.config import config_get_bool
+from rucio.common.config import config_get, config_get_bool
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.core.account_limit import set_local_account_limit
 from rucio.core.did import add_did, attach_dids
-from rucio.core.lock import successful_transfer, failed_transfer, get_replica_locks
+from rucio.core.lock import failed_transfer, get_replica_locks, successful_transfer
 from rucio.core.replica import get_replica
 from rucio.core.request import cancel_request_did
+from rucio.core.rse import add_rse, add_rse_attribute, update_rse
+from rucio.core.rule import add_rule, get_rule
 from rucio.core.transfer import cancel_transfers
-from rucio.core.rse import add_rse_attribute, add_rse, update_rse
-from rucio.core.rule import get_rule, add_rule
 from rucio.daemons.judge.evaluator import re_evaluator
 from rucio.daemons.judge.repairer import rule_repairer
 from rucio.db.sqla import models
-from rucio.db.sqla.constants import DIDType, RuleState, ReplicaState
+from rucio.db.sqla.constants import DIDType, ReplicaState, RuleState
 from rucio.db.sqla.session import get_session
-from rucio.tests.common import rse_name_generator, did_name_generator
+from rucio.tests.common import did_name_generator, rse_name_generator
 from rucio.tests.common_server import get_vo
+
 from .test_rule import create_files, tag_generator
 
 
 @pytest.fixture(scope="class")
 def setup_class(request, rse_factory_unittest):
     request.cls.setUpClass()
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_lifetime.py` & `rucio-webui-34.1.0/tests/test_lifetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
 import json
-
+import os
+from configparser import NoSectionError
 from datetime import datetime, timedelta
 
 import pytest
-from configparser import NoSectionError
 
-from rucio.common.exception import UnsupportedOperation, ConfigNotFound
+from rucio.common.exception import ConfigNotFound, UnsupportedOperation
 from rucio.common.policy import REGION
 from rucio.common.utils import generate_uuid as uuid
-from rucio.tests.common import skip_multivo
 from rucio.core import config as core_config
-from rucio.core.rule import add_rule, get_rule
-from rucio.core.did import set_metadata, get_metadata
+from rucio.core.did import get_metadata, set_metadata
 from rucio.core.lifetime_exception import add_exception
+from rucio.core.rule import add_rule, get_rule
 from rucio.daemons.atropos.atropos import atropos
 from rucio.db.sqla.constants import DIDType
+from rucio.tests.common import skip_multivo
 
 
 @skip_multivo(reason='only valid for ATLAS')
 def test_lifetime_creation_core(root_account, rse_factory, mock_scope, did_factory):
     """
     Test the creation of a lifetime exception on the core side
     """
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_message.py` & `rucio-webui-34.1.0/tests/test_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,20 +14,20 @@
 
 import json
 import random
 import string
 
 import pytest
 
-from rucio.db.sqla.models import Message
-from rucio.db.sqla.session import get_session
 from rucio.common.constants import MAX_MESSAGE_LENGTH
 from rucio.common.exception import InvalidObject, RucioException
 from rucio.common.utils import generate_uuid
-from rucio.core.message import add_message, add_messages, retrieve_messages, delete_messages, truncate_messages
+from rucio.core.message import add_message, add_messages, delete_messages, retrieve_messages, truncate_messages
+from rucio.db.sqla.models import Message
+from rucio.db.sqla.session import get_session
 
 
 @pytest.mark.noparallel(reason='fails when run in parallel')
 @pytest.mark.parametrize("core_config_mock", [{"table_content": [
     ('hermes', 'services_list', 'influx,activemq,elastic,email'),
 ]}], indirect=True)
 @pytest.mark.parametrize("caches_mock", [{"caches_to_mock": [
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_meta_conventions.py` & `rucio-webui-34.1.0/tests/test_meta_conventions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -11,18 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
 
-from rucio.common.exception import InvalidValueForKey, RucioException, UnsupportedValueType, UnsupportedKeyType
+from rucio.common.exception import InvalidValueForKey, RucioException, UnsupportedKeyType, UnsupportedValueType
 from rucio.common.utils import generate_uuid as uuid
 from rucio.core.meta_conventions import add_key
-from rucio.db.sqla import session, models
+from rucio.db.sqla import models, session
 from rucio.db.sqla.constants import DIDType, KeyType
 
 
 @pytest.mark.dirty
 class TestMetaConventionsClient:
 
     def test_add_and_list_keys(self, rucio_client):
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_meta_did.py` & `rucio-webui-34.1.0/tests/test_meta_did.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_module_import.py` & `rucio-webui-34.1.0/tests/test_module_import.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -12,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from rucio.common.utils import execute
 
 
-class TestModuleImport():
+class TestModuleImport:
     def test_import(self):
         """ """
         cmd = 'rucio --version'
         exitcode, out, err = execute(cmd)
         assert 'ImportError' not in err
         assert 'ImportError' not in out
         assert 'Exception' not in err
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_monitor.py` & `rucio-webui-34.1.0/tests/test_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_multi_vo.py` & `rucio-webui-34.1.0/tests/test_multi_vo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -14,17 +13,17 @@
 # limitations under the License.
 
 import os
 from logging import getLogger
 from os import remove
 from random import choice
 from re import search
-from string import ascii_uppercase, ascii_lowercase, ascii_letters, digits
+from string import ascii_letters, ascii_lowercase, ascii_uppercase, digits
 from unittest.mock import patch
-from urllib.parse import urlparse, parse_qs
+from urllib.parse import parse_qs, urlparse
 
 import pytest
 from oic import rndstr
 
 from rucio.api import vo as vo_api
 from rucio.api.account import add_account, list_accounts
 from rucio.api.account_limit import set_local_account_limit
@@ -38,31 +37,32 @@
 from rucio.api.scope import add_scope, list_scopes
 from rucio.api.subscription import add_subscription, list_subscriptions
 from rucio.client.accountlimitclient import AccountLimitClient
 from rucio.client.client import Client
 from rucio.client.replicaclient import ReplicaClient
 from rucio.client.subscriptionclient import SubscriptionClient
 from rucio.client.uploadclient import UploadClient
-from rucio.common.config import config_remove_option, config_set, config_has_section, config_add_section
-from rucio.common.exception import AccessDenied, Duplicate, InvalidRSEExpression, UnsupportedAccountName, \
-    UnsupportedOperation, RucioException
+from rucio.common.config import config_add_section, config_has_section, config_remove_option, config_set
+from rucio.common.exception import AccessDenied, Duplicate, InvalidRSEExpression, RucioException, UnsupportedAccountName, UnsupportedOperation
 from rucio.common.types import InternalAccount
 from rucio.common.utils import generate_uuid, get_tmp_dir, parse_response, ssh_sign
 from rucio.core import config as core_config
 from rucio.core.account_counter import add_counter
 from rucio.core.replica import add_replica
-from rucio.core.rse import get_rses_with_attribute_value, get_rse_id, get_rse_vo
+from rucio.core.rse import get_rse_id, get_rse_vo, get_rses_with_attribute_value
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.core.rule import add_rule
 from rucio.core.vo import map_vo
 from rucio.daemons.automatix.automatix import automatix
-from rucio.db.sqla import models, session as db_session
-from rucio.tests.common import execute, headers, hdrdict, vohdr, auth, loginhdr
+from rucio.db.sqla import models
+from rucio.db.sqla import session as db_session
+from rucio.tests.common import auth, execute, hdrdict, headers, loginhdr, vohdr
+
 from .test_authentication import PRIVATE_KEY, PUBLIC_KEY
-from .test_oidc import get_mock_oidc_client, NEW_TOKEN_DICT
+from .test_oidc import NEW_TOKEN_DICT, get_mock_oidc_client
 
 LOG = getLogger(__name__)
 
 # module-level skip, see https://docs.pytest.org/en/latest/skipping.html#skip-all-test-functions-of-a-class-or-module
 pytestmark = pytest.mark.skipif('SUITE' in os.environ and os.environ['SUITE'] != 'multi_vo',
                                 reason='No execution of the multi_vo tests in a suite other than the multi_vo suite')
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_naming_convention.py` & `rucio-webui-34.1.0/tests/test_naming_convention.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -14,18 +13,15 @@
 # limitations under the License.
 
 import pytest
 
 from rucio.common.exception import InvalidObject
 from rucio.common.types import InternalScope
 from rucio.common.utils import generate_uuid
-from rucio.core.naming_convention import (add_naming_convention,
-                                          validate_name,
-                                          list_naming_conventions,
-                                          delete_naming_convention)
+from rucio.core.naming_convention import add_naming_convention, delete_naming_convention, list_naming_conventions, validate_name
 from rucio.db.sqla.constants import KeyType
 
 
 @pytest.mark.noparallel(reason='changes global naming conventions, breaks other tests')
 class TestNamingConventionCore:
     '''
     Class to test naming convention enforcement.
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_oauthmanager.py` & `rucio-webui-34.1.0/tests/test_oauthmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_oidc.py` & `rucio-webui-34.1.0/tests/test_oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -14,33 +13,29 @@
 # limitations under the License.
 
 import time
 import traceback
 import uuid
 from datetime import datetime, timedelta
 from unittest.mock import MagicMock, patch
-from urllib.parse import urlparse, parse_qs
+from urllib.parse import parse_qs, urlparse
 
 import pytest
 from jwkest.jwt import JWT
 from oic import rndstr
 
 from rucio.common.config import config_get_bool
-from rucio.common.exception import (CannotAuthenticate, DatabaseException)
-from rucio.common.exception import Duplicate
+from rucio.common.exception import CannotAuthenticate, DatabaseException, Duplicate
 from rucio.common.types import InternalAccount
 from rucio.core.account import add_account
 from rucio.core.authentication import redirect_auth_oidc, validate_auth_token
 from rucio.core.identity import add_account_identity
-from rucio.core.oidc import (get_auth_oidc, get_token_oidc, get_token_for_account_operation,
-                             EXPECTED_OIDC_AUDIENCE, EXPECTED_OIDC_SCOPE, oidc_identity_string,
-                             _token_cache_get, _token_cache_set)
+from rucio.core.oidc import EXPECTED_OIDC_AUDIENCE, EXPECTED_OIDC_SCOPE, _token_cache_get, _token_cache_set, get_auth_oidc, get_token_for_account_operation, get_token_oidc, oidc_identity_string
 from rucio.db.sqla import models
-from rucio.db.sqla.constants import AccountType
-from rucio.db.sqla.constants import IdentityType
+from rucio.db.sqla.constants import AccountType, IdentityType
 from rucio.db.sqla.session import get_session
 from rucio.tests.common_server import get_vo
 
 NEW_TOKEN_DICT = {'access_token': 'eyJ3bG...',
                   'expires_in': 3599,
                   'id_token': {'sub': 'abcdefg23', 'iss': 'https://test_auth_url_string/', 'nonce': 'mynonce'},
                   'scope': 'openid profile',
@@ -187,15 +182,15 @@
         return None
 
     @classmethod
     def parse_response(cls, AuthorizationResponse, info=None, sformat="urlencoded"):
         return None
 
 
-class MockResponse(object):
+class MockResponse:
     def __init__(self, json_data):
         self.json_data = json_data
 
     def json(self):
         return self.json_data
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_permission.py` & `rucio-webui-34.1.0/tests/test_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -12,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from rucio.api.permission import has_permission
 from rucio.common.config import config_get
 from rucio.common.types import InternalScope
-from rucio.core.scope import add_scope
 from rucio.core.account import add_account_attribute
+from rucio.core.scope import add_scope
 from rucio.tests.common import scope_name_generator, skip_non_belleii
 
 
 class TestPermissionCoreApi:
     """
     Test the Permission Core and API
     """
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_pfns.py` & `rucio-webui-34.1.0/tests/test_pfns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_ping.py` & `rucio-webui-34.1.0/tests/test_ping.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_preparer.py` & `rucio-webui-34.1.0/tests/test_preparer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -12,23 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import pytest
 
-from rucio.core.distance import get_distances, add_distance
+from rucio.core.distance import add_distance, get_distances
 from rucio.core.replica import add_replicas
-from rucio.core.request import list_and_mark_transfer_requests_and_source_replicas, set_transfer_limit, list_transfer_limits, get_request
+from rucio.core.request import get_request, list_and_mark_transfer_requests_and_source_replicas, list_transfer_limits, set_transfer_limit
+from rucio.core.rse import RseCollection, RseData, add_rse_attribute
 from rucio.core.transfer import get_supported_transfertools
-from rucio.core.rse import add_rse_attribute, RseData, RseCollection
 from rucio.daemons.conveyor.preparer import preparer
-from rucio.db.sqla.session import get_session
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import RequestState
+from rucio.db.sqla.session import get_session
 
 
 @pytest.fixture
 def dest_rse(vo, rse_factory):
     rse_name, rse_id = rse_factory.make_mock_rse()
     yield {'name': rse_name, 'id': rse_id}
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_qos.py` & `rucio-webui-34.1.0/tests/test_qos.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from rucio.core.rse import update_rse, get_rse
+from rucio.core.rse import get_rse, update_rse
 
 
 class TestQoS:
 
     def test_update_and_remove_rse_qos_class(self, rse_factory):
         """ QoS (CORE): Update and remove QoS class for RSE """
         rse_name, rse_id = rse_factory.make_mock_rse()
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_quarantined_replica.py` & `rucio-webui-34.1.0/tests/test_quarantined_replica.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -13,16 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
 
 from rucio.common.config import config_get_bool
 from rucio.common.utils import generate_uuid
-from rucio.core.quarantined_replica import add_quarantined_replicas, list_quarantined_replicas, \
-    delete_quarantined_replicas
+from rucio.core.quarantined_replica import add_quarantined_replicas, delete_quarantined_replicas, list_quarantined_replicas
 from rucio.core.rse import get_rse_id
 from rucio.tests.common_server import get_vo
 
 
 @pytest.mark.noparallel(reason='uses pre-defined rses')
 def test_quarantined_replicas():
     """ QUARANTINED REPLICA (CORE): Add, List and Delete quarantined replicas """
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_reaper.py` & `rucio-webui-34.1.0/tests/test_reaper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -16,30 +15,29 @@
 from datetime import datetime, timedelta
 
 import pytest
 from sqlalchemy import and_, or_
 
 from rucio.api import replica as replica_api
 from rucio.api import rse as rse_api
-from rucio.db.sqla import models
-from rucio.db.sqla.constants import OBSOLETE
-from rucio.db.sqla.session import get_session
-from rucio.common.exception import ReplicaNotFound, DataIdentifierNotFound
+from rucio.common.exception import DataIdentifierNotFound, ReplicaNotFound
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.common.utils import generate_uuid
 from rucio.core import did as did_core
 from rucio.core import message as message_core
 from rucio.core import replica as replica_core
 from rucio.core import rse as rse_core
 from rucio.core import rule as rule_core
-from rucio.daemons.reaper.reaper import reaper
 from rucio.daemons.reaper.dark_reaper import reaper as dark_reaper
+from rucio.daemons.reaper.reaper import reaper
 from rucio.daemons.reaper.reaper import run as run_reaper
+from rucio.db.sqla import models
+from rucio.db.sqla.constants import OBSOLETE
 from rucio.db.sqla.models import ConstituentAssociationHistory
-from rucio.db.sqla.session import read_session
+from rucio.db.sqla.session import get_session, read_session
 from rucio.tests.common import rse_name_generator, skip_rse_tests_with_accounts
 from tests.ruciopytest import NoParallelGroups
 
 __mock_protocol = {'scheme': 'MOCK',
                    'hostname': 'localhost',
                    'port': 123,
                    'prefix': '/test/reaper',
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_redirect.py` & `rucio-webui-34.1.0/tests/test_redirect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_replica.py` & `rucio-webui-34.1.0/tests/test_replica.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -14,44 +13,38 @@
 # limitations under the License.
 
 import hashlib
 import os
 import time
 from datetime import datetime, timedelta
 from json import dumps
+from typing import TYPE_CHECKING
 from unittest import mock
 from xml.etree import ElementTree
 
 import pytest
 import xmltodict
-from werkzeug.datastructures import MultiDict
-from werkzeug.datastructures import Headers
+from werkzeug.datastructures import Headers, MultiDict
 
 from rucio.client.ruleclient import RuleClient
-from rucio.common.exception import (DataIdentifierNotFound, AccessDenied, RucioException,
-                                    ReplicaIsLocked, ReplicaNotFound, ScopeNotFound,
-                                    DatabaseException, InputValidationError)
+from rucio.common.exception import AccessDenied, DatabaseException, DataIdentifierNotFound, InputValidationError, ReplicaIsLocked, ReplicaNotFound, RucioException, ScopeNotFound
 from rucio.common.schema import get_schema_value
-from rucio.common.utils import generate_uuid, clean_surls, parse_response
+from rucio.common.utils import clean_surls, generate_uuid, parse_response
 from rucio.core.config import set as cconfig_set
-from rucio.core.did import add_did, attach_dids, get_did, set_status, list_files, get_did_atime
-from rucio.core.replica import (add_replica, add_replicas, delete_replicas, get_replicas_state,
-                                get_replica, list_replicas, update_replica_state,
-                                get_RSEcoverage_of_dataset, get_replica_atime,
-                                touch_replica, get_bad_pfns, set_tombstone, add_bad_dids)
+from rucio.core.did import add_did, attach_dids, get_did, get_did_atime, list_files, set_status
+from rucio.core.replica import add_bad_dids, add_replica, add_replicas, delete_replicas, get_bad_pfns, get_replica, get_replica_atime, get_replicas_state, get_RSEcoverage_of_dataset, list_replicas, set_tombstone, touch_replica, update_replica_state
 from rucio.core.rse import add_protocol, add_rse_attribute, del_rse_attribute
 from rucio.daemons.badreplicas.minos import minos
 from rucio.daemons.badreplicas.minos_temporary_expiration import minos_tu_expiration
 from rucio.db.sqla import models
-from rucio.db.sqla.constants import DIDType, ReplicaState, BadPFNStatus, OBSOLETE
+from rucio.db.sqla.constants import OBSOLETE, BadPFNStatus, DIDType, ReplicaState
 from rucio.db.sqla.session import transactional_session
 from rucio.rse import rsemanager as rsemgr
-from rucio.tests.common import execute, headers, auth, Mime, accept, did_name_generator
+from rucio.tests.common import Mime, accept, auth, did_name_generator, execute, headers
 
-from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .temp_factories import TemporaryRSEFactory
 
 
 def mocked_VP_requests_get(*args, **kwargs):
     """This method will be used by the mock to replace requests.get to VP server."""
     class MockResponse:
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_replica_recoverer.py` & `rucio-webui-34.1.0/tests/test_replica_recoverer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import json
 from datetime import datetime, timedelta
 from os import remove
 from time import sleep
 
 import pytest
-import json
 
-from rucio.core.replica import (update_replica_state, list_replicas, list_bad_replicas_status)
-from rucio.core.rse import add_rse_attribute
-from rucio.core.did import set_metadata
 from rucio.core import rse_expression_parser
+from rucio.core.did import set_metadata
+from rucio.core.replica import list_bad_replicas_status, list_replicas, update_replica_state
+from rucio.core.rse import add_rse_attribute
 from rucio.daemons.replicarecoverer.suspicious_replica_recoverer import run, stop
-from rucio.db.sqla.constants import DIDType, BadFilesStatus, ReplicaState
+from rucio.db.sqla.constants import BadFilesStatus, DIDType, ReplicaState
 from rucio.tests.common import execute
 
 
 class TestReplicaRecoverer:
 
     @pytest.fixture(autouse=True)
     def setup_obj(self, vo, rse_factory, replica_client, mock_scope, file_factory, scope_factory):
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_replica_sorting.py` & `rucio-webui-34.1.0/tests/test_replica_sorting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -12,27 +11,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 import json
 import os
+from tempfile import mkstemp
 from unittest import mock
 from urllib.parse import urlparse
-from tempfile import mkstemp
 
 import geoip2.database
 import pytest
 
-from rucio.common.utils import parse_replicas_from_string
 from rucio.common.config import config_get
-from rucio.core import rse_expression_parser, replica_sorter
+from rucio.common.utils import parse_replicas_from_string
+from rucio.core import replica_sorter, rse_expression_parser
 from rucio.core.replica import add_replicas, delete_replicas
-from rucio.core.rse import add_rse, del_rse, add_rse_attribute, add_protocol, del_rse_attribute
-from rucio.tests.common import rse_name_generator, headers, auth, vohdr, Mime, accept
+from rucio.core.rse import add_protocol, add_rse, add_rse_attribute, del_rse, del_rse_attribute
+from rucio.tests.common import Mime, accept, auth, headers, rse_name_generator, vohdr
+
 from .inputs import GEOIP_LITE2_CITY_TEST_DB
 
 LOCATION_TO_IP = {
     'Switzerland': '2a02:d000::1',
     'Romania': '2a02:e940::1',
     'Austria': '2a02:da80::1',
     'United Kingdom': '81.2.69.142',
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_request.py` & `rucio-webui-34.1.0/tests/test_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -19,19 +18,19 @@
 
 import pytest
 
 from rucio.common.config import config_get_bool
 from rucio.common.utils import generate_uuid, parse_response
 from rucio.core.distance import add_distance
 from rucio.core.replica import add_replica
-from rucio.core.request import queue_requests, get_request_by_did, list_requests, list_requests_history, set_transfer_limit, TransferStatsManager
+from rucio.core.request import TransferStatsManager, get_request_by_did, list_requests, list_requests_history, queue_requests, set_transfer_limit
 from rucio.core.rse import add_rse_attribute
-from rucio.db.sqla import models, constants
-from rucio.db.sqla.constants import RequestType, RequestState
-from rucio.tests.common import vohdr, hdrdict, headers, auth
+from rucio.db.sqla import constants, models
+from rucio.db.sqla.constants import RequestState, RequestType
+from rucio.tests.common import auth, hdrdict, headers, vohdr
 
 
 @pytest.mark.parametrize("file_config_mock", [
     # Run test twice: with, and without, preparer enabled
     {
         "overrides": [
             ('conveyor', 'use_preparer', 'true')
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_root_proxy.py` & `rucio-webui-34.1.0/tests/test_root_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,16 +14,16 @@
 
 from urllib.parse import urlencode
 
 import pytest
 
 from rucio.core.config import set as config_set
 from rucio.core.replica import add_replicas, delete_replicas
-from rucio.core.rse import add_rse, add_rse_attribute, del_rse, add_protocol
-from rucio.tests.common import rse_name_generator, vohdr, headers
+from rucio.core.rse import add_protocol, add_rse, add_rse_attribute, del_rse
+from rucio.tests.common import headers, rse_name_generator, vohdr
 
 client_location_without_proxy = {'ip': '192.168.0.1',
                                  'fqdn': 'anomalous-materials.blackmesa.com',
                                  'site': 'BLACKMESA1'}
 
 client_location_with_proxy = {'ip': '10.0.1.1',
                               'fqdn': 'test-chamber.aperture.com',
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rse.py` & `rucio-webui-34.1.0/tests/test_rse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -13,37 +12,46 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
 
 from rucio.client.replicaclient import ReplicaClient
 from rucio.common import exception
-from rucio.common.exception import (Duplicate, RSENotFound, RSEProtocolNotSupported,
-                                    InvalidObject, ResourceTemporaryUnavailable,
-                                    RSEAttributeNotFound, RSEOperationNotSupported,
-                                    InputValidationError)
+from rucio.common.exception import Duplicate, InputValidationError, InvalidObject, ResourceTemporaryUnavailable, RSEAttributeNotFound, RSENotFound, RSEOperationNotSupported, RSEProtocolNotSupported
 from rucio.common.schema import get_schema_value
-from rucio.common.utils import GLOBALLY_SUPPORTED_CHECKSUMS, CHECKSUM_KEY
-from rucio.core.account_limit import set_local_account_limit, get_rse_account_usage
+from rucio.common.utils import CHECKSUM_KEY, GLOBALLY_SUPPORTED_CHECKSUMS
+from rucio.core.account_limit import get_rse_account_usage, set_local_account_limit
 from rucio.core.did import add_did, attach_dids
+from rucio.core.request import delete_transfer_limit, set_transfer_limit
+from rucio.core.rse import (
+    add_rse,
+    add_rse_attribute,
+    del_rse,
+    del_rse_attribute,
+    get_rse,
+    get_rse_attribute,
+    get_rse_id,
+    get_rse_protocols,
+    get_rse_supported_checksums_from_attributes,
+    get_rse_transfer_limits,
+    list_rse_attributes,
+    list_rses,
+    parse_checksum_support_attribute,
+    restore_rse,
+    rse_exists,
+    rse_is_empty,
+    update_rse,
+)
 from rucio.core.rule import add_rule
-from rucio.core.request import set_transfer_limit, delete_transfer_limit
-from rucio.core.rse import (add_rse, get_rse_id, del_rse, restore_rse, list_rses,
-                            rse_exists, add_rse_attribute, list_rse_attributes,
-                            get_rse_transfer_limits,
-                            get_rse_protocols,
-                            del_rse_attribute, get_rse_attribute, get_rse, rse_is_empty,
-                            parse_checksum_support_attribute,
-                            get_rse_supported_checksums_from_attributes,
-                            update_rse)
 from rucio.daemons.abacus.account import account_update
-from rucio.db.sqla import session, models
-from rucio.db.sqla.constants import RSEType, DIDType
+from rucio.db.sqla import models, session
+from rucio.db.sqla.constants import DIDType, RSEType
 from rucio.rse import rsemanager as mgr
-from rucio.tests.common import rse_name_generator, hdrdict, auth, headers, did_name_generator
+from rucio.tests.common import auth, did_name_generator, hdrdict, headers, rse_name_generator
+
 from .test_rule import create_files
 
 
 class TestRSECoreApi:
 
     def test_create_and_check_for_rse(self, vo):
         """ RSE (CORE): Test the creation, query, and deletion of a RSE """
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rse_expression_parser.py` & `rucio-webui-34.1.0/tests/test_rse_expression_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -10,21 +9,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from random import choice
-from string import ascii_uppercase, ascii_lowercase
+from string import ascii_lowercase, ascii_uppercase
 
 import pytest
 
 from rucio.common.exception import InvalidRSEExpression, RSEWriteBlocked
-from rucio.core import rse
-from rucio.core import rse_expression_parser
+from rucio.core import rse, rse_expression_parser
 
 
 def attribute_name_generator(size=10):
     return ''.join(choice(ascii_uppercase)).join(choice(ascii_lowercase) for x in range(size - 1))
 
 
 @pytest.mark.noparallel(reason='uses pre-defined RSE, test_all_rse fails when run in parallel')
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rse_lfn2path.py` & `rucio-webui-34.1.0/tests/test_rse_lfn2path.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -11,22 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 import os
+from configparser import NoOptionError, NoSectionError
 
 import pytest
 
 from rucio.common import config
 from rucio.rse.protocols.protocol import RSEDeterministicTranslation
 
-from configparser import NoOptionError, NoSectionError
-
 
 @pytest.mark.noparallel(reason='uses pre-defined RSE, changes global configuration value')
 class TestDeterministicTranslation:
     """
     Verify the deterministic translator.
     """
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rse_protocol_gfal2.py` & `rucio-webui-34.1.0/tests/test_rse_protocol_gfal2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +14,16 @@
 
 import os
 
 import pytest
 
 from rucio.common.utils import execute
 from rucio.rse import rsemanager as mgr
-from rucio.tests.common import skip_rse_tests_with_accounts, load_test_conf_file
+from rucio.tests.common import load_test_conf_file, skip_rse_tests_with_accounts
+
 from .rsemgr_api_test import MgrTestCases
 
 
 @skip_rse_tests_with_accounts
 class TestRseGFAL2(MgrTestCases):
 
     @classmethod
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rse_protocol_gfal2_impl.py` & `rucio-webui-34.1.0/tests/test_rse_protocol_gfal2_impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +14,16 @@
 
 import os
 
 import pytest
 
 from rucio.common.utils import execute
 from rucio.rse import rsemanager
-from rucio.tests.common import skip_rse_tests_with_accounts, load_test_conf_file
+from rucio.tests.common import load_test_conf_file, skip_rse_tests_with_accounts
+
 from .rsemgr_api_test import MgrTestCases
 
 
 @pytest.mark.noparallel(reason='creates and removes a test directory with a fixed name')
 @skip_rse_tests_with_accounts
 class TestRseGFAL2Impl(MgrTestCases):
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rse_protocol_posix.py` & `rucio-webui-34.1.0/tests/test_rse_protocol_posix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +14,16 @@
 
 import os
 import shutil
 
 import pytest
 
 from rucio.rse import rsemanager as mgr
-from rucio.tests.common import skip_rse_tests_with_accounts, load_test_conf_file
+from rucio.tests.common import load_test_conf_file, skip_rse_tests_with_accounts
+
 from .rsemgr_api_test import MgrTestCases
 
 
 def setup_posix_test_env(rse_name, rse_settings, user):
     """POSIX (RSE/PROTOCOLS): Creating necessary directories and files """
 
     data = load_test_conf_file('rse_repository.json')
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rse_protocol_rclone.py` & `rucio-webui-34.1.0/tests/test_rse_protocol_rclone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -13,17 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 import pytest
 
-from rucio.common.utils import execute, PREFERRED_CHECKSUM, set_preferred_checksum
+from rucio.common.utils import PREFERRED_CHECKSUM, execute, set_preferred_checksum
 from rucio.rse import rsemanager
-from rucio.tests.common import skip_rse_tests_with_accounts, load_test_conf_file
+from rucio.tests.common import load_test_conf_file, skip_rse_tests_with_accounts
+
 from .rsemgr_api_test import MgrTestCases
 
 
 @pytest.mark.noparallel(reason='creates and removes a test directory with a fixed name')
 @skip_rse_tests_with_accounts
 class TestRseRCLONE(MgrTestCases):
     original_prefchecksum = PREFERRED_CHECKSUM
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rse_protocol_rsync.py` & `rucio-webui-34.1.0/tests/test_rse_protocol_rsync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -13,17 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 import pytest
 
-from rucio.common.utils import execute, PREFERRED_CHECKSUM, set_preferred_checksum
+from rucio.common.utils import PREFERRED_CHECKSUM, execute, set_preferred_checksum
 from rucio.rse import rsemanager
-from rucio.tests.common import skip_rse_tests_with_accounts, load_test_conf_file
+from rucio.tests.common import load_test_conf_file, skip_rse_tests_with_accounts
+
 from .rsemgr_api_test import MgrTestCases
 
 
 @pytest.mark.noparallel(reason='creates and removes a test directory with a fixed name')
 @skip_rse_tests_with_accounts
 class TestRseRSYNC(MgrTestCases):
     original_prefchecksum = PREFERRED_CHECKSUM
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rse_protocol_srm.py` & `rucio-webui-34.1.0/tests/test_rse_protocol_srm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +14,16 @@
 
 import os
 
 import pytest
 
 from rucio.common.utils import execute
 from rucio.rse import rsemanager as mgr
-from rucio.tests.common import skip_rse_tests_with_accounts, load_test_conf_file
+from rucio.tests.common import load_test_conf_file, skip_rse_tests_with_accounts
+
 from .rsemgr_api_test import MgrTestCases
 
 
 @skip_rse_tests_with_accounts
 class TestRseSRM(MgrTestCases):
 
     @classmethod
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rse_protocol_ssh.py` & `rucio-webui-34.1.0/tests/test_rse_protocol_ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -13,17 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 import pytest
 
-from rucio.common.utils import execute, PREFERRED_CHECKSUM, set_preferred_checksum
+from rucio.common.utils import PREFERRED_CHECKSUM, execute, set_preferred_checksum
 from rucio.rse import rsemanager
-from rucio.tests.common import skip_rse_tests_with_accounts, load_test_conf_file
+from rucio.tests.common import load_test_conf_file, skip_rse_tests_with_accounts
+
 from .rsemgr_api_test import MgrTestCases
 
 
 @pytest.mark.noparallel(reason='creates and removes a test directory with a fixed name')
 @skip_rse_tests_with_accounts
 class TestRseSSH(MgrTestCases):
     original_prefchecksum = PREFERRED_CHECKSUM
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rse_protocol_webdav.py` & `rucio-webui-34.1.0/tests/test_rse_protocol_webdav.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -16,15 +15,16 @@
 import os
 
 import pytest
 import requests
 
 from rucio.common.exception import FileReplicaAlreadyExists
 from rucio.rse import rsemanager
-from rucio.tests.common import skip_rse_tests_with_accounts, load_test_conf_file
+from rucio.tests.common import load_test_conf_file, skip_rse_tests_with_accounts
+
 from .rsemgr_api_test import MgrTestCases
 
 
 @skip_rse_tests_with_accounts
 class TestRseWebDAV(MgrTestCases):
     """
     Test the WebDAV protocol
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rse_protocol_xrootd.py` & `rucio-webui-34.1.0/tests/test_rse_protocol_xrootd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +14,16 @@
 
 import os
 
 import pytest
 
 from rucio.common.utils import execute
 from rucio.rse import rsemanager
-from rucio.tests.common import skip_rse_tests_with_accounts, load_test_conf_file
+from rucio.tests.common import load_test_conf_file, skip_rse_tests_with_accounts
+
 from .rsemgr_api_test import MgrTestCases
 
 
 @pytest.mark.noparallel(reason='creates and removes a test directory with a fixed name')
 @skip_rse_tests_with_accounts
 class TestRseXROOTD(MgrTestCases):
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rse_selector.py` & `rucio-webui-34.1.0/tests/test_rse_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -13,16 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import pytest
 
 from rucio.common.exception import InsufficientAccountLimit, InsufficientTargetRSEs
-from rucio.core.account_counter import update_account_counter, increase
-from rucio.core.account_limit import set_local_account_limit, set_global_account_limit
+from rucio.core.account_counter import increase, update_account_counter
+from rucio.core.account_limit import set_global_account_limit, set_local_account_limit
 from rucio.core.rse_selector import RSESelector
 
 
 @pytest.fixture
 def test_rses(rse_factory):
     rse1_name, rse1_id = rse_factory.make_mock_rse()
     rse2_name, rse2_id = rse_factory.make_mock_rse()
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rucio_server.py` & `rucio-webui-34.1.0/tests/test_rucio_server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_rule.py` & `rucio-webui-34.1.0/tests/test_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,61 +1,72 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from collections import namedtuple
 import json
 import random
 import string
+from collections import namedtuple
 from logging import getLogger
+from typing import TYPE_CHECKING
 
 import pytest
 
 import rucio.api.rule
 from rucio.api.account import add_account
 from rucio.client.ruleclient import RuleClient
 from rucio.common.config import config_get_bool
-from rucio.common.exception import (RucioException, RuleNotFound, AccessDenied, InsufficientAccountLimit, DuplicateRule, RSEWriteBlocked,
-                                    RSEOverQuota, RuleReplaceFailed, ManualRuleApprovalBlocked, InputValidationError,
-                                    UnsupportedOperation, InvalidValueForKey, InvalidSourceReplicaExpression)
+from rucio.common.exception import (
+    AccessDenied,
+    DuplicateRule,
+    InputValidationError,
+    InsufficientAccountLimit,
+    InvalidSourceReplicaExpression,
+    InvalidValueForKey,
+    ManualRuleApprovalBlocked,
+    RSEOverQuota,
+    RSEWriteBlocked,
+    RucioException,
+    RuleNotFound,
+    RuleReplaceFailed,
+    UnsupportedOperation,
+)
 from rucio.common.policy import get_policy
 from rucio.common.schema import get_schema_value
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.common.utils import generate_uuid as uuid
-from rucio.core.account import add_account_attribute, get_usage, get_account
-from rucio.core.account_limit import set_local_account_limit, set_global_account_limit
+from rucio.core.account import add_account_attribute, get_account, get_usage
+from rucio.core.account_limit import set_global_account_limit, set_local_account_limit
 from rucio.core.did import add_did, attach_dids, set_status
-from rucio.core.lock import get_replica_locks, get_dataset_locks, successful_transfer
+from rucio.core.lock import get_dataset_locks, get_replica_locks, successful_transfer
 from rucio.core.replica import add_replica, get_replica
 from rucio.core.request import get_request_by_did
-from rucio.core.rse import add_rse_attribute, add_rse, update_rse, get_rse_id, del_rse, del_rse_attribute, set_rse_limits
+from rucio.core.rse import add_rse, add_rse_attribute, del_rse, del_rse_attribute, get_rse_id, set_rse_limits, update_rse
 from rucio.core.rse_counter import get_counter as get_rse_counter
-from rucio.core.rule import add_rule, get_rule, delete_rule, add_rules, update_rule, reduce_rule, move_rule, list_rules
+from rucio.core.rule import add_rule, add_rules, delete_rule, get_rule, list_rules, move_rule, reduce_rule, update_rule
 from rucio.core.scope import add_scope
 from rucio.daemons.abacus.account import account_update
 from rucio.daemons.abacus.rse import rse_update
 from rucio.daemons.judge.evaluator import re_evaluator
 from rucio.db.sqla import models
-from rucio.db.sqla.constants import DIDType, OBSOLETE, RuleState, LockState
+from rucio.db.sqla.constants import OBSOLETE, DIDType, LockState, RuleState
 from rucio.db.sqla.session import transactional_session
-from rucio.tests.common import rse_name_generator, account_name_generator, did_name_generator
+from rucio.tests.common import account_name_generator, did_name_generator, rse_name_generator
 from rucio.tests.common_server import get_vo
 
-from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .temp_factories import TemporaryDidFactory, TemporaryRSEFactory
 
 LOG = getLogger(__name__)
 RSE_namedtuple = namedtuple('RSE_namedtuple', ['name', 'id'])
 
 
@@ -177,17 +188,18 @@
         1) by deleting the source RSE
         2) by referring to the source RSE via an RSE attribute and then deleting
             said RSE attribute from the source RSE
         in both cases the source replica expression is invalidated since it
         evaluates to an empty set.
         """
 
-        from dogpile.cache.api import NO_VALUE
         from hashlib import sha256
 
+        from dogpile.cache.api import NO_VALUE
+
         # create RSEs A, B, C (structured into namedtuples)
         rseA, rseB, rseC = (
             RSE_namedtuple(*rse_factory.make_mock_rse()) for _ in range(3)
         )
         rsekey, rseval = tag_generator(), tag_generator()
         add_rse_attribute(rseA.id, rsekey, rseval)
 
@@ -1377,14 +1389,29 @@
 
         ret = rucio_client.list_did_rules(scope=mock_scope.external, name=dataset['name'])
         ids = [rule['id'] for rule in ret]
 
         assert rule_id_1 in ids
         assert rule_id_2 in ids
 
+    def test_list_rules_by_name(self, mock_scope, did_factory, jdoe_account, rucio_client):
+        """ NAME (CLIENT): List Replication Rules per NAME """
+        files = create_files(1, mock_scope, self.rse1_id)
+        dataset = did_factory.random_dataset_did()
+        add_did(did_type=DIDType.DATASET, account=jdoe_account, **dataset)
+        attach_dids(dids=files, account=jdoe_account, **dataset)
+
+        rule_id_1 = add_rule(dids=[dataset], account=jdoe_account, copies=1, rse_expression=self.rse1, grouping='NONE', weight='fakeweight', lifetime=None, locked=False, subscription_id=None)[0]
+        rule_id_2 = add_rule(dids=[dataset], account=jdoe_account, copies=1, rse_expression=self.rse2, grouping='NONE', weight='fakeweight', lifetime=None, locked=False, subscription_id=None)[0]
+        ret = rucio_client.list_associated_rules_for_file(scope=mock_scope.external, name=files[0]['name'])
+        ids = [rule['id'] for rule in ret]
+
+        assert rule_id_1 in ids
+        assert rule_id_2 in ids
+
     def test_get_rule(self, mock_scope, did_factory, jdoe_account):
         """ REPLICATION RULE (CLIENT): Get Replication Rule by id """
         activity = get_schema_value('ACTIVITY')['enum'][0]
         files = create_files(3, mock_scope, self.rse1_id)
         dataset = did_factory.random_dataset_did()
         add_did(did_type=DIDType.DATASET, account=jdoe_account, **dataset)
         attach_dids(dids=files, account=jdoe_account, **dataset)
@@ -1435,32 +1462,32 @@
     def test_change_rule_lifetime(self, mock_scope, did_factory, jdoe_account):
         """ REPLICATION RULE (CLIENT): Change rule lifetime"""
         files = create_files(3, mock_scope, self.rse1_id)
         dataset = did_factory.random_dataset_did()
         add_did(did_type=DIDType.DATASET, account=jdoe_account, **dataset)
         attach_dids(dids=files, account=jdoe_account, **dataset)
 
-        rule_id_1 = add_rule(dids=[dataset], account=jdoe_account, copies=1, rse_expression=self.rse1, grouping='DATASET', weight='fakeweight', lifetime=150, locked=True, subscription_id=None)[0]
+        rule_id_1 = add_rule(dids=[dataset], account=jdoe_account, copies=1, rse_expression=self.rse1, grouping='DATASET', weight='fakeweight', lifetime=None, locked=True, subscription_id=None)[0]
 
         get = self.rule_client.get_replication_rule(rule_id_1)
 
-        self.rule_client.update_replication_rule(rule_id_1, options={'lifetime': 10000})
+        self.rule_client.update_replication_rule(rule_id_1, options={'lifetime': -1})
 
         get2 = self.rule_client.get_replication_rule(rule_id_1)
 
         assert (get['expires_at'] != get2['expires_at'])
 
     def test_approve_rule(self, mock_scope, did_factory, jdoe_account):
         """ REPLICATION RULE (CLIENT): Approve rule"""
         files = create_files(3, mock_scope, self.rse1_id)
         dataset = did_factory.random_dataset_did()
         add_did(did_type=DIDType.DATASET, account=jdoe_account, **dataset)
         attach_dids(dids=files, account=jdoe_account, **dataset)
 
-        rule_id = add_rule(dids=[dataset], account=jdoe_account, copies=1, rse_expression=self.rse1, grouping='DATASET', weight='fakeweight', lifetime=150, locked=True, subscription_id=None, ask_approval=True)[0]
+        rule_id = add_rule(dids=[dataset], account=jdoe_account, copies=1, rse_expression=self.rse1, grouping='DATASET', weight='fakeweight', lifetime=None, locked=True, subscription_id=None, ask_approval=True)[0]
         rule = self.rule_client.get_replication_rule(rule_id)
         assert rule['state'] == RuleState.WAITING_APPROVAL.name
         self.rule_client.approve_replication_rule(rule_id)
         rule = self.rule_client.get_replication_rule(rule_id)
         assert rule['state'] == RuleState.INJECT.name
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_schema_cms.py` & `rucio-webui-34.1.0/tests/test_schema_cms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -14,15 +13,14 @@
 # limitations under the License.
 
 import pytest
 
 from rucio.common.exception import InvalidObject
 from rucio.common.schema.cms import validate_schema
 
-
 # Some tests adapted from https://github.com/dmwm/WMCore/blob/master/test/python/WMCore_t/Lexicon_t.py
 
 class TestSchemaCMS:
 
     def test_site_names(self):
         """ CMS SCHEMA (COMMON): Test site/RSE names """
         validate_schema('rse', 'T2_US_Nebraska')
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_scope.py` & `rucio-webui-34.1.0/tests/test_scope.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -13,19 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from json import loads
 
 import pytest
 
-from rucio.common.exception import AccountNotFound, Duplicate, ScopeNotFound, InvalidObject
+from rucio.common.exception import AccountNotFound, Duplicate, InvalidObject, ScopeNotFound
 from rucio.common.types import InternalScope
 from rucio.common.utils import generate_uuid as uuid
-from rucio.core.scope import get_scopes, add_scope, is_scope_owner
-from rucio.tests.common import account_name_generator, scope_name_generator, headers, auth, hdrdict
+from rucio.core.scope import add_scope, get_scopes, is_scope_owner
+from rucio.tests.common import account_name_generator, auth, hdrdict, headers, scope_name_generator
 
 
 class TestScopeCoreApi:
 
     def test_list_scopes(self, vo, jdoe_account):
         scopes = [InternalScope(scope_name_generator(), vo=vo) for _ in range(5)]
         """ SCOPE (CORE): List scopes """
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_subscription.py` & `rucio-webui-34.1.0/tests/test_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,30 +14,28 @@
 
 from datetime import datetime
 from json import loads
 from json.decoder import JSONDecodeError
 
 import pytest
 
-from rucio.api.subscription import list_subscriptions, add_subscription, update_subscription, \
-    list_subscription_rule_states, get_subscription_by_id
-from rucio.db.sqla.constants import RuleState
-from rucio.common.exception import InvalidObject, SubscriptionNotFound, SubscriptionDuplicate
+from rucio.api.subscription import add_subscription, get_subscription_by_id, list_subscription_rule_states, list_subscriptions, update_subscription
+from rucio.common.exception import InvalidObject, SubscriptionDuplicate, SubscriptionNotFound
 from rucio.common.schema import get_schema_value
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.common.utils import generate_uuid as uuid
+from rucio.core import subscription as subscription_core
 from rucio.core.account import add_account
-from rucio.core.did import add_did, set_new_dids, list_new_dids, attach_dids, set_status
-from rucio.core.rule import add_rule
+from rucio.core.did import add_did, attach_dids, list_new_dids, set_new_dids, set_status
 from rucio.core.rse import add_rse_attribute
+from rucio.core.rule import add_rule
 from rucio.core.scope import add_scope
-from rucio.core import subscription as subscription_core
-from rucio.daemons.transmogrifier.transmogrifier import run, get_subscriptions
-from rucio.db.sqla.constants import AccountType, DIDType
-from rucio.tests.common import headers, auth, did_name_generator, rse_name_generator
+from rucio.daemons.transmogrifier.transmogrifier import get_subscriptions, run
+from rucio.db.sqla.constants import AccountType, DIDType, RuleState
+from rucio.tests.common import auth, did_name_generator, headers, rse_name_generator
 
 
 class TestSubscriptionCoreApi:
     projects = ['data12_900GeV', 'data12_8TeV', 'data13_900GeV', 'data13_8TeV']
     pattern1 = r'(_tid|physics_(Muons|JetTauEtmiss|Egamma)\..*\.ESD|express_express(?!.*NTUP|.*\.ESD|.*RAW)|(physics|express)(?!.*NTUP).* \
                 \.x|physics_WarmStart|calibration(?!_PixelBeam.merge.(NTUP_IDVTXLUMI|AOD))|merge.HIST|NTUP_MUONCALIB|NTUP_TRIG)'
     activity = get_schema_value('ACTIVITY')['enum'][0]
@@ -49,26 +46,26 @@
         rse2, _ = rse_factory.make_mock_rse()
         rse_expression = '%s|%s' % (rse1, rse2)
         subscription_name = uuid()
         with pytest.raises(InvalidObject):
             add_subscription(name=subscription_name,
                              account='root',
                              filter_={'project': self.projects, 'datatype': ['AOD', ], 'excluded_pattern': self.pattern1, 'account': ['tier0', ]},
-                             replication_rules=[{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': 'noactivity'}],
+                             replication_rules=[{'rse_expression': rse_expression, 'copies': 2, 'activity': 'noactivity'}],
                              lifetime=100000,
                              retroactive=False,
                              dry_run=False,
                              comments='This is a comment',
                              issuer='root',
                              vo=vo)
 
         sub_id = add_subscription(name=subscription_name,
                                   account='root',
                                   filter_={'project': self.projects, 'datatype': ['AOD', ], 'excluded_pattern': self.pattern1, 'account': ['tier0', ]},
-                                  replication_rules=[{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}],
+                                  replication_rules=[{'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}],
                                   lifetime=100000,
                                   retroactive=False,
                                   dry_run=False,
                                   comments='This is a comment',
                                   issuer='root',
                                   vo=vo)
 
@@ -94,15 +91,15 @@
         rse1, _ = rse_factory.make_mock_rse()
         rse2, _ = rse_factory.make_mock_rse()
         rse_expression = '%s|%s' % (rse1, rse2)
         subscription_name = uuid()
         subscription_id = add_subscription(name=subscription_name,
                                            account='root',
                                            filter_={'project': self.projects, 'datatype': ['AOD', ], 'excluded_pattern': self.pattern1, 'account': ['tier0', ]},
-                                           replication_rules=[{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}],
+                                           replication_rules=[{'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}],
                                            lifetime=100000,
                                            retroactive=False,
                                            dry_run=False,
                                            comments='This is a comment',
                                            issuer='root',
                                            vo=vo)
 
@@ -117,15 +114,15 @@
         rse_expression = '%s|%s' % (rse1, rse2)
 
         def genkwargs(rse_expression):
             kwargs = {
                 'name': subscription_name,
                 'account': 'root',
                 'filter_': {'project': self.projects, 'datatype': ['AOD', ], 'excluded_pattern': self.pattern1, 'account': ['tier0', ]},
-                'replication_rules': [{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}],
+                'replication_rules': [{'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}],
                 'lifetime': 100000,
                 'retroactive': 0,
                 'dry_run': 0,
                 'comments': 'This is a comment',
                 'issuer': 'root'
             }
             kwargs.update({'vo': vo})
@@ -158,15 +155,15 @@
         add_did(scope=tmp_scope, name=dsn,
                 did_type=DIDType.DATASET, account=root_account)
 
         subscription_name = uuid()
         subid = add_subscription(name=subscription_name,
                                  account='root',
                                  filter_={'account': ['root', ], 'scope': [tmp_scope.external, ]},
-                                 replication_rules=[{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}],
+                                 replication_rules=[{'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}],
                                  lifetime=100000,
                                  retroactive=False,
                                  dry_run=False,
                                  comments='This is a comment',
                                  issuer='root',
                                  vo=vo)
 
@@ -185,15 +182,15 @@
     rse1, _ = rse_factory.make_mock_rse()
     rse2, _ = rse_factory.make_mock_rse()
     rse_expression = '%s|%s' % (rse1, rse2)
     projects = ['data12_900GeV', 'data12_8TeV', 'data13_900GeV', 'data13_8TeV']
     pattern1 = r'(_tid|physics_(Muons|JetTauEtmiss|Egamma)\..*\.ESD|express_express(?!.*NTUP|.*\.ESD|.*RAW)|(physics|express)(?!.*NTUP).* \
                  \.x|physics_WarmStart|calibration(?!_PixelBeam.merge.(NTUP_IDVTXLUMI|AOD))|merge.HIST|NTUP_MUONCALIB|NTUP_TRIG)'
     data = {'options': {'filter': {'project': projects, 'datatype': ['AOD', ], 'excluded_pattern': pattern1, 'account': ['tier0', ]},
-                        'replication_rules': [{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': activity}],
+                        'replication_rules': [{'rse_expression': rse_expression, 'copies': 2, 'activity': activity}],
                         'lifetime': 100000, 'retroactive': 0, 'dry_run': 0, 'comments': 'blahblah'}}
     response = rest_client.post('/subscriptions/root/' + subscription_name, headers=headers(auth(auth_token)), json=data)
     assert response.status_code == 201
 
     data = {'options': {'filter': {'project': ['toto', ]}}}
     response = rest_client.put('/subscriptions/root/' + subscription_name, headers=headers(auth(auth_token)), json=data)
     assert response.status_code == 201
@@ -210,15 +207,15 @@
     rse1, _ = rse_factory.make_mock_rse()
     rse2, _ = rse_factory.make_mock_rse()
     rse_expression = '%s|%s' % (rse1, rse2)
     projects = ['data12_900GeV', 'data12_8TeV', 'data13_900GeV', 'data13_8TeV']
     pattern1 = r'(_tid|physics_(Muons|JetTauEtmiss|Egamma)\..*\.ESD|express_express(?!.*NTUP|.*\.ESD|.*RAW)|(physics|express)(?!.*NTUP).* \
                  \.x|physics_WarmStart|calibration(?!_PixelBeam.merge.(NTUP_IDVTXLUMI|AOD))|merge.HIST|NTUP_MUONCALIB|NTUP_TRIG)'
     data = {'options': {'filter': {'project': projects, 'datatype': ['AOD', ], 'excluded_pattern': pattern1, 'account': ['tier0', ]},
-                        'replication_rules': [{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': activity}],
+                        'replication_rules': [{'rse_expression': rse_expression, 'copies': 2, 'activity': activity}],
                         'lifetime': 100000, 'retroactive': 0, 'dry_run': 0, 'comments': 'blahblah'}}
     response = rest_client.post('/subscriptions/root/' + subscription_name, headers=headers(auth(auth_token)), json=data)
     assert response.status_code == 201
 
     subscription_id = response.get_data(as_text=True)
     response = rest_client.get('/subscriptions/Id/' + subscription_id, headers=headers(auth(auth_token)))
     assert response.status_code == 200
@@ -232,15 +229,15 @@
     rse1, _ = rse_factory.make_mock_rse()
     rse2, _ = rse_factory.make_mock_rse()
     rse_expression = '%s|%s' % (rse1, rse2)
     projects = ['data12_900GeV', 'data12_8TeV', 'data13_900GeV', 'data13_8TeV']
     pattern1 = r'(_tid|physics_(Muons|JetTauEtmiss|Egamma)\..*\.ESD|express_express(?!.*NTUP|.*\.ESD|.*RAW)|(physics|express)(?!.*NTUP).* \
                  \.x|physics_WarmStart|calibration(?!_PixelBeam.merge.(NTUP_IDVTXLUMI|AOD))|merge.HIST|NTUP_MUONCALIB|NTUP_TRIG)'
     data = {'options': {'name': subscription_name, 'filter': {'project': projects, 'datatype': ['AOD', ], 'excluded_pattern': pattern1, 'account': ['tier0', ]},
-                        'replication_rules': [{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': activity}],
+                        'replication_rules': [{'rse_expression': rse_expression, 'copies': 2, 'activity': activity}],
                         'lifetime': 100000, 'retroactive': 0, 'dry_run': 0, 'comments': 'We are the knights who say Ni !'}}
     response = rest_client.post('/subscriptions/root/' + subscription_name, headers=headers(auth(auth_token)), json=data)
     assert response.status_code == 201
 
     response = rest_client.post('/subscriptions/root/' + subscription_name, headers=headers(auth(auth_token)), json=data)
     assert response.status_code == 409
     assert response.headers.get('ExceptionClass') == 'SubscriptionDuplicate'
@@ -273,15 +270,15 @@
     add_did(scope=tmp_scope, name=dsn,
             did_type=DIDType.DATASET, account=root_account)
 
     subscription_name = uuid()
     subid = add_subscription(name=subscription_name,
                              account='root',
                              filter_={'account': ['root', ], 'scope': [tmp_scope.external, ]},
-                             replication_rules=[{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': activity}],
+                             replication_rules=[{'rse_expression': rse_expression, 'copies': 2, 'activity': activity}],
                              lifetime=100000,
                              retroactive=False,
                              dry_run=False,
                              comments='We want a shrubbery',
                              issuer='root',
                              vo=vo)
 
@@ -314,17 +311,17 @@
         """ SUBSCRIPTION (CLIENT): Test the creation of a new subscription, update it, list it """
         subscription_name = uuid()
         rse1, _ = rse_factory.make_mock_rse()
         rse2, _ = rse_factory.make_mock_rse()
         rse_expression = '%s|%s' % (rse1, rse2)
         with pytest.raises(InvalidObject):
             subid = rucio_client.add_subscription(name=subscription_name, account='root', filter_={'project': self.projects, 'datatype': ['AOD', ], 'excluded_pattern': self.pattern1, 'account': ['tier0', ]},
-                                                  replication_rules=[{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': 'noactivity'}], lifetime=100000, retroactive=False, dry_run=False, comments='Ni ! Ni!')
+                                                  replication_rules=[{'rse_expression': rse_expression, 'copies': 2, 'activity': 'noactivity'}], lifetime=100000, retroactive=False, dry_run=False, comments='Ni ! Ni!')
         subid = rucio_client.add_subscription(name=subscription_name, account='root', filter_={'project': self.projects, 'datatype': ['AOD', ], 'excluded_pattern': self.pattern1, 'account': ['tier0', ]},
-                                              replication_rules=[{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}], lifetime=100000, retroactive=False, dry_run=False, comments='Ni ! Ni!')
+                                              replication_rules=[{'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}], lifetime=100000, retroactive=False, dry_run=False, comments='Ni ! Ni!')
         result = [sub['id'] for sub in list_subscriptions(name=subscription_name, account='root', vo=vo)]
         assert subid == result[0]
         with pytest.raises(TypeError):
             result = rucio_client.update_subscription(name=subscription_name, account='root', filter_='toto')
         result = rucio_client.update_subscription(name=subscription_name, account='root', filter_={'project': ['toto', ]})
         assert result
         result = list_subscriptions(name=subscription_name, account='root', vo=vo)
@@ -337,19 +334,19 @@
     def test_create_existing_subscription(self, rse_factory, rucio_client):
         """ SUBSCRIPTION (CLIENT): Test the creation of a existing subscription """
         subscription_name = uuid()
         rse1, _ = rse_factory.make_mock_rse()
         rse2, _ = rse_factory.make_mock_rse()
         rse_expression = '%s|%s' % (rse1, rse2)
         result = rucio_client.add_subscription(name=subscription_name, account='root', filter_={'project': self.projects, 'datatype': ['AOD', ], 'excluded_pattern': self.pattern1, 'account': ['tier0', ]},
-                                               replication_rules=[{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}], lifetime=100000, retroactive=False, dry_run=False, comments='Ni ! Ni!')
+                                               replication_rules=[{'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}], lifetime=100000, retroactive=False, dry_run=False, comments='Ni ! Ni!')
         assert result
         with pytest.raises(SubscriptionDuplicate):
             rucio_client.add_subscription(name=subscription_name, account='root', filter_={'project': self.projects, 'datatype': ['AOD', ], 'excluded_pattern': self.pattern1, 'account': ['tier0', ]},
-                                          replication_rules=[{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}], lifetime=100000, retroactive=False, dry_run=False, comments='Ni ! Ni!')
+                                          replication_rules=[{'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}], lifetime=100000, retroactive=False, dry_run=False, comments='Ni ! Ni!')
 
     def test_update_nonexisting_subscription(self, rucio_client):
         """ SUBSCRIPTION (CLIENT): Test the update of a non-existing subscription """
         subscription_name = uuid()
         with pytest.raises(SubscriptionNotFound):
             rucio_client.update_subscription(name=subscription_name, filter_={'project': ['toto', ]})
 
@@ -358,26 +355,26 @@
         subscription_name = uuid()
         rse1, _ = rse_factory.make_mock_rse()
         rse2, _ = rse_factory.make_mock_rse()
         rse_expression = '%s|%s' % (rse1, rse2)
         account_name = uuid()[:10]
         add_account(InternalAccount(account_name, vo=vo), AccountType.USER, 'rucio@email.com')
         subid = rucio_client.add_subscription(name=subscription_name, account=account_name, filter_={'project': self.projects, 'datatype': ['AOD', ], 'excluded_pattern': self.pattern1, 'account': ['tier0', ]},
-                                              replication_rules=[{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}], lifetime=100000, retroactive=False, dry_run=False, comments='Ni ! Ni!')
+                                              replication_rules=[{'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}], lifetime=100000, retroactive=False, dry_run=False, comments='Ni ! Ni!')
         result = [sub['id'] for sub in rucio_client.list_subscriptions(account=account_name)]
         assert subid == result[0]
 
     def test_create_and_list_subscription_by_name(self, rse_factory, rucio_client):
         """ SUBSCRIPTION (CLIENT): Test retrieval of subscriptions for an account """
         subscription_name = uuid()
         rse1, _ = rse_factory.make_mock_rse()
         rse2, _ = rse_factory.make_mock_rse()
         rse_expression = '%s|%s' % (rse1, rse2)
         subid = rucio_client.add_subscription(name=subscription_name, account='root', filter_={'project': self.projects, 'datatype': ['AOD', ], 'excluded_pattern': self.pattern1, 'account': ['tier0', ]},
-                                              replication_rules=[{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}], lifetime=100000, retroactive=False, dry_run=False, comments='Ni ! Ni!')
+                                              replication_rules=[{'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}], lifetime=100000, retroactive=False, dry_run=False, comments='Ni ! Ni!')
         result = [sub['id'] for sub in rucio_client.list_subscriptions(name=subscription_name)]
         assert subid == result[0]
 
     @pytest.mark.noparallel(reason='runs transmogrifier. Cannot be run at the same time with other tests running it')
     def test_run_transmogrifier(self, vo, rse_factory, rucio_client, root_account):
         """ SUBSCRIPTION (DAEMON): Test the transmogrifier and the split_rule mode """
         new_dids = [did for did in list_new_dids(did_type=None, thread=None, total_threads=None, chunk_size=100000, session=None)]
@@ -391,15 +388,15 @@
         add_scope(tmp_scope, root_account)
         subscription_name = uuid()
         dsn_prefix = did_name_generator('dataset')
         dsn = '%sdataset-%s' % (dsn_prefix, uuid())
         add_did(scope=tmp_scope, name=dsn, did_type=DIDType.DATASET, account=root_account)
 
         subid = rucio_client.add_subscription(name=subscription_name, account='root', filter_={'scope': [tmp_scope.external, ], 'pattern': '%s.*' % dsn_prefix, 'split_rule': True},
-                                              replication_rules=[{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}],
+                                              replication_rules=[{'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}],
                                               lifetime=None, retroactive=False, dry_run=False, comments='Ni ! Ni!', priority=1)
         run(threads=1, bulk=1000000, once=True)
         rules = [rule for rule in rucio_client.list_did_rules(scope=tmp_scope.external, name=dsn) if str(rule['subscription_id']) == str(subid)]
         assert len(rules) == 2
         set_new_dids([{'scope': tmp_scope, 'name': dsn}, ], 1)
         run(threads=1, bulk=1000000, once=True)
         rules = [rule for rule in rucio_client.list_did_rules(scope=tmp_scope.external, name=dsn) if str(rule['subscription_id']) == str(subid)]
@@ -418,15 +415,15 @@
         add_scope(tmp_scope, root_account)
         subscription_name = uuid()
         dsn_prefix = did_name_generator('dataset')
         dsn = '%sdataset-%s' % (dsn_prefix, uuid())
         add_did(scope=tmp_scope, name=dsn, did_type=DIDType.DATASET, account=root_account)
 
         subid = rucio_client.add_subscription(name=subscription_name, account='root', filter_={'scope': [tmp_scope.external, ], 'pattern': '%s.*' % dsn_prefix, 'split_rule': True, 'did_type': ['DATASET', ]},
-                                              replication_rules=[{'lifetime': 86400, 'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}],
+                                              replication_rules=[{'rse_expression': rse_expression, 'copies': 2, 'activity': self.activity}],
                                               lifetime=None, retroactive=False, dry_run=False, comments='Ni ! Ni!', priority=1)
         run(threads=1, bulk=1000000, once=True)
         rules = [rule for rule in rucio_client.list_did_rules(scope=tmp_scope.external, name=dsn) if str(rule['subscription_id']) == str(subid)]
         assert len(rules) == 2
         set_new_dids([{'scope': tmp_scope, 'name': dsn}, ], 1)
         run(threads=1, bulk=1000000, once=True)
         rules = [rule for rule in rucio_client.list_did_rules(scope=tmp_scope.external, name=dsn) if str(rule['subscription_id']) == str(subid)]
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_throttler.py` & `rucio-webui-34.1.0/tests/test_throttler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -15,25 +14,32 @@
 
 from datetime import datetime, timedelta
 
 import pytest
 from sqlalchemy import delete
 
 from rucio.common.utils import generate_uuid
-from rucio.core.did import attach_dids, add_did
+from rucio.core.did import add_did, attach_dids
 from rucio.core.distance import add_distance
 from rucio.core.replica import add_replica
-from rucio.core.request import (queue_requests, get_request_by_did, release_waiting_requests_per_deadline,
-                                release_all_waiting_requests, release_waiting_requests_fifo, release_waiting_requests_grouped_fifo,
-                                release_waiting_requests_per_free_volume, delete_transfer_limit)
-from rucio.daemons.conveyor.throttler import throttler
+from rucio.core.request import (
+    delete_transfer_limit,
+    get_request_by_did,
+    queue_requests,
+    release_all_waiting_requests,
+    release_waiting_requests_fifo,
+    release_waiting_requests_grouped_fifo,
+    release_waiting_requests_per_deadline,
+    release_waiting_requests_per_free_volume,
+)
 from rucio.daemons.conveyor.preparer import preparer
+from rucio.daemons.conveyor.throttler import throttler
 from rucio.db.sqla import models
-from rucio.db.sqla.session import transactional_session, get_session
-from rucio.db.sqla.constants import DIDType, RequestType, RequestState, TransferLimitDirection
+from rucio.db.sqla.constants import DIDType, RequestState, RequestType, TransferLimitDirection
+from rucio.db.sqla.session import get_session, transactional_session
 from rucio.tests.common import skiplimitedsql
 
 
 @pytest.fixture
 def transfer_limit_factory():
     """
     Thin wrapper around request_core.set_transfer_limit, which cleans up
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_tpc.py` & `rucio-webui-34.1.0/tests/test_tpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import time
 import datetime
-import pytest
 import hashlib
 import re
+import time
 
+import pytest
+
+from rucio.client.rseclient import RSEClient
+from rucio.client.ruleclient import RuleClient
+from rucio.common.utils import generate_uuid, run_cmd_process
 from rucio.core.request import get_request_by_did, list_and_mark_transfer_requests_and_source_replicas
+from rucio.core.rule import add_rule
 from rucio.core.topology import Topology
 from rucio.core.transfer import ProtocolFactory
-from rucio.core.rule import add_rule
-from rucio.common.utils import generate_uuid
-from rucio.daemons.judge.evaluator import re_evaluator
-from rucio.daemons.conveyor import submitter, poller, finisher
+from rucio.daemons.conveyor import finisher, poller, submitter
 from rucio.daemons.conveyor.common import build_transfer_paths
-from rucio.client.rseclient import RSEClient
-from rucio.client.ruleclient import RuleClient
-from rucio.common.utils import run_cmd_process
+from rucio.daemons.judge.evaluator import re_evaluator
 
 MAX_POLL_WAIT_SECONDS = 60
 
 
 @pytest.fixture
 def rse_client():
     return RSEClient()
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_trace.py` & `rucio-webui-34.1.0/tests/test_trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -10,23 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
+import json
+import logging
 import time
 import uuid
-import logging
+
 import pytest
-import json
+
+from rucio.common.exception import InvalidObject
 from rucio.common.schema.generic import IPv4orIPv6
 from rucio.core.trace import SCHEMAS, validate_schema
-from rucio.common.exception import InvalidObject
-
 
 LOGGER = logging.getLogger(__name__)
 
 
 def test_submit_trace(rest_client):
     """ TRACE (REST): submit a trace via POST """
     payload = {'uuid': str(uuid.uuid4()),  # str, because not JSON serializable
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_transfer.py` & `rucio-webui-34.1.0/tests/test_transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pytest
-from concurrent.futures import ThreadPoolExecutor
 import datetime
+from concurrent.futures import ThreadPoolExecutor
+
+import pytest
 
 from rucio.common.exception import NoDistance
+from rucio.common.utils import generate_uuid
+from rucio.core import request as request_core
+from rucio.core import rse as rse_core
+from rucio.core import rule as rule_core
 from rucio.core.distance import add_distance
 from rucio.core.replica import add_replicas
 from rucio.core.request import list_and_mark_transfer_requests_and_source_replicas
-from rucio.core.transfer import build_transfer_paths, ProtocolFactory
-from rucio.core.topology import get_hops, Topology
-from rucio.core import rule as rule_core
-from rucio.core import request as request_core
-from rucio.core import rse as rse_core
+from rucio.core.topology import Topology, get_hops
+from rucio.core.transfer import ProtocolFactory, build_transfer_paths
+from rucio.daemons.conveyor.common import assign_paths_to_transfertool_and_create_hops, pick_and_prepare_submission_path
 from rucio.db.sqla import models
-from rucio.db.sqla.constants import RSEType, RequestState
+from rucio.db.sqla.constants import RequestState, RSEType
 from rucio.db.sqla.session import get_session
-from rucio.common.utils import generate_uuid
-from rucio.daemons.conveyor.common import assign_paths_to_transfertool_and_create_hops, pick_and_prepare_submission_path
 
 
 def _prepare_submission(rses):
     topology = Topology().configure_multihop()
     requests_with_sources = list_and_mark_transfer_requests_and_source_replicas(rse_collection=topology, rses=rses)
     pick_and_prepare_submission_path(requests_with_sources, topology=topology, protocol_factory=ProtocolFactory(), default_tombstone_delay=0)
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_transfer_plugins.py` & `rucio-webui-34.1.0/tests/test_transfer_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pytest
 import logging
 
-from rucio.transfertool.fts3 import FTS3Transfertool, build_job_params
-from rucio.core.topology import Topology
-from rucio.core.transfer import ProtocolFactory, build_transfer_paths
-from rucio.core.request import list_and_mark_transfer_requests_and_source_replicas
-
-from rucio.db.sqla.session import get_session
-from rucio.transfertool.fts3_plugins import FTS3TapeMetadataPlugin
+import pytest
 
 from rucio.core import distance as distance_core
 from rucio.core import replica as replica_core
 from rucio.core import rule as rule_core
-
+from rucio.core.request import list_and_mark_transfer_requests_and_source_replicas
+from rucio.core.topology import Topology
+from rucio.core.transfer import ProtocolFactory, build_transfer_paths
+from rucio.db.sqla.session import get_session
+from rucio.transfertool.fts3 import FTS3Transfertool, build_job_params
+from rucio.transfertool.fts3_plugins import FTS3TapeMetadataPlugin
 
 mock_session = get_session()
 
 MAX_POLL_WAIT_SECONDS = 60
 TEST_FTS_HOST = "https://fts:8446"
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_undertaker.py` & `rucio-webui-34.1.0/tests/test_undertaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -17,22 +16,22 @@
 from logging import getLogger
 
 import pytest
 
 from rucio.common.policy import get_policy
 from rucio.common.types import InternalScope
 from rucio.core.account_limit import set_local_account_limit
-from rucio.core.did import add_dids, attach_dids, list_expired_dids, get_did, set_metadata
+from rucio.core.did import add_dids, attach_dids, get_did, list_expired_dids, set_metadata
 from rucio.core.replica import add_replicas, get_replica
 from rucio.core.rse import add_rse
 from rucio.core.rule import add_rules, list_rules
 from rucio.daemons.judge.cleaner import rule_cleaner
 from rucio.daemons.undertaker.undertaker import undertaker
 from rucio.db.sqla.util import json_implemented
-from rucio.tests.common import rse_name_generator, did_name_generator
+from rucio.tests.common import did_name_generator, rse_name_generator
 
 LOG = getLogger(__name__)
 
 
 @pytest.mark.dirty
 @pytest.mark.noparallel(reason='uses pre-defined rses; runs undertaker, which impacts other tests')
 class TestUndertaker:
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_upload.py` & `rucio-webui-34.1.0/tests/test_upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -12,19 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import logging
 import os
-import pytest
 import shutil
 from tempfile import TemporaryDirectory
 from unittest.mock import patch
 
+import pytest
+
 from rucio.client.uploadclient import UploadClient
 from rucio.common.config import config_add_section, config_set
 from rucio.common.exception import InputValidationError, NoFilesUploaded, NotAllFilesUploaded
 from rucio.common.utils import adler32, generate_uuid
 from rucio.core.rse import add_protocol, add_rse_attribute
```

### Comparing `rucio-webui-34.0.0rc2/tests/test_utils.py` & `rucio-webui-34.1.0/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright European Organization for Nuclear Research (CERN) since 2012
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -17,16 +16,16 @@
 import logging
 import os
 from re import match
 
 import pytest
 
 from rucio.common.exception import InvalidType
-from rucio.common.utils import md5, adler32, parse_did_filter_from_string, Availability, retrying, bittorrent_v2_merkle_sha256
 from rucio.common.logging import formatted_logger
+from rucio.common.utils import Availability, adler32, bittorrent_v2_merkle_sha256, md5, parse_did_filter_from_string, retrying
 
 
 class TestUtils:
     """UTILS (COMMON): test utilisty functions"""
 
     def test_utils_md5(self, file_factory):
         """(COMMON/UTILS): test calculating MD5 of a file"""
```

