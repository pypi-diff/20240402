# Comparing `tmp/nextmv-0.4.1.dev1.tar.gz` & `tmp/nextmv-0.5.0.tar.gz`

## Comparing `nextmv-0.4.1.dev1.tar` & `nextmv-0.5.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv-py.code-workspace
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/requirements.txt
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/.github/workflows/python-lint.yml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/.github/workflows/python-test.yml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/__about__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/__init__.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/base_model.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/cloud/__init__.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/cloud/acceptance_test.py
--rw-r--r--   0        0        0    24828 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/cloud/application.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/cloud/batch_experiment.py
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/cloud/client.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/cloud/input_set.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/nextroute/__init__.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/nextroute/check/__init__.py
--rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/nextroute/check/schema.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/nextroute/schema/__init__.py
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/nextroute/schema/input.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/nextroute/schema/location.py
--rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/nextroute/schema/output.py
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/nextroute/schema/stop.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/nextmv/nextroute/schema/vehicle.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/tests/__init__.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/tests/test_base_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/tests/cloud/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/tests/cloud/test_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/tests/nextroute/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/tests/nextroute/schema/__init__.py
--rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/tests/nextroute/schema/input.json
--rw-r--r--   0        0        0    25755 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/tests/nextroute/schema/output.json
--rw-r--r--   0        0        0    28915 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/tests/nextroute/schema/output_with_check.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/tests/nextroute/schema/test_input.py
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/tests/nextroute/schema/test_output.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/LICENSE
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/README.md
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/pyproject.toml
--rw-r--r--   0        0        0    15401 2020-02-02 00:00:00.000000 nextmv-0.4.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv-py.code-workspace
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextmv-0.5.0/requirements.txt
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 nextmv-0.5.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 nextmv-0.5.0/.github/workflows/python-lint.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 nextmv-0.5.0/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/__about__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/base_model.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/cloud/__init__.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/cloud/acceptance_test.py
+-rw-r--r--   0        0        0    24971 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/cloud/application.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/cloud/batch_experiment.py
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/cloud/client.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/cloud/input_set.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/__init__.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/check/__init__.py
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/check/schema.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/schema/__init__.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/schema/input.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/schema/location.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/schema/output.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/schema/stop.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/schema/vehicle.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/test_base_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/cloud/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/cloud/test_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/schema/__init__.py
+-rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/schema/input.json
+-rw-r--r--   0        0        0    25755 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/schema/output.json
+-rw-r--r--   0        0        0    28915 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/schema/output_with_check.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/schema/test_input.py
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/schema/test_output.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 nextmv-0.5.0/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 nextmv-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nextmv-0.5.0/README.md
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 nextmv-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 nextmv-0.5.0/PKG-INFO
```

### Comparing `nextmv-0.4.1.dev1/.github/workflows/publish.yml` & `nextmv-0.5.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `nextmv-0.4.1.dev1/.github/workflows/python-lint.yml` & `nextmv-0.5.0/.github/workflows/python-lint.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: python lint
 on: [push]
 jobs:
   python-lint:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10", "3.11", "3.12"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: git clone
         uses: actions/checkout@v4
 
       - name: set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
```

### Comparing `nextmv-0.4.1.dev1/.github/workflows/python-test.yml` & `nextmv-0.5.0/.github/workflows/python-test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: python test
 on: [push]
 jobs:
   python-test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10", "3.11", "3.12"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: git clone
         uses: actions/checkout@v4
 
       - name: set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
```

### Comparing `nextmv-0.4.1.dev1/nextmv/cloud/__init__.py` & `nextmv-0.5.0/nextmv/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.4.1.dev1/nextmv/cloud/acceptance_test.py` & `nextmv-0.5.0/nextmv/cloud/acceptance_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module contains definitions for acceptance tests."""
 
 from datetime import datetime
 from enum import Enum
+from typing import List
 
 from nextmv.base_model import BaseModel
 
 
 class MetricType(str, Enum):
     """Type of metric when doing a comparison."""
 
@@ -78,13 +79,13 @@
     """ID of the app that owns the acceptance test."""
     experiment_id: str
     """ID of the batch experiment underlying in the acceptance test."""
     control: ComparisonInstance
     """Control instance of the acceptance test."""
     candidate: ComparisonInstance
     """Candidate instance of the acceptance test."""
-    metrics: list[Metric]
+    metrics: List[Metric]
     """Metrics of the acceptance test."""
     created_at: datetime
     """Creation date of the acceptance test."""
     updated_at: datetime
     """Last update date of the acceptance test."""
```

### Comparing `nextmv-0.4.1.dev1/nextmv/cloud/application.py` & `nextmv-0.5.0/nextmv/cloud/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module contains the application class."""
 
 import time
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Any
+from typing import Any, Dict, List, Optional, Union
 
 from nextmv.base_model import BaseModel
 from nextmv.cloud.acceptance_test import AcceptanceTest, Metric
 from nextmv.cloud.batch_experiment import BatchExperiment, BatchExperimentMetadata, BatchExperimentRun
 from nextmv.cloud.client import Client, get_size
 from nextmv.cloud.input_set import InputSet
 
@@ -22,19 +22,19 @@
     url: str
     """URL to use for downloading the file."""
 
 
 class ErrorLog(BaseModel):
     """Error log of a run, when it was not successful."""
 
-    error: str | None = None
+    error: Optional[str] = None
     """Error message."""
-    stdout: str | None = None
+    stdout: Optional[str] = None
     """Standard output."""
-    stderr: str | None = None
+    stderr: Optional[str] = None
     """Standard error."""
 
 
 class Metadata(BaseModel):
     """Metadata of a run, whether it was successful or not."""
 
     application_id: str
