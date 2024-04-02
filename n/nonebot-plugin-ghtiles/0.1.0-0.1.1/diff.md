# Comparing `tmp/nonebot_plugin_ghtiles-0.1.0.tar.gz` & `tmp/nonebot_plugin_ghtiles-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ghtiles-0.1.0.tar", last modified: Wed Mar 13 02:42:37 2024, max compression
+gzip compressed data, was "nonebot_plugin_ghtiles-0.1.1.tar", last modified: Tue Apr  2 00:36:08 2024, max compression
```

## Comparing `nonebot_plugin_ghtiles-0.1.0.tar` & `nonebot_plugin_ghtiles-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2024-03-13 02:42:22.932327 nonebot_plugin_ghtiles-0.1.0/LICENSE
--rw-r--r--   0        0        0     3002 2024-03-13 02:42:22.932327 nonebot_plugin_ghtiles-0.1.0/README.md
--rw-r--r--   0        0        0     5194 2024-03-13 02:42:22.932327 nonebot_plugin_ghtiles-0.1.0/nonebot_plugin_ghtiles/__init__.py
--rw-r--r--   0        0        0      241 2024-03-13 02:42:22.932327 nonebot_plugin_ghtiles-0.1.0/nonebot_plugin_ghtiles/config.py
--rw-r--r--   0        0        0     2098 2024-03-13 02:42:22.932327 nonebot_plugin_ghtiles-0.1.0/nonebot_plugin_ghtiles/utils.py
--rw-r--r--   0        0        0      885 2024-03-13 02:42:37.148378 nonebot_plugin_ghtiles-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3551 1970-01-01 00:00:00.000000 nonebot_plugin_ghtiles-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-02 00:35:53.354958 nonebot_plugin_ghtiles-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3002 2024-04-02 00:35:53.354958 nonebot_plugin_ghtiles-0.1.1/README.md
+-rw-r--r--   0        0        0     7242 2024-04-02 00:35:53.354958 nonebot_plugin_ghtiles-0.1.1/nonebot_plugin_ghtiles/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-02 00:35:53.354958 nonebot_plugin_ghtiles-0.1.1/nonebot_plugin_ghtiles/config.py
+-rw-r--r--   0        0        0     1774 2024-04-02 00:35:53.354958 nonebot_plugin_ghtiles-0.1.1/nonebot_plugin_ghtiles/utils.py
+-rw-r--r--   0        0        0     1142 2024-04-02 00:36:08.842974 nonebot_plugin_ghtiles-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3714 1970-01-01 00:00:00.000000 nonebot_plugin_ghtiles-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_ghtiles-0.1.0/LICENSE` & `nonebot_plugin_ghtiles-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ghtiles-0.1.0/README.md` & `nonebot_plugin_ghtiles-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ghtiles-0.1.0/nonebot_plugin_ghtiles/__init__.py` & `nonebot_plugin_ghtiles-0.1.1/nonebot_plugin_ghtiles/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-import time
-from nonebot import get_bot, get_plugin_config, require, get_driver
-from nonebot.plugin import PluginMetadata
+import asyncio
+
+import httpx
+from nonebot import get_bot, get_plugin_config, require, get_driver, logger
 from nonebot.adapters import Event
+from nonebot.plugin import PluginMetadata
 
-from nonebot_plugin_ghtiles.utils import (
+from .config import Config
+from .utils import (
     AutoSave,
     get_homepage_html,
     get_today,
     get_today_contributions,
-    check_contributions
+    check_contributions,
 )
-from .config import Config
 
 require("nonebot_plugin_alconna")
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_localstore")
 require("nonebot_plugin_session")
 
 import nonebot_plugin_localstore as store  # noqa: E402
@@ -22,15 +24,15 @@
     At,
     Command,
     Text,
     UniMessage,
     Target,
 )
 from nonebot_plugin_apscheduler import scheduler  # noqa: E402
