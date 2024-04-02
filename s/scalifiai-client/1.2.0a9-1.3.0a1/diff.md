# Comparing `tmp/scalifiai-client-1.2.0a9.tar.gz` & `tmp/scalifiai-client-1.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalifiai-client-1.2.0a9.tar", last modified: Mon Apr  1 15:50:04 2024, max compression
+gzip compressed data, was "scalifiai-client-1.3.0a1.tar", last modified: Mon Apr  1 18:37:05 2024, max compression
```

## Comparing `scalifiai-client-1.2.0a9.tar` & `scalifiai-client-1.3.0a1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:50:04.758211 scalifiai-client-1.2.0a9/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.2.0a9/LICENSE
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      899 2024-04-01 15:50:04.758211 scalifiai-client-1.2.0a9/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.2.0a9/README.md
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      971 2024-04-01 15:49:53.000000 scalifiai-client-1.2.0a9/pyproject.toml
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:50:04.750211 scalifiai-client-1.2.0a9/scalifiai/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a9/scalifiai/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6401 2024-04-01 15:40:25.000000 scalifiai-client-1.2.0a9/scalifiai/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-03-30 16:03:04.000000 scalifiai-client-1.2.0a9/scalifiai/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a9/scalifiai/credentials.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a9/scalifiai/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:50:04.750211 scalifiai-client-1.2.0a9/scalifiai/mcs/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-02-22 09:41:30.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:50:04.754212 scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:50:04.754212 scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/keras/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/keras/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       63 2024-02-19 07:02:09.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/keras/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-03-29 10:10:16.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/keras/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    11074 2024-03-31 04:37:07.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/keras/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-02-28 14:26:26.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/schema.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1800 2024-04-01 13:26:53.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/utils.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/main.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:50:04.754212 scalifiai-client-1.2.0a9/scalifiai/mcs/metadata/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/metadata/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-01 07:00:53.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/metadata/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-03-30 16:01:07.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/metadata/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13378 2024-04-01 15:40:31.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/metadata/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-02-28 12:22:03.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/metadata/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:50:04.754212 scalifiai-client-1.2.0a9/scalifiai/mcs/model/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/model/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-03-30 11:24:30.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/model/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-03-30 15:59:35.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/model/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    34019 2024-04-01 15:37:25.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/model/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/model/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:50:04.754212 scalifiai-client-1.2.0a9/scalifiai/mcs/model_version/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/model_version/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-03-30 11:20:38.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/model_version/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-03-30 15:58:50.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/model_version/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28463 2024-04-01 15:40:35.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/model_version/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-03-30 13:31:27.000000 scalifiai-client-1.2.0a9/scalifiai/mcs/model_version/schemas.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-03-30 16:03:04.000000 scalifiai-client-1.2.0a9/scalifiai/request_manager.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 15:50:04.758211 scalifiai-client-1.2.0a9/scalifiai_client.egg-info/
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      899 2024-04-01 15:50:04.000000 scalifiai-client-1.2.0a9/scalifiai_client.egg-info/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1353 2024-04-01 15:50:04.000000 scalifiai-client-1.2.0a9/scalifiai_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-01 15:50:04.000000 scalifiai-client-1.2.0a9/scalifiai_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      138 2024-04-01 15:50:04.000000 scalifiai-client-1.2.0a9/scalifiai_client.egg-info/requires.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-01 15:50:04.000000 scalifiai-client-1.2.0a9/scalifiai_client.egg-info/top_level.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-01 15:50:04.758211 scalifiai-client-1.2.0a9/setup.cfg
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 18:37:05.477814 scalifiai-client-1.3.0a1/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.3.0a1/LICENSE
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      908 2024-04-01 18:37:05.477814 scalifiai-client-1.3.0a1/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-03-01 10:40:07.000000 scalifiai-client-1.3.0a1/README.md
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      982 2024-04-01 18:34:59.000000 scalifiai-client-1.3.0a1/pyproject.toml
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 18:37:05.461813 scalifiai-client-1.3.0a1/scalifiai/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-02-19 06:55:52.000000 scalifiai-client-1.3.0a1/scalifiai/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6401 2024-04-01 15:40:25.000000 scalifiai-client-1.3.0a1/scalifiai/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-03-30 16:03:04.000000 scalifiai-client-1.3.0a1/scalifiai/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-02-19 06:55:52.000000 scalifiai-client-1.3.0a1/scalifiai/credentials.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-03-30 13:31:27.000000 scalifiai-client-1.3.0a1/scalifiai/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 18:37:05.465813 scalifiai-client-1.3.0a1/scalifiai/mcs/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-02-22 09:41:30.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-02-19 06:55:52.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-03-30 13:31:27.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 18:37:05.465813 scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-02-19 06:55:52.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-03-30 13:31:27.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 18:37:05.469813 scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/keras/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/keras/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       63 2024-02-19 07:02:09.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/keras/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-03-29 10:10:16.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/keras/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    10912 2024-04-01 18:30:11.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/keras/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-02-28 14:26:26.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/schema.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1800 2024-04-01 13:26:53.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/utils.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-03-30 13:31:27.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/main.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 18:37:05.469813 scalifiai-client-1.3.0a1/scalifiai/mcs/metadata/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/metadata/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-01 07:00:53.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/metadata/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-03-30 16:01:07.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/metadata/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13378 2024-04-01 15:40:31.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/metadata/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-02-28 12:22:03.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/metadata/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 18:37:05.469813 scalifiai-client-1.3.0a1/scalifiai/mcs/model/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/model/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-03-30 11:24:30.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/model/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-03-30 15:59:35.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/model/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    34019 2024-04-01 15:37:25.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/model/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-03-30 13:31:27.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/model/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 18:37:05.473814 scalifiai-client-1.3.0a1/scalifiai/mcs/model_version/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-02-19 06:55:52.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/model_version/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-03-30 11:20:38.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/model_version/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-03-30 15:58:50.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/model_version/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28463 2024-04-01 15:40:35.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/model_version/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-03-30 13:31:27.000000 scalifiai-client-1.3.0a1/scalifiai/mcs/model_version/schemas.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-03-30 16:03:04.000000 scalifiai-client-1.3.0a1/scalifiai/request_manager.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-01 18:37:05.473814 scalifiai-client-1.3.0a1/scalifiai_client.egg-info/
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      908 2024-04-01 18:37:05.000000 scalifiai-client-1.3.0a1/scalifiai_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1353 2024-04-01 18:37:05.000000 scalifiai-client-1.3.0a1/scalifiai_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-01 18:37:05.000000 scalifiai-client-1.3.0a1/scalifiai_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      147 2024-04-01 18:37:05.000000 scalifiai-client-1.3.0a1/scalifiai_client.egg-info/requires.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-01 18:37:05.000000 scalifiai-client-1.3.0a1/scalifiai_client.egg-info/top_level.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-01 18:37:05.477814 scalifiai-client-1.3.0a1/setup.cfg
```

### Comparing `scalifiai-client-1.2.0a9/PKG-INFO` & `scalifiai-client-1.3.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.2.0a9
+Version: 1.3.0a1
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,12 +12,12 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pandas>=1.3.0
 Requires-Dist: humanize>=2.0.0
 Requires-Dist: tzlocal>=2.1
 Provides-Extra: tf
