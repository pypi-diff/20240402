# Comparing `tmp/kdp-api-python-client-4.98.0.tar.gz` & `tmp/kdp-api-python-client-4.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdp-api-python-client-4.98.0.tar", last modified: Mon Nov 13 20:32:35 2023, max compression
+gzip compressed data, was "kdp-api-python-client-4.99.0.tar", last modified: Mon Nov 13 20:45:45 2023, max compression
```

## Comparing `kdp-api-python-client-4.98.0.tar` & `kdp-api-python-client-4.99.0.tar`

### file list

```diff
@@ -1,349 +1,349 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:32:35.440755 kdp-api-python-client-4.98.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1183 2023-11-13 20:32:35.440755 kdp-api-python-client-4.98.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27758 2023-11-13 20:30:45.000000 kdp-api-python-client-4.98.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:32:35.384755 kdp-api-python-client-4.98.0/kdp_api/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1372 2023-11-13 20:31:16.000000 kdp-api-python-client-4.98.0/kdp_api/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:32:35.388755 kdp-api-python-client-4.98.0/kdp_api/api/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      220 2023-11-13 20:31:18.000000 kdp-api-python-client-4.98.0/kdp_api/api/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12487 2023-11-13 20:31:18.000000 kdp-api-python-client-4.98.0/kdp_api/api/abac_label_parsers_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33506 2023-11-13 20:31:18.000000 kdp-api-python-client-4.98.0/kdp_api/api/applications_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35353 2023-11-13 20:31:18.000000 kdp-api-python-client-4.98.0/kdp_api/api/attribute_assignments_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33299 2023-11-13 20:31:18.000000 kdp-api-python-client-4.98.0/kdp_api/api/attributes_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7406 2023-11-13 20:31:19.000000 kdp-api-python-client-4.98.0/kdp_api/api/audit_log_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13991 2023-11-13 20:31:19.000000 kdp-api-python-client-4.98.0/kdp_api/api/audit_log_configs_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17488 2023-11-13 20:31:19.000000 kdp-api-python-client-4.98.0/kdp_api/api/authentication_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34183 2023-11-13 20:31:19.000000 kdp-api-python-client-4.98.0/kdp_api/api/dataset_permissions_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    41536 2023-11-13 20:31:19.000000 kdp-api-python-client-4.98.0/kdp_api/api/dataset_syncs_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33089 2023-11-13 20:31:20.000000 kdp-api-python-client-4.98.0/kdp_api/api/datasets_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34014 2023-11-13 20:31:20.000000 kdp-api-python-client-4.98.0/kdp_api/api/group_memberships_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32929 2023-11-13 20:31:20.000000 kdp-api-python-client-4.98.0/kdp_api/api/groups_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32864 2023-11-13 20:31:20.000000 kdp-api-python-client-4.98.0/kdp_api/api/indexes_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7173 2023-11-13 20:31:20.000000 kdp-api-python-client-4.98.0/kdp_api/api/ingest_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27838 2023-11-13 20:31:20.000000 kdp-api-python-client-4.98.0/kdp_api/api/jobs_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23682 2023-11-13 20:31:21.000000 kdp-api-python-client-4.98.0/kdp_api/api/query_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17576 2023-11-13 20:31:21.000000 kdp-api-python-client-4.98.0/kdp_api/api/read_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13109 2023-11-13 20:31:21.000000 kdp-api-python-client-4.98.0/kdp_api/api/segments_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7384 2023-11-13 20:31:21.000000 kdp-api-python-client-4.98.0/kdp_api/api/serve_media_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12216 2023-11-13 20:31:22.000000 kdp-api-python-client-4.98.0/kdp_api/api/source_types_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23758 2023-11-13 20:31:22.000000 kdp-api-python-client-4.98.0/kdp_api/api/storage_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8316 2023-11-13 20:31:22.000000 kdp-api-python-client-4.98.0/kdp_api/api/uploads_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32806 2023-11-13 20:31:22.000000 kdp-api-python-client-4.98.0/kdp_api/api/users_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28404 2023-11-13 20:31:22.000000 kdp-api-python-client-4.98.0/kdp_api/api/workspaces_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13314 2023-11-13 20:31:22.000000 kdp-api-python-client-4.98.0/kdp_api/api/write_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    39772 2023-11-13 20:31:17.000000 kdp-api-python-client-4.98.0/kdp_api/api_client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:32:35.388755 kdp-api-python-client-4.98.0/kdp_api/apis/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1764 2023-11-13 20:31:23.000000 kdp-api-python-client-4.98.0/kdp_api/apis/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17443 2023-11-13 20:31:17.000000 kdp-api-python-client-4.98.0/kdp_api/configuration.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5759 2023-11-13 20:31:17.000000 kdp-api-python-client-4.98.0/kdp_api/exceptions.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:32:35.416755 kdp-api-python-client-4.98.0/kdp_api/model/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      341 2023-11-13 20:31:23.000000 kdp-api-python-client-4.98.0/kdp_api/model/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12920 2023-11-13 20:31:23.000000 kdp-api-python-client-4.98.0/kdp_api/model/abac_label_parser_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12911 2023-11-13 20:31:23.000000 kdp-api-python-client-4.98.0/kdp_api/model/abac_label_parsers.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12709 2023-11-13 20:31:23.000000 kdp-api-python-client-4.98.0/kdp_api/model/abac_label_parsers_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12924 2023-11-13 20:31:23.000000 kdp-api-python-client-4.98.0/kdp_api/model/access_control_label.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12794 2023-11-13 20:31:24.000000 kdp-api-python-client-4.98.0/kdp_api/model/api_error.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15510 2023-11-13 20:31:24.000000 kdp-api-python-client-4.98.0/kdp_api/model/application.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14946 2023-11-13 20:31:24.000000 kdp-api-python-client-4.98.0/kdp_api/model/application_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12526 2023-11-13 20:31:24.000000 kdp-api-python-client-4.98.0/kdp_api/model/application_create_request_required_dataset_access_inner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12623 2023-11-13 20:31:24.000000 kdp-api-python-client-4.98.0/kdp_api/model/application_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12871 2023-11-13 20:31:25.000000 kdp-api-python-client-4.98.0/kdp_api/model/application_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15143 2023-11-13 20:31:25.000000 kdp-api-python-client-4.98.0/kdp_api/model/application_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12557 2023-11-13 20:31:25.000000 kdp-api-python-client-4.98.0/kdp_api/model/application_required_dataset_access_inner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15482 2023-11-13 20:31:25.000000 kdp-api-python-client-4.98.0/kdp_api/model/application_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13067 2023-11-13 20:31:25.000000 kdp-api-python-client-4.98.0/kdp_api/model/attribute.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13327 2023-11-13 20:31:25.000000 kdp-api-python-client-4.98.0/kdp_api/model/attribute_assignment.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12482 2023-11-13 20:31:26.000000 kdp-api-python-client-4.98.0/kdp_api/model/attribute_assignment_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12756 2023-11-13 20:31:26.000000 kdp-api-python-client-4.98.0/kdp_api/model/attribute_assignment_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12952 2023-11-13 20:31:26.000000 kdp-api-python-client-4.98.0/kdp_api/model/attribute_assignment_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12359 2023-11-13 20:31:26.000000 kdp-api-python-client-4.98.0/kdp_api/model/attribute_assignment_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12650 2023-11-13 20:31:26.000000 kdp-api-python-client-4.98.0/kdp_api/model/attribute_assignment_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12774 2023-11-13 20:31:27.000000 kdp-api-python-client-4.98.0/kdp_api/model/attribute_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12591 2023-11-13 20:31:27.000000 kdp-api-python-client-4.98.0/kdp_api/model/attribute_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12851 2023-11-13 20:31:27.000000 kdp-api-python-client-4.98.0/kdp_api/model/attribute_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12711 2023-11-13 20:31:27.000000 kdp-api-python-client-4.98.0/kdp_api/model/attribute_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12942 2023-11-13 20:31:27.000000 kdp-api-python-client-4.98.0/kdp_api/model/attribute_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13387 2023-11-13 20:31:28.000000 kdp-api-python-client-4.98.0/kdp_api/model/audit_log_configuration.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12793 2023-11-13 20:31:28.000000 kdp-api-python-client-4.98.0/kdp_api/model/audit_log_configuration_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12973 2023-11-13 20:31:28.000000 kdp-api-python-client-4.98.0/kdp_api/model/audit_log_configuration_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15345 2023-11-13 20:31:28.000000 kdp-api-python-client-4.98.0/kdp_api/model/audit_log_event.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12665 2023-11-13 20:31:28.000000 kdp-api-python-client-4.98.0/kdp_api/model/audit_log_event_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12878 2023-11-13 20:31:28.000000 kdp-api-python-client-4.98.0/kdp_api/model/audit_log_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13169 2023-11-13 20:31:29.000000 kdp-api-python-client-4.98.0/kdp_api/model/authentication.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13119 2023-11-13 20:31:29.000000 kdp-api-python-client-4.98.0/kdp_api/model/authentication_details.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12975 2023-11-13 20:31:29.000000 kdp-api-python-client-4.98.0/kdp_api/model/authentication_details_authentication.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13043 2023-11-13 20:31:29.000000 kdp-api-python-client-4.98.0/kdp_api/model/authentication_details_authentication_payload.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15754 2023-11-13 20:31:29.000000 kdp-api-python-client-4.98.0/kdp_api/model/authentication_details_user.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12671 2023-11-13 20:31:29.000000 kdp-api-python-client-4.98.0/kdp_api/model/authentication_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12918 2023-11-13 20:31:30.000000 kdp-api-python-client-4.98.0/kdp_api/model/authentication_sso.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12916 2023-11-13 20:31:30.000000 kdp-api-python-client-4.98.0/kdp_api/model/batch_write_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13570 2023-11-13 20:31:30.000000 kdp-api-python-client-4.98.0/kdp_api/model/connection_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13580 2023-11-13 20:31:30.000000 kdp-api-python-client-4.98.0/kdp_api/model/custom_identity_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12809 2023-11-13 20:31:30.000000 kdp-api-python-client-4.98.0/kdp_api/model/custom_identity_provider_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13619 2023-11-13 20:31:31.000000 kdp-api-python-client-4.98.0/kdp_api/model/data_source_params.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14962 2023-11-13 20:31:31.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13729 2023-11-13 20:31:31.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12656 2023-11-13 20:31:31.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_current_user_permissions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12559 2023-11-13 20:31:31.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12831 2023-11-13 20:31:31.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13575 2023-11-13 20:31:32.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13168 2023-11-13 20:31:32.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_permission.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12801 2023-11-13 20:31:32.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_permission_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12724 2023-11-13 20:31:32.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_permission_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12932 2023-11-13 20:31:32.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_permission_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12660 2023-11-13 20:31:32.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_permission_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12969 2023-11-13 20:31:33.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_permission_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17860 2023-11-13 20:31:33.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_sync.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12628 2023-11-13 20:31:33.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_sync_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12713 2023-11-13 20:31:33.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_sync_management_terminate_connection_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12872 2023-11-13 20:31:33.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_sync_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17896 2023-11-13 20:31:34.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_sync_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18371 2023-11-13 20:31:34.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_sync_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13620 2023-11-13 20:31:34.000000 kdp-api-python-client-4.98.0/kdp_api/model/dataset_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12290 2023-11-13 20:31:34.000000 kdp-api-python-client-4.98.0/kdp_api/model/delete_document_by_query_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13005 2023-11-13 20:31:34.000000 kdp-api-python-client-4.98.0/kdp_api/model/delete_record_by_id_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12280 2023-11-13 20:31:34.000000 kdp-api-python-client-4.98.0/kdp_api/model/delete_record_by_query_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14657 2023-11-13 20:31:35.000000 kdp-api-python-client-4.98.0/kdp_api/model/error_code.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12148 2023-11-13 20:31:35.000000 kdp-api-python-client-4.98.0/kdp_api/model/get_serve_media200_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13380 2023-11-13 20:31:35.000000 kdp-api-python-client-4.98.0/kdp_api/model/group.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13022 2023-11-13 20:31:35.000000 kdp-api-python-client-4.98.0/kdp_api/model/group_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12527 2023-11-13 20:31:35.000000 kdp-api-python-client-4.98.0/kdp_api/model/group_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13535 2023-11-13 20:31:36.000000 kdp-api-python-client-4.98.0/kdp_api/model/group_membership.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12710 2023-11-13 20:31:36.000000 kdp-api-python-client-4.98.0/kdp_api/model/group_membership_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12692 2023-11-13 20:31:36.000000 kdp-api-python-client-4.98.0/kdp_api/model/group_membership_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12912 2023-11-13 20:31:36.000000 kdp-api-python-client-4.98.0/kdp_api/model/group_membership_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12599 2023-11-13 20:31:36.000000 kdp-api-python-client-4.98.0/kdp_api/model/group_membership_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12878 2023-11-13 20:31:36.000000 kdp-api-python-client-4.98.0/kdp_api/model/group_membership_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12811 2023-11-13 20:31:37.000000 kdp-api-python-client-4.98.0/kdp_api/model/group_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12700 2023-11-13 20:31:37.000000 kdp-api-python-client-4.98.0/kdp_api/model/group_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13022 2023-11-13 20:31:37.000000 kdp-api-python-client-4.98.0/kdp_api/model/group_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12615 2023-11-13 20:31:37.000000 kdp-api-python-client-4.98.0/kdp_api/model/index.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12531 2023-11-13 20:31:37.000000 kdp-api-python-client-4.98.0/kdp_api/model/index_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12811 2023-11-13 20:31:38.000000 kdp-api-python-client-4.98.0/kdp_api/model/index_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12721 2023-11-13 20:31:38.000000 kdp-api-python-client-4.98.0/kdp_api/model/ingest_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15045 2023-11-13 20:31:38.000000 kdp-api-python-client-4.98.0/kdp_api/model/job.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12495 2023-11-13 20:31:38.000000 kdp-api-python-client-4.98.0/kdp_api/model/job_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12791 2023-11-13 20:31:38.000000 kdp-api-python-client-4.98.0/kdp_api/model/job_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11896 2023-11-13 20:31:38.000000 kdp-api-python-client-4.98.0/kdp_api/model/json_record.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14576 2023-11-13 20:31:39.000000 kdp-api-python-client-4.98.0/kdp_api/model/keycloak_provider_configuration.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14479 2023-11-13 20:31:39.000000 kdp-api-python-client-4.98.0/kdp_api/model/koverse_document_metadata.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13782 2023-11-13 20:31:39.000000 kdp-api-python-client-4.98.0/kdp_api/model/lucene_query_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13306 2023-11-13 20:31:39.000000 kdp-api-python-client-4.98.0/kdp_api/model/origin_dataset_sync_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13885 2023-11-13 20:31:39.000000 kdp-api-python-client-4.98.0/kdp_api/model/query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13835 2023-11-13 20:31:40.000000 kdp-api-python-client-4.98.0/kdp_api/model/query_datasets_summary.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12747 2023-11-13 20:31:40.000000 kdp-api-python-client-4.98.0/kdp_api/model/query_datasets_summary_datasets_inner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13844 2023-11-13 20:31:40.000000 kdp-api-python-client-4.98.0/kdp_api/model/query_datasets_summary_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13806 2023-11-13 20:31:40.000000 kdp-api-python-client-4.98.0/kdp_api/model/query_document_lucene_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12946 2023-11-13 20:31:40.000000 kdp-api-python-client-4.98.0/kdp_api/model/query_document_lucene_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13854 2023-11-13 20:31:41.000000 kdp-api-python-client-4.98.0/kdp_api/model/query_document_lucene_response_records_inner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14704 2023-11-13 20:31:41.000000 kdp-api-python-client-4.98.0/kdp_api/model/read_range_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13528 2023-11-13 20:31:41.000000 kdp-api-python-client-4.98.0/kdp_api/model/record_batch.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13059 2023-11-13 20:31:41.000000 kdp-api-python-client-4.98.0/kdp_api/model/reindex_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13619 2023-11-13 20:31:41.000000 kdp-api-python-client-4.98.0/kdp_api/model/replica_dataset_sync_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13998 2023-11-13 20:31:42.000000 kdp-api-python-client-4.98.0/kdp_api/model/security_label_info_params.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14682 2023-11-13 20:31:42.000000 kdp-api-python-client-4.98.0/kdp_api/model/segment.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12559 2023-11-13 20:31:42.000000 kdp-api-python-client-4.98.0/kdp_api/model/segment_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12831 2023-11-13 20:31:42.000000 kdp-api-python-client-4.98.0/kdp_api/model/segment_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13409 2023-11-13 20:31:42.000000 kdp-api-python-client-4.98.0/kdp_api/model/sequence_read_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12758 2023-11-13 20:31:42.000000 kdp-api-python-client-4.98.0/kdp_api/model/source_types.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12624 2023-11-13 20:31:43.000000 kdp-api-python-client-4.98.0/kdp_api/model/source_types_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12564 2023-11-13 20:31:43.000000 kdp-api-python-client-4.98.0/kdp_api/model/split_points.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13047 2023-11-13 20:31:43.000000 kdp-api-python-client-4.98.0/kdp_api/model/stripe_latest_charge.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13348 2023-11-13 20:31:43.000000 kdp-api-python-client-4.98.0/kdp_api/model/stripe_latest_charge1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13034 2023-11-13 20:31:43.000000 kdp-api-python-client-4.98.0/kdp_api/model/sync_kafka_consumer_group_id.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15181 2023-11-13 20:31:44.000000 kdp-api-python-client-4.98.0/kdp_api/model/sync_setup_origin.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15184 2023-11-13 20:31:44.000000 kdp-api-python-client-4.98.0/kdp_api/model/sync_setup_replica.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12800 2023-11-13 20:31:44.000000 kdp-api-python-client-4.98.0/kdp_api/model/terminate_connection_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14142 2023-11-13 20:31:44.000000 kdp-api-python-client-4.98.0/kdp_api/model/transfer_resource_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12825 2023-11-13 20:31:44.000000 kdp-api-python-client-4.98.0/kdp_api/model/transfer_resource_request_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13602 2023-11-13 20:31:45.000000 kdp-api-python-client-4.98.0/kdp_api/model/upload_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14107 2023-11-13 20:31:45.000000 kdp-api-python-client-4.98.0/kdp_api/model/user.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13823 2023-11-13 20:31:45.000000 kdp-api-python-client-4.98.0/kdp_api/model/user_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12511 2023-11-13 20:31:45.000000 kdp-api-python-client-4.98.0/kdp_api/model/user_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12801 2023-11-13 20:31:45.000000 kdp-api-python-client-4.98.0/kdp_api/model/user_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13844 2023-11-13 20:31:45.000000 kdp-api-python-client-4.98.0/kdp_api/model/user_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14221 2023-11-13 20:31:46.000000 kdp-api-python-client-4.98.0/kdp_api/model/user_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13348 2023-11-13 20:31:46.000000 kdp-api-python-client-4.98.0/kdp_api/model/workspace.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13070 2023-11-13 20:31:46.000000 kdp-api-python-client-4.98.0/kdp_api/model/workspace_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14612 2023-11-13 20:31:46.000000 kdp-api-python-client-4.98.0/kdp_api/model/workspace_create_request_subscription.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12773 2023-11-13 20:31:46.000000 kdp-api-python-client-4.98.0/kdp_api/model/workspace_create_request_subscription_subscription_item_ids.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12591 2023-11-13 20:31:47.000000 kdp-api-python-client-4.98.0/kdp_api/model/workspace_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12851 2023-11-13 20:31:47.000000 kdp-api-python-client-4.98.0/kdp_api/model/workspace_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13025 2023-11-13 20:31:47.000000 kdp-api-python-client-4.98.0/kdp_api/model/workspace_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14774 2023-11-13 20:31:47.000000 kdp-api-python-client-4.98.0/kdp_api/model/workspace_subscription.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12734 2023-11-13 20:31:47.000000 kdp-api-python-client-4.98.0/kdp_api/model/workspace_subscription_subscription_item_ids.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13070 2023-11-13 20:31:47.000000 kdp-api-python-client-4.98.0/kdp_api/model/workspace_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12731 2023-11-13 20:31:48.000000 kdp-api-python-client-4.98.0/kdp_api/model/write_batch_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    83279 2023-11-13 20:31:17.000000 kdp-api-python-client-4.98.0/kdp_api/model_utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:32:35.416755 kdp-api-python-client-4.98.0/kdp_api/models/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9984 2023-11-13 20:31:48.000000 kdp-api-python-client-4.98.0/kdp_api/models/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14956 2023-11-13 20:31:17.000000 kdp-api-python-client-4.98.0/kdp_api/rest.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:32:35.420755 kdp-api-python-client-4.98.0/kdp_api_python_client.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1183 2023-11-13 20:32:35.000000 kdp-api-python-client-4.98.0/kdp_api_python_client.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12374 2023-11-13 20:32:35.000000 kdp-api-python-client-4.98.0/kdp_api_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-11-13 20:32:35.000000 kdp-api-python-client-4.98.0/kdp_api_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       32 2023-11-13 20:32:35.000000 kdp-api-python-client-4.98.0/kdp_api_python_client.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-11-13 20:32:35.000000 kdp-api-python-client-4.98.0/kdp_api_python_client.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       69 2023-11-13 20:32:35.440755 kdp-api-python-client-4.98.0/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2524 2023-11-13 20:30:46.000000 kdp-api-python-client-4.98.0/setup.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:32:35.440755 kdp-api-python-client-4.98.0/test/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1627 2023-11-13 20:31:48.000000 kdp-api-python-client-4.98.0/test/test_abac_label_parser_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1442 2023-11-13 20:31:48.000000 kdp-api-python-client-4.98.0/test/test_abac_label_parsers.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1652 2023-11-13 20:31:48.000000 kdp-api-python-client-4.98.0/test/test_abac_label_parsers_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1582 2023-11-13 20:31:49.000000 kdp-api-python-client-4.98.0/test/test_abac_label_parsers_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1596 2023-11-13 20:31:49.000000 kdp-api-python-client-4.98.0/test/test_access_control_label.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1385 2023-11-13 20:31:49.000000 kdp-api-python-client-4.98.0/test/test_api_error.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1602 2023-11-13 20:31:49.000000 kdp-api-python-client-4.98.0/test/test_application.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1749 2023-11-13 20:31:50.000000 kdp-api-python-client-4.98.0/test/test_application_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1684 2023-11-13 20:31:50.000000 kdp-api-python-client-4.98.0/test/test_application_create_request_required_dataset_access_inner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1523 2023-11-13 20:31:50.000000 kdp-api-python-client-4.98.0/test/test_application_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1575 2023-11-13 20:31:50.000000 kdp-api-python-client-4.98.0/test/test_application_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1742 2023-11-13 20:31:50.000000 kdp-api-python-client-4.98.0/test/test_application_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1591 2023-11-13 20:31:50.000000 kdp-api-python-client-4.98.0/test/test_application_required_dataset_access_inner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1749 2023-11-13 20:31:51.000000 kdp-api-python-client-4.98.0/test/test_application_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2294 2023-11-13 20:31:51.000000 kdp-api-python-client-4.98.0/test/test_applications_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1391 2023-11-13 20:31:51.000000 kdp-api-python-client-4.98.0/test/test_attribute.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1604 2023-11-13 20:31:51.000000 kdp-api-python-client-4.98.0/test/test_attribute_assignment.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1555 2023-11-13 20:31:51.000000 kdp-api-python-client-4.98.0/test/test_attribute_assignment_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1613 2023-11-13 20:31:51.000000 kdp-api-python-client-4.98.0/test/test_attribute_assignment_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1665 2023-11-13 20:31:52.000000 kdp-api-python-client-4.98.0/test/test_attribute_assignment_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1548 2023-11-13 20:31:52.000000 kdp-api-python-client-4.98.0/test/test_attribute_assignment_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1555 2023-11-13 20:31:52.000000 kdp-api-python-client-4.98.0/test/test_attribute_assignment_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2479 2023-11-13 20:31:52.000000 kdp-api-python-client-4.98.0/test/test_attribute_assignments_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1484 2023-11-13 20:31:53.000000 kdp-api-python-client-4.98.0/test/test_attribute_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-11-13 20:31:53.000000 kdp-api-python-client-4.98.0/test/test_attribute_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1553 2023-11-13 20:31:53.000000 kdp-api-python-client-4.98.0/test/test_attribute_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1477 2023-11-13 20:31:53.000000 kdp-api-python-client-4.98.0/test/test_attribute_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1484 2023-11-13 20:31:53.000000 kdp-api-python-client-4.98.0/test/test_attribute_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2245 2023-11-13 20:31:53.000000 kdp-api-python-client-4.98.0/test/test_attributes_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1403 2023-11-13 20:31:54.000000 kdp-api-python-client-4.98.0/test/test_audit_log_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1659 2023-11-13 20:31:54.000000 kdp-api-python-client-4.98.0/test/test_audit_log_configs_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1477 2023-11-13 20:31:54.000000 kdp-api-python-client-4.98.0/test/test_audit_log_configuration.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1637 2023-11-13 20:31:54.000000 kdp-api-python-client-4.98.0/test/test_audit_log_configuration_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1689 2023-11-13 20:31:54.000000 kdp-api-python-client-4.98.0/test/test_audit_log_configuration_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1421 2023-11-13 20:31:54.000000 kdp-api-python-client-4.98.0/test/test_audit_log_event.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1549 2023-11-13 20:31:55.000000 kdp-api-python-client-4.98.0/test/test_audit_log_event_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1565 2023-11-13 20:31:55.000000 kdp-api-python-client-4.98.0/test/test_audit_log_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1426 2023-11-13 20:31:55.000000 kdp-api-python-client-4.98.0/test/test_authentication.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1845 2023-11-13 20:31:55.000000 kdp-api-python-client-4.98.0/test/test_authentication_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1810 2023-11-13 20:31:55.000000 kdp-api-python-client-4.98.0/test/test_authentication_details.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1791 2023-11-13 20:31:56.000000 kdp-api-python-client-4.98.0/test/test_authentication_details_authentication.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1625 2023-11-13 20:31:56.000000 kdp-api-python-client-4.98.0/test/test_authentication_details_authentication_payload.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1505 2023-11-13 20:31:56.000000 kdp-api-python-client-4.98.0/test/test_authentication_details_user.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1556 2023-11-13 20:31:56.000000 kdp-api-python-client-4.98.0/test/test_authentication_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1448 2023-11-13 20:31:56.000000 kdp-api-python-client-4.98.0/test/test_authentication_sso.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1589 2023-11-13 20:31:57.000000 kdp-api-python-client-4.98.0/test/test_batch_write_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1427 2023-11-13 20:31:57.000000 kdp-api-python-client-4.98.0/test/test_connection_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-11-13 20:31:57.000000 kdp-api-python-client-4.98.0/test/test_custom_identity_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1648 2023-11-13 20:31:57.000000 kdp-api-python-client-4.98.0/test/test_custom_identity_provider_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1684 2023-11-13 20:31:57.000000 kdp-api-python-client-4.98.0/test/test_data_source_params.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1541 2023-11-13 20:31:57.000000 kdp-api-python-client-4.98.0/test/test_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1470 2023-11-13 20:31:58.000000 kdp-api-python-client-4.98.0/test/test_dataset_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1534 2023-11-13 20:31:58.000000 kdp-api-python-client-4.98.0/test/test_dataset_current_user_permissions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1479 2023-11-13 20:31:58.000000 kdp-api-python-client-4.98.0/test/test_dataset_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2023-11-13 20:31:58.000000 kdp-api-python-client-4.98.0/test/test_dataset_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1463 2023-11-13 20:31:58.000000 kdp-api-python-client-4.98.0/test/test_dataset_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1448 2023-11-13 20:31:59.000000 kdp-api-python-client-4.98.0/test/test_dataset_permission.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1541 2023-11-13 20:31:59.000000 kdp-api-python-client-4.98.0/test/test_dataset_permission_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1591 2023-11-13 20:31:59.000000 kdp-api-python-client-4.98.0/test/test_dataset_permission_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1643 2023-11-13 20:31:59.000000 kdp-api-python-client-4.98.0/test/test_dataset_permission_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1534 2023-11-13 20:31:59.000000 kdp-api-python-client-4.98.0/test/test_dataset_permission_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1541 2023-11-13 20:32:00.000000 kdp-api-python-client-4.98.0/test/test_dataset_permission_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2438 2023-11-13 20:32:00.000000 kdp-api-python-client-4.98.0/test/test_dataset_permissions_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1406 2023-11-13 20:32:00.000000 kdp-api-python-client-4.98.0/test/test_dataset_sync.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1525 2023-11-13 20:32:00.000000 kdp-api-python-client-4.98.0/test/test_dataset_sync_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1662 2023-11-13 20:32:00.000000 kdp-api-python-client-4.98.0/test/test_dataset_sync_management_terminate_connection_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1577 2023-11-13 20:32:00.000000 kdp-api-python-client-4.98.0/test/test_dataset_sync_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1492 2023-11-13 20:32:01.000000 kdp-api-python-client-4.98.0/test/test_dataset_sync_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1499 2023-11-13 20:32:01.000000 kdp-api-python-client-4.98.0/test/test_dataset_sync_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2613 2023-11-13 20:32:01.000000 kdp-api-python-client-4.98.0/test/test_dataset_syncs_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1470 2023-11-13 20:32:01.000000 kdp-api-python-client-4.98.0/test/test_dataset_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2193 2023-11-13 20:32:01.000000 kdp-api-python-client-4.98.0/test/test_datasets_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1528 2023-11-13 20:32:02.000000 kdp-api-python-client-4.98.0/test/test_delete_document_by_query_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1493 2023-11-13 20:32:02.000000 kdp-api-python-client-4.98.0/test/test_delete_record_by_id_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1514 2023-11-13 20:32:02.000000 kdp-api-python-client-4.98.0/test/test_delete_record_by_query_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1392 2023-11-13 20:32:02.000000 kdp-api-python-client-4.98.0/test/test_error_code.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1499 2023-11-13 20:32:02.000000 kdp-api-python-client-4.98.0/test/test_get_serve_media200_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1363 2023-11-13 20:32:03.000000 kdp-api-python-client-4.98.0/test/test_group.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1456 2023-11-13 20:32:03.000000 kdp-api-python-client-4.98.0/test/test_group_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1457 2023-11-13 20:32:03.000000 kdp-api-python-client-4.98.0/test/test_group_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1560 2023-11-13 20:32:03.000000 kdp-api-python-client-4.98.0/test/test_group_membership.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1527 2023-11-13 20:32:03.000000 kdp-api-python-client-4.98.0/test/test_group_membership_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1569 2023-11-13 20:32:03.000000 kdp-api-python-client-4.98.0/test/test_group_membership_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1621 2023-11-13 20:32:04.000000 kdp-api-python-client-4.98.0/test/test_group_membership_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1520 2023-11-13 20:32:04.000000 kdp-api-python-client-4.98.0/test/test_group_membership_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1527 2023-11-13 20:32:04.000000 kdp-api-python-client-4.98.0/test/test_group_membership_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2423 2023-11-13 20:32:04.000000 kdp-api-python-client-4.98.0/test/test_group_memberships_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1509 2023-11-13 20:32:04.000000 kdp-api-python-client-4.98.0/test/test_group_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1449 2023-11-13 20:32:05.000000 kdp-api-python-client-4.98.0/test/test_group_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1456 2023-11-13 20:32:05.000000 kdp-api-python-client-4.98.0/test/test_group_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2191 2023-11-13 20:32:05.000000 kdp-api-python-client-4.98.0/test/test_groups_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1363 2023-11-13 20:32:05.000000 kdp-api-python-client-4.98.0/test/test_index.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1457 2023-11-13 20:32:05.000000 kdp-api-python-client-4.98.0/test/test_index_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1509 2023-11-13 20:32:06.000000 kdp-api-python-client-4.98.0/test/test_index_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2163 2023-11-13 20:32:06.000000 kdp-api-python-client-4.98.0/test/test_indexes_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1368 2023-11-13 20:32:06.000000 kdp-api-python-client-4.98.0/test/test_ingest_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1574 2023-11-13 20:32:06.000000 kdp-api-python-client-4.98.0/test/test_ingest_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1349 2023-11-13 20:32:06.000000 kdp-api-python-client-4.98.0/test/test_job.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1435 2023-11-13 20:32:06.000000 kdp-api-python-client-4.98.0/test/test_job_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1487 2023-11-13 20:32:07.000000 kdp-api-python-client-4.98.0/test/test_job_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1956 2023-11-13 20:32:07.000000 kdp-api-python-client-4.98.0/test/test_jobs_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1399 2023-11-13 20:32:07.000000 kdp-api-python-client-4.98.0/test/test_json_record.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1533 2023-11-13 20:32:07.000000 kdp-api-python-client-4.98.0/test/test_keycloak_provider_configuration.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1491 2023-11-13 20:32:08.000000 kdp-api-python-client-4.98.0/test/test_koverse_document_metadata.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1456 2023-11-13 20:32:08.000000 kdp-api-python-client-4.98.0/test/test_lucene_query_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1542 2023-11-13 20:32:08.000000 kdp-api-python-client-4.98.0/test/test_origin_dataset_sync_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1363 2023-11-13 20:32:08.000000 kdp-api-python-client-4.98.0/test/test_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1890 2023-11-13 20:32:08.000000 kdp-api-python-client-4.98.0/test/test_query_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1651 2023-11-13 20:32:08.000000 kdp-api-python-client-4.98.0/test/test_query_datasets_summary.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1563 2023-11-13 20:32:09.000000 kdp-api-python-client-4.98.0/test/test_query_datasets_summary_datasets_inner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1520 2023-11-13 20:32:09.000000 kdp-api-python-client-4.98.0/test/test_query_datasets_summary_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1513 2023-11-13 20:32:09.000000 kdp-api-python-client-4.98.0/test/test_query_document_lucene_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1726 2023-11-13 20:32:09.000000 kdp-api-python-client-4.98.0/test/test_query_document_lucene_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1745 2023-11-13 20:32:09.000000 kdp-api-python-client-4.98.0/test/test_query_document_lucene_response_records_inner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1676 2023-11-13 20:32:10.000000 kdp-api-python-client-4.98.0/test/test_read_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1442 2023-11-13 20:32:10.000000 kdp-api-python-client-4.98.0/test/test_read_range_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1492 2023-11-13 20:32:10.000000 kdp-api-python-client-4.98.0/test/test_record_batch.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1492 2023-11-13 20:32:10.000000 kdp-api-python-client-4.98.0/test/test_reindex_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1549 2023-11-13 20:32:10.000000 kdp-api-python-client-4.98.0/test/test_replica_dataset_sync_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1492 2023-11-13 20:32:11.000000 kdp-api-python-client-4.98.0/test/test_security_label_info_params.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1377 2023-11-13 20:32:11.000000 kdp-api-python-client-4.98.0/test/test_segment.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1479 2023-11-13 20:32:11.000000 kdp-api-python-client-4.98.0/test/test_segment_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2023-11-13 20:32:11.000000 kdp-api-python-client-4.98.0/test/test_segment_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1550 2023-11-13 20:32:11.000000 kdp-api-python-client-4.98.0/test/test_segments_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1463 2023-11-13 20:32:11.000000 kdp-api-python-client-4.98.0/test/test_sequence_read_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1464 2023-11-13 20:32:12.000000 kdp-api-python-client-4.98.0/test/test_serve_media_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1406 2023-11-13 20:32:12.000000 kdp-api-python-client-4.98.0/test/test_source_types.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1588 2023-11-13 20:32:12.000000 kdp-api-python-client-4.98.0/test/test_source_types_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1525 2023-11-13 20:32:12.000000 kdp-api-python-client-4.98.0/test/test_source_types_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1406 2023-11-13 20:32:12.000000 kdp-api-python-client-4.98.0/test/test_split_points.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1994 2023-11-13 20:32:12.000000 kdp-api-python-client-4.98.0/test/test_storage_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1456 2023-11-13 20:32:13.000000 kdp-api-python-client-4.98.0/test/test_stripe_latest_charge.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1463 2023-11-13 20:32:13.000000 kdp-api-python-client-4.98.0/test/test_stripe_latest_charge1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1500 2023-11-13 20:32:13.000000 kdp-api-python-client-4.98.0/test/test_sync_kafka_consumer_group_id.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1435 2023-11-13 20:32:13.000000 kdp-api-python-client-4.98.0/test/test_sync_setup_origin.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1442 2023-11-13 20:32:14.000000 kdp-api-python-client-4.98.0/test/test_sync_setup_replica.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1609 2023-11-13 20:32:14.000000 kdp-api-python-client-4.98.0/test/test_terminate_connection_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1491 2023-11-13 20:32:14.000000 kdp-api-python-client-4.98.0/test/test_transfer_resource_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1659 2023-11-13 20:32:14.000000 kdp-api-python-client-4.98.0/test/test_transfer_resource_request_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1546 2023-11-13 20:32:14.000000 kdp-api-python-client-4.98.0/test/test_upload_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1375 2023-11-13 20:32:14.000000 kdp-api-python-client-4.98.0/test/test_uploads_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1479 2023-11-13 20:32:15.000000 kdp-api-python-client-4.98.0/test/test_user.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1449 2023-11-13 20:32:15.000000 kdp-api-python-client-4.98.0/test/test_user_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-11-13 20:32:15.000000 kdp-api-python-client-4.98.0/test/test_user_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-11-13 20:32:15.000000 kdp-api-python-client-4.98.0/test/test_user_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1561 2023-11-13 20:32:15.000000 kdp-api-python-client-4.98.0/test/test_user_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1449 2023-11-13 20:32:16.000000 kdp-api-python-client-4.98.0/test/test_user_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-11-13 20:32:16.000000 kdp-api-python-client-4.98.0/test/test_users_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1521 2023-11-13 20:32:16.000000 kdp-api-python-client-4.98.0/test/test_workspace.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1668 2023-11-13 20:32:16.000000 kdp-api-python-client-4.98.0/test/test_workspace_create_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1832 2023-11-13 20:32:16.000000 kdp-api-python-client-4.98.0/test/test_workspace_create_request_subscription.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1705 2023-11-13 20:32:16.000000 kdp-api-python-client-4.98.0/test/test_workspace_create_request_subscription_subscription_item_ids.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-11-13 20:32:17.000000 kdp-api-python-client-4.98.0/test/test_workspace_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1553 2023-11-13 20:32:17.000000 kdp-api-python-client-4.98.0/test/test_workspace_paginator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1661 2023-11-13 20:32:17.000000 kdp-api-python-client-4.98.0/test/test_workspace_patch_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1685 2023-11-13 20:32:17.000000 kdp-api-python-client-4.98.0/test/test_workspace_subscription.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1612 2023-11-13 20:32:17.000000 kdp-api-python-client-4.98.0/test/test_workspace_subscription_subscription_item_ids.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1668 2023-11-13 20:32:18.000000 kdp-api-python-client-4.98.0/test/test_workspace_update_request.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2073 2023-11-13 20:32:18.000000 kdp-api-python-client-4.98.0/test/test_workspaces_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1507 2023-11-13 20:32:18.000000 kdp-api-python-client-4.98.0/test/test_write_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1456 2023-11-13 20:32:18.000000 kdp-api-python-client-4.98.0/test/test_write_batch_response.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:45:45.690517 kdp-api-python-client-4.99.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1183 2023-11-13 20:45:45.690517 kdp-api-python-client-4.99.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27758 2023-11-13 20:43:55.000000 kdp-api-python-client-4.99.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:45:45.602517 kdp-api-python-client-4.99.0/kdp_api/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1372 2023-11-13 20:44:27.000000 kdp-api-python-client-4.99.0/kdp_api/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:45:45.610517 kdp-api-python-client-4.99.0/kdp_api/api/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      220 2023-11-13 20:44:28.000000 kdp-api-python-client-4.99.0/kdp_api/api/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12487 2023-11-13 20:44:28.000000 kdp-api-python-client-4.99.0/kdp_api/api/abac_label_parsers_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33506 2023-11-13 20:44:28.000000 kdp-api-python-client-4.99.0/kdp_api/api/applications_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35353 2023-11-13 20:44:28.000000 kdp-api-python-client-4.99.0/kdp_api/api/attribute_assignments_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33299 2023-11-13 20:44:29.000000 kdp-api-python-client-4.99.0/kdp_api/api/attributes_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7406 2023-11-13 20:44:29.000000 kdp-api-python-client-4.99.0/kdp_api/api/audit_log_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13991 2023-11-13 20:44:29.000000 kdp-api-python-client-4.99.0/kdp_api/api/audit_log_configs_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17488 2023-11-13 20:44:29.000000 kdp-api-python-client-4.99.0/kdp_api/api/authentication_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34183 2023-11-13 20:44:29.000000 kdp-api-python-client-4.99.0/kdp_api/api/dataset_permissions_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    41536 2023-11-13 20:44:29.000000 kdp-api-python-client-4.99.0/kdp_api/api/dataset_syncs_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33089 2023-11-13 20:44:30.000000 kdp-api-python-client-4.99.0/kdp_api/api/datasets_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34014 2023-11-13 20:44:30.000000 kdp-api-python-client-4.99.0/kdp_api/api/group_memberships_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32929 2023-11-13 20:44:30.000000 kdp-api-python-client-4.99.0/kdp_api/api/groups_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32864 2023-11-13 20:44:30.000000 kdp-api-python-client-4.99.0/kdp_api/api/indexes_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7173 2023-11-13 20:44:30.000000 kdp-api-python-client-4.99.0/kdp_api/api/ingest_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27838 2023-11-13 20:44:30.000000 kdp-api-python-client-4.99.0/kdp_api/api/jobs_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23682 2023-11-13 20:44:31.000000 kdp-api-python-client-4.99.0/kdp_api/api/query_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17576 2023-11-13 20:44:31.000000 kdp-api-python-client-4.99.0/kdp_api/api/read_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13109 2023-11-13 20:44:31.000000 kdp-api-python-client-4.99.0/kdp_api/api/segments_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7384 2023-11-13 20:44:31.000000 kdp-api-python-client-4.99.0/kdp_api/api/serve_media_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12216 2023-11-13 20:44:32.000000 kdp-api-python-client-4.99.0/kdp_api/api/source_types_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23758 2023-11-13 20:44:32.000000 kdp-api-python-client-4.99.0/kdp_api/api/storage_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8316 2023-11-13 20:44:32.000000 kdp-api-python-client-4.99.0/kdp_api/api/uploads_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32806 2023-11-13 20:44:32.000000 kdp-api-python-client-4.99.0/kdp_api/api/users_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28404 2023-11-13 20:44:32.000000 kdp-api-python-client-4.99.0/kdp_api/api/workspaces_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13314 2023-11-13 20:44:32.000000 kdp-api-python-client-4.99.0/kdp_api/api/write_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    39772 2023-11-13 20:44:27.000000 kdp-api-python-client-4.99.0/kdp_api/api_client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:45:45.610517 kdp-api-python-client-4.99.0/kdp_api/apis/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1764 2023-11-13 20:44:33.000000 kdp-api-python-client-4.99.0/kdp_api/apis/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17443 2023-11-13 20:44:27.000000 kdp-api-python-client-4.99.0/kdp_api/configuration.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5759 2023-11-13 20:44:27.000000 kdp-api-python-client-4.99.0/kdp_api/exceptions.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:45:45.646517 kdp-api-python-client-4.99.0/kdp_api/model/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      341 2023-11-13 20:44:33.000000 kdp-api-python-client-4.99.0/kdp_api/model/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12920 2023-11-13 20:44:33.000000 kdp-api-python-client-4.99.0/kdp_api/model/abac_label_parser_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12911 2023-11-13 20:44:33.000000 kdp-api-python-client-4.99.0/kdp_api/model/abac_label_parsers.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12709 2023-11-13 20:44:33.000000 kdp-api-python-client-4.99.0/kdp_api/model/abac_label_parsers_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12924 2023-11-13 20:44:33.000000 kdp-api-python-client-4.99.0/kdp_api/model/access_control_label.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12794 2023-11-13 20:44:34.000000 kdp-api-python-client-4.99.0/kdp_api/model/api_error.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15510 2023-11-13 20:44:34.000000 kdp-api-python-client-4.99.0/kdp_api/model/application.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14946 2023-11-13 20:44:34.000000 kdp-api-python-client-4.99.0/kdp_api/model/application_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12526 2023-11-13 20:44:34.000000 kdp-api-python-client-4.99.0/kdp_api/model/application_create_request_required_dataset_access_inner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12623 2023-11-13 20:44:35.000000 kdp-api-python-client-4.99.0/kdp_api/model/application_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12871 2023-11-13 20:44:35.000000 kdp-api-python-client-4.99.0/kdp_api/model/application_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15143 2023-11-13 20:44:35.000000 kdp-api-python-client-4.99.0/kdp_api/model/application_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12557 2023-11-13 20:44:35.000000 kdp-api-python-client-4.99.0/kdp_api/model/application_required_dataset_access_inner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15482 2023-11-13 20:44:35.000000 kdp-api-python-client-4.99.0/kdp_api/model/application_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13067 2023-11-13 20:44:35.000000 kdp-api-python-client-4.99.0/kdp_api/model/attribute.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13327 2023-11-13 20:44:36.000000 kdp-api-python-client-4.99.0/kdp_api/model/attribute_assignment.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12482 2023-11-13 20:44:36.000000 kdp-api-python-client-4.99.0/kdp_api/model/attribute_assignment_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12756 2023-11-13 20:44:36.000000 kdp-api-python-client-4.99.0/kdp_api/model/attribute_assignment_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12952 2023-11-13 20:44:36.000000 kdp-api-python-client-4.99.0/kdp_api/model/attribute_assignment_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12359 2023-11-13 20:44:36.000000 kdp-api-python-client-4.99.0/kdp_api/model/attribute_assignment_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12650 2023-11-13 20:44:36.000000 kdp-api-python-client-4.99.0/kdp_api/model/attribute_assignment_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12774 2023-11-13 20:44:37.000000 kdp-api-python-client-4.99.0/kdp_api/model/attribute_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12591 2023-11-13 20:44:37.000000 kdp-api-python-client-4.99.0/kdp_api/model/attribute_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12851 2023-11-13 20:44:37.000000 kdp-api-python-client-4.99.0/kdp_api/model/attribute_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12711 2023-11-13 20:44:37.000000 kdp-api-python-client-4.99.0/kdp_api/model/attribute_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12942 2023-11-13 20:44:37.000000 kdp-api-python-client-4.99.0/kdp_api/model/attribute_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13387 2023-11-13 20:44:37.000000 kdp-api-python-client-4.99.0/kdp_api/model/audit_log_configuration.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12793 2023-11-13 20:44:38.000000 kdp-api-python-client-4.99.0/kdp_api/model/audit_log_configuration_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12973 2023-11-13 20:44:38.000000 kdp-api-python-client-4.99.0/kdp_api/model/audit_log_configuration_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15345 2023-11-13 20:44:38.000000 kdp-api-python-client-4.99.0/kdp_api/model/audit_log_event.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12665 2023-11-13 20:44:38.000000 kdp-api-python-client-4.99.0/kdp_api/model/audit_log_event_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12878 2023-11-13 20:44:39.000000 kdp-api-python-client-4.99.0/kdp_api/model/audit_log_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13169 2023-11-13 20:44:39.000000 kdp-api-python-client-4.99.0/kdp_api/model/authentication.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13119 2023-11-13 20:44:39.000000 kdp-api-python-client-4.99.0/kdp_api/model/authentication_details.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12975 2023-11-13 20:44:39.000000 kdp-api-python-client-4.99.0/kdp_api/model/authentication_details_authentication.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13043 2023-11-13 20:44:39.000000 kdp-api-python-client-4.99.0/kdp_api/model/authentication_details_authentication_payload.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15754 2023-11-13 20:44:39.000000 kdp-api-python-client-4.99.0/kdp_api/model/authentication_details_user.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12671 2023-11-13 20:44:40.000000 kdp-api-python-client-4.99.0/kdp_api/model/authentication_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12918 2023-11-13 20:44:40.000000 kdp-api-python-client-4.99.0/kdp_api/model/authentication_sso.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12916 2023-11-13 20:44:40.000000 kdp-api-python-client-4.99.0/kdp_api/model/batch_write_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13570 2023-11-13 20:44:40.000000 kdp-api-python-client-4.99.0/kdp_api/model/connection_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13580 2023-11-13 20:44:41.000000 kdp-api-python-client-4.99.0/kdp_api/model/custom_identity_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12809 2023-11-13 20:44:40.000000 kdp-api-python-client-4.99.0/kdp_api/model/custom_identity_provider_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13619 2023-11-13 20:44:41.000000 kdp-api-python-client-4.99.0/kdp_api/model/data_source_params.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14962 2023-11-13 20:44:41.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13729 2023-11-13 20:44:41.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12656 2023-11-13 20:44:41.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_current_user_permissions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12559 2023-11-13 20:44:42.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12831 2023-11-13 20:44:42.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13575 2023-11-13 20:44:42.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13168 2023-11-13 20:44:42.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_permission.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12801 2023-11-13 20:44:42.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_permission_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12724 2023-11-13 20:44:42.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_permission_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12932 2023-11-13 20:44:43.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_permission_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12660 2023-11-13 20:44:43.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_permission_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12969 2023-11-13 20:44:43.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_permission_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17860 2023-11-13 20:44:43.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_sync.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12628 2023-11-13 20:44:43.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_sync_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12713 2023-11-13 20:44:43.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_sync_management_terminate_connection_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12872 2023-11-13 20:44:44.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_sync_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17896 2023-11-13 20:44:44.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_sync_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18371 2023-11-13 20:44:44.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_sync_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13620 2023-11-13 20:44:44.000000 kdp-api-python-client-4.99.0/kdp_api/model/dataset_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12290 2023-11-13 20:44:44.000000 kdp-api-python-client-4.99.0/kdp_api/model/delete_document_by_query_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13005 2023-11-13 20:44:45.000000 kdp-api-python-client-4.99.0/kdp_api/model/delete_record_by_id_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12280 2023-11-13 20:44:45.000000 kdp-api-python-client-4.99.0/kdp_api/model/delete_record_by_query_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14657 2023-11-13 20:44:45.000000 kdp-api-python-client-4.99.0/kdp_api/model/error_code.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12148 2023-11-13 20:44:45.000000 kdp-api-python-client-4.99.0/kdp_api/model/get_serve_media200_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13380 2023-11-13 20:44:45.000000 kdp-api-python-client-4.99.0/kdp_api/model/group.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13022 2023-11-13 20:44:46.000000 kdp-api-python-client-4.99.0/kdp_api/model/group_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12527 2023-11-13 20:44:46.000000 kdp-api-python-client-4.99.0/kdp_api/model/group_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13535 2023-11-13 20:44:46.000000 kdp-api-python-client-4.99.0/kdp_api/model/group_membership.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12710 2023-11-13 20:44:46.000000 kdp-api-python-client-4.99.0/kdp_api/model/group_membership_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12692 2023-11-13 20:44:46.000000 kdp-api-python-client-4.99.0/kdp_api/model/group_membership_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12912 2023-11-13 20:44:47.000000 kdp-api-python-client-4.99.0/kdp_api/model/group_membership_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12599 2023-11-13 20:44:47.000000 kdp-api-python-client-4.99.0/kdp_api/model/group_membership_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12878 2023-11-13 20:44:47.000000 kdp-api-python-client-4.99.0/kdp_api/model/group_membership_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12811 2023-11-13 20:44:47.000000 kdp-api-python-client-4.99.0/kdp_api/model/group_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12700 2023-11-13 20:44:47.000000 kdp-api-python-client-4.99.0/kdp_api/model/group_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13022 2023-11-13 20:44:48.000000 kdp-api-python-client-4.99.0/kdp_api/model/group_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12615 2023-11-13 20:44:48.000000 kdp-api-python-client-4.99.0/kdp_api/model/index.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12531 2023-11-13 20:44:48.000000 kdp-api-python-client-4.99.0/kdp_api/model/index_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12811 2023-11-13 20:44:48.000000 kdp-api-python-client-4.99.0/kdp_api/model/index_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12721 2023-11-13 20:44:48.000000 kdp-api-python-client-4.99.0/kdp_api/model/ingest_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15045 2023-11-13 20:44:48.000000 kdp-api-python-client-4.99.0/kdp_api/model/job.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12495 2023-11-13 20:44:49.000000 kdp-api-python-client-4.99.0/kdp_api/model/job_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12791 2023-11-13 20:44:49.000000 kdp-api-python-client-4.99.0/kdp_api/model/job_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11896 2023-11-13 20:44:49.000000 kdp-api-python-client-4.99.0/kdp_api/model/json_record.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14576 2023-11-13 20:44:49.000000 kdp-api-python-client-4.99.0/kdp_api/model/keycloak_provider_configuration.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14479 2023-11-13 20:44:49.000000 kdp-api-python-client-4.99.0/kdp_api/model/koverse_document_metadata.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13782 2023-11-13 20:44:49.000000 kdp-api-python-client-4.99.0/kdp_api/model/lucene_query_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13306 2023-11-13 20:44:50.000000 kdp-api-python-client-4.99.0/kdp_api/model/origin_dataset_sync_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13885 2023-11-13 20:44:50.000000 kdp-api-python-client-4.99.0/kdp_api/model/query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13835 2023-11-13 20:44:50.000000 kdp-api-python-client-4.99.0/kdp_api/model/query_datasets_summary.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12747 2023-11-13 20:44:50.000000 kdp-api-python-client-4.99.0/kdp_api/model/query_datasets_summary_datasets_inner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13844 2023-11-13 20:44:50.000000 kdp-api-python-client-4.99.0/kdp_api/model/query_datasets_summary_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13806 2023-11-13 20:44:51.000000 kdp-api-python-client-4.99.0/kdp_api/model/query_document_lucene_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12946 2023-11-13 20:44:51.000000 kdp-api-python-client-4.99.0/kdp_api/model/query_document_lucene_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13854 2023-11-13 20:44:51.000000 kdp-api-python-client-4.99.0/kdp_api/model/query_document_lucene_response_records_inner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14704 2023-11-13 20:44:51.000000 kdp-api-python-client-4.99.0/kdp_api/model/read_range_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13528 2023-11-13 20:44:51.000000 kdp-api-python-client-4.99.0/kdp_api/model/record_batch.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13059 2023-11-13 20:44:52.000000 kdp-api-python-client-4.99.0/kdp_api/model/reindex_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13619 2023-11-13 20:44:52.000000 kdp-api-python-client-4.99.0/kdp_api/model/replica_dataset_sync_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13998 2023-11-13 20:44:52.000000 kdp-api-python-client-4.99.0/kdp_api/model/security_label_info_params.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14682 2023-11-13 20:44:52.000000 kdp-api-python-client-4.99.0/kdp_api/model/segment.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12559 2023-11-13 20:44:52.000000 kdp-api-python-client-4.99.0/kdp_api/model/segment_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12831 2023-11-13 20:44:52.000000 kdp-api-python-client-4.99.0/kdp_api/model/segment_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13409 2023-11-13 20:44:53.000000 kdp-api-python-client-4.99.0/kdp_api/model/sequence_read_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12758 2023-11-13 20:44:53.000000 kdp-api-python-client-4.99.0/kdp_api/model/source_types.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12624 2023-11-13 20:44:53.000000 kdp-api-python-client-4.99.0/kdp_api/model/source_types_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12564 2023-11-13 20:44:53.000000 kdp-api-python-client-4.99.0/kdp_api/model/split_points.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13047 2023-11-13 20:44:53.000000 kdp-api-python-client-4.99.0/kdp_api/model/stripe_latest_charge.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13348 2023-11-13 20:44:54.000000 kdp-api-python-client-4.99.0/kdp_api/model/stripe_latest_charge1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13034 2023-11-13 20:44:54.000000 kdp-api-python-client-4.99.0/kdp_api/model/sync_kafka_consumer_group_id.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15181 2023-11-13 20:44:54.000000 kdp-api-python-client-4.99.0/kdp_api/model/sync_setup_origin.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15184 2023-11-13 20:44:54.000000 kdp-api-python-client-4.99.0/kdp_api/model/sync_setup_replica.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12800 2023-11-13 20:44:54.000000 kdp-api-python-client-4.99.0/kdp_api/model/terminate_connection_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14142 2023-11-13 20:44:54.000000 kdp-api-python-client-4.99.0/kdp_api/model/transfer_resource_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12825 2023-11-13 20:44:55.000000 kdp-api-python-client-4.99.0/kdp_api/model/transfer_resource_request_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13602 2023-11-13 20:44:55.000000 kdp-api-python-client-4.99.0/kdp_api/model/upload_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14107 2023-11-13 20:44:55.000000 kdp-api-python-client-4.99.0/kdp_api/model/user.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13823 2023-11-13 20:44:55.000000 kdp-api-python-client-4.99.0/kdp_api/model/user_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12511 2023-11-13 20:44:55.000000 kdp-api-python-client-4.99.0/kdp_api/model/user_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12801 2023-11-13 20:44:56.000000 kdp-api-python-client-4.99.0/kdp_api/model/user_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13844 2023-11-13 20:44:56.000000 kdp-api-python-client-4.99.0/kdp_api/model/user_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14221 2023-11-13 20:44:56.000000 kdp-api-python-client-4.99.0/kdp_api/model/user_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13348 2023-11-13 20:44:56.000000 kdp-api-python-client-4.99.0/kdp_api/model/workspace.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13070 2023-11-13 20:44:56.000000 kdp-api-python-client-4.99.0/kdp_api/model/workspace_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14612 2023-11-13 20:44:57.000000 kdp-api-python-client-4.99.0/kdp_api/model/workspace_create_request_subscription.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12773 2023-11-13 20:44:57.000000 kdp-api-python-client-4.99.0/kdp_api/model/workspace_create_request_subscription_subscription_item_ids.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12591 2023-11-13 20:44:57.000000 kdp-api-python-client-4.99.0/kdp_api/model/workspace_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12851 2023-11-13 20:44:57.000000 kdp-api-python-client-4.99.0/kdp_api/model/workspace_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13025 2023-11-13 20:44:57.000000 kdp-api-python-client-4.99.0/kdp_api/model/workspace_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14774 2023-11-13 20:44:57.000000 kdp-api-python-client-4.99.0/kdp_api/model/workspace_subscription.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12734 2023-11-13 20:44:58.000000 kdp-api-python-client-4.99.0/kdp_api/model/workspace_subscription_subscription_item_ids.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13070 2023-11-13 20:44:58.000000 kdp-api-python-client-4.99.0/kdp_api/model/workspace_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12731 2023-11-13 20:44:58.000000 kdp-api-python-client-4.99.0/kdp_api/model/write_batch_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    83279 2023-11-13 20:44:28.000000 kdp-api-python-client-4.99.0/kdp_api/model_utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:45:45.646517 kdp-api-python-client-4.99.0/kdp_api/models/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9984 2023-11-13 20:44:58.000000 kdp-api-python-client-4.99.0/kdp_api/models/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14956 2023-11-13 20:44:27.000000 kdp-api-python-client-4.99.0/kdp_api/rest.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:45:45.646517 kdp-api-python-client-4.99.0/kdp_api_python_client.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1183 2023-11-13 20:45:45.000000 kdp-api-python-client-4.99.0/kdp_api_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12374 2023-11-13 20:45:45.000000 kdp-api-python-client-4.99.0/kdp_api_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-11-13 20:45:45.000000 kdp-api-python-client-4.99.0/kdp_api_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       32 2023-11-13 20:45:45.000000 kdp-api-python-client-4.99.0/kdp_api_python_client.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-11-13 20:45:45.000000 kdp-api-python-client-4.99.0/kdp_api_python_client.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       69 2023-11-13 20:45:45.690517 kdp-api-python-client-4.99.0/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2524 2023-11-13 20:43:56.000000 kdp-api-python-client-4.99.0/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-13 20:45:45.690517 kdp-api-python-client-4.99.0/test/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1627 2023-11-13 20:44:59.000000 kdp-api-python-client-4.99.0/test/test_abac_label_parser_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1442 2023-11-13 20:44:59.000000 kdp-api-python-client-4.99.0/test/test_abac_label_parsers.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1652 2023-11-13 20:44:59.000000 kdp-api-python-client-4.99.0/test/test_abac_label_parsers_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1582 2023-11-13 20:44:59.000000 kdp-api-python-client-4.99.0/test/test_abac_label_parsers_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1596 2023-11-13 20:44:59.000000 kdp-api-python-client-4.99.0/test/test_access_control_label.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1385 2023-11-13 20:45:00.000000 kdp-api-python-client-4.99.0/test/test_api_error.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1602 2023-11-13 20:45:00.000000 kdp-api-python-client-4.99.0/test/test_application.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1749 2023-11-13 20:45:00.000000 kdp-api-python-client-4.99.0/test/test_application_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1684 2023-11-13 20:45:00.000000 kdp-api-python-client-4.99.0/test/test_application_create_request_required_dataset_access_inner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1523 2023-11-13 20:45:00.000000 kdp-api-python-client-4.99.0/test/test_application_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1575 2023-11-13 20:45:00.000000 kdp-api-python-client-4.99.0/test/test_application_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1742 2023-11-13 20:45:01.000000 kdp-api-python-client-4.99.0/test/test_application_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1591 2023-11-13 20:45:01.000000 kdp-api-python-client-4.99.0/test/test_application_required_dataset_access_inner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1749 2023-11-13 20:45:01.000000 kdp-api-python-client-4.99.0/test/test_application_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2294 2023-11-13 20:45:01.000000 kdp-api-python-client-4.99.0/test/test_applications_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1391 2023-11-13 20:45:01.000000 kdp-api-python-client-4.99.0/test/test_attribute.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1604 2023-11-13 20:45:02.000000 kdp-api-python-client-4.99.0/test/test_attribute_assignment.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1555 2023-11-13 20:45:02.000000 kdp-api-python-client-4.99.0/test/test_attribute_assignment_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1613 2023-11-13 20:45:02.000000 kdp-api-python-client-4.99.0/test/test_attribute_assignment_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1665 2023-11-13 20:45:02.000000 kdp-api-python-client-4.99.0/test/test_attribute_assignment_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1548 2023-11-13 20:45:02.000000 kdp-api-python-client-4.99.0/test/test_attribute_assignment_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1555 2023-11-13 20:45:02.000000 kdp-api-python-client-4.99.0/test/test_attribute_assignment_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2479 2023-11-13 20:45:03.000000 kdp-api-python-client-4.99.0/test/test_attribute_assignments_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1484 2023-11-13 20:45:03.000000 kdp-api-python-client-4.99.0/test/test_attribute_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-11-13 20:45:03.000000 kdp-api-python-client-4.99.0/test/test_attribute_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1553 2023-11-13 20:45:03.000000 kdp-api-python-client-4.99.0/test/test_attribute_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1477 2023-11-13 20:45:03.000000 kdp-api-python-client-4.99.0/test/test_attribute_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1484 2023-11-13 20:45:04.000000 kdp-api-python-client-4.99.0/test/test_attribute_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2245 2023-11-13 20:45:04.000000 kdp-api-python-client-4.99.0/test/test_attributes_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1403 2023-11-13 20:45:04.000000 kdp-api-python-client-4.99.0/test/test_audit_log_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1659 2023-11-13 20:45:04.000000 kdp-api-python-client-4.99.0/test/test_audit_log_configs_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1477 2023-11-13 20:45:04.000000 kdp-api-python-client-4.99.0/test/test_audit_log_configuration.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1637 2023-11-13 20:45:04.000000 kdp-api-python-client-4.99.0/test/test_audit_log_configuration_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1689 2023-11-13 20:45:05.000000 kdp-api-python-client-4.99.0/test/test_audit_log_configuration_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1421 2023-11-13 20:45:05.000000 kdp-api-python-client-4.99.0/test/test_audit_log_event.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1549 2023-11-13 20:45:05.000000 kdp-api-python-client-4.99.0/test/test_audit_log_event_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1565 2023-11-13 20:45:05.000000 kdp-api-python-client-4.99.0/test/test_audit_log_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1426 2023-11-13 20:45:05.000000 kdp-api-python-client-4.99.0/test/test_authentication.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1845 2023-11-13 20:45:06.000000 kdp-api-python-client-4.99.0/test/test_authentication_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1810 2023-11-13 20:45:06.000000 kdp-api-python-client-4.99.0/test/test_authentication_details.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1791 2023-11-13 20:45:06.000000 kdp-api-python-client-4.99.0/test/test_authentication_details_authentication.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1625 2023-11-13 20:45:06.000000 kdp-api-python-client-4.99.0/test/test_authentication_details_authentication_payload.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1505 2023-11-13 20:45:06.000000 kdp-api-python-client-4.99.0/test/test_authentication_details_user.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1556 2023-11-13 20:45:07.000000 kdp-api-python-client-4.99.0/test/test_authentication_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1448 2023-11-13 20:45:07.000000 kdp-api-python-client-4.99.0/test/test_authentication_sso.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1589 2023-11-13 20:45:07.000000 kdp-api-python-client-4.99.0/test/test_batch_write_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1427 2023-11-13 20:45:07.000000 kdp-api-python-client-4.99.0/test/test_connection_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-11-13 20:45:07.000000 kdp-api-python-client-4.99.0/test/test_custom_identity_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1648 2023-11-13 20:45:07.000000 kdp-api-python-client-4.99.0/test/test_custom_identity_provider_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1684 2023-11-13 20:45:08.000000 kdp-api-python-client-4.99.0/test/test_data_source_params.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1541 2023-11-13 20:45:08.000000 kdp-api-python-client-4.99.0/test/test_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1470 2023-11-13 20:45:08.000000 kdp-api-python-client-4.99.0/test/test_dataset_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1534 2023-11-13 20:45:08.000000 kdp-api-python-client-4.99.0/test/test_dataset_current_user_permissions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1479 2023-11-13 20:45:08.000000 kdp-api-python-client-4.99.0/test/test_dataset_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2023-11-13 20:45:09.000000 kdp-api-python-client-4.99.0/test/test_dataset_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1463 2023-11-13 20:45:09.000000 kdp-api-python-client-4.99.0/test/test_dataset_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1448 2023-11-13 20:45:09.000000 kdp-api-python-client-4.99.0/test/test_dataset_permission.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1541 2023-11-13 20:45:09.000000 kdp-api-python-client-4.99.0/test/test_dataset_permission_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1591 2023-11-13 20:45:09.000000 kdp-api-python-client-4.99.0/test/test_dataset_permission_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1643 2023-11-13 20:45:10.000000 kdp-api-python-client-4.99.0/test/test_dataset_permission_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1534 2023-11-13 20:45:10.000000 kdp-api-python-client-4.99.0/test/test_dataset_permission_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1541 2023-11-13 20:45:10.000000 kdp-api-python-client-4.99.0/test/test_dataset_permission_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2438 2023-11-13 20:45:10.000000 kdp-api-python-client-4.99.0/test/test_dataset_permissions_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1406 2023-11-13 20:45:10.000000 kdp-api-python-client-4.99.0/test/test_dataset_sync.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1525 2023-11-13 20:45:10.000000 kdp-api-python-client-4.99.0/test/test_dataset_sync_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1662 2023-11-13 20:45:11.000000 kdp-api-python-client-4.99.0/test/test_dataset_sync_management_terminate_connection_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1577 2023-11-13 20:45:11.000000 kdp-api-python-client-4.99.0/test/test_dataset_sync_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1492 2023-11-13 20:45:11.000000 kdp-api-python-client-4.99.0/test/test_dataset_sync_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1499 2023-11-13 20:45:11.000000 kdp-api-python-client-4.99.0/test/test_dataset_sync_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2613 2023-11-13 20:45:11.000000 kdp-api-python-client-4.99.0/test/test_dataset_syncs_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1470 2023-11-13 20:45:12.000000 kdp-api-python-client-4.99.0/test/test_dataset_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2193 2023-11-13 20:45:12.000000 kdp-api-python-client-4.99.0/test/test_datasets_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1528 2023-11-13 20:45:12.000000 kdp-api-python-client-4.99.0/test/test_delete_document_by_query_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1493 2023-11-13 20:45:12.000000 kdp-api-python-client-4.99.0/test/test_delete_record_by_id_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1514 2023-11-13 20:45:12.000000 kdp-api-python-client-4.99.0/test/test_delete_record_by_query_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1392 2023-11-13 20:45:13.000000 kdp-api-python-client-4.99.0/test/test_error_code.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1499 2023-11-13 20:45:13.000000 kdp-api-python-client-4.99.0/test/test_get_serve_media200_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1363 2023-11-13 20:45:13.000000 kdp-api-python-client-4.99.0/test/test_group.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1456 2023-11-13 20:45:13.000000 kdp-api-python-client-4.99.0/test/test_group_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1457 2023-11-13 20:45:13.000000 kdp-api-python-client-4.99.0/test/test_group_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1560 2023-11-13 20:45:13.000000 kdp-api-python-client-4.99.0/test/test_group_membership.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1527 2023-11-13 20:45:14.000000 kdp-api-python-client-4.99.0/test/test_group_membership_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1569 2023-11-13 20:45:14.000000 kdp-api-python-client-4.99.0/test/test_group_membership_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1621 2023-11-13 20:45:14.000000 kdp-api-python-client-4.99.0/test/test_group_membership_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1520 2023-11-13 20:45:14.000000 kdp-api-python-client-4.99.0/test/test_group_membership_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1527 2023-11-13 20:45:15.000000 kdp-api-python-client-4.99.0/test/test_group_membership_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2423 2023-11-13 20:45:15.000000 kdp-api-python-client-4.99.0/test/test_group_memberships_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1509 2023-11-13 20:45:15.000000 kdp-api-python-client-4.99.0/test/test_group_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1449 2023-11-13 20:45:15.000000 kdp-api-python-client-4.99.0/test/test_group_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1456 2023-11-13 20:45:15.000000 kdp-api-python-client-4.99.0/test/test_group_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2191 2023-11-13 20:45:15.000000 kdp-api-python-client-4.99.0/test/test_groups_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1363 2023-11-13 20:45:16.000000 kdp-api-python-client-4.99.0/test/test_index.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1457 2023-11-13 20:45:16.000000 kdp-api-python-client-4.99.0/test/test_index_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1509 2023-11-13 20:45:16.000000 kdp-api-python-client-4.99.0/test/test_index_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2163 2023-11-13 20:45:16.000000 kdp-api-python-client-4.99.0/test/test_indexes_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1368 2023-11-13 20:45:16.000000 kdp-api-python-client-4.99.0/test/test_ingest_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1574 2023-11-13 20:45:16.000000 kdp-api-python-client-4.99.0/test/test_ingest_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1349 2023-11-13 20:45:17.000000 kdp-api-python-client-4.99.0/test/test_job.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1435 2023-11-13 20:45:17.000000 kdp-api-python-client-4.99.0/test/test_job_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1487 2023-11-13 20:45:17.000000 kdp-api-python-client-4.99.0/test/test_job_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1956 2023-11-13 20:45:17.000000 kdp-api-python-client-4.99.0/test/test_jobs_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1399 2023-11-13 20:45:17.000000 kdp-api-python-client-4.99.0/test/test_json_record.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1533 2023-11-13 20:45:18.000000 kdp-api-python-client-4.99.0/test/test_keycloak_provider_configuration.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1491 2023-11-13 20:45:18.000000 kdp-api-python-client-4.99.0/test/test_koverse_document_metadata.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1456 2023-11-13 20:45:18.000000 kdp-api-python-client-4.99.0/test/test_lucene_query_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1542 2023-11-13 20:45:18.000000 kdp-api-python-client-4.99.0/test/test_origin_dataset_sync_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1363 2023-11-13 20:45:18.000000 kdp-api-python-client-4.99.0/test/test_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1890 2023-11-13 20:45:19.000000 kdp-api-python-client-4.99.0/test/test_query_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1651 2023-11-13 20:45:19.000000 kdp-api-python-client-4.99.0/test/test_query_datasets_summary.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1563 2023-11-13 20:45:19.000000 kdp-api-python-client-4.99.0/test/test_query_datasets_summary_datasets_inner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1520 2023-11-13 20:45:19.000000 kdp-api-python-client-4.99.0/test/test_query_datasets_summary_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1513 2023-11-13 20:45:19.000000 kdp-api-python-client-4.99.0/test/test_query_document_lucene_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1726 2023-11-13 20:45:19.000000 kdp-api-python-client-4.99.0/test/test_query_document_lucene_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1745 2023-11-13 20:45:20.000000 kdp-api-python-client-4.99.0/test/test_query_document_lucene_response_records_inner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1676 2023-11-13 20:45:20.000000 kdp-api-python-client-4.99.0/test/test_read_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1442 2023-11-13 20:45:20.000000 kdp-api-python-client-4.99.0/test/test_read_range_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1492 2023-11-13 20:45:20.000000 kdp-api-python-client-4.99.0/test/test_record_batch.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1492 2023-11-13 20:45:20.000000 kdp-api-python-client-4.99.0/test/test_reindex_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1549 2023-11-13 20:45:20.000000 kdp-api-python-client-4.99.0/test/test_replica_dataset_sync_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1492 2023-11-13 20:45:21.000000 kdp-api-python-client-4.99.0/test/test_security_label_info_params.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1377 2023-11-13 20:45:21.000000 kdp-api-python-client-4.99.0/test/test_segment.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1479 2023-11-13 20:45:21.000000 kdp-api-python-client-4.99.0/test/test_segment_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2023-11-13 20:45:21.000000 kdp-api-python-client-4.99.0/test/test_segment_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1550 2023-11-13 20:45:21.000000 kdp-api-python-client-4.99.0/test/test_segments_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1463 2023-11-13 20:45:21.000000 kdp-api-python-client-4.99.0/test/test_sequence_read_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1464 2023-11-13 20:45:22.000000 kdp-api-python-client-4.99.0/test/test_serve_media_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1406 2023-11-13 20:45:22.000000 kdp-api-python-client-4.99.0/test/test_source_types.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1588 2023-11-13 20:45:22.000000 kdp-api-python-client-4.99.0/test/test_source_types_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1525 2023-11-13 20:45:22.000000 kdp-api-python-client-4.99.0/test/test_source_types_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1406 2023-11-13 20:45:23.000000 kdp-api-python-client-4.99.0/test/test_split_points.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1994 2023-11-13 20:45:23.000000 kdp-api-python-client-4.99.0/test/test_storage_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1456 2023-11-13 20:45:23.000000 kdp-api-python-client-4.99.0/test/test_stripe_latest_charge.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1463 2023-11-13 20:45:23.000000 kdp-api-python-client-4.99.0/test/test_stripe_latest_charge1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1500 2023-11-13 20:45:23.000000 kdp-api-python-client-4.99.0/test/test_sync_kafka_consumer_group_id.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1435 2023-11-13 20:45:23.000000 kdp-api-python-client-4.99.0/test/test_sync_setup_origin.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1442 2023-11-13 20:45:24.000000 kdp-api-python-client-4.99.0/test/test_sync_setup_replica.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1609 2023-11-13 20:45:24.000000 kdp-api-python-client-4.99.0/test/test_terminate_connection_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1491 2023-11-13 20:45:24.000000 kdp-api-python-client-4.99.0/test/test_transfer_resource_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1659 2023-11-13 20:45:24.000000 kdp-api-python-client-4.99.0/test/test_transfer_resource_request_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1546 2023-11-13 20:45:24.000000 kdp-api-python-client-4.99.0/test/test_upload_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1375 2023-11-13 20:45:24.000000 kdp-api-python-client-4.99.0/test/test_uploads_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1479 2023-11-13 20:45:25.000000 kdp-api-python-client-4.99.0/test/test_user.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1449 2023-11-13 20:45:25.000000 kdp-api-python-client-4.99.0/test/test_user_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-11-13 20:45:25.000000 kdp-api-python-client-4.99.0/test/test_user_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-11-13 20:45:25.000000 kdp-api-python-client-4.99.0/test/test_user_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1561 2023-11-13 20:45:25.000000 kdp-api-python-client-4.99.0/test/test_user_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1449 2023-11-13 20:45:25.000000 kdp-api-python-client-4.99.0/test/test_user_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-11-13 20:45:26.000000 kdp-api-python-client-4.99.0/test/test_users_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1521 2023-11-13 20:45:26.000000 kdp-api-python-client-4.99.0/test/test_workspace.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1668 2023-11-13 20:45:26.000000 kdp-api-python-client-4.99.0/test/test_workspace_create_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1832 2023-11-13 20:45:26.000000 kdp-api-python-client-4.99.0/test/test_workspace_create_request_subscription.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1705 2023-11-13 20:45:26.000000 kdp-api-python-client-4.99.0/test/test_workspace_create_request_subscription_subscription_item_ids.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-11-13 20:45:27.000000 kdp-api-python-client-4.99.0/test/test_workspace_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1553 2023-11-13 20:45:27.000000 kdp-api-python-client-4.99.0/test/test_workspace_paginator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1661 2023-11-13 20:45:27.000000 kdp-api-python-client-4.99.0/test/test_workspace_patch_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1685 2023-11-13 20:45:27.000000 kdp-api-python-client-4.99.0/test/test_workspace_subscription.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1612 2023-11-13 20:45:27.000000 kdp-api-python-client-4.99.0/test/test_workspace_subscription_subscription_item_ids.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1668 2023-11-13 20:45:28.000000 kdp-api-python-client-4.99.0/test/test_workspace_update_request.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2073 2023-11-13 20:45:28.000000 kdp-api-python-client-4.99.0/test/test_workspaces_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1507 2023-11-13 20:45:28.000000 kdp-api-python-client-4.99.0/test/test_write_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1456 2023-11-13 20:45:28.000000 kdp-api-python-client-4.99.0/test/test_write_batch_response.py
```

### Comparing `kdp-api-python-client-4.98.0/PKG-INFO` & `kdp-api-python-client-4.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdp-api-python-client
-Version: 4.98.0
+Version: 4.99.0
 Summary: Koverse Data Platform (KDP) API
 Home-page: UNKNOWN
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: UNKNOWN
 Keywords: OpenAPI,OpenAPI-Generator,Koverse Data Platform (KDP) API
 Platform: UNKNOWN
