# Comparing `tmp/angr-management-9.2.96.tar.gz` & `tmp/angr-management-9.2.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angr-management-9.2.96.tar", last modified: Tue Mar 26 17:02:38 2024, max compression
+gzip compressed data, was "angr-management-9.2.97.tar", last modified: Tue Apr  2 17:03:02 2024, max compression
```

## Comparing `angr-management-9.2.96.tar` & `angr-management-9.2.97.tar`

### file list

```diff
@@ -1,391 +1,402 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.357464 angr-management-9.2.96/
--rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-03-26 17:01:00.000000 angr-management-9.2.96/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     4827 2024-03-26 17:02:38.357464 angr-management-9.2.96/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3414 2024-03-26 17:01:00.000000 angr-management-9.2.96/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.353464 angr-management-9.2.96/angr_management.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     4827 2024-03-26 17:02:38.000000 angr-management-9.2.96/angr_management.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    14740 2024-03-26 17:02:38.000000 angr-management-9.2.96/angr_management.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-26 17:02:38.000000 angr-management-9.2.96/angr_management.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-26 17:02:38.000000 angr-management-9.2.96/angr_management.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      509 2024-03-26 17:02:38.000000 angr-management-9.2.96/angr_management.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-03-26 17:02:38.000000 angr-management-9.2.96/angr_management.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.277464 angr-management-9.2.96/angrmanagement/
--rw-r--r--   0 vsts      (1001) docker     (127)      270 2024-03-26 17:01:08.000000 angr-management-9.2.96/angrmanagement/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8451 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.281464 angr-management-9.2.96/angrmanagement/config/
--rw-r--r--   0 vsts      (1001) docker     (127)     1586 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27335 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/config/color_schemes.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/config/config_entry.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26486 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/config/config_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.281464 angr-management-9.2.96/angrmanagement/daemon/
--rw-r--r--   0 vsts      (1001) docker     (127)      775 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/daemon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2561 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/daemon/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5051 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/daemon/server.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5168 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/daemon/url_handler.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.281464 angr-management-9.2.96/angrmanagement/data/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11400 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/analysis_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2102 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/breakpoint.py
--rw-r--r--   0 vsts      (1001) docker     (127)      962 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/function_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)      267 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/highlight_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/indirect_jump.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14536 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/instance.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.285465 angr-management-9.2.96/angrmanagement/data/jobs/
--rw-r--r--   0 vsts      (1001) docker     (127)      903 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3470 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/cfg_generation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      704 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/code_tagging.py
--rw-r--r--   0 vsts      (1001) docker     (127)      637 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/ddg_generation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/decompile_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10957 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/dependency_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)      893 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/flirt_signature_recognition.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3628 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/job.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6291 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/loading.py
--rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/prototype_finding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1511 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/simgr_explore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1397 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/simgr_step.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3821 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/variable_recovery.py
--rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/jobs/vfg_generation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1882 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/library_docs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3019 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/log.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3838 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/object_container.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4417 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/tagged_interval_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1179 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/data/trace.py
--rw-r--r--   0 vsts      (1001) docker     (127)      306 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.285465 angr-management-9.2.96/angrmanagement/logic/
--rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.285465 angr-management-9.2.96/angrmanagement/logic/commands/
--rw-r--r--   0 vsts      (1001) docker     (127)      227 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2056 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/commands/command.py
--rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/commands/command_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.289465 angr-management-9.2.96/angrmanagement/logic/debugger/
--rw-r--r--   0 vsts      (1001) docker     (127)      226 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/debugger/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10828 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/debugger/bintrace.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5926 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/debugger/debugger.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3060 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/debugger/simgr.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.289465 angr-management-9.2.96/angrmanagement/logic/disassembly/
--rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/disassembly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13363 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/disassembly/info_dock.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/disassembly/jump_history.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5466 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/singleton.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7675 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/threads.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5658 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/logic/url_scheme.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.289465 angr-management-9.2.96/angrmanagement/plugins/
--rw-r--r--   0 vsts      (1001) docker     (127)     1110 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.289465 angr-management-9.2.96/angrmanagement/plugins/ail2asm/
--rw-r--r--   0 vsts      (1001) docker     (127)       94 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/ail2asm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10345 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/ail2asm/ail2arm32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1381 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/ail2asm/asm_output.py
--rw-r--r--   0 vsts      (1001) docker     (127)      262 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/ail2asm/plugin.toml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.293465 angr-management-9.2.96/angrmanagement/plugins/angr_binsync/
--rw-r--r--   0 vsts      (1001) docker     (127)      124 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/angr_binsync/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      271 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/angr_binsync/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     7399 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/base_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.293465 angr-management-9.2.96/angrmanagement/plugins/coverage/
--rw-r--r--   0 vsts      (1001) docker     (127)      103 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/coverage/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9825 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/coverage/coverage.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4676 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/coverage/parse_trace.py
--rw-r--r--   0 vsts      (1001) docker     (127)      283 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/coverage/plugin.toml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.293465 angr-management-9.2.96/angrmanagement/plugins/decompiler_poison/
--rw-r--r--   0 vsts      (1001) docker     (127)     6073 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/decompiler_poison/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      294 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/decompiler_poison/plugin.toml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.293465 angr-management-9.2.96/angrmanagement/plugins/dep_viewer/
--rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/dep_viewer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1973 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/dep_viewer/dep_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      289 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/dep_viewer/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     2797 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/dep_viewer/sinks.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.293465 angr-management-9.2.96/angrmanagement/plugins/execution_statistics_viewer/
--rw-r--r--   0 vsts      (1001) docker     (127)      151 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/execution_statistics_viewer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5389 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/execution_statistics_viewer/execution_statistics_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      316 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/execution_statistics_viewer/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     3852 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/load.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.293465 angr-management-9.2.96/angrmanagement/plugins/memory_checker/
--rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/memory_checker/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/memory_checker/memory_checker.py
--rw-r--r--   0 vsts      (1001) docker     (127)      287 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/memory_checker/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     3998 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/plugin_description.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22658 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/plugin_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.297464 angr-management-9.2.96/angrmanagement/plugins/precise_diffing/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/precise_diffing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      841 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/precise_diffing/diff_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11585 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/precise_diffing/function_diff.py
--rw-r--r--   0 vsts      (1001) docker     (127)      294 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/precise_diffing/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     6850 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/precise_diffing/precisediff_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7279 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/precise_diffing/settings_dialog.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1092 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/sample_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.297464 angr-management-9.2.96/angrmanagement/plugins/source_importer/
--rw-r--r--   0 vsts      (1001) docker     (127)     1642 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/source_importer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      283 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/source_importer/plugin.toml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.297464 angr-management-9.2.96/angrmanagement/plugins/source_viewer/
--rw-r--r--   0 vsts      (1001) docker     (127)      130 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/source_viewer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      291 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/source_viewer/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)    10729 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/source_viewer/source_viewer_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.297464 angr-management-9.2.96/angrmanagement/plugins/trace_viewer/
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/trace_viewer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8589 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/trace_viewer/afl_qemu_bitmap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4677 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/trace_viewer/multi_trace.py
--rw-r--r--   0 vsts      (1001) docker     (127)      304 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/trace_viewer/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)    19741 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/trace_viewer/qtrace_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14564 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/trace_viewer/trace_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9407 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/trace_viewer/trace_statistics.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.301464 angr-management-9.2.96/angrmanagement/plugins/value_search/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/value_search/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1030 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/value_search/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/value_search/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     6636 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/value_search/qsearch_table.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4714 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/value_search/search_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4106 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/value_search/value_search_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.301464 angr-management-9.2.96/angrmanagement/plugins/varec/
--rw-r--r--   0 vsts      (1001) docker     (127)       82 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/varec/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      286 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/varec/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     6570 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/plugins/varec/varec.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.269465 angr-management-9.2.96/angrmanagement/resources/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.301464 angr-management-9.2.96/angrmanagement/resources/fonts/
--rw-r--r--   0 vsts      (1001) docker     (127)   340712 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/fonts/DejaVuSansMono.ttf
--rw-r--r--   0 vsts      (1001) docker     (127)   212880 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/fonts/SourceCodePro-Regular.ttf
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.305464 angr-management-9.2.96/angrmanagement/resources/images/
--rw-r--r--   0 vsts      (1001) docker     (127)   100896 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/angr-ds.png
--rw-r--r--   0 vsts      (1001) docker     (127)   143434 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/angr-splash.png
--rw-r--r--   0 vsts      (1001) docker     (127)   165662 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/angr.ico
--rw-r--r--   0 vsts      (1001) docker     (127)    79574 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/angr.png
--rw-r--r--   0 vsts      (1001) docker     (127)    11090 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/benchmark-icon.png
--rw-r--r--   0 vsts      (1001) docker     (127)     9627 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/error-icon.png
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/run-icon.svg
--rw-r--r--   0 vsts      (1001) docker     (127)     9671 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/toolbar-docker-open.png
--rw-r--r--   0 vsts      (1001) docker     (127)   176067 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/toolbar-file-open.ico
--rw-r--r--   0 vsts      (1001) docker     (127)   103065 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/toolbar-file-save.png
--rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/toolbar-forward.png
--rw-r--r--   0 vsts      (1001) docker     (127)     1200 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/toolbar-previous.png
--rw-r--r--   0 vsts      (1001) docker     (127)     1891 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/toolbar-show-alignment.png
--rw-r--r--   0 vsts      (1001) docker     (127)    25190 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/images/warning-icon.png
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.305464 angr-management-9.2.96/angrmanagement/resources/themes/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.305464 angr-management-9.2.96/angrmanagement/resources/themes/Catppuccin Mocha/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.305464 angr-management-9.2.96/angrmanagement/resources/themes/Catppuccin Mocha/images/
--rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Catppuccin Mocha/images/close.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      185 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Catppuccin Mocha/images/provenance.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Catppuccin Mocha/images/tab-menu.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      385 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Catppuccin Mocha/theme.css
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.305464 angr-management-9.2.96/angrmanagement/resources/themes/Dark/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.309464 angr-management-9.2.96/angrmanagement/resources/themes/Dark/images/
--rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Dark/images/close.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      133 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Dark/images/provenance.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Dark/images/tab-menu.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      385 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Dark/theme.css
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.309464 angr-management-9.2.96/angrmanagement/resources/themes/Dracula/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.309464 angr-management-9.2.96/angrmanagement/resources/themes/Dracula/images/
--rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Dracula/images/close.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      185 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Dracula/images/provenance.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Dracula/images/tab-menu.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      385 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Dracula/theme.css
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.273465 angr-management-9.2.96/angrmanagement/resources/themes/Light/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.309464 angr-management-9.2.96/angrmanagement/resources/themes/Light/images/
--rw-r--r--   0 vsts      (1001) docker     (127)      694 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Light/images/close.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      133 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Light/images/provenance.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/Light/images/tab-menu.svg
--rw-r--r--   0 vsts      (1001) docker     (127)     3429 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/resources/themes/base.css
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.309464 angr-management-9.2.96/angrmanagement/ui/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3837 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/awesome_tooltip_event_filter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.309464 angr-management-9.2.96/angrmanagement/ui/css/
--rw-r--r--   0 vsts      (1001) docker     (127)     4136 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/css/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.317464 angr-management-9.2.96/angrmanagement/ui/dialogs/
--rw-r--r--   0 vsts      (1001) docker     (127)      512 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1952 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/about.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11010 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/analysis_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6536 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/assemble_patch.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4888 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/breakpoint.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9795 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/command_palette.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5124 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/data_dep_graph_search.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6179 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/dependson.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2528 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/env_config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1026 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/fs_mount.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1939 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/func_doc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5309 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4762 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/hook.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1727 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/input_prompt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2641 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/jumpto.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19381 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/load_binary.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1479 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/load_docker_prompt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4287 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/load_plugins.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15342 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/new_state.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10062 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/preferences.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3441 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/rename.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4003 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/rename_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9608 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/rename_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6459 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/retype_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2973 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/set_comment.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11317 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/socket_config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5913 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/type_editor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3416 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/welcome.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2786 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/dialogs/xref.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.317464 angr-management-9.2.96/angrmanagement/ui/documents/
--rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/documents/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5999 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/documents/qcodedocument.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1129 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/icons.py
--rw-r--r--   0 vsts      (1001) docker     (127)    37441 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/main_window.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.321464 angr-management-9.2.96/angrmanagement/ui/menus/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/menus/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1340 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/menus/analyze_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4251 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/menus/disasm_insn_context_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2733 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/menus/disasm_label_context_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2575 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/menus/disasm_options_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3489 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/menus/file_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1086 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/menus/function_context_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      820 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/menus/help_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/menus/log_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5225 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/menus/menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      508 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/menus/plugin_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6044 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/menus/view_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2178 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/toolbar_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.321464 angr-management-9.2.96/angrmanagement/ui/toolbars/
--rw-r--r--   0 vsts      (1001) docker     (127)      383 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/toolbars/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9051 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/toolbars/debug_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2072 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/toolbars/feature_map_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1313 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/toolbars/file_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/toolbars/function_table_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3576 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/toolbars/nav_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2556 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/toolbars/toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)      651 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/toolbars/toolbar_action.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2483 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/toolbars/toolbar_dock.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7373 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/view_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.325464 angr-management-9.2.96/angrmanagement/ui/views/
--rw-r--r--   0 vsts      (1001) docker     (127)     1317 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5973 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/breakpoints_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6366 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/call_explorer_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21141 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/code_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3678 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/console_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9776 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/data_dep_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4635 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/dep_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)    38085 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/disassembly_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2314 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/functions_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)    72410 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/hex_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18109 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/interaction_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1233 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/log_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1149 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/patches_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6239 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/proximity_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5257 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/registers_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6067 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/stack_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1524 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/states_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4112 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/strings_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4826 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/symexec_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1229 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/trace_map_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4809 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/traces_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5009 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/types_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9710 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/views/view.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.345464 angr-management-9.2.96/angrmanagement/ui/widgets/
--rw-r--r--   0 vsts      (1001) docker     (127)      987 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2435 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/filesystem_table.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1523 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qaddress_input.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6119 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qast_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14284 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qblock.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25547 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qblock_code.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2199 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qblock_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24425 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qccode_edit.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10063 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qccode_highlighter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1494 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qcolor_option.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2095 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qconstraint_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10223 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qdatadep_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7110 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qdatadepgraph_block.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9805 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qdecomp_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4447 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qdep_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7674 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qdepgraph_block.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3715 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qdisasm_base_control.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12665 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qdisasm_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4831 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qdisasm_statusbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26979 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qfeature_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2833 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qfiledesc_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qfont_option.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1934 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qfunction_combobox.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5922 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qfunction_header.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20238 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qfunction_table.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11772 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qgraph.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11714 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qgraph_arrow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1214 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qgraph_object.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1080 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qicon_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9249 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qinst_annotation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11637 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qinstruction.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1753 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qipython_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20717 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qlinear_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8606 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qlog_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9752 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qmemory_data_block.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5488 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qmemory_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9628 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qminimap.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19882 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qoperand.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4982 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qpatch_table.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4671 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qpathtree.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5187 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qphivariable.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5100 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qproximity_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12132 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qproximitygraph_block.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5600 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qregister_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9769 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qsimulation_manager_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12162 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qsimulation_managers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5464 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qstate_block.py
--rw-r--r--   0 vsts      (1001) docker     (127)      909 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qstate_combobox.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6199 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qstate_table.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8582 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qstring_table.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4799 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qsymexec_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15555 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qtrace_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4544 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qtypedef.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3480 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qunknown_block.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4278 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qvariable.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2417 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qvextemps_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10602 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/qxref_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1721 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/widgets/state_inspector.py
--rw-r--r--   0 vsts      (1001) docker     (127)    38264 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/ui/workspace.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.345464 angr-management-9.2.96/angrmanagement/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     8191 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      757 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/block_objects.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3562 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/cfg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      357 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/daemon_thread.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1655 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2387 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/env.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1314 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/func.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11456 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30785 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/graph_layouter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2451 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/io.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/layout.py
--rw-r--r--   0 vsts      (1001) docker     (127)      672 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/monkeypatch_stdio.py
--rw-r--r--   0 vsts      (1001) docker     (127)    42616 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/namegen.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11676 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/utils/tree_graph_layouter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.349464 angr-management-9.2.96/angrmanagement/vendor/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.353464 angr-management-9.2.96/angrmanagement/vendor/qtconsole/
--rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       73 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       72 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/_version.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14176 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/ansi_code_processor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6295 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/base_frontend_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3733 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/bracket_matcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10683 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/call_tip_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1971 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8839 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/comms.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12909 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/completion_html.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2234 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/completion_plain.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8151 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/completion_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)   104717 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/console_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34810 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/frontend_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9947 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/history_console_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2874 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/inprocess.py
--rw-r--r--   0 vsts      (1001) docker     (127)      169 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/ipython_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24994 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/jupyter_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1813 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/kernel_mixins.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3793 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/kill_ring.py
--rw-r--r--   0 vsts      (1001) docker     (127)    38376 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/mainwindow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2602 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9110 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/pygments_highlighter.py
--rw-r--r--   0 vsts      (1001) docker     (127)      540 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/qstringhelpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17176 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/qtconsoleapp.py
--rw-r--r--   0 vsts      (1001) docker     (127)      184 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/rich_ipython_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18469 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/rich_jupyter_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8638 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/rich_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3801 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/styles.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/svg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8349 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8354 2024-03-26 17:01:00.000000 angr-management-9.2.96/angrmanagement/vendor/qtconsole/util.py
--rw-r--r--   0 vsts      (1001) docker     (127)      596 2024-03-26 17:01:08.000000 angr-management-9.2.96/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1365 2024-03-26 17:02:38.357464 angr-management-9.2.96/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:38.353464 angr-management-9.2.96/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)     2053 2024-03-26 17:01:00.000000 angr-management-9.2.96/tests/test_qaddress_input.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5241 2024-03-26 17:01:00.000000 angr-management-9.2.96/tests/test_rename_functions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3681 2024-03-26 17:01:00.000000 angr-management-9.2.96/tests/test_rename_variables.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3487 2024-03-26 17:01:00.000000 angr-management-9.2.96/tests/test_tagged_interval_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)      873 2024-03-26 17:01:00.000000 angr-management-9.2.96/tests/test_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.278512 angr-management-9.2.97/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-04-02 17:01:37.000000 angr-management-9.2.97/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     4826 2024-04-02 17:03:02.278512 angr-management-9.2.97/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3414 2024-04-02 17:01:37.000000 angr-management-9.2.97/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.274512 angr-management-9.2.97/angr_management.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4826 2024-04-02 17:03:02.000000 angr-management-9.2.97/angr_management.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    15408 2024-04-02 17:03:02.000000 angr-management-9.2.97/angr_management.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-02 17:03:02.000000 angr-management-9.2.97/angr_management.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-02 17:03:02.000000 angr-management-9.2.97/angr_management.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      508 2024-04-02 17:03:02.000000 angr-management-9.2.97/angr_management.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-04-02 17:03:02.000000 angr-management-9.2.97/angr_management.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.190512 angr-management-9.2.97/angrmanagement/
+-rw-r--r--   0 vsts      (1001) docker     (127)      270 2024-04-02 17:01:44.000000 angr-management-9.2.97/angrmanagement/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8451 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.190512 angr-management-9.2.97/angrmanagement/config/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1586 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27335 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/config/color_schemes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/config/config_entry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26486 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/config/config_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.194512 angr-management-9.2.97/angrmanagement/daemon/
+-rw-r--r--   0 vsts      (1001) docker     (127)      775 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/daemon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2561 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/daemon/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5051 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/daemon/server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5168 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/daemon/url_handler.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.198512 angr-management-9.2.97/angrmanagement/data/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11400 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/analysis_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2102 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/breakpoint.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      962 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/function_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      267 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/highlight_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/indirect_jump.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14536 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/instance.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.202512 angr-management-9.2.97/angrmanagement/data/jobs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      903 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3470 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/cfg_generation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      704 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/code_tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      637 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/ddg_generation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/decompile_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10957 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/dependency_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      893 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/flirt_signature_recognition.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3628 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/job.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6291 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/loading.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/prototype_finding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1511 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/simgr_explore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1397 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/simgr_step.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3821 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/variable_recovery.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/jobs/vfg_generation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1882 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/library_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3019 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3838 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/object_container.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4417 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/tagged_interval_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1179 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/data/trace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      306 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.202512 angr-management-9.2.97/angrmanagement/logic/
+-rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.202512 angr-management-9.2.97/angrmanagement/logic/commands/
+-rw-r--r--   0 vsts      (1001) docker     (127)      227 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2056 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/commands/command.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/commands/command_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.206512 angr-management-9.2.97/angrmanagement/logic/debugger/
+-rw-r--r--   0 vsts      (1001) docker     (127)      226 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/debugger/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10828 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/debugger/bintrace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5926 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/debugger/debugger.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3060 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/debugger/simgr.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.210512 angr-management-9.2.97/angrmanagement/logic/disassembly/
+-rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/disassembly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13363 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/disassembly/info_dock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/disassembly/jump_history.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5466 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/singleton.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7675 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/threads.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5658 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/logic/url_scheme.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.210512 angr-management-9.2.97/angrmanagement/plugins/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1110 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.214512 angr-management-9.2.97/angrmanagement/plugins/ail2asm/
+-rw-r--r--   0 vsts      (1001) docker     (127)       94 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/ail2asm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10345 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/ail2asm/ail2arm32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1381 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/ail2asm/asm_output.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      262 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/ail2asm/plugin.toml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.214512 angr-management-9.2.97/angrmanagement/plugins/angr_binsync/
+-rw-r--r--   0 vsts      (1001) docker     (127)      124 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/angr_binsync/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      271 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/angr_binsync/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     7399 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/base_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.214512 angr-management-9.2.97/angrmanagement/plugins/coverage/
+-rw-r--r--   0 vsts      (1001) docker     (127)      103 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/coverage/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9825 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/coverage/coverage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4676 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/coverage/parse_trace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      283 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/coverage/plugin.toml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.214512 angr-management-9.2.97/angrmanagement/plugins/decompiler_poison/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6073 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/decompiler_poison/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      294 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/decompiler_poison/plugin.toml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.218512 angr-management-9.2.97/angrmanagement/plugins/dep_viewer/
+-rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/dep_viewer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1973 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/dep_viewer/dep_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      289 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/dep_viewer/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     2797 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/dep_viewer/sinks.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.218512 angr-management-9.2.97/angrmanagement/plugins/execution_statistics_viewer/
+-rw-r--r--   0 vsts      (1001) docker     (127)      151 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/execution_statistics_viewer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5389 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/execution_statistics_viewer/execution_statistics_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      316 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/execution_statistics_viewer/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     3852 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/load.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.218512 angr-management-9.2.97/angrmanagement/plugins/memory_checker/
+-rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/memory_checker/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/memory_checker/memory_checker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      287 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/memory_checker/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     3998 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/plugin_description.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22658 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/plugin_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.218512 angr-management-9.2.97/angrmanagement/plugins/precise_diffing/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/precise_diffing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      841 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/precise_diffing/diff_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11585 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/precise_diffing/function_diff.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      294 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/precise_diffing/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     6850 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/precise_diffing/precisediff_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7279 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/precise_diffing/settings_dialog.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1092 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/sample_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.218512 angr-management-9.2.97/angrmanagement/plugins/source_importer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1642 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/source_importer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      283 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/source_importer/plugin.toml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.218512 angr-management-9.2.97/angrmanagement/plugins/source_viewer/
+-rw-r--r--   0 vsts      (1001) docker     (127)      130 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/source_viewer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      291 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/source_viewer/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)    10729 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/source_viewer/source_viewer_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.222512 angr-management-9.2.97/angrmanagement/plugins/trace_viewer/
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/trace_viewer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8589 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/trace_viewer/afl_qemu_bitmap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4677 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/trace_viewer/multi_trace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      304 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/trace_viewer/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)    19741 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/trace_viewer/qtrace_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14564 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/trace_viewer/trace_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9407 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/trace_viewer/trace_statistics.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.222512 angr-management-9.2.97/angrmanagement/plugins/value_search/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/value_search/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1030 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/value_search/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/value_search/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     6636 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/value_search/qsearch_table.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4714 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/value_search/search_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4106 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/value_search/value_search_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.222512 angr-management-9.2.97/angrmanagement/plugins/varec/
+-rw-r--r--   0 vsts      (1001) docker     (127)       82 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/varec/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      286 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/varec/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     6570 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/plugins/varec/varec.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.182512 angr-management-9.2.97/angrmanagement/resources/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.222512 angr-management-9.2.97/angrmanagement/resources/fonts/
+-rw-r--r--   0 vsts      (1001) docker     (127)   340712 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/fonts/DejaVuSansMono.ttf
+-rw-r--r--   0 vsts      (1001) docker     (127)   212880 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/fonts/SourceCodePro-Regular.ttf
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.230512 angr-management-9.2.97/angrmanagement/resources/images/
+-rw-r--r--   0 vsts      (1001) docker     (127)   100896 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/angr-ds.png
+-rw-r--r--   0 vsts      (1001) docker     (127)   143434 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/angr-splash.png
+-rw-r--r--   0 vsts      (1001) docker     (127)   165662 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/angr.ico
+-rw-r--r--   0 vsts      (1001) docker     (127)    79574 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/angr.png
+-rw-r--r--   0 vsts      (1001) docker     (127)    11090 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/benchmark-icon.png
+-rw-r--r--   0 vsts      (1001) docker     (127)     9627 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/error-icon.png
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/run-icon.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     9671 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/toolbar-docker-open.png
+-rw-r--r--   0 vsts      (1001) docker     (127)   176067 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/toolbar-file-open.ico
+-rw-r--r--   0 vsts      (1001) docker     (127)   103065 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/toolbar-file-save.png
+-rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/toolbar-forward.png
+-rw-r--r--   0 vsts      (1001) docker     (127)     1200 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/toolbar-previous.png
+-rw-r--r--   0 vsts      (1001) docker     (127)     1891 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/toolbar-show-alignment.png
+-rw-r--r--   0 vsts      (1001) docker     (127)    25190 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/images/warning-icon.png
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.230512 angr-management-9.2.97/angrmanagement/resources/themes/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.230512 angr-management-9.2.97/angrmanagement/resources/themes/Catppuccin Mocha/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.230512 angr-management-9.2.97/angrmanagement/resources/themes/Catppuccin Mocha/images/
+-rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Catppuccin Mocha/images/close.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Catppuccin Mocha/images/drawing-pin.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Catppuccin Mocha/images/minimize-button.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      416 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Catppuccin Mocha/images/provenance.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Catppuccin Mocha/images/tab-menu.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      500 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Catppuccin Mocha/theme.css
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.230512 angr-management-9.2.97/angrmanagement/resources/themes/Dark/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.230512 angr-management-9.2.97/angrmanagement/resources/themes/Dark/images/
+-rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Dark/images/close.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Dark/images/drawing-pin.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Dark/images/minimize-button.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      363 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Dark/images/provenance.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Dark/images/tab-menu.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      500 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Dark/theme.css
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.230512 angr-management-9.2.97/angrmanagement/resources/themes/Dracula/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.234512 angr-management-9.2.97/angrmanagement/resources/themes/Dracula/images/
+-rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Dracula/images/close.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Dracula/images/drawing-pin.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Dracula/images/minimize-button.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      415 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Dracula/images/provenance.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Dracula/images/tab-menu.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      500 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Dracula/theme.css
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.234512 angr-management-9.2.97/angrmanagement/resources/themes/Light/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.234512 angr-management-9.2.97/angrmanagement/resources/themes/Light/images/
+-rw-r--r--   0 vsts      (1001) docker     (127)      694 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Light/images/close.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Light/images/drawing-pin-light.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1006 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Light/images/drawing-pin.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Light/images/minimize-button.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      337 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Light/images/provenance.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Light/images/tab-menu.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/Light/theme.css
+-rw-r--r--   0 vsts      (1001) docker     (127)     7502 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/resources/themes/base.css
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.234512 angr-management-9.2.97/angrmanagement/ui/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3837 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/awesome_tooltip_event_filter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.234512 angr-management-9.2.97/angrmanagement/ui/css/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4136 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/css/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.242512 angr-management-9.2.97/angrmanagement/ui/dialogs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      512 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1952 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/about.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11010 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/analysis_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6536 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/assemble_patch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4888 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/breakpoint.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9795 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/command_palette.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5124 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/data_dep_graph_search.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6179 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/dependson.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2528 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/env_config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1026 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/fs_mount.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1939 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/func_doc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5309 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4762 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/hook.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1727 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/input_prompt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2641 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/jumpto.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19381 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/load_binary.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1479 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/load_docker_prompt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4287 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/load_plugins.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15342 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/new_state.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10062 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/preferences.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3441 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/rename.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4003 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/rename_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9608 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/rename_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6459 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/retype_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2973 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/set_comment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11317 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/socket_config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5913 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/type_editor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3416 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/welcome.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2786 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/dialogs/xref.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.242512 angr-management-9.2.97/angrmanagement/ui/documents/
+-rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/documents/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5999 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/documents/qcodedocument.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1129 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/icons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    37584 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/main_window.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.246512 angr-management-9.2.97/angrmanagement/ui/menus/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/menus/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1340 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/menus/analyze_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4251 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/menus/disasm_insn_context_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2733 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/menus/disasm_label_context_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2575 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/menus/disasm_options_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3489 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/menus/file_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1086 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/menus/function_context_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      820 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/menus/help_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/menus/log_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5225 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/menus/menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      508 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/menus/plugin_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6044 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/menus/view_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2178 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/toolbar_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.246512 angr-management-9.2.97/angrmanagement/ui/toolbars/
+-rw-r--r--   0 vsts      (1001) docker     (127)      383 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/toolbars/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9051 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/toolbars/debug_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2072 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/toolbars/feature_map_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1313 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/toolbars/file_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/toolbars/function_table_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3576 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/toolbars/nav_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2556 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/toolbars/toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      651 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/toolbars/toolbar_action.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2483 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/toolbars/toolbar_dock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7437 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/view_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.254512 angr-management-9.2.97/angrmanagement/ui/views/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1317 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5973 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/breakpoints_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6366 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/call_explorer_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21141 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/code_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3678 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/console_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9781 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/data_dep_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4635 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/dep_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    38085 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/disassembly_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2314 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/functions_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    72410 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/hex_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18156 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/interaction_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1233 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/log_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1149 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/patches_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6239 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/proximity_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5257 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/registers_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6067 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/stack_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1524 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/states_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4112 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/strings_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4924 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/symexec_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1229 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/trace_map_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4809 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/traces_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5125 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/types_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9710 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/views/view.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.266512 angr-management-9.2.97/angrmanagement/ui/widgets/
+-rw-r--r--   0 vsts      (1001) docker     (127)      987 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2435 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/filesystem_table.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1523 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qaddress_input.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6119 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qast_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14284 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qblock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25547 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qblock_code.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2199 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qblock_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24777 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qccode_edit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10063 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qccode_highlighter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1494 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qcolor_option.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2095 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qconstraint_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10223 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qdatadep_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7110 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qdatadepgraph_block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9805 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qdecomp_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4447 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qdep_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7674 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qdepgraph_block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3715 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qdisasm_base_control.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12665 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qdisasm_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4831 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qdisasm_statusbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26979 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qfeature_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2833 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qfiledesc_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qfont_option.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1934 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qfunction_combobox.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5922 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qfunction_header.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20238 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qfunction_table.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11772 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qgraph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11714 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qgraph_arrow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1214 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qgraph_object.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1080 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qicon_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9249 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qinst_annotation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11637 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qinstruction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1753 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qipython_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20717 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qlinear_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8606 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qlog_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9752 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qmemory_data_block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5488 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qmemory_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9628 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qminimap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19882 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qoperand.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5087 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qpatch_table.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4671 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qpathtree.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5187 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qphivariable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5100 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qproximity_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12132 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qproximitygraph_block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5600 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qregister_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9769 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qsimulation_manager_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12162 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qsimulation_managers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5464 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qstate_block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      909 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qstate_combobox.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6199 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qstate_table.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8582 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qstring_table.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4799 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qsymexec_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15555 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qtrace_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4544 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qtypedef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3480 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qunknown_block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4278 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qvariable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2417 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qvextemps_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10602 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/qxref_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1721 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/widgets/state_inspector.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    38533 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/ui/workspace.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.266512 angr-management-9.2.97/angrmanagement/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8191 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      757 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/block_objects.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3562 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/cfg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      357 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/daemon_thread.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1655 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2387 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/env.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1314 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/func.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11456 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30785 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/graph_layouter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2451 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/io.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/layout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      672 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/monkeypatch_stdio.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    42616 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/namegen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11676 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/utils/tree_graph_layouter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.266512 angr-management-9.2.97/angrmanagement/vendor/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.274512 angr-management-9.2.97/angrmanagement/vendor/qtconsole/
+-rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       73 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       72 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14176 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/ansi_code_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6295 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/base_frontend_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3733 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/bracket_matcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10683 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/call_tip_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1971 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8839 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/comms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12909 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/completion_html.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2234 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/completion_plain.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8151 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/completion_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   104717 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/console_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34810 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/frontend_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9947 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/history_console_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2874 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/inprocess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      169 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/ipython_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24994 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/jupyter_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1813 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/kernel_mixins.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3793 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/kill_ring.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    38376 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/mainwindow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2602 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9110 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/pygments_highlighter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      540 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/qstringhelpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17176 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/qtconsoleapp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      184 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/rich_ipython_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18469 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/rich_jupyter_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8638 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/rich_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3801 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/styles.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/svg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8349 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8354 2024-04-02 17:01:37.000000 angr-management-9.2.97/angrmanagement/vendor/qtconsole/util.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      596 2024-04-02 17:01:44.000000 angr-management-9.2.97/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1364 2024-04-02 17:03:02.278512 angr-management-9.2.97/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:02.274512 angr-management-9.2.97/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2053 2024-04-02 17:01:37.000000 angr-management-9.2.97/tests/test_qaddress_input.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5241 2024-04-02 17:01:37.000000 angr-management-9.2.97/tests/test_rename_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3681 2024-04-02 17:01:37.000000 angr-management-9.2.97/tests/test_rename_variables.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3487 2024-04-02 17:01:37.000000 angr-management-9.2.97/tests/test_tagged_interval_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3220 2024-04-02 17:01:37.000000 angr-management-9.2.97/tests/test_views_open.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      873 2024-04-02 17:01:37.000000 angr-management-9.2.97/tests/test_workflow.py
```

### Comparing `angr-management-9.2.96/LICENSE` & `angr-management-9.2.97/LICENSE`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/PKG-INFO` & `angr-management-9.2.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: angr-management
-Version: 9.2.96
+Version: 9.2.97
 Summary: GUI for angr
 Home-page: https://github.com/angr/angr-management
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PySide6<=6.6.1,>=6.4.2
-Requires-Dist: PySide6-QtAds
+Requires-Dist: PySide6>=6.4.2
+Requires-Dist: PySide6-QtAds>=4.2.1
 Requires-Dist: QtAwesome
 Requires-Dist: QtPy
-Requires-Dist: angr[angrDB]==9.2.96
+Requires-Dist: angr[angrDB]==9.2.97
 Requires-Dist: bidict
 Requires-Dist: ipython
 Requires-Dist: pyqodeng>=0.0.10
 Requires-Dist: requests[socks]
 Requires-Dist: tomlkit
 Requires-Dist: pyobjc-framework-Cocoa; platform_system == "Darwin"
 Requires-Dist: thefuzz[speedup]
@@ -33,15 +33,15 @@
 Requires-Dist: packaging
 Provides-Extra: bintrace
 Requires-Dist: bintrace; extra == "bintrace"
 Provides-Extra: pyinstaller
 Requires-Dist: pyinstaller==6.5.0; extra == "pyinstaller"
 Requires-Dist: pillow; platform_system == "Darwin" and extra == "pyinstaller"
 Requires-Dist: keystone-engine; extra == "pyinstaller"
-Requires-Dist: archr==9.2.96; platform_system == "Linux" and extra == "pyinstaller"
+Requires-Dist: archr==9.2.97; platform_system == "Linux" and extra == "pyinstaller"
 
 # angr Management
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This is the GUI for angr.
 Launch it and analyze some binaries!
```

