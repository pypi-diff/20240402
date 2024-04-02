# Comparing `tmp/edri-2024.3.9.tar.gz` & `tmp/edri-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edri-2024.3.9.tar", last modified: Mon Mar 11 08:55:03 2024, max compression
+gzip compressed data, was "edri-2024.4.1.tar", last modified: Tue Apr  2 09:52:49 2024, max compression
```

## Comparing `edri-2024.3.9.tar` & `edri-2024.4.1.tar`

### file list

```diff
@@ -1,140 +1,139 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.204261 edri-2024.3.9/
--rw-r--r--   0 root         (0) root         (0)     1649 2024-03-11 08:55:03.204261 edri-2024.3.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11895 2024-03-07 10:37:30.000000 edri-2024.3.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.196261 edri-2024.3.9/edri/
--rw-rw-rw-   0 root         (0) root         (0)     2195 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.196261 edri-2024.3.9/edri/abstract/
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/abstract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4429 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/abstract/api_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.196261 edri-2024.3.9/edri/abstract/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/abstract/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    31977 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/abstract/manager/manager_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7635 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/abstract/manager/manager_priority_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.196261 edri-2024.3.9/edri/abstract/worker/
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/abstract/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9270 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/abstract/worker/worker.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/abstract/worker/worker_process.py
--rw-rw-rw-   0 root         (0) root         (0)     2122 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/abstract/worker/worker_thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.196261 edri-2024.3.9/edri/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/config/constant.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/config/logging.py
--rw-rw-rw-   0 root         (0) root         (0)      582 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/config/setting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.196261 edri-2024.3.9/edri/dataclass/
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/dataclass/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.196261 edri-2024.3.9/edri/dataclass/client/
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/dataclass/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/dataclass/client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.196261 edri-2024.3.9/edri/dataclass/event/
--rw-rw-rw-   0 root         (0) root         (0)     6593 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/dataclass/event/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/dataclass/event/event.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/dataclass/event/response.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/dataclass/queue_item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.196261 edri-2024.3.9/edri/dataclass/switch/
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/dataclass/switch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/dataclass/switch/connection.py
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/dataclass/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.196261 edri-2024.3.9/edri/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/events/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.196261 edri-2024.3.9/edri/events/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/events/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.196261 edri-2024.3.9/edri/events/api/client/
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/events/api/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/api/client/register.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/api/client/unregister.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.196261 edri-2024.3.9/edri/events/api/group/
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/events/api/group/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/api/group/client.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/api/group/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.200261 edri-2024.3.9/edri/events/api/manage/
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/events/api/manage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/api/manage/list_registered.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/api/manage/register.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/api/manage/unregister.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/api/manage/unregister_all.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.200261 edri-2024.3.9/edri/events/edri/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/events/edri/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.200261 edri-2024.3.9/edri/events/edri/group/
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/events/edri/group/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/group/manager.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/group/router.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/group/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/group/store.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/group/switch.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/group/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.200261 edri-2024.3.9/edri/events/edri/manager/
--rw-rw-rw-   0 root         (0) root         (0)      231 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/events/edri/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/manager/stream_close.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/manager/stream_create.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/manager/stream_message.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/manager/worker_quit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.200261 edri-2024.3.9/edri/events/edri/router/
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/events/edri/router/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/router/demands.py
--rw-rw-rw-   0 root         (0) root         (0)      234 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/router/health_check.py
--rw-rw-rw-   0 root         (0) root         (0)      125 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/router/last_events.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/router/send_from.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/events/edri/router/subscribe.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/router/subscribe_connector.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/router/subscribed_all.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/router/subscribed_new.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/router/unsubscribe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.200261 edri-2024.3.9/edri/events/edri/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/events/edri/scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/scheduler/cancel.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/events/edri/scheduler/set.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/scheduler/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.200261 edri-2024.3.9/edri/events/edri/store/
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/events/edri/store/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/store/delete.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/store/get.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/store/set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.200261 edri-2024.3.9/edri/events/edri/switch/
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/events/edri/switch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/switch/demands.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/switch/last_messages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.200261 edri-2024.3.9/edri/events/edri/test/
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/events/edri/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/test/ping.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/events/edri/test/ping2.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/events/edri/test/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.200261 edri-2024.3.9/edri/rest/
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/rest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25641 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/rest/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.200261 edri-2024.3.9/edri/router/
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/router/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5965 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/router/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6557 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/router/health_checker.py
--rw-rw-rw-   0 root         (0) root         (0)    11733 2024-03-08 11:06:35.000000 edri-2024.3.9/edri/router/router.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2024-03-08 11:06:35.000000 edri-2024.3.9/edri/store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.204261 edri-2024.3.9/edri/switch/
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/switch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1688 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/switch/forwarder.py
--rw-rw-rw-   0 root         (0) root         (0)     3269 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/switch/receiver.py
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/switch/sender.py
--rw-rw-rw-   0 root         (0) root         (0)     2714 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/switch/switch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.204261 edri-2024.3.9/edri/utility/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/utility/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13893 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/utility/api_broker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.204261 edri-2024.3.9/edri/utility/connector/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/utility/connector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10119 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/utility/connector/connector.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/utility/connector/socket.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2024-02-21 08:23:35.000000 edri-2024.3.9/edri/utility/eta.py
--rw-rw-rw-   0 root         (0) root         (0)     2182 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/utility/function.py
--rw-rw-rw-   0 root         (0) root         (0)     8454 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/utility/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     2247 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/utility/storage.py
--rw-rw-rw-   0 root         (0) root         (0)     3091 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/utility/store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.204261 edri-2024.3.9/edri/websocket/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-07 10:37:30.000000 edri-2024.3.9/edri/websocket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7001 2024-03-11 08:54:49.000000 edri-2024.3.9/edri/websocket/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.204261 edri-2024.3.9/edri.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1649 2024-03-11 08:55:03.000000 edri-2024.3.9/edri.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3326 2024-03-11 08:55:03.000000 edri-2024.3.9/edri.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 08:55:03.000000 edri-2024.3.9/edri.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2024-03-11 08:55:03.000000 edri-2024.3.9/edri.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-11 08:55:03.000000 edri-2024.3.9/edri.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-11 08:55:03.204261 edri-2024.3.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1841 2024-03-11 08:54:41.000000 edri-2024.3.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:55:03.204261 edri-2024.3.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-03-07 10:37:30.000000 edri-2024.3.9/tests/test_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.320612 edri-2024.4.1/
+-rw-r--r--   0 root         (0) root         (0)     1649 2024-04-02 09:52:49.320612 edri-2024.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11895 2024-03-07 10:37:30.000000 edri-2024.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.096617 edri-2024.4.1/edri/
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2024-03-13 10:35:39.000000 edri-2024.4.1/edri/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.108616 edri-2024.4.1/edri/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/abstract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4429 2024-03-13 10:35:39.000000 edri-2024.4.1/edri/abstract/api_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.136616 edri-2024.4.1/edri/abstract/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/abstract/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32374 2024-03-13 10:35:39.000000 edri-2024.4.1/edri/abstract/manager/manager_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7635 2024-03-13 10:35:39.000000 edri-2024.4.1/edri/abstract/manager/manager_priority_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.140616 edri-2024.4.1/edri/abstract/worker/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/abstract/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9319 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/abstract/worker/worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/abstract/worker/worker_process.py
+-rw-rw-rw-   0 root         (0) root         (0)     2122 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/abstract/worker/worker_thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.144616 edri-2024.4.1/edri/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-03-13 10:35:39.000000 edri-2024.4.1/edri/config/constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2024-03-13 12:02:40.000000 edri-2024.4.1/edri/config/setting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.152615 edri-2024.4.1/edri/dataclass/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/dataclass/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.156615 edri-2024.4.1/edri/dataclass/client/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/dataclass/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/dataclass/client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.164615 edri-2024.4.1/edri/dataclass/event/
+-rw-rw-rw-   0 root         (0) root         (0)     6593 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/dataclass/event/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/dataclass/event/event.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/dataclass/event/response.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/dataclass/queue_item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.168615 edri-2024.4.1/edri/dataclass/switch/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/dataclass/switch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/dataclass/switch/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/dataclass/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.168615 edri-2024.4.1/edri/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/events/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.168615 edri-2024.4.1/edri/events/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/events/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.176615 edri-2024.4.1/edri/events/api/client/
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/api/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/client/register.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/client/unregister.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.184615 edri-2024.4.1/edri/events/api/group/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/api/group/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/group/client.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/group/manage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.192615 edri-2024.4.1/edri/events/api/manage/
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/api/manage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/manage/list_registered.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/manage/register.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/manage/unregister.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/manage/unregister_all.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.192615 edri-2024.4.1/edri/events/edri/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/events/edri/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.204614 edri-2024.4.1/edri/events/edri/group/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/group/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/group/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/group/router.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/group/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/group/store.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/group/switch.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/group/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.212614 edri-2024.4.1/edri/events/edri/manager/
+-rw-rw-rw-   0 root         (0) root         (0)      231 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/manager/stream_close.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/manager/stream_create.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/manager/stream_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/manager/worker_quit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.228614 edri-2024.4.1/edri/events/edri/router/
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/router/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/demands.py
+-rw-rw-rw-   0 root         (0) root         (0)      234 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/health_check.py
+-rw-rw-rw-   0 root         (0) root         (0)      125 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/last_events.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/send_from.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/router/subscribe.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/subscribe_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/subscribed_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/subscribed_new.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/unsubscribe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.240614 edri-2024.4.1/edri/events/edri/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/scheduler/cancel.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/scheduler/set.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/scheduler/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.240614 edri-2024.4.1/edri/events/edri/store/
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/store/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/store/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/store/get.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/store/set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.248613 edri-2024.4.1/edri/events/edri/switch/
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/switch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/switch/demands.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/switch/last_messages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.252613 edri-2024.4.1/edri/events/edri/test/
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/test/ping.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/test/ping2.py
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/test/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.256613 edri-2024.4.1/edri/rest/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/rest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25647 2024-03-13 10:35:39.000000 edri-2024.4.1/edri/rest/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.264613 edri-2024.4.1/edri/router/
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/router/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5965 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/router/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6557 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/router/health_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11733 2024-03-08 11:06:35.000000 edri-2024.4.1/edri/router/router.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2024-03-08 11:06:35.000000 edri-2024.4.1/edri/store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.288612 edri-2024.4.1/edri/switch/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/switch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/switch/forwarder.py
+-rw-rw-rw-   0 root         (0) root         (0)     3269 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/switch/receiver.py
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/switch/sender.py
+-rw-rw-rw-   0 root         (0) root         (0)     2714 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/switch/switch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.304612 edri-2024.4.1/edri/utility/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/utility/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13893 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/utility/api_broker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.312612 edri-2024.4.1/edri/utility/connector/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/utility/connector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10119 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/utility/connector/connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/utility/connector/socket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/utility/eta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/utility/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     8454 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/utility/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2247 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/utility/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3091 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/utility/store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.316612 edri-2024.4.1/edri/websocket/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/websocket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7001 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/websocket/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.320612 edri-2024.4.1/edri.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1649 2024-04-02 09:52:49.000000 edri-2024.4.1/edri.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-04-02 09:52:49.000000 edri-2024.4.1/edri.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 09:52:49.000000 edri-2024.4.1/edri.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2024-04-02 09:52:49.000000 edri-2024.4.1/edri.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-02 09:52:49.000000 edri-2024.4.1/edri.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 09:52:49.320612 edri-2024.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2024-04-02 09:52:26.000000 edri-2024.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.320612 edri-2024.4.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-03-07 10:37:30.000000 edri-2024.4.1/tests/test_storage.py
```

### Comparing `edri-2024.3.9/PKG-INFO` & `edri-2024.4.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edri
-Version: 2024.3.9
+Version: 2024.4.1
 Summary: Event Driven Routing Infrastructure
 Author: Marek Olšan
 Author-email: marek.olsan@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `edri-2024.3.9/README.md` & `edri-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/__init__.py` & `edri-2024.4.1/edri/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from multiprocessing import Queue
 
 from edri.abstract import ManagerBase
 from edri.utility.connector import Connector
 from edri.utility.scheduler import Scheduler, Job
-from edri.config.setting import DEFAULT_TOKEN_LENGTH
+from edri.config.setting import TOKEN_LENGTH
 from edri.dataclass.event import Event
 from edri.router import Router
 from edri.rest import REST
 from edri.utility.store import Store
 from edri.utility.api_broker import ApiBroker
 from edri.websocket import API as WebSocket
```

