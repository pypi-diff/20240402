# Comparing `tmp/cvat_sdk-2.9.1.tar.gz` & `tmp/cvat_sdk-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat_sdk-2.9.1.tar", last modified: Mon Nov 27 13:51:22 2023, max compression
+gzip compressed data, was "cvat_sdk-2.9.2.tar", last modified: Mon Dec 11 18:26:32 2023, max compression
```

## Comparing `cvat_sdk-2.9.1.tar` & `cvat_sdk-2.9.2.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.359563 cvat_sdk-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-11-27 13:51:00.000000 cvat_sdk-2.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-11-27 13:51:22.359563 cvat_sdk-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-11-27 13:51:00.000000 cvat_sdk-2.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.319563 cvat_sdk-2.9.1/cvat_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.319563 cvat_sdk-2.9.1/cvat_sdk/api_client/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.323562 cvat_sdk-2.9.1/cvat_sdk/api_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/analytics_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21701 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/assets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    45482 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    55496 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/cloudstorages_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31685 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/comments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15033 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22686 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/guides_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41926 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/invitations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32175 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/issues_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    92415 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27037 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/labels_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    39147 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/lambda_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25294 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30153 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/organizations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    75400 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53937 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/quality_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/schema_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21452 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/server_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   132260 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30498 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    65705 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api/webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    45634 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.323562 cvat_sdk-2.9.1/cvat_sdk/api_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19679 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.351563 cvat_sdk-2.9.1/cvat_sdk/api_client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13042 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/about.py
--rw-r--r--   0 runner    (1001) docker     (127)    12451 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/accept_invitation_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    14014 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/accept_invitation_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14402 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/analytics_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    12965 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/analytics_report_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13058 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/analytics_report_target_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    15100 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_conflict.py
--rw-r--r--   0 runner    (1001) docker     (127)    15328 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_conflict_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12460 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_file_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14276 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_guide_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_guide_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13969 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    14124 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_id_shape_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13018 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_id_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    15640 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotations_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    13893 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/asset_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    14175 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    13942 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/attribute_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/attribute_val.py
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/attribute_val_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14272 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/backup_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/basic_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13574 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/basic_user_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13955 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/binary_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13023 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/chunk_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    12999 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/client_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/client_events_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13139 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/cloud_storage_content.py
--rw-r--r--   0 runner    (1001) docker     (127)    17475 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/cloud_storage_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    15488 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/cloud_storage_read_owner.py
--rw-r--r--   0 runner    (1001) docker     (127)    18328 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/cloud_storage_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14309 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/comment_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    12658 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/comment_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12743 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/comments_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    14282 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/credentials_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12508 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)    16405 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/data_meta_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    35562 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/data_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12406 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/dataset_file_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13648 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/dataset_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    12999 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/dataset_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    14276 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/dataset_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12966 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/default_view_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    18298 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    18849 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/event_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12988 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    18731 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/events_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    13186 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/file_info_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    13644 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/frame_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/frame_selection_method_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    15275 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/function_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    13576 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/function_call_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    17332 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/function_call_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12978 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/granularity_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/input_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    14396 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/invitation_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/invitation_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16025 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/issue_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    14034 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/issue_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/issues_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    16288 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_annotations_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    23241 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_read_assignee.py
--rw-r--r--   0 runner    (1001) docker     (127)    13213 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)    13203 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    13016 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    17144 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13540 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/jobs_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    17310 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/label.py
--rw-r--r--   0 runner    (1001) docker     (127)    13888 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/label_mapping_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14504 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14752 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_data_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14732 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    14901 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_image_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18094 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    18334 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_shape_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15751 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_track.py
--rw-r--r--   0 runner    (1001) docker     (127)    16062 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_track_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/labels_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12981 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/location_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/login_serializer_ex_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15044 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/membership_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    17616 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/meta_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    15176 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14138 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/metric_granularity.py
--rw-r--r--   0 runner    (1001) docker     (127)    12611 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/null_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12583 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/online_function_call_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13335 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/operation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    13063 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/operator_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    15460 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/organization_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    13788 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/organization_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13703 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_annotation_conflict_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13674 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13598 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_comment_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13643 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_invitation_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_issue_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13538 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_job_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13507 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_label_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13643 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_membership_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13553 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_meta_user_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13673 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_organization_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13598 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_project_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13628 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_quality_report_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13658 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_quality_settings_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13553 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_task_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13719 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13598 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_webhook_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13433 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/password_change_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13634 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/password_reset_confirm_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13147 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_annotation_guide_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18255 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_comment_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12418 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_data_meta_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_invitation_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13069 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_issue_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_job_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16560 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_label_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_labeled_data_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12514 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_membership_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13823 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_organization_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16059 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_project_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14845 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    21880 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_quality_settings_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16209 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_task_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    16216 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_user_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14962 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_webhook_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13269 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    12406 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/project_file_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    19350 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/project_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    14944 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/project_read_target_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    16024 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/project_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13747 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/provider_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12976 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/quality_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    15893 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/quality_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/quality_report_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15291 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/quality_report_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12851 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/quality_report_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    22444 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/quality_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13363 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/register_serializer_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)    14361 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/register_serializer_ex_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/rest_auth_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    13300 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12264 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/rq_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    13564 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/rq_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    13285 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/rq_status_state_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/severity_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/shape_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    12299 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/signing_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13430 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/sorting_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    13336 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12956 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/storage_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    13074 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/storage_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13123 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/storage_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    17568 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/sub_labeled_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    17737 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/sub_labeled_shape_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15225 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/sub_labeled_track.py
--rw-r--r--   0 runner    (1001) docker     (127)    15465 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/sub_labeled_track_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15279 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/sublabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12794 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/sublabel_mapping_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15414 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/sublabel_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16291 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/task_annotations_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14338 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/task_annotations_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12352 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/task_file_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    24015 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/task_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    14932 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/task_read_target_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    17123 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/task_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12728 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/tasks_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12255 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    16249 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/tracked_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    16355 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/tracked_shape_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12844 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/transformation_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)    17571 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    12666 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/webhook_content_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    16284 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/webhook_delivery_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    18526 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/webhook_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    12991 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/webhook_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    15742 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model/webhook_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    84700 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.351563 cvat_sdk-2.9.1/cvat_sdk/api_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)    17891 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14475 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/api_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.355563 cvat_sdk-2.9.1/cvat_sdk/auto_annotation/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/auto_annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11169 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/auto_annotation/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.355563 cvat_sdk-2.9.1/cvat_sdk/auto_annotation/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/auto_annotation/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/auto_annotation/functions/torchvision_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/auto_annotation/functions/torchvision_keypoint_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/auto_annotation/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.355563 cvat_sdk-2.9.1/cvat_sdk/core/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11877 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/downloading.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.355563 cvat_sdk-2.9.1/cvat_sdk/core/proxies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/proxies/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/proxies/issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/proxies/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/proxies/model_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/proxies/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/proxies/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    13881 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/proxies/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/proxies/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    14966 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/uploading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.355563 cvat_sdk-2.9.1/cvat_sdk/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11415 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/datasets/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/datasets/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/datasets/task_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.359563 cvat_sdk-2.9.1/cvat_sdk/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/pytorch/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/pytorch/project_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/pytorch/task_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/pytorch/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/cvat_sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.359563 cvat_sdk-2.9.1/cvat_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-11-27 13:51:22.000000 cvat_sdk-2.9.1/cvat_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12030 2023-11-27 13:51:22.000000 cvat_sdk-2.9.1/cvat_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 13:51:22.000000 cvat_sdk-2.9.1/cvat_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-11-27 13:51:22.000000 cvat_sdk-2.9.1/cvat_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-27 13:51:22.000000 cvat_sdk-2.9.1/cvat_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-11-27 13:51:00.000000 cvat_sdk-2.9.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:22.359563 cvat_sdk-2.9.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/requirements/api_client.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-11-27 13:51:00.000000 cvat_sdk-2.9.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 13:51:22.359563 cvat_sdk-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2023-11-27 13:51:13.000000 cvat_sdk-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.159770 cvat_sdk-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-11 18:26:10.000000 cvat_sdk-2.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-12-11 18:26:32.159770 cvat_sdk-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-12-11 18:26:10.000000 cvat_sdk-2.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.115770 cvat_sdk-2.9.2/cvat_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.119770 cvat_sdk-2.9.2/cvat_sdk/api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.123771 cvat_sdk-2.9.2/cvat_sdk/api_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/analytics_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21701 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/assets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45482 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55496 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/cloudstorages_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31685 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/comments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15033 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22686 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/guides_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41926 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/invitations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32175 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/issues_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92415 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27037 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/labels_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39147 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/lambda_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25294 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30153 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/organizations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75400 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53937 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/quality_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21452 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   132260 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30498 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65705 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45634 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.123771 cvat_sdk-2.9.2/cvat_sdk/api_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19679 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.151770 cvat_sdk-2.9.2/cvat_sdk/api_client/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13042 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12451 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/accept_invitation_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14014 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/accept_invitation_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/analytics_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12965 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/analytics_report_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13058 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/analytics_report_target_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15100 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_conflict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15328 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_conflict_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12460 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_file_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14276 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_guide_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_guide_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13969 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14124 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_id_shape_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13018 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_id_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15640 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotations_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13893 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/asset_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13942 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/attribute_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/attribute_val.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/attribute_val_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14272 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/backup_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/basic_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/basic_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13955 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/binary_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13023 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/chunk_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12999 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/client_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/client_events_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13139 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/cloud_storage_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17475 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/cloud_storage_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15488 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/cloud_storage_read_owner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18328 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/cloud_storage_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14309 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/comment_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12658 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/comment_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12743 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/comments_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14282 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/credentials_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12508 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16405 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/data_meta_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35562 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/data_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12406 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/dataset_file_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13648 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/dataset_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12999 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/dataset_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14276 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/dataset_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12966 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/default_view_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18298 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18849 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/event_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12988 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18731 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/events_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13186 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/file_info_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13644 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/frame_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/frame_selection_method_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15275 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/function_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13576 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/function_call_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17332 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/function_call_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12978 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/granularity_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/input_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14396 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/invitation_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/invitation_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16025 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/issue_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14034 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/issue_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/issues_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16288 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_annotations_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24265 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_read_assignee.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_read_target_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13213 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13203 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17144 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13540 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/jobs_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17310 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13888 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/label_mapping_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14504 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14752 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_data_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14732 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14901 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_image_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18094 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18334 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_shape_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15751 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_track.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16062 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_track_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/labels_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/location_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/login_serializer_ex_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15044 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/membership_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17616 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/meta_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15176 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14138 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/metric_granularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12611 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/null_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12583 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/online_function_call_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13335 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/operation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13063 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/operator_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15460 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/organization_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13788 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/organization_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13703 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_annotation_conflict_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13674 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13598 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_comment_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13643 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_invitation_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_issue_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13538 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_job_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13507 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_label_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13643 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_membership_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_meta_user_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13673 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_organization_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13598 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_project_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13628 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_quality_report_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_quality_settings_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_task_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13719 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13598 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_webhook_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13433 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/password_change_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13634 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/password_reset_confirm_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13147 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_annotation_guide_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18255 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_comment_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12418 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_data_meta_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_invitation_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13069 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_issue_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_job_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16560 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_label_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14787 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_labeled_data_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12514 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_membership_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13823 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_organization_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16059 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_project_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14710 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21880 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_quality_settings_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16209 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_task_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14697 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16216 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14962 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_webhook_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13269 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12406 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/project_file_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19350 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/project_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14809 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/project_read_target_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16024 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/project_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13747 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/provider_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12976 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/quality_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15893 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/quality_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/quality_report_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15291 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/quality_report_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12851 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/quality_report_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22444 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/quality_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13363 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/register_serializer_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/register_serializer_ex_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12298 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/rest_auth_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13300 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12264 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/rq_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13564 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/rq_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13285 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/rq_status_state_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/severity_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/shape_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12299 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/signing_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13430 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/sorting_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12956 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/storage_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12939 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/storage_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13123 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/storage_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17568 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/sub_labeled_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17737 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/sub_labeled_shape_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15225 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/sub_labeled_track.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15465 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/sub_labeled_track_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15279 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/sublabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12794 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/sublabel_mapping_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15414 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/sublabel_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16291 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/task_annotations_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14338 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/task_annotations_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12352 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/task_file_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24001 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/task_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17123 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/task_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12728 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/tasks_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12255 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16249 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/tracked_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16355 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/tracked_shape_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12844 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/transformation_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17571 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12666 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/webhook_content_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/webhook_delivery_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18526 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/webhook_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12991 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/webhook_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15742 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model/webhook_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84700 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.151770 cvat_sdk-2.9.2/cvat_sdk/api_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    17889 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14475 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/api_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.155770 cvat_sdk-2.9.2/cvat_sdk/auto_annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/auto_annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11169 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/auto_annotation/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.155770 cvat_sdk-2.9.2/cvat_sdk/auto_annotation/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/auto_annotation/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/auto_annotation/functions/torchvision_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/auto_annotation/functions/torchvision_keypoint_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/auto_annotation/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.155770 cvat_sdk-2.9.2/cvat_sdk/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/downloading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.155770 cvat_sdk-2.9.2/cvat_sdk/core/proxies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/proxies/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/proxies/issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/proxies/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/proxies/model_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/proxies/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/proxies/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13881 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/proxies/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/proxies/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14966 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/uploading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.155770 cvat_sdk-2.9.2/cvat_sdk/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11415 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/datasets/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/datasets/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/datasets/task_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.159770 cvat_sdk-2.9.2/cvat_sdk/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/pytorch/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/pytorch/project_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/pytorch/task_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2023-12-11 18:26:26.000000 cvat_sdk-2.9.2/cvat_sdk/pytorch/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/cvat_sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.159770 cvat_sdk-2.9.2/cvat_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-12-11 18:26:32.000000 cvat_sdk-2.9.2/cvat_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2023-12-11 18:26:32.000000 cvat_sdk-2.9.2/cvat_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 18:26:32.000000 cvat_sdk-2.9.2/cvat_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-11 18:26:32.000000 cvat_sdk-2.9.2/cvat_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-11 18:26:32.000000 cvat_sdk-2.9.2/cvat_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-11 18:26:10.000000 cvat_sdk-2.9.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:32.159770 cvat_sdk-2.9.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/requirements/api_client.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-11 18:26:10.000000 cvat_sdk-2.9.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 18:26:32.159770 cvat_sdk-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2023-12-11 18:26:25.000000 cvat_sdk-2.9.2/setup.py
```

### Comparing `cvat_sdk-2.9.1/PKG-INFO` & `cvat_sdk-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat_sdk
-Version: 2.9.1
+Version: 2.9.2
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.9.1/README.md` & `cvat_sdk-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/__init__.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
-__version__ = "2.9.1"
+__version__ = "2.9.2"
 
 from cvat_sdk.api_client.api_client import ApiClient
 
 from cvat_sdk.api_client.configuration import Configuration
 
 from cvat_sdk.api_client.exceptions import OpenApiException
 from cvat_sdk.api_client.exceptions import ApiAttributeError
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/analytics_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/analytics_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/assets_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/assets_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/auth_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/auth_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/cloudstorages_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/cloudstorages_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/comments_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/comments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/events_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/events_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/guides_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/guides_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/invitations_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/invitations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/issues_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/issues_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/jobs_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/jobs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/labels_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/labels_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/lambda_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/lambda_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/memberships_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/memberships_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/organizations_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/organizations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/projects_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/projects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/quality_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/quality_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/schema_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/schema_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/server_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/server_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/tasks_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/tasks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/users_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api/webhooks_api.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api/webhooks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/api_client.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import json
@@ -114,15 +114,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers: typing.Dict[str, str] = headers or {}
         self.cookies = SimpleCookie()
         if cookies:
             self.cookies.update(cookies)
         # Set default User-Agent.