### Comparing `angr-management-9.2.96/README.md` & `angr-management-9.2.97/README.md`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angr_management.egg-info/PKG-INFO` & `angr-management-9.2.97/angr_management.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: angr-management
-Version: 9.2.96
+Version: 9.2.97
 Summary: GUI for angr
 Home-page: https://github.com/angr/angr-management
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PySide6<=6.6.1,>=6.4.2
-Requires-Dist: PySide6-QtAds
+Requires-Dist: PySide6>=6.4.2
+Requires-Dist: PySide6-QtAds>=4.2.1
 Requires-Dist: QtAwesome
 Requires-Dist: QtPy
-Requires-Dist: angr[angrDB]==9.2.96
+Requires-Dist: angr[angrDB]==9.2.97
 Requires-Dist: bidict
 Requires-Dist: ipython
 Requires-Dist: pyqodeng>=0.0.10
 Requires-Dist: requests[socks]
 Requires-Dist: tomlkit
 Requires-Dist: pyobjc-framework-Cocoa; platform_system == "Darwin"
 Requires-Dist: thefuzz[speedup]
@@ -33,15 +33,15 @@
 Requires-Dist: packaging
 Provides-Extra: bintrace
 Requires-Dist: bintrace; extra == "bintrace"
 Provides-Extra: pyinstaller
 Requires-Dist: pyinstaller==6.5.0; extra == "pyinstaller"
 Requires-Dist: pillow; platform_system == "Darwin" and extra == "pyinstaller"
 Requires-Dist: keystone-engine; extra == "pyinstaller"
