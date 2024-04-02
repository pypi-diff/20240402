# Comparing `tmp/kimchima-0.2.1.tar.gz` & `tmp/kimchima-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimchima-0.2.1.tar", max compression
+gzip compressed data, was "kimchima-0.2.2.tar", max compression
```

## Comparing `kimchima-0.2.1.tar` & `kimchima-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0    11343 2024-03-31 12:59:59.909937 kimchima-0.2.1/LICENSE
--rw-r--r--   0        0        0      867 2024-03-31 12:59:59.913937 kimchima-0.2.1/README.md
--rw-r--r--   0        0        0       49 2024-03-31 12:59:59.913937 kimchima-0.2.1/pkg/__init__.py
--rw-r--r--   0        0        0       31 2024-03-31 12:59:59.913937 kimchima-0.2.1/pkg/auto/__init__.py
--rw-r--r--   0        0        0     3298 2024-03-31 12:59:59.913937 kimchima-0.2.1/pkg/auto/auto.py
--rw-r--r--   0        0        0       33 2024-03-31 12:59:59.913937 kimchima-0.2.1/pkg/devices/__init__.py
--rw-r--r--   0        0        0      987 2024-03-31 12:59:59.913937 kimchima-0.2.1/pkg/devices/devices.py
--rw-r--r--   0        0        0      663 2024-03-31 13:05:34.981923 kimchima-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 kimchima-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-02 12:46:40.224640 kimchima-0.2.2/LICENSE
+-rw-r--r--   0        0        0      647 2024-04-02 12:46:40.228640 kimchima-0.2.2/README.md
+-rw-r--r--   0        0        0      620 2024-04-02 12:46:40.228640 kimchima-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      688 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/cmds/__init__.py
+-rw-r--r--   0        0        0     1577 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/cmds/auto_cli.py
+-rw-r--r--   0        0        0     1334 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/cmds/kimchima_cli.py
+-rw-r--r--   0        0        0       95 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/pkg/__init__.py
+-rw-r--r--   0        0        0     3298 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/pkg/auto.py
+-rw-r--r--   0        0        0     1469 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/pkg/devices.py
+-rw-r--r--   0        0        0        0 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/tests/__init__.py
+-rw-r--r--   0        0        0     1386 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/tests/test_auto.py
+-rw-r--r--   0        0        0     1766 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/tests/test_devices.py
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 kimchima-0.2.2/PKG-INFO
```

### Comparing `kimchima-0.2.1/LICENSE` & `kimchima-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kimchima-0.2.1/pkg/auto/auto.py` & `kimchima-0.2.2/src/kimchima/pkg/auto.py`

 * *Files identical despite different names*

