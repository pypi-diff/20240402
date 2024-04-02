# Comparing `tmp/event-tracking-2.3.1.tar.gz` & `tmp/event-tracking-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event-tracking-2.3.1.tar", last modified: Fri Mar 22 15:15:57 2024, max compression
+gzip compressed data, was "event-tracking-2.3.2.tar", last modified: Tue Apr  2 19:15:56 2024, max compression
```

## Comparing `event-tracking-2.3.1.tar` & `event-tracking-2.3.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:57.475124 event-tracking-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-22 15:15:53.000000 event-tracking-2.3.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-03-22 15:15:53.000000 event-tracking-2.3.1/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-22 15:15:53.000000 event-tracking-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-03-22 15:15:57.475124 event-tracking-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-03-22 15:15:53.000000 event-tracking-2.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:57.475124 event-tracking-2.3.1/event_tracking.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-03-22 15:15:57.000000 event-tracking-2.3.1/event_tracking.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-22 15:15:57.000000 event-tracking-2.3.1/event_tracking.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 15:15:57.000000 event-tracking-2.3.1/event_tracking.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-22 15:15:57.000000 event-tracking-2.3.1/event_tracking.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-22 15:15:57.000000 event-tracking-2.3.1/event_tracking.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:57.471124 event-tracking-2.3.1/eventtracking/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:57.471124 event-tracking-2.3.1/eventtracking/backends/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/async_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:57.471124 event-tracking-2.3.1/eventtracking/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/tests/test_async_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/tests/test_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/tests/test_logger_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/tests/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/tests/test_mongodb_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/tests/test_mongodb_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/backends/tests/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:57.475124 event-tracking-2.3.1/eventtracking/django/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/django/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/django/django_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:57.475124 event-tracking-2.3.1/eventtracking/django/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/django/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/django/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/django/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/locator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:57.475124 event-tracking-2.3.1/eventtracking/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/processors/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/processors/regex_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:57.475124 event-tracking-2.3.1/eventtracking/processors/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/processors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/processors/tests/test_regex_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/processors/tests/test_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/processors/whitelist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:57.475124 event-tracking-2.3.1/eventtracking/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/tests/test_locator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/tests/test_track.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-03-22 15:15:53.000000 event-tracking-2.3.1/eventtracking/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:15:57.475124 event-tracking-2.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-22 15:15:53.000000 event-tracking-2.3.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-22 15:15:57.475124 event-tracking-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-03-22 15:15:53.000000 event-tracking-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:56.211442 event-tracking-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 19:15:48.000000 event-tracking-2.3.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-04-02 19:15:48.000000 event-tracking-2.3.2/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 19:15:48.000000 event-tracking-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-04-02 19:15:56.211442 event-tracking-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-02 19:15:48.000000 event-tracking-2.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:56.211442 event-tracking-2.3.2/event_tracking.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-04-02 19:15:56.000000 event-tracking-2.3.2/event_tracking.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-02 19:15:56.000000 event-tracking-2.3.2/event_tracking.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:15:56.000000 event-tracking-2.3.2/event_tracking.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 19:15:56.000000 event-tracking-2.3.2/event_tracking.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 19:15:56.000000 event-tracking-2.3.2/event_tracking.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:56.207442 event-tracking-2.3.2/eventtracking/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:56.207442 event-tracking-2.3.2/eventtracking/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/async_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:56.207442 event-tracking-2.3.2/eventtracking/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/tests/test_async_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/tests/test_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/tests/test_logger_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/tests/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/tests/test_mongodb_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/tests/test_mongodb_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/backends/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:56.211442 event-tracking-2.3.2/eventtracking/django/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/django/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/django/django_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:56.211442 event-tracking-2.3.2/eventtracking/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/django/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/django/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/django/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/locator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:56.211442 event-tracking-2.3.2/eventtracking/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/processors/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/processors/regex_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:56.211442 event-tracking-2.3.2/eventtracking/processors/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/processors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/processors/tests/test_regex_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/processors/tests/test_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/processors/whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:56.211442 event-tracking-2.3.2/eventtracking/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/tests/test_track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-02 19:15:48.000000 event-tracking-2.3.2/eventtracking/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:56.211442 event-tracking-2.3.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 19:15:48.000000 event-tracking-2.3.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-02 19:15:56.211442 event-tracking-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-02 19:15:48.000000 event-tracking-2.3.2/setup.py
```

### Comparing `event-tracking-2.3.1/LICENSE.TXT` & `event-tracking-2.3.2/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/PKG-INFO` & `event-tracking-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-tracking
-Version: 2.3.1
+Version: 2.3.2
 Summary: A simple event tracking system.
 Home-page: https://github.com/openedx/event-tracking
 Author: edX
 Author-email: oscm@edx.org
 License: AGPLv3 License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
@@ -17,22 +17,22 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 License-File: LICENSE.TXT
 License-File: AUTHORS
+Requires-Dist: celery
 Requires-Dist: pymongo<4.0.0,>=2.7.2
-Requires-Dist: openedx-events>=9.5.1
-Requires-Dist: edx-django-utils
-Requires-Dist: edx-toggles
 Requires-Dist: pytz
-Requires-Dist: celery
+Requires-Dist: edx-django-utils
 Requires-Dist: six
 Requires-Dist: django
+Requires-Dist: edx-toggles
+Requires-Dist: openedx-events>=9.5.1
 
 Part of `edX code`__.
 
 __ http://code.edx.org/
 
 Event Tracking library |build-status|
 =====================================