```

### Comparing `kdp-api-python-client-4.98.0/README.md` & `kdp-api-python-client-4.99.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # kdp-api-python-client
 The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 4.98.0
-- Package version: 4.98.0
+- API version: 4.99.0
+- Package version: 4.99.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >=3.6
 
 ## Installation & Usage
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/__init__.py` & `kdp-api-python-client-4.99.0/kdp_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # flake8: noqa
 
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "4.98.0"
+__version__ = "4.99.0"
 
 # import ApiClient
 from kdp_api.api_client import ApiClient
 
 # import Configuration
 from kdp_api.configuration import Configuration
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/abac_label_parsers_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/abac_label_parsers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/applications_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/applications_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/attribute_assignments_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/attribute_assignments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/attributes_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/attributes_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/audit_log_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/audit_log_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/audit_log_configs_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/audit_log_configs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/authentication_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/authentication_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/dataset_permissions_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/dataset_permissions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/dataset_syncs_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/dataset_syncs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/datasets_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/datasets_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/group_memberships_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/group_memberships_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/groups_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/groups_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/indexes_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/indexes_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/ingest_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/ingest_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/jobs_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/jobs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/query_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/query_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/read_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/read_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/segments_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/segments_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/serve_media_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/serve_media_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/source_types_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/source_types_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/storage_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/storage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/uploads_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/uploads_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/users_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/users_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/workspaces_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/workspaces_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api/write_api.py` & `kdp-api-python-client-4.99.0/kdp_api/api/write_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/api_client.py` & `kdp-api-python-client-4.99.0/kdp_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/4.98.0/python'
+        self.user_agent = 'OpenAPI-Generator/4.99.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/apis/__init__.py` & `kdp-api-python-client-4.99.0/kdp_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `kdp-api-python-client-4.98.0/kdp_api/configuration.py` & `kdp-api-python-client-4.99.0/kdp_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
@@ -384,16 +384,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 4.98.0\n"\
-               "SDK Package Version: 4.98.0".\
+               "Version of the API: 4.99.0\n"\
+               "SDK Package Version: 4.99.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/exceptions.py` & `kdp-api-python-client-4.99.0/kdp_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/abac_label_parser_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/abac_label_parser_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/abac_label_parsers.py` & `kdp-api-python-client-4.99.0/kdp_api/model/abac_label_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/abac_label_parsers_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/abac_label_parsers_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/access_control_label.py` & `kdp-api-python-client-4.99.0/kdp_api/model/access_control_label.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/api_error.py` & `kdp-api-python-client-4.99.0/kdp_api/model/api_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/application.py` & `kdp-api-python-client-4.99.0/kdp_api/model/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/application_create_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/application_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/application_create_request_required_dataset_access_inner.py` & `kdp-api-python-client-4.99.0/kdp_api/model/application_create_request_required_dataset_access_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/application_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/application_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/application_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/application_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/application_patch_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/application_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/application_required_dataset_access_inner.py` & `kdp-api-python-client-4.99.0/kdp_api/model/application_required_dataset_access_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/application_update_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/application_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/attribute.py` & `kdp-api-python-client-4.99.0/kdp_api/model/attribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/attribute_assignment.py` & `kdp-api-python-client-4.99.0/kdp_api/model/attribute_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/attribute_assignment_create_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/attribute_assignment_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/attribute_assignment_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/attribute_assignment_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/attribute_assignment_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/attribute_assignment_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/attribute_assignment_patch_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/attribute_assignment_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/attribute_assignment_update_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/attribute_assignment_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/attribute_create_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/attribute_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/attribute_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/attribute_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/attribute_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/attribute_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/attribute_patch_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/attribute_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/attribute_update_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/attribute_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/audit_log_configuration.py` & `kdp-api-python-client-4.99.0/kdp_api/model/audit_log_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/audit_log_configuration_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/audit_log_configuration_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/audit_log_configuration_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/audit_log_configuration_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/audit_log_event.py` & `kdp-api-python-client-4.99.0/kdp_api/model/audit_log_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/audit_log_event_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/audit_log_event_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/audit_log_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/audit_log_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/authentication.py` & `kdp-api-python-client-4.99.0/kdp_api/model/authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/authentication_details.py` & `kdp-api-python-client-4.99.0/kdp_api/model/authentication_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/authentication_details_authentication.py` & `kdp-api-python-client-4.99.0/kdp_api/model/authentication_details_authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/authentication_details_authentication_payload.py` & `kdp-api-python-client-4.99.0/kdp_api/model/authentication_details_authentication_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/authentication_details_user.py` & `kdp-api-python-client-4.99.0/kdp_api/model/authentication_details_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/authentication_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/authentication_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/authentication_sso.py` & `kdp-api-python-client-4.99.0/kdp_api/model/authentication_sso.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/batch_write_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/batch_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/connection_info.py` & `kdp-api-python-client-4.99.0/kdp_api/model/connection_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/custom_identity_provider.py` & `kdp-api-python-client-4.99.0/kdp_api/model/custom_identity_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/custom_identity_provider_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/custom_identity_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/data_source_params.py` & `kdp-api-python-client-4.99.0/kdp_api/model/data_source_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_create_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_current_user_permissions.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_current_user_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_patch_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_permission.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_permission_create_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_permission_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_permission_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_permission_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_permission_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_permission_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_permission_patch_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_permission_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_permission_update_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_permission_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_sync.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_sync_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_sync_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_sync_management_terminate_connection_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_sync_management_terminate_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_sync_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_sync_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_sync_patch_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_sync_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_sync_update_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_sync_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/dataset_update_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/dataset_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/delete_document_by_query_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/delete_document_by_query_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/delete_record_by_id_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/delete_record_by_id_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/delete_record_by_query_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/delete_record_by_query_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/error_code.py` & `kdp-api-python-client-4.99.0/kdp_api/model/error_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/get_serve_media200_response.py` & `kdp-api-python-client-4.99.0/kdp_api/model/get_serve_media200_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/group.py` & `kdp-api-python-client-4.99.0/kdp_api/model/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/group_create_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/group_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/group_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/group_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/group_membership.py` & `kdp-api-python-client-4.99.0/kdp_api/model/group_membership.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/group_membership_create_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/group_membership_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/group_membership_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/group_membership_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/group_membership_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/group_membership_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/group_membership_patch_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/group_membership_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/group_membership_update_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/group_membership_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/group_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/group_paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/group_patch_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/group_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/group_update_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/group_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/index.py` & `kdp-api-python-client-4.99.0/kdp_api/model/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/index_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/index_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/index_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/index_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/ingest_create_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/ingest_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/job.py` & `kdp-api-python-client-4.99.0/kdp_api/model/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/job_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/job_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/job_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/job_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/json_record.py` & `kdp-api-python-client-4.99.0/kdp_api/model/json_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/keycloak_provider_configuration.py` & `kdp-api-python-client-4.99.0/kdp_api/model/keycloak_provider_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/koverse_document_metadata.py` & `kdp-api-python-client-4.99.0/kdp_api/model/koverse_document_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/lucene_query_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/lucene_query_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/origin_dataset_sync_create_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/origin_dataset_sync_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/query.py` & `kdp-api-python-client-4.99.0/kdp_api/model/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/query_datasets_summary.py` & `kdp-api-python-client-4.99.0/kdp_api/model/query_datasets_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/query_datasets_summary_datasets_inner.py` & `kdp-api-python-client-4.99.0/kdp_api/model/query_datasets_summary_datasets_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/query_datasets_summary_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/query_datasets_summary_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/query_document_lucene_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/query_document_lucene_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/query_document_lucene_response.py` & `kdp-api-python-client-4.99.0/kdp_api/model/query_document_lucene_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/query_document_lucene_response_records_inner.py` & `kdp-api-python-client-4.99.0/kdp_api/model/query_document_lucene_response_records_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/read_range_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/read_range_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/record_batch.py` & `kdp-api-python-client-4.99.0/kdp_api/model/record_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/reindex_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/reindex_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/replica_dataset_sync_create_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/replica_dataset_sync_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/security_label_info_params.py` & `kdp-api-python-client-4.99.0/kdp_api/model/security_label_info_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/segment.py` & `kdp-api-python-client-4.99.0/kdp_api/model/segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/segment_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/segment_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/segment_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/segment_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/sequence_read_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/sequence_read_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/source_types.py` & `kdp-api-python-client-4.99.0/kdp_api/model/source_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/source_types_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/source_types_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/split_points.py` & `kdp-api-python-client-4.99.0/kdp_api/model/split_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/stripe_latest_charge.py` & `kdp-api-python-client-4.99.0/kdp_api/model/stripe_latest_charge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/stripe_latest_charge1.py` & `kdp-api-python-client-4.99.0/kdp_api/model/stripe_latest_charge1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/sync_kafka_consumer_group_id.py` & `kdp-api-python-client-4.99.0/kdp_api/model/sync_kafka_consumer_group_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/sync_setup_origin.py` & `kdp-api-python-client-4.99.0/kdp_api/model/sync_setup_origin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/sync_setup_replica.py` & `kdp-api-python-client-4.99.0/kdp_api/model/sync_setup_replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/terminate_connection_response.py` & `kdp-api-python-client-4.99.0/kdp_api/model/terminate_connection_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/transfer_resource_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/transfer_resource_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/transfer_resource_request_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/transfer_resource_request_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/upload_response.py` & `kdp-api-python-client-4.99.0/kdp_api/model/upload_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/user.py` & `kdp-api-python-client-4.99.0/kdp_api/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/user_create_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/user_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/user_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/user_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/user_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/user_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/user_patch_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/user_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/user_update_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/user_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/workspace.py` & `kdp-api-python-client-4.99.0/kdp_api/model/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/workspace_create_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/workspace_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/workspace_create_request_subscription.py` & `kdp-api-python-client-4.99.0/kdp_api/model/workspace_create_request_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/workspace_create_request_subscription_subscription_item_ids.py` & `kdp-api-python-client-4.99.0/kdp_api/model/workspace_create_request_subscription_subscription_item_ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/workspace_list.py` & `kdp-api-python-client-4.99.0/kdp_api/model/workspace_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/workspace_paginator.py` & `kdp-api-python-client-4.99.0/kdp_api/model/workspace_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/workspace_patch_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/workspace_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/workspace_subscription.py` & `kdp-api-python-client-4.99.0/kdp_api/model/workspace_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/workspace_subscription_subscription_item_ids.py` & `kdp-api-python-client-4.99.0/kdp_api/model/workspace_subscription_subscription_item_ids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/workspace_update_request.py` & `kdp-api-python-client-4.99.0/kdp_api/model/workspace_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model/write_batch_response.py` & `kdp-api-python-client-4.99.0/kdp_api/model/write_batch_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/model_utils.py` & `kdp-api-python-client-4.99.0/kdp_api/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api/models/__init__.py` & `kdp-api-python-client-4.99.0/kdp_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kdp-api-python-client-4.98.0/kdp_api/rest.py` & `kdp-api-python-client-4.99.0/kdp_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api_python_client.egg-info/PKG-INFO` & `kdp-api-python-client-4.99.0/kdp_api_python_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdp-api-python-client
-Version: 4.98.0
+Version: 4.99.0
 Summary: Koverse Data Platform (KDP) API
 Home-page: UNKNOWN
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: UNKNOWN
 Keywords: OpenAPI,OpenAPI-Generator,Koverse Data Platform (KDP) API
 Platform: UNKNOWN