-Requires-Dist: tensorflow==2.2.0; extra == "tf"
+Requires-Dist: tensorflow<=2.15.1,>=2.2.0; extra == "tf"
 Requires-Dist: pydantic>=2.0; extra == "tf"
 Requires-Dist: pandas>=1.3.0; extra == "tf"
 Requires-Dist: humanize>=2.0.0; extra == "tf"
 Requires-Dist: tzlocal>=2.1; extra == "tf"
```

### Comparing `scalifiai-client-1.2.0a9/pyproject.toml` & `scalifiai-client-1.3.0a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scalifiai-client"
-version = "1.2.0-alpha.9"
+version = "1.3.0-alpha.1"
 description = "SCALIFI AI NO CODE PLATFORM"
 readme = "README.md"
 authors = [{ name = "Scalifi Ai", email = "helpdesk@scalifiai.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -21,15 +21,15 @@
     "humanize >= 2.0.0",
     "tzlocal >= 2.1",
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 tf = [
-    "tensorflow == 2.2.0",
+    "tensorflow >= 2.2.0, <= 2.15.1",
     "pydantic >= 2.0",
     "pandas >= 1.3.0",
     "humanize >= 2.0.0",
     "tzlocal >= 2.1",
 ]
 
 [project.urls]
```

### Comparing `scalifiai-client-1.2.0a9/scalifiai/base.py` & `scalifiai-client-1.3.0a1/scalifiai/base.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/credentials.py` & `scalifiai-client-1.3.0a1/scalifiai/credentials.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/exceptions.py` & `scalifiai-client-1.3.0a1/scalifiai/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/exceptions.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/exceptions.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/keras/exceptions.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/keras/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/keras/main.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/keras/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,25 +153,22 @@
         request_manager=None,
         upload_url=None,
         parent_action=None,
         model_instance=None,
     ):
 
         from scalifiai.mcs.model_version.main import ModelVersion
-        # import tensorflow as tf
 
         with tempfile.TemporaryDirectory(dir=base_dir_path) as temp_dir:
 
             temp_dir_path = Path(temp_dir)
             model_save_file_path = temp_dir_path / Path(MODEL_SAVE_FOLDER_NAME)
 
             try:
                 self.model.save(model_save_file_path, save_format="tf")
-                # self.model.save(model_save_file_path)
-                # tf.saved_model.save(self.model, model_save_file_path)
             except Exception as ex:
                 print(f"type(ex): {type(ex)}")
                 print(f"ex: {ex}")
                 try:
                     raise KerasInvalidModelException(extra_info=str(ex))
                 except Exception as ex:
                     raise KerasInvalidModelException()
```

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/schema.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/schema.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/frameworks/utils.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/frameworks/utils.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/main.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/metadata/exceptions.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/metadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/metadata/main.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/metadata/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/metadata/schemas.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/metadata/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/model/constants.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/model/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/model/exceptions.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/model/main.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/model/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/model/schemas.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/model/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/model_version/constants.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/model_version/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/model_version/exceptions.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/model_version/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/model_version/main.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/model_version/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/mcs/model_version/schemas.py` & `scalifiai-client-1.3.0a1/scalifiai/mcs/model_version/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai/request_manager.py` & `scalifiai-client-1.3.0a1/scalifiai/request_manager.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.2.0a9/scalifiai_client.egg-info/PKG-INFO` & `scalifiai-client-1.3.0a1/scalifiai_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.2.0a9
+Version: 1.3.0a1
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,12 +12,12 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pandas>=1.3.0
 Requires-Dist: humanize>=2.0.0
 Requires-Dist: tzlocal>=2.1
 Provides-Extra: tf
-Requires-Dist: tensorflow==2.2.0; extra == "tf"
+Requires-Dist: tensorflow<=2.15.1,>=2.2.0; extra == "tf"
 Requires-Dist: pydantic>=2.0; extra == "tf"
 Requires-Dist: pandas>=1.3.0; extra == "tf"
 Requires-Dist: humanize>=2.0.0; extra == "tf"
 Requires-Dist: tzlocal>=2.1; extra == "tf"
```

### Comparing `scalifiai-client-1.2.0a9/scalifiai_client.egg-info/SOURCES.txt` & `scalifiai-client-1.3.0a1/scalifiai_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

