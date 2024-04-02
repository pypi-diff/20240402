# Comparing `tmp/intelli-0.3.1.tar.gz` & `tmp/intelli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intelli-0.3.1.tar", last modified: Mon Apr  1 00:03:35 2024, max compression
+gzip compressed data, was "intelli-0.3.2.tar", last modified: Tue Apr  2 10:34:11 2024, max compression
```

## Comparing `intelli-0.3.1.tar` & `intelli-0.3.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.135228 intelli-0.3.1/
--rw-r--r--   0 barqawicloud   (503) staff       (20)    11341 2024-02-07 02:41:23.000000 intelli-0.3.1/LICENSE
--rw-r--r--   0 barqawicloud   (503) staff       (20)     5643 2024-04-01 00:03:35.134942 intelli-0.3.1/PKG-INFO
--rw-r--r--   0 barqawicloud   (503) staff       (20)     5674 2024-03-09 16:51:25.000000 intelli-0.3.1/README.md
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.121571 intelli-0.3.1/intelli/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-01 22:27:56.000000 intelli-0.3.1/intelli/__init__.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     4315 2024-03-08 11:23:46.000000 intelli-0.3.1/intelli/config.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.123230 intelli-0.3.1/intelli/controller/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-04 14:46:04.000000 intelli-0.3.1/intelli/controller/__init__.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1468 2024-03-08 11:23:46.000000 intelli-0.3.1/intelli/controller/remote_embed_model.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1510 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/controller/remote_image_model.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1893 2024-03-09 15:27:57.000000 intelli-0.3.1/intelli/controller/remote_speech_model.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1720 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/controller/remote_vision_model.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.123880 intelli-0.3.1/intelli/flow/
--rw-r--r--   0 barqawicloud   (503) staff       (20)      413 2024-03-31 23:55:07.000000 intelli-0.3.1/intelli/flow/__init__.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.124321 intelli-0.3.1/intelli/flow/agents/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-07 03:19:36.000000 intelli-0.3.1/intelli/flow/agents/__init__.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     2883 2024-03-17 23:17:08.000000 intelli-0.3.1/intelli/flow/agents/agent.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     6115 2024-03-26 19:38:53.000000 intelli-0.3.1/intelli/flow/agents/kagent.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     5265 2024-04-01 00:00:13.000000 intelli-0.3.1/intelli/flow/flow.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.124867 intelli-0.3.1/intelli/flow/input/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-07 03:19:33.000000 intelli-0.3.1/intelli/flow/input/__init__.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)      369 2024-02-08 23:47:11.000000 intelli-0.3.1/intelli/flow/input/agent_input.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)      364 2024-02-11 16:27:41.000000 intelli-0.3.1/intelli/flow/input/task_input.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.125226 intelli-0.3.1/intelli/flow/processors/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-07 03:19:28.000000 intelli-0.3.1/intelli/flow/processors/__init__.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)      102 2024-02-06 00:48:36.000000 intelli-0.3.1/intelli/flow/processors/basic_processor.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)      730 2024-02-08 23:47:11.000000 intelli-0.3.1/intelli/flow/sequence_flow.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.125520 intelli-0.3.1/intelli/flow/tasks/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-08 23:47:11.000000 intelli-0.3.1/intelli/flow/tasks/__init__.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     3875 2024-03-17 22:17:44.000000 intelli-0.3.1/intelli/flow/tasks/task.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.125821 intelli-0.3.1/intelli/flow/template/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-07 03:19:19.000000 intelli-0.3.1/intelli/flow/template/__init__.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)      720 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/flow/template/basic_template.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)      403 2024-02-11 10:37:06.000000 intelli-0.3.1/intelli/flow/types.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.126116 intelli-0.3.1/intelli/function/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-04 14:46:04.000000 intelli-0.3.1/intelli/function/__init__.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     8213 2024-03-09 16:42:10.000000 intelli-0.3.1/intelli/function/chatbot.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.126367 intelli-0.3.1/intelli/model/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-04 14:46:04.000000 intelli-0.3.1/intelli/model/__init__.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.127696 intelli-0.3.1/intelli/model/input/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-04 14:46:04.000000 intelli-0.3.1/intelli/model/input/__init__.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     3818 2024-03-09 15:27:57.000000 intelli-0.3.1/intelli/model/input/chatbot_input.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)      980 2024-02-04 14:46:04.000000 intelli-0.3.1/intelli/model/input/embed_input.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     2355 2024-03-09 15:27:57.000000 intelli-0.3.1/intelli/model/input/image_input.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1529 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/model/input/text_speech_input.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     2163 2024-02-11 16:33:48.000000 intelli-0.3.1/intelli/model/input/vision_input.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.127923 intelli-0.3.1/intelli/resource/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-08 23:47:11.000000 intelli-0.3.1/intelli/resource/__init__.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.128218 intelli-0.3.1/intelli/resource/templates/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-08 23:02:07.000000 intelli-0.3.1/intelli/resource/templates/__init__.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)      373 2024-02-05 09:55:15.000000 intelli-0.3.1/intelli/resource/templates/augmented_chatbot.in
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.128410 intelli-0.3.1/intelli/test/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-04 14:46:04.000000 intelli-0.3.1/intelli/test/__init__.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.131955 intelli-0.3.1/intelli/test/integration/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-04 14:46:04.000000 intelli-0.3.1/intelli/test/integration/__init__.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     2431 2024-03-08 11:23:46.000000 intelli-0.3.1/intelli/test/integration/test_anthropic_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1254 2024-02-06 01:52:52.000000 intelli-0.3.1/intelli/test/integration/test_azure_chatbot.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     4103 2024-03-09 16:46:35.000000 intelli-0.3.1/intelli/test/integration/test_chatbot.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     3025 2024-02-06 01:52:52.000000 intelli-0.3.1/intelli/test/integration/test_chatbot_with_data.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     3484 2024-02-08 19:58:26.000000 intelli-0.3.1/intelli/test/integration/test_cohereai_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     2265 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/test/integration/test_flow_icons.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     7035 2024-03-26 19:38:53.000000 intelli-0.3.1/intelli/test/integration/test_flow_map.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     3529 2024-03-17 23:17:08.000000 intelli-0.3.1/intelli/test/integration/test_flow_sequence.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     2953 2024-02-10 22:31:44.000000 intelli-0.3.1/intelli/test/integration/test_geminiai_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)      727 2024-02-18 10:42:27.000000 intelli-0.3.1/intelli/test/integration/test_googleai_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1359 2024-02-06 01:52:52.000000 intelli-0.3.1/intelli/test/integration/test_intellicloud_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1507 2024-03-02 01:44:11.000000 intelli-0.3.1/intelli/test/integration/test_keras_agent.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1570 2024-02-06 01:52:52.000000 intelli-0.3.1/intelli/test/integration/test_mistralai_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     5366 2024-02-18 10:42:27.000000 intelli-0.3.1/intelli/test/integration/test_openai_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1252 2024-02-18 09:21:55.000000 intelli-0.3.1/intelli/test/integration/test_prod_data.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     2344 2024-03-08 11:23:46.000000 intelli-0.3.1/intelli/test/integration/test_remote_embed_model.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     4409 2024-02-06 01:52:52.000000 intelli-0.3.1/intelli/test/integration/test_remote_image_model.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     2152 2024-02-18 10:42:27.000000 intelli-0.3.1/intelli/test/integration/test_remote_speech_model.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1454 2024-02-10 22:31:31.000000 intelli-0.3.1/intelli/test/integration/test_remote_vision_model.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1945 2024-02-06 01:52:52.000000 intelli-0.3.1/intelli/test/integration/test_stability_wrapper.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.132860 intelli-0.3.1/intelli/utils/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-01-31 22:17:36.000000 intelli-0.3.1/intelli/utils/__init__.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)      753 2024-02-08 19:58:26.000000 intelli-0.3.1/intelli/utils/cohere_stream_parser.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)      450 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/utils/conn_helper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)      548 2024-02-08 23:47:11.000000 intelli-0.3.1/intelli/utils/logging.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     6123 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/utils/proxy_helper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     2026 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/utils/system_helper.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.134205 intelli-0.3.1/intelli/wrappers/
--rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-01-31 22:17:36.000000 intelli-0.3.1/intelli/wrappers/__init__.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1710 2024-03-09 15:27:57.000000 intelli-0.3.1/intelli/wrappers/anthropic_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1717 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/wrappers/cohereai_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     2611 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/wrappers/geminiai_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1231 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/wrappers/googleai_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1007 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/wrappers/intellicloud_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     1212 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/wrappers/mistralai_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)     6512 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/wrappers/openai_wrapper.py
--rw-r--r--   0 barqawicloud   (503) staff       (20)      888 2024-02-19 18:51:19.000000 intelli-0.3.1/intelli/wrappers/stability_wrapper.py
-drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-01 00:03:35.122492 intelli-0.3.1/intelli.egg-info/
--rw-r--r--   0 barqawicloud   (503) staff       (20)     5643 2024-04-01 00:03:35.000000 intelli-0.3.1/intelli.egg-info/PKG-INFO
--rw-r--r--   0 barqawicloud   (503) staff       (20)     2874 2024-04-01 00:03:35.000000 intelli-0.3.1/intelli.egg-info/SOURCES.txt
--rw-r--r--   0 barqawicloud   (503) staff       (20)        1 2024-04-01 00:03:35.000000 intelli-0.3.1/intelli.egg-info/dependency_links.txt
--rw-r--r--   0 barqawicloud   (503) staff       (20)       95 2024-04-01 00:03:35.000000 intelli-0.3.1/intelli.egg-info/requires.txt
--rw-r--r--   0 barqawicloud   (503) staff       (20)        8 2024-04-01 00:03:35.000000 intelli-0.3.1/intelli.egg-info/top_level.txt
--rw-r--r--   0 barqawicloud   (503) staff       (20)       38 2024-04-01 00:03:35.135276 intelli-0.3.1/setup.cfg
--rw-r--r--   0 barqawicloud   (503) staff       (20)      910 2024-03-31 23:56:14.000000 intelli-0.3.1/setup.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.194075 intelli-0.3.2/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)    11341 2024-02-07 02:41:23.000000 intelli-0.3.2/LICENSE
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     5643 2024-04-02 10:34:11.193791 intelli-0.3.2/PKG-INFO
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     5497 2024-04-02 10:33:22.000000 intelli-0.3.2/README.md
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.177574 intelli-0.3.2/intelli/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-01 22:27:56.000000 intelli-0.3.2/intelli/__init__.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     4315 2024-03-08 11:23:46.000000 intelli-0.3.2/intelli/config.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.179645 intelli-0.3.2/intelli/controller/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-04 14:46:04.000000 intelli-0.3.2/intelli/controller/__init__.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1468 2024-03-08 11:23:46.000000 intelli-0.3.2/intelli/controller/remote_embed_model.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1510 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/controller/remote_image_model.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1893 2024-03-09 15:27:57.000000 intelli-0.3.2/intelli/controller/remote_speech_model.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1720 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/controller/remote_vision_model.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.180473 intelli-0.3.2/intelli/flow/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      413 2024-03-31 23:55:07.000000 intelli-0.3.2/intelli/flow/__init__.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.180948 intelli-0.3.2/intelli/flow/agents/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-07 03:19:36.000000 intelli-0.3.2/intelli/flow/agents/__init__.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     2883 2024-03-17 23:17:08.000000 intelli-0.3.2/intelli/flow/agents/agent.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     6115 2024-03-26 19:38:53.000000 intelli-0.3.2/intelli/flow/agents/kagent.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     5363 2024-04-02 10:33:31.000000 intelli-0.3.2/intelli/flow/flow.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.181868 intelli-0.3.2/intelli/flow/input/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-07 03:19:33.000000 intelli-0.3.2/intelli/flow/input/__init__.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      369 2024-02-08 23:47:11.000000 intelli-0.3.2/intelli/flow/input/agent_input.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      364 2024-02-11 16:27:41.000000 intelli-0.3.2/intelli/flow/input/task_input.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.182169 intelli-0.3.2/intelli/flow/processors/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-07 03:19:28.000000 intelli-0.3.2/intelli/flow/processors/__init__.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      102 2024-02-06 00:48:36.000000 intelli-0.3.2/intelli/flow/processors/basic_processor.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      730 2024-02-08 23:47:11.000000 intelli-0.3.2/intelli/flow/sequence_flow.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.182455 intelli-0.3.2/intelli/flow/tasks/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-08 23:47:11.000000 intelli-0.3.2/intelli/flow/tasks/__init__.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     3875 2024-03-17 22:17:44.000000 intelli-0.3.2/intelli/flow/tasks/task.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.182756 intelli-0.3.2/intelli/flow/template/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-07 03:19:19.000000 intelli-0.3.2/intelli/flow/template/__init__.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      720 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/flow/template/basic_template.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      403 2024-02-11 10:37:06.000000 intelli-0.3.2/intelli/flow/types.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.183172 intelli-0.3.2/intelli/function/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-04 14:46:04.000000 intelli-0.3.2/intelli/function/__init__.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     8213 2024-03-09 16:42:10.000000 intelli-0.3.2/intelli/function/chatbot.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.183453 intelli-0.3.2/intelli/model/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-04 14:46:04.000000 intelli-0.3.2/intelli/model/__init__.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.184660 intelli-0.3.2/intelli/model/input/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-04 14:46:04.000000 intelli-0.3.2/intelli/model/input/__init__.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     3818 2024-03-09 15:27:57.000000 intelli-0.3.2/intelli/model/input/chatbot_input.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      980 2024-02-04 14:46:04.000000 intelli-0.3.2/intelli/model/input/embed_input.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     2355 2024-03-09 15:27:57.000000 intelli-0.3.2/intelli/model/input/image_input.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1529 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/model/input/text_speech_input.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     2163 2024-02-11 16:33:48.000000 intelli-0.3.2/intelli/model/input/vision_input.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.184923 intelli-0.3.2/intelli/resource/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-08 23:47:11.000000 intelli-0.3.2/intelli/resource/__init__.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.185192 intelli-0.3.2/intelli/resource/templates/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-08 23:02:07.000000 intelli-0.3.2/intelli/resource/templates/__init__.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      373 2024-02-05 09:55:15.000000 intelli-0.3.2/intelli/resource/templates/augmented_chatbot.in
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.185526 intelli-0.3.2/intelli/test/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-04 14:46:04.000000 intelli-0.3.2/intelli/test/__init__.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.190148 intelli-0.3.2/intelli/test/integration/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-02-04 14:46:04.000000 intelli-0.3.2/intelli/test/integration/__init__.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     2431 2024-03-08 11:23:46.000000 intelli-0.3.2/intelli/test/integration/test_anthropic_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1254 2024-02-06 01:52:52.000000 intelli-0.3.2/intelli/test/integration/test_azure_chatbot.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     4103 2024-03-09 16:46:35.000000 intelli-0.3.2/intelli/test/integration/test_chatbot.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     3025 2024-02-06 01:52:52.000000 intelli-0.3.2/intelli/test/integration/test_chatbot_with_data.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     3484 2024-02-08 19:58:26.000000 intelli-0.3.2/intelli/test/integration/test_cohereai_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     2265 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/test/integration/test_flow_icons.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     7035 2024-03-26 19:38:53.000000 intelli-0.3.2/intelli/test/integration/test_flow_map.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     3529 2024-03-17 23:17:08.000000 intelli-0.3.2/intelli/test/integration/test_flow_sequence.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     2953 2024-02-10 22:31:44.000000 intelli-0.3.2/intelli/test/integration/test_geminiai_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      727 2024-02-18 10:42:27.000000 intelli-0.3.2/intelli/test/integration/test_googleai_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1359 2024-02-06 01:52:52.000000 intelli-0.3.2/intelli/test/integration/test_intellicloud_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1507 2024-03-02 01:44:11.000000 intelli-0.3.2/intelli/test/integration/test_keras_agent.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1570 2024-02-06 01:52:52.000000 intelli-0.3.2/intelli/test/integration/test_mistralai_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     5366 2024-02-18 10:42:27.000000 intelli-0.3.2/intelli/test/integration/test_openai_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1252 2024-02-18 09:21:55.000000 intelli-0.3.2/intelli/test/integration/test_prod_data.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     2344 2024-03-08 11:23:46.000000 intelli-0.3.2/intelli/test/integration/test_remote_embed_model.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     4409 2024-02-06 01:52:52.000000 intelli-0.3.2/intelli/test/integration/test_remote_image_model.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     2152 2024-02-18 10:42:27.000000 intelli-0.3.2/intelli/test/integration/test_remote_speech_model.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1454 2024-02-10 22:31:31.000000 intelli-0.3.2/intelli/test/integration/test_remote_vision_model.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1945 2024-02-06 01:52:52.000000 intelli-0.3.2/intelli/test/integration/test_stability_wrapper.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.191331 intelli-0.3.2/intelli/utils/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-01-31 22:17:36.000000 intelli-0.3.2/intelli/utils/__init__.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      753 2024-02-08 19:58:26.000000 intelli-0.3.2/intelli/utils/cohere_stream_parser.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      450 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/utils/conn_helper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      548 2024-02-08 23:47:11.000000 intelli-0.3.2/intelli/utils/logging.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     6123 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/utils/proxy_helper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     2026 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/utils/system_helper.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.192938 intelli-0.3.2/intelli/wrappers/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        0 2024-01-31 22:17:36.000000 intelli-0.3.2/intelli/wrappers/__init__.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1710 2024-03-09 15:27:57.000000 intelli-0.3.2/intelli/wrappers/anthropic_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1717 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/wrappers/cohereai_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     2611 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/wrappers/geminiai_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1231 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/wrappers/googleai_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1007 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/wrappers/intellicloud_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     1212 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/wrappers/mistralai_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     6512 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/wrappers/openai_wrapper.py
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      888 2024-02-19 18:51:19.000000 intelli-0.3.2/intelli/wrappers/stability_wrapper.py
+drwxr-xr-x   0 barqawicloud   (503) staff       (20)        0 2024-04-02 10:34:11.178817 intelli-0.3.2/intelli.egg-info/
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     5643 2024-04-02 10:34:11.000000 intelli-0.3.2/intelli.egg-info/PKG-INFO
+-rw-r--r--   0 barqawicloud   (503) staff       (20)     2874 2024-04-02 10:34:11.000000 intelli-0.3.2/intelli.egg-info/SOURCES.txt
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        1 2024-04-02 10:34:11.000000 intelli-0.3.2/intelli.egg-info/dependency_links.txt
+-rw-r--r--   0 barqawicloud   (503) staff       (20)       95 2024-04-02 10:34:11.000000 intelli-0.3.2/intelli.egg-info/requires.txt
+-rw-r--r--   0 barqawicloud   (503) staff       (20)        8 2024-04-02 10:34:11.000000 intelli-0.3.2/intelli.egg-info/top_level.txt
+-rw-r--r--   0 barqawicloud   (503) staff       (20)       38 2024-04-02 10:34:11.194126 intelli-0.3.2/setup.cfg
+-rw-r--r--   0 barqawicloud   (503) staff       (20)      910 2024-04-02 10:33:51.000000 intelli-0.3.2/setup.py
```

### Comparing `intelli-0.3.1/LICENSE` & `intelli-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/PKG-INFO` & `intelli-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelli
-Version: 0.3.1
+Version: 0.3.2
 Summary: Create chatbots and AI agent workflows. Intelli provide unified layer to connect your data with multiple AI models.
 Home-page: https://www.intellinode.ai/
 Author: Intellinode
 Author-email: admin@intellinode.ai
 Project-URL: Source Code, https://github.com/intelligentnode/Intelli
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: intelli Version: 0.3.1 Summary: Create chatbots and
+Metadata-Version: 2.1 Name: intelli Version: 0.3.2 Summary: Create chatbots and
 AI agent workflows. Intelli provide unified layer to connect your data with
 multiple AI models. Home-page: https://www.intellinode.ai/ Author: Intellinode
 Author-email: admin@intellinode.ai Project-URL: Source Code, https://
 github.com/intelligentnode/Intelli Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: networkx==3.2.1 Provides-Extra: visual Requires-Dist:
 matplotlib==3.6.0; extra == "visual" Provides-Extra: offline Requires-Dist:
