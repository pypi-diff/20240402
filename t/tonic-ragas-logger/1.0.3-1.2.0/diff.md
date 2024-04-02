# Comparing `tmp/tonic_ragas_logger-1.0.3.tar.gz` & `tmp/tonic_ragas_logger-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic_ragas_logger-1.0.3.tar", max compression
+gzip compressed data, was "tonic_ragas_logger-1.2.0.tar", max compression
```

## Comparing `tonic_ragas_logger-1.0.3.tar` & `tonic_ragas_logger-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2024-02-26 20:50:08.095783 tonic_ragas_logger-1.0.3/LICENSE
--rw-r--r--   0        0        0     2463 2024-02-26 20:50:08.095783 tonic_ragas_logger-1.0.3/README.md
--rw-r--r--   0        0        0      448 2024-02-26 20:50:08.099783 tonic_ragas_logger-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       81 2024-02-26 20:50:08.099783 tonic_ragas_logger-1.0.3/tonic_ragas_logger/__init__.py
--rw-r--r--   0        0        0      343 2024-02-26 20:50:08.099783 tonic_ragas_logger-1.0.3/tonic_ragas_logger/config.py
--rw-r--r--   0        0        0     4150 2024-02-26 20:50:08.099783 tonic_ragas_logger-1.0.3/tonic_ragas_logger/ragas_validate_api.py
--rw-r--r--   0        0        0        0 2024-02-26 20:50:08.099783 tonic_ragas_logger-1.0.3/tonic_ragas_logger/utils/__init__.py
--rw-r--r--   0        0        0     2880 2024-02-26 20:50:08.099783 tonic_ragas_logger-1.0.3/tonic_ragas_logger/utils/http_client.py
--rw-r--r--   0        0        0     3036 1970-01-01 00:00:00.000000 tonic_ragas_logger-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-02 20:17:54.022697 tonic_ragas_logger-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2463 2024-04-02 20:17:54.022697 tonic_ragas_logger-1.2.0/README.md
+-rw-r--r--   0        0        0      448 2024-04-02 20:17:54.022697 tonic_ragas_logger-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-04-02 20:17:54.026697 tonic_ragas_logger-1.2.0/tonic_ragas_logger/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-02 20:17:54.026697 tonic_ragas_logger-1.2.0/tonic_ragas_logger/config.py
+-rw-r--r--   0        0        0     4027 2024-04-02 20:17:54.026697 tonic_ragas_logger-1.2.0/tonic_ragas_logger/ragas_validate_api.py
+-rw-r--r--   0        0        0        0 2024-04-02 20:17:54.026697 tonic_ragas_logger-1.2.0/tonic_ragas_logger/utils/__init__.py
+-rw-r--r--   0        0        0     2880 2024-04-02 20:17:54.026697 tonic_ragas_logger-1.2.0/tonic_ragas_logger/utils/http_client.py
+-rw-r--r--   0        0        0     3036 1970-01-01 00:00:00.000000 tonic_ragas_logger-1.2.0/PKG-INFO
```

### Comparing `tonic_ragas_logger-1.0.3/LICENSE` & `tonic_ragas_logger-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tonic_ragas_logger-1.0.3/README.md` & `tonic_ragas_logger-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tonic_ragas_logger-1.0.3/tonic_ragas_logger/ragas_validate_api.py` & `tonic_ragas_logger-1.2.0/tonic_ragas_logger/ragas_validate_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Dict
+from typing import Any, List, Optional, Dict
 
 from tonic_validate import Run, RunData
 from tonic_ragas_logger.config import Config
 
 from tonic_ragas_logger.utils.http_client import HttpClient
 from ragas.evaluation import Result
 
