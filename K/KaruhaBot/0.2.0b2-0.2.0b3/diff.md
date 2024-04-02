# Comparing `tmp/KaruhaBot-0.2.0b2.tar.gz` & `tmp/KaruhaBot-0.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KaruhaBot-0.2.0b2.tar", last modified: Wed Mar  6 08:25:58 2024, max compression
+gzip compressed data, was "KaruhaBot-0.2.0b3.tar", last modified: Tue Apr  2 12:10:42 2024, max compression
```

## Comparing `KaruhaBot-0.2.0b2.tar` & `KaruhaBot-0.2.0b3.tar`

### file list

```diff
@@ -1,59 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:25:58.942270 KaruhaBot-0.2.0b2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:25:58.942270 KaruhaBot-0.2.0b2/KaruhaBot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-03-06 08:25:58.000000 KaruhaBot-0.2.0b2/KaruhaBot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-06 08:25:58.000000 KaruhaBot-0.2.0b2/KaruhaBot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 08:25:58.000000 KaruhaBot-0.2.0b2/KaruhaBot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-06 08:25:58.000000 KaruhaBot-0.2.0b2/KaruhaBot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-06 08:25:58.000000 KaruhaBot-0.2.0b2/KaruhaBot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-03-06 08:25:58.942270 KaruhaBot-0.2.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:25:58.938270 KaruhaBot-0.2.0b2/karuha/
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28356 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:25:58.938270 KaruhaBot-0.2.0b2/karuha/command/
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/command/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/command/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/command/decoractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/command/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/command/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:25:58.938270 KaruhaBot-0.2.0b2/karuha/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:25:58.938270 KaruhaBot-0.2.0b2/karuha/event/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/event/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    30968 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/event/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/event/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/event/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/event/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/plugin_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:25:58.942270 KaruhaBot-0.2.0b2/karuha/text/
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/text/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/text/drafty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/text/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    15619 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/text/textchain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:25:58.942270 KaruhaBot-0.2.0b2/karuha/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/utils/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/utils/event_catcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/utils/proxy_propery.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/karuha/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 08:25:58.942270 KaruhaBot-0.2.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:25:58.942270 KaruhaBot-0.2.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/tests/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/tests/test_command_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-03-06 08:25:53.000000 KaruhaBot-0.2.0b2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.962828 KaruhaBot-0.2.0b3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.958828 KaruhaBot-0.2.0b3/KaruhaBot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-04-02 12:10:42.000000 KaruhaBot-0.2.0b3/KaruhaBot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-02 12:10:42.000000 KaruhaBot-0.2.0b3/KaruhaBot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:10:42.000000 KaruhaBot-0.2.0b3/KaruhaBot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-02 12:10:42.000000 KaruhaBot-0.2.0b3/KaruhaBot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 12:10:42.000000 KaruhaBot-0.2.0b3/KaruhaBot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-04-02 12:10:42.958828 KaruhaBot-0.2.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.950827 KaruhaBot-0.2.0b3/karuha/
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29966 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.950827 KaruhaBot-0.2.0b3/karuha/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/command/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/command/decoractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12054 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/command/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/command/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.954828 KaruhaBot-0.2.0b3/karuha/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.954828 KaruhaBot-0.2.0b3/karuha/event/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31583 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/plugin_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.954828 KaruhaBot-0.2.0b3/karuha/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/text/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/text/drafty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/text/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16074 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/text/textchain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.958828 KaruhaBot-0.2.0b3/karuha/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/event_catcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/proxy_propery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:10:42.962828 KaruhaBot-0.2.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.958828 KaruhaBot-0.2.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_command_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/utils.py
```

### Comparing `KaruhaBot-0.2.0b2/KaruhaBot.egg-info/PKG-INFO` & `KaruhaBot-0.2.0b3/KaruhaBot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: KaruhaBot
-Version: 0.2.0b2
+Version: 0.2.0b3
 Summary: A simple Tinode chatbot framework.
-Home-page: https://github.com/Ovizro/Karuha
+Home-page: https://github.com/Visecy/Karuha
 Author: Visecy
 Author-email: Visecy@visecy.org
 Maintainer: Ovizro
 Maintainer-email: Ovizro@visecy.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,22 +24,26 @@
 Requires-Dist: typing_extensions>=4.0
 Requires-Dist: grpcio>=1.40.0
 Requires-Dist: tinode-grpc>=0.20.0b3
 Requires-Dist: pydantic>2.0
 Requires-Dist: aiofiles
 Provides-Extra: image
 Requires-Dist: pillow; extra == "image"
+Provides-Extra: data
+Requires-Dist: greenback; extra == "data"
 Provides-Extra: all
 Requires-Dist: pillow; extra == "all"