```

### Comparing `event-tracking-2.3.1/README.rst` & `event-tracking-2.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/event_tracking.egg-info/PKG-INFO` & `event-tracking-2.3.2/event_tracking.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-tracking
-Version: 2.3.1
+Version: 2.3.2
 Summary: A simple event tracking system.
 Home-page: https://github.com/openedx/event-tracking
 Author: edX
 Author-email: oscm@edx.org
 License: AGPLv3 License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
@@ -17,22 +17,22 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 License-File: LICENSE.TXT
 License-File: AUTHORS
+Requires-Dist: celery
 Requires-Dist: pymongo<4.0.0,>=2.7.2
-Requires-Dist: openedx-events>=9.5.1
-Requires-Dist: edx-django-utils
-Requires-Dist: edx-toggles
 Requires-Dist: pytz
-Requires-Dist: celery
+Requires-Dist: edx-django-utils
 Requires-Dist: six
 Requires-Dist: django
+Requires-Dist: edx-toggles
+Requires-Dist: openedx-events>=9.5.1
 
 Part of `edX code`__.
 
 __ http://code.edx.org/
 
 Event Tracking library |build-status|
 =====================================
```

### Comparing `event-tracking-2.3.1/event_tracking.egg-info/SOURCES.txt` & `event-tracking-2.3.2/event_tracking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/async_routing.py` & `event-tracking-2.3.2/eventtracking/backends/async_routing.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/event_bus.py` & `event-tracking-2.3.2/eventtracking/backends/event_bus.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/logger.py` & `event-tracking-2.3.2/eventtracking/backends/logger.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/mongodb.py` & `event-tracking-2.3.2/eventtracking/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/routing.py` & `event-tracking-2.3.2/eventtracking/backends/routing.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/segment.py` & `event-tracking-2.3.2/eventtracking/backends/segment.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/tests/__init__.py` & `event-tracking-2.3.2/eventtracking/backends/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/tests/test_async_routing.py` & `event-tracking-2.3.2/eventtracking/backends/tests/test_async_routing.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/tests/test_event_bus.py` & `event-tracking-2.3.2/eventtracking/backends/tests/test_event_bus.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/tests/test_logger.py` & `event-tracking-2.3.2/eventtracking/backends/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/tests/test_logger_integration.py` & `event-tracking-2.3.2/eventtracking/backends/tests/test_logger_integration.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/tests/test_mongodb.py` & `event-tracking-2.3.2/eventtracking/backends/tests/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/tests/test_mongodb_integration.py` & `event-tracking-2.3.2/eventtracking/backends/tests/test_mongodb_integration.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/tests/test_mongodb_performance.py` & `event-tracking-2.3.2/eventtracking/backends/tests/test_mongodb_performance.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/tests/test_routing.py` & `event-tracking-2.3.2/eventtracking/backends/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/backends/tests/test_segment.py` & `event-tracking-2.3.2/eventtracking/backends/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/config.py` & `event-tracking-2.3.2/eventtracking/config.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/django/apps.py` & `event-tracking-2.3.2/eventtracking/django/apps.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/django/django_tracker.py` & `event-tracking-2.3.2/eventtracking/django/django_tracker.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/django/tests/test_configuration.py` & `event-tracking-2.3.2/eventtracking/django/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/handlers.py` & `event-tracking-2.3.2/eventtracking/handlers.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/locator.py` & `event-tracking-2.3.2/eventtracking/locator.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/processors/exceptions.py` & `event-tracking-2.3.2/eventtracking/processors/exceptions.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/processors/regex_filter.py` & `event-tracking-2.3.2/eventtracking/processors/regex_filter.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/processors/tests/test_regex_filter.py` & `event-tracking-2.3.2/eventtracking/processors/tests/test_regex_filter.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/processors/tests/test_whitelist.py` & `event-tracking-2.3.2/eventtracking/processors/tests/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/processors/whitelist.py` & `event-tracking-2.3.2/eventtracking/processors/whitelist.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,11 +21,18 @@
         except TypeError as error:
             raise TypeError(
                 'The NameWhitelistProcessor must be passed a collection of allowed names '
                 'using the "whitelist" parameter'
             ) from error
 
     def __call__(self, event):
-        if event['name'] not in self.whitelist:
+        """
+        Filter out events whose names aren't on the whitelist.
+
+        The event can be a single event or a list of events (when using event-routing-backends with batching enabled).
+        """
+        if isinstance(event, list):
+            return [e for e in event if e['name'] in self.whitelist]
+        elif event['name'] not in self.whitelist:
             raise EventEmissionExit()
 
         return event
```

### Comparing `event-tracking-2.3.1/eventtracking/tasks.py` & `event-tracking-2.3.2/eventtracking/tasks.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/tests/test_handlers.py` & `event-tracking-2.3.2/eventtracking/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/tests/test_locator.py` & `event-tracking-2.3.2/eventtracking/tests/test_locator.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/tests/test_tasks.py` & `event-tracking-2.3.2/eventtracking/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/tests/test_track.py` & `event-tracking-2.3.2/eventtracking/tests/test_track.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/eventtracking/tracker.py` & `event-tracking-2.3.2/eventtracking/tracker.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.3.1/setup.py` & `event-tracking-2.3.2/setup.py`

 * *Files identical despite different names*

