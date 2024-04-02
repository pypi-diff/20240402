# Comparing `tmp/edx-event-routing-backends-8.3.1.tar.gz` & `tmp/edx-event-routing-backends-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-event-routing-backends-8.3.1.tar", last modified: Mon Apr  1 19:55:33 2024, max compression
+gzip compressed data, was "edx-event-routing-backends-9.0.0.tar", last modified: Tue Apr  2 20:17:15 2024, max compression
```

## Comparing `edx-event-routing-backends-8.3.1.tar` & `edx-event-routing-backends-9.0.0.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/backends/async_events_router.py
--rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/backends/events_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/backends/sync_events_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44356 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/backends/tests/test_events_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/helpers/event_log_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/helpers/queued_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/recover_failed_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/tests/test_recover_failed_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/transform_tracking_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0002_auto_20210503_0648.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0003_auto_20210713_0344.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0004_auto_20211025_1053.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/envelope_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/test_caliper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/mixins/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/mixins/base_transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/openedx_filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/openedx_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/openedx_filters/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/transformers_test_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.378018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.378018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/tests/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.378018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.378018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/completion_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/exam_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/forum_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/grading_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    16362 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.378018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/test_xapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/test_xapi_event_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/event_routing_backends/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.366018 edx-event-routing-backends-8.3.1/event_routing_backends/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.366018 edx-event-routing-backends-8.3.1/event_routing_backends/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/event_routing_backends/static/admin/js/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.366018 edx-event-routing-backends-8.3.1/event_routing_backends/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/event_routing_backends/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/templates/admin/router_conf_change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/event_routing_backends/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/event_routing_backends/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/utils/xapi_lrs_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.294139 edx-event-routing-backends-9.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-02 20:17:15.294139 edx-event-routing-backends-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.294139 edx-event-routing-backends-9.0.0/edx_event_routing_backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-02 20:17:15.000000 edx-event-routing-backends-9.0.0/edx_event_routing_backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-02 20:17:15.000000 edx-event-routing-backends-9.0.0/edx_event_routing_backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:17:15.000000 edx-event-routing-backends-9.0.0/edx_event_routing_backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-02 20:17:15.000000 edx-event-routing-backends-9.0.0/edx_event_routing_backends.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:17:15.000000 edx-event-routing-backends-9.0.0/edx_event_routing_backends.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-02 20:17:15.000000 edx-event-routing-backends-9.0.0/edx_event_routing_backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 20:17:15.000000 edx-event-routing-backends-9.0.0/edx_event_routing_backends.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.278138 edx-event-routing-backends-9.0.0/event_routing_backends/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.282138 edx-event-routing-backends-9.0.0/event_routing_backends/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/backends/async_events_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13293 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/backends/events_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/backends/sync_events_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.282138 edx-event-routing-backends-9.0.0/event_routing_backends/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44447 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/backends/tests/test_events_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.282138 edx-event-routing-backends-9.0.0/event_routing_backends/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.282138 edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.282138 edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/helpers/event_log_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/helpers/queued_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/recover_failed_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.282138 edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/tests/test_recover_failed_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15596 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/transform_tracking_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.282138 edx-event-routing-backends-9.0.0/event_routing_backends/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/migrations/0002_auto_20210503_0648.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/migrations/0003_auto_20210713_0344.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/migrations/0004_auto_20211025_1053.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.282138 edx-event-routing-backends-9.0.0/event_routing_backends/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.286139 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/envelope_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.286139 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.286139 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/tests/test_caliper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.286139 edx-event-routing-backends-9.0.0/event_routing_backends/processors/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/mixins/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/mixins/base_transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.286139 edx-event-routing-backends-9.0.0/event_routing_backends/processors/openedx_filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/openedx_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/openedx_filters/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/openedx_filters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/openedx_filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.286139 edx-event-routing-backends-9.0.0/event_routing_backends/processors/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.286139 edx-event-routing-backends-9.0.0/event_routing_backends/processors/tests/openedx_filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/tests/openedx_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/tests/openedx_filters/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/tests/transformers_test_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.290139 edx-event-routing-backends-9.0.0/event_routing_backends/processors/transformer_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/transformer_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/transformer_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/transformer_utils/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.290139 edx-event-routing-backends-9.0.0/event_routing_backends/processors/transformer_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/transformer_utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.290139 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.290139 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/completion_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/exam_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/forum_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/grading_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16362 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.290139 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/tests/test_xapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/tests/test_xapi_event_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.294139 edx-event-routing-backends-9.0.0/event_routing_backends/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/settings/production.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.274139 edx-event-routing-backends-9.0.0/event_routing_backends/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.274139 edx-event-routing-backends-9.0.0/event_routing_backends/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.294139 edx-event-routing-backends-9.0.0/event_routing_backends/static/admin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.278138 edx-event-routing-backends-9.0.0/event_routing_backends/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.294139 edx-event-routing-backends-9.0.0/event_routing_backends/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/templates/admin/router_conf_change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.294139 edx-event-routing-backends-9.0.0/event_routing_backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.294139 edx-event-routing-backends-9.0.0/event_routing_backends/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/event_routing_backends/utils/xapi_lrs_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.294139 edx-event-routing-backends-9.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-02 20:17:15.294139 edx-event-routing-backends-9.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-02 20:17:12.000000 edx-event-routing-backends-9.0.0/setup.py
```

### Comparing `edx-event-routing-backends-8.3.1/CHANGELOG.rst` & `edx-event-routing-backends-9.0.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[9.0.0]
+~~~~~~~
+
+* **BREAKING CHANGE**: Use a single entry point for all event routing backends.
+  which allows to easily switch bettwen celery and the event bus for the backends.
+
 [8.3.0]
 
 * Allow to use any configured engine to replay tracking logs
 
 [8.2.0]
 
 * Add support for batching for EventsRouter.
