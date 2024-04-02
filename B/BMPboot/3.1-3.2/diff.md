# Comparing `tmp/BMPboot-3.1.tar.gz` & `tmp/BMPboot-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BMPboot-3.1.tar", last modified: Tue Apr  2 06:57:03 2024, max compression
+gzip compressed data, was "BMPboot-3.2.tar", last modified: Tue Apr  2 07:54:03 2024, max compression
```

## Comparing `BMPboot-3.1.tar` & `BMPboot-3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 06:57:03.845999 BMPboot-3.1/
-drwxrwxrwx   0        0        0        0 2024-04-02 06:57:03.829000 BMPboot-3.1/BMPboot/
--rw-rw-rw-   0        0        0       96 2024-04-02 06:52:40.000000 BMPboot-3.1/BMPboot/__init__.py
--rw-rw-rw-   0        0        0     2184 2024-04-01 14:02:43.000000 BMPboot-3.1/BMPboot/address_book.py
--rw-rw-rw-   0        0        0    18251 2024-04-02 06:48:20.000000 BMPboot-3.1/BMPboot/main.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:57:03.841999 BMPboot-3.1/BMPboot.egg-info/
--rw-rw-rw-   0        0        0      174 2024-04-02 06:57:03.000000 BMPboot-3.1/BMPboot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-04-02 06:57:03.000000 BMPboot-3.1/BMPboot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 06:57:03.000000 BMPboot-3.1/BMPboot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-02 06:57:03.000000 BMPboot-3.1/BMPboot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-04-02 06:57:03.000000 BMPboot-3.1/BMPboot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-02 06:57:03.000000 BMPboot-3.1/BMPboot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      174 2024-04-02 06:57:03.844000 BMPboot-3.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-02 06:57:03.845999 BMPboot-3.1/setup.cfg
--rw-rw-rw-   0        0        0      442 2024-04-02 06:57:01.000000 BMPboot-3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:57:03.840999 BMPboot-3.1/test/
--rw-rw-rw-   0        0        0      201 2024-04-02 06:51:34.000000 BMPboot-3.1/test/testowanie.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:54:03.541118 BMPboot-3.2/
+drwxrwxrwx   0        0        0        0 2024-04-02 07:54:03.524120 BMPboot-3.2/BMPboot/
+-rw-rw-rw-   0        0        0       96 2024-04-02 06:52:40.000000 BMPboot-3.2/BMPboot/__init__.py
+-rw-rw-rw-   0        0        0     2184 2024-04-01 14:02:43.000000 BMPboot-3.2/BMPboot/address_book.py
+-rw-rw-rw-   0        0        0    18251 2024-04-02 06:48:20.000000 BMPboot-3.2/BMPboot/main.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:54:03.538118 BMPboot-3.2/BMPboot.egg-info/
+-rw-rw-rw-   0        0        0     2299 2024-04-02 07:54:02.000000 BMPboot-3.2/BMPboot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-04-02 07:54:02.000000 BMPboot-3.2/BMPboot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 07:54:02.000000 BMPboot-3.2/BMPboot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-02 07:54:02.000000 BMPboot-3.2/BMPboot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-04-02 07:54:02.000000 BMPboot-3.2/BMPboot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-02 07:54:02.000000 BMPboot-3.2/BMPboot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2299 2024-04-02 07:54:03.539118 BMPboot-3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-02 07:54:03.541118 BMPboot-3.2/setup.cfg
+-rw-rw-rw-   0        0        0      674 2024-04-02 07:53:14.000000 BMPboot-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:54:03.536119 BMPboot-3.2/test/
+-rw-rw-rw-   0        0        0      201 2024-04-02 06:51:34.000000 BMPboot-3.2/test/testowanie.py
```

### Comparing `BMPboot-3.1/BMPboot/address_book.py` & `BMPboot-3.2/BMPboot/address_book.py`

 * *Files identical despite different names*

### Comparing `BMPboot-3.1/BMPboot/main.py` & `BMPboot-3.2/BMPboot/main.py`

 * *Files identical despite different names*

