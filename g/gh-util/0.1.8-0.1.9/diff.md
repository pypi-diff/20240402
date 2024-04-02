# Comparing `tmp/gh_util-0.1.8.tar.gz` & `tmp/gh_util-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gh_util-0.1.8.tar", last modified: Tue Mar 26 02:09:48 2024, max compression
+gzip compressed data, was "gh_util-0.1.9.tar", last modified: Wed Mar 27 06:01:53 2024, max compression
```

## Comparing `gh_util-0.1.8.tar` & `gh_util-0.1.9.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:48.479872 gh_util-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:48.455872 gh_util-0.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-26 02:09:41.000000 gh_util-0.1.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:48.455872 gh_util-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-26 02:09:41.000000 gh_util-0.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-26 02:09:41.000000 gh_util-0.1.8/.github/workflows/static-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-03-26 02:09:41.000000 gh_util-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-26 02:09:41.000000 gh_util-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-03-26 02:09:48.475872 gh_util-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-03-26 02:09:41.000000 gh_util-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:48.455872 gh_util-0.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:48.455872 gh_util-0.1.8/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:48.455872 gh_util-0.1.8/docs/assets/gifs/
--rw-r--r--   0 runner    (1001) docker     (127) 12080664 2024-03-26 02:09:41.000000 gh_util-0.1.8/docs/assets/gifs/gh-util-demo-read-issue.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:48.471872 gh_util-0.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/add_labels_to_issue.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/fetch_latest_release.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/hello_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:48.475872 gh_util-0.1.8/examples/on_event/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/on_event/Dockerfile.do
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/on_event/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/on_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/on_event/do.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/on_event/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/on_event/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/on_event/logging.yml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/on_event/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/on_event/resources.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/on_event/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/open_pull_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/read_issue.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/read_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-26 02:09:41.000000 gh_util-0.1.8/examples/read_repo_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-26 02:09:41.000000 gh_util-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 02:09:48.479872 gh_util-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:48.455872 gh_util-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:48.475872 gh_util-0.1.8/src/gh_util/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-26 02:09:41.000000 gh_util-0.1.8/src/gh_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-26 02:09:48.000000 gh_util-0.1.8/src/gh_util/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-26 02:09:41.000000 gh_util-0.1.8/src/gh_util/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-03-26 02:09:41.000000 gh_util-0.1.8/src/gh_util/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-26 02:09:41.000000 gh_util-0.1.8/src/gh_util/contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16503 2024-03-26 02:09:41.000000 gh_util-0.1.8/src/gh_util/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-03-26 02:09:41.000000 gh_util-0.1.8/src/gh_util/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-03-26 02:09:41.000000 gh_util-0.1.8/src/gh_util/print.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-26 02:09:41.000000 gh_util-0.1.8/src/gh_util/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-26 02:09:41.000000 gh_util-0.1.8/src/gh_util/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:48.475872 gh_util-0.1.8/src/gh_util/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:41.000000 gh_util-0.1.8/src/gh_util/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-26 02:09:41.000000 gh_util-0.1.8/src/gh_util/utilities/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-03-26 02:09:41.000000 gh_util-0.1.8/src/gh_util/utilities/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-26 02:09:41.000000 gh_util-0.1.8/src/gh_util/utilities/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:09:48.475872 gh_util-0.1.8/src/gh_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-03-26 02:09:48.000000 gh_util-0.1.8/src/gh_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-26 02:09:48.000000 gh_util-0.1.8/src/gh_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 02:09:48.000000 gh_util-0.1.8/src/gh_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-26 02:09:48.000000 gh_util-0.1.8/src/gh_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-26 02:09:48.000000 gh_util-0.1.8/src/gh_util.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:53.034646 gh_util-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:53.010646 gh_util-0.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-27 06:01:46.000000 gh_util-0.1.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:53.010646 gh_util-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-27 06:01:46.000000 gh_util-0.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-27 06:01:46.000000 gh_util-0.1.9/.github/workflows/static-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-03-27 06:01:46.000000 gh_util-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-27 06:01:46.000000 gh_util-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-03-27 06:01:53.034646 gh_util-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-03-27 06:01:46.000000 gh_util-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:53.010646 gh_util-0.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:53.010646 gh_util-0.1.9/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:53.010646 gh_util-0.1.9/docs/assets/gifs/
+-rw-r--r--   0 runner    (1001) docker     (127) 12080664 2024-03-27 06:01:46.000000 gh_util-0.1.9/docs/assets/gifs/gh-util-demo-read-issue.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:53.026646 gh_util-0.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/add_labels_to_issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/fetch_latest_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/hello_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:53.030646 gh_util-0.1.9/examples/on_event/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/on_event/Dockerfile.do
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/on_event/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/on_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/on_event/do.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/on_event/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/on_event/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/on_event/logging.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/on_event/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/on_event/resources.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/on_event/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/open_pull_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/read_issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/read_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-27 06:01:46.000000 gh_util-0.1.9/examples/read_repo_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-27 06:01:46.000000 gh_util-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 06:01:53.034646 gh_util-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:53.010646 gh_util-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:53.030646 gh_util-0.1.9/src/gh_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-27 06:01:52.000000 gh_util-0.1.9/src/gh_util/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16503 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:53.030646 gh_util-0.1.9/src/gh_util/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/types/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/types/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:53.030646 gh_util-0.1.9/src/gh_util/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/utilities/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/utilities/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-27 06:01:46.000000 gh_util-0.1.9/src/gh_util/utilities/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:01:53.030646 gh_util-0.1.9/src/gh_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-03-27 06:01:52.000000 gh_util-0.1.9/src/gh_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-27 06:01:53.000000 gh_util-0.1.9/src/gh_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 06:01:52.000000 gh_util-0.1.9/src/gh_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-27 06:01:52.000000 gh_util-0.1.9/src/gh_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-27 06:01:52.000000 gh_util-0.1.9/src/gh_util.egg-info/top_level.txt
```

### Comparing `gh_util-0.1.8/.github/dependabot.yml` & `gh_util-0.1.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/.gitignore` & `gh_util-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/PKG-INFO` & `gh_util-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh_util
-Version: 0.1.8
+Version: 0.1.9
 Summary: Minimal LLM friendly Python client for GitHub API.
 Project-URL: Code, https://github.com/zzstoatzz/gh
 Keywords: github,api,client,python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `gh_util-0.1.8/README.md` & `gh_util-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/docs/assets/gifs/gh-util-demo-read-issue.gif` & `gh_util-0.1.9/docs/assets/gifs/gh-util-demo-read-issue.gif`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/examples/on_event/Dockerfile.do` & `gh_util-0.1.9/examples/on_event/Dockerfile.do`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/examples/on_event/do.py` & `gh_util-0.1.9/examples/on_event/do.py`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/examples/on_event/handlers.py` & `gh_util-0.1.9/examples/on_event/handlers.py`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/examples/on_event/logging.yml` & `gh_util-0.1.9/examples/on_event/logging.yml`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/examples/on_event/resources.yml` & `gh_util-0.1.9/examples/on_event/resources.yml`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/examples/on_event/tasks.py` & `gh_util-0.1.9/examples/on_event/tasks.py`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/pyproject.toml` & `gh_util-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/src/gh_util/client.py` & `gh_util-0.1.9/src/gh_util/client.py`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/src/gh_util/contexts.py` & `gh_util-0.1.9/src/gh_util/contexts.py`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/src/gh_util/functions.py` & `gh_util-0.1.9/src/gh_util/functions.py`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/src/gh_util/logging.py` & `gh_util-0.1.9/src/gh_util/logging.py`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/src/gh_util/print.py` & `gh_util-0.1.9/src/gh_util/print.py`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/src/gh_util/settings.py` & `gh_util-0.1.9/src/gh_util/settings.py`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/src/gh_util/types.py` & `gh_util-0.1.9/src/gh_util/types/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from datetime import UTC, datetime
