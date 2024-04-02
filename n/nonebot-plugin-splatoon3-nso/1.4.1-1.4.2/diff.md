# Comparing `tmp/nonebot_plugin_splatoon3_nso-1.4.1.tar.gz` & `tmp/nonebot_plugin_splatoon3_nso-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_splatoon3_nso-1.4.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_splatoon3_nso-1.4.2.tar", max compression
```

## Comparing `nonebot_plugin_splatoon3_nso-1.4.1.tar` & `nonebot_plugin_splatoon3_nso-1.4.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1066 2024-03-28 14:53:28.834016 nonebot_plugin_splatoon3_nso-1.4.1/LICENSE
--rw-r--r--   0        0        0    12316 2024-03-28 14:53:28.834016 nonebot_plugin_splatoon3_nso-1.4.1/README.md
--rw-r--r--   0        0        0     5589 2024-03-28 14:53:28.834016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/__init__.py
--rw-r--r--   0        0        0     2817 2024-03-28 14:53:28.834016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/config.py
--rw-r--r--   0        0        0        0 2024-03-28 14:53:28.834016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/data/__init__.py
--rw-r--r--   0        0        0    18107 2024-03-28 14:53:28.834016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/data/data_source.py
--rw-r--r--   0        0        0     7111 2024-03-28 14:53:28.834016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/data/db_sqlite.py
--rw-r--r--   0        0        0     5015 2024-03-28 14:53:28.834016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/data/transfer.py
--rw-r--r--   0        0        0     3721 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/data/utils.py
--rw-r--r--   0        0        0      439 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/__init__.py
--rw-r--r--   0        0        0     4095 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/admin.py
--rw-r--r--   0        0        0    16296 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/b_or_c_tools.py
--rw-r--r--   0        0        0    19576 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/battle.py
--rw-r--r--   0        0        0     7951 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/coop.py
--rw-r--r--   0        0        0     5203 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/__init__.py
--rw-r--r--   0        0        0     3613 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/else_cron.py
--rw-r--r--   0        0        0     3545 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/event_top.py
--rw-r--r--   0        0        0    11040 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/report.py
--rw-r--r--   0        0        0     9115 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/stat_ink.py
--rw-r--r--   0        0        0     2874 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/user_friends.py
--rw-r--r--   0        0        0      671 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/utils.py
--rw-r--r--   0        0        0     6460 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/x_player.py
--rw-r--r--   0        0        0     8260 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/history.py
--rw-r--r--   0        0        0    14441 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/last.py
--rw-r--r--   0        0        0    15462 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/login.py
--rw-r--r--   0        0        0    20889 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/my.py
--rw-r--r--   0        0        0    12902 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/push.py
--rw-r--r--   0        0        0     3433 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/qq_md.py
--rw-r--r--   0        0        0     7951 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/report.py
--rw-r--r--   0        0        0     2747 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/screenshot.py
--rw-r--r--   0        0        0    12992 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/send_msg.py
--rw-r--r--   0        0        0    10179 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/top.py
--rw-r--r--   0        0        0    10994 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/utils.py
--rw-r--r--   0        0        0    31357 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/i18n/en-GB.json
--rw-r--r--   0        0        0    36257 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/i18n/ja-JP.json
--rw-r--r--   0        0        0    34122 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/i18n/ko-KR.json
--rw-r--r--   0        0        0    30879 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/i18n/zh-CN.json
--rw-r--r--   0        0        0    31079 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/i18n/zh-TW.json
--rw-r--r--   0        0        0      708 2024-03-28 14:53:28.838016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/md.css
--rw-r--r--   0        0        0   461502 2024-03-28 14:53:28.842016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/sp3bot-login.gif
--rw-r--r--   0        0        0        0 2024-03-28 14:53:28.842016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/s3s/__init__.py
--rw-r--r--   0        0        0    25882 2024-03-28 14:53:28.842016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/s3s/iksm.py
--rw-r--r--   0        0        0     5301 2024-03-28 14:53:28.842016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/s3s/splatnet_image.py
--rw-r--r--   0        0        0    22564 2024-03-28 14:53:28.842016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/s3s/splatoon.py
--rw-r--r--   0        0        0     6299 2024-03-28 14:53:28.842016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/s3s/utils.py
--rw-r--r--   0        0        0     4077 2024-03-28 14:53:28.842016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/util.py
--rw-r--r--   0        0        0       61 2024-03-28 14:53:28.842016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/utils/__init__.py
--rw-r--r--   0        0        0     3448 2024-03-28 14:53:28.842016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/utils/bot.py
--rw-r--r--   0        0        0     6127 2024-03-28 14:53:28.842016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/utils/http.py
--rw-r--r--   0        0        0     4106 2024-03-28 14:53:28.842016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/utils/time.py
--rw-r--r--   0        0        0     1838 2024-03-28 14:53:28.842016 nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/utils/utils.py
--rw-r--r--   0        0        0      969 2024-03-28 14:53:28.842016 nonebot_plugin_splatoon3_nso-1.4.1/pyproject.toml
--rw-r--r--   0        0        0    13429 1970-01-01 00:00:00.000000 nonebot_plugin_splatoon3_nso-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/LICENSE
+-rw-r--r--   0        0        0    12316 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/README.md
+-rw-r--r--   0        0        0     5589 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/__init__.py
+-rw-r--r--   0        0        0     2817 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/config.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/__init__.py
+-rw-r--r--   0        0        0    18107 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/data_source.py
+-rw-r--r--   0        0        0     7111 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/db_sqlite.py
+-rw-r--r--   0        0        0     5015 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/transfer.py
+-rw-r--r--   0        0        0     3721 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/utils.py
+-rw-r--r--   0        0        0      439 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/__init__.py
+-rw-r--r--   0        0        0     4095 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/admin.py
+-rw-r--r--   0        0        0    16296 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/b_or_c_tools.py
+-rw-r--r--   0        0        0    19576 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/battle.py
+-rw-r--r--   0        0        0     7951 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/coop.py
+-rw-r--r--   0        0        0     5203 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/__init__.py
+-rw-r--r--   0        0        0     3613 2024-04-02 16:28:36.144620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/else_cron.py
+-rw-r--r--   0        0        0     3545 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/event_top.py
+-rw-r--r--   0        0        0    11040 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/report.py
+-rw-r--r--   0        0        0     9115 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/stat_ink.py
+-rw-r--r--   0        0        0     2874 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/user_friends.py
+-rw-r--r--   0        0        0      671 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/utils.py
+-rw-r--r--   0        0        0     6460 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/x_player.py
+-rw-r--r--   0        0        0     8411 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/history.py
+-rw-r--r--   0        0        0    14441 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/last.py
+-rw-r--r--   0        0        0    15462 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/login.py
+-rw-r--r--   0        0        0    21068 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/my.py
+-rw-r--r--   0        0        0    13044 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/push.py
+-rw-r--r--   0        0        0     3433 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/qq_md.py
+-rw-r--r--   0        0        0     7951 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/report.py
+-rw-r--r--   0        0        0     2747 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/screenshot.py
+-rw-r--r--   0        0        0    12992 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/send_msg.py
+-rw-r--r--   0        0        0    10179 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/top.py
+-rw-r--r--   0        0        0    10994 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/utils.py
+-rw-r--r--   0        0        0    31357 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/en-GB.json
+-rw-r--r--   0        0        0    36257 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/ja-JP.json
+-rw-r--r--   0        0        0    34122 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/ko-KR.json
+-rw-r--r--   0        0        0    30879 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/zh-CN.json
+-rw-r--r--   0        0        0    31079 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/zh-TW.json
+-rw-r--r--   0        0        0      708 2024-04-02 16:28:36.148620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/md.css
+-rw-r--r--   0        0        0   461502 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/sp3bot-login.gif
+-rw-r--r--   0        0        0        0 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/__init__.py
+-rw-r--r--   0        0        0    26214 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/iksm.py
+-rw-r--r--   0        0        0     5301 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/splatnet_image.py
+-rw-r--r--   0        0        0    22564 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/splatoon.py
+-rw-r--r--   0        0        0     6299 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/utils.py
+-rw-r--r--   0        0        0     4077 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/util.py
+-rw-r--r--   0        0        0       61 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/__init__.py
+-rw-r--r--   0        0        0     3448 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/bot.py
+-rw-r--r--   0        0        0     6127 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/http.py
+-rw-r--r--   0        0        0     4106 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/time.py
+-rw-r--r--   0        0        0     1838 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/utils.py
+-rw-r--r--   0        0        0      969 2024-04-02 16:28:36.152620 nonebot_plugin_splatoon3_nso-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0    13429 1970-01-01 00:00:00.000000 nonebot_plugin_splatoon3_nso-1.4.2/PKG-INFO
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/LICENSE` & `nonebot_plugin_splatoon3_nso-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/README.md` & `nonebot_plugin_splatoon3_nso-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/__init__.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/config.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/data/data_source.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/data/db_sqlite.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/db_sqlite.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/data/transfer.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/transfer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/data/utils.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/data/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/admin.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/admin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/b_or_c_tools.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/b_or_c_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
 async def get_top_user(name, icon, player_code):
     """获取top玩家md信息"""
     top_user = model_get_top_player(player_code)
     if not top_user:
         return name, icon, 0
 
