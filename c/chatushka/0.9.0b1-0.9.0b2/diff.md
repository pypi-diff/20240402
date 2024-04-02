# Comparing `tmp/chatushka-0.9.0b1.tar.gz` & `tmp/chatushka-0.9.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatushka-0.9.0b1.tar", max compression
+gzip compressed data, was "chatushka-0.9.0b2.tar", max compression
```

## Comparing `chatushka-0.9.0b1.tar` & `chatushka-0.9.0b2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       73 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/__init__.py
--rw-r--r--   0        0        0      124 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/__main__.py
--rw-r--r--   0        0        0       73 2022-03-10 13:04:41.017312 chatushka-0.9.0b1/chatushka/__version__.py
--rw-r--r--   0        0        0        0 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/__init__.py
--rw-r--r--   0        0        0     1307 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/data/eight_ball.yaml
--rw-r--r--   0        0        0     3058 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/data/lukashenko.txt
--rw-r--r--   0        0        0        0 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/internal/__init__.py
--rw-r--r--   0        0        0      696 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/internal/data_dir.py
--rw-r--r--   0        0        0     2940 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/internal/mute.py
--rw-r--r--   0        0        0     1168 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/main.py
--rw-r--r--   0        0        0      607 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/matchers/__init__.py
--rw-r--r--   0        0        0      454 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/matchers/admin/__init__.py
--rw-r--r--   0        0        0     1592 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/matchers/admin/mute.py
--rw-r--r--   0        0        0     1680 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/matchers/admin/pin.py
--rw-r--r--   0        0        0      914 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/matchers/bobuk_jokes.py
--rw-r--r--   0        0        0     1562 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/matchers/eight_ball.py
--rw-r--r--   0        0        0     1324 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/matchers/helpers.py
--rw-r--r--   0        0        0      871 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/matchers/lukashenko.py
--rw-r--r--   0        0        0     1600 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/matchers/suicide.py
--rw-r--r--   0        0        0      678 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/matchers/welcoming.py
--rw-r--r--   0        0        0        0 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/models/__init__.py
--rw-r--r--   0        0        0      501 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/bot/settings.py
--rw-r--r--   0        0        0        0 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/__init__.py
--rw-r--r--   0        0        0     3937 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/bot.py
--rw-r--r--   0        0        0      645 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/matchers/__init__.py
--rw-r--r--   0        0        0     4570 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/matchers/base.py
--rw-r--r--   0        0        0      947 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/matchers/chat_users_movements.py
--rw-r--r--   0        0        0     2071 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/matchers/commands.py
--rw-r--r--   0        0        0      347 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/matchers/cron.py
--rw-r--r--   0        0        0      681 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/matchers/events.py
--rw-r--r--   0        0        0      774 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/matchers/regex.py
--rw-r--r--   0        0        0      533 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/models.py
--rw-r--r--   0        0        0     1164 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/protocols.py
--rw-r--r--   0        0        0        0 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/services/__init__.py
--rw-r--r--   0        0        0     1727 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/services/base.py
--rw-r--r--   0        0        0        0 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/services/mongodb/__init__.py
--rw-r--r--   0        0        0      206 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/services/mongodb/settings.py
--rw-r--r--   0        0        0      819 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/services/mongodb/utils.py
--rw-r--r--   0        0        0     1036 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/services/mongodb/wrapper.py
--rw-r--r--   0        0        0        0 2022-03-10 13:04:40.929306 chatushka-0.9.0b1/chatushka/core/transports/__init__.py
--rw-r--r--   0        0        0     2553 2022-03-10 13:04:40.933306 chatushka-0.9.0b1/chatushka/core/transports/models.py
--rw-r--r--   0        0        0     5217 2022-03-10 13:04:40.933306 chatushka-0.9.0b1/chatushka/core/transports/telegram_bot_api.py
--rw-r--r--   0        0        0      421 2022-03-10 13:04:40.933306 chatushka-0.9.0b1/chatushka/core/transports/utils.py
--rw-r--r--   0        0        0      528 2022-03-10 13:04:40.933306 chatushka-0.9.0b1/chatushka/core/utils.py
--rw-r--r--   0        0        0        0 2022-03-10 13:04:40.933306 chatushka-0.9.0b1/chatushka/webui/__init__.py
--rw-r--r--   0        0        0        0 2022-03-10 13:04:40.933306 chatushka-0.9.0b1/chatushka/webui/routes/__init__.py
--rw-r--r--   0        0        0     1512 2022-03-10 13:04:41.017312 chatushka-0.9.0b1/pyproject.toml
--rw-r--r--   0        0        0      480 2022-03-10 13:04:40.933306 chatushka-0.9.0b1/readme.md
--rw-r--r--   0        0        0     1640 2022-03-10 13:04:49.451110 chatushka-0.9.0b1/setup.py
--rw-r--r--   0        0        0     1202 2022-03-10 13:04:49.451449 chatushka-0.9.0b1/PKG-INFO
+-rw-r--r--   0        0        0       73 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/__init__.py
+-rw-r--r--   0        0        0      124 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/__main__.py
+-rw-r--r--   0        0        0       73 2022-03-10 17:08:52.218949 chatushka-0.9.0b2/chatushka/__version__.py
+-rw-r--r--   0        0        0        0 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/__init__.py
+-rw-r--r--   0        0        0     1307 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/data/eight_ball.yaml
+-rw-r--r--   0        0        0     3058 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/data/lukashenko.txt
+-rw-r--r--   0        0        0        0 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/internal/__init__.py
+-rw-r--r--   0        0        0      696 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/internal/data_dir.py
+-rw-r--r--   0        0        0     2940 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/internal/mute.py
+-rw-r--r--   0        0        0     1168 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/main.py
+-rw-r--r--   0        0        0      607 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/matchers/__init__.py
+-rw-r--r--   0        0        0      454 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/matchers/admin/__init__.py
+-rw-r--r--   0        0        0     1592 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/matchers/admin/mute.py
+-rw-r--r--   0        0        0     1680 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/matchers/admin/pin.py
+-rw-r--r--   0        0        0      914 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/matchers/bobuk_jokes.py
+-rw-r--r--   0        0        0     1562 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/matchers/eight_ball.py
+-rw-r--r--   0        0        0     1324 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/matchers/helpers.py
+-rw-r--r--   0        0        0      871 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/matchers/lukashenko.py
+-rw-r--r--   0        0        0     1600 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/matchers/suicide.py
+-rw-r--r--   0        0        0      678 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/matchers/welcoming.py
+-rw-r--r--   0        0        0        0 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/models/__init__.py
+-rw-r--r--   0        0        0      501 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/bot/settings.py
+-rw-r--r--   0        0        0        0 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/core/__init__.py
+-rw-r--r--   0        0        0     3937 2022-03-10 17:08:52.122944 chatushka-0.9.0b2/chatushka/core/bot.py
+-rw-r--r--   0        0        0      645 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/matchers/__init__.py
+-rw-r--r--   0        0        0     4570 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/matchers/base.py
+-rw-r--r--   0        0        0     1034 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/matchers/chat_users_movements.py
+-rw-r--r--   0        0        0     2071 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/matchers/commands.py
+-rw-r--r--   0        0        0      347 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/matchers/cron.py
+-rw-r--r--   0        0        0      681 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/matchers/events.py
+-rw-r--r--   0        0        0      774 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/matchers/regex.py
+-rw-r--r--   0        0        0      533 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/models.py
+-rw-r--r--   0        0        0     1164 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/protocols.py
+-rw-r--r--   0        0        0        0 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/services/__init__.py
+-rw-r--r--   0        0        0     1727 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/services/base.py
+-rw-r--r--   0        0        0        0 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/services/mongodb/__init__.py
+-rw-r--r--   0        0        0      206 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/services/mongodb/settings.py
+-rw-r--r--   0        0        0      819 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/services/mongodb/utils.py
+-rw-r--r--   0        0        0     1036 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/services/mongodb/wrapper.py
+-rw-r--r--   0        0        0        0 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/transports/__init__.py
+-rw-r--r--   0        0        0     2553 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/transports/models.py
+-rw-r--r--   0        0        0     5217 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/transports/telegram_bot_api.py
+-rw-r--r--   0        0        0      421 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/transports/utils.py
+-rw-r--r--   0        0        0      528 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/core/utils.py
+-rw-r--r--   0        0        0        0 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/webui/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/chatushka/webui/routes/__init__.py
+-rw-r--r--   0        0        0     1512 2022-03-10 17:08:52.218949 chatushka-0.9.0b2/pyproject.toml
+-rw-r--r--   0        0        0      480 2022-03-10 17:08:52.126944 chatushka-0.9.0b2/readme.md
+-rw-r--r--   0        0        0     1640 2022-03-10 17:09:05.944967 chatushka-0.9.0b2/setup.py
+-rw-r--r--   0        0        0     1202 2022-03-10 17:09:05.945293 chatushka-0.9.0b2/PKG-INFO
```

### Comparing `chatushka-0.9.0b1/chatushka/bot/data/eight_ball.yaml` & `chatushka-0.9.0b2/chatushka/bot/data/eight_ball.yaml`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/bot/data/lukashenko.txt` & `chatushka-0.9.0b2/chatushka/bot/data/lukashenko.txt`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/bot/internal/data_dir.py` & `chatushka-0.9.0b2/chatushka/bot/internal/data_dir.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/bot/internal/mute.py` & `chatushka-0.9.0b2/chatushka/bot/internal/mute.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/bot/main.py` & `chatushka-0.9.0b2/chatushka/bot/main.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/bot/matchers/__init__.py` & `chatushka-0.9.0b2/chatushka/bot/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/bot/matchers/admin/mute.py` & `chatushka-0.9.0b2/chatushka/bot/matchers/admin/mute.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/bot/matchers/admin/pin.py` & `chatushka-0.9.0b2/chatushka/bot/matchers/admin/pin.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/bot/matchers/bobuk_jokes.py` & `chatushka-0.9.0b2/chatushka/bot/matchers/bobuk_jokes.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/bot/matchers/eight_ball.py` & `chatushka-0.9.0b2/chatushka/bot/matchers/eight_ball.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/bot/matchers/helpers.py` & `chatushka-0.9.0b2/chatushka/bot/matchers/helpers.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/bot/matchers/lukashenko.py` & `chatushka-0.9.0b2/chatushka/bot/matchers/lukashenko.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/bot/matchers/suicide.py` & `chatushka-0.9.0b2/chatushka/bot/matchers/suicide.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/bot/matchers/welcoming.py` & `chatushka-0.9.0b2/chatushka/bot/matchers/welcoming.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/bot.py` & `chatushka-0.9.0b2/chatushka/core/bot.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/matchers/__init__.py` & `chatushka-0.9.0b2/chatushka/core/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/matchers/base.py` & `chatushka-0.9.0b2/chatushka/core/matchers/base.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/matchers/commands.py` & `chatushka-0.9.0b2/chatushka/core/matchers/commands.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/matchers/events.py` & `chatushka-0.9.0b2/chatushka/core/matchers/events.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/matchers/regex.py` & `chatushka-0.9.0b2/chatushka/core/matchers/regex.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/models.py` & `chatushka-0.9.0b2/chatushka/core/models.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/protocols.py` & `chatushka-0.9.0b2/chatushka/core/protocols.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/services/base.py` & `chatushka-0.9.0b2/chatushka/core/services/base.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/services/mongodb/utils.py` & `chatushka-0.9.0b2/chatushka/core/services/mongodb/utils.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/services/mongodb/wrapper.py` & `chatushka-0.9.0b2/chatushka/core/services/mongodb/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/transports/models.py` & `chatushka-0.9.0b2/chatushka/core/transports/models.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/transports/telegram_bot_api.py` & `chatushka-0.9.0b2/chatushka/core/transports/telegram_bot_api.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/chatushka/core/utils.py` & `chatushka-0.9.0b2/chatushka/core/utils.py`

 * *Files identical despite different names*

### Comparing `chatushka-0.9.0b1/pyproject.toml` & `chatushka-0.9.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatushka"
-version = "0.9.0b1"
+version = "0.9.0b2"
 description = "Bot that can make your chat explode!"
 authors = ["Aleksandr Shpak <shpaker@gmail.com>"]
 readme = "readme.md"
 homepage = "https://github.com/shpaker/chatushka"
 repository = "https://github.com/shpaker/chatushka"
 
 [tool.poetry.dependencies]
