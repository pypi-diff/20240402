# Comparing `tmp/libbs-1.1.0.tar.gz` & `tmp/libbs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbs-1.1.0.tar", last modified: Sat Mar 30 20:44:08 2024, max compression
+gzip compressed data, was "libbs-1.2.0.tar", last modified: Tue Apr  2 03:36:46 2024, max compression
```

## Comparing `libbs-1.1.0.tar` & `libbs-1.2.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.235860 libbs-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-30 20:44:04.000000 libbs-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-03-30 20:44:08.235860 libbs-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-03-30 20:44:04.000000 libbs-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.223860 libbs-1.1.0/libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.223860 libbs-1.1.0/libbs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/api/artifact_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/api/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/api/decompiler_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/api/type_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.227860 libbs-1.1.0/libbs/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/artifacts/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/artifacts/decompilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/artifacts/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/artifacts/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/artifacts/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/artifacts/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/artifacts/stack_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/artifacts/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.227860 libbs-1.1.0/libbs/decompiler_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompiler_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.227860 libbs-1.1.0/libbs/decompiler_stubs/angr_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompiler_stubs/angr_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.227860 libbs-1.1.0/libbs/decompiler_stubs/binja_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompiler_stubs/binja_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.227860 libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.227860 libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.227860 libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompiler_stubs/ida_libbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.227860 libbs-1.1.0/libbs/decompilers/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.227860 libbs-1.1.0/libbs/decompilers/angr/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/angr/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/angr/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/angr/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.231860 libbs-1.1.0/libbs/decompilers/binja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/binja/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/binja/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/binja/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.231860 libbs-1.1.0/libbs/decompilers/ghidra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/ghidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/ghidra/artifact_lifter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.231860 libbs-1.1.0/libbs/decompilers/ghidra/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/ghidra/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/ghidra/compat/ghidra_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/ghidra/compat/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/ghidra/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    30407 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/ghidra/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.231860 libbs-1.1.0/libbs/decompilers/ida/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/ida/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/ida/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/ida/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/decompilers/ida/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/plugin_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.231860 libbs-1.1.0/libbs/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/ui/qt_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-30 20:44:04.000000 libbs-1.1.0/libbs/ui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.231860 libbs-1.1.0/libbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-03-30 20:44:08.000000 libbs-1.1.0/libbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-03-30 20:44:08.000000 libbs-1.1.0/libbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 20:44:08.000000 libbs-1.1.0/libbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-30 20:44:08.000000 libbs-1.1.0/libbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-30 20:44:08.000000 libbs-1.1.0/libbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-30 20:44:08.000000 libbs-1.1.0/libbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-30 20:44:08.235860 libbs-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-30 20:44:04.000000 libbs-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:44:08.231860 libbs-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-03-30 20:44:04.000000 libbs-1.1.0/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-03-30 20:44:04.000000 libbs-1.1.0/tests/test_decompilers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.006895 libbs-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-02 03:36:39.000000 libbs-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-02 03:36:46.006895 libbs-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-02 03:36:39.000000 libbs-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:45.994895 libbs-1.2.0/libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:45.998895 libbs-1.2.0/libbs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/api/artifact_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/api/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/api/decompiler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/api/type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:45.998895 libbs-1.2.0/libbs/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/decompilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/stack_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:45.998895 libbs-1.2.0/libbs/decompiler_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:45.998895 libbs-1.2.0/libbs/decompiler_stubs/angr_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/angr_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompiler_stubs/binja_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/binja_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ida_libbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompilers/angr/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/angr/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/angr/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/angr/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompilers/binja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/binja/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/binja/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/binja/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompilers/ghidra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/artifact_lifter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.006895 libbs-1.2.0/libbs/decompilers/ghidra/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/compat/ghidra_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/compat/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31335 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.006895 libbs-1.2.0/libbs/decompilers/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ida/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ida/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ida/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ida/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/plugin_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.006895 libbs-1.2.0/libbs/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/ui/qt_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/ui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.006895 libbs-1.2.0/libbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-02 03:36:45.000000 libbs-1.2.0/libbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-02 03:36:45.000000 libbs-1.2.0/libbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 03:36:45.000000 libbs-1.2.0/libbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 03:36:45.000000 libbs-1.2.0/libbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-02 03:36:45.000000 libbs-1.2.0/libbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 03:36:45.000000 libbs-1.2.0/libbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-02 03:36:46.006895 libbs-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 03:36:39.000000 libbs-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.006895 libbs-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-02 03:36:39.000000 libbs-1.2.0/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-02 03:36:39.000000 libbs-1.2.0/tests/test_decompilers.py
```

### Comparing `libbs-1.1.0/LICENSE` & `libbs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/PKG-INFO` & `libbs-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.1.0
+Version: 1.2.0
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
```

### Comparing `libbs-1.1.0/README.md` & `libbs-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/__main__.py` & `libbs-1.2.0/libbs/__main__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/api/artifact_dict.py` & `libbs-1.2.0/libbs/api/artifact_dict.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/api/artifact_lifter.py` & `libbs-1.2.0/libbs/api/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/api/decompiler_interface.py` & `libbs-1.2.0/libbs/api/decompiler_interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/api/type_parser.py` & `libbs-1.2.0/libbs/api/type_parser.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/api/utils.py` & `libbs-1.2.0/libbs/api/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/artifacts/artifact.py` & `libbs-1.2.0/libbs/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/artifacts/comment.py` & `libbs-1.2.0/libbs/artifacts/comment.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/artifacts/decompilation.py` & `libbs-1.2.0/libbs/artifacts/decompilation.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/artifacts/enum.py` & `libbs-1.2.0/libbs/artifacts/enum.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/artifacts/func.py` & `libbs-1.2.0/libbs/artifacts/func.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/artifacts/global_variable.py` & `libbs-1.2.0/libbs/artifacts/global_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/artifacts/patch.py` & `libbs-1.2.0/libbs/artifacts/patch.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/artifacts/stack_variable.py` & `libbs-1.2.0/libbs/artifacts/stack_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/artifacts/struct.py` & `libbs-1.2.0/libbs/artifacts/struct.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py` & `libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py` & `libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompilers/angr/artifact_lifter.py` & `libbs-1.2.0/libbs/decompilers/angr/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompilers/angr/compat.py` & `libbs-1.2.0/libbs/decompilers/angr/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompilers/angr/interface.py` & `libbs-1.2.0/libbs/decompilers/angr/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompilers/binja/artifact_lifter.py` & `libbs-1.2.0/libbs/decompilers/binja/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompilers/binja/hooks.py` & `libbs-1.2.0/libbs/decompilers/binja/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompilers/binja/interface.py` & `libbs-1.2.0/libbs/decompilers/binja/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompilers/ghidra/artifact_lifter.py` & `libbs-1.2.0/libbs/decompilers/ghidra/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompilers/ghidra/compat/ghidra_api.py` & `libbs-1.2.0/libbs/decompilers/ghidra/compat/ghidra_api.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompilers/ghidra/interface.py` & `libbs-1.2.0/libbs/decompilers/ghidra/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Function, FunctionHeader, StackVariable, Comment, FunctionArgument, GlobalVariable, Struct, StructMember, Enum
 )
 from libbs.plugin_installer import PluginInstaller
 import psutil
 
 from .artifact_lifter import GhidraArtifactLifter
 from .compat import GhidraAPIWrapper, Transaction