### Comparing `edri-2024.3.9/edri/abstract/api_base.py` & `edri-2024.4.1/edri/abstract/api_base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         API component and its clients.
         logger (Logger): A logging.Logger instance for logging messages. The logger
         is named after the API.
 
     Methods:
         __init__(ab_queue: "Queue[Event]"): Constructor for APIBase.
         name: Abstract property. Must be implemented to return the name of the API.
-        type: Abstract property. Must be implemented to return the type of the API.
         register(): Attempts to register a client and returns a connection and key.
+        type: Abstract property. Must be implemented to return the type of the API.
         unregister(client_pipe: Pipe, key: str): Unregisters a client based on the key.
 
     Abstract Methods:
         name: Should return the name of the API, mainly used for logging purposes.
         type: Should return the specific ApiType of the API.
 
     Usage:
@@ -56,26 +56,14 @@
         primarily for logging purposes.
 
         Returns:
             str: The name of the API.
         """
         pass
 
-    @property
-    @abstractmethod
-    def type(self) -> ApiType:
-        """
-        Abstract property that should return the type of the API, as defined by the
-        ApiType enum. This type is used to identify the API's functionality.
-
-        Returns:
-            ApiType: The type of the API.
-        """
-        pass
-
     def register(self) -> Tuple[Connection, str] | None:
         """
         Attempts to register a new client with the API. This involves sending a
         registration request through the queue and waiting for a response.
 
         Returns:
             Tuple[Connection, str] | None: A tuple containing the client connection
@@ -97,14 +85,26 @@
             self.logger.critical("Key is missing, client registration failed!")
             client_pipe.close()
             return None
         client_ab_pipe.close()
         self.logger.debug("Client was registered %s", message._key)
         return client_pipe, message._key
 
