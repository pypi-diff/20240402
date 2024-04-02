# Comparing `tmp/fore-0.1.6.tar.gz` & `tmp/fore-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fore-0.1.6.tar", last modified: Wed Mar 20 17:40:08 2024, max compression
+gzip compressed data, was "fore-0.1.7.tar", last modified: Tue Apr  2 16:22:30 2024, max compression
```

## Comparing `fore-0.1.6.tar` & `fore-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 asheempanakkat   (501) staff       (20)        0 2024-03-20 17:40:08.901101 fore-0.1.6/
--rw-r--r--   0 asheempanakkat   (501) staff       (20)    11344 2024-02-20 13:35:34.000000 fore-0.1.6/LICENSE
--rw-r--r--   0 asheempanakkat   (501) staff       (20)     4908 2024-03-20 17:40:08.900885 fore-0.1.6/PKG-INFO
--rw-r--r--   0 asheempanakkat   (501) staff       (20)     4295 2024-03-20 17:14:20.000000 fore-0.1.6/README.md
-drwxr-xr-x   0 asheempanakkat   (501) staff       (20)        0 2024-03-20 17:40:08.897860 fore-0.1.6/fore/
--rw-r--r--   0 asheempanakkat   (501) staff       (20)        0 2024-02-20 13:35:34.000000 fore-0.1.6/fore/__init__.py
-drwxr-xr-x   0 asheempanakkat   (501) staff       (20)        0 2024-03-20 17:40:08.900312 fore-0.1.6/fore/foresight/
--rw-r--r--   0 asheempanakkat   (501) staff       (20)      178 2024-02-20 13:35:34.000000 fore-0.1.6/fore/foresight/__init__.py
--rw-r--r--   0 asheempanakkat   (501) staff       (20)    13099 2024-03-20 17:36:39.000000 fore-0.1.6/fore/foresight/client.py
--rw-r--r--   0 asheempanakkat   (501) staff       (20)    19998 2024-03-20 17:37:28.000000 fore-0.1.6/fore/foresight/client_test.py
--rw-r--r--   0 asheempanakkat   (501) staff       (20)     4390 2024-03-20 17:38:19.000000 fore-0.1.6/fore/foresight/schema.py
--rw-r--r--   0 asheempanakkat   (501) staff       (20)      300 2024-02-20 13:35:34.000000 fore-0.1.6/fore/foresight/utils.py
-drwxr-xr-x   0 asheempanakkat   (501) staff       (20)        0 2024-03-20 17:40:08.900532 fore-0.1.6/fore.egg-info/
--rw-r--r--   0 asheempanakkat   (501) staff       (20)     4908 2024-03-20 17:40:08.000000 fore-0.1.6/fore.egg-info/PKG-INFO
--rw-r--r--   0 asheempanakkat   (501) staff       (20)      319 2024-03-20 17:40:08.000000 fore-0.1.6/fore.egg-info/SOURCES.txt
--rw-r--r--   0 asheempanakkat   (501) staff       (20)        1 2024-03-20 17:40:08.000000 fore-0.1.6/fore.egg-info/dependency_links.txt
--rw-r--r--   0 asheempanakkat   (501) staff       (20)       59 2024-03-20 17:40:08.000000 fore-0.1.6/fore.egg-info/requires.txt
--rw-r--r--   0 asheempanakkat   (501) staff       (20)        5 2024-03-20 17:40:08.000000 fore-0.1.6/fore.egg-info/top_level.txt
--rw-r--r--   0 asheempanakkat   (501) staff       (20)      866 2024-03-20 17:38:34.000000 fore-0.1.6/pyproject.toml
--rw-r--r--   0 asheempanakkat   (501) staff       (20)       38 2024-03-20 17:40:08.901139 fore-0.1.6/setup.cfg
+drwxr-xr-x   0 asheempanakkat   (501) staff       (20)        0 2024-04-02 16:22:30.233880 fore-0.1.7/
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)    11344 2024-02-20 13:35:34.000000 fore-0.1.7/LICENSE
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)     4908 2024-04-02 16:22:30.233651 fore-0.1.7/PKG-INFO
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)     4295 2024-04-02 16:20:20.000000 fore-0.1.7/README.md
+drwxr-xr-x   0 asheempanakkat   (501) staff       (20)        0 2024-04-02 16:22:30.230687 fore-0.1.7/fore/
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)        0 2024-02-20 13:35:34.000000 fore-0.1.7/fore/__init__.py
+drwxr-xr-x   0 asheempanakkat   (501) staff       (20)        0 2024-04-02 16:22:30.232965 fore-0.1.7/fore/foresight/
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)      178 2024-02-20 13:35:34.000000 fore-0.1.7/fore/foresight/__init__.py
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)    13697 2024-04-02 16:20:20.000000 fore-0.1.7/fore/foresight/client.py
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)    22474 2024-04-02 16:20:20.000000 fore-0.1.7/fore/foresight/client_test.py
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)     4390 2024-04-02 16:20:20.000000 fore-0.1.7/fore/foresight/schema.py
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)      300 2024-02-20 13:35:34.000000 fore-0.1.7/fore/foresight/utils.py
+drwxr-xr-x   0 asheempanakkat   (501) staff       (20)        0 2024-04-02 16:22:30.233325 fore-0.1.7/fore.egg-info/
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)     4908 2024-04-02 16:22:30.000000 fore-0.1.7/fore.egg-info/PKG-INFO
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)      319 2024-04-02 16:22:30.000000 fore-0.1.7/fore.egg-info/SOURCES.txt
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)        1 2024-04-02 16:22:30.000000 fore-0.1.7/fore.egg-info/dependency_links.txt
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)       59 2024-04-02 16:22:30.000000 fore-0.1.7/fore.egg-info/requires.txt
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)        5 2024-04-02 16:22:30.000000 fore-0.1.7/fore.egg-info/top_level.txt
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)      866 2024-04-02 16:21:24.000000 fore-0.1.7/pyproject.toml
+-rw-r--r--   0 asheempanakkat   (501) staff       (20)       38 2024-04-02 16:22:30.233919 fore-0.1.7/setup.cfg
```

### Comparing `fore-0.1.6/LICENSE` & `fore-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fore-0.1.6/PKG-INFO` & `fore-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fore
-Version: 0.1.6
+Version: 0.1.7
 Summary: fore ai packages
 Author-email: fore ai <info@foreai.co>
 Maintainer-email: fore ai <info@foreai.co>
 License: Apache 2.0 License
 Project-URL: Homepage, https://foreai.co
 Project-URL: Repository, https://github.com/foreai-co/fore
 Project-URL: Issues, https://github.com/foreai-co/fore/issues