```

### Comparing `intelli-0.3.1/README.md` & `intelli-0.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -60,19 +60,16 @@
 ## Create AI Flows
 You can create a flow of tasks executed by different AI models. Here's an example of creating a blog post flow:
 
 <img src="assets/flow_example.jpg" width="680em">
 
 
 ```python
-from intelli.flow.agents.agent import Agent
-from intelli.flow.tasks.task import Task
-from intelli.flow.sequence_flow import SequenceFlow
-from intelli.flow.input.task_input import TextTaskInput
-from intelli.flow.processors.basic_processor import TextProcessor
+from intelli.flow import Agent, Task, SequenceFlow, TextTaskInput, TextProcessor
+
 
 # define agents
 blog_agent = Agent(agent_type='text', provider='openai', mission='write blog posts', model_params={'key': YOUR_OPENAI_API_KEY, 'model': 'gpt-4'})
 copy_agent = Agent(agent_type='text', provider='gemini', mission='generate description', model_params={'key': YOUR_GEMINI_API_KEY, 'model': 'gemini'})
 artist_agent = Agent(agent_type='image', provider='stability', mission='generate image', model_params={'key': YOUR_STABILITY_API_KEY})
 
 # define tasks
```

#### html2text {}

```diff
@@ -15,22 +15,19 @@
 instance openai_bot = Chatbot(YOUR_API_KEY, provider) response =
 openai_bot.chat(input) return response # call chatGPT call_chatbot
 (ChatProvider.OPENAI, "gpt-4") # call mistralai call_chatbot
 (ChatProvider.MISTRAL, "mistral-medium") # call claude3 call_chatbot
 (ChatProvider.ANTHROPIC, "claude-3-sonnet-20240229") # call google gemini
 call_chatbot(ChatProvider.GEMINI) ``` ## Create AI Flows You can create a flow
 of tasks executed by different AI models. Here's an example of creating a blog
