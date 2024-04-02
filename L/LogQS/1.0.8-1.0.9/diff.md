# Comparing `tmp/LogQS-1.0.8.tar.gz` & `tmp/LogQS-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogQS-1.0.8.tar", last modified: Mon Feb 12 19:01:04 2024, max compression
+gzip compressed data, was "LogQS-1.0.9.tar", last modified: Fri Feb 16 15:43:07 2024, max compression
```

## Comparing `LogQS-1.0.8.tar` & `LogQS-1.0.9.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.937248 LogQS-1.0.8/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.937248 LogQS-1.0.8/LogQS.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15100 2024-02-12 19:01:04.000000 LogQS-1.0.8/LogQS.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4059 2024-02-12 19:01:04.000000 LogQS-1.0.8/LogQS.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-02-12 19:01:04.000000 LogQS-1.0.8/LogQS.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2024-02-12 19:01:04.000000 LogQS-1.0.8/LogQS.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2024-02-12 19:01:04.000000 LogQS-1.0.8/LogQS.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-02-12 19:01:04.000000 LogQS-1.0.8/LogQS.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-01-29 16:28:55.000000 LogQS-1.0.8/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15100 2024-02-12 19:01:04.937248 LogQS-1.0.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4614 2024-01-31 18:56:52.000000 LogQS-1.0.8/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14175 2024-01-29 16:28:55.000000 LogQS-1.0.8/README_client.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.909248 LogQS-1.0.8/lqs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      110 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/__main__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.909248 LogQS-1.0.8/lqs/client/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1442 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/__main__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.913248 LogQS-1.0.8/lqs/client/admin/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/admin/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/admin/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12185 2024-02-07 20:46:36.000000 LogQS-1.0.8/lqs/client/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2024-02-07 20:43:45.000000 LogQS-1.0.8/lqs/client/config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.913248 LogQS-1.0.8/lqs/client/core/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      993 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/core/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3717 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/core/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2994 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/core/delete.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7756 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/core/fetch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6515 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/core/list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5311 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/core/update.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.913248 LogQS-1.0.8/lqs/client/dsm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/dsm/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1605 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/dsm/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1458 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/dsm/delete.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2728 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/dsm/fetch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/dsm/list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2633 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/dsm/update.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.917248 LogQS-1.0.8/lqs/client/pjm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      567 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/pjm/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      491 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/pjm/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      507 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/pjm/delete.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      690 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/pjm/fetch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      743 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/pjm/list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      679 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/pjm/update.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4331 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/client/server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    70683 2024-02-12 18:57:10.000000 LogQS-1.0.8/lqs/client/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.917248 LogQS-1.0.8/lqs/common/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/common/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2955 2024-01-29 16:28:55.000000 LogQS-1.0.8/lqs/common/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3716 2024-02-01 20:54:07.000000 LogQS-1.0.8/lqs/common/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1948 2024-02-07 16:41:19.000000 LogQS-1.0.8/lqs/common/facade.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10466 2024-02-10 16:16:25.000000 LogQS-1.0.8/lqs/common/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.917248 LogQS-1.0.8/lqs/interface/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.917248 LogQS-1.0.8/lqs/interface/admin/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/admin/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      967 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/admin/create.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.917248 LogQS-1.0.8/lqs/interface/admin/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/admin/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      683 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/admin/models/command.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.917248 LogQS-1.0.8/lqs/interface/base/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/base/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2156 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/base/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      606 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/base/delete.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      973 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/base/fetch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6309 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/base/list.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.921248 LogQS-1.0.8/lqs/interface/base/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8599 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/base/models/__common__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      189 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/base/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      699 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/base/models/api_key.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1337 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/base/models/role.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1158 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/base/models/user.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1200 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/base/update.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.921248 LogQS-1.0.8/lqs/interface/core/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      264 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27311 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7552 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/delete.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11519 2024-02-02 16:59:24.000000 LogQS-1.0.8/lqs/interface/core/fetch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    44479 2024-02-02 16:59:45.000000 LogQS-1.0.8/lqs/interface/core/list.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.925248 LogQS-1.0.8/lqs/interface/core/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2024-01-30 21:18:10.000000 LogQS-1.0.8/lqs/interface/core/models/__common__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1834 2024-02-08 18:17:54.000000 LogQS-1.0.8/lqs/interface/core/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      175 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/api_key.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1856 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/digestion.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2031 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/digestion_part.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1174 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/digestion_topic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1090 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/group.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1308 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/hook.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1720 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/ingestion.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2009 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/ingestion_part.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      571 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/label.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2292 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/log.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1771 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/object.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1285 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/object_store.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1117 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/query.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2024-02-12 18:10:59.000000 LogQS-1.0.8/lqs/interface/core/models/record.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      174 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/role.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/tag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3498 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/topic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      182 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/user.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1034 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/models/workflow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11282 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/core/update.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.929248 LogQS-1.0.8/lqs/interface/dsm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      259 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5420 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1512 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/delete.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1771 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/fetch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16253 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/list.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.929248 LogQS-1.0.8/lqs/interface/dsm/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      182 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/models/__common__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      497 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1293 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/models/announcement.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      175 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/models/api_key.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1303 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/models/comment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/models/configuration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1329 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/models/datastore.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1340 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/models/datastore_association.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      174 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/models/role.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      979 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/models/usage_tick.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      182 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/models/user.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2951 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/dsm/update.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.933248 LogQS-1.0.8/lqs/interface/pjm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      259 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/pjm/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1813 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/pjm/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      421 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/pjm/delete.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/pjm/fetch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4653 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/pjm/list.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.933248 LogQS-1.0.8/lqs/interface/pjm/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1617 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/pjm/models/__common__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      183 2024-02-08 18:18:22.000000 LogQS-1.0.8/lqs/interface/pjm/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1415 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/pjm/models/event.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1225 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/pjm/models/job.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3146 2024-02-12 18:10:59.000000 LogQS-1.0.8/lqs/interface/pjm/models/jsonl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      167 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/pjm/models/manifest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      826 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/interface/pjm/update.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.933248 LogQS-1.0.8/lqs/transcode/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2501 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/transcode/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      128 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/transcode/__main__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.933248 LogQS-1.0.8/lqs/transcode/ark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/transcode/ark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8023 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/transcode/ark/ark_deserialization_methods.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23227 2024-01-31 18:09:43.000000 LogQS-1.0.8/lqs/transcode/ark/ark_json_parser.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1029 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/transcode/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      101 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/transcode/errors.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-12 19:01:04.937248 LogQS-1.0.8/lqs/transcode/ros1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43555 2024-01-31 18:47:59.000000 LogQS-1.0.8/lqs/transcode/ros1/RosMessageLexer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    86509 2024-01-31 18:48:01.000000 LogQS-1.0.8/lqs/transcode/ros1/RosMessageParser.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8857 2024-01-31 18:48:00.000000 LogQS-1.0.8/lqs/transcode/ros1/RosMessageParserListener.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18705 2024-01-31 18:47:42.000000 LogQS-1.0.8/lqs/transcode/ros1/RosMessageParserVisitor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6792 2024-01-31 18:29:34.000000 LogQS-1.0.8/lqs/transcode/ros1/RosMessageParserVisitorForMD5.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/transcode/ros1/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3357 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/transcode/ros1/ros_deserialization_methods.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2024-01-29 16:28:56.000000 LogQS-1.0.8/lqs/transcode/ros1/ros_message_deserializer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      583 2024-01-29 16:28:56.000000 LogQS-1.0.8/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2024-01-29 16:28:56.000000 LogQS-1.0.8/requirements-client.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-02-12 19:01:04.937248 LogQS-1.0.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1346 2024-02-12 19:00:58.000000 LogQS-1.0.8/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.568962 LogQS-1.0.9/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.568962 LogQS-1.0.9/LogQS.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15100 2024-02-16 15:43:07.000000 LogQS-1.0.9/LogQS.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4059 2024-02-16 15:43:07.000000 LogQS-1.0.9/LogQS.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-02-16 15:43:07.000000 LogQS-1.0.9/LogQS.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2024-02-16 15:43:07.000000 LogQS-1.0.9/LogQS.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2024-02-16 15:43:07.000000 LogQS-1.0.9/LogQS.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-02-16 15:43:07.000000 LogQS-1.0.9/LogQS.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-01-29 16:28:55.000000 LogQS-1.0.9/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15100 2024-02-16 15:43:07.568962 LogQS-1.0.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4614 2024-01-31 18:56:52.000000 LogQS-1.0.9/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14175 2024-01-29 16:28:55.000000 LogQS-1.0.9/README_client.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.476961 LogQS-1.0.9/lqs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      110 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/__main__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.480961 LogQS-1.0.9/lqs/client/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1442 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/__main__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.480961 LogQS-1.0.9/lqs/client/admin/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/admin/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/admin/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12185 2024-02-07 20:46:36.000000 LogQS-1.0.9/lqs/client/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2024-02-07 20:43:45.000000 LogQS-1.0.9/lqs/client/config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.488961 LogQS-1.0.9/lqs/client/core/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      993 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/core/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3717 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/core/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2994 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/core/delete.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7756 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/core/fetch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6515 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/core/list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5311 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/core/update.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.492962 LogQS-1.0.9/lqs/client/dsm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/dsm/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1605 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/dsm/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1458 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/dsm/delete.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2728 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/dsm/fetch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/dsm/list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2633 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/dsm/update.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.496961 LogQS-1.0.9/lqs/client/pjm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      567 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/pjm/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      491 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/pjm/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      507 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/pjm/delete.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      690 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/pjm/fetch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      743 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/pjm/list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      679 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/pjm/update.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4331 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/client/server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    70699 2024-02-14 17:31:32.000000 LogQS-1.0.9/lqs/client/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.500961 LogQS-1.0.9/lqs/common/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/common/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2955 2024-01-29 16:28:55.000000 LogQS-1.0.9/lqs/common/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3716 2024-02-01 20:54:07.000000 LogQS-1.0.9/lqs/common/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1948 2024-02-07 16:41:19.000000 LogQS-1.0.9/lqs/common/facade.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10466 2024-02-10 16:16:25.000000 LogQS-1.0.9/lqs/common/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.500961 LogQS-1.0.9/lqs/interface/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.500961 LogQS-1.0.9/lqs/interface/admin/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/admin/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      967 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/admin/create.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.504962 LogQS-1.0.9/lqs/interface/admin/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/admin/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      683 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/admin/models/command.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.508962 LogQS-1.0.9/lqs/interface/base/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/base/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2156 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/base/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      606 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/base/delete.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      973 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/base/fetch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6310 2024-02-16 14:44:29.000000 LogQS-1.0.9/lqs/interface/base/list.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.508962 LogQS-1.0.9/lqs/interface/base/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8609 2024-02-16 15:39:06.000000 LogQS-1.0.9/lqs/interface/base/models/__common__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      189 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/base/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      699 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/base/models/api_key.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1337 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/base/models/role.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1158 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/base/models/user.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1200 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/base/update.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.512961 LogQS-1.0.9/lqs/interface/core/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      264 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27311 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7552 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/delete.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11519 2024-02-02 16:59:24.000000 LogQS-1.0.9/lqs/interface/core/fetch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46549 2024-02-16 15:00:43.000000 LogQS-1.0.9/lqs/interface/core/list.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.528962 LogQS-1.0.9/lqs/interface/core/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2024-01-30 21:18:10.000000 LogQS-1.0.9/lqs/interface/core/models/__common__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1834 2024-02-08 18:17:54.000000 LogQS-1.0.9/lqs/interface/core/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      175 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/api_key.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1856 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/digestion.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2031 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/digestion_part.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1174 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/digestion_topic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1090 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/group.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1308 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/hook.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1720 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/ingestion.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2009 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/ingestion_part.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      571 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/label.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2292 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/log.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1771 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/object.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1285 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/object_store.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1117 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/query.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2024-02-12 18:10:59.000000 LogQS-1.0.9/lqs/interface/core/models/record.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      174 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/role.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/tag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3498 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/topic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      182 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/user.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1034 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/models/workflow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11282 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/core/update.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.532962 LogQS-1.0.9/lqs/interface/dsm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      259 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5420 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1512 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/delete.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1771 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/fetch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17135 2024-02-16 14:57:18.000000 LogQS-1.0.9/lqs/interface/dsm/list.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.536962 LogQS-1.0.9/lqs/interface/dsm/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      182 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/models/__common__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      497 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1293 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/models/announcement.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      175 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/models/api_key.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1303 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/models/comment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/models/configuration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1329 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/models/datastore.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1340 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/models/datastore_association.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      174 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/models/role.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      979 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/models/usage_tick.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      182 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/models/user.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2951 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/dsm/update.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.540962 LogQS-1.0.9/lqs/interface/pjm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      259 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/pjm/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1813 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/pjm/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      421 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/pjm/delete.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/pjm/fetch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4935 2024-02-16 14:55:59.000000 LogQS-1.0.9/lqs/interface/pjm/list.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.548962 LogQS-1.0.9/lqs/interface/pjm/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1617 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/pjm/models/__common__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      183 2024-02-08 18:18:22.000000 LogQS-1.0.9/lqs/interface/pjm/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1415 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/pjm/models/event.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1225 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/pjm/models/job.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3146 2024-02-12 18:10:59.000000 LogQS-1.0.9/lqs/interface/pjm/models/jsonl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      167 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/pjm/models/manifest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      826 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/interface/pjm/update.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.552962 LogQS-1.0.9/lqs/transcode/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2501 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/transcode/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      128 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/transcode/__main__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.556962 LogQS-1.0.9/lqs/transcode/ark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/transcode/ark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8023 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/transcode/ark/ark_deserialization_methods.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23227 2024-01-31 18:09:43.000000 LogQS-1.0.9/lqs/transcode/ark/ark_json_parser.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1029 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/transcode/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      101 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/transcode/errors.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-16 15:43:07.568962 LogQS-1.0.9/lqs/transcode/ros1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43555 2024-01-31 18:47:59.000000 LogQS-1.0.9/lqs/transcode/ros1/RosMessageLexer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    86509 2024-01-31 18:48:01.000000 LogQS-1.0.9/lqs/transcode/ros1/RosMessageParser.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8857 2024-01-31 18:48:00.000000 LogQS-1.0.9/lqs/transcode/ros1/RosMessageParserListener.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18705 2024-01-31 18:47:42.000000 LogQS-1.0.9/lqs/transcode/ros1/RosMessageParserVisitor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6792 2024-01-31 18:29:34.000000 LogQS-1.0.9/lqs/transcode/ros1/RosMessageParserVisitorForMD5.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/transcode/ros1/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3357 2024-01-29 16:28:56.000000 LogQS-1.0.9/lqs/transcode/ros1/ros_deserialization_methods.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4811 2024-02-14 14:53:34.000000 LogQS-1.0.9/lqs/transcode/ros1/ros_message_deserializer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      583 2024-01-29 16:28:56.000000 LogQS-1.0.9/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2024-01-29 16:28:56.000000 LogQS-1.0.9/requirements-client.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-02-16 15:43:07.568962 LogQS-1.0.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1346 2024-02-16 15:43:01.000000 LogQS-1.0.9/setup.py
```

### Comparing `LogQS-1.0.8/LogQS.egg-info/PKG-INFO` & `LogQS-1.0.9/LogQS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogQS
-Version: 1.0.8
+Version: 1.0.9
 Summary: A client for interacting with the LogQS Service.
 Home-page: https://github.com/carnegierobotics/LogQS
 Author: Nathan Margaglio
 Author-email: nmargaglio@carnegierobotics.com
 Project-URL: Bug Tracker, https://github.com/carnegierobotics/LogQS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LogQS-1.0.8/LogQS.egg-info/SOURCES.txt` & `LogQS-1.0.9/LogQS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/PKG-INFO` & `LogQS-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogQS
-Version: 1.0.8
+Version: 1.0.9
 Summary: A client for interacting with the LogQS Service.
 Home-page: https://github.com/carnegierobotics/LogQS
 Author: Nathan Margaglio
 Author-email: nmargaglio@carnegierobotics.com
 Project-URL: Bug Tracker, https://github.com/carnegierobotics/LogQS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LogQS-1.0.8/README.md` & `LogQS-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/README_client.md` & `LogQS-1.0.9/README_client.md`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/__init__.py` & `LogQS-1.0.9/lqs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/common.py` & `LogQS-1.0.9/lqs/client/common.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/config.py` & `LogQS-1.0.9/lqs/client/config.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/core/__init__.py` & `LogQS-1.0.9/lqs/client/core/__init__.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/core/create.py` & `LogQS-1.0.9/lqs/client/core/create.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/core/delete.py` & `LogQS-1.0.9/lqs/client/core/delete.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/core/fetch.py` & `LogQS-1.0.9/lqs/client/core/fetch.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/core/list.py` & `LogQS-1.0.9/lqs/client/core/list.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/core/update.py` & `LogQS-1.0.9/lqs/client/core/update.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/dsm/__init__.py` & `LogQS-1.0.9/lqs/client/dsm/__init__.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/dsm/create.py` & `LogQS-1.0.9/lqs/client/dsm/create.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/dsm/delete.py` & `LogQS-1.0.9/lqs/client/dsm/delete.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/dsm/fetch.py` & `LogQS-1.0.9/lqs/client/dsm/fetch.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/dsm/list.py` & `LogQS-1.0.9/lqs/client/dsm/list.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/dsm/update.py` & `LogQS-1.0.9/lqs/client/dsm/update.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/pjm/__init__.py` & `LogQS-1.0.9/lqs/client/pjm/__init__.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/pjm/fetch.py` & `LogQS-1.0.9/lqs/client/pjm/fetch.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/pjm/list.py` & `LogQS-1.0.9/lqs/client/pjm/list.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/pjm/update.py` & `LogQS-1.0.9/lqs/client/pjm/update.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/server.py` & `LogQS-1.0.9/lqs/client/server.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/client/utils.py` & `LogQS-1.0.9/lqs/client/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,14 @@
         resource_name: Optional[str] = None,
         list_params: dict = {},
         create_if_missing: bool = True,
         create_params: dict = {},
         create_func: Optional[Callable] = None,
         list_func: Optional[Callable] = None,
         fetch_func: Optional[Callable] = None,
-        verbosity: Optional[str] = "debug",
     ) -> Any:
         """
         Fetch or create a resource by name.
 
         This function fetches a resource by id if provided, or by name if provided, or creates the resource if it doesn't exist and create_if_missing is True.
         If no resource id or name is provided, the function returns None.
 
@@ -86,27 +85,21 @@
             resource_name (str, optional): The name of the resource. Defaults to None.
             list_params (dict, optional): Additional parameters to use when listing the resource. Defaults to {}.
             create_if_missing (bool, optional): Whether to create the resource if it doesn't exist. Defaults to True.
             create_params (dict, optional): Additional parameters to use when creating the resource. Defaults to {}.
             create_func (Callable, optional): The function to use when creating the resource. Defaults to None.
             list_func (Callable, optional): The function to use when listing the resource. Defaults to None.
             fetch_func (Callable, optional): The function to use when fetching the resource. Defaults to None.
-            verbosity (Optional[str], optional): The verbosity level to use. One of "debug", "info", or "error". Defaults to "debug".
 
         Raises:
             NotFoundException: If no resource is found and create_if_missing is False.
 
         Returns:
             Any: The fetched or created resource, or None if no resource is found or created.
         """
-
-        def logger(msg):
-            if verbosity is not None:
-                getattr(self.app, verbosity.lower())(msg)
-
         resource = None
         if resource_id is None and resource_name is not None:
             # if no resource id is provided, we try to find the resource by name
             resources = list_func(name=resource_name, **list_params).data
             if len(resources) == 0:
                 # we didn't find the resource by name
                 if create_if_missing:
@@ -118,21 +111,15 @@
                     )
             else:
                 # we use the found resource
                 resource = resources[0]
         elif resource_id is not None and resource_name is None:
             # if no resource name is provided, we try to find the resource by id
             resource = fetch_func(resource_id).data
-        else:
-            logger(
-                f"No {resource_type} provided, will create {resource_type}s for each log file/directory found."
-            )
 
-        if resource is not None:
-            logger(f"Using {resource_type} {resource.name} ({resource.id})")
         return resource
 
     def calculate_etag(self, file_path: str, part_size: int = 100 * 1024 * 1024) -> str:
         """
         Calculate the ETag of a file.
 
         This function calculates the ETag of a file assuming it is uploaded as a multipart upload.
@@ -316,14 +303,17 @@
             ConflictException: If existing resources conflict with the upload.
 
         Returns:
             tuple["Object", list["ObjectPart"]]: The uploaded object and its parts.
         """
 
         # First, create/re-create/fetch/etc. the log object