```

### Comparing `fore-0.1.6/README.md` & `fore-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fore-0.1.6/fore/foresight/client.py` & `fore-0.1.7/fore/foresight/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from typing import Callable, Dict, List, Optional, Union
 
 import requests
 from requests import Response
 
 from fore.foresight.schema import (CreateEvalsetRequest, EvalRunConfig,
                                    EvalRunDetails, EvalRunEntry, EvalsetEntry,
-                                   EvalsetMetadata, InferenceOutput,
-                                   LogRequest, LogTuple, MetricType,
+                                   EvalsetMetadata, InferenceOutput, LogRequest,
+                                   LogTuple, MetricType,
                                    UploadInferenceOutputsRequest)
 from fore.foresight.utils import convert_to_pandas_dataframe
 
 GenerateFnT = Callable[[str], InferenceOutput]
 
 GATEWAY_URL = "https://foresight-gateway.foreai.co"
 UI_URL = "https://foresight.foreai.co"
@@ -84,18 +84,17 @@
         entries = []
 
         for i, query in enumerate(queries):
             reference_answer = None
             if reference_answers:
                 reference_answer = reference_answers[i]
             entries.append(
-                EvalsetEntry(
-                    query=query,
-                    reference_answer=reference_answer,
-                    entry_id=str(uuid.uuid4())))
+                EvalsetEntry(query=query,
+                             reference_answer=reference_answer,
+                             entry_id=str(uuid.uuid4())))
         evalset = CreateEvalsetRequest(evalset_id=evalset_id,
                                        evalset_entries=entries)
 
         response = self.__make_request(
             method="post",
             endpoint="/api/eval/set",
             input_json=evalset.model_dump(mode="json"))
@@ -147,50 +146,66 @@
 
         if response.status_code == 200:
             logging.info("Eval run with experiment_id %s created.",
                          run_config.experiment_id)
 
         return response
 