@@ -29,56 +29,55 @@
                     "No api key provided. Please provide an api key or set "
                     "TONIC_VALIDATE_API_KEY environment variable."
                 )
                 raise Exception(exception_message)
         self.client = HttpClient(self.config.TONIC_VALIDATE_BASE_URL, api_key)
 
     def upload_results(
-        self, project_id: str, results: Result, run_metadata: Dict[str, str] = {}
+        self,
+        project_id: str,
+        results: Result,
+        run_metadata: Dict[str, Any] = {},
+        tags: List[str] = [],
     ) -> str:
         """Uploads results to a Tonic Validate project.
 
         Parameters
         ----------
         project_id : str
             The ID of the project to upload the run to.
         results : Result
             The result to upload.
         run_metadata : Dict[str, str]
             Metadata to attach to the run. If the values are not strings, then they are
             converted to strings before making the request.
         """
-        # ensure run_metadata is Dict[str, str]
-        processed_run_metadata = {
-            str(key): str(value) for key, value in run_metadata.items()
-        }
-        run_response = self.client.http_post(f"/projects/{project_id}/runs")
-        run_response = self.client.http_put(
-            f"/projects/{project_id}/runs/{run_response['id']}",
-            data={"run_metadata": processed_run_metadata},
-        )
         run = self.__convert_to_run(results)
-        for run_data in run.run_data:
-            _ = self.client.http_post(
-                f"/projects/{project_id}/runs/{run_response['id']}/logs",
-                data=run_data.to_dict(),
-            )
+        run_response = self.client.http_post(
+            f"/projects/{project_id}/runs/with_data",
+            data={
+                "run_metadata": run_metadata,
+                "tags": tags,
+                "data": [run_data.to_dict() for run_data in run.run_data],
+            },
+        )
         return run_response["id"]
 
     def __convert_to_run(self, results: Result) -> Run:
         """Converts a Result to a Run.
 
         Parameters
         ----------
         results : Result
             The result to convert.
         """
         try:
             overall_scores = {
-                str(score): float(value) for score, value in results.items()
+                str(score): 0 if value is None else float(value)
+                for score, value in results.items()
             }
         except ValueError:
             raise ValueError(
                 "The scores in the results are in the format of {score: value} where score is a string and value is a float."
             )
 
         if not results.dataset:
@@ -91,15 +90,15 @@
                 "The length of results.scores and results.dataset are not the same"
             )
 
         run_data = []
         for i in range(len(results.scores)):
             try:
                 scores: Dict[str, float | None] = {
-                    str(score): float(value)
+                    str(score): 0 if value is None else float(value)
                     for score, value in results.scores[i].items()
                 }
             except ValueError:
                 raise ValueError(
                     "The scores in the results are in the format of {score: value} where score is a string and value is a float."
                 )
             run_data.append(
@@ -108,8 +107,13 @@
                     reference_question=results.dataset["question"][i],
                     reference_answer=results.dataset["ground_truth"][i],
                     llm_answer=results.dataset["answer"][i],
                     llm_context=results.dataset["contexts"][i],
                 )
             )
 
-        return Run(overall_scores=overall_scores, run_data=run_data, id=None)
+        return Run(
+            overall_scores=overall_scores,
+            run_data=run_data,
+            llm_evaluator=None,
+            id=None,
+        )
```

### Comparing `tonic_ragas_logger-1.0.3/tonic_ragas_logger/utils/http_client.py` & `tonic_ragas_logger-1.2.0/tonic_ragas_logger/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `tonic_ragas_logger-1.0.3/PKG-INFO` & `tonic_ragas_logger-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: tonic-ragas-logger
-Version: 1.0.3
+Version: 1.2.0
 Summary: Uploads results from ragas to Tonic Validate.
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: ragas (>=0.1.2,<0.2.0)
-Requires-Dist: tonic-validate (>=3.2.0,<4.0.0)
+Requires-Dist: tonic-validate (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Tonic Validate Ragas Logger
  
 The Tonic Validate Ragas Logger is a tool to upload your results from Ragas to the Tonic Validate UI for visualization. The UI is completely free to use.
 
 <picture>
```