-    _x = 'x' if ':6:' in top_user.top_type else 'X'
+    _x = 'x' if ':7:' in top_user.top_type else 'X'
     if '-a:' in top_user.top_type:
         color = "#fc0390"
     else:
         color = "red"
     name = name.replace('`', '&#96;').replace('|', '&#124;')
     name = name.strip() + f'</br><span style="color:{color}">{_x}{top_user.rank}({top_user.power})</span>'
     # 武器图片
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/battle.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/battle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/coop.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/coop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/__init__.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/else_cron.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/else_cron.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/event_top.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/event_top.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/report.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/report.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/stat_ink.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/stat_ink.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/user_friends.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/user_friends.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/utils.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/cron/x_player.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/cron/x_player.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/history.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     elif _type == "open":
         _type_name = "(组排)"
     elif _type == "fest":
         _type_name = ""
 
     msg += f'''
 |  |   ||  ||||||||||
-| --: |--:|--:|--:|--:|--:|--:|--:|--:|--:|--:|--:|--|
+| --: |--:|--:|--:|--:|--:|--:|--:|--:|--:|--:|--:|:---------|
 |胜负|分数变动{_type_name}|当前分数{_type_name}|武器|总|杀+助|死亡|kd|大招|涂地|耗时|比分|地图|
 '''
 
     dict_p = {}
     last_power = 0
     for b in battle_lst[::-1]:
         _id = b['id']
