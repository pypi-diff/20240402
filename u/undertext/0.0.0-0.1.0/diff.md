# Comparing `tmp/undertext-0.0.0.tar.gz` & `tmp/undertext-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undertext-0.0.0.tar", last modified: Mon Apr  1 11:08:35 2024, max compression
+gzip compressed data, was "undertext-0.1.0.tar", last modified: Tue Apr  2 13:45:02 2024, max compression
```

## Comparing `undertext-0.0.0.tar` & `undertext-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,33 @@
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-01 11:08:35.957023 undertext-0.0.0/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1074 2024-04-01 10:58:40.000000 undertext-0.0.0/LICENSE
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     1500 2024-04-01 11:08:35.957023 undertext-0.0.0/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      152 2024-04-01 11:06:10.000000 undertext-0.0.0/README.md
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-01 11:00:16.000000 undertext-0.0.0/pyproject.toml
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-01 11:08:35.957023 undertext-0.0.0/setup.cfg
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1802 2024-04-01 11:08:28.000000 undertext-0.0.0/setup.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-01 11:08:35.953023 undertext-0.0.0/src/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-01 11:08:35.953023 undertext-0.0.0/src/undertext/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1552 2024-04-01 11:03:31.000000 undertext-0.0.0/src/undertext/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       81 2024-04-01 11:02:54.000000 undertext-0.0.0/src/undertext/exceptions.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-01 11:08:35.957023 undertext-0.0.0/src/undertext.egg-info/
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     1500 2024-04-01 11:08:35.000000 undertext-0.0.0/src/undertext.egg-info/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      279 2024-04-01 11:08:35.000000 undertext-0.0.0/src/undertext.egg-info/SOURCES.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-01 11:08:35.000000 undertext-0.0.0/src/undertext.egg-info/dependency_links.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        7 2024-04-01 11:08:35.000000 undertext-0.0.0/src/undertext.egg-info/requires.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       10 2024-04-01 11:08:35.000000 undertext-0.0.0/src/undertext.egg-info/top_level.txt
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.865226 undertext-0.1.0/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1074 2024-04-01 10:58:40.000000 undertext-0.1.0/LICENSE
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3682 2024-04-02 13:45:02.865226 undertext-0.1.0/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2334 2024-04-02 12:06:09.000000 undertext-0.1.0/README.md
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-01 11:00:16.000000 undertext-0.1.0/pyproject.toml
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-02 13:45:02.865226 undertext-0.1.0/setup.cfg
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1917 2024-04-01 14:33:10.000000 undertext-0.1.0/setup.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.861226 undertext-0.1.0/src/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.861226 undertext-0.1.0/src/undertext/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1031 2024-04-02 13:05:36.000000 undertext-0.1.0/src/undertext/__cli__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1663 2024-04-02 13:32:00.000000 undertext-0.1.0/src/undertext/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2280 2024-04-02 11:53:18.000000 undertext-0.1.0/src/undertext/__main__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      189 2024-04-01 12:30:46.000000 undertext-0.1.0/src/undertext/exceptions.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.861226 undertext-0.1.0/src/undertext/readers/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      985 2024-04-02 13:20:03.000000 undertext-0.1.0/src/undertext/readers/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1262 2024-04-02 11:35:50.000000 undertext-0.1.0/src/undertext/readers/microdvd.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1699 2024-04-02 12:35:19.000000 undertext-0.1.0/src/undertext/readers/subrip.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     3073 2024-04-02 11:04:28.000000 undertext-0.1.0/src/undertext/readers/webvtt.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.861226 undertext-0.1.0/src/undertext/structures/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       86 2024-04-01 15:03:12.000000 undertext-0.1.0/src/undertext/structures/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2497 2024-04-02 12:35:19.000000 undertext-0.1.0/src/undertext/structures/caption.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.865226 undertext-0.1.0/src/undertext/writers/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1042 2024-04-02 13:20:10.000000 undertext-0.1.0/src/undertext/writers/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      942 2024-04-02 11:35:50.000000 undertext-0.1.0/src/undertext/writers/microdvd.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      926 2024-04-01 20:59:43.000000 undertext-0.1.0/src/undertext/writers/subrip.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1597 2024-04-02 11:01:15.000000 undertext-0.1.0/src/undertext/writers/webvtt.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.865226 undertext-0.1.0/src/undertext.egg-info/
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3682 2024-04-02 13:45:02.000000 undertext-0.1.0/src/undertext.egg-info/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      707 2024-04-02 13:45:02.000000 undertext-0.1.0/src/undertext.egg-info/SOURCES.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-02 13:45:02.000000 undertext-0.1.0/src/undertext.egg-info/dependency_links.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       54 2024-04-02 13:45:02.000000 undertext-0.1.0/src/undertext.egg-info/entry_points.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        7 2024-04-02 13:45:02.000000 undertext-0.1.0/src/undertext.egg-info/requires.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       10 2024-04-02 13:45:02.000000 undertext-0.1.0/src/undertext.egg-info/top_level.txt
```

### Comparing `undertext-0.0.0/LICENSE` & `undertext-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `undertext-0.0.0/setup.py` & `undertext-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,8 +48,13 @@
         "Programming Language :: Python :: 3.13",
         "Topic :: Utilities",
     ],
     python_requires=">=3.6",
     install_requires=install_requires,
     extras_require=extras_require,
     test_suite="tests",
+    entry_points={
+        "console_scripts": [
+            "undertext = undertext.__main__:main"
+        ]
+    },
 )
```

### Comparing `undertext-0.0.0/src/undertext/__init__.py` & `undertext-0.1.0/src/undertext/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,11 +28,15 @@
 __copyright__ = "Copyright 2024, utility-libraries"
 __credits__ = ["PlayerG9"]
 __license__ = "MIT"
 __maintainer__ = "PlayerG9"
 __email__ = None
 __status__ = "Prototype"  # Prototype, Development, Production
 __description__ = "library to load, edit and save different formats of subtitles"
-__version_info__ = (0, 0, 0)
+__version_info__ = (0, 1, 0)
 __version__ = '.'.join(str(_) for _ in __version_info__)
 
 from .exceptions import *
+from .structures import *
+from . import readers, writers
+from .readers import loads
+from .writers import dumps
```

