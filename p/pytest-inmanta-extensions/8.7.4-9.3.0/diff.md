# Comparing `tmp/pytest-inmanta-extensions-8.7.4.tar.gz` & `tmp/pytest-inmanta-extensions-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-inmanta-extensions-8.7.4.tar", last modified: Fri Mar 29 14:31:11 2024, max compression
+gzip compressed data, was "pytest-inmanta-extensions-9.3.0.tar", last modified: Tue Jul  4 11:30:21 2023, max compression
```

## Comparing `pytest-inmanta-extensions-8.7.4.tar` & `pytest-inmanta-extensions-9.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 jenkins    (989) jenkins    (986)        0 2024-03-29 14:31:11.490899 pytest-inmanta-extensions-8.7.4/
--rw-rw-r--   0 jenkins    (989) jenkins    (986)      199 2024-03-29 14:26:48.000000 pytest-inmanta-extensions-8.7.4/MANIFEST.in
--rw-r--r--   0 jenkins    (989) jenkins    (986)     1561 2024-03-29 14:31:11.490899 pytest-inmanta-extensions-8.7.4/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (986)      467 2024-03-29 14:26:48.000000 pytest-inmanta-extensions-8.7.4/README.md
--rw-rw-r--   0 jenkins    (989) jenkins    (986)       59 2024-03-29 14:31:11.490899 pytest-inmanta-extensions-8.7.4/setup.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (986)     2483 2024-03-29 14:26:48.000000 pytest-inmanta-extensions-8.7.4/setup.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (986)        0 2024-03-29 14:31:11.486899 pytest-inmanta-extensions-8.7.4/src/
-drwxrwxr-x   0 jenkins    (989) jenkins    (986)        0 2024-03-29 14:31:11.487898 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/
--rw-rw-r--   0 jenkins    (989) jenkins    (986)      627 2024-03-29 14:26:48.000000 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (986)    72709 2024-03-29 14:30:50.000000 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/conftest.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (986)        0 2024-03-29 14:31:11.488899 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/
-drwxrwxr-x   0 jenkins    (989) jenkins    (986)        0 2024-03-29 14:31:11.486899 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/ca/
-drwxrwxr-x   0 jenkins    (989) jenkins    (986)        0 2024-03-29 14:31:11.488899 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/ca/enduser-certs/
--rw-rw-r--   0 jenkins    (989) jenkins    (986)     6223 2024-03-29 14:26:48.000000 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/ca/enduser-certs/server.chain
--rw-rw-r--   0 jenkins    (989) jenkins    (986)     2069 2024-03-29 14:26:48.000000 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/ca/enduser-certs/server.crt
--rw-rw-r--   0 jenkins    (989) jenkins    (986)     3243 2024-03-29 14:26:48.000000 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/ca/enduser-certs/server.key
--rw-rw-r--   0 jenkins    (989) jenkins    (986)     3243 2024-03-29 14:26:48.000000 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/ca/enduser-certs/server.key.open
--rw-rw-r--   0 jenkins    (989) jenkins    (986)     1237 2024-03-29 14:30:50.000000 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/server.crt
--rw-rw-r--   0 jenkins    (989) jenkins    (986)     1679 2024-03-29 14:30:50.000000 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/server.open.key
-drwxrwxr-x   0 jenkins    (989) jenkins    (986)        0 2024-03-29 14:31:11.488899 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/db/
--rw-rw-r--   0 jenkins    (989) jenkins    (986)      980 2024-03-29 14:30:50.000000 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/db/common.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (986)        0 2024-03-29 14:31:11.489899 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/db/simple_project/
--rw-rw-r--   0 jenkins    (989) jenkins    (986)      212 2024-03-29 14:26:48.000000 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/db/simple_project/main.cf
--rw-rw-r--   0 jenkins    (989) jenkins    (986)      185 2024-03-29 14:26:48.000000 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/db/simple_project/project.yml
--rw-rw-r--   0 jenkins    (989) jenkins    (986)      685 2024-03-29 14:26:48.000000 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/plugin.py
--rw-rw-r--   0 jenkins    (989) jenkins    (986)    26335 2024-03-29 14:30:50.000000 pytest-inmanta-extensions-8.7.4/src/inmanta_tests/utils.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (986)        0 2024-03-29 14:31:11.490899 pytest-inmanta-extensions-8.7.4/src/pytest_inmanta_extensions.egg-info/
--rw-r--r--   0 jenkins    (989) jenkins    (986)     1561 2024-03-29 14:31:11.000000 pytest-inmanta-extensions-8.7.4/src/pytest_inmanta_extensions.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (986)      882 2024-03-29 14:31:11.000000 pytest-inmanta-extensions-8.7.4/src/pytest_inmanta_extensions.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (986)        1 2024-03-29 14:31:11.000000 pytest-inmanta-extensions-8.7.4/src/pytest_inmanta_extensions.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (986)       55 2024-03-29 14:31:11.000000 pytest-inmanta-extensions-8.7.4/src/pytest_inmanta_extensions.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (986)      124 2024-03-29 14:31:11.000000 pytest-inmanta-extensions-8.7.4/src/pytest_inmanta_extensions.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (986)       14 2024-03-29 14:31:11.000000 pytest-inmanta-extensions-8.7.4/src/pytest_inmanta_extensions.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.851827 pytest-inmanta-extensions-9.3.0/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      199 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/MANIFEST.in
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-07-04 11:30:21.851827 pytest-inmanta-extensions-9.3.0/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      467 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/README.md
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       59 2023-07-04 11:30:21.852827 pytest-inmanta-extensions-9.3.0/setup.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2481 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/setup.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.848827 pytest-inmanta-extensions-9.3.0/src/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.849827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    70339 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/conftest.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.850827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.848827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.850827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6223 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.chain
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2069 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.crt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1237 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/server.crt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1679 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/server.open.key
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.850827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      980 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/common.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.851827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/simple_project/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      212 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/simple_project/main.cf
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      185 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/simple_project/project.yml
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      685 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/plugin.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    25613 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/utils.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.851827 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      882 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       55 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      122 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       14 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/top_level.txt
```

### Comparing `pytest-inmanta-extensions-8.7.4/setup.py` & `pytest-inmanta-extensions-9.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
     Contact: code@inmanta.com
 """
 from os import path
 
 from setuptools import find_namespace_packages, setup
 
-version = "8.7.4"
+version = "9.3.0"
 
 requires = [
     "asyncpg",
     "click",
-    f"inmanta-core~={version}.0.dev",
+    f"inmanta-core~={version}.dev",
     "pip2pi",
     "pyformance",
     "pytest-asyncio",
     "pytest-env",
     "pytest-postgresql>=4",
     "psycopg>=3",
     "tornado",
```

### Comparing `pytest-inmanta-extensions-8.7.4/src/inmanta_tests/__init__.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.7.4/src/inmanta_tests/conftest.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
 import warnings
 
-from tornado.httpclient import AsyncHTTPClient
-
 import toml
 from inmanta.config import AuthJWTConfig
 from inmanta.logging import InmantaLoggerConfig
 
 """
 About the use of @parametrize_any and @slowtest:
 
