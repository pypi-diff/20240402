# Comparing `tmp/genice2_extra-2.1.tar.gz` & `tmp/genice2_extra-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genice2_extra-2.1.tar", last modified: Tue Mar 23 13:10:06 2021, max compression
+gzip compressed data, was "genice2_extra-2.2.tar", max compression
```

## Comparing `genice2_extra-2.1.tar` & `genice2_extra-2.2.tar`

### file list

```diff
@@ -1,11 +1,4 @@
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-03-23 13:10:06.275173 genice2_extra-2.1/
--rw-r--r--   0 matto      (505) staff       (20)      940 2021-03-23 13:10:06.275242 genice2_extra-2.1/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)      308 2021-01-26 08:20:32.000000 genice2_extra-2.1/README.md
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-03-23 13:10:06.275093 genice2_extra-2.1/genice2_extra.egg-info/
--rw-r--r--   0 matto      (505) staff       (20)      940 2021-03-23 13:10:06.000000 genice2_extra-2.1/genice2_extra.egg-info/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)      212 2021-03-23 13:10:06.000000 genice2_extra-2.1/genice2_extra.egg-info/SOURCES.txt
--rw-r--r--   0 matto      (505) staff       (20)        1 2021-03-23 13:10:06.000000 genice2_extra-2.1/genice2_extra.egg-info/dependency_links.txt
--rw-r--r--   0 matto      (505) staff       (20)       56 2021-03-23 13:10:06.000000 genice2_extra-2.1/genice2_extra.egg-info/requires.txt
--rw-r--r--   0 matto      (505) staff       (20)        1 2021-03-23 13:10:06.000000 genice2_extra-2.1/genice2_extra.egg-info/top_level.txt
--rw-r--r--   0 matto      (505) staff       (20)      108 2021-03-23 13:10:06.275444 genice2_extra-2.1/setup.cfg
--rw-r--r--   0 matto      (505) staff       (20)     1198 2021-03-23 13:03:17.000000 genice2_extra-2.1/setup.py
+-rw-r--r--   0        0        0      402 2024-04-02 04:15:49.644495 genice2_extra-2.2/README.md
+-rw-r--r--   0        0        0       20 2024-04-02 03:54:16.766285 genice2_extra-2.2/genice2_extra/__init__.py
+-rw-r--r--   0        0        0      960 2024-04-02 03:59:10.748209 genice2_extra-2.2/pyproject.toml
+-rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 genice2_extra-2.2/PKG-INFO
```

