# Comparing `tmp/fuzz-utils-0.0.1.tar.gz` & `tmp/fuzz-utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzz-utils-0.0.1.tar", last modified: Fri Feb 16 10:26:27 2024, max compression
+gzip compressed data, was "fuzz-utils-0.2.0.tar", last modified: Tue Apr  2 13:24:02 2024, max compression
```

## Comparing `fuzz-utils-0.0.1.tar` & `fuzz-utils-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:26:27.204921 fuzz-utils-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-02-16 10:26:27.204921 fuzz-utils-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:26:27.200921 fuzz-utils-0.0.1/fuzz_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/fuzz_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:26:27.204921 fuzz-utils-0.0.1/fuzz_utils/fuzzers/
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/fuzz_utils/fuzzers/Echidna.py
--rw-r--r--   0 runner    (1001) docker     (127)    13215 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/fuzz_utils/fuzzers/Medusa.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/fuzz_utils/fuzzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/fuzz_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:26:27.204921 fuzz-utils-0.0.1/fuzz_utils/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/fuzz_utils/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/fuzz_utils/templates/foundry_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:26:27.204921 fuzz-utils-0.0.1/fuzz_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/fuzz_utils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/fuzz_utils/utils/crytic_print.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/fuzz_utils/utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/fuzz_utils/utils/error_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:26:27.204921 fuzz-utils-0.0.1/fuzz_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-02-16 10:26:27.000000 fuzz-utils-0.0.1/fuzz_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-16 10:26:27.000000 fuzz-utils-0.0.1/fuzz_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 10:26:27.000000 fuzz-utils-0.0.1/fuzz_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-16 10:26:27.000000 fuzz-utils-0.0.1/fuzz_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-16 10:26:27.000000 fuzz-utils-0.0.1/fuzz_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-16 10:26:27.000000 fuzz-utils-0.0.1/fuzz_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 10:26:27.204921 fuzz-utils-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:26:27.204921 fuzz-utils-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-02-16 10:26:17.000000 fuzz-utils-0.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-02-16 10:26:18.000000 fuzz-utils-0.0.1/tests/test_types_echidna.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-02-16 10:26:18.000000 fuzz-utils-0.0.1/tests/test_types_medusa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:24:02.353084 fuzz-utils-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12521 2024-04-02 13:24:02.353084 fuzz-utils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:24:02.345084 fuzz-utils-0.2.0/fuzz_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:24:02.345084 fuzz-utils-0.2.0/fuzz_utils/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/generate/FoundryTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:24:02.349084 fuzz-utils-0.2.0/fuzz_utils/generate/fuzzers/
+-rw-r--r--   0 runner    (1001) docker     (127)    15061 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/generate/fuzzers/Echidna.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12427 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/generate/fuzzers/Medusa.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/generate/fuzzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:24:02.349084 fuzz-utils-0.2.0/fuzz_utils/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:24:02.349084 fuzz-utils-0.2.0/fuzz_utils/parsing/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/parsing/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/parsing/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/parsing/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/parsing/commands/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/parsing/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/parsing/parser_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:24:02.349084 fuzz-utils-0.2.0/fuzz_utils/template/
+-rw-r--r--   0 runner    (1001) docker     (127)    22953 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/template/HarnessGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:24:02.349084 fuzz-utils-0.2.0/fuzz_utils/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/templates/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/templates/foundry_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/templates/harness_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:24:02.349084 fuzz-utils-0.2.0/fuzz_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/utils/crytic_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/utils/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/utils/remappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/fuzz_utils/utils/slither_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:24:02.353084 fuzz-utils-0.2.0/fuzz_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12521 2024-04-02 13:24:02.000000 fuzz-utils-0.2.0/fuzz_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-02 13:24:02.000000 fuzz-utils-0.2.0/fuzz_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:24:02.000000 fuzz-utils-0.2.0/fuzz_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 13:24:02.000000 fuzz-utils-0.2.0/fuzz_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-02 13:24:02.000000 fuzz-utils-0.2.0/fuzz_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 13:24:02.000000 fuzz-utils-0.2.0/fuzz_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:24:02.353084 fuzz-utils-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:24:02.353084 fuzz-utils-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/tests/test_harness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/tests/test_remapping_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/tests/test_types_echidna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-02 13:23:57.000000 fuzz-utils-0.2.0/tests/test_types_medusa.py
```

### Comparing `fuzz-utils-0.0.1/LICENSE` & `fuzz-utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzz-utils-0.0.1/fuzz_utils/fuzzers/Echidna.py` & `fuzz-utils-0.2.0/fuzz_utils/generate/fuzzers/Echidna.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,75 @@
 """ Generates a test file from Echidna reproducers """
 # type: ignore[misc] # Ignores 'Any' input parameter
 from typing import Any, NoReturn
 import jinja2
 
 from slither import Slither
