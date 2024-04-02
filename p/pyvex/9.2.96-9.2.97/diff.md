# Comparing `tmp/pyvex-9.2.96.tar.gz` & `tmp/pyvex-9.2.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvex-9.2.96.tar", last modified: Tue Mar 26 17:01:39 2024, max compression
+gzip compressed data, was "pyvex-9.2.97.tar", last modified: Tue Apr  2 17:02:05 2024, max compression
```

## Comparing `pyvex-9.2.96.tar` & `pyvex-9.2.97.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.726004 pyvex-9.2.96/
--rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-03-26 17:00:55.000000 pyvex-9.2.96/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-03-26 17:00:55.000000 pyvex-9.2.96/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10117 2024-03-26 17:01:39.726004 pyvex-9.2.96/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8959 2024-03-26 17:00:55.000000 pyvex-9.2.96/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (127)     5136 2024-03-26 17:00:55.000000 pyvex-9.2.96/make_ffi.py
--rw-r--r--   0 vsts      (1001) docker     (127)      279 2024-03-26 17:01:09.000000 pyvex-9.2.96/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.650004 pyvex-9.2.96/pyvex/
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-03-26 17:01:09.000000 pyvex-9.2.96/pyvex/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49630 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/_register_info.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3695 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/arches.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24800 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/block.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9356 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/const.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1733 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/data_ref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4487 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1191 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/errors.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25727 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/expr.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.650004 pyvex-9.2.96/pyvex/lifting/
--rw-r--r--   0 vsts      (1001) docker     (127)      689 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.654004 pyvex-9.2.96/pyvex/lifting/gym/
--rw-r--r--   0 vsts      (1001) docker     (127)      204 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/gym/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1220 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/gym/aarch64_spotter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14999 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/gym/arm_spotter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4067 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/gym/x86_spotter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3665 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/libvex.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12832 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/lift_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5775 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/lifter.py
--rw-r--r--   0 vsts      (1001) docker     (127)      289 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/post_processor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.654004 pyvex-9.2.96/pyvex/lifting/util/
--rw-r--r--   0 vsts      (1001) docker     (127)      300 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17912 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/util/instr_helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5293 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/util/lifter_helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8824 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/util/syntax_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10080 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/util/vex_helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2580 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/lifting/zerodivision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2223 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/native.py
--rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)    22097 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/stmt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1040 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/types.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1415 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.722004 pyvex-9.2.96/pyvex.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10117 2024-03-26 17:01:39.000000 pyvex-9.2.96/pyvex.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     6212 2024-03-26 17:01:39.000000 pyvex-9.2.96/pyvex.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-26 17:01:39.000000 pyvex-9.2.96/pyvex.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      173 2024-03-26 17:01:39.000000 pyvex-9.2.96/pyvex.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-03-26 17:01:39.000000 pyvex-9.2.96/pyvex.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.654004 pyvex-9.2.96/pyvex_c/
--rw-r--r--   0 vsts      (1001) docker     (127)    18092 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex_c/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     1531 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex_c/Makefile
--rw-r--r--   0 vsts      (1001) docker     (127)      351 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex_c/Makefile-msvc
--rw-r--r--   0 vsts      (1001) docker     (127)    22449 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex_c/analysis.c
--rw-r--r--   0 vsts      (1001) docker     (127)     2765 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex_c/e4c_lite.h
--rw-r--r--   0 vsts      (1001) docker     (127)      794 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex_c/logging.c
--rw-r--r--   0 vsts      (1001) docker     (127)      226 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex_c/logging.h
--rw-r--r--   0 vsts      (1001) docker     (127)    12044 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex_c/postprocess.c
--rw-r--r--   0 vsts      (1001) docker     (127)    10990 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex_c/pyvex.c
--rw-r--r--   0 vsts      (1001) docker     (127)      923 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex_c/pyvex.def
--rw-r--r--   0 vsts      (1001) docker     (127)     1688 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex_c/pyvex.h
--rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-03-26 17:00:55.000000 pyvex-9.2.96/pyvex_c/pyvex_internal.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-03-26 17:01:39.726004 pyvex-9.2.96/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     4972 2024-03-26 17:00:55.000000 pyvex-9.2.96/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.658004 pyvex-9.2.96/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)     9771 2024-03-26 17:00:55.000000 pyvex-9.2.96/tests/test_arm_postprocess.py
--rw-r--r--   0 vsts      (1001) docker     (127)      883 2024-03-26 17:00:55.000000 pyvex-9.2.96/tests/test_gym.py
--rw-r--r--   0 vsts      (1001) docker     (127)      728 2024-03-26 17:00:55.000000 pyvex-9.2.96/tests/test_irsb_property_caching.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3263 2024-03-26 17:00:55.000000 pyvex-9.2.96/tests/test_lift.py
--rw-r--r--   0 vsts      (1001) docker     (127)      638 2024-03-26 17:00:55.000000 pyvex-9.2.96/tests/test_mips32_postprocess.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15877 2024-03-26 17:00:55.000000 pyvex-9.2.96/tests/test_pyvex.py
--rw-r--r--   0 vsts      (1001) docker     (127)      694 2024-03-26 17:00:55.000000 pyvex-9.2.96/tests/test_s390x_exrl.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-03-26 17:00:55.000000 pyvex-9.2.96/tests/test_s390x_lochi.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)      449 2024-03-26 17:00:55.000000 pyvex-9.2.96/tests/test_s390x_vl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3367 2024-03-26 17:00:55.000000 pyvex-9.2.96/tests/test_spotter.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-03-26 17:00:55.000000 pyvex-9.2.96/tests/test_ud2.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.658004 pyvex-9.2.96/vex/
--rw-r--r--   0 vsts      (1001) docker     (127)       28 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/.git
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.642004 pyvex-9.2.96/vex/.github/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.662004 pyvex-9.2.96/vex/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 vsts      (1001) docker     (127)     2230 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      205 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1734 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1293 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/.github/ISSUE_TEMPLATE/question.yml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.662004 pyvex-9.2.96/vex/.github/workflows/
--rw-r--r--   0 vsts      (1001) docker     (127)      838 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/.github/workflows/build.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (127)      176 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/HACKING.README
--rw-r--r--   0 vsts      (1001) docker     (127)    18011 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/LICENSE.GPL
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/LICENSE.README
--rw-r--r--   0 vsts      (1001) docker     (127)     5157 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/Makefile-gcc
--rw-r--r--   0 vsts      (1001) docker     (127)     1211 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/Makefile-msvc
--rw-r--r--   0 vsts      (1001) docker     (127)      133 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)     1028 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/TODO.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.662004 pyvex-9.2.96/vex/auxprogs/
--rw-r--r--   0 vsts      (1001) docker     (127)    33667 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/auxprogs/genoffsets.c
--rw-r--r--   0 vsts      (1001) docker     (127)     2999 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/common.mk
--rw-r--r--   0 vsts      (1001) docker     (127)      430 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/nanoarm.orig
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.662004 pyvex-9.2.96/vex/orig_amd64/
--rw-r--r--   0 vsts      (1001) docker     (127)     1612 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_amd64/Compare.hs
--rw-r--r--   0 vsts      (1001) docker     (127)      580 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_amd64/SortedToOrig.hs
--rw-r--r--   0 vsts      (1001) docker     (127)    77851 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_amd64/test1.orig
--rw-r--r--   0 vsts      (1001) docker     (127)    64255 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_amd64/test1.sorted
--rw-r--r--   0 vsts      (1001) docker     (127)   349947 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_amd64/test2.orig
--rw-r--r--   0 vsts      (1001) docker     (127)   349312 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_amd64/test2.sorted
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.662004 pyvex-9.2.96/vex/orig_arm/
--rw-r--r--   0 vsts      (1001) docker     (127)      359 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_arm/nanoarm
--rw-r--r--   0 vsts      (1001) docker     (127)      430 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_arm/nanoarm.orig
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.670004 pyvex-9.2.96/vex/orig_ppc32/
--rw-r--r--   0 vsts      (1001) docker     (127)  3443743 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_ppc32/date.orig
--rw-r--r--   0 vsts      (1001) docker     (127)  1156810 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_ppc32/loadsafp.orig
--rw-r--r--   0 vsts      (1001) docker     (127)   212994 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_ppc32/morefp.orig
--rw-r--r--   0 vsts      (1001) docker     (127)  1511720 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_ppc32/return0.orig
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.674004 pyvex-9.2.96/vex/orig_x86/
--rw-r--r--   0 vsts      (1001) docker     (127)   420476 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_x86/exit42.orig
--rw-r--r--   0 vsts      (1001) docker     (127)   869782 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_x86/fpu_mmx_sse.orig
--rw-r--r--   0 vsts      (1001) docker     (127)   426379 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/orig_x86/manyfp.orig
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.710004 pyvex-9.2.96/vex/priv/
--rw-r--r--   0 vsts      (1001) docker     (127)    23305 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_amd64_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)   158809 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_amd64_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (127)  1197373 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_amd64_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (127)    13043 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_arm64_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)    68566 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_arm64_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (127)   552369 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_arm64_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (127)    12853 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_arm_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)    50250 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_arm_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (127)   882026 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_arm_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (127)    50108 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_generic_bb_to_IR.c
--rw-r--r--   0 vsts      (1001) docker     (127)     7961 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_generic_bb_to_IR.h
--rw-r--r--   0 vsts      (1001) docker     (127)    39860 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_generic_x87.c
--rw-r--r--   0 vsts      (1001) docker     (127)     4929 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_generic_x87.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6065 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_mips_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)    29340 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_mips_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (127)   807179 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_mips_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (127)     6731 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_ppc_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)    34775 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_ppc_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (127)  1130268 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_ppc_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (127)     7656 2024-03-26 17:00:56.000000 pyvex-9.2.96/vex/priv/guest_riscv64_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)    21925 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/guest_riscv64_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (127)   136757 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/guest_riscv64_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (127)    17479 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/guest_s390_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)   101697 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/guest_s390_helpers.c
--rwxr-xr-x   0 vsts      (1001) docker     (127)    10118 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/guest_s390_insn_formats.py
--rw-r--r--   0 vsts      (1001) docker     (127)   727610 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/guest_s390_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (127)     4954 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/guest_tilegx_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)    20766 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/guest_tilegx_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (127)    79947 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/guest_tilegx_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (127)    16605 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/guest_x86_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)   100948 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/guest_x86_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (127)   552922 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/guest_x86_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (127)   145172 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_amd64_defs.c
--rw-r--r--   0 vsts      (1001) docker     (127)    30093 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_amd64_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)   191170 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_amd64_isel.c
--rw-r--r--   0 vsts      (1001) docker     (127)   218996 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_arm64_defs.c
--rw-r--r--   0 vsts      (1001) docker     (127)    37441 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_arm64_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)   163347 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_arm64_isel.c
--rw-r--r--   0 vsts      (1001) docker     (127)   183248 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_arm_defs.c
--rw-r--r--   0 vsts      (1001) docker     (127)    35420 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_arm_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)   257988 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_arm_isel.c
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_generic_maddf.c
--rw-r--r--   0 vsts      (1001) docker     (127)     1870 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_generic_maddf.h
--rw-r--r--   0 vsts      (1001) docker     (127)    60281 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_generic_reg_alloc2.c
--rw-r--r--   0 vsts      (1001) docker     (127)    55387 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_generic_reg_alloc3.c
--rw-r--r--   0 vsts      (1001) docker     (127)    11727 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_generic_regs.c
--rw-r--r--   0 vsts      (1001) docker     (127)    17459 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_generic_regs.h
--rw-r--r--   0 vsts      (1001) docker     (127)    13196 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_generic_simd128.c
--rw-r--r--   0 vsts      (1001) docker     (127)     3773 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_generic_simd128.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2155 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_generic_simd256.c
--rw-r--r--   0 vsts      (1001) docker     (127)     2066 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_generic_simd256.h
--rw-r--r--   0 vsts      (1001) docker     (127)    43649 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_generic_simd64.c
--rw-r--r--   0 vsts      (1001) docker     (127)     7296 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_generic_simd64.h
--rw-r--r--   0 vsts      (1001) docker     (127)   131651 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_mips_defs.c
--rw-r--r--   0 vsts      (1001) docker     (127)    26553 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_mips_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)   151524 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_mips_isel.c
--rw-r--r--   0 vsts      (1001) docker     (127)   231014 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_ppc_defs.c
--rw-r--r--   0 vsts      (1001) docker     (127)    43619 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_ppc_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)   266473 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_ppc_isel.c
--rw-r--r--   0 vsts      (1001) docker     (127)    91833 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_riscv64_defs.c
--rw-r--r--   0 vsts      (1001) docker     (127)    30525 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_riscv64_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)    74222 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_riscv64_isel.c
--rw-r--r--   0 vsts      (1001) docker     (127)   329366 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_s390_defs.c
--rw-r--r--   0 vsts      (1001) docker     (127)    34560 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_s390_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)   174718 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_s390_isel.c
--rw-r--r--   0 vsts      (1001) docker     (127)    76788 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_tilegx_defs.c
--rw-r--r--   0 vsts      (1001) docker     (127)    20244 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_tilegx_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)    56164 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_tilegx_isel.c
--rw-r--r--   0 vsts      (1001) docker     (127)   120030 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_x86_defs.c
--rw-r--r--   0 vsts      (1001) docker     (127)    26278 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_x86_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)   164986 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/host_x86_isel.c
--rw-r--r--   0 vsts      (1001) docker     (127)   190764 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/ir_defs.c
--rw-r--r--   0 vsts      (1001) docker     (127)    10919 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/ir_inject.c
--rw-r--r--   0 vsts      (1001) docker     (127)     3802 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/ir_match.c
--rw-r--r--   0 vsts      (1001) docker     (127)     3145 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/ir_match.h
--rw-r--r--   0 vsts      (1001) docker     (127)   231011 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/ir_opt.c
--rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/ir_opt.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2179 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/main_globals.c
--rw-r--r--   0 vsts      (1001) docker     (127)     2803 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/main_globals.h
--rw-r--r--   0 vsts      (1001) docker     (127)    86049 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/main_main.c
--rw-r--r--   0 vsts      (1001) docker     (127)    18330 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/main_util.c
--rw-r--r--   0 vsts      (1001) docker     (127)     5861 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/main_util.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3163 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/multiarch_main_main.c
--rw-r--r--   0 vsts      (1001) docker     (127)     6083 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/s390_defs.h
--rw-r--r--   0 vsts      (1001) docker     (127)    14758 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/s390_disasm.c
--rw-r--r--   0 vsts      (1001) docker     (127)     3277 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/s390_disasm.h
--rw-r--r--   0 vsts      (1001) docker     (127)   180250 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/tilegx_disasm.c
--rw-r--r--   0 vsts      (1001) docker     (127)    28210 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/priv/tilegx_disasm.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.714004 pyvex-9.2.96/vex/pub/
--rw-r--r--   0 vsts      (1001) docker     (127)    41851 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6612 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_basictypes.h
--rw-r--r--   0 vsts      (1001) docker     (127)     4889 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_emnote.h
--rw-r--r--   0 vsts      (1001) docker     (127)     8942 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_guest_amd64.h
--rw-r--r--   0 vsts      (1001) docker     (127)     7926 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_guest_arm.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6526 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_guest_arm64.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6330 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_guest_mips32.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6397 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_guest_mips64.h
--rw-r--r--   0 vsts      (1001) docker     (127)    11695 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_guest_ppc32.h
--rw-r--r--   0 vsts      (1001) docker     (127)    13411 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_guest_ppc64.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5098 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_guest_riscv64.h
--rw-r--r--   0 vsts      (1001) docker     (127)     7258 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_guest_s390x.h
--rw-r--r--   0 vsts      (1001) docker     (127)     4896 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_guest_tilegx.h
--rw-r--r--   0 vsts      (1001) docker     (127)    12432 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_guest_x86.h
--rw-r--r--   0 vsts      (1001) docker     (127)   122287 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_ir.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5025 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_s390x_common.h
--rw-r--r--   0 vsts      (1001) docker     (127)     4451 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/pub/libvex_trc_values.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.714004 pyvex-9.2.96/vex/switchback/
--rw-r--r--   0 vsts      (1001) docker     (127)      257 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/switchback/Makefile
--rwxr-xr-x   0 vsts      (1001) docker     (127)     9974 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/switchback/binary_switchback.pl
--rw-r--r--   0 vsts      (1001) docker     (127)    45293 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/switchback/linker.c
--rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/switchback/linker.h
--rw-r--r--   0 vsts      (1001) docker     (127)    24229 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/switchback/switchback.c
--rw-r--r--   0 vsts      (1001) docker     (127)   184904 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/switchback/test_bzip2.c
--rw-r--r--   0 vsts      (1001) docker     (127)    53078 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/switchback/test_emfloat.c
--rw-r--r--   0 vsts      (1001) docker     (127)      286 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/switchback/test_hello.c
--rw-r--r--   0 vsts      (1001) docker     (127)   115291 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/switchback/test_ppc_jm1.c
--rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/switchback/test_simple.c
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.722004 pyvex-9.2.96/vex/test/
--rw-r--r--   0 vsts      (1001) docker     (127)      542 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/fldenv.c
--rw-r--r--   0 vsts      (1001) docker     (127)      224 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/fp1.c
--rw-r--r--   0 vsts      (1001) docker     (127)      792 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/fp1.s
--rw-r--r--   0 vsts      (1001) docker     (127)     1572 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/fpconst.c
--rw-r--r--   0 vsts      (1001) docker     (127)     1451 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/fpgames.s
--rw-r--r--   0 vsts      (1001) docker     (127)      555 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/fpspeed.c
--rw-r--r--   0 vsts      (1001) docker     (127)      660 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/fpucw.c
--rw-r--r--   0 vsts      (1001) docker     (127)     1906 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/frstor.c
--rw-r--r--   0 vsts      (1001) docker     (127)     1557 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/fsave.c
--rw-r--r--   0 vsts      (1001) docker     (127)      393 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/fstenv.c
--rw-r--r--   0 vsts      (1001) docker     (127)     3462 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/fxsave.c
--rw-r--r--   0 vsts      (1001) docker     (127)    20405 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/mmxtest.c
--rw-r--r--   0 vsts      (1001) docker     (127)      694 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/mxcsr.c
--rw-r--r--   0 vsts      (1001) docker     (127)     2169 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/rounderr.c
--rw-r--r--   0 vsts      (1001) docker     (127)     2157 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/test-amd64-muldiv.h
--rw-r--r--   0 vsts      (1001) docker     (127)     4715 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/test-amd64-shift.h
--rw-r--r--   0 vsts      (1001) docker     (127)    45441 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/test-amd64.c
--rw-r--r--   0 vsts      (1001) docker     (127)     6381 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/test-amd64.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1521 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/test-i386-muldiv.h
--rw-r--r--   0 vsts      (1001) docker     (127)     4022 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/test-i386-shift.h
--rw-r--r--   0 vsts      (1001) docker     (127)    44331 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/test-i386.c
--rw-r--r--   0 vsts      (1001) docker     (127)     5372 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/test-i386.h
--rw-r--r--   0 vsts      (1001) docker     (127)      926 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/x87fxam.c
--rw-r--r--   0 vsts      (1001) docker     (127)      403 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/test/x87tst.c
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.722004 pyvex-9.2.96/vex/unused/
--rw-r--r--   0 vsts      (1001) docker     (127)     1593 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/unused/arena.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2502 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/unused/dispatch.c
--rw-r--r--   0 vsts      (1001) docker     (127)    43051 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/unused/linker.c
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:39.722004 pyvex-9.2.96/vex/useful/
--rw-r--r--   0 vsts      (1001) docker     (127)      235 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/useful/Makefile-vex
--rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/useful/cpuid.c
--rw-r--r--   0 vsts      (1001) docker     (127)    19175 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/useful/fp_80_64.c
--rw-r--r--   0 vsts      (1001) docker     (127)      191 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/useful/fpround.c
--rw-r--r--   0 vsts      (1001) docker     (127)      383 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/useful/fspill.c
--rw-r--r--   0 vsts      (1001) docker     (127)      201 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/useful/gradual_underflow.c
--rw-r--r--   0 vsts      (1001) docker     (127)    54111 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/useful/hd_fpu.c
--rw-r--r--   0 vsts      (1001) docker     (127)     4886 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/useful/show_fp_state.c
--rw-r--r--   0 vsts      (1001) docker     (127)     7171 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/useful/smchash.c
--rw-r--r--   0 vsts      (1001) docker     (127)    89474 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/useful/test_main.c
--rw-r--r--   0 vsts      (1001) docker     (127)      587 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/useful/test_main.h
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/useful/test_main.h.base
--rw-r--r--   0 vsts      (1001) docker     (127)     8384 2024-03-26 17:00:57.000000 pyvex-9.2.96/vex/useful/x87_to_vex_and_back.c
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.466301 pyvex-9.2.97/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-04-02 17:01:31.000000 pyvex-9.2.97/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-02 17:01:31.000000 pyvex-9.2.97/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10117 2024-04-02 17:02:05.466301 pyvex-9.2.97/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8959 2024-04-02 17:01:31.000000 pyvex-9.2.97/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     5136 2024-04-02 17:01:31.000000 pyvex-9.2.97/make_ffi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      279 2024-04-02 17:01:45.000000 pyvex-9.2.97/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.386301 pyvex-9.2.97/pyvex/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-02 17:01:45.000000 pyvex-9.2.97/pyvex/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49630 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/_register_info.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3695 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/arches.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24800 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9356 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/const.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1733 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/data_ref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4487 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1191 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25727 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/expr.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.386301 pyvex-9.2.97/pyvex/lifting/
+-rw-r--r--   0 vsts      (1001) docker     (127)      689 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.390301 pyvex-9.2.97/pyvex/lifting/gym/
+-rw-r--r--   0 vsts      (1001) docker     (127)      204 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/gym/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1220 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/gym/aarch64_spotter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14999 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/gym/arm_spotter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4067 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/gym/x86_spotter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3665 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/libvex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12832 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/lift_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5775 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/lifter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      289 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/post_processor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.390301 pyvex-9.2.97/pyvex/lifting/util/
+-rw-r--r--   0 vsts      (1001) docker     (127)      300 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17912 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/util/instr_helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5293 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/util/lifter_helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8824 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/util/syntax_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10080 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/util/vex_helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2580 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/lifting/zerodivision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2223 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/native.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)    22097 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/stmt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1040 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1415 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.466301 pyvex-9.2.97/pyvex.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10117 2024-04-02 17:02:05.000000 pyvex-9.2.97/pyvex.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     6212 2024-04-02 17:02:05.000000 pyvex-9.2.97/pyvex.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-02 17:02:05.000000 pyvex-9.2.97/pyvex.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      173 2024-04-02 17:02:05.000000 pyvex-9.2.97/pyvex.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-02 17:02:05.000000 pyvex-9.2.97/pyvex.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.394301 pyvex-9.2.97/pyvex_c/
+-rw-r--r--   0 vsts      (1001) docker     (127)    18092 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex_c/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     1531 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex_c/Makefile
+-rw-r--r--   0 vsts      (1001) docker     (127)      351 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex_c/Makefile-msvc
+-rw-r--r--   0 vsts      (1001) docker     (127)    22533 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex_c/analysis.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     2765 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex_c/e4c_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      794 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex_c/logging.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      226 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex_c/logging.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    12044 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex_c/postprocess.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    10990 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex_c/pyvex.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      923 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex_c/pyvex.def
+-rw-r--r--   0 vsts      (1001) docker     (127)     1688 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex_c/pyvex.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-02 17:01:31.000000 pyvex-9.2.97/pyvex_c/pyvex_internal.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-02 17:02:05.466301 pyvex-9.2.97/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     4972 2024-04-02 17:01:31.000000 pyvex-9.2.97/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.394301 pyvex-9.2.97/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9771 2024-04-02 17:01:31.000000 pyvex-9.2.97/tests/test_arm_postprocess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      883 2024-04-02 17:01:31.000000 pyvex-9.2.97/tests/test_gym.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      728 2024-04-02 17:01:31.000000 pyvex-9.2.97/tests/test_irsb_property_caching.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3263 2024-04-02 17:01:31.000000 pyvex-9.2.97/tests/test_lift.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      638 2024-04-02 17:01:31.000000 pyvex-9.2.97/tests/test_mips32_postprocess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15877 2024-04-02 17:01:31.000000 pyvex-9.2.97/tests/test_pyvex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      694 2024-04-02 17:01:31.000000 pyvex-9.2.97/tests/test_s390x_exrl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-02 17:01:31.000000 pyvex-9.2.97/tests/test_s390x_lochi.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      449 2024-04-02 17:01:31.000000 pyvex-9.2.97/tests/test_s390x_vl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3367 2024-04-02 17:01:31.000000 pyvex-9.2.97/tests/test_spotter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-02 17:01:31.000000 pyvex-9.2.97/tests/test_ud2.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.398301 pyvex-9.2.97/vex/
+-rw-r--r--   0 vsts      (1001) docker     (127)       28 2024-04-02 17:01:32.000000 pyvex-9.2.97/vex/.git
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.378301 pyvex-9.2.97/vex/.github/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.398301 pyvex-9.2.97/vex/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2230 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      205 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1734 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1293 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/.github/ISSUE_TEMPLATE/question.yml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.398301 pyvex-9.2.97/vex/.github/workflows/
+-rw-r--r--   0 vsts      (1001) docker     (127)      838 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/.github/workflows/build.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (127)      176 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/HACKING.README
+-rw-r--r--   0 vsts      (1001) docker     (127)    18011 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/LICENSE.GPL
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/LICENSE.README
+-rw-r--r--   0 vsts      (1001) docker     (127)     5157 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/Makefile-gcc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1211 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/Makefile-msvc
+-rw-r--r--   0 vsts      (1001) docker     (127)      133 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)     1028 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/TODO.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.398301 pyvex-9.2.97/vex/auxprogs/
+-rw-r--r--   0 vsts      (1001) docker     (127)    33667 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/auxprogs/genoffsets.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     2999 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/common.mk
+-rw-r--r--   0 vsts      (1001) docker     (127)      430 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/nanoarm.orig
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.402301 pyvex-9.2.97/vex/orig_amd64/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1612 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_amd64/Compare.hs
+-rw-r--r--   0 vsts      (1001) docker     (127)      580 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_amd64/SortedToOrig.hs
+-rw-r--r--   0 vsts      (1001) docker     (127)    77851 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_amd64/test1.orig
+-rw-r--r--   0 vsts      (1001) docker     (127)    64255 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_amd64/test1.sorted
+-rw-r--r--   0 vsts      (1001) docker     (127)   349947 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_amd64/test2.orig
+-rw-r--r--   0 vsts      (1001) docker     (127)   349312 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_amd64/test2.sorted
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.402301 pyvex-9.2.97/vex/orig_arm/
+-rw-r--r--   0 vsts      (1001) docker     (127)      359 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_arm/nanoarm
+-rw-r--r--   0 vsts      (1001) docker     (127)      430 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_arm/nanoarm.orig
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.410301 pyvex-9.2.97/vex/orig_ppc32/
+-rw-r--r--   0 vsts      (1001) docker     (127)  3443743 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_ppc32/date.orig
+-rw-r--r--   0 vsts      (1001) docker     (127)  1156810 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_ppc32/loadsafp.orig
+-rw-r--r--   0 vsts      (1001) docker     (127)   212994 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_ppc32/morefp.orig
+-rw-r--r--   0 vsts      (1001) docker     (127)  1511720 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_ppc32/return0.orig
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.414301 pyvex-9.2.97/vex/orig_x86/
+-rw-r--r--   0 vsts      (1001) docker     (127)   420476 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_x86/exit42.orig
+-rw-r--r--   0 vsts      (1001) docker     (127)   869782 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_x86/fpu_mmx_sse.orig
+-rw-r--r--   0 vsts      (1001) docker     (127)   426379 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/orig_x86/manyfp.orig
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.450301 pyvex-9.2.97/vex/priv/
+-rw-r--r--   0 vsts      (1001) docker     (127)    23305 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_amd64_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   158809 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_amd64_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (127)  1197373 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_amd64_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    13043 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_arm64_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    68566 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_arm64_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   552369 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_arm64_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    12853 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_arm_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    50250 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_arm_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   882026 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_arm_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    50108 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_generic_bb_to_IR.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     7961 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_generic_bb_to_IR.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    39860 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_generic_x87.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     4929 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_generic_x87.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6065 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_mips_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    29340 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_mips_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   807179 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_mips_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     6731 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_ppc_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    34775 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_ppc_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (127)  1130268 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_ppc_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     7656 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_riscv64_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    21925 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_riscv64_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   136757 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_riscv64_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    17479 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_s390_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   101697 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_s390_helpers.c
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    10118 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_s390_insn_formats.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   727610 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_s390_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     4954 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_tilegx_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    20766 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_tilegx_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    79947 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_tilegx_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    16605 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_x86_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   100948 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_x86_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   552922 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/guest_x86_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   145172 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_amd64_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    30093 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_amd64_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   191170 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_amd64_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   218996 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_arm64_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    37441 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_arm64_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   163347 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_arm64_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   183248 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_arm_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    35420 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_arm_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   257988 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_arm_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_generic_maddf.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     1870 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_generic_maddf.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    60281 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_generic_reg_alloc2.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    55387 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_generic_reg_alloc3.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    11727 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_generic_regs.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    17459 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_generic_regs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    13196 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_generic_simd128.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     3773 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_generic_simd128.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2155 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_generic_simd256.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     2066 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_generic_simd256.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    43649 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_generic_simd64.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     7296 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_generic_simd64.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   131651 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_mips_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    26553 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_mips_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   151524 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_mips_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   231014 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_ppc_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    43619 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_ppc_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   266473 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_ppc_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    91833 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_riscv64_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    30525 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_riscv64_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    74222 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_riscv64_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   329366 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_s390_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    34560 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_s390_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   174718 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_s390_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    76788 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_tilegx_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    20244 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_tilegx_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    56164 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_tilegx_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   120030 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_x86_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    26278 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_x86_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   164986 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/host_x86_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   190764 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/ir_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    10919 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/ir_inject.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     3802 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/ir_match.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     3145 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/ir_match.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   231011 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/ir_opt.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/ir_opt.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2179 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/main_globals.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     2803 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/main_globals.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    86049 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/main_main.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    18330 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/main_util.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     5861 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/main_util.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3163 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/multiarch_main_main.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     6083 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/s390_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    14758 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/s390_disasm.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     3277 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/s390_disasm.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   180250 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/tilegx_disasm.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    28210 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/priv/tilegx_disasm.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.454301 pyvex-9.2.97/vex/pub/
+-rw-r--r--   0 vsts      (1001) docker     (127)    41851 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6612 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_basictypes.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     4889 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_emnote.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     8942 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_guest_amd64.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     7926 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_guest_arm.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6526 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_guest_arm64.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6330 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_guest_mips32.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6397 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_guest_mips64.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    11695 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_guest_ppc32.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    13411 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_guest_ppc64.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5098 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_guest_riscv64.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     7258 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_guest_s390x.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     4896 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_guest_tilegx.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    12432 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_guest_x86.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   122287 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_ir.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5025 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_s390x_common.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     4451 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/pub/libvex_trc_values.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.454301 pyvex-9.2.97/vex/switchback/
+-rw-r--r--   0 vsts      (1001) docker     (127)      257 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/switchback/Makefile
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     9974 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/switchback/binary_switchback.pl
+-rw-r--r--   0 vsts      (1001) docker     (127)    45293 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/switchback/linker.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/switchback/linker.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    24229 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/switchback/switchback.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   184904 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/switchback/test_bzip2.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    53078 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/switchback/test_emfloat.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      286 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/switchback/test_hello.c
+-rw-r--r--   0 vsts      (1001) docker     (127)   115291 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/switchback/test_ppc_jm1.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/switchback/test_simple.c
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.462301 pyvex-9.2.97/vex/test/
+-rw-r--r--   0 vsts      (1001) docker     (127)      542 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/fldenv.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      224 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/fp1.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      792 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/fp1.s
+-rw-r--r--   0 vsts      (1001) docker     (127)     1572 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/fpconst.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     1451 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/fpgames.s
+-rw-r--r--   0 vsts      (1001) docker     (127)      555 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/fpspeed.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      660 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/fpucw.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     1906 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/frstor.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     1557 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/fsave.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      393 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/fstenv.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     3462 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/fxsave.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    20405 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/mmxtest.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      694 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/mxcsr.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     2169 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/rounderr.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     2157 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/test-amd64-muldiv.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     4715 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/test-amd64-shift.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    45441 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/test-amd64.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     6381 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/test-amd64.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1521 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/test-i386-muldiv.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     4022 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/test-i386-shift.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    44331 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/test-i386.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     5372 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/test-i386.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      926 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/x87fxam.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      403 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/test/x87tst.c
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.462301 pyvex-9.2.97/vex/unused/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1593 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/unused/arena.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2502 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/unused/dispatch.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    43051 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/unused/linker.c
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:05.466301 pyvex-9.2.97/vex/useful/
+-rw-r--r--   0 vsts      (1001) docker     (127)      235 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/useful/Makefile-vex
+-rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/useful/cpuid.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    19175 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/useful/fp_80_64.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      191 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/useful/fpround.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      383 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/useful/fspill.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      201 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/useful/gradual_underflow.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    54111 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/useful/hd_fpu.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     4886 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/useful/show_fp_state.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     7171 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/useful/smchash.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    89474 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/useful/test_main.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      587 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/useful/test_main.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/useful/test_main.h.base
+-rw-r--r--   0 vsts      (1001) docker     (127)     8384 2024-04-02 17:01:33.000000 pyvex-9.2.97/vex/useful/x87_to_vex_and_back.c
```

### Comparing `pyvex-9.2.96/LICENSE` & `pyvex-9.2.97/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/PKG-INFO` & `pyvex-9.2.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvex
-Version: 9.2.96
+Version: 9.2.97
 Summary: A Python interface to libVEX and VEX IR
 Home-page: https://github.com/angr/pyvex
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyvex-9.2.96/README.md` & `pyvex-9.2.97/README.md`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/make_ffi.py` & `pyvex-9.2.97/make_ffi.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/__init__.py` & `pyvex-9.2.97/pyvex/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 PyVEX provides an interface that translates binary code into the VEX intermediate representation (IR).
 For an introduction to VEX, take a look here: https://docs.angr.io/advanced-topics/ir
 """
 
-__version__ = "9.2.96"
+__version__ = "9.2.97"
 
 from . import const, expr, stmt
 from .arches import (
     ARCH_AMD64,
     ARCH_ARM64_BE,
     ARCH_ARM64_LE,
     ARCH_ARM_BE,
```

