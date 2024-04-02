# Comparing `tmp/scenario-execution-1.0.0.tar.gz` & `tmp/scenario_execution-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenario-execution-1.0.0.tar", last modified: Wed Mar 27 09:29:20 2024, max compression
+gzip compressed data, was "scenario_execution-1.1.0.tar", last modified: Tue Apr  2 09:03:31 2024, max compression
```

## Comparing `scenario-execution-1.0.0.tar` & `scenario_execution-1.1.0.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-03-27 09:29:20.127548 scenario-execution-1.0.0/
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)       45 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/MANIFEST.in
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1457 2024-03-27 09:29:20.127548 scenario-execution-1.0.0/PKG-INFO
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)      585 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/README.md
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)      768 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/package.xml
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1657 2024-03-27 09:27:28.000000 scenario-execution-1.0.0/pyproject.toml
-drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-03-27 09:29:20.123548 scenario-execution-1.0.0/resource/
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)        0 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/resource/scenario_execution_base
-drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-03-27 09:29:20.127548 scenario-execution-1.0.0/scenario_execution.egg-info/
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1457 2024-03-27 09:29:20.000000 scenario-execution-1.0.0/scenario_execution.egg-info/PKG-INFO
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2278 2024-03-27 09:29:20.000000 scenario-execution-1.0.0/scenario_execution.egg-info/SOURCES.txt
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)        1 2024-03-27 09:29:20.000000 scenario-execution-1.0.0/scenario_execution.egg-info/dependency_links.txt
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)      564 2024-03-27 09:29:20.000000 scenario-execution-1.0.0/scenario_execution.egg-info/entry_points.txt
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)      117 2024-03-27 09:29:20.000000 scenario-execution-1.0.0/scenario_execution.egg-info/requires.txt
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)       43 2024-03-27 09:29:20.000000 scenario-execution-1.0.0/scenario_execution.egg-info/top_level.txt
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)        1 2024-03-27 09:20:47.000000 scenario-execution-1.0.0/scenario_execution.egg-info/zip-safe
-drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-03-27 09:29:20.123548 scenario-execution-1.0.0/scenario_execution_base/
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)      938 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/scenario_execution_base/__init__.py
-drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-03-27 09:29:20.123548 scenario-execution-1.0.0/scenario_execution_base/actions/
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)      621 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/scenario_execution_base/actions/__init__.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1490 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/scenario_execution_base/actions/log.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     4359 2024-03-13 11:20:04.000000 scenario-execution-1.0.0/scenario_execution_base/actions/run_process.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)      960 2024-03-26 12:58:00.000000 scenario-execution-1.0.0/scenario_execution_base/get_osc_library.py
-drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-03-27 09:29:20.123548 scenario-execution-1.0.0/scenario_execution_base/lib_osc/
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)      166 2024-03-13 11:20:04.000000 scenario-execution-1.0.0/scenario_execution_base/lib_osc/helpers.osc
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)       57 2024-03-26 09:24:13.000000 scenario-execution-1.0.0/scenario_execution_base/lib_osc/robotics.osc
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)    69428 2024-03-26 08:42:54.000000 scenario-execution-1.0.0/scenario_execution_base/lib_osc/standard.osc
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)    10182 2024-03-26 08:42:54.000000 scenario-execution-1.0.0/scenario_execution_base/lib_osc/standard_base.osc
-drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-03-27 09:29:20.127548 scenario-execution-1.0.0/scenario_execution_base/model/
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)      621 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/scenario_execution_base/model/__init__.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1239 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/scenario_execution_base/model/error.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)    10341 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/scenario_execution_base/model/model_base_visitor.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)    87463 2024-03-26 08:42:54.000000 scenario-execution-1.0.0/scenario_execution_base/model/model_builder.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1869 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/scenario_execution_base/model/model_file_loader.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)    13427 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/scenario_execution_base/model/model_resolver.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)    11333 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/scenario_execution_base/model/model_to_py_tree.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     5512 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/scenario_execution_base/model/osc2_parser.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)    66201 2024-03-13 11:20:04.000000 scenario-execution-1.0.0/scenario_execution_base/model/types.py
-drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-03-27 09:29:20.127548 scenario-execution-1.0.0/scenario_execution_base/osc2_parsing/
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)    41862 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/scenario_execution_base/osc2_parsing/OpenSCENARIO2Lexer.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)    53750 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/scenario_execution_base/osc2_parsing/OpenSCENARIO2Listener.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)   434210 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/scenario_execution_base/osc2_parsing/OpenSCENARIO2Parser.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)    31536 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/scenario_execution_base/osc2_parsing/OpenSCENARIO2Visitor.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)      621 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/scenario_execution_base/osc2_parsing/__init__.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)    15339 2024-03-26 16:20:32.000000 scenario-execution-1.0.0/scenario_execution_base/scenario_execution.py
-drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-03-27 09:29:20.127548 scenario-execution-1.0.0/scenario_execution_base/utils/
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)      621 2024-03-06 10:04:49.000000 scenario-execution-1.0.0/scenario_execution_base/utils/__init__.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2828 2024-03-26 12:58:00.000000 scenario-execution-1.0.0/scenario_execution_base/utils/logging.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)      159 2024-03-27 09:29:20.127548 scenario-execution-1.0.0/setup.cfg
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2170 2024-03-26 16:20:19.000000 scenario-execution-1.0.0/setup.py
-drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-03-27 09:29:20.127548 scenario-execution-1.0.0/test/
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     6527 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_expression.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2630 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_model_ser_deser.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2196 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_osc2_parser_action.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2895 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_osc2_parser_actor.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)    14330 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_osc2_parser_behavior_invocation.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     4774 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_osc2_parser_enum.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2186 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_osc2_parser_event.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1763 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_osc2_parser_keep.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     5396 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_osc2_parser_list.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     9395 2024-03-26 08:42:54.000000 scenario-execution-1.0.0/test/test_osc2_parser_not_supported.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)    19991 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_osc2_parser_parameter.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2232 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_osc2_parser_physical_type.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2908 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_osc2_parser_si.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     6762 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_osc2_parser_struct.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     3167 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_osc2_parser_wait.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1760 2024-03-26 08:42:54.000000 scenario-execution-1.0.0/test/test_osc2_standard_osc.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     4079 2024-03-26 12:58:00.000000 scenario-execution-1.0.0/test/test_run_process.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     3375 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_scenario_events.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     3254 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_scenario_execution.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2293 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_scenario_oneof.py
--rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2257 2024-03-25 11:14:48.000000 scenario-execution-1.0.0/test/test_scenario_parallel.py
+drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-04-02 09:03:31.744897 scenario_execution-1.1.0/
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)       40 2024-03-28 16:15:45.000000 scenario_execution-1.1.0/MANIFEST.in
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1396 2024-04-02 09:03:31.744897 scenario_execution-1.1.0/PKG-INFO
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)      595 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/README.md
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)      754 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/package.xml
+drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-04-02 09:03:31.744897 scenario_execution-1.1.0/resource/
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)        0 2024-03-28 16:15:45.000000 scenario_execution-1.1.0/resource/scenario_execution
+drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-04-02 09:03:31.744897 scenario_execution-1.1.0/scenario_execution/
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)      933 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/__init__.py
+drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-04-02 09:03:31.744897 scenario_execution-1.1.0/scenario_execution/actions/
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)      621 2024-03-28 16:15:45.000000 scenario_execution-1.1.0/scenario_execution/actions/__init__.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1490 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/actions/log.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     4359 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/actions/run_process.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)      940 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/get_osc_library.py
+drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-04-02 09:03:31.744897 scenario_execution-1.1.0/scenario_execution/lib_osc/
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)      166 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/lib_osc/helpers.osc
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)       57 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/lib_osc/robotics.osc
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)    69428 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/lib_osc/standard.osc
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)    10182 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/lib_osc/standard_base.osc
+drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-04-02 09:03:31.744897 scenario_execution-1.1.0/scenario_execution/model/
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)      621 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/model/__init__.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1239 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/model/error.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)    10341 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/model/model_base_visitor.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)    87485 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/model/model_builder.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1793 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/model/model_file_loader.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)    13366 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/model/model_resolver.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)    11287 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/model/model_to_py_tree.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     5243 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/model/osc2_parser.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)    66196 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/model/types.py
+drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-04-02 09:03:31.744897 scenario_execution-1.1.0/scenario_execution/osc2_parsing/
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)    41862 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/osc2_parsing/OpenSCENARIO2Lexer.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)    53750 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/osc2_parsing/OpenSCENARIO2Listener.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)   434210 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/osc2_parsing/OpenSCENARIO2Parser.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)    31536 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/osc2_parsing/OpenSCENARIO2Visitor.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)      621 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/osc2_parsing/__init__.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)    15946 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/scenario_execution_base.py
+drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-04-02 09:03:31.744897 scenario_execution-1.1.0/scenario_execution/utils/
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)      621 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/utils/__init__.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2828 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/scenario_execution/utils/logging.py
+drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-04-02 09:03:31.744897 scenario_execution-1.1.0/scenario_execution.egg-info/
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1396 2024-04-02 09:03:31.000000 scenario_execution-1.1.0/scenario_execution.egg-info/PKG-INFO
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2133 2024-04-02 09:03:31.000000 scenario_execution-1.1.0/scenario_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)        1 2024-04-02 09:03:31.000000 scenario_execution-1.1.0/scenario_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)      534 2024-04-02 09:03:31.000000 scenario_execution-1.1.0/scenario_execution.egg-info/entry_points.txt
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)      124 2024-04-02 09:03:31.000000 scenario_execution-1.1.0/scenario_execution.egg-info/requires.txt
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)       33 2024-04-02 09:03:31.000000 scenario_execution-1.1.0/scenario_execution.egg-info/top_level.txt
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)        1 2024-03-28 16:22:32.000000 scenario_execution-1.1.0/scenario_execution.egg-info/zip-safe
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)      149 2024-04-02 09:03:31.744897 scenario_execution-1.1.0/setup.cfg
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2980 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/setup.py
+drwxr-xr-x   0 fmirus   (12017903) intelall  (2222)        0 2024-04-02 09:03:31.744897 scenario_execution-1.1.0/test/
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     5964 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_expression.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2535 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_model_ser_deser.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1972 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_parser_action.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2645 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_parser_actor.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)    13184 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_parser_behavior_invocation.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     4286 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_parser_enum.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1962 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_parser_event.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1673 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_parser_keep.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     4821 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_parser_list.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     8065 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_parser_not_supported.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)    17579 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_parser_parameter.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2083 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_parser_physical_type.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2625 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_parser_si.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     6452 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_parser_struct.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2758 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_parser_wait.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     1590 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_osc2_standard_osc.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     3795 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_run_process.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     3115 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_scenario_events.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     3859 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_scenario_execution.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2182 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_scenario_oneof.py
+-rw-r--r--   0 fmirus   (12017903) intelall  (2222)     2141 2024-04-02 09:02:45.000000 scenario_execution-1.1.0/test/test_scenario_parallel.py
```

### Comparing `scenario-execution-1.0.0/PKG-INFO` & `scenario_execution-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
-Name: scenario-execution
-Version: 1.0.0
-Summary: Robotics Scenario Execution
-Author-email: Intel Labs <scenario-execution@intel.com>
+Name: scenario_execution
+Version: 1.1.0
+Summary: Scenario Execution for Robotics
+Home-page: https://github.com/IntelLabs/scenario_execution
 Maintainer: Intel Labs
-Maintainer-email: Intel Labs <scenario-execution@intel.com>
+Maintainer-email: scenario-execution@intel.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/IntelLabs/scenario_execution
-Project-URL: Documentation, https://intellabs.github.io/scenario_execution/
+Project-URL: Documentation, https://github.com/IntelLabs/scenario_execution
 Project-URL: Issues, https://github.com/IntelLabs/scenario_execution/issues
-Keywords: robotics,scenarios,experiments,testing
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: antlr4-python3-runtime==4.7.2
 Requires-Dist: transforms3d==0.3.1
 Requires-Dist: pexpect==4.9.0
 Requires-Dist: defusedxml==0.7.1
-Requires-Dist: pyyaml
+Requires-Dist: pyyaml==6.0.1
 Requires-Dist: py-trees==2.1.6
 
-# Scenario Execution Base Package
+# Scenario Execution
 
-The `scenario_execution_base` package is the base package for scenario execution. It provides functionalities like parsing, py-trees creation and execution.
+The `scenario_execution` package is the core package of Scenario Execution for Robotics. It provides functionalities such as parsing, py-trees creation and execution.
 
-It provides the following scenario execution libraries:
+Furthermore, it provides the following scenario execution libraries:
 
 - `standard.osc`: The OpenSCENARIO 2 standard library. It is slightly modified to be in sync with the feature set of scenario execution. For convenience, numerical struct members are initialized with 0.
 - `robotics.osc`: robotic-specific specifications
 - `helper.osc`: helper actions
 - `networking.osc`: actions related to networking
