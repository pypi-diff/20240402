# Comparing `tmp/excell_functions-0.4.tar.gz` & `tmp/excell_functions-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excell_functions-0.4.tar", last modified: Sun Mar  3 06:53:59 2024, max compression
+gzip compressed data, was "excell_functions-0.5.tar", last modified: Tue Apr  2 09:14:43 2024, max compression
```

## Comparing `excell_functions-0.4.tar` & `excell_functions-0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.036000 excell_functions-0.4/
--rw-r--r--   0 root         (0) root         (0)     1494 2024-03-03 06:42:28.000000 excell_functions-0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      181 2024-03-03 06:53:59.036000 excell_functions-0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16076 2024-03-03 06:42:28.000000 excell_functions-0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.032000 excell_functions-0.4/excell_functions/
--rw-r--r--   0 root         (0) root         (0)      369 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.032000 excell_functions-0.4/excell_functions/compatibility/
--rw-r--r--   0 root         (0) root         (0)     4871 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/compatibility/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.032000 excell_functions-0.4/excell_functions/cube/
--rw-r--r--   0 root         (0) root         (0)     1449 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/cube/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.032000 excell_functions-0.4/excell_functions/database/
--rw-r--r--   0 root         (0) root         (0)     1600 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/database/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.032000 excell_functions-0.4/excell_functions/datetime/
--rw-r--r--   0 root         (0) root         (0)     3372 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/datetime/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.032000 excell_functions-0.4/excell_functions/engineering/
--rw-r--r--   0 root         (0) root         (0)     5935 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/engineering/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.032000 excell_functions-0.4/excell_functions/example/
--rw-r--r--   0 root         (0) root         (0)     1252 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/example/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.032000 excell_functions-0.4/excell_functions/financial/
--rw-r--r--   0 root         (0) root         (0)     7556 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/financial/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.032000 excell_functions-0.4/excell_functions/information/
--rw-r--r--   0 root         (0) root         (0)     2350 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/information/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.032000 excell_functions-0.4/excell_functions/logical/
--rw-r--r--   0 root         (0) root         (0)     9715 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/logical/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.036000 excell_functions-0.4/excell_functions/lookup/
--rw-r--r--   0 root         (0) root         (0)     4658 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/lookup/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.036000 excell_functions-0.4/excell_functions/math/
--rw-r--r--   0 root         (0) root         (0)     9489 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/math/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.036000 excell_functions-0.4/excell_functions/statistical/
--rw-r--r--   0 root         (0) root         (0)    14531 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/statistical/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.036000 excell_functions-0.4/excell_functions/text/
--rw-r--r--   0 root         (0) root         (0)    18359 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/text/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.036000 excell_functions-0.4/excell_functions/users/
--rw-r--r--   0 root         (0) root         (0)      597 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/users/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.036000 excell_functions-0.4/excell_functions/web/
--rw-r--r--   0 root         (0) root         (0)      351 2024-03-03 06:42:28.000000 excell_functions-0.4/excell_functions/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 06:53:59.032000 excell_functions-0.4/excell_functions.egg-info/
--rw-r--r--   0 root         (0) root         (0)      181 2024-03-03 06:53:59.000000 excell_functions-0.4/excell_functions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      786 2024-03-03 06:53:59.000000 excell_functions-0.4/excell_functions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-03 06:53:59.000000 excell_functions-0.4/excell_functions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-03 06:53:59.000000 excell_functions-0.4/excell_functions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-03 06:53:59.036000 excell_functions-0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      246 2024-03-03 06:51:59.000000 excell_functions-0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.936000 excell_functions-0.5/
+-rw-r--r--   0 root         (0) root         (0)     1494 2024-03-03 06:42:28.000000 excell_functions-0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      181 2024-04-02 09:14:43.936000 excell_functions-0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16076 2024-03-03 06:42:28.000000 excell_functions-0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.928000 excell_functions-0.5/excell_functions/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-04-02 08:40:20.000000 excell_functions-0.5/excell_functions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.932000 excell_functions-0.5/excell_functions/compatibility/
+-rw-r--r--   0 root         (0) root         (0)     4871 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/compatibility/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.932000 excell_functions-0.5/excell_functions/cube/
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/cube/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.932000 excell_functions-0.5/excell_functions/database/
+-rw-r--r--   0 root         (0) root         (0)     1600 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/database/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.932000 excell_functions-0.5/excell_functions/datetime/
+-rw-r--r--   0 root         (0) root         (0)     3372 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/datetime/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.932000 excell_functions-0.5/excell_functions/engineering/
+-rw-r--r--   0 root         (0) root         (0)     5935 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/engineering/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.932000 excell_functions-0.5/excell_functions/example/
+-rw-r--r--   0 root         (0) root         (0)     1252 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/example/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.936000 excell_functions-0.5/excell_functions/financial/
+-rw-r--r--   0 root         (0) root         (0)     7556 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/financial/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.936000 excell_functions-0.5/excell_functions/information/
+-rw-r--r--   0 root         (0) root         (0)     2350 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/information/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.936000 excell_functions-0.5/excell_functions/logical/
+-rw-r--r--   0 root         (0) root         (0)     9715 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/logical/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.936000 excell_functions-0.5/excell_functions/lookup/
+-rw-r--r--   0 root         (0) root         (0)     4658 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/lookup/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.936000 excell_functions-0.5/excell_functions/math/
+-rw-r--r--   0 root         (0) root         (0)     9489 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/math/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.936000 excell_functions-0.5/excell_functions/statistical/
+-rw-r--r--   0 root         (0) root         (0)    14531 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/statistical/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.936000 excell_functions-0.5/excell_functions/text/
+-rw-r--r--   0 root         (0) root         (0)    18359 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.936000 excell_functions-0.5/excell_functions/users/
+-rw-r--r--   0 root         (0) root         (0)      597 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/users/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.936000 excell_functions-0.5/excell_functions/web/
+-rw-r--r--   0 root         (0) root         (0)      351 2024-03-03 06:42:28.000000 excell_functions-0.5/excell_functions/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:14:43.932000 excell_functions-0.5/excell_functions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      181 2024-04-02 09:14:43.000000 excell_functions-0.5/excell_functions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      786 2024-04-02 09:14:43.000000 excell_functions-0.5/excell_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 09:14:43.000000 excell_functions-0.5/excell_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-02 09:14:43.000000 excell_functions-0.5/excell_functions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 09:14:43.940000 excell_functions-0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      246 2024-04-02 09:14:12.000000 excell_functions-0.5/setup.py
```

### Comparing `excell_functions-0.4/LICENSE` & `excell_functions-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/README.md` & `excell_functions-0.5/README.md`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/compatibility/__init__.py` & `excell_functions-0.5/excell_functions/compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/cube/__init__.py` & `excell_functions-0.5/excell_functions/cube/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/database/__init__.py` & `excell_functions-0.5/excell_functions/database/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/datetime/__init__.py` & `excell_functions-0.5/excell_functions/datetime/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/engineering/__init__.py` & `excell_functions-0.5/excell_functions/engineering/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/example/__init__.py` & `excell_functions-0.5/excell_functions/example/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/financial/__init__.py` & `excell_functions-0.5/excell_functions/financial/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/information/__init__.py` & `excell_functions-0.5/excell_functions/information/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/logical/__init__.py` & `excell_functions-0.5/excell_functions/logical/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/lookup/__init__.py` & `excell_functions-0.5/excell_functions/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/math/__init__.py` & `excell_functions-0.5/excell_functions/math/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/statistical/__init__.py` & `excell_functions-0.5/excell_functions/statistical/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/text/__init__.py` & `excell_functions-0.5/excell_functions/text/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions/users/__init__.py` & `excell_functions-0.5/excell_functions/users/__init__.py`

 * *Files identical despite different names*

### Comparing `excell_functions-0.4/excell_functions.egg-info/SOURCES.txt` & `excell_functions-0.5/excell_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