### Comparing `pyvex-9.2.96/pyvex/_register_info.py` & `pyvex-9.2.97/pyvex/_register_info.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/arches.py` & `pyvex-9.2.97/pyvex/arches.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/block.py` & `pyvex-9.2.97/pyvex/block.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/const.py` & `pyvex-9.2.97/pyvex/const.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/data_ref.py` & `pyvex-9.2.97/pyvex/data_ref.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/enums.py` & `pyvex-9.2.97/pyvex/enums.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/errors.py` & `pyvex-9.2.97/pyvex/errors.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/expr.py` & `pyvex-9.2.97/pyvex/expr.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/lifting/__init__.py` & `pyvex-9.2.97/pyvex/lifting/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/lifting/gym/aarch64_spotter.py` & `pyvex-9.2.97/pyvex/lifting/gym/aarch64_spotter.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/lifting/gym/arm_spotter.py` & `pyvex-9.2.97/pyvex/lifting/gym/arm_spotter.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/lifting/gym/x86_spotter.py` & `pyvex-9.2.97/pyvex/lifting/gym/x86_spotter.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/lifting/libvex.py` & `pyvex-9.2.97/pyvex/lifting/libvex.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/lifting/lift_function.py` & `pyvex-9.2.97/pyvex/lifting/lift_function.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/lifting/lifter.py` & `pyvex-9.2.97/pyvex/lifting/lifter.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/lifting/util/instr_helper.py` & `pyvex-9.2.97/pyvex/lifting/util/instr_helper.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/lifting/util/lifter_helper.py` & `pyvex-9.2.97/pyvex/lifting/util/lifter_helper.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/lifting/util/syntax_wrapper.py` & `pyvex-9.2.97/pyvex/lifting/util/syntax_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/lifting/util/vex_helper.py` & `pyvex-9.2.97/pyvex/lifting/util/vex_helper.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/lifting/zerodivision.py` & `pyvex-9.2.97/pyvex/lifting/zerodivision.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/native.py` & `pyvex-9.2.97/pyvex/native.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/stmt.py` & `pyvex-9.2.97/pyvex/stmt.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/types.py` & `pyvex-9.2.97/pyvex/types.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex/utils.py` & `pyvex-9.2.97/pyvex/utils.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex.egg-info/PKG-INFO` & `pyvex-9.2.97/pyvex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvex
-Version: 9.2.96
+Version: 9.2.97
 Summary: A Python interface to libVEX and VEX IR
 Home-page: https://github.com/angr/pyvex
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyvex-9.2.96/pyvex.egg-info/SOURCES.txt` & `pyvex-9.2.97/pyvex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex_c/LICENSE` & `pyvex-9.2.97/pyvex_c/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex_c/Makefile` & `pyvex-9.2.97/pyvex_c/Makefile`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex_c/analysis.c` & `pyvex-9.2.97/pyvex_c/analysis.c`

 * *Files 1% similar despite different names*

