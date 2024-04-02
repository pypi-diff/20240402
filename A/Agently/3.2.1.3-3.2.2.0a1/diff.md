# Comparing `tmp/Agently-3.2.1.3.tar.gz` & `tmp/Agently-3.2.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Agently-3.2.1.3.tar", last modified: Wed Mar 27 01:22:26 2024, max compression
+gzip compressed data, was "Agently-3.2.2.0a1.tar", last modified: Tue Apr  2 11:26:29 2024, max compression
```

## Comparing `Agently-3.2.1.3.tar` & `Agently-3.2.2.0a1.tar`

### file list

```diff
@@ -1,122 +1,131 @@
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.586857 Agently-3.2.1.3/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.561499 Agently-3.2.1.3/Agently/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.562696 Agently-3.2.1.3/Agently/Agent/
--rw-r--r--   0 moxin      (501) staff       (20)    13552 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Agent/Agent.py
--rw-r--r--   0 moxin      (501) staff       (20)     2259 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Agent/AgentFactory.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Agent/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.563055 Agently-3.2.1.3/Agently/Facility/
--rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Facility/FacilityManager.py
--rw-r--r--   0 moxin      (501) staff       (20)       44 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Facility/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.563945 Agently-3.2.1.3/Agently/Request/
--rw-r--r--   0 moxin      (501) staff       (20)     9217 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Request/Request.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Request/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.564375 Agently-3.2.1.3/Agently/WebSocket/
--rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/WebSocket/WebSocket.py
--rw-r--r--   0 moxin      (501) staff       (20)       55 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/WebSocket/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.565529 Agently-3.2.1.3/Agently/Workflow/
--rw-r--r--   0 moxin      (501) staff       (20)     6927 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/Chunk.py
--rw-r--r--   0 moxin      (501) staff       (20)    10302 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/MainExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/Schema.py
--rw-r--r--   0 moxin      (501) staff       (20)     2236 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/Workflow.py
--rw-r--r--   0 moxin      (501) staff       (20)       57 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.565939 Agently-3.2.1.3/Agently/Workflow/executors/
--rw-r--r--   0 moxin      (501) staff       (20)       67 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/executors/StartExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/executors/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      245 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/executors/install.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.567943 Agently-3.2.1.3/Agently/Workflow/lib/
--rw-r--r--   0 moxin      (501) staff       (20)     1033 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/lib/BreakingHub.py
--rw-r--r--   0 moxin      (501) staff       (20)      656 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/lib/ChunkExecutorABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      483 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/lib/Store.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/lib/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/lib/constants.py
--rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/lib/painter.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.569926 Agently-3.2.1.3/Agently/Workflow/utils/
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     3527 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/utils/exec_tree.py
--rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/utils/find.py
--rw-r--r--   0 moxin      (501) staff       (20)      613 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/utils/logger.py
--rw-r--r--   0 moxin      (501) staff       (20)      892 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/utils/runtime_supports.py
--rw-r--r--   0 moxin      (501) staff       (20)      242 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/utils/verify.py
--rw-r--r--   0 moxin      (501) staff       (20)      512 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/_global.py
--rw-r--r--   0 moxin      (501) staff       (20)      149 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/global_plugin_manager.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.570048 Agently-3.2.1.3/Agently/plugins/
--rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.573738 Agently-3.2.1.3/Agently/plugins/agent_component/
--rw-r--r--   0 moxin      (501) staff       (20)     2870 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Decorator.py
--rw-r--r--   0 moxin      (501) staff       (20)     1384 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/EventListener.py
--rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/OpenAIAssistant.py
--rw-r--r--   0 moxin      (501) staff       (20)      785 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/ReplyReformer.py
--rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Role.py
--rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Search.py
--rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Segment.py
--rw-r--r--   0 moxin      (501) staff       (20)     8287 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Session.py
--rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Status.py
--rw-r--r--   0 moxin      (501) staff       (20)     8878 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Tool.py
--rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/UserInfo.py
--rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      505 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.574091 Agently-3.2.1.3/Agently/plugins/agent_component/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      588 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/utils/ComponentABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.575698 Agently-3.2.1.3/Agently/plugins/facility/
--rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/Embedding.py
--rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/RoleManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/StatusManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)       85 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.576844 Agently-3.2.1.3/Agently/plugins/facility/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      266 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/utils/FacilityABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       36 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.579774 Agently-3.2.1.3/Agently/plugins/request/
--rw-r--r--   0 moxin      (501) staff       (20)     7405 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/Claude.py
--rw-r--r--   0 moxin      (501) staff       (20)    10385 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/ERNIE.py
--rw-r--r--   0 moxin      (501) staff       (20)     7440 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/Google.py
--rw-r--r--   0 moxin      (501) staff       (20)     7851 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/Kimi.py
--rw-r--r--   0 moxin      (501) staff       (20)    12342 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/MiniMax.py
--rw-r--r--   0 moxin      (501) staff       (20)    15538 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/OAIClient.py
--rw-r--r--   0 moxin      (501) staff       (20)    11607 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/OpenAI.py
--rw-r--r--   0 moxin      (501) staff       (20)    12788 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/ZhipuAI.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      139 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.581066 Agently-3.2.1.3/Agently/plugins/request/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     5387 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/utils/RequestABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      118 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     4330 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.581740 Agently-3.2.1.3/Agently/plugins/storage/
--rw-r--r--   0 moxin      (501) staff       (20)     3160 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/storage/FileStorage.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/storage/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      131 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/storage/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.581986 Agently-3.2.1.3/Agently/plugins/storage/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      745 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/storage/utils/StorageABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       34 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/storage/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.582846 Agently-3.2.1.3/Agently/plugins/tool/
--rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/tool/Code.py
--rw-r--r--   0 moxin      (501) staff       (20)     6912 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/tool/Web.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/tool/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      104 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/tool/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.583204 Agently-3.2.1.3/Agently/plugins/tool/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      443 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/tool/utils/ToolABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/tool/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      168 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/requirements.txt
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.586193 Agently-3.2.1.3/Agently/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/AliasManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/DataOps.py
--rw-r--r--   0 moxin      (501) staff       (20)      323 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/IdGenerator.py
--rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/PluginManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/RuntimeCtx.py
--rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/StorageDelegate.py
--rw-r--r--   0 moxin      (501) staff       (20)     4758 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/ToolManager.py
--rw-r--r--   0 moxin      (501) staff       (20)      491 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/check_version.py
--rw-r--r--   0 moxin      (501) staff       (20)     2773 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/load_json.py
--rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.586493 Agently-3.2.1.3/Agently.egg-info/
--rw-r--r--   0 moxin      (501) staff       (20)      819 2024-03-27 01:22:26.000000 Agently-3.2.1.3/Agently.egg-info/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)     3375 2024-03-27 01:22:26.000000 Agently-3.2.1.3/Agently.egg-info/SOURCES.txt
--rw-r--r--   0 moxin      (501) staff       (20)        1 2024-03-27 01:22:26.000000 Agently-3.2.1.3/Agently.egg-info/dependency_links.txt
--rw-r--r--   0 moxin      (501) staff       (20)      118 2024-03-27 01:22:26.000000 Agently-3.2.1.3/Agently.egg-info/requires.txt
--rw-r--r--   0 moxin      (501) staff       (20)        8 2024-03-27 01:22:26.000000 Agently-3.2.1.3/Agently.egg-info/top_level.txt
--rw-r--r--   0 moxin      (501) staff       (20)      819 2024-03-27 01:22:26.586684 Agently-3.2.1.3/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-03-27 01:22:26.586896 Agently-3.2.1.3/setup.cfg
--rw-------   0 moxin      (501) staff       (20)      974 2024-03-27 01:22:19.000000 Agently-3.2.1.3/setup.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.222868 Agently-3.2.2.0a1/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.204415 Agently-3.2.2.0a1/Agently/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.205620 Agently-3.2.2.0a1/Agently/Agent/
+-rw-r--r--   0 moxin      (501) staff       (20)    14078 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Agent/Agent.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2259 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Agent/AgentFactory.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Agent/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.206478 Agently-3.2.2.0a1/Agently/Facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Facility/FacilityManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)       44 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Facility/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.206990 Agently-3.2.2.0a1/Agently/Request/
+-rw-r--r--   0 moxin      (501) staff       (20)     9783 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Request/Request.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Request/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.207416 Agently-3.2.2.0a1/Agently/WebSocket/
+-rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/WebSocket/WebSocket.py
+-rw-r--r--   0 moxin      (501) staff       (20)       55 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/WebSocket/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.208825 Agently-3.2.2.0a1/Agently/Workflow/
+-rw-r--r--   0 moxin      (501) staff       (20)     7650 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/Chunk.py
+-rw-r--r--   0 moxin      (501) staff       (20)    16640 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/MainExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/Schema.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3165 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/Workflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)       57 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.209221 Agently-3.2.2.0a1/Agently/Workflow/executors/
+-rw-r--r--   0 moxin      (501) staff       (20)       67 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/executors/StartExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/executors/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      245 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/executors/install.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.210095 Agently-3.2.2.0a1/Agently/Workflow/lib/
+-rw-r--r--   0 moxin      (501) staff       (20)     1470 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/lib/BreakingHub.py
+-rw-r--r--   0 moxin      (501) staff       (20)      656 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/lib/ChunkExecutorABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      426 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/lib/ChunkExecutorManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      483 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/lib/Store.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/lib/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/lib/constants.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/lib/painter.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.211030 Agently-3.2.2.0a1/Agently/Workflow/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4599 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/utils/exec_tree.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/utils/find.py
+-rw-r--r--   0 moxin      (501) staff       (20)      613 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/utils/logger.py
+-rw-r--r--   0 moxin      (501) staff       (20)      892 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/utils/runtime_supports.py
+-rw-r--r--   0 moxin      (501) staff       (20)      242 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/utils/verify.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.211291 Agently-3.2.2.0a1/Agently/Workflow/yamlflow/
+-rw-r--r--   0 moxin      (501) staff       (20)       63 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/yamlflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.211828 Agently-3.2.2.0a1/Agently/Workflow/yamlflow/preset_chunks/
+-rw-r--r--   0 moxin      (501) staff       (20)      500 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/yamlflow/preset_chunks/Print.py
+-rw-r--r--   0 moxin      (501) staff       (20)      108 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/yamlflow/preset_chunks/Start.py
+-rw-r--r--   0 moxin      (501) staff       (20)      289 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/yamlflow/preset_chunks/UserInput.py
+-rw-r--r--   0 moxin      (501) staff       (20)      767 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/yamlflow/preset_chunks/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5710 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/Workflow/yamlflow/yamlflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)      512 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/_global.py
+-rw-r--r--   0 moxin      (501) staff       (20)      149 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/global_plugin_manager.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.211956 Agently-3.2.2.0a1/Agently/plugins/
+-rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.214425 Agently-3.2.2.0a1/Agently/plugins/agent_component/
+-rw-r--r--   0 moxin      (501) staff       (20)     2870 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/Decorator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1384 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/EventListener.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/OpenAIAssistant.py
+-rw-r--r--   0 moxin      (501) staff       (20)      785 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/ReplyReformer.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/Role.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/Search.py
+-rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/Segment.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8287 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/Session.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/Status.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8878 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/Tool.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/UserInfo.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      505 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.214681 Agently-3.2.2.0a1/Agently/plugins/agent_component/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      588 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/utils/ComponentABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/agent_component/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.215454 Agently-3.2.2.0a1/Agently/plugins/facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/facility/Embedding.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/facility/RoleManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/facility/StatusManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/facility/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)       85 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/facility/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.215734 Agently-3.2.2.0a1/Agently/plugins/facility/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      266 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/facility/utils/FacilityABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       36 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/facility/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.218122 Agently-3.2.2.0a1/Agently/plugins/request/
+-rw-r--r--   0 moxin      (501) staff       (20)     7323 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/request/Claude.py
+-rw-r--r--   0 moxin      (501) staff       (20)    10303 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/request/ERNIE.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7372 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/request/Google.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7769 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/request/Kimi.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12270 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/request/MiniMax.py
+-rw-r--r--   0 moxin      (501) staff       (20)    15354 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/request/OAIClient.py
+-rw-r--r--   0 moxin      (501) staff       (20)    11525 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/request/OpenAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12624 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/request/ZhipuAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/request/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      139 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/request/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.218634 Agently-3.2.2.0a1/Agently/plugins/request/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     5307 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/request/utils/RequestABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      118 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/request/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4330 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/request/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.219147 Agently-3.2.2.0a1/Agently/plugins/storage/
+-rw-r--r--   0 moxin      (501) staff       (20)     3160 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/storage/FileStorage.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/storage/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      131 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/storage/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.219408 Agently-3.2.2.0a1/Agently/plugins/storage/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      745 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/storage/utils/StorageABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       34 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/storage/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.220063 Agently-3.2.2.0a1/Agently/plugins/tool/
+-rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/tool/Code.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6912 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/tool/Web.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/tool/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      104 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/tool/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.220318 Agently-3.2.2.0a1/Agently/plugins/tool/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      443 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/tool/utils/ToolABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/plugins/tool/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      168 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/requirements.txt
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.222035 Agently-3.2.2.0a1/Agently/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/utils/AliasManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/utils/DataOps.py
+-rw-r--r--   0 moxin      (501) staff       (20)      323 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/utils/IdGenerator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/utils/PluginManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/utils/RuntimeCtx.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/utils/StorageDelegate.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4758 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/utils/ToolManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      491 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/utils/check_version.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2773 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/utils/load_json.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-04-02 04:36:44.000000 Agently-3.2.2.0a1/Agently/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-02 11:26:29.222478 Agently-3.2.2.0a1/Agently.egg-info/
+-rw-r--r--   0 moxin      (501) staff       (20)      821 2024-04-02 11:26:29.000000 Agently-3.2.2.0a1/Agently.egg-info/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)     3699 2024-04-02 11:26:29.000000 Agently-3.2.2.0a1/Agently.egg-info/SOURCES.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        1 2024-04-02 11:26:29.000000 Agently-3.2.2.0a1/Agently.egg-info/dependency_links.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      118 2024-04-02 11:26:29.000000 Agently-3.2.2.0a1/Agently.egg-info/requires.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        8 2024-04-02 11:26:29.000000 Agently-3.2.2.0a1/Agently.egg-info/top_level.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      821 2024-04-02 11:26:29.222685 Agently-3.2.2.0a1/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-02 11:26:29.222905 Agently-3.2.2.0a1/setup.cfg
+-rw-------   0 moxin      (501) staff       (20)      982 2024-04-02 11:26:07.000000 Agently-3.2.2.0a1/setup.py
```

### Comparing `Agently-3.2.1.3/Agently/Agent/Agent.py` & `Agently-3.2.2.0a1/Agently/Agent/Agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,20 +118,33 @@
         self.agent_storage.table("agent_runtime_ctx").update_by_dict(self.agent_runtime_ctx.get()).save()
         return self
 
     def set_settings(self, settings_key: str, settings_value: any):
         self.settings.set(settings_key, settings_value)
         return self
 