-from slither.core.declarations.contract import Contract
 from slither.core.declarations.function_contract import FunctionContract
 from slither.core.solidity_types.elementary_type import ElementaryType
 from slither.core.solidity_types.user_defined_type import UserDefinedType
 from slither.core.solidity_types.array_type import ArrayType
 from slither.core.declarations.structure import Structure
 from slither.core.declarations.structure_contract import StructureContract
 from slither.core.declarations.enum import Enum
 from fuzz_utils.utils.crytic_print import CryticPrint
 from fuzz_utils.templates.foundry_templates import templates
 from fuzz_utils.utils.encoding import parse_echidna_byte_string
 from fuzz_utils.utils.error_handler import handle_exit
+from fuzz_utils.utils.slither_utils import get_target_contract
 
 
+# pylint: disable=too-few-public-methods,too-many-instance-attributes
 class Echidna:
     """
     Handles the generation of Foundry test files from Echidna reproducers
     """
 
-    def __init__(self, target_name: str, corpus_path: str, slither: Slither) -> None:
+    def __init__(
+        self, target_name: str, corpus_path: str, slither: Slither, named_inputs: bool
+    ) -> None:
         self.name = "Echidna"
         self.target_name = target_name
         self.slither = slither
-        self.target = self.get_target_contract()
+        self.target = get_target_contract(slither, target_name)
         self.reproducer_dir = f"{corpus_path}/reproducers"
+        self.corpus_dirs = [f"{corpus_path}/coverage", self.reproducer_dir]
+        self.named_inputs = named_inputs
+        self.declared_variables: set[tuple[str, str]] = set()
 
-    def get_target_contract(self) -> Contract:
-        """Finds and returns Slither Contract"""
-        contracts = self.slither.get_contract_from_name(self.target_name)
-        # Loop in case slither fetches multiple contracts for some reason (e.g., similar names?)
-        for contract in contracts:
-            if contract.name == self.target_name:
-                return contract
-
-        handle_exit(f"\n* Slither could not find the specified contract `{self.target_name}`.")
-
-    def parse_reproducer(self, calls: Any, index: int) -> str:
+    def parse_reproducer(self, file_path: str, calls: Any, index: int) -> str:
         """
         Takes a list of call dicts and returns a Foundry unit test string containing the call sequence.
         """
         call_list = []
         end = len(calls) - 1
         function_name = ""
+        has_low_level_call: bool = False
+
+        # before each test case, we clear the declared variables, as those are locals
+        self.declared_variables = set()
+
         # 1. For each object in the list process the call object and add it to the call list
         for idx, call in enumerate(calls):
             call_str, fn_name = self._parse_call_object(call)
             call_list.append(call_str)
+            has_low_level_call = has_low_level_call or ("(success, " in call_str)
             if idx == end:
                 function_name = fn_name + "_" + str(index)
 
         # 2. Generate the test string and return it
         template = jinja2.Template(templates["TEST"])
-        return template.render(function_name=function_name, call_list=call_list)
+        return template.render(
+            function_name=function_name,
+            call_list=call_list,
+            file_path=file_path,
+            has_low_level_call=has_low_level_call,
+        )
 
+    # pylint: disable=too-many-locals,too-many-branches
     def _parse_call_object(self, call_dict: dict[Any, Any]) -> tuple[str, str]:
         """
         Takes a single call dictionary, parses it, and returns the series of function calls as a string, along with
         the name of the last function, which is used as the name of the test.
         """
         # 1. Parse call object and save the variables
         time_delay = int(call_dict["delay"][0], 16)
@@ -95,28 +103,39 @@
                 slither_entry_point = entry_point
 
         if "slither_entry_point" not in locals():
             handle_exit(
                 f"\n* Slither could not find the function `{function_name}` specified in the call object"
             )
 
