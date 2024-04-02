# Comparing `tmp/braintrust-0.0.98.tar.gz` & `tmp/braintrust-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braintrust-0.0.98.tar", last modified: Thu Feb 15 22:33:50 2024, max compression
+gzip compressed data, was "braintrust-0.0.99.tar", last modified: Tue Feb 20 23:16:33 2024, max compression
```

## Comparing `braintrust-0.0.98.tar` & `braintrust-0.0.99.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 manu       (501) staff       (20)        0 2024-02-15 22:33:50.589360 braintrust-0.0.98/
--rw-r--r--   0 manu       (501) staff       (20)     2399 2024-02-15 22:33:50.589133 braintrust-0.0.98/PKG-INFO
--rw-r--r--   0 manu       (501) staff       (20)      882 2024-02-06 04:57:28.000000 braintrust-0.0.98/README.md
--rw-r--r--   0 manu       (501) staff       (20)       38 2024-02-15 22:33:50.589397 braintrust-0.0.98/setup.cfg
--rw-r--r--   0 manu       (501) staff       (20)     1638 2024-02-15 22:33:48.000000 braintrust-0.0.98/setup.py
-drwxr-xr-x   0 manu       (501) staff       (20)        0 2024-02-15 22:33:50.582758 braintrust-0.0.98/src/
-drwxr-xr-x   0 manu       (501) staff       (20)        0 2024-02-15 22:33:50.586007 braintrust-0.0.98/src/braintrust/
--rw-r--r--   0 manu       (501) staff       (20)     1020 2024-02-06 04:57:28.000000 braintrust-0.0.98/src/braintrust/__init__.py
--rw-r--r--   0 manu       (501) staff       (20)      427 2024-02-06 04:57:28.000000 braintrust-0.0.98/src/braintrust/aws.py
--rw-r--r--   0 manu       (501) staff       (20)      170 2024-02-06 04:57:28.000000 braintrust-0.0.98/src/braintrust/cache.py
-drwxr-xr-x   0 manu       (501) staff       (20)        0 2024-02-15 22:33:50.587136 braintrust-0.0.98/src/braintrust/cli/
--rw-r--r--   0 manu       (501) staff       (20)        0 2024-02-06 04:57:28.000000 braintrust-0.0.98/src/braintrust/cli/__init__.py
--rw-r--r--   0 manu       (501) staff       (20)     1347 2024-02-06 04:57:28.000000 braintrust-0.0.98/src/braintrust/cli/__main__.py
--rw-r--r--   0 manu       (501) staff       (20)     8275 2024-02-09 19:38:45.000000 braintrust-0.0.98/src/braintrust/cli/eval.py
-drwxr-xr-x   0 manu       (501) staff       (20)        0 2024-02-15 22:33:50.587875 braintrust-0.0.98/src/braintrust/cli/install/
--rw-r--r--   0 manu       (501) staff       (20)     1289 2024-02-06 04:57:28.000000 braintrust-0.0.98/src/braintrust/cli/install/__init__.py
--rw-r--r--   0 manu       (501) staff       (20)     7801 2024-02-06 04:57:28.000000 braintrust-0.0.98/src/braintrust/cli/install/api.py
--rw-r--r--   0 manu       (501) staff       (20)     2723 2024-02-06 04:57:28.000000 braintrust-0.0.98/src/braintrust/cli/install/logs.py
--rw-r--r--   0 manu       (501) staff       (20)     6800 2024-02-06 04:57:28.000000 braintrust-0.0.98/src/braintrust/cli/install/redshift.py
--rw-r--r--   0 manu       (501) staff       (20)    21810 2024-02-09 19:38:45.000000 braintrust-0.0.98/src/braintrust/framework.py
--rw-r--r--   0 manu       (501) staff       (20)     5319 2024-02-15 05:51:04.000000 braintrust-0.0.98/src/braintrust/gitutil.py
--rw-r--r--   0 manu       (501) staff       (20)    89595 2024-02-15 22:30:17.000000 braintrust-0.0.98/src/braintrust/logger.py
--rw-r--r--   0 manu       (501) staff       (20)    10269 2024-02-09 19:38:45.000000 braintrust-0.0.98/src/braintrust/oai.py
--rw-r--r--   0 manu       (501) staff       (20)      723 2024-02-06 04:57:28.000000 braintrust-0.0.98/src/braintrust/resource_manager.py
--rw-r--r--   0 manu       (501) staff       (20)     2211 2024-02-15 22:30:18.000000 braintrust-0.0.98/src/braintrust/util.py
--rw-r--r--   0 manu       (501) staff       (20)       19 2024-02-15 22:32:22.000000 braintrust-0.0.98/src/braintrust/version.py
-drwxr-xr-x   0 manu       (501) staff       (20)        0 2024-02-15 22:33:50.588086 braintrust-0.0.98/src/braintrust.egg-info/
--rw-r--r--   0 manu       (501) staff       (20)     2399 2024-02-15 22:33:50.000000 braintrust-0.0.98/src/braintrust.egg-info/PKG-INFO
--rw-r--r--   0 manu       (501) staff       (20)      742 2024-02-15 22:33:50.000000 braintrust-0.0.98/src/braintrust.egg-info/SOURCES.txt
--rw-r--r--   0 manu       (501) staff       (20)        1 2024-02-15 22:33:50.000000 braintrust-0.0.98/src/braintrust.egg-info/dependency_links.txt
--rw-r--r--   0 manu       (501) staff       (20)       60 2024-02-15 22:33:50.000000 braintrust-0.0.98/src/braintrust.egg-info/entry_points.txt
--rw-r--r--   0 manu       (501) staff       (20)      306 2024-02-15 22:33:50.000000 braintrust-0.0.98/src/braintrust.egg-info/requires.txt
--rw-r--r--   0 manu       (501) staff       (20)       11 2024-02-15 22:33:50.000000 braintrust-0.0.98/src/braintrust.egg-info/top_level.txt
+drwxr-xr-x   0 manu       (501) staff       (20)        0 2024-02-20 23:16:33.589513 braintrust-0.0.99/
+-rw-r--r--   0 manu       (501) staff       (20)     2436 2024-02-20 23:16:33.589269 braintrust-0.0.99/PKG-INFO
+-rw-r--r--   0 manu       (501) staff       (20)      882 2024-02-06 04:57:28.000000 braintrust-0.0.99/README.md
+-rw-r--r--   0 manu       (501) staff       (20)       38 2024-02-20 23:16:33.589568 braintrust-0.0.99/setup.cfg
+-rw-r--r--   0 manu       (501) staff       (20)     1663 2024-02-20 23:16:31.000000 braintrust-0.0.99/setup.py
+drwxr-xr-x   0 manu       (501) staff       (20)        0 2024-02-20 23:16:33.583637 braintrust-0.0.99/src/
+drwxr-xr-x   0 manu       (501) staff       (20)        0 2024-02-20 23:16:33.586436 braintrust-0.0.99/src/braintrust/
+-rw-r--r--   0 manu       (501) staff       (20)     1020 2024-02-06 04:57:28.000000 braintrust-0.0.99/src/braintrust/__init__.py
+-rw-r--r--   0 manu       (501) staff       (20)      427 2024-02-06 04:57:28.000000 braintrust-0.0.99/src/braintrust/aws.py
+-rw-r--r--   0 manu       (501) staff       (20)      170 2024-02-06 04:57:28.000000 braintrust-0.0.99/src/braintrust/cache.py
+drwxr-xr-x   0 manu       (501) staff       (20)        0 2024-02-20 23:16:33.587419 braintrust-0.0.99/src/braintrust/cli/
+-rw-r--r--   0 manu       (501) staff       (20)        0 2024-02-06 04:57:28.000000 braintrust-0.0.99/src/braintrust/cli/__init__.py
+-rw-r--r--   0 manu       (501) staff       (20)     1347 2024-02-06 04:57:28.000000 braintrust-0.0.99/src/braintrust/cli/__main__.py
+-rw-r--r--   0 manu       (501) staff       (20)     8275 2024-02-17 00:16:30.000000 braintrust-0.0.99/src/braintrust/cli/eval.py
+drwxr-xr-x   0 manu       (501) staff       (20)        0 2024-02-20 23:16:33.588093 braintrust-0.0.99/src/braintrust/cli/install/
+-rw-r--r--   0 manu       (501) staff       (20)     1289 2024-02-06 04:57:28.000000 braintrust-0.0.99/src/braintrust/cli/install/__init__.py
+-rw-r--r--   0 manu       (501) staff       (20)     7801 2024-02-06 04:57:28.000000 braintrust-0.0.99/src/braintrust/cli/install/api.py
+-rw-r--r--   0 manu       (501) staff       (20)     2723 2024-02-06 04:57:28.000000 braintrust-0.0.99/src/braintrust/cli/install/logs.py
+-rw-r--r--   0 manu       (501) staff       (20)     6800 2024-02-06 04:57:28.000000 braintrust-0.0.99/src/braintrust/cli/install/redshift.py
+-rw-r--r--   0 manu       (501) staff       (20)    22866 2024-02-19 17:11:30.000000 braintrust-0.0.99/src/braintrust/framework.py
+-rw-r--r--   0 manu       (501) staff       (20)     5319 2024-02-15 05:51:04.000000 braintrust-0.0.99/src/braintrust/gitutil.py
+-rw-r--r--   0 manu       (501) staff       (20)    91130 2024-02-20 23:14:01.000000 braintrust-0.0.99/src/braintrust/logger.py
+-rw-r--r--   0 manu       (501) staff       (20)    10269 2024-02-09 19:38:45.000000 braintrust-0.0.99/src/braintrust/oai.py
+-rw-r--r--   0 manu       (501) staff       (20)      723 2024-02-06 04:57:28.000000 braintrust-0.0.99/src/braintrust/resource_manager.py
+-rw-r--r--   0 manu       (501) staff       (20)     2211 2024-02-15 22:30:18.000000 braintrust-0.0.99/src/braintrust/util.py
+-rw-r--r--   0 manu       (501) staff       (20)       19 2024-02-20 23:14:44.000000 braintrust-0.0.99/src/braintrust/version.py
+drwxr-xr-x   0 manu       (501) staff       (20)        0 2024-02-20 23:16:33.588276 braintrust-0.0.99/src/braintrust.egg-info/
+-rw-r--r--   0 manu       (501) staff       (20)     2436 2024-02-20 23:16:33.000000 braintrust-0.0.99/src/braintrust.egg-info/PKG-INFO
+-rw-r--r--   0 manu       (501) staff       (20)      742 2024-02-20 23:16:33.000000 braintrust-0.0.99/src/braintrust.egg-info/SOURCES.txt
+-rw-r--r--   0 manu       (501) staff       (20)        1 2024-02-20 23:16:33.000000 braintrust-0.0.99/src/braintrust.egg-info/dependency_links.txt
+-rw-r--r--   0 manu       (501) staff       (20)       60 2024-02-20 23:16:33.000000 braintrust-0.0.99/src/braintrust.egg-info/entry_points.txt
+-rw-r--r--   0 manu       (501) staff       (20)      328 2024-02-20 23:16:33.000000 braintrust-0.0.99/src/braintrust.egg-info/requires.txt
+-rw-r--r--   0 manu       (501) staff       (20)       11 2024-02-20 23:16:33.000000 braintrust-0.0.99/src/braintrust.egg-info/top_level.txt
```

### Comparing `braintrust-0.0.98/PKG-INFO` & `braintrust-0.0.99/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: braintrust
-Version: 0.0.98
+Version: 0.0.99
 Summary: SDK for integrating Braintrust
 Home-page: https://www.braintrustdata.com
 Author: Braintrust
 Author-email: info@braintrustdata.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: GitPython
 Requires-Dist: requests
