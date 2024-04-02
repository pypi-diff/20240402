# Comparing `tmp/ytmusic_deleter-2.1.1a1.tar.gz` & `tmp/ytmusic_deleter-2.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusic_deleter-2.1.1a1.tar", last modified: Sat Mar 23 01:26:36 2024, max compression
+gzip compressed data, was "ytmusic_deleter-2.1.2a0.tar", last modified: Tue Apr  2 02:07:28 2024, max compression
```

## Comparing `ytmusic_deleter-2.1.1a1.tar` & `ytmusic_deleter-2.1.2a0.tar`

### file list

```diff
@@ -1,10 +1,4 @@
--rw-r--r--   0        0        0     4027 2024-03-23 01:15:00.755947 ytmusic_deleter-2.1.1a1/./README.md
--rw-r--r--   0        0        0      490 2024-03-23 01:26:36.714262 ytmusic_deleter-2.1.1a1/pyproject.toml
--rw-r--r--   0        0        0     1164 2024-03-23 01:15:00.755947 ytmusic_deleter-2.1.1a1/src/auth.py
--rw-r--r--   0        0        0    14801 2024-03-23 01:15:00.755947 ytmusic_deleter-2.1.1a1/src/cli.py
--rw-r--r--   0        0        0      168 2024-03-23 01:15:00.755947 ytmusic_deleter-2.1.1a1/src/constants.py
--rw-r--r--   0        0        0      290 2024-03-23 01:15:00.755947 ytmusic_deleter-2.1.1a1/src/progress.py
--rw-r--r--   0        0        0     9314 2024-03-23 01:15:00.755947 ytmusic_deleter-2.1.1a1/src/uploads.py
--rw-r--r--   0        0        0        0 2024-03-23 01:15:00.755947 ytmusic_deleter-2.1.1a1/tests/__init__.py
--rw-r--r--   0        0        0      770 2024-03-23 01:15:00.755947 ytmusic_deleter-2.1.1a1/tests/test_cli.py
--rw-r--r--   0        0        0     4353 1970-01-01 00:00:00.000000 ytmusic_deleter-2.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0     3750 2024-03-26 02:39:07.905706 ytmusic_deleter-2.1.2a0/./README.md
+-rw-r--r--   0        0        0    35149 2024-03-03 22:51:33.484508 ytmusic_deleter-2.1.2a0/LICENSE
+-rw-r--r--   0        0        0     1141 2024-04-02 02:07:28.050764 ytmusic_deleter-2.1.2a0/pyproject.toml
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 ytmusic_deleter-2.1.2a0/PKG-INFO
```

