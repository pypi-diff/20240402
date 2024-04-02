# Comparing `tmp/Agently-3.2.1.2.tar.gz` & `tmp/Agently-3.2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Agently-3.2.1.2.tar", last modified: Wed Mar 27 00:20:00 2024, max compression
+gzip compressed data, was "Agently-3.2.1.3.tar", last modified: Wed Mar 27 01:22:26 2024, max compression
```

## Comparing `Agently-3.2.1.2.tar` & `Agently-3.2.1.3.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.538437 Agently-3.2.1.2/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.518226 Agently-3.2.1.2/Agently/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.519630 Agently-3.2.1.2/Agently/Agent/
--rw-r--r--   0 moxin      (501) staff       (20)    13552 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Agent/Agent.py
--rw-r--r--   0 moxin      (501) staff       (20)     2259 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Agent/AgentFactory.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Agent/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.521023 Agently-3.2.1.2/Agently/Facility/
--rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Facility/FacilityManager.py
--rw-r--r--   0 moxin      (501) staff       (20)       44 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Facility/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.521548 Agently-3.2.1.2/Agently/Request/
--rw-r--r--   0 moxin      (501) staff       (20)     9217 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Request/Request.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Request/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.521968 Agently-3.2.1.2/Agently/WebSocket/
--rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/WebSocket/WebSocket.py
--rw-r--r--   0 moxin      (501) staff       (20)       55 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/WebSocket/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.523381 Agently-3.2.1.2/Agently/Workflow/
--rw-r--r--   0 moxin      (501) staff       (20)     6927 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/Chunk.py
--rw-r--r--   0 moxin      (501) staff       (20)    10302 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/MainExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/Schema.py
--rw-r--r--   0 moxin      (501) staff       (20)     2236 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/Workflow.py
--rw-r--r--   0 moxin      (501) staff       (20)       57 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.523797 Agently-3.2.1.2/Agently/Workflow/executors/
--rw-r--r--   0 moxin      (501) staff       (20)       67 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/executors/StartExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/executors/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      245 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/executors/install.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.524797 Agently-3.2.1.2/Agently/Workflow/lib/
--rw-r--r--   0 moxin      (501) staff       (20)     1033 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/lib/BreakingHub.py
--rw-r--r--   0 moxin      (501) staff       (20)      656 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/lib/ChunkExecutorABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      483 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/lib/Store.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/lib/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/lib/constants.py
--rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/lib/painter.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.525718 Agently-3.2.1.2/Agently/Workflow/utils/
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     3527 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/utils/exec_tree.py
--rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/utils/find.py
--rw-r--r--   0 moxin      (501) staff       (20)      613 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/utils/logger.py
--rw-r--r--   0 moxin      (501) staff       (20)      892 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/utils/runtime_supports.py
--rw-r--r--   0 moxin      (501) staff       (20)      242 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/Workflow/utils/verify.py
--rw-r--r--   0 moxin      (501) staff       (20)      512 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/_global.py
--rw-r--r--   0 moxin      (501) staff       (20)      149 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/global_plugin_manager.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.525857 Agently-3.2.1.2/Agently/plugins/
--rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.528772 Agently-3.2.1.2/Agently/plugins/agent_component/
--rw-r--r--   0 moxin      (501) staff       (20)     2870 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/Decorator.py
--rw-r--r--   0 moxin      (501) staff       (20)     1384 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/EventListener.py
--rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/OpenAIAssistant.py
--rw-r--r--   0 moxin      (501) staff       (20)      785 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/ReplyReformer.py
--rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/Role.py
--rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/Search.py
--rw-r--r--   0 moxin      (501) staff       (20)     9782 2024-03-27 00:16:58.000000 Agently-3.2.1.2/Agently/plugins/agent_component/Segment.py
--rw-r--r--   0 moxin      (501) staff       (20)     8287 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/Session.py
--rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/Status.py
--rw-r--r--   0 moxin      (501) staff       (20)     8878 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/Tool.py
--rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/UserInfo.py
--rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      505 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.529111 Agently-3.2.1.2/Agently/plugins/agent_component/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      588 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/utils/ComponentABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/agent_component/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.529850 Agently-3.2.1.2/Agently/plugins/facility/
--rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/facility/Embedding.py
--rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/facility/RoleManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/facility/StatusManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/facility/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)       85 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/facility/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.530189 Agently-3.2.1.2/Agently/plugins/facility/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      266 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/facility/utils/FacilityABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       36 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/facility/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.532805 Agently-3.2.1.2/Agently/plugins/request/
--rw-r--r--   0 moxin      (501) staff       (20)     7405 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/request/Claude.py
--rw-r--r--   0 moxin      (501) staff       (20)    10385 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/request/ERNIE.py
--rw-r--r--   0 moxin      (501) staff       (20)     7440 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/request/Google.py
--rw-r--r--   0 moxin      (501) staff       (20)     7851 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/request/Kimi.py
--rw-r--r--   0 moxin      (501) staff       (20)    12342 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/request/MiniMax.py
--rw-r--r--   0 moxin      (501) staff       (20)    14730 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/request/OAIClient.py
--rw-r--r--   0 moxin      (501) staff       (20)    11607 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/request/OpenAI.py
--rw-r--r--   0 moxin      (501) staff       (20)    12788 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/request/ZhipuAI.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/request/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      139 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/request/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.533369 Agently-3.2.1.2/Agently/plugins/request/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     5387 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/request/utils/RequestABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      118 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/request/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     4326 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/request/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.533923 Agently-3.2.1.2/Agently/plugins/storage/
--rw-r--r--   0 moxin      (501) staff       (20)     3160 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/storage/FileStorage.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/storage/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      131 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/storage/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.534188 Agently-3.2.1.2/Agently/plugins/storage/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      745 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/storage/utils/StorageABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       34 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/storage/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.534878 Agently-3.2.1.2/Agently/plugins/tool/
--rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/tool/Code.py
--rw-r--r--   0 moxin      (501) staff       (20)     6912 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/tool/Web.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/tool/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      104 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/tool/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.535127 Agently-3.2.1.2/Agently/plugins/tool/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      443 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/tool/utils/ToolABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/plugins/tool/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      168 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/requirements.txt
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.537774 Agently-3.2.1.2/Agently/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/utils/AliasManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/utils/DataOps.py
--rw-r--r--   0 moxin      (501) staff       (20)      323 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/utils/IdGenerator.py
--rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/utils/PluginManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/utils/RuntimeCtx.py
--rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/utils/StorageDelegate.py
--rw-r--r--   0 moxin      (501) staff       (20)     4758 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/utils/ToolManager.py
--rw-r--r--   0 moxin      (501) staff       (20)      491 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/utils/check_version.py
--rw-r--r--   0 moxin      (501) staff       (20)     2773 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/utils/load_json.py
--rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-03-26 06:44:32.000000 Agently-3.2.1.2/Agently/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 00:20:00.538037 Agently-3.2.1.2/Agently.egg-info/
--rw-r--r--   0 moxin      (501) staff       (20)      819 2024-03-27 00:20:00.000000 Agently-3.2.1.2/Agently.egg-info/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)     3375 2024-03-27 00:20:00.000000 Agently-3.2.1.2/Agently.egg-info/SOURCES.txt
--rw-r--r--   0 moxin      (501) staff       (20)        1 2024-03-27 00:20:00.000000 Agently-3.2.1.2/Agently.egg-info/dependency_links.txt
--rw-r--r--   0 moxin      (501) staff       (20)      118 2024-03-27 00:20:00.000000 Agently-3.2.1.2/Agently.egg-info/requires.txt
--rw-r--r--   0 moxin      (501) staff       (20)        8 2024-03-27 00:20:00.000000 Agently-3.2.1.2/Agently.egg-info/top_level.txt
--rw-r--r--   0 moxin      (501) staff       (20)      819 2024-03-27 00:20:00.538254 Agently-3.2.1.2/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-03-27 00:20:00.538471 Agently-3.2.1.2/setup.cfg
--rw-------   0 moxin      (501) staff       (20)      974 2024-03-27 00:17:10.000000 Agently-3.2.1.2/setup.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.586857 Agently-3.2.1.3/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.561499 Agently-3.2.1.3/Agently/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.562696 Agently-3.2.1.3/Agently/Agent/
+-rw-r--r--   0 moxin      (501) staff       (20)    13552 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Agent/Agent.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2259 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Agent/AgentFactory.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Agent/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.563055 Agently-3.2.1.3/Agently/Facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Facility/FacilityManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)       44 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Facility/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.563945 Agently-3.2.1.3/Agently/Request/
+-rw-r--r--   0 moxin      (501) staff       (20)     9217 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Request/Request.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Request/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.564375 Agently-3.2.1.3/Agently/WebSocket/
+-rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/WebSocket/WebSocket.py
+-rw-r--r--   0 moxin      (501) staff       (20)       55 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/WebSocket/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.565529 Agently-3.2.1.3/Agently/Workflow/
+-rw-r--r--   0 moxin      (501) staff       (20)     6927 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/Chunk.py
+-rw-r--r--   0 moxin      (501) staff       (20)    10302 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/MainExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/Schema.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2236 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/Workflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)       57 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.565939 Agently-3.2.1.3/Agently/Workflow/executors/
+-rw-r--r--   0 moxin      (501) staff       (20)       67 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/executors/StartExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/executors/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      245 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/executors/install.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.567943 Agently-3.2.1.3/Agently/Workflow/lib/
+-rw-r--r--   0 moxin      (501) staff       (20)     1033 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/lib/BreakingHub.py
+-rw-r--r--   0 moxin      (501) staff       (20)      656 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/lib/ChunkExecutorABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      483 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/lib/Store.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/lib/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/lib/constants.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/lib/painter.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.569926 Agently-3.2.1.3/Agently/Workflow/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3527 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/utils/exec_tree.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/utils/find.py
+-rw-r--r--   0 moxin      (501) staff       (20)      613 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/utils/logger.py
+-rw-r--r--   0 moxin      (501) staff       (20)      892 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/utils/runtime_supports.py
+-rw-r--r--   0 moxin      (501) staff       (20)      242 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/Workflow/utils/verify.py
+-rw-r--r--   0 moxin      (501) staff       (20)      512 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/_global.py
+-rw-r--r--   0 moxin      (501) staff       (20)      149 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/global_plugin_manager.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.570048 Agently-3.2.1.3/Agently/plugins/
+-rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.573738 Agently-3.2.1.3/Agently/plugins/agent_component/
+-rw-r--r--   0 moxin      (501) staff       (20)     2870 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Decorator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1384 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/EventListener.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/OpenAIAssistant.py
+-rw-r--r--   0 moxin      (501) staff       (20)      785 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/ReplyReformer.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Role.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Search.py
+-rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Segment.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8287 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Session.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Status.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8878 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/Tool.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/UserInfo.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      505 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.574091 Agently-3.2.1.3/Agently/plugins/agent_component/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      588 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/utils/ComponentABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/agent_component/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.575698 Agently-3.2.1.3/Agently/plugins/facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/Embedding.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/RoleManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/StatusManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)       85 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.576844 Agently-3.2.1.3/Agently/plugins/facility/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      266 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/utils/FacilityABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       36 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/facility/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.579774 Agently-3.2.1.3/Agently/plugins/request/
+-rw-r--r--   0 moxin      (501) staff       (20)     7405 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/Claude.py
+-rw-r--r--   0 moxin      (501) staff       (20)    10385 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/ERNIE.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7440 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/Google.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7851 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/Kimi.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12342 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/MiniMax.py
+-rw-r--r--   0 moxin      (501) staff       (20)    15538 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/OAIClient.py
+-rw-r--r--   0 moxin      (501) staff       (20)    11607 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/OpenAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12788 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/ZhipuAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      139 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.581066 Agently-3.2.1.3/Agently/plugins/request/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     5387 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/utils/RequestABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      118 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4330 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/request/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.581740 Agently-3.2.1.3/Agently/plugins/storage/
+-rw-r--r--   0 moxin      (501) staff       (20)     3160 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/storage/FileStorage.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/storage/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      131 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/storage/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.581986 Agently-3.2.1.3/Agently/plugins/storage/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      745 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/storage/utils/StorageABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       34 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/storage/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.582846 Agently-3.2.1.3/Agently/plugins/tool/
+-rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/tool/Code.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6912 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/tool/Web.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/tool/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      104 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/tool/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.583204 Agently-3.2.1.3/Agently/plugins/tool/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      443 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/tool/utils/ToolABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/plugins/tool/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      168 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/requirements.txt
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.586193 Agently-3.2.1.3/Agently/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/AliasManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/DataOps.py
+-rw-r--r--   0 moxin      (501) staff       (20)      323 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/IdGenerator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/PluginManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/RuntimeCtx.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/StorageDelegate.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4758 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/ToolManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      491 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/check_version.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2773 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/load_json.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-03-27 01:16:18.000000 Agently-3.2.1.3/Agently/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-03-27 01:22:26.586493 Agently-3.2.1.3/Agently.egg-info/
+-rw-r--r--   0 moxin      (501) staff       (20)      819 2024-03-27 01:22:26.000000 Agently-3.2.1.3/Agently.egg-info/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)     3375 2024-03-27 01:22:26.000000 Agently-3.2.1.3/Agently.egg-info/SOURCES.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        1 2024-03-27 01:22:26.000000 Agently-3.2.1.3/Agently.egg-info/dependency_links.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      118 2024-03-27 01:22:26.000000 Agently-3.2.1.3/Agently.egg-info/requires.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        8 2024-03-27 01:22:26.000000 Agently-3.2.1.3/Agently.egg-info/top_level.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      819 2024-03-27 01:22:26.586684 Agently-3.2.1.3/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-03-27 01:22:26.586896 Agently-3.2.1.3/setup.cfg
+-rw-------   0 moxin      (501) staff       (20)      974 2024-03-27 01:22:19.000000 Agently-3.2.1.3/setup.py
```

### Comparing `Agently-3.2.1.2/Agently/Agent/Agent.py` & `Agently-3.2.1.3/Agently/Agent/Agent.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Agent/AgentFactory.py` & `Agently-3.2.1.3/Agently/Agent/AgentFactory.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Facility/FacilityManager.py` & `Agently-3.2.1.3/Agently/Facility/FacilityManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Request/Request.py` & `Agently-3.2.1.3/Agently/Request/Request.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/WebSocket/WebSocket.py` & `Agently-3.2.1.3/Agently/WebSocket/WebSocket.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Workflow/Chunk.py` & `Agently-3.2.1.3/Agently/Workflow/Chunk.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Workflow/MainExecutor.py` & `Agently-3.2.1.3/Agently/Workflow/MainExecutor.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Workflow/Schema.py` & `Agently-3.2.1.3/Agently/Workflow/Schema.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Workflow/Workflow.py` & `Agently-3.2.1.3/Agently/Workflow/Workflow.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Workflow/lib/BreakingHub.py` & `Agently-3.2.1.3/Agently/Workflow/lib/BreakingHub.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Workflow/lib/ChunkExecutorABC.py` & `Agently-3.2.1.3/Agently/Workflow/lib/ChunkExecutorABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Workflow/lib/constants.py` & `Agently-3.2.1.3/Agently/Workflow/lib/constants.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Workflow/lib/painter.py` & `Agently-3.2.1.3/Agently/Workflow/lib/painter.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Workflow/utils/exec_tree.py` & `Agently-3.2.1.3/Agently/Workflow/utils/exec_tree.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Workflow/utils/find.py` & `Agently-3.2.1.3/Agently/Workflow/utils/find.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Workflow/utils/logger.py` & `Agently-3.2.1.3/Agently/Workflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/Workflow/utils/runtime_supports.py` & `Agently-3.2.1.3/Agently/Workflow/utils/runtime_supports.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/__init__.py` & `Agently-3.2.1.3/Agently/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/_global.py` & `Agently-3.2.1.3/Agently/_global.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/__init__.py` & `Agently-3.2.1.3/Agently/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/agent_component/Decorator.py` & `Agently-3.2.1.3/Agently/plugins/agent_component/Decorator.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/agent_component/EventListener.py` & `Agently-3.2.1.3/Agently/plugins/agent_component/EventListener.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/agent_component/OpenAIAssistant.py` & `Agently-3.2.1.3/Agently/plugins/agent_component/OpenAIAssistant.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/agent_component/ReplyReformer.py` & `Agently-3.2.1.3/Agently/plugins/agent_component/ReplyReformer.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/agent_component/Role.py` & `Agently-3.2.1.3/Agently/plugins/agent_component/Role.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/agent_component/Search.py` & `Agently-3.2.1.3/Agently/plugins/agent_component/Search.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/agent_component/Segment.py` & `Agently-3.2.1.3/Agently/plugins/agent_component/Segment.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -188,8 +188,8 @@
                 "add_segment_listener": { "func": self.add_segment_listener },
                 "on_segment_delta": { "func": self.on_segment_delta },
                 "on_segment_done": { "func": self.on_segment_done },
             },
         }
 
 def export():