```

### Comparing `kdp-api-python-client-4.98.0/kdp_api_python_client.egg-info/SOURCES.txt` & `kdp-api-python-client-4.99.0/kdp_api_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kdp-api-python-client-4.98.0/setup.py` & `kdp-api-python-client-4.99.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "kdp-api-python-client"
-VERSION = "4.98.0"
+VERSION = "4.99.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `kdp-api-python-client-4.98.0/test/test_abac_label_parser_paginator.py` & `kdp-api-python-client-4.99.0/test/test_abac_label_parser_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_abac_label_parsers.py` & `kdp-api-python-client-4.99.0/test/test_abac_label_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_abac_label_parsers_api.py` & `kdp-api-python-client-4.99.0/test/test_abac_label_parsers_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_abac_label_parsers_list.py` & `kdp-api-python-client-4.99.0/test/test_abac_label_parsers_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_access_control_label.py` & `kdp-api-python-client-4.99.0/test/test_access_control_label.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_api_error.py` & `kdp-api-python-client-4.99.0/test/test_error_code.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.api_error import ApiError
+from kdp_api.model.error_code import ErrorCode
 
 
-class TestApiError(unittest.TestCase):
-    """ApiError unit test stubs"""
+class TestErrorCode(unittest.TestCase):
+    """ErrorCode unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testApiError(self):
-        """Test ApiError"""
+    def testErrorCode(self):
+        """Test ErrorCode"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ApiError()  # noqa: E501
+        # model = ErrorCode()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_application.py` & `kdp-api-python-client-4.99.0/test/test_application.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_application_create_request.py` & `kdp-api-python-client-4.99.0/test/test_application_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_application_create_request_required_dataset_access_inner.py` & `kdp-api-python-client-4.99.0/test/test_application_create_request_required_dataset_access_inner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_application_list.py` & `kdp-api-python-client-4.99.0/test/test_application_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_application_paginator.py` & `kdp-api-python-client-4.99.0/test/test_application_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_application_patch_request.py` & `kdp-api-python-client-4.99.0/test/test_application_patch_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_application_required_dataset_access_inner.py` & `kdp-api-python-client-4.99.0/test/test_application_required_dataset_access_inner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_application_update_request.py` & `kdp-api-python-client-4.99.0/test/test_application_update_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_applications_api.py` & `kdp-api-python-client-4.99.0/test/test_applications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attribute.py` & `kdp-api-python-client-4.99.0/test/test_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.attribute import Attribute
+from kdp_api.model.group import Group
 
 
-class TestAttribute(unittest.TestCase):
-    """Attribute unit test stubs"""
+class TestGroup(unittest.TestCase):
+    """Group unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAttribute(self):
-        """Test Attribute"""
+    def testGroup(self):
+        """Test Group"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Attribute()  # noqa: E501
+        # model = Group()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attribute_assignment.py` & `kdp-api-python-client-4.99.0/test/test_attribute_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attribute_assignment_create_request.py` & `kdp-api-python-client-4.99.0/test/test_attribute_assignment_create_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attribute_assignment_list.py` & `kdp-api-python-client-4.99.0/test/test_attribute_assignment_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attribute_assignment_paginator.py` & `kdp-api-python-client-4.99.0/test/test_attribute_assignment_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attribute_assignment_patch_request.py` & `kdp-api-python-client-4.99.0/test/test_attribute_assignment_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attribute_assignment_update_request.py` & `kdp-api-python-client-4.99.0/test/test_attribute_assignment_update_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attribute_assignments_api.py` & `kdp-api-python-client-4.99.0/test/test_attribute_assignments_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attribute_create_request.py` & `kdp-api-python-client-4.99.0/test/test_attribute_create_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attribute_list.py` & `kdp-api-python-client-4.99.0/test/test_attribute_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attribute_paginator.py` & `kdp-api-python-client-4.99.0/test/test_attribute_paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attribute_patch_request.py` & `kdp-api-python-client-4.99.0/test/test_group_patch_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.attribute_patch_request import AttributePatchRequest
+from kdp_api.model.group_patch_request import GroupPatchRequest
 
 
-class TestAttributePatchRequest(unittest.TestCase):
-    """AttributePatchRequest unit test stubs"""
+class TestGroupPatchRequest(unittest.TestCase):
+    """GroupPatchRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAttributePatchRequest(self):
-        """Test AttributePatchRequest"""
+    def testGroupPatchRequest(self):
+        """Test GroupPatchRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = AttributePatchRequest()  # noqa: E501
+        # model = GroupPatchRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attribute_update_request.py` & `kdp-api-python-client-4.99.0/test/test_attribute_update_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_attributes_api.py` & `kdp-api-python-client-4.99.0/test/test_attributes_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_audit_log_api.py` & `kdp-api-python-client-4.99.0/test/test_audit_log_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_audit_log_configs_api.py` & `kdp-api-python-client-4.99.0/test/test_audit_log_configs_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_audit_log_configuration.py` & `kdp-api-python-client-4.99.0/test/test_audit_log_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_audit_log_configuration_list.py` & `kdp-api-python-client-4.99.0/test/test_audit_log_configuration_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_audit_log_configuration_paginator.py` & `kdp-api-python-client-4.99.0/test/test_audit_log_configuration_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_audit_log_event.py` & `kdp-api-python-client-4.99.0/test/test_audit_log_event_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
 from kdp_api.model.audit_log_event import AuditLogEvent
