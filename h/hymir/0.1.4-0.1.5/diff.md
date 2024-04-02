# Comparing `tmp/hymir-0.1.4.tar.gz` & `tmp/hymir-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hymir-0.1.4.tar", max compression
+gzip compressed data, was "hymir-0.1.5.tar", max compression
```

## Comparing `hymir-0.1.4.tar` & `hymir-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1082 2024-03-28 16:11:16.405845 hymir-0.1.4/LICENSE
--rw-r--r--   0        0        0     1925 2024-03-28 16:11:16.405845 hymir-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-03-28 16:11:16.409845 hymir-0.1.4/hymir/__init__.py
--rw-r--r--   0        0        0     1097 2024-03-28 16:11:16.409845 hymir-0.1.4/hymir/config.py
--rw-r--r--   0        0        0      344 2024-03-28 16:11:16.409845 hymir-0.1.4/hymir/errors.py
--rw-r--r--   0        0        0     9035 2024-03-28 16:11:16.409845 hymir-0.1.4/hymir/executor.py
--rw-r--r--   0        0        0        0 2024-03-28 16:11:16.409845 hymir-0.1.4/hymir/executors/__init__.py
--rw-r--r--   0        0        0     7710 2024-03-28 16:11:16.409845 hymir-0.1.4/hymir/executors/celery.py
--rw-r--r--   0        0        0     5621 2024-03-28 16:11:16.409845 hymir-0.1.4/hymir/job.py
--rw-r--r--   0        0        0      146 2024-03-28 16:11:16.409845 hymir-0.1.4/hymir/types.py
--rw-r--r--   0        0        0      373 2024-03-28 16:11:16.409845 hymir-0.1.4/hymir/utils.py
--rw-r--r--   0        0        0     1564 2024-03-28 16:11:16.409845 hymir-0.1.4/hymir/visualize.py
--rw-r--r--   0        0        0     9359 2024-03-28 16:11:16.409845 hymir-0.1.4/hymir/workflow.py
--rw-r--r--   0        0        0      670 2024-03-28 16:11:16.409845 hymir-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 hymir-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-02 13:39:40.679547 hymir-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1925 2024-04-02 13:39:40.679547 hymir-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 13:39:40.679547 hymir-0.1.5/hymir/__init__.py
+-rw-r--r--   0        0        0     1097 2024-04-02 13:39:40.679547 hymir-0.1.5/hymir/config.py
+-rw-r--r--   0        0        0      344 2024-04-02 13:39:40.679547 hymir-0.1.5/hymir/errors.py
+-rw-r--r--   0        0        0     9180 2024-04-02 13:39:40.679547 hymir-0.1.5/hymir/executor.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:39:40.679547 hymir-0.1.5/hymir/executors/__init__.py
+-rw-r--r--   0        0        0     7746 2024-04-02 13:39:40.679547 hymir-0.1.5/hymir/executors/celery.py
+-rw-r--r--   0        0        0     5798 2024-04-02 13:39:40.679547 hymir-0.1.5/hymir/job.py
+-rw-r--r--   0        0        0      146 2024-04-02 13:39:40.679547 hymir-0.1.5/hymir/types.py
+-rw-r--r--   0        0        0      373 2024-04-02 13:39:40.679547 hymir-0.1.5/hymir/utils.py
+-rw-r--r--   0        0        0     1564 2024-04-02 13:39:40.679547 hymir-0.1.5/hymir/visualize.py
+-rw-r--r--   0        0        0     9193 2024-04-02 13:39:40.679547 hymir-0.1.5/hymir/workflow.py
+-rw-r--r--   0        0        0      670 2024-04-02 13:39:40.679547 hymir-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 hymir-0.1.5/PKG-INFO
```

### Comparing `hymir-0.1.4/LICENSE` & `hymir-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hymir-0.1.4/README.md` & `hymir-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hymir-0.1.4/hymir/config.py` & `hymir-0.1.5/hymir/config.py`

 * *Files identical despite different names*

### Comparing `hymir-0.1.4/hymir/executor.py` & `hymir-0.1.5/hymir/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         SUCCESS = 2
         FAILURE = 3
 
     #: The last known status of the job.
     status: Status = Status.PENDING
     #: The total number of times this job has been retried.
     retries: int = 0
+    #: Arbitrary data that can be stored with the job for subsequent runs.
+    context: dict[str, Any] = dataclasses.field(default_factory=dict)
 
     @classmethod
     def deserialize(cls, data: str) -> "JobState":
         """
         Deserialize a JobState from a JSON string.
         """
         return cls(**json.loads(data))
```

### Comparing `hymir-0.1.4/hymir/executors/celery.py` & `hymir-0.1.5/hymir/executors/celery.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
         )
     elif isinstance(ret, CheckLater):
         # The job is not ready to run yet, so we'll check back later.
         # This is useful for implementing workflows that are waiting for
         # external events to occur before they can proceed. We don't consider
         # this a retry, so we don't increment the retry count.
         state.status = JobState.Status.PENDING
+        state.context = ret.context
         CeleryExecutor.store_job_state(workflow_id, job_id, state)
     else:
         state.status = JobState.Status.FAILURE
         CeleryExecutor.store_job_state(workflow_id, job_id, state)
         raise InvalidJobReturn(
             f"The job {job.name!r} returned an invalid value: {ret!r}. Jobs"
             " must return a value of type Success, Failure, Retry, or"
```

### Comparing `hymir-0.1.4/hymir/job.py` & `hymir-0.1.5/hymir/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,18 +79,21 @@
 
     .. note::
 
         This result is _not_ a retry, and does not count towards the maximum
         number of retries for a job.
 
     :param wait_for: The number of seconds to wait before checking again.
+    :param context: A dictionary of context to pass back to the job when it is
+                    checked again.
     """
 
-    def __init__(self, *, wait_for: int = None):
+    def __init__(self, *, wait_for: int = None, context: dict[str, Any] = None):
         self.wait_for = wait_for
+        self.context = context
 
     def __repr__(self):
         return f"{self.__class__.__name__}(wait_for={self.wait_for})"
 
 
 @dataclasses.dataclass
 class Job:
```

### Comparing `hymir-0.1.4/hymir/visualize.py` & `hymir-0.1.5/hymir/visualize.py`

 * *Files identical despite different names*

### Comparing `hymir-0.1.4/hymir/workflow.py` & `hymir-0.1.5/hymir/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import functools
 import json
 from typing import Union, Callable, Iterator
 
 import networkx as nx
 from networkx.readwrite import json_graph
 
-from hymir.config import get_configuration
 from hymir.job import Job
 from hymir.types import JobResultT, ContainerT
 from hymir.utils import importable_name
 
 
 class Group:
     """
@@ -36,16 +35,14 @@
 
 class Workflow:
     """
     A Workflow class encapsulates a graph representing groups and chains
     of jobs to run, along with settings that may control its execution.
 
     :param workflow: The workflow to run.
-    :param on_finished: A job to run when the workflow has completed, even if
-                        the workflow failed.
     """
 
     class Callbacks(enum.Enum):
         ON_FINISHED = "on_finished"
 
     def __init__(self, workflow: Union[Chain, Group, nx.DiGraph]):
         self.callbacks = {}
```

### Comparing `hymir-0.1.4/pyproject.toml` & `hymir-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hymir"
-version = "0.1.4"
+version = "0.1.5"
 description = "Simple workflows."
 authors = ["Tyler Kennedy <tk@tkte.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `hymir-0.1.4/PKG-INFO` & `hymir-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hymir
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simple workflows.
 License: MIT
 Author: Tyler Kennedy
 Author-email: tk@tkte.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