-Requires-Dist: archr==9.2.96; platform_system == "Linux" and extra == "pyinstaller"
+Requires-Dist: archr==9.2.97; platform_system == "Linux" and extra == "pyinstaller"
 
 # angr Management
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This is the GUI for angr.
 Launch it and analyze some binaries!
```

### Comparing `angr-management-9.2.96/angr_management.egg-info/SOURCES.txt` & `angr-management-9.2.97/angr_management.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -129,25 +129,35 @@
 angrmanagement/resources/images/toolbar-forward.png
 angrmanagement/resources/images/toolbar-previous.png
 angrmanagement/resources/images/toolbar-show-alignment.png
 angrmanagement/resources/images/warning-icon.png
 angrmanagement/resources/themes/base.css
 angrmanagement/resources/themes/Catppuccin Mocha/theme.css
 angrmanagement/resources/themes/Catppuccin Mocha/images/close.svg
+angrmanagement/resources/themes/Catppuccin Mocha/images/drawing-pin.svg
+angrmanagement/resources/themes/Catppuccin Mocha/images/minimize-button.svg
 angrmanagement/resources/themes/Catppuccin Mocha/images/provenance.txt
 angrmanagement/resources/themes/Catppuccin Mocha/images/tab-menu.svg
 angrmanagement/resources/themes/Dark/theme.css
 angrmanagement/resources/themes/Dark/images/close.svg
