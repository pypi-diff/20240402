# Comparing `tmp/mojadateconverter70-0.0.3.tar.gz` & `tmp/mojadateconverter70-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojadateconverter70-0.0.3.tar", last modified: Fri Mar 29 04:56:52 2024, max compression
+gzip compressed data, was "mojadateconverter70-0.0.4.tar", last modified: Tue Apr  2 08:36:18 2024, max compression
```

## Comparing `mojadateconverter70-0.0.3.tar` & `mojadateconverter70-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 04:56:52.280411 mojadateconverter70-0.0.3/
--rw-rw-rw-   0        0        0      159 2024-03-29 04:56:52.280411 mojadateconverter70-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-29 04:56:52.280411 mojadateconverter70-0.0.3/mojadateconverter70.egg-info/
--rw-rw-rw-   0        0        0      159 2024-03-29 04:56:52.000000 mojadateconverter70-0.0.3/mojadateconverter70.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-03-29 04:56:52.000000 mojadateconverter70-0.0.3/mojadateconverter70.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 04:56:52.000000 mojadateconverter70-0.0.3/mojadateconverter70.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 04:56:52.000000 mojadateconverter70-0.0.3/mojadateconverter70.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 04:56:52.280411 mojadateconverter70-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      265 2024-03-29 04:56:39.000000 mojadateconverter70-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:36:18.985089 mojadateconverter70-0.0.4/
+-rw-rw-rw-   0        0        0      159 2024-04-02 08:36:18.981081 mojadateconverter70-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 08:36:18.970234 mojadateconverter70-0.0.4/mojadateconverter70/
+-rw-rw-rw-   0        0        0       57 2024-04-02 08:13:28.000000 mojadateconverter70-0.0.4/mojadateconverter70/__init__.py
+-rw-rw-rw-   0        0        0    13851 2024-03-26 08:04:44.000000 mojadateconverter70-0.0.4/mojadateconverter70/mojadateconverter70.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:36:18.981081 mojadateconverter70-0.0.4/mojadateconverter70.egg-info/
+-rw-rw-rw-   0        0        0      159 2024-04-02 08:36:18.000000 mojadateconverter70-0.0.4/mojadateconverter70.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-02 08:36:18.000000 mojadateconverter70-0.0.4/mojadateconverter70.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 08:36:18.000000 mojadateconverter70-0.0.4/mojadateconverter70.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-02 08:36:18.000000 mojadateconverter70-0.0.4/mojadateconverter70.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 08:36:18.985604 mojadateconverter70-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      292 2024-04-02 08:21:42.000000 mojadateconverter70-0.0.4/setup.py
```