+    @property
+    @abstractmethod
+    def type(self) -> ApiType:
+        """
+        Abstract property that should return the type of the API, as defined by the
+        ApiType enum. This type is used to identify the API's functionality.
+
+        Returns:
+            ApiType: The type of the API.
+        """
+        pass
+
     def unregister(self, client_pipe: Connection, key: str) -> None:
         """
         Unregisters a client based on the provided key and closes their communication pipe.
 
         Parameters:
             client_pipe (Connection): The communication pipe for the client.
             key (str): The registration key of the client to be unregistered.
```

### Comparing `edri-2024.3.9/edri/abstract/manager/manager_base.py` & `edri-2024.4.1/edri/abstract/manager/manager_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,39 +43,39 @@
         Inherits from `ABC` to be an abstract base class and `Process` for multiprocessing support.
 
         Attributes:
             router_queue (Optional["Queue[Event]"]): The queue for communicating with the router.
             logger (Optional[Logger]): Logger instance for logging messages.
             from_time (Optional[datetime]): Start time for filtering events.
 
-
         Methods:
             __init__: Constructor for initializing the manager.
+            _find_worker: Finds a worker based on its communication pipe.
+            _find_stream: Finds a worker associated with a specific stream.
+            _prepare: Prepares the manager before starting the event resolver loop.
+            _prepare_resolvers: Prepares methods for resolving request and response events.
+            _remove_worker: Removes a worker from the manager's tracking.
+            _resolve_undelivered_events: Resolves any undelivered events.
+            _subscribe: Subscribes to events based on requests and responses.
+            _subscribe_static_resolvers: Subscribes to static event resolvers.
             additional_pipes: Property for specifying additional pipes.
             name: Property for specifying the manager's name.
             workers: Property for defining workers and their associated messages.
-            _subscribe: Subscribes to events based on requests and responses.
-            _resolve_undelivered_events: Resolves any undelivered events.
-            resolve_callback_worker: Default method for resolving events received from workers.
+            after_start: Hook for actions after the manager starts.
+            get_pipes: Gets a set of all pipes including the router and worker pipes.
+            health_check: Handles health check events from the router.
+            resolve: The central method for resolving events received by the manager.
             resolve_callback_pipe: Handles events received from unknown pipes.
+            resolve_callback_worker: Default method for resolving events received from workers.
             resolve_unknown: Handles unknown events received from the router pipe.
-            get_pipes: Gets a set of all pipes including the router and worker pipes.
+            run: Main entry point for the manager process.
             run_resolver: Main loop for resolving events from all pipes.
-            _prepare_resolvers: Prepares methods for resolving request and response events.
-            _prepare: Prepares the manager before starting the event resolver loop.
-            _find_worker: Finds a worker based on its communication pipe.
-            _find_stream: Finds a worker associated with a specific stream.
+            start: Starts the manager process with an optional router queue.
             start_worker: Starts a new worker for handling an event.
-            _remove_worker: Removes a worker from the manager's tracking.
-            health_check: Handles health check events from the router.
             store_get: Handles store get requests.
-            _subscribe_static_resolvers: Subscribes to static event resolvers.
-            after_start: Hook for actions after the manager starts.
-            run: Main entry point for the manager process.
-            start: Starts the manager process with an optional router queue.
         """
 
     def __init__(self, router_queue: Optional[Queue] = None, logger: Optional[Logger] = None,
                  from_time: Optional[datetime] = None) -> None:
         """
         Initializes the manager with an optional router queue, logger, and start time for event filtering.
 
@@ -96,101 +96,93 @@
             self.logger = logger
         self._requests: dict[Type[Event], Union[Callable, Event]] = {}
         self._responses: dict[Type[Event], Union[Callable, Event]] = {}
         self._workers: Storage[Worker]
         self._manager_id: str
         self._from_time = from_time
 
-    def _subscribe(self) -> None:
-        """
-        Subscribes the manager to events by sending subscription requests to the router queue.
-        It handles both requests and responses, registering them for the manager to resolve.
+    def _find_worker(self, pipe: Connection) -> Tuple[str, Worker]:
         """
-        if not self._requests and not self._responses:
-            self.logger.info("No events to subscribe!")
-            return
-        self.router_pipe, pipe = Pipe(duplex=False)
-        self.logger.debug(f"Count of events to register as requests: %s", len(self._requests) + len(self._responses))
-        for event_type in self._requests.keys():
-            self.logger.debug(f"Registration event: %s", event_type)
-            self.router_queue.put(
-                Subscribe(pipe=pipe, name=self.name, event_type=event_type, request=True, from_time=self._from_time))
-            while True:
-                event = self.router_pipe.recv()
-                if isinstance(event, Subscribe):
-                    self.logger.debug(f"Event was registered: %s", event.event_type)
-                    break
-                else:
-                    self.logger.debug(f"Unresolved event was received: %s", event)
-                    self._unresolved.append(event)
+        Finds and returns the worker associated with a given pipe. This method iterates through all registered
+        workers, comparing the given pipe with each worker's associated pipe. When it finds a match, it returns
+        both the identifier of the worker and the worker instance itself.
 
-        for event_type in self._responses.keys():
-            self.logger.debug(f"Count of events to register as answers: %s ", event_type)
-            self.router_queue.put(
-                Subscribe(pipe=pipe, name=self.name, event_type=event_type, request=False, from_time=self._from_time))
-            while True:
-                event = self.router_pipe.recv()
-                if isinstance(event, Subscribe):
-                    self.logger.debug(f"Event was registered: %s", event.event_type)
-                    break
-                else:
-                    self.logger.debug(f"Unresolved event was received: %s", event)
-                    self._unresolved.append(event)
+        Parameters:
+            pipe (Connection): The communication pipe to match with a worker. This is used to identify the specific
+                               worker associated with the given communication channel.
 
-        pipe.close()
-        self.logger.debug(f"Registering was successful!")
-        unresolved_count = len(self._unresolved)
-        if unresolved_count > 0:
-            self.logger.debug(f"Received %s of undelivered events!", unresolved_count)
+        Returns:
+            Tuple[str, Worker]: A tuple containing the worker's identifier and the worker instance itself. The
+                                identifier is a unique string that represents the worker, and the Worker is the
+                                actual instance handling tasks for a specific pipe.
 
-    def _resolve_undelivered_events(self) -> None:
-        """
-        Processes any events that were received but not resolved immediately upon subscription.
-        This ensures no events are lost during the setup phase of the manager.
+        Raises:
+            ValueError: Raised if no worker is found that matches the given pipe. This exception indicates that
+                        the pipe provided does not correspond to any currently registered worker. It's crucial for
+                        callers to handle this exception, especially in cases where dynamic registration and
+                        deregistration of workers may lead to situations where a pipe is no longer valid.
+
+        Example:
+            To find a worker associated with a specific pipe, you would call this method with the pipe as the argument.
+            If a worker is found that uses this pipe for communication, the method will return the worker's identifier
+            and the worker instance. If no such worker exists, a ValueError will be raised.
         """
-        if self._unresolved:
-            while True:
-                try:
-                    event = self._unresolved.pop(0)
-                    self.logger.debug("Solving undelivered event: %s", event)
-                except IndexError:
-                    self.logger.debug(f"Unresolved events were resolved!")
-                    break
-                self.resolve(event)
+        for key, worker in self._workers.items():
+            if worker.pipe == pipe:
+                return key, worker
         else:
-            self.logger.debug(f"No unresolved events!")
-        del self._unresolved
+            raise ValueError
 
-    def _resolve_callback_stream_create(self, event: StreamCreate, worker: Worker) -> None:
+    def _find_stream(self, event: Event, stream: Optional[str] = None) -> Worker:
         """
-        Handles the creation of a new stream for communication between workers and the manager.
+        Locates a worker handling a specific event stream. This method searches through all available workers to find
+        one that is handling the stream associated with the given event. If a specific stream identifier is provided,
+        the method attempts to match the worker handling that exact stream. If no specific stream is provided, it looks
+        for any worker that handles the event type of the provided event.
 
         Parameters:
-            event (StreamCreate): The event indicating a request to create a new stream.
-            worker (Worker): The worker instance associated with the stream creation request.
-        """
-        raise NotImplementedError("yet")
-        # stream_message = event.message
-        # key = f"{stream_message._command}_{randint(1000, 9999)}"
-        # stream_message._stream = key
-        # worker.streams[stream_message.__class__] = key
-        # self.router_queue.put(stream_message)
+            event (Event): The event for which to find the associated stream. This parameter is used to determine
+                           the type of event and, optionally, its specific stream identifier.
+            stream (Optional[str]): An optional specific stream identifier to match. If provided, the method
+                                    will attempt to find a worker that handles not just the event type but also
+                                    this specific stream.
 
-    def _resolve_callback_stream_message(self, event: StreamMessage, worker: Worker) -> None:
+        Returns:
+            Worker: The worker instance handling the specified event stream. This worker is capable of processing
+                    the event, considering both its type and, if specified, its stream identifier.
+
+        Raises:
+            ValueError: If no worker is found that matches the criteria (both event type and, if provided, the
+                        specific stream identifier), a ValueError is raised. This exception indicates that there
+                        are no available workers for the given event and stream combination.
+
+        Note:
+            This method logs debug information about the number of workers and their streams during the search
+            process. If the event class does not match any worker's streams or if no worker is found for the
+            specified stream, additional debug information is logged.
+
+        Example:
+            Given an event of a certain type and, optionally, a specific stream identifier, this method will iterate
+            through all workers to find one that matches these criteria. If no match is found, it raises a ValueError.
         """
-        Processes a message within an existing stream, routing it appropriately based on the worker and stream state.
+        self.logger.debug("Count of workers: %s", len(self._workers.values()))
+        for worker in self._workers.values():
+            if event.__class__ not in worker.streams:
+                self.logger.debug("Count of streams: %s", len(worker.streams))
+                continue
+            if worker.streams[event.__class__] == stream or event._stream:
+                return worker
+        else:
+            raise ValueError
 