-    def generate_answers_and_run_eval(self, generate_fn: GenerateFnT,
-                                      run_config: EvalRunConfig) -> Response:
+    def generate_answers_and_run_eval(self,
+                                      generate_fn: GenerateFnT,
+                                      run_config: EvalRunConfig,
+                                      batch_size=10):
         """Creates an eval run entry, generates answers and runs the eval.
 
         This method calls the generate_fn on each query in the evalset, triggers
         the metric computation and caches all results in a new eval run.
 
         Args:
             generate_fn: A function that takes a query and returns an
                 InferenceOutput.
             run_config: The configuration for running the eval.
-
-        Returns: the HTTP response on success or raises an HTTPError on failure.
+            batch_size: The max number of inference outputs to upload in one
+                batch.
         """
         self.create_evalrun(run_config=run_config)
         experiment_id = run_config.experiment_id
         queries = self.get_evalrun_queries(experiment_id=experiment_id)
 
+        if not queries:
+            logging.error("No queries found for experiment_id: %s",
+                          experiment_id)
+            return
+
         outputs = {}
         for entry_id, query in queries.items():
             inference_output = generate_fn(query)
             outputs[entry_id] = inference_output
 
-        outputs = UploadInferenceOutputsRequest(
-            experiment_id=experiment_id, entry_id_to_inference_output=outputs)
-
-        response = self.__make_request(
-            method="put",
-            endpoint="/api/eval/run/entries",
-            input_json=outputs.model_dump(mode="json"))
+        for i in range(0, len(outputs), batch_size):
+            outputs_chunk = {
+                k: outputs[k] for k in list(outputs.keys())[i:i + batch_size]
+            }
+            output_request = UploadInferenceOutputsRequest(
+                experiment_id=experiment_id,
+                entry_id_to_inference_output=outputs_chunk)
 
-        if response.status_code == 200:
-            logging.info("Eval run successful."
-                         "Visit %s to view results.", self.ui_url)
+            res = self.__make_request(
+                method="put",
+                endpoint="/api/eval/run/entries",
+                input_json=output_request.model_dump(mode="json"))
 
-        return response
+            if res.status_code != 200:
+                logging.error(
+                    "Error uploading inference outputs for experiment_id: %s",
+                    experiment_id)
+                return
+
+        logging.info(
+            "Eval run started successfully."
+            "Visit %s to view results.", self.ui_url)
 
     def flush(self):
         """Flush the log entries and run evals on them.
         Currently only Groundedness evals are run on the log entries.
 
         Returns: The HTTP response on success or raises an HTTPError on failure.
         """