+globals()['AuditLogEvent'] = AuditLogEvent
+from kdp_api.model.audit_log_event_list import AuditLogEventList
 
 
-class TestAuditLogEvent(unittest.TestCase):
-    """AuditLogEvent unit test stubs"""
+class TestAuditLogEventList(unittest.TestCase):
+    """AuditLogEventList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAuditLogEvent(self):
-        """Test AuditLogEvent"""
+    def testAuditLogEventList(self):
+        """Test AuditLogEventList"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = AuditLogEvent()  # noqa: E501
+        # model = AuditLogEventList()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_audit_log_event_list.py` & `kdp-api-python-client-4.99.0/test/test_audit_log_event.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
 from kdp_api.model.audit_log_event import AuditLogEvent
-globals()['AuditLogEvent'] = AuditLogEvent
-from kdp_api.model.audit_log_event_list import AuditLogEventList
 
 
-class TestAuditLogEventList(unittest.TestCase):
-    """AuditLogEventList unit test stubs"""
+class TestAuditLogEvent(unittest.TestCase):
+    """AuditLogEvent unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAuditLogEventList(self):
-        """Test AuditLogEventList"""
+    def testAuditLogEvent(self):
+        """Test AuditLogEvent"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = AuditLogEventList()  # noqa: E501
+        # model = AuditLogEvent()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_audit_log_paginator.py` & `kdp-api-python-client-4.99.0/test/test_audit_log_paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_authentication.py` & `kdp-api-python-client-4.99.0/test/test_authentication.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_authentication_api.py` & `kdp-api-python-client-4.99.0/test/test_authentication_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_authentication_details.py` & `kdp-api-python-client-4.99.0/test/test_authentication_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_authentication_details_authentication.py` & `kdp-api-python-client-4.99.0/test/test_authentication_details_authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_authentication_details_authentication_payload.py` & `kdp-api-python-client-4.99.0/test/test_authentication_details_authentication_payload.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_authentication_details_user.py` & `kdp-api-python-client-4.99.0/test/test_authentication_details_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_authentication_list.py` & `kdp-api-python-client-4.99.0/test/test_authentication_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_authentication_sso.py` & `kdp-api-python-client-4.99.0/test/test_authentication_sso.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_batch_write_request.py` & `kdp-api-python-client-4.99.0/test/test_batch_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_connection_info.py` & `kdp-api-python-client-4.99.0/test/test_connection_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_custom_identity_provider.py` & `kdp-api-python-client-4.99.0/test/test_custom_identity_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_custom_identity_provider_list.py` & `kdp-api-python-client-4.99.0/test/test_custom_identity_provider_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_data_source_params.py` & `kdp-api-python-client-4.99.0/test/test_data_source_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset.py` & `kdp-api-python-client-4.99.0/test/test_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_create_request.py` & `kdp-api-python-client-4.99.0/test/test_dataset_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_current_user_permissions.py` & `kdp-api-python-client-4.99.0/test/test_dataset_current_user_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_list.py` & `kdp-api-python-client-4.99.0/test/test_dataset_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_paginator.py` & `kdp-api-python-client-4.99.0/test/test_dataset_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_patch_request.py` & `kdp-api-python-client-4.99.0/test/test_dataset_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_permission.py` & `kdp-api-python-client-4.99.0/test/test_dataset_permission.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_permission_create_request.py` & `kdp-api-python-client-4.99.0/test/test_dataset_permission_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_permission_list.py` & `kdp-api-python-client-4.99.0/test/test_dataset_permission_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_permission_paginator.py` & `kdp-api-python-client-4.99.0/test/test_dataset_permission_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_permission_patch_request.py` & `kdp-api-python-client-4.99.0/test/test_dataset_permission_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_permission_update_request.py` & `kdp-api-python-client-4.99.0/test/test_dataset_permission_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_permissions_api.py` & `kdp-api-python-client-4.99.0/test/test_dataset_permissions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_sync.py` & `kdp-api-python-client-4.99.0/test/test_dataset_sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_sync_list.py` & `kdp-api-python-client-4.99.0/test/test_dataset_sync_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_sync_management_terminate_connection_request.py` & `kdp-api-python-client-4.99.0/test/test_dataset_sync_management_terminate_connection_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_sync_paginator.py` & `kdp-api-python-client-4.99.0/test/test_dataset_sync_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_sync_patch_request.py` & `kdp-api-python-client-4.99.0/test/test_dataset_sync_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_sync_update_request.py` & `kdp-api-python-client-4.99.0/test/test_dataset_sync_update_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_syncs_api.py` & `kdp-api-python-client-4.99.0/test/test_dataset_syncs_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_dataset_update_request.py` & `kdp-api-python-client-4.99.0/test/test_dataset_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_datasets_api.py` & `kdp-api-python-client-4.99.0/test/test_datasets_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_delete_document_by_query_request.py` & `kdp-api-python-client-4.99.0/test/test_delete_document_by_query_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_delete_record_by_id_request.py` & `kdp-api-python-client-4.99.0/test/test_delete_record_by_id_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_delete_record_by_query_request.py` & `kdp-api-python-client-4.99.0/test/test_delete_record_by_query_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_error_code.py` & `kdp-api-python-client-4.99.0/test/test_group_create_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.error_code import ErrorCode
+from kdp_api.model.group_create_request import GroupCreateRequest
 
 
-class TestErrorCode(unittest.TestCase):
-    """ErrorCode unit test stubs"""
+class TestGroupCreateRequest(unittest.TestCase):
+    """GroupCreateRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testErrorCode(self):
-        """Test ErrorCode"""
+    def testGroupCreateRequest(self):
+        """Test GroupCreateRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ErrorCode()  # noqa: E501
+        # model = GroupCreateRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_get_serve_media200_response.py` & `kdp-api-python-client-4.99.0/test/test_get_serve_media200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_group.py` & `kdp-api-python-client-4.99.0/test/test_segment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.group import Group
+from kdp_api.model.segment import Segment
 
 
-class TestGroup(unittest.TestCase):
-    """Group unit test stubs"""
+class TestSegment(unittest.TestCase):
+    """Segment unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGroup(self):
-        """Test Group"""
+    def testSegment(self):
+        """Test Segment"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Group()  # noqa: E501
+        # model = Segment()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_group_create_request.py` & `kdp-api-python-client-4.99.0/test/test_group_update_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.group_create_request import GroupCreateRequest
+from kdp_api.model.group_update_request import GroupUpdateRequest
 
 
-class TestGroupCreateRequest(unittest.TestCase):
-    """GroupCreateRequest unit test stubs"""
+class TestGroupUpdateRequest(unittest.TestCase):
+    """GroupUpdateRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGroupCreateRequest(self):
-        """Test GroupCreateRequest"""
+    def testGroupUpdateRequest(self):
+        """Test GroupUpdateRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GroupCreateRequest()  # noqa: E501
+        # model = GroupUpdateRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_group_list.py` & `kdp-api-python-client-4.99.0/test/test_group_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_group_membership.py` & `kdp-api-python-client-4.99.0/test/test_group_membership.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_group_membership_create_request.py` & `kdp-api-python-client-4.99.0/test/test_group_membership_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_group_membership_list.py` & `kdp-api-python-client-4.99.0/test/test_group_membership_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_group_membership_paginator.py` & `kdp-api-python-client-4.99.0/test/test_group_membership_paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_group_membership_patch_request.py` & `kdp-api-python-client-4.99.0/test/test_group_membership_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_group_membership_update_request.py` & `kdp-api-python-client-4.99.0/test/test_group_membership_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_group_memberships_api.py` & `kdp-api-python-client-4.99.0/test/test_group_memberships_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_group_paginator.py` & `kdp-api-python-client-4.99.0/test/test_group_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_group_patch_request.py` & `kdp-api-python-client-4.99.0/test/test_user_patch_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.group_patch_request import GroupPatchRequest
+from kdp_api.model.stripe_latest_charge import StripeLatestCharge
+globals()['StripeLatestCharge'] = StripeLatestCharge
+from kdp_api.model.user_patch_request import UserPatchRequest
 
 
-class TestGroupPatchRequest(unittest.TestCase):
-    """GroupPatchRequest unit test stubs"""
+class TestUserPatchRequest(unittest.TestCase):
+    """UserPatchRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGroupPatchRequest(self):
-        """Test GroupPatchRequest"""
+    def testUserPatchRequest(self):
+        """Test UserPatchRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GroupPatchRequest()  # noqa: E501
+        # model = UserPatchRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_group_update_request.py` & `kdp-api-python-client-4.99.0/test/test_user_update_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.group_update_request import GroupUpdateRequest
+from kdp_api.model.user_update_request import UserUpdateRequest
 
 
-class TestGroupUpdateRequest(unittest.TestCase):
-    """GroupUpdateRequest unit test stubs"""
+class TestUserUpdateRequest(unittest.TestCase):
+    """UserUpdateRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGroupUpdateRequest(self):
-        """Test GroupUpdateRequest"""
+    def testUserUpdateRequest(self):
+        """Test UserUpdateRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GroupUpdateRequest()  # noqa: E501
+        # model = UserUpdateRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_groups_api.py` & `kdp-api-python-client-4.99.0/test/test_groups_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_index.py` & `kdp-api-python-client-4.99.0/test/test_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_index_list.py` & `kdp-api-python-client-4.99.0/test/test_index_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_index_paginator.py` & `kdp-api-python-client-4.99.0/test/test_index_paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_indexes_api.py` & `kdp-api-python-client-4.99.0/test/test_indexes_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_ingest_api.py` & `kdp-api-python-client-4.99.0/test/test_ingest_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_ingest_create_request.py` & `kdp-api-python-client-4.99.0/test/test_ingest_create_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_job.py` & `kdp-api-python-client-4.99.0/test/test_job.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_job_list.py` & `kdp-api-python-client-4.99.0/test/test_job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_job_paginator.py` & `kdp-api-python-client-4.99.0/test/test_job_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_jobs_api.py` & `kdp-api-python-client-4.99.0/test/test_jobs_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_json_record.py` & `kdp-api-python-client-4.99.0/test/test_json_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_keycloak_provider_configuration.py` & `kdp-api-python-client-4.99.0/test/test_keycloak_provider_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_koverse_document_metadata.py` & `kdp-api-python-client-4.99.0/test/test_koverse_document_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_lucene_query_request.py` & `kdp-api-python-client-4.99.0/test/test_lucene_query_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_origin_dataset_sync_create_request.py` & `kdp-api-python-client-4.99.0/test/test_origin_dataset_sync_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_query.py` & `kdp-api-python-client-4.99.0/test/test_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_query_api.py` & `kdp-api-python-client-4.99.0/test/test_query_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_query_datasets_summary.py` & `kdp-api-python-client-4.99.0/test/test_query_datasets_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_query_datasets_summary_datasets_inner.py` & `kdp-api-python-client-4.99.0/test/test_query_datasets_summary_datasets_inner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_query_datasets_summary_request.py` & `kdp-api-python-client-4.99.0/test/test_query_datasets_summary_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_query_document_lucene_request.py` & `kdp-api-python-client-4.99.0/test/test_query_document_lucene_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_query_document_lucene_response.py` & `kdp-api-python-client-4.99.0/test/test_query_document_lucene_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_query_document_lucene_response_records_inner.py` & `kdp-api-python-client-4.99.0/test/test_query_document_lucene_response_records_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_read_api.py` & `kdp-api-python-client-4.99.0/test/test_read_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_read_range_request.py` & `kdp-api-python-client-4.99.0/test/test_read_range_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_record_batch.py` & `kdp-api-python-client-4.99.0/test/test_record_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_reindex_request.py` & `kdp-api-python-client-4.99.0/test/test_reindex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_replica_dataset_sync_create_request.py` & `kdp-api-python-client-4.99.0/test/test_replica_dataset_sync_create_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_security_label_info_params.py` & `kdp-api-python-client-4.99.0/test/test_security_label_info_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_segment.py` & `kdp-api-python-client-4.99.0/test/test_segment_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
 from kdp_api.model.segment import Segment
