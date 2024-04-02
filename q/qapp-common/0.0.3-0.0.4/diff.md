# Comparing `tmp/qapp-common-0.0.3.tar.gz` & `tmp/qapp-common-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qapp-common-0.0.3.tar", last modified: Tue Apr  2 07:24:37 2024, max compression
+gzip compressed data, was "qapp-common-0.0.4.tar", last modified: Tue Apr  2 08:22:42 2024, max compression
```

## Comparing `qapp-common-0.0.3.tar` & `qapp-common-0.0.4.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:37.015350 qapp-common-0.0.3/
--rw-rw-rw-   0        0        0     1111 2024-03-27 03:03:06.000000 qapp-common-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1988 2024-04-02 07:24:37.012350 qapp-common-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-04-01 07:05:10.000000 qapp-common-0.0.3/README.md
--rw-rw-rw-   0        0        0      805 2024-04-02 07:24:25.000000 qapp-common-0.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.828353 qapp-common-0.0.3/qapp_common/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.847353 qapp-common-0.0.3/qapp_common/async_tasks/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/async_tasks/__init__.py
--rw-rw-rw-   0        0        0      212 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/async_tasks/async_task.py
--rw-rw-rw-   0        0        0     3916 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/async_tasks/export_circuit_task.py
--rw-rw-rw-   0        0        0     2298 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/async_tasks/post_processing_task.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.849350 qapp-common-0.0.3/qapp_common/component/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.856351 qapp-common-0.0.3/qapp_common/component/backend/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/component/backend/__init__.py
--rw-rw-rw-   0        0        0     8374 2024-04-02 04:55:37.000000 qapp-common-0.0.3/qapp_common/component/backend/invocation.py
--rw-rw-rw-   0        0        0     9503 2024-04-02 07:18:05.000000 qapp-common-0.0.3/qapp_common/component/backend/job_fetching.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.859349 qapp-common-0.0.3/qapp_common/component/callback/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/component/callback/__init__.py
--rw-rw-rw-   0        0        0     1241 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/component/callback/update_job_metadata.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.874352 qapp-common-0.0.3/qapp_common/component/device/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/component/device/__init__.py
--rw-rw-rw-   0        0        0     2228 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/component/device/device_selection.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.881354 qapp-common-0.0.3/qapp_common/config/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/config/__init__.py
--rw-rw-rw-   0        0        0      243 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/config/logging_config.py
--rw-rw-rw-   0        0        0      458 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/config/thread_config.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.884350 qapp-common-0.0.3/qapp_common/data/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.886383 qapp-common-0.0.3/qapp_common/data/async_task/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/async_task/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.893352 qapp-common-0.0.3/qapp_common/data/async_task/circuit_export/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/async_task/circuit_export/__init__.py
--rw-rw-rw-   0        0        0      412 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/async_task/circuit_export/backend_holder.py
--rw-rw-rw-   0        0        0      293 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/async_task/circuit_export/circuit_holder.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.898352 qapp-common-0.0.3/qapp_common/data/backend/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/backend/__init__.py
--rw-rw-rw-   0        0        0      462 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/backend/backend_information.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.901350 qapp-common-0.0.3/qapp_common/data/callback/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/callback/__init__.py
--rw-rw-rw-   0        0        0      363 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/callback/callback_url.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.907350 qapp-common-0.0.3/qapp_common/data/device/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/device/__init__.py
--rw-rw-rw-   0        0        0      555 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/device/circuit_running_option.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.917352 qapp-common-0.0.3/qapp_common/data/promise/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/promise/__init__.py
--rw-rw-rw-   0        0        0      698 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/promise/post_processing_promise.py
--rw-rw-rw-   0        0        0      413 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/promise/promise.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.927352 qapp-common-0.0.3/qapp_common/data/request/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/request/__init__.py
--rw-rw-rw-   0        0        0     1024 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/request/invocation_request.py
--rw-rw-rw-   0        0        0      346 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/request/job_fetching_request.py
--rw-rw-rw-   0        0        0     1187 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/request/request.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.937349 qapp-common-0.0.3/qapp_common/data/response/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/response/__init__.py
--rw-rw-rw-   0        0        0      277 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/response/authentication.py
--rw-rw-rw-   0        0        0     1221 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/response/job_response.py
--rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/response/project_header.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.960351 qapp-common-0.0.3/qapp_common/enum/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/base_enum.py
--rw-rw-rw-   0        0        0      270 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/http_header.py
--rw-rw-rw-   0        0        0      357 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/invocation_step.py
--rw-rw-rw-   0        0        0      359 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/media_type.py
--rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/processing_unit.py
--rw-rw-rw-   0        0        0      587 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/provider_tag.py
--rw-rw-rw-   0        0        0      509 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.967348 qapp-common-0.0.3/qapp_common/enum/status/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/status/__init__.py
--rw-rw-rw-   0        0        0      222 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/status/job_status.py
--rw-rw-rw-   0        0        0      201 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/status/status_code.py
--rw-rw-rw-   0        0        0      196 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/token_type.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.975350 qapp-common-0.0.3/qapp_common/factory/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/factory/__init__.py
--rw-rw-rw-   0        0        0      576 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/factory/device_factory.py
--rw-rw-rw-   0        0        0      513 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/factory/handler_factory.py
--rw-rw-rw-   0        0        0      533 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.979350 qapp-common-0.0.3/qapp_common/handler/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/handler/__init__.py
--rw-rw-rw-   0        0        0      501 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/handler/handler.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.982350 qapp-common-0.0.3/qapp_common/model/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.986350 qapp-common-0.0.3/qapp_common/model/device/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/model/device/__init__.py
--rw-rw-rw-   0        0        0     9546 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/model/device/device.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.992351 qapp-common-0.0.3/qapp_common/model/provider/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/model/provider/__init__.py
--rw-rw-rw-   0        0        0      882 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/model/provider/provider.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:37.006348 qapp-common-0.0.3/qapp_common/util/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/util/__init__.py
--rw-rw-rw-   0        0        0      562 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/util/circuit_utils.py
--rw-rw-rw-   0        0        0      553 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/util/file_utils.py
--rw-rw-rw-   0        0        0     1071 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/util/http_utils.py
--rw-rw-rw-   0        0        0     2504 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/util/json_parser_utils.py
--rw-rw-rw-   0        0        0     1167 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:24:37.009350 qapp-common-0.0.3/qapp_common.egg-info/
--rw-rw-rw-   0        0        0     1988 2024-04-02 07:24:36.000000 qapp-common-0.0.3/qapp_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2800 2024-04-02 07:24:36.000000 qapp-common-0.0.3/qapp_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 07:24:36.000000 qapp-common-0.0.3/qapp_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-04-02 07:24:36.000000 qapp-common-0.0.3/qapp_common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-02 07:24:36.000000 qapp-common-0.0.3/qapp_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 07:24:37.015350 qapp-common-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.906803 qapp-common-0.0.4/
+-rw-rw-rw-   0        0        0     1111 2024-03-27 03:03:06.000000 qapp-common-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1988 2024-04-02 08:22:42.903806 qapp-common-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-04-01 07:05:10.000000 qapp-common-0.0.4/README.md
+-rw-rw-rw-   0        0        0      805 2024-04-02 08:22:32.000000 qapp-common-0.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.770783 qapp-common-0.0.4/qapp_common/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.785782 qapp-common-0.0.4/qapp_common/async_tasks/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/async_tasks/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/async_tasks/async_task.py
+-rw-rw-rw-   0        0        0     3916 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/async_tasks/export_circuit_task.py
+-rw-rw-rw-   0        0        0     2298 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/async_tasks/post_processing_task.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.787783 qapp-common-0.0.4/qapp_common/component/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.791780 qapp-common-0.0.4/qapp_common/component/backend/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/component/backend/__init__.py
+-rw-rw-rw-   0        0        0     8374 2024-04-02 04:55:37.000000 qapp-common-0.0.4/qapp_common/component/backend/invocation.py
+-rw-rw-rw-   0        0        0     9371 2024-04-02 07:36:54.000000 qapp-common-0.0.4/qapp_common/component/backend/job_fetching.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.794784 qapp-common-0.0.4/qapp_common/component/callback/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/component/callback/__init__.py
+-rw-rw-rw-   0        0        0     1241 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/component/callback/update_job_metadata.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.798780 qapp-common-0.0.4/qapp_common/component/device/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/component/device/__init__.py
+-rw-rw-rw-   0        0        0     2228 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/component/device/device_selection.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.803782 qapp-common-0.0.4/qapp_common/config/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/config/__init__.py
+-rw-rw-rw-   0        0        0      243 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/config/logging_config.py
+-rw-rw-rw-   0        0        0      458 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/config/thread_config.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.805780 qapp-common-0.0.4/qapp_common/data/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.806786 qapp-common-0.0.4/qapp_common/data/async_task/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/async_task/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.811781 qapp-common-0.0.4/qapp_common/data/async_task/circuit_export/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/async_task/circuit_export/__init__.py
+-rw-rw-rw-   0        0        0      412 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/async_task/circuit_export/backend_holder.py
+-rw-rw-rw-   0        0        0      293 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/async_task/circuit_export/circuit_holder.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.814815 qapp-common-0.0.4/qapp_common/data/backend/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/backend/__init__.py
+-rw-rw-rw-   0        0        0      462 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/backend/backend_information.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.818781 qapp-common-0.0.4/qapp_common/data/callback/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/callback/__init__.py
+-rw-rw-rw-   0        0        0      363 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/callback/callback_url.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.822780 qapp-common-0.0.4/qapp_common/data/device/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/device/__init__.py
+-rw-rw-rw-   0        0        0      555 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/device/circuit_running_option.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.828801 qapp-common-0.0.4/qapp_common/data/promise/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/promise/__init__.py
+-rw-rw-rw-   0        0        0      698 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/promise/post_processing_promise.py
+-rw-rw-rw-   0        0        0      413 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/promise/promise.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.834802 qapp-common-0.0.4/qapp_common/data/request/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/request/__init__.py
+-rw-rw-rw-   0        0        0     1024 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/request/invocation_request.py
+-rw-rw-rw-   0        0        0      346 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/request/job_fetching_request.py
+-rw-rw-rw-   0        0        0     1187 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/request/request.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.842835 qapp-common-0.0.4/qapp_common/data/response/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/response/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/response/authentication.py
+-rw-rw-rw-   0        0        0     1221 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/response/job_response.py
+-rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/data/response/project_header.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.860851 qapp-common-0.0.4/qapp_common/enum/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/enum/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/enum/base_enum.py
+-rw-rw-rw-   0        0        0      270 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/enum/http_header.py
+-rw-rw-rw-   0        0        0      357 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/enum/invocation_step.py
+-rw-rw-rw-   0        0        0      359 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/enum/media_type.py
+-rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      587 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/enum/provider_tag.py
+-rw-rw-rw-   0        0        0      509 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/enum/sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.866803 qapp-common-0.0.4/qapp_common/enum/status/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/enum/status/__init__.py
+-rw-rw-rw-   0        0        0      222 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/enum/status/job_status.py
+-rw-rw-rw-   0        0        0      201 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/enum/status/status_code.py
+-rw-rw-rw-   0        0        0      196 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/enum/token_type.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.873801 qapp-common-0.0.4/qapp_common/factory/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/factory/__init__.py
+-rw-rw-rw-   0        0        0      639 2024-04-02 07:55:44.000000 qapp-common-0.0.4/qapp_common/factory/device_factory.py
+-rw-rw-rw-   0        0        0      541 2024-04-02 08:08:09.000000 qapp-common-0.0.4/qapp_common/factory/handler_factory.py
+-rw-rw-rw-   0        0        0      596 2024-04-02 07:55:44.000000 qapp-common-0.0.4/qapp_common/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.876836 qapp-common-0.0.4/qapp_common/handler/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/handler/__init__.py
+-rw-rw-rw-   0        0        0      513 2024-04-02 08:21:18.000000 qapp-common-0.0.4/qapp_common/handler/handler.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.878801 qapp-common-0.0.4/qapp_common/model/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.881800 qapp-common-0.0.4/qapp_common/model/device/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/model/device/__init__.py
+-rw-rw-rw-   0        0        0     9546 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/model/device/device.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.885802 qapp-common-0.0.4/qapp_common/model/provider/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/model/provider/__init__.py
+-rw-rw-rw-   0        0        0      882 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/model/provider/provider.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.898806 qapp-common-0.0.4/qapp_common/util/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/util/__init__.py
+-rw-rw-rw-   0        0        0      564 2024-04-02 08:10:23.000000 qapp-common-0.0.4/qapp_common/util/circuit_utils.py
+-rw-rw-rw-   0        0        0      553 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/util/file_utils.py
+-rw-rw-rw-   0        0        0     1071 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/util/http_utils.py
+-rw-rw-rw-   0        0        0     2504 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/util/json_parser_utils.py
+-rw-rw-rw-   0        0        0     1167 2024-04-01 07:10:10.000000 qapp-common-0.0.4/qapp_common/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:22:42.900801 qapp-common-0.0.4/qapp_common.egg-info/
+-rw-rw-rw-   0        0        0     1988 2024-04-02 08:22:42.000000 qapp-common-0.0.4/qapp_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2800 2024-04-02 08:22:42.000000 qapp-common-0.0.4/qapp_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 08:22:42.000000 qapp-common-0.0.4/qapp_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-02 08:22:42.000000 qapp-common-0.0.4/qapp_common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-02 08:22:42.000000 qapp-common-0.0.4/qapp_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 08:22:42.906803 qapp-common-0.0.4/setup.cfg
```

### Comparing `qapp-common-0.0.3/LICENSE` & `qapp-common-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/PKG-INFO` & `qapp-common-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qapp-common
-Version: 0.0.3
+Version: 0.0.4
 Summary: QApp common library supporting QApp Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `qapp-common-0.0.3/pyproject.toml` & `qapp-common-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qapp-common"
-version = "0.0.3"
+version = "0.0.4"
 description = "QApp common library supporting QApp Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `qapp-common-0.0.3/qapp_common/async_tasks/export_circuit_task.py` & `qapp-common-0.0.4/qapp_common/async_tasks/export_circuit_task.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/async_tasks/post_processing_task.py` & `qapp-common-0.0.4/qapp_common/async_tasks/post_processing_task.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/component/backend/invocation.py` & `qapp-common-0.0.4/qapp_common/component/backend/invocation.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/component/backend/job_fetching.py` & `qapp-common-0.0.4/qapp_common/component/backend/job_fetching.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,16 @@
 from ...data.request.job_fetching_request import JobFetchingRequest
 from ...data.response.authentication import Authentication
 from ...data.response.job_response import JobResponse
 from ...data.response.project_header import ProjectHeader
 from ...enum.invocation_step import InvocationStep
 from ...config.logging_config import logger
 from ...enum.media_type import MediaType