-post flow: [assets/flow_example.jpg]```python from intelli.flow.agents.agent
-import Agent from intelli.flow.tasks.task import Task from
-intelli.flow.sequence_flow import SequenceFlow from
-intelli.flow.input.task_input import TextTaskInput from
-intelli.flow.processors.basic_processor import TextProcessor # define agents
-blog_agent = Agent(agent_type='text', provider='openai', mission='write blog
-posts', model_params={'key': YOUR_OPENAI_API_KEY, 'model': 'gpt-4'}) copy_agent
-= Agent(agent_type='text', provider='gemini', mission='generate description',
+post flow: [assets/flow_example.jpg]```python from intelli.flow import Agent,
+Task, SequenceFlow, TextTaskInput, TextProcessor # define agents blog_agent =
+Agent(agent_type='text', provider='openai', mission='write blog posts',
+model_params={'key': YOUR_OPENAI_API_KEY, 'model': 'gpt-4'}) copy_agent = Agent
+(agent_type='text', provider='gemini', mission='generate description',
 model_params={'key': YOUR_GEMINI_API_KEY, 'model': 'gemini'}) artist_agent =
 Agent(agent_type='image', provider='stability', mission='generate image',
 model_params={'key': YOUR_STABILITY_API_KEY}) # define tasks task1 = Task
 (TextTaskInput('blog post about electric cars'), blog_agent, log=True) task2 =
 Task(TextTaskInput('Generate short image description for image model'),
 copy_agent, pre_process=TextProcessor.text_head, log=True) task3 = Task
 (TextTaskInput('Generate cartoon style image'), artist_agent, log=True) # start