+Requires-Dist: greenback; extra == "all"
 
 # Karuha
 
 [![License](https://img.shields.io/github/license/Ovizro/Karuha.svg)](LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/KaruhaBot.svg)](https://pypi.python.org/pypi/KaruhaBot)
 [![Build Status](https://github.com/Ovizro/Karuha/actions/workflows/build_test.yml/badge.svg)](https://github.com/Ovizro/Karuha/actions)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/KaruhaBot)
 ![Python Version](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12-blue.svg)
 
 A simple Tinode chatbot framework.
 
 **Language: English/[中文](README_cn.md)**
 
 The name of the library `Karuha` comes from the character Karuha Ramukone (カルハ・ラムコネ) in the game 星空鉄道とシロの旅.
@@ -56,30 +60,30 @@
 
 From pip:
 
     pip install KaruhaBot
 
 From source code:
 
-    git clone https://github.com/Ovizro/Karuha.git
+    git clone https://github.com/Visecy/Karuha.git
     cd Karuha
     make install
 
 ## Quick Start
 
 Before starting, you need to make sure you have the Tinode service running locally with its gRPC port set to the default value of 16060.
 
 > If your service is not local or the gRPC port has been changed, you may need to modify or add additional server configuration items in the following code.
 
 Create a new file config.json and write the configuration in it:
 
 ```json
 {
     "server": {
-        "host": "localhost:16060",
+        "host": "localhost:16060"
     },
     "bots": [
         {
             "name": "chatbot",
             "schema": "basic",
             "secret": "{chatbot_login_name}:{chatebot_login_passwd}"
         }
@@ -121,15 +125,15 @@
 You may be unfamiliar with line `(session: MessageSession) -> None`. This is a type annotation to indicate the parameter type and return value type of the function. Here we declare the type of session to be `MessageSession`, and the return type to be `None`, meaning no return value. Type annotations are optional in Python but recommended for Karuha commands to help parse message data.
 
 Then comes the function body, which is very short with only one line. `session` is a session object that encapsulates many APIs for receiving and sending messages. Here we use the `send` method to send a message. `send` is an asynchronous method, so we need to use await when calling it.
 
 After writing the command, we can run the chatbot to test it. Use the following command:
 
 ```sh
-python -m Karuha ./config.json -m hi
+python -m karuha ./config.json -m hi
 ```
 
 Then in the conversation with the bot, enter the following:
 
      /hi
```

### Comparing `KaruhaBot-0.2.0b2/KaruhaBot.egg-info/SOURCES.txt` & `KaruhaBot-0.2.0b3/KaruhaBot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,40 +9,51 @@
 karuha/__init__.py
 karuha/__main__.py
 karuha/bot.py
 karuha/config.py
 karuha/exception.py
 karuha/logger.py
 karuha/plugin_server.py
+karuha/store.py
 karuha/version.py
 karuha/command/__init__.py
 karuha/command/collection.py
 karuha/command/command.py
 karuha/command/decoractor.py
 karuha/command/parser.py
 karuha/command/session.py
 karuha/data/__init__.py
+karuha/data/cache.py
+karuha/data/data.py
+karuha/data/meta.py
+karuha/data/sub.py
+karuha/data/topic.py
+karuha/data/user.py
 karuha/event/__init__.py
 karuha/event/base.py
 karuha/event/bot.py
 karuha/event/command.py
 karuha/event/message.py
 karuha/event/plugin.py
+karuha/event/sys.py
 karuha/text/__init__.py
 karuha/text/convert.py
 karuha/text/drafty.py
 karuha/text/message.py
 karuha/text/textchain.py
 karuha/utils/__init__.py
+karuha/utils/argparse.py
 karuha/utils/context.py
 karuha/utils/decode.py
 karuha/utils/dispatcher.py
 karuha/utils/event_catcher.py
 karuha/utils/proxy_propery.py
 tests/__init__.py
 tests/test_bot.py
 tests/test_command.py
 tests/test_command_run.py
+tests/test_data.py
 tests/test_event.py
 tests/test_session.py
+tests/test_store.py
 tests/test_text.py
 tests/utils.py
```

### Comparing `KaruhaBot-0.2.0b2/LICENSE` & `KaruhaBot-0.2.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/PKG-INFO` & `KaruhaBot-0.2.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: KaruhaBot
-Version: 0.2.0b2
+Version: 0.2.0b3
 Summary: A simple Tinode chatbot framework.
-Home-page: https://github.com/Ovizro/Karuha
+Home-page: https://github.com/Visecy/Karuha
 Author: Visecy
 Author-email: Visecy@visecy.org
 Maintainer: Ovizro
 Maintainer-email: Ovizro@visecy.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,22 +24,26 @@
 Requires-Dist: typing_extensions>=4.0
 Requires-Dist: grpcio>=1.40.0
 Requires-Dist: tinode-grpc>=0.20.0b3
 Requires-Dist: pydantic>2.0
 Requires-Dist: aiofiles
 Provides-Extra: image
 Requires-Dist: pillow; extra == "image"
+Provides-Extra: data
+Requires-Dist: greenback; extra == "data"
 Provides-Extra: all
 Requires-Dist: pillow; extra == "all"
+Requires-Dist: greenback; extra == "all"
 
 # Karuha
 
 [![License](https://img.shields.io/github/license/Ovizro/Karuha.svg)](LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/KaruhaBot.svg)](https://pypi.python.org/pypi/KaruhaBot)
 [![Build Status](https://github.com/Ovizro/Karuha/actions/workflows/build_test.yml/badge.svg)](https://github.com/Ovizro/Karuha/actions)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/KaruhaBot)
 ![Python Version](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12-blue.svg)
 
 A simple Tinode chatbot framework.
 
 **Language: English/[中文](README_cn.md)**
 
 The name of the library `Karuha` comes from the character Karuha Ramukone (カルハ・ラムコネ) in the game 星空鉄道とシロの旅.
@@ -56,30 +60,30 @@
 
 From pip:
 
     pip install KaruhaBot
 
 From source code:
 
-    git clone https://github.com/Ovizro/Karuha.git
+    git clone https://github.com/Visecy/Karuha.git
     cd Karuha
     make install
 
 ## Quick Start
 
 Before starting, you need to make sure you have the Tinode service running locally with its gRPC port set to the default value of 16060.
 
 > If your service is not local or the gRPC port has been changed, you may need to modify or add additional server configuration items in the following code.
 
 Create a new file config.json and write the configuration in it:
 
 ```json
 {
     "server": {
-        "host": "localhost:16060",
+        "host": "localhost:16060"
     },
     "bots": [
         {
             "name": "chatbot",
             "schema": "basic",
             "secret": "{chatbot_login_name}:{chatebot_login_passwd}"
         }
@@ -121,15 +125,15 @@
 You may be unfamiliar with line `(session: MessageSession) -> None`. This is a type annotation to indicate the parameter type and return value type of the function. Here we declare the type of session to be `MessageSession`, and the return type to be `None`, meaning no return value. Type annotations are optional in Python but recommended for Karuha commands to help parse message data.
 
 Then comes the function body, which is very short with only one line. `session` is a session object that encapsulates many APIs for receiving and sending messages. Here we use the `send` method to send a message. `send` is an asynchronous method, so we need to use await when calling it.
 
 After writing the command, we can run the chatbot to test it. Use the following command:
 
 ```sh
-python -m Karuha ./config.json -m hi
+python -m karuha ./config.json -m hi
 ```
 
 Then in the conversation with the bot, enter the following:
 
      /hi
```

### Comparing `KaruhaBot-0.2.0b2/README.md` & `KaruhaBot-0.2.0b3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Karuha
 
 [![License](https://img.shields.io/github/license/Ovizro/Karuha.svg)](LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/KaruhaBot.svg)](https://pypi.python.org/pypi/KaruhaBot)
 [![Build Status](https://github.com/Ovizro/Karuha/actions/workflows/build_test.yml/badge.svg)](https://github.com/Ovizro/Karuha/actions)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/KaruhaBot)
 ![Python Version](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12-blue.svg)
 
 A simple Tinode chatbot framework.
 
 **Language: English/[中文](README_cn.md)**
 
 The name of the library `Karuha` comes from the character Karuha Ramukone (カルハ・ラムコネ) in the game 星空鉄道とシロの旅.
@@ -23,30 +24,30 @@
 
 From pip:
 
     pip install KaruhaBot
 
 From source code:
 
-    git clone https://github.com/Ovizro/Karuha.git
+    git clone https://github.com/Visecy/Karuha.git
     cd Karuha
     make install
 
 ## Quick Start
 
 Before starting, you need to make sure you have the Tinode service running locally with its gRPC port set to the default value of 16060.
 
 > If your service is not local or the gRPC port has been changed, you may need to modify or add additional server configuration items in the following code.
 
 Create a new file config.json and write the configuration in it:
 
 ```json
 {
     "server": {
-        "host": "localhost:16060",
+        "host": "localhost:16060"
     },
     "bots": [
         {
             "name": "chatbot",
             "schema": "basic",
             "secret": "{chatbot_login_name}:{chatebot_login_passwd}"
         }
@@ -88,15 +89,15 @@
 You may be unfamiliar with line `(session: MessageSession) -> None`. This is a type annotation to indicate the parameter type and return value type of the function. Here we declare the type of session to be `MessageSession`, and the return type to be `None`, meaning no return value. Type annotations are optional in Python but recommended for Karuha commands to help parse message data.
 
 Then comes the function body, which is very short with only one line. `session` is a session object that encapsulates many APIs for receiving and sending messages. Here we use the `send` method to send a message. `send` is an asynchronous method, so we need to use await when calling it.
 
 After writing the command, we can run the chatbot to test it. Use the following command:
 
 ```sh
-python -m Karuha ./config.json -m hi
+python -m karuha ./config.json -m hi
 ```
 
 Then in the conversation with the bot, enter the following:
 
      /hi
```

### Comparing `KaruhaBot-0.2.0b2/karuha/__init__.py` & `KaruhaBot-0.2.0b3/karuha/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 
 from .version import __version__
 from .config import get_config, load_config, init_config, save_config, Config
 from .config import Server as ServerConfig, Bot as BotConfig
 from .bot import Bot
 from .event import on, on_event, Event
+from .event.sys import SystemStartEvent, SystemStopEvent
 from .exception import KaruhaException
-from .command import CommandCollection, AbstractCommand, AbstractCommandParser, BaseSession, MessageSession, get_collection, on_command
-from .event.message import reset_message_lock
+from .command import CommandCollection, AbstractCommand, AbstractCommandParser, BaseSession, MessageSession, CommandSession, get_collection, on_command
 from .text import Drafty, BaseText, PlainText, Message, TextChain
 from .logger import logger
 
 
 _bot_cache: Dict[str, Bot] = {}
 _loop = None
 
@@ -78,26 +78,27 @@
         server = init_server(config.server.listen)
         _loop.call_soon(server.start)
     else:
         server = None
     
     if config.log_level == "DEBUG":
         _loop.set_debug(True)
-        
-    if not tasks:  # pragma: no cover
-        logger.warning("no bot found")
-        return
     
     try:
+        await SystemStartEvent.new_and_wait(config, _bot_cache.values())
+        if not tasks:  # pragma: no cover
+            logger.warning("no bot found, exit")
+            return
         await asyncio.gather(*tasks)
         logger.info("all bots have been cancelled, exit")
     finally:
         if server is not None:  # pragma: no cover
             logger.info("stop plugin server")
             server.stop(None)
+        await SystemStopEvent(config).trigger(return_exceptions=True)
         _loop = None
     
 
 def run() -> None:
     try:
         asyncio.run(async_run())
     except (KeyboardInterrupt, asyncio.CancelledError):  # pragma: no cover
@@ -134,14 +135,15 @@
     # command
     "CommandCollection",
     "AbstractCommand",
     "AbstractCommandParser",
     "get_collection",
     "BaseSession",
     "MessageSession",
+    "CommandSession",
     # decorator
     "on",
     "on_event",
     "on_command",
     # exception
     "KaruhaException"
 ]
```

### Comparing `KaruhaBot-0.2.0b2/karuha/__main__.py` & `KaruhaBot-0.2.0b3/karuha/__main__.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/karuha/bot.py` & `KaruhaBot-0.2.0b3/karuha/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+from datetime import datetime, timezone
 import platform
 import sys
 from asyncio.queues import Queue
 from base64 import b64decode
 from collections import defaultdict
 from contextlib import asynccontextmanager, contextmanager
 from enum import IntEnum
@@ -10,24 +11,26 @@
                     List, Literal, Optional, Tuple, Union, overload)
 from weakref import WeakSet, ref
 
 import grpc
 from aiofiles import open as aio_open
 from google.protobuf.message import Message
 from grpc import aio as grpc_aio
+from pydantic import GetCoreSchemaHandler, TypeAdapter
+from pydantic_core import CoreSchema, core_schema, from_json, to_json
 from tinode_grpc import pb
 from typing_extensions import Self, deprecated
 
 from .config import Bot as BotConfig
 from .config import Config
 from .config import Server as ServerConfig
 from .config import get_config, init_config
 from .logger import Level, get_sub_logger
 from .version import APP_VERSION, LIB_VERSION
-from .utils.decode import decode_mapping, encode_mapping, json
+from .utils.decode import decode_mapping, encode_mapping
 
 
 class State(IntEnum):
     disabled = 0
     running = 1
     stopped = 2
     restarting = 3
@@ -36,22 +39,29 @@
 class Bot(object):
     """
     the core class of the chatbot
 
     Provides many low-level API interfaces.
     """
     __slots__ = [
-        "queue", "state", "client", "logger", "config", "server",
+        "queue", "state", "client", "logger", "config", "server", "user_id", "token", "token_expires", "authlvl",
         "_wait_list", "_tid_counter", "_tasks", "_loop_task_ref"
     ]
 
     initialize_event_callback: Callable[[Self], Any]
     finalize_event_callback: Callable[[Self], Coroutine]
-    server_event_callbacks: Dict[str, List[Callable[[Self, Message], Any]]] = defaultdict(list)
-    client_event_callbacks: Dict[str, List[Callable[[Self, Message, Optional[Message]], Any]]] = defaultdict(list)
+    server_event_callbacks: Dict[str, List[Callable[[Self, Message], Any]]] = (
+        defaultdict(list)
+    )
+    client_event_callbacks: Dict[
+        str,
+        List[
+            Callable[[Self, Message, Optional[Message], Optional[pb.ClientExtra]], Any]
+        ],
+    ] = defaultdict(list)
 
     @overload
     def __init__(
         self,
         config: BotConfig,
         /, *,
         server: Union[ServerConfig, Any, None] = None,
@@ -107,14 +117,15 @@
         self.state = State.stopped
         self.logger = get_sub_logger(self.name)
         if log_level is not None:
             self.logger.setLevel(log_level)
         if server is not None and not isinstance(server, ServerConfig):
             server = ServerConfig.model_validate(server)
         self.server = server
+        self.token = None
         self._wait_list: Dict[str, asyncio.Future] = {}
         self._tid_counter = 100
         self._tasks = WeakSet()  # type: WeakSet[asyncio.Future]
         self._loop_task_ref = lambda: None
 
     async def hello(self, /, lang: str = "EN") -> Tuple[str, Dict[str, Any]]:
         """
@@ -157,15 +168,17 @@
         
         :return: tid and params
         :rtype: Tuple[str, Dict[str, Any]]
         """
         tid = self._get_tid()
         schema, secret = self.config.schema_, self.config.secret
         try:
-            if schema == "cookie":
+            if self.token is not None and self.token_expires > datetime.now(timezone.utc):
+                schema, secret = "token", self.token.encode("ascii")
+            elif schema == "cookie":
                 schema, secret = await read_auth_cookie(self.config.secret)
             else:
                 secret = secret.encode("ascii")
         except Exception as e:  # pragma: no cover
             err_text = f"fail to read auth secret: {e}"
             self.logger.error(err_text)
             self.cancel()
@@ -184,31 +197,31 @@
             return tid, decode_mapping(ctrl.params)
         elif ctrl.code < 200 or ctrl.code >= 400:
             err_text = f"fail to login: {ctrl.text}"
             self.logger.error(err_text)
             self.cancel()
             raise KaruhaBotError(err_text, bot=self, code=ctrl.code)
 
-        self.logger.info("login successful")
+        self.logger.info(f"login successful (schema {schema})")
 
-        params = ctrl.params
-        if not params:
-            return tid, {}
+        params = decode_mapping(ctrl.params)
         if "user" in params:
-            self.config.user = json.loads(params["user"].decode())
-        # if "token" in params:
-        #     self.config.schema_ = "token"
-        #     self.config.secret = json.loads(params["token"].decode())
-        return tid, decode_mapping(params)
+            self.user_id = params["user"]
+        if "token" in params:
+            self.token = params["token"]
+            # datetime.fromisoformat before 3.11 does not support any iso 8601 format, use pydantic instead
+            self.token_expires = TypeAdapter(datetime).validate_python(params["expires"])
+        return tid, params
 
     async def subscribe(
         self, /, topic: str,
         *,
         mode: Optional[str] = None,
         get: Optional[Union[pb.GetQuery, str]] = None,
+        set: Optional[pb.SetQuery] = None,
         get_since: Optional[int] = None,
         limit: int = 24,
         extra: Optional[pb.ClientExtra] = None
     ) -> Tuple[str, Dict[str, Any]]:
         """
         subscribe to a topic
         
@@ -223,36 +236,38 @@
         :param extra: extra data
         :type extra: Optional[pb.ClientExtra]
         :return: tid and params
         :rtype: Tuple[str, Dict[str, Any]]
         """
         tid = self._get_tid()
         if get_since is not None:
-            if get is not None:
-                raise ValueError("get_since and get cannot be used at the same time")
+            assert get is None, "get_since and get cannot be used at the same time"
             get = pb.GetQuery(
                 data=pb.GetOpts(
                     since_id=get_since,
                     limit=limit
                 ),
                 what="data"
             )
         elif isinstance(get, str):
             get = pb.GetQuery(
                 what=get
             )
+        if mode is not None:
+            assert set is None, "mode and set cannot be used at the same time"
+            set = pb.SetQuery(
+                sub=pb.SetSub(mode=mode)
+            )
         ctrl = await self.send_message(
             tid,
             sub=pb.ClientSub(
                 id=tid,
                 topic=topic,
                 get_query=get,
-                set_query=pb.SetQuery(
-                    sub=pb.SetSub(mode=mode)
-                )
+                set_query=set
             ),
             extra=extra
         )
         assert isinstance(ctrl, pb.ServerCtrl)
         if ctrl.code < 200 or ctrl.code >= 400:
             err_text = f"fail to subscribe topic {topic}: {ctrl.text}"
             self.logger.error(err_text)
@@ -333,76 +348,76 @@
         ctrl = await self.send_message(
             tid,
             pub=pb.ClientPub(
                 id=tid,
                 topic=topic,
                 no_echo=True,
                 head=head,
-                content=json.dumps(text).encode()
+                content=to_json(text)
             ),
             extra=extra
         )
         assert isinstance(ctrl, pb.ServerCtrl)
         if ctrl.code < 200 or ctrl.code >= 400:
             err_text = f"fail to publish message to {topic}: {ctrl.text}"
             self.logger.error(err_text)
             raise KaruhaBotError(err_text, bot=self, code=ctrl.code)
         return tid, decode_mapping(ctrl.params)
 
     @overload
     async def get(
-            self,
-            /,
-            topic: str,
-            what: Optional[Literal["desc"]] = None,
-            *,
-            desc: Optional[pb.GetOpts] = None,
-            extra: Optional[pb.ClientExtra] = None
+        self,
+        /,
+        topic: str,
+        what: Optional[Literal["desc"]] = None,
+        *,
+        desc: Optional[pb.GetOpts] = None,
+        extra: Optional[pb.ClientExtra] = None,
     ) -> Tuple[str, Optional[pb.ServerMeta]]: ...
 
     @overload
     async def get(
-            self,
-            /,
-            topic: str,
-            what: Optional[Literal["sub"]] = None,
-            *,
-            sub: Optional[pb.GetOpts] = None,
-            extra: Optional[pb.ClientExtra] = None
+        self,
+        /,
+        topic: str,
+        what: Optional[Literal["sub"]] = None,
+        *,
+        sub: Optional[pb.GetOpts] = None,
+        extra: Optional[pb.ClientExtra] = None,
     ) -> Tuple[str, Optional[pb.ServerMeta]]: ...
 
     @overload
     async def get(
-            self,
-            /,
-            topic: str,
-            what: Optional[Literal["data"]] = None,
-            *,
-            data: Optional[pb.GetOpts] = None,
-            extra: Optional[pb.ClientExtra] = None
+        self,
+        /,
+        topic: str,
+        what: Optional[Literal["data"]] = None,
+        *,
+        data: Optional[pb.GetOpts] = None,
+        extra: Optional[pb.ClientExtra] = None,
     ) -> Tuple[str, Optional[pb.ServerMeta]]: ...
 
     @overload
     async def get(
-            self,
-            /,
-            topic: str,
-            what: Literal["tags"],
-            *,
-            extra: Optional[pb.ClientExtra] = None
+        self,
+        /,
+        topic: str,
+        what: Literal["tags"],
+        *,
+        extra: Optional[pb.ClientExtra] = None,
     ) -> Tuple[str, Optional[pb.ServerMeta]]: ...
 
     @overload
     async def get(
-            self,
-            /,
-            topic: str,
-            what: Literal["cred"],
-            *,
-            extra: Optional[pb.ClientExtra] = None
+        self,
+        /,
+        topic: str,
+        what: Literal["cred"],
+        *,
+        extra: Optional[pb.ClientExtra] = None,
     ) -> Tuple[str, Optional[pb.ServerMeta]]: ...
 
     async def get(
             self,
             /,
             topic: str,
             what: Optional[Literal["desc", "sub", "data", "tags", "cred"]] = None,
@@ -508,15 +523,15 @@
                     sub=sub,
                     data=data
                 )
             ),
             extra=extra
         )
         return tid, None
-    
+
     async def set(
             self,
             /,
             topic: str,
             *,
             desc: Optional[pb.SetDesc] = None,
             sub: Optional[pb.SetSub] = None,
@@ -565,20 +580,40 @@
             raise KaruhaBotError(err_text, bot=self, code=ctrl.code)
         return tid, decode_mapping(ctrl.params)
 
     async def note_read(self, /, topic: str, seq: int) -> None:
         await self.send_message(note=pb.ClientNote(topic=topic, what=pb.READ, seq_id=seq))
 
     @overload
-    async def send_message(self, wait_tid: str, /, **kwds: Optional[Message]) -> Message: ...
+    async def send_message(
+        self,
+        wait_tid: str,
+        /,
+        *,
+        extra: Optional[pb.ClientExtra] = None,
+        **kwds: Optional[Message],
+    ) -> Message: ...
 
     @overload
-    async def send_message(self, wait_tid: None = None, /, **kwds: Optional[Message]) -> None: ...
+    async def send_message(
+        self,
+        wait_tid: None = None,
+        /,
+        *,
+        extra: Optional[pb.ClientExtra] = None,
+        **kwds: Optional[Message],
+    ) -> None: ...
 
-    async def send_message(self, wait_tid: Optional[str] = None, /, **kwds: Optional[Message]) -> Optional[Message]:
+    async def send_message(
+            self,
+            wait_tid: Optional[str] = None,
+            /, *,
+            extra: Optional[pb.ClientExtra] = None,
+            **kwds: Optional[Message]
+    ) -> Optional[Message]:
         """set messages to Tinode server
 
         :param wait_tid: if set, it willl wait until a response message with the same tid is received, defaults to None
         :type wait_tid: Optional[str], optional
         :return: message which has the same tid
         :rtype: Optional[Message]
         """
@@ -586,22 +621,23 @@
         if self.state != State.running:
             raise KaruhaBotError("bot is not running", bot=self)
         client_msg = pb.ClientMsg(**kwds)  # type: ignore
         ret = None
         if wait_tid is None:
             await self.queue.put(client_msg)
         else:
+            timeout = self.server.timeout if self.server is not None else 10
             with self._wait_reply(wait_tid) as future:
                 await self.queue.put(client_msg)
-                ret = await future
+                ret = await asyncio.wait_for(future, timeout=timeout)
         for k, v in kwds.items():
             if v is None:
                 continue
             for cb in self.client_event_callbacks[k]:
-                cb(self, v, ret)
+                cb(self, v, ret, extra)
         return ret
 
     async def async_run(self, server_config: Optional[ServerConfig] = None) -> None:  # pragma: no cover
         """
         run the bot in an async loop
 
         :param server_config: Optional server configuration. Defaults to None.
@@ -688,34 +724,39 @@
 
     @property
     def name(self) -> str:
         return self.config.name
 
     @property
     def uid(self) -> str:
-        uid = self.config.user
-        if uid is None:
-            raise ValueError(f"cannot fetch the uid of bot {self.name}")
-        return uid
+        return self.user_id
 
     def _get_tid(self) -> str:
         tid = str(self._tid_counter)
         self._tid_counter += 1
         return tid
 
     @contextmanager
     def _wait_reply(self, tid: Optional[str] = None) -> Generator[asyncio.Future, None, None]:
         tid = tid or self._get_tid()
         future = asyncio.get_running_loop().create_future()
         self._wait_list[tid] = future
         try:
             yield future
+        except asyncio.TimeoutError:
+            raise KaruhaTimeoutError(f"timeout while waiting for reply from bot {self.name}") from None
         finally:
             assert self._wait_list.pop(tid, None) is future
 
+    def _set_reply_message(self, tid: str, message: Any) -> None:
+        if tid in self._wait_list:
+            f = self._wait_list[tid]
+            if not f.done():
+                f.set_result(message)
+
     def _create_task(self, coro: Coroutine, /) -> asyncio.Task:
         task = asyncio.create_task(coro)
         self._tasks.add(task)
         return task
 
     def _prepare_loop_task(self) -> None:
         if self.state == State.running:
@@ -736,16 +777,18 @@
         opts = (('grpc.ssl_target_name_override', ssl_host),) if ssl_host else None
         self.logger.info(f"connecting to secure server at {host} SNI={ssl_host or host}")
         return grpc_aio.secure_channel(host, grpc.ssl_channel_credentials(), opts)
 
     @asynccontextmanager
     async def _run_context(self, server_config: ServerConfig, /) -> AsyncGenerator[grpc_aio.Channel, None]:  # pragma: no cover
         channel = self._get_channel(server_config)
-        self.initialize_event_callback(self)
+        old_server_config = self.server
+        self.server = server_config
         try:
+            self.initialize_event_callback(self)
             yield channel
         except grpc.RpcError:
             self.logger.error(f"disconnected from {server_config.host}, retrying...", exc_info=sys.exc_info())
             await asyncio.sleep(0.5)
         except asyncio.CancelledError:
             if self.state == State.restarting:
                 # uncancel from Bot.restart()
@@ -760,15 +803,16 @@
             try:
                 await channel.close()
                 await self.finalize_event_callback(self)
             except Exception:
                 self.logger.exception("error while finalizing event callback", exc_info=True)
             except asyncio.CancelledError:
                 pass
-            
+            self.server = old_server_config
+
             # clean up for restarting
             while not self.queue.empty():
                 self.queue.get_nowait()
 
             for t in self._tasks:
                 t.cancel()
 
@@ -784,17 +828,25 @@
         async for message in client:  # type: ignore
             self.logger.debug(f"in: {message}")
 
             for desc, msg in message.ListFields():
                 for e in self.server_event_callbacks[desc.name]:
                     e(self, msg)
 
+    @classmethod
+    def __get_pydantic_core_schema__(
+        cls, source_type: Any, handler: GetCoreSchemaHandler
+    ) -> CoreSchema:
+        return core_schema.no_info_plain_validator_function(
+            lambda x: x if isinstance(x, source_type) else Bot(x)
+        )
+
     def __repr__(self) -> str:
         state = self.state.name
-        uid = self.config.user or ''
+        uid = getattr(self, "user_id", 'unknown uid')
         host = self.server.host if self.server else 'unknown'
         return f"<bot {self.name} ({uid}) {state} on host {host}>"
 
 
 def get_stream(channel: grpc_aio.Channel, /) -> grpc_aio.StreamStreamMultiCallable:  # pragma: no cover
     return channel.stream_stream(
         '/pbx.Node/MessageLoop',
@@ -802,20 +854,20 @@
         response_deserializer=pb.ServerMsg.FromString
     )
 
 
 async def read_auth_cookie(cookie_file_name) -> Union[Tuple[str, bytes], Tuple[None, None]]:
     """Read authentication token from a file"""
     async with aio_open(cookie_file_name, 'r') as cookie:
-        params = json.loads(await cookie.read())
+        params = from_json(await cookie.read())
     schema = params.get("schema")
     secret = params.get('secret')
     if schema is None or secret is None:
         return None, None
     if schema == 'token':
         secret = b64decode(secret)
     else:
         secret = secret.encode('utf-8')
     return schema, secret
 
 
-from .exception import KaruhaBotError
+from .exception import KaruhaBotError, KaruhaTimeoutError
```

### Comparing `KaruhaBot-0.2.0b2/karuha/command/__init__.py` & `KaruhaBot-0.2.0b3/karuha/command/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .command import AbstractCommand, FunctionCommand, ParamFunctionCommand
 from .collection import (CommandCollection, add_sub_collection, get_collection,
                          new_collection, remove_sub_collection, reset_collection,
                          set_collection, set_collection_factory, set_prefix)
 from .decoractor import on_command
 from .parser import (AbstractCommandParser, ParamParser, ParamParserFlag,
                      SimpleCommandParser)
-from .session import BaseSession, MessageSession
+from .session import BaseSession, MessageSession, CommandSession
 
 from ..event.command import (BaseCommandEvent, CommandCompleteEvent, CommandEvent,
                     CommandFailEvent, CommandNotFoundEvent,
                     CommandPrepareEvent)
 
 
 __all__ = [
```

### Comparing `KaruhaBot-0.2.0b2/karuha/command/collection.py` & `KaruhaBot-0.2.0b3/karuha/command/collection.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/karuha/command/command.py` & `KaruhaBot-0.2.0b3/karuha/command/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,17 @@
             logger.info(f"command {self.name} canceled")
             raise
         try:
             args, kwargs = self.parse_message(message)
             result = self.__func__(*args, **kwargs)  # type: ignore
             if asyncio.iscoroutine(result):
                 result = await result
-        except asyncio.CancelledError:
+        except KaruhaCommandCanceledError:
             logger.info(f"command {self.name} canceled")
-            raise
+            return
         except Exception as e:  # pragma: no cover
             CommandFailEvent.new(message.collection, self, sys.exc_info())  # type: ignore
             logger.error(f"run command {self.name} failed", exc_info=True)
             raise KaruhaCommandError(f"run command {self.name} failed", name=self.name, command=self) from e
         else:
             logger.info(f"command {self.name} complete")
             CommandCompleteEvent.new(message.collection, self, result)
```

### Comparing `KaruhaBot-0.2.0b2/karuha/command/decoractor.py` & `KaruhaBot-0.2.0b3/karuha/command/decoractor.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/karuha/command/parser.py` & `KaruhaBot-0.2.0b3/karuha/command/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from abc import ABC, abstractmethod
 from enum import IntFlag, auto
 from functools import partial
 from inspect import Signature, Parameter, isclass
 from typing import Any, Callable, Iterable, List, NamedTuple, Optional, Tuple, Type, Union, get_args
 from typing_extensions import Self
 
+from ..text.textchain import Quote
+
 from ..utils.dispatcher import AbstractDispatcher
 from ..text import Drafty, BaseText, Message
 from ..exception import KaruhaParserError
 from ..bot import Bot
 from .session import CommandSession
 
 
@@ -31,14 +33,16 @@
 
     def __init__(self, prefix: Iterable[str]) -> None:
         self.prefixs = tuple(prefix)
     
     def parse(self, message: Message) -> Optional[Tuple[str, Union[List[str], List[BaseText]]]]:
         text = message.text
         text = text.split()
+        if text and isinstance(text[0], Quote):
+            text = text[1:]
         if not text:
             return
         
         name = str(text[0])
         for prefix in self.prefixs:
             if name.startswith(prefix):
                 name = name[len(prefix):]
```

### Comparing `KaruhaBot-0.2.0b2/karuha/command/session.py` & `KaruhaBot-0.2.0b3/karuha/command/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
 import os
 import re
 from collections import deque
-from typing import Any, Deque, Dict, Optional, Tuple, Union
+from typing import Any, Deque, Dict, NoReturn, Optional, Tuple, Union
 
 from ..bot import Bot
 from ..event.message import Message, MessageDispatcher, get_message_lock
-from ..exception import KaruhaRuntimeError
+from ..exception import KaruhaRuntimeError, KaruhaCommandCanceledError
 from ..text import BaseText, Drafty
 from ..text.textchain import (Bold, Button, File, Form, Image, NewLine, PlainText,
                               TextChain)
 from ..utils.dispatcher import FutureDispatcher
 
 
 class BaseSession(object):
@@ -164,14 +164,17 @@
         return self._messages[-1]
 
 
 class CommandSession(MessageSession):
     __slots__ = []
 
     _messages: Deque["CommandMessage"]
+
+    def cancel(self) -> NoReturn:
+        raise KaruhaCommandCanceledError
     
     @property
     def messages(self) -> Tuple["CommandMessage", ...]:
         return tuple(self._messages)
     
     @property
     def last_message(self) -> "CommandMessage":
```

### Comparing `KaruhaBot-0.2.0b2/karuha/config.py` & `KaruhaBot-0.2.0b3/karuha/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from pathlib import Path
 from typing import Iterable, Literal, Optional, Tuple, Union
-from pydantic import AnyUrl, BaseModel, Field, PrivateAttr, field_validator
+from pydantic import AnyUrl, BaseModel, Field, PrivateAttr, ValidationError, field_validator
 from typing_extensions import Annotated
 
 from .logger import logger, Level
 
 
 class Server(BaseModel):
     host: Annotated[str, AnyUrl] = "localhost:16060"
+    web_host: Annotated[str, AnyUrl] = "localhost:6060"
+    api_key: str = "AQEAAAABAAD_rAp4DJh05a1HAwFT3A6K"
     ssl: bool = False
     ssl_host: Optional[str] = None
     enable_plugin: bool = False
     listen: Annotated[str, AnyUrl] = "0.0.0.0:40051"
+    timeout: float = 5
+    retry: int = 5
 
 
 class Bot(BaseModel):
     name: str = "chatbot"
     schema_: Literal["basic", "token", "cookie"] = Field(alias="schema")
     secret: str
-    user: Optional[str] = None
     auto_subscribe_new_user: bool = False
 
 
 class Config(BaseModel):
     log_level: Level = "INFO"
     server: Server = Server()
     bots: Tuple[Bot, ...] = ()
@@ -66,19 +69,25 @@
     encoding: str = "utf-8",
     auto_create: bool = True
 ) -> "Config":
     global _config
     try:
         with open(path, "r", encoding=encoding) as f:
             config = Config.model_validate_json(f.read())
-    except Exception:
-        logger.warn(f"failed to load config from '{path}'")
+    except OSError:
+        logger.warn(f"failed to load file '{path}'", exc_info=True)
         config = Config(_path=path)  # type: ignore
         if auto_create:
             config.save(path, encoding=encoding, ignore_error=True)
+    except ValidationError:
+        logger.error(f"'{path}' is not valid config file")
+        raise
+    except Exception:
+        logger.error(f"failed to load config from '{path}'")
+        raise
     config._path = path  # type: ignore
     _config = config
     return config
 
 
 def init_config(
     server: Union[dict, Server] = Server(),
```

### Comparing `KaruhaBot-0.2.0b2/karuha/event/__init__.py` & `KaruhaBot-0.2.0b3/karuha/event/__init__.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/karuha/event/bot.py` & `KaruhaBot-0.2.0b3/karuha/event/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import asyncio
 from functools import partial
 from typing import Any, Awaitable, Callable, Coroutine, Mapping, Optional
 from typing_extensions import Self
 
 from google.protobuf.message import Message
 from tinode_grpc import pb
 
 from .. import bot
-from .base import Event
+from .base import Event, handler_runner
 from ..utils.proxy_propery import ProxyProperty
 
 
 def ensure_text_len(text: str, length: int = 128) -> str:
     if len(text) < length:
         return text
     tail_length = length // 4
@@ -20,23 +21,37 @@
 class BotEvent(Event):
     __slots__ = ["bot"]
 
     def __init__(self, bot: "bot.Bot", /) -> None:
         self.bot = bot
 
     def call_handler(self, handler: Callable[[Self], Coroutine]) -> Awaitable:
-        return self.bot._create_task(handler(self))
+        return self.bot._create_task(handler_runner(self, self.bot.logger, handler))
 
 
 class BotInitEvent(BotEvent):
     __slots__ = []
 
     async def __default_handler__(self) -> None:
-        await self.bot.hello()
-        await self.bot.login()
+        bot = self.bot
+        retry = bot.server.retry if bot.server is not None else 0
+        for i in range(retry):
+            try:
+                await self.bot.hello()
+                await self.bot.login()
+            except asyncio.TimeoutError:
+                self.bot.logger.warning(f"login failed, retrying {i+1} times")
+            else:
+                break
+        else:
+            try:
+                await self.bot.login()
+            except asyncio.TimeoutError:
+                self.bot.logger.error("login failed, cancel the bot")
+                self.bot.cancel()
 
 
 class BotFinishEvent(BotEvent):
     __slots__ = []
 
 
 bot.Bot.initialize_event_callback = BotInitEvent.new
@@ -140,16 +155,15 @@
     topic: ProxyProperty[str] = ServerMessageProperty()
     code: ProxyProperty[int] = ServerMessageProperty()
     text: ProxyProperty[str] = ServerMessageProperty()
     params: ProxyProperty[Mapping[str, bytes]] = ServerMessageProperty()
     
     async def __default_handler__(self) -> None:
         tid = self.server_message.id
-        if tid in self.bot._wait_list:
-            self.bot._wait_list[tid].set_result(self.server_message)
+        self.bot._set_reply_message(tid, self.server_message)
 
 
 class MetaEvent(ServerEvent, on_field="meta"):
     """
     Information about topic metadata or subscribers, sent in response to `{get}`,
     `{set}` or `{sub}` message to the originating session.
 
@@ -261,16 +275,15 @@
     server_message: pb.ServerMeta
 
     id: ProxyProperty[str] = ServerMessageProperty()
     topic: ProxyProperty[str] = ServerMessageProperty()
     
     async def __default_handler__(self) -> None:
         tid = self.server_message.id
-        if tid in self.bot._wait_list:
-            self.bot._wait_list[tid].set_result(self.server_message)
+        self.bot._set_reply_message(tid, self.server_message)
 
 
 class PresEvent(ServerEvent, on_field="pres"):
     """
     Tinode uses `{pres}` message to inform clients of important events.
     A separate [document](https://docs.google.com/spreadsheets/d/e/2PACX-1vStUDHb7DPrD8tF5eANLu4YIjRkqta8KOhLvcj2precsjqR40eDHvJnnuuS3bw-NcWsP1QKc7GSTYuX/pubhtml?gid=1959642482&single=true) explains all possible use cases.
 
@@ -326,19 +339,14 @@
     seq_id: ProxyProperty[int] = ServerMessageProperty()
     del_id: ProxyProperty[int] = ServerMessageProperty()
     target_user_id: ProxyProperty[str] = ServerMessageProperty()
     actor_user_id: ProxyProperty[str] = ServerMessageProperty()
 
     async def __default_handler__(self) -> None:
         msg = self.server_message
-        if msg.what == pb.ServerPres.ACS:
-            topic = msg.topic
-            _, meta = await self.bot.get(topic, "desc")
-            if meta:
-                await self.bot.set(topic, sub=pb.SetSub(mode=meta.desc.acs.given))
         if msg.topic != "me":
             return
         if msg.what == pb.ServerPres.ON:
             await self.bot.subscribe(msg.src, get="desc sub")
         elif msg.what == pb.ServerPres.MSG:
             await self.bot.subscribe(
                 msg.src,
@@ -349,14 +357,19 @@
                     )
                 )
             )
         elif msg.what == pb.ServerPres.OFF:
             await self.bot.leave(msg.src)
         elif msg.what == pb.ServerPres.UPD:
             await self.bot.get(msg.src, "desc")
+        elif msg.what == pb.ServerPres.ACS:
+            topic = msg.src
+            _, meta = await self.bot.get(topic, "desc")
+            if meta:
+                await self.bot.set(topic, sub=pb.SetSub(mode=meta.desc.acs.given))
 
 
 class InfoEvent(ServerEvent, on_field="info"):
     """
     Forwarded client-generated notification `{note}`. Server guarantees that the message complies
     with this specification and that content of `topic` and `from` fields is correct.
     The other content is copied from the `{note}` message verbatim and
@@ -386,32 +399,39 @@
     seq_id: ProxyProperty[int] = ServerMessageProperty()
     src: ProxyProperty[str] = ServerMessageProperty()
     payload: ProxyProperty[bytes] = ServerMessageProperty()
 
 
 # Client Event Part
 # =========================
-    
+
 
 ClientMessageProperty = partial(ProxyProperty, "client_message")
 
 
 class ClientEvent(BotEvent):
     """base class for client events
     
     NOTE: Such events will be triggered after the corresponding action is completed.
     """
 
-    __slots__ = ["client_message", "response_message"]
+    __slots__ = ["client_message", "response_message", "extra"]
 
-    def __init__(self, bot: "bot.Bot", message: Message, response_message: Optional[Message] = None) -> None:
+    def __init__(
+        self,
+        bot: "bot.Bot",
+        message: Message,
+        response_message: Optional[Message] = None,
+        extra: Optional[pb.ClientExtra] = None,
+    ) -> None:
         super().__init__(bot)
         self.client_message = message
         self.response_message = response_message
-    
+        self.extra = extra
+
     def __init_subclass__(cls, on_field: str, **kwds: Any) -> None:
         super().__init_subclass__(**kwds)
         bot.Bot.client_event_callbacks[on_field].append(cls.new)
 
 
 class LoginEvent(ClientEvent, on_field="login"):
     """
```

### Comparing `KaruhaBot-0.2.0b2/karuha/event/command.py` & `KaruhaBot-0.2.0b3/karuha/event/command.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/karuha/event/message.py` & `KaruhaBot-0.2.0b3/karuha/event/message.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/karuha/event/plugin.py` & `KaruhaBot-0.2.0b3/karuha/event/plugin.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/karuha/exception.py` & `KaruhaBot-0.2.0b3/karuha/exception.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,38 @@
+import asyncio
 from typing import Optional
 
 from . import bot
 
 
 class KaruhaException(Exception):
     """base exception for all errors in Karuha module"""
     __slots__ = []
 
 
 class KaruhaRuntimeError(KaruhaException):
-    """unspecified chatbot run-time error"""
+    """unspecified run-time error"""
     __slots__ = []
 
 
 class KaruhaBotError(KaruhaException):
     """unspecified chatbot run-time error"""
     __slots__ = ["bot", "code"]
 
     def __init__(self, *args: object, bot: Optional["bot.Bot"] = None, code: Optional[int] = None) -> None:
         super().__init__(*args)
         self.bot = bot
         self.code = code
 
 
+class KaruhaTimeoutError(KaruhaRuntimeError, asyncio.TimeoutError):
+    """run-time error: timeout"""
+    __slots__ = []
+
+
 class KaruhaCommandError(KaruhaException):
     """command error"""
     __slots__ = ["name", "collection", "_command"]
 
     def __init__(
             self,
             *args: object,
@@ -43,15 +49,15 @@
     def command(self) -> Optional["AbstractCommand"]:
         if self._command is not None:
             return self._command
         elif self.collection is not None:
             return self.collection.commands.get(self.name)
 
 
-class KaruhaCommandCanceledError(KaruhaCommandError):
+class KaruhaCommandCanceledError(asyncio.CancelledError):
     """command cancelled"""
     __slots__ = []
 
 
 class KaruhaParserError(KaruhaException):
     """param parser error"""
     __slots__ = []
```

### Comparing `KaruhaBot-0.2.0b2/karuha/logger.py` & `KaruhaBot-0.2.0b3/karuha/logger.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/karuha/plugin_server.py` & `KaruhaBot-0.2.0b3/karuha/plugin_server.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/karuha/text/__init__.py` & `KaruhaBot-0.2.0b3/karuha/text/__init__.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/karuha/text/convert.py` & `KaruhaBot-0.2.0b3/karuha/text/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         if last < i.start:
             chain += text[last:i.start]
         last = i.end
         chain += _convert(text, i)
     if end < 0:
         end = len(text)
     if last < end:
-        chain += text[last:]
+        chain += text[last:end]
     return chain.take()
 
 
 def _convert_spans(text: str, spans: Optional[List[Span]], /, start: int, end: int) -> BaseText:
     if not spans:
         return PlainText(text=text[start:end])
     elif spans[0].start == start and spans[0].end == end:
```

### Comparing `KaruhaBot-0.2.0b2/karuha/text/drafty.py` & `KaruhaBot-0.2.0b3/karuha/text/drafty.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 from pydantic import BaseModel, NonNegativeInt
 from typing import Any, Dict, List, Literal, Optional, Union
 from typing_extensions import Self
 
 
-InlineType = Literal["BR", "CO", "FM", "RW", "HL", "DL", "EM", "ST", "HD"]
+InlineType = Literal["BR", "CO", "FM", "RW", "HL", "DL", "EM", "ST", "HD", "QQ"]
 ExtendType = Literal["AU", "BN", "EX", "FM", "HT", "IM", "LN", "MN", "RW", "VC", "VD"]
 
 
 class DraftyFormat(BaseModel, frozen=True):
     at: int = 0     # -1 means not applying any styling to text.
     len: NonNegativeInt = 0
     key: NonNegativeInt = 0
```

### Comparing `KaruhaBot-0.2.0b2/karuha/text/message.py` & `KaruhaBot-0.2.0b3/karuha/text/message.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/karuha/text/textchain.py` & `KaruhaBot-0.2.0b3/karuha/text/textchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,14 +269,35 @@
     type: Final[InlineType] = "HD"
 
 
 class Row(_Container):
     type: Final[InlineType] = "RW"
 
 
+class Quote(_Container):
+    type: Final[InlineType] = "QQ"
+
+    @property
+    def mention(self) -> Optional["Mention"]:
+        if not isinstance(self.content, TextChain) or not self.content:
+            return
+        mn = self.content[0]
+        assert isinstance(mn, Mention)
+        return mn
+
+    @property
+    def quote_content(self) -> Optional[BaseText]:
+        if not isinstance(self.content, TextChain):
+            return
+        elif len(self.content) == 2 and isinstance(self.content[1], PlainText):
+            return PlainText(str(self.content[1])[1:])
+        elif len(self.content) == 3:
+            return self.content[2]
+
+
 class Form(_Container):
     type: Final[InlineType] = "FM"
 
     su: bool = False
 
     def to_drafty(self) -> Drafty:
         if not self.su:
@@ -380,15 +401,15 @@
 
 class _Attachment(_ExtensionText):
     text: str = ""
     type: ExtendType
 
     mime: str
     name: Optional[str] = None
-    val: Optional[str] = None
+    val: Optional[Any] = None
     ref: Optional[str] = None
     size: Optional[int] = None
 
     @classmethod
     def from_bytes(
             cls,
             content: bytes,
@@ -454,20 +475,14 @@
         if isinstance(data, MutableMapping):
             for k, v in tuple(data.items()):
                 if isinstance(k, str) and isinstance(v, bytes) and k.startswith("raw_"):
                     data.pop(k)
                     data[k[4:]] = b64encode(v).decode("ascii")
         return data
 
-    @model_validator(mode="after")
-    def check_data(self) -> Self:
-        if self.ref is None and self.val is None:
-            raise ValueError("no data provided")
-        return self
-
     def get_data(self) -> Dict[str, Any]:
         return self.model_dump(exclude={"text", "type"}, exclude_none=True)
 
     def __repr__(self) -> str:
         name = self.__class__.__name__
         if self.ref:
             return f"<{name} from {self.ref}>"
```

### Comparing `KaruhaBot-0.2.0b2/karuha/utils/decode.py` & `KaruhaBot-0.2.0b3/karuha/utils/decode.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 from typing import Any, Dict, Mapping, Union
 
 from google.protobuf.internal import containers
 from google.protobuf.message import Message
-
-try:
-    import ujson as json
-except ImportError:  # pragma: no cover
-    import json
+from pydantic_core import from_json, to_json
 
 
 def load_json(obj: Union[str, bytes], **kwds: Any) -> Any:
     if not obj:
         return
-    return json.loads(obj, **kwds)
+    return from_json(obj, **kwds)
 
 
 def encode_mapping(data: Mapping[str, Any]) -> Dict[str, bytes]:
-    return {k: json.dumps(v).encode() for k, v in data.items()}
+    return {k: to_json(v) for k, v in data.items()}
 
 
 def decode_mapping(data: Mapping[str, bytes]) -> Dict[str, Any]:
-    return {k: json.loads(v) for k, v in data.items()}
+    return {k: from_json(v) for k, v in data.items()}
 
 
 def msg2dict(msg: Message) -> Dict[str, Any]:
     return _msg2obj(msg)
 
 
 def _msg2obj(msg: Any) -> Any:
```

### Comparing `KaruhaBot-0.2.0b2/karuha/utils/dispatcher.py` & `KaruhaBot-0.2.0b3/karuha/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/karuha/utils/event_catcher.py` & `KaruhaBot-0.2.0b3/karuha/utils/event_catcher.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/karuha/utils/proxy_propery.py` & `KaruhaBot-0.2.0b3/karuha/utils/proxy_propery.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/setup.py` & `KaruhaBot-0.2.0b3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,27 +43,28 @@
     
     author="Visecy",
     author_email="Visecy@visecy.org",
     maintainer="Ovizro",
     maintainer_email="Ovizro@visecy.org",
     license="Apache 2.0",
 
-    url="https://github.com/Ovizro/Karuha",
+    url="https://github.com/Visecy/Karuha",
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=[
         "typing_extensions>=4.0",
         "grpcio>=1.40.0",
         "tinode-grpc>=0.20.0b3",
         "pydantic>2.0",
         "aiofiles"
     ],
     extras_require={
         "image": ["pillow"],
-        "all": ["pillow"],
+        "data": ["greenback"],
+        "all": ["pillow", "greenback"],
     },
 
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `KaruhaBot-0.2.0b2/tests/test_bot.py` & `KaruhaBot-0.2.0b3/tests/test_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import asyncio
 
 from tinode_grpc import pb
 
 from karuha.bot import State
-from karuha.config import Bot as BotConfig
+from karuha.config import Bot as BotConfig, Server
 from karuha.event.bot import (CtrlEvent, DataEvent, InfoEvent, LeaveEvent,
                               LoginEvent, MetaEvent, PresEvent, PublishEvent,
                               SubscribeEvent)
 from karuha.exception import KaruhaBotError
 
-from .utils import TEST_TIME_OUT, AsyncBotTestCase, BotMock
+from .utils import TEST_TIMEOUT, AsyncBotTestCase, BotMock
 
 
 class TestBot(AsyncBotTestCase):
     bot = BotMock("test_bot", "basic", "123456", log_level="DEBUG")
 
     def test_bot_init(self) -> None:
         self.assertEqual(
             self.bot.config,
-            BotConfig(name="test_bot", schema="basic", secret="123456", user="usr")
+            BotConfig(name="test_bot", schema="basic", secret="123456")
         )
         self.assertEqual(
             self.bot.server,
-            None
+            Server()
         )
         self.assertTrue(self.bot.queue.empty())
         self.assertEqual(self.bot.state, State.running)
 
     async def test_server_message(self) -> None:
         with self.catchEvent(DataEvent) as catcher:
             message = pb.ServerData(
@@ -81,26 +81,26 @@
         bot = self.bot
 
         hi_task = asyncio.create_task(bot.hello())
         hi_msg = await bot.consum_message()
         self.assertIsInstance(hi_msg.hi, pb.ClientHi)
         tid = bot.confirm_message(build="tinode-mysql", ver="0.22")
         self.assertEqual(tid, hi_msg.hi.id)
-        await asyncio.wait_for(hi_task, TEST_TIME_OUT)
+        await asyncio.wait_for(hi_task, TEST_TIMEOUT)
 
         login_task = asyncio.create_task(bot.login())
         login_msg = await bot.consum_message()
         login_msg_inner = login_msg.login
         self.assertIsInstance(login_msg_inner, pb.ClientLogin)
         self.assertEqual(login_msg_inner.scheme, "basic")
         self.assertEqual(login_msg_inner.secret, b"123456")
-        tid = bot.confirm_message(user="user_test", token="token_test")
+        tid = bot.confirm_message(user="user_test", token="token_test", expires=1708360886000)
         self.assertEqual(tid, login_msg_inner.id)
         with self.catchEvent(LoginEvent) as catcher:
-            await asyncio.wait_for(login_task, TEST_TIME_OUT)
+            await asyncio.wait_for(login_task, TEST_TIMEOUT)
             e = await catcher.catch_event()
             self.assertEqual(e.client_message, login_msg_inner)
             self.assertIsNotNone(e.response_message)
 
         sub_msg = await bot.consum_message()
         sub_msg_inner = sub_msg.sub
         self.assertIsInstance(sub_msg_inner, pb.ClientSub)
@@ -116,38 +116,38 @@
         sub_msg = await bot.consum_message()
         sub_msg_inner = sub_msg.sub
         self.assertIsInstance(sub_msg_inner, pb.ClientSub)
         self.assertEqual(sub_msg_inner.topic, "topic_test")
         tid = bot.confirm_message(code=400)
         self.assertEqual(tid, sub_msg_inner.id)
         with self.assertRaises(KaruhaBotError):
-            await asyncio.wait_for(sub_task, TEST_TIME_OUT)
+            await asyncio.wait_for(sub_task, TEST_TIMEOUT)
         
         pub_task = asyncio.create_task(bot.publish("topic_test", "Hello world!"))
         pub_msg = await bot.consum_message()
         pub_msg_inner = pub_msg.pub
         self.assertIsInstance(pub_msg_inner, pb.ClientPub)
         self.assertEqual(pub_msg_inner.topic, "topic_test")
         self.assertEqual(pub_msg_inner.content, b"\"Hello world!\"")
         tid = bot.confirm_message()
         self.assertEqual(tid, pub_msg_inner.id)
         with self.catchEvent(PublishEvent) as catcher:
-            await asyncio.wait_for(pub_task, TEST_TIME_OUT)
+            await asyncio.wait_for(pub_task, TEST_TIMEOUT)
             e = await catcher.catch_event()
             self.assertIsNotNone(e.response_message)
         
         leave_task = asyncio.create_task(bot.leave("topic_test"))
         leave_msg = await bot.consum_message()
         leave_msg_inner = leave_msg.leave
         self.assertIsInstance(leave_msg_inner, pb.ClientLeave)
         self.assertEqual(leave_msg_inner.topic, "topic_test")
         tid = bot.confirm_message()
         self.assertEqual(tid, leave_msg_inner.id)
         with self.catchEvent(LeaveEvent) as catcher:
-            await asyncio.wait_for(leave_task, TEST_TIME_OUT)
+            await asyncio.wait_for(leave_task, TEST_TIMEOUT)
             e = await catcher.catch_event()
             self.assertIsNotNone(e.response_message)
         
     async def test_restart(self) -> None:
         self.bot.restart()
         self.assertEqual(self.bot.state, State.restarting)
         await self.bot.wait_state(State.running)
```

### Comparing `KaruhaBot-0.2.0b2/tests/test_command.py` & `KaruhaBot-0.2.0b3/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/tests/test_command_run.py` & `KaruhaBot-0.2.0b3/tests/test_command_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 def has_return() -> int:
     return 1
 
 
 @on(CommandPrepareEvent)
 def command_prepare(event: CommandPrepareEvent) -> None:
     if event.command is should_cancel:
-        raise KaruhaCommandCanceledError(name=event.command.name, command=event.command)
+        raise KaruhaCommandCanceledError
 
 
 class TestCommandRun(AsyncBotTestCase):
     command_collection = get_collection()
 
     async def test_unexist(self) -> None:
         set_collection(self.command_collection)
```

### Comparing `KaruhaBot-0.2.0b2/tests/test_event.py` & `KaruhaBot-0.2.0b3/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b2/tests/test_session.py` & `KaruhaBot-0.2.0b3/tests/test_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 
 from karuha.command import MessageSession
 from karuha.event.message import get_message_lock
 from karuha.text import Drafty, PlainText, Button, File, Image, drafty2text
 
-from .utils import AsyncBotTestCase, new_test_message, TEST_TIME_OUT
+from .utils import AsyncBotTestCase, new_test_message, TEST_TIMEOUT
 
 
 class TestSession(AsyncBotTestCase):
     async def test_send(self) -> None:
         ss = MessageSession(self.bot, new_test_message())
         self.assertEqual(ss.topic, "test")
         self.assertEqual(ss.last_message.user_id, "user")
@@ -16,20 +16,20 @@
         self.assertEqual(len(ss.messages), 1)
 
         send_task = asyncio.create_task(ss.send(PlainText("test")))
         msg = await self.bot.consum_message()
         self.assertTrue(msg.pub)
         pubmsg = msg.pub
         self.bot.confirm_message(pubmsg.id, seq=0)
-        await asyncio.wait_for(send_task, timeout=TEST_TIME_OUT)
+        await asyncio.wait_for(send_task, timeout=TEST_TIMEOUT)
 
         wait_task = asyncio.create_task(ss.wait_reply())
         self.bot.receive_content(b'{"txt": "test1"}', topic="test1")
         self.bot.receive_content(b'{"txt": "test"}', from_user_id="user1")
-        msg = await asyncio.wait_for(wait_task, timeout=TEST_TIME_OUT)
+        msg = await asyncio.wait_for(wait_task, timeout=TEST_TIMEOUT)
         self.assertEqual(msg.content, b'{"txt": "test"}')
 
     async def test_form(self) -> None:
         ss = MessageSession(self.bot, new_test_message())
         form_task = asyncio.create_task(
             ss.send_form(
                 "title", "Yes", Button(text="No"), Button(text="Cancel", name="cancel")
@@ -40,15 +40,15 @@
         self.assertTrue(msg.pub)
         pubmsg = msg.pub
         self.bot.confirm_message(pubmsg.id, seq=114)
         self.bot.receive_content(
             b'{"ent":[{"data":{"mime":"application/json","val":{"resp":{"yes":1},"seq":114}},'
             b'"tp":"EX"}],"fmt":[{"at":-1}],"txt":"Yes"}',
         )
-        bid = await asyncio.wait_for(form_task, timeout=TEST_TIME_OUT)
+        bid = await asyncio.wait_for(form_task, timeout=TEST_TIMEOUT)
         self.assertEqual(bid, 0)
 
     async def test_form1(self) -> None:
         ss = MessageSession(self.bot, new_test_message())
         form_task = asyncio.create_task(
             ss.send_form(
                 "title", "Yes", Button(text="No"), Button(text="Cancel", name="cancel")
@@ -59,15 +59,15 @@
         self.assertTrue(msg.pub)
         pubmsg = msg.pub
         self.bot.confirm_message(pubmsg.id, seq=114)
         self.bot.receive_content(
             b'{"ent":[{"data":{"mime":"application/json","val":{"seq":114}},"tp":"EX"}],'
             b'"fmt":[{"at":-1}],"txt":"No"}',
         )
-        bid = await asyncio.wait_for(form_task, timeout=TEST_TIME_OUT)
+        bid = await asyncio.wait_for(form_task, timeout=TEST_TIMEOUT)
         self.assertEqual(bid, 1)
 
     async def test_form2(self) -> None:
         ss = MessageSession(self.bot, new_test_message())
         form_task = asyncio.create_task(
             ss.send_form(
                 "title",
@@ -81,15 +81,15 @@
         self.assertTrue(msg.pub)
         pubmsg = msg.pub
         self.bot.confirm_message(pubmsg.id, seq=114)
         self.bot.receive_content(
             b'{"ent":[{"data":{"mime":"application/json","val":{"resp":{"cancel":"cancel"},'
             b'"seq":114}},"tp":"EX"}],"fmt":[{"at":-1}],"txt":"Cancel"}',
         )
-        bid = await asyncio.wait_for(form_task, timeout=TEST_TIME_OUT)
+        bid = await asyncio.wait_for(form_task, timeout=TEST_TIMEOUT)
         self.assertEqual(bid, 2)
     
     async def test_file(self) -> None:
         ss = MessageSession(self.bot, new_test_message())
         file_task = asyncio.create_task(ss.send_file("karuha/version.py"))
         msg = await self.bot.consum_message()
         self.assertTrue(msg.pub)
@@ -97,23 +97,23 @@
         df = Drafty.model_validate_json(pubmsg.content)
         self.assertEqual(df.txt, '')
         ft = drafty2text(df)
         assert isinstance(ft, File)
         self.assertEqual(ft.name, 'version.py')
         self.assertIsNotNone(ft.val)
         self.bot.confirm_message(pubmsg.id, seq=0)
-        await asyncio.wait_for(file_task, timeout=TEST_TIME_OUT)
+        await asyncio.wait_for(file_task, timeout=TEST_TIMEOUT)
     
     async def test_image(self) -> None:
         ss = MessageSession(self.bot, new_test_message())
         image_task = asyncio.create_task(ss.send_image("docs/img/tw_icon-karuha2.png"))
         msg = await self.bot.consum_message()
         self.assertTrue(msg.pub)
         pubmsg = msg.pub
         df = Drafty.model_validate_json(pubmsg.content)
         self.assertEqual(df.txt, '')
         ft = drafty2text(df)
         assert isinstance(ft, Image)
         self.assertEqual(ft.name, 'tw_icon-karuha2.png')
         self.assertIsNotNone(ft.val)
         self.bot.confirm_message(pubmsg.id, seq=0)
-        await asyncio.wait_for(image_task, timeout=TEST_TIME_OUT)
+        await asyncio.wait_for(image_task, timeout=TEST_TIMEOUT)
```

### Comparing `KaruhaBot-0.2.0b2/tests/test_text.py` & `KaruhaBot-0.2.0b3/tests/test_text.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest import TestCase
 
 from karuha.text import PlainText, Form, Drafty, drafty2tree, drafty2text
-from karuha.text.textchain import File, TextChain, Bold, Hidden
+from karuha.text.textchain import File, Mention, Quote, TextChain, Bold, Hidden
 from karuha.text.convert import eval_spans, to_span_tree
 from karuha.event.message import MessageEvent
 
 from .utils import bot_mock, new_test_message
 
 
 example1 = Drafty.model_validate_json(
@@ -188,7 +188,31 @@
                     }
                 ],
                 "fmt": [{"at": -1}],
             }
         )
         f = drafty2text(df)
         self.assertIsInstance(f, File)
+    
+    def test_quote(self) -> None:
+        df = Drafty.model_validate(
+            {
+                "txt": "user quote textuser text",
+                "fmt": [
+                    {"len": 4},
+                    {"at": 4, "len": 1, "tp": "BR"},
+                    {"len": 15, "tp": "QQ"}
+                ],
+                "ent": [
+                    {"tp": "MN", "data": {"val": "user_id"}}
+                ]
+            }
+        )
+        t = drafty2text(df)
+        assert isinstance(t, TextChain)
+        self.assertEqual(len(t), 2)
+        qq = t[0]
+        assert isinstance(qq, Quote) and isinstance(qq.content, TextChain)
+        self.assertEqual(len(qq.content), 2)
+        self.assertEqual(qq.content[0], Mention(text="user", val="user_id"))
+        self.assertEqual(qq.content[1], PlainText("\nquote text"))
+        self.assertEqual(t[1], PlainText("user text"))
```

### Comparing `KaruhaBot-0.2.0b2/tests/utils.py` & `KaruhaBot-0.2.0b3/tests/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import asyncio
 import json
 from time import time
 from types import coroutine
-from typing import Any, Dict, Generator, Optional
+from typing import Any, Awaitable, Dict, Generator, Optional
 from unittest import IsolatedAsyncioTestCase
 
 from grpc import ChannelConnectivity
 from grpc import aio as grpc_aio
 from tinode_grpc import pb
 from typing_extensions import Self
 
 from karuha import async_run, try_add_bot
 from karuha.bot import Bot, State
 from karuha.command.collection import new_collection
 from karuha.command.command import CommandMessage, FunctionCommand
 from karuha.config import Server as ServerConfig
 from karuha.config import init_config
 from karuha.event import T_Event
+from karuha.store import T
 from karuha.text.message import Message
 from karuha.utils.event_catcher import EventCatcher as _EventCatcher
 
 
-TEST_TIME_OUT = 5
+TEST_TIMEOUT = 3
 
 
 @coroutine
 def run_forever() -> Generator[None, None, None]:
     while True:
         yield
 
@@ -82,14 +83,15 @@
         raise NotImplementedError
 
 
 class BotMock(Bot):
     __slots__ = []
     
     def receive_message(self, message: pb.ServerMsg, /) -> None:
+        self.logger.debug(f"in: {message}")
         for desc, msg in message.ListFields():
             for e in self.server_event_callbacks[desc.name]:
                 e(self, msg)
     
     def receive_content(
             self,
             content: bytes,
@@ -108,27 +110,32 @@
                     head=head.copy(),
                     content=content,
                 )
             )
         )
     
     async def consum_message(self) -> pb.ClientMsg:
-        return await asyncio.wait_for(self.queue.get(), TEST_TIME_OUT)
+        return await asyncio.wait_for(self.queue.get(), TEST_TIMEOUT)
     
     def clear_message(self) -> None:
         while not self.queue.empty():
             self.queue.get_nowait()
     
     def assert_message_nowait(self, message: pb.ClientMsg, /) -> None:
         assert self.queue.get_nowait() == message
     
     async def assert_message(self, message: pb.ClientMsg, /) -> None:
         assert await self.consum_message() == message
+    
+    async def assert_note_read(self, topic: str, seq_id: int, /) -> None:
+        assert await self.consum_message() == pb.ClientMsg(
+            note_read=pb.ClientNote(topic=topic, seq_id=seq_id, what=pb.READ)
+        )
 
-    async def wait_state(self, state: State, /, timeout: float = TEST_TIME_OUT) -> None:
+    async def wait_state(self, state: State, /, timeout: float = TEST_TIMEOUT) -> None:
         start = time()
         while self.state != state:
             await asyncio.sleep(0)
             if time() - start > timeout:
                 raise TimeoutError(f"bot state has not changed to {state}")
 
     async def wait_init(self) -> None:
@@ -139,18 +146,22 @@
         login_msg = await self.consum_message()
         assert login_msg.login
         self.confirm_message(login_msg.login.id, user="usr")
         sub_msg = await self.consum_message()
         assert sub_msg.sub and sub_msg.sub.topic == "me"
         self.confirm_message(sub_msg.sub.id)
     
+    def get_latest_tid(self) -> str:
+        print(self._wait_list)
+        assert len(self._wait_list) == 1
+        return tuple(self._wait_list.keys())[0]
+    
     def confirm_message(self, tid: Optional[str] = None, code: int = 200, **params: Any) -> str:
         if tid is None:
-            assert len(self._wait_list) == 1
-            tid = list(self._wait_list.keys())[0]
+            tid = self.get_latest_tid()
         if code < 200 or code >= 400:
             text = "test error"
         else:
             text = "OK"
         self._wait_list[tid].set_result(
             pb.ServerCtrl(
                 id=tid,
@@ -179,15 +190,15 @@
 
 bot_mock = BotMock("test", "basic", "123456", log_level="DEBUG")
 
 
 class EventCatcher(_EventCatcher[T_Event]):
     __slots__ = []
 
-    async def catch_event(self, timeout: float = TEST_TIME_OUT) -> T_Event:
+    async def catch_event(self, timeout: float = TEST_TIMEOUT) -> T_Event:
         return await super().catch_event(timeout)
 
 
 class AsyncBotTestCase(IsolatedAsyncioTestCase):
     bot = bot_mock
     config = init_config(log_level="DEBUG")
 
@@ -204,14 +215,17 @@
     catchEvent = EventCatcher
 
     async def assertBotMessage(self, message: pb.ClientMsg, /) -> None:
         await self.bot.assert_message(message)
     
     def assertBotMessageNowait(self, message: pb.ClientMsg, /) -> None:
         self.bot.assert_message_nowait(message)
+    
+    async def wait_for(self, future: Awaitable[T], /, timeout: Optional[float] = TEST_TIMEOUT) -> T:
+        return await asyncio.wait_for(future, timeout)
 
 
 def new_test_message(content: bytes = b"\"test\"") -> Message:
     return Message.new(
         bot_mock, "test", "user", 1, {}, content
     )
```