-        self.user_agent = 'cvat_sdk/2.9.1'
+        self.user_agent = 'cvat_sdk/2.9.2'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/apis/__init__.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/apis/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/configuration.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import copy
 import logging
 import multiprocessing
@@ -484,16 +484,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.9.1\n"\
-               "SDK Package Version: 2.9.1".\
+               "Version of the API: 2.9.2\n"\
+               "SDK Package Version: 2.9.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/exceptions.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/about.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/about.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/accept_invitation_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/accept_invitation_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/accept_invitation_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/accept_invitation_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/analytics_report.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/analytics_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/analytics_report_create_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/analytics_report_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/analytics_report_target_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/analytics_report_target_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_conflict.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_conflict.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_conflict_type_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_conflict_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_file_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_guide_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_guide_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_guide_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_guide_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_id.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_id_shape_type.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_id_shape_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotation_id_type_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotation_id_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/annotations_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/annotations_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/asset_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/asset_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/attribute.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/attribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/attribute_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/attribute_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/attribute_val.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/attribute_val.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/attribute_val_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/attribute_val_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/backup_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/backup_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/basic_user.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/basic_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/basic_user_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/basic_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/binary_operation.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/binary_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/chunk_type.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/chunk_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/client_events.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/client_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/client_events_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/client_events_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/cloud_storage_content.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/cloud_storage_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/cloud_storage_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/cloud_storage_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/cloud_storage_read_owner.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/cloud_storage_read_owner.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/cloud_storage_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/cloud_storage_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/comment_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/comment_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/comment_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/comment_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/comments_summary.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/comments_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/credentials_type_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/credentials_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/data_frame.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/data_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/data_meta_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/data_meta_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/data_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/dataset_file_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/dataset_file_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/dataset_format.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/dataset_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/dataset_formats.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/dataset_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/dataset_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/dataset_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/default_view_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/default_view_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/event.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/event_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/events.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/events_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/events_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/file_info.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/file_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/file_info_type_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/file_info_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/frame_meta.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/frame_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/frame_selection_method_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/frame_selection_method_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/function_call.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/function_call.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/function_call_params.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/function_call_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/function_call_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/function_call_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/granularity_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/granularity_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/input_type_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/input_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/invitation_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/invitation_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/invitation_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/invitation_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/issue_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/issue_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/issue_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/issue_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/issues_summary.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/issues_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_annotations_update_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_annotations_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_read.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -43,22 +43,24 @@
     from cvat_sdk.api_client.models import *
 
 
 def lazy_import():
     from cvat_sdk.api_client.model.chunk_type import ChunkType
     from cvat_sdk.api_client.model.issues_summary import IssuesSummary
     from cvat_sdk.api_client.model.job_read_assignee import JobReadAssignee