-Requires-Dist: braintrust_core>=0.0.16
+Requires-Dist: braintrust_core>=0.0.17
 Requires-Dist: tqdm
+Requires-Dist: exceptiongroup==1.2.0
 Provides-Extra: cli
 Requires-Dist: boto3; extra == "cli"
 Requires-Dist: psycopg2-binary; extra == "cli"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
```

### Comparing `braintrust-0.0.98/README.md` & `braintrust-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.98/setup.py` & `braintrust-0.0.99/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 version_contents = {}
 with open(os.path.join(dir_name, "src", "braintrust", "version.py"), encoding="utf-8") as f:
     exec(f.read(), version_contents)
 
 with open(os.path.join(dir_name, "README.md"), "r", encoding="utf-8") as f:
     long_description = f.read()
 
-install_requires = ["GitPython", "requests", "braintrust_core>=0.0.16", "tqdm"]
+install_requires = ["GitPython", "requests", "braintrust_core>=0.0.17", "tqdm", "exceptiongroup==1.2.0"]
 
 extras_require = {
     "cli": ["boto3", "psycopg2-binary"],
     "dev": [
         "black",
         "build",
         "flake8",
```

### Comparing `braintrust-0.0.98/src/braintrust/__init__.py` & `braintrust-0.0.99/src/braintrust/__init__.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.98/src/braintrust/cli/__main__.py` & `braintrust-0.0.99/src/braintrust/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.98/src/braintrust/cli/eval.py` & `braintrust-0.0.99/src/braintrust/cli/eval.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.98/src/braintrust/cli/install/__init__.py` & `braintrust-0.0.99/src/braintrust/cli/install/__init__.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.98/src/braintrust/cli/install/api.py` & `braintrust-0.0.99/src/braintrust/cli/install/api.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.98/src/braintrust/cli/install/logs.py` & `braintrust-0.0.99/src/braintrust/cli/install/logs.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.98/src/braintrust/cli/install/redshift.py` & `braintrust-0.0.99/src/braintrust/cli/install/redshift.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.98/src/braintrust/framework.py` & `braintrust-0.0.99/src/braintrust/framework.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import contextmanager
 from enum import Enum
 from multiprocessing import cpu_count
 from typing import Any, AsyncIterator, Awaitable, Callable, Dict, Iterator, List, Optional, TypeVar, Union
 
+import exceptiongroup
 from braintrust_core.score import Score, Scorer
 from braintrust_core.span_types import SpanTypeAttribute
 from braintrust_core.util import (
     SerializableDataClass,
     eprint,
 )
 from tqdm.asyncio import tqdm as async_tqdm
@@ -122,15 +123,15 @@
 
     """
     The name of the project the eval falls under.
     """
     project_name: str
 
     """
-    A name that uniquely defines this type of experiment. You do not need to change it each time the experiment runs, but you should not have other experiments in your code with the same name.
+    A name that describes the experiment. You do not need to change it each time the experiment runs.
     """
     eval_name: str
 
     """
     Returns an iterator over the evaluation dataset. Each element of the iterator should be an `EvalCase` or a dict
     with the same fields as an `EvalCase` (`input`, `expected`, `metadata`).
     """
@@ -219,15 +220,14 @@
             )
             for result in failing_results
         ]
 
         if jsonl:
             print(json.dumps({"eval_name": eval_name, "errors": errors}))
         else:
-            print(errors)
             info = "".join(errors).rstrip()
             eprint(f"{bcolors.FAIL}{info}{bcolors.ENDC}")
 
             eprint(f"{bcolors.FAIL}Add --verbose to see full stack traces.{bcolors.ENDC}")
     if summary:
         print(json.dumps(summary.as_dict()) if jsonl else f"{summary}")
     else:
@@ -298,15 +298,15 @@
     :param is_public: (Optional) Whether the experiment should be public. Defaults to false.
     :return: An `Evaluator` object.
     """
     eval_name = _make_eval_name(name, experiment_name)
 
     global _evals
     if eval_name in _evals:
-        raise ValueError(f"Evaluator {eval_name} already exists")
+        eval_name = f"{eval_name}_{len(_evals)}"
 
     evaluator = Evaluator(
         eval_name=eval_name,
         project_name=name,
         data=data,
         task=task,
         scores=scores,
@@ -449,14 +449,29 @@
     Set the maximum number of threads to use for running evaluators. By default, this is the number of
     CPUs on the machine.
     """
     with _THREAD_POOL_SINGLETON.get() as obj:
         obj.set_max_workers(max_workers)
 
 
+def _scorer_name(scorer, scorer_idx):
+    def helper():
+        if hasattr(scorer, "_name"):
+            return scorer._name()
+        elif hasattr(scorer, "__name__"):
+            return scorer.__name__
+        else:
+            return type(scorer).__name__
+
+    ret = helper()
+    if ret == "<lambda>":
+        ret = f"scorer_{scorer_idx}"
+    return ret
+
+
 async def run_evaluator(experiment, evaluator: Evaluator, position: Optional[int], filters: List[Filter]):
     #   if (typeof evaluator.data === "string") {
     #     throw new Error("Unimplemented: string data paths");
     #   }
     #   const dataResult = evaluator.data();
     #   let data = null;
     #   if (dataResult instanceof Promise) {