+angrmanagement/resources/themes/Dark/images/drawing-pin.svg
+angrmanagement/resources/themes/Dark/images/minimize-button.svg
 angrmanagement/resources/themes/Dark/images/provenance.txt
 angrmanagement/resources/themes/Dark/images/tab-menu.svg
 angrmanagement/resources/themes/Dracula/theme.css
 angrmanagement/resources/themes/Dracula/images/close.svg
+angrmanagement/resources/themes/Dracula/images/drawing-pin.svg
+angrmanagement/resources/themes/Dracula/images/minimize-button.svg
 angrmanagement/resources/themes/Dracula/images/provenance.txt
 angrmanagement/resources/themes/Dracula/images/tab-menu.svg
+angrmanagement/resources/themes/Light/theme.css
 angrmanagement/resources/themes/Light/images/close.svg
+angrmanagement/resources/themes/Light/images/drawing-pin-light.svg
+angrmanagement/resources/themes/Light/images/drawing-pin.svg
+angrmanagement/resources/themes/Light/images/minimize-button.svg
 angrmanagement/resources/themes/Light/images/provenance.txt
 angrmanagement/resources/themes/Light/images/tab-menu.svg
 angrmanagement/ui/__init__.py
 angrmanagement/ui/awesome_tooltip_event_filter.py
 angrmanagement/ui/icons.py
 angrmanagement/ui/main_window.py
 angrmanagement/ui/toolbar_manager.py
