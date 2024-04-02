# Comparing `tmp/qapp-common-0.0.2.tar.gz` & `tmp/qapp-common-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qapp-common-0.0.2.tar", last modified: Tue Apr  2 04:55:47 2024, max compression
+gzip compressed data, was "qapp-common-0.0.3.tar", last modified: Tue Apr  2 07:24:37 2024, max compression
```

## Comparing `qapp-common-0.0.2.tar` & `qapp-common-0.0.3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.074511 qapp-common-0.0.2/
--rw-rw-rw-   0        0        0     1111 2024-03-27 03:03:06.000000 qapp-common-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1988 2024-04-02 04:55:47.072509 qapp-common-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-04-01 07:05:10.000000 qapp-common-0.0.2/README.md
--rw-rw-rw-   0        0        0      805 2024-04-02 04:55:37.000000 qapp-common-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.948533 qapp-common-0.0.2/qapp_common/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.961495 qapp-common-0.0.2/qapp_common/async_tasks/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/async_tasks/__init__.py
--rw-rw-rw-   0        0        0      212 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/async_tasks/async_task.py
--rw-rw-rw-   0        0        0     3916 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/async_tasks/export_circuit_task.py
--rw-rw-rw-   0        0        0     2298 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/async_tasks/post_processing_task.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.962495 qapp-common-0.0.2/qapp_common/component/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.966496 qapp-common-0.0.2/qapp_common/component/backend/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/backend/__init__.py
--rw-rw-rw-   0        0        0     8374 2024-04-02 04:55:37.000000 qapp-common-0.0.2/qapp_common/component/backend/invocation.py
--rw-rw-rw-   0        0        0     6057 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/backend/job_fetching.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.969496 qapp-common-0.0.2/qapp_common/component/callback/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/callback/__init__.py
--rw-rw-rw-   0        0        0     1241 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/callback/update_job_metadata.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.973496 qapp-common-0.0.2/qapp_common/component/device/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/device/__init__.py
--rw-rw-rw-   0        0        0     2228 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/device/device_selection.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.980517 qapp-common-0.0.2/qapp_common/config/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/config/__init__.py
--rw-rw-rw-   0        0        0      243 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/config/logging_config.py
--rw-rw-rw-   0        0        0      458 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/config/thread_config.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.982496 qapp-common-0.0.2/qapp_common/data/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.984496 qapp-common-0.0.2/qapp_common/data/async_task/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/async_task/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.990528 qapp-common-0.0.2/qapp_common/data/async_task/circuit_export/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/async_task/circuit_export/__init__.py
--rw-rw-rw-   0        0        0      412 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/async_task/circuit_export/backend_holder.py
--rw-rw-rw-   0        0        0      293 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/async_task/circuit_export/circuit_holder.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.993497 qapp-common-0.0.2/qapp_common/data/backend/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/backend/__init__.py
--rw-rw-rw-   0        0        0      462 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/backend/backend_information.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.997496 qapp-common-0.0.2/qapp_common/data/callback/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/callback/__init__.py
--rw-rw-rw-   0        0        0      363 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/callback/callback_url.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.002498 qapp-common-0.0.2/qapp_common/data/device/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/device/__init__.py
--rw-rw-rw-   0        0        0      555 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/device/circuit_running_option.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.007495 qapp-common-0.0.2/qapp_common/data/promise/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/promise/__init__.py
--rw-rw-rw-   0        0        0      698 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/promise/post_processing_promise.py
--rw-rw-rw-   0        0        0      413 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/promise/promise.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.016497 qapp-common-0.0.2/qapp_common/data/request/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/request/__init__.py
--rw-rw-rw-   0        0        0     1024 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/request/invocation_request.py
--rw-rw-rw-   0        0        0      346 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/request/job_fetching_request.py
--rw-rw-rw-   0        0        0     1187 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/request/request.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.022499 qapp-common-0.0.2/qapp_common/data/response/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/response/__init__.py
--rw-rw-rw-   0        0        0      277 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/response/authentication.py
--rw-rw-rw-   0        0        0     1221 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/response/job_response.py
--rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/response/project_header.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.036513 qapp-common-0.0.2/qapp_common/enum/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/base_enum.py
--rw-rw-rw-   0        0        0      270 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/http_header.py
--rw-rw-rw-   0        0        0      357 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/invocation_step.py
--rw-rw-rw-   0        0        0      359 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/media_type.py
--rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/processing_unit.py
--rw-rw-rw-   0        0        0      587 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/provider_tag.py
--rw-rw-rw-   0        0        0      509 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.041512 qapp-common-0.0.2/qapp_common/enum/status/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/status/__init__.py
--rw-rw-rw-   0        0        0      222 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/status/job_status.py
--rw-rw-rw-   0        0        0      201 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/status/status_code.py
--rw-rw-rw-   0        0        0      196 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/token_type.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.048514 qapp-common-0.0.2/qapp_common/factory/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/factory/__init__.py
--rw-rw-rw-   0        0        0      576 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/factory/device_factory.py
--rw-rw-rw-   0        0        0      513 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/factory/handler_factory.py
--rw-rw-rw-   0        0        0      533 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.051511 qapp-common-0.0.2/qapp_common/handler/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/handler/__init__.py
--rw-rw-rw-   0        0        0      501 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/handler/handler.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.053514 qapp-common-0.0.2/qapp_common/model/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.055512 qapp-common-0.0.2/qapp_common/model/device/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/model/device/__init__.py
--rw-rw-rw-   0        0        0     9546 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/model/device/device.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.058514 qapp-common-0.0.2/qapp_common/model/provider/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/model/provider/__init__.py
--rw-rw-rw-   0        0        0      882 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/model/provider/provider.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.069512 qapp-common-0.0.2/qapp_common/util/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/util/__init__.py
--rw-rw-rw-   0        0        0      562 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/util/circuit_utils.py
--rw-rw-rw-   0        0        0      553 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/util/file_utils.py
--rw-rw-rw-   0        0        0     1071 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/util/http_utils.py
--rw-rw-rw-   0        0        0     2504 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/util/json_parser_utils.py
--rw-rw-rw-   0        0        0     1167 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.071510 qapp-common-0.0.2/qapp_common.egg-info/
--rw-rw-rw-   0        0        0     1988 2024-04-02 04:55:46.000000 qapp-common-0.0.2/qapp_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2800 2024-04-02 04:55:46.000000 qapp-common-0.0.2/qapp_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 04:55:46.000000 qapp-common-0.0.2/qapp_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-04-02 04:55:46.000000 qapp-common-0.0.2/qapp_common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-02 04:55:46.000000 qapp-common-0.0.2/qapp_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 04:55:47.074511 qapp-common-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:37.015350 qapp-common-0.0.3/
+-rw-rw-rw-   0        0        0     1111 2024-03-27 03:03:06.000000 qapp-common-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1988 2024-04-02 07:24:37.012350 qapp-common-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-04-01 07:05:10.000000 qapp-common-0.0.3/README.md
+-rw-rw-rw-   0        0        0      805 2024-04-02 07:24:25.000000 qapp-common-0.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.828353 qapp-common-0.0.3/qapp_common/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.847353 qapp-common-0.0.3/qapp_common/async_tasks/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/async_tasks/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/async_tasks/async_task.py
+-rw-rw-rw-   0        0        0     3916 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/async_tasks/export_circuit_task.py
+-rw-rw-rw-   0        0        0     2298 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/async_tasks/post_processing_task.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.849350 qapp-common-0.0.3/qapp_common/component/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.856351 qapp-common-0.0.3/qapp_common/component/backend/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/component/backend/__init__.py
+-rw-rw-rw-   0        0        0     8374 2024-04-02 04:55:37.000000 qapp-common-0.0.3/qapp_common/component/backend/invocation.py
+-rw-rw-rw-   0        0        0     9503 2024-04-02 07:18:05.000000 qapp-common-0.0.3/qapp_common/component/backend/job_fetching.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.859349 qapp-common-0.0.3/qapp_common/component/callback/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/component/callback/__init__.py
+-rw-rw-rw-   0        0        0     1241 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/component/callback/update_job_metadata.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.874352 qapp-common-0.0.3/qapp_common/component/device/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/component/device/__init__.py
+-rw-rw-rw-   0        0        0     2228 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/component/device/device_selection.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.881354 qapp-common-0.0.3/qapp_common/config/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/config/__init__.py
+-rw-rw-rw-   0        0        0      243 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/config/logging_config.py
+-rw-rw-rw-   0        0        0      458 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/config/thread_config.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.884350 qapp-common-0.0.3/qapp_common/data/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.886383 qapp-common-0.0.3/qapp_common/data/async_task/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/async_task/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.893352 qapp-common-0.0.3/qapp_common/data/async_task/circuit_export/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/async_task/circuit_export/__init__.py
+-rw-rw-rw-   0        0        0      412 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/async_task/circuit_export/backend_holder.py
+-rw-rw-rw-   0        0        0      293 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/async_task/circuit_export/circuit_holder.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.898352 qapp-common-0.0.3/qapp_common/data/backend/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/backend/__init__.py
+-rw-rw-rw-   0        0        0      462 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/backend/backend_information.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.901350 qapp-common-0.0.3/qapp_common/data/callback/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/callback/__init__.py
+-rw-rw-rw-   0        0        0      363 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/callback/callback_url.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.907350 qapp-common-0.0.3/qapp_common/data/device/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/device/__init__.py
+-rw-rw-rw-   0        0        0      555 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/device/circuit_running_option.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.917352 qapp-common-0.0.3/qapp_common/data/promise/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/promise/__init__.py
+-rw-rw-rw-   0        0        0      698 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/promise/post_processing_promise.py
+-rw-rw-rw-   0        0        0      413 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/promise/promise.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.927352 qapp-common-0.0.3/qapp_common/data/request/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/request/__init__.py
+-rw-rw-rw-   0        0        0     1024 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/request/invocation_request.py
+-rw-rw-rw-   0        0        0      346 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/request/job_fetching_request.py
+-rw-rw-rw-   0        0        0     1187 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/request/request.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.937349 qapp-common-0.0.3/qapp_common/data/response/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/response/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/response/authentication.py
+-rw-rw-rw-   0        0        0     1221 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/response/job_response.py
+-rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/data/response/project_header.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.960351 qapp-common-0.0.3/qapp_common/enum/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/base_enum.py
+-rw-rw-rw-   0        0        0      270 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/http_header.py
+-rw-rw-rw-   0        0        0      357 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/invocation_step.py
+-rw-rw-rw-   0        0        0      359 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/media_type.py
+-rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      587 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/provider_tag.py
+-rw-rw-rw-   0        0        0      509 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.967348 qapp-common-0.0.3/qapp_common/enum/status/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/status/__init__.py
+-rw-rw-rw-   0        0        0      222 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/status/job_status.py
+-rw-rw-rw-   0        0        0      201 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/status/status_code.py
+-rw-rw-rw-   0        0        0      196 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/enum/token_type.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.975350 qapp-common-0.0.3/qapp_common/factory/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/factory/__init__.py
+-rw-rw-rw-   0        0        0      576 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/factory/device_factory.py
+-rw-rw-rw-   0        0        0      513 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/factory/handler_factory.py
+-rw-rw-rw-   0        0        0      533 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.979350 qapp-common-0.0.3/qapp_common/handler/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/handler/__init__.py
+-rw-rw-rw-   0        0        0      501 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/handler/handler.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.982350 qapp-common-0.0.3/qapp_common/model/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.986350 qapp-common-0.0.3/qapp_common/model/device/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/model/device/__init__.py
+-rw-rw-rw-   0        0        0     9546 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/model/device/device.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:36.992351 qapp-common-0.0.3/qapp_common/model/provider/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/model/provider/__init__.py
+-rw-rw-rw-   0        0        0      882 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/model/provider/provider.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:37.006348 qapp-common-0.0.3/qapp_common/util/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/util/__init__.py
+-rw-rw-rw-   0        0        0      562 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/util/circuit_utils.py
+-rw-rw-rw-   0        0        0      553 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/util/file_utils.py
+-rw-rw-rw-   0        0        0     1071 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/util/http_utils.py
+-rw-rw-rw-   0        0        0     2504 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/util/json_parser_utils.py
+-rw-rw-rw-   0        0        0     1167 2024-04-01 07:10:10.000000 qapp-common-0.0.3/qapp_common/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:24:37.009350 qapp-common-0.0.3/qapp_common.egg-info/
+-rw-rw-rw-   0        0        0     1988 2024-04-02 07:24:36.000000 qapp-common-0.0.3/qapp_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2800 2024-04-02 07:24:36.000000 qapp-common-0.0.3/qapp_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 07:24:36.000000 qapp-common-0.0.3/qapp_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-02 07:24:36.000000 qapp-common-0.0.3/qapp_common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-02 07:24:36.000000 qapp-common-0.0.3/qapp_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 07:24:37.015350 qapp-common-0.0.3/setup.cfg
```

### Comparing `qapp-common-0.0.2/LICENSE` & `qapp-common-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/PKG-INFO` & `qapp-common-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qapp-common
-Version: 0.0.2
+Version: 0.0.3
 Summary: QApp common library supporting QApp Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `qapp-common-0.0.2/pyproject.toml` & `qapp-common-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qapp-common"
-version = "0.0.2"
+version = "0.0.3"
 description = "QApp common library supporting QApp Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `qapp-common-0.0.2/qapp_common/async_tasks/export_circuit_task.py` & `qapp-common-0.0.3/qapp_common/async_tasks/export_circuit_task.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/async_tasks/post_processing_task.py` & `qapp-common-0.0.3/qapp_common/async_tasks/post_processing_task.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/component/backend/invocation.py` & `qapp-common-0.0.3/qapp_common/component/backend/invocation.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/component/backend/job_fetching.py` & `qapp-common-0.0.3/qapp_common/component/backend/job_fetching.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 """
     QApp Platform Project job_fetching.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
-
+from abc import ABC, abstractmethod
 from typing import Any
 
 from ..callback.update_job_metadata import update_job_metadata
 from ...async_tasks.post_processing_task import PostProcessingTask
+from ...config.thread_config import circuit_running_pool
 from ...data.callback.callback_url import CallbackUrl
 from ...data.promise.post_processing_promise import PostProcessingPromise
 from ...data.request.job_fetching_request import JobFetchingRequest
 from ...data.response.authentication import Authentication
 from ...data.response.job_response import JobResponse
 from ...data.response.project_header import ProjectHeader
 from ...enum.invocation_step import InvocationStep
 from ...config.logging_config import logger
 from ...enum.media_type import MediaType
+from ...enum.provider_tag import ProviderTag
+from ...enum.sdk import Sdk
 from ...enum.status.job_status import JobStatus
 from ...enum.status.status_code import StatusCode
+from ...factory.provider_factory import ProviderFactory
 from ...util.json_parser_utils import JsonParserUtils
+from ...util.response_utils import ResponseUtils
 
 
-class JobFetching:
+class JobFetching(ABC):
     def __init__(self, request_data: JobFetchingRequest):
         self.provider_authentication: dict = request_data.provider_authentication
         self.provider_job_id: str = request_data.provider_job_id
         self.backend_authentication: Authentication = request_data.authentication
         self.project_header: ProjectHeader = request_data.project_header
         self.callback_dict: dict = {
             InvocationStep.EXECUTION: request_data.execution,
@@ -34,16 +39,69 @@
 
     def fetch(self, post_processing_fn):
         """
 
         @param post_processing_fn:
         @return:
         """
+        logger.debug("[Fetching] Fetch job")
+
+        job_response = JobResponse(
+            provider_job_id=self.provider_job_id,
+            authentication=self.backend_authentication,
+            project_header=self.project_header,
+            status_code=StatusCode.DONE)
+
+        try:
+            provider = self._collect_provider()
+
+            job = self._retrieve_job(provider)
+            job_status = self._get_job_status(job)
+            original_job_result = self._get_job_result(job)
+
+            job_response.job_status = job_status
+
+            if JobStatus.DONE.value.__eq__(job_response.job_status):
+                circuit_running_pool.submit(self.__handle_job_result,
+                                            original_job_result,
+                                            job_response,
+                                            self.callback_dict,
+                                            post_processing_fn)
+
+                update_job_metadata(
+                    job_response=job_response,
+                    callback_url=self.callback_dict.get(InvocationStep.EXECUTION).on_done)
+
+            elif JobStatus.ERROR.value.__eq__(job_response.job_status):
+                job_response.job_result = JsonParserUtils.parse(original_job_result)
+
+                update_job_metadata(
+                    job_response=job_response,
+                    callback_url=self.callback_dict.get(InvocationStep.EXECUTION).on_error)
+
+            else:
+                job_response.status_code = StatusCode.POLLING
+
+        except Exception as exception:
+            logger.debug("Exception when fetch job with provider_job_id {0}: {1}".format(
+                self.provider_job_id, str(exception)))
+
+            job_response.job_result = {
+                "error": "Exception when fetch job with provider_job_id {0}: {1}".format(
+                    self.provider_job_id, str(exception)),
+                "exception": str(exception),
+            }
+            job_response.status_code = StatusCode.ERROR
+            job_response.job_status = JobStatus.ERROR.value
+
+            update_job_metadata(
+                job_response=job_response,
+                callback_url=self.callback_dict.get(InvocationStep.EXECUTION).on_error)
 
-        raise Exception("[JobFetching] fetch")
+        return ResponseUtils.generate_response(job_response)
 
     def __handle_job_result(self,
                             original_job_result,
                             job_response: JobResponse,
                             callback_dict: dict,
                             post_processing_fn):
         """
