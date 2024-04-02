# Comparing `tmp/mediqbox-jobctxmgr-0.0.1.tar.gz` & `tmp/mediqbox-jobctxmgr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediqbox-jobctxmgr-0.0.1.tar", last modified: Mon Mar 18 13:31:17 2024, max compression
+gzip compressed data, was "mediqbox-jobctxmgr-0.0.2.tar", last modified: Tue Apr  2 00:50:00 2024, max compression
```

## Comparing `mediqbox-jobctxmgr-0.0.1.tar` & `mediqbox-jobctxmgr-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 zhaojiamin   (501) staff       (20)        0 2024-03-18 13:31:17.261561 mediqbox-jobctxmgr-0.0.1/
--rw-r--r--   0 zhaojiamin   (501) staff       (20)      231 2024-03-18 13:31:17.261046 mediqbox-jobctxmgr-0.0.1/PKG-INFO
--rw-r--r--   0 zhaojiamin   (501) staff       (20)       71 2024-03-18 13:18:53.000000 mediqbox-jobctxmgr-0.0.1/README.md
--rw-r--r--   0 zhaojiamin   (501) staff       (20)       38 2024-03-18 13:31:17.261674 mediqbox-jobctxmgr-0.0.1/setup.cfg
--rw-r--r--   0 zhaojiamin   (501) staff       (20)      462 2024-03-18 13:19:03.000000 mediqbox-jobctxmgr-0.0.1/setup.py
-drwxr-xr-x   0 zhaojiamin   (501) staff       (20)        0 2024-03-18 13:31:17.250682 mediqbox-jobctxmgr-0.0.1/src/
-drwxr-xr-x   0 zhaojiamin   (501) staff       (20)        0 2024-03-18 13:31:17.250487 mediqbox-jobctxmgr-0.0.1/src/mediqbox/
-drwxr-xr-x   0 zhaojiamin   (501) staff       (20)        0 2024-03-18 13:31:17.255860 mediqbox-jobctxmgr-0.0.1/src/mediqbox/jobctxmgr/
--rw-r--r--   0 zhaojiamin   (501) staff       (20)      698 2024-03-18 08:21:19.000000 mediqbox-jobctxmgr-0.0.1/src/mediqbox/jobctxmgr/__init__.py
--rw-r--r--   0 zhaojiamin   (501) staff       (20)     5369 2024-03-18 12:50:46.000000 mediqbox-jobctxmgr-0.0.1/src/mediqbox/jobctxmgr/context.py
--rw-r--r--   0 zhaojiamin   (501) staff       (20)      716 2024-03-18 08:49:59.000000 mediqbox-jobctxmgr-0.0.1/src/mediqbox/jobctxmgr/serialize.py
--rw-r--r--   0 zhaojiamin   (501) staff       (20)      275 2024-03-18 13:09:06.000000 mediqbox-jobctxmgr-0.0.1/src/mediqbox/jobctxmgr/settings.py
-drwxr-xr-x   0 zhaojiamin   (501) staff       (20)        0 2024-03-18 13:31:17.260465 mediqbox-jobctxmgr-0.0.1/src/mediqbox_jobctxmgr.egg-info/
--rw-r--r--   0 zhaojiamin   (501) staff       (20)      231 2024-03-18 13:31:17.000000 mediqbox-jobctxmgr-0.0.1/src/mediqbox_jobctxmgr.egg-info/PKG-INFO
--rw-r--r--   0 zhaojiamin   (501) staff       (20)      356 2024-03-18 13:31:17.000000 mediqbox-jobctxmgr-0.0.1/src/mediqbox_jobctxmgr.egg-info/SOURCES.txt
--rw-r--r--   0 zhaojiamin   (501) staff       (20)        1 2024-03-18 13:31:17.000000 mediqbox-jobctxmgr-0.0.1/src/mediqbox_jobctxmgr.egg-info/dependency_links.txt
--rw-r--r--   0 zhaojiamin   (501) staff       (20)        9 2024-03-18 13:31:17.000000 mediqbox-jobctxmgr-0.0.1/src/mediqbox_jobctxmgr.egg-info/top_level.txt
-drwxr-xr-x   0 zhaojiamin   (501) staff       (20)        0 2024-03-18 13:31:17.259348 mediqbox-jobctxmgr-0.0.1/tests/
--rw-r--r--   0 zhaojiamin   (501) staff       (20)      829 2024-03-18 13:09:44.000000 mediqbox-jobctxmgr-0.0.1/tests/test.py
+drwxr-xr-x   0 zhaojiamin   (501) staff       (20)        0 2024-04-02 00:50:00.098504 mediqbox-jobctxmgr-0.0.2/
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)      263 2024-04-02 00:50:00.096783 mediqbox-jobctxmgr-0.0.2/PKG-INFO
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)       71 2024-03-18 13:18:53.000000 mediqbox-jobctxmgr-0.0.2/README.md
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)       38 2024-04-02 00:50:00.098658 mediqbox-jobctxmgr-0.0.2/setup.cfg
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)      486 2024-04-02 00:47:03.000000 mediqbox-jobctxmgr-0.0.2/setup.py
+drwxr-xr-x   0 zhaojiamin   (501) staff       (20)        0 2024-04-02 00:50:00.087201 mediqbox-jobctxmgr-0.0.2/src/
+drwxr-xr-x   0 zhaojiamin   (501) staff       (20)        0 2024-04-02 00:50:00.087031 mediqbox-jobctxmgr-0.0.2/src/mediqbox/
+drwxr-xr-x   0 zhaojiamin   (501) staff       (20)        0 2024-04-02 00:50:00.091782 mediqbox-jobctxmgr-0.0.2/src/mediqbox/jobctxmgr/
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)      698 2024-03-18 08:21:19.000000 mediqbox-jobctxmgr-0.0.2/src/mediqbox/jobctxmgr/__init__.py
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)     5369 2024-03-18 12:50:46.000000 mediqbox-jobctxmgr-0.0.2/src/mediqbox/jobctxmgr/context.py
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)      716 2024-03-18 08:49:59.000000 mediqbox-jobctxmgr-0.0.2/src/mediqbox/jobctxmgr/serialize.py
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)      275 2024-03-18 13:09:06.000000 mediqbox-jobctxmgr-0.0.2/src/mediqbox/jobctxmgr/settings.py
+drwxr-xr-x   0 zhaojiamin   (501) staff       (20)        0 2024-04-02 00:50:00.096076 mediqbox-jobctxmgr-0.0.2/src/mediqbox_jobctxmgr.egg-info/
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)      263 2024-04-02 00:50:00.000000 mediqbox-jobctxmgr-0.0.2/src/mediqbox_jobctxmgr.egg-info/PKG-INFO
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)      401 2024-04-02 00:50:00.000000 mediqbox-jobctxmgr-0.0.2/src/mediqbox_jobctxmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)        1 2024-04-02 00:50:00.000000 mediqbox-jobctxmgr-0.0.2/src/mediqbox_jobctxmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)       17 2024-04-02 00:50:00.000000 mediqbox-jobctxmgr-0.0.2/src/mediqbox_jobctxmgr.egg-info/requires.txt
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)        9 2024-04-02 00:50:00.000000 mediqbox-jobctxmgr-0.0.2/src/mediqbox_jobctxmgr.egg-info/top_level.txt
+drwxr-xr-x   0 zhaojiamin   (501) staff       (20)        0 2024-04-02 00:50:00.094917 mediqbox-jobctxmgr-0.0.2/tests/
+-rw-r--r--   0 zhaojiamin   (501) staff       (20)      829 2024-03-18 13:09:44.000000 mediqbox-jobctxmgr-0.0.2/tests/test.py
```

### Comparing `mediqbox-jobctxmgr-0.0.1/src/mediqbox/jobctxmgr/__init__.py` & `mediqbox-jobctxmgr-0.0.2/src/mediqbox/jobctxmgr/__init__.py`

 * *Files identical despite different names*

### Comparing `mediqbox-jobctxmgr-0.0.1/src/mediqbox/jobctxmgr/context.py` & `mediqbox-jobctxmgr-0.0.2/src/mediqbox/jobctxmgr/context.py`

 * *Files identical despite different names*

### Comparing `mediqbox-jobctxmgr-0.0.1/src/mediqbox/jobctxmgr/serialize.py` & `mediqbox-jobctxmgr-0.0.2/src/mediqbox/jobctxmgr/serialize.py`

 * *Files identical despite different names*

### Comparing `mediqbox-jobctxmgr-0.0.1/tests/test.py` & `mediqbox-jobctxmgr-0.0.2/tests/test.py`

 * *Files identical despite different names*