@@ -334,8 +344,9 @@
 angrmanagement/vendor/qtconsole/svg.py
 angrmanagement/vendor/qtconsole/usage.py
 angrmanagement/vendor/qtconsole/util.py
 tests/test_qaddress_input.py
 tests/test_rename_functions.py
 tests/test_rename_variables.py
 tests/test_tagged_interval_map.py
+tests/test_views_open.py
 tests/test_workflow.py
```

### Comparing `angr-management-9.2.96/angrmanagement/__main__.py` & `angr-management-9.2.97/angrmanagement/__main__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/config/__init__.py` & `angr-management-9.2.97/angrmanagement/config/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/config/color_schemes.py` & `angr-management-9.2.97/angrmanagement/config/color_schemes.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/config/config_entry.py` & `angr-management-9.2.97/angrmanagement/config/config_entry.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/config/config_manager.py` & `angr-management-9.2.97/angrmanagement/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/daemon/__init__.py` & `angr-management-9.2.97/angrmanagement/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/daemon/client.py` & `angr-management-9.2.97/angrmanagement/daemon/client.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/daemon/server.py` & `angr-management-9.2.97/angrmanagement/daemon/server.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/daemon/url_handler.py` & `angr-management-9.2.97/angrmanagement/daemon/url_handler.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/analysis_options.py` & `angr-management-9.2.97/angrmanagement/data/analysis_options.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/breakpoint.py` & `angr-management-9.2.97/angrmanagement/data/breakpoint.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/function_graph.py` & `angr-management-9.2.97/angrmanagement/data/function_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/instance.py` & `angr-management-9.2.97/angrmanagement/data/instance.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/__init__.py` & `angr-management-9.2.97/angrmanagement/data/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/cfg_generation.py` & `angr-management-9.2.97/angrmanagement/data/jobs/cfg_generation.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/code_tagging.py` & `angr-management-9.2.97/angrmanagement/data/jobs/code_tagging.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/ddg_generation.py` & `angr-management-9.2.97/angrmanagement/data/jobs/ddg_generation.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/decompile_function.py` & `angr-management-9.2.97/angrmanagement/data/jobs/decompile_function.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/dependency_analysis.py` & `angr-management-9.2.97/angrmanagement/data/jobs/dependency_analysis.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/flirt_signature_recognition.py` & `angr-management-9.2.97/angrmanagement/data/jobs/flirt_signature_recognition.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/job.py` & `angr-management-9.2.97/angrmanagement/data/jobs/job.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/loading.py` & `angr-management-9.2.97/angrmanagement/data/jobs/loading.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/prototype_finding.py` & `angr-management-9.2.97/angrmanagement/data/jobs/prototype_finding.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/simgr_explore.py` & `angr-management-9.2.97/angrmanagement/data/jobs/simgr_explore.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/simgr_step.py` & `angr-management-9.2.97/angrmanagement/data/jobs/simgr_step.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/variable_recovery.py` & `angr-management-9.2.97/angrmanagement/data/jobs/variable_recovery.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/jobs/vfg_generation.py` & `angr-management-9.2.97/angrmanagement/data/jobs/vfg_generation.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/library_docs.py` & `angr-management-9.2.97/angrmanagement/data/library_docs.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/log.py` & `angr-management-9.2.97/angrmanagement/data/log.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/object_container.py` & `angr-management-9.2.97/angrmanagement/data/object_container.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/tagged_interval_map.py` & `angr-management-9.2.97/angrmanagement/data/tagged_interval_map.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/data/trace.py` & `angr-management-9.2.97/angrmanagement/data/trace.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/logic/__init__.py` & `angr-management-9.2.97/angrmanagement/logic/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/logic/commands/command.py` & `angr-management-9.2.97/angrmanagement/logic/commands/command.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/logic/commands/command_manager.py` & `angr-management-9.2.97/angrmanagement/logic/commands/command_manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/logic/debugger/bintrace.py` & `angr-management-9.2.97/angrmanagement/logic/debugger/bintrace.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/logic/debugger/debugger.py` & `angr-management-9.2.97/angrmanagement/logic/debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/logic/debugger/simgr.py` & `angr-management-9.2.97/angrmanagement/logic/debugger/simgr.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/logic/disassembly/info_dock.py` & `angr-management-9.2.97/angrmanagement/logic/disassembly/info_dock.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/logic/disassembly/jump_history.py` & `angr-management-9.2.97/angrmanagement/logic/disassembly/jump_history.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/logic/singleton.py` & `angr-management-9.2.97/angrmanagement/logic/singleton.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/logic/threads.py` & `angr-management-9.2.97/angrmanagement/logic/threads.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/logic/url_scheme.py` & `angr-management-9.2.97/angrmanagement/logic/url_scheme.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/__init__.py` & `angr-management-9.2.97/angrmanagement/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/ail2asm/ail2arm32.py` & `angr-management-9.2.97/angrmanagement/plugins/ail2asm/ail2arm32.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/ail2asm/asm_output.py` & `angr-management-9.2.97/angrmanagement/plugins/ail2asm/asm_output.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/base_plugin.py` & `angr-management-9.2.97/angrmanagement/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/coverage/coverage.py` & `angr-management-9.2.97/angrmanagement/plugins/coverage/coverage.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/coverage/parse_trace.py` & `angr-management-9.2.97/angrmanagement/plugins/coverage/parse_trace.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/decompiler_poison/__init__.py` & `angr-management-9.2.97/angrmanagement/plugins/decompiler_poison/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/dep_viewer/dep_plugin.py` & `angr-management-9.2.97/angrmanagement/plugins/dep_viewer/dep_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/dep_viewer/sinks.py` & `angr-management-9.2.97/angrmanagement/plugins/dep_viewer/sinks.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/execution_statistics_viewer/execution_statistics_viewer.py` & `angr-management-9.2.97/angrmanagement/plugins/execution_statistics_viewer/execution_statistics_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/load.py` & `angr-management-9.2.97/angrmanagement/plugins/load.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/memory_checker/memory_checker.py` & `angr-management-9.2.97/angrmanagement/plugins/memory_checker/memory_checker.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/plugin_description.py` & `angr-management-9.2.97/angrmanagement/plugins/plugin_description.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/plugin_manager.py` & `angr-management-9.2.97/angrmanagement/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/precise_diffing/diff_view.py` & `angr-management-9.2.97/angrmanagement/plugins/precise_diffing/diff_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/precise_diffing/function_diff.py` & `angr-management-9.2.97/angrmanagement/plugins/precise_diffing/function_diff.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/precise_diffing/precisediff_plugin.py` & `angr-management-9.2.97/angrmanagement/plugins/precise_diffing/precisediff_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         job = CFGGenerationJob(on_finish=self._generate_binary_cfg_done)
         self.diff_instance.add_job(job)
 
     def _generate_binary_cfg_done(self) -> None:
         self.revised_binary_loaded()
 
     def _create_revised_disassembly_view(self):
-        new_disass = DiffDisassemblyView(self.workspace, self.diff_instance, "center")
+        new_disass = DiffDisassemblyView(self.workspace, "center", self.diff_instance)
         new_disass.category = "diff"
         new_disass.base_caption = "Precise Diff"
         self.current_revised_view = new_disass
         self.workspace.add_view(self.current_revised_view)
         return self.current_revised_view
 
     def jump_to_in_revised_view(self, func) -> None:
```

### Comparing `angr-management-9.2.96/angrmanagement/plugins/precise_diffing/settings_dialog.py` & `angr-management-9.2.97/angrmanagement/plugins/precise_diffing/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/sample_plugin.py` & `angr-management-9.2.97/angrmanagement/plugins/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/source_importer/__init__.py` & `angr-management-9.2.97/angrmanagement/plugins/source_importer/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/source_viewer/source_viewer_plugin.py` & `angr-management-9.2.97/angrmanagement/plugins/source_viewer/source_viewer_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/trace_viewer/afl_qemu_bitmap.py` & `angr-management-9.2.97/angrmanagement/plugins/trace_viewer/afl_qemu_bitmap.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/trace_viewer/multi_trace.py` & `angr-management-9.2.97/angrmanagement/plugins/trace_viewer/multi_trace.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/trace_viewer/qtrace_viewer.py` & `angr-management-9.2.97/angrmanagement/plugins/trace_viewer/qtrace_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/trace_viewer/trace_plugin.py` & `angr-management-9.2.97/angrmanagement/plugins/trace_viewer/trace_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/trace_viewer/trace_statistics.py` & `angr-management-9.2.97/angrmanagement/plugins/trace_viewer/trace_statistics.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/value_search/constants.py` & `angr-management-9.2.97/angrmanagement/plugins/value_search/constants.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/value_search/qsearch_table.py` & `angr-management-9.2.97/angrmanagement/plugins/value_search/qsearch_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/plugins/value_search/search_view.py` & `angr-management-9.2.97/angrmanagement/plugins/value_search/search_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 class SearchView(InstanceView):
     """
     Container view for the QSearchTable Object.
     Has handlers for switching between search types and executing the search.
     """
 
     def __init__(
-        self, plugin, workspace: Workspace, instance: Instance, default_docking_position: str, *args, **kwargs
+        self, plugin, workspace: Workspace, default_docking_position: str, instance: Instance, *args, **kwargs
     ) -> None:
         super().__init__("search", workspace, default_docking_position, instance, *args, **kwargs)
 
         self.base_caption = "Search"
         self.plugin = plugin
 
         self._search_table: QSearchTable
```

### Comparing `angr-management-9.2.96/angrmanagement/plugins/value_search/value_search_plugin.py` & `angr-management-9.2.97/angrmanagement/plugins/value_search/value_search_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def color_insn(self, addr: int, selected, disasm_view) -> None:
         pass
 
     def teardown(self) -> None:
         self._destroy_search_view()
 
     def _create_search_view(self) -> None:
-        self.search_view = SearchView(self, self.workspace, self.workspace.main_instance, "center")
+        self.search_view = SearchView(self, self.workspace, "center", self.workspace.main_instance)
         self.workspace.add_view(self.search_view)
 
     def _destroy_search_view(self) -> None:
         self.workspace.remove_view(self.search_view)
 
     #
     # helpers