+globals()['Segment'] = Segment
+from kdp_api.model.segment_list import SegmentList
 
 
-class TestSegment(unittest.TestCase):
-    """Segment unit test stubs"""
+class TestSegmentList(unittest.TestCase):
+    """SegmentList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSegment(self):
-        """Test Segment"""
+    def testSegmentList(self):
+        """Test SegmentList"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Segment()  # noqa: E501
+        # model = SegmentList()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_segment_list.py` & `kdp-api-python-client-4.99.0/test/test_segment_paginator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.segment import Segment
-globals()['Segment'] = Segment
 from kdp_api.model.segment_list import SegmentList
+globals()['SegmentList'] = SegmentList
+from kdp_api.model.segment_paginator import SegmentPaginator
 
 
-class TestSegmentList(unittest.TestCase):
-    """SegmentList unit test stubs"""
+class TestSegmentPaginator(unittest.TestCase):
+    """SegmentPaginator unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSegmentList(self):
-        """Test SegmentList"""
+    def testSegmentPaginator(self):
+        """Test SegmentPaginator"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SegmentList()  # noqa: E501
+        # model = SegmentPaginator()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_segment_paginator.py` & `kdp-api-python-client-4.99.0/test/test_user_paginator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.segment_list import SegmentList
-globals()['SegmentList'] = SegmentList
-from kdp_api.model.segment_paginator import SegmentPaginator
+from kdp_api.model.user_list import UserList
+globals()['UserList'] = UserList
+from kdp_api.model.user_paginator import UserPaginator
 
 
-class TestSegmentPaginator(unittest.TestCase):
-    """SegmentPaginator unit test stubs"""
+class TestUserPaginator(unittest.TestCase):
+    """UserPaginator unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSegmentPaginator(self):
-        """Test SegmentPaginator"""
+    def testUserPaginator(self):
+        """Test UserPaginator"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SegmentPaginator()  # noqa: E501
+        # model = UserPaginator()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_segments_api.py` & `kdp-api-python-client-4.99.0/test/test_segments_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_sequence_read_request.py` & `kdp-api-python-client-4.99.0/test/test_sequence_read_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_serve_media_api.py` & `kdp-api-python-client-4.99.0/test/test_serve_media_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_source_types.py` & `kdp-api-python-client-4.99.0/test/test_source_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_source_types_api.py` & `kdp-api-python-client-4.99.0/test/test_source_types_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_source_types_list.py` & `kdp-api-python-client-4.99.0/test/test_source_types_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_split_points.py` & `kdp-api-python-client-4.99.0/test/test_split_points.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_storage_api.py` & `kdp-api-python-client-4.99.0/test/test_storage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_stripe_latest_charge.py` & `kdp-api-python-client-4.99.0/test/test_stripe_latest_charge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_stripe_latest_charge1.py` & `kdp-api-python-client-4.99.0/test/test_stripe_latest_charge1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_sync_kafka_consumer_group_id.py` & `kdp-api-python-client-4.99.0/test/test_sync_kafka_consumer_group_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_sync_setup_origin.py` & `kdp-api-python-client-4.99.0/test/test_sync_setup_origin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_sync_setup_replica.py` & `kdp-api-python-client-4.99.0/test/test_sync_setup_replica.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_terminate_connection_response.py` & `kdp-api-python-client-4.99.0/test/test_terminate_connection_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_transfer_resource_request.py` & `kdp-api-python-client-4.99.0/test/test_transfer_resource_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_transfer_resource_request_list.py` & `kdp-api-python-client-4.99.0/test/test_transfer_resource_request_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_upload_response.py` & `kdp-api-python-client-4.99.0/test/test_upload_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_uploads_api.py` & `kdp-api-python-client-4.99.0/test/test_uploads_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_user.py` & `kdp-api-python-client-4.99.0/test/test_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_user_create_request.py` & `kdp-api-python-client-4.99.0/test/test_user_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_user_list.py` & `kdp-api-python-client-4.99.0/test/test_user_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_user_paginator.py` & `kdp-api-python-client-4.99.0/test/test_workspace_paginator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.user_list import UserList
-globals()['UserList'] = UserList
-from kdp_api.model.user_paginator import UserPaginator
+from kdp_api.model.workspace_list import WorkspaceList
+globals()['WorkspaceList'] = WorkspaceList
+from kdp_api.model.workspace_paginator import WorkspacePaginator
 
 
-class TestUserPaginator(unittest.TestCase):
-    """UserPaginator unit test stubs"""
+class TestWorkspacePaginator(unittest.TestCase):
+    """WorkspacePaginator unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserPaginator(self):
-        """Test UserPaginator"""
+    def testWorkspacePaginator(self):
+        """Test WorkspacePaginator"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UserPaginator()  # noqa: E501
+        # model = WorkspacePaginator()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_user_patch_request.py` & `kdp-api-python-client-4.99.0/test/test_attribute_patch_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.stripe_latest_charge import StripeLatestCharge
-globals()['StripeLatestCharge'] = StripeLatestCharge
-from kdp_api.model.user_patch_request import UserPatchRequest
+from kdp_api.model.attribute_patch_request import AttributePatchRequest
 
 
-class TestUserPatchRequest(unittest.TestCase):
-    """UserPatchRequest unit test stubs"""
+class TestAttributePatchRequest(unittest.TestCase):
+    """AttributePatchRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserPatchRequest(self):
-        """Test UserPatchRequest"""
+    def testAttributePatchRequest(self):
+        """Test AttributePatchRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UserPatchRequest()  # noqa: E501
+        # model = AttributePatchRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_user_update_request.py` & `kdp-api-python-client-4.99.0/test/test_attribute.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.user_update_request import UserUpdateRequest
+from kdp_api.model.attribute import Attribute
 
 
-class TestUserUpdateRequest(unittest.TestCase):
-    """UserUpdateRequest unit test stubs"""
+class TestAttribute(unittest.TestCase):
+    """Attribute unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserUpdateRequest(self):
-        """Test UserUpdateRequest"""
+    def testAttribute(self):
+        """Test Attribute"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UserUpdateRequest()  # noqa: E501
+        # model = Attribute()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_users_api.py` & `kdp-api-python-client-4.99.0/test/test_users_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_workspace.py` & `kdp-api-python-client-4.99.0/test/test_workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_workspace_create_request.py` & `kdp-api-python-client-4.99.0/test/test_workspace_update_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
 from kdp_api.model.workspace_create_request_subscription import WorkspaceCreateRequestSubscription
 globals()['WorkspaceCreateRequestSubscription'] = WorkspaceCreateRequestSubscription
