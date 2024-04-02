# Comparing `tmp/archr-9.2.96.tar.gz` & `tmp/archr-9.2.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archr-9.2.96.tar", last modified: Tue Mar 26 17:02:44 2024, max compression
+gzip compressed data, was "archr-9.2.97.tar", last modified: Tue Apr  2 17:03:08 2024, max compression
```

## Comparing `archr-9.2.96.tar` & `archr-9.2.97.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.317410 archr-9.2.96/
--rw-r--r--   0 vsts      (1001) docker     (127)     1308 2024-03-26 17:01:01.000000 archr-9.2.96/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)       34 2024-03-26 17:01:01.000000 archr-9.2.96/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     5414 2024-03-26 17:02:44.317410 archr-9.2.96/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     4578 2024-03-26 17:01:01.000000 archr-9.2.96/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.301411 archr-9.2.96/archr/
--rw-r--r--   0 vsts      (1001) docker     (127)      555 2024-03-26 17:01:08.000000 archr-9.2.96/archr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.305410 archr-9.2.96/archr/analyzers/
--rw-r--r--   0 vsts      (1001) docker     (127)     4928 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7902 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/angr_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5448 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/angr_state.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2512 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/angr_ultimate_tracer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6567 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/bintrace_qemu_tracer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1796 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9291 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/datascout.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3111 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/gdb.py
--rw-r--r--   0 vsts      (1001) docker     (127)      512 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/gdbserver.py
--rw-r--r--   0 vsts      (1001) docker     (127)      906 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/input_fd.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/ltrace.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17666 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/qemu_tracer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1192 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/qtrace.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9155 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/rr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2474 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/strace.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2632 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/tcpdump.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1119 2024-03-26 17:01:01.000000 archr-9.2.96/archr/analyzers/udp_tcp_convert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      218 2024-03-26 17:01:01.000000 archr-9.2.96/archr/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.305410 archr-9.2.96/archr/implants/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.305410 archr-9.2.96/archr/implants/GENERIC/
--rwxr-xr-x   0 vsts      (1001) docker     (127)      511 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/GENERIC/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (127)      150 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/GENERIC/fire
--rw-r--r--   0 vsts      (1001) docker     (127)      867 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.305410 archr-9.2.96/archr/implants/bintrace_qemu/
--rwxr-xr-x   0 vsts      (1001) docker     (127)      671 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/bintrace_qemu/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (127)      352 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/bintrace_qemu/fire
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.305410 archr-9.2.96/archr/implants/emurrate/
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1146 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/emurrate/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (127)      200 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/emurrate/fire
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.305410 archr-9.2.96/archr/implants/gdb/
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1184 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/gdb/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (127)      218 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/gdb/fire
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.305410 archr-9.2.96/archr/implants/gdbserver/
--rwxr-xr-x   0 vsts      (1001) docker     (127)      429 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/gdbserver/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (127)      147 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/gdbserver/fire
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.309410 archr-9.2.96/archr/implants/ltrace/
--rwxr-xr-x   0 vsts      (1001) docker     (127)      402 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/ltrace/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (127)      170 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/ltrace/fire
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.309410 archr-9.2.96/archr/implants/qtrace/
--rwxr-xr-x   0 vsts      (1001) docker     (127)      851 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/qtrace/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (127)      211 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/qtrace/fire
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.309410 archr-9.2.96/archr/implants/rr/
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1685 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/rr/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (127)      217 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/rr/fire
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.309410 archr-9.2.96/archr/implants/shellphish_qemu/
--rwxr-xr-x   0 vsts      (1001) docker     (127)      617 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/shellphish_qemu/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (127)       62 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/shellphish_qemu/fire
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.309410 archr-9.2.96/archr/implants/udp_tcp_convert/
--rw-r--r--   0 vsts      (1001) docker     (127)      380 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/udp_tcp_convert/CMakeLists.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      527 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/udp_tcp_convert/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (127)      188 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/udp_tcp_convert/fire
--rw-r--r--   0 vsts      (1001) docker     (127)     5728 2024-03-26 17:01:01.000000 archr-9.2.96/archr/implants/udp_tcp_convert/udp_to_tcp.c
--rw-r--r--   0 vsts      (1001) docker     (127)     6881 2024-03-26 17:01:01.000000 archr-9.2.96/archr/strace_parser.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.313410 archr-9.2.96/archr/targets/
--rw-r--r--   0 vsts      (1001) docker     (127)    15683 2024-03-26 17:01:01.000000 archr-9.2.96/archr/targets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4779 2024-03-26 17:01:01.000000 archr-9.2.96/archr/targets/actions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20190 2024-03-26 17:01:01.000000 archr-9.2.96/archr/targets/docker_target.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3479 2024-03-26 17:01:01.000000 archr-9.2.96/archr/targets/flight.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5019 2024-03-26 17:01:01.000000 archr-9.2.96/archr/targets/local_target.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8066 2024-03-26 17:01:01.000000 archr-9.2.96/archr/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.317410 archr-9.2.96/archr.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     5414 2024-03-26 17:02:44.000000 archr-9.2.96/archr.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2236 2024-03-26 17:02:44.000000 archr-9.2.96/archr.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-26 17:02:44.000000 archr-9.2.96/archr.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      147 2024-03-26 17:02:44.000000 archr-9.2.96/archr.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-03-26 17:02:44.000000 archr-9.2.96/archr.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      174 2024-03-26 17:01:08.000000 archr-9.2.96/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-03-26 17:02:44.317410 archr-9.2.96/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     2508 2024-03-26 17:01:01.000000 archr-9.2.96/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:44.313410 archr-9.2.96/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)    10654 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_analyzer_angr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2776 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_analyzer_bintrace_qemu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      845 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_analyzer_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4350 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_analyzer_datascout.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1464 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_analyzer_gdbserver.py
--rw-r--r--   0 vsts      (1001) docker     (127)      730 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_analyzer_inputfd.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2661 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_analyzer_ltrace.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4725 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_analyzer_qemu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_analyzer_qtrace.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1143 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_analyzer_rr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2223 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_analyzer_strace.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1272 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_analyzer_udp_tcp_convert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      905 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_angr_tracing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1295 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_angr_ultimate_tracer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6046 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_dockertarget_fs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3753 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_dockertarget_simple.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1936 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_localtarget_simple.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1132 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_shellcode_hook.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4558 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_sync.py
--rw-r--r--   0 vsts      (1001) docker     (127)      693 2024-03-26 17:01:01.000000 archr-9.2.96/tests/test_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.598536 archr-9.2.97/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1308 2024-04-02 17:01:39.000000 archr-9.2.97/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)       34 2024-04-02 17:01:39.000000 archr-9.2.97/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     5414 2024-04-02 17:03:08.598536 archr-9.2.97/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     4578 2024-04-02 17:01:39.000000 archr-9.2.97/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.582536 archr-9.2.97/archr/
+-rw-r--r--   0 vsts      (1001) docker     (127)      555 2024-04-02 17:01:44.000000 archr-9.2.97/archr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.586536 archr-9.2.97/archr/analyzers/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4928 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7902 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/angr_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5448 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/angr_state.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2512 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/angr_ultimate_tracer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6567 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/bintrace_qemu_tracer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1796 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9291 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/datascout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3111 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/gdb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      512 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/gdbserver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      906 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/input_fd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/ltrace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17666 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/qemu_tracer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1192 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/qtrace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9155 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/rr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2474 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/strace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2632 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/tcpdump.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1119 2024-04-02 17:01:39.000000 archr-9.2.97/archr/analyzers/udp_tcp_convert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      218 2024-04-02 17:01:39.000000 archr-9.2.97/archr/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.586536 archr-9.2.97/archr/implants/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.586536 archr-9.2.97/archr/implants/GENERIC/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      511 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/GENERIC/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      150 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/GENERIC/fire
+-rw-r--r--   0 vsts      (1001) docker     (127)      867 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.590536 archr-9.2.97/archr/implants/bintrace_qemu/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      671 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/bintrace_qemu/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      352 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/bintrace_qemu/fire
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.590536 archr-9.2.97/archr/implants/emurrate/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1146 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/emurrate/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      200 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/emurrate/fire
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.590536 archr-9.2.97/archr/implants/gdb/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1184 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/gdb/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      218 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/gdb/fire
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.590536 archr-9.2.97/archr/implants/gdbserver/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      429 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/gdbserver/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      147 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/gdbserver/fire
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.590536 archr-9.2.97/archr/implants/ltrace/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      402 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/ltrace/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      170 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/ltrace/fire
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.590536 archr-9.2.97/archr/implants/qtrace/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      851 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/qtrace/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      211 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/qtrace/fire
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.590536 archr-9.2.97/archr/implants/rr/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1685 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/rr/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      217 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/rr/fire
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.590536 archr-9.2.97/archr/implants/shellphish_qemu/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      617 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/shellphish_qemu/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (127)       62 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/shellphish_qemu/fire
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.590536 archr-9.2.97/archr/implants/udp_tcp_convert/
+-rw-r--r--   0 vsts      (1001) docker     (127)      380 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/udp_tcp_convert/CMakeLists.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      527 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/udp_tcp_convert/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      188 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/udp_tcp_convert/fire
+-rw-r--r--   0 vsts      (1001) docker     (127)     5728 2024-04-02 17:01:39.000000 archr-9.2.97/archr/implants/udp_tcp_convert/udp_to_tcp.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     6881 2024-04-02 17:01:39.000000 archr-9.2.97/archr/strace_parser.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.594536 archr-9.2.97/archr/targets/
+-rw-r--r--   0 vsts      (1001) docker     (127)    15683 2024-04-02 17:01:39.000000 archr-9.2.97/archr/targets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4779 2024-04-02 17:01:39.000000 archr-9.2.97/archr/targets/actions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20190 2024-04-02 17:01:39.000000 archr-9.2.97/archr/targets/docker_target.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3479 2024-04-02 17:01:39.000000 archr-9.2.97/archr/targets/flight.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5019 2024-04-02 17:01:39.000000 archr-9.2.97/archr/targets/local_target.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8066 2024-04-02 17:01:39.000000 archr-9.2.97/archr/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.598536 archr-9.2.97/archr.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5414 2024-04-02 17:03:08.000000 archr-9.2.97/archr.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2236 2024-04-02 17:03:08.000000 archr-9.2.97/archr.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-02 17:03:08.000000 archr-9.2.97/archr.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      147 2024-04-02 17:03:08.000000 archr-9.2.97/archr.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-02 17:03:08.000000 archr-9.2.97/archr.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      174 2024-04-02 17:01:44.000000 archr-9.2.97/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-04-02 17:03:08.598536 archr-9.2.97/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     2508 2024-04-02 17:01:39.000000 archr-9.2.97/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:03:08.598536 archr-9.2.97/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10654 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_analyzer_angr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2776 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_analyzer_bintrace_qemu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      845 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_analyzer_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4350 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_analyzer_datascout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1464 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_analyzer_gdbserver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      730 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_analyzer_inputfd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2661 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_analyzer_ltrace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4725 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_analyzer_qemu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_analyzer_qtrace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1143 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_analyzer_rr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2223 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_analyzer_strace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1272 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_analyzer_udp_tcp_convert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      905 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_angr_tracing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1295 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_angr_ultimate_tracer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6046 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_dockertarget_fs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3753 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_dockertarget_simple.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1936 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_localtarget_simple.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1132 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_shellcode_hook.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4558 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_sync.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      693 2024-04-02 17:01:39.000000 archr-9.2.97/tests/test_utils.py
```

### Comparing `archr-9.2.96/LICENSE` & `archr-9.2.97/LICENSE`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/PKG-INFO` & `archr-9.2.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: archr
-Version: 9.2.96
+Version: 9.2.97
 Summary: Target-centric program analysis.
 Home-page: https://github.com/angr/archr
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cle==9.2.96
+Requires-Dist: cle==9.2.97
 Requires-Dist: docker
 Requires-Dist: nclib>=1.0.0rc3
 Requires-Dist: patchelf-wrapper
 Requires-Dist: ply
 Requires-Dist: pygdbmi
 Requires-Dist: shellphish-qemu>=0.12.2
 Provides-Extra: angr
-Requires-Dist: angr==9.2.96; extra == "angr"
+Requires-Dist: angr==9.2.97; extra == "angr"
 Provides-Extra: bintrace
 Requires-Dist: bintrace; extra == "bintrace"
 Provides-Extra: qtrace
 Requires-Dist: qtrace; extra == "qtrace"
 
 # archr
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `archr-9.2.96/README.md` & `archr-9.2.97/README.md`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/__init__.py` & `archr-9.2.97/archr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "9.2.96"
+__version__ = "9.2.97"
 
 import logging
 
 _LOG = logging.getLogger("archr")
 
 try:
     import angr
```