-    return ("Segment", Segment)
+    return ("Segment", Segment)
```

### Comparing `Agently-3.2.1.2/Agently/plugins/agent_component/Session.py` & `Agently-3.2.1.3/Agently/plugins/agent_component/Session.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/agent_component/Status.py` & `Agently-3.2.1.3/Agently/plugins/agent_component/Status.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/agent_component/Tool.py` & `Agently-3.2.1.3/Agently/plugins/agent_component/Tool.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/agent_component/UserInfo.py` & `Agently-3.2.1.3/Agently/plugins/agent_component/UserInfo.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/agent_component/__init__.py` & `Agently-3.2.1.3/Agently/plugins/agent_component/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/agent_component/utils/ComponentABC.py` & `Agently-3.2.1.3/Agently/plugins/agent_component/utils/ComponentABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/facility/Embedding.py` & `Agently-3.2.1.3/Agently/plugins/facility/Embedding.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/facility/RoleManager.py` & `Agently-3.2.1.3/Agently/plugins/facility/RoleManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/facility/StatusManager.py` & `Agently-3.2.1.3/Agently/plugins/facility/StatusManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/facility/__init__.py` & `Agently-3.2.1.3/Agently/plugins/facility/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/request/Claude.py` & `Agently-3.2.1.3/Agently/plugins/request/Claude.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/request/ERNIE.py` & `Agently-3.2.1.3/Agently/plugins/request/ERNIE.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/request/Google.py` & `Agently-3.2.1.3/Agently/plugins/request/Google.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/request/Kimi.py` & `Agently-3.2.1.3/Agently/plugins/request/Kimi.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/request/MiniMax.py` & `Agently-3.2.1.3/Agently/plugins/request/MiniMax.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/request/OAIClient.py` & `Agently-3.2.1.3/Agently/plugins/request/OAIClient.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,20 @@
         self.request = request
         self.model_name = "OAIClient"
         self.model_settings = RuntimeCtxNamespace(f"model.{ self.model_name }", self.request.settings)
         self.request_type = self.request.request_runtime_ctx.get("request_type", "chat")
         self.default_options = {
             "stream": True
         }