@@ -80,17 +78,16 @@
 import sys
 import tempfile
 import time
 import traceback
 import uuid
 import venv
 from collections import abc
-from collections.abc import AsyncIterator, Awaitable, Callable, Iterator
 from configparser import ConfigParser
-from typing import Dict, Optional, Union
+from typing import AsyncIterator, Awaitable, Callable, Dict, Iterator, List, Optional, Tuple, Union
 
 import asyncpg
 import pkg_resources
 import psutil
 import py
 import pyformance
 import pytest
@@ -114,15 +111,15 @@
 from inmanta.agent.agent import Agent
 from inmanta.ast import CompilerException
 from inmanta.data.schema import SCHEMA_VERSION_TABLE
 from inmanta.db import util as db_util
 from inmanta.env import LocalPackagePath, VirtualEnv, mock_process_env
 from inmanta.export import ResourceDict, cfg_env, unknown_parameters
 from inmanta.module import InmantaModuleRequirement, InstallMode, Project, RelationPrecedenceRule
-from inmanta.moduletool import DefaultIsolatedEnvCached, ModuleTool, V2ModuleBuilder
+from inmanta.moduletool import IsolatedEnvBuilderCached, ModuleTool, V2ModuleBuilder
 from inmanta.parser.plyInmantaParser import cache_manager
 from inmanta.protocol import VersionMatch
 from inmanta.server import SLICE_AGENT_MANAGER, SLICE_COMPILER
 from inmanta.server.bootloader import InmantaBootloader
 from inmanta.server.protocol import Server, SliceStartupException
 from inmanta.server.services import orchestrationservice
 from inmanta.server.services.compilerservice import CompilerService, CompileRun
@@ -250,15 +247,15 @@
 
     logger.info("Using database fixture %s", fixture)
     pg = request.getfixturevalue(fixture)
     yield pg
 
     if os.path.exists(pg_logfile):
         has_deadlock = False
-        with open(pg_logfile) as fh:
+        with open(pg_logfile, "r") as fh:
             for line in fh:
                 if "deadlock" in line:
                     has_deadlock = True
                     break
             sublogger = logging.getLogger("pytest.postgresql.deadlock")
             for line in fh:
                 sublogger.warning("%s", line)
@@ -266,15 +263,15 @@
         assert not has_deadlock
 
 
 @pytest.fixture
 async def run_without_keeping_psql_logs(postgres_db):
     if os.path.exists(pg_logfile):
         # Store the original content of the logfile
-        with open(pg_logfile) as file:
+        with open(pg_logfile, "r") as file:
             original_content = file.read()
     yield
 
     if os.path.exists(pg_logfile):
         # Restore the original content of the logfile
         with open(pg_logfile, "w") as file:
             file.write(original_content)
@@ -418,86 +415,63 @@
         if tables_to_truncate:
             truncate_query = "TRUNCATE %s CASCADE" % ", ".join(tables_to_truncate)
             await postgresql_client.execute(truncate_query)
 
 
 @pytest.fixture(scope="function")
 def get_columns_in_db_table(postgresql_client):
-    async def _get_columns_in_db_table(table_name: str) -> list[str]:
+    async def _get_columns_in_db_table(table_name: str) -> List[str]:
         result = await postgresql_client.fetch(
             "SELECT column_name "
             "FROM information_schema.columns "
             "WHERE table_schema='public' AND table_name='" + table_name + "'"
         )
         return [r["column_name"] for r in result]
 
     return _get_columns_in_db_table
 
 
 @pytest.fixture(scope="function")
 def get_primary_key_columns_in_db_table(postgresql_client):
-    async def _get_primary_key_columns_in_db_table(table_name: str) -> list[str]:
+    async def _get_primary_key_columns_in_db_table(table_name: str) -> List[str]:
         # Query taken from here: https://wiki.postgresql.org/wiki/Retrieve_primary_key_columns
         result = await postgresql_client.fetch(
             "SELECT a.attname FROM pg_index i "
             "JOIN pg_attribute a ON a.attrelid = i.indrelid AND a.attnum = ANY(i.indkey) "
             "WHERE i.indrelid = '" + table_name + "'::regclass "
             "AND i.indisprimary;"
         )
         return [r["attname"] for r in result]
 
     return _get_primary_key_columns_in_db_table
 
 
 @pytest.fixture(scope="function")
 def get_tables_in_db(postgresql_client):
-    async def _get_tables_in_db() -> list[str]:
+    async def _get_tables_in_db() -> List[str]:
         result = await postgresql_client.fetch("SELECT table_name FROM information_schema.tables WHERE table_schema='public'")
         return [r["table_name"] for r in result]
 
     return _get_tables_in_db
 
 
 @pytest.fixture(scope="function")
-def get_custom_postgresql_types(postgresql_client) -> Callable[[], Awaitable[list[str]]]:
+def get_custom_postgresql_types(postgresql_client) -> Callable[[], Awaitable[List[str]]]:
     """
     Fixture that returns an async callable that returns all the custom types defined
     in the PostgreSQL database.
     """
 
-    async def f() -> list[str]:
+    async def f() -> List[str]:
         return await db_util.postgres_get_custom_types(postgresql_client)
 
     return f
 
 
 @pytest.fixture(scope="function")
