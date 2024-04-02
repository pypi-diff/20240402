# Comparing `tmp/icoder_math-0.0.1.tar.gz` & `tmp/icoder_math-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icoder_math-0.0.1.tar", last modified: Tue Apr  2 18:27:05 2024, max compression
+gzip compressed data, was "icoder_math-0.0.2.tar", last modified: Tue Apr  2 18:55:31 2024, max compression
```

## Comparing `icoder_math-0.0.1.tar` & `icoder_math-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 18:27:05.320229 icoder_math-0.0.1/
--rw-rw-rw-   0        0        0      279 2024-04-02 18:27:05.313226 icoder_math-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      683 2024-04-02 17:58:23.000000 icoder_math-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 18:27:05.159226 icoder_math-0.0.1/icoder_math/
--rw-rw-rw-   0        0        0        0 2024-04-02 16:28:12.000000 icoder_math-0.0.1/icoder_math/__init__.py
--rw-rw-rw-   0        0        0      517 2024-04-02 16:29:12.000000 icoder_math-0.0.1/icoder_math/calculate.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:27:05.310224 icoder_math-0.0.1/icoder_math.egg-info/
--rw-rw-rw-   0        0        0      279 2024-04-02 18:27:04.000000 icoder_math-0.0.1/icoder_math.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-04-02 18:27:04.000000 icoder_math-0.0.1/icoder_math.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 18:27:04.000000 icoder_math-0.0.1/icoder_math.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-02 18:27:04.000000 icoder_math-0.0.1/icoder_math.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 18:27:05.321246 icoder_math-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      405 2024-04-02 18:26:05.000000 icoder_math-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:55:31.458989 icoder_math-0.0.2/
+-rw-rw-rw-   0        0        0      279 2024-04-02 18:55:31.455989 icoder_math-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2024-04-02 17:58:23.000000 icoder_math-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 18:55:31.363987 icoder_math-0.0.2/icoder_math/
+-rw-rw-rw-   0        0        0       18 2024-04-02 18:54:49.000000 icoder_math-0.0.2/icoder_math/__init__.py
+-rw-rw-rw-   0        0        0      517 2024-04-02 16:29:12.000000 icoder_math-0.0.2/icoder_math/calculate.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:55:31.451991 icoder_math-0.0.2/icoder_math.egg-info/
+-rw-rw-rw-   0        0        0      279 2024-04-02 18:55:31.000000 icoder_math-0.0.2/icoder_math.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-04-02 18:55:31.000000 icoder_math-0.0.2/icoder_math.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 18:55:31.000000 icoder_math-0.0.2/icoder_math.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-02 18:55:31.000000 icoder_math-0.0.2/icoder_math.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 18:55:31.458989 icoder_math-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      405 2024-04-02 18:55:26.000000 icoder_math-0.0.2/setup.py
```

### Comparing `icoder_math-0.0.1/README.md` & `icoder_math-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `icoder_math-0.0.1/icoder_math/calculate.py` & `icoder_math-0.0.2/icoder_math/calculate.py`

 * *Files identical despite different names*