-        self.message_rules = {
-            "no_multi_system_messages": True, # Will combine multi system messages into one message
-            "strict_orders": True, # Will arrange message in orders like "user-assisantant-user-assisntant-..."
-        }
+        if not self.model_settings.get_trace_back("message_rules.no_multi_system_messages"):
+            self.model_settings.set("message_rules.no_multi_system_messages", True)
+        if not self.model_settings.get_trace_back("message_rules.strict_orders"):
+            self.model_settings.set("message_rules.strict_orders", True)
+        if not self.model_settings.get_trace_back("message_rules.no_multi_type_messages"):
+            self.model_settings.set("message_rules.no_multi_type_messages", True)    
 
     def construct_request_messages(self):
         #init request messages
         request_messages = []
         # - general instruction
         general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general_instruction")
         if general_instruction_data:
@@ -79,39 +81,47 @@
         system_messages = []
         chat_messages = []
         role_list = ["user", "assistant"]
         current_role = 0
         for message in request_messages:
             if message["role"] == "system":
                 # no_multi_system_messages=True
-                if self.message_rules["no_multi_system_messages"]:
+                if self.model_settings.get_trace_back("message_rules.no_multi_system_messages"):
                     system_prompt += f"{ message['content'] }\n"
                 # no_multi_system_messages=False
                 else:
                     system_messages.append(message)
             else:
                 # strict_orders=True
