# Comparing `tmp/creyPY-0.1.2.tar.gz` & `tmp/creyPY-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creyPY-0.1.2.tar", last modified: Mon Apr  1 18:59:25 2024, max compression
+gzip compressed data, was "creyPY-0.2.0.tar", last modified: Tue Apr  2 09:42:00 2024, max compression
```

## Comparing `creyPY-0.1.2.tar` & `creyPY-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:25.813212 creyPY-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-01 18:59:11.000000 creyPY-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-01 18:59:25.813212 creyPY-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-01 18:59:11.000000 creyPY-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:25.809212 creyPY-0.1.2/creyPY/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:11.000000 creyPY-0.1.2/creyPY/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:25.813212 creyPY-0.1.2/creyPY/const/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-01 18:59:11.000000 creyPY-0.1.2/creyPY/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-01 18:59:11.000000 creyPY-0.1.2/creyPY/const/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-01 18:59:11.000000 creyPY-0.1.2/creyPY/const/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-01 18:59:11.000000 creyPY-0.1.2/creyPY/const/stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:25.813212 creyPY-0.1.2/creyPY/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-01 18:59:11.000000 creyPY-0.1.2/creyPY/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-01 18:59:11.000000 creyPY-0.1.2/creyPY/fastapi/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-01 18:59:11.000000 creyPY-0.1.2/creyPY/fastapi/crud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:25.813212 creyPY-0.1.2/creyPY/fastapi/models/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 18:59:11.000000 creyPY-0.1.2/creyPY/fastapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-01 18:59:11.000000 creyPY-0.1.2/creyPY/fastapi/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-01 18:59:11.000000 creyPY-0.1.2/creyPY/fastapi/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:25.813212 creyPY-0.1.2/creyPY/fastapi/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 18:59:11.000000 creyPY-0.1.2/creyPY/fastapi/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-01 18:59:11.000000 creyPY-0.1.2/creyPY/fastapi/schemas/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:59:25.813212 creyPY-0.1.2/creyPY.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-01 18:59:25.000000 creyPY-0.1.2/creyPY.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-01 18:59:25.000000 creyPY-0.1.2/creyPY.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:59:25.000000 creyPY-0.1.2/creyPY.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-01 18:59:25.000000 creyPY-0.1.2/creyPY.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 18:59:25.000000 creyPY-0.1.2/creyPY.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:59:25.813212 creyPY-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-01 18:59:11.000000 creyPY-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.828273 creyPY-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 09:41:46.000000 creyPY-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-02 09:42:00.828273 creyPY-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 09:41:46.000000 creyPY-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.824273 creyPY-0.2.0/creyPY/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.824273 creyPY-0.2.0/creyPY/const/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/const/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/const/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/const/stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.824273 creyPY-0.2.0/creyPY/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/crud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.824273 creyPY-0.2.0/creyPY/fastapi/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.824273 creyPY-0.2.0/creyPY/fastapi/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-02 09:41:46.000000 creyPY-0.2.0/creyPY/fastapi/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:42:00.824273 creyPY-0.2.0/creyPY.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-02 09:42:00.000000 creyPY-0.2.0/creyPY.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-02 09:42:00.000000 creyPY-0.2.0/creyPY.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:42:00.000000 creyPY-0.2.0/creyPY.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 09:42:00.000000 creyPY-0.2.0/creyPY.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 09:42:00.000000 creyPY-0.2.0/creyPY.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:42:00.828273 creyPY-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-02 09:41:46.000000 creyPY-0.2.0/setup.py
```

### Comparing `creyPY-0.1.2/LICENSE` & `creyPY-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `creyPY-0.1.2/PKG-INFO` & `creyPY-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: creyPY
-Version: 0.1.2
+Version: 0.2.0
 Summary: Collection of my Python and FastAPI shortcuts, snippets etc.
 Home-page: https://github.com/creyD/creyPY
 Author: Conrad Großer
 Author-email: conrad@noah.tech
 License: MIT
+Keywords: creyPY,Python,FastAPI,shortcuts,snippets,utils,personal library
+Platform: any
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pydantic-core==2.16.3
 Requires-Dist: typing-extensions==4.10.0
```

### Comparing `creyPY-0.1.2/creyPY/const/i18n.py` & `creyPY-0.2.0/creyPY/const/i18n.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.1.2/creyPY/const/stripe.py` & `creyPY-0.2.0/creyPY/const/stripe.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.1.2/creyPY/fastapi/app.py` & `creyPY-0.2.0/creyPY/fastapi/app.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.1.2/creyPY/fastapi/crud.py` & `creyPY-0.2.0/creyPY/fastapi/crud.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.1.2/creyPY/fastapi/models/base.py` & `creyPY-0.2.0/creyPY/fastapi/models/base.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.1.2/creyPY/fastapi/pagination.py` & `creyPY-0.2.0/creyPY/fastapi/pagination.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.1.2/creyPY.egg-info/PKG-INFO` & `creyPY-0.2.0/creyPY.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: creyPY
-Version: 0.1.2
+Version: 0.2.0
 Summary: Collection of my Python and FastAPI shortcuts, snippets etc.
 Home-page: https://github.com/creyD/creyPY
 Author: Conrad Großer
 Author-email: conrad@noah.tech
 License: MIT
+Keywords: creyPY,Python,FastAPI,shortcuts,snippets,utils,personal library
+Platform: any
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pydantic-core==2.16.3
 Requires-Dist: typing-extensions==4.10.0
```

### Comparing `creyPY-0.1.2/creyPY.egg-info/SOURCES.txt` & `creyPY-0.2.0/creyPY.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,11 +11,12 @@
 creyPY/const/groups.py
 creyPY/const/i18n.py
 creyPY/const/stripe.py
 creyPY/fastapi/__init__.py
 creyPY/fastapi/app.py
 creyPY/fastapi/crud.py
 creyPY/fastapi/pagination.py
+creyPY/fastapi/testing.py
 creyPY/fastapi/models/__init__.py
 creyPY/fastapi/models/base.py
 creyPY/fastapi/schemas/__init__.py
 creyPY/fastapi/schemas/base.py
```

### Comparing `creyPY-0.1.2/setup.py` & `creyPY-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,8 +29,18 @@
     author="Conrad Großer",
     author_email="conrad@noah.tech",
     packages=find_packages(),
     url="https://github.com/creyD/creyPY",
     license="MIT",
     python_requires=">=3.12",
     install_requires=requirements,
+    keywords=[
+        "creyPY",
+        "Python",
+        "FastAPI",
+        "shortcuts",
+        "snippets",
+        "utils",
+        "personal library",
+    ],
+    platforms="any",
 )
```

