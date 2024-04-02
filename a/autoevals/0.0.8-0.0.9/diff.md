# Comparing `tmp/autoevals-0.0.8.tar.gz` & `tmp/autoevals-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoevals-0.0.8.tar", last modified: Sat Aug  5 03:06:26 2023, max compression
+gzip compressed data, was "autoevals-0.0.9.tar", last modified: Wed Aug 16 06:13:52 2023, max compression
```

## Comparing `autoevals-0.0.8.tar` & `autoevals-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-08-05 03:06:26.558447 autoevals-0.0.8/
--rw-r--r--   0 ankur      (501) staff       (20)     1072 2023-07-24 12:02:52.000000 autoevals-0.0.8/LICENSE
--rw-r--r--   0 ankur      (501) staff       (20)       43 2023-08-05 02:57:58.000000 autoevals-0.0.8/MANIFEST.in
--rw-r--r--   0 ankur      (501) staff       (20)     5514 2023-08-05 03:06:26.558339 autoevals-0.0.8/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)     4996 2023-08-05 03:06:24.000000 autoevals-0.0.8/README.md
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-08-05 03:06:26.553502 autoevals-0.0.8/py/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-08-05 03:06:26.555271 autoevals-0.0.8/py/autoevals/
--rw-r--r--   0 ankur      (501) staff       (20)      703 2023-07-26 05:13:53.000000 autoevals-0.0.8/py/autoevals/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)     1506 2023-07-26 00:14:45.000000 autoevals-0.0.8/py/autoevals/base.py
--rw-r--r--   0 ankur      (501) staff       (20)     8276 2023-08-05 02:58:57.000000 autoevals-0.0.8/py/autoevals/llm.py
--rw-r--r--   0 ankur      (501) staff       (20)     1866 2023-07-26 00:14:45.000000 autoevals-0.0.8/py/autoevals/oai.py
--rw-r--r--   0 ankur      (501) staff       (20)      708 2023-07-26 05:14:10.000000 autoevals-0.0.8/py/autoevals/string.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-08-05 03:06:26.557109 autoevals-0.0.8/py/autoevals/templates/
--rw-r--r--   0 ankur      (501) staff       (20)      355 2023-07-26 00:14:45.000000 autoevals-0.0.8/py/autoevals/templates/battle.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      312 2023-07-26 00:14:45.000000 autoevals-0.0.8/py/autoevals/templates/closed_q_a.yaml
--rw-r--r--   0 ankur      (501) staff       (20)     1121 2023-07-26 00:14:45.000000 autoevals-0.0.8/py/autoevals/templates/factuality.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      107 2023-07-26 00:14:45.000000 autoevals-0.0.8/py/autoevals/templates/humor.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      636 2023-07-26 00:14:45.000000 autoevals-0.0.8/py/autoevals/templates/possible.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      109 2023-07-26 05:02:36.000000 autoevals-0.0.8/py/autoevals/templates/security.yaml
--rw-r--r--   0 ankur      (501) staff       (20)     1076 2023-07-26 00:14:45.000000 autoevals-0.0.8/py/autoevals/templates/sql.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      356 2023-07-26 00:14:45.000000 autoevals-0.0.8/py/autoevals/templates/summary.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      683 2023-07-26 00:14:45.000000 autoevals-0.0.8/py/autoevals/templates/translation.yaml
--rw-r--r--   0 ankur      (501) staff       (20)     5132 2023-07-26 00:14:45.000000 autoevals-0.0.8/py/autoevals/test_llm.py
--rw-r--r--   0 ankur      (501) staff       (20)      546 2023-07-26 00:14:45.000000 autoevals-0.0.8/py/autoevals/test_string.py
--rw-r--r--   0 ankur      (501) staff       (20)      307 2023-07-26 00:14:45.000000 autoevals-0.0.8/py/autoevals/util.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-08-05 03:02:27.000000 autoevals-0.0.8/py/autoevals/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-08-05 03:06:26.555931 autoevals-0.0.8/py/autoevals.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)     5514 2023-08-05 03:06:26.000000 autoevals-0.0.8/py/autoevals.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      980 2023-08-05 03:06:26.000000 autoevals-0.0.8/py/autoevals.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-08-05 03:06:26.000000 autoevals-0.0.8/py/autoevals.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)      259 2023-08-05 03:06:26.000000 autoevals-0.0.8/py/autoevals.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       10 2023-08-05 03:06:26.000000 autoevals-0.0.8/py/autoevals.egg-info/top_level.txt
--rw-r--r--   0 ankur      (501) staff       (20)       31 2023-07-24 12:02:52.000000 autoevals-0.0.8/pyproject.toml
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-08-05 03:06:26.558484 autoevals-0.0.8/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1575 2023-08-05 02:58:28.000000 autoevals-0.0.8/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-08-05 03:06:26.558164 autoevals-0.0.8/templates/
--rw-r--r--   0 ankur      (501) staff       (20)      355 2023-07-26 00:14:45.000000 autoevals-0.0.8/templates/battle.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      312 2023-07-26 00:14:45.000000 autoevals-0.0.8/templates/closed_q_a.yaml
--rw-r--r--   0 ankur      (501) staff       (20)     1121 2023-07-26 00:14:45.000000 autoevals-0.0.8/templates/factuality.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      107 2023-07-26 00:14:45.000000 autoevals-0.0.8/templates/humor.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      636 2023-07-26 00:14:45.000000 autoevals-0.0.8/templates/possible.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      109 2023-07-26 05:02:36.000000 autoevals-0.0.8/templates/security.yaml
--rw-r--r--   0 ankur      (501) staff       (20)     1076 2023-07-26 00:14:45.000000 autoevals-0.0.8/templates/sql.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      356 2023-07-26 00:14:45.000000 autoevals-0.0.8/templates/summary.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      683 2023-07-26 00:14:45.000000 autoevals-0.0.8/templates/translation.yaml
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-08-16 06:13:52.873825 autoevals-0.0.9/
+-rw-r--r--   0 ankur      (501) staff       (20)     1072 2023-07-24 12:02:52.000000 autoevals-0.0.9/LICENSE
+-rw-r--r--   0 ankur      (501) staff       (20)       43 2023-08-05 02:57:58.000000 autoevals-0.0.9/MANIFEST.in
+-rw-r--r--   0 ankur      (501) staff       (20)     5514 2023-08-16 06:13:52.873691 autoevals-0.0.9/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)     4996 2023-08-16 06:13:50.000000 autoevals-0.0.9/README.md
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-08-16 06:13:52.866966 autoevals-0.0.9/py/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-08-16 06:13:52.870242 autoevals-0.0.9/py/autoevals/
+-rw-r--r--   0 ankur      (501) staff       (20)      703 2023-07-26 05:13:53.000000 autoevals-0.0.9/py/autoevals/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1506 2023-07-26 00:14:45.000000 autoevals-0.0.9/py/autoevals/base.py
+-rw-r--r--   0 ankur      (501) staff       (20)     8275 2023-08-14 17:25:45.000000 autoevals-0.0.9/py/autoevals/llm.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1865 2023-08-14 17:25:45.000000 autoevals-0.0.9/py/autoevals/oai.py
+-rw-r--r--   0 ankur      (501) staff       (20)      708 2023-07-26 05:14:10.000000 autoevals-0.0.9/py/autoevals/string.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-08-16 06:13:52.872365 autoevals-0.0.9/py/autoevals/templates/
+-rw-r--r--   0 ankur      (501) staff       (20)      355 2023-07-26 00:14:45.000000 autoevals-0.0.9/py/autoevals/templates/battle.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      312 2023-07-26 00:14:45.000000 autoevals-0.0.9/py/autoevals/templates/closed_q_a.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     1121 2023-07-26 00:14:45.000000 autoevals-0.0.9/py/autoevals/templates/factuality.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      107 2023-07-26 00:14:45.000000 autoevals-0.0.9/py/autoevals/templates/humor.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      636 2023-07-26 00:14:45.000000 autoevals-0.0.9/py/autoevals/templates/possible.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      109 2023-07-26 05:02:36.000000 autoevals-0.0.9/py/autoevals/templates/security.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     1076 2023-07-26 00:14:45.000000 autoevals-0.0.9/py/autoevals/templates/sql.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      356 2023-07-26 00:14:45.000000 autoevals-0.0.9/py/autoevals/templates/summary.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      683 2023-07-26 00:14:45.000000 autoevals-0.0.9/py/autoevals/templates/translation.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     5222 2023-08-14 17:25:45.000000 autoevals-0.0.9/py/autoevals/test_llm.py
+-rw-r--r--   0 ankur      (501) staff       (20)      546 2023-07-26 00:14:45.000000 autoevals-0.0.9/py/autoevals/test_string.py
+-rw-r--r--   0 ankur      (501) staff       (20)      307 2023-07-26 00:14:45.000000 autoevals-0.0.9/py/autoevals/util.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-08-16 06:13:46.000000 autoevals-0.0.9/py/autoevals/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-08-16 06:13:52.870900 autoevals-0.0.9/py/autoevals.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)     5514 2023-08-16 06:13:52.000000 autoevals-0.0.9/py/autoevals.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      980 2023-08-16 06:13:52.000000 autoevals-0.0.9/py/autoevals.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-08-16 06:13:52.000000 autoevals-0.0.9/py/autoevals.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      259 2023-08-16 06:13:52.000000 autoevals-0.0.9/py/autoevals.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       10 2023-08-16 06:13:52.000000 autoevals-0.0.9/py/autoevals.egg-info/top_level.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       80 2023-08-14 17:25:45.000000 autoevals-0.0.9/pyproject.toml
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-08-16 06:13:52.873863 autoevals-0.0.9/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1574 2023-08-14 17:25:45.000000 autoevals-0.0.9/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-08-16 06:13:52.873520 autoevals-0.0.9/templates/
+-rw-r--r--   0 ankur      (501) staff       (20)      355 2023-07-26 00:14:45.000000 autoevals-0.0.9/templates/battle.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      312 2023-07-26 00:14:45.000000 autoevals-0.0.9/templates/closed_q_a.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     1121 2023-07-26 00:14:45.000000 autoevals-0.0.9/templates/factuality.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      107 2023-07-26 00:14:45.000000 autoevals-0.0.9/templates/humor.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      636 2023-07-26 00:14:45.000000 autoevals-0.0.9/templates/possible.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      109 2023-07-26 05:02:36.000000 autoevals-0.0.9/templates/security.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     1076 2023-07-26 00:14:45.000000 autoevals-0.0.9/templates/sql.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      356 2023-07-26 00:14:45.000000 autoevals-0.0.9/templates/summary.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      683 2023-07-26 00:14:45.000000 autoevals-0.0.9/templates/translation.yaml
```

### Comparing `autoevals-0.0.8/LICENSE` & `autoevals-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/PKG-INFO` & `autoevals-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoevals
-Version: 0.0.8
+Version: 0.0.9
 Summary: Universal library for evaluating AI models
 Home-page: https://www.braintrustdata.com
 Author: BrainTrust
 Author-email: info@braintrustdata.com
 Project-URL: Bug Tracker, https://github.com/braintrustdata/autoevals
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `autoevals-0.0.8/README.md` & `autoevals-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/py/autoevals/__init__.py` & `autoevals-0.0.9/py/autoevals/__init__.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/py/autoevals/base.py` & `autoevals-0.0.9/py/autoevals/base.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/py/autoevals/llm.py` & `autoevals-0.0.9/py/autoevals/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import chevron
 import openai
 import yaml
 
 from .base import Score, Scorer
 from .oai import arun_cached_request, run_cached_request
 
-
 SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
 
 NO_COT_SUFFIX = """\
 Answer the question by printing only a single choice from {{__choices}} (without quotes or punctuation)
 corresponding to the correct answer with no other text.
 """.strip().replace(
     "\n", " "
```