-                if self.message_rules["strict_orders"]:
+                if self.model_settings.get_trace_back("message_rules.strict_orders"):
                     if len(chat_messages) == 0 and message["role"] != "user":
                         chat_messages.append({ "role": "user", "content": "What did we talked about?" })
                         current_role = not current_role
                     if message["role"] == role_list[current_role]:
                         chat_messages.append(message)
                         current_role = not current_role
                     else:
                         content = f"{ chat_messages[-1]['content'] }\n{ message['content'] }"
                         chat_messages[-1]['content'] = content
                 # strict_orders=False
                 else:
                     chat_messages.append(message)
         # no_multi_system_messages=True
-        if self.message_rules["no_multi_system_messages"] and system_prompt != "":
+        if self.model_settings.get_trace_back("message_rules.no_multi_system_messages") and system_prompt != "":
             system_messages.append({ "role": "system", "content": system_prompt })
         formatted_messages = system_messages.copy()
         formatted_messages.extend(chat_messages)
+        # no_multi_type_messages=True
+        if self.model_settings.get_trace_back("message_rules.no_multi_type_messages"):
+            current_messages = formatted_messages.copy()
+            formatted_messages = []
+            for message in current_messages:
+                for item in message["content"]:
+                    if item["type"] == "text":
+                        formatted_messages.append({ "role": message["role"], "content": item["text"] })
         return formatted_messages
 
     def construct_completion_prompt(self):
         # - init prompt
         completion_prompt = ""
         # - general instruction
         general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general_instruction")