@@ -96,17 +96,17 @@
     user_email: str
     """Email of the user who submitted the run."""
 
 
 class RunResult(RunInformation):
     """Result of a run, wheter it was successful or not."""
 
-    error_log: ErrorLog | None = None
+    error_log: Optional[ErrorLog] = None
     """Error log of the run. Only available if the run failed."""
-    output: dict[str, Any] | None = None
+    output: Optional[Dict[str, Any]] = None
     """Output of the run. Only available if the run succeeded."""
 
 
 class UploadURL(BaseModel):
     """Result of getting an upload URL."""
 
     upload_id: str
@@ -114,15 +114,15 @@
     upload_url: str
     """URL to use for uploading the file."""
 
 
 class Configuration(BaseModel):
     """Configuration of an instance."""
 
-    execution_class: str | None = None
+    execution_class: Optional[str] = None
     """Execution class for the instance."""
 
 
 @dataclass
 class Application:
     """An application is a published decision model that can be executed."""
 
@@ -203,15 +203,15 @@
         response = self.client.request(
             method="GET",
             endpoint=f"{self.experiments_endpoint}/inputsets/{input_set_id}",
         )
 
         return InputSet.from_dict(response.json())
 
-    def list_acceptance_tests(self) -> list[AcceptanceTest]:
+    def list_acceptance_tests(self) -> List[AcceptanceTest]:
         """
         List all acceptance tests.
 
         Returns:
             List of acceptance tests.
 
         Raises:
@@ -221,15 +221,15 @@
         response = self.client.request(
             method="GET",
             endpoint=f"{self.experiments_endpoint}/acceptance",
         )
 
         return [AcceptanceTest.from_dict(acceptance_test) for acceptance_test in response.json()]
 
-    def list_batch_experiments(self) -> list[BatchExperimentMetadata]:
+    def list_batch_experiments(self) -> List[BatchExperimentMetadata]:
         """
         List all batch experiments.
 
         Returns:
             List of batch experiments.
 
         Raises:
@@ -239,15 +239,15 @@
         response = self.client.request(
             method="GET",
             endpoint=f"{self.experiments_endpoint}/batch",
         )
 
         return [BatchExperimentMetadata.from_dict(batch_experiment) for batch_experiment in response.json()]
 
-    def list_input_sets(self) -> list[InputSet]:
+    def list_input_sets(self) -> List[InputSet]:
         """
         List all input sets.
 
         Returns:
             List of input sets.
 
         Raises:
@@ -262,18 +262,18 @@
         return [InputSet.from_dict(input_set) for input_set in response.json()]
 
     def new_acceptance_test(
         self,
         candidate_instance_id: str,
         control_instance_id: str,
         id: str,
-        metrics: list[Metric | dict[str, Any]],
+        metrics: List[Union[Metric, Dict[str, Any]]],
         name: str,
-        input_set_id: str | None = None,
-        description: str | None = None,
+        input_set_id: Optional[str] = None,
+        description: Optional[str] = None,
     ) -> AcceptanceTest:
         """
         Create a new acceptance test. The acceptance test is based on a batch
         experiment. If you already started a batch experiment, you don't need
         to provide the input_set_id parameter. In that case, the ID of the
         acceptance test and the batch experiment must be the same. If the batch
         experiment does not exist, you can provide the input_set_id parameter
@@ -337,19 +337,19 @@
 
         return AcceptanceTest.from_dict(response.json())
 
     def new_batch_experiment(
         self,
         name: str,
         input_set_id: str,
-        instance_ids: list[str],
-        description: str | None = None,
-        id: str | None = None,
-        option_sets: dict[str, Any] | None = None,
-        runs: list[BatchExperimentRun | dict[str, Any]] | None = None,
+        instance_ids: List[str],
+        description: Optional[str] = None,
+        id: Optional[str] = None,
+        option_sets: Optional[Dict[str, Any]] = None,
+        runs: Optional[List[Union[BatchExperimentRun, Dict[str, Any]]]] = None,
     ) -> str:
         """
         Create a new batch experiment.
 
         Args:
             name: Name of the batch experiment.
             input_set_id: ID of the input set to use for the experiment.
@@ -391,20 +391,20 @@
 
         return response.json()["id"]
 
     def new_input_set(
         self,
         id: str,
         name: str,
-        description: str | None = None,
-        end_time: datetime | None = None,
-        instance_id: str | None = None,
-        maximum_runs: int | None = None,
-        run_ids: list[str] | None = None,
-        start_time: datetime | None = None,
+        description: Optional[str] = None,
+        end_time: Optional[datetime] = None,
+        instance_id: Optional[str] = None,
+        maximum_runs: Optional[int] = None,
+        run_ids: Optional[List[str]] = None,
+        start_time: Optional[datetime] = None,
     ) -> InputSet:
         """
         Create a new input set.
 
         Args:
             id: ID of the input set.
             name: Name of the input set.
