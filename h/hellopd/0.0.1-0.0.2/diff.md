# Comparing `tmp/hellopd-0.0.1.tar.gz` & `tmp/hellopd-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hellopd-0.0.1.tar", last modified: Tue Apr  2 07:03:38 2024, max compression
+gzip compressed data, was "hellopd-0.0.2.tar", last modified: Tue Apr  2 07:10:47 2024, max compression
```

## Comparing `hellopd-0.0.1.tar` & `hellopd-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 07:03:38.416224 hellopd-0.0.1/
--rw-rw-rw-   0        0        0      142 2024-04-02 07:03:38.415221 hellopd-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-02 06:57:23.000000 hellopd-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 07:03:38.392222 hellopd-0.0.1/hellopd/
--rw-rw-rw-   0        0        0       25 2024-04-02 06:59:02.000000 hellopd-0.0.1/hellopd/__init__.py
--rw-rw-rw-   0        0        0       56 2024-04-02 06:59:12.000000 hellopd-0.0.1/hellopd/main.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:03:38.413778 hellopd-0.0.1/hellopd.egg-info/
--rw-rw-rw-   0        0        0      142 2024-04-02 07:03:38.000000 hellopd-0.0.1/hellopd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2024-04-02 07:03:38.000000 hellopd-0.0.1/hellopd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 07:03:38.000000 hellopd-0.0.1/hellopd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-02 07:03:38.000000 hellopd-0.0.1/hellopd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 07:03:38.416224 hellopd-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      166 2024-04-02 07:01:00.000000 hellopd-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:10:47.981679 hellopd-0.0.2/
+-rw-rw-rw-   0        0        0      142 2024-04-02 07:10:47.980682 hellopd-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-02 06:57:23.000000 hellopd-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 07:10:47.949050 hellopd-0.0.2/hellopd/
+-rw-rw-rw-   0        0        0       25 2024-04-02 06:59:02.000000 hellopd-0.0.2/hellopd/__init__.py
+-rw-rw-rw-   0        0        0       56 2024-04-02 06:59:12.000000 hellopd-0.0.2/hellopd/main.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:10:47.979716 hellopd-0.0.2/hellopd.egg-info/
+-rw-rw-rw-   0        0        0      142 2024-04-02 07:10:47.000000 hellopd-0.0.2/hellopd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-04-02 07:10:47.000000 hellopd-0.0.2/hellopd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 07:10:47.000000 hellopd-0.0.2/hellopd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-02 07:10:47.000000 hellopd-0.0.2/hellopd.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-04-02 07:10:47.000000 hellopd-0.0.2/hellopd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 07:10:47.981679 hellopd-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      272 2024-04-02 07:10:21.000000 hellopd-0.0.2/setup.py
```