-from kdp_api.model.workspace_create_request import WorkspaceCreateRequest
+from kdp_api.model.workspace_update_request import WorkspaceUpdateRequest
 
 
-class TestWorkspaceCreateRequest(unittest.TestCase):
-    """WorkspaceCreateRequest unit test stubs"""
+class TestWorkspaceUpdateRequest(unittest.TestCase):
+    """WorkspaceUpdateRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWorkspaceCreateRequest(self):
-        """Test WorkspaceCreateRequest"""
+    def testWorkspaceUpdateRequest(self):
+        """Test WorkspaceUpdateRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WorkspaceCreateRequest()  # noqa: E501
+        # model = WorkspaceUpdateRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_workspace_create_request_subscription.py` & `kdp-api-python-client-4.99.0/test/test_workspace_create_request_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_workspace_create_request_subscription_subscription_item_ids.py` & `kdp-api-python-client-4.99.0/test/test_workspace_create_request_subscription_subscription_item_ids.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_workspace_list.py` & `kdp-api-python-client-4.99.0/test/test_workspace_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_workspace_paginator.py` & `kdp-api-python-client-4.99.0/test/test_workspace_create_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.workspace_list import WorkspaceList
-globals()['WorkspaceList'] = WorkspaceList
-from kdp_api.model.workspace_paginator import WorkspacePaginator
+from kdp_api.model.workspace_create_request_subscription import WorkspaceCreateRequestSubscription
+globals()['WorkspaceCreateRequestSubscription'] = WorkspaceCreateRequestSubscription
+from kdp_api.model.workspace_create_request import WorkspaceCreateRequest
 
 
-class TestWorkspacePaginator(unittest.TestCase):
-    """WorkspacePaginator unit test stubs"""
+class TestWorkspaceCreateRequest(unittest.TestCase):
+    """WorkspaceCreateRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWorkspacePaginator(self):
-        """Test WorkspacePaginator"""
+    def testWorkspaceCreateRequest(self):
+        """Test WorkspaceCreateRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WorkspacePaginator()  # noqa: E501
+        # model = WorkspaceCreateRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_workspace_patch_request.py` & `kdp-api-python-client-4.99.0/test/test_workspace_patch_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_workspace_subscription.py` & `kdp-api-python-client-4.99.0/test/test_workspace_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_workspace_subscription_subscription_item_ids.py` & `kdp-api-python-client-4.99.0/test/test_workspace_subscription_subscription_item_ids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.98.0/test/test_workspace_update_request.py` & `kdp-api-python-client-4.99.0/test/test_workspaces_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,63 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
-import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.workspace_create_request_subscription import WorkspaceCreateRequestSubscription
-globals()['WorkspaceCreateRequestSubscription'] = WorkspaceCreateRequestSubscription
-from kdp_api.model.workspace_update_request import WorkspaceUpdateRequest
+from kdp_api.api.workspaces_api import WorkspacesApi  # noqa: E501
 
 
-class TestWorkspaceUpdateRequest(unittest.TestCase):
-    """WorkspaceUpdateRequest unit test stubs"""
+class TestWorkspacesApi(unittest.TestCase):
+    """WorkspacesApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = WorkspacesApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testWorkspaceUpdateRequest(self):
-        """Test WorkspaceUpdateRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = WorkspaceUpdateRequest()  # noqa: E501
+    def test_get_workspaces(self):
+        """Test case for get_workspaces
+
+        Retrieves a list of workspaces  # noqa: E501
+        """
+        pass
+
+    def test_get_workspaces_id(self):
+        """Test case for get_workspaces_id
+
+        Retrieves Workspace with given ID  # noqa: E501
+        """
+        pass
+
+    def test_patch_workspaces_id(self):
+        """Test case for patch_workspaces_id
+
+        Updates provided fields of Workspace with the ID given  # noqa: E501
+        """
+        pass
+
+    def test_post_workspaces(self):
+        """Test case for post_workspaces
+
+        Creates a new Workspace  # noqa: E501
+        """
+        pass
+
+    def test_put_workspaces_id(self):
+        """Test case for put_workspaces_id
+
+        Updates Workspace with the ID given  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.98.0/test/test_write_api.py` & `kdp-api-python-client-4.99.0/test/test_write_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.98.0/test/test_write_batch_response.py` & `kdp-api-python-client-4.99.0/test/test_write_batch_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces. Please note that the Python client library follows Python's naming convention of snake casing for fields, even though they may appear in camel case in the API specification. <p><b>By default this api documentation targets the koverse production server at 'api.app.koverse.com' You can provide the hostname of your koverse instance to this documentation page via the 'host' query param.</p> <p><b>For example providing host - https://documentation.koverse.com/api?host=api.myHost.com, will update requests to target the provided host.</b></p> <p><b>Authentication request example with provided host - https://api.myHost.com/authentication</b></p>  # noqa: E501
 
-    The version of the OpenAPI document: 4.98.0
+    The version of the OpenAPI document: 4.99.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

