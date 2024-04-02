# Comparing `tmp/bu9-9.19.tar.gz` & `tmp/bu9-9.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bu9-9.19.tar", last modified: Tue Jan 23 16:20:36 2024, max compression
+gzip compressed data, was "bu9-9.20.tar", last modified: Tue Apr  2 12:35:06 2024, max compression
```

## Comparing `bu9-9.19.tar` & `bu9-9.20.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwx---   0 root         (0)     9997        0 2024-01-23 16:20:36.394162 bu9-9.19/
--rw-rw----   0 root         (0)     9997       46 2024-01-23 16:20:36.384162 bu9-9.19/PKG-INFO
-drwxrwx---   0 root         (0)     9997        0 2024-01-23 16:20:36.384162 bu9-9.19/bu9.egg-info/
--rw-rw----   0 root         (0)     9997       46 2024-01-23 16:20:35.000000 bu9-9.19/bu9.egg-info/PKG-INFO
--rw-rw----   0 root         (0)     9997      153 2024-01-23 16:20:35.000000 bu9-9.19/bu9.egg-info/SOURCES.txt
--rw-rw----   0 root         (0)     9997        1 2024-01-23 16:20:35.000000 bu9-9.19/bu9.egg-info/dependency_links.txt
--rw-rw----   0 root         (0)     9997       33 2024-01-23 16:20:35.000000 bu9-9.19/bu9.egg-info/entry_points.txt
--rw-rw----   0 root         (0)     9997        4 2024-01-23 16:20:35.000000 bu9-9.19/bu9.egg-info/top_level.txt
--rw-rw----   0 root         (0)     9997   273989 2024-01-23 16:16:16.000000 bu9-9.19/bu9.py
--rw-rw----   0 root         (0)     9997       38 2024-01-23 16:20:36.394162 bu9-9.19/setup.cfg
--rw-rw----   0 root         (0)     9997      263 2024-01-23 16:20:25.000000 bu9-9.19/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:35:06.285143 bu9-9.20/
+-rw-rw-rw-   0        0        0       49 2024-04-02 12:35:06.283143 bu9-9.20/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 12:35:06.281144 bu9-9.20/bu9.egg-info/
+-rw-rw-rw-   0        0        0       49 2024-04-02 12:35:05.000000 bu9-9.20/bu9.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2024-04-02 12:35:06.000000 bu9-9.20/bu9.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:35:05.000000 bu9-9.20/bu9.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-02 12:35:05.000000 bu9-9.20/bu9.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2024-04-02 12:35:05.000000 bu9-9.20/bu9.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 12:35:06.285143 bu9-9.20/setup.cfg
+-rw-rw-rw-   0        0        0      220 2024-04-02 12:34:48.000000 bu9-9.20/setup.py
```