```

### Comparing `scenario-execution-1.0.0/README.md` & `scenario_execution-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Scenario Execution Base Package
+# Scenario Execution
 
-The `scenario_execution_base` package is the base package for scenario execution. It provides functionalities like parsing, py-trees creation and execution.
+The `scenario_execution` package is the core package of Scenario Execution for Robotics. It provides functionalities such as parsing, py-trees creation and execution.
 
-It provides the following scenario execution libraries:
+Furthermore, it provides the following scenario execution libraries:
 
 - `standard.osc`: The OpenSCENARIO 2 standard library. It is slightly modified to be in sync with the feature set of scenario execution. For convenience, numerical struct members are initialized with 0.
 - `robotics.osc`: robotic-specific specifications
 - `helper.osc`: helper actions
 - `networking.osc`: actions related to networking
```

### Comparing `scenario-execution-1.0.0/package.xml` & `scenario_execution-1.1.0/package.xml`

 * *Files 14% similar despite different names*

#### Comparing `scenario-execution-1.0.0/package.xml` & `scenario_execution-1.1.0/package.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <?xml-model href="http://download.ros.org/schema/package_format3.xsd" schematypens="http://www.w3.org/2001/XMLSchema"?>
 <package format="3">
-  <name>scenario_execution_base</name>
-  <version>1.0.0</version>
-  <description>Robotics Scenario Execution</description>
+  <name>scenario_execution</name>
+  <version>1.1.0</version>
+  <description>Scenario Execution</description>
   <author email="scenario-execution@intel.com">Intel Labs</author>
   <maintainer email="scenario-execution@intel.com">Intel Labs</maintainer>
   <license file="../LICENSE">Apache-2.0</license>
   <exec_depend>py_trees</exec_depend>
   <test_depend>ament_copyright</test_depend>
   <test_depend>ament_flake8</test_depend>
   <test_depend>ament_pep257</test_depend>
```

### Comparing `scenario-execution-1.0.0/scenario_execution.egg-info/PKG-INFO` & `scenario_execution-1.1.0/scenario_execution.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
-Name: scenario-execution
-Version: 1.0.0
-Summary: Robotics Scenario Execution
-Author-email: Intel Labs <scenario-execution@intel.com>
+Name: scenario_execution
+Version: 1.1.0
+Summary: Scenario Execution for Robotics
+Home-page: https://github.com/IntelLabs/scenario_execution
 Maintainer: Intel Labs
-Maintainer-email: Intel Labs <scenario-execution@intel.com>
+Maintainer-email: scenario-execution@intel.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/IntelLabs/scenario_execution
-Project-URL: Documentation, https://intellabs.github.io/scenario_execution/
+Project-URL: Documentation, https://github.com/IntelLabs/scenario_execution
 Project-URL: Issues, https://github.com/IntelLabs/scenario_execution/issues
-Keywords: robotics,scenarios,experiments,testing
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: antlr4-python3-runtime==4.7.2
 Requires-Dist: transforms3d==0.3.1
 Requires-Dist: pexpect==4.9.0
 Requires-Dist: defusedxml==0.7.1
-Requires-Dist: pyyaml
+Requires-Dist: pyyaml==6.0.1
 Requires-Dist: py-trees==2.1.6
 
-# Scenario Execution Base Package
+# Scenario Execution
 
-The `scenario_execution_base` package is the base package for scenario execution. It provides functionalities like parsing, py-trees creation and execution.
+The `scenario_execution` package is the core package of Scenario Execution for Robotics. It provides functionalities such as parsing, py-trees creation and execution.
 
-It provides the following scenario execution libraries:
+Furthermore, it provides the following scenario execution libraries:
 
 - `standard.osc`: The OpenSCENARIO 2 standard library. It is slightly modified to be in sync with the feature set of scenario execution. For convenience, numerical struct members are initialized with 0.
 - `robotics.osc`: robotic-specific specifications
 - `helper.osc`: helper actions
 - `networking.osc`: actions related to networking
```

### Comparing `scenario-execution-1.0.0/scenario_execution.egg-info/SOURCES.txt` & `scenario_execution-1.1.0/scenario_execution.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 MANIFEST.in
 README.md
 package.xml
-pyproject.toml
 setup.cfg
 setup.py
-resource/scenario_execution_base
+resource/scenario_execution
+scenario_execution/__init__.py
+scenario_execution/get_osc_library.py
+scenario_execution/scenario_execution_base.py
 scenario_execution.egg-info/PKG-INFO
 scenario_execution.egg-info/SOURCES.txt
 scenario_execution.egg-info/dependency_links.txt
 scenario_execution.egg-info/entry_points.txt
 scenario_execution.egg-info/requires.txt
 scenario_execution.egg-info/top_level.txt
 scenario_execution.egg-info/zip-safe
-scenario_execution_base/__init__.py
-scenario_execution_base/get_osc_library.py
-scenario_execution_base/scenario_execution.py
-scenario_execution_base/actions/__init__.py
-scenario_execution_base/actions/log.py
-scenario_execution_base/actions/run_process.py
-scenario_execution_base/lib_osc/helpers.osc
-scenario_execution_base/lib_osc/robotics.osc
-scenario_execution_base/lib_osc/standard.osc
-scenario_execution_base/lib_osc/standard_base.osc
-scenario_execution_base/model/__init__.py
-scenario_execution_base/model/error.py
-scenario_execution_base/model/model_base_visitor.py
-scenario_execution_base/model/model_builder.py
-scenario_execution_base/model/model_file_loader.py
-scenario_execution_base/model/model_resolver.py
-scenario_execution_base/model/model_to_py_tree.py
-scenario_execution_base/model/osc2_parser.py
-scenario_execution_base/model/types.py
-scenario_execution_base/osc2_parsing/OpenSCENARIO2Lexer.py
-scenario_execution_base/osc2_parsing/OpenSCENARIO2Listener.py
-scenario_execution_base/osc2_parsing/OpenSCENARIO2Parser.py
-scenario_execution_base/osc2_parsing/OpenSCENARIO2Visitor.py
-scenario_execution_base/osc2_parsing/__init__.py
-scenario_execution_base/utils/__init__.py
-scenario_execution_base/utils/logging.py
+scenario_execution/actions/__init__.py
+scenario_execution/actions/log.py
+scenario_execution/actions/run_process.py
+scenario_execution/lib_osc/helpers.osc
+scenario_execution/lib_osc/robotics.osc
+scenario_execution/lib_osc/standard.osc
+scenario_execution/lib_osc/standard_base.osc
+scenario_execution/model/__init__.py
+scenario_execution/model/error.py
+scenario_execution/model/model_base_visitor.py
+scenario_execution/model/model_builder.py
+scenario_execution/model/model_file_loader.py
+scenario_execution/model/model_resolver.py
+scenario_execution/model/model_to_py_tree.py
+scenario_execution/model/osc2_parser.py
+scenario_execution/model/types.py
+scenario_execution/osc2_parsing/OpenSCENARIO2Lexer.py
+scenario_execution/osc2_parsing/OpenSCENARIO2Listener.py
+scenario_execution/osc2_parsing/OpenSCENARIO2Parser.py
+scenario_execution/osc2_parsing/OpenSCENARIO2Visitor.py
+scenario_execution/osc2_parsing/__init__.py
+scenario_execution/utils/__init__.py
+scenario_execution/utils/logging.py
 test/test_expression.py
 test/test_model_ser_deser.py
 test/test_osc2_parser_action.py
 test/test_osc2_parser_actor.py
 test/test_osc2_parser_behavior_invocation.py
 test/test_osc2_parser_enum.py
 test/test_osc2_parser_event.py
```

### Comparing `scenario-execution-1.0.0/scenario_execution_base/__init__.py` & `scenario_execution-1.1.0/scenario_execution/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 from . import actions
 from . import utils
 from . import model