```

### Comparing `angr-management-9.2.96/angrmanagement/plugins/varec/varec.py` & `angr-management-9.2.97/angrmanagement/plugins/varec/varec.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/fonts/DejaVuSansMono.ttf` & `angr-management-9.2.97/angrmanagement/resources/fonts/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/fonts/SourceCodePro-Regular.ttf` & `angr-management-9.2.97/angrmanagement/resources/fonts/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/angr-ds.png` & `angr-management-9.2.97/angrmanagement/resources/images/angr-ds.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/angr-splash.png` & `angr-management-9.2.97/angrmanagement/resources/images/angr-splash.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/angr.ico` & `angr-management-9.2.97/angrmanagement/resources/images/angr.ico`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/angr.png` & `angr-management-9.2.97/angrmanagement/resources/images/angr.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/benchmark-icon.png` & `angr-management-9.2.97/angrmanagement/resources/images/benchmark-icon.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/error-icon.png` & `angr-management-9.2.97/angrmanagement/resources/images/error-icon.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/run-icon.svg` & `angr-management-9.2.97/angrmanagement/resources/images/run-icon.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/toolbar-docker-open.png` & `angr-management-9.2.97/angrmanagement/resources/images/toolbar-docker-open.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/toolbar-file-open.ico` & `angr-management-9.2.97/angrmanagement/resources/images/toolbar-file-open.ico`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/toolbar-file-save.png` & `angr-management-9.2.97/angrmanagement/resources/images/toolbar-file-save.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/toolbar-forward.png` & `angr-management-9.2.97/angrmanagement/resources/images/toolbar-forward.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/toolbar-previous.png` & `angr-management-9.2.97/angrmanagement/resources/images/toolbar-previous.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/toolbar-show-alignment.png` & `angr-management-9.2.97/angrmanagement/resources/images/toolbar-show-alignment.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/images/warning-icon.png` & `angr-management-9.2.97/angrmanagement/resources/images/warning-icon.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/themes/Catppuccin Mocha/images/close.svg` & `angr-management-9.2.97/angrmanagement/resources/themes/Catppuccin Mocha/images/close.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/themes/Dark/images/close.svg` & `angr-management-9.2.97/angrmanagement/resources/themes/Dark/images/close.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/themes/Dracula/images/close.svg` & `angr-management-9.2.97/angrmanagement/resources/themes/Dracula/images/close.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/resources/themes/Light/images/close.svg` & `angr-management-9.2.97/angrmanagement/resources/themes/Light/images/close.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/awesome_tooltip_event_filter.py` & `angr-management-9.2.97/angrmanagement/ui/awesome_tooltip_event_filter.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/css/__init__.py` & `angr-management-9.2.97/angrmanagement/ui/css/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/__init__.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/about.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/about.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/analysis_options.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/analysis_options.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/assemble_patch.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/assemble_patch.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/breakpoint.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/breakpoint.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/command_palette.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/command_palette.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/data_dep_graph_search.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/data_dep_graph_search.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/dependson.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/dependson.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/env_config.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/env_config.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/fs_mount.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/fs_mount.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/func_doc.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/func_doc.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/function.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/function.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/hook.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/hook.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/input_prompt.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/input_prompt.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/jumpto.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/jumpto.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/load_binary.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/load_binary.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/load_docker_prompt.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/load_docker_prompt.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/load_plugins.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/load_plugins.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/new_state.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/new_state.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/preferences.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/preferences.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/rename.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/rename.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/rename_label.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/rename_label.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/rename_node.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/rename_node.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/retype_node.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/retype_node.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/set_comment.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/set_comment.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/socket_config.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/socket_config.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/type_editor.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/type_editor.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/welcome.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/welcome.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/dialogs/xref.py` & `angr-management-9.2.97/angrmanagement/ui/dialogs/xref.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/documents/qcodedocument.py` & `angr-management-9.2.97/angrmanagement/ui/documents/qcodedocument.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/icons.py` & `angr-management-9.2.97/angrmanagement/ui/icons.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/main_window.py` & `angr-management-9.2.97/angrmanagement/ui/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,14 +364,16 @@
                 | QtAds.CDockManager.OpaqueSplitterResize
                 | QtAds.CDockManager.FocusHighlighting
             )
             & ~QtAds.CDockManager.DockAreaHasUndockButton
         )
         self.dock_manager = QtAds.CDockManager(self)
         self.dock_manager.setStyleSheet("")  # Clear stylesheet overrides
+        self.dock_manager.setAutoHideConfigFlags(QtAds.CDockManager.DefaultAutoHideConfig)
+        self.dock_manager.createSideTabBarWidgets()
         self.setCentralWidget(self.dock_manager)
         wk = Workspace(self, Instance())
         self.workspace = wk
 
         def set_caption(**kwargs) -> None:  # pylint: disable=unused-argument
             if self.workspace.main_instance.project.am_none:
                 self.caption = ""
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/menus/analyze_menu.py` & `angr-management-9.2.97/angrmanagement/ui/menus/analyze_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/menus/disasm_insn_context_menu.py` & `angr-management-9.2.97/angrmanagement/ui/menus/disasm_insn_context_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/menus/disasm_label_context_menu.py` & `angr-management-9.2.97/angrmanagement/ui/menus/disasm_label_context_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/menus/disasm_options_menu.py` & `angr-management-9.2.97/angrmanagement/ui/menus/disasm_options_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/menus/file_menu.py` & `angr-management-9.2.97/angrmanagement/ui/menus/file_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/menus/function_context_menu.py` & `angr-management-9.2.97/angrmanagement/ui/menus/function_context_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/menus/help_menu.py` & `angr-management-9.2.97/angrmanagement/ui/menus/help_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/menus/log_menu.py` & `angr-management-9.2.97/angrmanagement/ui/menus/log_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/menus/menu.py` & `angr-management-9.2.97/angrmanagement/ui/menus/menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/menus/view_menu.py` & `angr-management-9.2.97/angrmanagement/ui/menus/view_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/toolbar_manager.py` & `angr-management-9.2.97/angrmanagement/ui/toolbar_manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/toolbars/debug_toolbar.py` & `angr-management-9.2.97/angrmanagement/ui/toolbars/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/toolbars/feature_map_toolbar.py` & `angr-management-9.2.97/angrmanagement/ui/toolbars/feature_map_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/toolbars/file_toolbar.py` & `angr-management-9.2.97/angrmanagement/ui/toolbars/file_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/toolbars/function_table_toolbar.py` & `angr-management-9.2.97/angrmanagement/ui/toolbars/function_table_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/toolbars/nav_toolbar.py` & `angr-management-9.2.97/angrmanagement/ui/toolbars/nav_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/toolbars/toolbar.py` & `angr-management-9.2.97/angrmanagement/ui/toolbars/toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/toolbars/toolbar_action.py` & `angr-management-9.2.97/angrmanagement/ui/toolbars/toolbar_action.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/toolbars/toolbar_dock.py` & `angr-management-9.2.97/angrmanagement/ui/toolbars/toolbar_dock.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/view_manager.py` & `angr-management-9.2.97/angrmanagement/ui/view_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,16 @@
         self._promote_view(view)
 
         # find the dock widget by the view
         dock = self.view_to_dock.get(view, None)
         if dock is None:
             return
 
