# Comparing `tmp/esbmc_ai-0.4.0.post0.tar.gz` & `tmp/esbmc_ai-0.5.0.dev0.tar.gz`

## Comparing `esbmc_ai-0.4.0.post0.tar` & `esbmc_ai-0.5.0.dev0.tar`

### file list

```diff
@@ -1,67 +1,76 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.env.example
--rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.pylintrc
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/Pipfile
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/build.sh
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/clean.sh
--rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/config.json
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc-ai
--rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/requirements.txt
--rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/upload.sh
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.github/workflows/workflow.yml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.vscode/launch.json
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.vscode/settings.json
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/__about__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/__init__.py
--rwxr-xr-x   0        0        0    14256 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/__main__.py
--rw-r--r--   0        0        0    11599 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/ai_models.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/api_key_collection.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/base_chat_interface.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/chat_response.py
--rw-r--r--   0        0        0    14227 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/config.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/esbmc_util.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/loading_widget.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/logging.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/msg_bus.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/optimize_code.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/solution_generator.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/user_chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/commands/__init__.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/commands/chat_command.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/commands/exit_command.py
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/commands/fix_code_command.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/commands/help_command.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/frontend/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/esbmc_ai/frontend/solution.py
--rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/notebooks/ast.ipynb
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/notebooks/samples/typedefs.c
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/add_last_unsafe.c
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/automatic_arrays.c
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/dynamic_mem_alloc.c
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/hello_world.c
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/mem_leak.c
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/optimize_code_test_01.c
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/threading.c
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/unsafe_access.c
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/ast/function_test_1.c
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/ast/function_test_2.c
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/optimize-code/fact_01.c
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/optimize-code/mult.c
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/optimize-code/sign_check.c
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/samples/optimize-code/sign_check_hard.c
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/scripts/function_equivalence.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/__init__.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/test_ai_models.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/test_base_chat_interface.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/test_command_parser.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/test_config.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/test_user_chat.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/regtest/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/regtest/test_base_chat_interface.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/LICENSE
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/README.md
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/pyproject.toml
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 esbmc_ai-0.4.0.post0/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.env.example
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.pylintrc
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/Pipfile
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/build.sh
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/clean.sh
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/config.json
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc-ai
+-rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/requirements.txt
+-rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/upload.sh
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.vscode/launch.json
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.vscode/settings.json
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/__about__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/__init__.py
+-rwxr-xr-x   0        0        0    14393 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/__main__.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/ai_models.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/api_key_collection.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/base_chat_interface.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/chat_response.py
+-rw-r--r--   0        0        0    15189 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/config.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/esbmc_util.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/loading_widget.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/logging.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/msg_bus.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/optimize_code.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/solution_generator.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/user_chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/commands/__init__.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/commands/chat_command.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/commands/exit_command.py
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/commands/fix_code_command.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/commands/help_command.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/frontend/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/frontend/solution.py
+-rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/notebooks/ast.ipynb
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/notebooks/samples/typedefs.c
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/add_last_unsafe.c
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/automatic_arrays.c
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/dynamic_mem_alloc.c
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/hello_world.c
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/mem_leak.c
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/optimize_code_test_01.c
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/threading.c
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/unsafe_access.c
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/ast/function_test_1.c
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/ast/function_test_2.c
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/optimize-code/fact_01.c
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/optimize-code/mult.c
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/optimize-code/sign_check.c
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/optimize-code/sign_check_hard.c
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/scripts/function_equivalence.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/__init__.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_ai_models.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_base_chat_interface.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_command_parser.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_config.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_esbmc_util.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_solution.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_solution_generator.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_user_chat.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/regtest/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/regtest/test_base_chat_interface.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
+-rw-r--r--   0        0        0  5597855 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c
+-rw-r--r--   0        0        0  1700020 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c
+-rw-r--r--   0        0        0  1226238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c
+-rw-r--r--   0        0        0  2808039 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c
+-rw-r--r--   0        0        0   373267 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/LICENSE
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/README.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/PKG-INFO
```

