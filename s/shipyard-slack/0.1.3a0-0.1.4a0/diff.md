# Comparing `tmp/shipyard_slack-0.1.3a0.tar.gz` & `tmp/shipyard_slack-0.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_slack-0.1.3a0.tar", max compression
+gzip compressed data, was "shipyard_slack-0.1.4a0.tar", max compression
```

## Comparing `shipyard_slack-0.1.3a0.tar` & `shipyard_slack-0.1.4a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.842181 shipyard_slack-0.1.3a0/README.md
--rw-r--r--   0        0        0      494 2024-03-06 18:46:05.377840 shipyard_slack-0.1.3a0/pyproject.toml
--rw-r--r--   0        0        0       31 2023-05-12 18:48:21.842512 shipyard_slack-0.1.3a0/shipyard_slack/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.764117 shipyard_slack-0.1.3a0/shipyard_slack/cli/__init__.py
--rw-r--r--   0        0        0      182 2024-01-11 03:34:57.764385 shipyard_slack-0.1.3a0/shipyard_slack/cli/authtest.py
--rw-r--r--   0        0        0     6611 2024-03-06 18:04:17.035912 shipyard_slack-0.1.3a0/shipyard_slack/cli/send_conditional_message.py
--rw-r--r--   0        0        0     4329 2024-03-06 18:45:44.594185 shipyard_slack-0.1.3a0/shipyard_slack/cli/send_message.py
--rw-r--r--   0        0        0     5254 2024-03-06 14:22:56.726126 shipyard_slack-0.1.3a0/shipyard_slack/cli/send_message_with_file.py
--rw-r--r--   0        0        0    10409 2024-03-06 18:41:12.091593 shipyard_slack-0.1.3a0/shipyard_slack/slack.py
--rw-r--r--   0        0        0     5860 2024-02-19 16:47:11.187471 shipyard_slack-0.1.3a0/shipyard_slack/slack_utils.py
--rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 shipyard_slack-0.1.3a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.842181 shipyard_slack-0.1.4a0/README.md
+-rw-r--r--   0        0        0      494 2024-04-02 02:35:46.856951 shipyard_slack-0.1.4a0/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-05-12 18:48:21.842512 shipyard_slack-0.1.4a0/shipyard_slack/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.764117 shipyard_slack-0.1.4a0/shipyard_slack/cli/__init__.py
+-rw-r--r--   0        0        0      182 2024-01-11 03:34:57.764385 shipyard_slack-0.1.4a0/shipyard_slack/cli/authtest.py
+-rw-r--r--   0        0        0     7054 2024-04-02 02:35:20.023020 shipyard_slack-0.1.4a0/shipyard_slack/cli/send_conditional_message.py
+-rw-r--r--   0        0        0     4564 2024-04-02 02:35:20.034021 shipyard_slack-0.1.4a0/shipyard_slack/cli/send_message.py
+-rw-r--r--   0        0        0     5364 2024-04-02 02:35:20.029663 shipyard_slack-0.1.4a0/shipyard_slack/cli/send_message_with_file.py
+-rw-r--r--   0        0        0    10409 2024-03-06 20:41:14.967938 shipyard_slack-0.1.4a0/shipyard_slack/slack.py
+-rw-r--r--   0        0        0     5860 2024-02-19 16:47:11.187471 shipyard_slack-0.1.4a0/shipyard_slack/slack_utils.py
+-rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 shipyard_slack-0.1.4a0/PKG-INFO
```

### Comparing `shipyard_slack-0.1.3a0/shipyard_slack/cli/send_conditional_message.py` & `shipyard_slack-0.1.4a0/shipyard_slack/cli/send_conditional_message.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import argparse
 import os
 import sys
-import argparse
 
-from shipyard_slack import SlackClient
-from shipyard_bp_utils.artifacts import Artifact
 from shipyard_bp_utils import files as file_utils
+from shipyard_bp_utils.artifacts import Artifact
 from shipyard_templates import ShipyardLogger, ExitCodeException, Messaging