+        if dock.isAutoHide():
+            dock.toggleView(True)
         if not dock.isTabbed():
             dock.show()
         dock.raise_()
         view.focusWidget()
 
     def get_center_docks(self) -> Sequence[QtAds.CDockWidget]:
         """
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/__init__.py` & `angr-management-9.2.97/angrmanagement/ui/views/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/breakpoints_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/breakpoints_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
 
 class BreakpointsView(InstanceView):
     """
     Breakpoints table view.
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("breakpoints", workspace, default_docking_position, instance)
         self.base_caption = "Breakpoints"
         self._tbl_widget: QBreakpointTableWidget | None = None
         self._init_widgets()
         self.reload()
 
     def reload(self) -> None:
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/call_explorer_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/call_explorer_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 
 class CallExplorerView(InstanceView):
     """
     Call Explorer view.
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("call_explorer", workspace, default_docking_position, instance)
 
         self._last_updated_func: int | Function | None = None
         self._inhibit_update: bool = False
 
         self.base_caption = "Call Explorer"
         self._tree: QTreeWidget | None = None
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/code_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/code_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 class CodeView(FunctionView):
     """
     A view to display pseudocode or source code. You should control this view by manipulating and observing its four
     ObjectContainers: .addr, .current_node, .codegen, and .function.
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("pseudocode", workspace, default_docking_position, instance)
 
         self.base_caption = "Pseudocode"
 
         self._function: ObjectContainer | Function = ObjectContainer(None, "The function to decompile")
         self.current_node = ObjectContainer(None, "Current selected C-code node")
         self.addr: ObjectContainer | int = ObjectContainer(0, "Current cursor address")
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/console_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/console_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class ConsoleView(InstanceView):
     """
     Console view providing IPython interactive session.
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("console", workspace, default_docking_position, instance)
 
         self.base_caption = "Console"
         self._ipython_widget = None
 
         if self.workspace.main_window.initialized:
             self.mainWindowInitializedEvent()
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/data_dep_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/data_dep_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,28 +29,20 @@
 class DataDepView(InstanceView):
     """Workspace view used to display a data dependency graph on the screen"""
 
     @property
     def function(self):
         raise NotImplementedError("Does not apply!")
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("data_dependency", workspace, default_docking_position, instance)
 
         self.base_caption = "Data Dependency"
 
-        # Get all instructions in the program
         self._instructions: dict[int, CsInsn] = {}
-        inst = self.instance
-        for _, func in inst.kb.functions.items():
-            for block in func.blocks:
-                disass = block.disassembly
-                for ins in disass.insns:
-                    self._instructions[ins.address] = ins
-
         self._end_state: SimState | None = None
         self._start_addr: int | None = None
         self._end_addr: int | None = None
         self._block_addrs: list[int] | None = None
 
         # UI widgets
         self._graph_widget: QDataDepGraph | None = None
@@ -154,17 +146,24 @@
         self.redraw_graph()
 
     def on_screen_changed(self) -> None:
         if self._graph_widget is not None:
             self._graph_widget.refresh()
 
     def reload(self) -> None:
-        if self._graph_widget is None:
+        if self.instance.am_none or self._graph_widget is None:
             return
 
+        # Get all instructions in the program
+        for _, func in self.instance.kb.functions.items():
+            for block in func.blocks:
+                disass = block.disassembly
+                for ins in disass.insns:
+                    self._instructions[ins.address] = ins
+
         # Re-Generate the graph
         if not self._data_dep:
             self._graph = None
             self._graph_widget.graph = None
             self._graph_widget.request_relayout()
             return
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/dep_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/dep_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 class DependencyView(InstanceView):
     """
     Creates view for dependency analysis.
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("dependencies", workspace, default_docking_position, instance)
 
         self.base_caption = "Dependencies"
 
         # UI widgets
         self._graph_widget: QDependencyGraph = None
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/disassembly_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/disassembly_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """
     Disassembly View
     """
 
     view_visibility_changed = Signal()
     disassembly_level_changed = Signal(DisassemblyLevel)
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("disassembly", workspace, default_docking_position, instance)
 
         self.base_caption = "Disassembly"
         self._disassembly_level = DisassemblyLevel.MachineCode
         self._show_minimap: bool = True
         self._show_address = True
         self._show_variable = True
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/functions_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/functions_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class FunctionsView(InstanceView):
     """
     View displaying functions in the project.
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("functions", workspace, default_docking_position, instance)
 
         self.base_caption = "Functions"
         self._function_table: QFunctionTable
 
         self.instance.cfg.am_subscribe(self.reload)
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/hex_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/hex_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1321,15 +1321,15 @@
 class HexView(SynchronizedInstanceView):
     """
     View and edit memory/object code in classic hex editor format.
     """
 
     _widgets_initialized: bool = False
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("hex", workspace, default_docking_position, instance)
         self.base_caption: str = "Hex"
         self.smart_highlighting_enabled: bool = True
         self._clipboard = None
         self._cfb_highlights: Sequence[HexHighlightRegion] = []
         self._sync_view_highlights: Sequence[HexHighlightRegion] = []
         self._patch_highlights: Sequence[PatchHighlightRegion] = []
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/interaction_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/interaction_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,16 +70,16 @@
     BEGINNING = 1
     RUNNING = 2
     STOPPED = 3
     VIEWING = 4
 
 
 class InteractionView(InstanceView):
-    def __init__(self, workspace: Workspace, instance: Instance) -> None:
-        super().__init__("interaction", workspace, "bottom", instance)
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
+        super().__init__("interaction", workspace, default_docking_position, instance)
         self.base_caption = "Interaction"
         self.current_log = (
             []
         )  # for now each entry is a dict. each entry has {"dir": "in"/"out", "data": bytes} and then whatever
         # "in" here means it's input to the program
         self.log_controls = []
         self.sock: nclib.Netcat | None = None
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/log_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/log_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class LogView(InstanceView):
     """
     Log view displays logging output.
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("log", workspace, default_docking_position, instance)
 
         self.base_caption = "Log"
         self._log_widget: QLogWidget = None
 
         self._init_widgets()
         self.reload()
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/patches_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/patches_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class PatchesView(InstanceView):
     """
     View showing all patches.
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("patches", workspace, default_docking_position, instance)
 
         self.base_caption = "Patches"
         self._patch_table: QPatchTable
 
         self._init_widgets()
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/proximity_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/proximity_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 class ProximityView(InstanceView):
     """
     Proximity View
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("proximity", workspace, default_docking_position, instance)
 
         self.base_caption = "Proximity"
 
         self._function: Function | None = None
         self._expand_function_addrs: set[int] = set()
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/registers_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/registers_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
 
 class RegistersView(InstanceView):
     """
     Register table view.
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("registers", workspace, default_docking_position, instance)
 
         self.base_caption = "Registers"
         self._tbl_widget: QRegisterTableWidget | None = None
         self._init_widgets()
         self.reload()
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/stack_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/stack_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
 
 class StackView(InstanceView):
     """
     Stack table view.
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("stack", workspace, default_docking_position, instance)
 
         self.base_caption = "Stack"
         self._tbl_widget: QStackTableWidget | None = None
         self._init_widgets()
         self.reload()
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/states_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/states_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 if TYPE_CHECKING:
     from angrmanagement.data.instance import Instance
     from angrmanagement.ui.workspace import Workspace
 
 
 class StatesView(InstanceView):
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("states", workspace, default_docking_position, instance)
 
         self.base_caption = "States"
         self._state_table: QStateTable
 
         self._init_widgets()
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/strings_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/strings_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     from angr.knowledge_plugins.cfg.memory_data import MemoryData
 
     from angrmanagement.data.instance import Instance
     from angrmanagement.ui.workspace import Workspace
 
 
 class StringsView(InstanceView):
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("strings", workspace, default_docking_position, instance)
 
         self.base_caption = "Strings"
 
         self._string_table: QStringTable
         self._function_list: QFunctionComboBox
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/symexec_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/symexec_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 from .view import InstanceView
 
 if TYPE_CHECKING:
     from angrmanagement.ui.workspace import Workspace
 
 
 class SymexecView(InstanceView):
-    def __init__(self, workspace: Workspace, instance: Instance) -> None:
-        super().__init__("symexec", workspace, "right", instance)
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
+        super().__init__("symexec", workspace, default_docking_position, instance)
+        assert not isinstance(self.instance, str)
 
         self.base_caption = "Symbolic Execution"
 
         self._pathtree: QPathTree
         self._simgrs: QSimulationManagers
         self._state_viewer: StateInspector
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/trace_map_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/trace_map_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class TraceMapView(InstanceView):
     """
     View container for QTraceMap.
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("tracemap", workspace, default_docking_position, instance)
         self.base_caption: str = "Trace Map"
         self.inner_widget: QTraceMap | None = None
         self._init_widgets()
 
     @staticmethod
     def minimumSizeHint():
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/traces_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/traces_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
 
 class TracesView(InstanceView):
     """
     Traces table view.
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("traces", workspace, default_docking_position, instance)
 
         self.base_caption = "Traces"
         self._tbl_widget: QTraceTableWidget | None = None
         self._init_widgets()
         self.reload()
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/types_view.py` & `angr-management-9.2.97/angrmanagement/ui/views/types_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 class TypesView(FunctionView):
     """
     The view that lets you modify project.kb.types. Creates a QTypeDef for each type.
     """
 
-    def __init__(self, workspace: Workspace, instance: Instance, default_docking_position: str) -> None:
+    def __init__(self, workspace: Workspace, default_docking_position: str, instance: Instance) -> None:
         super().__init__("types", workspace, default_docking_position, instance)
 
         self.base_caption = "Types"
 
         self._function = ObjectContainer(None, "Current function")
         self._function.am_subscribe(self.reload)
 
@@ -91,14 +91,18 @@
     def reload(self) -> None:
         for child in list(self._layout.parent().children()):
             if type(child) is QCTypeDef:
                 self._layout.takeAt(0)
                 self._layout.removeWidget(child)
                 child.deleteLater()
 
+        if self.instance.project.am_none:
+            self._caption_label.setText("Types View")
+            return
+
         # update the display
         if self.function.am_none:
             self._caption_label.setText("Persistent (global) variable types")
         else:
             txt = f"Temporary (local) variable types for function {self.function.addr:#x}"
             self._caption_label.setText(txt)
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/views/view.py` & `angr-management-9.2.97/angrmanagement/ui/views/view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/__init__.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/filesystem_table.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/filesystem_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qaddress_input.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qaddress_input.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qast_viewer.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qast_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qblock.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qblock.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qblock_code.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qblock_code.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qblock_label.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qblock_label.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qccode_edit.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qccode_edit.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,14 +426,19 @@
             self._code_view.codegen.am_event()
 
     def float_constant(self) -> None:
         if hasattr(self._selected_node, "fmt_float"):
             self._selected_node.fmt_float ^= True
             self._code_view.codegen.am_event()
 
+    def double_constant(self) -> None:
+        if hasattr(self._selected_node, "fmt_double"):
+            self._selected_node.fmt_double ^= True
+            self._code_view.codegen.am_event()
+
     def convert_to_ite_expr(self) -> None:
         node = self._selected_node
         if not isinstance(node, CExpression):
             return
         ailexpr = self._code_view.codegen.cnode2ailexpr.get(node, None)
         if ailexpr is None:
             return
@@ -605,14 +610,16 @@
         self.action_neg.triggered.connect(self.neg_constant)
         self.action_neg.setShortcut(QKeySequence("_"))
         self.action_char = QAction("Toggle char", self)
         self.action_char.triggered.connect(self.char_constant)
         self.action_char.setShortcut(QKeySequence("R"))
         self.action_float = QAction("Toggle float", self)
         self.action_float.triggered.connect(self.float_constant)
