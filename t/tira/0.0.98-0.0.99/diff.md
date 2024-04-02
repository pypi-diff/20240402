# Comparing `tmp/tira-0.0.98.tar.gz` & `tmp/tira-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tira-0.0.98.tar", last modified: Sun Nov 26 11:44:10 2023, max compression
+gzip compressed data, was "tira-0.0.99.tar", last modified: Sun Nov 26 12:16:40 2023, max compression
```

## Comparing `tira-0.0.98.tar` & `tira-0.0.99.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-11-26 11:44:10.033652 tira-0.0.98/
--rw-r--r--   0 maik      (1000) maik      (1000)     4361 2023-11-26 11:44:10.033652 tira-0.0.98/PKG-INFO
--rw-r--r--   0 maik      (1000) maik      (1000)     3352 2023-11-07 11:47:23.000000 tira-0.0.98/README.md
--rw-r--r--   0 maik      (1000) maik      (1000)       30 2023-11-23 14:25:39.000000 tira-0.0.98/pyproject.toml
--rw-r--r--   0 maik      (1000) maik      (1000)     1294 2023-11-26 11:44:10.033652 tira-0.0.98/setup.cfg
--rw-r--r--   0 maik      (1000) maik      (1000)       39 2023-08-04 11:15:41.000000 tira-0.0.98/setup.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-11-26 11:44:10.030319 tira-0.0.98/tests/
--rw-r--r--   0 maik      (1000) maik      (1000)        1 2023-08-04 11:15:41.000000 tira-0.0.98/tests/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1105 2023-11-23 14:50:40.000000 tira-0.0.98/tests/docker_integration_test.py
--rw-r--r--   0 maik      (1000) maik      (1000)      940 2023-09-18 06:54:16.000000 tira-0.0.98/tests/export_submission_from_jupyter_notebook_test.py
--rw-r--r--   0 maik      (1000) maik      (1000)    21840 2023-11-26 11:35:01.000000 tira-0.0.98/tests/ir_datasets_test.py
--rw-r--r--   0 maik      (1000) maik      (1000)     3500 2023-11-13 14:07:30.000000 tira-0.0.98/tests/irds_id_translation_test.py
--rw-r--r--   0 maik      (1000) maik      (1000)      974 2023-11-20 10:02:11.000000 tira-0.0.98/tests/load_rerank_data_test.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1566 2023-09-17 11:16:22.000000 tira-0.0.98/tests/pt_document_processing_loader_test.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1544 2023-09-13 08:11:51.000000 tira-0.0.98/tests/pt_from_retriever_for_re_ranking_submission_loader_test.py
--rw-r--r--   0 maik      (1000) maik      (1000)     2165 2023-11-10 21:40:14.000000 tira-0.0.98/tests/pt_from_retriever_submission_loader_test.py
--rw-r--r--   0 maik      (1000) maik      (1000)     3878 2023-11-23 07:35:51.000000 tira-0.0.98/tests/pt_query_processing_loader_test.py
--rw-r--r--   0 maik      (1000) maik      (1000)      863 2023-11-07 15:14:46.000000 tira-0.0.98/tests/rest_api_test.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1600 2023-11-26 11:11:28.000000 tira-0.0.98/tests/test_export_submission_environment.py
--rw-r--r--   0 maik      (1000) maik      (1000)      864 2023-11-20 19:14:48.000000 tira-0.0.98/tests/test_persisting_run_files.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-11-26 11:44:10.033652 tira-0.0.98/tira/
--rw-r--r--   0 maik      (1000) maik      (1000)       23 2023-11-26 11:40:39.000000 tira-0.0.98/tira/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)     6760 2023-11-22 16:16:16.000000 tira-0.0.98/tira/inference_server.py
--rw-r--r--   0 maik      (1000) maik      (1000)     6192 2023-11-26 11:35:01.000000 tira-0.0.98/tira/io_utils.py
--rw-r--r--   0 maik      (1000) maik      (1000)     9564 2023-11-23 14:25:39.000000 tira-0.0.98/tira/ir_datasets_util.py
--rw-r--r--   0 maik      (1000) maik      (1000)    11371 2023-11-23 14:25:39.000000 tira-0.0.98/tira/local_client.py
--rw-r--r--   0 maik      (1000) maik      (1000)    13321 2023-11-23 14:25:39.000000 tira-0.0.98/tira/local_execution_integration.py
--rw-r--r--   0 maik      (1000) maik      (1000)     2847 2023-11-23 07:56:10.000000 tira-0.0.98/tira/pandas_integration.py
--rw-r--r--   0 maik      (1000) maik      (1000)     5771 2023-11-23 07:36:01.000000 tira-0.0.98/tira/pyterrier_integration.py
--rw-r--r--   0 maik      (1000) maik      (1000)     5206 2023-11-22 16:16:16.000000 tira-0.0.98/tira/pyterrier_util.py
--rw-r--r--   0 maik      (1000) maik      (1000)    19736 2023-11-26 11:35:01.000000 tira-0.0.98/tira/rest_api_client.py
--rw-r--r--   0 maik      (1000) maik      (1000)     7403 2023-11-22 16:16:16.000000 tira-0.0.98/tira/third_party_integrations.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1853 2023-11-26 11:35:01.000000 tira-0.0.98/tira/tira_client.py
--rwxr-xr-x   0 maik      (1000) maik      (1000)     9588 2023-11-26 11:35:01.000000 tira-0.0.98/tira/tira_run.py
--rwxr-xr-x   0 maik      (1000) maik      (1000)     2458 2023-11-22 16:16:16.000000 tira-0.0.98/tira/tira_run_inference_server.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1040 2023-08-04 11:15:41.000000 tira-0.0.98/tira/tira_run_notebook.py
--rw-r--r--   0 maik      (1000) maik      (1000)     2416 2023-11-22 16:16:16.000000 tira-0.0.98/tira/tirex.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-11-26 11:44:10.033652 tira-0.0.98/tira.egg-info/
--rw-r--r--   0 maik      (1000) maik      (1000)     4361 2023-11-26 11:44:10.000000 tira-0.0.98/tira.egg-info/PKG-INFO
--rw-r--r--   0 maik      (1000) maik      (1000)     1100 2023-11-26 11:44:10.000000 tira-0.0.98/tira.egg-info/SOURCES.txt
--rw-r--r--   0 maik      (1000) maik      (1000)        1 2023-11-26 11:44:10.000000 tira-0.0.98/tira.egg-info/dependency_links.txt
--rw-r--r--   0 maik      (1000) maik      (1000)      160 2023-11-26 11:44:10.000000 tira-0.0.98/tira.egg-info/entry_points.txt
--rw-r--r--   0 maik      (1000) maik      (1000)       96 2023-11-26 11:44:10.000000 tira-0.0.98/tira.egg-info/requires.txt
--rw-r--r--   0 maik      (1000) maik      (1000)       11 2023-11-26 11:44:10.000000 tira-0.0.98/tira.egg-info/top_level.txt
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-11-26 12:16:40.929364 tira-0.0.99/
+-rw-r--r--   0 maik      (1000) maik      (1000)     4361 2023-11-26 12:16:40.929364 tira-0.0.99/PKG-INFO
+-rw-r--r--   0 maik      (1000) maik      (1000)     3352 2023-11-07 11:47:23.000000 tira-0.0.99/README.md
+-rw-r--r--   0 maik      (1000) maik      (1000)       30 2023-11-23 14:25:39.000000 tira-0.0.99/pyproject.toml
+-rw-r--r--   0 maik      (1000) maik      (1000)     1294 2023-11-26 12:16:40.929364 tira-0.0.99/setup.cfg
+-rw-r--r--   0 maik      (1000) maik      (1000)       39 2023-08-04 11:15:41.000000 tira-0.0.99/setup.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-11-26 12:16:40.926030 tira-0.0.99/tests/
+-rw-r--r--   0 maik      (1000) maik      (1000)        1 2023-08-04 11:15:41.000000 tira-0.0.99/tests/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1330 2023-11-26 12:05:30.000000 tira-0.0.99/tests/docker_integration_test.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1133 2023-11-26 12:05:30.000000 tira-0.0.99/tests/export_submission_from_jupyter_notebook_test.py
+-rw-r--r--   0 maik      (1000) maik      (1000)    21840 2023-11-26 11:35:01.000000 tira-0.0.99/tests/ir_datasets_test.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     3949 2023-11-26 12:05:30.000000 tira-0.0.99/tests/irds_id_translation_test.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1135 2023-11-26 12:05:30.000000 tira-0.0.99/tests/load_rerank_data_test.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1839 2023-11-26 12:05:30.000000 tira-0.0.99/tests/pt_document_processing_loader_test.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1871 2023-11-26 12:05:30.000000 tira-0.0.99/tests/pt_from_retriever_for_re_ranking_submission_loader_test.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     2537 2023-11-26 12:05:30.000000 tira-0.0.99/tests/pt_from_retriever_submission_loader_test.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     4322 2023-11-26 12:05:30.000000 tira-0.0.99/tests/pt_query_processing_loader_test.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1207 2023-11-26 12:05:30.000000 tira-0.0.99/tests/rest_api_test.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1600 2023-11-26 11:11:28.000000 tira-0.0.99/tests/test_export_submission_environment.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1031 2023-11-26 12:05:30.000000 tira-0.0.99/tests/test_persisting_run_files.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-11-26 12:16:40.926030 tira-0.0.99/tira/
+-rw-r--r--   0 maik      (1000) maik      (1000)       23 2023-11-26 12:11:56.000000 tira-0.0.99/tira/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     6760 2023-11-22 16:16:16.000000 tira-0.0.99/tira/inference_server.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     7172 2023-11-26 12:11:56.000000 tira-0.0.99/tira/io_utils.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     9564 2023-11-23 14:25:39.000000 tira-0.0.99/tira/ir_datasets_util.py
+-rw-r--r--   0 maik      (1000) maik      (1000)    11371 2023-11-23 14:25:39.000000 tira-0.0.99/tira/local_client.py
+-rw-r--r--   0 maik      (1000) maik      (1000)    13366 2023-11-26 12:05:30.000000 tira-0.0.99/tira/local_execution_integration.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     2847 2023-11-23 07:56:10.000000 tira-0.0.99/tira/pandas_integration.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     5771 2023-11-23 07:36:01.000000 tira-0.0.99/tira/pyterrier_integration.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     5206 2023-11-22 16:16:16.000000 tira-0.0.99/tira/pyterrier_util.py
+-rw-r--r--   0 maik      (1000) maik      (1000)    19736 2023-11-26 11:35:01.000000 tira-0.0.99/tira/rest_api_client.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     7403 2023-11-22 16:16:16.000000 tira-0.0.99/tira/third_party_integrations.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1866 2023-11-26 12:05:30.000000 tira-0.0.99/tira/tira_client.py
+-rwxr-xr-x   0 maik      (1000) maik      (1000)     9588 2023-11-26 11:35:01.000000 tira-0.0.99/tira/tira_run.py
+-rwxr-xr-x   0 maik      (1000) maik      (1000)     2458 2023-11-22 16:16:16.000000 tira-0.0.99/tira/tira_run_inference_server.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1040 2023-08-04 11:15:41.000000 tira-0.0.99/tira/tira_run_notebook.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     2416 2023-11-22 16:16:16.000000 tira-0.0.99/tira/tirex.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-11-26 12:16:40.929364 tira-0.0.99/tira.egg-info/
+-rw-r--r--   0 maik      (1000) maik      (1000)     4361 2023-11-26 12:16:40.000000 tira-0.0.99/tira.egg-info/PKG-INFO
+-rw-r--r--   0 maik      (1000) maik      (1000)     1100 2023-11-26 12:16:40.000000 tira-0.0.99/tira.egg-info/SOURCES.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)        1 2023-11-26 12:16:40.000000 tira-0.0.99/tira.egg-info/dependency_links.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)      160 2023-11-26 12:16:40.000000 tira-0.0.99/tira.egg-info/entry_points.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)       96 2023-11-26 12:16:40.000000 tira-0.0.99/tira.egg-info/requires.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)       11 2023-11-26 12:16:40.000000 tira-0.0.99/tira.egg-info/top_level.txt
```

### Comparing `tira-0.0.98/PKG-INFO` & `tira-0.0.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tira
-Version: 0.0.98
+Version: 0.0.99
 Summary: Simple access to the TIRA API.
 Home-page: https://github.com/tira-io/tira
 Author: Maik Fröbe
 Author-email: maik.froebe@uni-weimar.de
 Maintainer: Maik Fröbe
 Project-URL: Bug Tracker, https://github.com/tira-io/tira/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tira-0.0.98/README.md` & `tira-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/setup.cfg` & `tira-0.0.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tests/docker_integration_test.py` & `tira-0.0.99/tests/docker_integration_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from tira.local_execution_integration import LocalExecutionIntegration as Client
 import tempfile