### Comparing `esbmc_ai-0.4.0.post0/.pylintrc` & `esbmc_ai-0.5.0.dev0/.pylintrc`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/Pipfile` & `esbmc_ai-0.5.0.dev0/Pipfile`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/config.json` & `esbmc_ai-0.5.0.dev0/config.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6297619047619047%*

 * *Differences: {"'chat_modes'": "{'generate_solution': {'max_attempts': 5}, delete: ['optimize_code']}",*

 * * "'esbmc_output_type'": "'vp'",*

 * * "'llm_requests'": "OrderedDict([('max_tries', 5), ('timeout', 60)])",*

 * * "'source_code_format'": "'full'",*

 * * "'verifier_timeout'": '90',*

 * * 'delete': "['consecutive_prompt_delay']"}*

```diff
@@ -1,14 +1,15 @@
 {
     "ai_custom": {},
     "ai_model": "gpt-3.5-turbo-16k",
     "allow_successful": true,
     "chat_modes": {
         "generate_solution": {
             "initial": "Generate a correction for the source code provided. Show the code only. Do not reply with acknowledgements.",
+            "max_attempts": 5,
             "scenarios": {
                 "division by zero": {
                     "system": [
                         {
                             "content": "Here's a C program with a vulnerability:\n```c\n{source_code}\n```\nA Formal Verification tool identified a division by zero issue:\n{esbmc_output}\nTask: Modify the C code to safely handle scenarios where division by zero might occur. The solution should prevent undefined behavior or crashes due to division by zero. \nGuidelines: Focus on making essential changes only. Avoid adding or modifying comments, and ensure the changes are precise and minimal.\nGuidelines: Ensure the revised code avoids undefined behavior and handles division by zero cases effectively.\nGuidelines: Implement safeguards (like comparison) to prevent division by zero instead of using literal divisions like 1.0/0.0.Output: Provide the corrected, complete C code. The solution should compile and run error-free, addressing the division by zero vulnerability.\nStart the code snippet with ```c and end with ```. Reply OK if you understand.",
                             "role": "System"
                         },
@@ -43,36 +44,14 @@
                 {
                     "content": "OK",
                     "role": "AI"
                 }
             ],
             "temperature": 1.3
         },
-        "optimize_code": {
-            "esbmc_params": [
-                "--incremental-bmc",
-                "--no-bounds-check",
-                "--no-pointer-check",
-                "--no-div-by-zero-check",
-                "--max-k-step",
-                "10"
-            ],
-            "initial": "Optimize the function \"%s\". Reoply with the entire source file back.",
-            "system": [
-                {
-                    "content": "You are a code optimizer. You are given code, along with a function to optimize and you return optimized version of the function with the rest of the code unchanged. The optimized function should be smaller than the original function if possible and also execute faster than the original. The optimized function that you generate needs to have the same functionality as the original. From this point on, you can only reply in source code. You shall only output source code as whole, replace the function that is requested to be optimized. Reply OK if you understand.",
-                    "role": "System"
-                },
-                {
-                    "content": "OK",
-                    "role": "AI"
-                }
-            ],
-            "temperature": 1.0
-        },
         "user_chat": {
             "initial": "Walk me through the source code, while also explaining the output of ESBMC at the relevant parts. You shall not start the reply with an acknowledgement message such as 'Certainly'.",
             "set_solution": [
                 {
                     "content": "Here is the corrected code:\n\n```c\n{source_code_solution}```",
                     "role": "System"
                 },
@@ -106,15 +85,15 @@
                     "content": "OK",
                     "role": "AI"
                 }
             ],
             "temperature": 1.0
         }
     },
-    "consecutive_prompt_delay": 20,
+    "esbmc_output_type": "vp",
     "esbmc_params": [
         "--interval-analysis",
         "--goto-unwind",
         "--unlimited-goto-unwind",
         "--k-induction",
         "--state-hashing",
         "--add-symex-value-sets",
@@ -123,11 +102,17 @@
         "--floatbv",
         "--unlimited-k-steps",
         "--memory-leak-check",
         "--context-bound",
         "2"
     ],
     "esbmc_path": "~/.local/bin/esbmc",
+    "llm_requests": {
+        "max_tries": 5,
+        "timeout": 60
+    },
     "loading_hints": true,
+    "source_code_format": "full",
     "temp_auto_clean": false,
-    "temp_file_dir": "./temp"
+    "temp_file_dir": "./temp",
+    "verifier_timeout": 90
 }
```

