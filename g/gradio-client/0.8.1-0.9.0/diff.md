# Comparing `tmp/gradio_client-0.8.1.tar.gz` & `tmp/gradio_client-0.9.0.tar.gz`

## Comparing `gradio_client-0.8.1.tar` & `gradio_client-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 gradio_client-0.8.1/README.md
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 gradio_client-0.8.1/requirements.txt
--rw-r--r--   0        0        0    20355 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/CHANGELOG.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/__init__.py
--rw-r--r--   0        0        0    72032 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/client.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10915 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/documentation.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/exceptions.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/media_data.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/package.json
--rw-r--r--   0        0        0    20904 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/serializing.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/types.json
--rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/utils.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/cli/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/cli/deploy_discord.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 gradio_client-0.8.1/gradio_client/templates/discord_chat.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 gradio_client-0.8.1/.gitignore
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 gradio_client-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 gradio_client-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 gradio_client-0.9.0/README.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 gradio_client-0.9.0/requirements.txt
+-rw-r--r--   0        0        0    22152 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/CHANGELOG.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/__init__.py
+-rw-r--r--   0        0        0    72286 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/client.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    13357 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/documentation.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/exceptions.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/media_data.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/package.json
+-rw-r--r--   0        0        0    20904 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/serializing.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/types.json
+-rw-r--r--   0        0        0    31736 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/utils.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/cli/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/cli/deploy_discord.py
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 gradio_client-0.9.0/gradio_client/templates/discord_chat.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 gradio_client-0.9.0/.gitignore
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 gradio_client-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 gradio_client-0.9.0/PKG-INFO
```

### Comparing `gradio_client-0.8.1/README.md` & `gradio_client-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.8.1/gradio_client/CHANGELOG.md` & `gradio_client-0.9.0/gradio_client/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 # gradio_client
 