-        Parameters:
-            event (StreamMessage): The event containing a message for a specific stream.
-            worker (Worker): The worker instance that sent the stream message or for which the message is intended.
+    def _prepare(self) -> None:
         """
-        raise NotImplementedError("yet")
-        # stream_message = event.message
-        # stream_message._stream = worker.streams[stream_message.__class__]
-        # self.router_queue.put(event.message)
+        Prepares the manager before starting the event resolver loop, initializing necessary attributes and structures.
+        """
+        self._workers = Storage()
 
     def _prepare_resolvers(self) -> None:
         """
         Prepares and registers methods for resolving both request and response events based on their event types.
         This method iterates through all methods of the class that do not start with "__". It then registers those
         methods starting with "solve_req_" for request events and methods starting with "solve_res_" for response events
         by extracting the event type from the method's signature.
@@ -205,14 +197,15 @@
             instead of 'event' and logs detailed error information including the method signature.
 
         Example:
             If a method intended to solve a request event does not follow the expected signature, such as missing
             the 'event' parameter or having a different parameter name in its place, the KeyError will be raised
             with a message indicating the issue, and the problematic parameter name will be logged.
         """
+
         def get_event(sig: Signature) -> Type[Event]:
             try:
                 event_sig = dict(sig.parameters.items())["event"]
             except KeyError as e:
                 self.logger.error("Second parameter of solve function has to be 'event' not '%s'",
                                   list(sig.parameters.keys())[0], exc_info=e)
                 raise e
@@ -225,172 +218,52 @@
                 event = get_event(signature(method))
                 self._requests[event] = method
             elif method_name.startswith("solve_res_"):
                 method = getattr(self, method_name)
                 event = get_event(signature(method))
                 self._responses[event] = method
 
-    @property
-    def additional_pipes(self) -> set[Connection]:
-        """
-        Specifies additional pipes for the manager to listen on. Override to add custom pipes.
-
-        Returns:
-            set[Connection]: A set of additional pipes.
-        """
-        return set()
-
-    @property
-    def name(self) -> str:
-        """
-        Specifies the manager's name. Override to provide a custom name.
-
-        Returns:
-            str: The manager's name.
-        """
-        return self.__class__.__name__
-
-    @property
-    def workers(self) -> list[ManagerWorkerEvent]:
-        """
-        Defines workers and their associated events. Override to specify workers.
-
-        Returns:
-            list[ManagerWorkerEvent]: A list of `ManagerWorkerEvent` instances.
-        """
-        return []
-
-    def resolve_callback_worker(self, event: Event, worker: Worker) -> None:
-        """
-         Default method for handling events received from workers. It forwards received events to the router queue.
-
-         Parameters:
-             event (Event): The received event.
-             worker (Worker): Information about the worker that sent the event.
-         """
-        event._worker = worker.worker.name
-        self.router_queue.put(event)
-
-    def resolve_callback_pipe(self, event: Event, pipe: Connection) -> None:
-        """
-         Handles events received from unknown pipes, which are not associated with known workers.
-
-         Parameters:
-             event (Event): The received event.
-             pipe (Connection): The pipe from which the event was received.
-         """
-        self.logger.warning("Unknown event from unknown pipe: %s %s", event, pipe)
-
-    def resolve_unknown(self, event: Event) -> None:
-        """
-        Handles unknown events received from the router pipe that do not match any registered request or response.
-
-        Parameters:
-            event (Event): The unknown event received.
-        """
-        self.logger.warning("Unknown event: %s", event)
-
-    def _prepare(self) -> None:
-        """
-        Prepares the manager before starting the event resolver loop, initializing necessary attributes and structures.
-        """
-        self._workers = Storage()
-
-    def _subscribe_static_resolvers(self) -> None:
-        """
-         Registers static resolver methods for specific event types, such as health checks and store get requests.
-         """
-        self.logger.debug("Registering static resolvers")
-        self._requests[HealthCheck] = self.health_check
-        self._responses[Get] = self.store_get
-
-    def _find_stream(self, event: Event, stream: Optional[str] = None) -> Worker:
-        """
-        Locates a worker handling a specific event stream. This method searches through all available workers to find
-        one that is handling the stream associated with the given event. If a specific stream identifier is provided,
-        the method attempts to match the worker handling that exact stream. If no specific stream is provided, it looks
-        for any worker that handles the event type of the provided event.
-
-        Parameters:
-            event (Event): The event for which to find the associated stream. This parameter is used to determine
-                           the type of event and, optionally, its specific stream identifier.
-            stream (Optional[str]): An optional specific stream identifier to match. If provided, the method
-                                    will attempt to find a worker that handles not just the event type but also
-                                    this specific stream.
-
-        Returns:
-            Worker: The worker instance handling the specified event stream. This worker is capable of processing
-                    the event, considering both its type and, if specified, its stream identifier.
-
-        Raises:
-            ValueError: If no worker is found that matches the criteria (both event type and, if provided, the
-                        specific stream identifier), a ValueError is raised. This exception indicates that there
-                        are no available workers for the given event and stream combination.
-
-        Note:
-            This method logs debug information about the number of workers and their streams during the search
-            process. If the event class does not match any worker's streams or if no worker is found for the
-            specified stream, additional debug information is logged.
-
-        Example:
-            Given an event of a certain type and, optionally, a specific stream identifier, this method will iterate
-            through all workers to find one that matches these criteria. If no match is found, it raises a ValueError.
-        """
-        self.logger.debug("Count of workers: %s", len(self._workers.values()))
-        for worker in self._workers.values():
-            if event.__class__ not in worker.streams:
-                self.logger.debug("Count of streams: %s", len(worker.streams))
-                continue
-            if worker.streams[event.__class__] == stream or event._stream:
-                return worker
-        else:
-            raise ValueError
-
     def _remove_worker(self, worker_key: str) -> None:
         """
         Removes a worker from the manager's tracking based on its unique identifier.
 
         Parameters:
             worker_key (str): The identifier of the worker to remove.
         """
         worker = self._workers[worker_key]
         worker.pipe.close()
         self._workers.pop(worker_key)
 
-    def _find_worker(self, pipe: Connection) -> Tuple[str, Worker]:
+    def _resolve_callback_stream_create(self, event: StreamCreate, worker: Worker) -> None:
         """
-        Finds and returns the worker associated with a given pipe. This method iterates through all registered
-        workers, comparing the given pipe with each worker's associated pipe. When it finds a match, it returns
-        both the identifier of the worker and the worker instance itself.
+        Handles the creation of a new stream for communication between workers and the manager.
 
         Parameters:
-            pipe (Connection): The communication pipe to match with a worker. This is used to identify the specific
-                               worker associated with the given communication channel.
-
-        Returns:
-            Tuple[str, Worker]: A tuple containing the worker's identifier and the worker instance itself. The
-                                identifier is a unique string that represents the worker, and the Worker is the
-                                actual instance handling tasks for a specific pipe.
+            event (StreamCreate): The event indicating a request to create a new stream.
+            worker (Worker): The worker instance associated with the stream creation request.
+        """
+        raise NotImplementedError("yet")
+        # stream_message = event.message
+        # key = f"{stream_message._command}_{randint(1000, 9999)}"
+        # stream_message._stream = key
+        # worker.streams[stream_message.__class__] = key
+        # self.router_queue.put(stream_message)
 
-        Raises:
-            ValueError: Raised if no worker is found that matches the given pipe. This exception indicates that
-                        the pipe provided does not correspond to any currently registered worker. It's crucial for
-                        callers to handle this exception, especially in cases where dynamic registration and
-                        deregistration of workers may lead to situations where a pipe is no longer valid.
+    def _resolve_callback_stream_message(self, event: StreamMessage, worker: Worker) -> None:
+        """
+        Processes a message within an existing stream, routing it appropriately based on the worker and stream state.
 
-        Example:
-            To find a worker associated with a specific pipe, you would call this method with the pipe as the argument.
-            If a worker is found that uses this pipe for communication, the method will return the worker's identifier
-            and the worker instance. If no such worker exists, a ValueError will be raised.
+        Parameters:
+            event (StreamMessage): The event containing a message for a specific stream.
+            worker (Worker): The worker instance that sent the stream message or for which the message is intended.
         """