+from datetime import datetime
 
-from pydantic import BaseModel, ConfigDict, Field, HttpUrl, PrivateAttr
+from pydantic import BaseModel, ConfigDict, Field, HttpUrl
 
 
 class GitHubResourceModel(BaseModel):
     model_config = ConfigDict(extra="allow")
 
     created_at: datetime | None = None
     updated_at: datetime | None = None
@@ -113,39 +113,14 @@
     base: GitHubBranch
 
     # Timestamps
     closed_at: datetime | None = None
     merged_at: datetime | None = None
 
 
-class GitHubWebhookEventHeaders(BaseModel):
-    model_config = dict(extra="ignore")
-
-    host: str = Field(...)
-    event: str = Field(alias="x-github-event")
-    hook_id: int = Field(alias="x-github-hook-id")
-    delivery: str = Field(alias="x-github-delivery")
-
-
-class GitHubWebhookEvent(GitHubResourceModel):
-    action: str
-
-    repository: GitHubRepo | None = None
-    sender: GitHubUser | None = None
-
-
-class GitHubIssueEvent(GitHubWebhookEvent):
-    issue: GitHubIssue
-    comment: GitHubComment | None = None
-
-
-class GitHubPullRequestEvent(GitHubWebhookEvent):
-    pull_request: GitHubPullRequest
-
-
 class GitHubEventPayload(GitHubResourceModel):
     action: str | None = None
 
     commits: list[GitHubCommit] = Field(default_factory=list)
 
 
 class GitHubEvent(GitHubResourceModel):
