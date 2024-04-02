# Comparing `tmp/databind.json-4.4.2.tar.gz` & `tmp/databind_json-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind.json-4.4.2.tar", max compression
+gzip compressed data, was "databind_json-4.5.0.tar", max compression
```

## Comparing `databind.json-4.4.2.tar` & `databind_json-4.5.0.tar`

### file list

```diff
@@ -1,10 +1,4 @@
--rw-r--r--   0        0        0     3339 2023-11-11 12:23:10.179056 databind.json-4.4.2/README.md
--rw-r--r--   0        0        0     1654 2023-11-11 12:37:34.565533 databind.json-4.4.2/pyproject.toml
--rw-r--r--   0        0        0     2411 2023-11-11 12:37:34.565533 databind.json-4.4.2/src/databind/json/__init__.py
--rw-r--r--   0        0        0    35510 2023-11-11 12:23:10.179056 databind.json-4.4.2/src/databind/json/converters.py
--rw-r--r--   0        0        0     2952 2023-11-11 12:23:10.179056 databind.json-4.4.2/src/databind/json/module.py
--rw-r--r--   0        0        0        0 2023-11-11 12:23:10.179056 databind.json-4.4.2/src/databind/json/py.typed
--rw-r--r--   0        0        0     1933 2023-11-11 12:23:10.179056 databind.json-4.4.2/src/databind/json/settings.py
--rw-r--r--   0        0        0    27496 2023-11-11 12:23:10.179056 databind.json-4.4.2/src/databind/json/tests/converters_test.py
--rw-r--r--   0        0        0     4251 2023-11-11 12:37:42.610925 databind.json-4.4.2/setup.py
--rw-r--r--   0        0        0     4373 2023-11-11 12:37:42.611190 databind.json-4.4.2/PKG-INFO
+-rw-r--r--   0        0        0      157 2024-03-19 19:49:02.841346 databind_json-4.5.0/README.md
+-rw-r--r--   0        0        0      792 2024-03-19 19:50:25.488974 databind_json-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-03-19 19:42:46.046308 databind_json-4.5.0/src/_databind_json_proxy.py
+-rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 databind_json-4.5.0/PKG-INFO
```

