# Comparing `tmp/neon-utils-1.9.2a1.tar.gz` & `tmp/neon-utils-1.9.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-utils-1.9.2a1.tar", last modified: Thu Mar  7 23:25:06 2024, max compression
+gzip compressed data, was "neon-utils-1.9.2a2.tar", last modified: Tue Apr  2 00:27:32 2024, max compression
```

## Comparing `neon-utils-1.9.2a1.tar` & `neon-utils-1.9.2a2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.273216 neon-utils-1.9.2a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-07 23:25:06.273216 neon-utils-1.9.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.265216 neon-utils-1.9.2a1/neon_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/authentication_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    68558 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/configuration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.265216 neon-utils-1.9.2a1/neon_utils/default_configurations/
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/default_configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/default_configurations/default_user_conf.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16908 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/hana_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/language_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/location_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/messagebus_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/mq_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/net_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/packaging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/process_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.257216 neon-utils-1.9.2a1/neon_utils/res/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.265216 neon-utils-1.9.2a1/neon_utils/res/snd/
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/res/snd/acknowledge.mp3
--rw-r--r--   0 runner    (1001) docker     (127)   428660 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/res/snd/loaded.wav
--rw-r--r--   0 runner    (1001) docker     (127)    67090 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/res/snd/start_listening.wav
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.257216 neon-utils-1.9.2a1/neon_utils/res/text/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.265216 neon-utils-1.9.2a1/neon_utils/res/text/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/res/text/en-us/neon.voc
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/res/text/en-us/no.voc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/res/text/en-us/stop.voc
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/res/text/en-us/yes.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.265216 neon-utils-1.9.2a1/neon_utils/res/ui/
--rw-r--r--   0 runner    (1001) docker     (127)    11747 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/res/ui/neon_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/signal_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.269216 neon-utils-1.9.2a1/neon_utils/skills/
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/skills/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9762 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/skills/common_message_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/skills/common_play_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/skills/common_query_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/skills/instructor_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/skills/kiosk_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/skills/mycroft_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)    38699 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/skills/neon_fallback_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)    38468 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/skills/neon_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/skills/skill_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/socket_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/validator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/neon_utils/web_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.265216 neon-utils-1.9.2a1/neon_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-07 23:25:06.000000 neon-utils-1.9.2a1/neon_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-07 23:25:06.000000 neon-utils-1.9.2a1/neon_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 23:25:06.000000 neon-utils-1.9.2a1/neon_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-07 23:25:06.000000 neon-utils-1.9.2a1/neon_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-07 23:25:06.000000 neon-utils-1.9.2a1/neon_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-07 23:25:06.000000 neon-utils-1.9.2a1/neon_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 23:25:06.273216 neon-utils-1.9.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.273216 neon-utils-1.9.2a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/authentication_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/cache_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    63829 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/configuration_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/file_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/hana_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/language_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/location_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/log_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/message_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/messagebus_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/metric_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/mq_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    57964 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/neon_skill_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/net_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/packaging_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/parse_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/search_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/signal_util_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.273216 neon-utils-1.9.2a1/tests/skills/
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/skills/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.273216 neon-utils-1.9.2a1/tests/skills/test_skill/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/skills/test_skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/skills/test_skill/settingsmeta.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/socket_utils_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/user_util_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:25:06.273216 neon-utils-1.9.2a1/tests/valid_skill/
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/valid_skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/validator_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-03-07 23:24:58.000000 neon-utils-1.9.2a1/tests/web_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.469874 neon-utils-1.9.2a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-02 00:27:32.469874 neon-utils-1.9.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.461874 neon-utils-1.9.2a2/neon_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/authentication_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68558 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.461874 neon-utils-1.9.2a2/neon_utils/default_configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/default_configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/default_configurations/default_user_conf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16908 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/hana_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/language_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/location_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/messagebus_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/mq_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/packaging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/process_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.457874 neon-utils-1.9.2a2/neon_utils/res/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.461874 neon-utils-1.9.2a2/neon_utils/res/snd/
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/res/snd/acknowledge.mp3
+-rw-r--r--   0 runner    (1001) docker     (127)   428660 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/res/snd/loaded.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    67090 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/res/snd/start_listening.wav
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.457874 neon-utils-1.9.2a2/neon_utils/res/text/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.465874 neon-utils-1.9.2a2/neon_utils/res/text/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/res/text/en-us/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/res/text/en-us/no.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/res/text/en-us/stop.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/res/text/en-us/yes.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.465874 neon-utils-1.9.2a2/neon_utils/res/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    11747 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/res/ui/neon_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/signal_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.465874 neon-utils-1.9.2a2/neon_utils/skills/
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/skills/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9762 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/skills/common_message_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/skills/common_play_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/skills/common_query_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/skills/instructor_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/skills/kiosk_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/skills/mycroft_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38699 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/skills/neon_fallback_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38468 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/skills/neon_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/skills/skill_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/socket_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/validator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/neon_utils/web_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.461874 neon-utils-1.9.2a2/neon_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-02 00:27:32.000000 neon-utils-1.9.2a2/neon_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-02 00:27:32.000000 neon-utils-1.9.2a2/neon_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:27:32.000000 neon-utils-1.9.2a2/neon_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 00:27:32.000000 neon-utils-1.9.2a2/neon_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-02 00:27:32.000000 neon-utils-1.9.2a2/neon_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 00:27:32.000000 neon-utils-1.9.2a2/neon_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:27:32.469874 neon-utils-1.9.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.469874 neon-utils-1.9.2a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/authentication_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/cache_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63829 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/configuration_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/file_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/hana_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/language_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/location_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/log_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/message_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/messagebus_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/metric_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/mq_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57964 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/neon_skill_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/net_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/packaging_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/parse_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/search_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/signal_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.469874 neon-utils-1.9.2a2/tests/skills/
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/skills/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.469874 neon-utils-1.9.2a2/tests/skills/test_skill/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/skills/test_skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/skills/test_skill/settingsmeta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/socket_utils_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/user_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:27:32.469874 neon-utils-1.9.2a2/tests/valid_skill/
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/valid_skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/validator_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-02 00:27:26.000000 neon-utils-1.9.2a2/tests/web_util_tests.py
```

### Comparing `neon-utils-1.9.2a1/LICENSE.md` & `neon-utils-1.9.2a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/PKG-INFO` & `neon-utils-1.9.2a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-utils
-Version: 1.9.2a1
+Version: 1.9.2a2
 Summary: Utilities for NeonAI
 Home-page: https://github.com/neongeckocom/neon-skill-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-utils-1.9.2a1/neon_utils/__init__.py` & `neon-utils-1.9.2a2/neon_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/authentication_utils.py` & `neon-utils-1.9.2a2/neon_utils/authentication_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/cache_utils.py` & `neon-utils-1.9.2a2/neon_utils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/configuration_utils.py` & `neon-utils-1.9.2a2/neon_utils/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/decorators.py` & `neon-utils-1.9.2a2/neon_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/default_configurations/__init__.py` & `neon-utils-1.9.2a2/neon_utils/default_configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/default_configurations/default_user_conf.yml` & `neon-utils-1.9.2a2/neon_utils/default_configurations/default_user_conf.yml`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/file_utils.py` & `neon-utils-1.9.2a2/neon_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/hana_utils.py` & `neon-utils-1.9.2a2/neon_utils/hana_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/language_utils.py` & `neon-utils-1.9.2a2/neon_utils/language_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/location_utils.py` & `neon-utils-1.9.2a2/neon_utils/location_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/log_utils.py` & `neon-utils-1.9.2a2/neon_utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/logger.py` & `neon-utils-1.9.2a2/neon_utils/logger.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/message_utils.py` & `neon-utils-1.9.2a2/neon_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/messagebus_utils.py` & `neon-utils-1.9.2a2/neon_utils/messagebus_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/metrics_utils.py` & `neon-utils-1.9.2a2/neon_utils/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/mq_utils.py` & `neon-utils-1.9.2a2/neon_utils/mq_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/net_utils.py` & `neon-utils-1.9.2a2/neon_utils/net_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/packaging_utils.py` & `neon-utils-1.9.2a2/neon_utils/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/parse_utils.py` & `neon-utils-1.9.2a2/neon_utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/process_utils.py` & `neon-utils-1.9.2a2/neon_utils/process_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/res/snd/acknowledge.mp3` & `neon-utils-1.9.2a2/neon_utils/res/snd/acknowledge.mp3`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/res/snd/loaded.wav` & `neon-utils-1.9.2a2/neon_utils/res/snd/loaded.wav`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/res/snd/start_listening.wav` & `neon-utils-1.9.2a2/neon_utils/res/snd/start_listening.wav`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/res/ui/neon_logo.png` & `neon-utils-1.9.2a2/neon_utils/res/ui/neon_logo.png`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/search_utils.py` & `neon-utils-1.9.2a2/neon_utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/signal_utils.py` & `neon-utils-1.9.2a2/neon_utils/signal_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/skills/__init__.py` & `neon-utils-1.9.2a2/neon_utils/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/skills/common_message_skill.py` & `neon-utils-1.9.2a2/neon_utils/skills/common_message_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/skills/common_play_skill.py` & `neon-utils-1.9.2a2/neon_utils/skills/common_play_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/skills/common_query_skill.py` & `neon-utils-1.9.2a2/neon_utils/skills/common_query_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/skills/instructor_skill.py` & `neon-utils-1.9.2a2/neon_utils/skills/instructor_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/skills/kiosk_skill.py` & `neon-utils-1.9.2a2/neon_utils/skills/kiosk_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/skills/mycroft_skill.py` & `neon-utils-1.9.2a2/neon_utils/skills/mycroft_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/skills/neon_fallback_skill.py` & `neon-utils-1.9.2a2/neon_utils/skills/neon_fallback_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/skills/neon_skill.py` & `neon-utils-1.9.2a2/neon_utils/skills/neon_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/skills/skill_gui.py` & `neon-utils-1.9.2a2/neon_utils/skills/skill_gui.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/socket_utils.py` & `neon-utils-1.9.2a2/neon_utils/socket_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/user_utils.py` & `neon-utils-1.9.2a2/neon_utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/validator_utils.py` & `neon-utils-1.9.2a2/neon_utils/validator_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils/web_utils.py` & `neon-utils-1.9.2a2/neon_utils/web_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils.egg-info/PKG-INFO` & `neon-utils-1.9.2a2/neon_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-utils
