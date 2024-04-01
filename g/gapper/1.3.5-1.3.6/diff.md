# Comparing `tmp/gapper-1.3.5.tar.gz` & `tmp/gapper-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gapper-1.3.5.tar", max compression
+gzip compressed data, was "gapper-1.3.6.tar", max compression
```

## Comparing `gapper-1.3.5.tar` & `gapper-1.3.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1067 2024-03-23 19:19:20.679317 gapper-1.3.5/LICENSE
--rw-r--r--   0        0        0     1931 2024-03-23 19:19:20.679317 gapper-1.3.5/README.md
--rw-r--r--   0        0        0     1921 2024-03-23 19:19:20.683317 gapper-1.3.5/pyproject.toml
--rw-r--r--   0        0        0      798 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/__init__.py
--rw-r--r--   0        0        0       72 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/__main__.py
--rw-r--r--   0        0        0       56 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/_version.py
--rw-r--r--   0        0        0       65 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/cli/__init__.py
--rw-r--r--   0        0        0      492 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/cli/app.py
--rw-r--r--   0        0        0     1396 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/cli/check.py
--rw-r--r--   0        0        0     2712 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/cli/cli_options.py
--rw-r--r--   0        0        0     2826 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/cli/gen.py
--rw-r--r--   0        0        0     1538 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/cli/login.py
--rw-r--r--   0        0        0     1672 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/cli/rich_test_check_output.py
--rw-r--r--   0        0        0     1377 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/cli/rich_test_result_output.py
--rw-r--r--   0        0        0     2075 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/cli/run.py
--rw-r--r--   0        0        0     1357 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/cli/run_in_prod.py
--rw-r--r--   0        0        0     2476 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/cli/upload.py
--rw-r--r--   0        0        0     3450 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/cli/utils.py
--rw-r--r--   0        0        0       38 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/__init__.py
--rw-r--r--   0        0        0       29 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/api/__init__.py
--rw-r--r--   0        0        0     9394 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/api/account.py
--rw-r--r--   0        0        0     7775 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/api/assignment.py
--rw-r--r--   0        0        0     6733 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/api/course.py
--rw-r--r--   0        0        0     1295 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/api/mixins.py
--rw-r--r--   0        0        0     1264 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/api/utils.py
--rw-r--r--   0        0        0        0 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/gui/__init__.py
--rw-r--r--   0        0        0       83 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/gui/_test_app.py
--rw-r--r--   0        0        0     3060 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/gui/app_ui.py
--rw-r--r--   0        0        0     6624 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/gui/assignments_ui.py
--rw-r--r--   0        0        0     5695 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/gui/autograder_upload_ui.py
--rw-r--r--   0        0        0      180 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/gui/autograder_upload_ui.tcss
--rw-r--r--   0        0        0     5034 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/gui/course_assignment_ui.py
--rw-r--r--   0        0        0      478 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/gui/courses_assignment_ui.tcss
--rw-r--r--   0        0        0     6952 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/gui/login_ui.py
--rw-r--r--   0        0        0      517 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/gui/login_ui.tcss
--rw-r--r--   0        0        0      283 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/gui/messages.py
--rw-r--r--   0        0        0     1288 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/gui/upload_app_ui.py
--rw-r--r--   0        0        0      748 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/connect/gui/utils.py
--rw-r--r--   0        0        0        0 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/core/__init__.py
--rw-r--r--   0        0        0     5584 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/core/errors.py
--rw-r--r--   0        0        0     3540 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/core/file_handlers.py
--rw-r--r--   0        0        0     6419 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/core/hook.py
--rw-r--r--   0        0        0     6587 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/core/injection.py
--rw-r--r--   0        0        0     3419 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/core/pipeline_support.py
--rw-r--r--   0        0        0      147 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/core/problem/__init__.py
--rw-r--r--   0        0        0      181 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/core/problem/extras/__init__.py
--rw-r--r--   0        0        0     3087 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/core/problem/extras/gradescope_connect.py
--rw-r--r--   0        0        0     1117 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/core/problem/problem_config.py
--rw-r--r--   0        0        0     7438 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/core/problem/problem_def.py
--rw-r--r--   0        0        0     5619 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/core/result_synthesizer.py
--rw-r--r--   0        0        0    27743 2024-03-23 19:19:20.683317 gapper-1.3.5/src/gapper/core/test_parameter.py
--rw-r--r--   0        0        0     5156 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/core/test_result.py
--rw-r--r--   0        0        0      309 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/core/tester/__init__.py
--rw-r--r--   0        0        0     9322 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/core/tester/tester_def.py
--rw-r--r--   0        0        0      345 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/core/tester/tester_hooks.py
--rw-r--r--   0        0        0     5258 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/core/types.py
--rw-r--r--   0        0        0      144 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/core/unittest_wrapper/__init__.py
--rw-r--r--   0        0        0     1058 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/core/unittest_wrapper/utils.py
--rw-r--r--   0        0        0    12772 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/core/unittest_wrapper/wrapper_def.py
--rw-r--r--   0        0        0      564 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/core/unittest_wrapper/wrapper_hooks.py
--rw-r--r--   0        0        0     5896 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/core/utils.py
--rw-r--r--   0        0        0       48 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/gradescope/__init__.py
--rw-r--r--   0        0        0       36 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/gradescope/datatypes/__init__.py
--rw-r--r--   0        0        0     4397 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/gradescope/datatypes/gradescope_meta.py
--rw-r--r--   0        0        0     4955 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/gradescope/datatypes/gradescope_output.py
--rw-r--r--   0        0        0     2173 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/gradescope/main.py
--rw-r--r--   0        0        0     2667 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/gradescope/resources/requirements.txt
--rw-r--r--   0        0        0      129 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/gradescope/resources/run_autograder
--rw-r--r--   0        0        0      598 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/gradescope/resources/setup.j2
--rw-r--r--   0        0        0      985 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/gradescope/resources/setup.py
--rw-r--r--   0        0        0      476 2024-03-23 19:19:20.687317 gapper-1.3.5/src/gapper/gradescope/vars.py
--rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 gapper-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-01 23:41:44.998203 gapper-1.3.6/LICENSE
+-rw-r--r--   0        0        0     1931 2024-04-01 23:41:44.998203 gapper-1.3.6/README.md
+-rw-r--r--   0        0        0     1921 2024-04-01 23:41:45.002203 gapper-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0      798 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/__init__.py
+-rw-r--r--   0        0        0       72 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/__main__.py
+-rw-r--r--   0        0        0       56 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/_version.py
+-rw-r--r--   0        0        0       65 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/cli/__init__.py
+-rw-r--r--   0        0        0      492 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/cli/app.py
+-rw-r--r--   0        0        0     1396 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/cli/check.py
+-rw-r--r--   0        0        0     2712 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/cli/cli_options.py
+-rw-r--r--   0        0        0     2826 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/cli/gen.py
+-rw-r--r--   0        0        0     1538 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/cli/login.py
+-rw-r--r--   0        0        0     1672 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/cli/rich_test_check_output.py
+-rw-r--r--   0        0        0     1377 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/cli/rich_test_result_output.py
+-rw-r--r--   0        0        0     2075 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/cli/run.py
+-rw-r--r--   0        0        0     1357 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/cli/run_in_prod.py
+-rw-r--r--   0        0        0     2476 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/cli/upload.py
+-rw-r--r--   0        0        0     3450 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/cli/utils.py
+-rw-r--r--   0        0        0       38 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/__init__.py
+-rw-r--r--   0        0        0       29 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/api/__init__.py
+-rw-r--r--   0        0        0     9394 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/api/account.py
+-rw-r--r--   0        0        0     7775 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/api/assignment.py
+-rw-r--r--   0        0        0     6733 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/api/course.py
+-rw-r--r--   0        0        0     1295 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/api/mixins.py
+-rw-r--r--   0        0        0     1264 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/api/utils.py
+-rw-r--r--   0        0        0        0 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/gui/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/gui/_test_app.py
+-rw-r--r--   0        0        0     3060 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/gui/app_ui.py
+-rw-r--r--   0        0        0     6624 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/gui/assignments_ui.py
+-rw-r--r--   0        0        0     5695 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/gui/autograder_upload_ui.py
+-rw-r--r--   0        0        0      180 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/gui/autograder_upload_ui.tcss
+-rw-r--r--   0        0        0     5034 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/gui/course_assignment_ui.py
+-rw-r--r--   0        0        0      478 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/gui/courses_assignment_ui.tcss
+-rw-r--r--   0        0        0     6952 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/gui/login_ui.py
+-rw-r--r--   0        0        0      517 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/gui/login_ui.tcss
+-rw-r--r--   0        0        0      283 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/gui/messages.py
+-rw-r--r--   0        0        0     1288 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/gui/upload_app_ui.py
+-rw-r--r--   0        0        0      748 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/connect/gui/utils.py
+-rw-r--r--   0        0        0        0 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/__init__.py
+-rw-r--r--   0        0        0     5584 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/errors.py
+-rw-r--r--   0        0        0     3540 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/file_handlers.py
+-rw-r--r--   0        0        0     6419 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/hook.py
+-rw-r--r--   0        0        0     6587 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/injection.py
+-rw-r--r--   0        0        0     3419 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/pipeline_support.py
+-rw-r--r--   0        0        0      147 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/problem/__init__.py
+-rw-r--r--   0        0        0      181 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/problem/extras/__init__.py
+-rw-r--r--   0        0        0     3087 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/problem/extras/gradescope_connect.py
+-rw-r--r--   0        0        0     1117 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/problem/problem_config.py
+-rw-r--r--   0        0        0     7438 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/problem/problem_def.py
+-rw-r--r--   0        0        0     5699 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/result_synthesizer.py
+-rw-r--r--   0        0        0    27743 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/test_parameter.py
+-rw-r--r--   0        0        0     5156 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/test_result.py
+-rw-r--r--   0        0        0      309 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/tester/__init__.py
+-rw-r--r--   0        0        0     9322 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/tester/tester_def.py
+-rw-r--r--   0        0        0      345 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/tester/tester_hooks.py
+-rw-r--r--   0        0        0     5258 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/types.py
+-rw-r--r--   0        0        0      144 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/unittest_wrapper/__init__.py
+-rw-r--r--   0        0        0     1058 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/unittest_wrapper/utils.py
+-rw-r--r--   0        0        0    12772 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/unittest_wrapper/wrapper_def.py
+-rw-r--r--   0        0        0      564 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/unittest_wrapper/wrapper_hooks.py
+-rw-r--r--   0        0        0     5896 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/core/utils.py
+-rw-r--r--   0        0        0       48 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/gradescope/__init__.py
+-rw-r--r--   0        0        0       36 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/gradescope/datatypes/__init__.py
+-rw-r--r--   0        0        0     4397 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/gradescope/datatypes/gradescope_meta.py
+-rw-r--r--   0        0        0     4955 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/gradescope/datatypes/gradescope_output.py
+-rw-r--r--   0        0        0     2173 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/gradescope/main.py
+-rw-r--r--   0        0        0     2667 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/gradescope/resources/requirements.txt
+-rw-r--r--   0        0        0      129 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/gradescope/resources/run_autograder
+-rw-r--r--   0        0        0      598 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/gradescope/resources/setup.j2
+-rw-r--r--   0        0        0      985 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/gradescope/resources/setup.py
+-rw-r--r--   0        0        0      476 2024-04-01 23:41:45.002203 gapper-1.3.6/src/gapper/gradescope/vars.py
+-rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 gapper-1.3.6/PKG-INFO
```

### Comparing `gapper-1.3.5/LICENSE` & `gapper-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/README.md` & `gapper-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/pyproject.toml` & `gapper-1.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gapper"
-version = "1.3.5"
+version = "1.3.6"
 description = "Gradescope Autograder Packer"
 authors = ["Heyuan Zeng <hi@universe.observer>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/FlickerSoul/gapper"
 documentation = "https://gapper.universe.observer"
```

### Comparing `gapper-1.3.5/src/gapper/__init__.py` & `gapper-1.3.6/src/gapper/__init__.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/cli/check.py` & `gapper-1.3.6/src/gapper/cli/check.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/cli/cli_options.py` & `gapper-1.3.6/src/gapper/cli/cli_options.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/cli/gen.py` & `gapper-1.3.6/src/gapper/cli/gen.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/cli/login.py` & `gapper-1.3.6/src/gapper/cli/login.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/cli/rich_test_check_output.py` & `gapper-1.3.6/src/gapper/cli/rich_test_check_output.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/cli/rich_test_result_output.py` & `gapper-1.3.6/src/gapper/cli/rich_test_result_output.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/cli/run.py` & `gapper-1.3.6/src/gapper/cli/run.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/cli/run_in_prod.py` & `gapper-1.3.6/src/gapper/cli/run_in_prod.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/cli/upload.py` & `gapper-1.3.6/src/gapper/cli/upload.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/cli/utils.py` & `gapper-1.3.6/src/gapper/cli/utils.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/connect/api/account.py` & `gapper-1.3.6/src/gapper/connect/api/account.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/connect/api/assignment.py` & `gapper-1.3.6/src/gapper/connect/api/assignment.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/connect/api/course.py` & `gapper-1.3.6/src/gapper/connect/api/course.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/connect/api/mixins.py` & `gapper-1.3.6/src/gapper/connect/api/mixins.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/connect/api/utils.py` & `gapper-1.3.6/src/gapper/connect/api/utils.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/connect/gui/app_ui.py` & `gapper-1.3.6/src/gapper/connect/gui/app_ui.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/connect/gui/assignments_ui.py` & `gapper-1.3.6/src/gapper/connect/gui/assignments_ui.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/connect/gui/autograder_upload_ui.py` & `gapper-1.3.6/src/gapper/connect/gui/autograder_upload_ui.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/connect/gui/course_assignment_ui.py` & `gapper-1.3.6/src/gapper/connect/gui/course_assignment_ui.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/connect/gui/login_ui.py` & `gapper-1.3.6/src/gapper/connect/gui/login_ui.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/connect/gui/login_ui.tcss` & `gapper-1.3.6/src/gapper/connect/gui/login_ui.tcss`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/connect/gui/upload_app_ui.py` & `gapper-1.3.6/src/gapper/connect/gui/upload_app_ui.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/connect/gui/utils.py` & `gapper-1.3.6/src/gapper/connect/gui/utils.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/errors.py` & `gapper-1.3.6/src/gapper/core/errors.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/file_handlers.py` & `gapper-1.3.6/src/gapper/core/file_handlers.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/hook.py` & `gapper-1.3.6/src/gapper/core/hook.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/injection.py` & `gapper-1.3.6/src/gapper/core/injection.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/pipeline_support.py` & `gapper-1.3.6/src/gapper/core/pipeline_support.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/problem/extras/gradescope_connect.py` & `gapper-1.3.6/src/gapper/core/problem/extras/gradescope_connect.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/problem/problem_config.py` & `gapper-1.3.6/src/gapper/core/problem/problem_config.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/problem/problem_def.py` & `gapper-1.3.6/src/gapper/core/problem/problem_def.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/result_synthesizer.py` & `gapper-1.3.6/src/gapper/core/result_synthesizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,16 @@
         max_score_sum = 0.0
         weight_sum = 0
 
         for res in results:
             if res.max_score is not None and res.weight is not None:
                 raise InternalError(
                     "The max_score and weight of a test (result) cannot both be set. "
-                    f"But {res.rich_test_name} has both being None."
+                    f"But case `{res.rich_test_name}` has both being set. "
+                    f"max_score: {res.max_score}, weight: {res.weight}."
                 )
 
             if res.max_score is not None:
                 results_with_score.append(res)
                 max_score_sum += res.max_score
             elif res.weight is not None:
                 results_with_weight.append(res)
```

### Comparing `gapper-1.3.5/src/gapper/core/test_parameter.py` & `gapper-1.3.6/src/gapper/core/test_parameter.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/test_result.py` & `gapper-1.3.6/src/gapper/core/test_result.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/tester/tester_def.py` & `gapper-1.3.6/src/gapper/core/tester/tester_def.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/types.py` & `gapper-1.3.6/src/gapper/core/types.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/unittest_wrapper/utils.py` & `gapper-1.3.6/src/gapper/core/unittest_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/unittest_wrapper/wrapper_def.py` & `gapper-1.3.6/src/gapper/core/unittest_wrapper/wrapper_def.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/unittest_wrapper/wrapper_hooks.py` & `gapper-1.3.6/src/gapper/core/unittest_wrapper/wrapper_hooks.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/core/utils.py` & `gapper-1.3.6/src/gapper/core/utils.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/gradescope/datatypes/gradescope_meta.py` & `gapper-1.3.6/src/gapper/gradescope/datatypes/gradescope_meta.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/gradescope/datatypes/gradescope_output.py` & `gapper-1.3.6/src/gapper/gradescope/datatypes/gradescope_output.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/gradescope/main.py` & `gapper-1.3.6/src/gapper/gradescope/main.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/gradescope/resources/requirements.txt` & `gapper-1.3.6/src/gapper/gradescope/resources/requirements.txt`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/gradescope/resources/setup.j2` & `gapper-1.3.6/src/gapper/gradescope/resources/setup.j2`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/src/gapper/gradescope/resources/setup.py` & `gapper-1.3.6/src/gapper/gradescope/resources/setup.py`

 * *Files identical despite different names*

### Comparing `gapper-1.3.5/PKG-INFO` & `gapper-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gapper
-Version: 1.3.5
+Version: 1.3.6
 Summary: Gradescope Autograder Packer
 Home-page: https://github.com/FlickerSoul/gapper
 License: MIT
 Author: Heyuan Zeng
 Author-email: hi@universe.observer
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