-from nonebot_plugin_session import EventSession, SessionIdType  # noqa: E402
+from nonebot_plugin_session import EventSession  # noqa: E402
 
 __plugin_meta__ = PluginMetadata(
     name="ghtiles",
     description="看看你的 GitHub 瓷砖",
     usage="",
     homepage="https://github.com/Lipraty/nonebot-plugin-ghtiles",
     type="application",
@@ -39,28 +41,53 @@
         "license": "MIT",
         "author": "Lipraty",
     },
 )
 
 config = get_plugin_config(Config)
 
+driver = get_driver()
+
+_data = AutoSave(
+    store.get_data_file("ghtiles", "data.json"),
+    initial_data={"on_reminder": {}, "users": {}},
+)
+
+
+# data structure
+# {
+#     "on_reminder": {
+#         "{group_id}": list[{user_id}]
+#     },
+#     "users": {
+#         "{user_id}": {
+#             "username": "{username}",
+#             "token"?: "{token}"
+#         }
+#     }
+# }
+
 
 # messages
 def tile_msg(username: str, contributions: int):
+    logger.debug(
+        f"triggered tile_msg, username: {username}, contributions: {contributions}"
+    )
     if contributions == 0:
         return UniMessage(f"{username} 还没有贴瓷砖")
     else:
         return UniMessage(f"{username} 在 {get_today()} 贴了 {contributions} 个瓷砖")
 
 
 def winner_msg(username: str, contributions: int):
     return UniMessage(f"今天的瓷砖王是 {username}，贴了 {contributions} 个瓷砖！")
 
 
 def no_contributions_msg(user_id: list[str]):
+    logger.debug(f"triggered no_contributions_msg, user_id: {user_id}")
     msg = UniMessage()
     for id in user_id:
         msg.append(At("user", id))
     msg += Text("懒鬼懒鬼懒鬼！")
     return msg
 
 
@@ -70,87 +97,133 @@
         set(user for users in _data["on_reminder"].values() for user in users)
     )
     users = {
         user_id: data
         for user_id, data in _data["users"].items()
         if user_id in reminder_users
     }
+    logger.debug(f"get users: {users}, reminder_users: {reminder_users}")
     for user_id, user_data in users.items():
         username = user_data["username"]
         contributions = await get_today_contributions(
-            username, await get_homepage_html(username, config.ght_proxy)
+            await get_homepage_html(username, config.ght_proxy)
         )
         users[user_id]["contributions"] = contributions
-        time.sleep(1)  # avoid rate limit
+        await asyncio.sleep(1)  # avoid rate limit
+    logger.debug(f"users updated of contributions: {users}")
     bot = get_bot()
     for group_id, user_list in _data["on_reminder"].items():
         if not user_list:  # private, skip
             continue
         max_in_group = max(users[user_id]["contributions"] for user_id in user_list)
         max_in_group_username: str = [
             user_id
             for user_id in user_list
             if users[user_id]["contributions"] == max_in_group
         ][0]
         zero_in_group = [
             user_id for user_id in user_list if users[user_id]["contributions"] == 0
         ]
-        await UniMessage(winner_msg(max_in_group_username, max_in_group)).send(
-            Target(group_id, platform=bot.adapter.get_name())
-        )
+        await UniMessage(
+            winner_msg(
+                _data["users"].get(max_in_group_username)["username"], max_in_group
+            )
+        ).send(Target(group_id, platform=bot.adapter.get_name()))
+        logger.debug(f"send winner_msg to {group_id}, winner: {max_in_group_username}")
         if zero_in_group:
             await UniMessage(no_contributions_msg(zero_in_group)).send(
                 Target(group_id, platform=bot.adapter.get_name())
             )
