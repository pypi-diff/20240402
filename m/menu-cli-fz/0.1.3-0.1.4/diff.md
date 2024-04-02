# Comparing `tmp/menu_cli_fz-0.1.3.tar.gz` & `tmp/menu_cli_fz-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "menu_cli_fz-0.1.3.tar", max compression
+gzip compressed data, was "menu_cli_fz-0.1.4.tar", max compression
```

## Comparing `menu_cli_fz-0.1.3.tar` & `menu_cli_fz-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-02 12:54:28.705738 menu_cli_fz-0.1.3/menu_cli_fz/__init__.py
--rw-r--r--   0        0        0       64 2024-04-02 14:40:11.254391 menu_cli_fz-0.1.3/menu_cli_fz/__main__.py
--rw-r--r--   0        0        0     2172 2024-04-02 14:37:59.417085 menu_cli_fz-0.1.3/menu_cli_fz/main.py
--rw-r--r--   0        0        0      417 2024-04-02 14:46:52.525489 menu_cli_fz-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 12:54:28.706738 menu_cli_fz-0.1.3/README.md
--rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 menu_cli_fz-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-02 12:54:28.705738 menu_cli_fz-0.1.4/menu_cli_fz/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-02 14:40:11.254391 menu_cli_fz-0.1.4/menu_cli_fz/__main__.py
+-rw-r--r--   0        0        0     2172 2024-04-02 14:37:59.417085 menu_cli_fz-0.1.4/menu_cli_fz/main.py
+-rw-r--r--   0        0        0      423 2024-04-02 14:48:42.624030 menu_cli_fz-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 12:54:28.706738 menu_cli_fz-0.1.4/README.md
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 menu_cli_fz-0.1.4/PKG-INFO
```

### Comparing `menu_cli_fz-0.1.3/menu_cli_fz/main.py` & `menu_cli_fz-0.1.4/menu_cli_fz/main.py`

 * *Files identical despite different names*