@@ -153,14 +128,7 @@
     type: str
     actor: GitHubUser
     repo: GitHubRepo
     payload: GitHubEventPayload
     public: bool
     created_at: datetime
     org: GitHubOrg | None = None
-
-
-class GitHubWebhookRequest(BaseModel):
-    _received_at: datetime = PrivateAttr(default_factory=lambda: datetime.now(UTC))
-
-    headers: GitHubWebhookEventHeaders
-    event: GitHubWebhookEvent
```

### Comparing `gh_util-0.1.8/src/gh_util/utilities/process.py` & `gh_util-0.1.9/src/gh_util/utilities/process.py`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/src/gh_util/utilities/pydantic.py` & `gh_util-0.1.9/src/gh_util/utilities/pydantic.py`

 * *Files identical despite different names*

### Comparing `gh_util-0.1.8/src/gh_util.egg-info/PKG-INFO` & `gh_util-0.1.9/src/gh_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh_util
-Version: 0.1.8
+Version: 0.1.9
 Summary: Minimal LLM friendly Python client for GitHub API.
 Project-URL: Code, https://github.com/zzstoatzz/gh
 Keywords: github,api,client,python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `gh_util-0.1.8/src/gh_util.egg-info/SOURCES.txt` & `gh_util-0.1.9/src/gh_util.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -28,17 +28,19 @@
 src/gh_util/api.py
 src/gh_util/client.py
 src/gh_util/contexts.py
 src/gh_util/functions.py
 src/gh_util/logging.py
 src/gh_util/print.py
 src/gh_util/settings.py
-src/gh_util/types.py
 src/gh_util.egg-info/PKG-INFO
 src/gh_util.egg-info/SOURCES.txt
 src/gh_util.egg-info/dependency_links.txt
 src/gh_util.egg-info/requires.txt
 src/gh_util.egg-info/top_level.txt
+src/gh_util/types/__init__.py
+src/gh_util/types/core.py
+src/gh_util/types/webhooks.py
 src/gh_util/utilities/__init__.py
 src/gh_util/utilities/inspect.py
 src/gh_util/utilities/process.py
 src/gh_util/utilities/pydantic.py
```

