# Comparing `tmp/anaplan-api-0.2.8.tar.gz` & `tmp/anaplan-api-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anaplan-api-0.2.8.tar", last modified: Wed Mar 27 03:56:21 2024, max compression
+gzip compressed data, was "anaplan-api-0.2.9.tar", last modified: Tue Apr  2 07:54:55 2024, max compression
```

## Comparing `anaplan-api-0.2.8.tar` & `anaplan-api-0.2.9.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-03-27 03:56:21.294511 anaplan-api-0.2.8/
--rw-r--r--   0 jessewilson   (502) staff       (20)     1320 2024-03-11 03:40:42.000000 anaplan-api-0.2.8/LICENSE
--rw-r--r--   0 jessewilson   (502) staff       (20)     2237 2024-03-27 03:56:21.294439 anaplan-api-0.2.8/PKG-INFO
--rw-r--r--   0 jessewilson   (502) staff       (20)     1654 2024-03-20 07:10:10.000000 anaplan-api-0.2.8/README.md
-drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-03-27 03:56:21.273598 anaplan-api-0.2.8/anaplan_api/
-drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-03-27 03:56:21.284177 anaplan-api-0.2.8/anaplan_api/anaplan/
--rw-r--r--   0 jessewilson   (502) staff       (20)     7198 2024-03-12 13:45:08.000000 anaplan-api-0.2.8/anaplan_api/anaplan/Action.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2328 2024-03-26 08:46:41.000000 anaplan-api-0.2.8/anaplan_api/anaplan/ActionParser.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2306 2024-03-25 10:40:29.000000 anaplan-api-0.2.8/anaplan_api/anaplan/ActionTask.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2559 2024-03-26 08:46:41.000000 anaplan-api-0.2.8/anaplan_api/anaplan/ExportParser.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2252 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/ExportTask.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     5185 2024-03-26 06:28:37.000000 anaplan-api-0.2.8/anaplan_api/anaplan/File.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2554 2024-03-13 04:51:10.000000 anaplan-api-0.2.8/anaplan_api/anaplan/FileDownload.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     1438 2024-03-26 05:02:42.000000 anaplan-api-0.2.8/anaplan_api/anaplan/FileUpload.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2657 2024-03-26 08:47:16.000000 anaplan-api-0.2.8/anaplan_api/anaplan/ImportParser.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2150 2024-03-26 08:39:23.000000 anaplan-api-0.2.8/anaplan_api/anaplan/ImportTask.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     6148 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/KeystoreManager.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     1537 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/Model.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     4484 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/ParameterAction.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     3898 2024-03-26 08:43:52.000000 anaplan-api-0.2.8/anaplan_api/anaplan/Parser.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     4891 2024-03-26 08:46:41.000000 anaplan-api-0.2.8/anaplan_api/anaplan/ProcessParser.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2240 2024-03-26 08:36:55.000000 anaplan-api-0.2.8/anaplan_api/anaplan/ProcessTask.py
--rw-r--r--   0 jessewilson   (502) staff       (20)      553 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/ResourceParserFile.py
--rw-r--r--   0 jessewilson   (502) staff       (20)      610 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/ResourceParserList.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     4087 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/Resources.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     1613 2024-03-26 05:02:42.000000 anaplan-api-0.2.8/anaplan_api/anaplan/StreamUpload.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     4030 2024-03-26 08:55:09.000000 anaplan-api-0.2.8/anaplan_api/anaplan/TaskController.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     1297 2024-03-12 07:07:36.000000 anaplan-api-0.2.8/anaplan_api/anaplan/TaskFactoryGenerator.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     3915 2024-03-26 06:28:37.000000 anaplan-api-0.2.8/anaplan_api/anaplan/Upload.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     1151 2024-03-12 07:52:07.000000 anaplan-api-0.2.8/anaplan_api/anaplan/UploadFactory.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     4641 2024-03-26 06:28:37.000000 anaplan-api-0.2.8/anaplan_api/anaplan/User.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     1545 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/Workspace.py
--rw-r--r--   0 jessewilson   (502) staff       (20)        0 2024-03-12 07:07:36.000000 anaplan-api-0.2.8/anaplan_api/anaplan/__init__.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     4778 2024-03-26 08:49:23.000000 anaplan-api-0.2.8/anaplan_api/anaplan/anaplan.py
-drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-03-27 03:56:21.286063 anaplan-api-0.2.8/anaplan_api/anaplan/authentication/
--rw-r--r--   0 jessewilson   (502) staff       (20)     6001 2024-03-12 13:45:08.000000 anaplan-api-0.2.8/anaplan_api/anaplan/authentication/AnaplanAuthentication.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     1052 2024-03-12 07:07:36.000000 anaplan-api-0.2.8/anaplan_api/anaplan/authentication/AuthenticationFactory.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2844 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/authentication/AuthorizationManager.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2092 2024-03-12 13:45:08.000000 anaplan-api-0.2.8/anaplan_api/anaplan/authentication/BasicAuthentication.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     5796 2024-03-12 13:45:08.000000 anaplan-api-0.2.8/anaplan_api/anaplan/authentication/CertificateAuthentication.py
--rw-r--r--   0 jessewilson   (502) staff       (20)        0 2024-03-12 07:07:36.000000 anaplan-api-0.2.8/anaplan_api/anaplan/authentication/__init__.py
-drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-03-27 03:56:21.287036 anaplan-api-0.2.8/anaplan_api/anaplan/bases/
--rw-r--r--   0 jessewilson   (502) staff       (20)      715 2024-03-12 07:07:36.000000 anaplan-api-0.2.8/anaplan_api/anaplan/bases/AnaplanResource.py
--rw-r--r--   0 jessewilson   (502) staff       (20)      479 2024-03-12 07:52:07.000000 anaplan-api-0.2.8/anaplan_api/anaplan/bases/ResourceParserFactory.py
--rw-r--r--   0 jessewilson   (502) staff       (20)      812 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/bases/TaskFactory.py
--rw-r--r--   0 jessewilson   (502) staff       (20)        0 2024-03-12 07:07:37.000000 anaplan-api-0.2.8/anaplan_api/anaplan/bases/__init__.py
-drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-03-27 03:56:21.290050 anaplan-api-0.2.8/anaplan_api/anaplan/models/
--rw-r--r--   0 jessewilson   (502) staff       (20)      821 2024-03-19 12:44:17.000000 anaplan-api-0.2.8/anaplan_api/anaplan/models/ActionResponse.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2312 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/models/AnaplanConnection.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2608 2024-03-12 13:45:08.000000 anaplan-api-0.2.8/anaplan_api/anaplan/models/AnaplanResourceFile.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2729 2024-03-12 13:45:08.000000 anaplan-api-0.2.8/anaplan_api/anaplan/models/AnaplanResourceList.py
--rw-r--r--   0 jessewilson   (502) staff       (20)      424 2024-03-12 13:45:08.000000 anaplan-api-0.2.8/anaplan_api/anaplan/models/AnaplanVersion.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     2089 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/models/AuthToken.py
--rw-r--r--   0 jessewilson   (502) staff       (20)      984 2024-03-12 07:07:37.000000 anaplan-api-0.2.8/anaplan_api/anaplan/models/ModelDetails.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     1476 2024-03-26 08:40:53.000000 anaplan-api-0.2.8/anaplan_api/anaplan/models/ParserResponse.py
--rw-r--r--   0 jessewilson   (502) staff       (20)      455 2024-03-12 07:07:37.000000 anaplan-api-0.2.8/anaplan_api/anaplan/models/TaskResponse.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     1020 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/models/UserDetails.py
--rw-r--r--   0 jessewilson   (502) staff       (20)      920 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/models/WorkspaceDetails.py
--rw-r--r--   0 jessewilson   (502) staff       (20)        0 2024-03-12 07:07:37.000000 anaplan-api-0.2.8/anaplan_api/anaplan/models/__init__.py
-drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-03-27 03:56:21.290185 anaplan-api-0.2.8/anaplan_api/anaplan/pyjks/
--rw-r--r--   0 jessewilson   (502) staff       (20)        0 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/pyjks/__init__.py
-drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-03-27 03:56:21.291627 anaplan-api-0.2.8/anaplan_api/anaplan/pyjks/jks/
--rw-r--r--   0 jessewilson   (502) staff       (20)       66 2024-03-12 07:43:20.000000 anaplan-api-0.2.8/anaplan_api/anaplan/pyjks/jks/__init__.py
--rw-r--r--   0 jessewilson   (502) staff       (20)    34591 2024-03-26 06:35:21.000000 anaplan-api-0.2.8/anaplan_api/anaplan/pyjks/jks/jks.py
--rw-r--r--   0 jessewilson   (502) staff       (20)      278 2024-03-26 06:31:25.000000 anaplan-api-0.2.8/anaplan_api/anaplan/pyjks/jks/rfc2898.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     5865 2024-03-26 06:36:45.000000 anaplan-api-0.2.8/anaplan_api/anaplan/pyjks/jks/sun_crypto.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     9765 2024-03-26 06:39:32.000000 anaplan-api-0.2.8/anaplan_api/anaplan/pyjks/jks/util.py
-drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-03-27 03:56:21.292589 anaplan-api-0.2.8/anaplan_api/anaplan/util/
--rw-r--r--   0 jessewilson   (502) staff       (20)     1246 2024-03-26 06:28:37.000000 anaplan-api-0.2.8/anaplan_api/anaplan/util/RequestHandler.py
--rw-r--r--   0 jessewilson   (502) staff       (20)      563 2024-03-12 07:07:37.000000 anaplan-api-0.2.8/anaplan_api/anaplan/util/Util.py
--rw-r--r--   0 jessewilson   (502) staff       (20)        0 2024-03-12 07:07:37.000000 anaplan-api-0.2.8/anaplan_api/anaplan/util/__init__.py
--rw-r--r--   0 jessewilson   (502) staff       (20)     1064 2024-03-12 13:45:08.000000 anaplan-api-0.2.8/anaplan_api/anaplan/util/strtobool.py
-drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-03-27 03:56:21.293943 anaplan-api-0.2.8/anaplan_api/anaplan_api.egg-info/
--rw-r--r--   0 jessewilson   (502) staff       (20)     2237 2024-03-27 03:56:21.000000 anaplan-api-0.2.8/anaplan_api/anaplan_api.egg-info/PKG-INFO
--rw-r--r--   0 jessewilson   (502) staff       (20)     2905 2024-03-27 03:56:21.000000 anaplan-api-0.2.8/anaplan_api/anaplan_api.egg-info/SOURCES.txt
--rw-r--r--   0 jessewilson   (502) staff       (20)        1 2024-03-27 03:56:21.000000 anaplan-api-0.2.8/anaplan_api/anaplan_api.egg-info/dependency_links.txt
--rw-r--r--   0 jessewilson   (502) staff       (20)      107 2024-03-27 03:56:21.000000 anaplan-api-0.2.8/anaplan_api/anaplan_api.egg-info/requires.txt
--rw-r--r--   0 jessewilson   (502) staff       (20)        8 2024-03-27 03:56:21.000000 anaplan-api-0.2.8/anaplan_api/anaplan_api.egg-info/top_level.txt
--rw-r--r--   0 jessewilson   (502) staff       (20)      354 2024-03-27 02:26:01.000000 anaplan-api-0.2.8/pyproject.toml
--rw-r--r--   0 jessewilson   (502) staff       (20)      749 2024-03-27 03:56:21.294813 anaplan-api-0.2.8/setup.cfg
--rw-r--r--   0 jessewilson   (502) staff       (20)       68 2024-03-12 04:00:03.000000 anaplan-api-0.2.8/setup.py
+drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-04-02 07:54:55.058376 anaplan-api-0.2.9/
+-rw-r--r--   0 jessewilson   (502) staff       (20)     1320 2024-03-11 03:40:42.000000 anaplan-api-0.2.9/LICENSE
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2237 2024-04-02 07:54:55.058269 anaplan-api-0.2.9/PKG-INFO
+-rw-r--r--   0 jessewilson   (502) staff       (20)     1654 2024-03-20 07:10:10.000000 anaplan-api-0.2.9/README.md
+drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-04-02 07:54:55.037427 anaplan-api-0.2.9/anaplan_api/
+drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-04-02 07:54:55.047342 anaplan-api-0.2.9/anaplan_api/anaplan/
+-rw-r--r--   0 jessewilson   (502) staff       (20)     7198 2024-04-02 04:53:08.000000 anaplan-api-0.2.9/anaplan_api/anaplan/Action.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2328 2024-03-27 03:57:54.000000 anaplan-api-0.2.9/anaplan_api/anaplan/ActionParser.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2306 2024-03-25 10:40:29.000000 anaplan-api-0.2.9/anaplan_api/anaplan/ActionTask.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2559 2024-03-27 03:57:54.000000 anaplan-api-0.2.9/anaplan_api/anaplan/ExportParser.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2252 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/ExportTask.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     5185 2024-03-27 03:57:54.000000 anaplan-api-0.2.9/anaplan_api/anaplan/File.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2527 2024-04-02 07:32:21.000000 anaplan-api-0.2.9/anaplan_api/anaplan/FileDownload.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     1438 2024-03-26 05:02:42.000000 anaplan-api-0.2.9/anaplan_api/anaplan/FileUpload.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2657 2024-03-27 03:57:54.000000 anaplan-api-0.2.9/anaplan_api/anaplan/ImportParser.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2150 2024-03-26 08:39:23.000000 anaplan-api-0.2.9/anaplan_api/anaplan/ImportTask.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     6148 2024-04-02 04:54:46.000000 anaplan-api-0.2.9/anaplan_api/anaplan/KeystoreManager.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     1537 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/Model.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     4484 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/ParameterAction.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     3898 2024-03-27 03:57:54.000000 anaplan-api-0.2.9/anaplan_api/anaplan/Parser.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     4891 2024-03-27 03:57:54.000000 anaplan-api-0.2.9/anaplan_api/anaplan/ProcessParser.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2240 2024-03-26 08:36:55.000000 anaplan-api-0.2.9/anaplan_api/anaplan/ProcessTask.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)      553 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/ResourceParserFile.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)      610 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/ResourceParserList.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     4087 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/Resources.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     1613 2024-03-26 05:02:42.000000 anaplan-api-0.2.9/anaplan_api/anaplan/StreamUpload.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     4030 2024-03-27 03:57:54.000000 anaplan-api-0.2.9/anaplan_api/anaplan/TaskController.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     1297 2024-03-12 07:07:36.000000 anaplan-api-0.2.9/anaplan_api/anaplan/TaskFactoryGenerator.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     3915 2024-03-27 03:57:54.000000 anaplan-api-0.2.9/anaplan_api/anaplan/Upload.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     1151 2024-03-12 07:52:07.000000 anaplan-api-0.2.9/anaplan_api/anaplan/UploadFactory.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     4641 2024-03-27 03:57:54.000000 anaplan-api-0.2.9/anaplan_api/anaplan/User.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     1545 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/Workspace.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)        0 2024-03-12 07:07:36.000000 anaplan-api-0.2.9/anaplan_api/anaplan/__init__.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     4772 2024-04-02 07:32:21.000000 anaplan-api-0.2.9/anaplan_api/anaplan/anaplan.py
+drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-04-02 07:54:55.048934 anaplan-api-0.2.9/anaplan_api/anaplan/authentication/
+-rw-r--r--   0 jessewilson   (502) staff       (20)     6001 2024-03-12 13:45:08.000000 anaplan-api-0.2.9/anaplan_api/anaplan/authentication/AnaplanAuthentication.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     1051 2024-04-02 07:32:21.000000 anaplan-api-0.2.9/anaplan_api/anaplan/authentication/AuthenticationFactory.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2844 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/authentication/AuthorizationManager.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2092 2024-04-02 04:55:31.000000 anaplan-api-0.2.9/anaplan_api/anaplan/authentication/BasicAuthentication.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     5796 2024-04-02 04:55:45.000000 anaplan-api-0.2.9/anaplan_api/anaplan/authentication/CertificateAuthentication.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)        0 2024-03-12 07:07:36.000000 anaplan-api-0.2.9/anaplan_api/anaplan/authentication/__init__.py
+drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-04-02 07:54:55.049813 anaplan-api-0.2.9/anaplan_api/anaplan/bases/
+-rw-r--r--   0 jessewilson   (502) staff       (20)      715 2024-03-12 07:07:36.000000 anaplan-api-0.2.9/anaplan_api/anaplan/bases/AnaplanResource.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)      479 2024-03-12 07:52:07.000000 anaplan-api-0.2.9/anaplan_api/anaplan/bases/ResourceParserFactory.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)      812 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/bases/TaskFactory.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)        0 2024-03-12 07:07:37.000000 anaplan-api-0.2.9/anaplan_api/anaplan/bases/__init__.py
+drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-04-02 07:54:55.053832 anaplan-api-0.2.9/anaplan_api/anaplan/models/
+-rw-r--r--   0 jessewilson   (502) staff       (20)      821 2024-03-27 03:57:54.000000 anaplan-api-0.2.9/anaplan_api/anaplan/models/ActionResponse.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2312 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/models/AnaplanConnection.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2608 2024-03-12 13:45:08.000000 anaplan-api-0.2.9/anaplan_api/anaplan/models/AnaplanResourceFile.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2729 2024-03-12 13:45:08.000000 anaplan-api-0.2.9/anaplan_api/anaplan/models/AnaplanResourceList.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)      424 2024-03-12 13:45:08.000000 anaplan-api-0.2.9/anaplan_api/anaplan/models/AnaplanVersion.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2089 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/models/AuthToken.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)      984 2024-03-12 07:07:37.000000 anaplan-api-0.2.9/anaplan_api/anaplan/models/ModelDetails.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     1476 2024-03-27 03:57:54.000000 anaplan-api-0.2.9/anaplan_api/anaplan/models/ParserResponse.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)      455 2024-03-12 07:07:37.000000 anaplan-api-0.2.9/anaplan_api/anaplan/models/TaskResponse.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     1020 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/models/UserDetails.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)      920 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/models/WorkspaceDetails.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)        0 2024-03-12 07:07:37.000000 anaplan-api-0.2.9/anaplan_api/anaplan/models/__init__.py
+drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-04-02 07:54:55.053957 anaplan-api-0.2.9/anaplan_api/anaplan/pyjks/
+-rw-r--r--   0 jessewilson   (502) staff       (20)        0 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/pyjks/__init__.py
+drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-04-02 07:54:55.055627 anaplan-api-0.2.9/anaplan_api/anaplan/pyjks/jks/
+-rw-r--r--   0 jessewilson   (502) staff       (20)       66 2024-03-12 07:43:20.000000 anaplan-api-0.2.9/anaplan_api/anaplan/pyjks/jks/__init__.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)    34591 2024-03-26 06:35:21.000000 anaplan-api-0.2.9/anaplan_api/anaplan/pyjks/jks/jks.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)      278 2024-03-26 06:31:25.000000 anaplan-api-0.2.9/anaplan_api/anaplan/pyjks/jks/rfc2898.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     5865 2024-03-26 06:36:45.000000 anaplan-api-0.2.9/anaplan_api/anaplan/pyjks/jks/sun_crypto.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     9765 2024-03-26 06:39:32.000000 anaplan-api-0.2.9/anaplan_api/anaplan/pyjks/jks/util.py
+drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-04-02 07:54:55.056743 anaplan-api-0.2.9/anaplan_api/anaplan/util/
+-rw-r--r--   0 jessewilson   (502) staff       (20)     1246 2024-03-27 03:57:54.000000 anaplan-api-0.2.9/anaplan_api/anaplan/util/RequestHandler.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)      506 2024-04-02 07:32:21.000000 anaplan-api-0.2.9/anaplan_api/anaplan/util/Util.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)        0 2024-03-12 07:07:37.000000 anaplan-api-0.2.9/anaplan_api/anaplan/util/__init__.py
+-rw-r--r--   0 jessewilson   (502) staff       (20)     1064 2024-03-12 13:45:08.000000 anaplan-api-0.2.9/anaplan_api/anaplan/util/strtobool.py
+drwxr-xr-x   0 jessewilson   (502) staff       (20)        0 2024-04-02 07:54:55.057920 anaplan-api-0.2.9/anaplan_api/anaplan_api.egg-info/
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2237 2024-04-02 07:54:55.000000 anaplan-api-0.2.9/anaplan_api/anaplan_api.egg-info/PKG-INFO
+-rw-r--r--   0 jessewilson   (502) staff       (20)     2905 2024-04-02 07:54:55.000000 anaplan-api-0.2.9/anaplan_api/anaplan_api.egg-info/SOURCES.txt
+-rw-r--r--   0 jessewilson   (502) staff       (20)        1 2024-04-02 07:54:55.000000 anaplan-api-0.2.9/anaplan_api/anaplan_api.egg-info/dependency_links.txt
+-rw-r--r--   0 jessewilson   (502) staff       (20)      107 2024-04-02 07:54:55.000000 anaplan-api-0.2.9/anaplan_api/anaplan_api.egg-info/requires.txt
+-rw-r--r--   0 jessewilson   (502) staff       (20)        8 2024-04-02 07:54:55.000000 anaplan-api-0.2.9/anaplan_api/anaplan_api.egg-info/top_level.txt
+-rw-r--r--   0 jessewilson   (502) staff       (20)      354 2024-04-02 07:54:40.000000 anaplan-api-0.2.9/pyproject.toml
+-rw-r--r--   0 jessewilson   (502) staff       (20)      749 2024-04-02 07:54:55.058727 anaplan-api-0.2.9/setup.cfg
+-rw-r--r--   0 jessewilson   (502) staff       (20)       68 2024-03-12 04:00:03.000000 anaplan-api-0.2.9/setup.py
```

### Comparing `anaplan-api-0.2.8/LICENSE` & `anaplan-api-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/PKG-INFO` & `anaplan-api-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anaplan-api
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Python wrapper for the Anaplan Bulk API
 Home-page: https://github.com/jeswils-ap/anaplan-api
 Author: Jesse Wilson
 Author-email: jeswils@gmail.com
 License: BSD-2-Clause
 Keywords: anaplan
 Classifier: Programming Language :: Python :: 3