+
+from shipyard_slack import SlackClient
 from shipyard_slack.slack_utils import (
     format_user_list,
     create_name_tags,
     send_slack_message_with_file,
 )
 
 BYTE_MAX = 1000000000
@@ -88,15 +89,15 @@
     if args.users_to_notify and not args.user_lookup_method:
         raise ExitCodeException(
             "--users-to-notify requires a --user-lookup-method",
             Messaging.EXIT_CODE_INVALID_INPUT,
         )
 
     if args.file_upload == "yes" and (
-        not args.source_file_name_match_type or not args.source_file_name
+            not args.source_file_name_match_type or not args.source_file_name
     ):
         raise ExitCodeException(
             "--file-upload yes requires --source-file-name and --source-file-name-match-type",
             Messaging.EXIT_CODE_INVALID_INPUT,
         )
 
 
@@ -136,53 +137,59 @@
         elif conditional_send == "file_dne" and upload:
             logger.warning(
                 "File(s) found, but message was conditional based on file not existing. Message not sent."
             )
             sys.exit(0)
         if args.users_to_notify:
             user_id_list = format_user_list(
-                slack_client, args.users_to_notify, args.user_lookup_method
+                slack_client=slack_client, users_to_notify=args.users_to_notify,
+                user_lookup_method=args.user_lookup_method
             )
-            message = create_name_tags(user_id_list) + message
         else:
             user_id_list = []
 
         if args.destination_type == "dm" and file_upload:
             for user_id in user_id_list:
                 logger.info(f"Sending message with file to {user_id}...")
                 response = send_slack_message_with_file(
-                    slack_client, message, upload, user_id, include_in_thread
+                    slack_client=slack_client, message=message, file=upload, channel=user_id,
+                    include_in_thread=include_in_thread
                 )
                 responses.append(response.data)
         elif args.destination_type == "dm" and not file_upload:
             for user_id in user_id_list:
                 logger.info(f"Sending message to {user_id}...")
                 response = slack_client.send_message(
                     message=message, channel_name=user_id
                 )
                 responses.append(response.data)
-        elif file_upload:
+        elif file_upload and args.destination_type == "channel":
             logger.info(f"Sending message with file to {args.channel_name}...")
             response = send_slack_message_with_file(
-                slack_client,
-                message,
-                upload,
-                args.channel_name,
-                include_in_thread,
+                slack_client=slack_client,
+                message=create_name_tags(user_id_list) + message,
+                file=upload,
+                channel=args.channel_name,
+                include_in_thread=include_in_thread,
             )
 
             responses.append(response.data)
 
-        else:
+        elif not file_upload and args.destination_type == "channel":
             logger.info(f"Sending message to {args.channel_name}...")
             response = slack_client.send_message(
                 message=create_name_tags(user_id_list) + message,
                 channel_name=args.channel_name,
             )
             responses.append(response.data)
+        else:
+            raise ExitCodeException(
+                f"Invalid destination type: {args.destination_type}",
+                Messaging.EXIT_CODE_INVALID_INPUT,
+            )
         artifact.responses.write_json(
             os.getenv("SHIPYARD_BLUEPRINT_NAME", "send_conditional_message"), responses
         )
     except ExitCodeException as e:
         logger.error(e.message)
         sys.exit(e.exit_code)
     except Exception as e:
```

### Comparing `shipyard_slack-0.1.3a0/shipyard_slack/cli/send_message.py` & `shipyard_slack-0.1.4a0/shipyard_slack/cli/send_message.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+import argparse
 import os
 import sys
-import json
-import argparse
+
+from shipyard_bp_utils.artifacts import Artifact
+from shipyard_templates import ShipyardLogger, ExitCodeException, Messaging
 
 from shipyard_slack import SlackClient
 from shipyard_slack.slack_utils import create_user_id_list, create_name_tags
