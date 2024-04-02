# Comparing `tmp/esbmc_ai-0.4.0.dev6.tar.gz` & `tmp/esbmc_ai-0.4.0.post0.tar.gz`

## Comparing `esbmc_ai-0.4.0.dev6.tar` & `esbmc_ai-0.4.0.post0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/.env.example
--rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/.pylintrc
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/Pipfile
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/build.sh
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/clean.sh
--rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/config.json
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc-ai
--rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/requirements.txt
--rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/upload.sh
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/.github/workflows/workflow.yml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/.vscode/launch.json
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/.vscode/settings.json
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/__about__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/__init__.py
--rwxr-xr-x   0        0        0    14256 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/__main__.py
--rw-r--r--   0        0        0    11599 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/ai_models.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/api_key_collection.py
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/base_chat_interface.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/chat_response.py
--rw-r--r--   0        0        0    14227 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/config.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/esbmc_util.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/loading_widget.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/logging.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/msg_bus.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/optimize_code.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/solution_generator.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/user_chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/commands/__init__.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/commands/chat_command.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/commands/exit_command.py
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/commands/fix_code_command.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/commands/help_command.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/frontend/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/esbmc_ai/frontend/solution.py
--rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/notebooks/ast.ipynb
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/notebooks/samples/typedefs.c
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/add_last_unsafe.c
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/automatic_arrays.c
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/dynamic_mem_alloc.c
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/hello_world.c
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/mem_leak.c
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/optimize_code_test_01.c
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/threading.c
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/unsafe_access.c
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/ast/function_test_1.c
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/ast/function_test_2.c
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/optimize-code/fact_01.c
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/optimize-code/mult.c
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/optimize-code/sign_check.c
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/samples/optimize-code/sign_check_hard.c
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/scripts/function_equivalence.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/tests/__init__.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/tests/test_ai_models.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/tests/test_base_chat_interface.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/tests/test_command_parser.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/tests/test_config.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/tests/test_user_chat.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/tests/regtest/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/tests/regtest/test_base_chat_interface.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/LICENSE
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/README.md
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/pyproject.toml
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.dev6/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.env.example
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.pylintrc
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/Pipfile
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/build.sh
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/clean.sh
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/config.json
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc-ai
+-rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/requirements.txt
+-rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/upload.sh
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.vscode/launch.json
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.vscode/settings.json
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/__about__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/__init__.py
+-rwxr-xr-x   0        0        0    14256 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/__main__.py
+-rw-r--r--   0        0        0    11599 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/ai_models.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/api_key_collection.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/base_chat_interface.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/chat_response.py
+-rw-r--r--   0        0        0    14227 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/config.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/esbmc_util.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/loading_widget.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/logging.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/msg_bus.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/optimize_code.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/solution_generator.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/user_chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/commands/__init__.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/commands/chat_command.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/commands/exit_command.py
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/commands/fix_code_command.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/commands/help_command.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/frontend/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/frontend/solution.py
+-rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/notebooks/ast.ipynb
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/notebooks/samples/typedefs.c
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/add_last_unsafe.c
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/automatic_arrays.c
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/dynamic_mem_alloc.c
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/hello_world.c
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/mem_leak.c
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/optimize_code_test_01.c
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/threading.c
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/unsafe_access.c
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/ast/function_test_1.c
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/ast/function_test_2.c
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/optimize-code/fact_01.c
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/optimize-code/mult.c
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/optimize-code/sign_check.c
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/optimize-code/sign_check_hard.c
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/scripts/function_equivalence.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/__init__.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/test_ai_models.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/test_base_chat_interface.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/test_command_parser.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/test_config.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/test_user_chat.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/regtest/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/regtest/test_base_chat_interface.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/LICENSE
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/README.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/pyproject.toml
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/PKG-INFO
```

### Comparing `esbmc_ai-0.4.0.dev6/.pylintrc` & `esbmc_ai-0.4.0.post0/.pylintrc`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/config.json` & `esbmc_ai-0.4.0.post0/config.json`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/requirements.txt` & `esbmc_ai-0.4.0.post0/requirements.txt`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/.github/workflows/workflow.yml` & `esbmc_ai-0.4.0.post0/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/.vscode/launch.json` & `esbmc_ai-0.4.0.post0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/__main__.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/__main__.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/ai_models.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/base_chat_interface.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/base_chat_interface.py`

 * *Files 27% similar despite different names*