+    from cvat_sdk.api_client.model.job_read_target_storage import JobReadTargetStorage
     from cvat_sdk.api_client.model.job_stage import JobStage
     from cvat_sdk.api_client.model.job_status import JobStatus
     from cvat_sdk.api_client.model.job_type import JobType
     from cvat_sdk.api_client.model.labels_summary import LabelsSummary
     from cvat_sdk.api_client.model.operation_status import OperationStatus
     globals()['ChunkType'] = ChunkType
     globals()['IssuesSummary'] = IssuesSummary
     globals()['JobReadAssignee'] = JobReadAssignee
+    globals()['JobReadTargetStorage'] = JobReadTargetStorage
     globals()['JobStage'] = JobStage
     globals()['JobStatus'] = JobStatus
     globals()['JobType'] = JobType
     globals()['LabelsSummary'] = LabelsSummary
     globals()['OperationStatus'] = OperationStatus
 
 
@@ -181,14 +183,24 @@
     """
 
     organization: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
     """
 
+    target_storage: JobReadTargetStorage # noqa: E501
+    """
+    [optional]
+    """
+
+    source_storage: JobReadTargetStorage # noqa: E501
+    """
+    [optional]
+    """
+
 
 class JobRead(ModelNormal, IJobRead):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -236,14 +248,18 @@
 
       updated_date (datetime): [optional]  # noqa: E501
 
       type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
       organization (int, none_type): [optional]  # noqa: E501
 