@@ -213,11 +213,18 @@
     re = p['result']
     if not re:
         re = {"kill": 0, "death": 99, "assist": 0, "special": 0}
     ak = re['kill']
     k = re['kill'] - re['assist']
     k_str = f'{k}+{re["assist"]}'
     d = re['death']
-    ration = k / d if d else 99
+    # 避免除数和被除数为0的情况
+    if k != 0:
+        if d == 0:
+            ration = k / 1
+        else:
+            ration = k / d
+    else:
+        ration = 0
 
     t = f"{ak:>2}|{k_str:>5}k| {d:>2}d|{ration:>4.1f}|{re['special']:>3}sp| {p['paint']:>4}p "
     return t
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/last.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/last.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/login.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/my.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/my.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import unicodedata
 from nonebot import on_keyword
 
 from .send_msg import bot_send
 from .utils import _check_session_handler
 from ..data.data_source import dict_get_or_set_user_info, model_get_temp_image_path, model_get_or_set_user, \
-    model_get_power_rank, model_set_user_friend, model_get_another_account_user, global_user_info_dict
+    model_get_power_rank, model_set_user_friend, model_get_another_account_user, global_user_info_dict, model_get_all_top_all
 from ..data.utils import GlobalUserInfo
 from ..s3s.splatoon import Splatoon
 from ..utils import get_msg_id
 from ..utils.bot import *
 
 
 @on_command("me", priority=10, block=True).handle(parameterless=[Depends(_check_session_handler)])