```diff
@@ -88,32 +88,14 @@
                     message=response_message,
                     total_tokens=self.ai_model.tokens,
                 )
             else:
                 response = ChatResponse(
                     finish_reason=FinishReason.stop,
                     message=response_message,
-                    total_tokens=self.ai_model.tokens,
+                    total_tokens=new_tokens,
                 )
-        # FIXME
-        # except TokenLimitExceededException as e:
-        #     # HFTextGen
-        #     response = ChatResponse(
-        #         finish_reason=FinishReason.length,
-        #         # NOTE Show the total tokens of the model instead of 0
-        #         # (no token counting currently...)
-        #         total_tokens=self.ai_model.tokens,
-        #     )
-        except InternalServerError as e:
-            # OpenAI model error handling.
-            if e.code == AIModelOpenAI.context_length_exceeded_error:
-                response = ChatResponse(
-                    finish_reason=FinishReason.length,
-                    total_tokens=self.ai_model.tokens,
-                )
-            else:
-                raise
         except Exception as e:
             print(f"There was an unkown error when generating a response: {e}")
             exit(1)
 
         return response
```

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/chat_response.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/chat_response.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/config.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/esbmc_util.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/esbmc_util.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/loading_widget.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/loading_widget.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/optimize_code.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/optimize_code.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/solution_generator.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/solution_generator.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/user_chat.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/commands/chat_command.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/commands/chat_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/commands/fix_code_command.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/commands/fix_code_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/commands/help_command.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/commands/help_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/esbmc_ai/frontend/solution.py` & `esbmc_ai-0.4.0.post0/esbmc_ai/frontend/solution.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/notebooks/ast.ipynb` & `esbmc_ai-0.4.0.post0/notebooks/ast.ipynb`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/notebooks/samples/typedefs.c` & `esbmc_ai-0.4.0.post0/notebooks/samples/typedefs.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/samples/add_last_unsafe.c` & `esbmc_ai-0.4.0.post0/samples/add_last_unsafe.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/samples/optimize-code/sign_check.c` & `esbmc_ai-0.4.0.post0/samples/optimize-code/sign_check.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/samples/optimize-code/sign_check_hard.c` & `esbmc_ai-0.4.0.post0/samples/optimize-code/sign_check_hard.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/scripts/function_equivalence.c` & `esbmc_ai-0.4.0.post0/scripts/function_equivalence.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/tests/test_ai_models.py` & `esbmc_ai-0.4.0.post0/tests/test_ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/tests/test_base_chat_interface.py` & `esbmc_ai-0.4.0.post0/tests/test_base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/tests/test_command_parser.py` & `esbmc_ai-0.4.0.post0/tests/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/tests/test_config.py` & `esbmc_ai-0.4.0.post0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/tests/test_user_chat.py` & `esbmc_ai-0.4.0.post0/tests/test_user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/tests/regtest/test_base_chat_interface.py` & `esbmc_ai-0.4.0.post0/tests/regtest/test_base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out` & `esbmc_ai-0.4.0.post0/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out`

 * *Files 15% similar despite different names*

```diff
@@ -1,3 +1,3 @@
 (SystemMessage(content='System message'), AIMessage(content='OK'))
 [HumanMessage(content='Test 1'), AIMessage(content='OK 1'), HumanMessage(content='Test 2'), AIMessage(content='OK 2'), HumanMessage(content='Test 3'), AIMessage(content='OK 3')]
-[ChatResponse(message=AIMessage(content='OK 1'), total_tokens=1024, finish_reason=<FinishReason.stop: 1>), ChatResponse(message=AIMessage(content='OK 2'), total_tokens=1024, finish_reason=<FinishReason.stop: 1>), ChatResponse(message=AIMessage(content='OK 3'), total_tokens=1024, finish_reason=<FinishReason.stop: 1>)]
+[ChatResponse(message=AIMessage(content='OK 1'), total_tokens=15, finish_reason=<FinishReason.stop: 1>), ChatResponse(message=AIMessage(content='OK 2'), total_tokens=23, finish_reason=<FinishReason.stop: 1>), ChatResponse(message=AIMessage(content='OK 3'), total_tokens=31, finish_reason=<FinishReason.stop: 1>)]
```

### Comparing `esbmc_ai-0.4.0.dev6/.gitignore` & `esbmc_ai-0.4.0.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/LICENSE` & `esbmc_ai-0.4.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/README.md` & `esbmc_ai-0.4.0.post0/README.md`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.dev6/pyproject.toml` & `esbmc_ai-0.4.0.post0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "esbmc_ai"
 # https://hatch.pypa.io/latest/version/
-# version = "0.4.0dev0"
 dynamic = ["version"]
 authors = [
   { name="Yiannis Charalambous", email="yiannis128@hotmail.com" },
 ]
 description = "LLM driven development and automatic repair kit."
 readme = "README.md"
 license-files = { paths = ["LICENSE"] }
@@ -62,8 +61,26 @@
 "Source Code" = "https://github.com/Yiannis128/esbmc-ai"
 Documentation = "https://github.com/Yiannis128/esbmc-ai/wiki"
 Issues = "https://github.com/Yiannis128/esbmc-ai/issues"
 
 [tool.hatch.version]
 path = "esbmc_ai/__about__.py"
 
+# [tool.hatch.build.targets.esbmc_ai]
+# ignore-vcs = true
+# include = [
+#   "/esbmc_ai/**/*.py",
+#   "/esbmc_ai_config/**/*.py",
+# ]
+# exclude = [
+#  "/.github/*",
+#  "/.vscode",
+#  "/notebooks",
+#  "/samples",
+#  "/scripts",
+#  "/tests",
+#  "/env.example",
+#  "/.gitignore"
+# ]
 
+# [tool.hatch.build.targets.esbmc_ai.force-include]
+# "config.json" = "esbmc_ai_config/data/config.template.json"
```

### Comparing `esbmc_ai-0.4.0.dev6/PKG-INFO` & `esbmc_ai-0.4.0.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esbmc_ai
-Version: 0.4.0.dev6
+Version: 0.4.0.post0
 Summary: LLM driven development and automatic repair kit.
 Project-URL: Homepage, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Source Code, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Documentation, https://github.com/Yiannis128/esbmc-ai/wiki
 Project-URL: Issues, https://github.com/Yiannis128/esbmc-ai/issues
 Author-email: Yiannis Charalambous <yiannis128@hotmail.com>
 License-File: LICENSE
```