-Version: 1.9.2a1
+Version: 1.9.2a2
 Summary: Utilities for NeonAI
 Home-page: https://github.com/neongeckocom/neon-skill-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-utils-1.9.2a1/neon_utils.egg-info/SOURCES.txt` & `neon-utils-1.9.2a2/neon_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/neon_utils.egg-info/requires.txt` & `neon-utils-1.9.2a2/neon_utils.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ovos-bus-client~=0.0.3
 combo-lock~=0.2
 pendulum~=2.1
 timezonefinder~=5.2
 nltk~=3.5
 pyyaml<7.0,>=5.4
 ovos-lingua-franca~=0.4
-ovos_utils~=0.0.35
+ovos_utils>=0.0.35,~=0.0
 geopy~=2.1
 ovos-config~=0.0.9
 ovos-workshop~=0.0.15
 
 [audio]
 soundfile~=0.10
 librosa<0.10,~=0.8
```

### Comparing `neon-utils-1.9.2a1/setup.py` & `neon-utils-1.9.2a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/__init__.py` & `neon-utils-1.9.2a2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/authentication_util_tests.py` & `neon-utils-1.9.2a2/tests/authentication_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/cache_util_tests.py` & `neon-utils-1.9.2a2/tests/cache_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/configuration_util_tests.py` & `neon-utils-1.9.2a2/tests/configuration_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/file_util_tests.py` & `neon-utils-1.9.2a2/tests/file_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/hana_util_tests.py` & `neon-utils-1.9.2a2/tests/hana_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/language_util_tests.py` & `neon-utils-1.9.2a2/tests/language_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/location_util_tests.py` & `neon-utils-1.9.2a2/tests/location_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/log_util_tests.py` & `neon-utils-1.9.2a2/tests/log_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/message_util_tests.py` & `neon-utils-1.9.2a2/tests/message_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/messagebus_util_tests.py` & `neon-utils-1.9.2a2/tests/messagebus_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/metric_util_tests.py` & `neon-utils-1.9.2a2/tests/metric_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/mq_util_tests.py` & `neon-utils-1.9.2a2/tests/mq_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/neon_skill_tests.py` & `neon-utils-1.9.2a2/tests/neon_skill_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/net_util_tests.py` & `neon-utils-1.9.2a2/tests/net_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/packaging_util_tests.py` & `neon-utils-1.9.2a2/tests/packaging_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/parse_util_tests.py` & `neon-utils-1.9.2a2/tests/parse_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/search_util_tests.py` & `neon-utils-1.9.2a2/tests/search_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/signal_util_tests.py` & `neon-utils-1.9.2a2/tests/signal_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/skills/__init__.py` & `neon-utils-1.9.2a2/tests/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/skills/test_skill/__init__.py` & `neon-utils-1.9.2a2/tests/skills/test_skill/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/socket_utils_tests.py` & `neon-utils-1.9.2a2/tests/socket_utils_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/user_util_tests.py` & `neon-utils-1.9.2a2/tests/user_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/valid_skill/__init__.py` & `neon-utils-1.9.2a2/tests/valid_skill/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/validator_util_tests.py` & `neon-utils-1.9.2a2/tests/validator_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a1/tests/web_util_tests.py` & `neon-utils-1.9.2a2/tests/web_util_tests.py`

 * *Files identical despite different names*