+    def set_agent_prompt(self, key: str, value: any):
+        self.agent_runtime_ctx.set(f"prompt.{ key }", value)
+        return self
+
+    def get_agent_prompt(self, key: str):
+        return self.agent_runtime_ctx.get(f"prompt.{ key }")
+
+    def remove_agent_prompt(self, key: str):
+        self.agent_runtime_ctx.remove(f"prompt.{ key }")
+        return self
+
     async def start_async(self, request_type: str=None):
         try:
             is_debug = self.settings.get_trace_back("is_debug")
             # Auto Save Agent runtime_ctx
             if self.agent_runtime_ctx.get("agent_auto_save") ==  True:
                 self.save()
+            # Load Prompt in Agent runtime_ctx to Request runtime_ctx
+            self.request_runtime_ctx.set("prompt", self.agent_runtime_ctx.get("prompt", {}))
             # Call Prefix Funcs to Prepare Prefix Data(From agent_runtime_ctx To request_runtime_ctx)
             async def call_prefix_funcs(prefix_funcs):
                 if prefix_funcs != None:
                     for prefix_func in prefix_funcs:
                         prefix_data = await prefix_func() if asyncio.iscoroutinefunction(prefix_func) else prefix_func()
                         if prefix_data != None:
                             if isinstance(prefix_data, tuple) and isinstance(prefix_data[0], str) and prefix_data[1] != None:
```

### Comparing `Agently-3.2.1.3/Agently/Agent/AgentFactory.py` & `Agently-3.2.2.0a1/Agently/Agent/AgentFactory.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/Facility/FacilityManager.py` & `Agently-3.2.2.0a1/Agently/Facility/FacilityManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/Request/Request.py` & `Agently-3.2.2.0a1/Agently/Request/Request.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,32 +24,43 @@
             "type": None,
             "reply": None,
         }
         # Plugin Manager
         self.plugin_manager = PluginManager(parent = parent_plugin_manager)
         # Namespace
         self.model = RuntimeCtxNamespace("model", self.settings, return_to = self)
-        self.prompt_general = RuntimeCtxNamespace("prompt.general_instruction", self.request_runtime_ctx, return_to = self)
+        self.prompt_general = RuntimeCtxNamespace("prompt.general", self.request_runtime_ctx, return_to = self)
         self.prompt_role = RuntimeCtxNamespace("prompt.role", self.request_runtime_ctx, return_to = self)
         self.prompt_user_info = RuntimeCtxNamespace("prompt.user_info", self.request_runtime_ctx, return_to = self)
-        self.prompt_abstract = RuntimeCtxNamespace("prompt.headline", self.request_runtime_ctx, return_to = self)
+        self.prompt_abstract = RuntimeCtxNamespace("prompt.abstract", self.request_runtime_ctx, return_to = self)
         self.prompt_chat_history = RuntimeCtxNamespace("prompt.chat_history", self.request_runtime_ctx, return_to = self)
         self.prompt_input = RuntimeCtxNamespace("prompt.input", self.request_runtime_ctx, return_to = self)
-        self.prompt_information = RuntimeCtxNamespace("prompt.information", self.request_runtime_ctx, return_to = self)
-        self.prompt_instruction = RuntimeCtxNamespace("prompt.instruction", self.request_runtime_ctx, return_to = self)
+        self.prompt_info = RuntimeCtxNamespace("prompt.info", self.request_runtime_ctx, return_to = self)
+        self.prompt_instruct = RuntimeCtxNamespace("prompt.instruct", self.request_runtime_ctx, return_to = self)
         self.prompt_output = RuntimeCtxNamespace("prompt.output", self.request_runtime_ctx, return_to = self)
         self.prompt_files = RuntimeCtxNamespace("prompt.files", self.request_runtime_ctx, return_to = self)
         # Alias
         self.alias_manager = AliasManager(self)
         self._register_default_alias(self.alias_manager)
 
     def set_settings(self, settings_key: str, settings_value: any):
         self.settings.set(settings_key, settings_value)
         return self
 
