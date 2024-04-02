# Comparing `tmp/qapp-common-0.0.1.tar.gz` & `tmp/qapp-common-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qapp-common-0.0.1.tar", last modified: Mon Apr  1 07:41:08 2024, max compression
+gzip compressed data, was "qapp-common-0.0.2.tar", last modified: Tue Apr  2 04:55:47 2024, max compression
```

## Comparing `qapp-common-0.0.1.tar` & `qapp-common-0.0.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.203824 qapp-common-0.0.1/
--rw-rw-rw-   0        0        0     1111 2024-03-27 03:03:06.000000 qapp-common-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1988 2024-04-01 07:41:08.202857 qapp-common-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-04-01 07:05:10.000000 qapp-common-0.0.1/README.md
--rw-rw-rw-   0        0        0      805 2024-04-01 07:34:35.000000 qapp-common-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.062636 qapp-common-0.0.1/qapp_common/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.078636 qapp-common-0.0.1/qapp_common/async_tasks/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/async_tasks/__init__.py
--rw-rw-rw-   0        0        0      212 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/async_tasks/async_task.py
--rw-rw-rw-   0        0        0     3916 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/async_tasks/export_circuit_task.py
--rw-rw-rw-   0        0        0     2298 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/async_tasks/post_processing_task.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.080638 qapp-common-0.0.1/qapp_common/component/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.085637 qapp-common-0.0.1/qapp_common/component/backend/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/component/backend/__init__.py
--rw-rw-rw-   0        0        0     8662 2024-04-01 07:34:35.000000 qapp-common-0.0.1/qapp_common/component/backend/invocation.py
--rw-rw-rw-   0        0        0     6057 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/component/backend/job_fetching.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.088635 qapp-common-0.0.1/qapp_common/component/callback/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/component/callback/__init__.py
--rw-rw-rw-   0        0        0     1241 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/component/callback/update_job_metadata.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.092639 qapp-common-0.0.1/qapp_common/component/device/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/component/device/__init__.py
--rw-rw-rw-   0        0        0     2228 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/component/device/device_selection.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.099671 qapp-common-0.0.1/qapp_common/config/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/config/__init__.py
--rw-rw-rw-   0        0        0      243 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/config/logging_config.py
--rw-rw-rw-   0        0        0      458 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/config/thread_config.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.101671 qapp-common-0.0.1/qapp_common/data/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.104641 qapp-common-0.0.1/qapp_common/data/async_task/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/async_task/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.111652 qapp-common-0.0.1/qapp_common/data/async_task/circuit_export/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/async_task/circuit_export/__init__.py
--rw-rw-rw-   0        0        0      412 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/async_task/circuit_export/backend_holder.py
--rw-rw-rw-   0        0        0      293 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/async_task/circuit_export/circuit_holder.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.116823 qapp-common-0.0.1/qapp_common/data/backend/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/backend/__init__.py
--rw-rw-rw-   0        0        0      462 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/backend/backend_information.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.119825 qapp-common-0.0.1/qapp_common/data/callback/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/callback/__init__.py
--rw-rw-rw-   0        0        0      363 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/callback/callback_url.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.125826 qapp-common-0.0.1/qapp_common/data/device/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/device/__init__.py
--rw-rw-rw-   0        0        0      555 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/device/circuit_running_option.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.131822 qapp-common-0.0.1/qapp_common/data/promise/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/promise/__init__.py
--rw-rw-rw-   0        0        0      698 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/promise/post_processing_promise.py
--rw-rw-rw-   0        0        0      413 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/promise/promise.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.137822 qapp-common-0.0.1/qapp_common/data/request/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/request/__init__.py
--rw-rw-rw-   0        0        0     1024 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/request/invocation_request.py
--rw-rw-rw-   0        0        0      346 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/request/job_fetching_request.py
--rw-rw-rw-   0        0        0     1187 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/request/request.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.147822 qapp-common-0.0.1/qapp_common/data/response/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/response/__init__.py
--rw-rw-rw-   0        0        0      277 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/response/authentication.py
--rw-rw-rw-   0        0        0     1221 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/response/job_response.py
--rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/data/response/project_header.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.163823 qapp-common-0.0.1/qapp_common/enum/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/enum/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/enum/base_enum.py
--rw-rw-rw-   0        0        0      270 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/enum/http_header.py
--rw-rw-rw-   0        0        0      357 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/enum/invocation_step.py
--rw-rw-rw-   0        0        0      359 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/enum/media_type.py
--rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/enum/processing_unit.py
--rw-rw-rw-   0        0        0      587 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/enum/provider_tag.py
--rw-rw-rw-   0        0        0      509 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/enum/sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.167824 qapp-common-0.0.1/qapp_common/enum/status/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/enum/status/__init__.py
--rw-rw-rw-   0        0        0      222 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/enum/status/job_status.py
--rw-rw-rw-   0        0        0      201 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/enum/status/status_code.py
--rw-rw-rw-   0        0        0      196 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/enum/token_type.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.175827 qapp-common-0.0.1/qapp_common/factory/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/factory/__init__.py
--rw-rw-rw-   0        0        0      576 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/factory/device_factory.py
--rw-rw-rw-   0        0        0      513 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/factory/handler_factory.py
--rw-rw-rw-   0        0        0      533 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.178823 qapp-common-0.0.1/qapp_common/handler/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/handler/__init__.py
--rw-rw-rw-   0        0        0      501 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/handler/handler.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.180858 qapp-common-0.0.1/qapp_common/model/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.183822 qapp-common-0.0.1/qapp_common/model/device/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/model/device/__init__.py
--rw-rw-rw-   0        0        0     9546 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/model/device/device.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.186823 qapp-common-0.0.1/qapp_common/model/provider/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/model/provider/__init__.py
--rw-rw-rw-   0        0        0      882 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/model/provider/provider.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.198825 qapp-common-0.0.1/qapp_common/util/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/util/__init__.py
--rw-rw-rw-   0        0        0      562 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/util/circuit_utils.py
--rw-rw-rw-   0        0        0      553 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/util/file_utils.py
--rw-rw-rw-   0        0        0     1071 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/util/http_utils.py
--rw-rw-rw-   0        0        0     2504 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/util/json_parser_utils.py
--rw-rw-rw-   0        0        0     1167 2024-04-01 07:10:10.000000 qapp-common-0.0.1/qapp_common/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:41:08.200825 qapp-common-0.0.1/qapp_common.egg-info/
--rw-rw-rw-   0        0        0     1988 2024-04-01 07:41:07.000000 qapp-common-0.0.1/qapp_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2800 2024-04-01 07:41:08.000000 qapp-common-0.0.1/qapp_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 07:41:07.000000 qapp-common-0.0.1/qapp_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-04-01 07:41:07.000000 qapp-common-0.0.1/qapp_common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-01 07:41:07.000000 qapp-common-0.0.1/qapp_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 07:41:08.203824 qapp-common-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.074511 qapp-common-0.0.2/
+-rw-rw-rw-   0        0        0     1111 2024-03-27 03:03:06.000000 qapp-common-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1988 2024-04-02 04:55:47.072509 qapp-common-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-04-01 07:05:10.000000 qapp-common-0.0.2/README.md
+-rw-rw-rw-   0        0        0      805 2024-04-02 04:55:37.000000 qapp-common-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.948533 qapp-common-0.0.2/qapp_common/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.961495 qapp-common-0.0.2/qapp_common/async_tasks/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/async_tasks/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/async_tasks/async_task.py
+-rw-rw-rw-   0        0        0     3916 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/async_tasks/export_circuit_task.py
+-rw-rw-rw-   0        0        0     2298 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/async_tasks/post_processing_task.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.962495 qapp-common-0.0.2/qapp_common/component/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.966496 qapp-common-0.0.2/qapp_common/component/backend/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/backend/__init__.py
+-rw-rw-rw-   0        0        0     8374 2024-04-02 04:55:37.000000 qapp-common-0.0.2/qapp_common/component/backend/invocation.py
+-rw-rw-rw-   0        0        0     6057 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/backend/job_fetching.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.969496 qapp-common-0.0.2/qapp_common/component/callback/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/callback/__init__.py
+-rw-rw-rw-   0        0        0     1241 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/callback/update_job_metadata.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.973496 qapp-common-0.0.2/qapp_common/component/device/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/device/__init__.py
+-rw-rw-rw-   0        0        0     2228 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/component/device/device_selection.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.980517 qapp-common-0.0.2/qapp_common/config/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/config/__init__.py
+-rw-rw-rw-   0        0        0      243 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/config/logging_config.py
+-rw-rw-rw-   0        0        0      458 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/config/thread_config.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.982496 qapp-common-0.0.2/qapp_common/data/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.984496 qapp-common-0.0.2/qapp_common/data/async_task/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/async_task/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.990528 qapp-common-0.0.2/qapp_common/data/async_task/circuit_export/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/async_task/circuit_export/__init__.py
+-rw-rw-rw-   0        0        0      412 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/async_task/circuit_export/backend_holder.py
+-rw-rw-rw-   0        0        0      293 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/async_task/circuit_export/circuit_holder.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.993497 qapp-common-0.0.2/qapp_common/data/backend/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/backend/__init__.py
+-rw-rw-rw-   0        0        0      462 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/backend/backend_information.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:46.997496 qapp-common-0.0.2/qapp_common/data/callback/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/callback/__init__.py
+-rw-rw-rw-   0        0        0      363 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/callback/callback_url.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.002498 qapp-common-0.0.2/qapp_common/data/device/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/device/__init__.py
+-rw-rw-rw-   0        0        0      555 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/device/circuit_running_option.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.007495 qapp-common-0.0.2/qapp_common/data/promise/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/promise/__init__.py
+-rw-rw-rw-   0        0        0      698 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/promise/post_processing_promise.py
+-rw-rw-rw-   0        0        0      413 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/promise/promise.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.016497 qapp-common-0.0.2/qapp_common/data/request/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/request/__init__.py
+-rw-rw-rw-   0        0        0     1024 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/request/invocation_request.py
+-rw-rw-rw-   0        0        0      346 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/request/job_fetching_request.py
+-rw-rw-rw-   0        0        0     1187 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/request/request.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.022499 qapp-common-0.0.2/qapp_common/data/response/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/response/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/response/authentication.py
+-rw-rw-rw-   0        0        0     1221 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/response/job_response.py
+-rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/data/response/project_header.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.036513 qapp-common-0.0.2/qapp_common/enum/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/base_enum.py
+-rw-rw-rw-   0        0        0      270 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/http_header.py
+-rw-rw-rw-   0        0        0      357 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/invocation_step.py
+-rw-rw-rw-   0        0        0      359 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/media_type.py
+-rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      587 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/provider_tag.py
+-rw-rw-rw-   0        0        0      509 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.041512 qapp-common-0.0.2/qapp_common/enum/status/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/status/__init__.py
+-rw-rw-rw-   0        0        0      222 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/status/job_status.py
+-rw-rw-rw-   0        0        0      201 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/status/status_code.py
+-rw-rw-rw-   0        0        0      196 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/enum/token_type.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.048514 qapp-common-0.0.2/qapp_common/factory/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/factory/__init__.py
+-rw-rw-rw-   0        0        0      576 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/factory/device_factory.py
+-rw-rw-rw-   0        0        0      513 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/factory/handler_factory.py
+-rw-rw-rw-   0        0        0      533 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.051511 qapp-common-0.0.2/qapp_common/handler/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/handler/__init__.py
+-rw-rw-rw-   0        0        0      501 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/handler/handler.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.053514 qapp-common-0.0.2/qapp_common/model/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.055512 qapp-common-0.0.2/qapp_common/model/device/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/model/device/__init__.py
+-rw-rw-rw-   0        0        0     9546 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/model/device/device.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.058514 qapp-common-0.0.2/qapp_common/model/provider/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/model/provider/__init__.py
+-rw-rw-rw-   0        0        0      882 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/model/provider/provider.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.069512 qapp-common-0.0.2/qapp_common/util/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/util/__init__.py
+-rw-rw-rw-   0        0        0      562 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/util/circuit_utils.py
+-rw-rw-rw-   0        0        0      553 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/util/file_utils.py
+-rw-rw-rw-   0        0        0     1071 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/util/http_utils.py
+-rw-rw-rw-   0        0        0     2504 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/util/json_parser_utils.py
+-rw-rw-rw-   0        0        0     1167 2024-04-01 07:10:10.000000 qapp-common-0.0.2/qapp_common/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:55:47.071510 qapp-common-0.0.2/qapp_common.egg-info/
+-rw-rw-rw-   0        0        0     1988 2024-04-02 04:55:46.000000 qapp-common-0.0.2/qapp_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2800 2024-04-02 04:55:46.000000 qapp-common-0.0.2/qapp_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 04:55:46.000000 qapp-common-0.0.2/qapp_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-02 04:55:46.000000 qapp-common-0.0.2/qapp_common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-02 04:55:46.000000 qapp-common-0.0.2/qapp_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 04:55:47.074511 qapp-common-0.0.2/setup.cfg
```

### Comparing `qapp-common-0.0.1/LICENSE` & `qapp-common-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/PKG-INFO` & `qapp-common-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qapp-common
-Version: 0.0.1
+Version: 0.0.2
 Summary: QApp common library supporting QApp Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `qapp-common-0.0.1/pyproject.toml` & `qapp-common-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qapp-common"
-version = "0.0.1"
+version = "0.0.2"
 description = "QApp common library supporting QApp Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `qapp-common-0.0.1/qapp_common/async_tasks/export_circuit_task.py` & `qapp-common-0.0.2/qapp_common/async_tasks/export_circuit_task.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/async_tasks/post_processing_task.py` & `qapp-common-0.0.2/qapp_common/async_tasks/post_processing_task.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/component/backend/invocation.py` & `qapp-common-0.0.2/qapp_common/component/backend/invocation.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,22 @@
 from ...data.response.job_response import JobResponse
 from ...data.response.project_header import ProjectHeader
 from ...enum.invocation_step import InvocationStep
 from ...enum.media_type import MediaType
 from ...enum.sdk import Sdk
 from ...enum.status.job_status import JobStatus
 from ...enum.status.status_code import StatusCode