### Comparing `archr-9.2.96/archr/analyzers/__init__.py` & `archr-9.2.97/archr/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/angr_project.py` & `archr-9.2.97/archr/analyzers/angr_project.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/angr_state.py` & `archr-9.2.97/archr/analyzers/angr_state.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/angr_ultimate_tracer.py` & `archr-9.2.97/archr/analyzers/angr_ultimate_tracer.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/bintrace_qemu_tracer.py` & `archr-9.2.97/archr/analyzers/bintrace_qemu_tracer.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/core.py` & `archr-9.2.97/archr/analyzers/core.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/datascout.py` & `archr-9.2.97/archr/analyzers/datascout.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/gdb.py` & `archr-9.2.97/archr/analyzers/gdb.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/gdbserver.py` & `archr-9.2.97/archr/analyzers/gdbserver.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/input_fd.py` & `archr-9.2.97/archr/analyzers/input_fd.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/ltrace.py` & `archr-9.2.97/archr/analyzers/ltrace.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/qemu_tracer.py` & `archr-9.2.97/archr/analyzers/qemu_tracer.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/qtrace.py` & `archr-9.2.97/archr/analyzers/qtrace.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/rr.py` & `archr-9.2.97/archr/analyzers/rr.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/strace.py` & `archr-9.2.97/archr/analyzers/strace.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/tcpdump.py` & `archr-9.2.97/archr/analyzers/tcpdump.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/analyzers/udp_tcp_convert.py` & `archr-9.2.97/archr/analyzers/udp_tcp_convert.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/implants/__init__.py` & `archr-9.2.97/archr/implants/__init__.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/implants/bintrace_qemu/bundle` & `archr-9.2.97/archr/implants/bintrace_qemu/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/implants/emurrate/bundle` & `archr-9.2.97/archr/implants/emurrate/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/implants/gdb/bundle` & `archr-9.2.97/archr/implants/gdb/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/implants/qtrace/bundle` & `archr-9.2.97/archr/implants/qtrace/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/implants/rr/bundle` & `archr-9.2.97/archr/implants/rr/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/implants/shellphish_qemu/bundle` & `archr-9.2.97/archr/implants/shellphish_qemu/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/implants/udp_tcp_convert/bundle` & `archr-9.2.97/archr/implants/udp_tcp_convert/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/implants/udp_tcp_convert/udp_to_tcp.c` & `archr-9.2.97/archr/implants/udp_tcp_convert/udp_to_tcp.c`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/strace_parser.py` & `archr-9.2.97/archr/strace_parser.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/targets/__init__.py` & `archr-9.2.97/archr/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/targets/actions.py` & `archr-9.2.97/archr/targets/actions.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/targets/docker_target.py` & `archr-9.2.97/archr/targets/docker_target.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/targets/flight.py` & `archr-9.2.97/archr/targets/flight.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/targets/local_target.py` & `archr-9.2.97/archr/targets/local_target.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr/utils.py` & `archr-9.2.97/archr/utils.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/archr.egg-info/PKG-INFO` & `archr-9.2.97/archr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: archr
-Version: 9.2.96
+Version: 9.2.97
 Summary: Target-centric program analysis.
 Home-page: https://github.com/angr/archr
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cle==9.2.96
+Requires-Dist: cle==9.2.97
 Requires-Dist: docker
 Requires-Dist: nclib>=1.0.0rc3
 Requires-Dist: patchelf-wrapper
 Requires-Dist: ply
 Requires-Dist: pygdbmi
 Requires-Dist: shellphish-qemu>=0.12.2
 Provides-Extra: angr
