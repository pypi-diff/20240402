# Comparing `tmp/alohapy-0.1.tar.gz` & `tmp/alohapy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alohapy-0.1.tar", last modified: Tue Apr  2 08:48:02 2024, max compression
+gzip compressed data, was "alohapy-0.2.1.tar", last modified: Tue Apr  2 08:59:35 2024, max compression
```

## Comparing `alohapy-0.1.tar` & `alohapy-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 damonwu    (501) staff       (20)        0 2024-04-02 08:48:02.641220 alohapy-0.1/
--rw-r--r--   0 damonwu    (501) staff       (20)       49 2024-04-02 08:48:02.641096 alohapy-0.1/PKG-INFO
--rw-r--r--   0 damonwu    (501) staff       (20)        0 2024-04-02 08:36:32.000000 alohapy-0.1/README.md
-drwxr-xr-x   0 damonwu    (501) staff       (20)        0 2024-04-02 08:48:02.640280 alohapy-0.1/alohapy/
--rw-r--r--   0 damonwu    (501) staff       (20)      304 2024-04-02 08:41:17.000000 alohapy-0.1/alohapy/__init__.py
--rw-r--r--   0 damonwu    (501) staff       (20)       42 2024-04-02 08:38:06.000000 alohapy-0.1/alohapy/main.py
-drwxr-xr-x   0 damonwu    (501) staff       (20)        0 2024-04-02 08:48:02.640900 alohapy-0.1/alohapy.egg-info/
--rw-r--r--   0 damonwu    (501) staff       (20)       49 2024-04-02 08:48:02.000000 alohapy-0.1/alohapy.egg-info/PKG-INFO
--rw-r--r--   0 damonwu    (501) staff       (20)      178 2024-04-02 08:48:02.000000 alohapy-0.1/alohapy.egg-info/SOURCES.txt
--rw-r--r--   0 damonwu    (501) staff       (20)        1 2024-04-02 08:48:02.000000 alohapy-0.1/alohapy.egg-info/dependency_links.txt
--rw-r--r--   0 damonwu    (501) staff       (20)        8 2024-04-02 08:48:02.000000 alohapy-0.1/alohapy.egg-info/top_level.txt
--rw-r--r--   0 damonwu    (501) staff       (20)       38 2024-04-02 08:48:02.641270 alohapy-0.1/setup.cfg
--rw-r--r--   0 damonwu    (501) staff       (20)      208 2024-04-02 08:43:49.000000 alohapy-0.1/setup.py
+drwxr-xr-x   0 damonwu    (501) staff       (20)        0 2024-04-02 08:59:35.976019 alohapy-0.2.1/
+-rw-r--r--   0 damonwu    (501) staff       (20)       51 2024-04-02 08:59:35.975899 alohapy-0.2.1/PKG-INFO
+-rw-r--r--   0 damonwu    (501) staff       (20)      335 2024-04-02 08:59:32.000000 alohapy-0.2.1/README.md
+drwxr-xr-x   0 damonwu    (501) staff       (20)        0 2024-04-02 08:59:35.975076 alohapy-0.2.1/alohapy/
+-rw-r--r--   0 damonwu    (501) staff       (20)      304 2024-04-02 08:41:17.000000 alohapy-0.2.1/alohapy/__init__.py
+-rw-r--r--   0 damonwu    (501) staff       (20)       42 2024-04-02 08:38:06.000000 alohapy-0.2.1/alohapy/main.py
+drwxr-xr-x   0 damonwu    (501) staff       (20)        0 2024-04-02 08:59:35.975729 alohapy-0.2.1/alohapy.egg-info/
+-rw-r--r--   0 damonwu    (501) staff       (20)       51 2024-04-02 08:59:35.000000 alohapy-0.2.1/alohapy.egg-info/PKG-INFO
+-rw-r--r--   0 damonwu    (501) staff       (20)      212 2024-04-02 08:59:35.000000 alohapy-0.2.1/alohapy.egg-info/SOURCES.txt
+-rw-r--r--   0 damonwu    (501) staff       (20)        1 2024-04-02 08:59:35.000000 alohapy-0.2.1/alohapy.egg-info/dependency_links.txt
+-rw-r--r--   0 damonwu    (501) staff       (20)       44 2024-04-02 08:59:35.000000 alohapy-0.2.1/alohapy.egg-info/entry_points.txt
+-rw-r--r--   0 damonwu    (501) staff       (20)        8 2024-04-02 08:59:35.000000 alohapy-0.2.1/alohapy.egg-info/top_level.txt
+-rw-r--r--   0 damonwu    (501) staff       (20)       38 2024-04-02 08:59:35.976080 alohapy-0.2.1/setup.cfg
+-rw-r--r--   0 damonwu    (501) staff       (20)      387 2024-04-02 08:58:31.000000 alohapy-0.2.1/setup.py
```

