# Comparing `tmp/illumind-0.0.0.tar.gz` & `tmp/illumind-0.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "illumind-0.0.0.tar", last modified: Tue Apr  2 14:49:08 2024, max compression
+gzip compressed data, was "illumind-0.0.0.post1.tar", last modified: Tue Apr  2 16:48:16 2024, max compression
```

## Comparing `illumind-0.0.0.tar` & `illumind-0.0.0.post1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 14:49:08.975917 illumind-0.0.0/
--rw-rw-rw-   0        0        0       76 2024-04-02 14:42:51.000000 illumind-0.0.0/LICENSE
--rw-rw-rw-   0        0        0       78 2024-04-02 14:49:08.975917 illumind-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      120 2024-04-02 14:42:21.000000 illumind-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 14:49:08.948704 illumind-0.0.0/illumind/
--rw-rw-rw-   0        0        0        0 2024-04-02 14:40:21.000000 illumind-0.0.0/illumind/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:49:08.975917 illumind-0.0.0/illumind.egg-info/
--rw-rw-rw-   0        0        0       78 2024-04-02 14:49:08.000000 illumind-0.0.0/illumind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2024-04-02 14:49:08.000000 illumind-0.0.0/illumind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 14:49:08.000000 illumind-0.0.0/illumind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 14:49:08.000000 illumind-0.0.0/illumind.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      200 2024-04-02 14:41:45.000000 illumind-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 14:49:08.975917 illumind-0.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 16:48:16.534351 illumind-0.0.0.post1/
+-rw-rw-rw-   0        0        0       76 2024-04-02 14:42:51.000000 illumind-0.0.0.post1/LICENSE
+-rw-rw-rw-   0        0        0      319 2024-04-02 16:48:16.531767 illumind-0.0.0.post1/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2024-04-02 14:42:21.000000 illumind-0.0.0.post1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 16:48:16.501093 illumind-0.0.0.post1/illumind/
+-rw-rw-rw-   0        0        0        0 2024-04-02 14:40:21.000000 illumind-0.0.0.post1/illumind/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 16:48:16.531767 illumind-0.0.0.post1/illumind.egg-info/
+-rw-rw-rw-   0        0        0      319 2024-04-02 16:48:16.000000 illumind-0.0.0.post1/illumind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2024-04-02 16:48:16.000000 illumind-0.0.0.post1/illumind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 16:48:16.000000 illumind-0.0.0.post1/illumind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 16:48:16.000000 illumind-0.0.0.post1/illumind.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      333 2024-04-02 16:47:29.000000 illumind-0.0.0.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 16:48:16.534351 illumind-0.0.0.post1/setup.cfg
```