-Requires-Dist: angr==9.2.96; extra == "angr"
+Requires-Dist: angr==9.2.97; extra == "angr"
 Provides-Extra: bintrace
 Requires-Dist: bintrace; extra == "bintrace"
 Provides-Extra: qtrace
 Requires-Dist: qtrace; extra == "qtrace"
 
 # archr
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `archr-9.2.96/archr.egg-info/SOURCES.txt` & `archr-9.2.97/archr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/setup.cfg` & `archr-9.2.97/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find:
 install_requires = 
-	cle==9.2.96
+	cle==9.2.97
 	docker
 	nclib>=1.0.0rc3
 	patchelf-wrapper
 	ply
 	pygdbmi
 	shellphish-qemu>=0.12.2
 python_requires = >=3.8
 include_package_data = True
 
 [options.extras_require]
 angr = 
-	angr==9.2.96
+	angr==9.2.97
 bintrace = 
 	bintrace
 qtrace = 
 	qtrace
 
 [options.package_data]
 archr =
```

### Comparing `archr-9.2.96/setup.py` & `archr-9.2.97/setup.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_analyzer_angr.py` & `archr-9.2.97/tests/test_analyzer_angr.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_analyzer_bintrace_qemu.py` & `archr-9.2.97/tests/test_analyzer_bintrace_qemu.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_analyzer_core.py` & `archr-9.2.97/tests/test_analyzer_core.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_analyzer_datascout.py` & `archr-9.2.97/tests/test_analyzer_datascout.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_analyzer_gdbserver.py` & `archr-9.2.97/tests/test_analyzer_gdbserver.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_analyzer_inputfd.py` & `archr-9.2.97/tests/test_analyzer_inputfd.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_analyzer_ltrace.py` & `archr-9.2.97/tests/test_analyzer_ltrace.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_analyzer_qemu.py` & `archr-9.2.97/tests/test_analyzer_qemu.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_analyzer_qtrace.py` & `archr-9.2.97/tests/test_analyzer_qtrace.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_analyzer_rr.py` & `archr-9.2.97/tests/test_analyzer_rr.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_analyzer_strace.py` & `archr-9.2.97/tests/test_analyzer_strace.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_analyzer_udp_tcp_convert.py` & `archr-9.2.97/tests/test_analyzer_udp_tcp_convert.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_angr_tracing.py` & `archr-9.2.97/tests/test_angr_tracing.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_angr_ultimate_tracer.py` & `archr-9.2.97/tests/test_angr_ultimate_tracer.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_dockertarget_fs.py` & `archr-9.2.97/tests/test_dockertarget_fs.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_dockertarget_simple.py` & `archr-9.2.97/tests/test_dockertarget_simple.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_localtarget_simple.py` & `archr-9.2.97/tests/test_localtarget_simple.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_shellcode_hook.py` & `archr-9.2.97/tests/test_shellcode_hook.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_sync.py` & `archr-9.2.97/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.96/tests/test_utils.py` & `archr-9.2.97/tests/test_utils.py`

 * *Files identical despite different names*

