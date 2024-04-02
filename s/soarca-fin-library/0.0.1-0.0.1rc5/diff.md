# Comparing `tmp/soarca_fin_library-0.0.1.tar.gz` & `tmp/soarca_fin_library-0.0.1rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soarca_fin_library-0.0.1.tar", max compression
+gzip compressed data, was "soarca_fin_library-0.0.1rc5.tar", max compression
```

## Comparing `soarca_fin_library-0.0.1.tar` & `soarca_fin_library-0.0.1rc5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11332 2024-04-02 10:17:16.894840 soarca_fin_library-0.0.1/LICENSE
--rw-r--r--   0        0        0     2066 2024-04-02 10:17:16.894840 soarca_fin_library-0.0.1/README.md
--rw-r--r--   0        0        0      528 2024-04-02 10:17:16.894840 soarca_fin_library-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 10:17:16.894840 soarca_fin_library-0.0.1/soarca_fin_python_library/__init__.py
--rw-r--r--   0        0        0      211 2024-04-02 10:17:16.894840 soarca_fin_library-0.0.1/soarca_fin_python_library/abstract_classes/i_executor.py
--rw-r--r--   0        0        0      671 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/abstract_classes/i_mqtt_client.py
--rw-r--r--   0        0        0      255 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/abstract_classes/i_parser.py
--rw-r--r--   0        0        0      469 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/abstract_classes/i_soarca_fin.py
--rw-r--r--   0        0        0        0 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/enums/__init__.py
--rw-r--r--   0        0        0      120 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/enums/ack_status_enum.py
--rw-r--r--   0        0        0      134 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/enums/auth_type_enum.py
--rw-r--r--   0        0        0      101 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/enums/dispatcher_task_enum.py
--rw-r--r--   0        0        0      102 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/enums/timeout_status_enum.py
--rw-r--r--   0        0        0      411 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/enums/variable_type_enum.py
--rw-r--r--   0        0        0      298 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/enums/workflow_step_enum.py
--rw-r--r--   0        0        0     9098 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/executor.py
--rw-r--r--   0        0        0     2835 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/main.py
--rw-r--r--   0        0        0     7488 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/message_factory.py
--rw-r--r--   0        0        0        0 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/__init__.py
--rw-r--r--   0        0        0      152 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/ack.py
--rw-r--r--   0        0        0      109 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/agent_structure.py
--rw-r--r--   0        0        0      601 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/authentication_information.py
--rw-r--r--   0        0        0      464 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/capability_structure.py
--rw-r--r--   0        0        0      349 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/command.py
--rw-r--r--   0        0        0      475 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/command_sub_structure.py
--rw-r--r--   0        0        0      259 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/context.py
--rw-r--r--   0        0        0      289 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/external_reference.py
--rw-r--r--   0        0        0       93 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/message.py
--rw-r--r--   0        0        0       93 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/meta.py
--rw-r--r--   0        0        0      153 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/nack.py
--rw-r--r--   0        0        0      489 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/register.py
--rw-r--r--   0        0        0      333 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/result.py
--rw-r--r--   0        0        0      262 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/result_structure.py
--rw-r--r--   0        0        0      102 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/security.py
--rw-r--r--   0        0        0      283 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/step_structure.py
--rw-r--r--   0        0        0      288 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/unregister.py
--rw-r--r--   0        0        0      112 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/unregister_self.py
--rw-r--r--   0        0        0      256 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/models/variable.py
--rw-r--r--   0        0        0     2832 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/mqtt_client.py
--rw-r--r--   0        0        0     2466 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/parser.py
--rw-r--r--   0        0        0     5626 2024-04-02 10:17:16.898840 soarca_fin_library-0.0.1/soarca_fin_python_library/soarca_fin.py
--rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 soarca_fin_library-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11332 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/LICENSE
+-rw-r--r--   0        0        0     2066 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/README.md
+-rw-r--r--   0        0        0      735 2024-04-02 13:24:59.411511 soarca_fin_library-0.0.1rc5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/__init__.py
+-rw-r--r--   0        0        0      211 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/abstract_classes/i_executor.py
+-rw-r--r--   0        0        0      671 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/abstract_classes/i_mqtt_client.py
+-rw-r--r--   0        0        0      255 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/abstract_classes/i_parser.py
+-rw-r--r--   0        0        0      469 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/abstract_classes/i_soarca_fin.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/__init__.py
+-rw-r--r--   0        0        0      120 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/ack_status_enum.py
+-rw-r--r--   0        0        0      134 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/auth_type_enum.py
+-rw-r--r--   0        0        0      101 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/dispatcher_task_enum.py
+-rw-r--r--   0        0        0      102 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/timeout_status_enum.py
+-rw-r--r--   0        0        0      411 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/variable_type_enum.py
+-rw-r--r--   0        0        0      298 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/workflow_step_enum.py
+-rw-r--r--   0        0        0     9098 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/executor.py
+-rw-r--r--   0        0        0     2835 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/main.py
+-rw-r--r--   0        0        0     7488 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/message_factory.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/ack.py
+-rw-r--r--   0        0        0      109 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/agent_structure.py
+-rw-r--r--   0        0        0      601 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/authentication_information.py
+-rw-r--r--   0        0        0      464 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/capability_structure.py
+-rw-r--r--   0        0        0      349 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/command.py
+-rw-r--r--   0        0        0      475 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/command_sub_structure.py
+-rw-r--r--   0        0        0      259 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/context.py
+-rw-r--r--   0        0        0      289 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/external_reference.py
+-rw-r--r--   0        0        0       93 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/message.py
+-rw-r--r--   0        0        0       93 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/meta.py
+-rw-r--r--   0        0        0      153 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/nack.py
+-rw-r--r--   0        0        0      489 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/register.py
+-rw-r--r--   0        0        0      333 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/result.py
+-rw-r--r--   0        0        0      262 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/result_structure.py
+-rw-r--r--   0        0        0      102 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/security.py
+-rw-r--r--   0        0        0      283 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/step_structure.py
+-rw-r--r--   0        0        0      288 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/unregister.py
+-rw-r--r--   0        0        0      112 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/unregister_self.py
+-rw-r--r--   0        0        0      256 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/variable.py
+-rw-r--r--   0        0        0     2832 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/mqtt_client.py
+-rw-r--r--   0        0        0     2466 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/parser.py
+-rw-r--r--   0        0        0     5626 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/soarca_fin.py
+-rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 soarca_fin_library-0.0.1rc5/PKG-INFO
```

### Comparing `soarca_fin_library-0.0.1/LICENSE` & `soarca_fin_library-0.0.1rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `soarca_fin_library-0.0.1/README.md` & `soarca_fin_library-0.0.1rc5/README.md`

 * *Files identical despite different names*

