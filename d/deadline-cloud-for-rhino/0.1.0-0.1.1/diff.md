# Comparing `tmp/deadline_cloud_for_rhino-0.1.0.tar.gz` & `tmp/deadline_cloud_for_rhino-0.1.1.tar.gz`

## Comparing `deadline_cloud_for_rhino-0.1.0.tar` & `deadline_cloud_for_rhino-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/_version.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/src/deadline/rhino_submitter/__init__.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/src/deadline/rhino_submitter/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/src/deadline/rhino_submitter/_version.py
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/src/deadline/rhino_submitter/data_classes.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/src/deadline/rhino_submitter/default_rhino_job_template.yaml
--rw-r--r--   0        0        0     7573 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/src/deadline/rhino_submitter/rhino_render_submitter.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/src/deadline/rhino_submitter/ui/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/src/deadline/rhino_submitter/ui/components/__init__.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/src/deadline/rhino_submitter/ui/components/scene_settings_tab.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/.gitignore
--rw-r--r--   0        0        0    10317 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/LICENSE
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/NOTICE
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/README.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/hatch.toml
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/_version.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/src/deadline/rhino_submitter/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/src/deadline/rhino_submitter/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/src/deadline/rhino_submitter/_version.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/src/deadline/rhino_submitter/data_classes.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/src/deadline/rhino_submitter/default_rhino_job_template.yaml
+-rw-r--r--   0        0        0     7573 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/src/deadline/rhino_submitter/rhino_render_submitter.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/src/deadline/rhino_submitter/ui/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/src/deadline/rhino_submitter/ui/components/__init__.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/src/deadline/rhino_submitter/ui/components/scene_settings_tab.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/.gitignore
+-rw-r--r--   0        0        0    10317 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/LICENSE
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/NOTICE
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/hatch.toml
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.1/PKG-INFO
```

### Comparing `deadline_cloud_for_rhino-0.1.0/src/deadline/rhino_submitter/data_classes.py` & `deadline_cloud_for_rhino-0.1.1/src/deadline/rhino_submitter/data_classes.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.0/src/deadline/rhino_submitter/default_rhino_job_template.yaml` & `deadline_cloud_for_rhino-0.1.1/src/deadline/rhino_submitter/default_rhino_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.0/src/deadline/rhino_submitter/rhino_render_submitter.py` & `deadline_cloud_for_rhino-0.1.1/src/deadline/rhino_submitter/rhino_render_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.0/src/deadline/rhino_submitter/ui/components/scene_settings_tab.py` & `deadline_cloud_for_rhino-0.1.1/src/deadline/rhino_submitter/ui/components/scene_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.0/LICENSE` & `deadline_cloud_for_rhino-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.0/README.md` & `deadline_cloud_for_rhino-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.0/hatch.toml` & `deadline_cloud_for_rhino-0.1.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.0/pyproject.toml` & `deadline_cloud_for_rhino-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.0/PKG-INFO` & `deadline_cloud_for_rhino-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-rhino
-Version: 0.1.0
+Version: 0.1.1
 Summary: AWS Deadline Cloud for Rhino
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-rhino
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-rhino
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
```

