# Comparing `tmp/esbmc_ai-0.5.0.dev2.tar.gz` & `tmp/esbmc_ai-0.5.0.dev3.tar.gz`

## Comparing `esbmc_ai-0.5.0.dev2.tar` & `esbmc_ai-0.5.0.dev3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/.env.example
--rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/.pylintrc
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/Pipfile
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/build.sh
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/clean.sh
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/config.json
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc-ai
--rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/requirements.txt
--rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/upload.sh
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/.github/workflows/workflow.yml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/.vscode/launch.json
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/.vscode/settings.json
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/__about__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/__init__.py
--rwxr-xr-x   0        0        0    14341 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/__main__.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/ai_models.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/api_key_collection.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/base_chat_interface.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/chat_response.py
--rw-r--r--   0        0        0    15189 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/config.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/esbmc_util.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/loading_widget.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/logging.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/msg_bus.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/optimize_code.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/solution_generator.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/user_chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/commands/__init__.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/commands/chat_command.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/commands/exit_command.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/commands/fix_code_command.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/commands/help_command.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/frontend/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/esbmc_ai/frontend/solution.py
--rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/notebooks/ast.ipynb
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/notebooks/samples/typedefs.c
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/add_last_unsafe.c
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/automatic_arrays.c
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/dynamic_mem_alloc.c
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/hello_world.c
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/mem_leak.c
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/optimize_code_test_01.c
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/threading.c
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/unsafe_access.c
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/ast/function_test_1.c
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/ast/function_test_2.c
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/optimize-code/fact_01.c
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/optimize-code/mult.c
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/optimize-code/sign_check.c
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/samples/optimize-code/sign_check_hard.c
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/scripts/function_equivalence.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/__init__.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/test_ai_models.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/test_base_chat_interface.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/test_command_parser.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/test_config.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/test_esbmc_util.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/test_solution.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/test_solution_generator.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/test_user_chat.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/regtest/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/regtest/test_base_chat_interface.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
--rw-r--r--   0        0        0  5597855 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c
--rw-r--r--   0        0        0  1700020 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c
--rw-r--r--   0        0        0  1226238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c
--rw-r--r--   0        0        0  2808039 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c
--rw-r--r--   0        0        0   373267 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/LICENSE
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/README.md
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.env.example
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.pylintrc
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/Pipfile
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/build.sh
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/clean.sh
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/config.json
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc-ai
+-rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/requirements.txt
+-rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/upload.sh
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.vscode/launch.json
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.vscode/settings.json
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/__about__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/__init__.py
+-rwxr-xr-x   0        0        0    14558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/__main__.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/ai_models.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/api_key_collection.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/base_chat_interface.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/chat_response.py
+-rw-r--r--   0        0        0    15345 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/config.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/esbmc_util.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/loading_widget.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/logging.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/msg_bus.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/optimize_code.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/solution_generator.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/user_chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/commands/__init__.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/commands/chat_command.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/commands/exit_command.py
+-rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/commands/fix_code_command.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/commands/help_command.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/frontend/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/frontend/solution.py
+-rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/notebooks/ast.ipynb
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/notebooks/samples/typedefs.c
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/add_last_unsafe.c
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/automatic_arrays.c
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/dynamic_mem_alloc.c
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/hello_world.c
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/mem_leak.c
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/optimize_code_test_01.c
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/threading.c
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/unsafe_access.c
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/ast/function_test_1.c
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/ast/function_test_2.c
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/optimize-code/fact_01.c
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/optimize-code/mult.c
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/optimize-code/sign_check.c
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/optimize-code/sign_check_hard.c
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/scripts/function_equivalence.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/__init__.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_ai_models.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_base_chat_interface.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_command_parser.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_config.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_esbmc_util.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_solution.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_solution_generator.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_user_chat.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/regtest/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/regtest/test_base_chat_interface.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
+-rw-r--r--   0        0        0  5597855 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c
+-rw-r--r--   0        0        0  1700020 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c
+-rw-r--r--   0        0        0  1226238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c
+-rw-r--r--   0        0        0  2808039 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c
+-rw-r--r--   0        0        0   373267 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/LICENSE
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/README.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/PKG-INFO
```

### Comparing `esbmc_ai-0.5.0.dev2/.pylintrc` & `esbmc_ai-0.5.0.dev3/.pylintrc`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/Pipfile` & `esbmc_ai-0.5.0.dev3/Pipfile`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/config.json` & `esbmc_ai-0.5.0.dev3/config.json`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/requirements.txt` & `esbmc_ai-0.5.0.dev3/requirements.txt`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/.github/workflows/workflow.yml` & `esbmc_ai-0.5.0.dev3/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/.vscode/launch.json` & `esbmc_ai-0.5.0.dev3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/__main__.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,14 +220,22 @@
         default="",
         help="Which AI model to use. Built-in models: {"
         + ", ".join(_ai_model_names)
         + ", +custom models}",
     )
 
     parser.add_argument(
+        "-r",
+        "--raw-conversation",
+        action="store_true",
+        default=False,
+        help="Show the raw conversation at the end of a command. Good for debugging...",
+    )
+
+    parser.add_argument(
         "-a",
         "--append",
         action="store_true",
         default=False,
         help="Any ESBMC parameters passed after the file name will be appended to the ones set in the config file, or the default ones if config file options are not set.",
     )