```

### Comparing `anaplan-api-0.2.8/README.md` & `anaplan-api-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/Action.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/Action.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/ActionParser.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/ActionParser.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/ActionTask.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/ActionTask.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/ExportParser.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/ExportParser.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/ExportTask.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/ExportTask.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/File.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/File.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/FileDownload.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/FileDownload.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         :rtype: str
         """
         conn = self._conn
         endpoint = f"{super().endpoint}chunks/"
         current_chunk = 0
 
         file_data = []
-        file_contents = {}
 
         get_header = {
             "Authorization": conn.authorization.token_value,
         }
 
         while int(current_chunk) < int(self._chunk_count):
             try:
```

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/FileUpload.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/FileUpload.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/ImportParser.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/ImportParser.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/ImportTask.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/ImportTask.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/KeystoreManager.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/KeystoreManager.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/Model.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/Model.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/ParameterAction.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/ParameterAction.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/Parser.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/Parser.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/ProcessParser.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/ProcessParser.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/ProcessTask.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/ProcessTask.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/ResourceParserFile.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/ResourceParserFile.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/ResourceParserList.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/ResourceParserList.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/Resources.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/Resources.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/StreamUpload.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/StreamUpload.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/TaskController.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/TaskController.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/TaskFactoryGenerator.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/TaskFactoryGenerator.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/Upload.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/Upload.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/UploadFactory.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/UploadFactory.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/User.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/User.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/Workspace.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/Workspace.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/anaplan.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/anaplan.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Created:        11 Sep 2018
 # @author:        Jesse Wilson (Anaplan Asia Pte Ltd)
 # Description:    Library to implement Anaplan API to get lists of model resources, upload files to Anaplan server,
 #                 download files from Anaplan server, and execute actions.
 # ===============================================================================
 from __future__ import annotations
 import logging
-from typing import List, TYPE_CHECKING
+from typing import TYPE_CHECKING
 from .authentication.AuthorizationManager import AuthorizationManager
 from .UploadFactory import UploadFactory
 from .TaskController import TaskController
 from .Resources import Resources
 from .ResourceParserList import ResourceParserList
 from .FileDownload import FileDownload
```

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/authentication/AnaplanAuthentication.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/authentication/AnaplanAuthentication.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/authentication/AuthenticationFactory.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/authentication/AuthenticationFactory.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def create_authentication(method, **kwargs):
         if method not in AuthenticationFactory._auth_classes:
             raise ValueError(
                 f"Invalid authentication method: {method}. Should be one of {', '.join(AuthenticationFactory._auth_classes.keys())}"
             )
 
         auth_class = AuthenticationFactory._auth_classes[method]
-        required_params = auth_class._required_params
+        required_params = auth_class.required_params
 
         provided_params = set(kwargs.keys())
         missing_params = required_params - provided_params
 
         if missing_params:
             raise ValueError(
                 f"Missing required parameters for {method} authentication: {missing_params}"
```

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/authentication/AuthorizationManager.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/authentication/AuthorizationManager.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/authentication/BasicAuthentication.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/authentication/BasicAuthentication.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/authentication/CertificateAuthentication.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/authentication/CertificateAuthentication.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/bases/AnaplanResource.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/bases/AnaplanResource.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/bases/TaskFactory.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/bases/TaskFactory.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/models/ActionResponse.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/models/ActionResponse.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/models/AnaplanConnection.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/models/AnaplanConnection.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/models/AnaplanResourceFile.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/models/AnaplanResourceFile.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/models/AnaplanResourceList.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/models/AnaplanResourceList.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/models/AuthToken.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/models/AuthToken.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/models/ModelDetails.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/models/ModelDetails.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/models/ParserResponse.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/models/ParserResponse.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/models/UserDetails.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/models/UserDetails.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/models/WorkspaceDetails.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/models/WorkspaceDetails.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/pyjks/jks/jks.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/pyjks/jks/jks.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/pyjks/jks/sun_crypto.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/pyjks/jks/sun_crypto.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/pyjks/jks/util.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/pyjks/jks/util.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/util/RequestHandler.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/util/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan/util/strtobool.py` & `anaplan-api-0.2.9/anaplan_api/anaplan/util/strtobool.py`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan_api.egg-info/PKG-INFO` & `anaplan-api-0.2.9/anaplan_api/anaplan_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anaplan-api
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Python wrapper for the Anaplan Bulk API
 Home-page: https://github.com/jeswils-ap/anaplan-api
 Author: Jesse Wilson
 Author-email: jeswils@gmail.com
 License: BSD-2-Clause
 Keywords: anaplan
 Classifier: Programming Language :: Python :: 3
```

### Comparing `anaplan-api-0.2.8/anaplan_api/anaplan_api.egg-info/SOURCES.txt` & `anaplan-api-0.2.9/anaplan_api/anaplan_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anaplan-api-0.2.8/setup.cfg` & `anaplan-api-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = anaplan-api
-version = 0.2.8
+version = 0.2.9
 author = Jesse Wilson
 author_email = jeswils@gmail.com
 description = A Python wrapper for the Anaplan Bulk API
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = BSD-2-Clause
 url = https://github.com/jeswils-ap/anaplan-api
```