### Comparing `esbmc_ai-0.4.0.post0/requirements.txt` & `esbmc_ai-0.5.0.dev0/requirements.txt`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/.github/workflows/workflow.yml` & `esbmc_ai-0.5.0.dev0/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/.vscode/launch.json` & `esbmc_ai-0.5.0.dev0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/esbmc_ai/__main__.py` & `esbmc_ai-0.5.0.dev0/esbmc_ai/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 
 # Author: Yiannis Charalambous 2023
 
 import os
 import re
 import sys
-from time import sleep
 
 # Enables arrow key functionality for input(). Do not remove import.
 import readline
 
 import argparse
 from langchain.base_language import BaseLanguageModel
 
@@ -250,14 +249,17 @@
 
     config.load_envs()
     config.load_config(config.cfg_path)
     config.load_args(args)
 
     check_health()
 
+    printv(f"Source code format: {config.source_code_format}")
+    printv(f"ESBMC output type: {config.esbmc_output_type}")
+
     anim: LoadingWidget = create_loading_widget()
 
     # Read the source code and esbmc output.
     printv("Reading source code...")
     print(f"Running ESBMC with {config.esbmc_params}\n")
 
     # Cast to string (for language servers)
@@ -268,14 +270,15 @@
         # Add the main source file to the solution explorer.
         set_main_source_file(SourceFile(args.filename, file.read()))
 
     anim.start("ESBMC is processing... Please Wait")
     exit_code, esbmc_output, esbmc_err_output = esbmc(
         path=get_main_source_file_path(),
         esbmc_params=config.esbmc_params,
+        timeout=config.verifier_timeout,
     )
     anim.stop()
 
     # Print verbose lvl 2
     printvv("-" * os.get_terminal_size().columns)
     printvv(esbmc_output)
     printvv(esbmc_err_output)