-from scenario_execution_base.scenario_execution import ScenarioExecution
-from scenario_execution_base.utils.logging import BaseLogger, Logger
+from scenario_execution.scenario_execution_base import ScenarioExecution
+from scenario_execution.utils.logging import BaseLogger, Logger
 
 __all__ = [
     'actions',
     'utils',
     'model',
     'BaseLogger',
     "Logger",
```

### Comparing `scenario-execution-1.0.0/scenario_execution_base/actions/__init__.py` & `scenario_execution-1.1.0/scenario_execution/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/actions/log.py` & `scenario_execution-1.1.0/scenario_execution/actions/log.py`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/actions/run_process.py` & `scenario_execution-1.1.0/scenario_execution/actions/run_process.py`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/get_osc_library.py` & `scenario_execution-1.1.0/scenario_execution/get_osc_library.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 def get_robotics_library():
-    return 'scenario_execution_base', 'robotics.osc'
+    return 'scenario_execution', 'robotics.osc'
 
 
 def get_helpers_library():
-    return 'scenario_execution_base', 'helpers.osc'
+    return 'scenario_execution', 'helpers.osc'
 
 
 def get_standard_library():
-    return 'scenario_execution_base', 'standard.osc'
+    return 'scenario_execution', 'standard.osc'
 
 
 def get_standard_base_library():
-    return 'scenario_execution_base', 'standard_base.osc'
+    return 'scenario_execution', 'standard_base.osc'
```

### Comparing `scenario-execution-1.0.0/scenario_execution_base/lib_osc/standard.osc` & `scenario_execution-1.1.0/scenario_execution/lib_osc/standard.osc`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/lib_osc/standard_base.osc` & `scenario_execution-1.1.0/scenario_execution/lib_osc/standard_base.osc`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/model/__init__.py` & `scenario_execution-1.1.0/scenario_execution/model/__init__.py`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/model/error.py` & `scenario_execution-1.1.0/scenario_execution/model/error.py`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/model/model_base_visitor.py` & `scenario_execution-1.1.0/scenario_execution/model/model_base_visitor.py`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/model/model_builder.py` & `scenario_execution-1.1.0/scenario_execution/model/model_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from .types import CompilationUnit, PhysicalTypeDeclaration, UnitDeclaration, EnumDeclaration, EnumMemberDeclaration, EnumValueReference, StructDeclaration, StructInherits, ActionDeclaration, ActionInherits, ActorDeclaration, ActorInherits, FieldAccessExpression,  FloatLiteral, FunctionApplicationExpression, Argument, BehaviorInvocation, BinaryExpression, BoolLiteral, DoDirective, ElapsedExpression, DoMember, EmitDirective,  EventCondition, EventDeclaration, EventFieldDecl, EventReference,  GlobalParameterDeclaration, Identifier, IdentifierReference, IntegerLiteral, KeepConstraintDeclaration,  LogicalExpression, MethodBody,    NamedArgument, OnDirective, ParameterDeclaration, PhysicalLiteral, ParameterReference, PositionalArgument,  RelationExpression,     ScenarioInherits, SIUnitSpecifier, StringLiteral, ScenarioDeclaration, StructuredTypeExtension,  Type, VariableDeclaration, WaitDirective, ListExpression
 
 
 from ..osc2_parsing.OpenSCENARIO2Parser import OpenSCENARIO2Parser
 from ..osc2_parsing.OpenSCENARIO2Listener import OpenSCENARIO2Listener
 
-from scenario_execution_base.model.error import OSC2ParsingError
+from scenario_execution.model.error import OSC2ParsingError
 import ast
 
 from antlr4.tree.Tree import ParseTreeWalker
 import os
 from pkg_resources import iter_entry_points, resource_filename
 
 
@@ -115,18 +115,18 @@
 
             lib_class = libraries_found[0].load()
             resource, filename = lib_class()
 
             lib_osc_dir = resource_filename(resource, 'lib_osc')
             file = os.path.join(lib_osc_dir, filename)
 
-        imported_tree, errors = self.parse_file(file, self.log_model, f"{file} :")
-
-        if errors:
-            raise OSC2ParsingError(msg=f'{errors} parsing errors found in import {file}.', context=ctx)
+        try:
+            imported_tree = self.parse_file(file, self.log_model, f"{file} :")
+        except Exception as e:  # pylint: disable=broad-except
+            raise ValueError(f'Error while parsing import {file}: {e}') from e
 
         if imported_tree is not None:
             walker = ParseTreeWalker()
             prev_file = self.current_file
             self.current_file = file
             walker.walk(self, imported_tree)
             self.current_file = prev_file
```

### Comparing `scenario-execution-1.0.0/scenario_execution_base/model/model_file_loader.py` & `scenario_execution-1.1.0/scenario_execution/model/model_file_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,33 +12,28 @@
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 
 import yaml
-from scenario_execution_base.model.types import print_tree, deserialize
-from scenario_execution_base.model.model_to_py_tree import create_py_tree
-from scenario_execution_base.model.model_resolver import resolve_internal_model
+from scenario_execution.model.types import print_tree, deserialize
+from scenario_execution.model.model_to_py_tree import create_py_tree
+from scenario_execution.model.model_resolver import resolve_internal_model
 
 
 class ModelFileLoader(object):
 
     def __init__(self, logger) -> None:
         self.logger = logger
 
     def process_file(self, file_name, log_tree: bool = False, debug: bool = False):
         model = self.load_file(file_name, log_tree)
-
-        success = resolve_internal_model(model, self.logger, log_tree)
-        if not success:
-            return None
-
+        resolve_internal_model(model, self.logger, log_tree)
         scenarios = create_py_tree(model, self.logger, log_tree)
-
         return scenarios
 
     def load_file(self, file_name, log_tree):
         try:
             with open(file_name, 'rb') as input_file:
                 serialize_data = yaml.safe_load(input_file)  # nosec B301 TODO
                 model = deserialize(serialize_data)
```

### Comparing `scenario-execution-1.0.0/scenario_execution_base/model/model_resolver.py` & `scenario_execution-1.1.0/scenario_execution/model/model_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,37 +10,33 @@
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
-from scenario_execution_base.model.types import ActionDeclaration, ActionInherits, EnumDeclaration, EnumValueReference, KeepConstraintDeclaration, EmitDirective, Type
+from scenario_execution.model.types import ActionDeclaration, ActionInherits, EnumDeclaration, EnumValueReference, KeepConstraintDeclaration, EmitDirective, Type
 
 from .types import UnitDeclaration, EnumValueReference, StructInherits, ActionDeclaration, ActionInherits, ActorInherits, FieldAccessExpression,  BehaviorInvocation, EmitDirective, GlobalParameterDeclaration, IdentifierReference, Parameter, ModelElement, StructuredDeclaration, KeepConstraintDeclaration, NamedArgument, ParameterDeclaration, PhysicalLiteral,  PositionalArgument,  RelationExpression, ScenarioInherits, SIUnitSpecifier,  Type, EnumMemberDeclaration, ListExpression, print_tree
 
 from .model_base_visitor import ModelBaseVisitor
-from scenario_execution_base.model.error import OSC2ParsingError
+from scenario_execution.model.error import OSC2ParsingError
 
 
 def resolve_internal_model(model, logger, log_tree):
     osc2scenario_resolver = ModelResolver(logger)
     try:
         osc2scenario_resolver.visit(model)
     except OSC2ParsingError as e:
-        logger.error(
-            f'Error while creating tree:\nTraceback <line: {e.line}, column: {e.column}> in "{e.filename}":\n  -> {e.context}\n'
-            f'{e.__class__.__name__}: {e.msg}'
-        )
-        return False
+        raise ValueError(
+            f'Error while creating tree:\nTraceback <line: {e.line}, column: {e.column}> in "{e.filename}":\n  -> {e.context}\n{e.__class__.__name__}: {e.msg}') from e
 
     if log_tree:
         logger.info("----Internal model (resolved)-----")
         print_tree(model, logger)
-    return True
 
 
 class ModelResolver(ModelBaseVisitor):
 
     def __init__(self, logger) -> None:
         super().__init__()
         self.logger = logger
```

### Comparing `scenario-execution-1.0.0/scenario_execution_base/model/model_to_py_tree.py` & `scenario_execution-1.1.0/scenario_execution/model/model_to_py_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,30 +16,27 @@
 
 import py_trees
 from py_trees.common import Access, Status
 from pkg_resources import iter_entry_points
 
 import inspect
 
-from scenario_execution_base.model.types import EventReference, ScenarioDeclaration, DoMember, WaitDirective, EmitDirective, BehaviorInvocation, EventCondition, EventDeclaration, RelationExpression, LogicalExpression, ElapsedExpression, PhysicalLiteral
-from scenario_execution_base.model.model_base_visitor import ModelBaseVisitor
-from scenario_execution_base.model.error import OSC2ParsingError
+from scenario_execution.model.types import EventReference, ScenarioDeclaration, DoMember, WaitDirective, EmitDirective, BehaviorInvocation, EventCondition, EventDeclaration, RelationExpression, LogicalExpression, ElapsedExpression, PhysicalLiteral
+from scenario_execution.model.model_base_visitor import ModelBaseVisitor
+from scenario_execution.model.error import OSC2ParsingError
 
 
 def create_py_tree(model, logger, log_tree):
     model_to_py_tree = ModelToPyTree(logger)
     behavior_trees = None
     try:
         behavior_trees = model_to_py_tree.build(model, log_tree)
     except OSC2ParsingError as e:
-        logger.error(
-            f'Error while creating tree:\nTraceback <line: {e.line}, column: {e.column}> in "{e.filename}":\n  -> {e.context}\n'
-            f'{e.__class__.__name__}: {e.msg}'
-        )
-        return None
+        raise ValueError(
+            f'Error while creating py-tree:\nTraceback <line: {e.line}, column: {e.column}> in "{e.filename}":\n  -> {e.context}\n{e.__class__.__name__}: {e.msg}') from e
     return behavior_trees
 
 
 class TopicEquals(py_trees.behaviour.Behaviour):
     """
     Class to listen to a topic in Blackboard and check if it equals the defined message
```

### Comparing `scenario-execution-1.0.0/scenario_execution_base/model/osc2_parser.py` & `scenario_execution-1.1.0/scenario_execution/model/osc2_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,124 +10,107 @@
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import sys
 import re
 
 from antlr4 import FileStream, CommonTokenStream
 from antlr4.error.ErrorListener import ErrorListener
 from antlr4.tree.Tree import TerminalNodeImpl, ParseTreeWalker
-from scenario_execution_base.osc2_parsing.OpenSCENARIO2Parser import OpenSCENARIO2Parser
-from scenario_execution_base.osc2_parsing.OpenSCENARIO2Lexer import OpenSCENARIO2Lexer
-from scenario_execution_base.model.error import OSC2ParsingError
-from scenario_execution_base.model.model_builder import ModelBuilder
-from scenario_execution_base.model.types import print_tree
-from scenario_execution_base.model.model_to_py_tree import create_py_tree
-from scenario_execution_base.model.model_resolver import resolve_internal_model
+from scenario_execution.osc2_parsing.OpenSCENARIO2Parser import OpenSCENARIO2Parser
+from scenario_execution.osc2_parsing.OpenSCENARIO2Lexer import OpenSCENARIO2Lexer
+from scenario_execution.model.error import OSC2ParsingError
+from scenario_execution.model.model_builder import ModelBuilder
+from scenario_execution.model.types import print_tree
+from scenario_execution.model.model_to_py_tree import create_py_tree
+from scenario_execution.model.model_resolver import resolve_internal_model
 
 
 class OpenScenario2Parser(object):
     """ Helper class for parsing openscenario 2 files """
 
     def __init__(self, logger) -> None:
         self.logger = logger
         self.parsed_files = []
 
     def process_file(self, file, log_model: bool = False, debug: bool = False):
         """ Convenience method to execute the parsing and print out tree """
 
-        parsed_tree, errors = self.parse_file(file, log_model)
-        if errors:
-            return None
+        parsed_tree = self.parse_file(file, log_model)
 
-        try:
-            model = self.create_internal_model(parsed_tree, file, log_model, debug)
-        except Exception:  # pylint: disable=broad-except
-            return None
-        if model is None:
-            return None
+        model = self.create_internal_model(parsed_tree, file, log_model, debug)
 
         scenarios = create_py_tree(model, self.logger, log_model)
 
         return scenarios
 
     def load_internal_model(self, tree, file_name: str, log_model: bool = False, debug: bool = False):
         model_builder = ModelBuilder(self.logger, self.parse_file, file_name, log_model)
         walker = ParseTreeWalker()
 
         model = None
         try:
             walker.walk(model_builder, tree)
             model = model_builder.get_model()
         except OSC2ParsingError as e:
-            self.logger.error(
-                f'Error creating internal model: Traceback <line: {e.line}, column: {e.column}> in "{e.filename}":\n  -> {e.context}\n'
-                f'{e.__class__.__name__}: {e.msg}'
-            )
-            if debug:
-                self.logger.info(str(e))
-            return None
+            raise ValueError(
+                f'Error creating internal model: Traceback <line: {e.line}, column: {e.column}> in "{e.filename}":\n  -> {e.context}\n{e.__class__.__name__}: {e.msg}') from e
         if log_model:
             self.logger.info("----Internal model-----")
             print_tree(model, self.logger)
         return model
 
     def create_internal_model(self, tree, file_name: str, log_model: bool = False, debug: bool = False):
         model = self.load_internal_model(tree, file_name, log_model, debug)
-        if model is None:
-            return None
-
-        ret = resolve_internal_model(model, self.logger, log_model)
-        if ret:
-            return model
-
-        return None
+        resolve_internal_model(model, self.logger, log_model)
+        return model
 
     def parse_file(self, file: str, log_model: bool = False, error_prefix=""):
         """ Execute the parsing """
         if file in self.parsed_files:  # skip already parsed/imported files
-            return None, 0
+            return None
         self.parsed_files.append(file)
         try:
             input_stream = FileStream(file)
         except (OSError, UnicodeDecodeError) as e:
-            self.logger.error(f'{e}')
-            sys.exit(1)
+            raise ValueError(f'{e}') from e
         return self.parse_input_stream(input_stream, log_model, error_prefix)
 
     def parse_input_stream(self, input_stream, log_model=False, error_prefix=""):
         """ Execute the parsing """
         lexer = OpenSCENARIO2Lexer(input_stream)
         stream = CommonTokenStream(lexer)
 
         parser = OpenSCENARIO2Parser(stream)
         # if quiet:
         parser.removeErrorListeners()
 
         class TestErrorListener(ErrorListener):
             def __init__(self, prefix: str) -> None:
                 self.prefix = prefix
+                self.error_message = ""
                 super().__init__()
 
             def syntaxError(self, recognizer, offendingSymbol, line, column, msg, e):  # pylint: disable=invalid-name
-                print(self.prefix + "line " + str(line) + ":" +
-                      str(column) + " " + msg, file=sys.stderr)
-
-        parser.addErrorListener(TestErrorListener(error_prefix))
+                if self.error_message:
+                    self.error_message += "\n"
+                self.error_message += self.prefix + "line " + str(line) + ":" + str(column) + " " + msg
+        error_listener = TestErrorListener(error_prefix)
+        parser.addErrorListener(error_listener)
         tree = parser.osc_file()
         errors = parser.getNumberOfSyntaxErrors()  # pylint: disable=no-member
         if log_model:
             self.print_parsed_osc_tree(tree, self.logger, parser.ruleNames)
-
+        if errors:
+            raise ValueError(error_listener.error_message)
         del parser
-        return tree, errors
+        return tree
 
     @staticmethod
     def print_parsed_osc_tree(tree, logger, rule_names, indent=0):
         """ Print the parsed tree for debugging purposes """
         if isinstance(tree, TerminalNodeImpl):
             if not re.match(r"\r?\n[ \t]*", tree.getText()):
                 logger.info("{0}TOKEN '{1}'".format("  " * indent, tree.getText()))
```

### Comparing `scenario-execution-1.0.0/scenario_execution_base/model/types.py` & `scenario_execution-1.1.0/scenario_execution/model/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 from typing import List
-from scenario_execution_base.model.error import OSC2ParsingError
+from scenario_execution.model.error import OSC2ParsingError
 import sys
 
 
 def print_tree(elem, logger, whitespace=""):
 
     children = ""
     for child in elem.get_children():
```

### Comparing `scenario-execution-1.0.0/scenario_execution_base/osc2_parsing/OpenSCENARIO2Lexer.py` & `scenario_execution-1.1.0/scenario_execution/osc2_parsing/OpenSCENARIO2Lexer.py`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/osc2_parsing/OpenSCENARIO2Listener.py` & `scenario_execution-1.1.0/scenario_execution/osc2_parsing/OpenSCENARIO2Listener.py`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/osc2_parsing/OpenSCENARIO2Parser.py` & `scenario_execution-1.1.0/scenario_execution/osc2_parsing/OpenSCENARIO2Parser.py`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/osc2_parsing/OpenSCENARIO2Visitor.py` & `scenario_execution-1.1.0/scenario_execution/osc2_parsing/OpenSCENARIO2Visitor.py`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/osc2_parsing/__init__.py` & `scenario_execution-1.1.0/scenario_execution/osc2_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/scenario_execution.py` & `scenario_execution-1.1.0/scenario_execution/scenario_execution_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import os
 import sys
 import time
 import argparse
 import signal
 from datetime import datetime, timedelta
 import py_trees
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
-from scenario_execution_base.model.model_file_loader import ModelFileLoader
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import Logger
+from scenario_execution.model.model_file_loader import ModelFileLoader
 from dataclasses import dataclass
 
 
 @dataclass
 class ScenarioResult:
     name: str
     result: bool
@@ -111,59 +111,54 @@
         This method could be overriden by child classes and defined according to the middleware.
 
         return:
             A logger which has three logging levels: info, warning, error
         """
         return Logger('scenario_execution', debug)
 
-    def setup(self, tree: py_trees.behaviour.Behaviour, **kwargs) -> bool:
+    def setup(self, scenario: py_trees.behaviour.Behaviour, **kwargs) -> bool:
         """
         Setup each scenario before ticking
 
         Args:
             tree [py_trees.behavior.Behavior]: root of the tree
 
         return:
             True if the scenario is setup without errors
         """
+        self.logger.info(f"Executing scenario '{scenario.name}'")
         self.shutdown_requested = False
-        self.blackboard = tree.attach_blackboard_client(
+        self.current_scenario = scenario
+        self.current_scenario_start = datetime.now()
+        self.blackboard = scenario.attach_blackboard_client(
             name="MainBlackboardClient",
-            namespace=tree.name
+            namespace=scenario.name
         )
 
         self.blackboard.register_key("end", access=py_trees.common.Access.READ)
         self.blackboard.register_key("fail", access=py_trees.common.Access.READ)
 
         # Initialize end and fail events
         self.blackboard.register_key("end", access=py_trees.common.Access.WRITE)
         self.blackboard.register_key("fail", access=py_trees.common.Access.WRITE)
         self.blackboard.end = False
         self.blackboard.fail = False
-        self.behaviour_tree = self.setup_behaviour_tree(tree)  # Get the behaviour_tree
+        self.behaviour_tree = self.setup_behaviour_tree(scenario)  # Get the behaviour_tree
         self.behaviour_tree.add_pre_tick_handler(self.pre_tick_handler)
         self.behaviour_tree.add_post_tick_handler(self.post_tick_handler)
         self.last_snapshot_visitor = LastSnapshotVisitor()
         self.behaviour_tree.add_visitor(self.last_snapshot_visitor)
         if self.debug:
             self.behaviour_tree.add_visitor(py_trees.visitors.DebugVisitor())
         if self.live_tree:
             self.behaviour_tree.add_visitor(
                 py_trees.visitors.DisplaySnapshotVisitor(
                     display_blackboard=True
                 ))
-        try:
-            self.behaviour_tree.setup(timeout=self.setup_timeout, logger=self.logger, output_dir=self.output_dir, **kwargs)
-            return True
-        except RuntimeError as e:
-            self.logger.error(f'Runtime Error "{e}". Aborting... ')
-            return False
-        except Exception as e:  # pylint: disable=broad-except
-            self.logger.error(f"Error while setting up tree: {e}")
-            return False
+        self.behaviour_tree.setup(timeout=self.setup_timeout, logger=self.logger, output_dir=self.output_dir, **kwargs)
 
     def setup_behaviour_tree(self, tree):
         """
         Setup the behaviour tree.
 
         For other middleware, a subclass of behaviour_tree might be needed for additional support.
         Override this to adapt to other middleware.
@@ -172,82 +167,90 @@
             tree [py_trees.behaviour.Behaviour]: root of the behaviour tree
 
         return:
             py_trees.trees.BehaviourTree
         """
         return py_trees.trees.BehaviourTree(tree)
 
-    def parse(self):
+    def parse(self):  # pylint: disable=too-many-return-statements
         """
         Parse the OpenScenario2 file
 
         return:
             True if no errors occured during parsing
         """
         if self.scenario_file is None:
             self.logger.error(f"No scenario file given.")
             return False
+        start = datetime.now()
         file_extension = os.path.splitext(self.scenario_file)[1]
         if file_extension == '.osc':
             parser = OpenScenario2Parser(self.logger)
         elif file_extension == '.sce':
             parser = ModelFileLoader(self.logger)
         else:
-            self.logger.error(f"File '{self.scenario_file}' has unknown extension '{file_extension}'. Allowed [.osc, .sce]")
+            self.add_result(ScenarioResult(name=f'Parsing of {self.scenario_file}',
+                                           result=False,
+                                           failure_message="parsing failed",
+                                           failure_output=f"File has unknown extension '{file_extension}'. Allowed [.osc, .sce]",
+                                           processing_time=datetime.now() - start))
             return False
 
-        start = datetime.now()
         if not os.path.isfile(self.scenario_file):
             self.add_result(ScenarioResult(name=f'Parsing of {self.scenario_file}',
                                            result=False,
                                            failure_message="parsing failed",
                                            failure_output="File does not exist",
                                            processing_time=datetime.now() - start))
             return False
-        self.scenarios = parser.process_file(self.scenario_file, self.log_model, self.debug)
-        if self.scenarios is None:
+        try:
+            self.scenarios = parser.process_file(self.scenario_file, self.log_model, self.debug)
+        except Exception as e:  # pylint: disable=broad-except
             self.add_result(ScenarioResult(name=f'Parsing of {self.scenario_file}',
                                            result=False,
                                            failure_message="parsing failed",
-                                           failure_output="No scenario defined",
+                                           failure_output=str(e),
                                            processing_time=datetime.now() - start))
             return False
         if len(self.scenarios) == 0:
             self.add_result(ScenarioResult(name=f'Parsing of {self.scenario_file}',
                                            result=False,
                                            failure_message="parsing failed",
                                            failure_output="no scenario defined",
                                            processing_time=datetime.now() - start))
+            return False
         if len(self.scenarios) != 1:
             self.add_result(ScenarioResult(name=f'Parsing of {self.scenario_file}',
                                            result=False,
                                            failure_message="parsing failed",
                                            failure_output=f"more than one ({len(self.scenarios)}) scenario defined",
                                            processing_time=datetime.now() - start))
+            return False
 
-        return self.scenarios is not None and len(self.scenarios) == 1
+        return True
 
     def run(self):
         if len(self.scenarios) != 1:
             self.logger.error(f"Only one scenario per file is supported.")
-            return False
-        self.current_scenario = self.scenarios[0]
-        self.current_scenario_start = datetime.now()
-        result = self.setup(self.current_scenario)
-        if result:
-            while not self.shutdown_requested:
-                try:
-                    self.behaviour_tree.tick()
-                    time.sleep(self.tick_tock_period)
-                    if self.live_tree:
-                        self.logger.debug(py_trees.display.unicode_tree(
-                            root=self.behaviour_tree.root, show_status=True))
-                except KeyboardInterrupt:
-                    self.on_scenario_shutdown(False, "Aborted")
-        return self.process_results()
+            return
+        try:
+            self.setup(self.scenarios[0])
+        except Exception as e:  # pylint: disable=broad-except
+            self.on_scenario_shutdown(False, "Setup failed", f"{e}")
+            return
+
+        while not self.shutdown_requested:
+            try:
+                self.behaviour_tree.tick()
+                time.sleep(self.tick_tock_period)
+                if self.live_tree:
+                    self.logger.debug(py_trees.display.unicode_tree(
+                        root=self.behaviour_tree.root, show_status=True))
+            except KeyboardInterrupt:
+                self.on_scenario_shutdown(False, "Aborted")
 
     def add_result(self, result: ScenarioResult):
         if result.result is False:
             self.logger.error(f"{result.name}: {result.failure_message} {result.failure_output}")
         self.results.append(result)
 
     def process_results(self):
@@ -302,33 +305,39 @@
         if self.blackboard.fail or self.blackboard.end:
             result = True
             if self.blackboard.fail:
                 result = False
             if not self.shutdown_requested:
                 self.on_scenario_shutdown(result)
 
-    def on_scenario_shutdown(self, result, failure_message=""):
+    def on_scenario_shutdown(self, result, failure_message="", failure_output=""):
         self.shutdown_requested = True
         if self.behaviour_tree:
             self.behaviour_tree.interrupt()
-        failure_output = ""
         if self.current_scenario:
             if result:
                 self.logger.info(f"Scenario '{self.current_scenario.name}' succeeded.")
             else:
                 if not failure_message:
                     failure_message = "execution failed."
-                failure_output = self.last_snapshot_visitor.last_snapshot
+                if failure_output and self.last_snapshot_visitor.last_snapshot:
+                    failure_output += "\n\n"
+                failure_output += self.last_snapshot_visitor.last_snapshot
                 if self.log_model:
                     self.logger.error(self.last_snapshot_visitor.last_snapshot)
             self.add_result(ScenarioResult(name=self.current_scenario.name,
                                            result=result,
                                            failure_message=failure_message,
                                            failure_output=failure_output,
                                            processing_time=datetime.now()-self.current_scenario_start))
+        else:
+            self.add_result(ScenarioResult(name="",
+                                           result=result,
+                                           failure_message=failure_message,
+                                           failure_output=failure_output))
 
     @staticmethod
     def parse_args(args):
         parser = argparse.ArgumentParser()
         parser.add_argument('-d', '--debug', action='store_true', help='debugging output')
         parser.add_argument('-l', '--log-model', action='store_true',
                             help='Produce tree output of parsed openscenario2 content')
@@ -353,15 +362,16 @@
                                                scenario_file=args.scenario,
                                                output_dir=args.output_dir)
     except ValueError as e:
         print(f"Error while initializing: {e}")
         sys.exit(1)
     result = scenario_execution.parse()
     if result and not args.dry_run:
-        result = scenario_execution.run()
+        scenario_execution.run()
+    result = scenario_execution.process_results()
     if result:
         sys.exit(0)
     else:
         sys.exit(1)
 
 
 if __name__ == '__main__':
```

### Comparing `scenario-execution-1.0.0/scenario_execution_base/utils/__init__.py` & `scenario_execution-1.1.0/scenario_execution/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/scenario_execution_base/utils/logging.py` & `scenario_execution-1.1.0/scenario_execution/utils/logging.py`

 * *Files identical despite different names*

### Comparing `scenario-execution-1.0.0/setup.py` & `scenario_execution-1.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,47 +11,71 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """Setup python package"""
+from pathlib import Path
 from glob import glob
 import os
 from setuptools import find_namespace_packages, setup
 
-PACKAGE_NAME = 'scenario_execution_base'
+PACKAGE_NAME = 'scenario_execution'
+
+# read the contents of the README file
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name=PACKAGE_NAME,
-    version='1.0.0',
-    packages=find_namespace_packages(),
+    version='1.1.0',
+    packages=find_namespace_packages(exclude=['test*']),
     data_files=[
         ('share/ament_index/resource_index/packages',
             ['resource/' + PACKAGE_NAME]),
         ('share/' + PACKAGE_NAME, ['package.xml']),
         (os.path.join('share', PACKAGE_NAME, 'launch'), glob('launch/*launch.py'))
     ],
-    install_requires=['setuptools'],
+    install_requires=[
+        'setuptools',
+        'antlr4-python3-runtime==4.7.2',
+        'transforms3d==0.3.1',
+        'pexpect==4.9.0',
+        'defusedxml==0.7.1',
+        'pyyaml==6.0.1',
+        'py-trees==2.1.6'
+    ],
     zip_safe=True,
     include_package_data=True,
     maintainer='Intel Labs',
     maintainer_email='scenario-execution@intel.com',
-    description='Robotics Scenario Execution',
+    url='https://github.com/IntelLabs/scenario_execution',
+    project_urls={
+        "Homepage": "https://github.com/IntelLabs/scenario_execution",
+        "Documentation": "https://github.com/IntelLabs/scenario_execution",
+        "Issues": "https://github.com/IntelLabs/scenario_execution/issues",
+    },
+    description='Scenario Execution for Robotics',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     license='Apache License 2.0',
+    classifiers=[
+        "Programming Language :: Python :: 3",
+    ],
     tests_require=['pytest'],
     entry_points={
         'console_scripts': [
-            'scenario_execution_base = scenario_execution_base.scenario_execution:main',
+            'scenario_execution = scenario_execution.scenario_execution_base:main',
         ],
         'scenario_execution.actions': [
-            'log = scenario_execution_base.actions.log:Log',
-            'run_process = scenario_execution_base.actions.run_process:RunProcess',
+            'log = scenario_execution.actions.log:Log',
+            'run_process = scenario_execution.actions.run_process:RunProcess',
         ],
         'scenario_execution.osc_libraries': [
-            'helpers = scenario_execution_base.get_osc_library:get_helpers_library',
-            'standard = scenario_execution_base.get_osc_library:get_standard_library',
-            'standard.base = scenario_execution_base.get_osc_library:get_standard_base_library',
-            'robotics = scenario_execution_base.get_osc_library:get_robotics_library',
+            'helpers = scenario_execution.get_osc_library:get_helpers_library',
+            'standard = scenario_execution.get_osc_library:get_standard_library',
+            'standard.base = scenario_execution.get_osc_library:get_standard_base_library',
+            'robotics = scenario_execution.get_osc_library:get_robotics_library',
         ]
     },
 )