-from .hooks import create_context_action
+from .hooks import create_context_action, create_data_monitor
 
 _l = logging.getLogger(__name__)
 
 
 def ghidra_transaction(f):
     @wraps(f)
     def _ghidra_transaction(self: "GhidraDecompilerInterface", *args, **kwargs):
@@ -30,32 +30,51 @@
 
         return ret_val
 
     return _ghidra_transaction
 
 
 class GhidraDecompilerInterface(DecompilerInterface):
-    def __init__(self, loop_on_plugin=True, **kwargs):
+    def __init__(self, loop_on_plugin=True, start_headless_watchers=False, **kwargs):
         self.loop_on_plugin = loop_on_plugin
+        self._start_headless_watchers = start_headless_watchers
 
         self._last_addr = None
         self._last_func = None
         self.base_addr = None
 
         self._headless_g_project = None
         self._headless_script_name = "ghidra_libbs_mainthread_server.py"
 
+        self._data_monitor = None
+
         self.ghidra: Optional[GhidraAPIWrapper] = None
         super().__init__(name="ghidra", artifact_lifter=GhidraArtifactLifter(self), supports_undo=True, **kwargs)
 
     def _init_gui_components(self, *args, **kwargs):
         if not self.connect_ghidra_bridge():
             raise Exception("Failed to connect to the Ghidra Bridge. Check the Ghidra GUI for failures!")
         super()._init_gui_components(*args, **kwargs)
 