### Comparing `autoevals-0.0.8/py/autoevals/oai.py` & `autoevals-0.0.9/py/autoevals/oai.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 import os
 import sqlite3
 import tempfile
 from pathlib import Path
 
-
 _CACHE_DIR = None
 _CONN = None
 
 
 def set_cache_dir(path):
     global _CACHE_DIR
     _CACHE_DIR = path
```

### Comparing `autoevals-0.0.8/py/autoevals/string.py` & `autoevals-0.0.9/py/autoevals/string.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/py/autoevals/templates/factuality.yaml` & `autoevals-0.0.9/py/autoevals/templates/factuality.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/py/autoevals/templates/possible.yaml` & `autoevals-0.0.9/py/autoevals/templates/possible.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/py/autoevals/templates/sql.yaml` & `autoevals-0.0.9/py/autoevals/templates/sql.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/py/autoevals/templates/translation.yaml` & `autoevals-0.0.9/py/autoevals/templates/translation.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/py/autoevals/test_llm.py` & `autoevals-0.0.9/py/autoevals/test_llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,18 @@
+import asyncio
 import os
+import re
 
 from autoevals.oai import set_cache_dir
 
-
 # By default, we use the user's tmp cache directory (e.g. in the Library/Caches dir on macOS)
 # However, we'd like to cache (and commit) the results of our tests, so we monkey patch the library
 # to use a cache directory in the project root.
 _SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
 set_cache_dir(os.path.join(_SCRIPT_DIR, "../../.testcache"))