```

### Comparing `edx-event-routing-backends-8.3.1/LICENSE.txt` & `edx-event-routing-backends-9.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/PKG-INFO` & `edx-event-routing-backends-9.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 8.3.1
+Version: 9.0.0
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -22,15 +22,15 @@
 Requires-Dist: Django
 Requires-Dist: apache-libcloud
 Requires-Dist: django-config-models
 Requires-Dist: django-fernet-fields-v2
 Requires-Dist: django-redis
 Requires-Dist: edx-celeryutils
 Requires-Dist: edx-toggles
-Requires-Dist: event-tracking
+Requires-Dist: event-tracking>=2.3.2
 Requires-Dist: fasteners
 Requires-Dist: isodate
 Requires-Dist: jsonfield
 Requires-Dist: openedx-filters
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: requests
@@ -136,14 +136,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[9.0.0]
+~~~~~~~
+
+* **BREAKING CHANGE**: Use a single entry point for all event routing backends.
+  which allows to easily switch bettwen celery and the event bus for the backends.
+
 [8.3.0]
 
 * Allow to use any configured engine to replay tracking logs
 
 [8.2.0]
 
 * Add support for batching for EventsRouter.
```

### Comparing `edx-event-routing-backends-8.3.1/README.rst` & `edx-event-routing-backends-9.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/PKG-INFO` & `edx-event-routing-backends-9.0.0/edx_event_routing_backends.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 8.3.1
+Version: 9.0.0
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -22,15 +22,15 @@
 Requires-Dist: Django
 Requires-Dist: apache-libcloud
 Requires-Dist: django-config-models
 Requires-Dist: django-fernet-fields-v2
 Requires-Dist: django-redis
 Requires-Dist: edx-celeryutils
 Requires-Dist: edx-toggles
-Requires-Dist: event-tracking
+Requires-Dist: event-tracking>=2.3.2
 Requires-Dist: fasteners
 Requires-Dist: isodate
 Requires-Dist: jsonfield
 Requires-Dist: openedx-filters
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: requests
@@ -136,14 +136,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[9.0.0]
+~~~~~~~
+
+* **BREAKING CHANGE**: Use a single entry point for all event routing backends.
+  which allows to easily switch bettwen celery and the event bus for the backends.
+
 [8.3.0]
 
 * Allow to use any configured engine to replay tracking logs
 
 [8.2.0]
 
 * Add support for batching for EventsRouter.