+    def start_artifact_watchers(self):
+        if not self._artifact_watchers_started:
+            if self.ghidra is None:
+                raise RuntimeError("Cannot start artifact watchers without Ghidra Bridge connection.")
+
+            self._data_monitor = create_data_monitor(self.ghidra, self)
+            self.ghidra.currentProgram.addListener(self._data_monitor)
+            # TODO: generalize superclass method?
+            super().start_artifact_watchers()
+
+    def stop_artifact_watchers(self):
+        if self._artifact_watchers_started:
+            self._data_monitor = None
+            # TODO: generalize superclass method?
+            super().stop_artifact_watchers()
+
     def _init_headless_components(self, *args, **kwargs):
         if self._headless_dec_path is None:
             # attempt to grab it from the env vars
             path = os.environ.get("GHIDRA_HEADLESS_PATH", None)
             if path:
                 self._headless_dec_path = Path(path).absolute()
 
@@ -77,14 +96,17 @@
             self._headless_script_name
         ])
 
         time.sleep(1)
         if not self.connect_ghidra_bridge():
             raise Exception(f"Failed to connect to the Ghidra Bridge. Check if the {self._headless_dec_path} binary was ever started.")
 
+        if self._start_headless_watchers:
+            self.start_artifact_watchers()
+
     def _find_headless_proc(self):
         for proc in psutil.process_iter():
             try:
                 cmd = " ".join(proc.cmdline())
             except Exception as e:
                 continue
 
@@ -486,15 +508,15 @@
     def fill_global_var(self, var_addr, user=None, artifact=None, **kwargs):
         """
         TODO: remove me and implement me properly as setters and getters
         """
 
         changes = False
         global_var: GlobalVariable = artifact
-        all_global_vars = self.global_vars()
+        all_global_vars = self._global_vars()
 
         rename_label_cmd_cls = self.ghidra.import_module_object("ghidra.app.cmd.label", "RenameLabelCmd")
         src_type = self.ghidra.import_module_object("ghidra.program.model.symbol", "SourceType")
         for offset, gvar in all_global_vars.items():
             if offset != var_addr:
                 continue
 
@@ -508,19 +530,19 @@
                 # TODO: set type
                 pass
 
             break
 
         return changes
 
-    def global_var(self, addr) -> Optional[GlobalVariable]:
+    def _get_global_var(self, addr) -> Optional[GlobalVariable]:
         """
         TODO: remove me and implement me properly as setters and getters
         """
-        light_global_vars = self.global_vars()
+        light_global_vars = self._global_vars()
         for offset, global_var in light_global_vars.items():
             if offset == addr:
                 lst = self.ghidra.currentProgram.getListing()
                 g_addr = self.ghidra.toAddr(addr)
                 data = lst.getDataAt(g_addr)
                 if not data or data.isStructure():
                     return None
@@ -528,15 +550,15 @@
                     size = self.ghidra.currentProgram.getDefaultPointerSize()
                 else:
                     size = data.getLength()
 
                 global_var.size = size
                 return global_var
 
-    def global_vars(self) -> Dict[int, GlobalVariable]:
+    def _global_vars(self) -> Dict[int, GlobalVariable]:
         """
         TODO: remove me and implement me properly as setters and getters
         """
         symbol_type = self.ghidra.import_module_object("ghidra.program.model.symbol", "SymbolType")
         symbol_table = self.ghidra.currentProgram.getSymbolTable()
         # optimize by grabbing all symbols at once
         gvar_addr_and_name: Optional[List[Tuple[str, int]]] = self.ghidra.bridge.remote_eval(
```

### Comparing `libbs-1.1.0/libbs/decompilers/ida/artifact_lifter.py` & `libbs-1.2.0/libbs/decompilers/ida/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompilers/ida/compat.py` & `libbs-1.2.0/libbs/decompilers/ida/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompilers/ida/hooks.py` & `libbs-1.2.0/libbs/decompilers/ida/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/decompilers/ida/interface.py` & `libbs-1.2.0/libbs/decompilers/ida/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/logger.py` & `libbs-1.2.0/libbs/logger.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/plugin_installer.py` & `libbs-1.2.0/libbs/plugin_installer.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/ui/__init__.py` & `libbs-1.2.0/libbs/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/ui/qt_objects.py` & `libbs-1.2.0/libbs/ui/qt_objects.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs/ui/utils.py` & `libbs-1.2.0/libbs/ui/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/libbs.egg-info/PKG-INFO` & `libbs-1.2.0/libbs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.1.0
+Version: 1.2.0
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
```

### Comparing `libbs-1.1.0/libbs.egg-info/SOURCES.txt` & `libbs-1.2.0/libbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/setup.cfg` & `libbs-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `libbs-1.1.0/tests/test_artifacts.py` & `libbs-1.2.0/tests/test_artifacts.py`

 * *Files identical despite different names*

