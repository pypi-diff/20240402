# Comparing `tmp/shipyard_slack-0.1.4a0.tar.gz` & `tmp/shipyard_slack-0.1.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_slack-0.1.4a0.tar", max compression
+gzip compressed data, was "shipyard_slack-0.1.4a1.tar", max compression
```

## Comparing `shipyard_slack-0.1.4a0.tar` & `shipyard_slack-0.1.4a1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.842181 shipyard_slack-0.1.4a0/README.md
--rw-r--r--   0        0        0      494 2024-04-02 02:35:46.856951 shipyard_slack-0.1.4a0/pyproject.toml
--rw-r--r--   0        0        0       31 2023-05-12 18:48:21.842512 shipyard_slack-0.1.4a0/shipyard_slack/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.764117 shipyard_slack-0.1.4a0/shipyard_slack/cli/__init__.py
--rw-r--r--   0        0        0      182 2024-01-11 03:34:57.764385 shipyard_slack-0.1.4a0/shipyard_slack/cli/authtest.py
--rw-r--r--   0        0        0     7054 2024-04-02 02:35:20.023020 shipyard_slack-0.1.4a0/shipyard_slack/cli/send_conditional_message.py
--rw-r--r--   0        0        0     4564 2024-04-02 02:35:20.034021 shipyard_slack-0.1.4a0/shipyard_slack/cli/send_message.py
--rw-r--r--   0        0        0     5364 2024-04-02 02:35:20.029663 shipyard_slack-0.1.4a0/shipyard_slack/cli/send_message_with_file.py
--rw-r--r--   0        0        0    10409 2024-03-06 20:41:14.967938 shipyard_slack-0.1.4a0/shipyard_slack/slack.py
--rw-r--r--   0        0        0     5860 2024-02-19 16:47:11.187471 shipyard_slack-0.1.4a0/shipyard_slack/slack_utils.py
--rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 shipyard_slack-0.1.4a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.842181 shipyard_slack-0.1.4a1/README.md
+-rw-r--r--   0        0        0      494 2024-04-02 03:18:14.819226 shipyard_slack-0.1.4a1/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-05-12 18:48:21.842512 shipyard_slack-0.1.4a1/shipyard_slack/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.764117 shipyard_slack-0.1.4a1/shipyard_slack/cli/__init__.py
+-rw-r--r--   0        0        0      182 2024-01-11 03:34:57.764385 shipyard_slack-0.1.4a1/shipyard_slack/cli/authtest.py
+-rw-r--r--   0        0        0     7054 2024-04-02 02:35:20.023020 shipyard_slack-0.1.4a1/shipyard_slack/cli/send_conditional_message.py
+-rw-r--r--   0        0        0     4564 2024-04-02 02:35:20.034021 shipyard_slack-0.1.4a1/shipyard_slack/cli/send_message.py
+-rw-r--r--   0        0        0     5384 2024-04-02 03:18:00.189089 shipyard_slack-0.1.4a1/shipyard_slack/cli/send_message_with_file.py
+-rw-r--r--   0        0        0    10409 2024-03-06 20:41:14.967938 shipyard_slack-0.1.4a1/shipyard_slack/slack.py
+-rw-r--r--   0        0        0     5860 2024-02-19 16:47:11.187471 shipyard_slack-0.1.4a1/shipyard_slack/slack_utils.py
+-rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 shipyard_slack-0.1.4a1/PKG-INFO
```

### Comparing `shipyard_slack-0.1.4a0/shipyard_slack/cli/send_conditional_message.py` & `shipyard_slack-0.1.4a1/shipyard_slack/cli/send_conditional_message.py`

 * *Files identical despite different names*

### Comparing `shipyard_slack-0.1.4a0/shipyard_slack/cli/send_message.py` & `shipyard_slack-0.1.4a1/shipyard_slack/cli/send_message.py`

 * *Files identical despite different names*

### Comparing `shipyard_slack-0.1.4a0/shipyard_slack/cli/send_message_with_file.py` & `shipyard_slack-0.1.4a1/shipyard_slack/cli/send_message_with_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,16 @@
             )
         else:
             user_id_list = []
 
         if args.destination_type == "dm":
             for user_id in user_id_list:
                 response = send_slack_message_with_file(
-                    slack_client=slack_client, message=message, file=upload, channel=user_id, include_in_thread=include_in_thread
+                    slack_client=slack_client, message=message, file=upload, channel=user_id,
+                    include_in_thread=include_in_thread
                 )
                 responses.append(response.data)
 
         elif args.destination_type == "channel":
             response = send_slack_message_with_file(
                 slack_client=slack_client,
                 message=create_name_tags(user_id_list) + message,
```

### Comparing `shipyard_slack-0.1.4a0/shipyard_slack/slack.py` & `shipyard_slack-0.1.4a1/shipyard_slack/slack.py`

 * *Files identical despite different names*

### Comparing `shipyard_slack-0.1.4a0/shipyard_slack/slack_utils.py` & `shipyard_slack-0.1.4a1/shipyard_slack/slack_utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_slack-0.1.4a0/PKG-INFO` & `shipyard_slack-0.1.4a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-slack
-Version: 0.1.4a0
+Version: 0.1.4a1
 Summary: A local client for connecting and working with Slack
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