+        if continue_upload and overwrite:
+            raise Exception("Only one one of continue_upload, overwrite can be set to true")
+        
         log_id = str(log_id)
         if object_key is None:
             object_key = file_path.split("/")[-1]
         if key_replacement is not None:
             object_key = object_key.replace(*key_replacement)
         if key_prefix is not None:
             object_key = os.path.join(key_prefix, object_key)
@@ -487,14 +477,304 @@
             if not self.verify_object_integrity(file_path, log_object, part_size):
                 raise Exception(
                     f"Integrity check failed for object {object_key} in log {log_id}."
                 )
 
         return log_object, log_object_parts
 
+    def upload_log_object_part_from_memory(
+        self,
+        log_id: str,
+        object_key: str,
+        part_number: int,
+        part_data: bytes | str,
+        size: int,
+        max_attempts: int = 3,
+        backoff_factor: float = 5.0,
+        connect_timeout: int = 60,
+        read_timeout: int = 600,
+    ):
+        """
+        Upload a part of a file to a log object.
+
+        Args:
+            log_id (str): The log id to upload the object part to.
+            object_key (str): The key of the object to upload the part to.
+            part_number (int): The part number of the object part.
+            part_data (bytes | str): The data to upload.
+            size (int): The size of the part to upload.
+            max_attempts (int, optional): The maximum number of attempts to upload the part. Defaults to 3.
+            backoff_factor (float, optional): The backoff factor for retrying the upload. Defaults to 5.0.
+            connect_timeout (int, optional): The connection timeout for the upload. Defaults to 60.
+            read_timeout (int, optional): The read timeout for the upload. Defaults to 600.
+
+        Raises:
+            Exception: If the upload fails.
+
+        Returns:
+            ObjectPart: The uploaded object part.
+        """
+        log_id = str(log_id)
+        object_part = self.app.create.log_object_part(
+            log_id=log_id,
+            object_key=object_key,
+            size=size,
+            part_number=part_number,
+        ).data
+        upload_object_data_url = object_part.presigned_url
+
+        attempt_count = 0
+        response = None
+        for attempt_count in range(1, max_attempts + 1):
+            if attempt_count > 1:
+                self.app.debug(
+                    f"Retrying upload of part {part_number} of object {object_key} in log {log_id} (attempt {attempt_count}/{max_attempts})."
+                )
+            try:
+                response = requests.put(
+                    upload_object_data_url,
+                    data=part_data,
+                    timeout=(connect_timeout, read_timeout),
+                )
+                break
+            except Exception as e:
+                self.app.debug(
+                    f"Error while uploading part {part_number} of object {object_key} in log {log_id} (attempt {attempt_count}/{max_attempts}): {e}"
+                )
+                time.sleep(backoff_factor * (2 ** (attempt_count - 1)))
+                continue
+
+        if response is None:
+            raise Exception(
+                f"Failed to upload part {part_number} of object {object_key} in log {log_id} after {max_attempts} attempts."
+            )
+
+        if response.status_code != 200:
+            raise Exception(f"Error while uploading object part: {response.text}")
+
+        return self.app.fetch.log_object_part(
+            log_id=log_id,
+            object_key=object_key,
+            part_number=part_number,
+        ).data
+
+    def upload_log_object_from_memory(
+        self,
+        log_id: str,
+        file_like: io.BytesIO | io.StringIO,
+        object_key: str,
+        key_replacement: tuple[str, str] = None,
+        key_prefix: str = None,
+        part_size: int = 100 * 1024 * 1024,
+        max_workers: int | None = 8,
+        skip_if_exists: bool = False,
+        continue_upload: bool = True,
+        skip_if_complete: bool = False,
+        overwrite: bool = False,
+    ) -> tuple["Object", list["ObjectPart"]]:
+        """
+        Upload a file-like object to a log.
+
+        The file is uploaded as a log object, meaning it is associated with a single log given by log_id.
+        The file is split into parts of size part_size, which are uploaded in parallel using a maximum of max_workers workers.
+        Note that larger values for part_size and max_workers will generally result in faster uploads, but may also result in higher memory usage.
+
+        If skip_if_exists is set to True, the upload will be skipped if the object already exists.
+        If continue_upload is set to True, any existing parts of the object will be skipped and the upload will continue from where it left off.
+        If continue_upload is set to True and skip_if_complete is set to True, the upload will be skipped if the object is already complete.
+        If overwrite is set to True, any existing object with the same key will be deleted before the upload.
+
+        Args:
+            log_id (str): The log id to upload the object to.
+            file_like (io.BytesIO | io.StringIO): The file-like object to upload.
+            object_key (str): The key to use for the object.
+            key_replacement (tuple[str, str], optional): A tuple of strings to replace in the object key. Defaults to None.
+            key_prefix (str, optional): A prefix to add to the object key. Defaults to None.
+            part_size (int, optional): The size of each part to upload. Defaults to 100 * 1024 * 1024.
+            max_workers (int, optional): The maximum number of workers to use for parallel uploads. Defaults to 8.
+            skip_if_exists (bool, optional): Whether to skip the upload if the object already exists. Defaults to False.
+            continue_upload (bool, optional): Whether to continue an existing upload. Defaults to True.
+            skip_if_complete (bool, optional): Whether to skip the continued upload if the object is already complete. Defaults to False.
+            overwrite (bool, optional): Whether to overwrite the object if it already exists. Defaults to False.
+
+        Raises:
+            ConflictException: If existing resources conflict with the upload.
+
+        Returns:
+            tuple["Object", list["ObjectPart"]]: The uploaded object and its parts.
+        """
+
+        # First, create/re-create/fetch/etc. the log object
+        log_id = str(log_id)
+        if key_replacement is not None:
+            object_key = object_key.replace(*key_replacement)
+        if key_prefix is not None:
+            object_key = os.path.join(key_prefix, object_key)
+        if object_key.startswith("/"):
+            object_key = object_key[1:]
+
+        try:
+            log_object = self.app.create.log_object(
+                log_id=log_id,
+                key=object_key,
+            ).data
+        except ConflictException as e:
+            if skip_if_exists:
+                self.app.debug(
+                    f"Skipping upload of object {object_key} in log {log_id}."
+                )
+                log_object = self.app.fetch.log_object(
+                    log_id=log_id, object_key=object_key
+                ).data
+                return log_object, []
+
+            if continue_upload:
+                self.app.debug(
+                    f"Continuing upload of object {object_key} in log {log_id}."
+                )
+                log_object = self.app.fetch.log_object(
+                    log_id=log_id, object_key=object_key
+                ).data
+                if log_object.upload_state == "complete":
+                    if skip_if_complete:
+                        self.app.debug(
+                            f"Skipping complete upload of object {object_key} in log {log_id}."
+                        )
+                        return log_object, []
+                    else:
+                        raise ConflictException(
+                            f"Can't continue upload: Upload of Object {object_key} in log {log_id} is already complete."
+                        )
+            elif overwrite:
+                self.app.debug(f"Overwriting object {object_key} in log {log_id}.")
+                self.app.delete.log_object(log_id=log_id, object_key=object_key)
+                log_object = self.app.create.log_object(
+                    log_id=log_id,
+                    key=object_key,
+                ).data
+            else:
+                raise e
+
+        # Then, figure out which parts we need to upload
+        if isinstance(file_like, io.StringIO):
+            object_size = len(file_like.getvalue())
+        elif isinstance(file_like, io.BytesIO):
+            object_size = file_like.getbuffer().nbytes
+        else:
+            raise TypeError(
+                "file_like must be an instance of io.BytesIO or io.StringIO"
+            )
+        number_of_parts = object_size // part_size + 1
+        log_object_parts: List[ObjectPart] = []
+
+        parts_res = self.app.list.log_object_part(log_id=log_id, object_key=object_key)
+        log_object_parts += parts_res.data
+        while parts_res.is_truncated:
+            parts_res = self.app.list.log_object_part(
+                log_id=log_id,
+                object_key=object_key,
+                part_number_marker=parts_res.next_part_number_marker,
+            )
+            log_object_parts += parts_res.data
+        self.app.debug(
+            f"Found {len(log_object_parts)} existing parts for object {object_key} in log {log_id}."
+        )
+        if continue_upload is False:
+            if len(log_object_parts) > 0:
+                raise ConflictException(
+                    f"Object {object_key} in log {log_id} already has {len(log_object_parts)} parts."
+                    "Set continue_upload to True to continue the upload or overwrite to start over."
+                )
+        else:
+            self.app.debug(
+                f"Found {len(log_object_parts)} existing parts for object {object_key} in log {log_id}."
+            )
+        log_object_parts.sort(key=lambda part: part.part_number)
+
+        # Validate existing parts sizes
+        for idx, part in enumerate(log_object_parts):
+            if part.part_number == number_of_parts:
+                # the last part is allowed to be smaller than part_size
+                continue
+            if part.size == 0:
+                # the part exists, but it has no data, so we'll overwrite it anyways
+                continue
+            if part.size != part_size:
+                raise ConflictException(
+                    f"Part {part.part_number} of object {object_key} in log {log_id} has an unexpected size {part.size}."
+                    f"All parts except for the last part need to be the same size as the given part_size {part_size}."
+                    f"Either overwrite the object to start over or change the part_size to match existing parts."
+                )
+
+        def should_skip_part(part_number):
+            existing_part = next(
+                (part for part in log_object_parts if part.part_number == part_number),
+                None,
+            )
+            if existing_part is not None:
+                if existing_part.size == 0:
+                    self.app.debug(
+                        f"Overwriting empty part {part_number} of object {object_key} in log {log_id}."
+                    )
+                else:
+                    self.app.debug(
+                        f"Skipping existing part {part_number} of object {object_key} in log {log_id}."
+                    )
+                    return True
+            return False
+
+        # Upload the parts (in parallel if max_workers is set)
+        if max_workers is not None:
+            futures = []
+            with ThreadPoolExecutor(max_workers=max_workers) as executor:
+                for idx in range(0, number_of_parts):
+                    offset = idx * part_size
+                    file_like.seek(offset)
+                    size = min(part_size, object_size - offset)
+                    part_number = idx + 1
+                    if should_skip_part(part_number):
+                        continue
+                    futures.append(
+                        executor.submit(
+                            self.upload_log_object_part_from_memory,
+                            log_id=log_id,
+                            object_key=object_key,
+                            part_number=part_number,
+                            part_data=file_like.read(size),
+                            size=size,
+                        )
+                    )
+
+                for future in futures:
+                    log_object_parts.append(future.result())
+        else:
+            for idx in range(0, number_of_parts):
+                offset = idx * part_size
+                file_like.seek(offset)
+                size = min(part_size, object_size - offset)
+                part_number = idx + 1
+                if should_skip_part(part_number):
+                    continue
+                log_object_parts.append(
+                    self.upload_log_object_part_from_memory(
+                        log_id=log_id,
+                        object_key=object_key,
+                        part_number=part_number,
+                        part_data=file_like.read(size),
+                        size=size,
+                    )
+                )
+
+        # Finally, mark the object as complete to finish the upload
+        log_object = self.app.update.log_object(
+            log_id=log_id, object_key=object_key, data={"upload_state": "complete"}
+        ).data
+
+        return log_object, log_object_parts
+
     def upload_log_objects(
         self,
         log_id: str,
         file_dir: str,
         fail_if_empty: bool = True,
         key_replacement: tuple[str, str] = None,
         key_prefix: str = None,
@@ -702,78 +982,127 @@
             int: The number of uploaded log files.
         """
 
         def logger(msg):
             if verbosity is not None:
                 getattr(self.app, verbosity.lower())(msg)
 
-        # First, figure out which group we're working with
-        group = self.fetch_by_name_or_create(
-            resource_type="group",
-            resource_id=group_id,
-            resource_name=group_name,
-            list_params={},
-            create_if_missing=create_group_if_missing,
-            create_params={"note": group_note, "context": group_context},
-            create_func=self.app.create.group,
-            list_func=self.app.list.group,
-            fetch_func=self.app.fetch.group,
-            verbosity=verbosity,
-        )
+        # First, figure out which group/log we're working with
+        group = None
+        if group_id is not None or group_name is not None:
+            group = self.fetch_by_name_or_create(
+                resource_type="group",
+                resource_id=group_id,
+                resource_name=group_name,
+                list_params={},
+                create_if_missing=create_group_if_missing,
+                create_params={"note": group_note, "context": group_context},
+                create_func=self.app.create.group,
+                list_func=self.app.list.group,
+                fetch_func=self.app.fetch.group,
+            )
+        if group is None:
+            logger(
+                "No group ID or name provided; will create groups based on found log parameters."
+            )
 
         log = None
         if group is not None:
-            log = self.fetch_by_name_or_create(
-                resource_type="log",
-                resource_id=log_id,
-                resource_name=log_name,
-                list_params={"group_id": group.id},
-                create_if_missing=create_log_if_missing,
-                create_params={
-                    "group_id": group.id,
-                    "note": log_note,
-                    "context": log_context,
-                },
-                create_func=self.app.create.log,
-                list_func=self.app.list.log,
-                fetch_func=self.app.fetch.log,
-                verbosity=verbosity,
-            )
+            if log_id is not None or log_name is not None:
+                log = self.fetch_by_name_or_create(
+                    resource_type="log",
+                    resource_id=log_id,
+                    resource_name=log_name,
+                    list_params={"group_id": group.id},
+                    create_if_missing=create_log_if_missing,
+                    create_params={
+                        "group_id": group.id,
+                        "note": log_note,
+                        "context": log_context,
+                    },
+                    create_func=self.app.create.log,
+                    list_func=self.app.list.log,
+                    fetch_func=self.app.fetch.log,
+                )
+            if log is None:
+                logger(
+                    "No log ID or name provided; will create logs based on found log parameters."
+                )
 
         # Next, we find all the log files in the root directory
         log_param_sets = self.find_local_logs(
             root_dir=root_dir,
             log_file_regexes=log_file_regexes,
             max_depth=max_depth,
         )
         logger(f"Found {len(log_param_sets)} logs in {root_dir}")
 
         # for each log, we check if the log already exists in the group
         uploaded_file_count = 0
         for params in log_param_sets:
+            sync_group = None
+            sync_log = None
+
             log_name_param = params.get("log_name")
             group_name_param = params.get("group_name")
             log_dir_param = params.get("log_dir")
             log_path_param = params.get("log_path")
 
-            if group is None:
+            if log_path_param.endswith(".jsonl"):
+                # if the log_path_param points to a JSONL file, we attempt to parse it as a JSONLLog
+                jsonl_log = JSONLLog()
+                jsonl_log.load_jsonl_file(log_path_param)
+                if jsonl_log.header:
+                    header_log_name = jsonl_log.header.log_name
+                    header_group_name = jsonl_log.header.group_name
+                    jsonl_group = self.fetch_by_name_or_create(
+                        resource_type="group",
+                        resource_name=header_group_name,
+                        create_if_missing=create_group_if_missing,
+                        create_params={
+                            "note": jsonl_log.header.group_note,
+                            "context": jsonl_log.header.group_context,
+                        },
+                        create_func=self.app.create.group,
+                        list_func=self.app.list.group,
+                        fetch_func=self.app.fetch.group,
+                    )
+                    sync_log = self.fetch_by_name_or_create(
+                        resource_type="log",
+                        resource_name=header_log_name,
+                        list_params={"group_id": jsonl_group.id},
+                        create_if_missing=create_log_if_missing,
+                        create_params={
+                            "group_id": jsonl_group.id,
+                            "note": jsonl_log.header.log_note,
+                            "context": jsonl_log.header.log_context,
+                        },
+                        create_func=self.app.create.log,
+                        list_func=self.app.list.log,
+                        fetch_func=self.app.fetch.log,
+                    )
+                    logger(
+                        f"Using JSONL header defined log {sync_log.name} ({sync_log.id}) in group {jsonl_group.name} ({jsonl_group.id})"
+                    )
+
+            if sync_group is None and group is None:
                 groups = self.app.list.group(name=group_name_param).data
                 if len(groups) == 0:
                     logger(f"Creating group {group_name_param}")
                     sync_group = self.app.create.group(
                         name=group_name_param,
                         note=group_note,
                         context=group_context,
                     ).data
                 else:
                     sync_group = groups[0]
-            else:
+            elif sync_group is None and group is not None:
                 sync_group = group
 
-            if log is None:
+            if sync_log is None and log is None:
                 logs = self.app.list.log(
                     group_id=sync_group.id, name=log_name_param
                 ).data
                 if len(logs) == 0:
                     logger(
                         f"Creating log {log_name_param} in group {sync_group.name} ({sync_group.id})"
                     )
@@ -781,15 +1110,15 @@
                         group_id=sync_group.id,
                         name=log_name_param,
                         note=log_note,
                         context=log_context,
                     ).data
                 else:
                     sync_log = logs[0]
-            else:
+            elif sync_log is None and log is not None:
                 sync_log = log
 
             # for each log, we upload the log files
             logger(f"Uploading log files for log {sync_log.name} ({sync_log.id})")
             log_object_key = None
             if log_dir_param is not None:
                 key_replacement = (log_dir_param, "")
@@ -813,52 +1142,14 @@
                         log_object_key = log_object.key
                         break
                 if log_object_key is None:
                     raise Exception(
                         f"Log file {log_file_name} not found in uploaded objects."
                     )
             else:
-                if log_path_param.endswith(".jsonl"):
-                    # if the log_path_param points to a JSONL file, we attempt to parse it as a JSONLLog
-                    jsonl_log = JSONLLog()
-                    jsonl_log.load_jsonl_file(log_path_param)
-                    if jsonl_log.header:
-                        header_log_name = jsonl_log.header.log_name
-                        header_group_name = jsonl_log.header.group_name
-                        jsonl_group = self.fetch_by_name_or_create(
-                            resource_type="group",
-                            resource_name=header_group_name,
-                            create_if_missing=create_group_if_missing,
-                            create_params={
-                                "note": jsonl_log.header.group_note,
-                                "context": jsonl_log.header.group_context,
-                            },
-                            create_func=self.app.create.group,
-                            list_func=self.app.list.group,
-                            fetch_func=self.app.fetch.group,
-                            verbosity=verbosity,
-                        )
-                        sync_log = self.fetch_by_name_or_create(
-                            resource_type="log",
-                            resource_name=header_log_name,
-                            list_params={"group_id": jsonl_group.id},
-                            create_if_missing=create_log_if_missing,
-                            create_params={
-                                "group_id": jsonl_group.id,
-                                "note": jsonl_log.header.log_note,
-                                "context": jsonl_log.header.log_context,
-                            },
-                            create_func=self.app.create.log,
-                            list_func=self.app.list.log,
-                            fetch_func=self.app.fetch.log,
-                            verbosity=verbosity,
-                        )
-                        logger(
-                            f"Using JSONL header defined log {sync_log.name} ({sync_log.id}) in group {jsonl_group.name} ({jsonl_group.id})"
-                        )
                 log_object, _ = self.upload_log_object(
                     log_id=sync_log.id,
                     file_path=log_path_param,
                     part_size=part_size,
                     max_workers=max_workers,
                     skip_if_exists=skip_if_exists,
                     continue_upload=continue_upload,
@@ -891,304 +1182,14 @@
                     logger(
                         f"Ingestion {ingestion.id} created for log {sync_log.name} ({sync_log.id}) for {log_object_key}"
                     )
 
         logger(f"Uploaded {uploaded_file_count} log files")
         return uploaded_file_count
 
-    def upload_log_object_part_from_memory(
-        self,
-        log_id: str,
-        object_key: str,
-        part_number: int,
-        part_data: bytes | str,
-        size: int,
-        max_attempts: int = 3,
-        backoff_factor: float = 5.0,
-        connect_timeout: int = 60,
-        read_timeout: int = 600,
-    ):
-        """
-        Upload a part of a file to a log object.
-
-        Args:
-            log_id (str): The log id to upload the object part to.
-            object_key (str): The key of the object to upload the part to.
-            part_number (int): The part number of the object part.
-            part_data (bytes | str): The data to upload.
-            size (int): The size of the part to upload.
-            max_attempts (int, optional): The maximum number of attempts to upload the part. Defaults to 3.
-            backoff_factor (float, optional): The backoff factor for retrying the upload. Defaults to 5.0.
-            connect_timeout (int, optional): The connection timeout for the upload. Defaults to 60.
-            read_timeout (int, optional): The read timeout for the upload. Defaults to 600.
-
-        Raises:
-            Exception: If the upload fails.
-
-        Returns:
-            ObjectPart: The uploaded object part.
-        """
-        log_id = str(log_id)
-        object_part = self.app.create.log_object_part(
-            log_id=log_id,
-            object_key=object_key,
-            size=size,
-            part_number=part_number,
-        ).data
-        upload_object_data_url = object_part.presigned_url
-
-        attempt_count = 0
-        response = None
-        for attempt_count in range(1, max_attempts + 1):
-            if attempt_count > 1:
-                self.app.debug(
-                    f"Retrying upload of part {part_number} of object {object_key} in log {log_id} (attempt {attempt_count}/{max_attempts})."
-                )
-            try:
-                response = requests.put(
-                    upload_object_data_url,
-                    data=part_data,
-                    timeout=(connect_timeout, read_timeout),
-                )
-                break
-            except Exception as e:
-                self.app.debug(
-                    f"Error while uploading part {part_number} of object {object_key} in log {log_id} (attempt {attempt_count}/{max_attempts}): {e}"
-                )
-                time.sleep(backoff_factor * (2 ** (attempt_count - 1)))
-                continue
-
-        if response is None:
-            raise Exception(
-                f"Failed to upload part {part_number} of object {object_key} in log {log_id} after {max_attempts} attempts."
-            )
-
-        if response.status_code != 200:
-            raise Exception(f"Error while uploading object part: {response.text}")
-
-        return self.app.fetch.log_object_part(
-            log_id=log_id,
-            object_key=object_key,
-            part_number=part_number,
-        ).data
-
-    def upload_log_object_from_memory(
-        self,
-        log_id: str,
-        file_like: io.BytesIO | io.StringIO,
-        object_key: str,
-        key_replacement: tuple[str, str] = None,
-        key_prefix: str = None,
-        part_size: int = 100 * 1024 * 1024,
-        max_workers: int | None = 8,
-        skip_if_exists: bool = False,
-        continue_upload: bool = True,
-        skip_if_complete: bool = False,
-        overwrite: bool = False,
-    ) -> tuple["Object", list["ObjectPart"]]:
-        """
-        Upload a file-like object to a log.
-
-        The file is uploaded as a log object, meaning it is associated with a single log given by log_id.
-        The file is split into parts of size part_size, which are uploaded in parallel using a maximum of max_workers workers.
-        Note that larger values for part_size and max_workers will generally result in faster uploads, but may also result in higher memory usage.
-
-        If skip_if_exists is set to True, the upload will be skipped if the object already exists.
-        If continue_upload is set to True, any existing parts of the object will be skipped and the upload will continue from where it left off.
-        If continue_upload is set to True and skip_if_complete is set to True, the upload will be skipped if the object is already complete.
-        If overwrite is set to True, any existing object with the same key will be deleted before the upload.
-
-        Args:
-            log_id (str): The log id to upload the object to.
-            file_like (io.BytesIO | io.StringIO): The file-like object to upload.
-            object_key (str): The key to use for the object.
-            key_replacement (tuple[str, str], optional): A tuple of strings to replace in the object key. Defaults to None.
-            key_prefix (str, optional): A prefix to add to the object key. Defaults to None.
-            part_size (int, optional): The size of each part to upload. Defaults to 100 * 1024 * 1024.
-            max_workers (int, optional): The maximum number of workers to use for parallel uploads. Defaults to 8.
-            skip_if_exists (bool, optional): Whether to skip the upload if the object already exists. Defaults to False.
-            continue_upload (bool, optional): Whether to continue an existing upload. Defaults to True.
-            skip_if_complete (bool, optional): Whether to skip the continued upload if the object is already complete. Defaults to False.
-            overwrite (bool, optional): Whether to overwrite the object if it already exists. Defaults to False.
-
-        Raises:
-            ConflictException: If existing resources conflict with the upload.
-
-        Returns:
-            tuple["Object", list["ObjectPart"]]: The uploaded object and its parts.
-        """
-
-        # First, create/re-create/fetch/etc. the log object
-        log_id = str(log_id)
-        if key_replacement is not None:
-            object_key = object_key.replace(*key_replacement)
-        if key_prefix is not None:
-            object_key = os.path.join(key_prefix, object_key)
-        if object_key.startswith("/"):
-            object_key = object_key[1:]
-
-        try:
-            log_object = self.app.create.log_object(
-                log_id=log_id,
-                key=object_key,
-            ).data
-        except ConflictException as e:
-            if skip_if_exists:
-                self.app.debug(
-                    f"Skipping upload of object {object_key} in log {log_id}."
-                )
-                log_object = self.app.fetch.log_object(
-                    log_id=log_id, object_key=object_key
-                ).data
-                return log_object, []
-
-            if continue_upload:
-                self.app.debug(
-                    f"Continuing upload of object {object_key} in log {log_id}."
-                )
-                log_object = self.app.fetch.log_object(
-                    log_id=log_id, object_key=object_key
-                ).data
-                if log_object.upload_state == "complete":
-                    if skip_if_complete:
-                        self.app.debug(
-                            f"Skipping complete upload of object {object_key} in log {log_id}."
-                        )
-                        return log_object, []
-                    else:
-                        raise ConflictException(
-                            f"Can't continue upload: Upload of Object {object_key} in log {log_id} is already complete."
-                        )
-            elif overwrite:
-                self.app.debug(f"Overwriting object {object_key} in log {log_id}.")
-                self.app.delete.log_object(log_id=log_id, object_key=object_key)
-                log_object = self.app.create.log_object(
-                    log_id=log_id,
-                    key=object_key,
-                ).data
-            else:
-                raise e
-
-        # Then, figure out which parts we need to upload
-        if isinstance(file_like, io.StringIO):
-            object_size = len(file_like.getvalue())
-        elif isinstance(file_like, io.BytesIO):
-            object_size = file_like.getbuffer().nbytes
-        else:
-            raise TypeError(
-                "file_like must be an instance of io.BytesIO or io.StringIO"
-            )
-        number_of_parts = object_size // part_size + 1
-        log_object_parts: List[ObjectPart] = []
-
-        parts_res = self.app.list.log_object_part(log_id=log_id, object_key=object_key)
-        log_object_parts += parts_res.data
-        while parts_res.is_truncated:
-            parts_res = self.app.list.log_object_part(
-                log_id=log_id,
-                object_key=object_key,
-                part_number_marker=parts_res.next_part_number_marker,
-            )
-            log_object_parts += parts_res.data
-        self.app.debug(
-            f"Found {len(log_object_parts)} existing parts for object {object_key} in log {log_id}."
-        )
-        if continue_upload is False:
-            if len(log_object_parts) > 0:
-                raise ConflictException(
-                    f"Object {object_key} in log {log_id} already has {len(log_object_parts)} parts."
-                    "Set continue_upload to True to continue the upload or overwrite to start over."
-                )
-        else:
-            self.app.debug(
-                f"Found {len(log_object_parts)} existing parts for object {object_key} in log {log_id}."
-            )
-        log_object_parts.sort(key=lambda part: part.part_number)
-
-        # Validate existing parts sizes
-        for idx, part in enumerate(log_object_parts):
-            if part.part_number == number_of_parts:
-                # the last part is allowed to be smaller than part_size
-                continue
-            if part.size == 0:
-                # the part exists, but it has no data, so we'll overwrite it anyways
-                continue
-            if part.size != part_size:
-                raise ConflictException(
-                    f"Part {part.part_number} of object {object_key} in log {log_id} has an unexpected size {part.size}."
-                    f"All parts except for the last part need to be the same size as the given part_size {part_size}."
-                    f"Either overwrite the object to start over or change the part_size to match existing parts."
-                )
-
-        def should_skip_part(part_number):
-            existing_part = next(
-                (part for part in log_object_parts if part.part_number == part_number),
-                None,
-            )
-            if existing_part is not None:
-                if existing_part.size == 0:
-                    self.app.debug(
-                        f"Overwriting empty part {part_number} of object {object_key} in log {log_id}."
-                    )
-                else:
-                    self.app.debug(
-                        f"Skipping existing part {part_number} of object {object_key} in log {log_id}."
-                    )
-                    return True
-            return False
-
-        # Upload the parts (in parallel if max_workers is set)
-        if max_workers is not None:
-            futures = []
-            with ThreadPoolExecutor(max_workers=max_workers) as executor:
-                for idx in range(0, number_of_parts):
-                    offset = idx * part_size
-                    file_like.seek(offset)
-                    size = min(part_size, object_size - offset)
-                    part_number = idx + 1
-                    if should_skip_part(part_number):
-                        continue
-                    futures.append(
-                        executor.submit(
-                            self.upload_log_object_part_from_memory,
-                            log_id=log_id,
-                            object_key=object_key,
-                            part_number=part_number,
-                            part_data=file_like.read(size),
-                            size=size,
-                        )
-                    )
-
-                for future in futures:
-                    log_object_parts.append(future.result())
-        else:
-            for idx in range(0, number_of_parts):
-                offset = idx * part_size
-                file_like.seek(offset)
-                size = min(part_size, object_size - offset)
-                part_number = idx + 1
-                if should_skip_part(part_number):
-                    continue
-                log_object_parts.append(
-                    self.upload_log_object_part_from_memory(
-                        log_id=log_id,
-                        object_key=object_key,
-                        part_number=part_number,
-                        part_data=file_like.read(size),
-                        size=size,
-                    )
-                )
-
-        # Finally, mark the object as complete to finish the upload
-        log_object = self.app.update.log_object(
-            log_id=log_id, object_key=object_key, data={"upload_state": "complete"}
-        ).data
-
-        return log_object, log_object_parts
-
     # Downloading
 
     def load_auxiliary_data_image(self, source: Record | dict):
         if isinstance(source, Record):
             auxiliary_data = source.get_auxiliary_data()
         else:
             auxiliary_data = source
```

### Comparing `LogQS-1.0.8/lqs/common/config.py` & `LogQS-1.0.9/lqs/common/config.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/common/exceptions.py` & `LogQS-1.0.9/lqs/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/common/facade.py` & `LogQS-1.0.9/lqs/common/facade.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/common/utils.py` & `LogQS-1.0.9/lqs/common/utils.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/admin/create.py` & `LogQS-1.0.9/lqs/interface/admin/create.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/admin/models/command.py` & `LogQS-1.0.9/lqs/interface/admin/models/command.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/base/create.py` & `LogQS-1.0.9/lqs/interface/base/create.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/base/delete.py` & `LogQS-1.0.9/lqs/interface/base/delete.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/base/fetch.py` & `LogQS-1.0.9/lqs/interface/base/fetch.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/base/list.py` & `LogQS-1.0.9/lqs/interface/base/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         disabled: Optional[bool] = None,
         default: Optional[bool] = None,
         managed: Optional[bool] = None,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
-        order: Optional[str] = "timestamp",
+        order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
         updated_by_null: Optional[bool] = None,
         deleted_by_null: Optional[bool] = None,
         updated_at_null: Optional[bool] = None,
```

### Comparing `LogQS-1.0.8/lqs/interface/base/models/__common__.py` & `LogQS-1.0.9/lqs/interface/base/models/__common__.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 
 
 class PaginationModel(BaseModel):
     offset: int
     limit: int
     order: str
     sort: str
-    count: int
+    count: Optional[int]
 
 
 class PatchOperation(BaseModel):
     op: str
     path: str
     value: Optional[Union[str, int, float, bool, dict, list, None]]
```

### Comparing `LogQS-1.0.8/lqs/interface/base/models/api_key.py` & `LogQS-1.0.9/lqs/interface/base/models/api_key.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/base/models/role.py` & `LogQS-1.0.9/lqs/interface/base/models/role.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/base/models/user.py` & `LogQS-1.0.9/lqs/interface/base/models/user.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/base/update.py` & `LogQS-1.0.9/lqs/interface/base/update.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/create.py` & `LogQS-1.0.9/lqs/interface/core/create.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/delete.py` & `LogQS-1.0.9/lqs/interface/core/delete.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/fetch.py` & `LogQS-1.0.9/lqs/interface/core/fetch.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/list.py` & `LogQS-1.0.9/lqs/interface/core/list.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 class ListInterface(BaseListInterface):
     @abstractmethod
     def _digestion(self, **kwargs) -> models.DigestionListResponse:
         pass
 
     def digestion(
         self,
+        id: Optional[UUID] = None,
         group_id: Optional[UUID] = None,
         log_id: Optional[UUID] = None,
         workflow_id: Optional[UUID] = None,
         workflow_id_null: Optional[bool] = None,
         state: Optional[str] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         progress_null: Optional[bool] = None,
         progress_gte: Optional[float] = None,
         progress_lte: Optional[float] = None,
         error_like: Optional[str] = None,
         note_like: Optional[str] = None,
         context_filter: Optional[str] = None,
         workflow_context_filter: Optional[str] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -46,28 +48,30 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists digestions.
         """
         return self._digestion(
+            id=id,
             group_id=group_id,
             log_id=log_id,
             workflow_id=workflow_id,
             workflow_id_null=workflow_id_null,
             state=state,
             name=name,
             name_like=name_like,
             progress_null=progress_null,
             progress_gte=progress_gte,
             progress_lte=progress_lte,
             error_like=error_like,
             note_like=note_like,
             context_filter=context_filter,
             workflow_context_filter=workflow_context_filter,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -88,21 +92,23 @@
 
     @abstractmethod
     def _digestion_part(self, **kwargs) -> models.DigestionPartListResponse:
         pass
 
     def digestion_part(
         self,
+        id: Optional[UUID] = None,
         group_id: Optional[UUID] = None,
         log_id: Optional[UUID] = None,
         sequence: Optional[int] = None,
         digestion_id: Optional[UUID] = None,
         workflow_id: Optional[UUID] = None,
         workflow_id_null: Optional[bool] = None,
         state: Optional[str] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -117,21 +123,23 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists digestion parts.
         """
         return self._digestion_part(
+            id=id,
             group_id=group_id,
             log_id=log_id,
             sequence=sequence,
             digestion_id=digestion_id,
             workflow_id=workflow_id,
             workflow_id_null=workflow_id_null,
             state=state,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -152,24 +160,26 @@
 
     @abstractmethod
     def _digestion_topic(self, **kwargs) -> models.DigestionTopicListResponse:
         pass
 
     def digestion_topic(
         self,
-        digestion_id: UUID,  # TODO: should this still be a required parameter with group and log id changes?
+        id: Optional[UUID] = None,
+        digestion_id: Optional[UUID] = None,
         group_id: Optional[UUID] = None,
         log_id: Optional[UUID] = None,
         topic_id: Optional[UUID] = None,
         start_time_null: Optional[bool] = None,
         start_time_gte: Optional[int] = None,
         start_time_lte: Optional[int] = None,
         end_time_null: Optional[bool] = None,
         end_time_gte: Optional[int] = None,
         end_time_lte: Optional[int] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -184,24 +194,26 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists digestion topics.
         """
         return self._digestion_topic(
+            id=id,
             group_id=group_id,
             log_id=log_id,
             digestion_id=digestion_id,
             topic_id=topic_id,
             start_time_null=start_time_null,
             start_time_gte=start_time_gte,
             start_time_lte=start_time_lte,
             end_time_null=end_time_null,
             end_time_gte=end_time_gte,
             end_time_lte=end_time_lte,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -222,18 +234,20 @@
 
     @abstractmethod
     def _group(self, **kwargs) -> models.GroupListResponse:
         pass
 
     def group(
         self,
+        id: Optional[UUID] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         default_workflow_id: Optional[UUID] = None,
         default_workflow_id_null: Optional[bool] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -248,18 +262,20 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists groups.
         """
         return self._group(
+            id=id,
             name=name,
             name_like=name_like,
             default_workflow_id=default_workflow_id,
             default_workflow_id_null=default_workflow_id_null,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -280,24 +296,26 @@
 
     @abstractmethod
     def _hook(self, **kwargs) -> models.HookListResponse:
         pass
 
     def hook(
         self,
+        id: Optional[UUID] = None,
         workflow_id: Optional[UUID] = None,
         trigger_process: Optional[str] = None,
         trigger_state: Optional[str] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         note_like: Optional[str] = None,
         managed: Optional[bool] = None,
         disabled: Optional[bool] = None,
         uri: Optional[str] = None,
         uri_like: Optional[str] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -312,24 +330,26 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists hooks.
         """
         return self._hook(
+            id=id,
             workflow_id=workflow_id,
             trigger_process=trigger_process,
             trigger_state=trigger_state,
             name=name,
             name_like=name_like,
             note_like=note_like,
             uri=uri,
             uri_like=uri_like,
             managed=managed,
             disabled=disabled,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -350,14 +370,15 @@
 
     @abstractmethod
     def _ingestion(self, **kwargs) -> models.IngestionListResponse:
         pass
 
     def ingestion(
         self,
+        id: Optional[UUID] = None,
         group_id: Optional[UUID] = None,
         log_id: Optional[UUID] = None,
         object_store_id: Optional[UUID] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         object_key: Optional[str] = None,
         object_key_like: Optional[str] = None,
@@ -367,14 +388,15 @@
         state: Optional[str] = None,
         progress_null: Optional[bool] = None,
         progress_gte: Optional[float] = None,
         progress_lte: Optional[float] = None,
         error_like: Optional[str] = None,
         note_like: Optional[str] = None,
         context_filter: Optional[str] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -389,14 +411,15 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists ingestions.
         """
         return self._ingestion(
+            id=id,
             group_id=group_id,
             log_id=log_id,
             object_store_id=object_store_id,
             name=name,
             name_like=name_like,
             object_key=object_key,
             object_key_like=object_key_like,
@@ -406,14 +429,15 @@
             state=state,
             progress_null=progress_null,
             progress_gte=progress_gte,
             progress_lte=progress_lte,
             error_like=error_like,
             note_like=note_like,
             context_filter=context_filter,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -434,22 +458,24 @@
 
     @abstractmethod
     def _ingestion_part(self, **kwargs) -> models.IngestionPartListResponse:
         pass
 
     def ingestion_part(
         self,
+        id: Optional[UUID] = None,
         group_id: Optional[UUID] = None,
         log_id: Optional[UUID] = None,
         ingestion_id: Optional[UUID] = None,
         sequence: Optional[int] = None,
         source: Optional[str] = None,
         workflow_id: Optional[UUID] = None,
         workflow_id_null: Optional[bool] = None,
         state: Optional[str] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -464,22 +490,24 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists ingestion parts.
         """
         return self._ingestion_part(
+            id=id,
             group_id=group_id,
             log_id=log_id,
             sequence=sequence,
             ingestion_id=ingestion_id,
             workflow_id=workflow_id,
             workflow_id_null=workflow_id_null,
             state=state,
             source=source,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -500,17 +528,19 @@
 
     @abstractmethod
     def _label(self, **kwargs) -> models.LabelListResponse:
         pass
 
     def label(
         self,
+        id: Optional[UUID] = None,
         value: Optional[str] = None,
         value_like: Optional[str] = None,
         note_like: Optional[str] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -525,17 +555,19 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists labels.
         """
         return self._label(
+            id=id,
             value=value,
             value_like=value_like,
             note_like=note_like,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -556,14 +588,15 @@
 
     @abstractmethod
     def _log(self, **kwargs) -> models.LogListResponse:
         pass
 
     def log(
         self,
+        id: Optional[UUID] = None,
         group_id: Optional[UUID] = None,
         default_workflow_id: Optional[UUID] = None,
         default_workflow_id_null: Optional[bool] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         locked: Optional[bool] = None,
         note_like: Optional[str] = None,
@@ -581,14 +614,15 @@
         record_size_lte: Optional[int] = None,
         record_count_gte: Optional[int] = None,
         record_count_lte: Optional[int] = None,
         object_size_gte: Optional[int] = None,
         object_size_lte: Optional[int] = None,
         object_count_gte: Optional[int] = None,
         object_count_lte: Optional[int] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -603,14 +637,15 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists logs.
         """
         return self._log(
+            id=id,
             group_id=group_id,
             default_workflow_id=default_workflow_id,
             default_workflow_id_null=default_workflow_id_null,
             name=name,
             name_like=name_like,
             locked=locked,
             note_like=note_like,
@@ -628,14 +663,15 @@
             record_size_lte=record_size_lte,
             record_count_gte=record_count_gte,
             record_count_lte=record_count_lte,
             object_size_gte=object_size_gte,
             object_size_lte=object_size_lte,
             object_count_gte=object_count_gte,
             object_count_lte=object_count_lte,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -764,21 +800,23 @@
 
     @abstractmethod
     def _object_store(self, **kwargs) -> models.ObjectStoreListResponse:
         pass
 
     def object_store(
         self,
+        id: Optional[UUID] = None,
         bucket_name: Optional[str] = None,
         access_key_id: Optional[str] = None,
         region_name: Optional[str] = None,
         endpoint_url: Optional[str] = None,
         note: Optional[str] = None,
         note_like: Optional[str] = None,
         disabled: Optional[bool] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -793,21 +831,23 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists object stores.
         """
         return self._object_store(
+            id=id,
             bucket_name=bucket_name,
             access_key_id=access_key_id,
             region_name=region_name,
             endpoint_url=endpoint_url,
             note=note,
             note_like=note_like,
             disabled=disabled,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -828,25 +868,27 @@
 
     @abstractmethod
     def _query(self, **kwargs) -> models.QueryListResponse:
         pass
 
     def query(
         self,
+        id: Optional[UUID] = None,
         log_id: Optional[UUID] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         note_like: Optional[str] = None,
         statement: Optional[str] = None,
         statement_like: Optional[str] = None,
         workflow_id: Optional[UUID] = None,
         workflow_id_null: Optional[bool] = None,
         workflow_context_filter: Optional[str] = None,
         state: Optional[str] = None,
         context_filter: Optional[str] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -861,25 +903,27 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists queries.
         """
         return self._query(
+            id=id,
             log_id=log_id,
             name=name,
             name_like=name_like,
             note_like=note_like,
             statement=statement,
             statement_like=statement_like,
             workflow_id=workflow_id,
             workflow_id_null=workflow_id_null,
             workflow_context_filter=workflow_context_filter,
             state=state,
             context_filter=context_filter,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -901,14 +945,15 @@
     @abstractmethod
     def _record(self, **kwargs) -> models.RecordListResponse:
         pass
 
     def record(
         self,
         topic_id: UUID,
+        timestamp: Optional[int] = None,
         log_id: Optional[UUID] = None,
         ingestion_id: Optional[UUID] = None,
         workflow_id: Optional[UUID] = None,
         workflow_id_null: Optional[bool] = None,
         state: Optional[str] = None,
         error_like: Optional[str] = None,
         note_like: Optional[str] = None,
@@ -928,14 +973,15 @@
         chunk_compression: Optional[str] = None,
         chunk_offset_gte: Optional[int] = None,
         chunk_offset_lte: Optional[int] = None,
         chunk_length_gte: Optional[int] = None,
         chunk_length_lte: Optional[int] = None,
         include_auxiliary_data: Optional[bool] = False,
         include_raw_data: Optional[bool] = False,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "timestamp",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -951,14 +997,15 @@
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists records.
         """
         return self._record(
             topic_id=topic_id,
+            timestamp=timestamp,
             log_id=log_id,
             ingestion_id=ingestion_id,
             workflow_id=workflow_id,
             workflow_id_null=workflow_id_null,
             state=state,
             error_like=error_like,
             note_like=note_like,
@@ -978,14 +1025,15 @@
             chunk_compression=chunk_compression,
             chunk_offset_gte=chunk_offset_gte,
             chunk_offset_lte=chunk_offset_lte,
             chunk_length_gte=chunk_length_gte,
             chunk_length_lte=chunk_length_lte,
             include_auxiliary_data=include_auxiliary_data,
             include_raw_data=include_raw_data,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -1006,26 +1054,28 @@
 
     @abstractmethod
     def _tag(self, **kwargs) -> models.TagListResponse:
         pass
 
     def tag(
         self,
+        id: Optional[UUID] = None,
         log_id: Optional[UUID] = None,
         label_id: Optional[UUID] = None,
         topic_id: Optional[UUID] = None,
         note: Optional[str] = None,
         note_like: Optional[str] = None,
         context_filter: Optional[str] = None,
         start_time_null: Optional[bool] = None,
         start_time_gte: Optional[int] = None,
         start_time_lte: Optional[int] = None,
         end_time_null: Optional[bool] = None,
         end_time_gte: Optional[int] = None,
         end_time_lte: Optional[int] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -1040,26 +1090,28 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists tags.
         """
         return self._tag(
+            id=id,
             label_id=label_id,
             log_id=log_id,
             topic_id=topic_id,
             note=note,
             note_like=note_like,
             context_filter=context_filter,
             start_time_null=start_time_null,
             start_time_gte=start_time_gte,
             start_time_lte=start_time_lte,
             end_time_null=end_time_null,
             end_time_gte=end_time_gte,
             end_time_lte=end_time_lte,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -1080,14 +1132,15 @@
 
     @abstractmethod
     def _topic(self, **kwargs) -> models.TopicListResponse:
         pass
 
     def topic(
         self,
+        id: Optional[UUID] = None,
         log_id: Optional[UUID] = None,
         group_id: Optional[UUID] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         associated_topic_id: Optional[UUID] = None,
         latched: Optional[bool] = None,
         strict: Optional[bool] = None,
@@ -1105,14 +1158,15 @@
         record_count_lte: Optional[int] = None,
         type_name: Optional[str] = None,
         type_name_like: Optional[str] = None,
         type_encoding: Optional[models.TypeEncoding] = None,
         type_data: Optional[str] = None,
         type_data_like: Optional[str] = None,
         type_schema_filter: Optional[str] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -1127,14 +1181,15 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists topics.
         """
         return self._topic(
+            id=id,
             group_id=group_id,
             name=name,
             name_like=name_like,
             log_id=log_id,
             associated_topic_id=associated_topic_id,
             latched=latched,
             strict=strict,
@@ -1152,14 +1207,15 @@
             record_count_lte=record_count_lte,
             type_name=type_name,
             type_name_like=type_name_like,
             type_encoding=type_encoding,
             type_data=type_data,
             type_data_like=type_data_like,
             type_schema_filter=type_schema_filter,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -1180,20 +1236,22 @@
 
     @abstractmethod
     def _workflow(self, **kwargs) -> models.WorkflowListResponse:
         pass
 
     def workflow(
         self,
+        id: Optional[UUID] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         default: Optional[bool] = None,
         disabled: Optional[bool] = None,
         managed: Optional[bool] = None,
         context_schema_filter: Optional[str] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -1208,20 +1266,22 @@
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         """
         Lists workflows.
         """
         return self._workflow(
+            id=id,
             name=name,
             name_like=name_like,
             default=default,
             disabled=disabled,
             managed=managed,
             context_schema_filter=context_schema_filter,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
```

### Comparing `LogQS-1.0.8/lqs/interface/core/models/__common__.py` & `LogQS-1.0.9/lqs/interface/core/models/__common__.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/__init__.py` & `LogQS-1.0.9/lqs/interface/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/digestion.py` & `LogQS-1.0.9/lqs/interface/core/models/digestion.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/digestion_part.py` & `LogQS-1.0.9/lqs/interface/core/models/digestion_part.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/digestion_topic.py` & `LogQS-1.0.9/lqs/interface/core/models/digestion_topic.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/group.py` & `LogQS-1.0.9/lqs/interface/core/models/group.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/hook.py` & `LogQS-1.0.9/lqs/interface/core/models/hook.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/ingestion.py` & `LogQS-1.0.9/lqs/interface/core/models/ingestion.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/ingestion_part.py` & `LogQS-1.0.9/lqs/interface/core/models/ingestion_part.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/label.py` & `LogQS-1.0.9/lqs/interface/core/models/label.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/log.py` & `LogQS-1.0.9/lqs/interface/core/models/log.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/object.py` & `LogQS-1.0.9/lqs/interface/core/models/object.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/object_store.py` & `LogQS-1.0.9/lqs/interface/core/models/object_store.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/query.py` & `LogQS-1.0.9/lqs/interface/core/models/query.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/record.py` & `LogQS-1.0.9/lqs/interface/core/models/record.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/tag.py` & `LogQS-1.0.9/lqs/interface/core/models/tag.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/topic.py` & `LogQS-1.0.9/lqs/interface/core/models/topic.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/models/workflow.py` & `LogQS-1.0.9/lqs/interface/core/models/workflow.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/core/update.py` & `LogQS-1.0.9/lqs/interface/core/update.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/dsm/create.py` & `LogQS-1.0.9/lqs/interface/dsm/create.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/dsm/delete.py` & `LogQS-1.0.9/lqs/interface/dsm/delete.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/dsm/fetch.py` & `LogQS-1.0.9/lqs/interface/dsm/fetch.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/dsm/list.py` & `LogQS-1.0.9/lqs/interface/dsm/list.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 class ListInterface(BaseListInterface):
     @abstractmethod
     def _announcement(self, **kwargs) -> models.AnnouncementListResponse:
         pass
 
     def announcement(
         self,
+        id: Optional[UUID] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         datastore_id: Optional[UUID] = None,
         subject: Optional[str] = None,
         subject_like: Optional[str] = None,
@@ -45,14 +47,16 @@
         updated_at_lte: Optional[datetime] = None,
         deleted_at_lte: Optional[datetime] = None,
         created_at_gte: Optional[datetime] = None,
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         return self._announcement(
+            id=id,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             datastore_id=datastore_id,
             subject=subject,
             subject_like=subject_like,
@@ -89,14 +93,16 @@
 
     @abstractmethod
     def _comment(self, **kwargs) -> models.CommentListResponse:
         pass
 
     def comment(
         self,
+        id: Optional[UUID] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         user_id: Optional[UUID] = None,
         datastore_id: Optional[UUID] = None,
         resource_type: Optional[str] = None,
@@ -119,14 +125,16 @@
         updated_at_lte: Optional[datetime] = None,
         deleted_at_lte: Optional[datetime] = None,
         created_at_gte: Optional[datetime] = None,
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         return self._comment(
+            id=id,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             user_id=user_id,
             datastore_id=datastore_id,
             resource_type=resource_type,
@@ -158,14 +166,16 @@
 
     @abstractmethod
     def _configuration(self, **kwargs) -> models.ConfigurationListResponse:
         pass
 
     def configuration(
         self,
+        id: Optional[UUID] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         value: Optional[dict] = None,
         name: Optional[str] = None,
         name_like: Optional[str] = None,
@@ -184,14 +194,16 @@
         updated_at_lte: Optional[datetime] = None,
         deleted_at_lte: Optional[datetime] = None,
         created_at_gte: Optional[datetime] = None,
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         return self._configuration(
+            id=id,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             value=value,
             name=name,
             name_like=name_like,
@@ -219,14 +231,16 @@
 
     @abstractmethod
     def _datastore(self, **kwargs) -> models.DataStoreListResponse:
         pass
 
     def datastore(
         self,
+        id: Optional[UUID] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         name: Optional[str] = None,
         name_like: Optional[str] = None,
         owner_id: Optional[UUID] = None,
@@ -241,14 +255,16 @@
         updated_at_lte: Optional[datetime] = None,
         deleted_at_lte: Optional[datetime] = None,
         created_at_gte: Optional[datetime] = None,
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         return self._datastore(
+            id=id,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             name=name,
             name_like=name_like,
             owner_id=owner_id,
@@ -274,14 +290,16 @@
     def _datastore_association(
         self, **kwargs
     ) -> models.DataStoreAssociationListResponse:
         pass
 
     def datastore_association(
         self,
+        id: Optional[UUID] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         user_id: Optional[UUID] = None,
         datastore_id: Optional[UUID] = None,
         datastore_user_id: Optional[UUID] = None,
@@ -298,14 +316,16 @@
         updated_at_lte: Optional[datetime] = None,
         deleted_at_lte: Optional[datetime] = None,
         created_at_gte: Optional[datetime] = None,
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         return self._datastore_association(
+            id=id,
+            include_count=include_count,
             user_id=user_id,
             datastore_id=datastore_id,
             datastore_user_id=datastore_user_id,
             manager=manager,
             disabled=disabled,
             offset=offset,
             limit=limit,
@@ -331,15 +351,16 @@
 
     @abstractmethod
     def _usage_tick(self, **kwargs) -> models.UsageTickListResponse:
         pass
 
     def usage_tick(
         self,
-        datastore_id: UUID,
+        timestamp: Optional[int] = None,
+        datastore_id: Optional[UUID] = None,
         timestamp_gt: Optional[int] = None,
         timestamp_lt: Optional[int] = None,
         timestamp_gte: Optional[int] = None,
         timestamp_lte: Optional[int] = None,
         log_count_gt: Optional[int] = None,
         log_count_lt: Optional[int] = None,
         log_count_gte: Optional[int] = None,
@@ -360,17 +381,18 @@
         object_size_lt: Optional[int] = None,
         object_size_gte: Optional[int] = None,
         object_size_lte: Optional[int] = None,
         transfer_size_gt: Optional[int] = None,
         transfer_size_lt: Optional[int] = None,
         transfer_size_gte: Optional[int] = None,
         transfer_size_lte: Optional[int] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
-        order: Optional[str] = "created_at",
+        order: Optional[str] = "timestamp",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
         updated_by_null: Optional[bool] = None,
         deleted_by_null: Optional[bool] = None,
         updated_at_null: Optional[bool] = None,
@@ -379,14 +401,15 @@
         updated_at_lte: Optional[datetime] = None,
         deleted_at_lte: Optional[datetime] = None,
         created_at_gte: Optional[datetime] = None,
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         return self._usage_tick(
+            timestamp=timestamp,
             datastore_id=datastore_id,
             timestamp_gt=timestamp_gt,
             timestamp_lt=timestamp_lt,
             timestamp_gte=timestamp_gte,
             timestamp_lte=timestamp_lte,
             log_count_gt=log_count_gt,
             log_count_lt=log_count_lt,
@@ -408,14 +431,15 @@
             object_size_lt=object_size_lt,
             object_size_gte=object_size_gte,
             object_size_lte=object_size_lte,
             transfer_size_gt=transfer_size_gt,
             transfer_size_lt=transfer_size_lt,
             transfer_size_gte=transfer_size_gte,
             transfer_size_lte=transfer_size_lte,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
```

### Comparing `LogQS-1.0.8/lqs/interface/dsm/models/announcement.py` & `LogQS-1.0.9/lqs/interface/dsm/models/announcement.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/dsm/models/comment.py` & `LogQS-1.0.9/lqs/interface/dsm/models/comment.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/dsm/models/configuration.py` & `LogQS-1.0.9/lqs/interface/dsm/models/configuration.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/dsm/models/datastore.py` & `LogQS-1.0.9/lqs/interface/dsm/models/datastore.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/dsm/models/datastore_association.py` & `LogQS-1.0.9/lqs/interface/dsm/models/datastore_association.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/dsm/models/usage_tick.py` & `LogQS-1.0.9/lqs/interface/dsm/models/usage_tick.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/dsm/update.py` & `LogQS-1.0.9/lqs/interface/dsm/update.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/pjm/create.py` & `LogQS-1.0.9/lqs/interface/pjm/create.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/pjm/fetch.py` & `LogQS-1.0.9/lqs/interface/pjm/fetch.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/pjm/list.py` & `LogQS-1.0.9/lqs/interface/pjm/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 class ListInterface(ABC):
     @abstractmethod
     def _event(self, **kwargs) -> models.EventListResponse:
         pass
 
     def event(
         self,
+        id: Optional[UUID] = None,
         previous_state: Optional[str] = None,
         current_state: Optional[str] = None,
         process_type: Optional[str] = None,
         resource_id: Optional[UUID] = None,
         workflow_id: Optional[UUID] = None,
         hook_id: Optional[UUID] = None,
         datastore_id: Optional[UUID] = None,
         datastore_endpoint: Optional[str] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -36,22 +38,24 @@
         updated_at_lte: Optional[datetime] = None,
         deleted_at_lte: Optional[datetime] = None,
         created_at_gte: Optional[datetime] = None,
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         return self._event(
+            id=id,
             previous_state=previous_state,
             current_state=current_state,
             process_type=process_type,
             resource_id=resource_id,
             workflow_id=workflow_id,
             hook_id=hook_id,
             datastore_id=datastore_id,
             datastore_endpoint=datastore_endpoint,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
@@ -72,20 +76,22 @@
 
     @abstractmethod
     def _job(self, **kwargs) -> models.JobListResponse:
         pass
 
     def job(
         self,
+        id: Optional[UUID] = None,
         event_id: Optional[UUID] = None,
         process_type: Optional[str] = None,
         resource_id: Optional[UUID] = None,
         datastore_id: Optional[UUID] = None,
         datastore_endpoint: Optional[str] = None,
         state: Optional[str] = None,
+        include_count: Optional[bool] = True,
         offset: Optional[int] = 0,
         limit: Optional[int] = 100,
         order: Optional[str] = "created_at",
         sort: Optional[str] = "ASC",
         created_by: Optional[UUID] = None,
         updated_by: Optional[UUID] = None,
         deleted_by: Optional[UUID] = None,
@@ -97,20 +103,22 @@
         updated_at_lte: Optional[datetime] = None,
         deleted_at_lte: Optional[datetime] = None,
         created_at_gte: Optional[datetime] = None,
         updated_at_gte: Optional[datetime] = None,
         deleted_at_gte: Optional[datetime] = None,
     ):
         return self._job(
+            id=id,
             event_id=event_id,
             process_type=process_type,
             resource_id=resource_id,
             datastore_id=datastore_id,
             datastore_endpoint=datastore_endpoint,
             state=state,
+            include_count=include_count,
             offset=offset,
             limit=limit,
             order=order,
             sort=sort,
             created_by=created_by,
             updated_by=updated_by,
             deleted_by=deleted_by,
```

### Comparing `LogQS-1.0.8/lqs/interface/pjm/models/__common__.py` & `LogQS-1.0.9/lqs/interface/pjm/models/__common__.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/pjm/models/event.py` & `LogQS-1.0.9/lqs/interface/pjm/models/event.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/pjm/models/job.py` & `LogQS-1.0.9/lqs/interface/pjm/models/job.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/pjm/models/jsonl.py` & `LogQS-1.0.9/lqs/interface/pjm/models/jsonl.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/interface/pjm/update.py` & `LogQS-1.0.9/lqs/interface/pjm/update.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/transcode/__init__.py` & `LogQS-1.0.9/lqs/transcode/__init__.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/transcode/ark/ark_deserialization_methods.py` & `LogQS-1.0.9/lqs/transcode/ark/ark_deserialization_methods.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/transcode/ark/ark_json_parser.py` & `LogQS-1.0.9/lqs/transcode/ark/ark_json_parser.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/transcode/config.py` & `LogQS-1.0.9/lqs/transcode/config.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/transcode/ros1/RosMessageLexer.py` & `LogQS-1.0.9/lqs/transcode/ros1/RosMessageLexer.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/transcode/ros1/RosMessageParser.py` & `LogQS-1.0.9/lqs/transcode/ros1/RosMessageParser.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/transcode/ros1/RosMessageParserListener.py` & `LogQS-1.0.9/lqs/transcode/ros1/RosMessageParserListener.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/transcode/ros1/RosMessageParserVisitor.py` & `LogQS-1.0.9/lqs/transcode/ros1/RosMessageParserVisitor.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/transcode/ros1/RosMessageParserVisitorForMD5.py` & `LogQS-1.0.9/lqs/transcode/ros1/RosMessageParserVisitorForMD5.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/transcode/ros1/ros_deserialization_methods.py` & `LogQS-1.0.9/lqs/transcode/ros1/ros_deserialization_methods.py`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/lqs/transcode/ros1/ros_message_deserializer.py` & `LogQS-1.0.9/lqs/transcode/ros1/ros_message_deserializer.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,20 +12,38 @@
 
 
 import sys
 import types
 
 # TODO consider using slots like genpy does
 
+header_def = '''
+# Standard metadata for higher-level stamped data types.
+# This is generally used to communicate timestamped data 
+# in a particular coordinate frame.
+# 
+# sequence ID: consecutively increasing ID 
+uint32 seq
+#Two-integer timestamp that is expressed as:
+# * stamp.sec: seconds (stamp_secs) since epoch (in Python the variable is called 'secs')
+# * stamp.nsec: nanoseconds since stamp_secs (in Python the variable is called 'nsecs')
+# time-handling sugar is provided by the client library
+time stamp
+#Frame this data is associated with
+string frame_id
+'''
 
 class RosMessageDeserializer:
     def __init__(self, trim_size=None, generate_unnested_schema=True) -> None:
         self._class_registry = {}
         self._trim_size = trim_size
         self.generate_unnested_schema = generate_unnested_schema
+        self._register(
+            "std_msgs/Header",header_def
+        )
 
     def _register(self, message_type, message_type_data) -> None:
         lexer = RosMessageLexer(InputStream(message_type_data))
         stream = CommonTokenStream(lexer)
         parser = RosMessageParser(stream)
         tree = parser.rosbag_input()
         if parser.getNumberOfSyntaxErrors() > 0:
@@ -59,15 +77,14 @@
                 )
 
     def deserialize(self, message_bytes, message_type, message_type_data=None):
         main_package, main_class_name = message_type.rsplit("/")
         if message_type.replace("/", ".") not in self._class_registry:
             self._register(message_type, message_type_data)
         main_cls = getattr(__import__(main_package), main_class_name)
-
         res = main_cls()
         res.deserialize(message_bytes, TRIM_SIZE=self._trim_size)
         return res
 
     def get_json_schema(self, message_type, message_type_data) -> dict:
         lexer = RosMessageLexer(InputStream(message_type_data))
         stream = CommonTokenStream(lexer)
```

### Comparing `LogQS-1.0.8/pyproject.toml` & `LogQS-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `LogQS-1.0.8/setup.py` & `LogQS-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements-client.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="LogQS",
-    version="1.0.8",
+    version="1.0.9",
     author="Nathan Margaglio",
     author_email="nmargaglio@carnegierobotics.com",
     description="A client for interacting with the LogQS Service.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/carnegierobotics/LogQS",
     project_urls={
```

