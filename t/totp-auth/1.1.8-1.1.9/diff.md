# Comparing `tmp/totp_auth-1.1.8.tar.gz` & `tmp/totp_auth-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totp_auth-1.1.8.tar", last modified: Sat Mar 30 12:52:21 2024, max compression
+gzip compressed data, was "totp_auth-1.1.9.tar", last modified: Sat Mar 30 12:55:30 2024, max compression
```

## Comparing `totp_auth-1.1.8.tar` & `totp_auth-1.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:52:21.313761 totp_auth-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-30 12:52:17.000000 totp_auth-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-30 12:52:21.313761 totp_auth-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-30 12:52:17.000000 totp_auth-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-30 12:52:17.000000 totp_auth-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 12:52:21.313761 totp_auth-1.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:52:21.309761 totp_auth-1.1.8/totp_auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:52:17.000000 totp_auth-1.1.8/totp_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:52:21.313761 totp_auth-1.1.8/totp_auth/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-30 12:52:17.000000 totp_auth-1.1.8/totp_auth/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-03-30 12:52:17.000000 totp_auth-1.1.8/totp_auth/classes/db_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-30 12:52:17.000000 totp_auth-1.1.8/totp_auth/classes/http_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-30 12:52:17.000000 totp_auth-1.1.8/totp_auth/classes/page_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-03-30 12:52:17.000000 totp_auth-1.1.8/totp_auth/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-30 12:52:17.000000 totp_auth-1.1.8/totp_auth/cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-03-30 12:52:17.000000 totp_auth-1.1.8/totp_auth/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:52:21.313761 totp_auth-1.1.8/totp_auth/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-30 12:52:17.000000 totp_auth-1.1.8/totp_auth/migrations/1.sql
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-30 12:52:17.000000 totp_auth-1.1.8/totp_auth/migrations/_default.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-30 12:52:17.000000 totp_auth-1.1.8/totp_auth/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-30 12:52:17.000000 totp_auth-1.1.8/totp_auth/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:52:21.313761 totp_auth-1.1.8/totp_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-30 12:52:21.000000 totp_auth-1.1.8/totp_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-30 12:52:21.000000 totp_auth-1.1.8/totp_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 12:52:21.000000 totp_auth-1.1.8/totp_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-30 12:52:21.000000 totp_auth-1.1.8/totp_auth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-30 12:52:21.000000 totp_auth-1.1.8/totp_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-30 12:52:21.000000 totp_auth-1.1.8/totp_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:55:30.744636 totp_auth-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-30 12:55:26.000000 totp_auth-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-30 12:55:30.740636 totp_auth-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-30 12:55:26.000000 totp_auth-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-30 12:55:26.000000 totp_auth-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 12:55:30.744636 totp_auth-1.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:55:30.740636 totp_auth-1.1.9/totp_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:55:26.000000 totp_auth-1.1.9/totp_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:55:30.740636 totp_auth-1.1.9/totp_auth/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-30 12:55:26.000000 totp_auth-1.1.9/totp_auth/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-03-30 12:55:26.000000 totp_auth-1.1.9/totp_auth/classes/db_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-30 12:55:26.000000 totp_auth-1.1.9/totp_auth/classes/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-30 12:55:26.000000 totp_auth-1.1.9/totp_auth/classes/page_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-03-30 12:55:26.000000 totp_auth-1.1.9/totp_auth/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-30 12:55:26.000000 totp_auth-1.1.9/totp_auth/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-03-30 12:55:26.000000 totp_auth-1.1.9/totp_auth/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:55:30.740636 totp_auth-1.1.9/totp_auth/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-30 12:55:26.000000 totp_auth-1.1.9/totp_auth/migrations/1.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-30 12:55:26.000000 totp_auth-1.1.9/totp_auth/migrations/_default.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-30 12:55:26.000000 totp_auth-1.1.9/totp_auth/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-30 12:55:26.000000 totp_auth-1.1.9/totp_auth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:55:30.740636 totp_auth-1.1.9/totp_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-30 12:55:30.000000 totp_auth-1.1.9/totp_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-30 12:55:30.000000 totp_auth-1.1.9/totp_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 12:55:30.000000 totp_auth-1.1.9/totp_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-30 12:55:30.000000 totp_auth-1.1.9/totp_auth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-30 12:55:30.000000 totp_auth-1.1.9/totp_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-30 12:55:30.000000 totp_auth-1.1.9/totp_auth.egg-info/top_level.txt
```

### Comparing `totp_auth-1.1.8/LICENSE` & `totp_auth-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `totp_auth-1.1.8/PKG-INFO` & `totp_auth-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totp_auth
-Version: 1.1.8
+Version: 1.1.9
 Summary: Easy setup totp-based login for your application
 Author-email: MoxForever <moxforever10@gmail.com>
 Project-URL: Homepage, https://github.com/MoxForever/totp_auth
 Project-URL: Issues, https://github.com/MoxForever/totp_auth/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `totp_auth-1.1.8/README.md` & `totp_auth-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `totp_auth-1.1.8/pyproject.toml` & `totp_auth-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "totp_auth"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
     { name="MoxForever", email="moxforever10@gmail.com" },
 ]
 description = "Easy setup totp-based login for your application"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `totp_auth-1.1.8/totp_auth/classes/db_config.py` & `totp_auth-1.1.9/totp_auth/classes/db_config.py`

 * *Files identical despite different names*

### Comparing `totp_auth-1.1.8/totp_auth/classes/http_request.py` & `totp_auth-1.1.9/totp_auth/classes/http_request.py`

 * *Files identical despite different names*

### Comparing `totp_auth-1.1.8/totp_auth/cli.py` & `totp_auth-1.1.9/totp_auth/cli.py`

 * *Files identical despite different names*

### Comparing `totp_auth-1.1.8/totp_auth/cookie.py` & `totp_auth-1.1.9/totp_auth/cookie.py`

 * *Files identical despite different names*

### Comparing `totp_auth-1.1.8/totp_auth/login.html` & `totp_auth-1.1.9/totp_auth/login.html`

 * *Files identical despite different names*

### Comparing `totp_auth-1.1.8/totp_auth/migrations/1.sql` & `totp_auth-1.1.9/totp_auth/migrations/1.sql`

 * *Files identical despite different names*

### Comparing `totp_auth-1.1.8/totp_auth/server.py` & `totp_auth-1.1.9/totp_auth/server.py`

 * *Files identical despite different names*

### Comparing `totp_auth-1.1.8/totp_auth.egg-info/PKG-INFO` & `totp_auth-1.1.9/totp_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totp_auth
-Version: 1.1.8
+Version: 1.1.9
 Summary: Easy setup totp-based login for your application
 Author-email: MoxForever <moxforever10@gmail.com>
 Project-URL: Homepage, https://github.com/MoxForever/totp_auth
 Project-URL: Issues, https://github.com/MoxForever/totp_auth/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `totp_auth-1.1.8/totp_auth.egg-info/SOURCES.txt` & `totp_auth-1.1.9/totp_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