### Comparing `soarca_fin_library-0.0.1/pyproject.toml` & `soarca_fin_library-0.0.1rc5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 [tool.poetry]
 name = "soarca-fin-library"
-version = "0.0.1"
+version = "0.0.1-pre.5"
 description = "SOARCA FIN lib allows for extending custom SOARCA capabilities through a python library"
 authors = ["Maarten de Kruijf","RabbITCybErSeC","xncz8h (Ivo)"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{include = "soarca_fin_python_library"}]
-
-
+ 
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
+metadata = false
+dirty = true
+pattern = "default-unprefixed"
+ 
 [tool.poetry.dependencies]
 python = "^3.10"
 paho-mqtt = "2.0.0"
 pydantic = "2.6.4"
 python-dotenv = "1.0.1"
-
-
+ 
+ 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `soarca_fin_library-0.0.1/soarca_fin_python_library/abstract_classes/i_mqtt_client.py` & `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/abstract_classes/i_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `soarca_fin_library-0.0.1/soarca_fin_python_library/executor.py` & `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/executor.py`

 * *Files identical despite different names*

### Comparing `soarca_fin_library-0.0.1/soarca_fin_python_library/main.py` & `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/main.py`

 * *Files identical despite different names*

### Comparing `soarca_fin_library-0.0.1/soarca_fin_python_library/message_factory.py` & `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/message_factory.py`

 * *Files identical despite different names*

### Comparing `soarca_fin_library-0.0.1/soarca_fin_python_library/models/authentication_information.py` & `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/authentication_information.py`

 * *Files identical despite different names*

### Comparing `soarca_fin_library-0.0.1/soarca_fin_python_library/mqtt_client.py` & `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `soarca_fin_library-0.0.1/soarca_fin_python_library/parser.py` & `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/parser.py`

 * *Files identical despite different names*

### Comparing `soarca_fin_library-0.0.1/soarca_fin_python_library/soarca_fin.py` & `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/soarca_fin.py`

 * *Files identical despite different names*

### Comparing `soarca_fin_library-0.0.1/PKG-INFO` & `soarca_fin_library-0.0.1rc5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soarca-fin-library
-Version: 0.0.1
+Version: 0.0.1rc5
 Summary: SOARCA FIN lib allows for extending custom SOARCA capabilities through a python library
 License: Apache-2.0
 Author: Maarten de Kruijf
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