```

### Comparing `scenario-execution-1.0.0/test/test_expression.py` & `scenario_execution-1.1.0/test/test_expression.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import unittest
 
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestExpression(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
     """
     Unit test for expression parsing
@@ -37,18 +37,17 @@
 unit s          of time is SI(s: 1, factor: 1)
 unit ms         of time is SI(s: 1, factor: 0.001)
 
 global test1: float = 2.0 + 1.1
 global test2: time = 2.0s + 1.1s
 global test3: time = 2.0s + 1ms
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual(model._ModelElement__children[3].get_resolved_value(), 3.1)
         self.assertEqual(model._ModelElement__children[4].get_resolved_value(), 3.1)
         self.assertEqual(model._ModelElement__children[5].get_resolved_value(), 2.001)
 
     @unittest.skip(reason="requires porting")
     def test_substract(self):
         scenario_content = """
@@ -56,51 +55,48 @@
 unit s          of time is SI(s: 1, factor: 1)
 unit ms         of time is SI(s: 1, factor: 0.001)
 
 global test1: float = 2.0 - 1.1
 global test2: time = 2.0s - 1.1s
 global test3: time = 2.0s - 1ms
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual(model._ModelElement__children[3].get_resolved_value(), 0.9)
         self.assertEqual(model._ModelElement__children[4].get_resolved_value(), 0.9)
         self.assertEqual(model._ModelElement__children[5].get_resolved_value(), 1.999)
 
     @unittest.skip(reason="requires porting")
     def test_multiply(self):
         scenario_content = """
 type time is SI(s: 1)
 unit ms         of time is SI(s: 1, factor: 0.001)
 
 global test1: float = 2.0 * 1.1
 global test2: time = 2.0ms * 1.1
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual(model._ModelElement__children[3].get_resolved_value(), 2.2)
         self.assertEqual(model._ModelElement__children[4].get_resolved_value(), 0.0022)
 
     @unittest.skip(reason="requires porting")
     def test_divide(self):
         scenario_content = """
 type time is SI(s: 1)
 unit ms         of time is SI(s: 1, factor: 0.001)
 
 global test1: float = 5.0 / 2.0
 global test2: time = 5.0ms / 2.0
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual(model._ModelElement__children[3].get_resolved_value(), 2.5)
         self.assertEqual(model._ModelElement__children[4].get_resolved_value(), 0.0025)
 
     @unittest.skip(reason="requires porting")
     def test_relation(self):
         scenario_content = """
 type time is SI(s: 1)
@@ -110,44 +106,41 @@
 global test2: bool = 5 > 2
 global test3: bool = 5 < 2
 global test4: bool = 5 == 2
 global test5: bool = 5 != 2
 global test6: bool = 5 >= 2
 global test7: bool = 5 <= 2
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual(model._ModelElement__children[3].get_resolved_value(), True)
         self.assertEqual(model._ModelElement__children[4].get_resolved_value(), True)
         self.assertEqual(model._ModelElement__children[5].get_resolved_value(), False)
         self.assertEqual(model._ModelElement__children[6].get_resolved_value(), False)
         self.assertEqual(model._ModelElement__children[7].get_resolved_value(), True)
         self.assertEqual(model._ModelElement__children[8].get_resolved_value(), True)
         self.assertEqual(model._ModelElement__children[9].get_resolved_value(), False)
 
     @unittest.skip(reason="requires porting")
     def test_negation(self):
         scenario_content = """
 global test1: bool = not True
 global test1: bool = not 5 > 2
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual(model._ModelElement__children[0].get_resolved_value(), False)
         self.assertEqual(model._ModelElement__children[1].get_resolved_value(), False)
 
     @unittest.skip(reason="requires porting")
     def test_compound_expression(self):
         scenario_content = """
 global test1: bool = 2 > 1 and 3 >= 2
 global test1: bool = 2 > 1 or 3 < 2
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual(model._ModelElement__children[0].get_resolved_value(), True)
         self.assertEqual(model._ModelElement__children[1].get_resolved_value(), True)
```

### Comparing `scenario-execution-1.0.0/test/test_model_ser_deser.py` & `scenario_execution-1.1.0/test/test_model_ser_deser.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Test for Intermediate Scenario model Serialization and Deserialization
 """
 import unittest
 
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import BaseLogger, Logger
-from scenario_execution_base.model.types import print_tree, serialize, deserialize
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import BaseLogger, Logger
+from scenario_execution.model.types import print_tree, serialize, deserialize
 from antlr4.InputStream import InputStream
 
 
 class DebugLogger(BaseLogger):
 
     def __init__(self, name):
         super().__init__(name, False)
@@ -58,18 +58,16 @@
     msg: string
 
 scenario test:
     do serial:
         log("foo")
         emit end
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.load_internal_model(parsed_tree, "test.osc", False, False)
-        self.assertIsNotNone(model)
         serialize_data = serialize(model)['CompilationUnit']['_children']
         self.assertGreater(len(serialize_data), 0)
         deserialized_model = deserialize(serialize_data)
 
         # validate model
         deserialize_model_logger = DebugLogger('out')
         input_model_logger = DebugLogger('in')
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_parser_action.py` & `scenario_execution-1.1.0/test/test_osc2_parser_action.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,49 +15,43 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Test action parsing
 """
 import unittest
 
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
 
     def setUp(self) -> None:
         self.parser = OpenScenario2Parser(Logger('test', False))
 
     def test_action_valid(self):
         scenario_content = """
 action test_action:
     param1: string = "value1"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
     def test_action_unknown_actor(self):
         scenario_content = """
 action UNKNOWN.test_action:
     param1: string = "value1"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_action_valid_actor(self):
         scenario_content = """
 actor base
 
 action base.test_action:
     param1: string = "value1"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_parser_actor.py` & `scenario_execution-1.1.0/test/test_osc2_parser_actor.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,59 +15,53 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Test actor parsing
 """
 import unittest
 
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
 
     def setUp(self) -> None:
         self.parser = OpenScenario2Parser(Logger('test', False))
 
     def test_actor(self):
         scenario_content = """
 actor base:
     param1: string = "value1"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
         self.assertEqual(model._ModelElement__children[0].actor, "base")
         self.assertEqual(model._ModelElement__children[0]._ModelElement__children[0].get_resolved_value(), "value1")
 
     def test_actor_inheritance(self):
         scenario_content = """
 actor base:
     param1: string = "value1"
 actor derived inherits base:
     param2: string = "value2"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
         self.assertEqual(model._ModelElement__children[0]._ModelElement__children[0].get_resolved_value(), "value1")
         self.assertEqual(model._ModelElement__children[1]._ModelElement__children[1].get_resolved_value(), "value2")
 
     def test_actor_inheritance_override(self):  # TODO: expected?
         scenario_content = """
 actor base:
     param1: string = "value1"
 actor derived inherits base:
     param1: string = "OVERRIDE"
     param2: string = "value2"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         params = model._ModelElement__children[1].get_resolved_value()
         self.assertEqual({'param1': 'OVERRIDE', 'param2': 'value2'}, params)
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_parser_behavior_invocation.py` & `scenario_execution-1.1.0/test/test_osc2_parser_behavior_invocation.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Test behavior invocation parsing
 """
 import unittest
 
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
 
     def setUp(self) -> None:
@@ -52,18 +52,16 @@
         keep(it.name == 'test_obstacle1')
         keep(it.model_file == 'test_model')
     do parallel:
         test_drive: serial:
             spawn_it: test_obstacle1.spawn() with:
                 keep(it.namespace == 'bll')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
         behavior = model._ModelElement__children[3]._ModelElement__children[1]._ModelElement__children[0]._ModelElement__children[0]._ModelElement__children[0]
         params = behavior.get_resolved_value()
         self.assertEqual({'spawn_pose': {'x': 'x_val'}, 'world_name': 'default',
                          'namespace': 'bll', 'entity_name': '', 'model_file': '', 'xacro_arguments': ''}, params)
 
     def test_behavior_named_arg(self):
         scenario_content = """
@@ -74,18 +72,16 @@
     param2: string = 'val2'
 
 scenario test:
     test_obstacle1: osc_object
     do parallel:
         spawn_it: test_obstacle1.spawn(param1: 'override1')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         behavior = model._ModelElement__children[2]._ModelElement__children[1]._ModelElement__children[0]._ModelElement__children[0]
         params = behavior.get_resolved_value()
         self.assertEqual(params, {'param1': 'override1', 'param2': 'val2'})
 
     def test_behavior_from_base_actor(self):
         scenario_content = """
@@ -97,67 +93,59 @@
 actor robot inherits osc_object
 
 scenario test:
     test_obstacle1: robot
     do parallel:
         spawn_it: test_obstacle1.spawn(param1: 'override1')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
     def test_behavior_invalid_param_name(self):
         scenario_content = """
 actor osc_object
 
 action osc_object.spawn:
     name: string = 'NOTALLOWED'
 
 scenario test:
     test_obstacle1: osc_object
     do parallel:
         spawn_it: test_obstacle1.spawn(param1: 'override1')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_behavior_invalid_param_associated_actor(self):
         scenario_content = """
 actor osc_object
 
 action osc_object.spawn:
     associated_actor: string = 'NOTALLOWED'
     param1: string
 
 scenario test:
     test_obstacle1: osc_object
     do parallel:
         spawn_it: test_obstacle1.spawn(param1: 'override1')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_behavior_positional_arg(self):
         scenario_content = """
 action test:
     param1: string = 'base'
 
 scenario test:
     do parallel:
         spawn_it: test('override1')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         behavior = model._ModelElement__children[1]._ModelElement__children[0]._ModelElement__children[0]._ModelElement__children[0]
         params = behavior.get_resolved_value()
         self.assertEqual(params, {'param1': 'override1'})
 
     @unittest.skip(reason="requires porting")
     def test_behavior_empty_args(self):
@@ -166,111 +154,101 @@
     param1: string
     param2: string
 
 scenario test:
     do parallel:
         spawn_it: test()
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
         self.assertIsNone(model)
 
     @unittest.skip(reason="requires porting")
     def test_behavior_partially_defined_args(self):
         scenario_content = """
 action test:
     param1: string = 'val1'
     param2: string
 
 scenario test:
     do parallel:
         spawn_it: test()
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc")
         self.assertIsNone(model)
 
     @unittest.skip(reason="requires porting")
     def test_behavior_partially_overridden_positional_args(self):
         scenario_content = """
 action test:
     param1: string
     param2: string
 
 scenario test:
     do parallel:
         spawn_it: test('override1')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc")
         self.assertIsNone(model)
 
     @unittest.skip(reason="requires porting")
     def test_behavior_partially_overridden_named_args(self):
         scenario_content = """
 action test:
     param1: string
     param2: string
 
 scenario test:
     do parallel:
         spawn_it: test(param2: 'override2')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc")
         self.assertIsNone(model)
 
     def test_behavior_too_many_named_args(self):
         scenario_content = """
 action test:
     param1: string
     param2: string
 
 scenario test:
     do parallel:
         spawn_it: test(param1: 'override1', param2: 'override2', param3: 'override3')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_behavior_too_many_positional_args(self):
         scenario_content = """
 action test:
     param1: string
     param2: string
 
 scenario test:
     do parallel:
         spawn_it: test('override1', 'override2', 'override3')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_behavior_unknown_named_args(self):
         scenario_content = """
 action test:
     param1: string
     param2: string
 
 scenario test:
     do parallel:
         spawn_it: test(param1: 'override1', UNKNOWN: 'override2')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     @unittest.skip(reason="requires porting")
     def test_behavior_struct_param_named_override(self):
         scenario_content = """
 struct test_struct:
     param1: string = "val1"
     param2: string = "val2"
@@ -279,18 +257,16 @@
     struct_param: test_struct
 
 scenario test:
     do serial:
         test_action() with:
             keep(it.struct_param == test_struct(param2: 'OVERRIDE'))
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         behavior = model._ModelElement__children[2]._ModelElement__children[1]._ModelElement__children[0]._ModelElement__children[1]
         params = behavior.get_resolved_value()
         self.assertEqual(params, {'struct_param': {'param1': 'val1', 'param2': 'OVERRIDE'}})
 
     def test_behavior_struct_param_positional_override(self):
         scenario_content = """
@@ -302,18 +278,16 @@
     struct_param: test_struct
 
 scenario test:
     do serial:
         test_action() with:
             keep(it.struct_param == test_struct('OVERRIDE'))
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         behavior = model._ModelElement__children[2]._ModelElement__children[0]._ModelElement__children[0]._ModelElement__children[0]
         params = behavior.get_resolved_value()
         self.assertEqual(params, {'struct_param': {'param1': 'OVERRIDE', 'param2': 'val2'}})
 
     def test_behavior_struct_param_partially_named_positional_override(self):
         scenario_content = """
@@ -326,18 +300,16 @@
     struct_param: test_struct
 
 scenario test:
     do serial:
         test_action() with:
             keep(it.struct_param == test_struct('OVERRIDE1', param3: 'OVERRIDE3'))
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         behavior = model._ModelElement__children[2]._ModelElement__children[0]._ModelElement__children[0]._ModelElement__children[0]
         params = behavior.get_resolved_value()
         self.assertEqual(params, {'struct_param': {'param1': 'OVERRIDE1',
                          'param2': 'val2', 'param3': 'OVERRIDE3'}})
 
     @unittest.skip(reason="requires porting")
@@ -351,16 +323,15 @@
     struct_param: test_struct
 
 scenario test:
     do serial:
         test_action() with:
             keep(it.struct_param == test_struct('OVERRIDE1'))
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc")
         self.assertIsNone(model)
 
     def test_base_vals(self):
         scenario_content = """
 type length is SI(m: 1)
 unit m          of length is SI(m: 1, factor: 1)
@@ -397,18 +368,16 @@
             turtlebot4.spawn() with:                            # spawn the robot
                 keep(it.spawn_pose.position.x == 0.0m)
                 keep(it.spawn_pose.position.y == 0.0m)
                 keep(it.spawn_pose.position.z == 0.1m)
                 keep(it.spawn_pose.orientation.yaw == 0.0rad)
                 keep(it.spawn_pose.orientation.roll == 1.0rad)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         pose_struct = model._ModelElement__children[7].get_resolved_value()
         self.assertEqual({'position': {'x': 0., 'y': 0., 'z': 0.}, 'orientation': {
                          'roll': 0., 'pitch': 0., 'yaw': 0.}}, pose_struct)
 
         behavior = model._ModelElement__children[10]._ModelElement__children[1]._ModelElement__children[0]._ModelElement__children[0].get_resolved_value(
         )
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_parser_enum.py` & `scenario_execution-1.1.0/test/test_osc2_parser_enum.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Test enum parsing
 """
 import unittest
 
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
     """
     Unit test for osc2_parser
@@ -38,48 +38,43 @@
 enum test_enum: [
     val1,
     val2
 ]
 struct test:
     param1: test_enum = test_enum!val1
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         test_struct = model._ModelElement__children[1]
         self.assertEqual(test_struct.get_resolved_value(), {'param1': ('val1', 0)})
 
     def test_enum_ref_invalid(self):
         scenario_content = """
 enum test_enum: [
     val1,
     val2
 ]
 struct test:
     param1: test_enum = test_enum!UNKNOWN
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_enum_ref_invalid_type(self):
         scenario_content = """
 enum test_enum: [
     val1,
     val2
 ]
 struct test:
     param1: test_enum = UNKNOWN!val1
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_enum_ref_other_enum_type(self):
         scenario_content = """
 enum other_enum: [
     val1,
     val2
 ]
@@ -88,65 +83,60 @@
     val1,
     val2
 ]
 
 struct test:
     param1: test_enum = other_enum!val1
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_enum_val_non_numeric(self):
         scenario_content = """
 enum test_enum: [
     val1,
     val2
 ]
 
 struct test:
     param1: test_enum = test_enum!val1
     param2: test_enum = test_enum!val2
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         test_struct = model._ModelElement__children[1]
         self.assertEqual(test_struct.get_resolved_value(), {'param1': ('val1', 0), 'param2': ('val2', 1)})
 
     def test_enum_partially_numeric(self):
         scenario_content = """
 enum test_enum: [
     val1 = 4,
     val2
 ]
 
 struct test:
     param1: test_enum = test_enum!val1
     param2: test_enum = test_enum!val2
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         test_struct = model._ModelElement__children[1]
         self.assertEqual(test_struct.get_resolved_value(), {'param1': ('val1', 4), 'param2': ('val2', 5)})
 
     def test_enum_fully_numeric(self):
         scenario_content = """
 enum test_enum: [
     val1 = 4,
     val2 = 19
 ]
 
 struct test:
     param1: test_enum = test_enum!val1
     param2: test_enum = test_enum!val2
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         test_struct = model._ModelElement__children[1]
         self.assertEqual(test_struct.get_resolved_value(), {'param1': ('val1', 4), 'param2': ('val2', 19)})
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_parser_event.py` & `scenario_execution-1.1.0/test/test_osc2_parser_wait.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,54 +11,71 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
-Test event parsing
+Test wait parsing
 """
 import unittest
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
+
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.model.model_to_py_tree import create_py_tree
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
-class TestScenarioExectionSuccess(unittest.TestCase):
+class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
 
     def setUp(self) -> None:
         self.parser = OpenScenario2Parser(Logger('test', False))
 
-    def test_unknown_event(self):
+    def test_wait_success(self):
+        scenario_content = """
+type time is SI(s: 1)
+unit s          of time is SI(s: 1, factor: 1)
+
+scenario test:
+    do serial:
+        wait elapsed(1s)
+"""
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
+        model = create_py_tree(model, self.parser.logger, False)
+
+    def test_wait_invalid(self):
         scenario_content = """
+type time is SI(s: 1)
+unit s          of time is SI(s: 1, factor: 1)
+
 scenario test:
     do serial:
-        emit UNKNOWN
+        wait(1s)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
 
-    def test_event_success(self):
+        self.assertRaises(ValueError, create_py_tree, model, self.parser.logger, False)
+
+    def test_wait_invalid_literal(self):
         scenario_content = """
 scenario test:
-    event test1
     do serial:
-        emit test1
+        wait(1)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
-    def test_event_end(self):
+        self.assertRaises(ValueError, create_py_tree, model, self.parser.logger, False)
+
+    def test_wait_invalid_literal2(self):
         scenario_content = """
 scenario test:
     do serial:
-        emit end
+        wait elapsed(1)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
+        self.assertRaises(ValueError, create_py_tree, model, self.parser.logger, False)
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_parser_keep.py` & `scenario_execution-1.1.0/test/test_osc2_parser_keep.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Test keep parsing
 """
 import unittest
 
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
 
     def setUp(self) -> None:
@@ -37,13 +37,11 @@
 actor differential_drive_robot inherits osc_object:
     namespace: string = ''
 
 scenario nav2_simulation_nav_to_pose:
     turtlebot4: differential_drive_robot with:
         keep(it.namespace == 'test')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
         robot = model._ModelElement__children[2]._ModelElement__children[0].get_resolved_value()
         self.assertEqual({'namespace': 'test'}, robot)
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_parser_list.py` & `scenario_execution-1.1.0/test/test_osc2_parser_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Test list parsing
 """
 import unittest
 
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
     """
     Unit test for osc2_parser
@@ -35,109 +35,92 @@
 
     def test_invalid_listof(self):
         scenario_content = """
 struct listoffoo
 
 global test: listoffoo
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_string_list(self):
         scenario_content = """
 global test: list of string = ["foo", "bar"]
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         test_list = model._ModelElement__children[0].get_resolved_value()
         self.assertEqual(["foo", "bar"], test_list)
 
     def test_empty_list(self):
         scenario_content = """
 global test: list of string = [ ]
 """
-        _, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 1)
+        self.assertRaises(ValueError, self.parser.parse_input_stream, InputStream(scenario_content))
 
     def test_mixed_basetypes_list(self):
         scenario_content = """
 global test: list of string = ["foo", 3]
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_struct_list(self):
         scenario_content = """
 struct test_struct:
     member: string
 global test: list of test_struct = [test_struct('val1'), test_struct('val2')]
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         test_list = model._ModelElement__children[1].get_resolved_value()
         self.assertEqual([{'member': 'val1'}, {'member': 'val2'}], test_list)
 
     def test_different_structs_in_list(self):
         scenario_content = """
 struct test_struct:
     member: string
 struct second_struct:
     member2: string
 global test: list of test_struct = [test_struct('val1'), second_struct('invalid')]
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_assign_struct_list(self):
         scenario_content = """
 struct test_struct:
     member: string
 
 global test1: list of test_struct = [test_struct('val1'), test_struct('val2')]
 global test2: list of test_struct = test1
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         test1 = model._ModelElement__children[1].get_resolved_value()
         test2 = model._ModelElement__children[2].get_resolved_value()
         self.assertEqual([{'member': 'val1'}, {'member': 'val2'}], test1)
         self.assertEqual([{'member': 'val1'}, {'member': 'val2'}], test2)
 
     def test_assign_basetype_list(self):
         scenario_content = """
 global test1: list of float = [2.1, 4.3]
 global test2: list of float = test1
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         test1 = model._ModelElement__children[0].get_resolved_value()
         test2 = model._ModelElement__children[1].get_resolved_value()
         self.assertEqual([2.1, 4.3], test1)
         self.assertEqual([2.1, 4.3], test2)
 
     def test_assign_wrong_basetype_list(self):
         scenario_content = """
 global test1: list of float = [2.1, 4.3]
 global test2: list of string = test1
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_parser_not_supported.py` & `scenario_execution-1.1.0/test/test_osc2_parser_not_supported.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,260 +15,216 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Test parsing error reporting for features that are not yet supported
 """
 import unittest
 
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable, too-many-public-methods
 
     def setUp(self) -> None:
         self.parser = OpenScenario2Parser(Logger('test', False))
 
     def test_method(self):
         scenario_content = """
 actor test:
     def get_value() -> float is external TEST()
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_cover(self):
         scenario_content = """
 scenario test:
     cover()
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_lt_expr(self):
         scenario_content = """
 actor car:
     current_position: float
     keep(current_position < 100.0)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_gt_expr(self):
         scenario_content = """
 actor car:
     current_position: float
     keep(current_position > 100.0)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_le_expr(self):
         scenario_content = """
 actor car:
     current_position: float
     keep(current_position <= 100.0)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_ge_expr(self):
         scenario_content = """
 actor car:
     current_position: float
     keep(current_position >= 100.0)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_range(self):
         scenario_content = """
 global test: float = range(0,1)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_element_access(self):
         scenario_content = """
 global foo: list of float
 global test: float = foo[2]
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_type_test(self):
         scenario_content = """
 global foo: float
 global test: bool = foo.is(float)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_cast(self):
         scenario_content = """
 global foo: float
 global test: int = foo.as(int)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_sample(self):
         scenario_content = """
 import osc.standard.base
 
 scenario simple_drive:    
     environment: environment
     var sim_start_time: time = sample(environment.datetime, @root_phase.start)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_every(self):
         scenario_content = """
 scenario test:
     event test is every(1)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_rise(self):
         scenario_content = """
 scenario test:
     event test is rise(true)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_fall(self):
         scenario_content = """
 scenario test:
     event test is fall(true)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_modifier(self):
         scenario_content = """
 modifier test
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_modifier_application(self):
         scenario_content = """
 modifier test_modifier:
     param1: string
 
 action test_action:
     param2: string
 
 scenario test:
     do serial:
         test_action() with:
             test_modifier(6)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_until(self):
         scenario_content = """
 scenario test:
     event ev
     do serial:
         test_action() with:
             until @ev
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_call(self):
         scenario_content = """
 scenario test:
     do serial:
         call log(true)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_remove_default(self):
         scenario_content = """
 struct base:
     param_base: string = "base"
     
 struct test:
     param1: base = base with:
         remove_default(it.param_base)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_record(self):
         scenario_content = """
 scenario test:
     record()
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_enum_extend(self):
         scenario_content = """
 enum test: [a, b]
 extend test: [c]
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_conditional_inheritance(self):
         scenario_content = """
 struct vehicle:
     is_electric: bool
 
 actor electric_vehicle inherits vehicle(is_electric == true)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_parser_parameter.py` & `scenario_execution-1.1.0/test/test_osc2_parser_parameter.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Test parameter parsing
 """
 import unittest
 
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.model.model_to_py_tree import create_py_tree
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.model.model_to_py_tree import create_py_tree
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable, too-many-public-methods
     """
     Unit test for osc2_parser
@@ -34,332 +34,296 @@
     def setUp(self) -> None:
         self.parser = OpenScenario2Parser(Logger('test', False))
 
     def test_invalid(self):
         scenario_content = """
 invalid
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 1)
+        self.assertRaises(ValueError, self.parser.parse_input_stream, InputStream(scenario_content))
 
     def test_empty(self):
         scenario_content = ""
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         scenarios = create_py_tree(model, self.parser.logger, False)
         self.assertEqual([], scenarios)
 
     def test_global_var(self):
         scenario_content = """
 global level1: string = "hey!"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         param = model._ModelElement__children[0].get_resolved_value()
         self.assertEqual(param, "hey!")
 
     def test_global_var_indirect_1(self):
         scenario_content = """
 global level1: string = "hey!"
 global level2: string = level1
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual(len(model._ModelElement__children), 2)
         glob_param1 = model._ModelElement__children[0]
         val1 = glob_param1.get_resolved_value()
         self.assertEqual(val1, "hey!")
         glob_param2 = model._ModelElement__children[1]
         val2 = glob_param2.get_resolved_value()
         self.assertEqual(val2, "hey!")
 
     def test_global_var_indirect_2(self):
         scenario_content = """
 global level1: string = "hey!"
 global level2: string = level1
 global level3: string = level2
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual(model._ModelElement__children[0].get_resolved_value(), 'hey!')
         self.assertEqual(model._ModelElement__children[1].get_resolved_value(), 'hey!')
         self.assertEqual(model._ModelElement__children[2].get_resolved_value(), 'hey!')
 
     def test_global_var_indirect_2_wrong_type(self):
         scenario_content = """
 global level1: string = "hey!"
 global level2: int = level1
 global level3: string = level2
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_global_var_indirect_3(self):
         scenario_content = """
 global level1: string = "hey!"
 global level2: string = level1
 global level3: string = level2
 
 scenario test:
     var test_var: string = level3
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual(model._ModelElement__children[0].get_resolved_value(), 'hey!')
         self.assertEqual(model._ModelElement__children[1].get_resolved_value(), 'hey!')
         self.assertEqual(model._ModelElement__children[2].get_resolved_value(), 'hey!')
         self.assertEqual(model._ModelElement__children[3]._ModelElement__children[0].get_resolved_value(), 'hey!')
 
     def test_global_var_indirect_not_found(self):
         scenario_content = """
 global level1: string = "hey!"
 global level2: int = levelUNKNOWN
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_global_var_indirect_in_struct(self):
         scenario_content = """
 global z_param: string = "z_global"
 struct test_struct:
     z: string = z_param
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual({'z': 'z_global'}, model._ModelElement__children[1].get_resolved_value())
 
     def test_global_var_indirect_in_actor(self):
         scenario_content = """
 global z_param: string = "z_global"
 actor test_struct:
     z: string = z_param
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual({'z': 'z_global'}, model._ModelElement__children[1].get_resolved_value())
 
     def test_var_instance_unknown_type(self):
         scenario_content = """
 scenario test:
     test_pose: unknownType 
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_var_instance_keep_not_it(self):
         scenario_content = """
 struct pose3d:
     z: string = "base"
 scenario network_drop_straight:
     test_pose: pose3d with:
         keep(NO.z == "override")
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_var_instance_keep_unknown_member(self):
         scenario_content = """
 struct pose3d:
     z: string = "base"
 scenario network_drop_straight:
     test_pose: pose3d with:
         keep(it.UNKNOWN == "override")
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_var_instance_keep_success(self):
         scenario_content = """
 struct pose3d:
     z: string = "base"
 scenario network_drop_straight:
     test_pose: pose3d with:
         keep(it.z == "override")
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
     def test_var_instance_keep_not_equal(self):
         scenario_content = """
 struct pose3d:
     z: string = "base"
 scenario network_drop_straight:
     test_pose: pose3d with:
         keep(it.z <= "override")
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_struct_inheritance(self):
         scenario_content = """
 struct base:
     x: string = "base"
     
 struct derived inherits base:
     y: string = "derived"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual({'x': 'base', 'y': 'derived'},
                          model._ModelElement__children[1].get_resolved_value())
 
     def test_actor_inheritance(self):
         scenario_content = """
 actor base:
     x: string = "base"
     
 actor derived inherits base:
     y: string = "derived"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual({'x': 'base', 'y': 'derived'},
                          model._ModelElement__children[1].get_resolved_value())
 
     def test_actor_inheritance_invalid(self):
         scenario_content = """
 actor derived inherits UNKNOWN:
     y: string = "derived"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
         scenario_content = """
 action base:
     x: string = "base"
     
 action derived inherits base:
     y: string = "derived"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         self.assertEqual({'x': 'base', 'y': 'derived'},
                          model._ModelElement__children[1].get_resolved_value())
 
     def test_action_inheritance_invalid(self):
         scenario_content = """
 action derived inherits UNKNOWN:
     y: string = "derived"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_scenario_inheritance(self):
         scenario_content = """
 scenario base:
     x: string = "base"
     
 scenario derived inherits base:
     y: string = "derived"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         derived = model._ModelElement__children[1]
         self.assertEqual({'x': 'base', 'y': 'derived'}, derived.get_resolved_value())
 
     def test_scenario_inheritance_invalid(self):
         scenario_content = """
 scenario derived inherits UNKNOWN:
     y: string = "derived"
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_parameter_to_dict(self):
         scenario_content = """
 struct test_struct:
     x: string = "value_x"
     y: string = "value_y"
     
 scenario test:
     foo: test_struct with:
         keep(it.x == "override_x")
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         param = model._ModelElement__children[1]._ModelElement__children[0]
         values = param.get_resolved_value()
         self.assertEqual({"x": "override_x", "y": "value_y"}, values)
 
     def test_struct_with_keep(self):
         scenario_content = """
 struct test_struct:
     x: string = "value_x"
     y: string = "value_y"
     
 global foo: test_struct with:
         keep(it.x == "override_x")
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         param = model._ModelElement__children[1]
         values = param.get_resolved_value()
         self.assertEqual({"x": "override_x", "y": "value_y"}, values)
 
     @unittest.skip(reason="requires porting")
     def test_struct_with_keep_member_unknown(self):
         scenario_content = """
 struct test_struct:
     x: string = "value_x"
     y: string = "value_y"
     
 global foo: test_struct with:
         keep(it.UNKNOWN == "override_x")
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         param = model._ModelElement__children[1]
         values = param.get_resolved_value()  # parse should already fail!
 
     def test_parameter_to_dict_two_level(self):
         scenario_content = """
 struct base_struct:
     x: string = "base_x"
@@ -368,36 +332,34 @@
 struct test_struct inherits base_struct:
     z: string = "value_z"
     
 scenario test:
     foo: test_struct with:
         keep(it.x == "override_x")
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         param = model._ModelElement__children[2]._ModelElement__children[0]
         values = param.get_resolved_value()
         self.assertEqual({"x": "override_x", "y": "base_y", "z": "value_z"}, values)
 
     def test_parameter_struct_in_struct(self):
         scenario_content = """
 struct base_struct:
     a: string = "base_a"
     b: string = "base_b"
     
 struct test_struct:
     x: string = "value_x"
     y: base_struct
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         base_struct = model._ModelElement__children[0]
 
         values = base_struct.get_resolved_value()
         self.assertEqual({"a": "base_a", "b": "base_b"}, values)
         test_struct = model._ModelElement__children[1]
         values = test_struct.get_resolved_value()
         self.assertEqual({"x": "value_x", "y": {"a": "base_a", "b": "base_b"}}, values)
@@ -411,18 +373,17 @@
     b: string = "value_x"
     c: base_struct
     
 struct l2_struct:
     d: string = "value_x"
     e: l1_struct
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         base_struct = model._ModelElement__children[0]
         self.assertEqual({"a": "base_a"}, base_struct.get_resolved_value())
         l1_struct = model._ModelElement__children[1]
         self.assertEqual({'b': 'value_x', 'c': {'a': 'base_a'}}, l1_struct.get_resolved_value())
         l2_struct = model._ModelElement__children[2]
         self.assertEqual({'d': 'value_x', 'e': {'b': 'value_x', 'c': {
                          'a': 'base_a'}}}, l2_struct.get_resolved_value())
@@ -430,31 +391,28 @@
     def test_unknown_type(self):
         scenario_content = """
 type length is SI(m: 1)
 unit cm         of length is SI(m: 1, factor: 0.01)
 
 global val1: UNKNOWN
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_struct_param_default(self):
         scenario_content = """
 struct test_struct:
     param1: string = "val1"
     param2: string = "val2"
 
 global test_struct1: test_struct = test_struct(param2: 'OVERRIDE')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         test_struct1 = model._ModelElement__children[1]
         self.assertEqual({'param1': 'val1', 'param2': 'OVERRIDE'},
                          test_struct1.get_resolved_value())
 
     def test_struct_param_function_wrong_type(self):
         scenario_content = """
 struct other_type:
@@ -462,61 +420,56 @@
 
 struct test_struct:
     param1: string = "val1"
     param2: string = "val2"
 
 global test_struct1: test_struct = other_type(param2: 'OVERRIDE')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_struct_assigned_empty(self):
         scenario_content = """
 struct base_struct:
     base_param1: string = "base1"
 
 struct test_struct:
     param_base_struct: base_struct = base_struct()
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         test_struct = model._ModelElement__children[1]
         self.assertEqual({'param_base_struct': {'base_param1': 'base1'}},
                          test_struct.get_resolved_value())
 
     def test_struct_assigned_with_params(self):
         scenario_content = """
 struct base_struct:
     base_param1: string = "base1"
 
 struct test_struct:
     param_base_struct: base_struct = base_struct('OVERRIDE')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         test_struct = model._ModelElement__children[1]
         self.assertEqual({'param_base_struct': {'base_param1': 'OVERRIDE'}},
                          test_struct.get_resolved_value())
 
     def test_struct_assigned_by_var(self):
         scenario_content = """
 struct base_struct:
     base_param1: string = "base1"
 
 global test_struct1: base_struct = base_struct(base_param1: 'OVERRIDE')
 
 struct test_struct:
     param_base_struct: base_struct = test_struct1
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         test_struct = model._ModelElement__children[2]
         self.assertEqual({'param_base_struct': {'base_param1': 'OVERRIDE'}},
                          test_struct.get_resolved_value())
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_parser_physical_type.py` & `scenario_execution-1.1.0/test/test_osc2_parser_physical_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Test physical type parsing
 """
 import unittest
 
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
 
     def setUp(self) -> None:
@@ -37,29 +37,26 @@
 unit m          of length is SI(m: 1, factor: 1)
 type time is SI(s: 1)
 unit s          of time is SI(s: 1, factor: 1)
 
 action odometry_distance_traveled:
     distance: length = 3m
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         action = model._ModelElement__children[4].get_resolved_value()
         self.assertEqual({'distance': 3.0}, action)
 
     def test_wrong_type(self):
         scenario_content = """
 
 type length is SI(m: 1)
 unit m          of length is SI(m: 1, factor: 1)
 type time is SI(s: 1)
 unit s          of time is SI(s: 1, factor: 1)
 
 action odometry_distance_traveled:
     distance: length = 3s
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_parser_si.py` & `scenario_execution-1.1.0/test/test_osc2_parser_si.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Test si parsing
 """
 import unittest
 
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
 
     def setUp(self) -> None:
@@ -33,49 +33,42 @@
     def test_si_invalid_type(self):
         scenario_content = """
 type length is SI(m: 1)
 unit cm         of length is SI(m: 1, factor: 0.01)
 
 global val1: string = 3.2cm
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
 
     def test_si(self):
         scenario_content = """
 type length is SI(m: 1)
 unit cm         of length is SI(m: 1, factor: 0.01)
 
 global val1: length = 3.2cm
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         param = model._ModelElement__children[2]
         self.assertEqual(param.get_resolved_value(), 0.032)
 
     def test_si_naming(self):
         scenario_content = """
 type length is SI(m: 1)
 unit m          of length is SI(m: 1, factor: 1)
 global val1: length = 3.2m
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
+
         param = model._ModelElement__children[2]
         self.assertEqual(param.get_resolved_value(), 3.2)
 
     def test_si_unknown_type(self):
         scenario_content = """
 type length is SI(m: 1)
 unit m          of UNKNOWN is SI(m: 1, factor: 1)
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc")
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_parser_struct.py` & `scenario_execution-1.1.0/test/test_osc2_parser_struct.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Test struct parsing
 """
 import unittest
 
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
 
     def setUp(self) -> None:
@@ -63,18 +63,16 @@
 scenario test:
     struct2e: struct1a with:
         keep(it.struct_param == base_struct('override'))
 
     struct2f: struct1a with:
         keep(it.struct_param == base_struct(base_param1: 'override'))
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         struct1a = model._ModelElement__children[4].get_resolved_value()
         struct1b = model._ModelElement__children[5].get_resolved_value()
         struct1c = model._ModelElement__children[6].get_resolved_value()
         struct2a = model._ModelElement__children[7].get_resolved_value()
         struct2b = model._ModelElement__children[8].get_resolved_value()
         struct2c = model._ModelElement__children[9].get_resolved_value()
@@ -114,18 +112,16 @@
         
     struct4: l2_struct with:
         keep(it.l1.base.param1 == 'override')
         
     struct5: l2_struct with:
         keep(it.l1.base == base_struct('override'))
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         struct1 = model._ModelElement__children[3]._ModelElement__children[0].get_resolved_value()
         struct2 = model._ModelElement__children[3]._ModelElement__children[1].get_resolved_value()
         struct3 = model._ModelElement__children[3]._ModelElement__children[2].get_resolved_value()
         struct4 = model._ModelElement__children[3]._ModelElement__children[3].get_resolved_value()
         struct5 = model._ModelElement__children[3]._ModelElement__children[4].get_resolved_value()
         self.assertEqual({'l1': {'base': {'param1': 'test'}}}, struct1)
@@ -145,18 +141,16 @@
 struct l2_struct:
     l1: l1_struct
     
 scenario test:        
     struct4: l2_struct with:
         keep(it.l1.base.param1 == 'override')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
         struct1 = model._ModelElement__children[3]._ModelElement__children[0].get_resolved_value()
         self.assertEqual({'l1': {'base': {'param1': 'override'}}}, struct1)
 
     def test_sub_struct_invalid_membername(self):
         scenario_content = """
 struct base_struct:
@@ -168,11 +162,9 @@
 struct l2_struct:
     l1: l1_struct
     
 scenario test:        
     struct4: l2_struct with:
         keep(it.l1.UNKNOWN.param1 == 'override')
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNone(model)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc")
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_parser_wait.py` & `scenario_execution-1.1.0/test/test_scenario_events.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,83 +11,73 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
-Test wait parsing
+Test predefined events
 """
 import unittest
-
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.model.model_to_py_tree import create_py_tree
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.scenario_execution_base import ScenarioExecution
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.model.model_to_py_tree import create_py_tree
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
 
     def setUp(self) -> None:
         self.parser = OpenScenario2Parser(Logger('test', False))
+        self.scenario_execution = ScenarioExecution(debug=True, log_model=True, live_tree=True, scenario_file='test.osc', output_dir="")
 
-    def test_wait_success(self):
+    def test_failure(self):
         scenario_content = """
-type time is SI(s: 1)
-unit s          of time is SI(s: 1, factor: 1)
-
 scenario test:
     do serial:
-        wait elapsed(1s)
+        emit fail
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
-        model = create_py_tree(model, self.parser.logger, False)
-        self.assertIsNotNone(model)
+        scenarios = create_py_tree(model, self.parser.logger, False)
+        self.scenario_execution.scenarios = scenarios
+        self.scenario_execution.run()
+        self.assertFalse(self.scenario_execution.process_results())
 
-    def test_wait_invalid(self):
+    def test_success(self):
         scenario_content = """
-type time is SI(s: 1)
-unit s          of time is SI(s: 1, factor: 1)
-
 scenario test:
     do serial:
-        wait(1s)
+        emit end
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
-
         scenarios = create_py_tree(model, self.parser.logger, False)
-        self.assertIsNone(scenarios)
+        self.scenario_execution.scenarios = scenarios
+        self.scenario_execution.run()
+        self.assertTrue(self.scenario_execution.process_results())
 
-    def test_wait_invalid_literal(self):
+    def test_wait_for_event(self):
         scenario_content = """
-scenario test:
-    do serial:
-        wait(1)
-"""
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
-        model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
-
-        model = create_py_tree(model, self.parser.logger, False)
-        self.assertIsNone(model)
+type time is SI(s: 1)
+unit s          of time is SI(s: 1, factor: 1)
 
-    def test_wait_invalid_literal2(self):
-        scenario_content = """
 scenario test:
-    do serial:
-        wait elapsed(1)
+    event test
+    do parallel:
+        serial:
+            wait elapsed(1s)
+            emit test
+            wait elapsed(10s)
+            emit fail
+        serial:
+            wait @test
+            emit end
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
-
-        model = create_py_tree(model, self.parser.logger, False)
-        self.assertIsNone(model)
+        scenarios = create_py_tree(model, self.parser.logger, False)
+        self.scenario_execution.scenarios = scenarios
+        self.scenario_execution.run()
+        self.assertTrue(self.scenario_execution.process_results())
```

### Comparing `scenario-execution-1.0.0/test/test_osc2_standard_osc.py` & `scenario_execution-1.1.0/test/test_osc2_parser_event.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,39 +11,48 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
-Test standard.osc parsing
+Test event parsing
 """
 import unittest
-
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
-class TestOSC2Parser(unittest.TestCase):
+class TestScenarioExectionSuccess(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
 
     def setUp(self) -> None:
         self.parser = OpenScenario2Parser(Logger('test', False))
 
-    def test_standard_osc(self):
+    def test_unknown_event(self):
+        scenario_content = """
+scenario test:
+    do serial:
+        emit UNKNOWN
+"""
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
+        self.assertRaises(ValueError, self.parser.create_internal_model, parsed_tree, "test.osc", True)
+
+    def test_event_success(self):
         scenario_content = """
-import osc.standard
+scenario test:
+    event test1
+    do serial:
+        emit test1
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
 
-    def test_standard_common_osc(self):
+    def test_event_end(self):
         scenario_content = """
-import osc.standard.base
+scenario test:
+    do serial:
+        emit end
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
```

### Comparing `scenario-execution-1.0.0/test/test_run_process.py` & `scenario_execution-1.1.0/test/test_run_process.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import unittest
 import rclpy
-from scenario_execution_base import ScenarioExecution
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.model.model_to_py_tree import create_py_tree
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution import ScenarioExecution
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.model.model_to_py_tree import create_py_tree
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestScenarioExecutionSuccess(unittest.TestCase):
     # pylint: disable=missing-function-docstring
 
     def setUp(self) -> None:
@@ -49,23 +49,20 @@
             run_process() with:
                 keep(it.command == 'false')
             emit end
         time_out: serial:
             wait elapsed(10s)
             time_out_shutdown: emit fail
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", False)
-        self.assertIsNotNone(model)
         scenarios = create_py_tree(model, self.parser.logger, False)
-        self.assertIsNotNone(scenarios)
         self.scenario_execution.scenarios = scenarios
-        ret = self.scenario_execution.run()
-        self.assertFalse(ret)
+        self.scenario_execution.run()
+        self.assertFalse(self.scenario_execution.process_results())
 
     def test_success(self):
         scenario_content = """
 import osc.standard.base
 import osc.helpers
 
 scenario test_run_process:
@@ -74,23 +71,20 @@
             run_process() with:
                 keep(it.command == 'true')
             emit end
         time_out: serial:
             wait elapsed(10s)
             time_out_shutdown: emit fail
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
         scenarios = create_py_tree(model, self.parser.logger, False)
-        self.assertIsNotNone(scenarios)
         self.scenario_execution.scenarios = scenarios
-        ret = self.scenario_execution.run()
-        self.assertTrue(ret)
+        self.scenario_execution.run()
+        self.assertTrue(self.scenario_execution.process_results())
 
     def test_multi_element_command(self):
         scenario_content = """
 import osc.standard.base
 import osc.helpers
 
 scenario test_run_process:
@@ -98,16 +92,13 @@
         serial:
             run_process('sleep 2')
             emit end
         time_out: serial:
             wait elapsed(10s)
             time_out_shutdown: emit fail
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
         scenarios = create_py_tree(model, self.parser.logger, False)
-        self.assertIsNotNone(scenarios)
         self.scenario_execution.scenarios = scenarios
-        ret = self.scenario_execution.run()
-        self.assertTrue(ret)
+        self.scenario_execution.run()
+        self.assertTrue(self.scenario_execution.process_results())
```

### Comparing `scenario-execution-1.0.0/test/test_scenario_execution.py` & `scenario_execution-1.1.0/test/test_scenario_execution.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,57 +12,66 @@
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import unittest
 import os
-from scenario_execution_base.scenario_execution import ScenarioExecution
+from scenario_execution.scenario_execution_base import ScenarioExecution
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
 
     def test_scenario_file_not_existing(self):
         scenario_execution = ScenarioExecution(debug=False,
                                                log_model=False,
                                                live_tree=False,
                                                scenario_file='UNKNOWN_FILE.sce',
                                                output_dir="")
         result = scenario_execution.parse()
         self.assertFalse(result)
+        self.assertEqual(len(scenario_execution.results), 1)
+        self.assertEqual(scenario_execution.results[0].result, False)
 
     def test_scenario_file_wrong_extension(self):
         scenario_execution = ScenarioExecution(debug=False,
                                                log_model=False,
                                                live_tree=False,
                                                scenario_file='UNKNOWN_FILE',
                                                output_dir="")
         result = scenario_execution.parse()
         self.assertFalse(result)
+        self.assertEqual(len(scenario_execution.results), 1)
+        self.assertEqual(scenario_execution.results[0].result, False)
 
     def test_no_scenario(self):
         scenario_execution = ScenarioExecution(debug=False,
                                                log_model=False,
                                                live_tree=False,
                                                scenario_file=os.path.join(os.path.dirname(__file__), 'scenarios', 'no_scenario.osc'),
                                                output_dir="")
         result = scenario_execution.parse()
         self.assertFalse(result)
+        self.assertEqual(len(scenario_execution.results), 1)
+        self.assertEqual(scenario_execution.results[0].result, False)
 
     def test_scenario(self):
         scenario_execution = ScenarioExecution(debug=False,
                                                log_model=False,
                                                live_tree=False,
                                                scenario_file=os.path.join(os.path.dirname(__file__), 'scenarios', 'test_scenario.osc'),
                                                output_dir="")
         result = scenario_execution.parse()
         self.assertTrue(result)
+        self.assertEqual(len(scenario_execution.results), 0)  # not yet executed
 
     def test_two_scenarios(self):
         scenario_execution = ScenarioExecution(debug=False,
                                                log_model=False,
                                                live_tree=False,
                                                scenario_file=os.path.join(os.path.dirname(__file__), 'scenarios', 'two_scenarios.osc'),
                                                output_dir="")
         result = scenario_execution.parse()
         self.assertFalse(result)
+        self.assertEqual(len(scenario_execution.results), 1)
+        self.assertEqual(scenario_execution.results[0].result, False)
```

### Comparing `scenario-execution-1.0.0/test/test_scenario_oneof.py` & `scenario_execution-1.1.0/test/test_scenario_parallel.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,53 +11,50 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
-Test oneof parsing
+Test parallel parsing
 """
 import unittest
-from datetime import datetime
 
-from scenario_execution_base.scenario_execution import ScenarioExecution
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.model.model_to_py_tree import create_py_tree
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.scenario_execution_base import ScenarioExecution
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.model.model_to_py_tree import create_py_tree
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
+    """
+    Unit test for osc2_parser
+    """
 
     def setUp(self) -> None:
         self.parser = OpenScenario2Parser(Logger('test', False))
         self.scenario_execution = ScenarioExecution(debug=True, log_model=True, live_tree=True, scenario_file='test.osc', output_dir="")
 
-    def test_oneof(self):
+    def test_parallel(self):
         scenario_content = """
 type time is SI(s: 1)
 unit s          of time is SI(s: 1, factor: 1)
 
 scenario test:
     do serial:
-        one_of:
-            wait elapsed(120s)
-            wait elapsed(5s)
-        emit end        
+        parallel:
+            serial:
+                wait elapsed(5s)
+                emit end
+            serial:
+                wait elapsed(1s)
+        wait elapsed(1s)
+        emit fail
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
         scenarios = create_py_tree(model, self.parser.logger, False)
-        self.assertIsNotNone(scenarios)
         self.scenario_execution.scenarios = scenarios
-
-        start_time = datetime.now()
-        ret = self.scenario_execution.run()
-        end_time = datetime.now()
-        self.assertTrue(ret)
-
-        delta = end_time - start_time
-        self.assertLess(delta.total_seconds(), 15.)
+        self.scenario_execution.run()
+        self.assertTrue(self.scenario_execution.process_results())
```

### Comparing `scenario-execution-1.0.0/test/test_scenario_parallel.py` & `scenario_execution-1.1.0/test/test_scenario_oneof.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,53 +11,50 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
-Test parallel parsing
+Test oneof parsing
 """
 import unittest
+from datetime import datetime
 
-from scenario_execution_base.scenario_execution import ScenarioExecution
-from scenario_execution_base.model.osc2_parser import OpenScenario2Parser
-from scenario_execution_base.model.model_to_py_tree import create_py_tree
-from scenario_execution_base.utils.logging import Logger
+from scenario_execution.scenario_execution_base import ScenarioExecution
+from scenario_execution.model.osc2_parser import OpenScenario2Parser
+from scenario_execution.model.model_to_py_tree import create_py_tree
+from scenario_execution.utils.logging import Logger
 from antlr4.InputStream import InputStream
 
 
 class TestOSC2Parser(unittest.TestCase):
     # pylint: disable=missing-function-docstring, protected-access, no-member, unused-variable
-    """
-    Unit test for osc2_parser
-    """
 
     def setUp(self) -> None:
         self.parser = OpenScenario2Parser(Logger('test', False))
         self.scenario_execution = ScenarioExecution(debug=True, log_model=True, live_tree=True, scenario_file='test.osc', output_dir="")
 
-    def test_parallel(self):
+    def test_oneof(self):
         scenario_content = """
 type time is SI(s: 1)
 unit s          of time is SI(s: 1, factor: 1)
 
 scenario test:
     do serial:
-        parallel:
-            serial:
-                wait elapsed(5s)
-                emit end
-            serial:
-                wait elapsed(1s)
-        wait elapsed(1s)
-        emit fail             
+        one_of:
+            wait elapsed(120s)
+            wait elapsed(5s)
+        emit end
 """
-        parsed_tree, errors = self.parser.parse_input_stream(InputStream(scenario_content))
-        self.assertEqual(errors, 0)
+        parsed_tree = self.parser.parse_input_stream(InputStream(scenario_content))
         model = self.parser.create_internal_model(parsed_tree, "test.osc", True)
-        self.assertIsNotNone(model)
         scenarios = create_py_tree(model, self.parser.logger, False)
-        self.assertIsNotNone(scenarios)
         self.scenario_execution.scenarios = scenarios
-        ret = self.scenario_execution.run()
-        self.assertTrue(ret)
+
+        start_time = datetime.now()
+        self.scenario_execution.run()
+        end_time = datetime.now()
+        self.assertTrue(self.scenario_execution.process_results())
+
+        delta = end_time - start_time
+        self.assertLess(delta.total_seconds(), 15.)
```