@@ -481,18 +496,15 @@
                         var.reset(tok)
 
             with _THREAD_POOL_SINGLETON.get() as thread_pool:
                 return await event_loop.run_in_executor(
                     thread_pool.thread_pool(), run_f, args, kwargs, contextvars.copy_context()
                 )
 
-    async def await_or_run_scorer(root_span, scorer, scorer_idx, **kwargs):
-        name = scorer._name() if hasattr(scorer, "_name") else scorer.__name__
-        if name == "<lambda>":
-            name = f"scorer_{scorer_idx}"
+    async def await_or_run_scorer(root_span, scorer, name, **kwargs):
         with root_span.start_span(
             name=name, span_attributes={"type": SpanTypeAttribute.SCORE}, input=dict(**kwargs)
         ) as span:
             score = scorer.eval_async if isinstance(scorer, Scorer) else scorer
 
             scorer_args = kwargs
 
@@ -542,35 +554,52 @@
                 root_span.log(output=output)
 
                 # First, resolve the scorers if they are classes
                 scorers = [
                     scorer() if inspect.isclass(scorer) and issubclass(scorer, Scorer) else scorer
                     for scorer in evaluator.scores
                 ]
+                scorer_names = [_scorer_name(scorer, i) for i, scorer in enumerate(scorers)]
                 score_promises = [
-                    asyncio.create_task(await_or_run_scorer(root_span, score, idx, **datum.as_dict(), output=output))
-                    for idx, score in enumerate(scorers)
+                    asyncio.create_task(await_or_run_scorer(root_span, score, name, **datum.as_dict(), output=output))
+                    for score, name in zip(scorers, scorer_names)
                 ]