@@ -140,16 +198,16 @@
         @param job_result:
         @return:
         """
         logger.debug("[Fetching] Produce histogram")
 
         try:
             return job_result.get_counts()
-        except Exception as exception:
-            logger.debug("Can't produce histogram with error: {0}".format(str(exception)))
+        except Exception as qiskit_error:
+            logger.debug("Can't produce histogram with error: {0}".format(str(qiskit_error)))
             return None
 
     @staticmethod
     def __get_execution_time(job_result):
         """
 
         @param job_result:
@@ -166,7 +224,39 @@
                 metadata is None
                 or not bool(metadata)
                 or "time_taken_execute" not in metadata
         ):
             return None
 
         return metadata["time_taken_execute"]
+
+    @abstractmethod
+    def _collect_provider(self, ):
+        """
+        Create provider with ProviderFactory
+        """
+
+        raise NotImplemented('[Invocation] _create_provider() method must be implemented')
+
+    @abstractmethod
+    def _retrieve_job(self, provider):
+        """
+        Retrieve job from provider
+        """
+
+        raise NotImplemented('[Invocation] _retrieve_job() method must be implemented')
+
+    @abstractmethod
+    def _get_job_status(self, job):
+        """
+        Get job status
+        """
+
+        raise NotImplemented('[Invocation] _get_job_status() method must be implemented')
+
+    @abstractmethod
+    def _get_job_result(self, job):
+        """
+        Get job result
+        """
+
+        raise NotImplemented('[Invocation] _get_job_result() method must be implemented')
```

### Comparing `qapp-common-0.0.2/qapp_common/component/callback/update_job_metadata.py` & `qapp-common-0.0.3/qapp_common/component/callback/update_job_metadata.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/component/device/device_selection.py` & `qapp-common-0.0.3/qapp_common/component/device/device_selection.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/data/device/circuit_running_option.py` & `qapp-common-0.0.3/qapp_common/data/device/circuit_running_option.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/data/promise/post_processing_promise.py` & `qapp-common-0.0.3/qapp_common/data/promise/post_processing_promise.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/data/request/invocation_request.py` & `qapp-common-0.0.3/qapp_common/data/request/invocation_request.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/data/request/request.py` & `qapp-common-0.0.3/qapp_common/data/request/request.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/data/response/job_response.py` & `qapp-common-0.0.3/qapp_common/data/response/job_response.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/enum/provider_tag.py` & `qapp-common-0.0.3/qapp_common/enum/provider_tag.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/factory/device_factory.py` & `qapp-common-0.0.3/qapp_common/factory/device_factory.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/factory/handler_factory.py` & `qapp-common-0.0.3/qapp_common/factory/handler_factory.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/factory/provider_factory.py` & `qapp-common-0.0.3/qapp_common/factory/provider_factory.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/model/device/device.py` & `qapp-common-0.0.3/qapp_common/model/device/device.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/model/provider/provider.py` & `qapp-common-0.0.3/qapp_common/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/util/circuit_utils.py` & `qapp-common-0.0.3/qapp_common/util/circuit_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/util/file_utils.py` & `qapp-common-0.0.3/qapp_common/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/util/http_utils.py` & `qapp-common-0.0.3/qapp_common/util/http_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/util/json_parser_utils.py` & `qapp-common-0.0.3/qapp_common/util/json_parser_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common/util/response_utils.py` & `qapp-common-0.0.3/qapp_common/util/response_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.2/qapp_common.egg-info/PKG-INFO` & `qapp-common-0.0.3/qapp_common.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qapp-common
-Version: 0.0.2
+Version: 0.0.3
 Summary: QApp common library supporting QApp Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `qapp-common-0.0.2/qapp_common.egg-info/SOURCES.txt` & `qapp-common-0.0.3/qapp_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