-def get_type_of_column(postgresql_client) -> Callable[[], Awaitable[Optional[str]]]:
-    """
-    Fixture that returns the type of a column in a table
-    """
-
-    async def _get_type_of_column(table_name: str, column_name: str) -> Optional[str]:
-        data_type = await postgresql_client.fetchval(
-            """
-                SELECT data_type
-                FROM information_schema.columns
-                WHERE table_schema = 'public'
-                    AND table_name = $1
-                    AND column_name = $2;
-            """,
-            table_name,
-            column_name,
-        )
-        return data_type
-
-    return _get_type_of_column
-
-
-@pytest.fixture(scope="function")
 def deactive_venv():
     old_os_path = os.environ.get("PATH", "")
     old_prefix = sys.prefix
     old_path = list(sys.path)
     old_meta_path = sys.meta_path.copy()
     old_path_hooks = sys.path_hooks.copy()
     old_pythonpath = os.environ.get("PYTHONPATH", None)
@@ -558,37 +532,36 @@
 
 @pytest.fixture(scope="session", autouse=True)
 def clean_reset_session():
     """
     Execute cleanup tasks that should only run at the end of the test suite.
     """
     yield
-    DefaultIsolatedEnvCached.get_instance().destroy()
+    IsolatedEnvBuilderCached.get_instance().destroy()
 
 
 def reset_all_objects():
     resources.resource.reset()
     asyncio.set_child_watcher(None)
     reset_metrics()
     # No dynamic loading of commands at the moment, so no need to reset/reload
     # command.Commander.reset()
     handler.Commander.reset()
     Project._project = None
     unknown_parameters.clear()
     InmantaBootloader.AVAILABLE_EXTENSIONS = None
-    V2ModuleBuilder.DISABLE_DEFAULT_ISOLATED_ENV_CACHED = False
+    V2ModuleBuilder.DISABLE_ISOLATED_ENV_BUILDER_CACHE = False
     compiler.Finalizers.reset_finalizers()
     AuthJWTConfig.reset()
     InmantaLoggerConfig.clean_instance()
-    AsyncHTTPClient.configure(None)
 
 
 @pytest.fixture()
 def disable_isolated_env_builder_cache() -> None:
-    V2ModuleBuilder.DISABLE_DEFAULT_ISOLATED_ENV_CACHED = True
+    V2ModuleBuilder.DISABLE_ISOLATED_ENV_BUILDER_CACHE = True
 
 
 @pytest.fixture(scope="function", autouse=True)
 def restore_cwd():
     """
     Restore the current working directory after search test.
     """
@@ -677,17 +650,17 @@
     config.Config.set("config", "agent-repair-interval", "0")
 
     started_agents = []
 
     async def create_agent(
         environment: uuid.UUID,
         hostname: Optional[str] = None,
-        agent_map: Optional[dict[str, str]] = None,
+        agent_map: Optional[Dict[str, str]] = None,
         code_loader: bool = False,
-        agent_names: list[str] = [],
+        agent_names: List[str] = [],
     ) -> None:
         a = Agent(hostname=hostname, environment=environment, agent_map=agent_map, code_loader=code_loader)
         for agent_name in agent_names:
             await a.add_end_point_name(agent_name)
         await a.start()
         started_agents.append(a)
         await utils.retry_limited(lambda: a.sessionid in agentmanager.sessions, 10)
@@ -761,22 +734,19 @@
 @pytest.fixture(scope="function")
 async def server_config(event_loop, inmanta_config, postgres_db, database_name, clean_reset, unused_tcp_port_factory):
     reset_metrics()
 
     with tempfile.TemporaryDirectory() as state_dir:
         port = str(unused_tcp_port_factory())
 
-        # Config.set() always expects a string value
-        pg_password = "" if postgres_db.password is None else postgres_db.password
-
         config.Config.set("database", "name", database_name)
         config.Config.set("database", "host", "localhost")
         config.Config.set("database", "port", str(postgres_db.port))
         config.Config.set("database", "username", postgres_db.user)
-        config.Config.set("database", "password", pg_password)
+        config.Config.set("database", "password", postgres_db.password)
         config.Config.set("database", "connection_timeout", str(3))
         config.Config.set("config", "state-dir", state_dir)
         config.Config.set("config", "log-dir", os.path.join(state_dir, "logs"))
         config.Config.set("agent_rest_transport", "port", port)
         config.Config.set("compiler_rest_transport", "port", port)
         config.Config.set("client_rest_transport", "port", port)
         config.Config.set("cmdline_rest_transport", "port", port)
@@ -859,23 +829,20 @@
                 config.Config.set(x, "ssl_key_file", os.path.join(capath, "server.key.open"))
                 config.Config.set(x, "ssl_ca_cert_file", os.path.join(capath, "server.chain"))
                 config.Config.set(x, "ssl", "True")
             if auth and ct is not None:
                 token = protocol.encode_token(ct)
                 config.Config.set(x, "token", token)
 
-        # Config.set() always expects a string value
-        pg_password = "" if postgres_db.password is None else postgres_db.password
-
         port = str(unused_tcp_port_factory())
         config.Config.set("database", "name", database_name)
         config.Config.set("database", "host", "localhost")
         config.Config.set("database", "port", str(postgres_db.port))
         config.Config.set("database", "username", postgres_db.user)
-        config.Config.set("database", "password", pg_password)
+        config.Config.set("database", "password", postgres_db.password)
         config.Config.set("database", "connection_timeout", str(3))
         config.Config.set("config", "state-dir", state_dir)
         config.Config.set("config", "log-dir", os.path.join(state_dir, "logs"))
         config.Config.set("agent_rest_transport", "port", port)
         config.Config.set("compiler_rest_transport", "port", port)
         config.Config.set("client_rest_transport", "port", port)
         config.Config.set("cmdline_rest_transport", "port", port)
@@ -1034,15 +1001,15 @@
         schema_update_file = os.path.join(schema_updates_dir, str(schema_version) + ".sql")
         with open(schema_update_file, "w+", encoding="utf-8") as f:
             f.write(content_file)
 
     yield _write_db_update_file
 
 
-class KeepOnFail:
+class KeepOnFail(object):
     def keep(self) -> "Optional[Dict[str, str]]":
         pass
 
 
 @pytest.hookimpl(tryfirst=True, hookwrapper=True)
 def pytest_runtest_makereport(item, call):
     # execute all other hooks to obtain the report object
@@ -1057,28 +1024,30 @@
                 msg = fixture.keep()
                 if msg:
                     for label, res in msg.items():
                         resources[label] = res
 
         if resources:
             # we are behind report formatting, so write to report, not item
