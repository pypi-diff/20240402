# Comparing `tmp/mozilla-taskgraph-1.3.1.tar.gz` & `tmp/mozilla-taskgraph-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-taskgraph-1.3.1.tar", last modified: Thu Mar 28 17:12:17 2024, max compression
+gzip compressed data, was "mozilla-taskgraph-1.3.2.tar", last modified: Tue Apr  2 13:55:03 2024, max compression
```

## Comparing `mozilla-taskgraph-1.3.1.tar` & `mozilla-taskgraph-1.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:12:17.791528 mozilla-taskgraph-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-28 17:12:17.791528 mozilla-taskgraph-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:12:17.791528 mozilla-taskgraph-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:12:17.787528 mozilla-taskgraph-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:12:17.787528 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:12:17.791528 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/actions/release_promotion.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:12:17.791528 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:12:17.791528 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/transforms/scriptworker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/transforms/scriptworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:12:17.791528 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/transforms/scriptworker/shipit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/transforms/scriptworker/shipit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/worker_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:12:17.791528 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-28 17:12:17.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-28 17:12:17.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:12:17.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-28 17:12:17.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-28 17:12:17.000000 mozilla-taskgraph-1.3.1/src/mozilla_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:12:17.791528 mozilla-taskgraph-1.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/test/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-03-28 17:12:14.000000 mozilla-taskgraph-1.3.1/test/test_worker_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.030306 mozilla-taskgraph-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/actions/release_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/shipit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/shipit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/worker_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-02 13:55:02.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-02 13:55:03.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:55:02.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 13:55:02.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 13:55:02.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/test/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/test/test_worker_types.py
```

### Comparing `mozilla-taskgraph-1.3.1/LICENSE` & `mozilla-taskgraph-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.1/PKG-INFO` & `mozilla-taskgraph-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-taskgraph
-Version: 1.3.1
+Version: 1.3.2
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mozilla-taskgraph-1.3.1/README.md` & `mozilla-taskgraph-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.1/pyproject.toml` & `mozilla-taskgraph-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.1/setup.py` & `mozilla-taskgraph-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/__init__.py` & `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/actions/__init__.py` & `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/actions/release_promotion.py` & `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/actions/release_promotion.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/config.py` & `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py` & `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py` & `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.1/src/mozilla_taskgraph/worker_types.py` & `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/worker_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,25 +83,40 @@
         [f"{scope_prefix}:bitrise:workflow:{wf}" for wf in bitrise["workflows"]]
     )
 
     # Set some build_params implicitly from Taskcluster params.
     build_params.setdefault("commit_hash", config.params["head_rev"])
     build_params.setdefault("branch_repo_owner", config.params["head_repository"])
 
-    if config.params["head_ref"]:
-        build_params.setdefault("branch", config.params["head_ref"])
+    def normref(ref, type="heads"):
+        if ref:
+            prefix = f"refs/{type}/"
+            if ref.startswith(prefix):
+                return ref[len(prefix) :]
+            # The ref is a different type than the requested one, return None
+            # to indicate this.
+            elif ref.startswith("refs/"):
+                return None
+        return ref
+
+    head_ref = normref(config.params["head_ref"])
+    head_tag = normref(config.params["head_tag"], type="tags")
+    base_ref = normref(config.params["base_ref"])
 
-    if config.params["head_tag"]:
-        build_params.setdefault("tag", config.params["head_tag"])
+    if head_ref:
+        build_params.setdefault("branch", head_ref)
+
+    if head_tag:
+        build_params.setdefault("tag", head_tag)
 
     if config.params["tasks_for"] == "github-pull-request":
         build_params.setdefault("pull_request_author", config.params["owner"])
 
-        if config.params["base_ref"]:
-            build_params.setdefault("branch_dest", config.params["base_ref"])
+        if base_ref:
+            build_params.setdefault("branch_dest", base_ref)
 
         if config.params["base_repository"]:
             build_params.setdefault(
                 "branch_dest_repo_owner", config.params["base_repository"]
             )
 
     task_def["payload"] = {"build_params": build_params}
```

### Comparing `mozilla-taskgraph-1.3.1/src/mozilla_taskgraph.egg-info/PKG-INFO` & `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-taskgraph
-Version: 1.3.1
+Version: 1.3.2
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mozilla-taskgraph-1.3.1/src/mozilla_taskgraph.egg-info/SOURCES.txt` & `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.1/test/test_register.py` & `mozilla-taskgraph-1.3.2/test/test_register.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.1/test/test_worker_types.py` & `mozilla-taskgraph-1.3.2/test/test_worker_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -74,14 +74,61 @@
                     }
                 },
                 "scopes": ["foo:bitrise:app:some-app", "foo:bitrise:workflow:bar"],
                 "tags": {"worker-implementation": "scriptworker"},
             },
             id="opposite params",  # this test helps hit other half of if statements
         ),
+        pytest.param(
+            {"bitrise": {"app": "some-app", "workflows": ["bar"]}},
+            {
+                "base_ref": "refs/heads/foo",
+                "base_repository": "",
+                "head_ref": "refs/heads/bar",
+                "head_tag": "refs/tags/some-tag",
+                "tasks_for": "github-pull-request",
+            },
+            {
+                "payload": {
+                    "build_params": {
+                        "branch": "bar",
+                        "branch_dest": "foo",
+                        "branch_repo_owner": "http://example.com/head/repo",
+                        "commit_hash": "abcdef",
+                        "pull_request_author": "some-owner",
+                        "tag": "some-tag",
+                    }
+                },
+                "scopes": ["foo:bitrise:app:some-app", "foo:bitrise:workflow:bar"],
+                "tags": {"worker-implementation": "scriptworker"},
+            },
+            id="normalize refs",
+        ),
+        pytest.param(
+            {"bitrise": {"app": "some-app", "workflows": ["bar"]}},
+            {
+                "base_ref": "refs/tags/foo",
+                "base_repository": "",
+                "head_ref": "refs/tags/bar",
+                "head_tag": "refs/heads/some-tag",
+                "tasks_for": "github-pull-request",
+            },
+            {
+                "payload": {
+                    "build_params": {
+                        "branch_repo_owner": "http://example.com/head/repo",
+                        "commit_hash": "abcdef",
+                        "pull_request_author": "some-owner",
+                    }
+                },
+                "scopes": ["foo:bitrise:app:some-app", "foo:bitrise:workflow:bar"],
+                "tags": {"worker-implementation": "scriptworker"},
+            },
+            id="normalize refs wrong type",
+        ),
     ),
 )
 def test_build_bitrise_payload(
     make_graph_config, make_transform_config, parameters, worker, extra_params, expected
 ):
     schema = payload_builders["scriptworker-bitrise"].schema
```

