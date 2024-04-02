# Comparing `tmp/utils_huna-0.1.7.tar.gz` & `tmp/utils_huna-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_huna-0.1.7.tar", last modified: Mon Apr  1 18:14:03 2024, max compression
+gzip compressed data, was "utils_huna-0.1.8.tar", last modified: Tue Apr  2 19:40:18 2024, max compression
```

## Comparing `utils_huna-0.1.7.tar` & `utils_huna-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 18:14:03.385572 utils_huna-0.1.7/
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-01 18:14:03.385572 utils_huna-0.1.7/PKG-INFO
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      326 2024-03-18 14:37:13.000000 utils_huna-0.1.7/README.md
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       38 2024-04-01 18:14:03.385572 utils_huna-0.1.7/setup.cfg
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      204 2024-04-01 18:13:51.000000 utils_huna-0.1.7/setup.py
-drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 18:14:03.385572 utils_huna-0.1.7/utils_huna/
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       17 2024-04-01 17:00:32.000000 utils_huna-0.1.7/utils_huna/__init__.py
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      449 2024-04-01 18:13:17.000000 utils_huna-0.1.7/utils_huna/utils.py
-drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 18:14:03.385572 utils_huna-0.1.7/utils_huna.egg-info/
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-01 18:14:03.000000 utils_huna-0.1.7/utils_huna.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      197 2024-04-01 18:14:03.000000 utils_huna-0.1.7/utils_huna.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)        1 2024-04-01 18:14:03.000000 utils_huna-0.1.7/utils_huna.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       11 2024-04-01 18:14:03.000000 utils_huna-0.1.7/utils_huna.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-02 19:40:18.947942 utils_huna-0.1.8/
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-02 19:40:18.947942 utils_huna-0.1.8/PKG-INFO
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      326 2024-03-18 14:37:13.000000 utils_huna-0.1.8/README.md
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       38 2024-04-02 19:40:18.947942 utils_huna-0.1.8/setup.cfg
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      204 2024-04-02 19:39:02.000000 utils_huna-0.1.8/setup.py
+drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-02 19:40:18.947942 utils_huna-0.1.8/utils_huna/
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       17 2024-04-01 17:00:32.000000 utils_huna-0.1.8/utils_huna/__init__.py
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      666 2024-04-02 19:37:54.000000 utils_huna-0.1.8/utils_huna/utils.py
+drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-02 19:40:18.947942 utils_huna-0.1.8/utils_huna.egg-info/
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-02 19:40:18.000000 utils_huna-0.1.8/utils_huna.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      197 2024-04-02 19:40:18.000000 utils_huna-0.1.8/utils_huna.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)        1 2024-04-02 19:40:18.000000 utils_huna-0.1.8/utils_huna.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       11 2024-04-02 19:40:18.000000 utils_huna-0.1.8/utils_huna.egg-info/top_level.txt
```