```

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/ai_models.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/base_chat_interface.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/chat_response.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/chat_response.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/config.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 
 requests_max_tries: int = 5
 requests_timeout: float = 60
 verifier_timeout: float = 60
 
 loading_hints: bool = False
 allow_successful: bool = False
+# Show the raw conversation after the command ends
+raw_conversation: bool = False
 
 cfg_path: str
 
 
 class AIAgentConversation(NamedTuple):
     """Immutable class describing the conversation definition for an AI agent. The
     class represents the system messages of the AI agent defined and contains a load
@@ -471,13 +473,16 @@
     if args.ai_model != "":
         if is_valid_ai_model(args.ai_model):
             ai_model = get_ai_model_by_name(args.ai_model)
         else:
             print(f"Error: invalid --ai-model parameter {args.ai_model}")
             sys.exit(4)
 
+    global raw_conversation
+    raw_conversation = args.raw_conversation
+
     global esbmc_params
     # If append flag is set, then append.
     if args.append:
         esbmc_params.extend(args.remaining)
     elif len(args.remaining) != 0:
         esbmc_params = args.remaining
```

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/esbmc_util.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/esbmc_util.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/loading_widget.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/loading_widget.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/optimize_code.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/optimize_code.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/solution_generator.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/solution_generator.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/user_chat.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/commands/chat_command.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/commands/chat_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/commands/fix_code_command.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/commands/fix_code_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,35 +115,48 @@
             # Print verbose lvl 2
             printvv("-" * get_terminal_size().columns)
             printvv(esbmc_output)
             printvv("-" * get_terminal_size().columns)
 
             if exit_code == 0:
                 self.on_solution_signal.emit(llm_solution)
+
+                if config.raw_conversation:
+                    messages: list[str] = [
+                        f"{msg.type}: {msg.content}"
+                        for msg in solution_generator.messages
+                    ]
+                    print("\n" + "\n\n".join(messages))
+
                 return False, llm_solution
 
             # Failure case
             print(f"Failure {idx+1}/{max_retries}: Retrying...")
             # If final iteration no need to sleep.
             if idx < max_retries - 1:
 
                 # Inform solution generator chat about the ESBMC response.
                 # TODO Add option to customize in config.
                 if exit_code != 1:
                     # The program did not compile.
                     solution_generator.push_to_message_stack(
                         message=HumanMessage(
-                            content=f"Here is the ESBMC output, please fix the code:\n\n```\n{esbmc_output}\n```"
+                            content=f"Here is the ESBMC output:\n\n```\n{esbmc_output}\n```"
                         )
                     )
                 else:
                     solution_generator.push_to_message_stack(
                         message=HumanMessage(
-                            content=f"Here is the ESBMC output, please fix the code:\n\n```\n{esbmc_output}\n```"
+                            content=f"Here is the ESBMC output:\n\n```\n{esbmc_output}\n```"
                         )
                     )
 
                 solution_generator.push_to_message_stack(
                     AIMessage(content="Understood.")
                 )
 
+        if config.raw_conversation:
+            messages: list[str] = [
+                f"{msg.type}: {msg.content}" for msg in solution_generator.messages
+            ]
+            print("\n" + "\n\n".join(messages))
         return True, "Failed all attempts..."
```

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/commands/help_command.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/commands/help_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/esbmc_ai/frontend/solution.py` & `esbmc_ai-0.5.0.dev3/esbmc_ai/frontend/solution.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/notebooks/ast.ipynb` & `esbmc_ai-0.5.0.dev3/notebooks/ast.ipynb`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/notebooks/samples/typedefs.c` & `esbmc_ai-0.5.0.dev3/notebooks/samples/typedefs.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/samples/add_last_unsafe.c` & `esbmc_ai-0.5.0.dev3/samples/add_last_unsafe.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/samples/optimize-code/sign_check.c` & `esbmc_ai-0.5.0.dev3/samples/optimize-code/sign_check.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/samples/optimize-code/sign_check_hard.c` & `esbmc_ai-0.5.0.dev3/samples/optimize-code/sign_check_hard.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/scripts/function_equivalence.c` & `esbmc_ai-0.5.0.dev3/scripts/function_equivalence.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/test_ai_models.py` & `esbmc_ai-0.5.0.dev3/tests/test_ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/test_base_chat_interface.py` & `esbmc_ai-0.5.0.dev3/tests/test_base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/test_command_parser.py` & `esbmc_ai-0.5.0.dev3/tests/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/test_config.py` & `esbmc_ai-0.5.0.dev3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/test_esbmc_util.py` & `esbmc_ai-0.5.0.dev3/tests/test_esbmc_util.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/test_solution_generator.py` & `esbmc_ai-0.5.0.dev3/tests/test_solution_generator.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/test_user_chat.py` & `esbmc_ai-0.5.0.dev3/tests/test_user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/regtest/test_base_chat_interface.py` & `esbmc_ai-0.5.0.dev3/tests/regtest/test_base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out` & `esbmc_ai-0.5.0.dev3/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c` & `esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c` & `esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c` & `esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c` & `esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c` & `esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c` & `esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/.gitignore` & `esbmc_ai-0.5.0.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/LICENSE` & `esbmc_ai-0.5.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/README.md` & `esbmc_ai-0.5.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/pyproject.toml` & `esbmc_ai-0.5.0.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev2/PKG-INFO` & `esbmc_ai-0.5.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: esbmc_ai
-Version: 0.5.0.dev2
+Version: 0.5.0.dev3
 Summary: LLM driven development and automatic repair kit.
 Project-URL: Homepage, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Source Code, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Documentation, https://github.com/Yiannis128/esbmc-ai/wiki
 Project-URL: Issues, https://github.com/Yiannis128/esbmc-ai/issues
 Author-email: Yiannis Charalambous <yiannis128@hotmail.com>
 License-File: LICENSE
```

