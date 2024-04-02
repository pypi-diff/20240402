# Comparing `tmp/glapi-0.7.5.tar.gz` & `tmp/glapi-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glapi-0.7.5.tar", last modified: Tue Feb 27 00:43:26 2024, max compression
+gzip compressed data, was "glapi-0.7.6.tar", last modified: Tue Apr  2 00:42:46 2024, max compression
```

## Comparing `glapi-0.7.5.tar` & `glapi-0.7.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:43:26.543150 glapi-0.7.5/
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-02-27 00:43:16.000000 glapi-0.7.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      493 2024-02-27 00:43:26.543150 glapi-0.7.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-02-27 00:43:16.000000 glapi-0.7.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2024-02-27 00:43:16.000000 glapi-0.7.5/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:43:26.538150 glapi-0.7.5/glapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-27 00:43:16.000000 glapi-0.7.5/glapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2024-02-27 00:43:16.000000 glapi-0.7.5/glapi/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5279 2024-02-27 00:43:16.000000 glapi-0.7.5/glapi/connection.py
--rw-rw-rw-   0 root         (0) root         (0)     5925 2024-02-27 00:43:16.000000 glapi-0.7.5/glapi/epic.py
--rw-rw-rw-   0 root         (0) root         (0)     4745 2024-02-27 00:43:16.000000 glapi-0.7.5/glapi/group.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-02-27 00:43:16.000000 glapi-0.7.5/glapi/issue.py
--rw-rw-rw-   0 root         (0) root         (0)     5175 2024-02-27 00:43:16.000000 glapi-0.7.5/glapi/project.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2024-02-27 00:43:16.000000 glapi-0.7.5/glapi/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:43:26.542150 glapi-0.7.5/glapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      493 2024-02-27 00:43:26.000000 glapi-0.7.5/glapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2024-02-27 00:43:26.000000 glapi-0.7.5/glapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 00:43:26.000000 glapi-0.7.5/glapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-02-27 00:43:26.000000 glapi-0.7.5/glapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-02-27 00:43:26.000000 glapi-0.7.5/glapi.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-02-27 00:43:16.000000 glapi-0.7.5/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2024-02-27 00:43:16.000000 glapi-0.7.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 00:43:26.543150 glapi-0.7.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      698 2024-02-27 00:43:16.000000 glapi-0.7.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:43:26.542150 glapi-0.7.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)      213 2024-02-27 00:43:16.000000 glapi-0.7.5/tests/test_class-gitlabconnection.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-02-27 00:43:16.000000 glapi-0.7.5/tests/test_class-gitlabepic.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-02-27 00:43:16.000000 glapi-0.7.5/tests/test_class-gitlabgroup.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2024-02-27 00:43:16.000000 glapi-0.7.5/tests/test_class-gitlabissue.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2024-02-27 00:43:16.000000 glapi-0.7.5/tests/test_class-gitlabproject.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2024-02-27 00:43:16.000000 glapi-0.7.5/tests/test_class-gitlabuser.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-02-27 00:43:16.000000 glapi-0.7.5/tests/test_package-build.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 00:42:46.371662 glapi-0.7.6/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-04-02 00:42:33.000000 glapi-0.7.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      493 2024-04-02 00:42:46.371662 glapi-0.7.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-02 00:42:33.000000 glapi-0.7.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-04-02 00:42:33.000000 glapi-0.7.6/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 00:42:46.367662 glapi-0.7.6/glapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 00:42:33.000000 glapi-0.7.6/glapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      731 2024-04-02 00:42:33.000000 glapi-0.7.6/glapi/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5375 2024-04-02 00:42:33.000000 glapi-0.7.6/glapi/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     5925 2024-04-02 00:42:33.000000 glapi-0.7.6/glapi/epic.py
+-rw-rw-rw-   0 root         (0) root         (0)     4745 2024-04-02 00:42:33.000000 glapi-0.7.6/glapi/group.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-04-02 00:42:33.000000 glapi-0.7.6/glapi/issue.py
+-rw-rw-rw-   0 root         (0) root         (0)     5175 2024-04-02 00:42:33.000000 glapi-0.7.6/glapi/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2024-04-02 00:42:33.000000 glapi-0.7.6/glapi/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 00:42:46.370662 glapi-0.7.6/glapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      493 2024-04-02 00:42:46.000000 glapi-0.7.6/glapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2024-04-02 00:42:46.000000 glapi-0.7.6/glapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 00:42:46.000000 glapi-0.7.6/glapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-02 00:42:46.000000 glapi-0.7.6/glapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-02 00:42:46.000000 glapi-0.7.6/glapi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-02 00:42:33.000000 glapi-0.7.6/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-02 00:42:33.000000 glapi-0.7.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 00:42:46.371662 glapi-0.7.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      698 2024-04-02 00:42:33.000000 glapi-0.7.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 00:42:46.370662 glapi-0.7.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-04-02 00:42:33.000000 glapi-0.7.6/tests/test_class-gitlabconnection.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-04-02 00:42:33.000000 glapi-0.7.6/tests/test_class-gitlabepic.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-02 00:42:33.000000 glapi-0.7.6/tests/test_class-gitlabgroup.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2024-04-02 00:42:33.000000 glapi-0.7.6/tests/test_class-gitlabissue.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-04-02 00:42:33.000000 glapi-0.7.6/tests/test_class-gitlabproject.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2024-04-02 00:42:33.000000 glapi-0.7.6/tests/test_class-gitlabuser.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-02 00:42:33.000000 glapi-0.7.6/tests/test_package-build.py
```

### Comparing `glapi-0.7.5/glapi/configuration.py` & `glapi-0.7.6/glapi/configuration.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.5/glapi/connection.py` & `glapi-0.7.6/glapi/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
         except Exception as e:
             raise e
 
         # read in as dictionary and expose some request info
         return {
             "data": json.loads(result.text) if (result.status_code == 200 and result.text and "raw" not in endpoint and "ref" not in params) else (result.text if "raw" in endpoint and "ref" in params else list()),
             "headers": result.headers,
+            "message": result.json()["message"] if result.status_code > 200 else result.reason,
             "status": result.status_code
         }
 
     def paginate(self, endpoint, params=dict(), data=list()):
         """
         Paginate through GitLab API headers to ensure all results captured.
```

### Comparing `glapi-0.7.5/glapi/epic.py` & `glapi-0.7.6/glapi/epic.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.5/glapi/group.py` & `glapi-0.7.6/glapi/group.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.5/glapi/issue.py` & `glapi-0.7.6/glapi/issue.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.5/glapi/project.py` & `glapi-0.7.6/glapi/project.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.5/glapi/user.py` & `glapi-0.7.6/glapi/user.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.5/glapi.egg-info/SOURCES.txt` & `glapi-0.7.6/glapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glapi-0.7.5/setup.py` & `glapi-0.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.5/tests/test_class-gitlabepic.py` & `glapi-0.7.6/tests/test_class-gitlabepic.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.5/tests/test_class-gitlabgroup.py` & `glapi-0.7.6/tests/test_class-gitlabgroup.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.5/tests/test_class-gitlabissue.py` & `glapi-0.7.6/tests/test_class-gitlabissue.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.5/tests/test_class-gitlabproject.py` & `glapi-0.7.6/tests/test_class-gitlabproject.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.5/tests/test_class-gitlabuser.py` & `glapi-0.7.6/tests/test_class-gitlabuser.py`

 * *Files identical despite different names*