+        if not slither_entry_point.payable:
+            value = 0
+
         # 2. Decode the function parameters
         variable_definition, call_definition = self._decode_function_params(
             function_parameters, False, slither_entry_point
         )
+        parameters_str: str = ""
+        if isinstance(slither_entry_point.parameters, list):
+            if self.named_inputs and len(slither_entry_point.parameters) > 0:
+                for idx, input_param in enumerate(slither_entry_point.parameters):
+                    call_definition[idx] = input_param.name + ": " + call_definition[idx]
+                parameters_str = "{" + ", ".join(call_definition) + "}"
+            else:
+                parameters_str = ", ".join(call_definition)
 
         # 3. Generate a call string and return it
         template = jinja2.Template(templates["CALL"])
         call_str = template.render(
             has_delay=has_delay,
             time_delay=time_delay,
             block_delay=block_delay,
             caller=caller,
             value=value,
-            function_parameters=", ".join(call_definition),
+            function_parameters=parameters_str,
             function_name=function_name,
             contract_name=self.target_name,
         )
         # If we need to define local variables, append them to the call sequence
         if variable_definition is not None:
             call_str = variable_definition + call_str
 
@@ -152,29 +171,29 @@
                 return param["contents"]
             case "AbiBytes" | "AbiBytesDynamic":
                 is_fixed_size = isinstance(param["contents"], list)
                 size = param["contents"][0] if is_fixed_size else ""
                 contents = param["contents"][1] if is_fixed_size else param["contents"]
 
                 # Haskell encoding needs to be stripped and then converted to a hex literal
-                hex_string = parse_echidna_byte_string(contents.strip('"'))
+                hex_string = parse_echidna_byte_string(contents.strip('"'), True)
                 interpreted_string = f'hex"{hex_string}"'
                 if not recursive:
                     result = (
                         f"bytes{size}({interpreted_string})"
                         if is_fixed_size
                         else interpreted_string
                     )
                     return result
 
                 casting = f"bytes{size}({interpreted_string})"
                 return casting
             case "AbiString":