```

### Comparing `intelli-0.3.1/intelli/config.py` & `intelli-0.3.2/intelli/config.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/controller/remote_embed_model.py` & `intelli-0.3.2/intelli/controller/remote_embed_model.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/controller/remote_image_model.py` & `intelli-0.3.2/intelli/controller/remote_image_model.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/controller/remote_speech_model.py` & `intelli-0.3.2/intelli/controller/remote_speech_model.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/controller/remote_vision_model.py` & `intelli-0.3.2/intelli/controller/remote_vision_model.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/flow/agents/agent.py` & `intelli-0.3.2/intelli/flow/agents/agent.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/flow/agents/kagent.py` & `intelli-0.3.2/intelli/flow/agents/kagent.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/flow/flow.py` & `intelli-0.3.2/intelli/flow/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import networkx as nx
 import os
 from functools import partial
-
+import traceback
 from intelli.flow.types import AgentTypes, InputTypes, Matcher
 from intelli.utils.logging import Logger
 
 try:
     import matplotlib
 
     matplotlib.use('Agg')
@@ -80,18 +80,19 @@
         ordered_tasks = list(nx.topological_sort(self.graph))
         task_coroutines = {task_name: self._execute_task(task_name) for task_name in ordered_tasks}
         async with asyncio.Semaphore(max_workers):
             for task_name in ordered_tasks:
                 try:
                     await task_coroutines[task_name]
                 except Exception as e:
-                    error_message = f"Error in task '{task_name}': {e}"
-                    print(f"Error in task '{task_name}': {e}")
+                    full_stack_trace = traceback.format_exc()
+                    error_message = f"Error in task '{task_name}': {e}\nFull stack trace:\n{full_stack_trace}"
+                    print(error_message)
                     self.errors[task_name] = error_message
-                    break
+                    continue
 
         # Filter the outputs (and types) of excluded tasks
         filtered_output = {
             task_name: {'output': self.output[task_name]['output'], 'type': self.output[task_name]['type']}
             for task_name in ordered_tasks if not self.tasks[task_name].exclude and task_name in self.output
         }
```

### Comparing `intelli-0.3.1/intelli/flow/sequence_flow.py` & `intelli-0.3.2/intelli/flow/sequence_flow.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/flow/tasks/task.py` & `intelli-0.3.2/intelli/flow/tasks/task.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/flow/template/basic_template.py` & `intelli-0.3.2/intelli/flow/template/basic_template.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/function/chatbot.py` & `intelli-0.3.2/intelli/function/chatbot.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/model/input/chatbot_input.py` & `intelli-0.3.2/intelli/model/input/chatbot_input.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/model/input/embed_input.py` & `intelli-0.3.2/intelli/model/input/embed_input.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/model/input/image_input.py` & `intelli-0.3.2/intelli/model/input/image_input.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/model/input/text_speech_input.py` & `intelli-0.3.2/intelli/model/input/text_speech_input.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/model/input/vision_input.py` & `intelli-0.3.2/intelli/model/input/vision_input.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_anthropic_wrapper.py` & `intelli-0.3.2/intelli/test/integration/test_anthropic_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_azure_chatbot.py` & `intelli-0.3.2/intelli/test/integration/test_azure_chatbot.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_chatbot.py` & `intelli-0.3.2/intelli/test/integration/test_chatbot.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_chatbot_with_data.py` & `intelli-0.3.2/intelli/test/integration/test_chatbot_with_data.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_cohereai_wrapper.py` & `intelli-0.3.2/intelli/test/integration/test_cohereai_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_flow_icons.py` & `intelli-0.3.2/intelli/test/integration/test_flow_icons.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_flow_map.py` & `intelli-0.3.2/intelli/test/integration/test_flow_map.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_flow_sequence.py` & `intelli-0.3.2/intelli/test/integration/test_flow_sequence.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_geminiai_wrapper.py` & `intelli-0.3.2/intelli/test/integration/test_geminiai_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_googleai_wrapper.py` & `intelli-0.3.2/intelli/test/integration/test_googleai_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_intellicloud_wrapper.py` & `intelli-0.3.2/intelli/test/integration/test_intellicloud_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_keras_agent.py` & `intelli-0.3.2/intelli/test/integration/test_keras_agent.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_mistralai_wrapper.py` & `intelli-0.3.2/intelli/test/integration/test_mistralai_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_openai_wrapper.py` & `intelli-0.3.2/intelli/test/integration/test_openai_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_prod_data.py` & `intelli-0.3.2/intelli/test/integration/test_prod_data.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_remote_embed_model.py` & `intelli-0.3.2/intelli/test/integration/test_remote_embed_model.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_remote_image_model.py` & `intelli-0.3.2/intelli/test/integration/test_remote_image_model.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_remote_speech_model.py` & `intelli-0.3.2/intelli/test/integration/test_remote_speech_model.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_remote_vision_model.py` & `intelli-0.3.2/intelli/test/integration/test_remote_vision_model.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/test/integration/test_stability_wrapper.py` & `intelli-0.3.2/intelli/test/integration/test_stability_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/utils/cohere_stream_parser.py` & `intelli-0.3.2/intelli/utils/cohere_stream_parser.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/utils/logging.py` & `intelli-0.3.2/intelli/utils/logging.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/utils/proxy_helper.py` & `intelli-0.3.2/intelli/utils/proxy_helper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/utils/system_helper.py` & `intelli-0.3.2/intelli/utils/system_helper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/wrappers/anthropic_wrapper.py` & `intelli-0.3.2/intelli/wrappers/anthropic_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/wrappers/cohereai_wrapper.py` & `intelli-0.3.2/intelli/wrappers/cohereai_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/wrappers/geminiai_wrapper.py` & `intelli-0.3.2/intelli/wrappers/geminiai_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/wrappers/googleai_wrapper.py` & `intelli-0.3.2/intelli/wrappers/googleai_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/wrappers/intellicloud_wrapper.py` & `intelli-0.3.2/intelli/wrappers/intellicloud_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/wrappers/mistralai_wrapper.py` & `intelli-0.3.2/intelli/wrappers/mistralai_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/wrappers/openai_wrapper.py` & `intelli-0.3.2/intelli/wrappers/openai_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli/wrappers/stability_wrapper.py` & `intelli-0.3.2/intelli/wrappers/stability_wrapper.py`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/intelli.egg-info/PKG-INFO` & `intelli-0.3.2/intelli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelli
-Version: 0.3.1
+Version: 0.3.2
 Summary: Create chatbots and AI agent workflows. Intelli provide unified layer to connect your data with multiple AI models.
 Home-page: https://www.intellinode.ai/
 Author: Intellinode
 Author-email: admin@intellinode.ai
 Project-URL: Source Code, https://github.com/intelligentnode/Intelli
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: intelli Version: 0.3.1 Summary: Create chatbots and
+Metadata-Version: 2.1 Name: intelli Version: 0.3.2 Summary: Create chatbots and
 AI agent workflows. Intelli provide unified layer to connect your data with
 multiple AI models. Home-page: https://www.intellinode.ai/ Author: Intellinode
 Author-email: admin@intellinode.ai Project-URL: Source Code, https://
 github.com/intelligentnode/Intelli Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: networkx==3.2.1 Provides-Extra: visual Requires-Dist:
 matplotlib==3.6.0; extra == "visual" Provides-Extra: offline Requires-Dist:
```

### Comparing `intelli-0.3.1/intelli.egg-info/SOURCES.txt` & `intelli-0.3.2/intelli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intelli-0.3.1/setup.py` & `intelli-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("PIPREADME.md", "r", encoding="utf-8") as fh:
     pip_description = fh.read()
 
 setup(
     name="intelli",
-    version="0.3.1",
+    version="0.3.2",
     author="Intellinode",
     author_email="admin@intellinode.ai",
     description="Create chatbots and AI agent workflows. Intelli provide unified layer to connect your data with multiple AI models.",
     long_description=pip_description,
     long_description_content_type="text/markdown",
     url="https://www.intellinode.ai/",
     project_urls={
```