```diff
@@ -442,20 +442,23 @@
 Bool load_value(ULong addr, int size, int endness, void *value) {
 	int pos = find_region(addr);
 	if (pos < 0 || pos >= next_unused_region_id) {
 		// Does not exist
 		return False;
 	}
 	unsigned char* ptr = NULL;
-	if (regions[pos].in_use && regions[pos].start <= addr &&
-			regions[pos].start + regions[pos].size >= addr + size) {
+	if (regions[pos].in_use &&
+		regions[pos].start <= addr &&
+		regions[pos].start <= addr + size &&
+		regions[pos].start + regions[pos].size >= addr + size) {
 		ptr = regions[pos].content + (addr - regions[pos].start);
 	} else if (pos > 0 &&
 			regions[pos - 1].in_use &&
 			regions[pos - 1].start <= addr &&
+			regions[pos - 1].start <= addr + size &&
 			regions[pos - 1].start + regions[pos - 1].size >= addr + size) {
 		ptr = regions[pos - 1].content + (addr - regions[pos - 1].start);
 	} else {
 		return False;
 	}
 
 	// Do the load!
```

### Comparing `pyvex-9.2.96/pyvex_c/e4c_lite.h` & `pyvex-9.2.97/pyvex_c/e4c_lite.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex_c/logging.c` & `pyvex-9.2.97/pyvex_c/logging.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex_c/postprocess.c` & `pyvex-9.2.97/pyvex_c/postprocess.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex_c/pyvex.c` & `pyvex-9.2.97/pyvex_c/pyvex.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex_c/pyvex.def` & `pyvex-9.2.97/pyvex_c/pyvex.def`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex_c/pyvex.h` & `pyvex-9.2.97/pyvex_c/pyvex.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/pyvex_c/pyvex_internal.h` & `pyvex-9.2.97/pyvex_c/pyvex_internal.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/setup.cfg` & `pyvex-9.2.97/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/setup.py` & `pyvex-9.2.97/setup.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/tests/test_arm_postprocess.py` & `pyvex-9.2.97/tests/test_arm_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/tests/test_gym.py` & `pyvex-9.2.97/tests/test_gym.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/tests/test_irsb_property_caching.py` & `pyvex-9.2.97/tests/test_irsb_property_caching.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/tests/test_lift.py` & `pyvex-9.2.97/tests/test_lift.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/tests/test_mips32_postprocess.py` & `pyvex-9.2.97/tests/test_mips32_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/tests/test_pyvex.py` & `pyvex-9.2.97/tests/test_pyvex.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/tests/test_s390x_exrl.py` & `pyvex-9.2.97/tests/test_s390x_exrl.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/tests/test_spotter.py` & `pyvex-9.2.97/tests/test_spotter.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/.github/ISSUE_TEMPLATE/bug-report.yml` & `pyvex-9.2.97/vex/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/.github/ISSUE_TEMPLATE/feature-request.yml` & `pyvex-9.2.97/vex/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/.github/ISSUE_TEMPLATE/question.yml` & `pyvex-9.2.97/vex/.github/ISSUE_TEMPLATE/question.yml`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/.github/workflows/build.yml` & `pyvex-9.2.97/vex/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/LICENSE.GPL` & `pyvex-9.2.97/vex/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/LICENSE.README` & `pyvex-9.2.97/vex/LICENSE.README`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/Makefile-gcc` & `pyvex-9.2.97/vex/Makefile-gcc`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/Makefile-msvc` & `pyvex-9.2.97/vex/Makefile-msvc`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/TODO.txt` & `pyvex-9.2.97/vex/TODO.txt`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/auxprogs/genoffsets.c` & `pyvex-9.2.97/vex/auxprogs/genoffsets.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/common.mk` & `pyvex-9.2.97/vex/common.mk`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/orig_amd64/Compare.hs` & `pyvex-9.2.97/vex/orig_amd64/Compare.hs`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/orig_amd64/SortedToOrig.hs` & `pyvex-9.2.97/vex/orig_amd64/SortedToOrig.hs`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/orig_amd64/test1.orig` & `pyvex-9.2.97/vex/orig_amd64/test1.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/orig_amd64/test1.sorted` & `pyvex-9.2.97/vex/orig_amd64/test1.sorted`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/orig_amd64/test2.orig` & `pyvex-9.2.97/vex/orig_amd64/test2.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/orig_amd64/test2.sorted` & `pyvex-9.2.97/vex/orig_amd64/test2.sorted`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/orig_ppc32/date.orig` & `pyvex-9.2.97/vex/orig_ppc32/date.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/orig_ppc32/loadsafp.orig` & `pyvex-9.2.97/vex/orig_ppc32/loadsafp.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/orig_ppc32/morefp.orig` & `pyvex-9.2.97/vex/orig_ppc32/morefp.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/orig_ppc32/return0.orig` & `pyvex-9.2.97/vex/orig_ppc32/return0.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/orig_x86/exit42.orig` & `pyvex-9.2.97/vex/orig_x86/exit42.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/orig_x86/fpu_mmx_sse.orig` & `pyvex-9.2.97/vex/orig_x86/fpu_mmx_sse.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/orig_x86/manyfp.orig` & `pyvex-9.2.97/vex/orig_x86/manyfp.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_amd64_defs.h` & `pyvex-9.2.97/vex/priv/guest_amd64_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_amd64_helpers.c` & `pyvex-9.2.97/vex/priv/guest_amd64_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_amd64_toIR.c` & `pyvex-9.2.97/vex/priv/guest_amd64_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_arm64_defs.h` & `pyvex-9.2.97/vex/priv/guest_arm64_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_arm64_helpers.c` & `pyvex-9.2.97/vex/priv/guest_arm64_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_arm64_toIR.c` & `pyvex-9.2.97/vex/priv/guest_arm64_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_arm_defs.h` & `pyvex-9.2.97/vex/priv/guest_arm_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_arm_helpers.c` & `pyvex-9.2.97/vex/priv/guest_arm_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_arm_toIR.c` & `pyvex-9.2.97/vex/priv/guest_arm_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_generic_bb_to_IR.c` & `pyvex-9.2.97/vex/priv/guest_generic_bb_to_IR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_generic_bb_to_IR.h` & `pyvex-9.2.97/vex/priv/guest_generic_bb_to_IR.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_generic_x87.c` & `pyvex-9.2.97/vex/priv/guest_generic_x87.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_generic_x87.h` & `pyvex-9.2.97/vex/priv/guest_generic_x87.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_mips_defs.h` & `pyvex-9.2.97/vex/priv/guest_mips_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_mips_helpers.c` & `pyvex-9.2.97/vex/priv/guest_mips_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_mips_toIR.c` & `pyvex-9.2.97/vex/priv/guest_mips_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_ppc_defs.h` & `pyvex-9.2.97/vex/priv/guest_ppc_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_ppc_helpers.c` & `pyvex-9.2.97/vex/priv/guest_ppc_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_ppc_toIR.c` & `pyvex-9.2.97/vex/priv/guest_ppc_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_riscv64_defs.h` & `pyvex-9.2.97/vex/priv/guest_riscv64_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_riscv64_helpers.c` & `pyvex-9.2.97/vex/priv/guest_riscv64_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_riscv64_toIR.c` & `pyvex-9.2.97/vex/priv/guest_riscv64_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_s390_defs.h` & `pyvex-9.2.97/vex/priv/guest_s390_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_s390_helpers.c` & `pyvex-9.2.97/vex/priv/guest_s390_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_s390_insn_formats.py` & `pyvex-9.2.97/vex/priv/guest_s390_insn_formats.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_s390_toIR.c` & `pyvex-9.2.97/vex/priv/guest_s390_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_tilegx_defs.h` & `pyvex-9.2.97/vex/priv/guest_tilegx_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_tilegx_helpers.c` & `pyvex-9.2.97/vex/priv/guest_tilegx_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_tilegx_toIR.c` & `pyvex-9.2.97/vex/priv/guest_tilegx_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_x86_defs.h` & `pyvex-9.2.97/vex/priv/guest_x86_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_x86_helpers.c` & `pyvex-9.2.97/vex/priv/guest_x86_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/guest_x86_toIR.c` & `pyvex-9.2.97/vex/priv/guest_x86_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_amd64_defs.c` & `pyvex-9.2.97/vex/priv/host_amd64_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_amd64_defs.h` & `pyvex-9.2.97/vex/priv/host_amd64_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_amd64_isel.c` & `pyvex-9.2.97/vex/priv/host_amd64_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_arm64_defs.c` & `pyvex-9.2.97/vex/priv/host_arm64_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_arm64_defs.h` & `pyvex-9.2.97/vex/priv/host_arm64_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_arm64_isel.c` & `pyvex-9.2.97/vex/priv/host_arm64_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_arm_defs.c` & `pyvex-9.2.97/vex/priv/host_arm_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_arm_defs.h` & `pyvex-9.2.97/vex/priv/host_arm_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_arm_isel.c` & `pyvex-9.2.97/vex/priv/host_arm_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_generic_maddf.c` & `pyvex-9.2.97/vex/priv/host_generic_maddf.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_generic_maddf.h` & `pyvex-9.2.97/vex/priv/host_generic_maddf.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_generic_reg_alloc2.c` & `pyvex-9.2.97/vex/priv/host_generic_reg_alloc2.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_generic_reg_alloc3.c` & `pyvex-9.2.97/vex/priv/host_generic_reg_alloc3.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_generic_regs.c` & `pyvex-9.2.97/vex/priv/host_generic_regs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_generic_regs.h` & `pyvex-9.2.97/vex/priv/host_generic_regs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_generic_simd128.c` & `pyvex-9.2.97/vex/priv/host_generic_simd128.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_generic_simd128.h` & `pyvex-9.2.97/vex/priv/host_generic_simd128.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_generic_simd256.c` & `pyvex-9.2.97/vex/priv/host_generic_simd256.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_generic_simd256.h` & `pyvex-9.2.97/vex/priv/host_generic_simd256.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_generic_simd64.c` & `pyvex-9.2.97/vex/priv/host_generic_simd64.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_generic_simd64.h` & `pyvex-9.2.97/vex/priv/host_generic_simd64.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_mips_defs.c` & `pyvex-9.2.97/vex/priv/host_mips_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_mips_defs.h` & `pyvex-9.2.97/vex/priv/host_mips_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_mips_isel.c` & `pyvex-9.2.97/vex/priv/host_mips_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_ppc_defs.c` & `pyvex-9.2.97/vex/priv/host_ppc_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_ppc_defs.h` & `pyvex-9.2.97/vex/priv/host_ppc_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_ppc_isel.c` & `pyvex-9.2.97/vex/priv/host_ppc_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_riscv64_defs.c` & `pyvex-9.2.97/vex/priv/host_riscv64_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_riscv64_defs.h` & `pyvex-9.2.97/vex/priv/host_riscv64_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_riscv64_isel.c` & `pyvex-9.2.97/vex/priv/host_riscv64_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_s390_defs.c` & `pyvex-9.2.97/vex/priv/host_s390_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_s390_defs.h` & `pyvex-9.2.97/vex/priv/host_s390_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_s390_isel.c` & `pyvex-9.2.97/vex/priv/host_s390_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_tilegx_defs.c` & `pyvex-9.2.97/vex/priv/host_tilegx_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_tilegx_defs.h` & `pyvex-9.2.97/vex/priv/host_tilegx_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_tilegx_isel.c` & `pyvex-9.2.97/vex/priv/host_tilegx_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_x86_defs.c` & `pyvex-9.2.97/vex/priv/host_x86_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_x86_defs.h` & `pyvex-9.2.97/vex/priv/host_x86_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/host_x86_isel.c` & `pyvex-9.2.97/vex/priv/host_x86_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/ir_defs.c` & `pyvex-9.2.97/vex/priv/ir_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/ir_inject.c` & `pyvex-9.2.97/vex/priv/ir_inject.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/ir_match.c` & `pyvex-9.2.97/vex/priv/ir_match.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/ir_match.h` & `pyvex-9.2.97/vex/priv/ir_match.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/ir_opt.c` & `pyvex-9.2.97/vex/priv/ir_opt.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/ir_opt.h` & `pyvex-9.2.97/vex/priv/ir_opt.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/main_globals.c` & `pyvex-9.2.97/vex/priv/main_globals.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/main_globals.h` & `pyvex-9.2.97/vex/priv/main_globals.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/main_main.c` & `pyvex-9.2.97/vex/priv/main_main.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/main_util.c` & `pyvex-9.2.97/vex/priv/main_util.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/main_util.h` & `pyvex-9.2.97/vex/priv/main_util.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/multiarch_main_main.c` & `pyvex-9.2.97/vex/priv/multiarch_main_main.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/s390_defs.h` & `pyvex-9.2.97/vex/priv/s390_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/s390_disasm.c` & `pyvex-9.2.97/vex/priv/s390_disasm.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/s390_disasm.h` & `pyvex-9.2.97/vex/priv/s390_disasm.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/tilegx_disasm.c` & `pyvex-9.2.97/vex/priv/tilegx_disasm.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/priv/tilegx_disasm.h` & `pyvex-9.2.97/vex/priv/tilegx_disasm.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex.h` & `pyvex-9.2.97/vex/pub/libvex.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_basictypes.h` & `pyvex-9.2.97/vex/pub/libvex_basictypes.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_emnote.h` & `pyvex-9.2.97/vex/pub/libvex_emnote.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_guest_amd64.h` & `pyvex-9.2.97/vex/pub/libvex_guest_amd64.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_guest_arm.h` & `pyvex-9.2.97/vex/pub/libvex_guest_arm.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_guest_arm64.h` & `pyvex-9.2.97/vex/pub/libvex_guest_arm64.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_guest_mips32.h` & `pyvex-9.2.97/vex/pub/libvex_guest_mips32.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_guest_mips64.h` & `pyvex-9.2.97/vex/pub/libvex_guest_mips64.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_guest_ppc32.h` & `pyvex-9.2.97/vex/pub/libvex_guest_ppc32.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_guest_ppc64.h` & `pyvex-9.2.97/vex/pub/libvex_guest_ppc64.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_guest_riscv64.h` & `pyvex-9.2.97/vex/pub/libvex_guest_riscv64.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_guest_s390x.h` & `pyvex-9.2.97/vex/pub/libvex_guest_s390x.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_guest_tilegx.h` & `pyvex-9.2.97/vex/pub/libvex_guest_tilegx.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_guest_x86.h` & `pyvex-9.2.97/vex/pub/libvex_guest_x86.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_ir.h` & `pyvex-9.2.97/vex/pub/libvex_ir.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_s390x_common.h` & `pyvex-9.2.97/vex/pub/libvex_s390x_common.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/pub/libvex_trc_values.h` & `pyvex-9.2.97/vex/pub/libvex_trc_values.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/switchback/binary_switchback.pl` & `pyvex-9.2.97/vex/switchback/binary_switchback.pl`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/switchback/linker.c` & `pyvex-9.2.97/vex/switchback/linker.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/switchback/switchback.c` & `pyvex-9.2.97/vex/switchback/switchback.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/switchback/test_bzip2.c` & `pyvex-9.2.97/vex/switchback/test_bzip2.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/switchback/test_emfloat.c` & `pyvex-9.2.97/vex/switchback/test_emfloat.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/switchback/test_ppc_jm1.c` & `pyvex-9.2.97/vex/switchback/test_ppc_jm1.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/fldenv.c` & `pyvex-9.2.97/vex/test/fldenv.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/fp1.s` & `pyvex-9.2.97/vex/test/fp1.s`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/fpconst.c` & `pyvex-9.2.97/vex/test/fpconst.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/fpgames.s` & `pyvex-9.2.97/vex/test/fpgames.s`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/fpspeed.c` & `pyvex-9.2.97/vex/test/fpspeed.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/fpucw.c` & `pyvex-9.2.97/vex/test/fpucw.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/frstor.c` & `pyvex-9.2.97/vex/test/frstor.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/fsave.c` & `pyvex-9.2.97/vex/test/fsave.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/fxsave.c` & `pyvex-9.2.97/vex/test/fxsave.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/mmxtest.c` & `pyvex-9.2.97/vex/test/mmxtest.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/mxcsr.c` & `pyvex-9.2.97/vex/test/mxcsr.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/rounderr.c` & `pyvex-9.2.97/vex/test/rounderr.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/test-amd64-muldiv.h` & `pyvex-9.2.97/vex/test/test-amd64-muldiv.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/test-amd64-shift.h` & `pyvex-9.2.97/vex/test/test-amd64-shift.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/test-amd64.c` & `pyvex-9.2.97/vex/test/test-amd64.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/test-amd64.h` & `pyvex-9.2.97/vex/test/test-amd64.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/test-i386-muldiv.h` & `pyvex-9.2.97/vex/test/test-i386-muldiv.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/test-i386-shift.h` & `pyvex-9.2.97/vex/test/test-i386-shift.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/test-i386.c` & `pyvex-9.2.97/vex/test/test-i386.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/test-i386.h` & `pyvex-9.2.97/vex/test/test-i386.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/test/x87fxam.c` & `pyvex-9.2.97/vex/test/x87fxam.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/unused/arena.h` & `pyvex-9.2.97/vex/unused/arena.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/unused/dispatch.c` & `pyvex-9.2.97/vex/unused/dispatch.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/unused/linker.c` & `pyvex-9.2.97/vex/unused/linker.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/useful/cpuid.c` & `pyvex-9.2.97/vex/useful/cpuid.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/useful/fp_80_64.c` & `pyvex-9.2.97/vex/useful/fp_80_64.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/useful/hd_fpu.c` & `pyvex-9.2.97/vex/useful/hd_fpu.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/useful/show_fp_state.c` & `pyvex-9.2.97/vex/useful/show_fp_state.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/useful/smchash.c` & `pyvex-9.2.97/vex/useful/smchash.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/useful/test_main.c` & `pyvex-9.2.97/vex/useful/test_main.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/useful/test_main.h` & `pyvex-9.2.97/vex/useful/test_main.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/useful/test_main.h.base` & `pyvex-9.2.97/vex/useful/test_main.h.base`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.96/vex/useful/x87_to_vex_and_back.c` & `pyvex-9.2.97/vex/useful/x87_to_vex_and_back.c`

 * *Files identical despite different names*

