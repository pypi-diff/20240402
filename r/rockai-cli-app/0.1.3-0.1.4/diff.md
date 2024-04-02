# Comparing `tmp/rockai_cli_app-0.1.3.tar.gz` & `tmp/rockai_cli_app-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockai_cli_app-0.1.3.tar", max compression
+gzip compressed data, was "rockai_cli_app-0.1.4.tar", max compression
```

## Comparing `rockai_cli_app-0.1.3.tar` & `rockai_cli_app-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       72 2024-03-05 09:01:49.763544 rockai_cli_app-0.1.3/README.md
--rw-r--r--   0        0        0      619 2024-03-29 04:08:55.542689 rockai_cli_app-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-07 03:29:24.441443 rockai_cli_app-0.1.3/rockai_cli_app/__init__.py
--rw-r--r--   0        0        0     2310 2024-02-28 07:00:47.957586 rockai_cli_app-0.1.3/rockai_cli_app/data_class.py
--rw-r--r--   0        0        0        0 2024-03-01 08:25:13.083771 rockai_cli_app-0.1.3/rockai_cli_app/docker/__init__.py
--rw-r--r--   0        0        0    11551 2024-03-29 04:08:32.447830 rockai_cli_app-0.1.3/rockai_cli_app/docker/docker_util.py
--rw-r--r--   0        0        0     2819 2024-03-01 08:15:55.566855 rockai_cli_app-0.1.3/rockai_cli_app/docker/tf_compat.json
--rw-r--r--   0        0        0      604 2024-03-26 06:45:43.007156 rockai_cli_app-0.1.3/rockai_cli_app/docker/torch_compat.json
--rw-r--r--   0        0        0     1406 2024-03-08 06:28:07.738273 rockai_cli_app-0.1.3/rockai_cli_app/main.py
--rw-r--r--   0        0        0        0 2024-02-28 08:04:20.239254 rockai_cli_app-0.1.3/rockai_cli_app/parser/__init__.py
--rw-r--r--   0        0        0      799 2024-02-28 09:29:39.709568 rockai_cli_app-0.1.3/rockai_cli_app/parser/config_util.py
--rw-r--r--   0        0        0      290 2024-02-07 03:35:01.202042 rockai_cli_app-0.1.3/rockai_cli_app/predictor.py
--rw-r--r--   0        0        0        0 2024-02-07 03:35:44.528854 rockai_cli_app-0.1.3/rockai_cli_app/server/__init__.py
--rw-r--r--   0        0        0     2477 2024-03-08 08:01:30.731983 rockai_cli_app-0.1.3/rockai_cli_app/server/http.py
--rw-r--r--   0        0        0       77 2024-02-07 06:52:07.739336 rockai_cli_app-0.1.3/rockai_cli_app/server/runner.py
--rw-r--r--   0        0        0        0 2024-02-20 09:20:10.188788 rockai_cli_app-0.1.3/rockai_cli_app/server/test/__init__.py
--rw-r--r--   0        0        0      783 2024-02-28 07:05:00.986936 rockai_cli_app-0.1.3/rockai_cli_app/server/test/predict.py
--rw-r--r--   0        0        0      149 2024-02-20 06:38:03.569237 rockai_cli_app-0.1.3/rockai_cli_app/server/test/test_config.yaml
--rw-r--r--   0        0        0     8582 2024-02-23 06:25:29.351387 rockai_cli_app-0.1.3/rockai_cli_app/server/types.py
--rw-r--r--   0        0        0     8639 2024-02-28 09:23:42.650045 rockai_cli_app-0.1.3/rockai_cli_app/server/utils.py
--rw-r--r--   0        0        0        0 2024-02-07 05:25:34.434644 rockai_cli_app-0.1.3/rockai_cli_app/server/worker.py
--rw-r--r--   0        0        0      703 2024-02-22 08:32:41.013574 rockai_cli_app-0.1.3/rockai_cli_app/test.py
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 rockai_cli_app-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       72 2024-03-05 09:01:49.763544 rockai_cli_app-0.1.4/README.md
+-rw-r--r--   0        0        0      619 2024-04-02 07:17:18.525280 rockai_cli_app-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-07 03:29:24.441443 rockai_cli_app-0.1.4/rockai_cli_app/__init__.py
+-rw-r--r--   0        0        0     2310 2024-02-28 07:00:47.957586 rockai_cli_app-0.1.4/rockai_cli_app/data_class.py
+-rw-r--r--   0        0        0        0 2024-03-01 08:25:13.083771 rockai_cli_app-0.1.4/rockai_cli_app/docker/__init__.py
+-rw-r--r--   0        0        0    11633 2024-04-02 07:17:07.254895 rockai_cli_app-0.1.4/rockai_cli_app/docker/docker_util.py
+-rw-r--r--   0        0        0     2819 2024-03-01 08:15:55.566855 rockai_cli_app-0.1.4/rockai_cli_app/docker/tf_compat.json
+-rw-r--r--   0        0        0      604 2024-03-26 06:45:43.007156 rockai_cli_app-0.1.4/rockai_cli_app/docker/torch_compat.json
+-rw-r--r--   0        0        0     1406 2024-03-08 06:28:07.738273 rockai_cli_app-0.1.4/rockai_cli_app/main.py
+-rw-r--r--   0        0        0        0 2024-02-28 08:04:20.239254 rockai_cli_app-0.1.4/rockai_cli_app/parser/__init__.py
+-rw-r--r--   0        0        0      799 2024-02-28 09:29:39.709568 rockai_cli_app-0.1.4/rockai_cli_app/parser/config_util.py
+-rw-r--r--   0        0        0      290 2024-02-07 03:35:01.202042 rockai_cli_app-0.1.4/rockai_cli_app/predictor.py
+-rw-r--r--   0        0        0        0 2024-02-07 03:35:44.528854 rockai_cli_app-0.1.4/rockai_cli_app/server/__init__.py
+-rw-r--r--   0        0        0     2477 2024-03-08 08:01:30.731983 rockai_cli_app-0.1.4/rockai_cli_app/server/http.py
+-rw-r--r--   0        0        0       77 2024-02-07 06:52:07.739336 rockai_cli_app-0.1.4/rockai_cli_app/server/runner.py
+-rw-r--r--   0        0        0        0 2024-02-20 09:20:10.188788 rockai_cli_app-0.1.4/rockai_cli_app/server/test/__init__.py
+-rw-r--r--   0        0        0      783 2024-02-28 07:05:00.986936 rockai_cli_app-0.1.4/rockai_cli_app/server/test/predict.py
+-rw-r--r--   0        0        0      149 2024-02-20 06:38:03.569237 rockai_cli_app-0.1.4/rockai_cli_app/server/test/test_config.yaml
+-rw-r--r--   0        0        0     8582 2024-02-23 06:25:29.351387 rockai_cli_app-0.1.4/rockai_cli_app/server/types.py
+-rw-r--r--   0        0        0     8639 2024-02-28 09:23:42.650045 rockai_cli_app-0.1.4/rockai_cli_app/server/utils.py
+-rw-r--r--   0        0        0        0 2024-02-07 05:25:34.434644 rockai_cli_app-0.1.4/rockai_cli_app/server/worker.py
+-rw-r--r--   0        0        0      703 2024-02-22 08:32:41.013574 rockai_cli_app-0.1.4/rockai_cli_app/test.py
+-rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 rockai_cli_app-0.1.4/PKG-INFO
```

### Comparing `rockai_cli_app-0.1.3/pyproject.toml` & `rockai_cli_app-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rockai-cli-app"
-version = "0.1.3"
+version = "0.1.4"
 description = "for inference and training"
 authors = ["Rocky <some_developer@example.com>"]
 readme = "README.md"
 include = ["./rockai_cli_app/docker/tf_compat.json","./rockai_cli_app/docker/torch_compat.json"]
 
 [tool.poetry.scripts]
 rock = "rockai_cli_app.main:app"