```

### Comparing `edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/SOURCES.txt` & `edx-event-routing-backends-9.0.0/edx_event_routing_backends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/admin.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/admin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/apps.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/apps.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/backends/async_events_router.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/backends/async_events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/backends/events_router.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/backends/events_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,16 @@
                     )
 
     def queue_event(self, redis, event):
         """
         Queue the event to be sent to configured routers.
 
         """
-        event["timestamp"] = event["timestamp"].isoformat()
+        if isinstance(event["timestamp"], datetime):
+            event["timestamp"] = event["timestamp"].isoformat()
         queue_size = redis.lpush(self.queue_name, json.dumps(event, cls=DateTimeJSONEncoder))
         logger.info(f'Event {event["name"]} has been queued for batching. Queue size: {queue_size}')
 
         if queue_size >= settings.EVENT_ROUTING_BACKEND_BATCH_SIZE or self.time_to_send(redis):
             batch = redis.rpop(self.queue_name, queue_size)
 
             orig_size = len(batch)
```

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/backends/sync_events_router.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/backends/sync_events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/backends/tests/test_events_router.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/backends/tests/test_events_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,22 +271,25 @@
         router = EventsRouter(processors=[], backend_name='test')
         redis_mock = MagicMock()
         mock_get_redis_connection.return_value = redis_mock
         redis_mock.lpush.return_value = None
         event1 = copy(self.transformed_event)
         event1["timestamp"] = datetime.datetime.now()
         event2 = copy(self.transformed_event)
-        event2["timestamp"] = datetime.datetime.now()
+        event2_emission = datetime.datetime.now()
+        event2["timestamp"] = event2_emission
         events = [event1, event2]
         formatted_events = []
         for event in events:
             formatted_event = copy(event)
-            formatted_event["timestamp"] = formatted_event["timestamp"].isoformat()
+            formatted_event["timestamp"] = event["timestamp"].isoformat()
             formatted_events.append(json.dumps(formatted_event).encode('utf-8'))
 
+        event2["timestamp"] = event2_emission.isoformat()
+
         redis_mock.rpop.return_value = formatted_events
         redis_mock.lpush.return_value = 1
         redis_mock.get.return_value.decode.return_value = datetime.datetime.now().isoformat()
 
         router.send(event1)
         redis_mock.lpush.return_value = 2
         router.send(event2)
```

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/helpers.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/helpers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/helpers/event_log_parser.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/helpers/event_log_parser.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/helpers/queued_sender.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/helpers/queued_sender.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,16 @@
         # Bookkeeping
         self.queued_lines = 0
         self.skipped_lines = 0
         self.unparsable_lines = 0
         self.batches_sent = 0
 
         self.tracker = get_tracker()
-        self.engine = self.tracker.backends[self.transformer_type]
+        self.engine = self.tracker.backends["event_transformer"]
+        self.backend = self.engine.backends[self.transformer_type]
 
     def is_known_event(self, event):
         """
         Check whether any processor cares about this event.
         """
         if "name" in event:
             for processor in self.engine.processors:
@@ -94,16 +95,15 @@
         """
         Send to the LRS if we're configured for that, otherwise a no-op.
 
         Events are converted to the output xAPI / Caliper format in the router.
         """
         if self.destination == "LRS":
             print(f"Sending {len(self.event_queue)} events to LRS...")