@@ -200,33 +215,30 @@
         if not has_entries_to_flush:
             logging.info("No log entries to flush.")
             return
 
         for tag, log_entries in self.tag_to_log_entries.items():
             log_request = LogRequest(
                 log_entries=log_entries,
-                experiment_id_prefix=(
-                    tag if tag != DEFAULT_TAG_NAME else None))
+                experiment_id_prefix=(tag if tag != DEFAULT_TAG_NAME else None))
             response = self.__make_request(
                 method="put",
                 endpoint="/api/eval/log",
                 input_json=log_request.model_dump(mode="json"))
 
             if response.status_code == 200:
                 logging.info(
                     "Log entries flushed successfully for %s tag."
-                    " Visit %s to view results.",
-                    tag, self.ui_url)
+                    " Visit %s to view results.", tag, self.ui_url)
                 # Clear log entries after flushing
                 log_entries.clear()
             else:
                 logging.error(
                     "Flushing log entries failed with response code: %s",
-                    response.status_code
-                )
+                    response.status_code)
 
         return response
 
     def log(self,
             query: str,
             response: str,
             contexts: list[str],
@@ -244,16 +256,16 @@
             response: The response from your AI system.
             contexts: List of contexts relevant to the query.
             tag: An optional tag for the request. e.g. "great-model-v01".
                 This will be prepended to the name of the eval run
                 (experiment_id). The complete eval run experiment_id will be
                 of the form: "great-model-v01_logs_groundedness_YYYYMMDD"
         """
-        inference_output = InferenceOutput(
-            generated_response=response, contexts=contexts)
+        inference_output = InferenceOutput(generated_response=response,
+                                           contexts=contexts)
         log_entry = LogTuple(query=query, inference_output=inference_output)
         tag = tag if tag else DEFAULT_TAG_NAME
         entries_for_tag = self.tag_to_log_entries[tag]
         entries_for_tag.append(log_entry)
         if len(entries_for_tag) >= self.max_entries_before_auto_flush:
             # Auto flush if the number of entries for any tag is greater than a
             # certain threshold.
```

### Comparing `fore-0.1.6/fore/foresight/client_test.py` & `fore-0.1.7/fore/foresight/client_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 import unittest
 from typing import Any, Dict
 from unittest.mock import MagicMock, call, patch
 
 import pandas as pd
 
 from fore.foresight.client import Foresight
-from fore.foresight.schema import (EvalRunConfig, EvalRunDetails, EvalsetMetadata,
-                                   InferenceOutput, LogTuple, MetricType)
+from fore.foresight.schema import (EvalRunConfig, EvalRunDetails,
+                                   EvalsetMetadata, InferenceOutput, LogTuple,
+                                   MetricType)
 
 TEST_TOKEN = "VERY_SECRET_TOKEN"
 TEST_URL = "http://foresight:8010"
 TEST_TIMEOUT = 1
 MAX_ENTRIES_BEFORE_FLUSH = 2
 
 
 class TestForeSight(unittest.TestCase):
     """Tests for the client class."""
 
     def setUp(self):
         self.client = Foresight(
-            api_token=TEST_TOKEN, api_url=TEST_URL,
+            api_token=TEST_TOKEN,
+            api_url=TEST_URL,
             max_entries_before_auto_flush=MAX_ENTRIES_BEFORE_FLUSH)
         self.client.timeout_seconds = TEST_TIMEOUT
 
     @patch("uuid.uuid4")
     @patch("requests.request")
     def test_create_simple_evalset(self, mock_request, mock_uuid):
         mock_response = MagicMock()
@@ -61,16 +63,16 @@
             },
             timeout=TEST_TIMEOUT)
 
         assert isinstance(result, EvalsetMetadata)
 
     @patch("uuid.uuid4")
     @patch("requests.request")
-    def test_create_simple_evalset_with_references(
-            self, mock_request, mock_uuid):
+    def test_create_simple_evalset_with_references(self, mock_request,
+                                                   mock_uuid):
         mock_response = MagicMock()
         mock_response.json.return_value = {
             "evalset_id": "my_evalset",
             "num_entries": 2
         }
 
         mock_request.return_value = mock_response
@@ -201,14 +203,18 @@
     @patch("requests.request")
     def test_generate_answers_and_run_eval(self, mock_request):
 
         def generate_fn(query: str) -> InferenceOutput:
             return InferenceOutput(generated_response=query.upper(),
                                    contexts=[])
 
+        mock_response = MagicMock()
+        mock_response.status_code = 200
+        mock_request.return_value = mock_response
+
         self.client.generate_answers_and_run_eval(
             generate_fn=generate_fn,
             run_config=EvalRunConfig(experiment_id="my_experiment",
                                      evalset_id="my_evalset",
                                      metrics=[
                                          MetricType.RELEVANCE,
                                          MetricType.COMPLETENESS,
@@ -236,14 +242,75 @@
                         "debug_info": None,
                         "source_docids": None,
                     }
                 }
             },
             timeout=TEST_TIMEOUT)
 
+    @patch("fore.foresight.client.Foresight.get_evalrun_queries",
+           mock_get_evalrun_queries)
+    @patch("requests.request")
+    def test_generate_answers_and_run_eval_batched(self, mock_request):
+
+        def generate_fn(query: str) -> InferenceOutput:
+            return InferenceOutput(generated_response=query.upper(),
+                                   contexts=[])
+
+        mock_response = MagicMock()
+        mock_response.status_code = 200
+        mock_request.return_value = mock_response
+
+        self.client.generate_answers_and_run_eval(
+            generate_fn=generate_fn,
+            run_config=EvalRunConfig(experiment_id="my_experiment",
+                                     evalset_id="my_evalset",
+                                     metrics=[
+                                         MetricType.RELEVANCE,
+                                         MetricType.COMPLETENESS,
+                                         MetricType.GROUNDEDNESS,
+                                     ],
+                                     metadata={"my_key": "my_value"}),
+            batch_size=1)
+
+        # Skip the first request that creates the evalrun.
+        self.assertSequenceEqual(mock_request.call_args_list[1:], [
+            call(method="put",
+                 url=f"{TEST_URL}/api/eval/run/entries",
+                 headers={"Authorization": f"Bearer {TEST_TOKEN}"},
+                 params=None,
+                 json={
+                     "experiment_id": "my_experiment",
+                     "entry_id_to_inference_output": {
+                         "entry_id1": {
+                             "generated_response": "QUERY1",
+                             "contexts": [],
+                             "debug_info": None,
+                             "source_docids": None,
+                         },
+                     }
+                 },
+                 timeout=TEST_TIMEOUT),
+            call(method="put",
+                 url=f"{TEST_URL}/api/eval/run/entries",
+                 headers={"Authorization": f"Bearer {TEST_TOKEN}"},
+                 params=None,
+                 json={
+                     "experiment_id": "my_experiment",
+                     "entry_id_to_inference_output": {
+                         "entry_id2": {
+                             "generated_response": "QUERY2",
+                             "contexts": [],
+                             "debug_info": None,
+                             "source_docids": None,
+                         }
+                     }
+                 },
+                 timeout=TEST_TIMEOUT)
+        ])
+
     @patch("requests.request")
     def test_log_adds_entries(self, mock_request):
         """Tests for adding log entries."""
         mock_response = MagicMock()
         mock_response.status_code = 200
         mock_request.return_value = mock_response
 
@@ -265,145 +332,130 @@
 
         self.client.log(query1, llm_response1, contexts1)
         self.client.log(query4, llm_response4, contexts4, tag="great_model")
         self.client.log(query2, llm_response2, contexts2)
         self.client.log(query3, llm_response3, contexts3)
 
         expected_calls = [
-            call(
-                method="put",
-                url=f"{TEST_URL}/api/eval/log",
-                headers={"Authorization": f"Bearer {TEST_TOKEN}"},
-                params=None,
-                json={
-                    "log_entries": [
-                        {
-                            "query": "test_query1",
-                            "inference_output": {
-                                "generated_response": "test_response1",
-                                "source_docids": None,
-                                "contexts": ["context1", "context2"],
-                                "debug_info": None
-                            }
-                        },
-                        {
-                            "query": "test_query2",
-                            "inference_output": {
-                                "generated_response": "test_response2",
-                                "source_docids": None,
-                                "contexts": ["context3", "context4"],
-                                "debug_info": None
-                            }
-                        }
-                    ],
-                    "experiment_id_prefix": None
-                },
-                timeout=TEST_TIMEOUT
-            ),
-            call(
-                method="put",
-                url=f"{TEST_URL}/api/eval/log",
-                headers={"Authorization": f"Bearer {TEST_TOKEN}"},
-                params=None,
-                json={
-                    "log_entries": [
-                        {
-                            "query": "test_query4",
-                            "inference_output": {
-                                "generated_response": "test_response4",
-                                "source_docids": None,
-                                "contexts": ["context7", "context8"],
-                                "debug_info": None
-                            }
-                        },
-                    ],
-                    "experiment_id_prefix": "great_model"
-                },
-                timeout=TEST_TIMEOUT
-            )
+            call(method="put",
+                 url=f"{TEST_URL}/api/eval/log",
+                 headers={"Authorization": f"Bearer {TEST_TOKEN}"},
+                 params=None,
+                 json={
+                     "log_entries": [{
+                         "query": "test_query1",
+                         "inference_output": {
+                             "generated_response": "test_response1",
+                             "source_docids": None,
+                             "contexts": ["context1", "context2"],
+                             "debug_info": None
+                         }
+                     }, {
+                         "query": "test_query2",
+                         "inference_output": {
+                             "generated_response": "test_response2",
+                             "source_docids": None,
+                             "contexts": ["context3", "context4"],
+                             "debug_info": None
+                         }
+                     }],
+                     "experiment_id_prefix": None
+                 },
+                 timeout=TEST_TIMEOUT),
+            call(method="put",
+                 url=f"{TEST_URL}/api/eval/log",
+                 headers={"Authorization": f"Bearer {TEST_TOKEN}"},
+                 params=None,
+                 json={
+                     "log_entries": [{
+                         "query": "test_query4",
+                         "inference_output": {
+                             "generated_response": "test_response4",
+                             "source_docids": None,
+                             "contexts": ["context7", "context8"],
+                             "debug_info": None
+                         }
+                     },],
+                     "experiment_id_prefix": "great_model"
+                 },
+                 timeout=TEST_TIMEOUT)
         ]
 
         mock_request.assert_has_calls(expected_calls, any_order=True)
 
         self.assertEqual(len(self.client.tag_to_log_entries), 2)
         self.assertDictEqual(
-            self.client.tag_to_log_entries,
-            {"default":
-             [
-                 LogTuple(
-                query="test_query3",
-                inference_output=InferenceOutput(
-                    generated_response="test_response3",
-                    contexts=["context5", "context6"]))
-             ],
-             "great_model": []})
+            self.client.tag_to_log_entries, {
+                "default": [
+                    LogTuple(query="test_query3",
+                             inference_output=InferenceOutput(
+                                 generated_response="test_response3",
+                                 contexts=["context5", "context6"]))
+                ],
+                "great_model": []
+            })
 
     @patch("requests.request")
     def test_flush_sends_request_and_clears_entries(self, mock_request):
         """Tests for flushing log entries."""
         mock_response = MagicMock()
         mock_response.status_code = 200
         mock_request.return_value = mock_response
 
         # Add some log entries and flush
         self.client.log("test_query1", "test_response1", ["context1"])
         response1 = self.client.flush()
-        self.client.log("test_query2", "test_response2",
-                        ["context2"], tag="great_model")
+        self.client.log("test_query2",
+                        "test_response2", ["context2"],
+                        tag="great_model")
         response2 = self.client.flush()
         expected_calls = [
-            call(
-                method="put",
-                url=f"{TEST_URL}/api/eval/log",
-                headers={"Authorization": f"Bearer {TEST_TOKEN}"},
-                params=None,
-                json={
-                    "log_entries": [
-                        {
-                            "query": "test_query1",
-                            "inference_output": {
-                                "generated_response": "test_response1",
-                                "source_docids": None,
-                                "contexts": ["context1"],
-                                "debug_info": None
-                            }
-                        }
-                    ],
-                    "experiment_id_prefix": None
-                },
-                timeout=TEST_TIMEOUT
-            ),
-            call(
-                method="put",
-                url=f"{TEST_URL}/api/eval/log",
-                headers={"Authorization": f"Bearer {TEST_TOKEN}"},
-                params=None,
-                json={
-                    "log_entries": [
-                        {
-                            "query": "test_query2",
-                            "inference_output": {
-                                "generated_response": "test_response2",
-                                "source_docids": None,
-                                "contexts": ["context2"],
-                                "debug_info": None
-                            }
-                        },
-                    ],
-                    "experiment_id_prefix": "great_model"
-                },
-                timeout=TEST_TIMEOUT
-            )
+            call(method="put",
+                 url=f"{TEST_URL}/api/eval/log",
+                 headers={"Authorization": f"Bearer {TEST_TOKEN}"},
+                 params=None,
+                 json={
+                     "log_entries": [{
+                         "query": "test_query1",
+                         "inference_output": {
+                             "generated_response": "test_response1",
+                             "source_docids": None,
+                             "contexts": ["context1"],
+                             "debug_info": None
+                         }
+                     }],
+                     "experiment_id_prefix": None
+                 },
+                 timeout=TEST_TIMEOUT),
+            call(method="put",
+                 url=f"{TEST_URL}/api/eval/log",
+                 headers={"Authorization": f"Bearer {TEST_TOKEN}"},
+                 params=None,
+                 json={
+                     "log_entries": [{
+                         "query": "test_query2",
+                         "inference_output": {
+                             "generated_response": "test_response2",
+                             "source_docids": None,
+                             "contexts": ["context2"],
+                             "debug_info": None
+                         }
+                     },],
+                     "experiment_id_prefix": "great_model"
+                 },
+                 timeout=TEST_TIMEOUT)
         ]
 
         mock_request.assert_has_calls(expected_calls, any_order=True)
 
         # Assert that log_entries is empty after flushing
-        self.assertDictEqual(
-            self.client.tag_to_log_entries, {"default": [], "great_model": []})
+        self.assertDictEqual(self.client.tag_to_log_entries, {
+            "default": [],
+            "great_model": []
+        })
 
         # Assert the response from flush
         self.assertEqual(response1.status_code, 200)
         self.assertEqual(response2.status_code, 200)
 
     @staticmethod
     def get_evalrun_details_sample(
```

### Comparing `fore-0.1.6/fore/foresight/schema.py` & `fore-0.1.7/fore/foresight/schema.py`

 * *Files identical despite different names*

### Comparing `fore-0.1.6/fore.egg-info/PKG-INFO` & `fore-0.1.7/fore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fore
-Version: 0.1.6
+Version: 0.1.7
 Summary: fore ai packages
 Author-email: fore ai <info@foreai.co>
 Maintainer-email: fore ai <info@foreai.co>
 License: Apache 2.0 License
 Project-URL: Homepage, https://foreai.co
 Project-URL: Repository, https://github.com/foreai-co/fore
 Project-URL: Issues, https://github.com/foreai-co/fore/issues
```

### Comparing `fore-0.1.6/pyproject.toml` & `fore-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fore"
-version = "0.1.6"
+version = "0.1.7"
 readme = "README.md"
 authors = [
     { name = "fore ai", email = "info@foreai.co" }
 ]
 description = "fore ai packages"
 requires-python = ">= 3.8"
 maintainers = [
```

