# Comparing `tmp/ortelius-cli-9.3.265.tar.gz` & `tmp/ortelius-cli-9.3.266.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortelius-cli-9.3.265.tar", last modified: Thu Mar 21 23:57:27 2024, max compression
+gzip compressed data, was "ortelius-cli-9.3.266.tar", last modified: Tue Apr  2 20:42:51 2024, max compression
```

## Comparing `ortelius-cli-9.3.265.tar` & `ortelius-cli-9.3.266.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-03-21 23:57:27.744907 ortelius-cli-9.3.265/
--rw-r--r--   0 steve      (502) staff       (20)    10480 2023-12-11 19:25:24.000000 ortelius-cli-9.3.265/LICENSE
--rw-r--r--   0 steve      (502) staff       (20)       17 2023-12-11 19:25:24.000000 ortelius-cli-9.3.265/MANIFEST.in
--rw-r--r--   0 steve      (502) staff       (20)    12461 2024-03-21 23:57:27.743636 ortelius-cli-9.3.265/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      818 2023-12-11 19:25:24.000000 ortelius-cli-9.3.265/README.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-03-21 23:57:27.656684 ortelius-cli-9.3.265/bin/
--rwxr-xr-x   0 steve      (502) staff       (20)    70841 2024-03-21 23:56:49.000000 ortelius-cli-9.3.265/bin/dh
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-03-21 23:57:27.662042 ortelius-cli-9.3.265/deployhub/
--rw-r--r--   0 steve      (502) staff       (20)       65 2024-03-21 23:56:49.000000 ortelius-cli-9.3.265/deployhub/__init__.py
--rw-r--r--   0 steve      (502) staff       (20)    71098 2024-03-21 23:53:08.000000 ortelius-cli-9.3.265/deployhub/dhapi.py
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-03-21 23:57:27.664568 ortelius-cli-9.3.265/doc/
--rw-r--r--   0 steve      (502) staff       (20)    23768 2023-12-11 19:25:24.000000 ortelius-cli-9.3.265/doc/deployhub.md
--rw-r--r--   0 steve      (502) staff       (20)    11674 2023-12-11 19:25:24.000000 ortelius-cli-9.3.265/doc/dh.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-03-21 23:57:27.741421 ortelius-cli-9.3.265/ortelius_cli.egg-info/
--rw-r--r--   0 steve      (502) staff       (20)    12461 2024-03-21 23:57:27.000000 ortelius-cli-9.3.265/ortelius_cli.egg-info/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      292 2024-03-21 23:57:27.000000 ortelius-cli-9.3.265/ortelius_cli.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (502) staff       (20)        1 2024-03-21 23:57:27.000000 ortelius-cli-9.3.265/ortelius_cli.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (502) staff       (20)       68 2024-03-21 23:57:27.000000 ortelius-cli-9.3.265/ortelius_cli.egg-info/requires.txt
--rw-r--r--   0 steve      (502) staff       (20)       10 2024-03-21 23:57:27.000000 ortelius-cli-9.3.265/ortelius_cli.egg-info/top_level.txt
--rw-r--r--   0 steve      (502) staff       (20)       38 2024-03-21 23:57:27.745092 ortelius-cli-9.3.265/setup.cfg
--rw-r--r--   0 steve      (502) staff       (20)     1069 2024-03-21 23:56:49.000000 ortelius-cli-9.3.265/setup.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-02 20:42:51.229957 ortelius-cli-9.3.266/
+-rw-r--r--   0 steve      (502) staff       (20)    10480 2023-12-11 19:25:24.000000 ortelius-cli-9.3.266/LICENSE
+-rw-r--r--   0 steve      (502) staff       (20)       17 2023-12-11 19:25:24.000000 ortelius-cli-9.3.266/MANIFEST.in
+-rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-02 20:42:51.228391 ortelius-cli-9.3.266/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      818 2023-12-11 19:25:24.000000 ortelius-cli-9.3.266/README.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-02 20:42:51.212846 ortelius-cli-9.3.266/bin/
+-rwxr-xr-x   0 steve      (502) staff       (20)    70820 2024-04-02 20:42:32.000000 ortelius-cli-9.3.266/bin/dh
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-02 20:42:51.215039 ortelius-cli-9.3.266/deployhub/
+-rw-r--r--   0 steve      (502) staff       (20)       65 2024-04-02 20:42:32.000000 ortelius-cli-9.3.266/deployhub/__init__.py
+-rw-r--r--   0 steve      (502) staff       (20)    71098 2024-03-21 23:53:08.000000 ortelius-cli-9.3.266/deployhub/dhapi.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-02 20:42:51.217553 ortelius-cli-9.3.266/doc/
+-rw-r--r--   0 steve      (502) staff       (20)    23768 2023-12-11 19:25:24.000000 ortelius-cli-9.3.266/doc/deployhub.md
+-rw-r--r--   0 steve      (502) staff       (20)    11674 2023-12-11 19:25:24.000000 ortelius-cli-9.3.266/doc/dh.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-02 20:42:51.223299 ortelius-cli-9.3.266/ortelius_cli.egg-info/
+-rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-02 20:42:51.000000 ortelius-cli-9.3.266/ortelius_cli.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      292 2024-04-02 20:42:51.000000 ortelius-cli-9.3.266/ortelius_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (502) staff       (20)        1 2024-04-02 20:42:51.000000 ortelius-cli-9.3.266/ortelius_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (502) staff       (20)       68 2024-04-02 20:42:51.000000 ortelius-cli-9.3.266/ortelius_cli.egg-info/requires.txt
+-rw-r--r--   0 steve      (502) staff       (20)       10 2024-04-02 20:42:51.000000 ortelius-cli-9.3.266/ortelius_cli.egg-info/top_level.txt
+-rw-r--r--   0 steve      (502) staff       (20)       38 2024-04-02 20:42:51.230714 ortelius-cli-9.3.266/setup.cfg
+-rw-r--r--   0 steve      (502) staff       (20)     1069 2024-04-02 20:42:32.000000 ortelius-cli-9.3.266/setup.py
```

### Comparing `ortelius-cli-9.3.265/LICENSE` & `ortelius-cli-9.3.266/LICENSE`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.265/PKG-INFO` & `ortelius-cli-9.3.266/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.265
+Version: 9.3.266
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/ortelius-cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.265/README.md` & `ortelius-cli-9.3.266/README.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.265/bin/dh` & `ortelius-cli-9.3.266/bin/dh`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     `--todom` To Domain
 
 """
 
 # To generate markdown use:
 # pydoc-markdown -I bin | awk '/dh.main/ {p=1}; p==0 {print}'
 
-__version__ = "9.3.265"
+__version__ = "9.3.266"
 
 import json
 import os
 import re
 import stat
 import sys
 from datetime import datetime
@@ -1423,15 +1423,15 @@
 
     # if the buildnum, git_repo, git_url, git_commit_time, git_lines not in os.environ and not in attrvars and not in export then export
     run_fetch = True
     if mapping.get("SHORT_SHA", None) is None:
         mapping["SHORT_SHA"] = dhapi.run_cmd("git log --oneline -n 1 | cut -d' '  -f1")
 
     if mapping.get("GIT_COMMIT", None) is None:
-        mapping["GIT_COMMIT"] = dhapi.run_cmd("git log --oneline -n 1 | cut -d' '  -f1")
+        mapping["GIT_COMMIT"] = dhapi.run_cmd("git rev-parse HEAD")
 
     if mapping.get("GIT_VERIFY_COMMIT", None) is None:
         mapping["GIT_VERIFY_COMMIT"] = dhapi.run_cmd("git verify-commit " + mapping.get("GIT_COMMIT", "") + " 2>&1 | grep -i 'Signature made' | wc -l")
 
     if mapping.get("GIT_SIGNED_OFF_BY", None) is None:
         mapping["GIT_SIGNED_OFF_BY"] = dhapi.run_cmd(
             "git log -1 " + mapping.get("GIT_COMMIT", "") + " | grep 'Signed-off-by:' | cut -d: -f2 | sed 's/^[ \t]*//;s/[ \t]*$//' | sed 's/&/&amp;/g; s/</&lt;/g; s/>/&gt;/g;'"
```

### Comparing `ortelius-cli-9.3.265/deployhub/dhapi.py` & `ortelius-cli-9.3.266/deployhub/dhapi.py`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.265/doc/deployhub.md` & `ortelius-cli-9.3.266/doc/deployhub.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.265/doc/dh.md` & `ortelius-cli-9.3.266/doc/dh.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.265/ortelius_cli.egg-info/PKG-INFO` & `ortelius-cli-9.3.266/ortelius_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.265
+Version: 9.3.266
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/ortelius-cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.265/setup.py` & `ortelius-cli-9.3.266/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "Issues": "https://github.com/ortelius/ortelius/issues",
         "Ortelius CLI Documentation": "https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md",
         "Python Python API Documentation": "https://github.com/ortelius/ortelius-cli/blob/main/doc/deployhub.md",
     },
     author="Steve Taylor",
     author_email="steve@deployhub.com",
     name="ortelius-cli",
-    version="9.3.265",
+    version="9.3.266",
     packages=[
         "deployhub",
     ],
     scripts=["bin/dh"],
     license="Apache-2.0",
     long_description=open("doc/dh.md").read(),
     long_description_content_type="text/markdown",
```

