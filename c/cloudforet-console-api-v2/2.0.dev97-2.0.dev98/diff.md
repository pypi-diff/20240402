# Comparing `tmp/cloudforet-console-api-v2-2.0.dev97.tar.gz` & `tmp/cloudforet-console-api-v2-2.0.dev98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudforet-console-api-v2-2.0.dev97.tar", last modified: Fri Mar 29 02:05:27 2024, max compression
+gzip compressed data, was "cloudforet-console-api-v2-2.0.dev98.tar", last modified: Tue Apr  2 01:03:21 2024, max compression
```

## Comparing `cloudforet-console-api-v2-2.0.dev97.tar` & `cloudforet-console-api-v2-2.0.dev98.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:27.813142 cloudforet-console-api-v2-2.0.dev97/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-29 02:05:27.813142 cloudforet-console-api-v2-2.0.dev97/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:27.805142 cloudforet-console-api-v2-2.0.dev97/cloudforet/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:27.809142 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:27.809142 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/conf/global_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/conf/router_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:27.809142 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/error/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/error/cloudforet.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/error/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/error/swagger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:27.809142 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:27.809142 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/rest/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/rest/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/rest/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/rest/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/rest/swagger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:27.809142 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/manager/cloudforet_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:27.809142 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/manager/resource_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/manager/resource_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/manager/resource_manager/cost_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/manager/resource_manager/inventory_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:27.809142 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:27.809142 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/model/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/model/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/model/auth/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/model/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:27.809142 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/service/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/service/proxy_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/service/resource_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:05:27.813142 cloudforet-console-api-v2-2.0.dev97/cloudforet_console_api_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-29 02:05:27.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet_console_api_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-29 02:05:27.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet_console_api_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 02:05:27.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet_console_api_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 02:05:27.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet_console_api_v2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-29 02:05:27.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet_console_api_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 02:05:27.000000 cloudforet-console-api-v2-2.0.dev97/cloudforet_console_api_v2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 02:05:27.813142 cloudforet-console-api-v2-2.0.dev97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-29 02:05:18.000000 cloudforet-console-api-v2-2.0.dev97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:21.529193 cloudforet-console-api-v2-2.0.dev98/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-02 01:03:21.529193 cloudforet-console-api-v2-2.0.dev98/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:21.521193 cloudforet-console-api-v2-2.0.dev98/cloudforet/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:21.525193 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:21.525193 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/conf/global_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/conf/router_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:21.525193 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/error/cloudforet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/error/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/error/swagger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:21.525193 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:21.525193 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/rest/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/rest/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/rest/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/rest/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/rest/swagger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:21.525193 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/manager/cloudforet_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:21.525193 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/manager/resource_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/manager/resource_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/manager/resource_manager/cost_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/manager/resource_manager/inventory_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:21.525193 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:21.525193 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/model/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/model/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/model/auth/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/model/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:21.525193 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/service/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/service/proxy_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/service/resource_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:03:21.529193 cloudforet-console-api-v2-2.0.dev98/cloudforet_console_api_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-02 01:03:21.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet_console_api_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-02 01:03:21.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet_console_api_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:03:21.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet_console_api_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:03:21.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet_console_api_v2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 01:03:21.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet_console_api_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 01:03:21.000000 cloudforet-console-api-v2-2.0.dev98/cloudforet_console_api_v2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:03:21.529193 cloudforet-console-api-v2-2.0.dev98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-02 01:03:12.000000 cloudforet-console-api-v2-2.0.dev98/setup.py
```

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/conf/global_conf.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/conf/router_conf.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/conf/router_conf.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/rest/api.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/rest/api.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/rest/auth.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/rest/auth.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/rest/proxy.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/rest/proxy.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/rest/resource.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/rest/resource.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/interface/rest/swagger.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/interface/rest/swagger.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/manager/cloudforet_manager.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/manager/cloudforet_manager.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/manager/resource_manager/__init__.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/manager/resource_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/manager/resource_manager/cost_analysis_manager.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/manager/resource_manager/cost_analysis_manager.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/manager/resource_manager/inventory_manager.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/manager/resource_manager/inventory_manager.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/model/__init__.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/model/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/model/resource.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/model/resource.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/service/auth_service.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/service/proxy_service.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/service/proxy_service.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet/console_api_v2/service/resource_service.py` & `cloudforet-console-api-v2-2.0.dev98/cloudforet/console_api_v2/service/resource_service.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/cloudforet_console_api_v2.egg-info/SOURCES.txt` & `cloudforet-console-api-v2-2.0.dev98/cloudforet_console_api_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-2.0.dev97/setup.py` & `cloudforet-console-api-v2-2.0.dev98/setup.py`

 * *Files identical despite different names*