+    def set_request_prompt(self, key: str, value: any):
+        self.request_runtime_ctx.set(f"prompt.{ key }", value)
+        return self
+
+    def get_request_prompt(self, key: str):
+        return self.request_runtime_ctx.get(f"prompt.{ key }")
+
+    def remove_request_prompt(self, key: str):
+        self.request_runtime_ctx.remove(f"prompt.{ key }")
+        return self
+
     def _register_default_alias(self, alias_manager):
         def set_model_settings(key: str, value: any, *, model_name:str = None):
             model_name = model_name if model_name else self.settings.get_trace_back("current_model")
             if model_name == None:
                 raise Exception("[Model Settings] No model was appointed. Use .use_model(<model name>) or kwarg parameter model_name=<model_name> to set.")
             self.settings.update(f"model.{ model_name }.{ key }", value)
 
@@ -61,19 +72,22 @@
         alias_manager.register("set_proxy", lambda proxy: self.settings.set("proxy", proxy))
         alias_manager.register("general", self.prompt_general.assign)
         alias_manager.register("role", self.prompt_role.assign)
         alias_manager.register("user_info", self.prompt_user_info.assign)
         alias_manager.register("abstract", self.prompt_abstract.assign)
         alias_manager.register("chat_history", self.prompt_chat_history.assign)
         alias_manager.register("input", self.prompt_input.assign)
-        alias_manager.register("info", self.prompt_information.assign)
-        alias_manager.register("instruct", self.prompt_instruction.assign)
+        alias_manager.register("info", self.prompt_info.assign)
+        alias_manager.register("instruct", self.prompt_instruct.assign)
         alias_manager.register("output", self.prompt_output.assign)
         alias_manager.register("file", self.prompt_files.append)
-        alias_manager.register("files", self.prompt_files.extend)        
+        alias_manager.register("files", self.prompt_files.extend)
+        alias_manager.register("set_request_prompt", self.set_request_prompt)
+        alias_manager.register("get_request_prompt", self.get_request_prompt)
+        alias_manager.register("remove_request_prompt", self.remove_request_prompt) 
         
     async def get_event_generator(self, request_type: str=None):
         # Set Request Type
         self.request_runtime_ctx.set("request_type", request_type)
         # Erase response cache
         self.response_cache = {
             "prompt": {},
```

### Comparing `Agently-3.2.1.3/Agently/WebSocket/WebSocket.py` & `Agently-3.2.2.0a1/Agently/WebSocket/WebSocket.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/Workflow/Chunk.py` & `Agently-3.2.2.0a1/Agently/Workflow/Chunk.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,31 +13,22 @@
         """
         可选参数 handles(连接点，{'inputs': [], 'outputs': []}) 字段，如没有 handles 字段，则会自动追加上默认设置、interactions、title，必选参数 executor，或 type 为 'Start'
         """
         # 校验必填字段(要么 type 为特殊类型，否则必须包含 executor)
         if not type or (type not in SPECIAL_CHUNK_TYPES):
             if not executor:
                 raise ValueError("Missing required key: 'executor'")
-        
-        handles = chunk_desc.get('handles') or {
-            'inputs': [DEFAULT_INPUT_HANDLE.copy()],
-            'outputs': [DEFAULT_OUTPUT_HANDLE.copy()]
-        }
-        if 'inputs' not in handles:
-            handles['inputs'] = [DEFAULT_INPUT_HANDLE.copy()]
-        if 'outputs' not in handles:
-            handles['outputs'] = [DEFAULT_OUTPUT_HANDLE.copy()]
 
         self.chunk = {
             'id': chunk_desc.get('id', str(uuid.uuid4())),
             'title': chunk_desc.get('title'),
             'interactions': chunk_desc.get('interactions') or {}, # 交互配置
             'type': type or EXECUTOR_TYPE_NORMAL,
             'executor': executor,
-            'handles': handles,
+            'handles': self._fix_handles(chunk_desc.get('handles')),
             # 连接条件（默认无条件连通）
             'connect_condition': chunk_desc.get('connect_condition') or None,
             # 当前激活的待连接的 handle 名
             'active_handle': chunk_desc.get('active_handle') or None
         }
 
         self.workflow_schema = workflow_schema
@@ -150,8 +141,33 @@
         self.chunk['connect_condition'] = condition
     
     def has_handle(self, name: str, from_inputs = True) -> bool:
         """
         判断连接手柄是否存在
         """
         search_range = self.chunk.get('handles').get('inputs' if from_inputs else 'outputs', [])
-        return has_target_by_attr(search_range, 'handle', name)
+        return has_target_by_attr(search_range, 'handle', name)
+
+    def _fix_handles(self, custom_handles):
+        """修正用户传入的 handles 配置"""
+        # 处理默认 handle
+        handles = custom_handles or {
+            'inputs': [DEFAULT_INPUT_HANDLE.copy()],
+            'outputs': [DEFAULT_OUTPUT_HANDLE.copy()]
+        }
+        if 'inputs' not in handles:
+            handles['inputs'] = [DEFAULT_INPUT_HANDLE.copy()]
+        if 'outputs' not in handles:
+            handles['outputs'] = [DEFAULT_OUTPUT_HANDLE.copy()]
+
+        # 处理 handle 点简写的情况（如：{ "inputs": ['topic', 'type'], "outputs": [{"handle": "output"}] } 中的 inputs 的定义方式）
+        def fix_handle_core(handle_list):
+            if not handle_list:
+                return
+            if handle_list and len(handle_list):
+                for idx, handle in enumerate(handle_list):
+                    if isinstance(handle, str):
+                        handle_list[idx] = { "handle": handle }
+
+        fix_handle_core(handles['inputs'])
+        fix_handle_core(handles['outputs'])
+        return handles
```

### Comparing `Agently-3.2.1.3/Agently/Workflow/Schema.py` & `Agently-3.2.2.0a1/Agently/Workflow/Schema.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/Workflow/Workflow.py` & `Agently-3.2.2.0a1/Agently/Workflow/Workflow.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from .MainExecutor import MainExecutor
 from .utils.exec_tree import resolve_runtime_data
 from .Schema import Schema
 from ..utils import RuntimeCtx
 from .._global import global_settings
 from .executors.install import mount_built_in_executors
-from .lib.constants import EXECUTOR_TYPE_NORMAL, DEFAULT_INPUT_HANDLE_VALUE, DEFAULT_OUTPUT_HANDLE_VALUE
+from .lib.constants import EXECUTOR_TYPE_NORMAL
 from .lib.painter import draw_with_mermaid
+from .yamlflow.yamlflow import start_yaml_from_str, start_yaml_from_path
+from .lib.ChunkExecutorManager import ChunkExecutorManager
 from Agently.utils import IdGenerator
 
 class Workflow:
     def __init__(self, *, schema_data: dict = None, settings: dict = {}, workflow_id:str=None):
         """
         Workflow，初始参数 schema_data 形如 { 'chunks': [], 'edges': [] }，handler 为要处理响应的函数
         """
@@ -22,27 +24,46 @@
         self.schema = Schema(schema_data or {'chunks': [], 'edges': []})
         # 初始化执行器
         self.executor = MainExecutor(self.workflow_id, self.settings)
         # 装载内置类型
         mount_built_in_executors(self.executor)
         # Chunk Storage
         self.chunks = {}
+        # Executor Manager
+        self.executor_manager = ChunkExecutorManager()
 
     def chunk(self, chunk_id: str, type=EXECUTOR_TYPE_NORMAL, **chunk_desc):
         if "title" not in chunk_desc or chunk_desc["title"] == "":
             chunk_desc.update({ "title": chunk_id })
         def create_chunk_decorator(func: callable):
             return self.chunks.update({
                 chunk_id: self.schema.create_chunk(
                         executor = func,
                         type = type,
                         **chunk_desc
                     )
             })
         return create_chunk_decorator
+
+    def register_executor_func(self, executor_id: str, executor_func: callable):
+        self.executor_manager.register(executor_id, executor_func)
+        return self
+
+    def executor_func(self, executor_id: str):
+        def register_executor_decorator(func: callable):
+            return self.executor_manager.register(executor_id, func)
+        return register_executor_decorator
+
+    def start_yaml(self, yaml_str=None, *, path=None, draw=False):
+        if yaml_str:
+            return start_yaml_from_str(self, yaml_str, draw=draw)
+        elif path:
+            return start_yaml_from_path(self, path, draw=draw)
+        else:
+            raise Exception("[Workflow] At least one parameter in `yaml_str` and `path` is required when using workflow.load_yaml().")
     
     def start(self):
         runtime_data = resolve_runtime_data(self.schema)
         self.executor.start(runtime_data)
     
     def reset(self, schema_data: dict):
         self.schema = Schema(schema_data or {'chunks': [], 'edges': []})
```

### Comparing `Agently-3.2.1.3/Agently/Workflow/lib/ChunkExecutorABC.py` & `Agently-3.2.2.0a1/Agently/Workflow/lib/ChunkExecutorABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/Workflow/lib/constants.py` & `Agently-3.2.2.0a1/Agently/Workflow/lib/constants.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/Workflow/lib/painter.py` & `Agently-3.2.2.0a1/Agently/Workflow/lib/painter.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/Workflow/utils/find.py` & `Agently-3.2.2.0a1/Agently/Workflow/utils/find.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/Workflow/utils/logger.py` & `Agently-3.2.2.0a1/Agently/Workflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/Workflow/utils/runtime_supports.py` & `Agently-3.2.2.0a1/Agently/Workflow/utils/runtime_supports.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/__init__.py` & `Agently-3.2.2.0a1/Agently/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/_global.py` & `Agently-3.2.2.0a1/Agently/_global.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/__init__.py` & `Agently-3.2.2.0a1/Agently/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/agent_component/Decorator.py` & `Agently-3.2.2.0a1/Agently/plugins/agent_component/Decorator.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/agent_component/EventListener.py` & `Agently-3.2.2.0a1/Agently/plugins/agent_component/EventListener.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/agent_component/OpenAIAssistant.py` & `Agently-3.2.2.0a1/Agently/plugins/agent_component/OpenAIAssistant.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/agent_component/ReplyReformer.py` & `Agently-3.2.2.0a1/Agently/plugins/agent_component/ReplyReformer.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/agent_component/Role.py` & `Agently-3.2.2.0a1/Agently/plugins/agent_component/Role.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/agent_component/Search.py` & `Agently-3.2.2.0a1/Agently/plugins/agent_component/Search.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/agent_component/Segment.py` & `Agently-3.2.2.0a1/Agently/plugins/agent_component/Segment.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/agent_component/Session.py` & `Agently-3.2.2.0a1/Agently/plugins/agent_component/Session.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/agent_component/Status.py` & `Agently-3.2.2.0a1/Agently/plugins/agent_component/Status.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/agent_component/Tool.py` & `Agently-3.2.2.0a1/Agently/plugins/agent_component/Tool.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/agent_component/UserInfo.py` & `Agently-3.2.2.0a1/Agently/plugins/agent_component/UserInfo.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/agent_component/__init__.py` & `Agently-3.2.2.0a1/Agently/plugins/agent_component/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/agent_component/utils/ComponentABC.py` & `Agently-3.2.2.0a1/Agently/plugins/agent_component/utils/ComponentABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/facility/Embedding.py` & `Agently-3.2.2.0a1/Agently/plugins/facility/Embedding.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/facility/RoleManager.py` & `Agently-3.2.2.0a1/Agently/plugins/facility/RoleManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/facility/StatusManager.py` & `Agently-3.2.2.0a1/Agently/plugins/facility/StatusManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/facility/__init__.py` & `Agently-3.2.2.0a1/Agently/plugins/facility/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/request/Claude.py` & `Agently-3.2.2.0a1/Agently/plugins/request/Claude.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,55 +14,55 @@
             "stream": True,
         }
     
     def construct_request_messages(self):
         #init request messages
         request_messages = []
         # - general instruction