+            logger.debug(
+                f"send no_contributions_msg to {group_id}, users: {zero_in_group}"
+            )
 
 
-driver = get_driver()
-_data = AutoSave(store.get_data_file("ghtiles", "data.json"))
-# data structure
-# {
-#     "on_reminder": {
-#         "{group_id}": list[{user_id}]
-#     },
-#     "users": {
-#         "{user_id}": {
-#             "username": "{username}",
-#             "token"?: "{token}"
-#         }
-#     }
-# }
+tile_cmd = (
+    Command("tile", "获取 GitHub 瓷砖")
+    .alias("瓷砖")
+    .usage("tile, 获取今天的 GitHub 瓷砖")
+    .build()
+)
+
 
-tile_cmd = Command("tile").alias("瓷砖").build()
 @tile_cmd.handle()
 async def tile_cmd_handle(event: Event, session: EventSession):
     user_id = session.id1
-    username = _data[user_id]["username"]
+    logger.debug(f"triggered tile_cmd_handle, user_id: {user_id}")
+    user_id = _data["users"].get(user_id)
+    if not user_id:
+        await tile_cmd.finish(
+            "好像没有绑定过 GitHub? 输入 `/tile.bind <github username>` 来绑定"
+        )
+    username = user_id["username"]
+    logger.debug(f"triggered tile_cmd_handle, user_id: {user_id}, username: {username}")
     contributions = await get_today_contributions(
-        username, await get_homepage_html(username, config.ght_proxy)
+        await get_homepage_html(username, config.ght_proxy)
     )
-    return await tile_msg(username, contributions).send(event)
+    logger.debug(f"get contributions: {contributions} of {username}")
+    await tile_msg(username, contributions).send(event)
+
+
+tile_bind_cmd = (
+    Command("tile.bind <username:str>", "绑定 GitHub 用户名")
+    .alias("绑定")
+    .usage("tile.bind <username>, 绑定 GitHub 用户名")
+    .build()
+)
 
 
-tile_bind_cmd = Command("tile.bind <username:str>", "绑定 GitHub 用户名").alias("绑定").build()
 @tile_bind_cmd.handle()
 async def tile_bind_cmd_handle(event: Event, username: str, session: EventSession):
     user_id = session.id1
     # check
     if user_id in _data["users"]:
+        logger.debug(f"binded user_id: {user_id}")
         return await UniMessage("你已经绑定过了").send(event)
     # check username
-    if check_contributions(username, await get_homepage_html(username, config.ght_proxy)):
-        return await UniMessage("这个用户不存在或者没有公开活动").send(event)
-    _data["users"][user_id] = {"username": username}
+    try:
+        if not await check_contributions(
+            gh_html=await get_homepage_html(username, config.ght_proxy)
+        ):
+            logger.debug(f"username: {username} has no public activity")
+            return await UniMessage("这个用户没有公开活动").send(event)
+    except httpx.HTTPStatusError as e:
+        if e.response.status_code == 404:
+            logger.debug(f"username: {username} not exists")
+            return await UniMessage("这个用户不存在").send(event)
+    users_copy = _data["users"].copy()
+
+    user_info = users_copy.get(user_id, {})
+
+    user_info["username"] = username
+    users_copy[user_id] = user_info
+
+    _data["users"] = users_copy
+    logger.debug(f"binded username: {username} to user_id: {user_id}")
     return await UniMessage(f"绑定成功，你的 GitHub 用户名是 {username}").send(event)
 
 
-tile_remine_cmd = Command("tile.remind").alias("创建提醒").build()
+tile_remine_cmd = (
+    Command("tile.remind")
+    .alias("创建提醒")
+    .usage("tile.remind, 创建提醒，每天 23:30 发送")
+    .build()
+)
+
+
 @tile_remine_cmd.handle()
 async def tile_remine_cmd_handle(event: Event, session: EventSession):
     user_id = session.id1
     group_id = session.id2
-    if group_id not in _data["on_reminder"].keys():
-        _data["on_reminder"][group_id] = []
-    if user_id in _data["on_reminder"][group_id]:
+
+    on_reminder_updated = _data["on_reminder"].copy()
+
+    if group_id not in on_reminder_updated:
+        on_reminder_updated[group_id] = []
+
+    if user_id in on_reminder_updated[group_id]:
         return await UniMessage("你已经创建过提醒了").send(event)
