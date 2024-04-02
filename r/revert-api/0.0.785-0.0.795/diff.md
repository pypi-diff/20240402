# Comparing `tmp/revert_api-0.0.785.tar.gz` & `tmp/revert_api-0.0.795.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revert_api-0.0.785.tar", max compression
+gzip compressed data, was "revert_api-0.0.795.tar", max compression
```

## Comparing `revert_api-0.0.785.tar` & `revert_api-0.0.795.tar`

### file list

```diff
@@ -1,234 +1,234 @@
--rw-r--r--   0        0        0     1688 2024-03-26 16:49:38.204271 revert_api-0.0.785/README.md
--rw-r--r--   0        0        0      404 2024-03-26 16:49:38.204271 revert_api-0.0.785/pyproject.toml
--rw-r--r--   0        0        0     1767 2024-03-26 16:49:38.204271 revert_api-0.0.785/src/revert/__init__.py
--rw-r--r--   0        0        0     2971 2024-03-26 16:49:38.204271 revert_api-0.0.785/src/revert/client.py
--rw-r--r--   0        0        0      519 2024-03-26 16:49:38.204271 revert_api-0.0.785/src/revert/core/__init__.py
--rw-r--r--   0        0        0      426 2024-03-26 16:49:38.204271 revert_api-0.0.785/src/revert/core/api_error.py
--rw-r--r--   0        0        0      930 2024-03-26 16:49:38.204271 revert_api-0.0.785/src/revert/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-03-26 16:49:38.204271 revert_api-0.0.785/src/revert/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      310 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/environment.py
--rw-r--r--   0        0        0        0 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/py.typed
--rw-r--r--   0        0        0     1725 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/__init__.py
--rw-r--r--   0        0        0      431 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/__init__.py
--rw-r--r--   0        0        0     1075 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/client.py
--rw-r--r--   0        0        0      449 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/__init__.py
--rw-r--r--   0        0        0      139 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/channels/__init__.py
--rw-r--r--   0        0        0     5785 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/channels/client.py
--rw-r--r--   0        0        0      155 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/channels/types/__init__.py
--rw-r--r--   0        0        0     1134 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/channels/types/get_channels_response.py
--rw-r--r--   0        0        0      221 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/messages/__init__.py
--rw-r--r--   0        0        0     5982 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/messages/client.py
--rw-r--r--   0        0        0      292 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/messages/types/__init__.py
--rw-r--r--   0        0        0      860 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/messages/types/createor_update_message_request.py
--rw-r--r--   0        0        0     1064 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/messages/types/createor_update_message_response.py
--rw-r--r--   0        0        0      133 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/users/__init__.py
--rw-r--r--   0        0        0     5743 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/users/client.py
--rw-r--r--   0        0        0      146 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/users/types/__init__.py
--rw-r--r--   0        0        0     1135 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/chat/resources/users/types/get_users_response.py
--rw-r--r--   0        0        0     1969 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/__init__.py
--rw-r--r--   0        0        0     2016 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/__init__.py
--rw-r--r--   0        0        0      381 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/associations/__init__.py
--rw-r--r--   0        0        0      515 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/associations/types/__init__.py
--rw-r--r--   0        0        0     1190 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/associations/types/company_association.py
--rw-r--r--   0        0        0     1341 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/associations/types/contact_association.py
--rw-r--r--   0        0        0     1327 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/associations/types/deal_association.py
--rw-r--r--   0        0        0     1378 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/associations/types/event_association.py
--rw-r--r--   0        0        0     1506 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/associations/types/lead_association.py
--rw-r--r--   0        0        0     1185 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/associations/types/task_association.py
--rw-r--r--   0        0        0      290 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/errors/__init__.py
--rw-r--r--   0        0        0      353 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/errors/errors/__init__.py
--rw-r--r--   0        0        0      277 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/errors/errors/bad_request_error.py
--rw-r--r--   0        0        0      281 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/errors/errors/internal_server_error.py
--rw-r--r--   0        0        0      275 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/errors/errors/not_found_error.py
--rw-r--r--   0        0        0      279 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/errors/errors/un_authorized_error.py
--rw-r--r--   0        0        0      124 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/errors/types/__init__.py
--rw-r--r--   0        0        0      871 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/errors/types/base_error.py
--rw-r--r--   0        0        0      437 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/types/__init__.py
--rw-r--r--   0        0        0      607 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/types/types/__init__.py
--rw-r--r--   0        0        0     1308 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/types/types/account.py
--rw-r--r--   0        0        0     1420 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/types/types/app.py
--rw-r--r--   0        0        0      926 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/types/types/app_config.py
--rw-r--r--   0        0        0     1300 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/types/types/connection.py
--rw-r--r--   0        0        0      441 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/types/types/response_status.py
--rw-r--r--   0        0        0     1155 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/types/types/revert_user.py
--rw-r--r--   0        0        0     1286 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/types/types/standard_object.py
--rw-r--r--   0        0        0      889 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/types/types/ticket_priority.py
--rw-r--r--   0        0        0      638 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/types/types/ticket_status.py
--rw-r--r--   0        0        0     1207 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/types/types/tpid.py
--rw-r--r--   0        0        0     1021 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/__init__.py
--rw-r--r--   0        0        0     1537 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/__init__.py
--rw-r--r--   0        0        0     1213 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/channel.py
--rw-r--r--   0        0        0     1123 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/comment_ticket_write.py
--rw-r--r--   0        0        0     1594 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/common_unified_fields.py
--rw-r--r--   0        0        0     1729 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/company.py
--rw-r--r--   0        0        0     1057 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/company_address.py
--rw-r--r--   0        0        0      893 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/contact.py
--rw-r--r--   0        0        0     1294 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/contact_read.py
--rw-r--r--   0        0        0      950 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/contact_write.py
--rw-r--r--   0        0        0      881 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/deal.py
--rw-r--r--   0        0        0     1742 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/deal_read.py
--rw-r--r--   0        0        0      929 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/deal_write.py
--rw-r--r--   0        0        0      885 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/event.py
--rw-r--r--   0        0        0     1588 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/event_read.py
--rw-r--r--   0        0        0      936 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/event_write.py
--rw-r--r--   0        0        0      881 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/lead.py
--rw-r--r--   0        0        0     1279 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/lead_read.py
--rw-r--r--   0        0        0      929 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/lead_write.py
--rw-r--r--   0        0        0     1078 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/message.py
--rw-r--r--   0        0        0      881 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/note.py
--rw-r--r--   0        0        0      952 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/note_read.py
--rw-r--r--   0        0        0      929 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/note_write.py
--rw-r--r--   0        0        0      881 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/task.py
--rw-r--r--   0        0        0     1345 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/task_read.py
--rw-r--r--   0        0        0      909 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/task_ticket.py
--rw-r--r--   0        0        0     1912 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/task_ticket_write.py
--rw-r--r--   0        0        0      974 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/task_write.py
--rw-r--r--   0        0        0      884 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/user.py
--rw-r--r--   0        0        0     1231 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/user_chat.py
--rw-r--r--   0        0        0     1408 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/common/resources/unified/types/user_write.py
--rw-r--r--   0        0        0      687 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/connection/__init__.py
--rw-r--r--   0        0        0    29807 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/connection/client.py
--rw-r--r--   0        0        0      997 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/connection/types/__init__.py
--rw-r--r--   0        0        0      477 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/connection/types/connection_status.py
--rw-r--r--   0        0        0      979 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/connection/types/create_connection_webhook_request.py
--rw-r--r--   0        0        0     1272 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/connection/types/create_connection_webhook_response.py
--rw-r--r--   0        0        0     1061 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/connection/types/delete_connection_response.py
--rw-r--r--   0        0        0     1142 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/connection/types/delete_connection_webhook_response.py
--rw-r--r--   0        0        0      198 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/connection/types/get_all_connection_response.py
--rw-r--r--   0        0        0     1264 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/connection/types/get_connect_status_response.py
--rw-r--r--   0        0        0      889 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/connection/types/get_connection_response.py
--rw-r--r--   0        0        0     1163 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/connection/types/get_connection_webhook_response.py
--rw-r--r--   0        0        0     3061 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/__init__.py
--rw-r--r--   0        0        0     2536 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/client.py
--rw-r--r--   0        0        0     3207 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/__init__.py
--rw-r--r--   0        0        0      409 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/company/__init__.py
--rw-r--r--   0        0        0    23881 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/company/client.py
--rw-r--r--   0        0        0      563 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/company/types/__init__.py
--rw-r--r--   0        0        0     1007 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/company/types/create_or_update_company_request.py
--rw-r--r--   0        0        0     1020 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/company/types/create_or_update_company_response.py
--rw-r--r--   0        0        0     1135 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/company/types/get_companies_response.py
--rw-r--r--   0        0        0     1053 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/company/types/get_company_response.py
--rw-r--r--   0        0        0     1072 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/company/types/search_companies_response.py
--rw-r--r--   0        0        0      405 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/contact/__init__.py
--rw-r--r--   0        0        0    24439 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/contact/client.py
--rw-r--r--   0        0        0      557 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/contact/types/__init__.py
--rw-r--r--   0        0        0     1145 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/contact/types/create_or_update_contact_request.py
--rw-r--r--   0        0        0     1020 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/contact/types/create_or_update_contact_response.py
--rw-r--r--   0        0        0     1053 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/contact/types/get_contact_response.py
--rw-r--r--   0        0        0     1134 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/contact/types/get_contacts_response.py
--rw-r--r--   0        0        0     1071 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/contact/types/search_contacts_response.py
--rw-r--r--   0        0        0      375 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/deal/__init__.py
--rw-r--r--   0        0        0    23576 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/deal/client.py
--rw-r--r--   0        0        0      512 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/deal/types/__init__.py
--rw-r--r--   0        0        0     1133 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/deal/types/create_or_update_deal_request.py
--rw-r--r--   0        0        0     1017 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/deal/types/create_or_update_deal_response.py
--rw-r--r--   0        0        0     1041 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/deal/types/get_deal_response.py
--rw-r--r--   0        0        0     1122 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/deal/types/get_deals_response.py
--rw-r--r--   0        0        0     1059 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/deal/types/search_deals_response.py
--rw-r--r--   0        0        0      437 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/event/__init__.py
--rw-r--r--   0        0        0    27691 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/event/client.py
--rw-r--r--   0        0        0      609 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/event/types/__init__.py
--rw-r--r--   0        0        0     1137 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/event/types/create_or_update_event_request.py
--rw-r--r--   0        0        0     1018 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/event/types/create_or_update_event_response.py
--rw-r--r--   0        0        0      987 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/event/types/delete_event_response.py
--rw-r--r--   0        0        0     1045 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/event/types/get_event_response.py
--rw-r--r--   0        0        0     1126 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/event/types/get_events_response.py
--rw-r--r--   0        0        0     1063 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/event/types/search_events_response.py
--rw-r--r--   0        0        0      375 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/lead/__init__.py
--rw-r--r--   0        0        0    23576 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/lead/client.py
--rw-r--r--   0        0        0      512 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/lead/types/__init__.py
--rw-r--r--   0        0        0     1133 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/lead/types/create_or_update_lead_request.py
--rw-r--r--   0        0        0     1017 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/lead/types/create_or_update_lead_response.py
--rw-r--r--   0        0        0     1041 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/lead/types/get_lead_response.py
--rw-r--r--   0        0        0     1122 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/lead/types/get_leads_response.py
--rw-r--r--   0        0        0     1059 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/lead/types/search_leads_response.py
--rw-r--r--   0        0        0      375 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/note/__init__.py
--rw-r--r--   0        0        0    23576 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/note/client.py
--rw-r--r--   0        0        0      512 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/note/types/__init__.py
--rw-r--r--   0        0        0     1133 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/note/types/create_or_update_note_request.py
--rw-r--r--   0        0        0     1017 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/note/types/create_or_update_note_response.py
--rw-r--r--   0        0        0     1041 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/note/types/get_note_response.py
--rw-r--r--   0        0        0     1122 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/note/types/get_notes_response.py
--rw-r--r--   0        0        0     1059 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/note/types/search_notes_response.py
--rw-r--r--   0        0        0      465 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/properties/__init__.py
--rw-r--r--   0        0        0    10251 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/properties/client.py
--rw-r--r--   0        0        0      652 2024-03-26 16:49:38.208272 revert_api-0.0.785/src/revert/resources/crm/resources/properties/types/__init__.py
--rw-r--r--   0        0        0      912 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/properties/types/field_details_type.py
--rw-r--r--   0        0        0     1026 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/properties/types/field_details_type_read.py
--rw-r--r--   0        0        0     1118 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/properties/types/field_details_type_request.py
--rw-r--r--   0        0        0      203 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/properties/types/get_object_properties_response.py
--rw-r--r--   0        0        0      183 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/properties/types/set_object_properties_request.py
--rw-r--r--   0        0        0      121 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/properties/types/set_object_properties_response.py
--rw-r--r--   0        0        0      173 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/proxy/__init__.py
--rw-r--r--   0        0        0     5499 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/proxy/client.py
--rw-r--r--   0        0        0      218 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/proxy/types/__init__.py
--rw-r--r--   0        0        0     1065 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/proxy/types/post_proxy_request_body.py
--rw-r--r--   0        0        0      883 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/proxy/types/proxy_response.py
--rw-r--r--   0        0        0      375 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/task/__init__.py
--rw-r--r--   0        0        0    23576 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/task/client.py
--rw-r--r--   0        0        0      512 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/task/types/__init__.py
--rw-r--r--   0        0        0     1133 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/task/types/create_or_update_task_request.py
--rw-r--r--   0        0        0     1017 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/task/types/create_or_update_task_response.py
--rw-r--r--   0        0        0     1041 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/task/types/get_task_response.py
--rw-r--r--   0        0        0     1122 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/task/types/get_tasks_response.py
--rw-r--r--   0        0        0     1059 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/task/types/search_tasks_response.py
--rw-r--r--   0        0        0      283 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/user/__init__.py
--rw-r--r--   0        0        0    14641 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/user/client.py
--rw-r--r--   0        0        0      411 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/user/types/__init__.py
--rw-r--r--   0        0        0     1133 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/user/types/create_or_update_user_request.py
--rw-r--r--   0        0        0     1017 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/user/types/create_or_update_user_response.py
--rw-r--r--   0        0        0     1041 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/user/types/get_user_response.py
--rw-r--r--   0        0        0     1122 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/crm/resources/user/types/get_users_response.py
--rw-r--r--   0        0        0      793 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/field_mapping/__init__.py
--rw-r--r--   0        0        0    22972 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/field_mapping/client.py
--rw-r--r--   0        0        0     1170 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/field_mapping/types/__init__.py
--rw-r--r--   0        0        0     1052 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/field_mapping/types/create_account_field_mapping_request_body.py
--rw-r--r--   0        0        0      980 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/field_mapping/types/create_account_field_mapping_response.py
--rw-r--r--   0        0        0     1157 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/field_mapping/types/create_field_mapping_request_body.py
--rw-r--r--   0        0        0      973 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/field_mapping/types/create_field_mapping_response.py
--rw-r--r--   0        0        0      986 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/field_mapping/types/delete_account_field_mapping_config_response.py
--rw-r--r--   0        0        0      990 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/field_mapping/types/delete_field_mapping_response.py
--rw-r--r--   0        0        0     1061 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/field_mapping/types/field_mapping_type.py
--rw-r--r--   0        0        0     1206 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/field_mapping/types/get_field_mapping_config_response.py
--rw-r--r--   0        0        0     1054 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/field_mapping/types/get_field_mappings_response.py
--rw-r--r--   0        0        0     1108 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/field_mapping/types/mappable_field_type.py
--rw-r--r--   0        0        0      191 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/metadata/__init__.py
--rw-r--r--   0        0        0     3656 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/metadata/client.py
--rw-r--r--   0        0        0      255 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/metadata/types/__init__.py
--rw-r--r--   0        0        0     1190 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/metadata/types/crm_metadata.py
--rw-r--r--   0        0        0      985 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/metadata/types/crm_metadata_response.py
--rw-r--r--   0        0        0      461 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/metadata/types/crm_status.py
--rw-r--r--   0        0        0      943 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/__init__.py
--rw-r--r--   0        0        0     1494 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/client.py
--rw-r--r--   0        0        0      973 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/__init__.py
--rw-r--r--   0        0        0      145 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/collection/__init__.py
--rw-r--r--   0        0        0     5829 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/collection/client.py
--rw-r--r--   0        0        0      164 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/collection/types/__init__.py
--rw-r--r--   0        0        0     1063 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/collection/types/get_collections_response.py
--rw-r--r--   0        0        0      307 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/comment/__init__.py
--rw-r--r--   0        0        0    19749 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/comment/client.py
--rw-r--r--   0        0        0      447 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/comment/types/__init__.py
--rw-r--r--   0        0        0      204 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/comment/types/create_or_update_comment_request.py
--rw-r--r--   0        0        0     1020 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/comment/types/create_or_update_comment_response.py
--rw-r--r--   0        0        0      992 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/comment/types/get_comment_response.py
--rw-r--r--   0        0        0     1060 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/comment/types/get_comments_response.py
--rw-r--r--   0        0        0      173 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/proxy/__init__.py
--rw-r--r--   0        0        0     5529 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/proxy/client.py
--rw-r--r--   0        0        0      218 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/proxy/types/__init__.py
--rw-r--r--   0        0        0     1065 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/proxy/types/post_proxy_request_body.py
--rw-r--r--   0        0        0      883 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/proxy/types/proxy_response.py
--rw-r--r--   0        0        0      283 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/task/__init__.py
--rw-r--r--   0        0        0    19908 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/task/client.py
--rw-r--r--   0        0        0      411 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/task/types/__init__.py
--rw-r--r--   0        0        0      192 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/task/types/create_or_update_task_request.py
--rw-r--r--   0        0        0     1017 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/task/types/create_or_update_task_response.py
--rw-r--r--   0        0        0     1060 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/task/types/get_task_response.py
--rw-r--r--   0        0        0     1141 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/task/types/get_tasks_response.py
--rw-r--r--   0        0        0      169 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/user/__init__.py
--rw-r--r--   0        0        0    10114 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/user/client.py
--rw-r--r--   0        0        0      212 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/user/types/__init__.py
--rw-r--r--   0        0        0      989 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/user/types/get_user_response.py
--rw-r--r--   0        0        0     1057 2024-03-26 16:49:38.212272 revert_api-0.0.785/src/revert/resources/ticket/resources/user/types/get_users_response.py
--rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 revert_api-0.0.785/PKG-INFO
+-rw-r--r--   0        0        0     1688 2024-04-02 08:45:32.002374 revert_api-0.0.795/README.md
+-rw-r--r--   0        0        0      404 2024-04-02 08:45:32.002374 revert_api-0.0.795/pyproject.toml
+-rw-r--r--   0        0        0     1767 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/__init__.py
+-rw-r--r--   0        0        0     2971 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/client.py
+-rw-r--r--   0        0        0      519 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/core/api_error.py
+-rw-r--r--   0        0        0      930 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      310 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/environment.py
+-rw-r--r--   0        0        0        0 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/py.typed
+-rw-r--r--   0        0        0     1725 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/__init__.py
+-rw-r--r--   0        0        0      431 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/__init__.py
+-rw-r--r--   0        0        0     1075 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/client.py
+-rw-r--r--   0        0        0      449 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/channels/__init__.py
+-rw-r--r--   0        0        0     5785 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/channels/client.py
+-rw-r--r--   0        0        0      155 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/channels/types/__init__.py
+-rw-r--r--   0        0        0     1134 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/channels/types/get_channels_response.py
+-rw-r--r--   0        0        0      221 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/messages/__init__.py
+-rw-r--r--   0        0        0     5982 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/messages/client.py
+-rw-r--r--   0        0        0      292 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/messages/types/__init__.py
+-rw-r--r--   0        0        0      860 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/messages/types/createor_update_message_request.py
+-rw-r--r--   0        0        0     1064 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/messages/types/createor_update_message_response.py
+-rw-r--r--   0        0        0      133 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/users/__init__.py
+-rw-r--r--   0        0        0     5743 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/users/client.py
+-rw-r--r--   0        0        0      146 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/users/types/__init__.py
+-rw-r--r--   0        0        0     1135 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/chat/resources/users/types/get_users_response.py
+-rw-r--r--   0        0        0     1969 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/__init__.py
+-rw-r--r--   0        0        0     2016 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/__init__.py
+-rw-r--r--   0        0        0      381 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/associations/__init__.py
+-rw-r--r--   0        0        0      515 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/associations/types/__init__.py
+-rw-r--r--   0        0        0     1190 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/associations/types/company_association.py
+-rw-r--r--   0        0        0     1341 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/associations/types/contact_association.py
+-rw-r--r--   0        0        0     1327 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/associations/types/deal_association.py
+-rw-r--r--   0        0        0     1378 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/associations/types/event_association.py
+-rw-r--r--   0        0        0     1506 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/associations/types/lead_association.py
+-rw-r--r--   0        0        0     1185 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/associations/types/task_association.py
+-rw-r--r--   0        0        0      290 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/errors/__init__.py
+-rw-r--r--   0        0        0      353 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/errors/errors/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/errors/errors/bad_request_error.py
+-rw-r--r--   0        0        0      281 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/errors/errors/internal_server_error.py
+-rw-r--r--   0        0        0      275 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/errors/errors/not_found_error.py
+-rw-r--r--   0        0        0      279 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/errors/errors/un_authorized_error.py
+-rw-r--r--   0        0        0      124 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/errors/types/__init__.py
+-rw-r--r--   0        0        0      871 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/errors/types/base_error.py
+-rw-r--r--   0        0        0      437 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/types/__init__.py
+-rw-r--r--   0        0        0      607 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/types/types/__init__.py
+-rw-r--r--   0        0        0     1308 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/types/types/account.py
+-rw-r--r--   0        0        0     1420 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/types/types/app.py
+-rw-r--r--   0        0        0      926 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/types/types/app_config.py
+-rw-r--r--   0        0        0     1300 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/types/types/connection.py
+-rw-r--r--   0        0        0      441 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/types/types/response_status.py
+-rw-r--r--   0        0        0     1155 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/types/types/revert_user.py
+-rw-r--r--   0        0        0     1286 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/types/types/standard_object.py
+-rw-r--r--   0        0        0      889 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/types/types/ticket_priority.py
+-rw-r--r--   0        0        0      638 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/types/types/ticket_status.py
+-rw-r--r--   0        0        0     1207 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/types/types/tpid.py
+-rw-r--r--   0        0        0     1021 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/__init__.py
+-rw-r--r--   0        0        0     1537 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/__init__.py
+-rw-r--r--   0        0        0     1213 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/channel.py
+-rw-r--r--   0        0        0     1123 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/comment_ticket_write.py
+-rw-r--r--   0        0        0     1594 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/common_unified_fields.py
+-rw-r--r--   0        0        0     1729 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/company.py
+-rw-r--r--   0        0        0     1057 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/company_address.py
+-rw-r--r--   0        0        0      893 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/contact.py
+-rw-r--r--   0        0        0     1294 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/contact_read.py
+-rw-r--r--   0        0        0      950 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/contact_write.py
+-rw-r--r--   0        0        0      881 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/deal.py
+-rw-r--r--   0        0        0     1742 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/deal_read.py
+-rw-r--r--   0        0        0      929 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/deal_write.py
+-rw-r--r--   0        0        0      885 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/event.py
+-rw-r--r--   0        0        0     1588 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/event_read.py
+-rw-r--r--   0        0        0      936 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/event_write.py
+-rw-r--r--   0        0        0      881 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/lead.py
+-rw-r--r--   0        0        0     1279 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/lead_read.py
+-rw-r--r--   0        0        0      929 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/lead_write.py
+-rw-r--r--   0        0        0     1078 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/message.py
+-rw-r--r--   0        0        0      881 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/note.py
+-rw-r--r--   0        0        0      952 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/note_read.py
+-rw-r--r--   0        0        0      929 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/note_write.py
+-rw-r--r--   0        0        0      881 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/task.py
+-rw-r--r--   0        0        0     1345 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/task_read.py
+-rw-r--r--   0        0        0      909 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/task_ticket.py
+-rw-r--r--   0        0        0     1912 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/task_ticket_write.py
+-rw-r--r--   0        0        0      974 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/task_write.py
+-rw-r--r--   0        0        0      884 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/user.py
+-rw-r--r--   0        0        0     1231 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/user_chat.py
+-rw-r--r--   0        0        0     1408 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/common/resources/unified/types/user_write.py
+-rw-r--r--   0        0        0      687 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/connection/__init__.py
+-rw-r--r--   0        0        0    29807 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/connection/client.py
+-rw-r--r--   0        0        0      997 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/connection/types/__init__.py
+-rw-r--r--   0        0        0      477 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/connection/types/connection_status.py
+-rw-r--r--   0        0        0      979 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/connection/types/create_connection_webhook_request.py
+-rw-r--r--   0        0        0     1272 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/connection/types/create_connection_webhook_response.py
+-rw-r--r--   0        0        0     1061 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/connection/types/delete_connection_response.py
+-rw-r--r--   0        0        0     1142 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/connection/types/delete_connection_webhook_response.py
+-rw-r--r--   0        0        0      198 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/connection/types/get_all_connection_response.py
+-rw-r--r--   0        0        0     1264 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/connection/types/get_connect_status_response.py
+-rw-r--r--   0        0        0      889 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/connection/types/get_connection_response.py
+-rw-r--r--   0        0        0     1163 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/connection/types/get_connection_webhook_response.py
+-rw-r--r--   0        0        0     3061 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/__init__.py
+-rw-r--r--   0        0        0     2536 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/client.py
+-rw-r--r--   0        0        0     3207 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/company/__init__.py
+-rw-r--r--   0        0        0    23881 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/company/client.py
+-rw-r--r--   0        0        0      563 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/company/types/__init__.py
+-rw-r--r--   0        0        0     1007 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/company/types/create_or_update_company_request.py
+-rw-r--r--   0        0        0     1020 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/company/types/create_or_update_company_response.py
+-rw-r--r--   0        0        0     1135 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/company/types/get_companies_response.py
+-rw-r--r--   0        0        0     1053 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/company/types/get_company_response.py
+-rw-r--r--   0        0        0     1072 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/company/types/search_companies_response.py
+-rw-r--r--   0        0        0      405 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/contact/__init__.py
+-rw-r--r--   0        0        0    24439 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/contact/client.py
+-rw-r--r--   0        0        0      557 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/contact/types/__init__.py
+-rw-r--r--   0        0        0     1145 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/contact/types/create_or_update_contact_request.py
+-rw-r--r--   0        0        0     1020 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/contact/types/create_or_update_contact_response.py
+-rw-r--r--   0        0        0     1053 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/contact/types/get_contact_response.py
+-rw-r--r--   0        0        0     1134 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/contact/types/get_contacts_response.py
+-rw-r--r--   0        0        0     1071 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/contact/types/search_contacts_response.py
+-rw-r--r--   0        0        0      375 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/deal/__init__.py
+-rw-r--r--   0        0        0    23576 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/deal/client.py
+-rw-r--r--   0        0        0      512 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/deal/types/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/deal/types/create_or_update_deal_request.py
+-rw-r--r--   0        0        0     1017 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/deal/types/create_or_update_deal_response.py
+-rw-r--r--   0        0        0     1041 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/deal/types/get_deal_response.py
+-rw-r--r--   0        0        0     1122 2024-04-02 08:45:32.002374 revert_api-0.0.795/src/revert/resources/crm/resources/deal/types/get_deals_response.py
+-rw-r--r--   0        0        0     1059 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/deal/types/search_deals_response.py
+-rw-r--r--   0        0        0      437 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/event/__init__.py
+-rw-r--r--   0        0        0    27691 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/event/client.py
+-rw-r--r--   0        0        0      609 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/event/types/__init__.py
+-rw-r--r--   0        0        0     1137 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/event/types/create_or_update_event_request.py
+-rw-r--r--   0        0        0     1018 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/event/types/create_or_update_event_response.py
+-rw-r--r--   0        0        0      987 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/event/types/delete_event_response.py
+-rw-r--r--   0        0        0     1045 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/event/types/get_event_response.py
+-rw-r--r--   0        0        0     1126 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/event/types/get_events_response.py
+-rw-r--r--   0        0        0     1063 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/event/types/search_events_response.py
+-rw-r--r--   0        0        0      375 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/lead/__init__.py
+-rw-r--r--   0        0        0    23576 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/lead/client.py
+-rw-r--r--   0        0        0      512 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/lead/types/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/lead/types/create_or_update_lead_request.py
+-rw-r--r--   0        0        0     1017 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/lead/types/create_or_update_lead_response.py
+-rw-r--r--   0        0        0     1041 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/lead/types/get_lead_response.py
+-rw-r--r--   0        0        0     1122 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/lead/types/get_leads_response.py
+-rw-r--r--   0        0        0     1059 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/lead/types/search_leads_response.py
+-rw-r--r--   0        0        0      375 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/note/__init__.py
+-rw-r--r--   0        0        0    23576 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/note/client.py
+-rw-r--r--   0        0        0      512 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/note/types/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/note/types/create_or_update_note_request.py
+-rw-r--r--   0        0        0     1017 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/note/types/create_or_update_note_response.py
+-rw-r--r--   0        0        0     1041 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/note/types/get_note_response.py
+-rw-r--r--   0        0        0     1122 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/note/types/get_notes_response.py
+-rw-r--r--   0        0        0     1059 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/note/types/search_notes_response.py
+-rw-r--r--   0        0        0      465 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/properties/__init__.py
+-rw-r--r--   0        0        0    10251 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/properties/client.py
+-rw-r--r--   0        0        0      652 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/properties/types/__init__.py
+-rw-r--r--   0        0        0      912 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/properties/types/field_details_type.py
+-rw-r--r--   0        0        0     1026 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/properties/types/field_details_type_read.py
+-rw-r--r--   0        0        0     1118 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/properties/types/field_details_type_request.py
+-rw-r--r--   0        0        0      203 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/properties/types/get_object_properties_response.py
+-rw-r--r--   0        0        0      183 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/properties/types/set_object_properties_request.py
+-rw-r--r--   0        0        0      121 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/properties/types/set_object_properties_response.py
+-rw-r--r--   0        0        0      173 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/proxy/__init__.py
+-rw-r--r--   0        0        0     5499 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/proxy/client.py
+-rw-r--r--   0        0        0      218 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/proxy/types/__init__.py
+-rw-r--r--   0        0        0     1065 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/proxy/types/post_proxy_request_body.py
+-rw-r--r--   0        0        0      883 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/proxy/types/proxy_response.py
+-rw-r--r--   0        0        0      375 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/task/__init__.py
+-rw-r--r--   0        0        0    23576 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/task/client.py
+-rw-r--r--   0        0        0      512 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/task/types/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/task/types/create_or_update_task_request.py
+-rw-r--r--   0        0        0     1017 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/task/types/create_or_update_task_response.py
+-rw-r--r--   0        0        0     1041 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/task/types/get_task_response.py
+-rw-r--r--   0        0        0     1122 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/task/types/get_tasks_response.py
+-rw-r--r--   0        0        0     1059 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/task/types/search_tasks_response.py
+-rw-r--r--   0        0        0      283 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/user/__init__.py
+-rw-r--r--   0        0        0    14641 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/user/client.py
+-rw-r--r--   0        0        0      411 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/user/types/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/user/types/create_or_update_user_request.py
+-rw-r--r--   0        0        0     1017 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/user/types/create_or_update_user_response.py
+-rw-r--r--   0        0        0     1041 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/user/types/get_user_response.py
+-rw-r--r--   0        0        0     1122 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/crm/resources/user/types/get_users_response.py
+-rw-r--r--   0        0        0      793 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/field_mapping/__init__.py
+-rw-r--r--   0        0        0    22972 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/field_mapping/client.py
+-rw-r--r--   0        0        0     1170 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/field_mapping/types/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/field_mapping/types/create_account_field_mapping_request_body.py
+-rw-r--r--   0        0        0      980 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/field_mapping/types/create_account_field_mapping_response.py
+-rw-r--r--   0        0        0     1157 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/field_mapping/types/create_field_mapping_request_body.py
+-rw-r--r--   0        0        0      973 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/field_mapping/types/create_field_mapping_response.py
+-rw-r--r--   0        0        0      986 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/field_mapping/types/delete_account_field_mapping_config_response.py
+-rw-r--r--   0        0        0      990 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/field_mapping/types/delete_field_mapping_response.py
+-rw-r--r--   0        0        0     1061 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/field_mapping/types/field_mapping_type.py
+-rw-r--r--   0        0        0     1206 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/field_mapping/types/get_field_mapping_config_response.py
+-rw-r--r--   0        0        0     1054 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/field_mapping/types/get_field_mappings_response.py
+-rw-r--r--   0        0        0     1108 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/field_mapping/types/mappable_field_type.py
+-rw-r--r--   0        0        0      191 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/metadata/__init__.py
+-rw-r--r--   0        0        0     3656 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/metadata/client.py
+-rw-r--r--   0        0        0      255 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/metadata/types/__init__.py
+-rw-r--r--   0        0        0     1190 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/metadata/types/crm_metadata.py
+-rw-r--r--   0        0        0      985 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/metadata/types/crm_metadata_response.py
+-rw-r--r--   0        0        0      461 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/metadata/types/crm_status.py
+-rw-r--r--   0        0        0      943 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/__init__.py
+-rw-r--r--   0        0        0     1494 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/client.py
+-rw-r--r--   0        0        0      973 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/collection/__init__.py
+-rw-r--r--   0        0        0     5829 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/collection/client.py
+-rw-r--r--   0        0        0      164 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/collection/types/__init__.py
+-rw-r--r--   0        0        0     1063 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/collection/types/get_collections_response.py
+-rw-r--r--   0        0        0      307 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/comment/__init__.py
+-rw-r--r--   0        0        0    19749 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/comment/client.py
+-rw-r--r--   0        0        0      447 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/comment/types/__init__.py
+-rw-r--r--   0        0        0      204 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/comment/types/create_or_update_comment_request.py
+-rw-r--r--   0        0        0     1020 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/comment/types/create_or_update_comment_response.py
+-rw-r--r--   0        0        0      992 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/comment/types/get_comment_response.py
+-rw-r--r--   0        0        0     1060 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/comment/types/get_comments_response.py
+-rw-r--r--   0        0        0      173 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/proxy/__init__.py
+-rw-r--r--   0        0        0     5529 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/proxy/client.py
+-rw-r--r--   0        0        0      218 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/proxy/types/__init__.py
+-rw-r--r--   0        0        0     1065 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/proxy/types/post_proxy_request_body.py
+-rw-r--r--   0        0        0      883 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/proxy/types/proxy_response.py
+-rw-r--r--   0        0        0      283 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/task/__init__.py
+-rw-r--r--   0        0        0    19908 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/task/client.py
+-rw-r--r--   0        0        0      411 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/task/types/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/task/types/create_or_update_task_request.py
+-rw-r--r--   0        0        0     1017 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/task/types/create_or_update_task_response.py
+-rw-r--r--   0        0        0     1060 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/task/types/get_task_response.py
+-rw-r--r--   0        0        0     1141 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/task/types/get_tasks_response.py
+-rw-r--r--   0        0        0      169 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/user/__init__.py
+-rw-r--r--   0        0        0    10114 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/user/client.py
+-rw-r--r--   0        0        0      212 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/user/types/__init__.py
+-rw-r--r--   0        0        0      989 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/user/types/get_user_response.py
+-rw-r--r--   0        0        0     1057 2024-04-02 08:45:32.006374 revert_api-0.0.795/src/revert/resources/ticket/resources/user/types/get_users_response.py
+-rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 revert_api-0.0.795/PKG-INFO
```

### Comparing `revert_api-0.0.785/README.md` & `revert_api-0.0.795/README.md`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/__init__.py` & `revert_api-0.0.795/src/revert/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/client.py` & `revert_api-0.0.795/src/revert/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/core/__init__.py` & `revert_api-0.0.795/src/revert/core/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/core/client_wrapper.py` & `revert_api-0.0.795/src/revert/core/client_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     def __init__(self, *, base_url: str):
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "revert-api",
-            "X-Fern-SDK-Version": "0.0.785",
+            "X-Fern-SDK-Version": "0.0.795",
         }
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `revert_api-0.0.785/src/revert/core/datetime_utils.py` & `revert_api-0.0.795/src/revert/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/core/jsonable_encoder.py` & `revert_api-0.0.795/src/revert/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/__init__.py` & `revert_api-0.0.795/src/revert/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/chat/client.py` & `revert_api-0.0.795/src/revert/resources/chat/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/chat/resources/channels/client.py` & `revert_api-0.0.795/src/revert/resources/chat/resources/channels/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/chat/resources/channels/types/get_channels_response.py` & `revert_api-0.0.795/src/revert/resources/chat/resources/channels/types/get_channels_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/chat/resources/messages/client.py` & `revert_api-0.0.795/src/revert/resources/chat/resources/messages/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/chat/resources/messages/types/createor_update_message_request.py` & `revert_api-0.0.795/src/revert/resources/chat/resources/messages/types/createor_update_message_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/chat/resources/messages/types/createor_update_message_response.py` & `revert_api-0.0.795/src/revert/resources/chat/resources/messages/types/createor_update_message_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/chat/resources/users/client.py` & `revert_api-0.0.795/src/revert/resources/chat/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/chat/resources/users/types/get_users_response.py` & `revert_api-0.0.795/src/revert/resources/chat/resources/users/types/get_users_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/__init__.py` & `revert_api-0.0.795/src/revert/resources/common/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/__init__.py` & `revert_api-0.0.795/src/revert/resources/common/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/associations/types/__init__.py` & `revert_api-0.0.795/src/revert/resources/common/resources/associations/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/associations/types/company_association.py` & `revert_api-0.0.795/src/revert/resources/common/resources/associations/types/company_association.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/associations/types/contact_association.py` & `revert_api-0.0.795/src/revert/resources/common/resources/associations/types/contact_association.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/associations/types/deal_association.py` & `revert_api-0.0.795/src/revert/resources/common/resources/associations/types/deal_association.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/associations/types/event_association.py` & `revert_api-0.0.795/src/revert/resources/common/resources/associations/types/event_association.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/associations/types/lead_association.py` & `revert_api-0.0.795/src/revert/resources/common/resources/associations/types/lead_association.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/associations/types/task_association.py` & `revert_api-0.0.795/src/revert/resources/common/resources/associations/types/task_association.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/errors/types/base_error.py` & `revert_api-0.0.795/src/revert/resources/common/resources/errors/types/base_error.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/types/types/__init__.py` & `revert_api-0.0.795/src/revert/resources/common/resources/types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/types/types/account.py` & `revert_api-0.0.795/src/revert/resources/common/resources/types/types/account.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/types/types/app.py` & `revert_api-0.0.795/src/revert/resources/common/resources/types/types/app.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/types/types/app_config.py` & `revert_api-0.0.795/src/revert/resources/common/resources/types/types/app_config.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/types/types/connection.py` & `revert_api-0.0.795/src/revert/resources/common/resources/types/types/connection.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/types/types/revert_user.py` & `revert_api-0.0.795/src/revert/resources/common/resources/types/types/revert_user.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/types/types/standard_object.py` & `revert_api-0.0.795/src/revert/resources/common/resources/types/types/standard_object.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/types/types/ticket_priority.py` & `revert_api-0.0.795/src/revert/resources/common/resources/types/types/ticket_priority.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/types/types/ticket_status.py` & `revert_api-0.0.795/src/revert/resources/common/resources/types/types/ticket_status.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/types/types/tpid.py` & `revert_api-0.0.795/src/revert/resources/common/resources/types/types/tpid.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/__init__.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/__init__.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/channel.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/channel.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/comment_ticket_write.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/comment_ticket_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/common_unified_fields.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/common_unified_fields.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/company.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/company.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/company_address.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/company_address.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/contact.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/contact.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/contact_read.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/contact_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/contact_write.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/contact_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/deal.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/deal.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/deal_read.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/deal_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/deal_write.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/deal_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/event.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/event.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/event_read.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/event_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/event_write.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/event_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/lead.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/lead.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/lead_read.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/lead_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/lead_write.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/lead_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/message.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/message.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/note.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/note.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/note_read.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/note_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/note_write.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/note_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/task.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/task.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/task_read.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/task_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/task_ticket.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/task_ticket.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/task_ticket_write.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/task_ticket_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/task_write.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/task_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/user.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/user.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/user_chat.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/user_chat.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/common/resources/unified/types/user_write.py` & `revert_api-0.0.795/src/revert/resources/common/resources/unified/types/user_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/connection/__init__.py` & `revert_api-0.0.795/src/revert/resources/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/connection/client.py` & `revert_api-0.0.795/src/revert/resources/connection/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/connection/types/__init__.py` & `revert_api-0.0.795/src/revert/resources/connection/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/connection/types/create_connection_webhook_request.py` & `revert_api-0.0.795/src/revert/resources/connection/types/create_connection_webhook_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/connection/types/create_connection_webhook_response.py` & `revert_api-0.0.795/src/revert/resources/connection/types/create_connection_webhook_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/connection/types/delete_connection_response.py` & `revert_api-0.0.795/src/revert/resources/connection/types/delete_connection_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/connection/types/delete_connection_webhook_response.py` & `revert_api-0.0.795/src/revert/resources/connection/types/delete_connection_webhook_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/connection/types/get_connect_status_response.py` & `revert_api-0.0.795/src/revert/resources/connection/types/get_connect_status_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/connection/types/get_connection_response.py` & `revert_api-0.0.795/src/revert/resources/connection/types/get_connection_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/connection/types/get_connection_webhook_response.py` & `revert_api-0.0.795/src/revert/resources/connection/types/get_connection_webhook_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/__init__.py` & `revert_api-0.0.795/src/revert/resources/crm/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/client.py` & `revert_api-0.0.795/src/revert/resources/crm/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/__init__.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/company/client.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/company/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/company/types/__init__.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/company/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/company/types/create_or_update_company_request.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/company/types/create_or_update_company_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/company/types/create_or_update_company_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/company/types/create_or_update_company_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/company/types/get_companies_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/company/types/get_companies_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/company/types/get_company_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/company/types/get_company_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/company/types/search_companies_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/company/types/search_companies_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/contact/client.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/contact/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/contact/types/__init__.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/contact/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/contact/types/create_or_update_contact_request.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/contact/types/create_or_update_contact_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/contact/types/create_or_update_contact_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/contact/types/create_or_update_contact_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/contact/types/get_contact_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/contact/types/get_contact_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/contact/types/get_contacts_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/contact/types/get_contacts_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/contact/types/search_contacts_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/contact/types/search_contacts_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/deal/client.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/deal/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/deal/types/__init__.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/deal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/deal/types/create_or_update_deal_request.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/deal/types/create_or_update_deal_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/deal/types/create_or_update_deal_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/deal/types/create_or_update_deal_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/deal/types/get_deal_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/deal/types/get_deal_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/deal/types/get_deals_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/deal/types/get_deals_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/deal/types/search_deals_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/deal/types/search_deals_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/event/client.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/event/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/event/types/__init__.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/event/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/event/types/create_or_update_event_request.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/event/types/create_or_update_event_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/event/types/create_or_update_event_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/event/types/create_or_update_event_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/event/types/delete_event_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/event/types/delete_event_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/event/types/get_event_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/event/types/get_event_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/event/types/get_events_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/event/types/get_events_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/event/types/search_events_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/event/types/search_events_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/lead/client.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/lead/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/lead/types/__init__.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/lead/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/lead/types/create_or_update_lead_request.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/lead/types/create_or_update_lead_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/lead/types/create_or_update_lead_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/lead/types/create_or_update_lead_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/lead/types/get_lead_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/lead/types/get_lead_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/lead/types/get_leads_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/lead/types/get_leads_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/lead/types/search_leads_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/lead/types/search_leads_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/note/client.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/note/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/note/types/__init__.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/note/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/note/types/create_or_update_note_request.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/note/types/create_or_update_note_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/note/types/create_or_update_note_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/note/types/create_or_update_note_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/note/types/get_note_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/note/types/get_note_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/note/types/get_notes_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/note/types/get_notes_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/note/types/search_notes_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/note/types/search_notes_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/properties/client.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/properties/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/properties/types/__init__.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/properties/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/properties/types/field_details_type.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/properties/types/field_details_type.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/properties/types/field_details_type_read.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/properties/types/field_details_type_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/properties/types/field_details_type_request.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/properties/types/field_details_type_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/proxy/client.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/proxy/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/proxy/types/post_proxy_request_body.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/proxy/types/post_proxy_request_body.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/proxy/types/proxy_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/proxy/types/proxy_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/task/client.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/task/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/task/types/__init__.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/task/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/task/types/create_or_update_task_request.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/task/types/create_or_update_task_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/task/types/create_or_update_task_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/task/types/create_or_update_task_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/task/types/get_task_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/task/types/get_task_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/task/types/get_tasks_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/task/types/get_tasks_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/task/types/search_tasks_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/task/types/search_tasks_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/user/client.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/user/types/create_or_update_user_request.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/user/types/create_or_update_user_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/user/types/create_or_update_user_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/user/types/create_or_update_user_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/user/types/get_user_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/user/types/get_user_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/crm/resources/user/types/get_users_response.py` & `revert_api-0.0.795/src/revert/resources/crm/resources/user/types/get_users_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/field_mapping/__init__.py` & `revert_api-0.0.795/src/revert/resources/field_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/field_mapping/client.py` & `revert_api-0.0.795/src/revert/resources/field_mapping/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/field_mapping/types/__init__.py` & `revert_api-0.0.795/src/revert/resources/field_mapping/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/field_mapping/types/create_account_field_mapping_request_body.py` & `revert_api-0.0.795/src/revert/resources/field_mapping/types/create_account_field_mapping_request_body.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/field_mapping/types/create_account_field_mapping_response.py` & `revert_api-0.0.795/src/revert/resources/field_mapping/types/create_account_field_mapping_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/field_mapping/types/create_field_mapping_request_body.py` & `revert_api-0.0.795/src/revert/resources/field_mapping/types/create_field_mapping_request_body.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/field_mapping/types/create_field_mapping_response.py` & `revert_api-0.0.795/src/revert/resources/field_mapping/types/create_field_mapping_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/field_mapping/types/delete_account_field_mapping_config_response.py` & `revert_api-0.0.795/src/revert/resources/field_mapping/types/delete_account_field_mapping_config_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/field_mapping/types/delete_field_mapping_response.py` & `revert_api-0.0.795/src/revert/resources/field_mapping/types/delete_field_mapping_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/field_mapping/types/field_mapping_type.py` & `revert_api-0.0.795/src/revert/resources/field_mapping/types/field_mapping_type.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/field_mapping/types/get_field_mapping_config_response.py` & `revert_api-0.0.795/src/revert/resources/field_mapping/types/get_field_mapping_config_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/field_mapping/types/get_field_mappings_response.py` & `revert_api-0.0.795/src/revert/resources/field_mapping/types/get_field_mappings_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/field_mapping/types/mappable_field_type.py` & `revert_api-0.0.795/src/revert/resources/field_mapping/types/mappable_field_type.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/metadata/client.py` & `revert_api-0.0.795/src/revert/resources/metadata/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/metadata/types/crm_metadata.py` & `revert_api-0.0.795/src/revert/resources/metadata/types/crm_metadata.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/metadata/types/crm_metadata_response.py` & `revert_api-0.0.795/src/revert/resources/metadata/types/crm_metadata_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/__init__.py` & `revert_api-0.0.795/src/revert/resources/ticket/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/client.py` & `revert_api-0.0.795/src/revert/resources/ticket/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/__init__.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/collection/client.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/collection/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/collection/types/get_collections_response.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/collection/types/get_collections_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/comment/client.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/comment/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/comment/types/create_or_update_comment_response.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/comment/types/create_or_update_comment_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/comment/types/get_comment_response.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/comment/types/get_comment_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/comment/types/get_comments_response.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/comment/types/get_comments_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/proxy/client.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/proxy/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/proxy/types/post_proxy_request_body.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/proxy/types/post_proxy_request_body.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/proxy/types/proxy_response.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/proxy/types/proxy_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/task/client.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/task/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/task/types/create_or_update_task_response.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/task/types/create_or_update_task_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/task/types/get_task_response.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/task/types/get_task_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/task/types/get_tasks_response.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/task/types/get_tasks_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/user/client.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/user/types/get_user_response.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/user/types/get_user_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/src/revert/resources/ticket/resources/user/types/get_users_response.py` & `revert_api-0.0.795/src/revert/resources/ticket/resources/user/types/get_users_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.785/PKG-INFO` & `revert_api-0.0.795/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revert-api
-Version: 0.0.785
+Version: 0.0.795
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