-from ...enum.provider_tag import ProviderTag
-from ...enum.sdk import Sdk
 from ...enum.status.job_status import JobStatus
 from ...enum.status.status_code import StatusCode
-from ...factory.provider_factory import ProviderFactory
 from ...util.json_parser_utils import JsonParserUtils
 from ...util.response_utils import ResponseUtils
 
 
 class JobFetching(ABC):
     def __init__(self, request_data: JobFetchingRequest):
         self.provider_authentication: dict = request_data.provider_authentication
```

### Comparing `qapp-common-0.0.3/qapp_common/component/callback/update_job_metadata.py` & `qapp-common-0.0.4/qapp_common/component/callback/update_job_metadata.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/component/device/device_selection.py` & `qapp-common-0.0.4/qapp_common/component/device/device_selection.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/data/device/circuit_running_option.py` & `qapp-common-0.0.4/qapp_common/data/device/circuit_running_option.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/data/promise/post_processing_promise.py` & `qapp-common-0.0.4/qapp_common/data/promise/post_processing_promise.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/data/request/invocation_request.py` & `qapp-common-0.0.4/qapp_common/data/request/invocation_request.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/data/request/request.py` & `qapp-common-0.0.4/qapp_common/data/request/request.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/data/response/job_response.py` & `qapp-common-0.0.4/qapp_common/data/response/job_response.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/enum/provider_tag.py` & `qapp-common-0.0.4/qapp_common/enum/provider_tag.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/factory/device_factory.py` & `qapp-common-0.0.4/qapp_common/factory/device_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
     QApp Platform Project device_factory.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