-                score_results = [await p for p in score_promises]
+                passing_scorers_and_results = []
+                failing_scorers_and_exceptions = []
+                for name, p in zip(scorer_names, score_promises):
+                    try:
+                        passing_scorers_and_results.append((name, await p))
+                    except Exception as e:
+                        exc_info = traceback.format_exc()
+                        failing_scorers_and_exceptions.append((name, e, exc_info))
                 score_metadata = {}
-                for scorer, score_result in zip(scorers, score_results):
+                for scorer_name, score_result in passing_scorers_and_results:
                     if not isinstance(score_result, Score):
-                        score_result = Score(name=scorer.__name__, score=score_result)
+                        score_result = Score(name=scorer_name, score=score_result)
                     scores[score_result.name] = score_result.score
                     m = {**(score_result.metadata or {})}
-                    if score_result.error is not None:
-                        m["error"] = str(score_result.error)
                     if len(m) > 0:
                         score_metadata[score_result.name] = m
 
                 if len(score_metadata) > 0:
                     hooks.meta(scores=score_metadata)
 
                 # XXX: We could probably log these as they are being produced
                 root_span.log(metadata=metadata, scores=scores)
+
+                if failing_scorers_and_exceptions:
+                    scorer_errors = {
+                        scorer_name: exc_info for scorer_name, _, exc_info in failing_scorers_and_exceptions
+                    }
+                    metadata["scorer_errors"] = scorer_errors
+                    names = ", ".join(scorer_errors.keys())
+                    exceptions = [x[1] for x in failing_scorers_and_exceptions]
+                    raise exceptiongroup.ExceptionGroup(
+                        f"Found exceptions for the following scorers: {names}", exceptions
+                    )
             except Exception as e:
                 error = e
                 # Python3.10 has a different set of arguments to format_exception than earlier versions,
                 # so just capture the stack trace here.
                 exc_info = traceback.format_exc()
 
         return EvalResult(output=output, metadata=metadata, scores=scores, error=error, exc_info=exc_info)
```

### Comparing `braintrust-0.0.98/src/braintrust/gitutil.py` & `braintrust-0.0.99/src/braintrust/gitutil.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.98/src/braintrust/logger.py` & `braintrust-0.0.99/src/braintrust/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,26 +465,26 @@
                     # old fashioned way.
                     _BackgroundLogger._submit_logs_request(items, conn, self._outfile)
 
             concurrent.futures.wait(post_promises)
 
     @staticmethod
     def _submit_logs_request(items, conn, outfile):
-        dataS = construct_logs3_data(items)
+        dataStr = construct_logs3_data(items)
         for i in range(NUM_RETRIES):
             start_time = time.time()
