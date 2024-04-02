# Comparing `tmp/bu9-9.20.tar.gz` & `tmp/bu9-9.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bu9-9.20.tar", last modified: Tue Apr  2 12:35:06 2024, max compression
+gzip compressed data, was "bu9-9.21.tar", last modified: Tue Apr  2 13:37:19 2024, max compression
```

## Comparing `bu9-9.20.tar` & `bu9-9.21.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 12:35:06.285143 bu9-9.20/
--rw-rw-rw-   0        0        0       49 2024-04-02 12:35:06.283143 bu9-9.20/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 12:35:06.281144 bu9-9.20/bu9.egg-info/
--rw-rw-rw-   0        0        0       49 2024-04-02 12:35:05.000000 bu9-9.20/bu9.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-04-02 12:35:06.000000 bu9-9.20/bu9.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 12:35:05.000000 bu9-9.20/bu9.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-02 12:35:05.000000 bu9-9.20/bu9.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2024-04-02 12:35:05.000000 bu9-9.20/bu9.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 12:35:06.285143 bu9-9.20/setup.cfg
--rw-rw-rw-   0        0        0      220 2024-04-02 12:34:48.000000 bu9-9.20/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:37:19.464019 bu9-9.21/
+-rw-rw-rw-   0        0        0       49 2024-04-02 13:37:19.460021 bu9-9.21/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 13:37:19.458021 bu9-9.21/bu9.egg-info/
+-rw-rw-rw-   0        0        0       49 2024-04-02 13:37:19.000000 bu9-9.21/bu9.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2024-04-02 13:37:19.000000 bu9-9.21/bu9.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 13:37:19.000000 bu9-9.21/bu9.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-02 13:37:19.000000 bu9-9.21/bu9.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2024-04-02 13:37:19.000000 bu9-9.21/bu9.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 13:37:19.464019 bu9-9.21/setup.cfg
+-rw-rw-rw-   0        0        0      220 2024-04-02 13:37:04.000000 bu9-9.21/setup.py
```

