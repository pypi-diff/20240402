# Comparing `tmp/agentforge-0.2.8.tar.gz` & `tmp/agentforge-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentforge-0.2.8.tar", last modified: Sat Mar  9 22:06:06 2024, max compression
+gzip compressed data, was "agentforge-0.2.9.tar", last modified: Fri Mar 22 22:14:16 2024, max compression
```

## Comparing `agentforge-0.2.8.tar` & `agentforge-0.2.9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.639119 agentforge-0.2.8/
--rw-rw-rw-   0        0        0    35149 2023-11-05 01:11:53.000000 agentforge-0.2.8/LICENSE
--rw-rw-rw-   0        0        0      246 2023-11-05 01:11:53.000000 agentforge-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6327 2024-03-09 22:06:06.638118 agentforge-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     5556 2024-03-07 17:45:26.000000 agentforge-0.2.8/README.md
--rw-rw-rw-   0        0        0       42 2024-03-09 22:06:06.639119 agentforge-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     2357 2024-03-09 20:42:15.000000 agentforge-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.249118 agentforge-0.2.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.304190 agentforge-0.2.8/src/agentforge/
--rw-rw-rw-   0        0        0        0 2023-11-05 01:11:53.000000 agentforge-0.2.8/src/agentforge/__init__.py
--rw-rw-rw-   0        0        0     6173 2024-03-01 01:43:06.000000 agentforge-0.2.8/src/agentforge/agent.py
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.360173 agentforge-0.2.8/src/agentforge/agents/
--rw-rw-rw-   0        0        0     1272 2024-02-22 23:07:46.000000 agentforge-0.2.8/src/agentforge/agents/ActionPrimingAgent.py
--rw-rw-rw-   0        0        0     6205 2024-02-25 19:07:28.000000 agentforge-0.2.8/src/agentforge/agents/ActionSelectionAgent.py
--rw-rw-rw-   0        0        0     1021 2024-02-22 23:07:46.000000 agentforge-0.2.8/src/agentforge/agents/LearnKGAgent.py
--rw-rw-rw-   0        0        0     1024 2024-03-01 01:43:40.000000 agentforge-0.2.8/src/agentforge/agents/MetadataKGAgent.py
--rw-rw-rw-   0        0        0        0 2023-11-05 01:11:53.000000 agentforge-0.2.8/src/agentforge/agents/__init__.py
--rw-rw-rw-   0        0        0     9226 2024-02-28 12:43:58.000000 agentforge-0.2.8/src/agentforge/config.py
--rw-rw-rw-   0        0        0     3994 2024-03-08 22:49:07.000000 agentforge-0.2.8/src/agentforge/init_agentforge.py
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.419119 agentforge-0.2.8/src/agentforge/llm/
--rw-rw-rw-   0        0        0      111 2023-11-05 01:11:53.000000 agentforge-0.2.8/src/agentforge/llm/__init__.py
--rw-rw-rw-   0        0        0     3884 2024-03-08 01:12:50.000000 agentforge-0.2.8/src/agentforge/llm/anthropic.py
--rw-rw-rw-   0        0        0     3512 2024-03-07 18:45:00.000000 agentforge-0.2.8/src/agentforge/llm/claude_old.py
--rw-rw-rw-   0        0        0     1968 2024-02-22 23:07:46.000000 agentforge-0.2.8/src/agentforge/llm/customapi.py
--rw-rw-rw-   0        0        0     3484 2024-02-22 23:07:46.000000 agentforge-0.2.8/src/agentforge/llm/gemini.py
--rw-rw-rw-   0        0        0     4945 2024-02-22 23:07:46.000000 agentforge-0.2.8/src/agentforge/llm/oobabooga.py
--rw-rw-rw-   0        0        0     4032 2024-02-22 23:07:46.000000 agentforge-0.2.8/src/agentforge/llm/openai.py
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.451118 agentforge-0.2.8/src/agentforge/modules/
--rw-rw-rw-   0        0        0     9460 2024-02-25 19:07:28.000000 agentforge-0.2.8/src/agentforge/modules/ActionExecution.py
--rw-rw-rw-   0        0        0     3014 2024-03-07 17:45:26.000000 agentforge-0.2.8/src/agentforge/modules/InjectKG.py
--rw-rw-rw-   0        0        0     6396 2024-03-07 17:45:26.000000 agentforge-0.2.8/src/agentforge/modules/KnowledgeTraversal.py
--rw-rw-rw-   0        0        0     5048 2024-03-07 17:45:27.000000 agentforge-0.2.8/src/agentforge/modules/LearnDoc.py
--rw-rw-rw-   0        0        0        0 2023-11-05 01:11:53.000000 agentforge-0.2.8/src/agentforge/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.453118 agentforge-0.2.8/src/agentforge/setup_files/
--rw-rw-rw-   0        0        0        0 2024-02-25 19:07:27.000000 agentforge-0.2.8/src/agentforge/setup_files/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.457118 agentforge-0.2.8/src/agentforge/setup_files/actions/
--rw-rw-rw-   0        0        0      593 2024-02-25 19:07:27.000000 agentforge-0.2.8/src/agentforge/setup_files/actions/WebSearch.yaml
--rw-rw-rw-   0        0        0      871 2024-02-25 19:07:27.000000 agentforge-0.2.8/src/agentforge/setup_files/actions/WriteFile.yaml
--rw-rw-rw-   0        0        0        0 2024-03-08 20:43:54.000000 agentforge-0.2.8/src/agentforge/setup_files/actions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.459143 agentforge-0.2.8/src/agentforge/setup_files/agents/
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.467120 agentforge-0.2.8/src/agentforge/setup_files/agents/ModuleAgents/
--rw-rw-rw-   0        0        0     1314 2024-02-25 19:07:27.000000 agentforge-0.2.8/src/agentforge/setup_files/agents/ModuleAgents/ActionPrimingAgent.yaml
--rw-rw-rw-   0        0        0     1394 2024-02-25 19:07:27.000000 agentforge-0.2.8/src/agentforge/setup_files/agents/ModuleAgents/ActionSelectionAgent.yaml
--rw-rw-rw-   0        0        0     2241 2024-03-07 17:45:26.000000 agentforge-0.2.8/src/agentforge/setup_files/agents/ModuleAgents/LearnKGAgent.yaml
--rw-rw-rw-   0        0        0     1865 2024-03-07 17:45:26.000000 agentforge-0.2.8/src/agentforge/setup_files/agents/ModuleAgents/MetadataKGAgent.yaml
--rw-rw-rw-   0        0        0        0 2024-03-08 22:49:07.000000 agentforge-0.2.8/src/agentforge/setup_files/agents/ModuleAgents/__init__.py
--rw-rw-rw-   0        0        0        0 2024-03-08 20:43:54.000000 agentforge-0.2.8/src/agentforge/setup_files/agents/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.471118 agentforge-0.2.8/src/agentforge/setup_files/personas/
--rw-rw-rw-   0        0        0        0 2024-03-08 20:43:54.000000 agentforge-0.2.8/src/agentforge/setup_files/personas/__init__.py
--rw-rw-rw-   0        0        0     3133 2024-03-04 17:34:34.000000 agentforge-0.2.8/src/agentforge/setup_files/personas/default.yaml
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.479128 agentforge-0.2.8/src/agentforge/setup_files/settings/
--rw-rw-rw-   0        0        0        0 2024-03-08 20:43:54.000000 agentforge-0.2.8/src/agentforge/setup_files/settings/__init__.py
--rw-rw-rw-   0        0        0     1939 2024-03-08 01:11:23.000000 agentforge-0.2.8/src/agentforge/setup_files/settings/models.yaml
--rw-rw-rw-   0        0        0      285 2024-03-01 03:03:24.000000 agentforge-0.2.8/src/agentforge/setup_files/settings/storage.yaml
--rw-rw-rw-   0        0        0      221 2024-03-08 01:14:02.000000 agentforge-0.2.8/src/agentforge/setup_files/settings/system.yaml
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.491119 agentforge-0.2.8/src/agentforge/setup_files/tools/
--rw-rw-rw-   0        0        0      647 2024-02-25 19:07:27.000000 agentforge-0.2.8/src/agentforge/setup_files/tools/FileWriter.yaml
--rw-rw-rw-   0        0        0      747 2024-02-25 19:07:27.000000 agentforge-0.2.8/src/agentforge/setup_files/tools/GoogleSearch.yaml
--rw-rw-rw-   0        0        0      739 2024-02-25 19:07:27.000000 agentforge-0.2.8/src/agentforge/setup_files/tools/IntelligentChunk.yaml
--rw-rw-rw-   0        0        0     1380 2024-02-25 19:07:27.000000 agentforge-0.2.8/src/agentforge/setup_files/tools/ReadDirectory.yaml
--rw-rw-rw-   0        0        0      482 2024-02-25 19:07:27.000000 agentforge-0.2.8/src/agentforge/setup_files/tools/ReadFile.yaml
--rw-rw-rw-   0        0        0      641 2024-02-25 19:07:27.000000 agentforge-0.2.8/src/agentforge/setup_files/tools/WebScrape.yaml
--rw-rw-rw-   0        0        0        0 2024-03-08 20:43:54.000000 agentforge-0.2.8/src/agentforge/setup_files/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.559119 agentforge-0.2.8/src/agentforge/tools/
--rw-rw-rw-   0        0        0      840 2024-03-01 02:15:14.000000 agentforge-0.2.8/src/agentforge/tools/CleanString.py
--rw-rw-rw-   0        0        0     1531 2023-11-05 01:11:53.000000 agentforge-0.2.8/src/agentforge/tools/CommandExecutor.py
--rw-rw-rw-   0        0        0     4041 2024-02-25 19:04:33.000000 agentforge-0.2.8/src/agentforge/tools/Directory.py
--rw-rw-rw-   0        0        0     1630 2024-02-22 23:07:46.000000 agentforge-0.2.8/src/agentforge/tools/GetText.py
--rw-rw-rw-   0        0        0     1853 2023-11-05 01:11:53.000000 agentforge-0.2.8/src/agentforge/tools/GoogleSearch.py
--rw-rw-rw-   0        0        0     1456 2024-03-01 02:26:55.000000 agentforge-0.2.8/src/agentforge/tools/IntelligentChunk.py
--rw-rw-rw-   0        0        0     8938 2024-03-01 01:43:40.000000 agentforge-0.2.8/src/agentforge/tools/TripleExtract.py
--rw-rw-rw-   0        0        0     2158 2023-11-05 01:11:53.000000 agentforge-0.2.8/src/agentforge/tools/UserInput.py
--rw-rw-rw-   0        0        0     1208 2024-02-25 19:04:33.000000 agentforge-0.2.8/src/agentforge/tools/WebScrape.py
--rw-rw-rw-   0        0        0     1839 2023-11-05 01:11:53.000000 agentforge-0.2.8/src/agentforge/tools/WriteFile.py
--rw-rw-rw-   0        0        0        0 2023-11-05 01:11:53.000000 agentforge-0.2.8/src/agentforge/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.582119 agentforge-0.2.8/src/agentforge/utils/
--rw-rw-rw-   0        0        0        0 2023-11-05 01:11:53.000000 agentforge-0.2.8/src/agentforge/utils/__init__.py
--rw-rw-rw-   0        0        0    17118 2024-03-01 01:43:06.000000 agentforge-0.2.8/src/agentforge/utils/chroma_utils.py
--rw-rw-rw-   0        0        0     1911 2024-02-22 23:07:46.000000 agentforge-0.2.8/src/agentforge/utils/function_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.624124 agentforge-0.2.8/src/agentforge/utils/functions/
--rw-rw-rw-   0        0        0     6381 2024-02-22 23:07:46.000000 agentforge-0.2.8/src/agentforge/utils/functions/AgentUtils.py
--rw-rw-rw-   0        0        0    12984 2024-03-04 17:34:34.000000 agentforge-0.2.8/src/agentforge/utils/functions/Logger.py
--rw-rw-rw-   0        0        0     3792 2024-02-22 23:07:46.000000 agentforge-0.2.8/src/agentforge/utils/functions/PromptHandling.py
--rw-rw-rw-   0        0        0     4596 2024-02-22 23:07:46.000000 agentforge-0.2.8/src/agentforge/utils/functions/ToolUtils.py
--rw-rw-rw-   0        0        0     3666 2024-03-01 01:43:06.000000 agentforge-0.2.8/src/agentforge/utils/functions/UserInterface.py
--rw-rw-rw-   0        0        0        0 2023-11-05 01:11:53.000000 agentforge-0.2.8/src/agentforge/utils/functions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.256118 agentforge-0.2.8/src/agentforge/utils/guiutils/
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.631120 agentforge-0.2.8/src/agentforge/utils/guiutils/__pycache__/
--rw-rw-rw-   0        0        0      167 2023-11-05 01:25:48.000000 agentforge-0.2.8/src/agentforge/utils/guiutils/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1894 2023-11-05 01:25:48.000000 agentforge-0.2.8/src/agentforge/utils/guiutils/__pycache__/listenforui.cpython-311.pyc
--rw-rw-rw-   0        0        0     1847 2023-11-15 20:19:25.000000 agentforge-0.2.8/src/agentforge/utils/guiutils/__pycache__/sendtoui.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.257119 agentforge-0.2.8/src/agentforge/utils/installer/
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.635118 agentforge-0.2.8/src/agentforge/utils/installer/__pycache__/
--rw-rw-rw-   0        0        0      168 2023-11-05 03:47:12.000000 agentforge-0.2.8/src/agentforge/utils/installer/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     6875 2023-12-08 19:16:40.000000 agentforge-0.2.8/src/agentforge/utils/installer/__pycache__/agentforge_cli.cpython-311.pyc
--rw-rw-rw-   0        0        0     1373 2023-11-26 23:09:06.000000 agentforge-0.2.8/src/agentforge/utils/pinecone_utils.py
--rw-rw-rw-   0        0        0     3573 2024-02-28 12:43:58.000000 agentforge-0.2.8/src/agentforge/utils/storage_interface.py
-drwxrwxrwx   0        0        0        0 2024-03-09 22:06:06.334119 agentforge-0.2.8/src/agentforge.egg-info/
--rw-rw-rw-   0        0        0     6327 2024-03-09 22:06:06.000000 agentforge-0.2.8/src/agentforge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3354 2024-03-09 22:06:06.000000 agentforge-0.2.8/src/agentforge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 22:06:06.000000 agentforge-0.2.8/src/agentforge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      457 2024-03-09 22:06:06.000000 agentforge-0.2.8/src/agentforge.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-09 22:06:06.000000 agentforge-0.2.8/src/agentforge.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.772834 agentforge-0.2.9/
+-rw-rw-rw-   0        0        0    35149 2023-11-05 01:11:53.000000 agentforge-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      246 2023-11-05 01:11:53.000000 agentforge-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6327 2024-03-22 22:14:16.772834 agentforge-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5556 2024-03-07 17:45:26.000000 agentforge-0.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-22 22:14:16.773841 agentforge-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     2357 2024-03-22 22:13:07.000000 agentforge-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.118997 agentforge-0.2.9/src/
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.168998 agentforge-0.2.9/src/agentforge/
+-rw-rw-rw-   0        0        0        0 2023-11-05 01:11:53.000000 agentforge-0.2.9/src/agentforge/__init__.py
+-rw-rw-rw-   0        0        0     6173 2024-03-01 01:43:06.000000 agentforge-0.2.9/src/agentforge/agent.py
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.244725 agentforge-0.2.9/src/agentforge/agents/
+-rw-rw-rw-   0        0        0     1272 2024-02-22 23:07:46.000000 agentforge-0.2.9/src/agentforge/agents/ActionPrimingAgent.py
+-rw-rw-rw-   0        0        0     6205 2024-02-25 19:07:28.000000 agentforge-0.2.9/src/agentforge/agents/ActionSelectionAgent.py
+-rw-rw-rw-   0        0        0     1021 2024-02-22 23:07:46.000000 agentforge-0.2.9/src/agentforge/agents/LearnKGAgent.py
+-rw-rw-rw-   0        0        0     1024 2024-03-01 01:43:40.000000 agentforge-0.2.9/src/agentforge/agents/MetadataKGAgent.py
+-rw-rw-rw-   0        0        0        0 2023-11-05 01:11:53.000000 agentforge-0.2.9/src/agentforge/agents/__init__.py
+-rw-rw-rw-   0        0        0     9226 2024-02-28 12:43:58.000000 agentforge-0.2.9/src/agentforge/config.py
+-rw-rw-rw-   0        0        0     3994 2024-03-08 22:49:07.000000 agentforge-0.2.9/src/agentforge/init_agentforge.py
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.311725 agentforge-0.2.9/src/agentforge/llm/
+-rw-rw-rw-   0        0        0      111 2023-11-05 01:11:53.000000 agentforge-0.2.9/src/agentforge/llm/__init__.py
+-rw-rw-rw-   0        0        0     3919 2024-03-18 22:29:05.000000 agentforge-0.2.9/src/agentforge/llm/anthropic.py
+-rw-rw-rw-   0        0        0     3512 2024-03-07 18:45:00.000000 agentforge-0.2.9/src/agentforge/llm/claude_old.py
+-rw-rw-rw-   0        0        0     1968 2024-02-22 23:07:46.000000 agentforge-0.2.9/src/agentforge/llm/customapi.py
+-rw-rw-rw-   0        0        0     3484 2024-02-22 23:07:46.000000 agentforge-0.2.9/src/agentforge/llm/gemini.py
+-rw-rw-rw-   0        0        0     4945 2024-02-22 23:07:46.000000 agentforge-0.2.9/src/agentforge/llm/oobabooga.py
+-rw-rw-rw-   0        0        0     4032 2024-02-22 23:07:46.000000 agentforge-0.2.9/src/agentforge/llm/openai.py
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.358724 agentforge-0.2.9/src/agentforge/modules/
+-rw-rw-rw-   0        0        0     9460 2024-02-25 19:07:28.000000 agentforge-0.2.9/src/agentforge/modules/ActionExecution.py
+-rw-rw-rw-   0        0        0     3014 2024-03-07 17:45:26.000000 agentforge-0.2.9/src/agentforge/modules/InjectKG.py
+-rw-rw-rw-   0        0        0     6396 2024-03-07 17:45:26.000000 agentforge-0.2.9/src/agentforge/modules/KnowledgeTraversal.py
+-rw-rw-rw-   0        0        0     5048 2024-03-07 17:45:27.000000 agentforge-0.2.9/src/agentforge/modules/LearnDoc.py
+-rw-rw-rw-   0        0        0        0 2023-11-05 01:11:53.000000 agentforge-0.2.9/src/agentforge/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.360725 agentforge-0.2.9/src/agentforge/setup_files/
+-rw-rw-rw-   0        0        0        0 2024-02-25 19:07:27.000000 agentforge-0.2.9/src/agentforge/setup_files/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.372725 agentforge-0.2.9/src/agentforge/setup_files/actions/
+-rw-rw-rw-   0        0        0      593 2024-02-25 19:07:27.000000 agentforge-0.2.9/src/agentforge/setup_files/actions/WebSearch.yaml
+-rw-rw-rw-   0        0        0      871 2024-02-25 19:07:27.000000 agentforge-0.2.9/src/agentforge/setup_files/actions/WriteFile.yaml
+-rw-rw-rw-   0        0        0        0 2024-03-08 20:43:54.000000 agentforge-0.2.9/src/agentforge/setup_files/actions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.374753 agentforge-0.2.9/src/agentforge/setup_files/agents/
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.401725 agentforge-0.2.9/src/agentforge/setup_files/agents/ModuleAgents/
+-rw-rw-rw-   0        0        0     1314 2024-02-25 19:07:27.000000 agentforge-0.2.9/src/agentforge/setup_files/agents/ModuleAgents/ActionPrimingAgent.yaml
+-rw-rw-rw-   0        0        0     1394 2024-02-25 19:07:27.000000 agentforge-0.2.9/src/agentforge/setup_files/agents/ModuleAgents/ActionSelectionAgent.yaml
+-rw-rw-rw-   0        0        0     2241 2024-03-07 17:45:26.000000 agentforge-0.2.9/src/agentforge/setup_files/agents/ModuleAgents/LearnKGAgent.yaml
+-rw-rw-rw-   0        0        0     1865 2024-03-07 17:45:26.000000 agentforge-0.2.9/src/agentforge/setup_files/agents/ModuleAgents/MetadataKGAgent.yaml
+-rw-rw-rw-   0        0        0        0 2024-03-08 22:49:07.000000 agentforge-0.2.9/src/agentforge/setup_files/agents/ModuleAgents/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-03-08 20:43:54.000000 agentforge-0.2.9/src/agentforge/setup_files/agents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.411725 agentforge-0.2.9/src/agentforge/setup_files/personas/
+-rw-rw-rw-   0        0        0        0 2024-03-08 20:43:54.000000 agentforge-0.2.9/src/agentforge/setup_files/personas/__init__.py
+-rw-rw-rw-   0        0        0     3133 2024-03-04 17:34:34.000000 agentforge-0.2.9/src/agentforge/setup_files/personas/default.yaml
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.437725 agentforge-0.2.9/src/agentforge/setup_files/settings/
+-rw-rw-rw-   0        0        0        0 2024-03-08 20:43:54.000000 agentforge-0.2.9/src/agentforge/setup_files/settings/__init__.py
+-rw-rw-rw-   0        0        0     1939 2024-03-08 01:11:23.000000 agentforge-0.2.9/src/agentforge/setup_files/settings/models.yaml
+-rw-rw-rw-   0        0        0      285 2024-03-01 03:03:24.000000 agentforge-0.2.9/src/agentforge/setup_files/settings/storage.yaml
+-rw-rw-rw-   0        0        0      221 2024-03-08 01:14:02.000000 agentforge-0.2.9/src/agentforge/setup_files/settings/system.yaml
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.472725 agentforge-0.2.9/src/agentforge/setup_files/tools/
+-rw-rw-rw-   0        0        0      647 2024-02-25 19:07:27.000000 agentforge-0.2.9/src/agentforge/setup_files/tools/FileWriter.yaml
+-rw-rw-rw-   0        0        0      747 2024-02-25 19:07:27.000000 agentforge-0.2.9/src/agentforge/setup_files/tools/GoogleSearch.yaml
+-rw-rw-rw-   0        0        0      739 2024-02-25 19:07:27.000000 agentforge-0.2.9/src/agentforge/setup_files/tools/IntelligentChunk.yaml
+-rw-rw-rw-   0        0        0     1380 2024-02-25 19:07:27.000000 agentforge-0.2.9/src/agentforge/setup_files/tools/ReadDirectory.yaml
+-rw-rw-rw-   0        0        0      482 2024-02-25 19:07:27.000000 agentforge-0.2.9/src/agentforge/setup_files/tools/ReadFile.yaml
+-rw-rw-rw-   0        0        0      641 2024-02-25 19:07:27.000000 agentforge-0.2.9/src/agentforge/setup_files/tools/WebScrape.yaml
+-rw-rw-rw-   0        0        0        0 2024-03-08 20:43:54.000000 agentforge-0.2.9/src/agentforge/setup_files/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.578730 agentforge-0.2.9/src/agentforge/tools/
+-rw-rw-rw-   0        0        0      840 2024-03-01 02:15:14.000000 agentforge-0.2.9/src/agentforge/tools/CleanString.py
+-rw-rw-rw-   0        0        0     1531 2023-11-05 01:11:53.000000 agentforge-0.2.9/src/agentforge/tools/CommandExecutor.py
+-rw-rw-rw-   0        0        0     4041 2024-02-25 19:04:33.000000 agentforge-0.2.9/src/agentforge/tools/Directory.py
+-rw-rw-rw-   0        0        0     1630 2024-02-22 23:07:46.000000 agentforge-0.2.9/src/agentforge/tools/GetText.py
+-rw-rw-rw-   0        0        0     1853 2023-11-05 01:11:53.000000 agentforge-0.2.9/src/agentforge/tools/GoogleSearch.py
+-rw-rw-rw-   0        0        0     1456 2024-03-01 02:26:55.000000 agentforge-0.2.9/src/agentforge/tools/IntelligentChunk.py
+-rw-rw-rw-   0        0        0     8938 2024-03-01 01:43:40.000000 agentforge-0.2.9/src/agentforge/tools/TripleExtract.py
+-rw-rw-rw-   0        0        0     2158 2023-11-05 01:11:53.000000 agentforge-0.2.9/src/agentforge/tools/UserInput.py
+-rw-rw-rw-   0        0        0     1208 2024-02-25 19:04:33.000000 agentforge-0.2.9/src/agentforge/tools/WebScrape.py
+-rw-rw-rw-   0        0        0     1839 2023-11-05 01:11:53.000000 agentforge-0.2.9/src/agentforge/tools/WriteFile.py
+-rw-rw-rw-   0        0        0        0 2023-11-05 01:11:53.000000 agentforge-0.2.9/src/agentforge/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.622725 agentforge-0.2.9/src/agentforge/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-05 01:11:53.000000 agentforge-0.2.9/src/agentforge/utils/__init__.py
+-rw-rw-rw-   0        0        0    17118 2024-03-01 01:43:06.000000 agentforge-0.2.9/src/agentforge/utils/chroma_utils.py
+-rw-rw-rw-   0        0        0     1911 2024-02-22 23:07:46.000000 agentforge-0.2.9/src/agentforge/utils/function_utils.py
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.759835 agentforge-0.2.9/src/agentforge/utils/functions/
+-rw-rw-rw-   0        0        0     6381 2024-02-22 23:07:46.000000 agentforge-0.2.9/src/agentforge/utils/functions/AgentUtils.py
+-rw-rw-rw-   0        0        0    12984 2024-03-04 17:34:34.000000 agentforge-0.2.9/src/agentforge/utils/functions/Logger.py
+-rw-rw-rw-   0        0        0     3792 2024-02-22 23:07:46.000000 agentforge-0.2.9/src/agentforge/utils/functions/PromptHandling.py
+-rw-rw-rw-   0        0        0     4596 2024-02-22 23:07:46.000000 agentforge-0.2.9/src/agentforge/utils/functions/ToolUtils.py
+-rw-rw-rw-   0        0        0     3666 2024-03-01 01:43:06.000000 agentforge-0.2.9/src/agentforge/utils/functions/UserInterface.py
+-rw-rw-rw-   0        0        0        0 2023-11-05 01:11:53.000000 agentforge-0.2.9/src/agentforge/utils/functions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.126007 agentforge-0.2.9/src/agentforge/utils/guiutils/
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.765860 agentforge-0.2.9/src/agentforge/utils/guiutils/__pycache__/
+-rw-rw-rw-   0        0        0      167 2023-11-05 01:25:48.000000 agentforge-0.2.9/src/agentforge/utils/guiutils/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1894 2023-11-05 01:25:48.000000 agentforge-0.2.9/src/agentforge/utils/guiutils/__pycache__/listenforui.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1847 2023-11-15 20:19:25.000000 agentforge-0.2.9/src/agentforge/utils/guiutils/__pycache__/sendtoui.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.127005 agentforge-0.2.9/src/agentforge/utils/installer/
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.769834 agentforge-0.2.9/src/agentforge/utils/installer/__pycache__/
+-rw-rw-rw-   0        0        0      168 2023-11-05 03:47:12.000000 agentforge-0.2.9/src/agentforge/utils/installer/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6875 2023-12-08 19:16:40.000000 agentforge-0.2.9/src/agentforge/utils/installer/__pycache__/agentforge_cli.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1373 2023-11-26 23:09:06.000000 agentforge-0.2.9/src/agentforge/utils/pinecone_utils.py
+-rw-rw-rw-   0        0        0     3573 2024-02-28 12:43:58.000000 agentforge-0.2.9/src/agentforge/utils/storage_interface.py
+drwxrwxrwx   0        0        0        0 2024-03-22 22:14:16.201552 agentforge-0.2.9/src/agentforge.egg-info/
+-rw-rw-rw-   0        0        0     6327 2024-03-22 22:14:15.000000 agentforge-0.2.9/src/agentforge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3354 2024-03-22 22:14:16.000000 agentforge-0.2.9/src/agentforge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-22 22:14:15.000000 agentforge-0.2.9/src/agentforge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      457 2024-03-22 22:14:15.000000 agentforge-0.2.9/src/agentforge.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-22 22:14:15.000000 agentforge-0.2.9/src/agentforge.egg-info/top_level.txt
```

### Comparing `agentforge-0.2.8/LICENSE` & `agentforge-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/PKG-INFO` & `agentforge-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentforge
-Version: 0.2.8
+Version: 0.2.9
 Summary: AI-driven task automation system
 Home-page: https://github.com/DataBassGit/HiAGI
 Author: John Smith, Ansel Anselmi
 Author-email: contact@agentforge.net
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `agentforge-0.2.8/README.md` & `agentforge-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/setup.py` & `agentforge-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def get_long_description():
     with open("README.md") as file:
         return file.read()
 
 
 setup(
     name="agentforge",
-    version="0.2.8",
+    version="0.2.9",
     description="AI-driven task automation system",
     author="John Smith, Ansel Anselmi",
     author_email="contact@agentforge.net",
     url="https://github.com/DataBassGit/HiAGI",
     include_package_data=True,
     packages=find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `agentforge-0.2.8/src/agentforge/agent.py` & `agentforge-0.2.9/src/agentforge/agent.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/agents/ActionPrimingAgent.py` & `agentforge-0.2.9/src/agentforge/agents/ActionPrimingAgent.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/agents/ActionSelectionAgent.py` & `agentforge-0.2.9/src/agentforge/agents/ActionSelectionAgent.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/agents/LearnKGAgent.py` & `agentforge-0.2.9/src/agentforge/agents/LearnKGAgent.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/agents/MetadataKGAgent.py` & `agentforge-0.2.9/src/agentforge/agents/MetadataKGAgent.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/config.py` & `agentforge-0.2.9/src/agentforge/config.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/init_agentforge.py` & `agentforge-0.2.9/src/agentforge/init_agentforge.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/llm/anthropic.py` & `agentforge-0.2.9/src/agentforge/llm/anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             str or None: The generated text from the model or None if the operation fails after retry attempts.
 
         This method attempts to generate content with the provided prompts and configuration, retrying up to a
         specified number of times with exponential backoff in case of errors. It logs the process and outcomes.
         """
         self.logger = Logger(name=params.pop('agent_name', 'NamelessAgent'))
         prompt = parse_prompts(prompts)
-        self.logger.log_prompt(prompt)
+        self.logger.log_prompt(f"System: {prompts[0]}\n\nUser: {prompt}")
 
         # Will retry to get chat if a rate limit or bad gateway error is received from the chat
         response = None
         for attempt in range(self.num_retries):
             backoff = 2 ** (attempt + 2)
             try:
                 response = client.messages.create(
```

### Comparing `agentforge-0.2.8/src/agentforge/llm/claude_old.py` & `agentforge-0.2.9/src/agentforge/llm/claude_old.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/llm/customapi.py` & `agentforge-0.2.9/src/agentforge/llm/customapi.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/llm/gemini.py` & `agentforge-0.2.9/src/agentforge/llm/gemini.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/llm/oobabooga.py` & `agentforge-0.2.9/src/agentforge/llm/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/llm/openai.py` & `agentforge-0.2.9/src/agentforge/llm/openai.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/modules/ActionExecution.py` & `agentforge-0.2.9/src/agentforge/modules/ActionExecution.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/modules/InjectKG.py` & `agentforge-0.2.9/src/agentforge/modules/InjectKG.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/modules/KnowledgeTraversal.py` & `agentforge-0.2.9/src/agentforge/modules/KnowledgeTraversal.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/modules/LearnDoc.py` & `agentforge-0.2.9/src/agentforge/modules/LearnDoc.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/setup_files/actions/WebSearch.yaml` & `agentforge-0.2.9/src/agentforge/setup_files/actions/WebSearch.yaml`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/setup_files/actions/WriteFile.yaml` & `agentforge-0.2.9/src/agentforge/setup_files/actions/WriteFile.yaml`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/setup_files/agents/ModuleAgents/ActionPrimingAgent.yaml` & `agentforge-0.2.9/src/agentforge/setup_files/agents/ModuleAgents/ActionPrimingAgent.yaml`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/setup_files/agents/ModuleAgents/ActionSelectionAgent.yaml` & `agentforge-0.2.9/src/agentforge/setup_files/agents/ModuleAgents/ActionSelectionAgent.yaml`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/setup_files/agents/ModuleAgents/LearnKGAgent.yaml` & `agentforge-0.2.9/src/agentforge/setup_files/agents/ModuleAgents/LearnKGAgent.yaml`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/setup_files/agents/ModuleAgents/MetadataKGAgent.yaml` & `agentforge-0.2.9/src/agentforge/setup_files/agents/ModuleAgents/MetadataKGAgent.yaml`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/setup_files/personas/default.yaml` & `agentforge-0.2.9/src/agentforge/setup_files/personas/default.yaml`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/setup_files/settings/models.yaml` & `agentforge-0.2.9/src/agentforge/setup_files/settings/models.yaml`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/setup_files/tools/FileWriter.yaml` & `agentforge-0.2.9/src/agentforge/setup_files/tools/FileWriter.yaml`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/setup_files/tools/GoogleSearch.yaml` & `agentforge-0.2.9/src/agentforge/setup_files/tools/GoogleSearch.yaml`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/setup_files/tools/IntelligentChunk.yaml` & `agentforge-0.2.9/src/agentforge/setup_files/tools/IntelligentChunk.yaml`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/setup_files/tools/ReadDirectory.yaml` & `agentforge-0.2.9/src/agentforge/setup_files/tools/ReadDirectory.yaml`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/setup_files/tools/WebScrape.yaml` & `agentforge-0.2.9/src/agentforge/setup_files/tools/WebScrape.yaml`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/tools/CleanString.py` & `agentforge-0.2.9/src/agentforge/tools/CleanString.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/tools/CommandExecutor.py` & `agentforge-0.2.9/src/agentforge/tools/CommandExecutor.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/tools/Directory.py` & `agentforge-0.2.9/src/agentforge/tools/Directory.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/tools/GetText.py` & `agentforge-0.2.9/src/agentforge/tools/GetText.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/tools/GoogleSearch.py` & `agentforge-0.2.9/src/agentforge/tools/GoogleSearch.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/tools/IntelligentChunk.py` & `agentforge-0.2.9/src/agentforge/tools/IntelligentChunk.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/tools/TripleExtract.py` & `agentforge-0.2.9/src/agentforge/tools/TripleExtract.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/tools/UserInput.py` & `agentforge-0.2.9/src/agentforge/tools/UserInput.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/tools/WebScrape.py` & `agentforge-0.2.9/src/agentforge/tools/WebScrape.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/tools/WriteFile.py` & `agentforge-0.2.9/src/agentforge/tools/WriteFile.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/utils/chroma_utils.py` & `agentforge-0.2.9/src/agentforge/utils/chroma_utils.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/utils/function_utils.py` & `agentforge-0.2.9/src/agentforge/utils/function_utils.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/utils/functions/AgentUtils.py` & `agentforge-0.2.9/src/agentforge/utils/functions/AgentUtils.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/utils/functions/Logger.py` & `agentforge-0.2.9/src/agentforge/utils/functions/Logger.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/utils/functions/PromptHandling.py` & `agentforge-0.2.9/src/agentforge/utils/functions/PromptHandling.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/utils/functions/ToolUtils.py` & `agentforge-0.2.9/src/agentforge/utils/functions/ToolUtils.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/utils/functions/UserInterface.py` & `agentforge-0.2.9/src/agentforge/utils/functions/UserInterface.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/utils/guiutils/__pycache__/listenforui.cpython-311.pyc` & `agentforge-0.2.9/src/agentforge/utils/guiutils/__pycache__/listenforui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/utils/guiutils/__pycache__/sendtoui.cpython-311.pyc` & `agentforge-0.2.9/src/agentforge/utils/guiutils/__pycache__/sendtoui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/utils/installer/__pycache__/agentforge_cli.cpython-311.pyc` & `agentforge-0.2.9/src/agentforge/utils/installer/__pycache__/agentforge_cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/utils/pinecone_utils.py` & `agentforge-0.2.9/src/agentforge/utils/pinecone_utils.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge/utils/storage_interface.py` & `agentforge-0.2.9/src/agentforge/utils/storage_interface.py`

 * *Files identical despite different names*

### Comparing `agentforge-0.2.8/src/agentforge.egg-info/PKG-INFO` & `agentforge-0.2.9/src/agentforge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentforge
-Version: 0.2.8
+Version: 0.2.9
 Summary: AI-driven task automation system
 Home-page: https://github.com/DataBassGit/HiAGI
 Author: John Smith, Ansel Anselmi
 Author-email: contact@agentforge.net
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `agentforge-0.2.8/src/agentforge.egg-info/SOURCES.txt` & `agentforge-0.2.9/src/agentforge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