+import unittest
 
-def test_export_of_file_from_bash_image():
-    tira = Client()
-    local_file = tempfile.NamedTemporaryFile().name
-    tira.export_file_from_software('/etc/issue', local_file, image='bash:alpine3.16')
-    
-    actual = open(local_file).read()
-    expected = '''Welcome to Alpine Linux 3.16
+# .. todo:: there are no assertions in this file
+
+class TestDockerIntegration(unittest.TestCase):
+    def test_export_of_file_from_bash_image(self):
+        tira = Client()
+        local_file = tempfile.NamedTemporaryFile().name
+        tira.export_file_from_software('/etc/issue', local_file, image='bash:alpine3.16')
+        
+        actual = open(local_file).read()
+        expected = '''Welcome to Alpine Linux 3.16
 Kernel \\r on an \\m (\\l)
 
 '''
-    assert actual == expected
-
-def test_export_of_file():
-    tira = Client()
-    local_file = tempfile.NamedTemporaryFile().name
-    tira.export_file_from_software('/etc/alpine-release', local_file, image='bash:alpine3.16')
-    
-    actual = open(local_file).read()
-    expected = '''3.16.5\n'''
-    assert actual == expected
-
-def test_extraction_of_entrypoint():
-    expected = 'docker-entrypoint.sh'
-
-    tira = Client()
-    actual = tira.extract_entrypoint(image='bash:alpine3.16')
-
-    assert actual == expected
-
-#def test_execution_of_software():
-#    tira = Client()
-#    tira.run(image='bash:alpine3.16', command='sleep 2s;', input_dir="/tmp/input", output_dir="/tmp/output")
+        assert actual == expected
 
+    def test_export_of_file(self):
+        tira = Client()
+        local_file = tempfile.NamedTemporaryFile().name
+        tira.export_file_from_software('/etc/alpine-release', local_file, image='bash:alpine3.16')
+        
+        actual = open(local_file).read()
+        expected = '''3.16.5\n'''
+        assert actual == expected
+
+    def test_extraction_of_entrypoint(self):
+        expected = 'docker-entrypoint.sh'
+
+        tira = Client()
+        actual = tira.extract_entrypoint(image='bash:alpine3.16')
+
+        assert actual == expected
+
+    #def test_execution_of_software(self):
+    #    tira = Client()
+    #    tira.run(image='bash:alpine3.16', command='sleep 2s;', input_dir="/tmp/input", output_dir="/tmp/output")
```

### Comparing `tira-0.0.98/tests/export_submission_from_jupyter_notebook_test.py` & `tira-0.0.99/tests/export_submission_from_jupyter_notebook_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from tira.local_execution_integration import LocalExecutionIntegration
+import unittest
 
+# .. todo:: there are no assertions in this file
 
-def test_non_existing_notebook_1():
-    notebook = 'does-not-exist'
+class TestExporSubmissionFromJupyterNotebook(unittest.TestCase):
+    def test_non_existing_notebook_1(self):
+        notebook = 'does-not-exist'
 
-    actual = LocalExecutionIntegration().export_submission_from_jupyter_notebook(notebook)
+        actual = LocalExecutionIntegration().export_submission_from_jupyter_notebook(notebook)
 
-    assert actual is None
+        assert actual is None
 
 
-def test_non_existing_notebook_2():
-    notebook = 'does-not-exist/1/does-not-exist.ipynb'
+    def test_non_existing_notebook_2(self):
+        notebook = 'does-not-exist/1/does-not-exist.ipynb'
 
-    actual = LocalExecutionIntegration().export_submission_from_jupyter_notebook(notebook)
+        actual = LocalExecutionIntegration().export_submission_from_jupyter_notebook(notebook)
 
-    assert actual is None
+        assert actual is None
 
 
-def test_notebook_submission_without_previous_stages():
-    notebook = 'tests/resources/pyterrier-notebook-without-previous-stages.ipynb'
+    def test_notebook_submission_without_previous_stages(self):
+        notebook = 'tests/resources/pyterrier-notebook-without-previous-stages.ipynb'
 
-    expected = 'TIRA_COMMAND=/workspace/run-pyterrier-notebook.py --input ${TIRA_INPUT_DIRECTORY} --output ${TIRA_OUTPUT_DIRECTORY} --notebook /workspace/pyterrier-notebook-without-previous-stages.ipynb'
-    actual = LocalExecutionIntegration().export_submission_from_jupyter_notebook(notebook)
-
-    assert expected == actual
+        expected = 'TIRA_COMMAND=/workspace/run-pyterrier-notebook.py --input ${TIRA_INPUT_DIRECTORY} --output ${TIRA_OUTPUT_DIRECTORY} --notebook /workspace/pyterrier-notebook-without-previous-stages.ipynb'
+        actual = LocalExecutionIntegration().export_submission_from_jupyter_notebook(notebook)
 
+        assert expected == actual
```

### Comparing `tira-0.0.98/tests/ir_datasets_test.py` & `tira-0.0.99/tests/ir_datasets_test.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tests/irds_id_translation_test.py` & `tira-0.0.99/tests/irds_id_translation_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,91 @@
 from tira.ir_datasets_util import translate_irds_id_to_tirex
 from tira.third_party_integrations import ensure_pyterrier_is_loaded
 import pyterrier as pt
+import unittest
 
+# .. todo:: there are no assertions in this file
 
-def test_for_tirex_id_robust04_01():
-    ensure_pyterrier_is_loaded(patch_ir_datasets=False)
-    expected = 'disks45-nocr-trec-robust-2004-20230209-training'
-    actual = translate_irds_id_to_tirex( 'disks45-nocr-trec-robust-2004-20230209-training')
-    
-    assert expected == actual
-
-def test_for_tirex_id_robust04_02():
-    ensure_pyterrier_is_loaded(patch_ir_datasets=True)
-    expected = 'disks45-nocr-trec-robust-2004-20230209-training'
-    actual = translate_irds_id_to_tirex( 'disks45-nocr-trec-robust-2004-20230209-training')
-    
-    assert expected == actual
-
-def test_for_tirex_id_cw09_2014_01():
-    ensure_pyterrier_is_loaded(patch_ir_datasets=False)
-    expected = 'clueweb12-trec-web-2014-20230107-training'
-    actual = translate_irds_id_to_tirex('clueweb12-trec-web-2014-20230107-training')
-    
-    assert expected == actual
-
-def test_for_tirex_id_cw09_2014_02():
-    ensure_pyterrier_is_loaded(patch_ir_datasets=True)
-    expected = 'clueweb12-trec-web-2014-20230107-training'
-    actual = translate_irds_id_to_tirex('clueweb12-trec-web-2014-20230107-training')
-    
-    assert expected == actual
-
-def test_for_raw_string_robust04_01():
-    ensure_pyterrier_is_loaded(patch_ir_datasets=False)
-    expected = 'disks45-nocr-trec-robust-2004-20230209-training'
-    actual = translate_irds_id_to_tirex('disks45/nocr/trec-robust-2004')
-    
-    assert expected == actual
-
-def test_for_raw_string_robust04_02():
-    ensure_pyterrier_is_loaded(patch_ir_datasets=True)
-    expected = 'disks45-nocr-trec-robust-2004-20230209-training'
-    actual = translate_irds_id_to_tirex('disks45/nocr/trec-robust-2004')
-    
-    assert expected == actual
-
-def test_for_raw_string_cw09_2014_01():
-    ensure_pyterrier_is_loaded(patch_ir_datasets=False)
-    expected = 'clueweb12-trec-web-2014-20230107-training'
-    actual = translate_irds_id_to_tirex('clueweb12/trec-web-2014')
-    
-    assert expected == actual
-
-def test_for_raw_string_cw09_2014_02():
-    ensure_pyterrier_is_loaded(patch_ir_datasets=True)
-    expected = 'clueweb12-trec-web-2014-20230107-training'
-    actual = translate_irds_id_to_tirex('clueweb12/trec-web-2014')
-    
-    assert expected == actual
-
-def test_for_pyterrier_dataset_robust04_01():
-    ensure_pyterrier_is_loaded(patch_ir_datasets=False)
-    expected = 'disks45-nocr-trec-robust-2004-20230209-training'
-    actual = translate_irds_id_to_tirex(pt.get_dataset("irds:disks45/nocr/trec-robust-2004"))
-    
-    assert expected == actual
-
-def test_for_pyterrier_dataset_robust04_02():
-    ensure_pyterrier_is_loaded(patch_ir_datasets=True)
-    expected = 'disks45-nocr-trec-robust-2004-20230209-training'
-    actual = translate_irds_id_to_tirex(pt.get_dataset("irds:disks45/nocr/trec-robust-2004"))
-    
-    assert expected == actual
-
-def test_for_pyterrier_dataset_cw09_2009_01():
-    ensure_pyterrier_is_loaded(patch_ir_datasets=False)
-    expected = 'clueweb09-en-trec-web-2009-20230107-training'
-    actual = translate_irds_id_to_tirex(pt.get_dataset("irds:clueweb09/en/trec-web-2009"))
-    
-    assert expected == actual
-
-def test_for_pyterrier_dataset_cw09_2009_02():
-    ensure_pyterrier_is_loaded(patch_ir_datasets=True)
-    expected = 'clueweb09-en-trec-web-2009-20230107-training'
-    actual = translate_irds_id_to_tirex(pt.get_dataset("irds:clueweb09/en/trec-web-2009"))
-    
-    assert expected == actual
+class TestIrdsIdTranslation(unittest.TestCase):
+    def test_for_tirex_id_robust04_01(self):
+        ensure_pyterrier_is_loaded(patch_ir_datasets=False)
+        expected = 'disks45-nocr-trec-robust-2004-20230209-training'
+        actual = translate_irds_id_to_tirex( 'disks45-nocr-trec-robust-2004-20230209-training')
+        
+        assert expected == actual
+
+    def test_for_tirex_id_robust04_02(self):
+        ensure_pyterrier_is_loaded(patch_ir_datasets=True)
+        expected = 'disks45-nocr-trec-robust-2004-20230209-training'
+        actual = translate_irds_id_to_tirex( 'disks45-nocr-trec-robust-2004-20230209-training')
+        
+        assert expected == actual
+
+    def test_for_tirex_id_cw09_2014_01(self):
+        ensure_pyterrier_is_loaded(patch_ir_datasets=False)
+        expected = 'clueweb12-trec-web-2014-20230107-training'
+        actual = translate_irds_id_to_tirex('clueweb12-trec-web-2014-20230107-training')
+        
+        assert expected == actual
+
+    def test_for_tirex_id_cw09_2014_02(self):
+        ensure_pyterrier_is_loaded(patch_ir_datasets=True)
+        expected = 'clueweb12-trec-web-2014-20230107-training'
+        actual = translate_irds_id_to_tirex('clueweb12-trec-web-2014-20230107-training')
+        
+        assert expected == actual
+
+    def test_for_raw_string_robust04_01(self):
+        ensure_pyterrier_is_loaded(patch_ir_datasets=False)
+        expected = 'disks45-nocr-trec-robust-2004-20230209-training'
+        actual = translate_irds_id_to_tirex('disks45/nocr/trec-robust-2004')
+        
+        assert expected == actual
+
+    def test_for_raw_string_robust04_02(self):
+        ensure_pyterrier_is_loaded(patch_ir_datasets=True)
+        expected = 'disks45-nocr-trec-robust-2004-20230209-training'
+        actual = translate_irds_id_to_tirex('disks45/nocr/trec-robust-2004')
+        
+        assert expected == actual
+
+    def test_for_raw_string_cw09_2014_01(self):
+        ensure_pyterrier_is_loaded(patch_ir_datasets=False)
+        expected = 'clueweb12-trec-web-2014-20230107-training'
+        actual = translate_irds_id_to_tirex('clueweb12/trec-web-2014')
+        
+        assert expected == actual
+
+    def test_for_raw_string_cw09_2014_02(self):
+        ensure_pyterrier_is_loaded(patch_ir_datasets=True)
+        expected = 'clueweb12-trec-web-2014-20230107-training'
+        actual = translate_irds_id_to_tirex('clueweb12/trec-web-2014')
+        
+        assert expected == actual
+
+    def test_for_pyterrier_dataset_robust04_01(self):
+        ensure_pyterrier_is_loaded(patch_ir_datasets=False)
+        expected = 'disks45-nocr-trec-robust-2004-20230209-training'
+        actual = translate_irds_id_to_tirex(pt.get_dataset("irds:disks45/nocr/trec-robust-2004"))
+        
+        assert expected == actual
+
+    def test_for_pyterrier_dataset_robust04_02(self):
+        ensure_pyterrier_is_loaded(patch_ir_datasets=True)
+        expected = 'disks45-nocr-trec-robust-2004-20230209-training'
+        actual = translate_irds_id_to_tirex(pt.get_dataset("irds:disks45/nocr/trec-robust-2004"))
+        
+        assert expected == actual
+
+    def test_for_pyterrier_dataset_cw09_2009_01(self):
+        ensure_pyterrier_is_loaded(patch_ir_datasets=False)
+        expected = 'clueweb09-en-trec-web-2009-20230107-training'
+        actual = translate_irds_id_to_tirex(pt.get_dataset("irds:clueweb09/en/trec-web-2009"))
+        
+        assert expected == actual
+
+    def test_for_pyterrier_dataset_cw09_2009_02(self):
+        ensure_pyterrier_is_loaded(patch_ir_datasets=True)
+        expected = 'clueweb09-en-trec-web-2009-20230107-training'
+        actual = translate_irds_id_to_tirex(pt.get_dataset("irds:clueweb09/en/trec-web-2009"))
+        
+        assert expected == actual
```

### Comparing `tira-0.0.98/tests/load_rerank_data_test.py` & `tira-0.0.99/tests/load_rerank_data_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from tira.third_party_integrations import load_rerank_data
+import unittest
 
-def test_loading_rerank_data_from_local_file():
-    re_rank_data = load_rerank_data(default='tests/resources/re-ranking-outputs/')
-    
-    assert 3 == len(re_rank_data)
-    assert {"qid": "1", "query": "query 1", "docno": "doc-1", "text": "Text of doc-1", "rank": 1, "score": 10} == re_rank_data.iloc[0].to_dict()
-    assert {"qid": "3", "query": "query 3", "docno": "doc-3", "text": "Text of doc-3", "rank": 1, "score": 1} == re_rank_data.iloc[2].to_dict()
-
-def test_loading_rerank_data_from_remote_file():
-    re_rank_data = load_rerank_data(default='workshop-on-open-web-search/re-ranking-20231027-training')
-    
-    assert 6 == len(re_rank_data)
-    assert {"qid": "2", "query": "how to exit vim?", "docno": "doc-1", "text": "Press ESC key, then the : (colon), and type the wq command after the colon and hit the Enter key to save and leave Vim.", "rank": 1, "score": 10} == re_rank_data.iloc[2].to_dict()
+# .. todo:: there are no assertions in this file
 
+class TestLoadRerankData(unittest.TestCase):
+    def test_loading_rerank_data_from_local_file(self):
+        re_rank_data = load_rerank_data(default='tests/resources/re-ranking-outputs/')
+        
+        assert 3 == len(re_rank_data)
+        assert {"qid": "1", "query": "query 1", "docno": "doc-1", "text": "Text of doc-1", "rank": 1, "score": 10} == re_rank_data.iloc[0].to_dict()
+        assert {"qid": "3", "query": "query 3", "docno": "doc-3", "text": "Text of doc-3", "rank": 1, "score": 1} == re_rank_data.iloc[2].to_dict()
 
+    def test_loading_rerank_data_from_remote_file(self):
+        re_rank_data = load_rerank_data(default='workshop-on-open-web-search/re-ranking-20231027-training')
+        
+        assert 6 == len(re_rank_data)
+        assert {"qid": "2", "query": "how to exit vim?", "docno": "doc-1", "text": "Press ESC key, then the : (colon), and type the wq command after the colon and hit the Enter key to save and leave Vim.", "rank": 1, "score": 10} == re_rank_data.iloc[2].to_dict()
```

### Comparing `tira-0.0.98/tests/pt_document_processing_loader_test.py` & `tira-0.0.99/tests/pt_document_processing_loader_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from tira.local_client import Client
 
 import pandas as pd
+import unittest
 
-
-def test_for_loading_keyphrase_extraction_for_multiple_documents():
-    expected = {
-        'FT921-3964': ["increased economic aid","king hussein","increase aid","president george bush","tariq aziz iraq's deputy prime minister"],
-        'LA061489-0137': ["public appearances gorbachev","crowds","government ministries gorbachev","place gorbachev","west german well-wishers"]}
-    
-    actual = keyphrase_extraction(['FT921-3964', 'LA061489-0137'])
-    
-    assert len(actual) == 2
-    assert actual['FT921-3964'] == expected['FT921-3964']
-    assert actual['LA061489-0137'] == expected['LA061489-0137']
-
-
-def test_for_loading_keyphrase_extraction_for_single_documents():
-    expected = {"LA120390-0047": ["even friendly technology takeovers","largest technology takeover","computer industry takeover","statement sunday","attempts"]}
-    
-    actual = keyphrase_extraction(["LA120390-0047"])
-    
-    assert len(actual) == 1
-    assert actual["LA120390-0047"] == expected["LA120390-0047"]
-
-
-def test_pyterrier_can_be_loaded():
-    from tira.third_party_integrations import ensure_pyterrier_is_loaded
-    ensure_pyterrier_is_loaded()
-
+# .. todo:: this file still uses "unclean" assertions and should be converted to use unittest assertions
 
 def keyphrase_extraction(docs):
     queries = pd.DataFrame([{'docno': str(i)} for i in docs])
     tira = Client('tests/resources/')
     query_segmentation =  tira.pt.transform_documents('ir-benchmarks/webis-keyphrase-extraction/BCExtractorFO', dataset='d1')
     
     ret = query_segmentation(queries)
     return {i['docno']: i['keyphrases'] for _, i in ret.iterrows()}
 
+
+class TestPtDocumentProcessingLoaderTest(unittest.TestCase):
+    def test_for_loading_keyphrase_extraction_for_multiple_documents(self):
+        expected = {
+            'FT921-3964': ["increased economic aid","king hussein","increase aid","president george bush","tariq aziz iraq's deputy prime minister"],
+            'LA061489-0137': ["public appearances gorbachev","crowds","government ministries gorbachev","place gorbachev","west german well-wishers"]}
+        
+        actual = keyphrase_extraction(['FT921-3964', 'LA061489-0137'])
+        
+        assert len(actual) == 2
+        assert actual['FT921-3964'] == expected['FT921-3964']
+        assert actual['LA061489-0137'] == expected['LA061489-0137']
+
+
+    def test_for_loading_keyphrase_extraction_for_single_documents(self):
+        expected = {"LA120390-0047": ["even friendly technology takeovers","largest technology takeover","computer industry takeover","statement sunday","attempts"]}
+        
+        actual = keyphrase_extraction(["LA120390-0047"])
+        
+        assert len(actual) == 1
+        assert actual["LA120390-0047"] == expected["LA120390-0047"]
+
+
+    def test_pyterrier_can_be_loaded(self):
+        from tira.third_party_integrations import ensure_pyterrier_is_loaded
+        ensure_pyterrier_is_loaded()
```

### Comparing `tira-0.0.98/tests/pt_from_retriever_for_re_ranking_submission_loader_test.py` & `tira-0.0.99/tests/pt_from_retriever_for_re_ranking_submission_loader_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 from tira.local_client import Client
 
 import pandas as pd
+import unittest
 
-def test_for_multiple_queries():
-    expected = [
-        {'qid': '1', 'docno': 'doc-1', 'score':10, 'text': "Text of doc-1"},
-        {'qid': '1', 'docno': 'doc-2', 'score':9, 'text': "Text of doc-2"},
-        {'qid': '3', 'docno': 'doc-3', 'score': 1, 'text': "Text of doc-3"},
-    ]
-    
-    actual = retrieval_submission([1, 3])
-
-    assert len(actual) == 3
-    assert actual[0] == expected[0]
-    assert actual[1] == expected[1]
-    assert actual[2] == expected[2]
-
-def test_for_single_query_no_1():
-    expected = [
-        {'qid': '1', 'docno': 'doc-1', 'score':10, 'text': "Text of doc-1"},
-        {'qid': '1', 'docno': 'doc-2', 'score':9, 'text': "Text of doc-2"},
-    ]
-    
-    actual = retrieval_submission([1])
-
-    assert len(actual) == 2
-    assert actual[0] == expected[0]
-    assert actual[1] == expected[1]
-
-def test_for_single_query_no_3():
-    expected = [
-        {'qid': '3', 'docno': 'doc-3', 'score': 1, 'text': "Text of doc-3"},
-    ]
-    
-    actual = retrieval_submission([3])
-
-    assert len(actual) == 1
-    assert actual[0] == expected[0]
+# .. todo:: this file still uses "unclean" assertions and should be converted to use unittest assertions
 
 def retrieval_submission(queries):
     queries = pd.DataFrame([{'qid': str(i)} for i in queries])
     tira = Client('tests/resources/')
     retriever =  tira.pt.from_retriever_submission('ir-benchmarks/tira-ir-starters/retriever-for-re-ranking', dataset='d1')
     
     ret = retriever(queries)
     return [{'qid': i['qid'], 'docno': i['docno'], 'score': i['score'], 'text': i['text']} for _, i in ret.iterrows()]
 
+class TestPtFromRetrieverForReRankingSubmissionLoader(unittest.TestCase):
+    def test_for_multiple_queries(self):
+        expected = [
+            {'qid': '1', 'docno': 'doc-1', 'score':10, 'text': "Text of doc-1"},
+            {'qid': '1', 'docno': 'doc-2', 'score':9, 'text': "Text of doc-2"},
+            {'qid': '3', 'docno': 'doc-3', 'score': 1, 'text': "Text of doc-3"},
+        ]
+        
+        actual = retrieval_submission([1, 3])
+
+        assert len(actual) == 3
+        assert actual[0] == expected[0]
+        assert actual[1] == expected[1]
+        assert actual[2] == expected[2]
+
+    def test_for_single_query_no_1(self):
+        expected = [
+            {'qid': '1', 'docno': 'doc-1', 'score':10, 'text': "Text of doc-1"},
+            {'qid': '1', 'docno': 'doc-2', 'score':9, 'text': "Text of doc-2"},
+        ]
+        
+        actual = retrieval_submission([1])
+
+        assert len(actual) == 2
+        assert actual[0] == expected[0]
+        assert actual[1] == expected[1]
+
+    def test_for_single_query_no_3(self):
+        expected = [
+            {'qid': '3', 'docno': 'doc-3', 'score': 1, 'text': "Text of doc-3"},
+        ]
+        
+        actual = retrieval_submission([3])
+
+        assert len(actual) == 1
+        assert actual[0] == expected[0]
```

### Comparing `tira-0.0.98/tests/pt_from_retriever_submission_loader_test.py` & `tira-0.0.99/tests/pt_from_retriever_submission_loader_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 from tira.local_client import Client
 
 import pandas as pd
+import unittest
 
-def test_for_multiple_queries():
-    expected = [
-        {'qid': '1', 'docno': 'doc-1', 'score':10},
-        {'qid': '1', 'docno': 'doc-2', 'score':9},
-        {'qid': '3', 'docno': 'doc-3', 'score': 1},
-    ]
-    
-    actual = retrieval_submission([1, 3])
-
-    assert len(actual) == 3
-    assert actual[0] == expected[0]
-    assert actual[1] == expected[1]
-    assert actual[2] == expected[2]
-
-def test_for_single_query_no_1():
-    expected = [
-        {'qid': '1', 'docno': 'doc-1', 'score':10},
-        {'qid': '1', 'docno': 'doc-2', 'score':9},
-    ]
-    
-    actual = retrieval_submission([1])
-
-    assert len(actual) == 2
-    assert actual[0] == expected[0]
-    assert actual[1] == expected[1]
-
-def test_for_single_query_no_3():
-    expected = [
-        {'qid': '3', 'docno': 'doc-3', 'score': 1},
-    ]
-    
-    actual = retrieval_submission([3])
-
-    assert len(actual) == 1
-    assert actual[0] == expected[0]
-
-def test_retrieval_submission_from_rest_api():
-    from tira.rest_api_client import Client
-    from tira.third_party_integrations import ensure_pyterrier_is_loaded
-    import pyterrier as pt
-    ensure_pyterrier_is_loaded()
-    tira = Client()
-
-    q = tira.pt.from_submission('ir-benchmarks/tira-ir-starter/BM25 Re-Rank (tira-ir-starter-pyterrier)', pt.get_dataset("irds:disks45/nocr/trec-robust-2004"))
-    assert len(q(pd.DataFrame([{'qid': '306'}]))) == 1000
-    assert q(pd.DataFrame([{'qid': '306'}])).iloc[0].to_dict()['docno'] == 'LA021790-0114'
-    assert q(pd.DataFrame([{'qid': '306'}])).iloc[0].to_dict()['qid'] == '306'
-    assert q(pd.DataFrame([{'qid': '306'}])).iloc[999].to_dict()['docno'] == 'FBIS4-47956'
-    assert q(pd.DataFrame([{'qid': '306'}])).iloc[999].to_dict()['qid'] == '306'
+# .. todo:: this file still uses "unclean" assertions and should be converted to use unittest assertions
 
 def retrieval_submission(queries):
     queries = pd.DataFrame([{'qid': str(i)} for i in queries])
     tira = Client('tests/resources/')
     retriever =  tira.pt.from_retriever_submission('ir-benchmarks/tira-ir-starters/retriever', dataset='d1')
     
     ret = retriever(queries)
     return [{'qid': i['qid'], 'docno': i['docno'], 'score': i['score']} for _, i in ret.iterrows()]
+
+class TestPtFromRetrieverSubmissionLoaderTest(unittest.TestCase):
+    def test_for_multiple_queries(self):
+        expected = [
+            {'qid': '1', 'docno': 'doc-1', 'score':10},
+            {'qid': '1', 'docno': 'doc-2', 'score':9},
+            {'qid': '3', 'docno': 'doc-3', 'score': 1},
+        ]
+        
+        actual = retrieval_submission([1, 3])
+
+        assert len(actual) == 3
+        assert actual[0] == expected[0]
+        assert actual[1] == expected[1]
+        assert actual[2] == expected[2]
+
+    def test_for_single_query_no_1(self):
+        expected = [
+            {'qid': '1', 'docno': 'doc-1', 'score':10},
+            {'qid': '1', 'docno': 'doc-2', 'score':9},
+        ]
+        
+        actual = retrieval_submission([1])
+
+        assert len(actual) == 2
+        assert actual[0] == expected[0]
+        assert actual[1] == expected[1]
+
+    def test_for_single_query_no_3(self):
+        expected = [
+            {'qid': '3', 'docno': 'doc-3', 'score': 1},
+        ]
+        
+        actual = retrieval_submission([3])
+
+        assert len(actual) == 1
+        assert actual[0] == expected[0]
+
+    def test_retrieval_submission_from_rest_api(self):
+        from tira.rest_api_client import Client
+        from tira.third_party_integrations import ensure_pyterrier_is_loaded
+        import pyterrier as pt
+        ensure_pyterrier_is_loaded()
+        tira = Client()
+
+        q = tira.pt.from_submission('ir-benchmarks/tira-ir-starter/BM25 Re-Rank (tira-ir-starter-pyterrier)', pt.get_dataset("irds:disks45/nocr/trec-robust-2004"))
+        assert len(q(pd.DataFrame([{'qid': '306'}]))) == 1000
+        assert q(pd.DataFrame([{'qid': '306'}])).iloc[0].to_dict()['docno'] == 'LA021790-0114'
+        assert q(pd.DataFrame([{'qid': '306'}])).iloc[0].to_dict()['qid'] == '306'
+        assert q(pd.DataFrame([{'qid': '306'}])).iloc[999].to_dict()['docno'] == 'FBIS4-47956'
+        assert q(pd.DataFrame([{'qid': '306'}])).iloc[999].to_dict()['qid'] == '306'
```

### Comparing `tira-0.0.98/tests/pt_query_processing_loader_test.py` & `tira-0.0.99/tests/pt_query_processing_loader_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,90 @@
 from tira.local_client import Client
 
 import pandas as pd
+import unittest
 
-
-def test_for_loading_query_segmentations_for_multiple_queries():
-    expected = {'350': ["health and","computer terminals"], '353': ["antarctica","exploration"]}
-    
-    actual = query_segmentation([350, 353])
-    
-    assert len(actual) == 2
-    assert actual['350'] == expected['350']
-    assert actual['353'] == expected['353']
-
-
-def test_for_loading_query_segmentations_for_single_query():
-    expected = {'351': ["falkland","petroleum exploration"]}
-    
-    actual = query_segmentation([351])
-    
-    assert len(actual) == 1
-    assert actual['351'] == expected['351']
-
-
-def test_pyterrier_can_be_loaded():
-    from tira.third_party_integrations import ensure_pyterrier_is_loaded
-    ensure_pyterrier_is_loaded()
-
-def test_rest_query_submission_with_rest_api_01():
-    from tira.rest_api_client import Client
-    tira = Client()
-
-    q = tira.pt.transform_queries('ir-benchmarks/ows/query-segmentation-wt-snp', 'disks45-nocr-trec-robust-2004-20230209-training')
-    assert len(q(pd.DataFrame([{'qid': '303'}]))) == 1
-    assert q(pd.DataFrame([{'qid': '303'}])).iloc[0].to_dict()['segmentation'] == ['hubble telescope achievements']
-
-def test_rest_query_submission_with_rest_api_02():
-    from tira.rest_api_client import Client
-    tira = Client()
-
-    q = tira.pt.transform_queries('ir-benchmarks/ows/query-segmentation-hyb-a', 'disks45-nocr-trec-robust-2004-20230209-training')
-    assert len(q(pd.DataFrame([{'qid': '303'}]))) == 1
-    assert q(pd.DataFrame([{'qid': '303'}])).iloc[0].to_dict()['segmentation'] == ['hubble telescope', 'achievements']
-
-def test_rest_query_submission_with_rest_api_03():
-    from tira.rest_api_client import Client
-    from tira.third_party_integrations import ensure_pyterrier_is_loaded
-    import pyterrier as pt
-    ensure_pyterrier_is_loaded()
-    tira = Client()
-
-    q = tira.pt.transform_queries('ir-benchmarks/fschlatt/matching-taping', pt.get_dataset("irds:clueweb09/en/trec-web-2009"))
-    assert len(q(pd.DataFrame([{'qid': '26'}]))) == 1
-    assert q(pd.DataFrame([{'qid': '26'}])).iloc[0].to_dict()['mean_health_score'] == 168.416
-    assert q(pd.DataFrame([{'qid': '26'}])).iloc[0].to_dict()['median_health_score'] == 130.3137
-
-def test_rest_query_submission_with_rest_api_and_custom_selection():
-    from tira.rest_api_client import Client
-    from tira.third_party_integrations import ensure_pyterrier_is_loaded
-    import pyterrier as pt
-    ensure_pyterrier_is_loaded()
-    tira = Client()
-
-    q = tira.pt.transform_queries('ir-benchmarks/fschlatt/matching-taping', pt.get_dataset("irds:clueweb09/en/trec-web-2009"), '/q*.jsonl')
-    assert len(q(pd.DataFrame([{'qid': '26'}]))) == 1
-    assert q(pd.DataFrame([{'qid': '26'}])).iloc[0].to_dict()['mean_health_score'] == 168.416
-    assert q(pd.DataFrame([{'qid': '26'}])).iloc[0].to_dict()['median_health_score'] == 130.3137
-
-def test_rest_query_submission_with_rest_api_04():
-    from tira.rest_api_client import Client
-    from tira.third_party_integrations import ensure_pyterrier_is_loaded
-    import pyterrier as pt
-    ensure_pyterrier_is_loaded()
-    tira = Client()
-
-    q = tira.pt.transform_queries('ir-benchmarks/qpptk/fixed-sealer', pt.get_dataset("irds:disks45/nocr/trec-robust-2004"))
-    assert len(q(pd.DataFrame([{'qid': '301'}]))) == 1
-    assert q(pd.DataFrame([{'qid': '301'}])).iloc[0].to_dict()['max-idf'] == 3.5629408815
-    assert q(pd.DataFrame([{'qid': '301'}])).iloc[0].to_dict()['avg-idf'] == 2.4740487603
+# .. todo:: this file still uses "unclean" assertions and should be converted to use unittest assertions
 
 def query_segmentation(queries):
     queries = pd.DataFrame([{'qid': str(i)} for i in queries])
     tira = Client('tests/resources/')
     query_segmentation =  tira.pt.transform_queries('ir-benchmarks/webis-query-segmentation/wt-snp-baseline', dataset='d1')
     
     ret = query_segmentation(queries)
     return {i['qid']: i['segmentation'] for _, i in ret.iterrows()}
 
+class TestQueryProcessingLoader(unittest.TestCase):
+    def test_for_loading_query_segmentations_for_multiple_queries(self):
+        expected = {'350': ["health and","computer terminals"], '353': ["antarctica","exploration"]}
+        
+        actual = query_segmentation([350, 353])
+        
+        assert len(actual) == 2
+        assert actual['350'] == expected['350']
+        assert actual['353'] == expected['353']
+
+
+    def test_for_loading_query_segmentations_for_single_query(self):
+        expected = {'351': ["falkland","petroleum exploration"]}
+        
+        actual = query_segmentation([351])
+        
+        assert len(actual) == 1
+        assert actual['351'] == expected['351']
+
+
+    def test_pyterrier_can_be_loaded(self):
+        from tira.third_party_integrations import ensure_pyterrier_is_loaded
+        ensure_pyterrier_is_loaded()
+
+    def test_rest_query_submission_with_rest_api_01(self):
+        from tira.rest_api_client import Client
+        tira = Client()
+
+        q = tira.pt.transform_queries('ir-benchmarks/ows/query-segmentation-wt-snp', 'disks45-nocr-trec-robust-2004-20230209-training')
+        assert len(q(pd.DataFrame([{'qid': '303'}]))) == 1
+        assert q(pd.DataFrame([{'qid': '303'}])).iloc[0].to_dict()['segmentation'] == ['hubble telescope achievements']
+
+    def test_rest_query_submission_with_rest_api_02(self):
+        from tira.rest_api_client import Client
+        tira = Client()
+
+        q = tira.pt.transform_queries('ir-benchmarks/ows/query-segmentation-hyb-a', 'disks45-nocr-trec-robust-2004-20230209-training')
+        assert len(q(pd.DataFrame([{'qid': '303'}]))) == 1
+        assert q(pd.DataFrame([{'qid': '303'}])).iloc[0].to_dict()['segmentation'] == ['hubble telescope', 'achievements']
+
+    def test_rest_query_submission_with_rest_api_03(self):
+        from tira.rest_api_client import Client
+        from tira.third_party_integrations import ensure_pyterrier_is_loaded
+        import pyterrier as pt
+        ensure_pyterrier_is_loaded()
+        tira = Client()
+
+        q = tira.pt.transform_queries('ir-benchmarks/fschlatt/matching-taping', pt.get_dataset("irds:clueweb09/en/trec-web-2009"))
+        assert len(q(pd.DataFrame([{'qid': '26'}]))) == 1
+        assert q(pd.DataFrame([{'qid': '26'}])).iloc[0].to_dict()['mean_health_score'] == 168.416
+        assert q(pd.DataFrame([{'qid': '26'}])).iloc[0].to_dict()['median_health_score'] == 130.3137
+
+    def test_rest_query_submission_with_rest_api_and_custom_selection(self):
+        from tira.rest_api_client import Client
+        from tira.third_party_integrations import ensure_pyterrier_is_loaded
+        import pyterrier as pt
+        ensure_pyterrier_is_loaded()
+        tira = Client()
+
+        q = tira.pt.transform_queries('ir-benchmarks/fschlatt/matching-taping', pt.get_dataset("irds:clueweb09/en/trec-web-2009"), '/q*.jsonl')
+        assert len(q(pd.DataFrame([{'qid': '26'}]))) == 1
+        assert q(pd.DataFrame([{'qid': '26'}])).iloc[0].to_dict()['mean_health_score'] == 168.416
+        assert q(pd.DataFrame([{'qid': '26'}])).iloc[0].to_dict()['median_health_score'] == 130.3137
+
+    def test_rest_query_submission_with_rest_api_04(self):
+        from tira.rest_api_client import Client
+        from tira.third_party_integrations import ensure_pyterrier_is_loaded
+        import pyterrier as pt
+        ensure_pyterrier_is_loaded()
+        tira = Client()
+
+        q = tira.pt.transform_queries('ir-benchmarks/qpptk/fixed-sealer', pt.get_dataset("irds:disks45/nocr/trec-robust-2004"))
+        assert len(q(pd.DataFrame([{'qid': '301'}]))) == 1
+        assert q(pd.DataFrame([{'qid': '301'}])).iloc[0].to_dict()['max-idf'] == 3.5629408815
+        assert q(pd.DataFrame([{'qid': '301'}])).iloc[0].to_dict()['avg-idf'] == 2.4740487603
```

### Comparing `tira-0.0.98/tests/rest_api_test.py` & `tira-0.0.99/tests/rest_api_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 from tira.rest_api_client import Client
-tira = Client()
+import unittest
 
+# .. todo:: this file still uses "unclean" assertions and should be converted to use unittest assertions
 
-def test_all_softwares_works_for_tirex():
-    actual = tira.all_softwares("ir-benchmarks")
-    
-    assert 'ir-benchmarks/tira-ir-starter/ChatNoir' in actual
-    assert 'ir-benchmarks/tira-ir-starter/Index (tira-ir-starter-pyterrier)' in actual
-
-def test_details_of_public_software_01():
-    actual = tira.docker_software( 'ir-benchmarks/tira-ir-starter/TF_IDF (tira-ir-starter-pyterrier)')
-
-    assert actual is not None
-    assert actual['ir_re_ranker'] == False
-
-def test_output_of_run():
-    actual = tira.get_run_output('ir-benchmarks/tira-ir-starter/BM25 Re-Rank (tira-ir-starter-pyterrier)', 'antique-test-20230107-training')
-    actual = open(actual + '/run.txt', 'r').read()
-    
-    assert actual.startswith('8293 Q0 8293_1 1 33.568841093129976 pyterrier.default_pipelines.wmodel_text_scorer')
+class TestRestAPI(unittest.TestCase):
+    tira: Client
+
+    @classmethod
+    def setUpClass(cls):
+        TestRestAPI.tira = Client()
+
+    def test_all_softwares_works_for_tirex(self):
+        actual = TestRestAPI.tira.all_softwares("ir-benchmarks")
+        
+        assert 'ir-benchmarks/tira-ir-starter/ChatNoir' in actual
+        assert 'ir-benchmarks/tira-ir-starter/Index (tira-ir-starter-pyterrier)' in actual
+
+    def test_details_of_public_software_01(self):
+        actual = TestRestAPI.tira.docker_software( 'ir-benchmarks/tira-ir-starter/TF_IDF (tira-ir-starter-pyterrier)')
+
+        assert actual is not None
+        assert actual['ir_re_ranker'] == False
+
+    def test_output_of_run(self):
+        actual = TestRestAPI.tira.get_run_output('ir-benchmarks/tira-ir-starter/BM25 Re-Rank (tira-ir-starter-pyterrier)', 'antique-test-20230107-training')
+        actual = open(actual + '/run.txt', 'r').read()
+        
+        assert actual.startswith('8293 Q0 8293_1 1 33.568841093129976 pyterrier.default_pipelines.wmodel_text_scorer')
```

### Comparing `tira-0.0.98/tests/test_export_submission_environment.py` & `tira-0.0.99/tests/test_export_submission_environment.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tests/test_persisting_run_files.py` & `tira-0.0.99/tests/test_persisting_run_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from tira.third_party_integrations import persist_and_normalize_run
 import pandas as pd
+import unittest
 
-def test_variant_01():
-    run = pd.DataFrame([{"qid": "1", "score": "1", "docno": "d1"},  {"qid": "1", "score": "0", "docno": "d2"},  {"qid": "1", "score": "2", "docno": "d3"}])
-    persist_and_normalize_run(run, 'system_name', default_output='/tmp/variant_01.run.txt')
-    
-def test_variant_02():
-    run = pd.DataFrame([{"qid": "1", "score": "1", "docno": "d1"},  {"qid": "1", "score": "0", "docno": "d2"},  {"qid": "1", "score": "2", "docno": "d3"}])
-    persist_and_normalize_run(run, 'system_name', output_file='/tmp/variant_02.run.txt')
+# .. todo:: there are no assertions in this file
 
-def test_variant_03():
-    run = pd.DataFrame([{"qid": "1", "score": "1", "docno": "d1"},  {"qid": "1", "score": "0", "docno": "d2"},  {"qid": "1", "score": "2", "docno": "d3"}])
-    persist_and_normalize_run(run, 'system_name')
+class TestPersistingRunFiles(unittest.TestCase):
 
+    def test_variant_01(self):
+        run = pd.DataFrame([{"qid": "1", "score": "1", "docno": "d1"},  {"qid": "1", "score": "0", "docno": "d2"},  {"qid": "1", "score": "2", "docno": "d3"}])
+        persist_and_normalize_run(run, 'system_name', default_output='/tmp/variant_01.run.txt')
+        
+    def test_variant_02(self):
+        run = pd.DataFrame([{"qid": "1", "score": "1", "docno": "d1"},  {"qid": "1", "score": "0", "docno": "d2"},  {"qid": "1", "score": "2", "docno": "d3"}])
+        persist_and_normalize_run(run, 'system_name', output_file='/tmp/variant_02.run.txt')
+
+    def test_variant_03(self):
+        run = pd.DataFrame([{"qid": "1", "score": "1", "docno": "d1"},  {"qid": "1", "score": "0", "docno": "d2"},  {"qid": "1", "score": "2", "docno": "d3"}])
+        persist_and_normalize_run(run, 'system_name')
```

### Comparing `tira-0.0.98/tira/inference_server.py` & `tira-0.0.99/tira/inference_server.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tira/io_utils.py` & `tira-0.0.99/tira/io_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import pandas as pd
 from glob import glob
 import gzip
 import json
 import os
-from typing import Any, Iterable, Dict, Union
+from typing import Any, Iterable, Dict, Union, Generator
+from pathlib import Path
+import logging
 
 
 def parse_jsonl_line(input: Union[str, bytearray, bytes], load_default_text: bool) -> Dict:
-
     """
     Deseralizes the line using JSON deserialization. Optionally strips the 'original_query' and 'original_document'
     fields from the resulting object and converts the qid and docno fields to strings.
 
     :param str | bytearray | bytes input: A json-serialized string.
-    :param bool load_default_text: If true, the origianl_query and original_document fields are removed and the qid and docno
-        values are converted to strings.
+    :param bool load_default_text: If true, the original_query and original_document fields are removed and the qid and
+        docno values are converted to strings.
     :return: The deserialized and (optionally) processed object.
     :rtype: dict
 
     :Example:
         >>> parse_jsonl_line('{}', False)
         {}
         >>> parse_jsonl_line('{"original_query": "xxxx"}', False)
@@ -39,15 +40,19 @@
         for field_to_str in ['qid', 'docno']:
             if field_to_str in obj:
                 obj[field_to_str] = str(obj[field_to_str])
 
     return obj
 
 
-def stream_all_lines(input_file, load_default_text):
+def stream_all_lines(input_file: Union[str, Iterable[bytes]], load_default_text: bool) -> Generator[Dict, Any, Any]:
+    """
+    .. todo:: add documentation
+    .. todo:: this function has two semantics: handling a file and handling file-contents
+    """
     if type(input_file) is str:
         if not os.path.isfile(input_file):
             return
 
         if input_file.endswith('.gz'):
             with gzip.open(input_file, 'rt', encoding='utf-8') as f:
                 yield from stream_all_lines(f, load_default_text)
@@ -57,15 +62,19 @@
 
         return
 
     for line in input_file:
         yield parse_jsonl_line(line, load_default_text)
 
 
-def all_lines_to_pandas(input_file: str | Iterable[str], load_default_text):
+def all_lines_to_pandas(input_file: Union[str, Iterable[str]], load_default_text: bool) -> pd.DataFrame:
+    """
+    .. todo:: add documentation
+    .. todo:: this function has two semantics: handling a file and handling file-contents
+    """
     if type(input_file) is str:
         if input_file.endswith('.gz'):
             with gzip.open(input_file, 'rt', encoding='utf-8') as f:
                 return all_lines_to_pandas(f, load_default_text)
         else:
             with open(input_file, 'r') as f:
                 return all_lines_to_pandas(f, load_default_text)
@@ -75,25 +84,44 @@
 
     for line in input_file:
         ret += [parse_jsonl_line(line, load_default_text)]
 
     return pd.DataFrame(ret)
 
 
-def __num(s):
+def __num(input: str) -> Union[str, int, float]:
+    """
+    Converts the input to an int or float if possible. Returns the inputted string otherwise.
+
+    :param str input: The string that should be converted to a float or int if possible.
+    :return: The intrepteted input.
+    :rtype: str | int | float
+
+    :Example:
+        >>> __num("hello world")
+        "hello world"
+        >>> __num("-42")
+        -42
+        >>> __num("3.5")
+        3.5
+        >>> __num("2e-6")
+        2e-6
+        >>> __num(" -42")
+        " -42"
+    """
     try:
-        return int(s)
+        return int(input)
     except ValueError:
         try:
-            return float(s)
+            return float(input)
         except ValueError:
-            return s
+            return input
 
 
-def run_cmd(cmd, ignore_failure=False):
+def run_cmd(cmd: list[str], ignore_failure=False):
     import subprocess
     exit_code = subprocess.call(cmd)
 
     if not ignore_failure and exit_code != 0:
         raise ValueError(f'Command {cmd} did exit with return code {exit_code}.')
 
 
@@ -144,27 +172,26 @@
                 raise ValueError(f'I need the parameter {k} to continue, but could not find one or it is empty. This likely is a configuration error, e.g., due to missing secrets.')
             
             ret['IMAGE_TAG'] = f'registry.webis.de/code-research/tira/tira-user-{ret["TIRA_VM_ID"]}/submission-{ret["TIRA_DOCKER_PATH"].replace("/", "-").replace(" ", "-")}:{ret["GITHUB_SHA"]}'
 
     return [k + '=' + v for k, v in ret.items()]
 
 
-def load_output_of_directory(directory, evaluation=False, verbose=False):
+def load_output_of_directory(directory: Path, evaluation: bool=False) -> Union[Dict, pd.DataFrame]:
     files = glob(str(directory) + '/*')
 
     if evaluation:
         files = [i for i in files if i.endswith('.prototext')]
 
     if len(files) != 1:
         raise ValueError('Expected exactly one output file. Got: ', files)
 
     files = files[0]
 
-    if verbose:
-        print(f'Read file from {files}')
+    logging.debug(f'Read file from {files}')
 
     if evaluation:
         ret = {}
         for i in [i for i in open(files, 'r').read().split('measure') if 'key:' in i and 'value:' in i]:
             key = i.split('key:')[1].split('value')[0].split('"')[1]
             value = i.split('key:')[1].split('value')[1].split('"')[1]
```

### Comparing `tira-0.0.98/tira/ir_datasets_util.py` & `tira-0.0.99/tira/ir_datasets_util.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tira/local_client.py` & `tira-0.0.99/tira/local_client.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tira/local_execution_integration.py` & `tira-0.0.99/tira/local_execution_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import docker
 import json
 from copy import deepcopy
 import tempfile
 import subprocess
 import tarfile
 import logging
+from pathlib import Path
+import pandas as pd
 
 
 class LocalExecutionIntegration():
     def __init__(self, tira_client=None):
         self.tira_client = tira_client
 
     def __normalize_command(self, cmd, evaluator):
```

### Comparing `tira-0.0.98/tira/pandas_integration.py` & `tira-0.0.99/tira/pandas_integration.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tira/pyterrier_integration.py` & `tira-0.0.99/tira/pyterrier_integration.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tira/pyterrier_util.py` & `tira-0.0.99/tira/pyterrier_util.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tira/rest_api_client.py` & `tira-0.0.99/tira/rest_api_client.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tira/third_party_integrations.py` & `tira-0.0.99/tira/third_party_integrations.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tira/tira_client.py` & `tira-0.0.99/tira/tira_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC
-from typing import TYPE_CHECKING, Literal, overload
+from typing import TYPE_CHECKING, Literal, Union, overload
 
 if TYPE_CHECKING:
     from typing import Any, Dict, Optional
 
     import pandas as pd
 
 # .. todo:: this file needs further documentation
@@ -71,10 +71,10 @@
         self,
         task,
         dataset,
         software,
         team=None,
         previous_stage=None,
         return_metadata: bool = False,
-    ) -> "pd.DataFrame | tuple[pd.DataFrame, str]":
+    ) -> "Union[pd.DataFrame, tuple[pd.DataFrame, str]]":
         # .. todo:: typehint
         pass
```

### Comparing `tira-0.0.98/tira/tira_run.py` & `tira-0.0.99/tira/tira_run.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tira/tira_run_inference_server.py` & `tira-0.0.99/tira/tira_run_inference_server.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tira/tira_run_notebook.py` & `tira-0.0.99/tira/tira_run_notebook.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tira/tirex.py` & `tira-0.0.99/tira/tirex.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.98/tira.egg-info/PKG-INFO` & `tira-0.0.99/tira.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tira
-Version: 0.0.98
+Version: 0.0.99
 Summary: Simple access to the TIRA API.
 Home-page: https://github.com/tira-io/tira
 Author: Maik Fröbe
 Author-email: maik.froebe@uni-weimar.de
 Maintainer: Maik Fröbe
 Project-URL: Bug Tracker, https://github.com/tira-io/tira/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tira-0.0.98/tira.egg-info/SOURCES.txt` & `tira-0.0.99/tira.egg-info/SOURCES.txt`

 * *Files identical despite different names*