@@ -446,21 +446,21 @@
             payload=payload,
         )
 
         return InputSet.from_dict(response.json())
 
     def new_run(
         self,
-        input: dict[str, Any] | BaseModel = None,
-        instance_id: str | None = None,
-        name: str | None = None,
-        description: str | None = None,
-        upload_id: str | None = None,
-        options: dict[str, Any] | None = None,
-        configuration: Configuration | None = None,
+        input: Union[Dict[str, Any], BaseModel] = None,
+        instance_id: Optional[str] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        upload_id: Optional[str] = None,
+        options: Optional[Dict[str, Any]] = None,
+        configuration: Optional[Configuration] = None,
     ) -> str:
         """
         Submit an input to start a new run of the application. Returns the
         run_id of the submitted run.
 
         Args:
             input: Input to use for the run.
@@ -518,22 +518,22 @@
             query_params=query_params,
         )
 
         return response.json()["run_id"]
 
     def new_run_with_result(
         self,
-        input: dict[str, Any] | BaseModel = None,
-        instance_id: str | None = None,
-        name: str | None = None,
-        description: str | None = None,
-        upload_id: str | None = None,
-        run_options: dict[str, Any] | None = None,
+        input: Union[Dict[str, Any], BaseModel] = None,
+        instance_id: Optional[str] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        upload_id: Optional[str] = None,
+        run_options: Optional[Dict[str, Any]] = None,
         polling_options: PollingOptions = _DEFAULT_POLLING_OPTIONS,
-        configuration: Configuration | None = None,
+        configuration: Optional[Configuration] = None,
     ) -> RunResult:
         """
         Submit an input to start a new run of the application and poll for the
         result. This is a convenience method that combines the new_run and
         run_result_with_polling methods, applying polling logic to check when
         the run succeeded.
 