-from shipyard_templates import ShipyardLogger, ExitCodeException, Messaging
-from shipyard_bp_utils.artifacts import Artifact
 
 logger = ShipyardLogger().get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument(
@@ -96,35 +96,38 @@
 
         destination_type = args.destination_type
         channel_name = args.channel_name
         message = args.message
 
         if args.users_to_notify:
             user_id_list = create_user_id_list(
-                slack_client, args.users_to_notify, args.user_lookup_method
+                slack_client=slack_client, users_to_notify=args.users_to_notify,
+                user_lookup_method=args.user_lookup_method
             )
-            message = create_name_tags(user_id_list) + message
-
         else:
             user_id_list = []
 
         if destination_type == "dm":
             for user_id in user_id_list:
                 response = slack_client.send_message(
                     message=message, channel_name=user_id
                 )
                 responses.append(response.data)
 
-        else:
+        elif destination_type == "channel":
             response = slack_client.send_message(
-                message=message,
+                message=create_name_tags(user_id_list) + message,
                 channel_name=channel_name,
             )
             responses.append(response.data)
-
+        else:
+            raise ExitCodeException(
+                f"Invalid destination type: {destination_type}",
+                slack_client.EXIT_CODE_INVALID_INPUT,
+            )
         artifact.responses.write_json(
             os.getenv("SHIPYARD_BLUEPRINT_NAME", "send_message"), responses
         )
 
     except ExitCodeException as e:
         logger.error(e)
         sys.exit(e.exit_code)
```

### Comparing `shipyard_slack-0.1.3a0/shipyard_slack/cli/send_message_with_file.py` & `shipyard_slack-0.1.4a0/shipyard_slack/cli/send_message_with_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import argparse
 import os
 import sys
-import argparse
 
-from shipyard_slack import SlackClient
-from shipyard_bp_utils.artifacts import Artifact
 from shipyard_bp_utils import files as file_utils
+from shipyard_bp_utils.artifacts import Artifact
 from shipyard_templates import ShipyardLogger, ExitCodeException, Messaging
+
+from shipyard_slack import SlackClient
 from shipyard_slack.slack_utils import (
     format_user_list,
     create_name_tags,
     send_slack_message_with_file,
 )
 
 BYTE_MAX = 1000000000
@@ -123,32 +124,31 @@
                 f"No files found with name {args.source_file_name}",
                 slack_client.EXIT_CODE_FILE_NOT_FOUND,
             )
         if args.users_to_notify:
             user_id_list = format_user_list(
                 slack_client, args.users_to_notify, args.user_lookup_method
             )
-            message = create_name_tags(user_id_list) + message
         else:
             user_id_list = []
 
         if args.destination_type == "dm":
             for user_id in user_id_list:
                 response = send_slack_message_with_file(
-                    slack_client, message, upload, user_id, include_in_thread
+                    slack_client=slack_client, message=message, file=upload, channel=user_id, include_in_thread=include_in_thread
                 )
                 responses.append(response.data)
 
-        else:
+        elif args.destination_type == "channel":
             response = send_slack_message_with_file(
-                slack_client,
-                message,
-                upload,
-                args.channel_name,
-                include_in_thread,
+                slack_client=slack_client,
+                message=create_name_tags(user_id_list) + message,
+                file=upload,
+                channel=args.channel_name,
+                include_in_thread=include_in_thread,
             )
             responses.append(response.data)
 
         artifact.responses.write_json(
             os.getenv("SHIPYARD_BLUEPRINT_NAME", "send_message_with_file"), responses
         )
     except ExitCodeException as e:
```

### Comparing `shipyard_slack-0.1.3a0/shipyard_slack/slack.py` & `shipyard_slack-0.1.4a0/shipyard_slack/slack.py`

 * *Files identical despite different names*

### Comparing `shipyard_slack-0.1.3a0/shipyard_slack/slack_utils.py` & `shipyard_slack-0.1.4a0/shipyard_slack/slack_utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_slack-0.1.3a0/PKG-INFO` & `shipyard_slack-0.1.4a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-slack
-Version: 0.1.3a0
+Version: 0.1.4a0
 Summary: A local client for connecting and working with Slack
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