```

### Comparing `Agently-3.2.1.2/Agently/plugins/request/OpenAI.py` & `Agently-3.2.1.3/Agently/plugins/request/OpenAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/request/ZhipuAI.py` & `Agently-3.2.1.3/Agently/plugins/request/ZhipuAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/request/__init__.py` & `Agently-3.2.1.3/Agently/plugins/request/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/request/utils/RequestABC.py` & `Agently-3.2.1.3/Agently/plugins/request/utils/RequestABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/request/utils/transform.py` & `Agently-3.2.1.3/Agently/utils/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,16 +99,16 @@
                         continue
                 if char == "\"":
                     in_quote = True
                 if char == "[" or char == "{":
                     layer += 1
                 elif char == "]" or char == "}":
                     layer -= 1
-                elif char in ("\t", " ", "\n"):
-                    char = ""
+                #elif char in ("\t", " ", "\n"):
+                    #char = ""
                 json_blocks[block_num] += char
             else:
                 if char == "\\":
                     char += origin[index + 1]
                     skip_next = True
                 elif char == "\n":
                     char = "\\n"
```

### Comparing `Agently-3.2.1.2/Agently/plugins/storage/FileStorage.py` & `Agently-3.2.1.3/Agently/plugins/storage/FileStorage.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/storage/__init__.py` & `Agently-3.2.1.3/Agently/plugins/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/storage/utils/StorageABC.py` & `Agently-3.2.1.3/Agently/plugins/storage/utils/StorageABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/tool/Code.py` & `Agently-3.2.1.3/Agently/plugins/tool/Code.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/tool/Web.py` & `Agently-3.2.1.3/Agently/plugins/tool/Web.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/plugins/tool/__init__.py` & `Agently-3.2.1.3/Agently/plugins/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/utils/AliasManager.py` & `Agently-3.2.1.3/Agently/utils/AliasManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/utils/DataOps.py` & `Agently-3.2.1.3/Agently/utils/DataOps.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/utils/PluginManager.py` & `Agently-3.2.1.3/Agently/utils/PluginManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/utils/RuntimeCtx.py` & `Agently-3.2.1.3/Agently/utils/RuntimeCtx.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/utils/StorageDelegate.py` & `Agently-3.2.1.3/Agently/utils/StorageDelegate.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/utils/ToolManager.py` & `Agently-3.2.1.3/Agently/utils/ToolManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/utils/check_version.py` & `Agently-3.2.1.3/Agently/utils/check_version.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/utils/load_json.py` & `Agently-3.2.1.3/Agently/utils/load_json.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/Agently/utils/transform.py` & `Agently-3.2.1.3/Agently/plugins/request/utils/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     elif isinstance(origin, (list, set)):
         json_string = ""
         if layer_count > 0:
             json_string += "\n"
         json_string += ("\t" * layer_count) + "[\n"
         for item in origin:
             json_string += ("\t" * (layer_count + 1)) + to_json_desc(item, layer_count + 1) + ",\n"