-        general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general_instruction")
+        general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general")
         if general_instruction_data:
             request_messages.append({ "role": "system", "content": [{"type": "text", "text": f"[GENERAL INSTRUCTION]\n{ to_instruction(general_instruction_data) }" }] })
         # - role
         role_data = self.request.request_runtime_ctx.get_trace_back("prompt.role")
         if role_data:
             request_messages.append({ "role": "system", "content": [{"type": "text", "text": f"[ROLE SETTINGS]\n{ to_instruction(role_data) }" }] })
         # - user info
         user_info_data = self.request.request_runtime_ctx.get_trace_back("prompt.user_info")
         if user_info_data:
             request_messages.append({ "role": "system", "content": [{"type": "text", "text": f"[ABOUT USER]\n{ to_instruction(user_info_data) }" }] })
-        # - headline
-        headline_data = self.request.request_runtime_ctx.get_trace_back("prompt.headline")
+        # - abstract
+        headline_data = self.request.request_runtime_ctx.get_trace_back("prompt.abstract")
         if headline_data:
             request_messages.append({ "role": "assistant", "content": [{"type": "text", "text": to_instruction(headline_data) }] })
         # - chat history
         chat_history_data = self.request.request_runtime_ctx.get_trace_back("prompt.chat_history")
         if chat_history_data:
             request_messages.extend(chat_history_data)
         # - request message (prompt)
         prompt_input_data = self.request.request_runtime_ctx.get_trace_back("prompt.input")
-        prompt_information_data = self.request.request_runtime_ctx.get_trace_back("prompt.information")
-        prompt_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.instruction")
+        prompt_info_data = self.request.request_runtime_ctx.get_trace_back("prompt.info")
+        prompt_instruct_data = self.request.request_runtime_ctx.get_trace_back("prompt.instruct")
         prompt_output_data = self.request.request_runtime_ctx.get_trace_back("prompt.output")
         # - files
         files_data = self.request.request_runtime_ctx.get_trace_back("prompt.files")
         # --- only input
-        if not prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
-            raise Exception("[Request] Missing 'prompt.input', 'prompt.information', 'prompt.instruction', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
+        if not prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
+            raise Exception("[Request] Missing 'prompt.input', 'prompt.info', 'prompt.instruct', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
         prompt_text = ""
-        if prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
+        if prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
             prompt_text = to_instruction(prompt_input_data)
         # --- construct prompt
         else:
             prompt_dict = {}
             if prompt_input_data:
                 prompt_dict["[INPUT]"] = to_instruction(prompt_input_data)
-            if prompt_information_data:
-                prompt_dict["[HELPFUL INFORMATION]"] = str(prompt_information_data)
-            if prompt_instruction_data:
-                prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruction_data)
+            if prompt_info_data:
+                prompt_dict["[HELPFUL INFORMATION]"] = str(prompt_info_data)
+            if prompt_instruct_data:
+                prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruct_data)
             if prompt_output_data:
                 if isinstance(prompt_output_data, (dict, list, set)):
                     prompt_dict["[OUTPUT REQUIREMENT]"] = {
                         "TYPE": "JSON can be parsed in Python",
                         "FORMAT": to_json_desc(prompt_output_data),
                     }
                     self.request.request_runtime_ctx.set("response:type", "JSON")
```

### Comparing `Agently-3.2.1.3/Agently/plugins/request/ERNIE.py` & `Agently-3.2.2.0a1/Agently/plugins/request/ERNIE.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,58 +23,58 @@
         return client
 
     def construct_request_messages(self):
         # init request messages
         request_messages = []
         # - general instruction
         general_instruction_data = self.request.request_runtime_ctx.get(
-            "prompt.general_instruction")
+            "prompt.general")
         if general_instruction_data:
             request_messages.append({"role": "system",
                                      "content": f"[重要指导说明]\n{to_instruction(general_instruction_data)}"})
         # - role
         role_data = self.request.request_runtime_ctx.get("prompt.role")
         if role_data:
             request_messages.append(
                 {"role": "system", "content": f"[角色及行为设定]\n{to_instruction(role_data)}"})
         # - user info
         user_info_data = self.request.request_runtime_ctx.get("prompt.user_info")
         if user_info_data:
             request_messages.append(
                 {"role": "system", "content": f"[用户信息]\n{to_instruction(user_info_data)}"})
-        # - headline
-        headline_data = self.request.request_runtime_ctx.get("prompt.headline")
+        # - abstract
+        headline_data = self.request.request_runtime_ctx.get("prompt.abstract")
         if headline_data:
             request_messages.append(
                 {"role": "user", "content": f"[主题及摘要]{to_instruction(headline_data)}"})
             request_messages.append({"role": "assistant", "content": "OK"})
         # - chat history
         chat_history_data = self.request.request_runtime_ctx.get("prompt.chat_history")
         if chat_history_data:
             request_messages.extend(chat_history_data)
         # - request message (prompt)
         prompt_input_data = self.request.request_runtime_ctx.get("prompt.input")
-        prompt_information_data = self.request.request_runtime_ctx.get("prompt.information")
-        prompt_instruction_data = self.request.request_runtime_ctx.get("prompt.instruction")
+        prompt_info_data = self.request.request_runtime_ctx.get("prompt.info")
+        prompt_instruct_data = self.request.request_runtime_ctx.get("prompt.instruct")
         prompt_output_data = self.request.request_runtime_ctx.get("prompt.output")
         # --- only input