-            resp = conn.post("/logs3", data=dataS)
+            resp = conn.post("/logs3", data=dataStr)
             if not resp.ok:
                 legacyDataS = construct_json_array([json.dumps(make_legacy_event(json.loads(r))) for r in items])
                 resp = conn.post("/logs", data=legacyDataS)
             if resp.ok:
                 return
             retrying_text = "" if i + 1 == NUM_RETRIES else " Retrying"
             print(
-                f"log request failed. Elapsed time: {time.time() - start_time} seconds. Payload size: {len(dataS)}. Error: {resp.status_code}: {resp.text}.{retrying_text}",
+                f"log request failed. Elapsed time: {time.time() - start_time} seconds. Payload size: {len(dataStr)}. Error: {resp.status_code}: {resp.text}.{retrying_text}",
                 file=outfile,
             )
         if not resp.ok:
             print(f"log request failed after {NUM_RETRIES} retries. Dropping batch", file=outfile)
 
 
 def _ensure_object(object_type, object_id, force=False):
@@ -814,17 +814,22 @@
     with login_lock:
         if not force_login and _state.logged_in:
             # We have already logged in. If any provided login inputs disagree
             # with our existing settings, raise an Exception warning the user to
             # try again with `force_login=True`.
             def check_updated_param(varname, arg, orig):
                 if arg is not None and orig is not None and arg != orig:
-                    raise Exception(f"Re-logging in with different {varname} ({arg}) than original ({orig}). To force re-login, pass `force_login=True`")
+                    raise Exception(
+                        f"Re-logging in with different {varname} ({arg}) than original ({orig}). To force re-login, pass `force_login=True`"
+                    )
+
             check_updated_param("app_url", app_url, _state.app_url)
-            check_updated_param("api_key", HTTPConnection.sanitize_token(api_key) if api_key else None, _state.login_token)
+            check_updated_param(
+                "api_key", HTTPConnection.sanitize_token(api_key) if api_key else None, _state.login_token
+            )
             check_updated_param("org_name", org_name, _state.org_name)
             return
 
         if app_url is None:
             app_url = os.environ.get("BRAINTRUST_APP_URL", "https://www.braintrustdata.com")
 
         if api_key is None:
@@ -1252,15 +1257,15 @@
         self._fetched_data = None
 
     @property
     def version(self):
         if self._pinned_version is not None:
             return self._pinned_version
         else:
-            return max([int(record.get(TRANSACTION_ID_FIELD, 0)) for record in self._fetched_data] or [0])
+            return max([int(record.get(TRANSACTION_ID_FIELD, 0)) for record in self._refetch()] or [0])
 
 
 @dataclasses.dataclass
 class ParentExperimentIds:
     project_id: str
     experiment_id: str
 
@@ -1437,29 +1442,38 @@
         expected=None,
         scores=None,
         metadata=None,
         metrics=None,
         id=None,
         dataset_record_id=None,
         inputs=None,
+        allow_log_concurrent_with_active_span=False,
     ):
         """
         Log a single event to the experiment. The event will be batched and uploaded behind the scenes.
 
         :param input: The arguments that uniquely define a test case (an arbitrary, JSON serializable object). Later on, Braintrust will use the `input` to know whether two test cases are the same between experiments, so they should not contain experiment-specific state. A simple rule of thumb is that if you run the same experiment twice, the `input` should be identical.
         :param output: The output of your application, including post-processing (an arbitrary, JSON serializable object), that allows you to determine whether the result is correct or not. For example, in an app that generates SQL queries, the `output` should be the _result_ of the SQL query generated by the model, not the query itself, because there may be multiple valid queries that answer a single question.
         :param expected: (Optional) the ground truth value (an arbitrary, JSON serializable object) that you'd compare to `output` to determine if your `output` value is correct or not. Braintrust currently does not compare `output` to `expected` for you, since there are so many different ways to do that correctly. Instead, these values are just used to help you navigate your experiments while digging into analyses. However, we may later use these values to re-score outputs or fine-tune your models.
         :param scores: A dictionary of numeric values (between 0 and 1) to log. The scores should give you a variety of signals that help you determine how accurate the outputs are compared to what you expect and diagnose failures. For example, a summarization app might have one score that tells you how accurate the summary is, and another that measures the word similarity between the generated and grouth truth summary. The word similarity score could help you determine whether the summarization was covering similar concepts or not. You can use these scores to help you sort, filter, and compare experiments.
         :param metadata: (Optional) a dictionary with additional data about the test example, model outputs, or just about anything else that's relevant, that you can use to help find and analyze examples later. For example, you could log the `prompt`, example's `id`, or anything else that would be useful to slice/dice later. The values in `metadata` can be any JSON-serializable type, but its keys must be strings.
         :param metrics: (Optional) a dictionary of metrics to log. The following keys are populated automatically: "start", "end".
         :param id: (Optional) a unique identifier for the event. If you don't provide one, BrainTrust will generate one for you.
         :param dataset_record_id: (Optional) the id of the dataset record that this event is associated with. This field is required if and only if the experiment is associated with a dataset.
         :param inputs: (Deprecated) the same as `input` (will be removed in a future version).
+        :param allow_log_concurrent_with_active_span: (Optional) in rare cases where you need to log at the top level separately from an active span on the experiment, set this to True.
         :returns: The `id` of the logged event.
         """