```

### Comparing `rockai_cli_app-0.1.3/rockai_cli_app/data_class.py` & `rockai_cli_app-0.1.4/rockai_cli_app/data_class.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.3/rockai_cli_app/docker/docker_util.py` & `rockai_cli_app-0.1.4/rockai_cli_app/docker/docker_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,18 @@
                 config_map["build"]["python_version"],
             )
         )
     )
     docker_list.append(add_expose(5000))
     if config_map['build']['python_requirements']:
         remove_some_libs(config_map['build']['python_requirements'],'tensorflow-metal')
+        remove_some_libs(config_map['build']['python_requirements'],'tensorflow-macos')
         docker_list.append(add_run("pip install -r {}".format(config_map['build']['python_requirements'])))
 
-    docker_list.append(add_cmd("python --version"))
+    docker_list.append(add_cmd("rock start"))
     save_docker_file(docker_list)
     subprocess.run(["docker", "build", "--platform", platform,"-t", tag, "."])
     subprocess.run(["docker", "run", "--rm", tag])
         
 
 
 def tf_compat_matrix():
```

### Comparing `rockai_cli_app-0.1.3/rockai_cli_app/docker/tf_compat.json` & `rockai_cli_app-0.1.4/rockai_cli_app/docker/tf_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.3/rockai_cli_app/docker/torch_compat.json` & `rockai_cli_app-0.1.4/rockai_cli_app/docker/torch_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.3/rockai_cli_app/main.py` & `rockai_cli_app-0.1.4/rockai_cli_app/main.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.3/rockai_cli_app/parser/config_util.py` & `rockai_cli_app-0.1.4/rockai_cli_app/parser/config_util.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.3/rockai_cli_app/server/http.py` & `rockai_cli_app-0.1.4/rockai_cli_app/server/http.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.3/rockai_cli_app/server/test/predict.py` & `rockai_cli_app-0.1.4/rockai_cli_app/server/test/predict.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.3/rockai_cli_app/server/types.py` & `rockai_cli_app-0.1.4/rockai_cli_app/server/types.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.3/rockai_cli_app/server/utils.py` & `rockai_cli_app-0.1.4/rockai_cli_app/server/utils.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.3/rockai_cli_app/test.py` & `rockai_cli_app-0.1.4/rockai_cli_app/test.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.3/PKG-INFO` & `rockai_cli_app-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockai-cli-app
-Version: 0.1.3
+Version: 0.1.4
 Summary: for inference and training
 Author: Rocky
 Author-email: some_developer@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