-        if not prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
+        if not prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
             raise Exception(
-                "[Request] Missing 'prompt.input', 'prompt.information', 'prompt.instruction', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
-        if prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
+                "[Request] Missing 'prompt.input', 'prompt.info', 'prompt.instruct', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
+        if prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
             request_messages.append({"role": "user", "content": to_instruction(prompt_input_data)})
         # --- construct prompt
         else:
             prompt_dict = {}
             if prompt_input_data:
                 prompt_dict["[输入]"] = to_instruction(prompt_input_data)
-            if prompt_information_data:
-                prompt_dict["[补充信息]"] = str(prompt_information_data)
-            if prompt_instruction_data:
-                prompt_dict["[处理规则]"] = to_instruction(prompt_instruction_data)
+            if prompt_info_data:
+                prompt_dict["[补充信息]"] = str(prompt_info_data)
+            if prompt_instruct_data:
+                prompt_dict["[处理规则]"] = to_instruction(prompt_instruct_data)
             if prompt_output_data:
                 if isinstance(prompt_output_data, (dict, list, set)):
                     prompt_dict["[输出要求]"] = {
                         "TYPE": "可被解析的JSON字符串",
                         "FORMAT": to_json_desc(prompt_output_data),
                     }
                     self.request.request_runtime_ctx.set("response:type", "JSON")
```

### Comparing `Agently-3.2.1.3/Agently/plugins/request/Google.py` & `Agently-3.2.2.0a1/Agently/plugins/request/Google.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,39 +9,39 @@
         self.model_name = "Google"
         self.model_settings = RuntimeCtxNamespace(f"model.{ self.model_name }", self.request.settings)
         
     def construct_request_messages(self):
         #init request messages
         request_messages = []
         # - general instruction
-        general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general_instruction")
+        general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general")
         if general_instruction_data:
-            request_messages.append({ "role": "user", "parts": [{ "text": f"[YOUR GENERAL INSTRUCTION]?" }] })
+            request_messages.append({ "role": "user", "parts": [{ "text": f"[YOUR GENERAL INSTRUCTION]:" }] })
             request_messages.append({ "role": "model", "parts": [{ "text": f"{ to_instruction(general_instruction_data) }" }] })
         # - role
         role_data = self.request.request_runtime_ctx.get_trace_back("prompt.role")
         if role_data:
-            request_messages.append({ "role": "user", "parts": [{ "text": f"[YOUR ROLE SETTINGS]?" }] })
+            request_messages.append({ "role": "user", "parts": [{ "text": f"[YOUR ROLE DESCRIPTION]:" }] })
             request_messages.append({ "role": "model", "parts": [{ "text": f"{ to_instruction(role_data) }" }] })
         # - user info
         user_info_data = self.request.request_runtime_ctx.get_trace_back("prompt.user_info")
         if user_info_data:
-            request_messages.append({ "role": "user", "parts": [{ "text": f"[USER INFO WHOM YOU'RE TALKING TO]?" }] })
+            request_messages.append({ "role": "user", "parts": [{ "text": f"[USER'S INTRODUCTION ABOUT HIMSELF/HERSELF]:" }] })
             request_messages.append({ "role": "model", "parts": [{ "text": f"{ to_instruction(user_info_data) }" }] })
-        # - headline
-        headline_data = self.request.request_runtime_ctx.get_trace_back("prompt.headline")
+        # - abstract
+        headline_data = self.request.request_runtime_ctx.get_trace_back("prompt.abstract")
         if headline_data:
-            request_messages.append({ "role": "user", "parts": [{ "text": f"[HEADLINE ABOUT WHAT WE'RE TALKING ABOUT]?" }] })
+            request_messages.append({ "role": "user", "parts": [{ "text": f"[ABSTRACT ABOUT CHAT HISTORY BEFORE]:" }] })
             request_messages.append({ "role": "model", "parts": [{ "text": f"{ to_instruction(headline_data) }" }] })
         # - chat history
         chat_history_data = self.request.request_runtime_ctx.get_trace_back("prompt.chat_history")
         if chat_history_data:
             # make sure start with role "user"
             if chat_history_data[0]["role"] != "user":
-                request_messages.append({ "role": "user", "parts": [{ "text": "[CHAT HISTORY]:" }] })
+                request_messages.append({ "role": "user", "parts": [{ "text": "[LATEST CHAT HISTORY]:" }] })
                 current_role = "model"
             else:
                 current_role = "user"
             for message in chat_history_data:
                 if message["role"] != "user":
                     message["role"] = "model"
                 if message["role"] == current_role:
@@ -50,34 +50,34 @@
                     request_messages[-1]["parts"][0]["text"] += f"\n{ message['content'] }"
                 current_role = "user" if current_role == "model" else "model"
             # make sure end with role "model"
             if request_messages[-1]["role"] != "model":
                 request_messages.append({ "role": "model", "parts": [{ "text": "[CHAT HISTORY END]" }] })
         # - request message (prompt)
         prompt_input_data = self.request.request_runtime_ctx.get_trace_back("prompt.input")
-        prompt_information_data = self.request.request_runtime_ctx.get_trace_back("prompt.information")
-        prompt_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.instruction")
+        prompt_info_data = self.request.request_runtime_ctx.get_trace_back("prompt.info")
+        prompt_instruct_data = self.request.request_runtime_ctx.get_trace_back("prompt.instruct")
         prompt_output_data = self.request.request_runtime_ctx.get_trace_back("prompt.output")
         # - files
         files_data = self.request.request_runtime_ctx.get_trace_back("prompt.files")
         # --- only input
-        if not prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
-            raise Exception("[Request] Missing 'prompt.input', 'prompt.information', 'prompt.instruction', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
+        if not prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
+            raise Exception("[Request] Missing 'prompt.input', 'prompt.info', 'prompt.instruct', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
         prompt_text = ""
-        if prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
+        if prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
             prompt_text = to_instruction(prompt_input_data)
         # --- construct prompt
         else:
             prompt_dict = {}
             if prompt_input_data:
                 prompt_dict["[INPUT]"] = to_instruction(prompt_input_data)
-            if prompt_information_data:
-                prompt_dict["[HELPFUL INFORMATION]"] = str(prompt_information_data)
-            if prompt_instruction_data:
-                prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruction_data)
+            if prompt_info_data:
+                prompt_dict["[HELPFUL INFORMATION]"] = str(prompt_info_data)
+            if prompt_instruct_data:
+                prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruct_data)
             if prompt_output_data:
                 if isinstance(prompt_output_data, (dict, list, set)):
                     prompt_dict["[OUTPUT REQUIREMENT]"] = {
                         "TYPE": "JSON can be parsed in runtime",
                         "FORMAT": to_json_desc(prompt_output_data),
                     }
                     self.request.request_runtime_ctx.set("response:type", "JSON")
```

### Comparing `Agently-3.2.1.3/Agently/plugins/request/Kimi.py` & `Agently-3.2.2.0a1/Agently/plugins/request/Kimi.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,55 +30,55 @@
         client = OpenAIClient(**client_params)
         return client
 
     def construct_request_messages(self):
         #init request messages
         request_messages = []
         # - general instruction
-        general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general_instruction")
+        general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general")
         if general_instruction_data:
             request_messages.append({ "role": "system", "content": f"[GENERAL INSTRUCTION]\n{ to_instruction(general_instruction_data) }" })
         # - role
         role_data = self.request.request_runtime_ctx.get_trace_back("prompt.role")
         if role_data:
             request_messages.append({ "role": "system", "content": f"[ROLE SETTINGS]\n{ to_instruction(role_data) }" })
         # - user info
         user_info_data = self.request.request_runtime_ctx.get_trace_back("prompt.user_info")
         if user_info_data:
             request_messages.append({ "role": "system", "content": f"[ABOUT USER]\n{ to_instruction(user_info_data) }" })
-        # - headline
-        headline_data = self.request.request_runtime_ctx.get_trace_back("prompt.headline")
+        # - abstract
+        headline_data = self.request.request_runtime_ctx.get_trace_back("prompt.abstract")
         if headline_data:
             request_messages.append({ "role": "assistant", "content": to_instruction(headline_data) })
         # - chat history
         chat_history_data = self.request.request_runtime_ctx.get_trace_back("prompt.chat_history")
         if chat_history_data:
             request_messages.extend(chat_history_data)
         # - request message (prompt)
         prompt_input_data = self.request.request_runtime_ctx.get_trace_back("prompt.input")
-        prompt_information_data = self.request.request_runtime_ctx.get_trace_back("prompt.information")
-        prompt_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.instruction")
+        prompt_info_data = self.request.request_runtime_ctx.get_trace_back("prompt.info")
+        prompt_instruct_data = self.request.request_runtime_ctx.get_trace_back("prompt.instruct")
         prompt_output_data = self.request.request_runtime_ctx.get_trace_back("prompt.output")
         # - files
         files_data = self.request.request_runtime_ctx.get_trace_back("prompt.files")
         # --- only input
-        if not prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
-            raise Exception("[Request] Missing 'prompt.input', 'prompt.information', 'prompt.instruction', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
+        if not prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
+            raise Exception("[Request] Missing 'prompt.input', 'prompt.info', 'prompt.instruct', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
         prompt_text = ""
-        if prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
+        if prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
             prompt_text = to_instruction(prompt_input_data)
         # --- construct prompt
         else:
             prompt_dict = {}
             if prompt_input_data:
                 prompt_dict["[INPUT]"] = to_instruction(prompt_input_data)
-            if prompt_information_data:
-                prompt_dict["[HELPFUL INFORMATION]"] = str(prompt_information_data)
-            if prompt_instruction_data:
-                prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruction_data)
+            if prompt_info_data:
+                prompt_dict["[HELPFUL INFORMATION]"] = str(prompt_info_data)
+            if prompt_instruct_data:
+                prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruct_data)
             if prompt_output_data:
                 if isinstance(prompt_output_data, (dict, list, set)):
                     prompt_dict["[OUTPUT REQUIREMENT]"] = {
                         "TYPE": "JSON can be parsed in Python",
                         "FORMAT": to_json_desc(prompt_output_data),
                     }
                     self.request.request_runtime_ctx.set("response:type", "JSON")
```

### Comparing `Agently-3.2.1.3/Agently/plugins/request/MiniMax.py` & `Agently-3.2.2.0a1/Agently/plugins/request/MiniMax.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 if role_val:
                     bot_role_name = role_val
                     break
             req_bot_desc.append(to_instruction(role_data))
 
         # 处理指令
         general_instruction_data = self.request.request_runtime_ctx.get_trace_back(
-            "prompt.general_instruction")
+            "prompt.general")
         if general_instruction_data:
             req_bot_desc.append(
                 f"[重要指导说明]{to_instruction(general_instruction_data)}")
 
         # 处理用户信息
         user_role_name = DEFAULT_USER_NAME
         user_info_data = self.request.request_runtime_ctx.get_trace_back(
@@ -63,15 +63,15 @@
                     break
             req_messages.append(to_user_msg(
                 f"[这是我的信息介绍]：{to_instruction(user_info_data)}", user_role_name))
             req_messages.append(to_bot_msg('收到', bot_role_name))
 
         # 主题摘要
         headline_data = self.request.request_runtime_ctx.get_trace_back(
-            "prompt.headline")
+            "prompt.abstract")
         if headline_data:
             req_messages.append(to_user_msg(
                 f"[这是我们要聊的话题]：{to_instruction(headline_data)}", user_role_name))
             req_messages.append(to_bot_msg('收到', bot_role_name))
 
         # 历史信息
         chat_history_data = self.request.request_runtime_ctx.get(
@@ -82,31 +82,31 @@
                 user_name=user_role_name,
                 robot_name=bot_role_name
             ))
 
         # - request message (prompt)
         prompt_input_data = self.request.request_runtime_ctx.get(
             "prompt.input")