+from abc import ABC, abstractmethod
 
 from ..enum.sdk import Sdk
 from ..model.provider.provider import Provider
 
 
-class DeviceFactory:
+class DeviceFactory(ABC):
 
+    @abstractmethod
     def create_device(self, provider: Provider, device_specification: str, authentication: dict, sdk: Sdk):
         """
         @param sdk:
         @param provider:
         @param device_specification:
         @param authentication:
         @return:
```

### Comparing `qapp-common-0.0.3/qapp_common/factory/handler_factory.py` & `qapp-common-0.0.4/qapp_common/factory/handler_factory.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
     QApp Platform Project handler_factory.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
+from abc import ABC
 
 from ..handler.handler import Handler
 from ..config.logging_config import *
 
 
-class HandlerFactory:
+class HandlerFactory(ABC):
+
     @staticmethod
     def create_handler(
             event,
             circuit_preparation_fn,
             post_processing_fn,
     ) -> Handler:
         logger.debug("Create InvocationHandler")
```

### Comparing `qapp-common-0.0.3/qapp_common/model/device/device.py` & `qapp-common-0.0.4/qapp_common/model/device/device.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/model/provider/provider.py` & `qapp-common-0.0.4/qapp_common/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/util/circuit_utils.py` & `qapp-common-0.0.4/qapp_common/util/circuit_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
     QApp Platform Project circuit_utils.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
 
 
 class CircuitUtils:
+
     @staticmethod
     def get_depth(circuit):
         """
 
         @param circuit:
         @return:
         """
```

### Comparing `qapp-common-0.0.3/qapp_common/util/file_utils.py` & `qapp-common-0.0.4/qapp_common/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/util/http_utils.py` & `qapp-common-0.0.4/qapp_common/util/http_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/util/json_parser_utils.py` & `qapp-common-0.0.4/qapp_common/util/json_parser_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common/util/response_utils.py` & `qapp-common-0.0.4/qapp_common/util/response_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.3/qapp_common.egg-info/PKG-INFO` & `qapp-common-0.0.4/qapp_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qapp-common
-Version: 0.0.3
+Version: 0.0.4
 Summary: QApp common library supporting QApp Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `qapp-common-0.0.3/qapp_common.egg-info/SOURCES.txt` & `qapp-common-0.0.4/qapp_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