-        json_string += ("\t" * (layer_count + 1)) + "...\n"
+        json_string += ("\t" * (layer_count + 1)) + "\\\\...\n"
         if layer_count > 0:
             json_string += ("\t" * layer_count) + "],"
         else:
             json_string += "]"
         return json_string
     elif isinstance(origin, tuple):
         if isinstance(origin[0], (dict, list, set)):
@@ -99,16 +99,16 @@
                         continue
                 if char == "\"":
                     in_quote = True
                 if char == "[" or char == "{":
                     layer += 1
                 elif char == "]" or char == "}":
                     layer -= 1
-                #elif char in ("\t", " ", "\n"):
-                    #char = ""
+                elif char in ("\t", " ", "\n"):
+                    char = ""
                 json_blocks[block_num] += char
             else:
                 if char == "\\":
                     char += origin[index + 1]
                     skip_next = True
                 elif char == "\n":
                     char = "\\n"
```

### Comparing `Agently-3.2.1.2/Agently.egg-info/PKG-INFO` & `Agently-3.2.1.3/Agently.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.1.2
+Version: 3.2.1.3
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Agently-3.2.1.2/Agently.egg-info/SOURCES.txt` & `Agently-3.2.1.3/Agently.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Agently-3.2.1.2/PKG-INFO` & `Agently-3.2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.1.2
+Version: 3.2.1.3
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Agently-3.2.1.2/setup.py` & `Agently-3.2.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 requirements = []
 for requirement in origin_requirements:
     if not requirement.startswith("#"):
         requirements.append(requirement)
 
 setuptools.setup(
     name = "Agently",
-    version = "3.2.1.2",
+    version = "3.2.1.3",
     author = "Maplemx",
     author_email = "maplemx@gmail.com",
     description = "Agently, a framework to build applications based on language model powered intelligent agents.",
     long_description = "https://github.com/Maplemx/Agently",
     url = "https://github.com/Maplemx/Agently",
     license='Apache License, Version 2.0',
     packages = setuptools.find_packages(),
```