-    _data["on_reminder"][group_id].append(user_id)
+
+    on_reminder_updated[group_id].append(user_id)
+    _data["on_reminder"] = on_reminder_updated
+    logger.debug(f"create reminder for user_id: {user_id} in group_id: {group_id}")
     return await UniMessage("创建提醒成功").send(event)
```

### Comparing `nonebot_plugin_ghtiles-0.1.0/nonebot_plugin_ghtiles/utils.py` & `nonebot_plugin_ghtiles-0.1.1/nonebot_plugin_ghtiles/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,62 +13,51 @@
     url = f"{proxy}/{gh_name}"
     async with httpx.AsyncClient() as client:
         response = await client.get(url)
         response.raise_for_status()
         return response.text
 
 
-async def check_contributions(gh_name: str, gh_html: str) -> bool:
+async def check_contributions(gh_html: str) -> bool:
     return re.compile(r"\'s activity is private\<\/h2\>").search(gh_html) is None
 
 
-async def get_today_contributions(gh_name: str, gh_html: str):
+async def get_today_contributions(gh_html: str) -> int:
     match = re.compile(
         r'data-date="' + get_today() + r".*?(\d+|No) contributions"
     ).search(gh_html)
     if match:
         contributions = match.group(1)
         if contributions == "No":
             return 0
         else:
             return int(contributions)
     else:
         return 0
 
 
 class AutoSave:
-    def __init__(self, fileProxy: Path, proxy = None):
+    def __init__(self, fileProxy: Path, proxy: dict = None, initial_data: dict = None):
+        self._fileProxy = fileProxy
         if proxy is None:
             if fileProxy.exists():
-                self._proxy = json.loads(fileProxy.read_text())
+                load_by_file = json.loads(fileProxy.read_text())
+                self._proxy = load_by_file if load_by_file else initial_data or {}
             else:
-                self._proxy = {}
+                self._proxy = initial_data or {}
         else:
             self._proxy = proxy
-        self._fileProxy = fileProxy
+        self._save()
 
     def _save(self):
         self._fileProxy.write_text(json.dumps(self._proxy, ensure_ascii=False))
-    
-    def __getattr__(self, name):
-        return getattr(self._proxy, name)
-    
+
     def __getitem__(self, name):
         return self._proxy[name]
-    
-    def __setattr__(self, __name: str, __value):
-        if __name == "_proxy" or __name == "_fileProxy":
-            super().__setattr__("_proxy", __name)
-        else:
-            setattr(self._proxy, __name, __value)
-            self._save()
-    
-    def __setitem__(self, __name: str, __value):
-        if __name == "_proxy":
-            super().__setattr__("_proxy", __name)
-        else:
-            self._proxy[__name] = __value
-            self._save()
-    
-    def __delitem__(self, __name: str):
-        del self._proxy[__name]
+
+    def __setitem__(self, name: str, value):
+        self._proxy[name] = value
+        self._save()
+
+    def __delitem__(self, name: str):
+        del self._proxy[name]
         self._save()
```

### Comparing `nonebot_plugin_ghtiles-0.1.0/pyproject.toml` & `nonebot_plugin_ghtiles-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 [project]
 name = "nonebot-plugin-ghtiles"