-
-
-import asyncio
-import re
-
 from autoevals.llm import *
 
 
 def test_openai():
     def parse_best_title(grade):
         return int(re.findall(r"Winner: (\d+)", grade)[0])
 
@@ -112,21 +108,29 @@
     asyncio.run(nested_async())
 
 
 def test_battle():
     for use_cot in [True, False]:
         print("use_cot", use_cot)
         e = Battle(use_cot=use_cot)
-        response = e(instructions="Add the following numbers: 1, 2, 3", output="600", expected="6")
+        response = e(
+            instructions="Add the following numbers: 1, 2, 3",
+            output="600",
+            expected="6",
+        )
 
         print(response.as_json(indent=2))
         assert response.score == 0
         assert response.error is None
 
-        response = e(instructions="Add the following numbers: 1, 2, 3", output="6", expected="600")
+        response = e(
+            instructions="Add the following numbers: 1, 2, 3",
+            output="6",
+            expected="600",
+        )
 
         print(response.as_json(indent=2))
         assert response.score == (1 if use_cot else 0)
         assert response.error is None
 
         response = e(instructions="Add the following numbers: 1, 2, 3", output="6", expected="6")
```

### Comparing `autoevals-0.0.8/py/autoevals/test_string.py` & `autoevals-0.0.9/py/autoevals/test_string.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/py/autoevals.egg-info/PKG-INFO` & `autoevals-0.0.9/py/autoevals.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoevals
-Version: 0.0.8
+Version: 0.0.9
 Summary: Universal library for evaluating AI models
 Home-page: https://www.braintrustdata.com
 Author: BrainTrust
 Author-email: info@braintrustdata.com
 Project-URL: Bug Tracker, https://github.com/braintrustdata/autoevals
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `autoevals-0.0.8/py/autoevals.egg-info/SOURCES.txt` & `autoevals-0.0.9/py/autoevals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/setup.py` & `autoevals-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 
 import setuptools
 
-
 dir_name = os.path.abspath(os.path.dirname(__file__))
 
 version_contents = {}
 with open(os.path.join(dir_name, "py", "autoevals", "version.py"), encoding="utf-8") as f:
     exec(f.read(), version_contents)
 
 with open(os.path.join(dir_name, "README.md"), "r", encoding="utf-8") as f:
```

### Comparing `autoevals-0.0.8/templates/factuality.yaml` & `autoevals-0.0.9/templates/factuality.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/templates/possible.yaml` & `autoevals-0.0.9/templates/possible.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/templates/sql.yaml` & `autoevals-0.0.9/templates/sql.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.8/templates/translation.yaml` & `autoevals-0.0.9/templates/translation.yaml`

 * *Files identical despite different names*