-        prompt_information_data = self.request.request_runtime_ctx.get(
-            "prompt.information")
-        prompt_instruction_data = self.request.request_runtime_ctx.get(
-            "prompt.instruction")
+        prompt_info_data = self.request.request_runtime_ctx.get(
+            "prompt.info")
+        prompt_instruct_data = self.request.request_runtime_ctx.get(
+            "prompt.instruct")
         prompt_output_data = self.request.request_runtime_ctx.get(
             "prompt.output")
         # --- only input
-        if not prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
+        if not prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
             raise Exception(
-                "[Request] Missing 'prompt.input', 'prompt.information', 'prompt.instruction', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
+                "[Request] Missing 'prompt.input', 'prompt.info', 'prompt.instruct', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
 
         func_args = {}
         prompt_dict = {}
-        if prompt_information_data:
-            prompt_dict["[补充信息]"] = str(prompt_information_data)
-        if prompt_instruction_data:
-            prompt_dict["[处理规则]"] = to_instruction(prompt_instruction_data)
+        if prompt_info_data:
+            prompt_dict["[补充信息]"] = str(prompt_info_data)
+        if prompt_instruct_data:
+            prompt_dict["[处理规则]"] = to_instruction(prompt_instruct_data)
 
         if prompt_output_data:
             if isinstance(prompt_output_data, (dict, list, set)):
                 # 采用 func 辅助修正格式
                 if self.use_func_fix_json:
                     func_args["functions"] = [{
                         "name": "output_result",
```

### Comparing `Agently-3.2.1.3/Agently/plugins/request/OAIClient.py` & `Agently-3.2.2.0a1/Agently/plugins/request/OAIClient.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,53 +20,53 @@
         if not self.model_settings.get_trace_back("message_rules.no_multi_type_messages"):
             self.model_settings.set("message_rules.no_multi_type_messages", True)    
 
     def construct_request_messages(self):
         #init request messages
         request_messages = []
         # - general instruction
-        general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general_instruction")
+        general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general")
         if general_instruction_data:
             request_messages.append({ "role": "system", "content": [{"type": "text", "text": f"[GENERAL INSTRUCTION]\n{ to_instruction(general_instruction_data) }" }] })
         # - role
         role_data = self.request.request_runtime_ctx.get_trace_back("prompt.role")
         if role_data:
             request_messages.append({ "role": "system", "content": [{"type": "text", "text": f"[ROLE SETTINGS]\n{ to_instruction(role_data) }" }] })
         # - user info
         user_info_data = self.request.request_runtime_ctx.get_trace_back("prompt.user_info")
         if user_info_data:
             request_messages.append({ "role": "system", "content": [{"type": "text", "text": f"[ABOUT USER]\n{ to_instruction(user_info_data) }" }] })
-        # - headline
-        headline_data = self.request.request_runtime_ctx.get_trace_back("prompt.headline")
+        # - abstract
+        headline_data = self.request.request_runtime_ctx.get_trace_back("prompt.abstract")
         if headline_data:
             request_messages.append({ "role": "assistant", "content": [{"type": "text", "text": f"[ABSTRACT]\n{ to_instruction(headline_data) }" }] })
         # - chat history
         chat_history_data = self.request.request_runtime_ctx.get_trace_back("prompt.chat_history")
         if chat_history_data:
             request_messages.extend(chat_history_data)
         # - request message (prompt)
         prompt_input_data = self.request.request_runtime_ctx.get_trace_back("prompt.input")
-        prompt_information_data = self.request.request_runtime_ctx.get_trace_back("prompt.information")
-        prompt_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.instruction")
+        prompt_info_data = self.request.request_runtime_ctx.get_trace_back("prompt.info")
+        prompt_instruct_data = self.request.request_runtime_ctx.get_trace_back("prompt.instruct")
         prompt_output_data = self.request.request_runtime_ctx.get_trace_back("prompt.output")
         # --- only input
-        if not prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
-            raise Exception("[Request] Missing 'prompt.input', 'prompt.information', 'prompt.instruction', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
+        if not prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
+            raise Exception("[Request] Missing 'prompt.input', 'prompt.info', 'prompt.instruct', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
         prompt_text = ""
-        if prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
+        if prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
             prompt_text = to_instruction(prompt_input_data)
         # --- construct prompt
         else:
             prompt_dict = {}
             if prompt_input_data:
                 prompt_dict["[INPUT]"] = to_instruction(prompt_input_data)
-            if prompt_information_data:
-                prompt_dict["[HELPFUL INFORMATION]"] = str(prompt_information_data)
-            if prompt_instruction_data:
-                prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruction_data)
+            if prompt_info_data:
+                prompt_dict["[HELPFUL INFORMATION]"] = str(prompt_info_data)
+            if prompt_instruct_data:
+                prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruct_data)
             if prompt_output_data:
                 if isinstance(prompt_output_data, (dict, list, set)):
                     prompt_dict["[OUTPUT REQUIREMENT]"] = {
                         "TYPE": "JSON can be parsed in Python",
                         "FORMAT": to_json_desc(prompt_output_data),
                     }
                     self.request.request_runtime_ctx.set("response:type", "JSON")
@@ -120,39 +120,39 @@
                         formatted_messages.append({ "role": message["role"], "content": item["text"] })
         return formatted_messages
 
     def construct_completion_prompt(self):
         # - init prompt
         completion_prompt = ""
         # - general instruction
-        general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general_instruction")
+        general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general")
         if general_instruction_data:
             completion_prompt += f"[GENERAL INSTRUCTION]\n{ to_instruction(general_instruction_data) }\n"
         # - role
         role_data = self.request.request_runtime_ctx.get_trace_back("prompt.role")
         if role_data:
             completion_prompt += f"[ROLE SETTINGS]\n{ to_instruction(role_data) }\n"
         # - user info
         user_info_data = self.request.request_runtime_ctx.get_trace_back("prompt.user_info")
         if user_info_data:
             completion_prompt += f"[ABOUT USER]\n{ to_instruction(user_info_data) }\n"
-        # - headline
-        headline_data = self.request.request_runtime_ctx.get_trace_back("prompt.headline")
+        # - abstract
+        headline_data = self.request.request_runtime_ctx.get_trace_back("prompt.abstract")
         if headline_data:
             completion_prompt += f"[ABSTRACT]\n{ to_instruction(headline_data) }\n"
         # - main prompt
         chat_history_data = self.request.request_runtime_ctx.get_trace_back("prompt.chat_history")
         prompt_input_data = self.request.request_runtime_ctx.get_trace_back("prompt.input")
-        prompt_information_data = self.request.request_runtime_ctx.get_trace_back("prompt.information")
-        prompt_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.instruction")
+        prompt_info_data = self.request.request_runtime_ctx.get_trace_back("prompt.info")
+        prompt_instruct_data = self.request.request_runtime_ctx.get_trace_back("prompt.instruct")
         prompt_output_data = self.request.request_runtime_ctx.get_trace_back("prompt.output")
-        if not prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data and not chat_history_data:
-            raise Exception("[Request] Missing 'prompt.chat_history', 'prompt.input', 'prompt.information', 'prompt.instruction', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
+        if not prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data and not chat_history_data:
+            raise Exception("[Request] Missing 'prompt.chat_history', 'prompt.input', 'prompt.info', 'prompt.instruct', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
         # --- only input
-        if prompt_input_data and not chat_history_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
+        if prompt_input_data and not chat_history_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
             if completion_prompt == "":
                 completion_prompt += to_instruction(prompt_input_data)
             else:
                 completion_prompt += f"[OUTPUT]\n{ to_instruction(prompt_input_data) }"
         # --- construct prompt
         else:
             # - with output format
@@ -160,36 +160,36 @@
                 prompt_dict = {}
                 if chat_history_data:
                     prompt_dict["[HISTORY LOGS]"] = ""
                     for message in chat_history_data:
                         prompt_dict["[HISTORY LOGS]"] += f"{ message['role'] }: { message['content'] }\n"
                 if prompt_input_data:
                     prompt_dict["[INPUT]"] = to_instruction(prompt_input_data)
-                if prompt_information_data:
-                    prompt_dict["[HELPFUL INFORMATION]"] = str(prompt_information_data)
-                if prompt_instruction_data:
-                    prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruction_data)
+                if prompt_info_data:
+                    prompt_dict["[HELPFUL INFORMATION]"] = str(prompt_info_data)
+                if prompt_instruct_data:
+                    prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruct_data)
                 if prompt_output_data:
                     prompt_dict["[OUTPUT REQUIREMENT]"] = {
                         "TYPE": "JSON can be parsed in Python",
                         "FORMAT": to_json_desc(prompt_output_data),
                     }
                     self.request.request_runtime_ctx.set("response:type", "JSON")
                 completion_prompt += to_prompt_structure(
                     prompt_dict,
                     end="[OUTPUT]:\nassistant: "
                         if chat_history_data and len(chat_history_data) > 0
                         else "[OUTPUT]:\n"
                 )
             # without output format
             else:
-                if prompt_information_data:
-                    completion_prompt += f"[HELPFUL INFORMATION]\n{ str(prompt_information_data) }\n"
-                if prompt_instruction_data:
-                    completion_prompt += f"[INSTRUCTION]\n{ to_instruction(prompt_instruction_data) }\n"
+                if prompt_info_data:
+                    completion_prompt += f"[HELPFUL INFORMATION]\n{ str(prompt_info_data) }\n"
+                if prompt_instruct_data:
+                    completion_prompt += f"[INSTRUCTION]\n{ to_instruction(prompt_instruct_data) }\n"
                 if prompt_output_data:
                     completion_prompt += f"[OUTPUT REQUIREMENT]\n{ str(prompt_output_data) }\n"
                 completion_prompt += "[OUTPUT]\n"
                 # chat completion
                 if chat_history_data:
                     for message in chat_history_data:
                         completion_prompt += f"{ message['role'] }: { message['content'] }\n"
```

### Comparing `Agently-3.2.1.3/Agently/plugins/request/OpenAI.py` & `Agently-3.2.2.0a1/Agently/plugins/request/OpenAI.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,55 +31,55 @@
         client = OpenAIClient(**client_params)
         return client
 
     def construct_request_messages(self):
         #init request messages
         request_messages = []
         # - general instruction
-        general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general_instruction")
+        general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general")
         if general_instruction_data:
             request_messages.append({ "role": "system", "content": f"[GENERAL INSTRUCTION]\n{ to_instruction(general_instruction_data) }" })
         # - role
         role_data = self.request.request_runtime_ctx.get_trace_back("prompt.role")
         if role_data:
             request_messages.append({ "role": "system", "content": f"[ROLE SETTINGS]\n{ to_instruction(role_data) }" })
         # - user info
         user_info_data = self.request.request_runtime_ctx.get_trace_back("prompt.user_info")
         if user_info_data:
             request_messages.append({ "role": "system", "content": f"[ABOUT USER]\n{ to_instruction(user_info_data) }" })
-        # - headline
-        headline_data = self.request.request_runtime_ctx.get_trace_back("prompt.headline")
+        # - abstract
+        headline_data = self.request.request_runtime_ctx.get_trace_back("prompt.abstract")
         if headline_data:
             request_messages.append({ "role": "assistant", "content": to_instruction(headline_data) })
         # - chat history
         chat_history_data = self.request.request_runtime_ctx.get_trace_back("prompt.chat_history")
         if chat_history_data:
             request_messages.extend(chat_history_data)
         # - request message (prompt)
         prompt_input_data = self.request.request_runtime_ctx.get_trace_back("prompt.input")
-        prompt_information_data = self.request.request_runtime_ctx.get_trace_back("prompt.information")
-        prompt_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.instruction")
+        prompt_info_data = self.request.request_runtime_ctx.get_trace_back("prompt.info")
+        prompt_instruct_data = self.request.request_runtime_ctx.get_trace_back("prompt.instruct")
         prompt_output_data = self.request.request_runtime_ctx.get_trace_back("prompt.output")
         # - files
         files_data = self.request.request_runtime_ctx.get_trace_back("prompt.files")
         # --- only input
-        if not prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
-            raise Exception("[Request] Missing 'prompt.input', 'prompt.information', 'prompt.instruction', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
+        if not prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
+            raise Exception("[Request] Missing 'prompt.input', 'prompt.info', 'prompt.instruct', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
         prompt_text = ""
-        if prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
+        if prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
             prompt_text = to_instruction(prompt_input_data)
         # --- construct prompt
         else:
             prompt_dict = {}
             if prompt_input_data:
                 prompt_dict["[INPUT]"] = to_instruction(prompt_input_data)
-            if prompt_information_data:
-                prompt_dict["[HELPFUL INFORMATION]"] = str(prompt_information_data)
-            if prompt_instruction_data:
-                prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruction_data)
+            if prompt_info_data:
+                prompt_dict["[HELPFUL INFORMATION]"] = str(prompt_info_data)
+            if prompt_instruct_data:
+                prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruct_data)
             if prompt_output_data:
                 if isinstance(prompt_output_data, (dict, list, set)):
                     prompt_dict["[OUTPUT REQUIREMENT]"] = {
                         "TYPE": "JSON can be parsed in Python",
                         "FORMAT": to_json_desc(prompt_output_data),
                     }
                     self.request.request_runtime_ctx.set("response:type", "JSON")
```

### Comparing `Agently-3.2.1.3/Agently/plugins/request/ZhipuAI.py` & `Agently-3.2.2.0a1/Agently/plugins/request/ZhipuAI.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,56 +11,56 @@
         if self.request_type == None:
             self.request_type = "chat"
 
     def construct_request_messages(self):
         #init request messages
         request_messages = []
         # - general instruction
-        general_instruction_data = self.request.request_runtime_ctx.get("prompt.general_instruction")
+        general_instruction_data = self.request.request_runtime_ctx.get("prompt.general")
         if general_instruction_data:
             request_messages.append({ "role": "user", "content": f"[重要指导说明]\n{ to_instruction(general_instruction_data) }" })
             request_messages.append({ "role": "assistant", "content": "OK" })
         # - role
         role_data = self.request.request_runtime_ctx.get("prompt.role")
         if role_data and self.request_type == "chat":
             request_messages.append({ "role": "user", "content": f"[角色及行为设定]\n{ to_instruction(role_data) }" })
             request_messages.append({ "role": "assistant", "content": "OK" })
         # - user info
         user_info_data = self.request.request_runtime_ctx.get("prompt.user_info")
         if user_info_data and self.request_type == "chat":
             request_messages.append({ "role": "user", "content": f"[用户信息]\n{ to_instruction(user_info_data) }" })
             request_messages.append({ "role": "assistant", "content": "OK" })
-        # - headline
-        headline_data = self.request.request_runtime_ctx.get("prompt.headline")
+        # - abstract
+        headline_data = self.request.request_runtime_ctx.get("prompt.abstract")
         if headline_data:
             request_messages.append({ "role": "user", "content": f"[主题及摘要]{to_instruction(headline_data)}" })
             request_messages.append({ "role": "assistant", "content": "OK" })
         # - chat history
         chat_history_data = self.request.request_runtime_ctx.get("prompt.chat_history")
         if chat_history_data:
             request_messages.extend(chat_history_data)
         # - request message (prompt)
         prompt_input_data = self.request.request_runtime_ctx.get("prompt.input")
-        prompt_information_data = self.request.request_runtime_ctx.get("prompt.information")
-        prompt_instruction_data = self.request.request_runtime_ctx.get("prompt.instruction")
+        prompt_info_data = self.request.request_runtime_ctx.get("prompt.info")
+        prompt_instruct_data = self.request.request_runtime_ctx.get("prompt.instruct")
         prompt_output_data = self.request.request_runtime_ctx.get("prompt.output")
         # --- only input
-        if not prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
-            raise Exception("[Request] Missing 'prompt.input', 'prompt.information', 'prompt.instruction', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
-        if prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
+        if not prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
+            raise Exception("[Request] Missing 'prompt.input', 'prompt.info', 'prompt.instruct', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
+        if prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
             request_messages.append({ "role": "user", "content": to_instruction(prompt_input_data) })
         # --- construct prompt
         else:
             prompt_dict = {}
             if prompt_input_data:
                 prompt_dict["[输入]"] = to_instruction(prompt_input_data)
-            if prompt_information_data:
-                prompt_dict["[补充信息]"] = str(prompt_information_data)
-            if prompt_instruction_data:
-                prompt_dict["[处理规则]"] = to_instruction(prompt_instruction_data)
+            if prompt_info_data:
+                prompt_dict["[补充信息]"] = str(prompt_info_data)
+            if prompt_instruct_data:
+                prompt_dict["[处理规则]"] = to_instruction(prompt_instruct_data)
             if prompt_output_data:
                 if isinstance(prompt_output_data, (dict, list, set)):
                     prompt_dict["[输出要求]"] = {
                         "TYPE": "JSON can be parsed in runtime",
                         "FORMAT": to_json_desc(prompt_output_data),
                     }
                     self.request.request_runtime_ctx.set("response:type", "JSON")
@@ -69,52 +69,52 @@
             request_messages.append({ "role": "user", "content": to_prompt_structure(prompt_dict, end="[输出]:\n") })
         return request_messages
 
     def construct_request_messages_for_gml4(self):
         #init request messages
         request_messages = []
         # - general instruction
-        general_instruction_data = self.request.request_runtime_ctx.get("prompt.general_instruction")
+        general_instruction_data = self.request.request_runtime_ctx.get("prompt.general")
         if general_instruction_data:
             request_messages.append({ "role": "system", "content": f"[重要指导说明]\n{ to_instruction(general_instruction_data) }" })
         # - role
         role_data = self.request.request_runtime_ctx.get("prompt.role")
         if role_data:
             request_messages.append({ "role": "system", "content": f"[角色及行为设定]\n{ to_instruction(role_data) }" })
         # - user info
         user_info_data = self.request.request_runtime_ctx.get("prompt.user_info")
         if user_info_data:
             request_messages.append({ "role": "system", "content": f"[用户信息]\n{ to_instruction(user_info_data) }" })
-        # - headline
-        headline_data = self.request.request_runtime_ctx.get("prompt.headline")
+        # - abstract
+        headline_data = self.request.request_runtime_ctx.get("prompt.abstract")
         if headline_data:
             request_messages.append({ "role": "system", "content": f"[主题及摘要]{to_instruction(headline_data)}" })
         # - chat history
         chat_history_data = self.request.request_runtime_ctx.get("prompt.chat_history")
         if chat_history_data:
             request_messages.extend(chat_history_data)
         # - request message (prompt)
         prompt_input_data = self.request.request_runtime_ctx.get("prompt.input")
-        prompt_information_data = self.request.request_runtime_ctx.get("prompt.information")
-        prompt_instruction_data = self.request.request_runtime_ctx.get("prompt.instruction")
+        prompt_info_data = self.request.request_runtime_ctx.get("prompt.info")
+        prompt_instruct_data = self.request.request_runtime_ctx.get("prompt.instruct")
         prompt_output_data = self.request.request_runtime_ctx.get("prompt.output")
         # --- only input
-        if not prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
-            raise Exception("[Request] Missing 'prompt.input', 'prompt.information', 'prompt.instruction', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
-        if prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
+        if not prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
+            raise Exception("[Request] Missing 'prompt.input', 'prompt.info', 'prompt.instruct', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
+        if prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
             request_messages.append({ "role": "user", "content": to_instruction(prompt_input_data) })
         # --- construct prompt
         else:
             prompt_dict = {}
             if prompt_input_data:
                 prompt_dict["[输入]"] = to_instruction(prompt_input_data)
-            if prompt_information_data:
-                prompt_dict["[补充信息]"] = str(prompt_information_data)
-            if prompt_instruction_data:
-                prompt_dict["[处理规则]"] = to_instruction(prompt_instruction_data)
+            if prompt_info_data:
+                prompt_dict["[补充信息]"] = str(prompt_info_data)
+            if prompt_instruct_data:
+                prompt_dict["[处理规则]"] = to_instruction(prompt_instruct_data)
             if prompt_output_data:
                 if isinstance(prompt_output_data, (dict, list, set)):
                     prompt_dict["[输出要求]"] = {
                         "TYPE": "JSON can be parsed in runtime",
                         "FORMAT": to_json_desc(prompt_output_data),
                     }
                     self.request.request_runtime_ctx.set("response:type", "JSON")
```

### Comparing `Agently-3.2.1.3/Agently/plugins/request/__init__.py` & `Agently-3.2.2.0a1/Agently/plugins/request/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/request/utils/RequestABC.py` & `Agently-3.2.2.0a1/Agently/plugins/request/utils/RequestABC.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,56 +12,56 @@
         # self.model_settings = RuntimeCtxNamespace(f"model.{ self.model_name }", self.request.settings)
 
     def construct_request_messages(self):
         '''
         This is an example to help you understand how to construct your own request message or prompt
         Here're Standard LLM Request Inputs from Agently that you can use :
         self.request.request_runtime_ctx.get("prompt.system")
-        self.request.request_runtime_ctx.get("prompt.headline")
+        self.request.request_runtime_ctx.get("prompt.abstract")
         self.request.request_runtime_ctx.get("prompt.chat_history")
         self.request.request_runtime_ctx.get("prompt.input")
-        self.request.request_runtime_ctx.get("prompt.information")
-        self.request.request_runtime_ctx.get("prompt.instruction")
+        self.request.request_runtime_ctx.get("prompt.info")
+        self.request.request_runtime_ctx.get("prompt.instruct")
         self.request.request_runtime_ctx.get("prompt.output")
         You can use them to construct request or prompt following the model rules.
         And down below is just one example that usually fits OpenAI messages rules.
         '''
         #init request messages
         request_messages = []
         # - system message
         system_data = self.request.request_runtime_ctx.get("prompt.system")
         if system_data:
             request_messages.append({ "role": "system", "content": to_instruction(system_data) })
-        # - headline
-        headline_data = self.request.request_runtime_ctx.get("prompt.headline")
+        # - abstract
+        headline_data = self.request.request_runtime_ctx.get("prompt.abstract")
         if headline_data:
             request_messages.append({ "role": "assistant", "content": to_instruction(headline_data) })
         # - chat history
         chat_history_data = self.request.request_runtime_ctx.get("prompt.chat_history")
         if chat_history_data:
             request_messages.extend(chat_history_data)
         # - request message (prompt)
         prompt_input_data = self.request.request_runtime_ctx.get("prompt.input")
-        prompt_information_data = self.request.request_runtime_ctx.get("prompt.information")
-        prompt_instruction_data = self.request.request_runtime_ctx.get("prompt.instruction")
+        prompt_info_data = self.request.request_runtime_ctx.get("prompt.info")
+        prompt_instruct_data = self.request.request_runtime_ctx.get("prompt.instruct")
         prompt_output_data = self.request.request_runtime_ctx.get("prompt.output")
         # --- only input
-        if not prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
-            raise Exception("[Request] Missing 'prompt.input', 'prompt.information', 'prompt.instruction', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
-        if prompt_input_data and not prompt_information_data and not prompt_instruction_data and not prompt_output_data:
+        if not prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
+            raise Exception("[Request] Missing 'prompt.input', 'prompt.info', 'prompt.instruct', 'prompt.output' in request_runtime_ctx. At least set value to one of them.")
+        if prompt_input_data and not prompt_info_data and not prompt_instruct_data and not prompt_output_data:
             request_messages.append({ "role": "user", "content": to_instruction(prompt_input_data) })
         # --- construct prompt
         else:
             prompt_dict = {}
             if prompt_input_data:
                 prompt_dict["[INPUT]"] = to_instruction(prompt_input_data)
-            if prompt_information_data:
-                prompt_dict["[HELPFUL INFORMATION]"] = to_instruction(prompt_information_data)
-            if prompt_instruction_data:
-                prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruction_data)
+            if prompt_info_data:
+                prompt_dict["[HELPFUL INFORMATION]"] = to_instruction(prompt_info_data)
+            if prompt_instruct_data:
+                prompt_dict["[INSTRUCTION]"] = to_instruction(prompt_instruct_data)
             if prompt_output_data:
                 if isinstance(prompt_output_data, (dict, list, set)):
                     prompt_dict["[OUTPUT REQUIREMENT]"] = {
                         "TYPE": "JSON can be parsed in Python",
                         "FORMAT": to_json_desc(prompt_output_data),
                     }
                     self.request.request_runtime_ctx.set("response:type", "JSON")
```

### Comparing `Agently-3.2.1.3/Agently/plugins/request/utils/transform.py` & `Agently-3.2.2.0a1/Agently/plugins/request/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/storage/FileStorage.py` & `Agently-3.2.2.0a1/Agently/plugins/storage/FileStorage.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/storage/__init__.py` & `Agently-3.2.2.0a1/Agently/plugins/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/storage/utils/StorageABC.py` & `Agently-3.2.2.0a1/Agently/plugins/storage/utils/StorageABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/tool/Code.py` & `Agently-3.2.2.0a1/Agently/plugins/tool/Code.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/tool/Web.py` & `Agently-3.2.2.0a1/Agently/plugins/tool/Web.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/plugins/tool/__init__.py` & `Agently-3.2.2.0a1/Agently/plugins/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/utils/AliasManager.py` & `Agently-3.2.2.0a1/Agently/utils/AliasManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/utils/DataOps.py` & `Agently-3.2.2.0a1/Agently/utils/DataOps.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/utils/PluginManager.py` & `Agently-3.2.2.0a1/Agently/utils/PluginManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/utils/RuntimeCtx.py` & `Agently-3.2.2.0a1/Agently/utils/RuntimeCtx.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/utils/StorageDelegate.py` & `Agently-3.2.2.0a1/Agently/utils/StorageDelegate.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/utils/ToolManager.py` & `Agently-3.2.2.0a1/Agently/utils/ToolManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/utils/check_version.py` & `Agently-3.2.2.0a1/Agently/utils/check_version.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/utils/load_json.py` & `Agently-3.2.2.0a1/Agently/utils/load_json.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently/utils/transform.py` & `Agently-3.2.2.0a1/Agently/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.3/Agently.egg-info/PKG-INFO` & `Agently-3.2.2.0a1/Agently.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.1.3
+Version: 3.2.2.0a1
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Agently-3.2.1.3/Agently.egg-info/SOURCES.txt` & `Agently-3.2.2.0a1/Agently.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,24 +23,31 @@
 Agently/Workflow/Workflow.py
 Agently/Workflow/__init__.py
 Agently/Workflow/executors/StartExecutor.py
 Agently/Workflow/executors/__init__.py
 Agently/Workflow/executors/install.py
 Agently/Workflow/lib/BreakingHub.py
 Agently/Workflow/lib/ChunkExecutorABC.py
+Agently/Workflow/lib/ChunkExecutorManager.py
 Agently/Workflow/lib/Store.py
 Agently/Workflow/lib/__init__.py
 Agently/Workflow/lib/constants.py
 Agently/Workflow/lib/painter.py
 Agently/Workflow/utils/__init__.py
 Agently/Workflow/utils/exec_tree.py
 Agently/Workflow/utils/find.py
 Agently/Workflow/utils/logger.py
 Agently/Workflow/utils/runtime_supports.py
 Agently/Workflow/utils/verify.py
+Agently/Workflow/yamlflow/__init__.py
+Agently/Workflow/yamlflow/yamlflow.py
+Agently/Workflow/yamlflow/preset_chunks/Print.py
+Agently/Workflow/yamlflow/preset_chunks/Start.py
+Agently/Workflow/yamlflow/preset_chunks/UserInput.py
+Agently/Workflow/yamlflow/preset_chunks/__init__.py
 Agently/plugins/__init__.py
 Agently/plugins/agent_component/Decorator.py
 Agently/plugins/agent_component/EventListener.py
 Agently/plugins/agent_component/OpenAIAssistant.py
 Agently/plugins/agent_component/ReplyReformer.py
 Agently/plugins/agent_component/Role.py
 Agently/plugins/agent_component/Search.py
```

### Comparing `Agently-3.2.1.3/PKG-INFO` & `Agently-3.2.2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.1.3
+Version: 3.2.2.0a1
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Agently-3.2.1.3/setup.py` & `Agently-3.2.2.0a1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 requirements = []
 for requirement in origin_requirements:
     if not requirement.startswith("#"):
         requirements.append(requirement)
 
 setuptools.setup(
     name = "Agently",
-    version = "3.2.1.3",
+    version = "3.2.2.0-alpha-1",
     author = "Maplemx",
     author_email = "maplemx@gmail.com",
     description = "Agently, a framework to build applications based on language model powered intelligent agents.",
     long_description = "https://github.com/Maplemx/Agently",
     url = "https://github.com/Maplemx/Agently",
     license='Apache License, Version 2.0',
     packages = setuptools.find_packages(),
```