-        for key, worker in self._workers.items():
-            if worker.pipe == pipe:
-                return key, worker
-        else:
-            raise ValueError
+        raise NotImplementedError("yet")
+        # stream_message = event.message
+        # stream_message._stream = worker.streams[stream_message.__class__]
+        # self.router_queue.put(event.message)
 
     def _resolve_callback_stream_close(self, event: StreamClose, worker: Worker) -> None:
         """
         Handles the closing of a stream, cleaning up any resources or references associated with the stream.
 
         Parameters:
             event (StreamClose): The event indicating a request to close a specific stream.
@@ -416,14 +289,144 @@
         #         self.logger.error("Nelze určit typ zprávy pro ukončení streamu: %s", event)
         # else:
         #     response = Response(0)
         #     stream_message.set_response(response)
         #
         # self.router_queue.put(stream_message)
 
+    def _resolve_undelivered_events(self) -> None:
+        """
+        Processes any events that were received but not resolved immediately upon subscription.
+        This ensures no events are lost during the setup phase of the manager.
+        """
+        if self._unresolved:
+            while True:
+                try:
+                    event = self._unresolved.pop(0)
+                    self.logger.debug("Solving undelivered event: %s", event)
+                except IndexError:
+                    self.logger.debug(f"Unresolved events were resolved!")
+                    break
+                self.resolve(event)
+        else:
+            self.logger.debug(f"No unresolved events!")
+        del self._unresolved
+
+    def _subscribe(self) -> None:
+        """
+        Subscribes the manager to events by sending subscription requests to the router queue.
+        It handles both requests and responses, registering them for the manager to resolve.
+        """
+        if not self._requests and not self._responses:
+            self.logger.info("No events to subscribe!")
+            return
+        self.router_pipe, pipe = Pipe(duplex=False)
+        self.logger.debug(f"Count of events to register as requests: %s", len(self._requests) + len(self._responses))
+        for event_type in self._requests.keys():
+            self.logger.debug(f"Registration event: %s", event_type)
+            self.router_queue.put(
+                Subscribe(pipe=pipe, name=self.name, event_type=event_type, request=True, from_time=self._from_time))
+            while True:
+                event = self.router_pipe.recv()
+                if isinstance(event, Subscribe):
+                    self.logger.debug(f"Event was registered: %s", event.event_type)
+                    break
+                else:
+                    self.logger.debug(f"Unresolved event was received: %s", event)
+                    self._unresolved.append(event)
+
+        for event_type in self._responses.keys():
+            self.logger.debug(f"Count of events to register as answers: %s ", event_type)
+            self.router_queue.put(
+                Subscribe(pipe=pipe, name=self.name, event_type=event_type, request=False, from_time=self._from_time))
+            while True:
+                event = self.router_pipe.recv()
+                if isinstance(event, Subscribe):
+                    self.logger.debug(f"Event was registered: %s", event.event_type)
+                    break
+                else:
+                    self.logger.debug(f"Unresolved event was received: %s", event)
+                    self._unresolved.append(event)
+
+        pipe.close()
+        self.logger.debug(f"Registering was successful!")
+        unresolved_count = len(self._unresolved)
+        if unresolved_count > 0:
+            self.logger.debug(f"Received %s of undelivered events!", unresolved_count)
+
+    def _subscribe_static_resolvers(self) -> None:
+        """
+        Registers static resolver methods for specific event types, such as health checks and store get requests.
+        """
+        self.logger.debug("Registering static resolvers")
+        self._requests[HealthCheck] = self.health_check
+        self._responses[Get] = self.store_get
+
+    @property
+    def additional_pipes(self) -> set[Connection]:
+        """
+        Specifies additional pipes for the manager to listen on. Override to add custom pipes.
+
+        Returns:
+            set[Connection]: A set of additional pipes.
+        """
+        return set()
+
+    @property
+    def name(self) -> str:
+        """
+        Specifies the manager's name. Override to provide a custom name.
+
+        Returns:
+            str: The manager's name.
+        """
+        return self.__class__.__name__
+
+    @property
+    def workers(self) -> list[ManagerWorkerEvent]:
+        """
+        Defines workers and their associated events. Override to specify workers.
+
+        Returns:
+            list[ManagerWorkerEvent]: A list of `ManagerWorkerEvent` instances.
+        """
+        return []
+
+    def after_start(self) -> None:
+        """
+        Hook method called after the manager process starts. Can be overridden to perform initialization tasks.
+        """
+        pass
+
+    def get_pipes(self) -> set[Connection]:
+        """
+        Collects all communication pipes used by the manager, including the router pipe and any worker pipes.
+
+        Returns:
+            set[Connection]: A set of all pipes for the manager to listen on.
+        """
+        pipes = set()
+        if self.router_pipe:
+            pipes.add(self.router_pipe)
+        if self._workers:
+            worker_pipes = set(worker.pipe for worker in self._workers.values())
+            pipes.update(worker_pipes)
+            self.logger.debug("Count of workers to listen to: %s", len(worker_pipes))
+        pipes.update(self.additional_pipes)
+        return pipes
+
+    def health_check(self, event: HealthCheck) -> None:
+        """
+        Responds to a health check request from the router, indicating the manager's status.
+
+        Parameters:
+            event (HealthCheck): The health check event received from the router.
+        """
+        event.response.name = self.name
+
     def resolve(self, event: Event) -> None:
         """
         The central method for resolving events received by the manager. This method determines how an event
         is processed, whether it's an incoming request, a response to a previous request, or a system event like
         stream creation or closing.
 
         Parameters:
@@ -485,30 +488,61 @@
                 self.resolve_unknown(event)
             else:
                 had_response = event.has_response()
                 resolver(event)
                 if not had_response and event.has_response() and event.response._changed:
                     self.router_queue.put(event)
 
-    def get_pipes(self) -> set[Connection]:
+    def resolve_callback_pipe(self, event: Event, pipe: Connection) -> None:
         """
-        Collects all communication pipes used by the manager, including the router pipe and any worker pipes.
+        Handles events received from unknown pipes, which are not associated with known workers.
+        It's designed to log warnings for these unhandled events. This function can be overridden
+        in subclasses, but such an override should be performed only by users who are aware of the
+        potential implications and have a clear understanding of the function's internals and the
+        event handling mechanism.
 
-        Returns:
-            set[Connection]: A set of all pipes for the manager to listen on.
+         Parameters:
+            event (Event): The received event.
+            pipe (Connection): The pipe from which the event was received.
+         """
+        self.logger.warning("Event from unknown pipe: %s %s", event, pipe)
+
+    def resolve_callback_worker(self, event: Event, worker: Worker) -> None:
         """
-        pipes = set()
-        if self.router_pipe:
-            pipes.add(self.router_pipe)
-        if self._workers:
-            worker_pipes = set(worker.pipe for worker in self._workers.values())
-            pipes.update(worker_pipes)
-            self.logger.debug("Count of workers to listen to: %s", len(worker_pipes))
-        pipes.update(self.additional_pipes)
-        return pipes
+        Default method for handling events received from workers. It forwards received events to the router queue.
+
+        Parameters:
+            event (Event): The received event.
+            worker (Worker): Information about the worker that sent the event.
+        """
+        event._worker = worker.worker.name
+        self.router_queue.put(event)
+
+    def resolve_unknown(self, event: Event) -> None:
+        """
+        Handles unknown events received from the router pipe that do not match any registered request or response.
+
+        Parameters:
+            event (Event): The unknown event received.
+        """
+        self.logger.warning("Unknown event: %s", event)
+
+    def run(self) -> None:
+        """
+        Main entry point for the manager process. Sets up event subscriptions, prepares the manager,
+        and enters the main event resolution loop.
+        """
+        self.logger.debug(f"{self.name} is running!")
+        self._prepare_resolvers()
+        self._subscribe_static_resolvers()
+        self._subscribe()
+        self._prepare()
+        self.after_start()
+        self._resolve_undelivered_events()
+        self.run_resolver()
 
     def run_resolver(self) -> None:
         """
         Main event loop of the manager. Listens on all pipes for incoming events and resolves them appropriately.
         """
         while True:
             pipes = self.get_pipes()