+        self.action_double = QAction("Toggle double", self)
+        self.action_double.triggered.connect(self.double_constant)
         self.action_to_ite_expr = QAction("Create a ternary expression")
         self.action_to_ite_expr.triggered.connect(self.convert_to_ite_expr)
         self.action_swap_binop_operands = QAction("Swap operands")
         self.action_swap_binop_operands.triggered.connect(self.swap_binop_operands)
 
         expr_actions = [
             self.action_to_ite_expr,
@@ -635,14 +642,15 @@
         self.function_name_actions = [self.action_rename_node, self.action_xref]
 
         self.constant_actions = [
             self.action_hex,
             self.action_neg,
             self.action_char,
             self.action_float,
+            self.action_double,
         ]
 
         self.call_actions = [self.action_rename_node, self.action_xref]
 
         self.constant_actions += base_actions + expr_actions
         self.operator_actions += base_actions + expr_actions
         self.variable_actions += base_actions + expr_actions
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qccode_highlighter.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qccode_highlighter.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qcolor_option.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qcolor_option.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qconstraint_viewer.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qconstraint_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qdatadep_graph.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qdatadep_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qdatadepgraph_block.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qdatadepgraph_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qdecomp_options.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qdecomp_options.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qdep_graph.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qdep_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qdepgraph_block.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qdepgraph_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qdisasm_base_control.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qdisasm_base_control.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qdisasm_graph.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qdisasm_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qdisasm_statusbar.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qdisasm_statusbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qfeature_map.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qfeature_map.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qfiledesc_viewer.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qfiledesc_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qfont_option.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qfont_option.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qfunction_combobox.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qfunction_combobox.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qfunction_header.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qfunction_header.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qfunction_table.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qfunction_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qgraph.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qgraph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qgraph_arrow.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qgraph_arrow.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qgraph_object.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qgraph_object.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qicon_label.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qicon_label.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qinst_annotation.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qinst_annotation.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qinstruction.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qinstruction.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qipython_widget.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qipython_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qlinear_viewer.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qlinear_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qlog_widget.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qlog_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qmemory_data_block.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qmemory_data_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qmemory_viewer.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qmemory_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qminimap.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qminimap.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qoperand.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qoperand.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qpatch_table.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qpatch_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,18 +79,22 @@
         else:
             return None
 
     def reload(self) -> None:
         self._reloading = True
         self.clearContents()
 
-        self.items = [
-            QPatchTableItem(item, self._get_bytes(self.instance.project, item.addr, len(item)))
-            for item in self.instance.project.kb.patches.values()
-        ]
+        self.items = (
+            [
+                QPatchTableItem(item, self._get_bytes(self.instance.project, item.addr, len(item)))
+                for item in self.instance.project.kb.patches.values()
+            ]
+            if not self.instance.project.am_none
+            else []
+        )
         items_count = len(self.items)
         self.setRowCount(items_count)
 
         for idx, item in enumerate(self.items):
             for i, it in enumerate(item.widgets()):
                 self.setItem(idx, i, it)
```

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qpathtree.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qpathtree.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qphivariable.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qphivariable.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qproximity_graph.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qproximity_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qproximitygraph_block.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qproximitygraph_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qregister_viewer.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qregister_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qsimulation_manager_viewer.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qsimulation_manager_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qsimulation_managers.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qsimulation_managers.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qstate_block.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qstate_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qstate_combobox.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qstate_combobox.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qstate_table.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qstate_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qstring_table.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qstring_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qsymexec_graph.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qsymexec_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qtrace_map.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qtrace_map.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qtypedef.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qtypedef.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qunknown_block.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qunknown_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qvariable.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qvariable.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qvextemps_viewer.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qvextemps_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/qxref_viewer.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/qxref_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/widgets/state_inspector.py` & `angr-management-9.2.97/angrmanagement/ui/widgets/state_inspector.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/ui/workspace.py` & `angr-management-9.2.97/angrmanagement/ui/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from angr import StateHierarchy
 from angr.knowledge_plugins.cfg import MemoryData, MemoryDataSort
 from angr.knowledge_plugins.functions.function import Function
 from angr.knowledge_plugins.patches import Patch
 from angr.misc.testing import is_testing
 from cle import SymbolType
 from PySide6.QtWidgets import QMessageBox
+from PySide6QtAds import SideBarBottom
 
 from angrmanagement.config import Conf
 from angrmanagement.data.analysis_options import (
     AnalysesConfiguration,
     CFGAnalysisConfiguration,
     CodeTaggingConfiguration,
     FlirtAnalysisConfiguration,
@@ -102,31 +103,37 @@
         instance.simgrs.am_subscribe(self._update_simgr_debuggers)
         instance.handle_comment_changed_callback = self.plugins.handle_comment_changed
         instance.job_worker_exception_callback = self._handle_job_exception
 
         self.current_screen = ObjectContainer(None, name="current_screen")
 
         self.default_tabs = [
-            DisassemblyView(self, self._main_instance, "center"),
-            HexView(self, self._main_instance, "center"),
-            CodeView(self, self._main_instance, "center"),
-            FunctionsView(self, self._main_instance, "left"),
+            DisassemblyView(self, "center", self._main_instance),
+            HexView(self, "center", self._main_instance),
+            CodeView(self, "center", self._main_instance),
+            FunctionsView(self, "left", self._main_instance),
         ]
         if Conf.has_operation_mango:
-            self.default_tabs.append(DependencyView(self, self._main_instance, "center"))
-        self.default_tabs += [
-            ConsoleView(self, self._main_instance, "bottom"),
-            LogView(self, self._main_instance, "bottom"),
+            self.default_tabs.append(DependencyView(self, "center", self._main_instance))
+        minimized_tabs = [
+            ConsoleView(self, "bottom", self._main_instance),
+            LogView(self, "bottom", self._main_instance),
         ]
+        self.default_tabs += minimized_tabs
 
         enabled_tabs = [x.strip() for x in Conf.enabled_tabs.split(",") if x.strip()]
         for tab in self.default_tabs:
             if tab.__class__.__name__ in enabled_tabs or len(enabled_tabs) == 0:
                 self.add_view(tab)
 
+        for view in minimized_tabs:
+            dock = self.view_manager.view_to_dock.get(view, None)
+            if dock is not None:
+                dock.setAutoHide(True, SideBarBottom)
+
         self._dbg_watcher = DebuggerWatcher(self.on_debugger_state_updated, self.main_instance.debugger_mgr.debugger)
         self.on_debugger_state_updated()
 
         DisassemblyView.register_commands(self)
 
         instance.patches.am_subscribe(self._on_patch_event)
 
@@ -331,15 +338,15 @@
     def new_disassembly_view(self) -> DisassemblyView:
         """
         Add a new disassembly view.
         """
         disassembly_view = self.view_manager.first_view_in_category("disassembly")
         current_addr = disassembly_view.jump_history.current if disassembly_view is not None else None
 
-        view = DisassemblyView(self, self._main_instance, "center")
+        view = DisassemblyView(self, "center", self._main_instance)
         self.add_view(view)
         self.raise_view(view)
         view._linear_viewer.initialize()  # FIXME: Don't access protected member
         if current_addr is not None:
             view.jump_to(current_addr)
         # TODO move view tab to front of dock
         return view
@@ -818,15 +825,15 @@
     def show_console_view(self) -> None:
         self.show_view("console", ConsoleView, position="bottom")
 
     def show_log_view(self) -> None:
         self.show_view("log", LogView, position="bottom")
 
     def create_and_show_hex_view(self):
-        view = HexView(self, self._main_instance, "center")
+        view = HexView(self, "center", self._main_instance)
         self.add_view(view)
         return view
 
     def toggle_exec_breakpoint(self) -> None:
         if self.main_instance is None:
             return
 
@@ -982,10 +989,10 @@
     #
 
     def _get_or_create_view(self, category: str, view_type: type[T], position: str = "center") -> T:
         view = self.view_manager.current_view_in_category(category)
         if view is None:
             view = self.view_manager.first_view_in_category(category)
         if view is None:
-            view = view_type(self, self._main_instance, position)
+            view = view_type(self, position, self._main_instance)
             self.add_view(view)
         return view
```

### Comparing `angr-management-9.2.96/angrmanagement/utils/__init__.py` & `angr-management-9.2.97/angrmanagement/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/utils/block_objects.py` & `angr-management-9.2.97/angrmanagement/utils/block_objects.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/utils/cfg.py` & `angr-management-9.2.97/angrmanagement/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/utils/edge.py` & `angr-management-9.2.97/angrmanagement/utils/edge.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/utils/env.py` & `angr-management-9.2.97/angrmanagement/utils/env.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/utils/func.py` & `angr-management-9.2.97/angrmanagement/utils/func.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/utils/graph.py` & `angr-management-9.2.97/angrmanagement/utils/graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/utils/graph_layouter.py` & `angr-management-9.2.97/angrmanagement/utils/graph_layouter.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/utils/io.py` & `angr-management-9.2.97/angrmanagement/utils/io.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/utils/monkeypatch_stdio.py` & `angr-management-9.2.97/angrmanagement/utils/monkeypatch_stdio.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/utils/namegen.py` & `angr-management-9.2.97/angrmanagement/utils/namegen.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/utils/tree_graph_layouter.py` & `angr-management-9.2.97/angrmanagement/utils/tree_graph_layouter.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/ansi_code_processor.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/ansi_code_processor.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/base_frontend_mixin.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/base_frontend_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/bracket_matcher.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/bracket_matcher.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/call_tip_widget.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/call_tip_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/client.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/client.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/comms.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/comms.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/completion_html.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/completion_html.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/completion_plain.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/completion_plain.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/completion_widget.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/completion_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/console_widget.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/console_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/frontend_widget.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/frontend_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/history_console_widget.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/history_console_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/inprocess.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/inprocess.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/jupyter_widget.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/jupyter_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/kernel_mixins.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/kernel_mixins.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/kill_ring.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/kill_ring.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/mainwindow.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/mainwindow.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/manager.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/pygments_highlighter.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/pygments_highlighter.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/qstringhelpers.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/qstringhelpers.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/qtconsoleapp.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/qtconsoleapp.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/rich_jupyter_widget.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/rich_jupyter_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/rich_text.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/rich_text.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/styles.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/styles.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/svg.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/svg.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/usage.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/usage.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/angrmanagement/vendor/qtconsole/util.py` & `angr-management-9.2.97/angrmanagement/vendor/qtconsole/util.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/pyproject.toml` & `angr-management-9.2.97/pyproject.toml`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/setup.cfg` & `angr-management-9.2.97/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find:
 install_requires = 
-	PySide6>=6.4.2,<=6.6.1
-	PySide6-QtAds
+	PySide6>=6.4.2
+	PySide6-QtAds>=4.2.1
 	QtAwesome
 	QtPy
-	angr[angrDB]==9.2.96
+	angr[angrDB]==9.2.97
 	bidict
 	ipython
 	pyqodeng>=0.0.10
 	requests[socks]
 	tomlkit
 	pyobjc-framework-Cocoa;platform_system == "Darwin"
 	thefuzz[speedup]
@@ -47,15 +47,15 @@
 [options.extras_require]
 bintrace = 
 	bintrace
 pyinstaller = 
 	pyinstaller==6.5.0
 	pillow;platform_system == "Darwin"
 	keystone-engine
-	archr==9.2.96;platform_system == "Linux"
+	archr==9.2.97;platform_system == "Linux"
 
 [options.package_data]
 angrmanagement = 
 	plugins/**/plugin.toml
 	resources/fonts/*.ttf
 	resources/images/*
 	resources/themes/**/*
```

### Comparing `angr-management-9.2.96/tests/test_qaddress_input.py` & `angr-management-9.2.97/tests/test_qaddress_input.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/tests/test_rename_functions.py` & `angr-management-9.2.97/tests/test_rename_functions.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/tests/test_rename_variables.py` & `angr-management-9.2.97/tests/test_rename_variables.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/tests/test_tagged_interval_map.py` & `angr-management-9.2.97/tests/test_tagged_interval_map.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.96/tests/test_workflow.py` & `angr-management-9.2.97/tests/test_workflow.py`

 * *Files identical despite different names*

