# Comparing `tmp/deepl_translator-0.1.2.tar.gz` & `tmp/deepl_translator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepl_translator-0.1.2.tar", last modified: Tue Apr  2 02:01:42 2024, max compression
+gzip compressed data, was "deepl_translator-0.1.3.tar", last modified: Tue Apr  2 02:05:27 2024, max compression
```

## Comparing `deepl_translator-0.1.2.tar` & `deepl_translator-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 yostos     (501) staff       (20)        0 2024-04-02 02:01:42.334489 deepl_translator-0.1.2/
--rw-r--r--   0 yostos     (501) staff       (20)     1064 2024-04-02 01:50:11.000000 deepl_translator-0.1.2/LICENSE
--rw-r--r--   0 yostos     (501) staff       (20)       34 2024-04-02 01:50:11.000000 deepl_translator-0.1.2/MANIFEST.in
--rw-r--r--   0 yostos     (501) staff       (20)      156 2024-04-02 02:01:42.334320 deepl_translator-0.1.2/PKG-INFO
--rw-r--r--   0 yostos     (501) staff       (20)     1829 2024-04-02 01:50:11.000000 deepl_translator-0.1.2/README.md
-drwxr-xr-x   0 yostos     (501) staff       (20)        0 2024-04-02 02:01:42.333174 deepl_translator-0.1.2/deepl_translator/
--rwxr-xr-x   0 yostos     (501) staff       (20)       54 2024-04-02 01:50:11.000000 deepl_translator-0.1.2/deepl_translator/__init__.py
--rw-r--r--   0 yostos     (501) staff       (20)      972 2024-04-02 01:50:11.000000 deepl_translator-0.1.2/deepl_translator/cli.py
--rw-r--r--   0 yostos     (501) staff       (20)      217 2024-04-02 01:50:11.000000 deepl_translator-0.1.2/deepl_translator/config.py
--rw-r--r--   0 yostos     (501) staff       (20)      531 2024-04-02 01:50:11.000000 deepl_translator-0.1.2/deepl_translator/translator.py
-drwxr-xr-x   0 yostos     (501) staff       (20)        0 2024-04-02 02:01:42.334150 deepl_translator-0.1.2/deepl_translator.egg-info/
--rw-r--r--   0 yostos     (501) staff       (20)      156 2024-04-02 02:01:42.000000 deepl_translator-0.1.2/deepl_translator.egg-info/PKG-INFO
--rw-r--r--   0 yostos     (501) staff       (20)      434 2024-04-02 02:01:42.000000 deepl_translator-0.1.2/deepl_translator.egg-info/SOURCES.txt
--rw-r--r--   0 yostos     (501) staff       (20)        1 2024-04-02 02:01:42.000000 deepl_translator-0.1.2/deepl_translator.egg-info/dependency_links.txt
--rw-r--r--   0 yostos     (501) staff       (20)       69 2024-04-02 02:01:42.000000 deepl_translator-0.1.2/deepl_translator.egg-info/entry_points.txt
--rw-r--r--   0 yostos     (501) staff       (20)       29 2024-04-02 02:01:42.000000 deepl_translator-0.1.2/deepl_translator.egg-info/requires.txt
--rw-r--r--   0 yostos     (501) staff       (20)       23 2024-04-02 02:01:42.000000 deepl_translator-0.1.2/deepl_translator.egg-info/top_level.txt
--rw-r--r--   0 yostos     (501) staff       (20)       38 2024-04-02 02:01:42.334532 deepl_translator-0.1.2/setup.cfg
--rw-r--r--   0 yostos     (501) staff       (20)      356 2024-04-02 02:00:44.000000 deepl_translator-0.1.2/setup.py
-drwxr-xr-x   0 yostos     (501) staff       (20)        0 2024-04-02 02:01:42.334007 deepl_translator-0.1.2/tests/
--rw-r--r--   0 yostos     (501) staff       (20)       41 2024-04-02 01:50:11.000000 deepl_translator-0.1.2/tests/__init__.py
--rw-r--r--   0 yostos     (501) staff       (20)      934 2024-04-02 01:50:11.000000 deepl_translator-0.1.2/tests/test_translator.py
+drwxr-xr-x   0 yostos     (501) staff       (20)        0 2024-04-02 02:05:27.523388 deepl_translator-0.1.3/
+-rw-r--r--   0 yostos     (501) staff       (20)     1064 2024-04-02 01:50:11.000000 deepl_translator-0.1.3/LICENSE
+-rw-r--r--   0 yostos     (501) staff       (20)       34 2024-04-02 01:50:11.000000 deepl_translator-0.1.3/MANIFEST.in
+-rw-r--r--   0 yostos     (501) staff       (20)      156 2024-04-02 02:05:27.523220 deepl_translator-0.1.3/PKG-INFO
+-rw-r--r--   0 yostos     (501) staff       (20)     1829 2024-04-02 01:50:11.000000 deepl_translator-0.1.3/README.md
+drwxr-xr-x   0 yostos     (501) staff       (20)        0 2024-04-02 02:05:27.522117 deepl_translator-0.1.3/deepl_translator/
+-rwxr-xr-x   0 yostos     (501) staff       (20)      106 2024-04-02 02:03:52.000000 deepl_translator-0.1.3/deepl_translator/__init__.py
+-rw-r--r--   0 yostos     (501) staff       (20)      972 2024-04-02 01:50:11.000000 deepl_translator-0.1.3/deepl_translator/cli.py
+-rw-r--r--   0 yostos     (501) staff       (20)      217 2024-04-02 01:50:11.000000 deepl_translator-0.1.3/deepl_translator/config.py
+-rw-r--r--   0 yostos     (501) staff       (20)      531 2024-04-02 01:50:11.000000 deepl_translator-0.1.3/deepl_translator/translator.py
+drwxr-xr-x   0 yostos     (501) staff       (20)        0 2024-04-02 02:05:27.523057 deepl_translator-0.1.3/deepl_translator.egg-info/
+-rw-r--r--   0 yostos     (501) staff       (20)      156 2024-04-02 02:05:27.000000 deepl_translator-0.1.3/deepl_translator.egg-info/PKG-INFO
+-rw-r--r--   0 yostos     (501) staff       (20)      434 2024-04-02 02:05:27.000000 deepl_translator-0.1.3/deepl_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 yostos     (501) staff       (20)        1 2024-04-02 02:05:27.000000 deepl_translator-0.1.3/deepl_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 yostos     (501) staff       (20)       53 2024-04-02 02:05:27.000000 deepl_translator-0.1.3/deepl_translator.egg-info/entry_points.txt
+-rw-r--r--   0 yostos     (501) staff       (20)       29 2024-04-02 02:05:27.000000 deepl_translator-0.1.3/deepl_translator.egg-info/requires.txt
+-rw-r--r--   0 yostos     (501) staff       (20)       23 2024-04-02 02:05:27.000000 deepl_translator-0.1.3/deepl_translator.egg-info/top_level.txt
+-rw-r--r--   0 yostos     (501) staff       (20)       38 2024-04-02 02:05:27.523423 deepl_translator-0.1.3/setup.cfg
+-rw-r--r--   0 yostos     (501) staff       (20)      340 2024-04-02 02:05:14.000000 deepl_translator-0.1.3/setup.py
+drwxr-xr-x   0 yostos     (501) staff       (20)        0 2024-04-02 02:05:27.522919 deepl_translator-0.1.3/tests/
+-rw-r--r--   0 yostos     (501) staff       (20)       41 2024-04-02 01:50:11.000000 deepl_translator-0.1.3/tests/__init__.py
+-rw-r--r--   0 yostos     (501) staff       (20)      934 2024-04-02 01:50:11.000000 deepl_translator-0.1.3/tests/test_translator.py
```

### Comparing `deepl_translator-0.1.2/LICENSE` & `deepl_translator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepl_translator-0.1.2/README.md` & `deepl_translator-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `deepl_translator-0.1.2/deepl_translator/cli.py` & `deepl_translator-0.1.3/deepl_translator/cli.py`

 * *Files identical despite different names*

### Comparing `deepl_translator-0.1.2/deepl_translator/translator.py` & `deepl_translator-0.1.3/deepl_translator/translator.py`

 * *Files identical despite different names*

### Comparing `deepl_translator-0.1.2/tests/test_translator.py` & `deepl_translator-0.1.3/tests/test_translator.py`

 * *Files identical despite different names*