@@ -547,14 +581,48 @@
                                 self.resolve_callback_worker(event, worker)
                         except ValueError:
                             self.resolve_callback_pipe(event, active_pipe)
 
             except KeyboardInterrupt:
                 return
 
+    def start(self, router_queue: Optional[Queue] = None) -> None:
+        """
+        Starts the manager process with an optional router queue specified. This method initiates the manager's
+        operation, allowing it to begin processing events. The router queue is a crucial component for communication
+        between the manager and the router, facilitating the dispatch and handling of events.
+
+        Parameters:
+            router_queue (Optional[Queue[Event]]): The event queue used for communication with the router. If provided,
+                                                   this queue will be set as the current router queue for the manager.
+                                                   This queue is essential for the manager to receive and process events.
+
+        Raises:
+            RuntimeError: Raised if no router queue is provided and no router queue has been set previously. This
+                          exception ensures that the manager cannot start without a means to communicate with the
+                          router, as the lack of a router queue would prevent the manager from functioning correctly.
+
+        Note:
+            If a router queue is not provided as an argument to this method, the manager will attempt to use a
+            previously set router queue. It's essential to either provide a router queue when calling this method
+            or set one before its execution. Failure to do so will result in a RuntimeError, indicating the
+            manager's inability to start due to the absence of a communication channel with the router.
+
+        Example:
+            To start the manager, you may either provide a router queue directly when calling the start method
+            or ensure that the manager has a router queue set beforehand. This flexibility allows for different
+            use cases, such as reusing an existing queue or setting a new one as needed.
+        """
+        if router_queue is not None:
+            self.router_queue = router_queue
+        if self.router_queue is None:
+            raise RuntimeError("Queue must be specified")
+        self.router_queue = self.router_queue
+        super().start()
+
     def start_worker(self, event: Event, resolver: Callable, *args, **kwargs) -> Worker:
         """
         Starts a new worker process or thread to handle an event based on the specified resolver.
 
         Parameters:
             event (Event): The event that needs handling.
             resolver (Callable): The function or callable object that will handle the event.
@@ -576,82 +644,19 @@
         self._workers.append(worker)
         worker.worker.start()
         if isinstance(resolver, WorkerProcess):
             pipe_remote.close()
         self.logger.debug("Worker %s has been started", worker.worker.name)
         return worker
 
-    def health_check(self, event: HealthCheck) -> None:
-        """
-        Responds to a health check request from the router, indicating the manager's status.
-
-        Parameters:
-            event (HealthCheck): The health check event received from the router.
-        """
-        event.response.name = self.name
-
     def store_get(self, event: Get) -> None:
         """
         Handles store get requests, typically for retrieving data from the manager's internal storage or cache.
 
         Parameters:
             event (Get): The get request event, containing details of what data to retrieve.
         """
         if self._workers and event._worker is not None:
             for worker in self._workers.values():
                 if worker.worker.name == event._worker:
                     worker.pipe.send(event)
                     break
-
-    def run(self) -> None:
-        """
-        Main entry point for the manager process. Sets up event subscriptions, prepares the manager,
-        and enters the main event resolution loop.
-        """
-        self.logger.debug(f"{self.name} is running!")
-        self._prepare_resolvers()
-        self._subscribe_static_resolvers()
-        self._subscribe()
-        self._prepare()
-        self.after_start()
-        self._resolve_undelivered_events()
-        self.run_resolver()
-
-    def start(self, router_queue: Optional[Queue] = None) -> None:
-        """
-        Starts the manager process with an optional router queue specified. This method initiates the manager's
-        operation, allowing it to begin processing events. The router queue is a crucial component for communication
-        between the manager and the router, facilitating the dispatch and handling of events.
-
-        Parameters:
-            router_queue (Optional[Queue[Event]]): The event queue used for communication with the router. If provided,
-                                                   this queue will be set as the current router queue for the manager.
-                                                   This queue is essential for the manager to receive and process events.
-
-        Raises:
-            RuntimeError: Raised if no router queue is provided and no router queue has been set previously. This
-                          exception ensures that the manager cannot start without a means to communicate with the
-                          router, as the lack of a router queue would prevent the manager from functioning correctly.
-
-        Note:
-            If a router queue is not provided as an argument to this method, the manager will attempt to use a
-            previously set router queue. It's essential to either provide a router queue when calling this method
-            or set one before its execution. Failure to do so will result in a RuntimeError, indicating the
-            manager's inability to start due to the absence of a communication channel with the router.
-
-        Example:
-            To start the manager, you may either provide a router queue directly when calling the start method
-            or ensure that the manager has a router queue set beforehand. This flexibility allows for different
-            use cases, such as reusing an existing queue or setting a new one as needed.
-        """
-        if router_queue is not None:
-            self.router_queue = router_queue
-        if self.router_queue is None:
-            raise RuntimeError("Queue must be specified")
-        self.router_queue = self.router_queue
-        super().start()
-
-    def after_start(self) -> None:
-        """
-        Hook method called after the manager process starts. Can be overridden to perform initialization tasks.
-        """
-        pass
```

### Comparing `edri-2024.3.9/edri/abstract/manager/manager_priority_base.py` & `edri-2024.4.1/edri/abstract/manager/manager_priority_base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,20 +24,20 @@
     Attributes:
         event_queue (PriorityQueue[QueueItem]): A priority queue for managing events based on their priority.
         event_worker (Thread): A thread dedicated to handling command execution based on event priority.
         waking_up (tuple[Connection, Connection]): A pair of connections used to wake up the manager when a new worker starts.
 
     Methods:
         __init__: Initializes the ManagerPriorityBase with an optional router queue and logger.
-        get_priority: Abstract method that must be implemented to define the priority of events.
         _prepare: Prepares the manager by initializing the event queue, event worker thread, and waking up pipe.
         additional_pipes: Property to include the waking_up pipe in the set of additional pipes the manager listens to.
-        start_worker: Overrides the start_worker method to wake up the manager when a new worker is started.
-        run_resolver: Main event loop, enhanced to handle events based on priority.
         command_handler: Thread target function that processes events from the priority queue.
+        get_priority: Abstract method that must be implemented to define the priority of events.
+        run_resolver: Main event loop, enhanced to handle events based on priority.
+        start_worker: Overrides the start_worker method to wake up the manager when a new worker is started.
     """
 
     def __init__(self, router_queue: Optional["Queue[Event]"] = None, logger: Optional[Logger] = None) -> None:
         """
         Initializes the ManagerPriorityBase with an optional router queue and logger, setting up the foundation
         for event priority management.
 
@@ -46,28 +46,14 @@
             logger (Optional[Logger]): Logger instance for logging messages.
         """
         super().__init__(router_queue, logger)
         self.event_queue: "PriorityQueue[QueueItem]" = None  # type: ignore
         self.event_worker: Thread = None  # type: ignore
         self.waking_up: tuple[Connection, Connection] = None  # type: ignore
 
-    @abstractmethod
-    def get_priority(self, event: Type[Event]) -> int:
-        """
-        Abstract method that determines the priority of an event. Must be implemented by subclasses
-        to define how event priorities are assigned.
-
-        Parameters:
-            event (Type[Event]): The class of the event for which the priority needs to be determined.
-
-        Returns:
-            int: The priority of the event.
-        """
-        pass
-
     def _prepare(self) -> None:
         """
         Prepares the manager by initializing the event queue, starting the event worker thread,
         and setting up the waking_up pipe used to signal new work.
         """
         super()._prepare()
         self.event_queue = PriorityQueue()
@@ -81,31 +67,36 @@
         Includes the waking_up pipe in the set of additional pipes the manager listens to.
 
         Returns:
             set[Connection]: A set of additional pipes, including the waking_up pipe.
         """
         return {self.waking_up[0]}
 
-    def start_worker(self, event: Event, resolver: Callable, *args, **kwargs) -> Worker:
+    def command_handler(self) -> None:
         """