```

### Comparing `chatushka-0.9.0b1/setup.py` & `chatushka-0.9.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'click>=8.0.1,<9.0.0',
  'httpx>=0.22.0,<0.23.0',
  'motor>=2.5.0,<3.0.0',
  'pydantic[dotenv]>=1.8.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'chatushka',
-    'version': '0.9.0b1',
+    'version': '0.9.0b2',
     'description': 'Bot that can make your chat explode!',
     'long_description': '# Chatushka bot\n\nБот для чатиков (пока только для телеграмушки)\n\n\n# Usage\n\n## Installation\n\n```shell\npip install chatushka\n```\n\n## Start bot\n\n```shell\npython -m chatushka --token <telegrambotapitoken>\n```\n\n## Test bot\n\n- [x] добавить ботика в чат\n- [x] делегировать боту админские права\n- [x] написать в чатик /help\n\n```shell\npython -m chatushka --token <telegrambotapitoken>\n```\n',
     'author': 'Aleksandr Shpak',
     'author_email': 'shpaker@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/shpaker/chatushka',
```

### Comparing `chatushka-0.9.0b1/PKG-INFO` & `chatushka-0.9.0b2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatushka
-Version: 0.9.0b1
+Version: 0.9.0b2
 Summary: Bot that can make your chat explode!
 Home-page: https://github.com/shpaker/chatushka
 Author: Aleksandr Shpak
 Author-email: shpaker@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

