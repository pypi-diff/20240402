# Comparing `tmp/WebServerStatusCheckerAJM-1.2.3.tar.gz` & `tmp/WebServerStatusCheckerAJM-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebServerStatusCheckerAJM-1.2.3.tar", last modified: Wed Mar 13 18:45:06 2024, max compression
+gzip compressed data, was "WebServerStatusCheckerAJM-1.3.tar", last modified: Tue Apr  2 13:17:59 2024, max compression
```

## Comparing `WebServerStatusCheckerAJM-1.2.3.tar` & `WebServerStatusCheckerAJM-1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 18:45:06.459613 WebServerStatusCheckerAJM-1.2.3/
--rw-rw-rw-   0        0        0     1084 2024-03-11 11:41:37.000000 WebServerStatusCheckerAJM-1.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0      587 2024-03-13 18:45:06.461617 WebServerStatusCheckerAJM-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      336 2024-03-13 16:08:16.000000 WebServerStatusCheckerAJM-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-13 18:45:06.429693 WebServerStatusCheckerAJM-1.2.3/WebServerStatusCheckerAJM/
--rw-rw-rw-   0        0        0    15607 2024-03-13 18:32:35.000000 WebServerStatusCheckerAJM-1.2.3/WebServerStatusCheckerAJM/WebServerStatusCheckerAJM.py
--rw-rw-rw-   0        0        0      136 2024-03-13 18:32:05.000000 WebServerStatusCheckerAJM-1.2.3/WebServerStatusCheckerAJM/__init__.py
--rw-rw-rw-   0        0        0       23 2024-03-13 18:33:16.000000 WebServerStatusCheckerAJM-1.2.3/WebServerStatusCheckerAJM/_version.py
-drwxrwxrwx   0        0        0        0 2024-03-13 18:45:06.455623 WebServerStatusCheckerAJM-1.2.3/WebServerStatusCheckerAJM.egg-info/
--rw-rw-rw-   0        0        0      587 2024-03-13 18:45:06.000000 WebServerStatusCheckerAJM-1.2.3/WebServerStatusCheckerAJM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2024-03-13 18:45:06.000000 WebServerStatusCheckerAJM-1.2.3/WebServerStatusCheckerAJM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 18:45:06.000000 WebServerStatusCheckerAJM-1.2.3/WebServerStatusCheckerAJM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-03-13 18:45:06.000000 WebServerStatusCheckerAJM-1.2.3/WebServerStatusCheckerAJM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-03-13 18:45:06.000000 WebServerStatusCheckerAJM-1.2.3/WebServerStatusCheckerAJM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-13 18:45:06.468588 WebServerStatusCheckerAJM-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1050 2024-03-13 15:42:59.000000 WebServerStatusCheckerAJM-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:17:59.207353 WebServerStatusCheckerAJM-1.3/
+-rw-rw-rw-   0        0        0     1084 2024-03-11 11:41:37.000000 WebServerStatusCheckerAJM-1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      638 2024-04-02 13:17:59.199395 WebServerStatusCheckerAJM-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2024-03-13 16:08:16.000000 WebServerStatusCheckerAJM-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 13:17:59.160133 WebServerStatusCheckerAJM-1.3/WebServerStatusCheckerAJM/
+-rw-rw-rw-   0        0        0    18976 2024-04-02 13:13:27.000000 WebServerStatusCheckerAJM-1.3/WebServerStatusCheckerAJM/WebServerStatusCheckerAJM.py
+-rw-rw-rw-   0        0        0      136 2024-03-13 18:32:05.000000 WebServerStatusCheckerAJM-1.3/WebServerStatusCheckerAJM/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-02 13:14:13.000000 WebServerStatusCheckerAJM-1.3/WebServerStatusCheckerAJM/_version.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:17:59.195002 WebServerStatusCheckerAJM-1.3/WebServerStatusCheckerAJM.egg-info/
+-rw-rw-rw-   0        0        0      638 2024-04-02 13:17:59.000000 WebServerStatusCheckerAJM-1.3/WebServerStatusCheckerAJM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2024-04-02 13:17:59.000000 WebServerStatusCheckerAJM-1.3/WebServerStatusCheckerAJM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 13:17:59.000000 WebServerStatusCheckerAJM-1.3/WebServerStatusCheckerAJM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-02 13:17:59.000000 WebServerStatusCheckerAJM-1.3/WebServerStatusCheckerAJM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-02 13:17:59.000000 WebServerStatusCheckerAJM-1.3/WebServerStatusCheckerAJM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-02 13:17:59.210345 WebServerStatusCheckerAJM-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1050 2024-03-13 15:42:59.000000 WebServerStatusCheckerAJM-1.3/setup.py
```

### Comparing `WebServerStatusCheckerAJM-1.2.3/LICENSE.txt` & `WebServerStatusCheckerAJM-1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `WebServerStatusCheckerAJM-1.2.3/setup.py` & `WebServerStatusCheckerAJM-1.3/setup.py`

 * *Files identical despite different names*

