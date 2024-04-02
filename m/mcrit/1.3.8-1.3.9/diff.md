# Comparing `tmp/mcrit-1.3.8.tar.gz` & `tmp/mcrit-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcrit-1.3.8.tar", last modified: Fri Feb 16 09:10:53 2024, max compression
+gzip compressed data, was "mcrit-1.3.9.tar", last modified: Fri Feb 16 15:38:05 2024, max compression
```

## Comparing `mcrit-1.3.8.tar` & `mcrit-1.3.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 09:10:53.219593 mcrit-1.3.8/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    35149 2022-05-13 09:44:28.000000 mcrit-1.3.8/LICENSE
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    19349 2024-02-16 09:10:53.219593 mcrit-1.3.8/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    16612 2024-02-16 08:50:53.000000 mcrit-1.3.8/README.md
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 09:10:53.215593 mcrit-1.3.8/mcrit/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    23516 2024-02-12 08:21:11.000000 mcrit-1.3.8/mcrit/Worker.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3205 2023-10-13 11:23:48.000000 mcrit-1.3.8/mcrit/__main__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 09:10:53.215593 mcrit-1.3.8/mcrit/client/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    33012 2024-01-24 07:48:46.000000 mcrit-1.3.8/mcrit/client/McritClient.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    22943 2024-01-05 08:32:32.000000 mcrit-1.3.8/mcrit/client/McritConsole.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/client/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 09:10:53.215593 mcrit-1.3.8/mcrit/config/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      855 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/config/ConfigInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      547 2023-09-14 21:06:07.000000 mcrit-1.3.8/mcrit/config/GunicornConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1149 2024-02-16 08:50:38.000000 mcrit-1.3.8/mcrit/config/McritConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2622 2023-09-18 16:19:10.000000 mcrit-1.3.8/mcrit/config/MinHashConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      985 2024-02-16 07:48:15.000000 mcrit-1.3.8/mcrit/config/QueueConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1974 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/config/ShinglerConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2034 2024-01-30 13:45:03.000000 mcrit-1.3.8/mcrit/config/StorageConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/config/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 09:10:53.215593 mcrit-1.3.8/mcrit/index/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    30717 2024-01-24 07:48:06.000000 mcrit-1.3.8/mcrit/index/MinHashIndex.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3890 2022-08-08 11:41:38.000000 mcrit-1.3.8/mcrit/index/SearchCursor.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6210 2022-08-08 11:41:38.000000 mcrit-1.3.8/mcrit/index/SearchQueryParser.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6366 2022-08-08 11:41:38.000000 mcrit-1.3.8/mcrit/index/SearchQueryTree.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/index/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 09:10:53.215593 mcrit-1.3.8/mcrit/libs/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/libs/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      726 2023-08-30 06:52:35.000000 mcrit-1.3.8/mcrit/libs/graph.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    29143 2024-01-30 13:45:03.000000 mcrit-1.3.8/mcrit/libs/mongoqueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14152 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/libs/pymmh3.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2276 2023-09-08 13:17:36.000000 mcrit-1.3.8/mcrit/libs/utility.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 09:10:53.215593 mcrit-1.3.8/mcrit/matchers/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10820 2023-08-01 13:44:26.000000 mcrit-1.3.8/mcrit/matchers/FunctionCfgMatcher.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6378 2022-08-31 07:13:17.000000 mcrit-1.3.8/mcrit/matchers/MatcherCross.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    29591 2024-02-01 07:42:36.000000 mcrit-1.3.8/mcrit/matchers/MatcherInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3014 2022-11-25 14:50:57.000000 mcrit-1.3.8/mcrit/matchers/MatcherQuery.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3097 2023-04-10 15:53:10.000000 mcrit-1.3.8/mcrit/matchers/MatcherQueryFunction.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      751 2022-09-28 13:53:00.000000 mcrit-1.3.8/mcrit/matchers/MatcherSample.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2429 2022-12-14 11:14:13.000000 mcrit-1.3.8/mcrit/matchers/MatcherVs.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:59:30.000000 mcrit-1.3.8/mcrit/matchers/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 09:10:53.219593 mcrit-1.3.8/mcrit/minhash/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3662 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/minhash/MinHash.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10547 2022-11-11 10:02:06.000000 mcrit-1.3.8/mcrit/minhash/MinHasher.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3212 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/minhash/ShingleLoader.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/minhash/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 09:10:53.219593 mcrit-1.3.8/mcrit/queue/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1486 2023-09-15 11:50:24.000000 mcrit-1.3.8/mcrit/queue/JobCollection.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    18467 2023-12-28 07:25:53.000000 mcrit-1.3.8/mcrit/queue/LocalQueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1118 2023-09-12 14:05:30.000000 mcrit-1.3.8/mcrit/queue/QueueFactory.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    16364 2024-02-12 08:10:09.000000 mcrit-1.3.8/mcrit/queue/QueueRemoteCalls.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:36:44.000000 mcrit-1.3.8/mcrit/queue/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 09:10:53.219593 mcrit-1.3.8/mcrit/server/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1297 2023-03-21 14:19:34.000000 mcrit-1.3.8/mcrit/server/BlocksResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6004 2023-03-21 14:19:34.000000 mcrit-1.3.8/mcrit/server/FamilyResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3764 2023-05-12 13:35:06.000000 mcrit-1.3.8/mcrit/server/FunctionResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7987 2024-01-05 06:11:25.000000 mcrit-1.3.8/mcrit/server/JobResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3551 2023-03-21 14:19:34.000000 mcrit-1.3.8/mcrit/server/MatchResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7608 2023-03-22 15:50:20.000000 mcrit-1.3.8/mcrit/server/QueryResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    12311 2023-11-17 07:39:40.000000 mcrit-1.3.8/mcrit/server/SampleResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6571 2024-01-29 09:31:31.000000 mcrit-1.3.8/mcrit/server/StatusResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/server/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7696 2024-01-24 09:08:17.000000 mcrit-1.3.8/mcrit/server/application_routes.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1868 2023-03-21 14:19:34.000000 mcrit-1.3.8/mcrit/server/utils.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       69 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/server/wsgi.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 09:10:53.219593 mcrit-1.3.8/mcrit/storage/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2077 2022-08-03 10:24:19.000000 mcrit-1.3.8/mcrit/storage/FamilyEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6537 2023-09-08 13:17:36.000000 mcrit-1.3.8/mcrit/storage/FunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1661 2023-03-21 14:19:34.000000 mcrit-1.3.8/mcrit/storage/FunctionLabelEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3008 2023-09-15 13:49:11.000000 mcrit-1.3.8/mcrit/storage/MatchedFunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6617 2023-02-14 15:17:18.000000 mcrit-1.3.8/mcrit/storage/MatchedSampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1389 2023-04-10 15:53:10.000000 mcrit-1.3.8/mcrit/storage/MatchingCache.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    37766 2024-02-16 08:51:24.000000 mcrit-1.3.8/mcrit/storage/MatchingResult.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    47092 2023-12-28 07:36:13.000000 mcrit-1.3.8/mcrit/storage/MemoryStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    70184 2024-01-30 13:45:04.000000 mcrit-1.3.8/mcrit/storage/MongoDbStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5055 2023-09-08 13:17:36.000000 mcrit-1.3.8/mcrit/storage/SampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      735 2022-11-13 10:29:45.000000 mcrit-1.3.8/mcrit/storage/StorageFactory.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    26056 2024-01-24 11:55:45.000000 mcrit-1.3.8/mcrit/storage/StorageInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6989 2024-01-02 09:35:34.000000 mcrit-1.3.8/mcrit/storage/UniqueBlocksResult.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.8/mcrit/storage/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 09:10:53.215593 mcrit-1.3.8/mcrit.egg-info/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    19349 2024-02-16 09:10:53.000000 mcrit-1.3.8/mcrit.egg-info/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2120 2024-02-16 09:10:53.000000 mcrit-1.3.8/mcrit.egg-info/SOURCES.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        1 2024-02-16 09:10:53.000000 mcrit-1.3.8/mcrit.egg-info/dependency_links.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      238 2024-02-16 09:10:53.000000 mcrit-1.3.8/mcrit.egg-info/requires.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        6 2024-02-16 09:10:53.000000 mcrit-1.3.8/mcrit.egg-info/top_level.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      235 2024-02-16 08:52:03.000000 mcrit-1.3.8/requirements.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2024-02-16 09:10:53.219593 mcrit-1.3.8/setup.cfg
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1161 2024-02-16 08:50:47.000000 mcrit-1.3.8/setup.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 15:38:05.668985 mcrit-1.3.9/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    35149 2022-05-13 09:44:28.000000 mcrit-1.3.9/LICENSE
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    19487 2024-02-16 15:38:05.668985 mcrit-1.3.9/PKG-INFO
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    16742 2024-02-16 15:37:32.000000 mcrit-1.3.9/README.md
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 15:38:05.660985 mcrit-1.3.9/mcrit/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    26781 2024-02-16 15:36:06.000000 mcrit-1.3.9/mcrit/Worker.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3205 2023-10-13 11:23:48.000000 mcrit-1.3.9/mcrit/__main__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 15:38:05.660985 mcrit-1.3.9/mcrit/client/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    33012 2024-01-24 07:48:46.000000 mcrit-1.3.9/mcrit/client/McritClient.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    22943 2024-01-05 08:32:32.000000 mcrit-1.3.9/mcrit/client/McritConsole.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/client/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 15:38:05.660985 mcrit-1.3.9/mcrit/config/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      855 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/config/ConfigInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      547 2023-09-14 21:06:07.000000 mcrit-1.3.9/mcrit/config/GunicornConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1149 2024-02-16 15:37:11.000000 mcrit-1.3.9/mcrit/config/McritConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2622 2023-09-18 16:19:10.000000 mcrit-1.3.9/mcrit/config/MinHashConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      985 2024-02-16 07:48:15.000000 mcrit-1.3.9/mcrit/config/QueueConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1974 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/config/ShinglerConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2284 2024-02-16 15:36:06.000000 mcrit-1.3.9/mcrit/config/StorageConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/config/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 15:38:05.664985 mcrit-1.3.9/mcrit/index/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    31954 2024-02-16 15:36:06.000000 mcrit-1.3.9/mcrit/index/MinHashIndex.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3890 2022-08-08 11:41:38.000000 mcrit-1.3.9/mcrit/index/SearchCursor.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6210 2022-08-08 11:41:38.000000 mcrit-1.3.9/mcrit/index/SearchQueryParser.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6366 2022-08-08 11:41:38.000000 mcrit-1.3.9/mcrit/index/SearchQueryTree.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/index/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 15:38:05.664985 mcrit-1.3.9/mcrit/libs/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/libs/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      726 2023-08-30 06:52:35.000000 mcrit-1.3.9/mcrit/libs/graph.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    29920 2024-02-16 15:36:06.000000 mcrit-1.3.9/mcrit/libs/mongoqueue.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    14152 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/libs/pymmh3.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2276 2023-09-08 13:17:36.000000 mcrit-1.3.9/mcrit/libs/utility.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 15:38:05.664985 mcrit-1.3.9/mcrit/matchers/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10820 2023-08-01 13:44:26.000000 mcrit-1.3.9/mcrit/matchers/FunctionCfgMatcher.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6378 2022-08-31 07:13:17.000000 mcrit-1.3.9/mcrit/matchers/MatcherCross.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    29591 2024-02-01 07:42:36.000000 mcrit-1.3.9/mcrit/matchers/MatcherInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3014 2022-11-25 14:50:57.000000 mcrit-1.3.9/mcrit/matchers/MatcherQuery.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3097 2023-04-10 15:53:10.000000 mcrit-1.3.9/mcrit/matchers/MatcherQueryFunction.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      751 2022-09-28 13:53:00.000000 mcrit-1.3.9/mcrit/matchers/MatcherSample.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2429 2022-12-14 11:14:13.000000 mcrit-1.3.9/mcrit/matchers/MatcherVs.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:59:30.000000 mcrit-1.3.9/mcrit/matchers/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 15:38:05.664985 mcrit-1.3.9/mcrit/minhash/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3662 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/minhash/MinHash.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10547 2022-11-11 10:02:06.000000 mcrit-1.3.9/mcrit/minhash/MinHasher.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3212 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/minhash/ShingleLoader.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/minhash/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 15:38:05.664985 mcrit-1.3.9/mcrit/queue/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1486 2023-09-15 11:50:24.000000 mcrit-1.3.9/mcrit/queue/JobCollection.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    18467 2023-12-28 07:25:53.000000 mcrit-1.3.9/mcrit/queue/LocalQueue.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1118 2023-09-12 14:05:30.000000 mcrit-1.3.9/mcrit/queue/QueueFactory.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    16439 2024-02-16 15:36:06.000000 mcrit-1.3.9/mcrit/queue/QueueRemoteCalls.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:36:44.000000 mcrit-1.3.9/mcrit/queue/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 15:38:05.664985 mcrit-1.3.9/mcrit/server/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1297 2023-03-21 14:19:34.000000 mcrit-1.3.9/mcrit/server/BlocksResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6004 2023-03-21 14:19:34.000000 mcrit-1.3.9/mcrit/server/FamilyResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3764 2023-05-12 13:35:06.000000 mcrit-1.3.9/mcrit/server/FunctionResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7987 2024-01-05 06:11:25.000000 mcrit-1.3.9/mcrit/server/JobResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3551 2023-03-21 14:19:34.000000 mcrit-1.3.9/mcrit/server/MatchResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7608 2023-03-22 15:50:20.000000 mcrit-1.3.9/mcrit/server/QueryResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    12311 2023-11-17 07:39:40.000000 mcrit-1.3.9/mcrit/server/SampleResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6571 2024-01-29 09:31:31.000000 mcrit-1.3.9/mcrit/server/StatusResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/server/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7696 2024-01-24 09:08:17.000000 mcrit-1.3.9/mcrit/server/application_routes.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1868 2023-03-21 14:19:34.000000 mcrit-1.3.9/mcrit/server/utils.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       69 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/server/wsgi.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 15:38:05.668985 mcrit-1.3.9/mcrit/storage/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2077 2022-08-03 10:24:19.000000 mcrit-1.3.9/mcrit/storage/FamilyEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6537 2023-09-08 13:17:36.000000 mcrit-1.3.9/mcrit/storage/FunctionEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1661 2023-03-21 14:19:34.000000 mcrit-1.3.9/mcrit/storage/FunctionLabelEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3008 2023-09-15 13:49:11.000000 mcrit-1.3.9/mcrit/storage/MatchedFunctionEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6617 2023-02-14 15:17:18.000000 mcrit-1.3.9/mcrit/storage/MatchedSampleEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1389 2023-04-10 15:53:10.000000 mcrit-1.3.9/mcrit/storage/MatchingCache.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    37766 2024-02-16 08:51:24.000000 mcrit-1.3.9/mcrit/storage/MatchingResult.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    47092 2023-12-28 07:36:13.000000 mcrit-1.3.9/mcrit/storage/MemoryStorage.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    71255 2024-02-16 15:36:06.000000 mcrit-1.3.9/mcrit/storage/MongoDbStorage.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     5184 2024-02-16 15:36:06.000000 mcrit-1.3.9/mcrit/storage/SampleEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      735 2022-11-13 10:29:45.000000 mcrit-1.3.9/mcrit/storage/StorageFactory.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    26783 2024-02-16 15:36:06.000000 mcrit-1.3.9/mcrit/storage/StorageInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6989 2024-01-02 09:35:34.000000 mcrit-1.3.9/mcrit/storage/UniqueBlocksResult.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.3.9/mcrit/storage/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2024-02-16 15:38:05.660985 mcrit-1.3.9/mcrit.egg-info/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    19487 2024-02-16 15:38:05.000000 mcrit-1.3.9/mcrit.egg-info/PKG-INFO
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2120 2024-02-16 15:38:05.000000 mcrit-1.3.9/mcrit.egg-info/SOURCES.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        1 2024-02-16 15:38:05.000000 mcrit-1.3.9/mcrit.egg-info/dependency_links.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      238 2024-02-16 15:38:05.000000 mcrit-1.3.9/mcrit.egg-info/requires.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        6 2024-02-16 15:38:05.000000 mcrit-1.3.9/mcrit.egg-info/top_level.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      235 2024-02-16 08:52:03.000000 mcrit-1.3.9/requirements.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2024-02-16 15:38:05.668985 mcrit-1.3.9/setup.cfg
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1161 2024-02-16 15:37:08.000000 mcrit-1.3.9/setup.py
```

### Comparing `mcrit-1.3.8/LICENSE` & `mcrit-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/PKG-INFO` & `mcrit-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.3.8
+Version: 1.3.9
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
 Description: # MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
         [![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
@@ -125,14 +125,15 @@
         
         ### Reference Data 
         
         In July 2023, we started populating a [Github repository](https://github.com/danielplohmann/mcrit-data) which contains ready-to-use reference data for common compilers and libraries.
         
         
         ## Version History
+         * 2024-02-16 v1.3.9:  Finished and integrated automated queue cleanup feature (disabled by default) proposed by @yankovs - THX!!
          * 2024-02-15 v1.3.8:  Bump SMDA to address issues with version recognition in SmdaFunction, fixed exception prints in IDA plugin's McritInterface (THX to @malwarefrank!!).
          * 2024-02-12 v1.3.5:  Recalculating minhashes will now show correct percentages (THX to @malwarefrank!!).
          * 2024-02-02 v1.3.4:  Mini fix in the IDA plugin to avoid referencing a potentially uninitialized object (THX to @r0ny123!!).
          * 2024-02-01 v1.3.2:  FIX: Non-parallelized matching now outputs the [same data format](https://github.com/danielplohmann/mcrit/pull/63) (THX to @dannyquist!!).
          * 2024-01-30 v1.3.1:  The connection to MongoDB is now fully [configurable](https://github.com/danielplohmann/mcrit/pull/61) (THX to @dannyquist!!).
          * 2024-01-24 v1.3.0:  BREAKING: Milestone release with indexing improvements for PicHash and MinHash. To ensure full backward compatibility, recalculation of all hashes is recommended. Check this [migration guide](https://github.com/danielplohmann/mcrit/blob/main/docs/migration-v1.3.0.md). 
          * 2024-01-23 v1.2.26: Pinning lief to 0.13.2 in order to ensure that the pinned SMDA remains compatible.
```

### Comparing `mcrit-1.3.8/README.md` & `mcrit-1.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 
 ### Reference Data 
 
 In July 2023, we started populating a [Github repository](https://github.com/danielplohmann/mcrit-data) which contains ready-to-use reference data for common compilers and libraries.
 
 
 ## Version History
+ * 2024-02-16 v1.3.9:  Finished and integrated automated queue cleanup feature (disabled by default) proposed by @yankovs - THX!!
  * 2024-02-15 v1.3.8:  Bump SMDA to address issues with version recognition in SmdaFunction, fixed exception prints in IDA plugin's McritInterface (THX to @malwarefrank!!).
  * 2024-02-12 v1.3.5:  Recalculating minhashes will now show correct percentages (THX to @malwarefrank!!).
  * 2024-02-02 v1.3.4:  Mini fix in the IDA plugin to avoid referencing a potentially uninitialized object (THX to @r0ny123!!).
  * 2024-02-01 v1.3.2:  FIX: Non-parallelized matching now outputs the [same data format](https://github.com/danielplohmann/mcrit/pull/63) (THX to @dannyquist!!).
  * 2024-01-30 v1.3.1:  The connection to MongoDB is now fully [configurable](https://github.com/danielplohmann/mcrit/pull/61) (THX to @dannyquist!!).
  * 2024-01-24 v1.3.0:  BREAKING: Milestone release with indexing improvements for PicHash and MinHash. To ensure full backward compatibility, recalculation of all hashes is recommended. Check this [migration guide](https://github.com/danielplohmann/mcrit/blob/main/docs/migration-v1.3.0.md). 
  * 2024-01-23 v1.2.26: Pinning lief to 0.13.2 in order to ensure that the pinned SMDA remains compatible.
```

### Comparing `mcrit-1.3.8/mcrit/Worker.py` & `mcrit-1.3.9/mcrit/Worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python3
 
 import os
+import re
 import uuid
 import json
 import logging
 import hashlib
 from random import sample
+from datetime import datetime, timedelta
 from collections import defaultdict
 from itertools import zip_longest
 from multiprocessing import Pool, cpu_count
 from typing import Dict, List, Optional, TYPE_CHECKING, Tuple
 
 import tqdm
 from smda.common.BinaryInfo import BinaryInfo
@@ -27,14 +29,15 @@
 from mcrit.config.McritConfig import McritConfig
 from mcrit.config.StorageConfig import StorageConfig
 from mcrit.matchers.MatcherCross import MatcherCross
 from mcrit.matchers.MatcherQuery import MatcherQuery
 from mcrit.matchers.MatcherSample import MatcherSample
 from mcrit.matchers.MatcherVs import MatcherVs
 from mcrit.minhash.MinHasher import MinHasher
+from mcrit.queue.LocalQueue import Job
 from mcrit.queue.QueueFactory import QueueFactory
 from mcrit.queue.QueueRemoteCalls import NoProgressReporter, QueueRemoteCallee, Remote
 from mcrit.storage.SampleEntry import SampleEntry
 from mcrit.storage.StorageFactory import StorageFactory
 
 if TYPE_CHECKING:
     from mcrit.storage.StorageInterface import StorageInterface
@@ -172,15 +175,68 @@
             SMDA_REPORT.version = version
         sample_entry = self._addReport(SMDA_REPORT)
         LOGGER.info("Disassembled and indexed sample: %s", sample_entry)
         if sample_entry is not None:
             return {"sample_info": sample_entry.toDict()}
         else:
             return None
-
+        
+    # Reports PROGRESS
+    @Remote(progress=True)
+    def doDbCleanup(self, progress_reporter=NoProgressReporter()):
+        now = datetime.now()
+        delta = timedelta(seconds=self._storage_config.STORAGE_MONGODB_CLEANUP_TTL)
+        time_cutoff = now - delta
+        unmapped_finished = self.getQueueData(0, 0, method="getMatchesForUnmappedBinary", state="finished")
+        mapped_finished = self.getQueueData(0, 0, method="getMatchesForMappedBinary", state="finished")
+        smda_finished = self.getQueueData(0, 0, method="getMatchesForSmdaReport", state="finished")
+        recent_samples = set([])
+        samples_to_be_deleted = {}
+        jobs_to_be_deleted = []
+        for job_collection in [unmapped_finished, mapped_finished]:
+            for job_dict in unmapped_finished:
+                job = Job(job_dict, None)
+                # we keep those query samples that have been submitted since the cutoff
+                if job.finished_at > time_cutoff:
+                    recent_samples.add(job.sha256)
+                else:
+                    jobs_to_be_deleted.append(job)
+                    if job.sha256 not in samples_to_be_deleted:
+                        sample_entry = self._storage.getSampleBySha256(job.sha256, is_query=True)
+                        if sample_entry:
+                            samples_to_be_deleted[job.sha256] = sample_entry
+        for job_dict in smda_finished:
+            job = Job(job_dict, None)
+            # find sample info based on smda report, extract sha256 via regex
+            smda_dict_start = self.queue.getFileByHash(job.sha256, max_bytes=2048)
+            match = re.search(b'"sha256": "(?P<sha256>[A-Fa-f0-9]{64})"', smda_dict_start)
+            if match:
+                smda_file_sha256 = match.group('sha256').decode("ascii")
+                # we keep those query samples that have been submitted since the cutoff
+                if job.finished_at > time_cutoff:
+                    recent_samples.add(smda_file_sha256)
+                else:
+                    jobs_to_be_deleted.append(job)
+                    if smda_file_sha256 not in samples_to_be_deleted:
+                        sample_entry = self._storage.getSampleBySha256(smda_file_sha256, is_query=True)
+                        if sample_entry:
+                            samples_to_be_deleted[smda_file_sha256] = sample_entry
+            else:
+                LOGGER.warn(f"Target SHA256 not found in first 2048 bytes of SMDA report with file hash {job.sha256}.")
+        for sha256 in recent_samples:
+            samples_to_be_deleted.pop(sha256)
+        LOGGER.info(f"Found {len(samples_to_be_deleted)} query samples that can be deleted")
+        for sample_sha256, sample_entry in samples_to_be_deleted.items():
+            LOGGER.info(f"Deleting {sample_entry.sample_id}.")
+            self._storage.deleteSample(sample_entry.sample_id)
+        # now remove the respective data also from the queue, which also deletes the results from GridFS
+        LOGGER.info(f"Found {len(jobs_to_be_deleted)} query jobs that can be deleted.")
+        for job in jobs_to_be_deleted:
+            self.queue.delete_job(job.job_id)
+        
     # Reports PROGRESS
     @Remote(progress=True)
     def rebuildIndex(self, progress_reporter=NoProgressReporter()):
         return self._storage.rebuildMinhashBandIndex(progress_reporter=progress_reporter)
     
     # Reports PROGRESS
     @Remote(progress=True)
```

### Comparing `mcrit-1.3.8/mcrit/__main__.py` & `mcrit-1.3.9/mcrit/__main__.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/client/McritClient.py` & `mcrit-1.3.9/mcrit/client/McritClient.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/client/McritConsole.py` & `mcrit-1.3.9/mcrit/client/McritConsole.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/config/ConfigInterface.py` & `mcrit-1.3.9/mcrit/config/ConfigInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/config/GunicornConfig.py` & `mcrit-1.3.9/mcrit/config/GunicornConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/config/McritConfig.py` & `mcrit-1.3.9/mcrit/config/McritConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .ShinglerConfig import ShinglerConfig
 from .StorageConfig import StorageConfig
 
 
 class McritConfig(object):
 
     # NOTE to self: always change this in setup.py as well!
-    VERSION = "1.3.8"
+    VERSION = "1.3.9"
     # basic pathing info
     CONFIG_FILE_PATH = str(os.path.abspath(__file__))
     PROJECT_ROOT = str(os.path.abspath(os.sep.join([CONFIG_FILE_PATH, "..", ".."])))
 
     # Authentication token, which can be optionally used to lock down communication with the API
     AUTH_TOKEN = ""
```

### Comparing `mcrit-1.3.8/mcrit/config/MinHashConfig.py` & `mcrit-1.3.9/mcrit/config/MinHashConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/config/QueueConfig.py` & `mcrit-1.3.9/mcrit/config/QueueConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/config/ShinglerConfig.py` & `mcrit-1.3.9/mcrit/config/ShinglerConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/config/StorageConfig.py` & `mcrit-1.3.9/mcrit/config/StorageConfig.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,18 @@
     STORAGE_PORT: str = "27017"
     # By default, MongoDbStorage's DB's name and MongoQueue's DB's name are both "mcrit"
     # Changing one DB name here or at runtime DOES NOT change the other name!
     STORAGE_MONGODB_DBNAME: str = "mcrit"
     STORAGE_MONGODB_USERNAME: str = None
     STORAGE_MONGODB_PASSWORD: str = None
     STORAGE_MONGODB_FLAGS: str = ""
+    # Enable periodic deletion of queried samples and their results after a given time
+    STORAGE_MONGODB_ENABLE_CLEANUP: bool = False
+    STORAGE_MONGODB_CLEANUP_DELTA: int = 60 * 60 * 24 * 7
+    STORAGE_MONGODB_CLEANUP_TTL: int = 60 * 60 * 24 * 7
     # Once MinHashes have been calculated, discard disassembly from function entries
     STORAGE_DROP_DISASSEMBLY: bool = False
     # random seed to be used when deriving sequences used as bands
     STORAGE_BAND_SEED: int = 0xDEADBEEF
     # Banding supports:
     #  * MemoryStorage: arbitrary banding configuration, multiple lengths
     #  * MongoDbStorage: arbitrary banding configuration, multiple lengths
```

### Comparing `mcrit-1.3.8/mcrit/index/MinHashIndex.py` & `mcrit-1.3.9/mcrit/index/MinHashIndex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 import re
 import json
 import time
 import logging
+from datetime import datetime, timedelta
 from typing import Dict, List
 
 from smda.common.SmdaReport import SmdaReport
 
 from mcrit.config.McritConfig import McritConfig
 from mcrit.config.MinHashConfig import MinHashConfig
 from mcrit.config.ShinglerConfig import ShinglerConfig
@@ -64,22 +65,46 @@
         self.config = config
         self._storage_config = config.STORAGE_CONFIG
         self._minhash_config = config.MINHASH_CONFIG
         self._shingler_config = config.SHINGLER_CONFIG
         self._queue_config = config.QUEUE_CONFIG
         self.minhasher = MinHasher(self._minhash_config, self._shingler_config)
         self._storage = StorageFactory.getStorage(config)
+        self._cleanup_delta = timedelta(seconds=int(self._storage_config.STORAGE_MONGODB_CLEANUP_DELTA))
         # config.QUEUE_CONFIG.QUEUE_METHOD = QueueFactory.QUEUE_METHOD_FAKE
         queue = QueueFactory().getQueue(config, storage=self._storage, consumer_id="index")
         self.search_query_parser = SearchQueryParser()
         super().__init__(queue)
 
+    def _getLastCleanup(self):
+        try:
+            timestamp = self._storage.getDbCleanupTimestamp()
+            if not timestamp:
+                timestamp = self._storage.updateDbCleanupTimestamp()
+            return timestamp
+        except Exception as e:
+            LOGGER.error(f"Failed getting last cleanup: {e}, this should no automatically fix itself with the next request.")
+    
+    def _cleanupCallback(self):
+        if not self._storage_config.STORAGE_MONGODB_ENABLE_CLEANUP:
+            return
+        last_timestamp = self._getLastCleanup()
+        if last_timestamp:
+            now = datetime.now()
+            if last_timestamp + self._cleanup_delta < now:
+                LOGGER.info("Scheduling a cleanup for query samples.")
+                self.doDbCleanup(force_recalculation=True)
+                self._storage.updateDbCleanupTimestamp()
+        else:
+            LOGGER.info("Couldn't determine last db cleanup time, this should no automatically fix itself with the next request.")
+            # Should we do cleanup anyway in such cases?
+
     def _indexCallback(self):
         """ called whenever other functionality in MinHashIndex is used, intended for scheduling maintainance jobs etc. """
-        pass
+        self._cleanupCallback()
     
     #### STORAGE IO ####
     def getStorage(self):
         """Get an interface to the storage"""
         # use this as a callback in all other functions to trigger functionality
         self._indexCallback()
         return self._storage
```

### Comparing `mcrit-1.3.8/mcrit/index/SearchCursor.py` & `mcrit-1.3.9/mcrit/index/SearchCursor.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/index/SearchQueryParser.py` & `mcrit-1.3.9/mcrit/index/SearchQueryParser.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/index/SearchQueryTree.py` & `mcrit-1.3.9/mcrit/index/SearchQueryTree.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/libs/graph.py` & `mcrit-1.3.9/mcrit/libs/graph.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/libs/mongoqueue.py` & `mcrit-1.3.9/mcrit/libs/mongoqueue.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,15 +334,14 @@
             else:
                 for job_document in self._getCollection().find(query_filter, sort=[("_id", -1)]).skip(start_index).limit(limit):
                     jobs.append(self._wrap_one(job_document))
         else:
             # we go with an inefficient implementation for now to see if this is a desired feature and revise the query in case we deem this useful.
             # TODO improve performance of these queries, we probably want to find a query_filter for the different possible states to allow use of skip/limit
             all_jobs = []
-            print(start_index, limit, method, state, ascending)
             if ascending:
                 for job_document in self._getCollection().find(query_filter):
                     if self._identifyJobState(job_document) == state:
                         all_jobs.append(self._wrap_one(job_document))
             else:
                 for job_document in self._getCollection().find(query_filter, sort=[("_id", -1)]):
                     if self._identifyJobState(job_document) == state:
@@ -354,23 +353,26 @@
                 jobs = all_jobs[start_index:]
         return jobs
 
     def get_job(self, job_id):
         job_id = ObjectId(job_id)
         return self._wrap_one(self._getCollection().find_one({"_id": job_id}))
 
-    def delete_job(self, job_id):
+    def delete_job(self, job_id, with_result=True):
         job_id = ObjectId(job_id)
-        job = self._getCollection().find_one({"_id": job_id})
-        if job:
-            self.updateQueueCounter(job["payload"]["method"], self._identifyJobState(job), -1)
-        result = self._getCollection().delete_one({"_id": job_id})
-        return result.deleted_count
+        deletable_job = self._getCollection().find_one({"_id": job_id})
+        if deletable_job:
+            self.updateQueueCounter(deletable_job["payload"]["method"], self._identifyJobState(deletable_job), -1)
+            if with_result:
+                # delete result from GridFS  
+                self._getFs().delete(ObjectId(deletable_job["result"]))
+        job_deletion_result = self._getCollection().delete_one({"_id": job_id})
+        return job_deletion_result.deleted_count
 
-    def delete_jobs(self, method=None, created_before=None, finished_before=None):
+    def delete_jobs(self, method=None, created_before=None, finished_before=None, with_results=True):
         filter_count = len([1 for item in [method, created_before, finished_before] if item is not None])
         combined_filter = {"$and": []} if filter_count > 1 else {}
         method_filter = {}
         created_filter = {}
         finished_filter = {}
         if method is not None:
             method_filter = {"payload.method": method}
@@ -386,19 +388,26 @@
                 combined_filter = created_filter
         elif finished_before is not None:
             finished_filter = {"finished_at": {"$lt": finished_before}}
             if filter_count > 1:
                 combined_filter["$and"].append(finished_filter)
             else:
                 combined_filter = finished_filter
-        print(f"delete_jobs: {combined_filter}")
-        # run find() first to determine how many jobs of which method will be deleted
-        result = self._getCollection().delete_many(combined_filter)
-        # TODO update counters - accordingly to find result, if result.deleted_count matches expectation
-        return result.deleted_count
+        # run find() first to determine how many jobs of which method will be deleted and what their results are
+        jobs_to_be_deleted = [j for j in self._getCollection().find(combined_filter)]
+        # delete results
+        for deletable_job in jobs_to_be_deleted:
+            self.updateQueueCounter(deletable_job["payload"]["method"], self._identifyJobState(deletable_job), -1)
+            if with_results and deletable_job["result"]:
+                    # delete result from GridFS  
+                    self._getFs().delete(ObjectId(deletable_job["result"]))
+        job_deletion_result = self._getCollection().delete_many(combined_filter)
+        if len(jobs_to_be_deleted) != job_deletion_result.deleted_count:
+            raise Exception("Number of deleted jobs was unequal to number of jobs to delete!")
+        return job_deletion_result.deleted_count
 
     def _file_to_grid(self, binary, metadata=None):
         object_id = self._getFs().put(binary, metadata=metadata)
         return str(object_id)
 
     def _grid_to_file(self, grid, results_only=True):
         oid = ObjectId(grid)
@@ -441,16 +450,18 @@
                     "terminated": False,
                 },
                 sort=[("created_at", pymongo.DESCENDING)],
             )
         )
         return job and job.job_id or None
 
-    def _get_file_by_hash(self, sha256):
+    def getFileByHash(self, sha256, max_bytes=-1):
         file = self._getFs().find_one({"metadata.sha256": sha256})
+        if file:
+            return file.read(max_bytes)
 
     def get_file_by_hash_inc_lock(self, sha256):
         file = self._getFsFiles().find_one_and_update({"metadata.sha256": sha256}, {"$inc": {"metadata.tmp_lock": 1}})
         return file and str(file["_id"]) or None
 
     def add_job_id_to_file(self, job_id, file_id):
         file_id = ObjectId(file_id)
```

### Comparing `mcrit-1.3.8/mcrit/libs/pymmh3.py` & `mcrit-1.3.9/mcrit/libs/pymmh3.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/libs/utility.py` & `mcrit-1.3.9/mcrit/libs/utility.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/matchers/FunctionCfgMatcher.py` & `mcrit-1.3.9/mcrit/matchers/FunctionCfgMatcher.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/matchers/MatcherCross.py` & `mcrit-1.3.9/mcrit/matchers/MatcherCross.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/matchers/MatcherInterface.py` & `mcrit-1.3.9/mcrit/matchers/MatcherInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/matchers/MatcherQuery.py` & `mcrit-1.3.9/mcrit/matchers/MatcherQuery.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/matchers/MatcherQueryFunction.py` & `mcrit-1.3.9/mcrit/matchers/MatcherQueryFunction.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/matchers/MatcherSample.py` & `mcrit-1.3.9/mcrit/matchers/MatcherSample.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/matchers/MatcherVs.py` & `mcrit-1.3.9/mcrit/matchers/MatcherVs.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/minhash/MinHash.py` & `mcrit-1.3.9/mcrit/minhash/MinHash.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/minhash/MinHasher.py` & `mcrit-1.3.9/mcrit/minhash/MinHasher.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/minhash/ShingleLoader.py` & `mcrit-1.3.9/mcrit/minhash/ShingleLoader.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/queue/JobCollection.py` & `mcrit-1.3.9/mcrit/queue/JobCollection.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/queue/LocalQueue.py` & `mcrit-1.3.9/mcrit/queue/LocalQueue.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/queue/QueueFactory.py` & `mcrit-1.3.9/mcrit/queue/QueueFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/queue/QueueRemoteCalls.py` & `mcrit-1.3.9/mcrit/queue/QueueRemoteCalls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from datetime import datetime
-import hashlib
-import json
 import os
-from sqlite3 import Timestamp
 import time
-from functools import wraps
+import json
+import hashlib
 import logging
+from datetime import datetime
+from functools import wraps
+
+from typing import Any, TYPE_CHECKING, Dict, Iterable, List, Optional, Set, Tuple, Union
 
 
 # Only do basicConfig if no handlers have been configured
 if len(logging._handlerList) == 0:
     logging.basicConfig(level=logging.INFO, format="%(asctime)-15s %(message)s")
 LOGGER = logging.getLogger(__name__)
 
@@ -30,15 +31,15 @@
         # -> either return "Done" with result / where to find result, OR NotFound
         pass
 
     def getQueueStats(self, refresh=False):
         LOGGER.debug(f"called getQueueStats()")
         return self.queue.getQueueStatistics(refresh=refresh)
 
-    def getQueueData(self, start_index: int, limit: int, method=None, state=None, filter=None, ascending=False):
+    def getQueueData(self, start_index: int, limit: int, method=None, state=None, filter=None, ascending=False) -> List["Job"]:
         LOGGER.debug(f"called getQueueData(start_index={start_index}, limit={method}, method={method}, state={state}, filter={filter}, ascending={ascending}):")
         if filter is not None:
             # TODO apply filter to more fields
             return [job._data for job in self.queue.get_jobs(start_index, limit, method, state, ascending) if filter in job.parameters]
         return [job._data for job in self.queue.get_jobs(start_index, limit, method, state, ascending)]
     
     def deleteQueueData(self, method=None, created_before=None, finished_before=None):
```

### Comparing `mcrit-1.3.8/mcrit/server/BlocksResource.py` & `mcrit-1.3.9/mcrit/server/BlocksResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/server/FamilyResource.py` & `mcrit-1.3.9/mcrit/server/FamilyResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/server/FunctionResource.py` & `mcrit-1.3.9/mcrit/server/FunctionResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/server/JobResource.py` & `mcrit-1.3.9/mcrit/server/JobResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/server/MatchResource.py` & `mcrit-1.3.9/mcrit/server/MatchResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/server/QueryResource.py` & `mcrit-1.3.9/mcrit/server/QueryResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/server/SampleResource.py` & `mcrit-1.3.9/mcrit/server/SampleResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/server/StatusResource.py` & `mcrit-1.3.9/mcrit/server/StatusResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/server/application_routes.py` & `mcrit-1.3.9/mcrit/server/application_routes.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/server/utils.py` & `mcrit-1.3.9/mcrit/server/utils.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/storage/FamilyEntry.py` & `mcrit-1.3.9/mcrit/storage/FamilyEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/storage/FunctionEntry.py` & `mcrit-1.3.9/mcrit/storage/FunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/storage/FunctionLabelEntry.py` & `mcrit-1.3.9/mcrit/storage/FunctionLabelEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/storage/MatchedFunctionEntry.py` & `mcrit-1.3.9/mcrit/storage/MatchedFunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/storage/MatchedSampleEntry.py` & `mcrit-1.3.9/mcrit/storage/MatchedSampleEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/storage/MatchingCache.py` & `mcrit-1.3.9/mcrit/storage/MatchingCache.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/storage/MatchingResult.py` & `mcrit-1.3.9/mcrit/storage/MatchingResult.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/storage/MemoryStorage.py` & `mcrit-1.3.9/mcrit/storage/MemoryStorage.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/storage/MongoDbStorage.py` & `mcrit-1.3.9/mcrit/storage/MongoDbStorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,29 @@
         
     def _getDbTimestamp(self):
         result = self._getDb().settings.find_one({})
         if result is None:
             raise Exception("Database does not have a state field yet")
         elif "db_timestamp" in result:
             return result["db_timestamp"]
-            
+        
+    def updateDbCleanupTimestamp(self):
+        result = self._getDb().settings.find_one_and_update({}, { "$inc": { "db_state": 1}})
+        result = self._getDb().settings.find_one_and_update({}, { "$set": {"db_cleanup_timestamp": self._getCurrentTimestamp()}}, upsert=True)
+        if result is None:
+            raise Exception("Database does not have a db_state field")
+        else:
+            return result["db_cleanup_timestamp"]
+    
+    def getDbCleanupTimestamp(self):
+        result = self._getDb().settings.find_one({})
+        if result is None:
+            raise Exception("Database does not have a state field yet")
+        elif "db_cleanup_timestamp" in result:
+            return result["db_cleanup_timestamp"]
 
     ###############################################################################
     # Conversion
     ###############################################################################
 
     def _encodeXcfg(self, function_dict: Dict, delete_old: bool = True) -> None:
         if "xcfg" in function_dict:
@@ -557,21 +571,27 @@
         collections = ["samples", "families", "functions", "matches", "candidates", "counters", "query_samples", "query_functions"]
         for band_id in range(self._storage_config.STORAGE_NUM_BANDS):
             collections.append("band_%d" % band_id)
         for c in collections:
             self._getDb()[c].drop()
         self._ensureIndexAndUnknownFamily()
 
-    def getSampleBySha256(self, sha256: str) -> Optional["SampleEntry"]:
-        if self._getDb().samples.count_documents(filter={}):
-            report_dict = self._getDb().samples.find_one({"sha256": sha256})
-            if not report_dict:
-                return None
-            return SampleEntry.fromDict(report_dict)
-        return None
+    def getSampleBySha256(self, sha256: str, is_query=False) -> Optional["SampleEntry"]:
+        target_sample = None
+        if is_query:
+            if self._getDb().query_samples.count_documents(filter={}):
+                report_dict = self._getDb().query_samples.find_one({"sha256": sha256})
+                if report_dict:
+                    target_sample = SampleEntry.fromDict(report_dict)
+        else:
+            if self._getDb().samples.count_documents(filter={}):
+                report_dict = self._getDb().samples.find_one({"sha256": sha256})
+                if report_dict:
+                    target_sample = SampleEntry.fromDict(report_dict)
+        return target_sample
 
     def updateFunctionLabels(self, smda_report: "SmdaReport", username) -> Optional["SampleEntry"]:
         sample_entry = self.getSampleBySha256(smda_report.sha256)
         if not sample_entry:
             return False
         # check which functions in the SmdaReport have suitable function_names
         submitted_labels = {}
```

### Comparing `mcrit-1.3.8/mcrit/storage/SampleEntry.py` & `mcrit-1.3.9/mcrit/storage/SampleEntry.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,7 +123,11 @@
         sample_entry.timestamp = sample.timestamp
         return sample_entry
 
     def __str__(self):
         return "Sample {} ({}, {} bit) - {} ({}): ".format(
             self.sample_id, self.architecture, self.bitness, self.filename, self.family
         )
+
+    def __hash__(self):
+        """Override the default hash behavior"""
+        return hash(f"{self.sample_id}_{self.sha256}")
```

### Comparing `mcrit-1.3.8/mcrit/storage/StorageFactory.py` & `mcrit-1.3.9/mcrit/storage/StorageFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit/storage/StorageInterface.py` & `mcrit-1.3.9/mcrit/storage/StorageInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import random
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Tuple, Union
 
 from mcrit.minhash.MinHash import MinHash
 
 if TYPE_CHECKING: # pragma: no cover
     from mcrit.config.StorageConfig import StorageConfig
@@ -48,14 +49,32 @@
         """ Log an event to the database
 
         Args:
             event_msg: a string describing the event
             username: (optional) a username tied to this event
             details: a dict with arbitrary additional information
         """
+        raise NotImplementedError
+
+    def updateDbCleanupTimestamp(self) -> datetime.datetime:
+        """ Update a timestamp indicating the last time queried samples were deleted
+
+        Returns:
+            db_cleanup_timestamp: a datetime.datetime when the DB was last cleaned
+        """
+        raise NotImplementedError
+
+    def getDbCleanupTimestamp(self) -> datetime.datetime:
+        """ Get a timestamp indicating the last time queried samples were deleted
+
+        Returns:
+            db_cleanup_timestamp: a datetime.datetime when the DB was last cleaned
+        """
+        raise NotImplementedError
+
 
     # -> Set[function_id]
     def getCandidatesForMinHash(self, minhash: "MinHash", band_matches_required=1) -> Set[int]:
         """Given a MinHash, return all candidates from all matching bands.
 
         Args:
             minhash: a MinHash
@@ -102,19 +121,20 @@
         """Delete all contents in the storage, reinitialize an empty storage, ensure indexing and add Family \"\" with family_id.
 
         Returns:
             None
         """
         raise NotImplementedError
 
-    def getSampleBySha256(self, sha256: str) -> Optional["SampleEntry"]:
+    def getSampleBySha256(self, sha256: str, is_query=False) -> Optional["SampleEntry"]:
         """Check if the given SHA256 is already associated with a sample in the storage
 
         Args:
             sha256: The SHA256 value to look up.
+            is_query: look in collection for query_samples instead of samples
 
         Returns:
             A SampleEntry with the specified SHA256 or None, if no such SampleEntry exists.
         """
         raise NotImplementedError
 
     def addSmdaReport(self, smda_report: "SmdaReport", isQuery=False) -> Optional["SampleEntry"]:
```

### Comparing `mcrit-1.3.8/mcrit/storage/UniqueBlocksResult.py` & `mcrit-1.3.9/mcrit/storage/UniqueBlocksResult.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/mcrit.egg-info/PKG-INFO` & `mcrit-1.3.9/mcrit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.3.8
+Version: 1.3.9
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
 Description: # MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
         [![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
@@ -125,14 +125,15 @@
         
         ### Reference Data 
         
         In July 2023, we started populating a [Github repository](https://github.com/danielplohmann/mcrit-data) which contains ready-to-use reference data for common compilers and libraries.
         
         
         ## Version History
+         * 2024-02-16 v1.3.9:  Finished and integrated automated queue cleanup feature (disabled by default) proposed by @yankovs - THX!!
          * 2024-02-15 v1.3.8:  Bump SMDA to address issues with version recognition in SmdaFunction, fixed exception prints in IDA plugin's McritInterface (THX to @malwarefrank!!).
          * 2024-02-12 v1.3.5:  Recalculating minhashes will now show correct percentages (THX to @malwarefrank!!).
          * 2024-02-02 v1.3.4:  Mini fix in the IDA plugin to avoid referencing a potentially uninitialized object (THX to @r0ny123!!).
          * 2024-02-01 v1.3.2:  FIX: Non-parallelized matching now outputs the [same data format](https://github.com/danielplohmann/mcrit/pull/63) (THX to @dannyquist!!).
          * 2024-01-30 v1.3.1:  The connection to MongoDB is now fully [configurable](https://github.com/danielplohmann/mcrit/pull/61) (THX to @dannyquist!!).
          * 2024-01-24 v1.3.0:  BREAKING: Milestone release with indexing improvements for PicHash and MinHash. To ensure full backward compatibility, recalculation of all hashes is recommended. Check this [migration guide](https://github.com/danielplohmann/mcrit/blob/main/docs/migration-v1.3.0.md). 
          * 2024-01-23 v1.2.26: Pinning lief to 0.13.2 in order to ensure that the pinned SMDA remains compatible.
```

### Comparing `mcrit-1.3.8/mcrit.egg-info/SOURCES.txt` & `mcrit-1.3.9/mcrit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcrit-1.3.8/setup.py` & `mcrit-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     README = f.read()
 
 setup(
     name='mcrit',
-    version="1.3.8",
+    version="1.3.9",
     description='MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.',
     long_description_content_type="text/markdown",
     long_description=README,
     author='Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko',
     author_email='daniel.plohmann@fkie.fraunhofer.de',
     url='https://github.com/danielplohmann/mcrit',
     license="NU General Public License v3 (GPLv3)",
```