-            rep.sections.append(("Resources Kept", "\n".join([f"{label} {resource}" for label, resource in resources.items()])))
+            rep.sections.append(
+                ("Resources Kept", "\n".join(["%s %s" % (label, resource) for label, resource in resources.items()]))
+            )
 
 
 class ReentrantVirtualEnv(VirtualEnv):
     """
     A virtual env that can be de-activated and re-activated
 
     This allows faster reloading due to improved caching of the working set
 
     This is intended for use in testcases to require a lot of venv switching
     """
 
     def __init__(self, env_path: str) -> None:
-        super().__init__(env_path)
+        super(ReentrantVirtualEnv, self).__init__(env_path)
         self.working_set = None
 
     def deactivate(self):
         if self._using_venv:
             self._using_venv = False
             self.working_set = pkg_resources.working_set
 
@@ -1100,15 +1069,15 @@
             pkg_resources.working_set = self.working_set
             self._using_venv = True
 
 
 class SnippetCompilationTest(KeepOnFail):
     def setUpClass(self):
         self.libs = tempfile.mkdtemp()
-        self.repo = "https://github.com/inmanta/"
+        self.repo: str = "https://github.com/inmanta/"
         self.env = tempfile.mkdtemp()
         self.venv = ReentrantVirtualEnv(env_path=self.env)
         config.Config.load_config()
         self.keep_shared = False
         self.project = None
 
     def tearDownClass(self):
@@ -1136,23 +1105,23 @@
 
     def setup_for_snippet(
         self,
         snippet: str,
         *,
         autostd: bool = True,
         install_project: bool = True,
-        install_v2_modules: Optional[list[LocalPackagePath]] = None,
-        add_to_module_path: Optional[list[str]] = None,
-        python_package_sources: Optional[list[str]] = None,
-        project_requires: Optional[list[InmantaModuleRequirement]] = None,
-        python_requires: Optional[list[Requirement]] = None,
+        install_v2_modules: Optional[List[LocalPackagePath]] = None,
+        add_to_module_path: Optional[List[str]] = None,
+        python_package_sources: Optional[List[str]] = None,
+        project_requires: Optional[List[InmantaModuleRequirement]] = None,
+        python_requires: Optional[List[Requirement]] = None,
         install_mode: Optional[InstallMode] = None,
-        relation_precedence_rules: Optional[list[RelationPrecedenceRule]] = None,
+        relation_precedence_rules: Optional[List[RelationPrecedenceRule]] = None,
         strict_deps_check: Optional[bool] = None,
-        main_file: str = "main.cf",
+        use_pip_config_file: Optional[bool] = False,
     ) -> Project:
         """
         Sets up the project to compile a snippet of inmanta DSL. Activates the compiler environment (and patches
         env.process_env).
 
         :param install_project: Install the project and all its modules. This is required to be able to compile the model.
         :param install_v2_modules: Indicates which V2 modules should be installed in the compiler venv
@@ -1163,36 +1132,34 @@
                                  file
         :param python_requires: The dependencies on Python packages providing v2 modules.
         :param install_mode: The install mode to configure in the project.yml file of the inmanta project. If None,
                              no install mode is set explicitly in the project.yml file.
         :param relation_precedence_policy: The relation precedence policy that should be stored in the project.yml file of the
                                            Inmanta project.
         :param strict_deps_check: True iff the returned project should have strict dependency checking enabled.
-        :param main_file: Path to the .cf file to use as main entry point. A relative or an absolute path can be provided.
-            If a relative path is used, it's interpreted relative to the root of the project directory.
+        :param use_pip_config_file: True iff the pip config file should be used and no source is required for v2 to work
+                                    False if a package source is needed for v2 modules to work
         """
         self.setup_for_snippet_external(
             snippet,
             add_to_module_path,
             python_package_sources,
             project_requires,
             python_requires,
             install_mode,
             relation_precedence_rules,
-            main_file,
-        )
-        return self._load_project(
-            autostd, install_project, install_v2_modules, strict_deps_check=strict_deps_check, main_file=main_file
+            use_pip_config_file,
         )
+        return self._load_project(autostd, install_project, install_v2_modules, strict_deps_check=strict_deps_check)
 
     def _load_project(
         self,
         autostd: bool,
         install_project: bool,
-        install_v2_modules: Optional[list[LocalPackagePath]] = None,
+        install_v2_modules: Optional[List[LocalPackagePath]] = None,
         main_file: str = "main.cf",
         strict_deps_check: Optional[bool] = None,
     ):
         loader.PluginModuleFinder.reset()
         self.project = Project(
             self.project_dir, autostd=autostd, main_file=main_file, venv_path=self.venv, strict_deps_check=strict_deps_check
         )
@@ -1207,15 +1174,15 @@
     def _patch_process_env(self) -> None:
         """
         Patch env.process_env to accommodate the SnippetCompilationTest's switching between active environments within a single
         running process.
         """
         env.mock_process_env(env_path=self.env)
 
-    def _install_v2_modules(self, install_v2_modules: Optional[list[LocalPackagePath]] = None) -> None:
+    def _install_v2_modules(self, install_v2_modules: Optional[List[LocalPackagePath]] = None) -> None:
         install_v2_modules = install_v2_modules if install_v2_modules is not None else []
         module_tool = ModuleTool()
         for mod in install_v2_modules:
             with tempfile.TemporaryDirectory() as build_dir:
                 if mod.editable:
                     install_path = mod.path
                 else:
@@ -1226,21 +1193,21 @@
         Project.set(Project(self.project_dir, autostd=Project.get().autostd, venv_path=self.env))
         loader.unload_inmanta_plugins()
         loader.PluginModuleFinder.reset()
 
     def setup_for_snippet_external(
         self,
         snippet: str,
-        add_to_module_path: Optional[list[str]] = None,
-        python_package_sources: Optional[list[str]] = None,
-        project_requires: Optional[list[InmantaModuleRequirement]] = None,
-        python_requires: Optional[list[Requirement]] = None,
+        add_to_module_path: Optional[List[str]] = None,
+        python_package_sources: Optional[List[str]] = None,
+        project_requires: Optional[List[InmantaModuleRequirement]] = None,
+        python_requires: Optional[List[Requirement]] = None,
         install_mode: Optional[InstallMode] = None,
-        relation_precedence_rules: Optional[list[RelationPrecedenceRule]] = None,
-        main_file: str = "main.cf",
+        relation_precedence_rules: Optional[List[RelationPrecedenceRule]] = None,
+        use_pip_config_file: bool = False,
     ) -> None:
         add_to_module_path = add_to_module_path if add_to_module_path is not None else []
         python_package_sources = python_package_sources if python_package_sources is not None else []
         project_requires = project_requires if project_requires is not None else []
         python_requires = python_requires if python_requires is not None else []
         relation_precedence_rules = relation_precedence_rules if relation_precedence_rules else []
         with open(os.path.join(self.project_dir, "project.yml"), "w", encoding="utf-8") as cfg:
@@ -1250,89 +1217,84 @@
             modulepath: {self._get_modulepath_for_project_yml_file(add_to_module_path)}
             downloadpath: {self.libs}
             version: 1.0
             repo:
                 - {{type: git, url: {self.repo} }}
             """.rstrip()
             )
-            if python_package_sources:
-                cfg.write(
-                    "".join(
-                        f"""
-                - {{type: package, url: {source} }}
-                        """.rstrip()
-                        for source in python_package_sources
-                    )
-                )
+
             if relation_precedence_rules:
                 cfg.write("\n            relation_precedence_policy:\n")
                 cfg.write("\n".join(f"                - {rule}" for rule in relation_precedence_rules))
             if project_requires:
                 cfg.write("\n            requires:\n")
                 cfg.write("\n".join(f"                - {req}" for req in project_requires))
             if install_mode:
                 cfg.write(f"\n            install_mode: {install_mode.value}")
+            cfg.write(
+                f"""
+            pip:
+                use_config_file: {use_pip_config_file}
+                index_urls: [{", ".join(url for url in python_package_sources)}]
+            """
+            )
         with open(os.path.join(self.project_dir, "requirements.txt"), "w", encoding="utf-8") as fd:
             fd.write("\n".join(str(req) for req in python_requires))
-        self.main = os.path.join(self.project_dir, main_file)
+        self.main = os.path.join(self.project_dir, "main.cf")
         with open(self.main, "w", encoding="utf-8") as x:
             x.write(snippet)
 
-    def _get_modulepath_for_project_yml_file(self, add_to_module_path: list[str] = []) -> str:
+    def _get_modulepath_for_project_yml_file(self, add_to_module_path: List[str] = []) -> str:
         dirs = [self.libs]
         if self.modules_dir:
             dirs.append(self.modules_dir)
         if add_to_module_path:
             dirs.extend(add_to_module_path)
         return f"[{', '.join(dirs)}]"
 
     def do_export(
         self,
         include_status=False,
         do_raise=True,
         partial_compile: bool = False,
-        resource_sets_to_remove: Optional[list[str]] = None,
-        soft_delete=False,
+        resource_sets_to_remove: Optional[List[str]] = None,
     ) -> Union[tuple[int, ResourceDict], tuple[int, ResourceDict, dict[str, const.ResourceState]]]:
         return self._do_export(
             deploy=False,
             include_status=include_status,
             do_raise=do_raise,
             partial_compile=partial_compile,
             resource_sets_to_remove=resource_sets_to_remove,
-            soft_delete=soft_delete,
         )
 
     def get_exported_json(self) -> JsonType:
         with open(os.path.join(self.project_dir, "dump.json")) as fh:
             return json.load(fh)
 
     def _do_export(
         self,
         deploy=False,
         include_status=False,
         do_raise=True,
         partial_compile: bool = False,
-        resource_sets_to_remove: Optional[list[str]] = None,
-        soft_delete=False,
+        resource_sets_to_remove: Optional[List[str]] = None,
     ) -> Union[tuple[int, ResourceDict], tuple[int, ResourceDict, dict[str, const.ResourceState]]]:
         """
         helper function to allow actual export to be run on a different thread
         i.e. export.run must run off main thread to allow it to start a new ioloop for run_sync
         """
 
-        class Options:
+        class Options(object):
             pass
 
         options = Options()
         options.json = os.path.join(self.project_dir, "dump.json") if not deploy else None
         options.depgraph = False
         options.deploy = deploy
         options.ssl = False
-        options.soft_delete = soft_delete
 
         from inmanta.export import Exporter  # noqa: H307
 
         try:
             (types, scopes) = compiler.do_compile()
         except Exception:
             types, scopes = (None, None)
@@ -1355,26 +1317,24 @@
         )
 
     async def do_export_and_deploy(
         self,
         include_status=False,
         do_raise=True,
         partial_compile: bool = False,
-        resource_sets_to_remove: Optional[list[str]] = None,
-        soft_delete: bool = False,
+        resource_sets_to_remove: Optional[List[str]] = None,
     ) -> Union[tuple[int, ResourceDict], tuple[int, ResourceDict, dict[str, const.ResourceState], Optional[dict[str, object]]]]:
         return await asyncio.get_running_loop().run_in_executor(
             None,
             lambda: self._do_export(
                 deploy=True,
                 include_status=include_status,
                 do_raise=do_raise,
                 partial_compile=partial_compile,
                 resource_sets_to_remove=resource_sets_to_remove,
-                soft_delete=soft_delete,
             ),
         )
 
     def setup_for_error(self, snippet, shouldbe, indent_offset=0):
         """
         Set up project to expect an error during compilation or project install.
         """
@@ -1453,15 +1413,15 @@
 
 
 @pytest.fixture(scope="session")
 def projects_dir() -> str:
     yield os.path.join(os.path.dirname(os.path.abspath(__file__)), "data")
 
 
-class CLI:
+class CLI(object):
     async def run(self, *args, **kwargs):
         # set column width very wide so lines are not wrapped
         os.environ["COLUMNS"] = "1000"
         runner = testing.CliRunner(mix_stderr=False)
         cmd_args = ["--host", "localhost", "--port", config.Config.get("cmdline_rest_transport", "port")]
         cmd_args.extend(args)
 
@@ -1479,15 +1439,15 @@
     # caplog will break this code when emitting any log line to cli
     # due to mysterious interference when juggling with sys.stdout
     # https://github.com/pytest-dev/pytest/issues/10553
     with caplog.at_level(logging.FATAL):
         yield CLI()
 
 
-class AsyncCleaner:
+class AsyncCleaner(object):
     def __init__(self):
         self.register = []
 
     def add(self, method):
         self.register.append(method)
 
     def __call__(self, method):
@@ -1497,26 +1457,26 @@
 @pytest.fixture
 async def async_finalizer():
     cleaner = AsyncCleaner()
     yield cleaner
     await asyncio.gather(*[item() for item in cleaner.register])
 
 
-class CompileRunnerMock:
+class CompileRunnerMock(object):
     def __init__(
         self, request: data.Compile, make_compile_fail: bool = False, runner_queue: Optional[queue.Queue] = None
     ) -> None:
         self.request = request
         self.version: Optional[int] = None
         self._make_compile_fail = make_compile_fail
         self._make_pull_fail = False
         self._runner_queue = runner_queue
         self.block = False
 
-    async def run(self, force_update: Optional[bool] = False) -> tuple[bool, None]:
+    async def run(self, force_update: Optional[bool] = False) -> Tuple[bool, None]:
         now = datetime.datetime.now()
 
         if self._runner_queue is not None:
             self._runner_queue.put(self)
             self.block = True
             while self.block:
                 await asyncio.sleep(0.1)
@@ -1563,15 +1523,15 @@
     runner_queue = queue.Queue()
     monkey_patch_compiler_service(monkeypatch, server, True, runner_queue)
 
     yield runner_queue
 
 
 @pytest.fixture
-def tmpvenv(tmpdir: py.path.local) -> Iterator[tuple[py.path.local, py.path.local]]:
+def tmpvenv(tmpdir: py.path.local) -> Iterator[Tuple[py.path.local, py.path.local]]:
     """
     Creates a venv with the latest pip in `${tmpdir}/.venv` where `${tmpdir}` is the directory returned by the `tmpdir`
     fixture. This venv is completely decoupled from the active development venv.
 
     :return: A tuple of the paths to the venv and the Python executable respectively.
     """
     venv_dir: py.path.local = tmpdir.join(".venv")
@@ -1579,16 +1539,16 @@
     venv.create(venv_dir, with_pip=True)
     subprocess.check_output([str(python_path), "-m", "pip", "install", "-U", "pip"])
     yield (venv_dir, python_path)
 
 
 @pytest.fixture
 def tmpvenv_active(
-    deactive_venv, tmpvenv: tuple[py.path.local, py.path.local]
-) -> Iterator[tuple[py.path.local, py.path.local]]:
+    deactive_venv, tmpvenv: Tuple[py.path.local, py.path.local]
+) -> Iterator[Tuple[py.path.local, py.path.local]]:
     """
     Activates the venv created by the `tmpvenv` fixture within the currently running process. This venv is completely decoupled
     from the active development venv. As a result, any attempts to load new modules from the development venv will fail until
     cleanup. If using this fixture, it should always be listed before other fixtures that are expected to live in this
     environment context because its setup and teardown will then wrap the dependent setup and teardown. This works because
     pytest fixture setup and teardown use LIFO semantics
     (https://docs.pytest.org/en/6.2.x/fixture.html#yield-fixtures-recommended). The snippetcompiler fixture in particular should
@@ -1661,49 +1621,20 @@
     venv_dir: py.path.local = tmpdir.join(".venv")
     venv: env.VirtualEnv = env.VirtualEnv(str(venv_dir))
     venv.use_virtual_env()
     yield venv
     loader.unload_modules_for_path(venv.site_packages_dir)
 
 
-@pytest.fixture
-def create_empty_local_package_index_factory() -> Callable[[str], str]:
-    """
-    A fixture that acts as a factory to create empty local pip package indexes.
-    Each call creates a new index in a different temporary directory.
-    """
-
-    created_directories: list[str] = []
-
-    def _create_local_package_index(prefix: str = "test"):
-        """
-        Creates an empty pip index. The prefix argument is used as a prefix for the temporary directory name
-        for clarity and debugging purposes. The 'dir2pi' tool will then create a 'simple' directory inside
-        this temporary directory, which contains the index files.
-        """
-        tmpdir = tempfile.mkdtemp(prefix=f"{prefix}-")
-        created_directories.append(tmpdir)  # Keep track of the tempdir for cleanup
-        dir2pi(argv=["dir2pi", tmpdir])
-        index_dir = os.path.join(tmpdir, "simple")  # The 'simple' directory is created inside the tmpdir by dir2pi
-        return index_dir
-
-    yield _create_local_package_index
-
-    # Cleanup after the session ends
-    for directory in created_directories:
-        shutil.rmtree(directory)
-
-
 @pytest.fixture(scope="session")
 def local_module_package_index(modules_v2_dir: str) -> Iterator[str]:
     """
     Creates a local pip index for all v2 modules in the modules v2 dir. The modules are built and published to the index.
     :return: The path to the index
     """
-
     cache_dir = os.path.abspath(os.path.join(os.path.dirname(modules_v2_dir), f"{os.path.basename(modules_v2_dir)}.cache"))
     build_dir = os.path.join(cache_dir, "build")
     index_dir = os.path.join(build_dir, "simple")
     timestamp_file = os.path.join(cache_dir, "cache_creation_timestamp")
 
     def _should_rebuild_cache() -> bool:
         if any(not os.path.exists(f) for f in [build_dir, index_dir, timestamp_file]):
@@ -1716,28 +1647,29 @@
         return any(
             os.path.getmtime(os.path.join(root, f)) > os.path.getmtime(timestamp_file)
             for root, _, files in os.walk(modules_v2_dir)
             for f in files
         )
 
     if _should_rebuild_cache():
-        logger.info("Cache %s is dirty. Rebuilding cache.", cache_dir)  # Remove cache
+        logger.info(f"Cache {cache_dir} is dirty. Rebuilding cache.")
+        # Remove cache
         if os.path.exists(cache_dir):
             shutil.rmtree(cache_dir)
         os.makedirs(build_dir)
         # Build modules
         for module_dir in os.listdir(modules_v2_dir):
             path: str = os.path.join(modules_v2_dir, module_dir)
             ModuleTool().build(path=path, output_dir=build_dir)
         # Build python package repository
         dir2pi(argv=["dir2pi", build_dir])
         # Update timestamp file
         open(timestamp_file, "w").close()
     else:
-        logger.info("Using cache %s", cache_dir)
+        logger.info(f"Using cache {cache_dir}")
 
     yield index_dir
 
 
 @pytest.fixture
 async def migrate_db_from(
     request: pytest.FixtureRequest, hard_clean_db, hard_clean_db_post, postgresql_client: asyncpg.Connection, server_pre_start
@@ -1747,15 +1679,15 @@
 
     :param db_restore_dump: The db version dump file to restore (set via `@pytest.mark.db_restore_dump(<file>)`.
     """
     marker: Optional[pytest.mark.Mark] = request.node.get_closest_marker("db_restore_dump")
     if marker is None or len(marker.args) != 1:
         raise ValueError("Please set the db version to restore using `@pytest.mark.db_restore_dump(<file>)`")
     # restore old version
-    with open(marker.args[0]) as fh:
+    with open(marker.args[0], "r") as fh:
         await PGRestore(fh.readlines(), postgresql_client).run()
 
     bootloader: InmantaBootloader = InmantaBootloader()
 
     async def migrate() -> None:
         # start boatloader, triggering db migration
         await bootloader.start()
@@ -1766,15 +1698,15 @@
 
     await bootloader.stop(timeout=15)
 
 
 @pytest.fixture(scope="session", autouse=not PYTEST_PLUGIN_MODE)
 def guard_invariant_on_v2_modules_in_data_dir(modules_v2_dir: str) -> None:
     """
-    When the test suite runs, the python environment used to build V2 modules is cached using the DefaultIsolatedEnvCached
+    When the test suite runs, the python environment used to build V2 modules is cached using the IsolatedEnvBuilderCached
     class. This cache relies on the fact that all modules in the tests/data/modules_v2 directory use the same build-backand
     and build requirements. This guard verifies whether that assumption is fulfilled and raises an exception if it's not.
     """
     for dir_name in os.listdir(modules_v2_dir):
         module_path = os.path.join(modules_v2_dir, dir_name)
         pyproject_toml_path = os.path.join(module_path, "pyproject.toml")
         error_message = f"""
@@ -1785,15 +1717,15 @@
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 All modules present in the tests/data/module_v2 directory should satisfy the above-mentioned requirements, because
 the test suite caches the python environment used to build the V2 modules. This cache relies on the assumption that all modules
 use the same build-backend and build requirements.
         """.strip()
-        with open(pyproject_toml_path, encoding="utf-8") as fh:
+        with open(pyproject_toml_path, "r", encoding="utf-8") as fh:
             pyproject_toml_as_dct = toml.load(fh)
             try:
                 if pyproject_toml_as_dct["build-system"]["build-backend"] != "setuptools.build_meta" or set(
                     pyproject_toml_as_dct["build-system"]["requires"]
                 ) != {"setuptools", "wheel"}:
                     raise Exception(error_message)
             except (KeyError, TypeError):
```

### Comparing `pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/ca/enduser-certs/server.chain` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.chain`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/ca/enduser-certs/server.crt` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.crt`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/ca/enduser-certs/server.key` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/ca/enduser-certs/server.key.open` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/server.crt` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/server.crt`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.7.4/src/inmanta_tests/data/server.open.key` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/server.open.key`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.7.4/src/inmanta_tests/db/common.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/common.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.7.4/src/inmanta_tests/plugin.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.7.4/src/inmanta_tests/utils.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,43 +20,39 @@
 import datetime
 import json
 import logging
 import os
 import shutil
 import uuid
 from collections import abc
-from collections.abc import Sequence
 from dataclasses import dataclass
 from datetime import timezone
-from typing import Any, Optional, TypeVar, Union
+from typing import Any, Dict, Optional, Sequence, Type, TypeVar, Union
 
 import pytest
 import yaml
 from pkg_resources import Requirement, parse_version
 from pydantic.tools import lru_cache
 
 import build
 import build.env
 from _pytest.mark import MarkDecorator
 from inmanta import const, data, env, module, util
-from inmanta.data import ResourceIdStr
 from inmanta.moduletool import ModuleTool
 from inmanta.protocol import Client
 from inmanta.server.bootloader import InmantaBootloader
 from inmanta.server.extensions import ProductMetadata
 from inmanta.util import get_compiler_version
 from libpip2pi.commands import dir2pi
 from packaging import version
 
 T = TypeVar("T")
 
-LOGGER = logging.getLogger(__name__)
 
-
-def get_all_subclasses(cls: type[T]) -> set[type[T]]:
+def get_all_subclasses(cls: Type[T]) -> set[Type[T]]:
     """
     Returns all loaded subclasses of any depth for a given class. Includes the class itself.
     """
     return {cls}.union(*(get_all_subclasses(sub) for sub in cls.__subclasses__()))
 
 
 async def retry_limited(
@@ -111,24 +107,26 @@
     elif minimal is UNKWN:
         return
     else:
         assert minimal == actual, f"Minimal value expected is '{minimal}' but got '{actual}'"
 
 
 def assert_graph(graph, expected):
-    lines = [f"{f.id.get_attribute_value()}: {t.id.get_attribute_value()}" for f in graph.values() for t in f.resource_requires]
+    lines = [
+        "%s: %s" % (f.id.get_attribute_value(), t.id.get_attribute_value()) for f in graph.values() for t in f.resource_requires
+    ]
     lines = sorted(lines)
 
     elines = [x.strip() for x in expected.split("\n")]
     elines = sorted(elines)
 
     assert elines == lines, (lines, elines)
 
 
-class AsyncClosing:
+class AsyncClosing(object):
     def __init__(self, awaitable):
         self.awaitable = awaitable
 
     async def __aenter__(self):
         self.closable = await self.awaitable
         return object
 
@@ -184,15 +182,15 @@
         for logger_name, log_level, message in close:
             print(logger_name, log_level, message)
         print("------------")
 
     assert False
 
 
-class LogSequence:
+class LogSequence(object):
     def __init__(self, caplog, index=0, allow_errors=True, ignore=[]):
         """
 
         :param caplog: caplog fixture
         :param index: start index in the log
         :param allow_errors: allow errors between log entries that are requested by log_contains
         :param ignore: ignore following namespaces
@@ -308,53 +306,37 @@
         result = await client.get_version(environment, version)
         print(version, result.result)
         return result.result["model"]["deployed"]
 
     await retry_limited(is_deployment_finished, timeout)
 
 
-async def _wait_for_resource_actions(
-    client: Client, environment: str, rid: ResourceIdStr, deploy_count: int, timeout: int = 10
-) -> None:
-    async def is_deployment_finished() -> bool:
-        result = await client.resource_logs(environment, rid, filter={"action": ["deploy"]})
-        assert result.code == 200
-        end_lines = [line for line in result.result["data"] if "End run" in line.get("msg", "")]
-        LOGGER.info("Deploys done: %s", end_lines)
-        return len(end_lines) >= deploy_count
-
-    await retry_limited(is_deployment_finished, timeout)
-
-
-class ClientHelper:
+class ClientHelper(object):
     def __init__(self, client: Client, environment: uuid.UUID) -> None:
         self.client = client
         self.environment = environment
 
     async def get_version(self) -> int:
         res = await self.client.reserve_version(self.environment)
         assert res.code == 200
         return res.result["data"]
 
-    async def put_version_simple(self, resources: dict[str, Any], version: int) -> None:
+    async def put_version_simple(self, resources: Dict[str, Any], version: int) -> None:
         res = await self.client.put_version(
             tid=self.environment,
             version=version,
             resources=resources,
             unknowns=[],
             version_info={},
             compiler_version=get_compiler_version(),
         )
         assert res.code == 200, res.result
 
-    async def wait_for_deployed(self, version: int) -> None:
-        await _wait_until_deployment_finishes(client=self.client, environment=self.environment, version=version)
 
-
-def get_resource(version: int, key: str = "key1", agent: str = "agent1", value: str = "value1") -> dict[str, Any]:
+def get_resource(version: int, key: str = "key1", agent: str = "agent1", value: str = "value1") -> Dict[str, Any]:
     return {
         "key": key,
         "value": value,
         "id": f"test::Resource[{agent},key={key}],v=%d" % version,
         "send_event": False,
         "purged": False,
         "requires": [],
@@ -402,15 +384,15 @@
     pkg_version: version.Version,
     path: str,
     *,
     requirements: Optional[Sequence[Requirement]] = None,
     install: bool = False,
     editable: bool = False,
     publish_index: Optional[PipIndex] = None,
-    optional_dependencies: Optional[dict[str, Sequence[Requirement]]] = None,
+    optional_dependencies: Optional[Dict[str, Sequence[Requirement]]] = None,
 ) -> None:
     """
     Creates an empty Python package.
 
     :param name: The name of the package.
     :param pkg_version: The version of the package.
     :param path: The path to an empty or non-existant directory to create the package in.
@@ -469,16 +451,18 @@
             for option_name, requirements in optional_dependencies.items():
                 requirements_as_string = "".join(f"\n  {req}" for req in requirements)
                 fd.write(f"\n{option_name} ={requirements_as_string}")
 
     if install:
         env.process_env.install_from_source([env.LocalPackagePath(path=path, editable=editable)])
     if publish_index is not None:
-        with build.env.DefaultIsolatedEnv() as build_env:
-            builder = build.ProjectBuilder(source_dir=path, python_executable=build_env.python_executable)
+        with build.env.IsolatedEnvBuilder() as build_env:
+            builder = build.ProjectBuilder(
+                srcdir=path, python_executable=build_env.executable, scripts_dir=build_env.scripts_dir
+            )
             build_env.install(builder.build_system_requires)
             build_env.install(builder.get_requires_for_build(distribution="wheel"))
             builder.build(distribution="wheel", output_directory=publish_index.artifact_dir)
         publish_index.publish()
 
 
 def module_from_template(
@@ -538,15 +522,15 @@
         os.rename(
             os.path.join(dest_dir, const.PLUGINS_PACKAGE, old_name),
             os.path.join(dest_dir, const.PLUGINS_PACKAGE, new_name),
         )
         config["metadata"]["name"] = module.ModuleV2Source.get_package_name_for(new_name)
         manifest_file: str = os.path.join(dest_dir, "MANIFEST.in")
         manifest_content: str
-        with open(manifest_file) as fd:
+        with open(manifest_file, "r") as fd:
             manifest_content: str = fd.read()
         with open(manifest_file, "w", encoding="utf-8") as fd:
             fd.write(manifest_content.replace(f"inmanta_plugins/{old_name}/", f"inmanta_plugins/{new_name}/"))
     if new_requirements:
         config["options"]["install_requires"] = "\n    ".join(to_python_requires(new_requirements))
     if new_extras:
         # start from a clean slate
@@ -570,15 +554,15 @@
     with open(config_file, "w") as fh:
         config.write(fh)
     if install:
         ModuleTool().install(editable=editable, path=dest_dir)
     if publish_index is not None:
         ModuleTool().build(path=dest_dir, output_dir=publish_index.artifact_dir)
         publish_index.publish()
-    with open(config_file) as fh:
+    with open(config_file, "r") as fh:
         return module.ModuleV2Metadata.parse(fh)
 
 
 def v1_module_from_template(
     source_dir: str,
     dest_dir: str,
     *,
@@ -597,16 +581,16 @@
     :param new_name: The new name of the inmanta module, if any.
     :param new_requirements: The new Python requirements for the module, if any.
     :param new_content_init_cf: The new content of the _init.cf file.
     :param new_content_init_py: The new content of the __init__.py file.
     """
     shutil.copytree(source_dir, dest_dir)
     config_file: str = os.path.join(dest_dir, module.ModuleV1.MODULE_FILE)
-    config: dict[str, object] = configparser.ConfigParser()
-    with open(config_file) as fd:
+    config: Dict[str, object] = configparser.ConfigParser()
+    with open(config_file, "r") as fd:
         config = yaml.safe_load(fd)
     if new_version is not None:
         config["version"] = str(new_version)
     if new_name is not None:
         config["name"] = new_name
     if new_content_init_cf is not None:
         init_cf_file = os.path.join(dest_dir, "model", "_init.cf")
@@ -624,15 +608,15 @@
         with open(os.path.join(dest_dir, "requirements.txt"), "w") as fd:
             fd.write(
                 "\n".join(
                     str(req if isinstance(req, Requirement) else req.get_python_package_requirement())
                     for req in new_requirements
                 )
             )
-    with open(config_file) as fd:
+    with open(config_file, "r") as fd:
         return module.ModuleV1Metadata.parse(fd)
 
 
 def parse_datetime_to_utc(time: str) -> datetime.datetime:
     return datetime.datetime.strptime(time, "%Y-%m-%dT%H:%M:%S.%f").replace(tzinfo=datetime.timezone.utc)
```

### Comparing `pytest-inmanta-extensions-8.7.4/src/pytest_inmanta_extensions.egg-info/SOURCES.txt` & `pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