-                hex_string = parse_echidna_byte_string(param["contents"].strip('"'))
-                interpreted_string = f'string(hex"{hex_string}")'
+                hex_string = parse_echidna_byte_string(param["contents"].strip('"'), False)
+                interpreted_string = f'string(unicode"{hex_string}")'
                 return interpreted_string
             case _:
                 handle_exit(
                     f"\n* The parameter tag `{param['tag']}` could not be found in the call object. This could indicate an issue in decoding the call sequence, or a missing feature. Please open an issue at https://github.com/crytic/fuzz-utils/issues"
                 )
 
     def _match_array_type(
@@ -284,9 +303,17 @@
     def _get_memarr(
         self, function_params: dict, index: int, input_parameter: Any
     ) -> tuple[str, str]:
         length = len(function_params[1])
 
         input_type = input_parameter.type
         name = f"dyn{input_type}Arr_{index}"
-        declaration = f"{input_type}[] memory {name} = new {input_type}[]({length});\n"
+
+        # If the variable was already declared, just assign the new value
+        if (input_type, name) in self.declared_variables:
+            declaration = f"{name} = new {input_type}[]({length});\n"
+        else:
+            declaration = f"{input_type}[] memory {name} = new {input_type}[]({length});\n"
+
+        self.declared_variables.add((input_type, name))
+
         return name, declaration
```

### Comparing `fuzz-utils-0.0.1/fuzz_utils/main.py` & `fuzz-utils-0.2.0/fuzz_utils/parsing/commands/generate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,111 +1,29 @@
-""" Generates a test file from Echidna reproducers """
-import os
-import sys
-import json
-import argparse
-import jinja2
-
-from pkg_resources import require
-
+"""Defines the flags and logic associated with the `generate` command"""
+from pathlib import Path
+from argparse import Namespace, ArgumentParser
 from slither import Slither
-from slither.core.declarations.contract import Contract
 from fuzz_utils.utils.crytic_print import CryticPrint
-from fuzz_utils.templates.foundry_templates import templates
-from fuzz_utils.fuzzers.Medusa import Medusa
-from fuzz_utils.fuzzers.Echidna import Echidna
+from fuzz_utils.generate.FoundryTest import FoundryTest
+from fuzz_utils.generate.fuzzers.Medusa import Medusa
+from fuzz_utils.generate.fuzzers.Echidna import Echidna
 from fuzz_utils.utils.error_handler import handle_exit
+from fuzz_utils.parsing.parser_util import check_config_and_set_default_values, open_config
+from fuzz_utils.utils.slither_utils import get_target_contract
 
+COMMAND: str = "generate"
 
-class FoundryTest:
-    """
-    Handles the generation of Foundry test files
-    """
-
-    def __init__(
-        self,
-        inheritance_path: str,
-        target_name: str,
-        corpus_path: str,
-        test_dir: str,
-        slither: Slither,
-        fuzzer: Echidna | Medusa,
-    ) -> None:
-        self.inheritance_path = inheritance_path
-        self.target_name = target_name
-        self.corpus_path = corpus_path
-        self.test_dir = test_dir
-        self.slither = slither
-        self.target = self.get_target_contract()
-        self.fuzzer = fuzzer
-
-    def get_target_contract(self) -> Contract:
-        """Gets the Slither Contract object for the specified contract file"""
-        contracts = self.slither.get_contract_from_name(self.target_name)
-        # Loop in case slither fetches multiple contracts for some reason (e.g., similar names?)
-        for contract in contracts:
-            if contract.name == self.target_name:
-                return contract
-
-        # TODO throw error if no contract found
-        sys.exit(-1)
-
-    def create_poc(self) -> str:
-        """Takes in a directory path to the echidna reproducers and generates a test file"""
-
-        file_list = []
-        tests_list = []
-        # 1. Iterate over each reproducer file (open it)
-        for entry in os.listdir(self.fuzzer.reproducer_dir):
-            full_path = os.path.join(self.fuzzer.reproducer_dir, entry)
-
-            if os.path.isfile(full_path):
-                try:
-                    with open(full_path, "r", encoding="utf-8") as file:
-                        file_list.append(json.load(file))
-                except Exception:  # pylint: disable=broad-except
-                    print(f"Fail on {full_path}")
-
-        # 2. Parse each reproducer file and add each test function to the functions list
-        for idx, file in enumerate(file_list):
-            try:
-                tests_list.append(self.fuzzer.parse_reproducer(file, idx))
-            except Exception:  # pylint: disable=broad-except
-                print(f"Parsing fail on {file}: index: {idx}")
-
-        # 4. Generate the test file
-        template = jinja2.Template(templates["CONTRACT"])
-        write_path = f"{self.test_dir}{self.target_name}"
-        inheritance_path = f"{self.inheritance_path}{self.target_name}"
-
-        # 5. Save the test file
-        test_file_str = template.render(
-            file_path=f"{inheritance_path}.sol",
-            target_name=self.target_name,
-            amount=0,
-            tests=tests_list,
-            fuzzer=self.fuzzer.name,
-        )
-        with open(f"{write_path}_{self.fuzzer.name}_Test.t.sol", "w", encoding="utf-8") as outfile:
-            outfile.write(test_file_str)
-        CryticPrint().print_success(
-            f"Generated a test file in {write_path}_{self.fuzzer.name}_Test.t.sol"
-        )
 
-        return test_file_str
-
-
-def main() -> None:  # type: ignore[func-returns-value]
-    """The main entry point"""
-    parser = argparse.ArgumentParser(
-        prog="fuzz-utils", description="Generate test harnesses for Echidna failed properties."
+def generate_flags(parser: ArgumentParser) -> None:
+    """The unit test generation parser flags"""
+    parser.add_argument(
+        "compilation_path", help="Path to the Echidna/Medusa test harness or Foundry directory."
     )
-    parser.add_argument("file_path", help="Path to the Echidna test harness.")
     parser.add_argument(
-        "-cd", "--corpus-dir", dest="corpus_dir", help="Path to the corpus directory", required=True
+        "-cd", "--corpus-dir", dest="corpus_dir", help="Path to the corpus directory"
     )
     parser.add_argument("-c", "--contract", dest="target_contract", help="Define the contract name")
     parser.add_argument(
         "-td",
         "--test-directory",
         dest="test_directory",
         help="Define the directory that contains the Foundry tests.",
@@ -119,50 +37,114 @@
     parser.add_argument(
         "-f",
         "--fuzzer",
         dest="selected_fuzzer",
         help="Define the fuzzer used. Valid inputs: 'echidna', 'medusa'",
     )
     parser.add_argument(
-        "--version",
-        help="displays the current version",
-        version=require("fuzz-utils")[0].version,
-        action="version",
-    )
-
-    args = parser.parse_args()
-
-    missing_args = [arg for arg, value in vars(args).items() if value is None]
-    if missing_args:
-        parser.print_help()
-        handle_exit(f"\n* Missing required arguments: {', '.join(missing_args)}")
-
-    file_path = args.file_path
-    corpus_dir = args.corpus_dir
-    test_directory = args.test_directory
-    inheritance_path = args.inheritance_path
-    target_contract = args.target_contract
-    slither = Slither(file_path)
+        "--named-inputs",
+        dest="named_inputs",
+        help="Include function input names when making calls.",
+        default=False,
+        action="store_true",
+    )
+    parser.add_argument(
+        "--config",
+        dest="config",
+        help="Define the location of the config file.",
+    )
+    parser.add_argument(
+        "--all-sequences",
+        dest="all_sequences",
+        help="Include all corpus sequences when generating unit tests.",
+        default=False,
+        action="store_true",
+    )
+
+
+# pylint: disable=too-many-branches
+def generate_command(args: Namespace) -> None:
+    """The execution logic of the `generate` command"""
+    config: dict = {}
+    # If the config file is defined, read it
+    if args.config:
+        config = open_config(args.config, COMMAND)
+    # Override the config with the CLI values
+    if args.compilation_path:
+        config["compilationPath"] = args.compilation_path
+    if args.test_directory:
+        config["testsDir"] = args.test_directory
+    if args.inheritance_path:
+        config["inheritancePath"] = args.inheritance_path
+    if args.selected_fuzzer:
+        config["fuzzer"] = args.selected_fuzzer.lower()
+    if args.corpus_dir:
+        config["corpusDir"] = args.corpus_dir
+    if args.target_contract:
+        config["targetContract"] = args.target_contract
+    if args.named_inputs:
+        config["namedInputs"] = args.named_inputs
+    else:
+        if "namedInputs" not in config:
+            config["namedInputs"] = False
+    if args.all_sequences:
+        config["allSequences"] = args.all_sequences
+    else:
+        if "allSequences" not in config:
+            config["allSequences"] = False
+
+    check_config_and_set_default_values(
+        config,
+        ["compilationPath", "testsDir", "fuzzer", "corpusDir"],
+        [".", "test", "medusa", "corpus"],
+    )
+
+    CryticPrint().print_information("Running Slither...")
+    slither = Slither(args.compilation_path)
     fuzzer: Echidna | Medusa
 
-    match args.selected_fuzzer.lower():
+    derive_config(slither, config)
+
+    match config["fuzzer"]:
         case "echidna":
-            fuzzer = Echidna(target_contract, corpus_dir, slither)
+            fuzzer = Echidna(
+                config["targetContract"], config["corpusDir"], slither, config["namedInputs"]
+            )
         case "medusa":
-            fuzzer = Medusa(target_contract, corpus_dir, slither)
+            fuzzer = Medusa(
+                config["targetContract"], config["corpusDir"], slither, config["namedInputs"]
+            )
         case _:
             handle_exit(
-                f"\n* The requested fuzzer {args.selected_fuzzer} is not supported. Supported fuzzers: echidna, medusa."
+                f"\n* The requested fuzzer {config['fuzzer']} is not supported. Supported fuzzers: echidna, medusa."
             )
 
     CryticPrint().print_information(
         f"Generating Foundry unit tests based on the {fuzzer.name} reproducers..."
     )
-    foundry_test = FoundryTest(
-        inheritance_path, target_contract, corpus_dir, test_directory, slither, fuzzer
-    )
+    foundry_test = FoundryTest(config, slither, fuzzer)
     foundry_test.create_poc()
     CryticPrint().print_success("Done!")
 
 
-if __name__ == "__main__":
-    sys.exit(main())  # type: ignore[func-returns-value]
+def derive_config(slither: Slither, config: dict) -> None:
+    """Derive values for the target contract and inheritance path"""
+    # Derive target if it is not defined but the compilationPath only contains one contract
+    if "targetContract" not in config or len(config["targetContract"]) == 0:
+        if len(slither.contracts_derived) == 1:
+            config["targetContract"] = slither.contracts_derived[0].name
+            CryticPrint().print_information(
+                f"Target contract not specified. Using derived target: {config['targetContract']}."
+            )
+        else:
+            handle_exit(
+                "Target contract cannot be determined. Please specify the target with `-c targetName`"
+            )
+
+    # Derive inheritance path if it is not defined
+    if "inheritancePath" not in config or len(config["inheritancePath"]) == 0:
+        contract = get_target_contract(slither, config["targetContract"])
+        contract_path = Path(contract.source_mapping.filename.relative)
+        tests_path = Path(config["testsDir"])
+        config["inheritancePath"] = str(
+            Path(*([".." * len(tests_path.parts)])).joinpath(contract_path)
+        )
```

### Comparing `fuzz-utils-0.0.1/fuzz_utils/templates/foundry_templates.py` & `fuzz-utils-0.2.0/fuzz_utils/templates/foundry_templates.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 """ Defines the template strings used to generate the test file"""
 
 __CONTRACT_TEMPLATE: str = """// SPDX-License-Identifier: UNLICENSED
 pragma solidity ^0.8.13;
+
+/// --------------------------------------------------------------------
+/// @notice This file was automatically generated using fuzz-utils 
+/// --------------------------------------------------------------------
+
 import "forge-std/Test.sol";
 import "forge-std/console2.sol";
 import "{{file_path}}";
 
 contract {{target_name}}_{{fuzzer}}_Test is Test {
     {{target_name}} target;
 
@@ -19,44 +24,48 @@
     {{test}}
     {% endfor %}
 }
 
     """
 
 __CALL_TEMPLATE: str = """
-        {%- if has_delay -%}
+        {%- if has_delay %}
         vm.warp(block.timestamp + {{time_delay}});
         vm.roll(block.number + {{block_delay}});
         {%- endif %}
         vm.prank({{caller}});
         {%- if value > 0 %}
         target.{{function_name}}{value: {{value}}}({{function_parameters}});
         {%- else %}
         target.{{function_name}}({{function_parameters}});
         {%- endif %}
 """
 
 __TRANSFER__TEMPLATE: str = """
-        {%- if has_delay -%}
+        {%- if has_delay %}
         vm.warp(block.timestamp + {{time_delay}});
         vm.roll(block.number + {{block_delay}});
         {%- endif %}
         vm.prank({{caller}});
-        (bool success, ) = payable(address(target)).call{value: {{value}}}("");
+        (success, ) = payable(address(target)).call{value: {{value}}}("");
         require(success, "Low level call failed.");
 """
 
 __EMPTY_CALL_TEMPLATE: str = """
         // This is an empty call which just increases the block number and timestamp
         vm.warp(block.timestamp + {{time_delay}});
         vm.roll(block.number + {{block_delay}});
     """
 
 __TEST_TEMPLATE: str = """
-    function test_auto_{{function_name}}() public { {% for call in call_list %}
+    // Reproduced from: {{file_path}}
+    function test_auto_{{function_name}}() public { 
+        {%- if has_low_level_call %}
+        bool success; 
+        {%- endif %} {% for call in call_list %}
         {{call}}{% endfor %}
     }"""
 
 __INTERFACE_TEMPLATE: str = """
 interface I{target_name} {
     {% for struct in structs -%}
     {{struct}}
```

### Comparing `fuzz-utils-0.0.1/fuzz_utils/utils/crytic_print.py` & `fuzz-utils-0.2.0/fuzz_utils/utils/crytic_print.py`

 * *Files identical despite different names*

### Comparing `fuzz-utils-0.0.1/pyproject.toml` & `fuzz-utils-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fuzz-utils"
-version = "0.0.1"
+version = "0.2.0"
 authors = [{ name = "Trail of Bits" }]
 description = "A tool for automatically generating unit tests from Echidna and Medusa reproducers."
 readme = "README.md"
 license = { "text" = "AGPL-3.0" }
 urls = { "Homepage" = "https://github.com/crytic/fuzz-utils" }
 requires-python = ">=3.10"
 dependencies = [
     "colorama>=0.4.0",
     "slither_analyzer>=0.10.0",
-    "jinja2>=3.1.0"
+    "jinja2>=3.1.0",
+    "eth_abi>=5.0.1",
+    "eth_utils>=4.0.0",
+    "eth_typing>=4.0.0"
 ]
 
 [project.optional-dependencies]
 lint = [
     "pylint==2.13.4",
     "black==22.3.0"
 ]
```