-            for backend in self.engine.backends.values():
-                backend.bulk_send(self.event_queue)
+            self.backend.bulk_send(self.event_queue)
         else:
             print("Skipping send, we're storing with libcloud instead of an LRS.")
 
     def store(self):
         """
         Store to a libcloud destination if we're configured for that.
```

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/recover_failed_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/recover_failed_events.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 
 import logging
 from textwrap import dedent
 
 from django.conf import settings
 from django.core.management.base import BaseCommand
-from eventtracking.backends.event_bus import EventBusRoutingBackend
 from eventtracking.tracker import get_tracker
 
 from event_routing_backends.processors.transformer_utils.exceptions import EventNotDispatched
 
 logger = logging.getLogger(__name__)
 
 
@@ -22,15 +21,15 @@
     """
 
     help = dedent(__doc__).strip()
 
     def add_arguments(self, parser):
         parser.add_argument(
             "--transformer_type",
-            choices=["xapi", "caliper", "all"],
+            choices=["xapi", "caliper"],
             required=True,
             help="The type of transformed events to recover.",
         )
         parser.add_argument(
             "--batch_size",
             default=100,
             help="The number of events to recover at a time. Default is 100.",
@@ -42,51 +41,40 @@
         """
         logger.info("Recovering failed events")
         logger.warning("This command is intended for use in recovery situations only.")
         transformer_type = options["transformer_type"]
         batch_size = options["batch_size"]
         tracker = get_tracker()
 
-        engines = {
-            name: engine
-            for name, engine in tracker.backends.items()
-            if isinstance(engine, EventBusRoutingBackend)
-        }
-
-        if not engines:
-            logger.info("No compatible backend found.")
-            return
+        engine = tracker.backends["event_transformer"]
+        backend = engine.backends[transformer_type]
 
         # In the recovery process we are disabling batching to prevent
         # single event failures from blocking the recovery process.
         settings.EVENT_ROUTING_BACKEND_BATCHING_ENABLED = False
 
         success = 0
         malformed = 0
         failed = 0
-        for name, engine in engines.items():
-            if transformer_type not in ("all", name):
-                logger.info("Skipping backend: {}".format(name))
-                continue
-            for backend_name, backend in engine.backends.items():
-                while failed_events := backend.get_failed_events(batch_size):
-                    logger.info(
-                        "Recovering {} failed events for backend {}".format(
-                            len(failed_events), backend_name
-                        )
-                    )
-                    for event in failed_events:
-                        try:
-                            backend.send(event)
-                            success += 1
-                        except EventNotDispatched:
-                            logger.error("Malformed event: {}".format(event["name"]))
-                            malformed += 1
-                        except Exception as e:  # pylint: disable=broad-except
-                            # Backend can still be in a bad state, so we need to catch all exceptions
-                            logger.error("Failed to send event: {}".format(e))
-                            failed += 1
+
+        while failed_events := backend.get_failed_events(batch_size):
+            logger.info(
+                "Recovering {} failed events for backend {}".format(
+                    len(failed_events), transformer_type
+                )
+            )
+            for event in failed_events:
+                try:
+                    backend.send(event)
+                    success += 1
+                except EventNotDispatched:
+                    logger.error("Malformed event: {}".format(event["name"]))
+                    malformed += 1
+                except Exception as e:  # pylint: disable=broad-except
+                    # Backend can still be in a bad state, so we need to catch all exceptions
+                    logger.error("Failed to send event: {}".format(e))
+                    failed += 1
 
         logger.info("Recovery process completed.")
         logger.info("Recovered events  : {}".format(success))
         logger.info("Failed to recover : {}".format(failed))
         logger.info("Malformed events  : {} ".format(malformed))
```

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/tests/test_recover_failed_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/tests/test_recover_failed_events.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             return [{"name": "test"}]
         return []
 
 
 class TestRecoverFailedEvents(TestCase):
     @override_settings(
         EVENT_TRACKING_BACKENDS={
-            "event_bus": {
+            "event_transformer": {
                 "ENGINE": "eventtracking.backends.event_bus.EventBusRoutingBackend",
                 "OPTIONS": {
                     "backends": {"xapi": XAPI_PROCESSOR},
                 },
             },
         }
     )
@@ -57,24 +57,24 @@
     def test_send_tracking_log_to_backends(self, mock_get_tracker):
         """
         Test for send_tracking_log_to_backends
         """
         tracker = DjangoTracker()
         mock_get_tracker.return_value = tracker
         mock_backend = Mock()
-        tracker.backends["event_bus"].backends["xapi"] = mock_backend
+        tracker.backends["event_transformer"].backends["xapi"] = mock_backend
         mock_backend.get_failed_events = Mocker().custom_get_failed_events
 
-        call_command("recover_failed_events", transformer_type="all")
+        call_command("recover_failed_events", transformer_type="xapi")
 
         mock_backend.send.assert_called_once_with({"name": "test"})
 
     @override_settings(
         EVENT_TRACKING_BACKENDS={
-            "event_bus": {
+            "event_transformer": {
                 "ENGINE": "eventtracking.backends.event_bus.EventBusRoutingBackend",
                 "OPTIONS": {
                     "backends": {"xapi": XAPI_PROCESSOR},
                 },
             },
         }
     )
@@ -87,25 +87,25 @@
     ):
         """
         Test for send_tracking_log_to_backends
         """
         tracker = DjangoTracker()
         mock_get_tracker.return_value = tracker
         mock_backend = Mock()
-        tracker.backends["event_bus"].backends["xapi"] = mock_backend
+        tracker.backends["event_transformer"].backends["xapi"] = mock_backend
         mock_backend.get_failed_events = Mocker().custom_get_failed_events
         mock_backend.send.side_effect = Exception("Error")
 
-        call_command("recover_failed_events", transformer_type="all")
+        call_command("recover_failed_events", transformer_type="xapi")
 
         mock_logger.error.assert_called_once_with("Failed to send event: Error")
 
     @override_settings(
         EVENT_TRACKING_BACKENDS={
-            "event_bus": {
+            "event_transformer": {
                 "ENGINE": "eventtracking.backends.event_bus.EventBusRoutingBackend",
                 "OPTIONS": {
                     "backends": {"xapi": XAPI_PROCESSOR},
                 },
             },
         }
     )
@@ -118,25 +118,25 @@
     ):
         """
         Test for send_tracking_log_to_backends
         """
         tracker = DjangoTracker()
         mock_get_tracker.return_value = tracker
         mock_backend = Mock()
-        tracker.backends["event_bus"].backends["xapi"] = mock_backend
+        tracker.backends["event_transformer"].backends["xapi"] = mock_backend
         mock_backend.get_failed_events = Mocker().custom_get_failed_events
         mock_backend.send.side_effect = EventNotDispatched("Error")
 
-        call_command("recover_failed_events", transformer_type="all")
+        call_command("recover_failed_events", transformer_type="xapi")
 
         mock_logger.error.assert_called_once_with("Malformed event: {}".format("test"))
 
     @override_settings(
         EVENT_TRACKING_BACKENDS={
-            "event_bus": {
+            "event_transformer": {
                 "ENGINE": "eventtracking.backends.event_bus.EventBusRoutingBackend",
                 "OPTIONS": {
                     "backends": {"xapi": XAPI_PROCESSOR},
                 },
             },
             "xapi": {
                 "ENGINE": "eventtracking.backends.event_bus.EventBusRoutingBackend",
@@ -152,39 +152,13 @@
     def test_send_tracking_log_to_backends_no_failed_events(self, mock_get_tracker):
         """
         Test for send_tracking_log_to_backends
         """
         tracker = DjangoTracker()
         mock_get_tracker.return_value = tracker
         mock_backend = Mock()
-        tracker.backends["xapi"].backends["xapi"] = mock_backend
+        tracker.backends["event_transformer"].backends["xapi"] = mock_backend
         mock_backend.get_failed_events.return_value = []
 
         call_command("recover_failed_events", transformer_type="xapi")
 
         mock_backend.send.assert_not_called()
-
-    @override_settings(
-        EVENT_TRACKING_BACKENDS={
-            "event_bus": {
-                "ENGINE": "eventtracking.backends.logger.LoggerBackend",
-                "OPTIONS": {},
-            },
-        }
-    )
-    @patch(
-        "event_routing_backends.management.commands.recover_failed_events.get_tracker"
-    )
-    @patch("event_routing_backends.management.commands.recover_failed_events.logger")
-    def test_send_tracking_log_to_backends_no_engines(
-        self, mock_logger, mock_get_tracker
-    ):
-        """
-        Test for send_tracking_log_to_backends
-        """
-        tracker = DjangoTracker()
-        mock_get_tracker.return_value = tracker
-
-        call_command("recover_failed_events", transformer_type="all")
-
-        mock_logger.info.assert_any_call("Recovering failed events")
-        mock_logger.info.assert_any_call("No compatible backend found.")
```

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,16 +207,16 @@
     mock_libcloud_get_driver.return_value = mm
 
     mm2 = MagicMock()
     # Fake a router mapping so some events in the log are actually processed
     mm2.registry.mapping = {"problem_check": 1}
     # Fake a process response that can be serialized to json
     mm2.return_value = {"foo": "bar"}
-    tracker.backends["xapi"].processors = [mm2]
-    for backend in tracker.backends["xapi"].backends.values():
+    tracker.backends["event_transformer"].processors = [mm2]
+    for backend in tracker.backends["event_transformer"].backends.values():
         backend.bulk_send = MagicMock()
 
     call_command(
         'transform_tracking_logs',
         **command_opts
     )
```

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/transform_tracking_logs.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/management/commands/transform_tracking_logs.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0001_initial.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0002_auto_20210503_0648.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/migrations/0002_auto_20210503_0648.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0004_auto_20211025_1053.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/migrations/0004_auto_20211025_1053.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/models.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/__init__.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/envelope_processor.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/__init__.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/navigation_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/video_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/test_caliper.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/tests/test_caliper.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/test_envelope_processor.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/test_transformers.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/transformer.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/transformer_processor.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/caliper/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/mixins/base_transformer.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/mixins/base_transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/mixins/base_transformer_processor.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/mixins/base_transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/decorators.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/openedx_filters/decorators.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/filters.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/openedx_filters/filters.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/openedx_filters/test_filters.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/tests/openedx_filters/test_filters.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/transformers_test_mixin.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/tests/transformers_test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/registry.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/transformer_utils/registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/tests/test_registry.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/__init__.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/constants.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/constants.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/__init__.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/completion_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/completion_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/exam_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/exam_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/forum_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/forum_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/grading_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/grading_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/navigation_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/video_events.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/test_transformers.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/test_xapi.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/test_xapi_event_transformers.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/tests/test_xapi_event_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/transformer.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/transformer_processor.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/processors/xapi/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/settings/common.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/settings/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,64 +169,65 @@
         'seek_video',
         'edx.video.position.changed',
         'edx.course.grade.passed.first_time',
         'edx.course.grade.now_passed',
         'edx.course.grade.now_failed'
     ]
 
-    settings.EVENT_BUS_TRACKING_LOGS = set(allowed_xapi_events + allowed_caliper_events)
+    allowed_events = set(allowed_xapi_events + allowed_caliper_events)
+
+    # Operators can configure the event bus allowed events via EVENT_BUS_TRACKING_LOGS and by default
+    # we are allowing the supported events by xAPI and Caliper so that operators don't need to configure
+    # the events manually.
+    settings.EVENT_BUS_TRACKING_LOGS = allowed_events
 
     settings.EVENT_TRACKING_BACKENDS.update({
-        'xapi': {
+        'event_transformer': {
             'ENGINE': 'eventtracking.backends.async_routing.AsyncRoutingBackend',
             'OPTIONS': {
-                'backend_name': 'xapi',
+                'backend_name': 'events',
                 'processors': [
                     {
                         'ENGINE': 'eventtracking.processors.whitelist.NameWhitelistProcessor',
                         'OPTIONS': {
-                                'whitelist': allowed_xapi_events
+                            'whitelist': allowed_events
                         }
                     },
                 ],
                 'backends': {
                     'xapi': {
                         'ENGINE': 'event_routing_backends.backends.async_events_router.AsyncEventsRouter',
                         'OPTIONS': {
                             'processors': [
                                 {
+                                    'ENGINE': 'eventtracking.processors.whitelist.NameWhitelistProcessor',
+                                    'OPTIONS': {
+                                        'whitelist': allowed_xapi_events
+                                    }
+                                },
+                                {
                                     'ENGINE':
                                         'event_routing_backends.processors.xapi.transformer_processor.XApiProcessor',
                                     'OPTIONS': {}
                                 }
                             ],
                             'backend_name': 'xapi',
                         }
-                    }
-                },
-            },
-        },
-        "caliper": {
-            "ENGINE": "eventtracking.backends.async_routing.AsyncRoutingBackend",
-            "OPTIONS": {
-                "backend_name": "caliper",
-                "processors": [
-                    {
-                        "ENGINE": "eventtracking.processors.whitelist.NameWhitelistProcessor",
-                        "OPTIONS": {
-                            "whitelist": allowed_caliper_events
-                        }
-                    }
-                ],
-                "backends": {
+                    },
                     "caliper": {
                         'ENGINE': 'event_routing_backends.backends.async_events_router.AsyncEventsRouter',
                         "OPTIONS": {
                             "processors": [
                                 {
+                                    "ENGINE": "eventtracking.processors.whitelist.NameWhitelistProcessor",
+                                    "OPTIONS": {
+                                        "whitelist": allowed_caliper_events
+                                    }
+                                },
+                                {
                                     "ENGINE":
                                         "event_routing_backends.processors."
                                         "caliper.transformer_processor.CaliperProcessor",
                                     "OPTIONS": {}
                                 },
                                 {
                                     "ENGINE":
@@ -236,11 +237,11 @@
                                         "sensor_id": settings.LMS_ROOT_URL
                                     }
                                 }
                             ],
                             "backend_name": "caliper"
                         }
                     }
-                }
-            }
-        }
+                },
+            },
+        },
     })
```

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/settings/production.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/settings/production.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js` & `edx-event-routing-backends-9.0.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/tasks.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/tests/factories.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_helpers.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_mixin.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_models.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_settings.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/tests/test_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,31 @@
     """
 
     def test_common_settings(self):
         """
         Test common settings
         """
         common_settings.plugin_settings(settings)
-        self.assertIn('xapi', settings.EVENT_TRACKING_BACKENDS)
-        self.assertIn('caliper', settings.EVENT_TRACKING_BACKENDS)
+        self.assertIn('event_transformer', settings.EVENT_TRACKING_BACKENDS)
+        self.assertIn('xapi', settings.EVENT_TRACKING_BACKENDS["event_transformer"]["OPTIONS"]["backends"])
+        self.assertIn('caliper', settings.EVENT_TRACKING_BACKENDS["event_transformer"]["OPTIONS"]["backends"])
         self.assertIn('edx.course.enrollment.activated', settings.EVENT_TRACKING_BACKENDS_BUSINESS_CRITICAL_EVENTS)
         self.assertFalse(settings.CALIPER_EVENTS_ENABLED)
         self.assertFalse(settings.CALIPER_EVENT_LOGGING_ENABLED)
         self.assertTrue(settings.XAPI_EVENTS_ENABLED)
         self.assertTrue(settings.XAPI_EVENT_LOGGING_ENABLED)
 
     def test_devstack_settings(self):
         """
         Test devstack settings
         """
         devstack_settings.plugin_settings(settings)
-        self.assertIn('xapi', settings.EVENT_TRACKING_BACKENDS)
-        self.assertIn('caliper', settings.EVENT_TRACKING_BACKENDS)
+        self.assertIn('event_transformer', settings.EVENT_TRACKING_BACKENDS)
+        self.assertIn('xapi', settings.EVENT_TRACKING_BACKENDS["event_transformer"]["OPTIONS"]["backends"])
+        self.assertIn('caliper', settings.EVENT_TRACKING_BACKENDS["event_transformer"]["OPTIONS"]["backends"])
         self.assertIn('edx.course.enrollment.deactivated', settings.EVENT_TRACKING_BACKENDS_BUSINESS_CRITICAL_EVENTS)
         self.assertFalse(settings.CALIPER_EVENTS_ENABLED)
         self.assertFalse(settings.CALIPER_EVENT_LOGGING_ENABLED)
         self.assertTrue(settings.XAPI_EVENTS_ENABLED)
         self.assertTrue(settings.XAPI_EVENT_LOGGING_ENABLED)
 
     def test_production_settings(self):
```

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/utils/http_client.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/event_routing_backends/utils/xapi_lrs_client.py` & `edx-event-routing-backends-9.0.0/event_routing_backends/utils/xapi_lrs_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.1/requirements/constraints.txt` & `edx-event-routing-backends-9.0.0/requirements/constraints.txt`

 * *Files 7% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 
 # greater version failing docs build
 sphinx==4.2.0
 # Sphinx requires docutils<0.18 && doc8<1.0.0
 # This pin can be removed once sphinx constraint is removed.
 docutils<0.18
 doc8<1.0.0
+event-tracking>=2.3.2
```

### Comparing `edx-event-routing-backends-8.3.1/setup.py` & `edx-event-routing-backends-9.0.0/setup.py`

 * *Files identical despite different names*

