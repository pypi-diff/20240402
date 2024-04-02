# Comparing `tmp/agentops-0.1.0b4.tar.gz` & `tmp/agentops-0.1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentops-0.1.0b4.tar", last modified: Tue Mar 26 01:14:50 2024, max compression
+gzip compressed data, was "agentops-0.1.0b5.tar", last modified: Tue Apr  2 00:56:12 2024, max compression
```

## Comparing `agentops-0.1.0b4.tar` & `agentops-0.1.0b5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 01:14:50.170432 agentops-0.1.0b4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-26 01:14:45.000000 agentops-0.1.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-03-26 01:14:50.166432 agentops-0.1.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-03-26 01:14:45.000000 agentops-0.1.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 01:14:50.166432 agentops-0.1.0b4/agentops/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1522 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    11455 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/host_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22721 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/langchain_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12502 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/llm_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-26 01:14:45.000000 agentops-0.1.0b4/agentops/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 01:14:50.166432 agentops-0.1.0b4/agentops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-03-26 01:14:50.000000 agentops-0.1.0b4/agentops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-26 01:14:50.000000 agentops-0.1.0b4/agentops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 01:14:50.000000 agentops-0.1.0b4/agentops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-26 01:14:50.000000 agentops-0.1.0b4/agentops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-26 01:14:50.000000 agentops-0.1.0b4/agentops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-26 01:14:45.000000 agentops-0.1.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 01:14:50.170432 agentops-0.1.0b4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 01:14:50.166432 agentops-0.1.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-26 01:14:45.000000 agentops-0.1.0b4/tests/test_canary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-03-26 01:14:45.000000 agentops-0.1.0b4/tests/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-03-26 01:14:45.000000 agentops-0.1.0b4/tests/test_record_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-03-26 01:14:45.000000 agentops-0.1.0b4/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-26 01:14:45.000000 agentops-0.1.0b4/tests/test_teardown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:56:12.950603 agentops-0.1.0b5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 00:56:06.000000 agentops-0.1.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-02 00:56:12.950603 agentops-0.1.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-02 00:56:06.000000 agentops-0.1.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:56:12.946603 agentops-0.1.0b5/agentops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1394 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/host_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22227 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/langchain_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/llm_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:56:12.946603 agentops-0.1.0b5/agentops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-02 00:56:12.000000 agentops-0.1.0b5/agentops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 00:56:12.000000 agentops-0.1.0b5/agentops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:56:12.000000 agentops-0.1.0b5/agentops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 00:56:12.000000 agentops-0.1.0b5/agentops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 00:56:12.000000 agentops-0.1.0b5/agentops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-02 00:56:06.000000 agentops-0.1.0b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:56:12.950603 agentops-0.1.0b5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:56:12.946603 agentops-0.1.0b5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 00:56:06.000000 agentops-0.1.0b5/tests/test_canary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-02 00:56:06.000000 agentops-0.1.0b5/tests/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-02 00:56:06.000000 agentops-0.1.0b5/tests/test_record_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-02 00:56:06.000000 agentops-0.1.0b5/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-02 00:56:06.000000 agentops-0.1.0b5/tests/test_teardown.py
```

### Comparing `agentops-0.1.0b4/LICENSE` & `agentops-0.1.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b4/PKG-INFO` & `agentops-0.1.0b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.0b4
+Version: 0.1.0b5
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
-Requires-Dist: pydantic>=1.9.0
-Requires-Dist: packaging<24.0,>=23.1
-Requires-Dist: toml>=0.10.2
 Requires-Dist: psutil==5.9.8
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: requests_mock==1.11.0; extra == "dev"
 Provides-Extra: langchain
 Requires-Dist: langchain>=0.0.354; extra == "langchain"
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.0b4 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.0b5 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests==2.31.0 Requires-Dist: pydantic>=1.9.0 Requires-Dist:
-packaging<24.0,>=23.1 Requires-Dist: toml>=0.10.2 Requires-Dist: psutil==5.9.8
-Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
-requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
-langchain>=0.0.354; extra == "langchain"
+requests==2.31.0 Requires-Dist: psutil==5.9.8 Provides-Extra: dev Requires-
+Dist: pytest==7.4.0; extra == "dev" Requires-Dist: requests_mock==1.11.0; extra
+== "dev" Provides-Extra: langchain Requires-Dist: langchain>=0.0.354; extra ==
+"langchain"
                                     [Logo]
                             _D_o_c_u_m_e_n_t_a_t_i_o_n | _D_i_s_c_o_r_d
                      AI agents suck. Weâre fixing that.
 Build your next agent with benchmarks, observability, and replay analytics.
 AgentOps is the toolkit for evaluating and developing robust and reliable AI
 agents. AgentOps is open beta. You can sign up for AgentOps [here](https://
 app.agentops.ai). [![License: MIT](https://img.shields.io/badge/License-MIT-
```

### Comparing `agentops-0.1.0b4/README.md` & `agentops-0.1.0b5/README.md`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b4/agentops/agent.py` & `agentops-0.1.0b5/agentops/agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,36 @@
+import logging
 from uuid import uuid4
 from agentops import Client
 from inspect import isclass, isfunction
 
 
 def track_agent(name: str | None = None):
     def decorator(obj):
         if name:
             obj.agent_ops_agent_name = name
 
         if isclass(obj):
             original_init = obj.__init__
 
             def new_init(self, *args, **kwargs):
-                original_init(self, *args, **kwargs)
-                self.agent_ops_agent_id = uuid4()
-                ao_client = Client()
-                ao_client.create_agent(self.agent_ops_agent_id, self.agent_ops_agent_name)
+                try:
+                    original_init(self, *args, **kwargs)
+                    self.agent_ops_agent_id = uuid4()
+                    Client().create_agent(self.agent_ops_agent_id, self.agent_ops_agent_name)
+                except AttributeError as e:
+                    logging.error("AgentOps failed to track an agent. This often happens if agentops.init() was not "
+                                  "called before initializing an agent with the @track_agent decorator.")
+                    raise e
 
             obj.__init__ = new_init
 
         elif isfunction(obj):
             obj.agent_ops_agent_id = uuid4()
-            ao_client = Client()
-            ao_client.create_agent(obj.agent_ops_agent_id, obj.agent_ops_agent_name)
+            Client().create_agent(obj.agent_ops_agent_id, obj.agent_ops_agent_name)
 
         else:
             raise Exception("Invalid input, 'obj' must be a class or a function")
 
         return obj
 
     return decorator
```

### Comparing `agentops-0.1.0b4/agentops/client.py` & `agentops-0.1.0b5/agentops/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,80 +2,86 @@
 AgentOps client module that provides a client class with public interfaces and configuration.
 
 Classes:
     Client: Provides methods to interact with the AgentOps service.
 """
 
 from .event import ActionEvent, ErrorEvent, Event
+from .enums import EndState
 from .helpers import get_ISO_time, singleton, check_call_stack_for_agent_id
 from .session import Session
 from .worker import Worker
 from .host_env import get_host_env
 from uuid import uuid4
 from typing import Optional, List
-from pydantic import Field
-from os import environ
 import traceback
 import logging
 import inspect
 import atexit
 import signal
 import sys
 
 from .meta_client import MetaClient
-from .config import Configuration
+from .config import Configuration, ConfigurationError
 from .llm_tracker import LlmTracker
 
 
 @singleton
 class Client(metaclass=MetaClient):
     """
     Client for AgentOps service.
 
     Args:
+
         api_key (str, optional): API Key for AgentOps services. If none is provided, key will 
             be read from the AGENTOPS_API_KEY environment variable.
-        tags (List[str], optional): Tags for the sessions that can be used for grouping or 
-            sorting later (e.g. ["GPT-4"]).
-        endpoint (str, optional): The endpoint for the AgentOps service. Defaults to 'https://api.agentops.ai'.
+        parent_key (str, optional): Organization key to give visibility of all user sessions the user's organization. If none is provided, key will 
+            be read from the AGENTOPS_PARENT_KEY environment variable.
+        endpoint (str, optional): The endpoint for the AgentOps service. If none is provided, key will 
+            be read from the AGENTOPS_API_ENDPOINT environment variable. Defaults to 'https://api.agentops.ai'.
         max_wait_time (int, optional): The maximum time to wait in milliseconds before flushing the queue. 
-            Defaults to 1000.
+            Defaults to 30,000 (30 seconds)
         max_queue_size (int, optional): The maximum size of the event queue. Defaults to 100.
+        tags (List[str], optional): Tags for the sessions that can be used for grouping or 
+            sorting later (e.g. ["GPT-4"]).
         override (bool): Whether to override and LLM calls to emit as events.
+        auto_start_session (bool): Whether to start a session automatically when the client is created.
     Attributes:
         _session (Session, optional): A Session is a grouping of events (e.g. a run of your agent).
+        _worker (Worker, optional): A Worker manages the event queue and sends session updates to the AgentOps api server
     """
 
-    def __init__(self, api_key: Optional[str] = None,
+    def __init__(self,
+                 api_key: Optional[str] = None,
+                 parent_key: Optional[str] = None,
+                 endpoint: Optional[str] = None,
+                 max_wait_time: Optional[int] = None,
+                 max_queue_size: Optional[int] = None,
                  tags: Optional[List[str]] = None,
-                 endpoint: Optional[str] = environ.get('AGENTOPS_API_ENDPOINT', 'https://api.agentops.ai'),
-                 max_wait_time: Optional[int] = 1000,
-                 max_queue_size: Optional[int] = 100,
                  override=True,
                  auto_start_session=True
                  ):
 
         self._session = None
         self._worker = None
         self._tags = tags
-        self.config = None
 
-        if not api_key and not environ.get('AGENTOPS_API_KEY'):
-            logging.warning("AgentOps: No API key provided - no data will be recorded.")
+        try:
+            self.config = Configuration(api_key=api_key,
+                                        parent_key=parent_key,
+                                        endpoint=endpoint,
+                                        max_wait_time=max_wait_time,
+                                        max_queue_size=max_queue_size)
+        except ConfigurationError:
             return
 
-        self.config = Configuration(api_key or environ.get('AGENTOPS_API_KEY'),
-                                    endpoint,
-                                    max_wait_time,
-                                    max_queue_size)
-
         self._handle_unclean_exits()
 
         if auto_start_session:
-            self.start_session(tags)
+            self.start_session(tags, self.config)
 
         if override:
             if 'openai' in sys.modules:
                 self.llm_tracker = LlmTracker(self)
                 self.llm_tracker.override_api('openai')
 
     def add_tags(self, tags: List[str]):
@@ -100,14 +106,17 @@
         Record an event with the AgentOps service.
 
         Args:
             event (Event): The event to record.
         """
 
         if self._session is not None and not self._session.has_ended:
+            agent_id = check_call_stack_for_agent_id()
+            if agent_id:
+                event.agent_id = agent_id
             self._worker.add_event(event.__dict__)
         else:
             logging.warning(
                 "AgentOps: Cannot record event - no current session")
 
     def _record_event_sync(self, func, event_name, *args, **kwargs):
         init_time = get_ISO_time()
@@ -203,33 +212,35 @@
 
         if not config and not self.config:
             return logging.warning("AgentOps: Cannot start session - missing configuration")
 
         self._session = Session(uuid4(), tags or self._tags, host_env=get_host_env())
         self._worker = Worker(config or self.config)
         self._worker.start_session(self._session)
-        logging.info('View info on this session at https://agentops.ai/dashboard?session_id={}'
+        logging.info('View info on this session at https://app.agentops.ai/dashboard?session_id={}'
                      .format(self._session.session_id))
 
-    def end_session(self, end_state: str = Field("Indeterminate",
-                                                 description="End state of the session",
-                                                 pattern="^(Success|Fail|Indeterminate)$"),
+    def end_session(self,
+                    end_state: str,
                     end_state_reason: Optional[str] = None,
                     video: Optional[str] = None):
         """
         End the current session with the AgentOps service.
 
         Args:
-            end_state (str, optional): The final state of the session.
+            end_state (str): The final state of the session. Options: Success, Fail, or Indeterminate.
             end_state_reason (str, optional): The reason for ending the session.
             video (str, optional): The video screen recording of the session
         """
         if self._session is None or self._session.has_ended:
             return logging.warning("AgentOps: Cannot end session - no current session")
 
+        if not any(end_state == state.value for state in EndState):
+            return logging.warning("AgentOps: Invalid end_state. Please use one of the EndState enums")
+
         self._session.video = video
         self._session.end_session(end_state, end_state_reason)
         self._worker.end_session(self._session)
         self._session = None
         self._worker = None
 
     def create_agent(self, agent_id: str, name: str):
@@ -272,15 +283,16 @@
 
             self.end_session(end_state='Fail',
                              end_state_reason=f"{str(exc_value)}: {formatted_traceback}")
 
             # Then call the default excepthook to exit the program
             sys.__excepthook__(exc_type, exc_value, exc_traceback)
 
-        atexit.register(lambda: cleanup(end_state="Success", end_state_reason="Process exited normally"))
+        atexit.register(lambda: cleanup(end_state="Indeterminate",
+                        end_state_reason="Process exited without calling end_session()"))
         signal.signal(signal.SIGINT, signal_handler)
         signal.signal(signal.SIGTERM, signal_handler)
         sys.excepthook = handle_exception
 
     @property
     def current_session_id(self):
         return self._session.session_id
```

### Comparing `agentops-0.1.0b4/agentops/decorators.py` & `agentops-0.1.0b5/agentops/decorators.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b4/agentops/enums.py` & `agentops-0.1.0b5/agentops/enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,10 +19,11 @@
     GPT_4 = "gpt-4"
     GPT_4_32K = "gpt-4-32k"
     GPT_4_32K_0314 = "gpt-4-32k-0314"
     GPT_4_0613 = "gpt-4-0613"
     TEXT_EMBEDDING_ADA_002 = "text-embedding-ada-002"
 
 
-class LLMMessageFormat(Enum):
-    STRING = "string"
-    CHATML = "chatml"
+class EndState(Enum):
+    SUCCESS = "Success"
+    FAIL = "Fail"
+    INDETERMINATE = "Indeterminate"
```

### Comparing `agentops-0.1.0b4/agentops/helpers.py` & `agentops-0.1.0b5/agentops/helpers.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b4/agentops/host_env.py` & `agentops-0.1.0b5/agentops/host_env.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b4/agentops/http_client.py` & `agentops-0.1.0b5/agentops/http_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,24 +57,28 @@
             return HttpStatus.FAILED
         return HttpStatus.UNKNOWN
 
 
 class HttpClient:
 
     @staticmethod
-    def post(url: str, payload: bytes, api_key: Optional[str] = None, header=None) -> Response:
+    def post(url: str, payload: bytes, api_key: Optional[str] = None, parent_key: Optional[str] = None,
+             header=None) -> Response:
         result = Response()
         try:
             # Create request session with retries configured
             request_session = requests.Session()
             request_session.mount(url, HTTPAdapter(max_retries=retry_config))
 
-            if api_key != None:
+            if api_key is not None:
                 JSON_HEADER["X-Agentops-Auth"] = api_key
 
+            if parent_key is not None:
+                JSON_HEADER["X-Agentops-Parent-Key"] = parent_key
+
             res = request_session.post(url, data=payload,
                                        headers=JSON_HEADER, timeout=20)
 
             result.parse(res)
         except requests.exceptions.Timeout:
             result.code = 408
             result.status = HttpStatus.TIMEOUT
@@ -89,15 +93,15 @@
                 result.status = Response.get_status(e.response.status_code)
                 result.body = {'error': str(e)}
         except requests.exceptions.RequestException as e:
             result.body = {'error': str(e)}
 
         if result.code == 401:
             logging.warning(
-                'AgentOps: Could not post data - API server rejected your API key')
+                f'AgentOps: Could not post data - API server rejected your API key: {api_key}')
         if result.code == 400:
             logging.warning(f'AgentOps: Could not post data - {result.body}')
         if result.code == 500:
             logging.warning(
                 f'AgentOps: Could not post data - internal server error')
 
         return result
```

### Comparing `agentops-0.1.0b4/agentops/langchain_callback_handler.py` & `agentops-0.1.0b5/agentops/langchain_callback_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from langchain.callbacks.base import BaseCallbackHandler, AsyncCallbackHandler
 from langchain_core.messages import BaseMessage
 
 from tenacity import RetryCallState
 
 from agentops import Client as AOClient
 from agentops import ActionEvent, LLMEvent, ToolEvent, ErrorEvent
-from agentops import LLMMessageFormat
 from agentops.helpers import get_ISO_time
 
 from .helpers import debug_print_function_params
 
 
 class Events:
     llm: Dict[str, LLMEvent] = {}
@@ -61,15 +60,15 @@
         **kwargs: Any,
     ) -> Any:
         self.events.llm[str(run_id)] = LLMEvent(
             params={**serialized,
                     **({} if metadata is None else metadata),
                     **kwargs},  # TODO: params is inconsistent, in ToolEvent we put it in logs
             model=kwargs['invocation_params']['model'],
-            prompt_messages=prompts[0]
+            prompt=prompts[0]
             # tags=tags # TODO
         )
 
     @debug_print_function_params
     def on_llm_error(
             self,
             error: BaseException,
@@ -96,25 +95,23 @@
         llm_event: LLMEvent = self.events.llm[str(run_id)]
         llm_event.returns = {
             "content": response.generations[0][0].message.content,
             "generations": response.generations
         }
         llm_event.end_timestamp = get_ISO_time()
         if response.llm_output is not None:
-            llm_event.completion_message = response.generations[0][0].message.content  # TODO
-            llm_event.completion_message_format = LLMMessageFormat.STRING  # TODO
+            llm_event.completion = response.generations[0][0].message.content  # TODO
             llm_event.prompt_tokens = response.llm_output['token_usage']['prompt_tokens']
             llm_event.completion_tokens = response.llm_output['token_usage']['completion_tokens']
-            llm_event.format_messages()  # TODO: Find somewhere logical to call this on the user's behalf. They shouldn't call it
         self.ao_client.record(llm_event)
 
         if len(response.generations) == 0:
             # TODO: more descriptive error
             error_event = ErrorEvent(trigger_event=self.events.llm[str(run_id)],
-                                    details="on_llm_end: No generations", timestamp=get_ISO_time())
+                                     details="on_llm_end: No generations", timestamp=get_ISO_time())
             self.ao_client.record(error_event)
 
     @debug_print_function_params
     def on_chain_start(
         self,
         serialized: Dict[str, Any],
         inputs: Dict[str, Any],
@@ -362,15 +359,15 @@
         **kwargs: Any,
     ) -> Any:
         self.events.llm[str(run_id)] = LLMEvent(
             params={**serialized,
                     **({} if metadata is None else metadata),
                     **kwargs},  # TODO: params is inconsistent, in ToolEvent we put it in logs
             model=kwargs['invocation_params']['model'],
-            prompt_messages=prompts[0]
+            prompt=prompts[0]
         )
 
     @debug_print_function_params
     async def on_chat_model_start(
         self,
         serialized: Dict[str, Any],
         messages: List[List[BaseMessage]],
@@ -423,25 +420,23 @@
         llm_event: LLMEvent = self.events.llm[str(run_id)]
         llm_event.returns = {
             "content": response.generations[0][0].message.content,
             "generations": response.generations
         }
         llm_event.end_timestamp = get_ISO_time()
         if response.llm_output is not None:
-            llm_event.completion_message = response.generations[0][0].message.content  # TODO
-            llm_event.completion_message_format = LLMMessageFormat.STRING  # TODO
+            llm_event.completion = response.generations[0][0].message.content  # TODO
             llm_event.prompt_tokens = response.llm_output['token_usage']['prompt_tokens']
             llm_event.completion_tokens = response.llm_output['token_usage']['completion_tokens']
-            llm_event.format_messages()  # TODO: Find somewhere logical to call this on the user's behalf. They shouldn't call it
         self.ao_client.record(llm_event)
 
         if len(response.generations) == 0:
             # TODO: more descriptive error
             error_event = ErrorEvent(trigger_event=self.events.llm[str(run_id)],
-                                    details="on_llm_end: No generations", timestamp=get_ISO_time())
+                                     details="on_llm_end: No generations", timestamp=get_ISO_time())
             self.ao_client.record(error_event)
 
     @debug_print_function_params
     async def on_chain_start(
         self,
         serialized: Dict[str, Any],
         inputs: Dict[str, Any],
```

### Comparing `agentops-0.1.0b4/agentops/llm_tracker.py` & `agentops-0.1.0b5/agentops/llm_tracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import sys
 from importlib import import_module
 from packaging.version import parse
 import logging
 from .event import LLMEvent, ErrorEvent
 from .helpers import get_ISO_time, check_call_stack_for_agent_id
 import inspect
-from .enums import LLMMessageFormat
 
 
 class LlmTracker:
     SUPPORTED_APIS = {
         'openai': {
             '1.0.0': (
                 "chat.completions.create",
@@ -37,31 +36,29 @@
         def handle_stream_chunk(chunk):
             self.llm_event = LLMEvent(
                 init_timestamp=init_timestamp,
                 params=kwargs
             )
 
             try:
+                # NOTE: prompt/completion usage not returned in response when streaming
                 model = chunk['model']
                 choices = chunk['choices']
                 token = choices[0]['delta'].get('content', '')
                 finish_reason = choices[0]['finish_reason']
                 if token:
                     self.completion += token
 
                 if finish_reason:
                     self.llm_event.agent_id = check_call_stack_for_agent_id()
-                    self.llm_event.prompt_messages = kwargs["messages"]
-                    self.llm_event.prompt_messages_format = LLMMessageFormat.CHATML
-                    self.llm_event.completion_message = {"role": "assistant", "content": self.completion}
-                    self.llm_event.completion_message_format = LLMMessageFormat.CHATML
+                    self.llm_event.prompt = kwargs["messages"]
+                    self.llm_event.completion = {"role": "assistant", "content": self.completion}
                     self.llm_event.returns = {"finish_reason": finish_reason, "content": self.completion}
                     self.llm_event.model = model
                     self.llm_event.end_timestamp = get_ISO_time()
-                    self.llm_event.format_messages()
 
                     self.client.record(self.llm_event)
             except Exception as e:
                 self.client.record(ErrorEvent(trigger_event=self.llm_event, details={f"{type(e).__name__}": str(e)}))
                 # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
                 logging.warning(
                     f"AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
@@ -86,22 +83,21 @@
         self.llm_event = LLMEvent(
             init_timestamp=init_timestamp,
             params=kwargs
         )
         # v0.0.0 responses are dicts
         try:
             self.llm_event.agent_id = check_call_stack_for_agent_id()
-            self.llm_event.prompt_messages = kwargs["messages"]
-            self.llm_event.prompt_messages_format = LLMMessageFormat.CHATML
-            self.llm_event.completion_message = response['choices'][0]['message']
-            self.llm_event.completion_message_format = LLMMessageFormat.CHATML
+            self.llm_event.prompt = kwargs["messages"]
+            self.llm_event.prompt_tokens = response['usage']['prompt_tokens']
+            self.llm_event.completion = response['choices'][0]['message']['content']
+            self.llm_event.completion_tokens = response['usage']['completion_tokens']
             self.llm_event.returns = {"content": response['choices'][0]['message']['content']}
             self.llm_event.model = response["model"]
             self.llm_event.end_timestamp = get_ISO_time()
-            self.llm_event.format_messages()
 
             self.client.record(self.llm_event)
         except Exception as e:
             self.client.record(ErrorEvent(trigger_event=self.llm_event, details={f"{type(e).__name__}": str(e)}))
             # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
             logging.warning(
                 f"AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
@@ -121,35 +117,33 @@
 
             self.llm_event = LLMEvent(
                 init_timestamp=init_timestamp,
                 params=kwargs
             )
 
             try:
+                # NOTE: prompt/completion usage not returned in response when streaming
                 model = chunk.model
                 choices = chunk.choices
                 token = choices[0].delta.content
                 finish_reason = choices[0].finish_reason
                 function_call = choices[0].delta.function_call
                 tool_calls = choices[0].delta.tool_calls
                 role = choices[0].delta.role
                 if token:
                     self.completion += token
 
                 if finish_reason:
                     self.llm_event.agent_id = check_call_stack_for_agent_id()
-                    self.llm_event.prompt_messages = kwargs["messages"]
-                    self.llm_event.prompt_messages_format = LLMMessageFormat.CHATML
-                    self.llm_event.completion_message = {"role": "assistant", "content": self.completion}
-                    self.llm_event.completion_message_format = LLMMessageFormat.CHATML
+                    self.llm_event.prompt = kwargs["messages"]
+                    self.llm_event.completion = {"role": "assistant", "content": self.completion}
                     self.llm_event.returns = {"finish_reason": finish_reason, "content": self.completion,
                                               "function_call": function_call, "tool_calls": tool_calls, "role": role}
                     self.llm_event.model = model
                     self.llm_event.end_timestamp = get_ISO_time()
-                    self.llm_event.format_messages()
 
                     self.client.record(self.llm_event)
             except Exception as e:
                 self.client.record(ErrorEvent(trigger_event=self.llm_event, details={f"{type(e).__name__}": str(e)}))
                 # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
                 logging.warning(
                     f"AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
@@ -181,21 +175,20 @@
         self.llm_event = LLMEvent(
             init_timestamp=init_timestamp,
             params=kwargs
         )
         # v1.0.0+ responses are objects
         try:
             self.llm_event.agent_id = check_call_stack_for_agent_id()
-            self.llm_event.prompt_messages = kwargs["messages"]
-            self.llm_event.prompt_messages_format = LLMMessageFormat.CHATML
-            self.llm_event.completion_message = response.choices[0].message.model_dump()
-            self.llm_event.completion_message_format = LLMMessageFormat.CHATML
+            self.llm_event.prompt = kwargs["messages"]
+            self.llm_event.prompt_tokens = response.usage.prompt_tokens
+            self.llm_event.completion = response.choices[0].message.model_dump().get('content')
+            self.llm_event.completion_tokens = response.usage.completion_tokens
             self.llm_event.returns = response.model_dump()
             self.llm_event.model = response.model
-            self.llm_event.format_messages()
 
             self.client.record(self.llm_event)
         except Exception as e:
             self.client.record(ErrorEvent(trigger_event=self.llm_event, details={f"{type(e).__name__}": str(e)}))
             # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
             logging.warning(
                 f"AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
```

### Comparing `agentops-0.1.0b4/agentops/meta_client.py` & `agentops-0.1.0b5/agentops/meta_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,12 +41,14 @@
 def handle_exceptions(method):
     """Decorator within the metaclass to wrap method execution in try-except block."""
 
     def wrapper(self, *args, **kwargs):
         try:
             return method(self, *args, **kwargs)
         except Exception as e:
-            type(self).send_exception_to_server(e, self.config._api_key)
             logging.warning(f"AgentOps: Error: {e}")
+            config = getattr(self, 'config', None)
+            if config is not None:
+                type(self).send_exception_to_server(e, self.config._api_key)
             raise e
 
-    return wrapper
+    return wrapper
```

### Comparing `agentops-0.1.0b4/agentops/session.py` & `agentops-0.1.0b5/agentops/session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b4/agentops/worker.py` & `agentops-0.1.0b5/agentops/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import threading
 import time
 from .http_client import HttpClient
-from .config import Configuration
+from .config import Configuration, ConfigurationError
 from .session import Session
 from .helpers import safe_serialize, filter_unjsonable
 from typing import Dict
 
 
 class Worker:
     def __init__(self, config: Configuration) -> None:
@@ -35,66 +35,70 @@
                     "session_id": self._session.session_id,
                     "events": events
                 }
 
                 serialized_payload = safe_serialize(payload).encode("utf-8")
                 HttpClient.post(f'{self.config.endpoint}/events',
                                 serialized_payload,
-                                self.config.api_key)
+                                self.config.api_key,
+                                self.config.parent_key)
 
     def start_session(self, session: Session) -> None:
         self._session = session
         with self.lock:
             payload = {
                 "session": session.__dict__
             }
             serialized_payload = json.dumps(filter_unjsonable(payload)).encode("utf-8")
             HttpClient.post(f'{self.config.endpoint}/sessions',
                             serialized_payload,
-                            self.config.api_key)
+                            self.config.api_key,
+                            self.config.parent_key)
 
     def end_session(self, session: Session) -> None:
         self.stop_flag.set()
-        self.thread.join()
+        self.thread.join(timeout=1)
         self.flush_queue()
         self._session = None
 
         with self.lock:
             payload = {
                 "session": session.__dict__
             }
 
             HttpClient.post(f'{self.config.endpoint}/sessions',
                             json.dumps(filter_unjsonable(
                                 payload)).encode("utf-8"),
-                            self.config.api_key)
+                            self.config.api_key,
+                            self.config.parent_key)
 
     def update_session(self, session: Session) -> None:
         with self.lock:
             payload = {
                 "session": session.__dict__
             }
 
             HttpClient.post(f'{self.config.endpoint}/sessions',
                             json.dumps(filter_unjsonable(
                                 payload)).encode("utf-8"),
                             self.config.api_key,
-                            self.config.org_key)
+                            self.config.parent_key)
 
     def create_agent(self, agent_id, name):
         payload = {
             "id": agent_id,
             "name": name,
             "session_id": self._session.session_id
         }
 
         serialized_payload = \
             safe_serialize(payload).encode("utf-8")
         HttpClient.post(f'{self.config.endpoint}/agents',
                         serialized_payload,
-                        self.config.api_key)
+                        self.config.api_key,
+                        self.config.parent_key)
 
     def run(self) -> None:
         while not self.stop_flag.is_set():
             time.sleep(self.config.max_wait_time / 1000)
             if self.queue:
                 self.flush_queue()
```

### Comparing `agentops-0.1.0b4/agentops.egg-info/PKG-INFO` & `agentops-0.1.0b5/agentops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.0b4
+Version: 0.1.0b5
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
-Requires-Dist: pydantic>=1.9.0
-Requires-Dist: packaging<24.0,>=23.1
-Requires-Dist: toml>=0.10.2
 Requires-Dist: psutil==5.9.8
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: requests_mock==1.11.0; extra == "dev"
 Provides-Extra: langchain
 Requires-Dist: langchain>=0.0.354; extra == "langchain"
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.0b4 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.0b5 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests==2.31.0 Requires-Dist: pydantic>=1.9.0 Requires-Dist:
-packaging<24.0,>=23.1 Requires-Dist: toml>=0.10.2 Requires-Dist: psutil==5.9.8
-Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
-requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
-langchain>=0.0.354; extra == "langchain"
+requests==2.31.0 Requires-Dist: psutil==5.9.8 Provides-Extra: dev Requires-
+Dist: pytest==7.4.0; extra == "dev" Requires-Dist: requests_mock==1.11.0; extra
+== "dev" Provides-Extra: langchain Requires-Dist: langchain>=0.0.354; extra ==
+"langchain"
                                     [Logo]
                             _D_o_c_u_m_e_n_t_a_t_i_o_n | _D_i_s_c_o_r_d
                      AI agents suck. Weâre fixing that.
 Build your next agent with benchmarks, observability, and replay analytics.
 AgentOps is the toolkit for evaluating and developing robust and reliable AI
 agents. AgentOps is open beta. You can sign up for AgentOps [here](https://
 app.agentops.ai). [![License: MIT](https://img.shields.io/badge/License-MIT-
```

### Comparing `agentops-0.1.0b4/agentops.egg-info/SOURCES.txt` & `agentops-0.1.0b5/agentops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b4/pyproject.toml` & `agentops-0.1.0b5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "agentops"
-version = "0.1.0-beta.4"
+version = "0.1.0-beta.5"
 authors = [
   { name="Alex Reibman", email="areibman@gmail.com" },
   { name="Shawn Qiu", email="siyangqiu@gmail.com" },
   { name="Braelyn Boynton", email="bboynton97@gmail.com" },
   { name="Howard Gil", email="howardbgil@gmail.com" }
 ]
 description = "Python SDK for developing AI agent evals and observability"
@@ -17,17 +17,14 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests==2.31.0",
-    "pydantic>=1.9.0",
-    "packaging>=23.1,<24.0",
-    "toml>=0.10.2",
     "psutil==5.9.8"
 ]
 [project.optional-dependencies]
 dev = [
     "pytest==7.4.0",
     "requests_mock==1.11.0"
 ]
```

### Comparing `agentops-0.1.0b4/tests/test_canary.py` & `agentops-0.1.0b5/tests/test_canary.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b4/tests/test_patcher.py` & `agentops-0.1.0b5/tests/test_patcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import pytest
-from unittest.mock import MagicMock
-from agentops.llm_tracker import LlmTracker
-
-# Mock the openai library
-
-
-@pytest.fixture
-def mock_openai(mocker):
-    mock = mocker.MagicMock()
-    mocker.patch.dict('sys.modules', {'openai': mock})
-    return mock
-
-# Test that the correct methods are overridden for version >= 1.0.0
-
-
-def test_override_api_version_ge_1(mock_openai):
-    mock_openai.__version__ = '1.0.0'  # Version is exactly 1.0.0
-    tracker = LlmTracker(client=MagicMock())
-
-    original_method = MagicMock()
-    mock_openai.chat = MagicMock(completions=MagicMock(create=original_method))
-
-    tracker.override_api('openai')
-
-    # The original method should be replaced with a new method
-    assert mock_openai.chat.completions.create != original_method
-    assert callable(mock_openai.chat.completions.create)
-
-# Test that the correct methods are overridden for version < 1.0.0
-
-
-def test_override_api_version_lt_1(mock_openai):
-    mock_openai.__version__ = '0.9.9'  # Version is less than 1.0.0
-    tracker = LlmTracker(client=MagicMock())
-
-    original_method = MagicMock()
-    mock_openai.ChatCompletion = MagicMock(create=original_method)
-
-    tracker.override_api('openai')
-
-    # The original method should be replaced with a new method
-    assert mock_openai.ChatCompletion.create != original_method
-    assert callable(mock_openai.ChatCompletion.create)
-
-# Test that the override_api method handles missing __version__ attribute
-
-
-def test_override_api_missing_version_attribute(mocker):
-    mock_openai = mocker.MagicMock()
-    mocker.patch.dict('sys.modules', {'openai': mock_openai})
-    tracker = LlmTracker(client=MagicMock())
-
-    # This should not raise an error, and should use the methods for version < 1.0.0
-    tracker.override_api('openai')
-
-    # Now you need to assert that the correct methods for version < 1.0.0 are overridden
-    # Assuming 'ChatCompletion.create' is the method to be overridden for version < 1.0.0
-    assert hasattr(mock_openai, 'ChatCompletion')
-    assert callable(mock_openai.ChatCompletion.create)
+# import pytest
+# from unittest.mock import MagicMock
+# from agentops.llm_tracker import LlmTracker
+#
+# # Mock the openai library
+#
+#
+# @pytest.fixture
+# def mock_openai(mocker):
+#     mock = mocker.MagicMock()
+#     mocker.patch.dict('sys.modules', {'openai': mock})
+#     return mock
+#
+# # Test that the correct methods are overridden for version >= 1.0.0
+#
+#
+# def test_override_api_version_ge_1(mock_openai):
+#     mock_openai.__version__ = '1.0.0'  # Version is exactly 1.0.0
+#     tracker = LlmTracker(client=MagicMock())
+#
+#     original_method = MagicMock()
+#     mock_openai.chat = MagicMock(completions=MagicMock(create=original_method))
+#
+#     tracker.override_api('openai')
+#
+#     # The original method should be replaced with a new method
+#     assert mock_openai.chat.completions.create != original_method
+#     assert callable(mock_openai.chat.completions.create)
+#
+# # Test that the correct methods are overridden for version < 1.0.0
+#
+#
+# def test_override_api_version_lt_1(mock_openai):
+#     mock_openai.__version__ = '0.9.9'  # Version is less than 1.0.0
+#     tracker = LlmTracker(client=MagicMock())
+#
+#     original_method = MagicMock()
+#     mock_openai.ChatCompletion = MagicMock(create=original_method)
+#
+#     tracker.override_api('openai')
+#
+#     # The original method should be replaced with a new method
+#     assert mock_openai.ChatCompletion.create != original_method
+#     assert callable(mock_openai.ChatCompletion.create)
+#
+# # Test that the override_api method handles missing __version__ attribute
+#
+#
+# def test_override_api_missing_version_attribute(mocker):
+#     mock_openai = mocker.MagicMock()
+#     mocker.patch.dict('sys.modules', {'openai': mock_openai})
+#     tracker = LlmTracker(client=MagicMock())
+#
+#     # This should not raise an error, and should use the methods for version < 1.0.0
+#     tracker.override_api('openai')
+#
+#     # Now you need to assert that the correct methods for version < 1.0.0 are overridden
+#     # Assuming 'ChatCompletion.create' is the method to be overridden for version < 1.0.0
+#     assert hasattr(mock_openai, 'ChatCompletion')
+#     assert callable(mock_openai.ChatCompletion.create)
```

### Comparing `agentops-0.1.0b4/tests/test_record_function.py` & `agentops-0.1.0b5/tests/test_record_function.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b4/tests/test_session.py` & `agentops-0.1.0b5/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b4/tests/test_teardown.py` & `agentops-0.1.0b5/tests/test_teardown.py`

 * *Files identical despite different names*