@@ -573,15 +573,15 @@
             run_id=run_id,
             polling_options=polling_options,
         )
 
     def run_input(
         self,
         run_id: str,
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         """
         Get the input of a run.
 
         Args:
             run_id: ID of the run.
 
         Returns:
@@ -698,15 +698,15 @@
                 f"run {run_id} did not succeed after {polling_options.max_tries} tries",
             )
 
         return self._run_result(run_id=run_id, run_information=run_information)
 
     def upload_large_input(
         self,
-        input: dict[str, Any],
+        input: Dict[str, Any],
         upload_url: UploadURL,
     ) -> None:
         """
         Upload the file located at the given path to the provided upload URL.
 
         Args:
             upload_url: Upload URL to use for uploading the file.
```

### Comparing `nextmv-0.4.1.dev1/nextmv/cloud/batch_experiment.py` & `nextmv-0.5.0/nextmv/cloud/batch_experiment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 """This module contains definitions for batch experiments."""
 
 from datetime import datetime
-from typing import Any
+from typing import Any, Dict, List, Optional
 
 from nextmv.base_model import BaseModel
 
 
 class BatchExperimentInformation(BaseModel):
     """Information about a batch experiment. This serves as a base for all the
     other batch experiment models."""
 
     name: str
     """Name of the batch experiment."""
     input_set_id: str
     """ID of the input set used for the experiment."""
-    instance_ids: list[str]
+    instance_ids: List[str]
     """List of instance IDs used for the experiment."""
 
-    description: str | None = None
+    description: Optional[str] = None
     """Description of the batch experiment."""
-    id: str | None = None
+    id: Optional[str] = None
     """ID of the batch experiment."""
 
 
 class BatchExperiment(BatchExperimentInformation):
     """A batch experiment compares two or more instances by executing all the
     inputs contained in the input set."""
 
     created_at: datetime
     """Creation date of the batch experiment."""
     status: str
     """Status of the batch experiment."""
 
-    grouped_distributional_summaries: list[dict[str, Any]] | None = None
+    grouped_distributional_summaries: Optional[List[Dict[str, Any]]] = None
     """Grouped distributional summaries of the batch experiment."""
-    option_sets: dict[str, Any] | None = None
+    option_sets: Optional[Dict[str, Any]] = None
     """Option sets used for the experiment."""
 
 
 class BatchExperimentRun(BaseModel):
     """A batch experiment run is a single execution of a batch experiment."""
 
     option_set: str
     """Option set used for the experiment."""
     input_id: str
     """ID of the input used for the experiment."""
 
-    instance_id: str | None = None
+    instance_id: Optional[str] = None
     """ID of the instance used for the experiment."""
-    version_id: str | None = None
+    version_id: Optional[str] = None
     """ID of the version used for the experiment."""
 
 
 class BatchExperimentMetadata(BatchExperimentInformation):
     """Metadata of a batch experiment."""
 
     status: str
```

### Comparing `nextmv-0.4.1.dev1/nextmv/cloud/client.py` & `nextmv-0.5.0/nextmv/cloud/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module with the client class."""
 
 import json
 import os
 from dataclasses import dataclass, field
-from typing import Any
+from typing import Any, Dict, List, Optional
 from urllib.parse import urljoin
 
 import requests
 import yaml
 from requests.adapters import HTTPAdapter, Retry
 
 _MAX_LAMBDA_PAYLOAD_SIZE: int = 500 * 1024 * 1024
@@ -19,39 +19,39 @@
     """
     Client that interacts directly with the Nextmv Cloud API. The API key will
     be searched, in order of precedence, in: the api_key arg in the
     constructor, the NEXTMV_API_KEY environment variable, the
     ~/.nextmv/config.yaml file used by the Nextmv CLI.
     """
 
-    api_key: str | None = None
+    api_key: Optional[str] = None
     """API key to use for authenticating with the Nextmv Cloud API. If not
     provided, the client will look for the NEXTMV_API_KEY environment
     variable."""
-    allowed_methods: list[str] = field(
+    allowed_methods: List[str] = field(
         default_factory=lambda: ["GET", "POST", "PUT", "DELETE"],
     )
     """Allowed HTTP methods to use for retries in requests to the Nextmv Cloud
     API."""
     backoff_factor: float = 1
     """Exponential backoff factor to use for requests to the Nextmv Cloud
     API."""
     backoff_jitter: float = 0.1
     """Jitter to use for requests to the Nextmv Cloud API when backing off."""
     backoff_max: float = 60
     """Maximum backoff time to use for requests to the Nextmv Cloud API, in
     seconds."""
     configuration_file: str = "~/.nextmv/config.yaml"
     """Path to the configuration file used by the Nextmv CLI."""
-    headers: dict[str, str] | None = None
+    headers: Optional[Dict[str, str]] = None
     """Headers to use for requests to the Nextmv Cloud API."""
     max_retries: int = 10
     """Maximum number of retries to use for requests to the Nextmv Cloud
     API."""
-    status_forcelist: list[int] = field(
+    status_forcelist: List[int] = field(
         default_factory=lambda: [429, 500, 502, 503, 504, 507, 509],
     )
     """Status codes to retry for requests to the Nextmv Cloud API."""
     timeout: float = 20
     """Timeout to use for requests to the Nextmv Cloud API."""
     url: str = "https://api.cloud.nextmv.io"
     """URL of the Nextmv Cloud API."""
@@ -99,18 +99,18 @@
 
         self._set_headers_api_key(api_key)
 
     def request(
         self,
         method: str,
         endpoint: str,
-        data: Any | None = None,
-        headers: dict[str, str] | None = None,
-        payload: dict[str, Any] | None = None,
-        query_params: dict[str, Any] | None = None,
+        data: Optional[Any] = None,
+        headers: Optional[Dict[str, str]] = None,
+        payload: Optional[Dict[str, Any]] = None,
+        query_params: Optional[Dict[str, Any]] = None,
     ) -> requests.Response:
         """
         Method to make a request to the Nextmv Cloud API.
 
         Args:
             method: HTTP method to use. Valid methods include: GET, POST.
             endpoint: Endpoint to send the request to.
@@ -185,12 +185,12 @@
 
         self.headers = {
             "Authorization": f"Bearer {api_key}",
             "Content-Type": "application/json",
         }
 
 
-def get_size(obj: dict[str, Any]) -> int:
+def get_size(obj: Dict[str, Any]) -> int:
     """Finds the size of an object in bytes."""
 
     obj_str = json.dumps(obj, separators=(",", ":"))
     return len(obj_str.encode("utf-8"))
```

### Comparing `nextmv-0.4.1.dev1/nextmv/nextroute/check/__init__.py` & `nextmv-0.5.0/nextmv/nextroute/check/__init__.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.4.1.dev1/nextmv/nextroute/schema/__init__.py` & `nextmv-0.5.0/nextmv/nextroute/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.4.1.dev1/nextmv/nextroute/schema/input.py` & `nextmv-0.5.0/nextmv/nextroute/schema/input.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 """Defines the input class."""
 
-from typing import Any
+from typing import Any, List, Optional
 
 from nextmv.base_model import BaseModel
 from nextmv.nextroute.schema.stop import AlternateStop, Stop, StopDefaults
 from nextmv.nextroute.schema.vehicle import Vehicle, VehicleDefaults
 
 
 class Defaults(BaseModel):
     """Default values for vehicles and stops."""
 
-    stops: StopDefaults | None = None
+    stops: Optional[StopDefaults] = None
     """Default values for stops."""
-    vehicles: VehicleDefaults | None = None
+    vehicles: Optional[VehicleDefaults] = None
     """Default values for vehicles."""
 
 
 class DurationGroup(BaseModel):
     """Represents a group of stops that get additional duration whenever a stop
     of the group is approached for the first time."""
 
     duration: int
     """Duration to add when visiting the group."""
-    group: list[str]
+    group: List[str]
     """Stop IDs contained in the group."""
 
 
 class Input(BaseModel):
     """Input schema for Nextroute."""
 
-    stops: list[Stop]
+    stops: List[Stop]
     """Stops that must be visited by the vehicles."""
-    vehicles: list[Vehicle]
+    vehicles: List[Vehicle]
     """Vehicles that service the stops."""
 
-    alternate_stops: list[AlternateStop] | None = None
+    alternate_stops: Optional[List[AlternateStop]] = None
     """A set of alternate stops for the vehicles."""
-    custom_data: Any | None = None
+    custom_data: Optional[Any] = None
     """Arbitrary data associated with the input."""
-    defaults: Defaults | None = None
+    defaults: Optional[Defaults] = None
     """Default values for vehicles and stops."""
-    distance_matrix: list[list[float]] | None = None
+    distance_matrix: Optional[List[List[float]]] = None
     """Matrix of travel distances in meters between stops."""
-    duratrion_groups: list[DurationGroup] | None = None
+    duratrion_groups: Optional[List[DurationGroup]] = None
     """Duration in seconds added when approaching the group."""
-    duration_matrix: list[list[float]] | None = None
+    duration_matrix: Optional[List[List[float]]] = None
     """Matrix of travel durations in seconds between stops."""
-    options: Any | None = None
+    options: Optional[Any] = None
     """Arbitrary options."""
-    stop_groups: list[list[str]] | None = None
+    stop_groups: Optional[List[List[str]]] = None
     """Groups of stops that must be part of the same route."""
```

### Comparing `nextmv-0.4.1.dev1/nextmv/nextroute/schema/output.py` & `nextmv-0.5.0/nextmv/nextroute/check/schema.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,202 +1,141 @@
-"""Defines the output class."""
+"""This module contains definitions for the schema in the Nextroute check."""
 
-
-from datetime import datetime
-from typing import Any
-
-from pydantic import Field
+from typing import Dict, List, Optional
 
 from nextmv.base_model import BaseModel
-from nextmv.nextroute.check import Output as checkOutput
-from nextmv.nextroute.schema.location import Location
-
-
-class Version(BaseModel):
-    """A version used for solving."""
-
-    sdk: str
-    """Nextmv SDK."""
-
-
-class StopOutput(BaseModel):
-    """Basic structure for the output of a stop."""
-
-    id: str
-    """ID of the stop."""
-    location: Location
-    """Location of the stop."""
-
-    custom_data: Any | None = None
-    """Custom data of the stop."""
-
-
-class PlannedStopOutput(BaseModel):
-    """Output of a stop planned in the solution."""
-
-    stop: StopOutput
-    """Basic information on the stop."""
-
-    arrival_time: datetime | None = None
-    """Actual arrival time at this stop."""
-    cumulative_travel_distance: float | None = None
-    """Cumulative distance to travel from the first stop to this one, in meters."""
-    cumulative_travel_duration: float | None = None
-    """Cumulative duration to travel from the first stop to this one, in seconds."""
-    custom_data: Any | None = None
-    """Custom data of the stop."""
-    duration: float | None = None
-    """Duration of the service at the stop, in seconds."""
-    early_arrival_duration: float | None = None
-    """Duration of early arrival at the stop, in seconds."""
-    end_time: datetime | None = None
-    """End time of the service at the stop."""
-    late_arrival_duration: float | None = None
-    """Duration of late arrival at the stop, in seconds."""
-    mix_items: Any | None = None
-    """Mix items at the stop."""
-    start_time: datetime | None = None
-    """Start time of the service at the stop."""
-    target_arrival_time: datetime | None = None
-    """Target arrival time at this stop."""
-    travel_distance: float | None = None
-    """Distance to travel from the previous stop to this one, in meters."""
-    travel_duration: float | None = None
-    """Duration to travel from the previous stop to this one, in seconds."""
-    waiting_duration: float | None = None
-    """Waiting duratino at the stop, in seconds."""
 
 
-class VehicleOutput(BaseModel):
-    """Output of a vehicle in the solution."""
+class ObjectiveTerm(BaseModel):
+    """Check of the individual terms of the objective for a move."""
 
-    id: str
-    """ID of the vehicle."""
-
-    alternate_stops: list[str] | None = None
-    """List of alternate stops that were planned on the vehicle."""
-    custom_data: Any | None = None
-    """Custom data of the vehicle."""
-    route: list[PlannedStopOutput] | None = None
-    """Route of the vehicle, which is a list of stops that were planned on
-    it."""
-    route_duration: float | None = None
-    """Total duration of the vehicle's route, in seconds."""
-    route_stops_duration: float | None = None
-    """Total duration of the stops of the vehicle, in seconds."""
-    route_travel_distance: float | None = None
-    """Total travel distance of the vehicle, in meters."""
-    route_travel_duration: float | None = None
-    """Total travel duration of the vehicle, in seconds."""
-    route_waiting_duration: float | None = None
-    """Total waiting duration of the vehicle, in seconds."""
-
-
-class ObjectiveOutput(BaseModel):
-    """Information of the objective (value function)."""
-
-    name: str
-    """Name of the objective."""
-
-    base: float | None = None
-    """Base of the objective."""
-    custom_data: Any | None = None
-    """Custom data of the objective."""
-    factor: float | None = None
-    """Factor of the objective."""
-    objectives: list[dict[str, Any]] | None = None
-    """List of objectives. Each list is actually of the same class
-    `ObjectiveOutput`, but we avoid a recursive definition here."""
-    value: float | None = None
-    """Value of the objective, which is equivalent to `self.base *
+    base: Optional[float] = None
+    """Base of the objective term."""
+    factor: Optional[float] = None
+    """Factor of the objective term."""
+    name: Optional[str] = None
+    """Name of the objective term."""
+    value: Optional[float] = None
+    """Value of the objective term, which is equivalent to `self.base *
     self.factor`."""
 
 
-class Solution(BaseModel):
-    """Solution to a Vehicle Routing Problem (VRP)."""
-
-    unplanned: list[StopOutput] | None = None
-    """List of stops that were not planned in the solution."""
-    vehicles: list[VehicleOutput] | None = None
-    """List of vehicles in the solution."""
-    objective: ObjectiveOutput | None = None
-    """Information of the objective (value function)."""
-    check: checkOutput | None = None
-    """Check of the solution, if enabled."""
+class Objective(BaseModel):
+    """Estimate of an objective of a move."""
 
+    terms: Optional[List[ObjectiveTerm]] = None
+    """Check of the individual terms of the objective."""
+    value: Optional[float] = None
+    """Value of the objective."""
+    vehicle: Optional[str] = None
+    """ID of the vehicle for which it reports the objective."""
 
-class RunStatistics(BaseModel):
-    """Statistics about a general run."""
-
-    duration: float | None = None
-    """Duration of the run in seconds."""
-    iterations: int | None = None
-    """Number of iterations."""
-    custom: Any | None = None
-    """Custom statistics created by the user. Can normally expect a `dict[str,
-    Any]`."""
-
-
-class ResultStatistics(BaseModel):
-    """Statistics about a specific result."""
-
-    duration: float | None = None
-    """Duration of the run in seconds."""
-    value: float | None = None
-    """Value of the result."""
-    custom: Any | None = None
-    """Custom statistics created by the user. Can normally expect a `dict[str,
-    Any]`."""
-
-
-class DataPoint(BaseModel):
-    """A data point."""
-
-    x: float
-    """X coordinate of the data point."""
-    y: float
-    """Y coordinate of the data point."""
-
-
-class Series(BaseModel):
-    """A series of data points."""
-
-    name: str | None = None
-    """Name of the series."""
-    data_points: list[DataPoint] | None = None
-    """Data of the series."""
 
+class Solution(BaseModel):
+    """Solution that the check has been executed on."""
 
-class SeriesData(BaseModel):
-    """Data of a series."""
+    objective: Optional[Objective] = None
+    """Objective of the start solution."""
+    plan_units_planned: Optional[int] = None
+    """Number of plan units planned in the start solution."""
+    plan_units_unplanned: Optional[int] = None
+    """Number of plan units unplanned in the start solution."""
+    stops_planned: Optional[int] = None
+    """Number of stops planned in the start solution."""
+    vehicles_not_used: Optional[int] = None
+    """Number of vehicles not used in the start solution."""
+    vehicles_used: Optional[int] = None
+    """Number of vehicles used in the start solution."""
+
+
+class Summary(BaseModel):
+    """Summary of the check."""
+
+    moves_failed: Optional[int] = None
+    """number of moves that failed. A move can fail if the estimate of a
+    constraint is incorrect. A constraint is incorrect if `ModelConstraint.
+    EstimateIsViolated` returns true and one of the violation checks returns
+    false. Violation checks are implementations of one or more of the
+    interfaces [SolutionStopViolationCheck], [SolutionVehicleViolationCheck] or
+    [SolutionViolationCheck] on the same constraint. Most constraints do not
+    need and do not have violation checks as the estimate is perfect. The
+    number of moves failed can be more than one per plan unit as we continue to
+    try moves on different vehicles until we find a move that is executable or
+    all vehicles have been visited."""
+    plan_units_best_move_failed: Optional[int] = None
+    """Number of plan units for which the best move can not be planned. This
+    should not happen if all the constraints are implemented correct."""
+    plan_units_best_move_found: Optional[int] = None
+    """Number of plan units for which at least one move has been found and the
+    move is executable."""
+    plan_units_best_move_increases_objective: Optional[int] = None
+    """Number of plan units for which the best move is executable but would
+    increase the objective value instead of decreasing it."""
+    plan_units_checked: Optional[int] = None
+    """Number of plan units that have been checked. If this is less than
+    `self.plan_units_to_be_checked` the check timed out."""
+    plan_units_have_no_move: Optional[int] = None
+    """Number of plan units for which no feasible move has been found. This
+    implies there is no move that can be executed without violating a
+    constraint."""
+    plan_units_to_be_checked: Optional[int] = None
+    """Number of plan units to be checked."""
+
+
+class PlanUnit(BaseModel):
+    """Check of a plan unit."""
+
+    best_move_failed: Optional[bool] = None
+    """True if the plan unit's best move failed to execute."""
+    best_move_increases_objective: Optional[bool] = None
+    """True if the best move for the plan unit increases the objective."""
+    best_move_objective: Optional[Objective] = None
+    """Estimate of the objective of the best move if the plan unit has a best
+    move."""
+    constraints: Optional[Dict[str, int]] = None
+    """Constraints that are violated for the plan unit."""
+    has_best_move: Optional[bool] = None
+    """True if a move is found for the plan unit. A plan unit has no move found
+    if the plan unit is over-constrained or the move found is too expensive."""
+    stops: Optional[List[str]] = None
+    """IDs of the sops in the plan unit."""
+    vehicles_have_moves: Optional[int] = None
+    """Number of vehicles that have moves for the plan unit. Only calculated if
+    the verbosity is very high."""
+    vehicles_with_moves: Optional[List[str]] = None
+    """IDs of the vehicles that have moves for the plan unit. Only calculated
+    if the verbosity is very high."""
 
-    value: Series | None = None
-    """A series for the value of the solution."""
-    custom: list[Series] | None = None
-    """A list of series for custom statistics."""
 
+class Vehicle(BaseModel):
+    """Check of a vehicle."""
 
-class Statistics(BaseModel):
-    """Statistics of a solution."""
+    id: str
+    """ID of the vehicle."""
 
-    run: RunStatistics | None = None
-    """Statistics about the run."""
-    result: ResultStatistics | None = None
-    """Statistics about the last result."""
-    series_data: SeriesData | None = None
-    """Data of the series."""
-    statistics_schema: str | None = Field(alias="schema")
-    """Schema (version)."""
+    plan_units_have_moves: Optional[int] = None
+    """Number of plan units that have moves for the vehicle. Only calculated if
+    the depth is medium."""
 
 
 class Output(BaseModel):
-    """Output schema for Nextroute."""
+    """Output of a feasibility check."""
 
-    options: dict[str, Any]
-    """Options used to obtain this output."""
-    version: Version
-    """Versions used for the solution."""
-
-    solutions: list[Solution] | None = None
-    """Solutions to the problem."""
-    statistics: Statistics | None = None
-    """Statistics of the solution."""
+    duration_maximum: Optional[float] = None
+    """Maximum duration of the check, in seconds."""
+    duration_used: Optional[float] = None
+    """Duration used by the check, in seconds."""
+    error: Optional[str] = None
+    """Error raised during the check."""
+    plan_units: Optional[List[PlanUnit]] = None
+    """Check of the individual plan units."""
+    remark: Optional[str] = None
+    """Remark of the check. It can be "ok", "timeout" or anything else that
+    should explain itself."""
+    solution: Optional[Solution] = None
+    """Start soltuion of the check."""
+    summary: Optional[Summary] = None
+    """Summary of the check."""
+    vehicles: Optional[List[Vehicle]] = None
+    """Check of the vehicles."""
+    verbosity: Optional[str] = None
+    """Verbosity level of the check."""
```

### Comparing `nextmv-0.4.1.dev1/nextmv/nextroute/schema/stop.py` & `nextmv-0.5.0/nextmv/nextroute/schema/stop.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,61 @@
 """Defines the stop class."""
 
-
 from datetime import datetime
-from typing import Any
+from typing import Any, List, Optional
 
 from nextmv.base_model import BaseModel
 from nextmv.nextroute.schema.location import Location
 
 
 class StopDefaults(BaseModel):
     """Default values for a stop."""
 
-    compatibility_attributes: list[str] | None = None
+    compatibility_attributes: Optional[List[str]] = None
     """Attributes that the stop is compatible with."""
-    duration: int | None = None
+    duration: Optional[int] = None
     """Duration of the stop in seconds."""
-    early_arrival_time_penalty: float | None = None
+    early_arrival_time_penalty: Optional[float] = None
     """Penalty per second for arriving at the stop before the target arrival time."""
-    late_arrival_time_penalty: float | None = None
+    late_arrival_time_penalty: Optional[float] = None
     """Penalty per second for arriving at the stop after the target arrival time."""
-    max_wait: int | None = None
+    max_wait: Optional[int] = None
     """Maximum waiting duration in seconds at the stop."""
-    quantity: Any | None = None
+    quantity: Optional[Any] = None
     """Quantity of the stop."""
-    start_time_window: Any | None = None
+    start_time_window: Optional[Any] = None
     """Time window in which the stop can start service."""
-    target_arrival_time: datetime | None = None
+    target_arrival_time: Optional[datetime] = None
     """Target arrival time at the stop."""
-    unplanned_penalty: int | None = None
+    unplanned_penalty: Optional[int] = None
     """Penalty for not planning a stop."""
 
 
 class Stop(StopDefaults):
     """Stop is a location that must be visited by a vehicle in a Vehicle
     Routing Problem (VRP.)"""
 
     id: str
     """Unique identifier for the stop."""
     location: Location
     """Location of the stop."""
 
-    custom_data: Any | None = None
+    custom_data: Optional[Any] = None
     """Arbitrary data associated with the stop."""
-    mixing_items: Any | None = None
+    mixing_items: Optional[Any] = None
     """Defines the items that are inserted or removed from the vehicle when visiting the stop."""
-    precedes: Any | None = None
+    precedes: Optional[Any] = None
     """Stops that must be visited after this one on the same route."""
-    succeeds: Any | None = None
+    succeeds: Optional[Any] = None
     """Stops that must be visited before this one on the same route."""
 
 
 class AlternateStop(StopDefaults):
     """An alternate stop can be serviced instead of another stop."""
 
     id: str
     """Unique identifier for the stop."""
     location: Location
     """Location of the stop."""
 
-    custom_data: Any | None = None
+    custom_data: Optional[Any] = None
     """Arbitrary data associated with the stop."""
```

### Comparing `nextmv-0.4.1.dev1/nextmv/nextroute/schema/vehicle.py` & `nextmv-0.5.0/nextmv/nextroute/schema/vehicle.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 """Defines the vehicle class."""
 
-
 from datetime import datetime
-from typing import Any
+from typing import Any, List, Optional
 
 from nextmv.base_model import BaseModel
 from nextmv.nextroute.schema.location import Location
 
 
 class InitialStop(BaseModel):
     """Represents a stop that is already planned on a vehicle."""
 
     id: str
     """Unique identifier of the stop."""
 
-    fixed: bool | None = None
+    fixed: Optional[bool] = None
     """Whether the stop is fixed on the route."""
 
 
 class VehicleDefaults(BaseModel):
     """Default values for vehicles."""
 
-    activation_penalty: int | None = None
+    activation_penalty: Optional[int] = None
     """Penalty of using the vehicle."""
-    alternate_stops: list[str] | None = None
+    alternate_stops: Optional[List[str]] = None
     """A set of alternate stops for which only one should be serviced."""
-    capacity: Any | None = None
+    capacity: Optional[Any] = None
     """Capacity of the vehicle."""
-    compatibility_attributes: list[str] | None = None
+    compatibility_attributes: Optional[List[str]] = None
     """Attributes that the vehicle is compatible with."""
-    end_location: Location | None = None
+    end_location: Optional[Location] = None
     """Location where the vehicle ends."""
-    end_time: datetime | None = None
+    end_time: Optional[datetime] = None
     """Latest time at which the vehicle ends its route."""
-    max_distance: int | None = None
+    max_distance: Optional[int] = None
     """Maximum distance in meters that the vehicle can travel."""
-    max_duration: int | None = None
+    max_duration: Optional[int] = None
     """Maximum duration in seconds that the vehicle can travel."""
-    max_stops: int | None = None
+    max_stops: Optional[int] = None
     """Maximum number of stops that the vehicle can visit."""
-    max_wait: int | None = None
+    max_wait: Optional[int] = None
     """Maximum aggregated waiting time that the vehicle can wait across route stops."""
-    min_stops: int | None = None
+    min_stops: Optional[int] = None
     """Minimum stops that a vehicle should visit."""
-    min_stops_penalty: float | None = None
+    min_stops_penalty: Optional[float] = None
     """Penalty for not visiting the minimum number of stops."""
-    speed: float | None = None
+    speed: Optional[float] = None
     """Speed of the vehicle in meters per second."""
-    start_level: Any | None = None
+    start_level: Optional[Any] = None
     """Initial level of the vehicle."""
-    start_location: Location | None = None
+    start_location: Optional[Location] = None
     """Location where the vehicle starts."""
-    start_time: datetime | None = None
+    start_time: Optional[datetime] = None
     """Time when the vehicle starts its route."""
 
 
 class Vehicle(VehicleDefaults):
     """A vehicle services stops in a Vehicle Routing Problem (VRP)."""
 
     id: str
     """Unique identifier of the vehicle."""
 
-    custom_data: Any | None = None
+    custom_data: Optional[Any] = None
     """Arbitrary custom data."""
-    initial_stops: list[InitialStop] | None = None
+    initial_stops: Optional[List[InitialStop]] = None
     """Initial stops planned on the vehicle."""
-    stop_duration_multiplier: float | None = None
+    stop_duration_multiplier: Optional[float] = None
     """Multiplier for the duration of stops."""
```

### Comparing `nextmv-0.4.1.dev1/tests/test_base_model.py` & `nextmv-0.5.0/tests/test_base_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import unittest
+from typing import List, Optional
 
 from nextmv.base_model import BaseModel
 
 
 class Foo(BaseModel):
     bar: str
-    baz: int | None = None
+    baz: Optional[int] = None
 
 
 class Roh(BaseModel):
     foo: Foo
-    qux: list[str] | None = None
-    lorem: str | None = None
+    qux: Optional[List[str]] = None
+    lorem: Optional[str] = None
 
 
 class TestBaseModel(unittest.TestCase):
     valid_dict = {
         "foo": {
             "bar": "bar",
             "baz": 1,
```

### Comparing `nextmv-0.4.1.dev1/tests/cloud/test_client.py` & `nextmv-0.5.0/tests/cloud/test_client.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.4.1.dev1/tests/nextroute/schema/input.json` & `nextmv-0.5.0/tests/nextroute/schema/input.json`

 * *Files identical despite different names*

### Comparing `nextmv-0.4.1.dev1/tests/nextroute/schema/output.json` & `nextmv-0.5.0/tests/nextroute/schema/output.json`

 * *Files identical despite different names*

### Comparing `nextmv-0.4.1.dev1/tests/nextroute/schema/output_with_check.json` & `nextmv-0.5.0/tests/nextroute/schema/output_with_check.json`

 * *Files identical despite different names*

### Comparing `nextmv-0.4.1.dev1/tests/nextroute/schema/test_input.py` & `nextmv-0.5.0/tests/nextroute/schema/test_input.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.4.1.dev1/tests/nextroute/schema/test_output.py` & `nextmv-0.5.0/tests/nextroute/schema/test_output.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.4.1.dev1/.gitignore` & `nextmv-0.5.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 # SageMath parsed files
 *.sage.py
 
 # Environments
 .env
 .venv
 env/
-venv/
+venv*/
 ENV/
 env.bak/
 venv.bak/
 
 # Spyder project settings
 .spyderproject
 .spyproject
```

### Comparing `nextmv-0.4.1.dev1/LICENSE` & `nextmv-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nextmv-0.4.1.dev1/README.md` & `nextmv-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 1. [Sign up][signup] for a Nextmv account.
 2. Get your API key. Go to [Team > API Key][api-key].
 
 Visit the [docs][docs] for more information.
 
 ## Installation
 
-Requires Python `>=3.10`. Install using `pip`:
+Requires Python `>=3.8`. Install using `pip`:
 
 ```bash
 pip install nextmv
 ```
 
 ## Usage
```

### Comparing `nextmv-0.4.1.dev1/pyproject.toml` & `nextmv-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "pydantic>=2.5.2",
+    "urllib3>=2.1.0",
     "requests>=2.31.0",
     "pyyaml>=6.0.1",
 ]
 description = "The Python SDK for Nextmv"
 dynamic = [
     "version",
 ]
@@ -33,23 +34,23 @@
 ]
 license = { file = "LICENSE" }
 maintainers = [
     { email = "tech@nextmv.io", name = "Nextmv" }
 ]
 name = "nextmv"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://www.nextmv.io"
 Documentation = "https://www.nextmv.io/docs"
 Repository = "https://github.com/nextmv-io/nextmv-py"
 
 [tool.ruff]
-target-version = "py312"
+target-version = "py38"
 lint.select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
```

### Comparing `nextmv-0.4.1.dev1/PKG-INFO` & `nextmv-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: nextmv
-Version: 0.4.1.dev1
+Version: 0.5.0
 Summary: The Python SDK for Nextmv
 Project-URL: Homepage, https://www.nextmv.io
 Project-URL: Documentation, https://www.nextmv.io/docs
 Project-URL: Repository, https://github.com/nextmv-io/nextmv-py
 Author-email: Nextmv <tech@nextmv.io>
 Maintainer-email: Nextmv <tech@nextmv.io>
 License:                                  Apache License
@@ -209,32 +209,33 @@
            See the License for the specific language governing permissions and
            limitations under the License.
 License-File: LICENSE
 Keywords: decision engineering,decision science,decisions,nextmv,operations research,optimization,shift scheduling,solver,vehicle routing problem
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Requires-Dist: pydantic>=2.5.2
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: requests>=2.31.0
+Requires-Dist: urllib3>=2.1.0
 Description-Content-Type: text/markdown
 
 # Nextmv Python SDK
 
 This is the Python SDK for the Nextmv Platform. Before starting:
 
 1. [Sign up][signup] for a Nextmv account.
 2. Get your API key. Go to [Team > API Key][api-key].
 
 Visit the [docs][docs] for more information.
 
 ## Installation
 
-Requires Python `>=3.10`. Install using `pip`:
+Requires Python `>=3.8`. Install using `pip`:
 
 ```bash
 pip install nextmv
 ```
 
 ## Usage
```