@@ -169,14 +169,17 @@
 开放 | {_open}
 首次游玩 | {s_time:%Y-%m-%d %H:%M:%S} +08:00
 当前时间 | {c_time:%Y-%m-%d %H:%M:%S} +08:00
 {x_msg}
 {coop_msg}
 |||
 """
+    top_res = model_get_all_top_all(user.game_sp_id)
+    if top_res:
+        msg += f"上榜记录 | {len(top_res)}次 &nbsp;&nbsp; /top 查询排行榜\n"
     return msg
 
 
 @on_command("friends", aliases={'friend', 'fr'}, priority=10, block=True).handle(
     parameterless=[Depends(_check_session_handler)])
 async def friends(bot: Bot, event: Event):
     platform = bot.adapter.get_name()
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/push.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/push.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     logger.info(f"add push_job {job_id}")
     job_data = {
         'platform': platform,
         'user_id': user_id,
         'msg_id': msg_id,
         'this_push_cnt': 0,
         'error_push_cnt': 0,
+        'match_push_cnt': 0,
         'game_name': user.game_name or "",
         'job_id': job_id,
         'last_battle_id': "",
         'channel_id': channel_id,
         'last_channel_msg_id': "",
         'push_interval': push_interval,
         'push_statistics': PushStatistics(),
@@ -221,15 +222,15 @@
                 # 关闭定时，更新push状态，发送统计
                 dict_get_or_set_user_info(platform, user_id, push=0)
                 msg = 'No game record for 20 minutes, stop push.'
 
                 # 获取统计数据
                 st_msg, push_time_minute = close_push(platform, user_id)
                 if isinstance(bot, All_BOT):
-                    msg = f"20分钟内没有游戏记录，停止推送，本次推送持续 {push_time_minute}分钟\n"
+                    msg = f"20分钟内没有游戏记录，停止推送，本次推送持续 {push_time_minute}分钟, {job_data.get('match_push_cnt') or 0}次对局\n"
                     if not user.stat_key and user.push_cnt <= 10:
                         msg += "/set_stat_key 可保存数据到 stat.ink\n(App最多可查看最近50*5场对战和50场打工,该网站可记录全部对战或打工,也可用于武器/地图/模式/胜率的战绩分析)\n"
                 msg += st_msg
 
                 logger.info(
                     f"push auto end,user：{msg_id:>3},gamer：{user.game_name:>7}, push {push_time_minute} minutes")
 
@@ -255,14 +256,16 @@
                 if job_data.get('last_channel_msg_id'):
                     await bot.delete_message(chat_id=r.chat.id, message_id=job_data['last_channel_msg_id'])
             message_id = r.message_id
             job_data.update({"last_channel_msg_id": message_id})
 
         # 连续error计数置0
         job_data.update({"error_push_cnt": 0})
+        # 比赛计数+1
+        job_data['match_push_cnt'] += 1
 
     except Exception as e:
         logger.warning(f'push_latest_battle error: {e}')
         error_push_cnt += 1
         job_data.update({"error_push_cnt": error_push_cnt})
         return
     finally:
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/qq_md.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/qq_md.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/report.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/report.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/screenshot.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/screenshot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/send_msg.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/send_msg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/top.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/top.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/handle/utils.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/handle/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/i18n/en-GB.json` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/en-GB.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/i18n/ja-JP.json` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/ja-JP.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/i18n/ko-KR.json` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/ko-KR.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/i18n/zh-CN.json` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/i18n/zh-TW.json` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/i18n/zh-TW.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/md.css` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/md.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/resource/sp3bot-login.gif` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/resource/sp3bot-login.gif`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/s3s/iksm.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/iksm.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import base64
 import hashlib
 import json
 import os
 import re
 import sys
 import urllib
+import random
 
 import httpx
 from bs4 import BeautifulSoup
 from nonebot import logger as nb_logger
 
 from .utils import SPLATNET3_URL
 from ..utils import BOT_VERSION, get_or_init_client, HttpReq, ReqClient
@@ -35,15 +36,20 @@
 class S3S:
     def __init__(self, platform, user_id, _type="normal"):
         self.req_client: ReqClient = get_or_init_client(platform, user_id, _type)
         self.r_user_id = ""  # 请求内部所使用的user_id,不是消息平台的user_id
         self.user_nickname = ""
         self.user_lang = "zh-CN"
         self.user_country = "JP"
-        self.f_gen_url = F_GEN_URL
+
+        # 两个f_api 负载均衡
+        f_url_lst = [F_GEN_URL, F_GEN_URL_2]
+        random.shuffle(f_url_lst)
+        self.f_gen_url = f_url_lst[0]
+
         self.logger = nb_logger
         if _type == "cron":
             self.logger = nb_logger.bind(cron=True)
 
     @staticmethod
     def get_nsoapp_version(f_gen_url=None):
         """Fetches the current Nintendo Switch Online app version from f API or the Apple App Store and sets it globally."""
@@ -510,38 +516,44 @@
         res = await self.call_f_api(access_token, step, f_gen_url, r_user_id,
                                     coral_user_id=coral_user_id)
         if isinstance(res, tuple):
             # 解析tuple
             f, uuid, timestamp = res
             return f, uuid, timestamp
         else:
+            # 判断重试时的对象名称以及f地址
             if self.f_gen_url == F_GEN_URL:
-                if not res:
-                    # 无响应结果
-                    self.logger.warning(f"F_GEN_URL no res，try F_GEN_URL_2 again")
-                elif isinstance(res, str):
-                    # 错误信息
-                    # 改为f_url_2并重新请求一次
-                    if "NetConnectError" in res:
-                        self.logger.warning(f"F_GEN_URL ConnectError，try F_GEN_URL_2 again")
-                    elif "NetConnectTimeout" in res:
-                        self.logger.warning(f"F_GEN_URL ConnectTimeout，try F_GEN_URL_2 again")
-                    else:
-                        self.logger.warning(f"F_GEN_URL res Error，try F_GEN_URL_2 again, Error:{res}")
-                self.f_gen_url = F_GEN_URL_2
-                res = await self.call_f_api(access_token, step, self.f_gen_url, r_user_id,
-                                            coral_user_id=coral_user_id)
-                if isinstance(res, tuple):
-                    # 解析tuple
-                    f, uuid, timestamp = res
-                    return f, uuid, timestamp
+                now_f_str = "F_URL"
+                next_f_str = "F_URL_2"
+                next_f_url = F_GEN_URL_2
+            else:
+                now_f_str = "F_URL_2"
+                next_f_str = "F_URL"
+                next_f_url = F_GEN_URL
+            if not res:
+                # 无响应结果
+                self.logger.warning(f"{now_f_str} no res，try {next_f_str} again")
+            elif isinstance(res, str):
+                # 错误信息
+                # 改为另一个f接口并重新请求一次
+                if "NetConnectError" in res:
+                    self.logger.warning(f"{now_f_str} ConnectError，try {next_f_str} again")
+                elif "NetConnectTimeout" in res:
+                    self.logger.warning(f"{now_f_str} ConnectTimeout，try {next_f_str} again")
                 else:
-                    self.logger.warning(f"F_GEN_URL2 Error: {res}")
-                    return None
+                    self.logger.warning(f"{now_f_str} res Error，try {next_f_str} again, Error:{res}")
+            self.f_gen_url = next_f_url
+            res = await self.call_f_api(access_token, step, self.f_gen_url, r_user_id,
+                                        coral_user_id=coral_user_id)
+            if isinstance(res, tuple):
+                # 解析tuple
+                f, uuid, timestamp = res
+                return f, uuid, timestamp
             else:
+                self.logger.warning(f"{next_f_str} Both Error: {res}")
                 return None
 
     async def call_f_api(self, access_token, step, f_gen_url, r_user_id, coral_user_id=None):
         """Passes naIdToken & user ID to f generation API (default: imink) & fetches response (f token, UUID, timestamp)."""
 
         api_head = {}
         api_body = {}
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/s3s/splatnet_image.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/splatnet_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/s3s/splatoon.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/splatoon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/s3s/utils.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/s3s/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/util.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/utils/bot.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/utils/http.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/http.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/utils/time.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/nonebot_plugin_splatoon3_nso/utils/utils.py` & `nonebot_plugin_splatoon3_nso-1.4.2/nonebot_plugin_splatoon3_nso/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-BOT_VERSION = "2.6.1"
+BOT_VERSION = "2.6.2"
 DIR_RESOURCE = f"{os.path.abspath(os.path.join(__file__, os.pardir, os.pardir))}/resource"
 plugin_release_time = "2024-01-30 02:35:58"  # 预留  2.0.0重构版nso插件发布时间，预计发布时对全部用户先显示一周，之后再判断用户创建时间
 
 
 def multiple_replace(text, _dict):
     """批量替换文本"""
     for key in _dict:
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/pyproject.toml` & `nonebot_plugin_splatoon3_nso-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-splatoon3-nso"
-version = "1.4.1"
+version = "1.4.2"
 description = "一个基于nonebot2框架的splatoon3游戏nso数据查询插件"
 authors = ["cypas <ayano05@outlook.com>"]
 readme = "README.md"
 packages = [{include = "nonebot_plugin_splatoon3_nso"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nonebot_plugin_splatoon3_nso-1.4.1/PKG-INFO` & `nonebot_plugin_splatoon3_nso-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-splatoon3-nso
-Version: 1.4.1
+Version: 1.4.2
 Summary: 一个基于nonebot2框架的splatoon3游戏nso数据查询插件
 Author: cypas
 Author-email: ayano05@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-splatoon3-nso Version: 1.4.1
+Metadata-Version: 2.1 Name: nonebot-plugin-splatoon3-nso Version: 1.4.2
 Summary: ä¸ä¸ªåºäºnonebot2æ¡æ¶çsplatoon3æ¸¸ænsoæ°æ®æ¥è¯¢æä»¶
 Author: cypas Author-email: ayano05@outlook.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: Pillow
 (==9.5.0) Requires-Dist: SQLAlchemy (>=2.0.25,<3.0.0) Requires-Dist:
 beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: httpx (>=0.24.1,<0.25.0)
```