@@ -308,14 +311,16 @@
                     )
             sys.exit(0)
 
     printv(f"Initializing the LLM: {config.ai_model.name}\n")
     chat_llm: BaseLanguageModel = config.ai_model.create_llm(
         api_keys=config.api_keys,
         temperature=config.chat_prompt_user_mode.temperature,
+        requests_max_tries=config.requests_max_tries,
+        requests_timeout=config.requests_timeout,
     )
 
     printv("Creating user chat")
     global chat
     chat = UserChat(
         ai_model_agent=config.chat_prompt_user_mode,
         ai_model=config.ai_model,
@@ -400,17 +405,15 @@
             anim.stop()
             if response.finish_reason == FinishReason.stop:
                 break
             elif response.finish_reason == FinishReason.length:
                 anim.start(
                     "Message stack limit reached. Shortening message stack... Please Wait"
                 )
-                sleep(config.consecutive_prompt_delay)
                 chat.compress_message_stack()
-                sleep(config.consecutive_prompt_delay)
                 anim.stop()
                 continue
             else:
                 raise NotImplementedError(
                     f"User Chat Mode: Finish Reason: {response.finish_reason}"
                 )
```

### Comparing `esbmc_ai-0.4.0.post0/esbmc_ai/ai_models.py` & `esbmc_ai-0.5.0.dev0/esbmc_ai/ai_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Author: Yiannis Charalambous
 
 from abc import abstractmethod
 from typing import Any, Iterable, Union
 from enum import Enum
+from pydantic.v1.types import SecretStr
 from typing_extensions import override
 
 from langchain.prompts import PromptTemplate
 from langchain.base_language import BaseLanguageModel
 
 from langchain_openai import ChatOpenAI
-from langchain_community.llms import HuggingFaceTextGenInference
+from langchain_community.llms.huggingface_text_gen_inference import (
+    HuggingFaceTextGenInference,
+)
 
 from langchain.prompts.chat import (
     AIMessagePromptTemplate,
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
     SystemMessagePromptTemplate,
 )
@@ -39,14 +42,16 @@
         self.tokens = tokens
 
     @abstractmethod
     def create_llm(
         self,
         api_keys: APIKeyCollection,
         temperature: float = 1.0,
+        requests_max_tries: int = 5,
+        requests_timeout: float = 60,
     ) -> BaseLanguageModel:
         """Initializes a large language model model with the provided parameters."""
         raise NotImplementedError()
 
     @classmethod
     def convert_messages_to_tuples(
         cls, messages: Iterable[BaseMessage]
@@ -140,20 +145,24 @@
     """Error code for when the length has been reached."""
 
     @override
     def create_llm(
         self,
         api_keys: APIKeyCollection,
         temperature: float = 1.0,
+        requests_max_tries: int = 5,
+        requests_timeout: float = 60,
     ) -> BaseLanguageModel:
         return ChatOpenAI(
             model=self.name,
-            api_key=api_keys.openai,
+            api_key=SecretStr(api_keys.openai),
             max_tokens=None,
             temperature=temperature,
+            max_retries=requests_max_tries,
+            timeout=requests_timeout,
             model_kwargs={},
         )
 
 
 class AIModelTextGen(AIModel):
     """Below are only used for models that need them, such as models that
     are using the provider "text_inference_server"."""
@@ -201,27 +210,31 @@
         self.stop_sequences: list[str] = stop_sequences
 
     @override
     def create_llm(
         self,
         api_keys: APIKeyCollection,
         temperature: float = 1.0,
+        requests_max_tries: int = 5,
+        requests_timeout: float = 60,
     ) -> BaseLanguageModel:
         return HuggingFaceTextGenInference(
             client=None,
             async_client=None,
             inference_server_url=self.url,
             server_kwargs={
                 "headers": {"Authorization": f"Bearer {api_keys.huggingface}"}
             },
             # FIXME Need to find a way to make output bigger. When token
             # tracking for this LLM type is added.
             max_new_tokens=5000,
             temperature=temperature,
             stop_sequences=self.stop_sequences,
+            max_retries=requests_max_tries,
+            timeout=requests_timeout,
         )
 
     @override
     def apply_chat_template(
         self,
         messages: Iterable[BaseMessage],
         **format_values: Any,
```

### Comparing `esbmc_ai-0.4.0.post0/esbmc_ai/base_chat_interface.py` & `esbmc_ai-0.5.0.dev0/esbmc_ai/base_chat_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # Author: Yiannis Charalambous
 
 from abc import abstractmethod
 
 from langchain.base_language import BaseLanguageModel
-from langchain_community.callbacks import get_openai_callback
 from langchain.schema import (
     AIMessage,
     BaseMessage,
     HumanMessage,
     LLMResult,
     PromptValue,
 )
 
-from openai import InternalServerError
-
-from .config import ChatPromptSettings
+from esbmc_ai.config import ChatPromptSettings
 from .chat_response import ChatResponse, FinishReason
-from .ai_models import AIModel, AIModelOpenAI
+from .ai_models import AIModel
 
 
 class BaseChatInterface(object):
     def __init__(
         self,
         ai_model_agent: ChatPromptSettings,
         llm: BaseLanguageModel,
```

### Comparing `esbmc_ai-0.4.0.post0/esbmc_ai/chat_response.py` & `esbmc_ai-0.5.0.dev0/esbmc_ai/chat_response.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/esbmc_ai/config.py` & `esbmc_ai-0.5.0.dev0/esbmc_ai/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,17 +34,25 @@
     "--compact-trace",
     "--context-bound",
     "2",
 ]
 
 temp_auto_clean: bool = True
 temp_file_dir: str = "."
-consecutive_prompt_delay: float = 20.0
 ai_model: AIModel = AIModels.GPT_3.value
 
+esbmc_output_type: str = "full"
+source_code_format: str = "full"
+
+fix_code_max_attempts: int = 5
+
+requests_max_tries: int = 5
+requests_timeout: float = 60
+verifier_timeout: float = 60
+
 loading_hints: bool = False
 allow_successful: bool = False
 
 cfg_path: str
 
 
 class AIAgentConversation(NamedTuple):
@@ -281,30 +289,14 @@
             config["chat_modes"]["generate_solution"]["system"]
         ),
         initial_prompt=config["chat_modes"]["generate_solution"]["initial"],
         temperature=config["chat_modes"]["generate_solution"]["temperature"],
         scenarios=fcm_scenarios,
     )
 
-    global chat_prompt_optimize_code
-    chat_prompt_optimize_code = ChatPromptSettings(
-        system_messages=AIAgentConversation.load_from_config(
-            config["chat_modes"]["optimize_code"]["system"]
-        ),
-        initial_prompt=config["chat_modes"]["optimize_code"]["initial"],
-        temperature=config["chat_modes"]["optimize_code"]["temperature"],
-    )
-
-    global esbmc_params_optimize_code
-    esbmc_params_optimize_code, _ = _load_config_value(
-        config["chat_modes"]["optimize_code"],
-        "esbmc_params",
-        esbmc_params_optimize_code,
-    )
-
 
 def _load_config_value(
     config_file: dict, name: str, default: object = None
 ) -> tuple[Any, bool]:
     if name in config_file:
         return config_file[name], True
     else:
@@ -353,19 +345,68 @@
     global esbmc_params
     esbmc_params, _ = _load_config_value(
         config_file,
         "esbmc_params",
         esbmc_params,
     )
 
-    global consecutive_prompt_delay
-    consecutive_prompt_delay = _load_config_real_number(
-        config_file,
-        "consecutive_prompt_delay",
-        consecutive_prompt_delay,
+    global fix_code_max_attempts
+    fix_code_max_attempts = int(
+        _load_config_real_number(
+            config_file=config_file["chat_modes"]["generate_solution"],
+            name="max_attempts",
+            default=fix_code_max_attempts,
+        )
+    )
+
+    global source_code_format
+    source_code_format, _ = _load_config_value(
+        config_file=config_file,
+        name="source_code_format",
+        default=source_code_format,
+    )
+
+    if source_code_format not in ["full", "single"]:
+        raise Exception(
+            f"Source code format in the config is not valid: {source_code_format}"
+        )
+
+    global esbmc_output_type
+    esbmc_output_type, _ = _load_config_value(
+        config_file=config_file,
+        name="esbmc_output_type",
+        default=esbmc_output_type,
+    )
+
+    if esbmc_output_type not in ["full", "vp", "ce"]:
+        raise Exception(
+            f"ESBMC output type in the config is not valid: {esbmc_output_type}"
+        )
+
+    global requests_max_tries
+    requests_max_tries = int(
+        _load_config_real_number(
+            config_file=config_file["llm_requests"],
+            name="max_tries",
+            default=requests_max_tries,
+        )
+    )
+
+    global requests_timeout
+    requests_timeout = _load_config_real_number(
+        config_file=config_file["llm_requests"],
+        name="timeout",
+        default=requests_timeout,
+    )
+
+    global verifier_timeout
+    verifier_timeout = _load_config_real_number(
+        config_file=config_file,
+        name="verifier_timeout",
+        default=verifier_timeout,
     )
 
     global temp_auto_clean
     temp_auto_clean, _ = _load_config_value(
         config_file,
         "temp_auto_clean",
         temp_auto_clean,
```

### Comparing `esbmc_ai-0.4.0.post0/esbmc_ai/loading_widget.py` & `esbmc_ai-0.5.0.dev0/esbmc_ai/loading_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
         self.done = False
         self.loading_text = text
         self.thread = Thread(target=self._animate)
         self.thread.daemon = True
         self.thread.start()
 
     def stop(self) -> None:
+        if not config.loading_hints:
+            return
         self.done = True
         # Block until end.
         if self.thread:
             self.thread.join()
 
 
 _widgets: list[LoadingWidget] = []
```

### Comparing `esbmc_ai-0.4.0.post0/esbmc_ai/optimize_code.py` & `esbmc_ai-0.5.0.dev0/esbmc_ai/optimize_code.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/esbmc_ai/user_chat.py` & `esbmc_ai-0.5.0.dev0/esbmc_ai/user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/esbmc_ai/commands/chat_command.py` & `esbmc_ai-0.5.0.dev0/esbmc_ai/commands/chat_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/esbmc_ai/commands/fix_code_command.py` & `esbmc_ai-0.5.0.dev0/esbmc_ai/commands/fix_code_command.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Author: Yiannis Charalambous
 
 from os import get_terminal_size
-from time import sleep
 from typing import Any, Tuple
 from typing_extensions import override
 from langchain.schema import AIMessage, HumanMessage
 
 from esbmc_ai.chat_response import FinishReason
 
 from .chat_command import ChatCommand
 from .. import config
 from ..msg_bus import Signal
 from ..loading_widget import create_loading_widget
-from ..esbmc_util import esbmc_load_source_code
-from ..solution_generator import SolutionGenerator
+from ..esbmc_util import (
+    esbmc_get_error_type,
+    esbmc_load_source_code,
+)
+from ..solution_generator import SolutionGenerator, get_esbmc_output_formatted
 from ..logging import printv, printvv
 
 # TODO Remove built in messages and move them to config.
 
 
 class FixCodeCommand(ChatCommand):
     on_solution_signal: Signal = Signal()
@@ -25,121 +27,109 @@
     def __init__(self) -> None:
         super().__init__(
             command_name="fix-code",
             help_message="Generates a solution for this code, and reevaluates it with ESBMC.",
         )
         self.anim = create_loading_widget()
 
-    def _resolve_scenario(self, esbmc_output: str) -> str:
-        # Start search from the marker.
-        marker: str = "Violated property:\n"
-        violated_property_index: int = esbmc_output.rfind(marker) + len(marker)
-        from_loc_error_msg: str = esbmc_output[violated_property_index:]
-        # Find second new line which contains the location of the violated
-        # property and that should point to the line with the type of error.
-        # In this case, the type of error is the "scenario".
-        scenario_index: int = from_loc_error_msg.find("\n")
-        scenario: str = from_loc_error_msg[scenario_index + 1 :]
-        scenario_end_l_index: int = scenario.find("\n")
-        scenario = scenario[:scenario_end_l_index].strip()
-        return scenario
-
     @override
     def execute(self, **kwargs: Any) -> Tuple[bool, str]:
         file_name: str = kwargs["file_name"]
         source_code: str = kwargs["source_code"]
         esbmc_output: str = kwargs["esbmc_output"]
 
-        wait_time: int = int(config.consecutive_prompt_delay)
-        # Create time left animation to show how much time left between API calls
-        # This is done by creating a list of all the numbers to be displayed and
-        # setting the animation delay to 1 second.
-        wait_anim = create_loading_widget(
-            anim_speed=1,
-            animation=[str(num) for num in range(wait_time, 0, -1)],
-        )
-
         # Parse the esbmc output here and determine what "Scenario" to use.
-        scenario: str = self._resolve_scenario(esbmc_output)
+        scenario: str = esbmc_get_error_type(esbmc_output)
 
         printv(f"Scenario: {scenario}")
         printv(
             f"Using dynamic prompt..."
             if scenario in config.chat_prompt_generator_mode.scenarios
             else "Using generic prompt..."
         )
 
-        llm = config.ai_model.create_llm(
-            api_keys=config.api_keys,
-            temperature=config.chat_prompt_generator_mode.temperature,
-        )
-
         solution_generator = SolutionGenerator(
             ai_model_agent=config.chat_prompt_generator_mode,
             source_code=source_code,
             esbmc_output=esbmc_output,
             ai_model=config.ai_model,
-            llm=llm,
+            llm=config.ai_model.create_llm(
+                api_keys=config.api_keys,
+                temperature=config.chat_prompt_generator_mode.temperature,
+                requests_max_tries=config.requests_max_tries,
+                requests_timeout=config.requests_timeout,
+            ),
             scenario=scenario,
+            source_code_format=config.source_code_format,
+            esbmc_output_type=config.esbmc_output_type,
         )
 
         print()
 
-        max_retries: int = 10
+        max_retries: int = config.fix_code_max_attempts
         for idx in range(max_retries):
             # Get a response. Use while loop to account for if the message stack
             # gets full, then need to compress and retry.
-            response: str = ""
+            llm_solution: str = ""
             while True:
                 # Generate AI solution
                 self.anim.start("Generating Solution... Please Wait")
-                response, finish_reason = solution_generator.generate_solution()
+                llm_solution, finish_reason = solution_generator.generate_solution()
                 self.anim.stop()
                 if finish_reason == FinishReason.length:
                     self.anim.start("Compressing message stack... Please Wait")
                     solution_generator.compress_message_stack()
                     self.anim.stop()
                 else:
                     break
 
             # Print verbose lvl 2
             printvv("\nGeneration:")
             printvv("-" * get_terminal_size().columns)
-            printvv(response)
+            printvv(llm_solution)
             printvv("-" * get_terminal_size().columns)
             printvv("")
 
             # Pass to ESBMC, a workaround is used where the file is saved
             # to a temporary location since ESBMC needs it in file format.
             self.anim.start("Verifying with ESBMC... Please Wait")
             exit_code, esbmc_output, esbmc_err_output = esbmc_load_source_code(
                 file_path=file_name,
-                source_code=str(response),
+                source_code=llm_solution,
                 esbmc_params=config.esbmc_params,
                 auto_clean=config.temp_auto_clean,
+                timeout=config.verifier_timeout,
             )
             self.anim.stop()
 
+            # TODO Move this process into Solution Generator since have (beginning) is done
+            # inside, and the other half is done here.
+            try:
+                esbmc_output = get_esbmc_output_formatted(
+                    esbmc_output_type=config.esbmc_output_type,
+                    esbmc_output=esbmc_output,
+                )
+            except ValueError:
+                # Probably did not compile and so ESBMC source code is clang output.
+                pass
+
             # Print verbose lvl 2
             printvv("-" * get_terminal_size().columns)
             printvv(esbmc_output)
             printvv(esbmc_err_output)
             printvv("-" * get_terminal_size().columns)
 
             if exit_code == 0:
-                self.on_solution_signal.emit(response)
-                return False, response
+                self.on_solution_signal.emit(llm_solution)
+                return False, llm_solution
 
             # Failure case
             print(f"Failure {idx+1}/{max_retries}: Retrying...")
             # If final iteration no need to sleep.
             if idx < max_retries - 1:
-                wait_anim.start(f"Sleeping due to rate limit:")
-                sleep(config.consecutive_prompt_delay)
-                wait_anim.stop()
 
                 # Inform solution generator chat about the ESBMC response.
                 if exit_code != 1:
                     # The program did not compile.
                     solution_generator.push_to_message_stack(
                         message=HumanMessage(
                             content=f"The source code you provided does not compile. Fix the compilation errors. Use ESBMC output to fix the compilation errors:\n\n```\n{esbmc_output}\n```"
```

### Comparing `esbmc_ai-0.4.0.post0/esbmc_ai/commands/help_command.py` & `esbmc_ai-0.5.0.dev0/esbmc_ai/commands/help_command.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,12 +24,10 @@
 
         for command in self.commands:
             print(f"/{command.command_name}: {command.help_message}")
 
         print()
         print("Useful AI Questions:")
         print("1) How can I correct this code?")
-        print("2) Show me the corrected code.")
-        # TODO This needs to be uncommented as soon as ESBMC-AI can detect this query
-        # and trigger ESBMC to verify the code.
-        # print("3) Can you verify this corrected code with ESBMC again?")
+        print("2) What is the line with the error?")
+        print("3) What is the exact error?")
         print()
```

### Comparing `esbmc_ai-0.4.0.post0/notebooks/ast.ipynb` & `esbmc_ai-0.5.0.dev0/notebooks/ast.ipynb`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/notebooks/samples/typedefs.c` & `esbmc_ai-0.5.0.dev0/notebooks/samples/typedefs.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/samples/add_last_unsafe.c` & `esbmc_ai-0.5.0.dev0/samples/add_last_unsafe.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/samples/optimize-code/sign_check.c` & `esbmc_ai-0.5.0.dev0/samples/optimize-code/sign_check.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/samples/optimize-code/sign_check_hard.c` & `esbmc_ai-0.5.0.dev0/samples/optimize-code/sign_check_hard.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/scripts/function_equivalence.c` & `esbmc_ai-0.5.0.dev0/scripts/function_equivalence.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/tests/test_ai_models.py` & `esbmc_ai-0.5.0.dev0/tests/test_ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/tests/test_base_chat_interface.py` & `esbmc_ai-0.5.0.dev0/tests/test_base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/tests/test_command_parser.py` & `esbmc_ai-0.5.0.dev0/tests/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/tests/test_config.py` & `esbmc_ai-0.5.0.dev0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/tests/test_user_chat.py` & `esbmc_ai-0.5.0.dev0/tests/test_user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/tests/regtest/test_base_chat_interface.py` & `esbmc_ai-0.5.0.dev0/tests/regtest/test_base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out` & `esbmc_ai-0.5.0.dev0/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/.gitignore` & `esbmc_ai-0.5.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/LICENSE` & `esbmc_ai-0.5.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/README.md` & `esbmc_ai-0.5.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/pyproject.toml` & `esbmc_ai-0.5.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.4.0.post0/PKG-INFO` & `esbmc_ai-0.5.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: esbmc_ai
-Version: 0.4.0.post0
+Version: 0.5.0.dev0
 Summary: LLM driven development and automatic repair kit.
 Project-URL: Homepage, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Source Code, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Documentation, https://github.com/Yiannis128/esbmc-ai/wiki
 Project-URL: Issues, https://github.com/Yiannis128/esbmc-ai/issues
 Author-email: Yiannis Charalambous <yiannis128@hotmail.com>
 License-File: LICENSE
```