-from ...factory.device_factory import DeviceFactory
-from ...factory.provider_factory import ProviderFactory
 from ...model.provider.provider import Provider
 from ...util.circuit_utils import CircuitUtils
 
 EXPORT_CIRCUIT_SDK = {Sdk.QISKIT, Sdk.BRAKET}
 
 
 class Invocation(ABC):
-    def __init__(self, request_data: InvocationRequest, provider_factory: ProviderFactory,
-                 device_factory: DeviceFactory):
+    def __init__(self, request_data: InvocationRequest):
         self.sdk: Sdk = Sdk.resolve(request_data.sdk)
         self.input = request_data.input
         self.device_id = request_data.device_id
         self.backend_information: BackendInformation
         self.authentication: Authentication = request_data.authentication
         self.project_header: ProjectHeader = request_data.project_header
         self.options = CircuitRunningOption(
@@ -45,16 +42,14 @@
         self.circuit_export_url: str = request_data.circuit_export_url
         self.callback_dict: dict = {
             InvocationStep.PREPARATION: request_data.preparation,
             InvocationStep.EXECUTION: request_data.execution,
             InvocationStep.ANALYSIS: request_data.analysis,
             InvocationStep.FINALIZATION: request_data.finalization,
         }
-        self.providerFactory = provider_factory
-        self.deviceFactory = device_factory
 
     def submit_job(self, circuit_preparation_fn, post_processing_fn):
         """
 
         @param post_processing_fn: Post-processing function
         @param circuit_preparation_fn: Circuit-preparation function
         @return: Job result
```

### Comparing `qapp-common-0.0.1/qapp_common/component/backend/job_fetching.py` & `qapp-common-0.0.2/qapp_common/component/backend/job_fetching.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/component/callback/update_job_metadata.py` & `qapp-common-0.0.2/qapp_common/component/callback/update_job_metadata.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/component/device/device_selection.py` & `qapp-common-0.0.2/qapp_common/component/device/device_selection.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/data/device/circuit_running_option.py` & `qapp-common-0.0.2/qapp_common/data/device/circuit_running_option.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/data/promise/post_processing_promise.py` & `qapp-common-0.0.2/qapp_common/data/promise/post_processing_promise.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/data/request/invocation_request.py` & `qapp-common-0.0.2/qapp_common/data/request/invocation_request.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/data/request/request.py` & `qapp-common-0.0.2/qapp_common/data/request/request.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/data/response/job_response.py` & `qapp-common-0.0.2/qapp_common/data/response/job_response.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/enum/provider_tag.py` & `qapp-common-0.0.2/qapp_common/enum/provider_tag.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/factory/device_factory.py` & `qapp-common-0.0.2/qapp_common/factory/device_factory.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/factory/handler_factory.py` & `qapp-common-0.0.2/qapp_common/factory/handler_factory.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/factory/provider_factory.py` & `qapp-common-0.0.2/qapp_common/factory/provider_factory.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/model/device/device.py` & `qapp-common-0.0.2/qapp_common/model/device/device.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/model/provider/provider.py` & `qapp-common-0.0.2/qapp_common/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/util/circuit_utils.py` & `qapp-common-0.0.2/qapp_common/util/circuit_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/util/file_utils.py` & `qapp-common-0.0.2/qapp_common/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/util/http_utils.py` & `qapp-common-0.0.2/qapp_common/util/http_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/util/json_parser_utils.py` & `qapp-common-0.0.2/qapp_common/util/json_parser_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common/util/response_utils.py` & `qapp-common-0.0.2/qapp_common/util/response_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.1/qapp_common.egg-info/PKG-INFO` & `qapp-common-0.0.2/qapp_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qapp-common
-Version: 0.0.1
+Version: 0.0.2
 Summary: QApp common library supporting QApp Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `qapp-common-0.0.1/qapp_common.egg-info/SOURCES.txt` & `qapp-common-0.0.2/qapp_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