-        Starts a worker to handle an event and signals the manager that new work has started,
-        potentially affecting the priority queue.
+         The thread target function that processes events from the priority queue, ensuring that events are handled
+         in order of their priority.
+         """
+        while True:
+            event = self.event_queue.get().item
+            self.resolve(event)
+
+    @abstractmethod
+    def get_priority(self, event: Type[Event]) -> int:
+        """
+        Abstract method that determines the priority of an event. Must be implemented by subclasses
+        to define how event priorities are assigned.
 
         Parameters:
-            event (Event): The event to be handled by the worker.
-            resolver (Callable): The function that will handle the event.
-            *args: Additional positional arguments for the resolver.
-            **kwargs: Additional keyword arguments for the resolver.
+            event (Type[Event]): The class of the event for which the priority needs to be determined.
 
         Returns:
-            Worker: The worker instance that was started to handle the event.
+            int: The priority of the event.
         """
-        worker = super().start_worker(event, resolver, *args, **kwargs)
-        self.waking_up[1].send(None)
-        return worker
+        pass
 
     def run_resolver(self) -> None:
         """
         The main event loop for the manager, enhanced to handle events based on priority. It listens on all pipes,
         including the waking_up pipe, to efficiently process and prioritize events.
         """
         while True:
@@ -149,15 +140,24 @@
                             else:
                                 self.resolve_callback_worker(event, worker)
                         except ValueError:
                             self.resolve_callback_pipe(event, active_pipe)
             except KeyboardInterrupt:
                 return
 
-    def command_handler(self) -> None:
+    def start_worker(self, event: Event, resolver: Callable, *args, **kwargs) -> Worker:
         """
-         The thread target function that processes events from the priority queue, ensuring that events are handled
-         in order of their priority.
-         """
-        while True:
-            event = self.event_queue.get().item
-            self.resolve(event)
+        Starts a worker to handle an event and signals the manager that new work has started,
+        potentially affecting the priority queue.
+
+        Parameters:
+            event (Event): The event to be handled by the worker.
+            resolver (Callable): The function that will handle the event.
+            *args: Additional positional arguments for the resolver.
+            **kwargs: Additional keyword arguments for the resolver.
+
+        Returns:
+            Worker: The worker instance that was started to handle the event.
+        """
+        worker = super().start_worker(event, resolver, *args, **kwargs)
+        self.waking_up[1].send(None)
+        return worker
```

### Comparing `edri-2024.3.9/edri/abstract/worker/worker.py` & `edri-2024.4.1/edri/abstract/worker/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,54 +13,62 @@
 
 class Worker(Generic[T]):
     """
     A generic worker class designed to communicate with a manager through events. It supports sending and receiving messages,
     creating message streams for continuous communication, and handling the lifecycle of these streams.
 
     Attributes:
-        _name (str): The name of the worker, used for logging purposes.
-        _manager_pipe (Connection): The communication pipe to the manager.
-        event (EventType): The initial event associated with the worker.
-        logger (Logger): Logger instance for logging messages.
         _buffer (List[Event]): A buffer for storing received events that are not yet processed.
+        _manager_pipe (Connection): The communication pipe to the manager.
+        _name (str): The name of the worker, used for logging purposes.
         _stream_buffer (Optional[Event]): A buffer for the last received stream event.
         _stream_key (Optional[str]): The unique key identifying the current stream.
+        event (EventType): The initial event associated with the worker.
+        logger (Logger): Logger instance for logging messages.
 
     Methods:
+        __init__: Initializes a new Worker instance.
+        do: Abstract method defining the main logic of the worker; to be implemented by subclasses.
         message_send: Sends a message to the manager.
         message_receive: Receives a message from the manager, blocking if no message is available.
+        run: Entry point for the worker's execution, wrapping the `do` method with error handling and cleanup.
+        stream_close: Closes the current message stream.
         stream_create: Initiates a stream for sending and receiving messages of a specific type.
         stream_exists: Checks if a message stream currently exists.
         stream_poll: Checks if there are messages available in the stream.
-        stream_wait: Waits for a message in the stream, with an optional timeout.
         stream_receive: Receives a message from the stream.
         stream_send: Sends a message through the stream.
-        stream_close: Closes the current message stream.
-        do: Abstract method defining the main logic of the worker; to be implemented by subclasses.
-        run: Entry point for the worker's execution, wrapping the `do` method with error handling and cleanup.
+        stream_wait: Waits for a message in the stream, with an optional timeout.
     """
-    def __init__(self, pipe: Connection, event: Event, name: str) -> None:
+    def __init__(self, pipe: Connection, event: T, name: str) -> None:
         """
         Initializes a new Worker instance.
 
         Parameters:
             pipe (Connection): The communication pipe to the manager.
             event (EventType): The initial event associated with this worker.
             name (str): A name for the worker, used for logging.
         """
-        self._name = name
-        self._manager_pipe = pipe
-        self.event = event
-        self.logger = getLogger(self._name)
         self._buffer: List[Event] = []
+        self._manager_pipe = pipe
+        self._name = name
         self._stream_buffer: Optional[Event] = None
         self._stream_key: Optional[str] = None
+        self.event = event
+        self.logger = getLogger(self._name)
         if event._stream:
             self._stream_key = event._stream
 
+    @abstractmethod
+    def do(self) -> None:
+        """
+        Abstract method that should be implemented by subclasses to define the worker's main logic.
+        """
+        pass
+
     def message_send(self, message: Event) -> None:
         """
         Sends a message to the manager.
 
         Parameters:
             message (Event): The event to be sent.
         """
@@ -84,14 +92,47 @@
                     self.logger.debug("Stream closed")
                 else:
                     self.logger.warning("Wrong key for closing stream: %s", message._stream)
                 continue
             else:
                 return message
 
+    def run(self) -> None:
+        """
+        The main entry point for the worker's execution. It calls the `do` method and handles any exceptions,
+        ensuring proper cleanup and communication with the manager upon termination.
+        """
+        try:
+            self.do()
+        except Exception as e:
+            self.logger.error("Worker %s was closed unexpectedly", self._name, exc_info=e)
+        finally:
+            worker_quit = WorkerQuit()
+            self._manager_pipe.send(worker_quit)
+
+    def stream_close(self, message: Optional[Type[Event]] = None) -> bool:
+        """
+        Closes the current message stream, optionally sending a final message as part of the closure process.
+
+        Parameters:
+            message (Optional[Type[Event]]): The type of the final message to send before closing the stream, if any.
+
+        Returns:
+            bool: True if the stream was successfully closed; False if there was an issue closing the stream.
+        """
+        self.logger.debug("Closing the stream...")
+        if not self._stream_key:
+            self.logger.warning("Key was not provided")
+            return False
+        self.logger.debug("Stream uzavřen: %s", self._stream_key)
+        stream_close = StreamClose(message=message)
+        stream_close._stream = self._stream_key
+        self.message_send(stream_close)
+        return True
+
     def stream_create(self, message: Event) -> bool:
         """
         Initiates a message stream for continuous communication with the manager, or potentially other workers,
         using a specific type of message.
 
         Parameters:
             message (Event): The initial message for which the stream is to be created.
@@ -131,42 +172,14 @@
             if message._stream:
                 self._stream_buffer = message
                 return True
             else:
                 self._buffer.append(message)
         return False
 
-    def stream_wait(self, timeout: Optional[int] = None) -> bool:
-        """
-         Waits for a message to be available in the stream, optionally with a timeout. This method is blocking
-         and will pause execution until a message is received or the timeout is reached.
-
-         Parameters:
-             timeout (Optional[int]): The maximum time to wait for a message, in seconds. If None, waits indefinitely.
-
-         Returns:
-             bool: True if a message became available in the stream; False if the timeout was reached without receiving a message.
-         """
-        if self._stream_buffer:
-            return True
-        while self.stream_exists:
-            if self._manager_pipe.poll(timeout) is not None:
-                message = self._manager_pipe.recv()
-                if message._stream.endswith(STREAM_CLOSE_MARK):
-                    self.logger.debug("Stream closed on both ends: %s", message._stream[:-len(STREAM_CLOSE_MARK)])
-                    self._stream_key = None
-                    return False
-                if message._stream:
-                    self._stream_buffer = message
-                    return True
-                else:
-                    self._buffer.append(message)
-
-        return False
-
     def stream_receive(self) -> Event:
         """
         Receives a message from the current stream. This method should be called after confirming that a message
         is available via `stream_poll` or `stream_wait`.
 
         Returns:
             Event: The next message from the stream.