+## 0.9.0
+
+### Features
+
+- [#7062](https://github.com/gradio-app/gradio/pull/7062) [`0fddd0f`](https://github.com/gradio-app/gradio/commit/0fddd0f971761bff3ef6ccc7ab9deb1891cd80d0) - Determine documentation group automatically.  Thanks [@akx](https://github.com/akx)!
+- [#7102](https://github.com/gradio-app/gradio/pull/7102) [`68a54a7`](https://github.com/gradio-app/gradio/commit/68a54a7a310d8d7072fdae930bf1cfdf12c45a7f) - Improve chatbot streaming performance with diffs.  Thanks [@aliabid94](https://github.com/aliabid94)!/n  Note that this PR changes the API format for generator functions, which would be a breaking change for any clients reading the EventStream directly
+- [#7116](https://github.com/gradio-app/gradio/pull/7116) [`3c8c4ac`](https://github.com/gradio-app/gradio/commit/3c8c4ac2db284e1cb503c397205a79a6dcc27e23) - Document the `gr.ParamViewer` component, and fix component preprocessing/postprocessing docstrings.  Thanks [@abidlabs](https://github.com/abidlabs)!
+- [#7061](https://github.com/gradio-app/gradio/pull/7061) [`05d8a3c`](https://github.com/gradio-app/gradio/commit/05d8a3c8030b733bd47250f5db6f89f230f9a707) - Update ruff to 0.1.13, enable more rules, fix issues.  Thanks [@akx](https://github.com/akx)!
+
+### Fixes
+
+- [#7178](https://github.com/gradio-app/gradio/pull/7178) [`9f23b0b`](https://github.com/gradio-app/gradio/commit/9f23b0bc54b4ef63c056b309370df52ec2c2a43c) - Optimize client view_api method.  Thanks [@freddyaboulton](https://github.com/freddyaboulton)!
+- [#7322](https://github.com/gradio-app/gradio/pull/7322) [`b25e95e`](https://github.com/gradio-app/gradio/commit/b25e95e164e80d66203ef71ce6bdb67ceb6b24df) - Fix `processing_utils.save_url_to_cache()` to follow redirects when accessing the URL.  Thanks [@whitphx](https://github.com/whitphx)!
+
 ## 0.8.1
 
 ### Features
 
 - [#7075](https://github.com/gradio-app/gradio/pull/7075) [`1fc8a94`](https://github.com/gradio-app/gradio/commit/1fc8a941384775f587a6ef30365960f43353cb0d) - fix lint.  Thanks [@freddyaboulton](https://github.com/freddyaboulton)!
 - [#7054](https://github.com/gradio-app/gradio/pull/7054) [`64c65d8`](https://github.com/gradio-app/gradio/commit/64c65d821983961111297a969946d87e2fc4105d) - Add encoding to open/writing files on the deploy_discord function.  Thanks [@WilliamHarer](https://github.com/WilliamHarer)!
```

### Comparing `gradio_client-0.8.1/gradio_client/client.py` & `gradio_client-0.9.0/gradio_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,29 +27,26 @@
     RepositoryNotFoundError,
     build_hf_headers,
     send_telemetry,
 )
 from packaging import version
 
 from gradio_client import serializing, utils
-from gradio_client.documentation import document, set_documentation_group
+from gradio_client.documentation import document
 from gradio_client.exceptions import SerializationSetupError
 from gradio_client.utils import (
     Communicator,
     JobStatus,
     Message,
     QueueError,
     ServerMessage,
     Status,
     StatusUpdate,
 )
 
-set_documentation_group("py-client")
-
-
 DEFAULT_TEMP_DIR = os.environ.get("GRADIO_TEMP_DIR") or str(
     Path(tempfile.gettempdir()) / "gradio"
 )
 
 
 @document("predict", "submit", "view_api", "duplicate", "deploy_discord")
 class Client:
@@ -142,15 +139,15 @@
         )
         self.ws_url = urllib.parse.urljoin(
             self.src.replace("http", "ws", 1), utils.WS_URL
         )
         self.upload_url = urllib.parse.urljoin(self.src, utils.UPLOAD_URL)
         self.reset_url = urllib.parse.urljoin(self.src, utils.RESET_URL)
         self.app_version = version.parse(self.config.get("version", "2.0"))
-        self._info = self._get_api_info()
+        self._info = None
         self.session_hash = str(uuid.uuid4())
 
         endpoint_class = (
             Endpoint if self.protocol.startswith("sse") else EndpointV3Compatibility
         )
         self.endpoints = [
             endpoint_class(self, fn_index, dependency, self.protocol)
@@ -424,15 +421,20 @@
             >> <Status.STARTING: 'STARTING'>
             job.result()  # blocking call
             >> 9.0
         """
         inferred_fn_index = self._infer_fn_index(api_name, fn_index)
 
         helper = None
-        if self.endpoints[inferred_fn_index].protocol in ("ws", "sse", "sse_v1"):
+        if self.endpoints[inferred_fn_index].protocol in (
+            "ws",
+            "sse",
+            "sse_v1",
+            "sse_v2",
+        ):
             helper = self.new_helper(inferred_fn_index)
         end_to_end_fn = self.endpoints[inferred_fn_index].make_end_to_end_fn(helper)
         future = self.executor.submit(end_to_end_fn, *args)
 
         job = Job(
             future, communicator=helper, verbose=self.verbose, space_id=self.space_id
         )
@@ -552,14 +554,16 @@
                             ]
                         }
                     }
                 }
             }
 
         """
+        if not self._info:
+            self._info = self._get_api_info()
         num_named_endpoints = len(self._info["named_endpoints"])
         num_unnamed_endpoints = len(self._info["unnamed_endpoints"])
         if num_named_endpoints == 0 and all_endpoints is None:
             all_endpoints = True
 
         human_info = "Client.predict() Usage Info\n---------------------------\n"
         human_info += f"Named API endpoints: {num_named_endpoints}\n"
@@ -569,17 +573,16 @@
 
         if all_endpoints:
             human_info += f"\nUnnamed API endpoints: {num_unnamed_endpoints}\n"
             for fn_index, endpoint_info in self._info["unnamed_endpoints"].items():
                 # When loading from json, the fn_indices are read as strings
                 # because json keys can only be strings
                 human_info += self._render_endpoints_info(int(fn_index), endpoint_info)
-        else:
-            if num_unnamed_endpoints > 0:
-                human_info += f"\nUnnamed API endpoints: {num_unnamed_endpoints}, to view, run Client.view_api(all_endpoints=True)\n"
+        elif num_unnamed_endpoints > 0:
+            human_info += f"\nUnnamed API endpoints: {num_unnamed_endpoints}, to view, run Client.view_api(all_endpoints=True)\n"
 
         if print_info:
             print(human_info)
         if return_format == "str":
             return human_info
         elif return_format == "dict":
             return self._info
@@ -992,21 +995,23 @@
                 "session_hash": self.client.session_hash,
             }
 
             if self.protocol == "sse":
                 result = utils.synchronize_async(
                     self._sse_fn_v0, data, hash_data, helper
                 )
-            elif self.protocol == "sse_v1":
+            elif self.protocol in ("sse_v1", "sse_v2"):
                 event_id = utils.synchronize_async(
                     self.client.send_data, data, hash_data
                 )
                 self.client.pending_event_ids.add(event_id)
                 self.client.pending_messages_per_event[event_id] = []
-                result = utils.synchronize_async(self._sse_fn_v1, helper, event_id)
+                result = utils.synchronize_async(
+                    self._sse_fn_v1_v2, helper, event_id, self.protocol
+                )
             else:
                 raise ValueError(f"Unsupported protocol: {self.protocol}")
 
             if "error" in result:
                 raise ValueError(result["error"])
 
             try:
@@ -1191,28 +1196,31 @@
                 helper,
                 self.client.sse_url,
                 self.client.sse_data_url,
                 self.client.headers,
                 self.client.cookies,
             )
 
-    async def _sse_fn_v1(self, helper: Communicator, event_id: str):
-        return await utils.get_pred_from_sse_v1(
+    async def _sse_fn_v1_v2(
+        self, helper: Communicator, event_id: str, protocol: Literal["sse_v1", "sse_v2"]
+    ):
+        return await utils.get_pred_from_sse_v1_v2(
             helper,
             self.client.headers,
             self.client.cookies,
             self.client.pending_messages_per_event,
             event_id,
+            protocol,
         )
 
 
 class EndpointV3Compatibility:
     """Endpoint class for connecting to v3 endpoints. Backwards compatibility."""
 
-    def __init__(self, client: Client, fn_index: int, dependency: dict, *args):
+    def __init__(self, client: Client, fn_index: int, dependency: dict, *_args):
         self.client: Client = client
         self.fn_index = fn_index
         self.dependency = dependency
         api_name = dependency.get("api_name")
         self.api_name: str | Literal[False] | None = (
             "/" + api_name if isinstance(api_name, str) else api_name
         )
@@ -1553,16 +1561,20 @@
 
         while True:
             with self.communicator.lock:
                 if len(self.communicator.job.outputs) >= self._counter + 1:
                     o = self.communicator.job.outputs[self._counter]
                     self._counter += 1
                     return o
-                if self.communicator.job.latest_status.code == Status.FINISHED:
+                if (
+                    self.communicator.job.latest_status.code == Status.FINISHED
+                    and self._counter >= len(self.communicator.job.outputs)
+                ):
                     raise StopIteration()
+                time.sleep(0.001)
 
     def result(self, timeout: float | None = None) -> Any:
         """
         Return the result of the call that the future represents. Raises CancelledError: If the future was cancelled, TimeoutError: If the future didn't finish executing before the given timeout, and Exception: If the call raised then that exception will be raised.
 
         Parameters:
             timeout: The number of seconds to wait for the result if the future isn't done. If None, then there is no limit on the wait time.
@@ -1653,34 +1665,33 @@
                     rank=0,
                     queue_size=None,
                     success=False,
                     time=time,
                     eta=None,
                     progress_data=None,
                 )
+        elif not self.communicator:
+            return StatusUpdate(
+                code=Status.PROCESSING,
+                rank=0,
+                queue_size=None,
+                success=None,
+                time=time,
+                eta=None,
+                progress_data=None,
+            )
         else:
-            if not self.communicator:
-                return StatusUpdate(
-                    code=Status.PROCESSING,
-                    rank=0,
-                    queue_size=None,
-                    success=None,
-                    time=time,
-                    eta=None,
-                    progress_data=None,
-                )
-            else:
-                with self.communicator.lock:
-                    eta = self.communicator.job.latest_status.eta
-                    if self.verbose and self.space_id and eta and eta > 30:
-                        print(
-                            f"Due to heavy traffic on this app, the prediction will take approximately {int(eta)} seconds."
-                            f"For faster predictions without waiting in queue, you may duplicate the space using: Client.duplicate({self.space_id})"
-                        )
-                    return self.communicator.job.latest_status
+            with self.communicator.lock:
+                eta = self.communicator.job.latest_status.eta
+                if self.verbose and self.space_id and eta and eta > 30:
+                    print(
+                        f"Due to heavy traffic on this app, the prediction will take approximately {int(eta)} seconds."
+                        f"For faster predictions without waiting in queue, you may duplicate the space using: Client.duplicate({self.space_id})"
+                    )
+                return self.communicator.job.latest_status
 
     def __getattr__(self, name):
         """Forwards any properties to the Future class."""
         return getattr(self.future, name)
 
     def cancel(self) -> bool:
         """Cancels the job as best as possible.
```

### Comparing `gradio_client-0.8.1/gradio_client/documentation.py` & `gradio_client-0.9.0/gradio_client/documentation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """Contains methods that generate documentation for Gradio functions and classes."""
 
 from __future__ import annotations
 
 import inspect
+import warnings
+from collections import defaultdict
+from functools import lru_cache
 from typing import Callable
 
-classes_to_document = {}
+classes_to_document = defaultdict(list)
 classes_inherit_documentation = {}
-documentation_group = None
-
-
-def set_documentation_group(m):
-    global documentation_group
-    documentation_group = m
-    if m not in classes_to_document:
-        classes_to_document[m] = []
 
 
 def extract_instance_attr_doc(cls, attr):
     code = inspect.getsource(cls.__init__)
     lines = [line.strip() for line in code.split("\n")]
     i = None
     for i, line in enumerate(lines):  # noqa: B007
@@ -38,32 +33,66 @@
                 + "\n start:"
                 + lines[i]
             )
     doc_string = " ".join(lines[start_line + 1 : end_line])
     return doc_string
 
 
-def document(*fns, inherit=False):
+_module_prefixes = [
+    ("gradio._simple_templates", "component"),
+    ("gradio.block", "block"),
+    ("gradio.chat", "chatinterface"),
+    ("gradio.component", "component"),
+    ("gradio.events", "helpers"),
+    ("gradio.exceptions", "helpers"),
+    ("gradio.external", "helpers"),
+    ("gradio.flag", "flagging"),
+    ("gradio.helpers", "helpers"),
+    ("gradio.interface", "interface"),
+    ("gradio.layout", "layout"),
+    ("gradio.route", "routes"),
+    ("gradio.theme", "themes"),
+    ("gradio_client", "py-client"),
+]
+
+
+@lru_cache(maxsize=10)
+def _get_module_documentation_group(modname) -> str:
+    for prefix, group in _module_prefixes:
+        if modname.startswith(prefix):
+            return group
+    raise ValueError(f"No known documentation group for module {modname!r}")
+
+
+def document(*fns, inherit=False, documentation_group=None):
     """
     Defines the @document decorator which adds classes or functions to the Gradio
     documentation at www.gradio.app/docs.
 
     Usage examples:
     - Put @document() above a class to document the class and its constructor.
     - Put @document("fn1", "fn2") above a class to also document methods fn1 and fn2.
     - Put @document("*fn3") with an asterisk above a class to document the instance attribute methods f3.
     """
+    _documentation_group = documentation_group
 
     def inner_doc(cls):
         functions = list(fns)
         if hasattr(cls, "EVENTS"):
             functions += cls.EVENTS
-        global documentation_group
         if inherit:
             classes_inherit_documentation[cls] = None
+
+        documentation_group = _documentation_group  # avoid `nonlocal` reassignment
+        if _documentation_group is None:
+            try:
+                modname = inspect.getmodule(cls).__name__  # type: ignore
+                documentation_group = _get_module_documentation_group(modname)
+            except Exception as exc:
+                warnings.warn(f"Could not get documentation group for {cls}: {exc}")
         classes_to_document[documentation_group].append((cls, functions))
         return cls
 
     return inner_doc
 
 
 def document_fn(fn: Callable, cls) -> tuple[str, list[dict], dict, str | None]:
@@ -119,14 +148,16 @@
             elif mode == "example":
                 examples.append(line)
     description_doc = " ".join(description)
     parameter_docs = []
     for param_name, param in signature.parameters.items():
         if param_name.startswith("_"):
             continue
+        if param_name == "self":
+            continue
         if param_name in ["kwargs", "args"] and param_name not in parameters:
             continue
         parameter_doc = {
             "name": param_name,
             "annotation": param.annotation,
             "doc": parameters.get(param_name),
         }
@@ -143,15 +174,15 @@
             if "kwargs" in parameter_doc["doc"]:
                 parameter_doc["kwargs"] = True
             if "args" in parameter_doc["doc"]:
                 parameter_doc["args"] = True
         parameter_docs.append(parameter_doc)
     assert (
         len(parameters) == 0
-    ), f"Documentation format for {fn.__name__} documents nonexistent parameters: {''.join(parameters.keys())}"
+    ), f"Documentation format for {fn.__name__} documents nonexistent parameters: {', '.join(parameters.keys())}. Valid parameters: {', '.join(signature.parameters.keys())}"
     if len(returns) == 0:
         return_docs = {}
     elif len(returns) == 1:
         return_docs = {"annotation": signature.return_annotation, "doc": returns[0]}
     else:
         return_docs = {}
         # raise ValueError("Does not support multiple returns yet.")
@@ -171,23 +202,22 @@
         if line.endswith(":") and " " not in line:
             mode = line[:-1].lower()
             tags[mode] = []
         elif line.split(" ")[0].endswith(":") and not line.startswith("    "):
             tag = line[: line.index(":")].lower()
             value = line[line.index(":") + 2 :]
             tags[tag] = value
+        elif mode == "description":
+            description_lines.append(line if line.strip() else "<br>")
         else:
-            if mode == "description":
-                description_lines.append(line if line.strip() else "<br>")
-            else:
-                if not (line.startswith("    ") or not line.strip()):
-                    raise SyntaxError(
-                        f"Documentation format for {cls.__name__} has format error in line: {line}"
-                    )
-                tags[mode].append(line[4:])
+            if not (line.startswith("    ") or not line.strip()):
+                raise SyntaxError(
+                    f"Documentation format for {cls.__name__} has format error in line: {line}"
+                )
+            tags[mode].append(line[4:])
     if "example" in tags:
         example = "\n".join(tags["example"])
         del tags["example"]
     else:
         example = None
     for key, val in tags.items():
         if isinstance(val, list):
@@ -199,25 +229,51 @@
 def generate_documentation():
     documentation = {}
     for mode, class_list in classes_to_document.items():
         documentation[mode] = []
         for cls, fns in class_list:
             fn_to_document = cls if inspect.isfunction(cls) else cls.__init__
             _, parameter_doc, return_doc, _ = document_fn(fn_to_document, cls)
+            if (
+                hasattr(cls, "preprocess")
+                and callable(cls.preprocess)  # type: ignore
+                and hasattr(cls, "postprocess")
+                and callable(cls.postprocess)  # type: ignore
+            ):
+                preprocess_doc = document_fn(cls.preprocess, cls)  # type: ignore
+                postprocess_doc = document_fn(cls.postprocess, cls)  # type: ignore
+                preprocess_doc, postprocess_doc = (
+                    {
+                        "parameter_doc": preprocess_doc[1],
+                        "return_doc": preprocess_doc[2],
+                    },
+                    {
+                        "parameter_doc": postprocess_doc[1],
+                        "return_doc": postprocess_doc[2],
+                    },
+                )
             cls_description, cls_tags, cls_example = document_cls(cls)
             cls_documentation = {
                 "class": cls,
                 "name": cls.__name__,
                 "description": cls_description,
                 "tags": cls_tags,
                 "parameters": parameter_doc,
                 "returns": return_doc,
                 "example": cls_example,
                 "fns": [],
             }
+            if (
+                hasattr(cls, "preprocess")
+                and callable(cls.preprocess)  # type: ignore
+                and hasattr(cls, "postprocess")
+                and callable(cls.postprocess)  # type: ignore
+            ):
+                cls_documentation["preprocess"] = preprocess_doc  # type: ignore
+                cls_documentation["postprocess"] = postprocess_doc  # type: ignore
             for fn_name in fns:
                 instance_attribute_fn = fn_name.startswith("*")
                 if instance_attribute_fn:
                     fn_name = fn_name[1:]
                     # Instance attribute fns are classes
                     # whose __call__ method determines their behavior
                     fn = getattr(cls(), fn_name).__call__
```

### Comparing `gradio_client-0.8.1/gradio_client/media_data.py` & `gradio_client-0.9.0/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.8.1/gradio_client/serializing.py` & `gradio_client-0.9.0/gradio_client/serializing.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.8.1/gradio_client/types.json` & `gradio_client-0.9.0/gradio_client/types.json`

 * *Files identical despite different names*

### Comparing `gradio_client-0.8.1/gradio_client/utils.py` & `gradio_client-0.9.0/gradio_client/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 import base64
+import copy
 import hashlib
 import json
 import mimetypes
 import os
 import pkgutil
 import secrets
 import shutil
@@ -13,15 +14,15 @@
 import warnings
 from concurrent.futures import CancelledError
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from threading import Lock
-from typing import Any, Callable, Optional, TypedDict
+from typing import Any, Callable, Literal, Optional, TypedDict
 
 import fsspec.asyn
 import httpx
 import huggingface_hub
 from huggingface_hub import SpaceStage
 from websockets.legacy.protocol import WebSocketCommonProtocol
 
@@ -377,44 +378,44 @@
             pass
 
     assert len(done) == 1
     for task in done:
         return task.result()
 
 
-async def get_pred_from_sse_v1(
+async def get_pred_from_sse_v1_v2(
     helper: Communicator,
     headers: dict[str, str],
     cookies: dict[str, str] | None,
     pending_messages_per_event: dict[str, list[Message | None]],
     event_id: str,
+    protocol: Literal["sse_v1", "sse_v2"],
 ) -> dict[str, Any] | None:
     done, pending = await asyncio.wait(
         [
             asyncio.create_task(check_for_cancel(helper, headers, cookies)),
             asyncio.create_task(
-                stream_sse_v1(
-                    helper,
-                    pending_messages_per_event,
-                    event_id,
-                )
+                stream_sse_v1_v2(helper, pending_messages_per_event, event_id, protocol)
             ),
         ],
         return_when=asyncio.FIRST_COMPLETED,
     )
 
     for task in pending:
         task.cancel()
         try:
             await task
         except asyncio.CancelledError:
             pass
 
     assert len(done) == 1
     for task in done:
+        exception = task.exception()
+        if exception:
+            raise exception
         return task.result()
 
 
 async def check_for_cancel(
     helper: Communicator, headers: dict[str, str], cookies: dict[str, str] | None
 ):
     while True:
@@ -498,21 +499,23 @@
                 else:
                     raise ValueError(f"Unexpected message: {line}")
         raise ValueError("Did not receive process_completed message.")
     except asyncio.CancelledError:
         raise
 
 
-async def stream_sse_v1(
+async def stream_sse_v1_v2(
     helper: Communicator,
     pending_messages_per_event: dict[str, list[Message | None]],
     event_id: str,
+    protocol: Literal["sse_v1", "sse_v2"],
 ) -> dict[str, Any]:
     try:
         pending_messages = pending_messages_per_event[event_id]
+        pending_responses_for_diffs = None
 
         while True:
             if len(pending_messages) > 0:
                 msg = pending_messages.pop(0)
             else:
                 await asyncio.sleep(0.05)
                 continue
@@ -536,14 +539,27 @@
                     eta=msg.get("rank_eta"),
                     progress_data=ProgressUnit.from_msg(msg["progress_data"])
                     if "progress_data" in msg
                     else None,
                     log=log_message,
                 )
                 output = msg.get("output", {}).get("data", [])
+                if (
+                    msg["msg"] == ServerMessage.process_generating
+                    and protocol == "sse_v2"
+                ):
+                    if pending_responses_for_diffs is None:
+                        pending_responses_for_diffs = list(output)
+                    else:
+                        for i, value in enumerate(output):
+                            prev_output = pending_responses_for_diffs[i]
+                            new_output = apply_diff(prev_output, value)
+                            pending_responses_for_diffs[i] = new_output
+                            output[i] = new_output
+
                 if output and status_update.code != Status.FINISHED:
                     try:
                         result = helper.prediction_processor(*output)
                     except Exception as e:
                         result = [e]
                     helper.job.outputs.append(result)
                 helper.job.latest_status = status_update
@@ -553,14 +569,56 @@
             elif msg["msg"] == ServerMessage.server_stopped:
                 raise ValueError("Server stopped.")
 
     except asyncio.CancelledError:
         raise
 
 
+def apply_diff(obj, diff):
+    obj = copy.deepcopy(obj)
+
+    def apply_edit(target, path, action, value):
+        if len(path) == 0:
+            if action == "replace":
+                return value
+            elif action == "append":
+                return target + value
+            else:
+                raise ValueError(f"Unsupported action: {action}")
+
+        current = target
+        for i in range(len(path) - 1):
+            current = current[path[i]]
+
+        last_path = path[-1]
+        if action == "replace":
+            current[last_path] = value
+        elif action == "append":
+            current[last_path] += value
+        elif action == "add":
+            if isinstance(current, list):
+                current.insert(int(last_path), value)
+            else:
+                current[last_path] = value
+        elif action == "delete":
+            if isinstance(current, list):
+                del current[int(last_path)]
+            else:
+                del current[last_path]
+        else:
+            raise ValueError(f"Unknown action: {action}")
+
+        return target
+
+    for action, path, value in diff:
+        obj = apply_edit(obj, path, action, value)
+
+    return obj
+
+
 ########################
 # Data processing utils
 ########################
 
 
 def download_file(
     url_path: str,
@@ -571,15 +629,17 @@
         os.makedirs(dir, exist_ok=True)
     headers = {"Authorization": "Bearer " + hf_token} if hf_token else {}
 
     sha1 = hashlib.sha1()
     temp_dir = Path(tempfile.gettempdir()) / secrets.token_hex(20)
     temp_dir.mkdir(exist_ok=True, parents=True)
 
-    with httpx.stream("GET", url_path, headers=headers) as response:
+    with httpx.stream(
+        "GET", url_path, headers=headers, follow_redirects=True
+    ) as response:
         response.raise_for_status()
         with open(temp_dir / Path(url_path).name, "wb") as f:
             for chunk in response.iter_bytes(chunk_size=128 * sha1.block_size):
                 sha1.update(chunk)
                 f.write(chunk)
 
     directory = Path(dir) / sha1.hexdigest()
@@ -604,15 +664,17 @@
     if dir is not None:
         os.makedirs(dir, exist_ok=True)
     headers = {"Authorization": "Bearer " + hf_token} if hf_token else {}
     directory = Path(dir or tempfile.gettempdir()) / secrets.token_hex(20)
     directory.mkdir(exist_ok=True, parents=True)
     file_path = directory / Path(url_path).name
 
-    with httpx.stream("GET", url_path, headers=headers) as response:
+    with httpx.stream(
+        "GET", url_path, headers=headers, follow_redirects=True
+    ) as response:
         response.raise_for_status()
         with open(file_path, "wb") as f:
             for chunk in response.iter_raw():
                 f.write(chunk)
     return str(file_path.resolve())
```

### Comparing `gradio_client-0.8.1/gradio_client/cli/deploy_discord.py` & `gradio_client-0.9.0/gradio_client/cli/deploy_discord.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.8.1/gradio_client/templates/discord_chat.py` & `gradio_client-0.9.0/gradio_client/templates/discord_chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,51 +137,51 @@
 
 if not DISCORD_TOKEN:
     welcome_message = """
 
     ## You have not specified a DISCORD_TOKEN, which means you have not created a bot account. Please follow these steps:
 
     ### 1. Go to https://discord.com/developers/applications and click 'New Application'
-    
+
     ### 2. Give your bot a name 🤖
 
     ![](https://gradio-builds.s3.amazonaws.com/demo-files/discordbots/BotName.png)
-    
+
     ## 3. In Settings > Bot, click the 'Reset Token' button to get a new token. Write it down and keep it safe 🔐
-    
+
     ![](https://gradio-builds.s3.amazonaws.com/demo-files/discordbots/ResetToken.png)
-    
+
     ## 4. Optionally make the bot public if you want anyone to be able to add it to their servers
-    
+
     ## 5. Scroll down and enable 'Message Content Intent' under 'Priviledged Gateway Intents'
-    
+
     ![](https://gradio-builds.s3.amazonaws.com/demo-files/discordbots/MessageContentIntent.png)
 
     ## 6. Save your changes!
 
     ## 7. The token from step 3 is the DISCORD_TOKEN. Rerun the deploy_discord command, e.g client.deploy_discord(discord_bot_token=DISCORD_TOKEN, ...), or add the token as a space secret manually.
 """
 else:
     permissions = Permissions(326417525824)
     url = oauth_url(bot.user.id, permissions=permissions)
     welcome_message = f"""
-    ## Add this bot to your server by clicking this link: 
-    
+    ## Add this bot to your server by clicking this link:
+
     {url}
 
     ## How to use it?
 
     The bot can be triggered via `/<<command-name>>` followed by your text prompt.
-    
+
     This will create a thread with the bot's response to your text prompt.
     You can reply in the thread (without `/<<command-name>>`) to continue the conversation.
     In the thread, the bot will only reply to the original author of the command.
 
     ⚠️ Note ⚠️: Please make sure this bot's command does have the same name as another command in your server.
-    
+
     ⚠️ Note ⚠️: Bot commands do not work in DMs with the bot as of now.
     """
 
 
 with gr.Blocks() as demo:
     gr.Markdown(
         f"""
```

### Comparing `gradio_client-0.8.1/.gitignore` & `gradio_client-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gradio_client-0.8.1/pyproject.toml` & `gradio_client-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradio_client-0.8.1/PKG-INFO` & `gradio_client-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <gradio-team@huggingface.co>, Ali Abid <gradio-team@huggingface.co>, Ali Abdalla <gradio-team@huggingface.co>, Dawood Khan <gradio-team@huggingface.co>, Ahsen Khaliq <gradio-team@huggingface.co>, Pete Allen <gradio-team@huggingface.co>, Freddy Boulton <gradio-team@huggingface.co>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