+        if not allow_log_concurrent_with_active_span:
+            check_current_span = current_span()
+            if getattr(check_current_span, "parent_object", None) == self:
+                raise Exception(
+                    "Cannot run toplevel Experiment.log method while there is an active span. To log to the span, use Span.log"
+                )
+
         event = _validate_and_sanitize_experiment_log_full_args(
             dict(
                 input=input,
                 output=output,
                 expected=expected,
                 scores=scores,
                 metadata=metadata,
@@ -1513,14 +1527,15 @@
     def start_span(self, name="root", span_attributes={}, start_time=None, set_current=None, parent_id=None, **event):
         """Create a new toplevel span underneath the experiment. The name defaults to "root".
 
         See `Span.start_span` for full details
         """
 
         return SpanImpl(
+            parent_object=self,
             parent_ids=self._lazy_parent_ids(),
             bg_logger=self.bg_logger,
             name=name,
             span_attributes=span_attributes,
             start_time=start_time,
             set_current=set_current,
             parent_id=parent_id,
@@ -1653,14 +1668,15 @@
     """Primary implementation of the `Span` interface. See the `Span` interface for full details on each method.
 
     We suggest using one of the various `start_span` methods, instead of creating Spans directly. See `Span.start_span` for full details.
     """
 
     def __init__(
         self,
+        parent_object: Union["Experiment", "Logger"],
         parent_ids: LazyValue[Union[ParentExperimentIds, ParentProjectLogIds]],
         bg_logger,
         parent_span_info: Optional[ParentSpanInfo] = None,
         # This is similarly named, but semantically different than parent_span_info. parent_span_info
         # very directly populates the span_parents field of the span, whereas parent_id is the plain-old
         # id field of the parent span, and is resolved on the server, not in the SDK.
         parent_id=None,
@@ -1700,14 +1716,15 @@
             ),
             span_attributes=dict(**span_attributes, name=name, exec_counter=exec_counter),
             created=datetime.datetime.now(datetime.timezone.utc).isoformat(),
         )
         if caller_location:
             self.internal_data["context"] = caller_location
 
+        self.parent_object = parent_object
         self.parent_ids = parent_ids
 
         id = event.get("id", None)
         if id is None:
             id = str(uuid.uuid4())
         span_id = str(uuid.uuid4())
         self.row_ids = RowIds(
@@ -1778,14 +1795,15 @@
             bg_logger=self.bg_logger,
             parent_ids=self.parent_ids,
             **args,
         )
 
     def start_span(self, name=None, span_attributes={}, start_time=None, set_current=None, parent_id=None, **event):
         return SpanImpl(
+            parent_object=self.parent_object,
             parent_ids=self.parent_ids,
             bg_logger=self.bg_logger,
             parent_span_info=ParentSpanInfo(span_id=self.span_id, root_span_id=self.root_span_id),
             name=name,
             span_attributes=span_attributes,
             start_time=start_time,
             set_current=set_current,
@@ -2065,40 +2083,53 @@
     def org_id(self):
         return self._lazy_metadata.get().org_id
 
     @property
     def project(self):
         return self._lazy_metadata.get().project
 
+    @property
+    def id(self):
+        return self.project.id
+
     def _get_state(self) -> BraintrustState:
         # Ensure the login state is populated by fetching the lazy_metadata.
         self._lazy_metadata.get()
         return _state
 
     def log(
         self,
         input=None,
         output=None,
         expected=None,
         scores=None,
         metadata=None,
         metrics=None,
         id=None,
+        allow_log_concurrent_with_active_span=False,
     ):
         """
         Log a single event. The event will be batched and uploaded behind the scenes.
 
         :param input: (Optional) the arguments that uniquely define a user input(an arbitrary, JSON serializable object).
         :param output: (Optional) the output of your application, including post-processing (an arbitrary, JSON serializable object), that allows you to determine whether the result is correct or not. For example, in an app that generates SQL queries, the `output` should be the _result_ of the SQL query generated by the model, not the query itself, because there may be multiple valid queries that answer a single question.
         :param expected: (Optional) the ground truth value (an arbitrary, JSON serializable object) that you'd compare to `output` to determine if your `output` value is correct or not. Braintrust currently does not compare `output` to `expected` for you, since there are so many different ways to do that correctly. Instead, these values are just used to help you navigate while digging into analyses. However, we may later use these values to re-score outputs or fine-tune your models.
         :param scores: (Optional) a dictionary of numeric values (between 0 and 1) to log. The scores should give you a variety of signals that help you determine how accurate the outputs are compared to what you expect and diagnose failures. For example, a summarization app might have one score that tells you how accurate the summary is, and another that measures the word similarity between the generated and grouth truth summary. The word similarity score could help you determine whether the summarization was covering similar concepts or not. You can use these scores to help you sort, filter, and compare logs.
         :param metadata: (Optional) a dictionary with additional data about the test example, model outputs, or just about anything else that's relevant, that you can use to help find and analyze examples later. For example, you could log the `prompt`, example's `id`, or anything else that would be useful to slice/dice later. The values in `metadata` can be any JSON-serializable type, but its keys must be strings.
         :param metrics: (Optional) a dictionary of metrics to log. The following keys are populated automatically: "start", "end".
         :param id: (Optional) a unique identifier for the event. If you don't provide one, BrainTrust will generate one for you.
+        :param allow_log_concurrent_with_active_span: (Optional) in rare cases where you need to log at the top level separately from an active span on the logger, set this to True.
         """
+        if not allow_log_concurrent_with_active_span:
+            check_current_span = current_span()
+            if getattr(check_current_span, "parent_object", None) == self:
+                raise Exception(
+                    "Cannot run toplevel Logger.log method while there is an active span. To log to the span, use Span.log"
+                )
+
         span = self.start_span(
             start_time=self.last_start_time,
             input=input,
             output=output,
             expected=expected,
             scores=scores,
             metadata=metadata,
@@ -2155,14 +2186,15 @@
     def start_span(self, name="root", span_attributes={}, start_time=None, set_current=None, parent_id=None, **event):
         """Create a new toplevel span underneath the logger. The name parameter defaults to "root".
 
         See `Span.start_span` for full details
         """
 
         return SpanImpl(
+            parent_object=self,
             parent_ids=self._lazy_parent_ids(),
             bg_logger=self.bg_logger,
             name=name,
             span_attributes=span_attributes,
             start_time=start_time,
             set_current=set_current,
             parent_id=parent_id,
```

### Comparing `braintrust-0.0.98/src/braintrust/oai.py` & `braintrust-0.0.99/src/braintrust/oai.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.98/src/braintrust/resource_manager.py` & `braintrust-0.0.99/src/braintrust/resource_manager.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.98/src/braintrust/util.py` & `braintrust-0.0.99/src/braintrust/util.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.98/src/braintrust.egg-info/PKG-INFO` & `braintrust-0.0.99/src/braintrust.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: braintrust
-Version: 0.0.98
+Version: 0.0.99
 Summary: SDK for integrating Braintrust
 Home-page: https://www.braintrustdata.com
 Author: Braintrust
 Author-email: info@braintrustdata.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: GitPython
 Requires-Dist: requests
-Requires-Dist: braintrust_core>=0.0.16
+Requires-Dist: braintrust_core>=0.0.17
 Requires-Dist: tqdm
+Requires-Dist: exceptiongroup==1.2.0
 Provides-Extra: cli
 Requires-Dist: boto3; extra == "cli"
 Requires-Dist: psycopg2-binary; extra == "cli"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
```

### Comparing `braintrust-0.0.98/src/braintrust.egg-info/SOURCES.txt` & `braintrust-0.0.99/src/braintrust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

