# Comparing `tmp/ploomber-cloud-0.1.8.tar.gz` & `tmp/ploomber-cloud-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomber-cloud-0.1.8.tar", last modified: Thu Feb  1 02:18:15 2024, max compression
+gzip compressed data, was "ploomber-cloud-0.1.9.tar", last modified: Thu Feb  1 19:55:40 2024, max compression
```

## Comparing `ploomber-cloud-0.1.8.tar` & `ploomber-cloud-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:18:15.642361 ploomber-cloud-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-01 02:18:15.642361 ploomber-cloud-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-01 02:18:15.642361 ploomber-cloud-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:18:15.638361 ploomber-cloud-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:18:15.642361 ploomber-cloud-0.1.8/src/ploomber_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/src/ploomber_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/src/ploomber_cloud/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/src/ploomber_cloud/api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/src/ploomber_cloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/src/ploomber_cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/src/ploomber_cloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/src/ploomber_cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/src/ploomber_cloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/src/ploomber_cloud/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/src/ploomber_cloud/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/src/ploomber_cloud/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-02-01 02:17:58.000000 ploomber-cloud-0.1.8/src/ploomber_cloud/zip_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:18:15.642361 ploomber-cloud-0.1.8/src/ploomber_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-01 02:18:15.000000 ploomber-cloud-0.1.8/src/ploomber_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-01 02:18:15.000000 ploomber-cloud-0.1.8/src/ploomber_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 02:18:15.000000 ploomber-cloud-0.1.8/src/ploomber_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-01 02:18:15.000000 ploomber-cloud-0.1.8/src/ploomber_cloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-01 02:18:15.000000 ploomber-cloud-0.1.8/src/ploomber_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-01 02:18:15.000000 ploomber-cloud-0.1.8/src/ploomber_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:55:40.404400 ploomber-cloud-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-01 19:55:40.404400 ploomber-cloud-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-01 19:55:40.404400 ploomber-cloud-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:55:40.400400 ploomber-cloud-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:55:40.400400 ploomber-cloud-0.1.9/src/ploomber_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/zip_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:55:40.400400 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-01 19:55:40.000000 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-01 19:55:40.000000 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 19:55:40.000000 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-01 19:55:40.000000 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-01 19:55:40.000000 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-01 19:55:40.000000 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/top_level.txt
```

### Comparing `ploomber-cloud-0.1.8/CHANGELOG.md` & `ploomber-cloud-0.1.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## 0.1.9 (2024-02-01)
+
+- [Feature] Add support for Solara applications ([#31](https://github.com/ploomber/ploomber-cloud/issues/31))
+
 ## 0.1.8 (2024-01-31)
 
 - [Feature] Add support for secrets via `.env` file ([#26](https://github.com/ploomber/ploomber-cloud/issues/26))
 - [Fix] Shorter error when trying to deploy a project that hasn't been initialized
 - [Fix] Changed deployment link from `dashboards` to `applications` ([#34](https://github.com/ploomber/ploomber-cloud/issues/34))
 
 ## 0.1.7 (2024-01-24)
```

### Comparing `ploomber-cloud-0.1.8/pyproject.toml` & `ploomber-cloud-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.1.8/setup.py` & `ploomber-cloud-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.1.8/src/ploomber_cloud/api.py` & `ploomber-cloud-0.1.9/src/ploomber_cloud/api.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.1.8/src/ploomber_cloud/api_key.py` & `ploomber-cloud-0.1.9/src/ploomber_cloud/api_key.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.1.8/src/ploomber_cloud/cli.py` & `ploomber-cloud-0.1.9/src/ploomber_cloud/cli.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.1.8/src/ploomber_cloud/config.py` & `ploomber-cloud-0.1.9/src/ploomber_cloud/config.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.1.8/src/ploomber_cloud/deploy.py` & `ploomber-cloud-0.1.9/src/ploomber_cloud/deploy.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.1.8/src/ploomber_cloud/github.py` & `ploomber-cloud-0.1.9/src/ploomber_cloud/github.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.1.8/src/ploomber_cloud/init.py` & `ploomber-cloud-0.1.9/src/ploomber_cloud/init.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.1.8/src/ploomber_cloud/util.py` & `ploomber-cloud-0.1.9/src/ploomber_cloud/util.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.1.8/src/ploomber_cloud/zip_.py` & `ploomber-cloud-0.1.9/src/ploomber_cloud/zip_.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.1.8/src/ploomber_cloud.egg-info/SOURCES.txt` & `ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