+      target_storage (JobReadTargetStorage): [optional]  # noqa: E501
+
+      source_storage (JobReadTargetStorage): [optional]  # noqa: E501
+
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
           and the value is json key in definition.
@@ -325,14 +341,16 @@
             'stop_frame': (int,),  # noqa: E501
             'data_chunk_size': (int, none_type,),  # noqa: E501
             'data_compressed_chunk_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'updated_date': (datetime,),  # noqa: E501
             'type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'organization': (int, none_type,),  # noqa: E501
+            'target_storage': (JobReadTargetStorage,),  # noqa: E501
+            'source_storage': (JobReadTargetStorage,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -357,14 +375,16 @@
         'stop_frame': 'stop_frame',  # noqa: E501
         'data_chunk_size': 'data_chunk_size',  # noqa: E501
         'data_compressed_chunk_type': 'data_compressed_chunk_type',  # noqa: E501
         'created_date': 'created_date',  # noqa: E501
         'updated_date': 'updated_date',  # noqa: E501
         'type': 'type',  # noqa: E501
         'organization': 'organization',  # noqa: E501
+        'target_storage': 'target_storage',  # noqa: E501
+        'source_storage': 'source_storage',  # noqa: E501
     }
 
     read_only_vars = {
         'url',  # noqa: E501
         'id',  # noqa: E501
         'task_id',  # noqa: E501
         'project_id',  # noqa: E501
@@ -436,14 +456,18 @@
 
             updated_date (datetime): [optional]  # noqa: E501
 
             type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             organization (int, none_type): [optional]  # noqa: E501
 
+            target_storage (JobReadTargetStorage): [optional]  # noqa: E501
+
+            source_storage (JobReadTargetStorage): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -570,14 +594,18 @@
 
             updated_date (datetime): [optional]  # noqa: E501
 
             type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             organization (int, none_type): [optional]  # noqa: E501
 
+            target_storage (JobReadTargetStorage): [optional]  # noqa: E501
+
+            source_storage (JobReadTargetStorage): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_read_assignee.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_read_assignee.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_stage.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_status.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_type.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/job_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/jobs_summary.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/jobs_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/label.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/label.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/label_mapping_entry_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/label_mapping_entry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_data.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_data_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_image.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_image_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_image_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_shape.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_shape_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_track.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/labeled_track_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/labeled_track_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/labels_summary.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/labels_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/location_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/location_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/login_serializer_ex_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/login_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/membership_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/membership_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/meta_user.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/meta_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/metric.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/metric_granularity.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/metric_granularity.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/null_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/null_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/online_function_call_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/online_function_call_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/operation_status.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/operation_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/operator_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/operator_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/organization_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/organization_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/organization_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/organization_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_annotation_conflict_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_annotation_conflict_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_comment_read_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_comment_read_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_invitation_read_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_invitation_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_issue_read_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_issue_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_job_read_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_job_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_label_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_label_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_membership_read_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_membership_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_meta_user_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_meta_user_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_organization_read_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_organization_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_project_read_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_project_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_quality_report_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_quality_report_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_quality_settings_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_quality_settings_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_task_read_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_task_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/paginated_webhook_read_list.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/paginated_webhook_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/password_change_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/password_change_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/password_reset_confirm_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/password_reset_confirm_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_annotation_guide_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_annotation_guide_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_comment_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_comment_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_data_meta_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_data_meta_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_invitation_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_invitation_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_issue_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_issue_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_job_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_job_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_label_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_label_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_labeled_data_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_labeled_data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_membership_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_membership_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_organization_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_organization_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_project_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_project_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -74,18 +74,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('cloud_storage_id',): {
-            'inclusive_maximum': 2147483647,
-            'inclusive_minimum': -2147483648,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_quality_settings_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_quality_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_task_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_task_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -74,18 +74,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('cloud_storage_id',): {
-            'inclusive_maximum': 2147483647,
-            'inclusive_minimum': -2147483648,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_user_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/patched_webhook_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/patched_webhook_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/plugins.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/project_file_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/project_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/project_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/project_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/project_read_target_storage.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/job_read_target_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -46,15 +46,15 @@
 def lazy_import():
     from cvat_sdk.api_client.model.location_enum import LocationEnum
     from cvat_sdk.api_client.model.storage import Storage
     globals()['LocationEnum'] = LocationEnum
     globals()['Storage'] = Storage
 
 
-class ProjectReadTargetStorage(ModelComposed):
+class JobReadTargetStorage(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -74,18 +74,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('cloud_storage_id',): {
-            'inclusive_maximum': 2147483647,
-            'inclusive_minimum': -2147483648,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -126,16 +122,16 @@
 
     read_only_vars = {
         'id',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs) -> ProjectReadTargetStorage:  # noqa: E501
-        """ProjectReadTargetStorage - a model defined in OpenAPI
+    def _from_openapi_data(cls, *args, **kwargs) -> JobReadTargetStorage:  # noqa: E501
+        """JobReadTargetStorage - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -237,15 +233,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ProjectReadTargetStorage - a model defined in OpenAPI
+        """JobReadTargetStorage - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/project_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/project_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/provider_type_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/provider_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/quality_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/quality_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/quality_report.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/quality_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/quality_report_create_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/quality_report_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/quality_report_summary.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/quality_report_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/quality_report_target.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/quality_report_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/quality_settings.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/quality_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/register_serializer_ex.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/register_serializer_ex.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/register_serializer_ex_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/register_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/rest_auth_detail.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/rest_auth_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/role_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/role_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/rq_id.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/rq_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/rq_status.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/rq_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/rq_status_state_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/rq_status_state_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/severity_enum.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/severity_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/shape_type.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/shape_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/signing_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/signing_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/sorting_method.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/sorting_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/storage.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -107,18 +107,14 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('cloud_storage_id',): {
-            'inclusive_maximum': 2147483647,
-            'inclusive_minimum': -2147483648,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/storage_method.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/storage_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/storage_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/storage_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -100,18 +100,14 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('cloud_storage_id',): {
-            'inclusive_maximum': 2147483647,
-            'inclusive_minimum': -2147483648,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/storage_type.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/storage_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/sub_labeled_shape.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/sub_labeled_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/sub_labeled_shape_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/sub_labeled_shape_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/sub_labeled_track.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/sub_labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/sub_labeled_track_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/sub_labeled_track_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/sublabel.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/sublabel.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/sublabel_mapping_entry_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/sublabel_mapping_entry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/sublabel_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/sublabel_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/task_annotations_update_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/task_annotations_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/task_annotations_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/task_annotations_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/task_file_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/task_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/task_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/task_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -42,24 +42,24 @@
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 def lazy_import():
     from cvat_sdk.api_client.model.chunk_type import ChunkType
     from cvat_sdk.api_client.model.cloud_storage_read_owner import CloudStorageReadOwner
+    from cvat_sdk.api_client.model.job_read_target_storage import JobReadTargetStorage
     from cvat_sdk.api_client.model.job_status import JobStatus
     from cvat_sdk.api_client.model.jobs_summary import JobsSummary
     from cvat_sdk.api_client.model.labels_summary import LabelsSummary
-    from cvat_sdk.api_client.model.task_read_target_storage import TaskReadTargetStorage
     globals()['ChunkType'] = ChunkType
     globals()['CloudStorageReadOwner'] = CloudStorageReadOwner
+    globals()['JobReadTargetStorage'] = JobReadTargetStorage
     globals()['JobStatus'] = JobStatus
     globals()['JobsSummary'] = JobsSummary
     globals()['LabelsSummary'] = LabelsSummary
-    globals()['TaskReadTargetStorage'] = TaskReadTargetStorage
 
 
 
 class ITaskRead(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -179,20 +179,20 @@
     """
 
     organization: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
     """
 
-    target_storage: TaskReadTargetStorage # noqa: E501
+    target_storage: JobReadTargetStorage # noqa: E501
     """
     [optional]
     """
 
-    source_storage: TaskReadTargetStorage # noqa: E501
+    source_storage: JobReadTargetStorage # noqa: E501
     """
     [optional]
     """
 
     jobs: JobsSummary # noqa: E501
     """
     """
@@ -256,17 +256,17 @@
 
       dimension (str): [optional]  # noqa: E501
 
       subset (str): [optional]  # noqa: E501
 
       organization (int, none_type): [optional]  # noqa: E501
 
-      target_storage (TaskReadTargetStorage): [optional]  # noqa: E501
+      target_storage (JobReadTargetStorage): [optional]  # noqa: E501
 
-      source_storage (TaskReadTargetStorage): [optional]  # noqa: E501
+      source_storage (JobReadTargetStorage): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -345,16 +345,16 @@
             'data_original_chunk_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'size': (int,),  # noqa: E501
             'image_quality': (int,),  # noqa: E501
             'data': (int,),  # noqa: E501
             'dimension': (str,),  # noqa: E501
             'subset': (str,),  # noqa: E501
             'organization': (int, none_type,),  # noqa: E501
-            'target_storage': (TaskReadTargetStorage,),  # noqa: E501
-            'source_storage': (TaskReadTargetStorage,),  # noqa: E501
+            'target_storage': (JobReadTargetStorage,),  # noqa: E501
+            'source_storage': (JobReadTargetStorage,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -464,17 +464,17 @@
 
             dimension (str): [optional]  # noqa: E501
 
             subset (str): [optional]  # noqa: E501
 
             organization (int, none_type): [optional]  # noqa: E501
 
-            target_storage (TaskReadTargetStorage): [optional]  # noqa: E501
+            target_storage (JobReadTargetStorage): [optional]  # noqa: E501
 
-            source_storage (TaskReadTargetStorage): [optional]  # noqa: E501
+            source_storage (JobReadTargetStorage): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -606,17 +606,17 @@
 
             dimension (str): [optional]  # noqa: E501
 
             subset (str): [optional]  # noqa: E501
 
             organization (int, none_type): [optional]  # noqa: E501
 
-            target_storage (TaskReadTargetStorage): [optional]  # noqa: E501
+            target_storage (JobReadTargetStorage): [optional]  # noqa: E501
 
-            source_storage (TaskReadTargetStorage): [optional]  # noqa: E501
+            source_storage (JobReadTargetStorage): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/task_read_target_storage.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/project_read_target_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -46,15 +46,15 @@
 def lazy_import():
     from cvat_sdk.api_client.model.location_enum import LocationEnum
     from cvat_sdk.api_client.model.storage import Storage
     globals()['LocationEnum'] = LocationEnum
     globals()['Storage'] = Storage
 
 
-class TaskReadTargetStorage(ModelComposed):
+class ProjectReadTargetStorage(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -74,18 +74,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('cloud_storage_id',): {
-            'inclusive_maximum': 2147483647,
-            'inclusive_minimum': -2147483648,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -126,16 +122,16 @@
 
     read_only_vars = {
         'id',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs) -> TaskReadTargetStorage:  # noqa: E501
-        """TaskReadTargetStorage - a model defined in OpenAPI
+    def _from_openapi_data(cls, *args, **kwargs) -> ProjectReadTargetStorage:  # noqa: E501
+        """ProjectReadTargetStorage - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -237,15 +233,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TaskReadTargetStorage - a model defined in OpenAPI
+        """ProjectReadTargetStorage - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/task_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/task_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/tasks_summary.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/tasks_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/token.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/tracked_shape.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/tracked_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/tracked_shape_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/tracked_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/transformation.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/transformation_binary.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/transformation_binary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/user.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/webhook_content_type.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/webhook_content_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/webhook_delivery_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/webhook_delivery_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/webhook_read.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/webhook_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/webhook_type.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/webhook_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model/webhook_write_request.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model/webhook_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/model_utils.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import copy, deepcopy
 import inspect
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/models/__init__.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
@@ -80,14 +80,15 @@
 from cvat_sdk.api_client.model.invitation_write_request import InvitationWriteRequest, IInvitationWriteRequest
 from cvat_sdk.api_client.model.issue_read import IssueRead, IIssueRead
 from cvat_sdk.api_client.model.issue_write_request import IssueWriteRequest, IIssueWriteRequest
 from cvat_sdk.api_client.model.issues_summary import IssuesSummary, IIssuesSummary
 from cvat_sdk.api_client.model.job_annotations_update_request import JobAnnotationsUpdateRequest
 from cvat_sdk.api_client.model.job_read import JobRead, IJobRead
 from cvat_sdk.api_client.model.job_read_assignee import JobReadAssignee
+from cvat_sdk.api_client.model.job_read_target_storage import JobReadTargetStorage
 from cvat_sdk.api_client.model.job_stage import JobStage, IJobStage
 from cvat_sdk.api_client.model.job_status import JobStatus, IJobStatus
 from cvat_sdk.api_client.model.job_type import JobType, IJobType
 from cvat_sdk.api_client.model.job_write_request import JobWriteRequest, IJobWriteRequest
 from cvat_sdk.api_client.model.jobs_summary import JobsSummary, IJobsSummary
 from cvat_sdk.api_client.model.label import Label, ILabel
 from cvat_sdk.api_client.model.label_mapping_entry_request import LabelMappingEntryRequest, ILabelMappingEntryRequest
@@ -183,15 +184,14 @@
 from cvat_sdk.api_client.model.sublabel import Sublabel, ISublabel
 from cvat_sdk.api_client.model.sublabel_mapping_entry_request import SublabelMappingEntryRequest, ISublabelMappingEntryRequest
 from cvat_sdk.api_client.model.sublabel_request import SublabelRequest, ISublabelRequest
 from cvat_sdk.api_client.model.task_annotations_update_request import TaskAnnotationsUpdateRequest
 from cvat_sdk.api_client.model.task_annotations_write_request import TaskAnnotationsWriteRequest
 from cvat_sdk.api_client.model.task_file_request import TaskFileRequest, ITaskFileRequest
 from cvat_sdk.api_client.model.task_read import TaskRead, ITaskRead
-from cvat_sdk.api_client.model.task_read_target_storage import TaskReadTargetStorage
 from cvat_sdk.api_client.model.task_write_request import TaskWriteRequest, ITaskWriteRequest
 from cvat_sdk.api_client.model.tasks_summary import TasksSummary, ITasksSummary
 from cvat_sdk.api_client.model.token import Token, IToken
 from cvat_sdk.api_client.model.tracked_shape import TrackedShape, ITrackedShape
 from cvat_sdk.api_client.model.tracked_shape_request import TrackedShapeRequest, ITrackedShapeRequest
 from cvat_sdk.api_client.model.transformation import Transformation, ITransformation
 from cvat_sdk.api_client.model.transformation_binary import TransformationBinary
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/api_client/rest.py` & `cvat_sdk-2.9.2/cvat_sdk/api_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import io
 import json
 import logging
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk/auto_annotation/driver.py` & `cvat_sdk-2.9.2/cvat_sdk/auto_annotation/driver.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/auto_annotation/functions/torchvision_detection.py` & `cvat_sdk-2.9.2/cvat_sdk/auto_annotation/functions/torchvision_detection.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/auto_annotation/functions/torchvision_keypoint_detection.py` & `cvat_sdk-2.9.2/cvat_sdk/auto_annotation/functions/torchvision_keypoint_detection.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/auto_annotation/interface.py` & `cvat_sdk-2.9.2/cvat_sdk/auto_annotation/interface.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/client.py` & `cvat_sdk-2.9.2/cvat_sdk/core/client.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/downloading.py` & `cvat_sdk-2.9.2/cvat_sdk/core/downloading.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/helpers.py` & `cvat_sdk-2.9.2/cvat_sdk/core/helpers.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/progress.py` & `cvat_sdk-2.9.2/cvat_sdk/core/progress.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/proxies/annotations.py` & `cvat_sdk-2.9.2/cvat_sdk/core/proxies/annotations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/proxies/issues.py` & `cvat_sdk-2.9.2/cvat_sdk/core/proxies/issues.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/proxies/jobs.py` & `cvat_sdk-2.9.2/cvat_sdk/core/proxies/jobs.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/proxies/model_proxy.py` & `cvat_sdk-2.9.2/cvat_sdk/core/proxies/model_proxy.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/proxies/organizations.py` & `cvat_sdk-2.9.2/cvat_sdk/core/proxies/organizations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/proxies/projects.py` & `cvat_sdk-2.9.2/cvat_sdk/core/proxies/projects.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/proxies/tasks.py` & `cvat_sdk-2.9.2/cvat_sdk/core/proxies/tasks.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/proxies/users.py` & `cvat_sdk-2.9.2/cvat_sdk/core/proxies/users.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/uploading.py` & `cvat_sdk-2.9.2/cvat_sdk/core/uploading.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/core/utils.py` & `cvat_sdk-2.9.2/cvat_sdk/core/utils.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/datasets/caching.py` & `cvat_sdk-2.9.2/cvat_sdk/datasets/caching.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/datasets/common.py` & `cvat_sdk-2.9.2/cvat_sdk/datasets/common.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/datasets/task_dataset.py` & `cvat_sdk-2.9.2/cvat_sdk/datasets/task_dataset.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/pytorch/common.py` & `cvat_sdk-2.9.2/cvat_sdk/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/pytorch/project_dataset.py` & `cvat_sdk-2.9.2/cvat_sdk/pytorch/project_dataset.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/pytorch/task_dataset.py` & `cvat_sdk-2.9.2/cvat_sdk/pytorch/task_dataset.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk/pytorch/transforms.py` & `cvat_sdk-2.9.2/cvat_sdk/pytorch/transforms.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.9.1/cvat_sdk.egg-info/PKG-INFO` & `cvat_sdk-2.9.2/cvat_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-sdk
-Version: 2.9.1
+Version: 2.9.2
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.9.1/cvat_sdk.egg-info/SOURCES.txt` & `cvat_sdk-2.9.2/cvat_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 ./cvat_sdk/api_client/model/invitation_write_request.py
 ./cvat_sdk/api_client/model/issue_read.py
 ./cvat_sdk/api_client/model/issue_write_request.py
 ./cvat_sdk/api_client/model/issues_summary.py
 ./cvat_sdk/api_client/model/job_annotations_update_request.py
 ./cvat_sdk/api_client/model/job_read.py
 ./cvat_sdk/api_client/model/job_read_assignee.py
+./cvat_sdk/api_client/model/job_read_target_storage.py
 ./cvat_sdk/api_client/model/job_stage.py
 ./cvat_sdk/api_client/model/job_status.py
 ./cvat_sdk/api_client/model/job_type.py
 ./cvat_sdk/api_client/model/job_write_request.py
 ./cvat_sdk/api_client/model/jobs_summary.py
 ./cvat_sdk/api_client/model/label.py
 ./cvat_sdk/api_client/model/label_mapping_entry_request.py
@@ -199,15 +200,14 @@
 ./cvat_sdk/api_client/model/sublabel.py
 ./cvat_sdk/api_client/model/sublabel_mapping_entry_request.py
 ./cvat_sdk/api_client/model/sublabel_request.py
 ./cvat_sdk/api_client/model/task_annotations_update_request.py
 ./cvat_sdk/api_client/model/task_annotations_write_request.py
 ./cvat_sdk/api_client/model/task_file_request.py
 ./cvat_sdk/api_client/model/task_read.py
-./cvat_sdk/api_client/model/task_read_target_storage.py
 ./cvat_sdk/api_client/model/task_write_request.py
 ./cvat_sdk/api_client/model/tasks_summary.py
 ./cvat_sdk/api_client/model/token.py
 ./cvat_sdk/api_client/model/tracked_shape.py
 ./cvat_sdk/api_client/model/tracked_shape_request.py
 ./cvat_sdk/api_client/model/transformation.py
 ./cvat_sdk/api_client/model/transformation_binary.py
```

### Comparing `cvat_sdk-2.9.1/setup.py` & `cvat_sdk-2.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.9.1
+# The version of the OpenAPI document: 2.9.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import os.path as osp
 import re
 from setuptools import find_packages, setup
```