@@ -187,46 +200,34 @@
 
         Parameters:
             message (Event): The message to be sent through the stream.
         """
         stream_message = StreamMessage(message=message)
         self._manager_pipe.send(stream_message)
 
-    def stream_close(self, message: Optional[Type[Event]] = None) -> bool:
+    def stream_wait(self, timeout: Optional[int] = None) -> bool:
         """
-        Closes the current message stream, optionally sending a final message as part of the closure process.
-
-        Parameters:
-            message (Optional[Type[Event]]): The type of the final message to send before closing the stream, if any.
+         Waits for a message to be available in the stream, optionally with a timeout. This method is blocking
+         and will pause execution until a message is received or the timeout is reached.
 
-        Returns:
-            bool: True if the stream was successfully closed; False if there was an issue closing the stream.
-        """
-        self.logger.debug("Closing the stream...")
-        if not self._stream_key:
-            self.logger.warning("Key was not provided")
-            return False
-        self.logger.debug("Stream uzavřen: %s", self._stream_key)
-        stream_close = StreamClose(message=message)
-        stream_close._stream = self._stream_key
-        self.message_send(stream_close)
-        return True
+         Parameters:
+             timeout (Optional[int]): The maximum time to wait for a message, in seconds. If None, waits indefinitely.
 
-    @abstractmethod
-    def do(self) -> None:
-        """
-        Abstract method that should be implemented by subclasses to define the worker's main logic.
-        """
-        pass
+         Returns:
+             bool: True if a message became available in the stream; False if the timeout was reached without receiving a message.
+         """
+        if self._stream_buffer:
+            return True
+        while self.stream_exists:
+            if self._manager_pipe.poll(timeout) is not None:
+                message = self._manager_pipe.recv()
+                if message._stream.endswith(STREAM_CLOSE_MARK):
+                    self.logger.debug("Stream closed on both ends: %s", message._stream[:-len(STREAM_CLOSE_MARK)])
+                    self._stream_key = None
+                    return False
+                if message._stream:
+                    self._stream_buffer = message
+                    return True
+                else:
+                    self._buffer.append(message)
 
-    def run(self) -> None:
-        """
-        The main entry point for the worker's execution. It calls the `do` method and handles any exceptions,
-        ensuring proper cleanup and communication with the manager upon termination.
-        """
-        try:
-            self.do()
-        except Exception as e:
-            self.logger.error("Worker %s was closed unexpectedly", self._name, exc_info=e)
-        finally:
-            worker_quit = WorkerQuit()
-            self._manager_pipe.send(worker_quit)
+        return False
```

### Comparing `edri-2024.3.9/edri/abstract/worker/worker_process.py` & `edri-2024.4.1/edri/abstract/worker/worker_process.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/abstract/worker/worker_thread.py` & `edri-2024.4.1/edri/abstract/worker/worker_thread.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/dataclass/event/__init__.py` & `edri-2024.4.1/edri/dataclass/event/__init__.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/dataclass/event/event.py` & `edri-2024.4.1/edri/dataclass/event/event.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/dataclass/event/response.py` & `edri-2024.4.1/edri/dataclass/event/response.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/rest/server.py` & `edri-2024.4.1/edri/rest/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from logging import getLogger
 from multiprocessing import Process
 from multiprocessing.queues import Queue
 from os import remove
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from types import NoneType
-from typing import Optional, Type, Any, Union, Pattern
+from typing import Type, Any, Union, Pattern
 from urllib.parse import parse_qs, quote
 from re import compile
 from http.cookies import SimpleCookie
 
 from uvicorn import Config, Server
 
-from edri.config.setting import UPLOAD_FILES_PREFIX, REST_RESPONSE_TIMEOUT
+from edri.config.setting import UPLOAD_FILES_PREFIX, REST_RESPONSE_TIMEOUT, REST_PORT
 from edri.abstract.api_base import APIBase
 from edri.config.constant import ApiType
 from edri.dataclass.event import Method, Event, api_events
 from edri.dataclass.event.response import ResponseStatus
 from edri.utility.function import snake2camel, camel2snake
 
 
@@ -576,12 +576,12 @@
                 self.unregister(pipe, key)
 
     def run(self) -> None:
         """
         Configures and starts the Uvicorn server to run the ASGI application for
         handling RESTful API requests.
         """
-        config = Config(self.App(self.api_broker_queue), host="0.0.0.0", port=8878, log_level="debug", workers=8)
+        config = Config(self.App(self.api_broker_queue), host="0.0.0.0", port=REST_PORT, log_level="debug", workers=8)
         # ssl_keyfile="/home/marek/rest.key",
         # ssl_certfile="/home/marek/rest.crt")
         server = Server(config)
         server.run()
```

### Comparing `edri-2024.3.9/edri/router/cache.py` & `edri-2024.4.1/edri/router/cache.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/router/health_checker.py` & `edri-2024.4.1/edri/router/health_checker.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/router/router.py` & `edri-2024.4.1/edri/router/router.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/store.py` & `edri-2024.4.1/edri/store.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/switch/forwarder.py` & `edri-2024.4.1/edri/switch/forwarder.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/switch/receiver.py` & `edri-2024.4.1/edri/switch/receiver.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/switch/sender.py` & `edri-2024.4.1/edri/switch/sender.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/switch/switch.py` & `edri-2024.4.1/edri/switch/switch.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/utility/api_broker.py` & `edri-2024.4.1/edri/utility/api_broker.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/utility/connector/connector.py` & `edri-2024.4.1/edri/utility/connector/connector.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/utility/connector/socket.py` & `edri-2024.4.1/edri/utility/connector/socket.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/utility/eta.py` & `edri-2024.4.1/edri/utility/eta.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/utility/function.py` & `edri-2024.4.1/edri/utility/function.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/utility/scheduler.py` & `edri-2024.4.1/edri/utility/scheduler.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/utility/storage.py` & `edri-2024.4.1/edri/utility/storage.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/utility/store.py` & `edri-2024.4.1/edri/utility/store.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri/websocket/api.py` & `edri-2024.4.1/edri/websocket/api.py`

 * *Files identical despite different names*

### Comparing `edri-2024.3.9/edri.egg-info/PKG-INFO` & `edri-2024.4.1/edri.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edri
-Version: 2024.3.9
+Version: 2024.4.1
 Summary: Event Driven Routing Infrastructure
 Author: Marek Olšan
 Author-email: marek.olsan@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `edri-2024.3.9/edri.egg-info/SOURCES.txt` & `edri-2024.4.1/edri.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 edri/abstract/manager/manager_priority_base.py
 edri/abstract/worker/__init__.py
 edri/abstract/worker/worker.py
 edri/abstract/worker/worker_process.py
 edri/abstract/worker/worker_thread.py
 edri/config/__init__.py
 edri/config/constant.py
-edri/config/logging.py
 edri/config/setting.py
 edri/dataclass/__init__.py
 edri/dataclass/queue_item.py
 edri/dataclass/worker.py
 edri/dataclass/client/__init__.py
 edri/dataclass/client/client.py
 edri/dataclass/event/__init__.py
```

### Comparing `edri-2024.3.9/setup.py` & `edri-2024.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 where events act as messages exchanged between various components to control and manage operations. Drawing parallels with TCP/IP in 
 computer networks, EDRI's **routing infrastructure** facilitates the exchange and delivery of events. Instead of IP ranges, event types (
 e.g., file uploads) are used to determine the destination of each event, ensuring efficient and targeted delivery to the appropriate 
 recipients. This approach streamlines the process of managing distributed tasks within applications."""
 
 setup(
     name='edri',
-    version='2024.03.09',
+    version='2024.04.01',
     packages=find_packages(),
     description='Event Driven Routing Infrastructure',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Marek Olšan',
     author_email='marek.olsan@gmail.com',
     install_requires=[
```

### Comparing `edri-2024.3.9/tests/test_storage.py` & `edri-2024.4.1/tests/test_storage.py`

 * *Files identical despite different names*

