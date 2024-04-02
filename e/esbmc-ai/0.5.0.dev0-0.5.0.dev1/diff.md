# Comparing `tmp/esbmc_ai-0.5.0.dev0.tar.gz` & `tmp/esbmc_ai-0.5.0.dev1.tar.gz`

## Comparing `esbmc_ai-0.5.0.dev0.tar` & `esbmc_ai-0.5.0.dev1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.env.example
--rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.pylintrc
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/Pipfile
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/build.sh
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/clean.sh
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/config.json
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc-ai
--rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/requirements.txt
--rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/upload.sh
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.github/workflows/workflow.yml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.vscode/launch.json
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.vscode/settings.json
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/__about__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/__init__.py
--rwxr-xr-x   0        0        0    14393 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/__main__.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/ai_models.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/api_key_collection.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/base_chat_interface.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/chat_response.py
--rw-r--r--   0        0        0    15189 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/config.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/esbmc_util.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/loading_widget.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/logging.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/msg_bus.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/optimize_code.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/solution_generator.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/user_chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/commands/__init__.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/commands/chat_command.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/commands/exit_command.py
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/commands/fix_code_command.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/commands/help_command.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/frontend/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/esbmc_ai/frontend/solution.py
--rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/notebooks/ast.ipynb
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/notebooks/samples/typedefs.c
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/add_last_unsafe.c
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/automatic_arrays.c
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/dynamic_mem_alloc.c
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/hello_world.c
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/mem_leak.c
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/optimize_code_test_01.c
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/threading.c
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/unsafe_access.c
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/ast/function_test_1.c
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/ast/function_test_2.c
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/optimize-code/fact_01.c
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/optimize-code/mult.c
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/optimize-code/sign_check.c
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/samples/optimize-code/sign_check_hard.c
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/scripts/function_equivalence.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/__init__.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_ai_models.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_base_chat_interface.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_command_parser.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_config.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_esbmc_util.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_solution.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_solution_generator.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/test_user_chat.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/regtest/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/regtest/test_base_chat_interface.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
--rw-r--r--   0        0        0  5597855 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c
--rw-r--r--   0        0        0  1700020 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c
--rw-r--r--   0        0        0  1226238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c
--rw-r--r--   0        0        0  2808039 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c
--rw-r--r--   0        0        0   373267 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/LICENSE
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/README.md
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/.env.example
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/.pylintrc
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/Pipfile
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/build.sh
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/clean.sh
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/config.json
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc-ai
+-rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/requirements.txt
+-rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/upload.sh
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/.vscode/launch.json
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/.vscode/settings.json
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/__about__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/__init__.py
+-rwxr-xr-x   0        0        0    14393 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/__main__.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/ai_models.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/api_key_collection.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/base_chat_interface.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/chat_response.py
+-rw-r--r--   0        0        0    15189 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/config.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/esbmc_util.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/loading_widget.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/logging.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/msg_bus.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/optimize_code.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/solution_generator.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/user_chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/commands/__init__.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/commands/chat_command.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/commands/exit_command.py
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/commands/fix_code_command.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/commands/help_command.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/frontend/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/esbmc_ai/frontend/solution.py
+-rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/notebooks/ast.ipynb
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/notebooks/samples/typedefs.c
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/add_last_unsafe.c
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/automatic_arrays.c
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/dynamic_mem_alloc.c
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/hello_world.c
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/mem_leak.c
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/optimize_code_test_01.c
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/threading.c
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/unsafe_access.c
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/ast/function_test_1.c
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/ast/function_test_2.c
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/optimize-code/fact_01.c
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/optimize-code/mult.c
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/optimize-code/sign_check.c
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/samples/optimize-code/sign_check_hard.c
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/scripts/function_equivalence.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/__init__.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/test_ai_models.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/test_base_chat_interface.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/test_command_parser.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/test_config.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/test_esbmc_util.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/test_solution.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/test_solution_generator.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/test_user_chat.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/regtest/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/regtest/test_base_chat_interface.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
+-rw-r--r--   0        0        0  5597855 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c
+-rw-r--r--   0        0        0  1700020 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c
+-rw-r--r--   0        0        0  1226238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c
+-rw-r--r--   0        0        0  2808039 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c
+-rw-r--r--   0        0        0   373267 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/LICENSE
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/README.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev1/PKG-INFO
```

### Comparing `esbmc_ai-0.5.0.dev0/.pylintrc` & `esbmc_ai-0.5.0.dev1/.pylintrc`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/Pipfile` & `esbmc_ai-0.5.0.dev1/Pipfile`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/config.json` & `esbmc_ai-0.5.0.dev1/config.json`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/requirements.txt` & `esbmc_ai-0.5.0.dev1/requirements.txt`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/.github/workflows/workflow.yml` & `esbmc_ai-0.5.0.dev1/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/.vscode/launch.json` & `esbmc_ai-0.5.0.dev1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/__main__.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/__main__.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/ai_models.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/base_chat_interface.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/chat_response.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/chat_response.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/config.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/esbmc_util.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/esbmc_util.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/loading_widget.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/loading_widget.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/optimize_code.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/optimize_code.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/solution_generator.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/solution_generator.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/user_chat.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/commands/chat_command.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/commands/chat_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/commands/fix_code_command.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/commands/fix_code_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,25 +124,26 @@
 
             # Failure case
             print(f"Failure {idx+1}/{max_retries}: Retrying...")
             # If final iteration no need to sleep.
             if idx < max_retries - 1:
 
                 # Inform solution generator chat about the ESBMC response.