-version = "0.1.0"
+version = "0.1.1"
 description = "A nonebot2 plugin for show GitHub contributions"
 readme = "README.md"
 requires-python = ">=3.9, <4.0"
 dependencies = [
-    "nonebot2>=2.0.0",
+    "nonebot2>=2.2.0",
+    "httpx~=0.27",
     "nonebot-plugin-alconna>=0.38.1",
+    "nonebot-plugin-apscheduler~=0.4",
+    "nonebot-plugin-session~=0.3",
+    "nonebot-plugin-localstore~=0.6",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-homepage = "https://gtihub.com/Lipraty/nonebot-plugin-ghtiles"
+homepage = "https://github.com/Lipraty/nonebot-plugin-ghtiles"
 
 [tool.nonebot]
 adapters = [
     { name = "Satori", module_name = "nonebot.adapters.satori" },
+    { name = "OneBot V12", module_name = "nonebot.adapters.onebot.v12" },
+    { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" },
 ]
 plugins = [
-    "nonebot_plugin_alconna",
-    "nonebot_plugin_apscheduler",
-    "nonebot_plugin_localstore",
-    "nonebot_plugin_session",
-]
-plugin_dirs = [
     "nonebot_plugin_ghtiles",
 ]
-builtin_plugins = [
-    "echo",
+
+[tool.pdm.dev-dependencies]
+dev = [
+    "nonebot-adapter-satori~=0.10",
+    "nonebot-adapter-onebot~=2.4",
+    "nonebot2[fastapi,httpx,websockets]~=2.2",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `nonebot_plugin_ghtiles-0.1.0/PKG-INFO` & `nonebot_plugin_ghtiles-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ghtiles
-Version: 0.1.0
+Version: 0.1.1
 Summary: A nonebot2 plugin for show GitHub contributions
-Home-page: https://gtihub.com/Lipraty/nonebot-plugin-ghtiles
+Home-page: https://github.com/Lipraty/nonebot-plugin-ghtiles
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Project-URL: Homepage, https://gtihub.com/Lipraty/nonebot-plugin-ghtiles
+Project-URL: Homepage, https://github.com/Lipraty/nonebot-plugin-ghtiles
 Requires-Python: <4.0,>=3.9
-Requires-Dist: nonebot2>=2.0.0
+Requires-Dist: nonebot2>=2.2.0
+Requires-Dist: httpx~=0.27
 Requires-Dist: nonebot-plugin-alconna>=0.38.1
+Requires-Dist: nonebot-plugin-apscheduler~=0.4
+Requires-Dist: nonebot-plugin-session~=0.3
+Requires-Dist: nonebot-plugin-localstore~=0.6
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store">
     <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="180" height="180" alt="logo">
   </a>
   <br>
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ghtiles Version: 0.1.0 Summary: A
-nonebot2 plugin for show GitHub contributions Home-page: https://gtihub.com/
+Metadata-Version: 2.1 Name: nonebot-plugin-ghtiles Version: 0.1.1 Summary: A
+nonebot2 plugin for show GitHub contributions Home-page: https://github.com/
 Lipraty/nonebot-plugin-ghtiles Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Project-URL: Homepage, https://gtihub.com/Lipraty/nonebot-
-plugin-ghtiles Requires-Python: <4.0,>=3.9 Requires-Dist: nonebot2>=2.0.0
-Requires-Dist: nonebot-plugin-alconna>=0.38.1 Description-Content-Type: text/
-markdown
+:: OS Independent Project-URL: Homepage, https://github.com/Lipraty/nonebot-
+plugin-ghtiles Requires-Python: <4.0,>=3.9 Requires-Dist: nonebot2>=2.2.0
+Requires-Dist: httpx~=0.27 Requires-Dist: nonebot-plugin-alconna>=0.38.1
+Requires-Dist: nonebot-plugin-apscheduler~=0.4 Requires-Dist: nonebot-plugin-
+session~=0.3 Requires-Dist: nonebot-plugin-localstore~=0.6 Description-Content-
+Type: text/markdown
                                     _[_l_o_g_o_]
                                     [logo]
   # NoneBot-Plugin-GHTiles _â¨ ççä½ ç GitHub ç·ç  for NoneBot2 â¨_
                              [python]_[_p_d_m_-_m_a_n_a_g_e_d_]
             _[_P_y_d_a_n_t_i_c_ _V_e_r_s_i_o_n_ _1_ _O_r_ _2_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð ä»ç» NoneBot2 æä»¶ï¼ç¨äºæ¥çä½ ç GitHub ç·ç  ## ð¿
 å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯ [æ¨è] ä½¿ç¨ nb-cli
```

