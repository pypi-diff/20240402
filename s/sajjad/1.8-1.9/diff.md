# Comparing `tmp/sajjad-1.8.tar.gz` & `tmp/sajjad-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sajjad-1.8.tar", last modified: Mon Apr  1 23:16:34 2024, max compression
+gzip compressed data, was "sajjad-1.9.tar", last modified: Tue Apr  2 14:16:08 2024, max compression
```

## Comparing `sajjad-1.8.tar` & `sajjad-1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 23:16:34.362785 sajjad-1.8/
--rw-rw-rw-   0        0        0      473 2024-04-01 23:16:34.361812 sajjad-1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-01 23:16:34.345214 sajjad-1.8/sajjad/
--rw-rw-rw-   0        0        0       21 2024-04-01 20:31:53.000000 sajjad-1.8/sajjad/__init__.py
--rw-rw-rw-   0        0        0      248 2024-04-01 23:15:53.000000 sajjad-1.8/sajjad/sajjad.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:16:34.360804 sajjad-1.8/sajjad.egg-info/
--rw-rw-rw-   0        0        0      473 2024-04-01 23:16:34.000000 sajjad-1.8/sajjad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2024-04-01 23:16:34.000000 sajjad-1.8/sajjad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 23:16:34.000000 sajjad-1.8/sajjad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-01 23:16:34.000000 sajjad-1.8/sajjad.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 23:16:34.000000 sajjad-1.8/sajjad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 23:16:34.362785 sajjad-1.8/setup.cfg
--rw-rw-rw-   0        0        0      622 2024-04-01 23:15:42.000000 sajjad-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:16:08.698794 sajjad-1.9/
+-rw-rw-rw-   0        0        0      490 2024-04-02 14:16:08.697795 sajjad-1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 14:16:08.684175 sajjad-1.9/sajjad/
+-rw-rw-rw-   0        0        0       21 2024-04-01 20:31:53.000000 sajjad-1.9/sajjad/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-04-01 23:15:53.000000 sajjad-1.9/sajjad/sajjad.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:16:08.696795 sajjad-1.9/sajjad.egg-info/
+-rw-rw-rw-   0        0        0      490 2024-04-02 14:16:08.000000 sajjad-1.9/sajjad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2024-04-02 14:16:08.000000 sajjad-1.9/sajjad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 14:16:08.000000 sajjad-1.9/sajjad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-02 14:16:08.000000 sajjad-1.9/sajjad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 14:16:08.000000 sajjad-1.9/sajjad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 14:16:08.698794 sajjad-1.9/setup.cfg
+-rw-rw-rw-   0        0        0      639 2024-04-02 14:15:56.000000 sajjad-1.9/setup.py
```