+                # TODO Add option to customize in config.
                 if exit_code != 1:
                     # The program did not compile.
                     solution_generator.push_to_message_stack(
                         message=HumanMessage(
-                            content=f"The source code you provided does not compile. Fix the compilation errors. Use ESBMC output to fix the compilation errors:\n\n```\n{esbmc_output}\n```"
+                            content=f"Here is the ESBMC output, please fix the code:\n\n```\n{esbmc_output}\n```"
                         )
                     )
                 else:
                     solution_generator.push_to_message_stack(
                         message=HumanMessage(
-                            content=f"ESBMC has reported that verification failed, use the ESBMC output to find out what is wrong, and fix it. Here is ESBMC output:\n\n```\n{esbmc_output}\n```"
+                            content=f"Here is the ESBMC output, please fix the code:\n\n```\n{esbmc_output}\n```"
                         )
                     )
 
                 solution_generator.push_to_message_stack(
                     AIMessage(content="Understood.")
                 )
```

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/commands/help_command.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/commands/help_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/esbmc_ai/frontend/solution.py` & `esbmc_ai-0.5.0.dev1/esbmc_ai/frontend/solution.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/notebooks/ast.ipynb` & `esbmc_ai-0.5.0.dev1/notebooks/ast.ipynb`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/notebooks/samples/typedefs.c` & `esbmc_ai-0.5.0.dev1/notebooks/samples/typedefs.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/samples/add_last_unsafe.c` & `esbmc_ai-0.5.0.dev1/samples/add_last_unsafe.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/samples/optimize-code/sign_check.c` & `esbmc_ai-0.5.0.dev1/samples/optimize-code/sign_check.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/samples/optimize-code/sign_check_hard.c` & `esbmc_ai-0.5.0.dev1/samples/optimize-code/sign_check_hard.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/scripts/function_equivalence.c` & `esbmc_ai-0.5.0.dev1/scripts/function_equivalence.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/test_ai_models.py` & `esbmc_ai-0.5.0.dev1/tests/test_ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/test_base_chat_interface.py` & `esbmc_ai-0.5.0.dev1/tests/test_base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/test_command_parser.py` & `esbmc_ai-0.5.0.dev1/tests/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/test_config.py` & `esbmc_ai-0.5.0.dev1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/test_esbmc_util.py` & `esbmc_ai-0.5.0.dev1/tests/test_esbmc_util.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/test_solution_generator.py` & `esbmc_ai-0.5.0.dev1/tests/test_solution_generator.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/test_user_chat.py` & `esbmc_ai-0.5.0.dev1/tests/test_user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/regtest/test_base_chat_interface.py` & `esbmc_ai-0.5.0.dev1/tests/regtest/test_base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out` & `esbmc_ai-0.5.0.dev1/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c` & `esbmc_ai-0.5.0.dev1/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c` & `esbmc_ai-0.5.0.dev1/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c` & `esbmc_ai-0.5.0.dev1/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c` & `esbmc_ai-0.5.0.dev1/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c` & `esbmc_ai-0.5.0.dev1/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c` & `esbmc_ai-0.5.0.dev1/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/.gitignore` & `esbmc_ai-0.5.0.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/LICENSE` & `esbmc_ai-0.5.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/README.md` & `esbmc_ai-0.5.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/pyproject.toml` & `esbmc_ai-0.5.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev0/PKG-INFO` & `esbmc_ai-0.5.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: esbmc_ai
-Version: 0.5.0.dev0
+Version: 0.5.0.dev1
 Summary: LLM driven development and automatic repair kit.
 Project-URL: Homepage, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Source Code, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Documentation, https://github.com/Yiannis128/esbmc-ai/wiki
 Project-URL: Issues, https://github.com/Yiannis128/esbmc-ai/issues
 Author-email: Yiannis Charalambous <yiannis128@hotmail.com>
 License-File: LICENSE
```

