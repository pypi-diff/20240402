# Comparing `tmp/autobuild-3.9.3.tar.gz` & `tmp/autobuild-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobuild-3.9.3.tar", last modified: Sat Jan 20 07:53:23 2024, max compression
+gzip compressed data, was "autobuild-3.9.4.tar", last modified: Tue Apr  2 06:57:02 2024, max compression
```

## Comparing `autobuild-3.9.3.tar` & `autobuild-3.9.4.tar`

### file list

```diff
@@ -1,132 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.799513 autobuild-3.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.779513 autobuild-3.9.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-20 07:53:00.000000 autobuild-3.9.3/.github/dependabot.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-20 07:53:00.000000 autobuild-3.9.3/.github/release.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.779513 autobuild-3.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-20 07:53:00.000000 autobuild-3.9.3/.github/workflows/bump-major.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-01-20 07:53:00.000000 autobuild-3.9.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-20 07:53:00.000000 autobuild-3.9.3/.github/workflows/cla.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-20 07:53:00.000000 autobuild-3.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-01-20 07:53:00.000000 autobuild-3.9.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-20 07:53:00.000000 autobuild-3.9.3/BuildParams
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-20 07:53:00.000000 autobuild-3.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-20 07:53:00.000000 autobuild-3.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-01-20 07:53:23.799513 autobuild-3.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-01-20 07:53:00.000000 autobuild-3.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.783513 autobuild-3.9.3/autobuild/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/archive_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/autobuild_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/autobuild_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    13027 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/autobuild_tool_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/autobuild_tool_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/autobuild_tool_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/autobuild_tool_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    43528 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/autobuild_tool_install.py
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/autobuild_tool_installables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/autobuild_tool_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    18158 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/autobuild_tool_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/autobuild_tool_print.py
--rw-r--r--   0 runner    (1001) docker     (127)    39621 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/autobuild_tool_source_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/autobuild_tool_uninstall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/build_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    20366 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    33521 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/configfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/executable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/hash_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.783513 autobuild-3.9.3/autobuild/scm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/scm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/scm/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    13546 2024-01-20 07:53:00.000000 autobuild-3.9.3/autobuild/update.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-20 07:53:23.000000 autobuild-3.9.3/autobuild/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.795513 autobuild-3.9.3/autobuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-01-20 07:53:23.000000 autobuild-3.9.3/autobuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-01-20 07:53:23.000000 autobuild-3.9.3/autobuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 07:53:23.000000 autobuild-3.9.3/autobuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-20 07:53:23.000000 autobuild-3.9.3/autobuild.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-20 07:53:23.000000 autobuild-3.9.3/autobuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-20 07:53:23.000000 autobuild-3.9.3/autobuild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-20 07:53:23.799513 autobuild-3.9.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1434 2024-01-20 07:53:00.000000 autobuild-3.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.787513 autobuild-3.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/baseline_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/basetest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.787513 autobuild-3.9.3/tests/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/bin/autobuild
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/bin/autobuild.cmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.795513 autobuild-3.9.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/archive.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/archive.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/archive.tar.zst
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/archive.zip
--rw-r--r--   0 runner    (1001) docker     (127)    17012 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/argparse-1.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/autobuild-package-config.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/autobuild-package-disallowedpath-config.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/autobuild-package-missing-config.xml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/bad_assignment
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/bad_substitution
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/bad_variable
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/bingo-0.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/bogus-0.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/bogus-0.1-common-111.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/bogus-0.1-common-111.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/bogus-0.1-common-111.tar.zst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/bogus-0.1-common-111.zip
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/bogus-0.2-common-222.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/bongo-0.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/config_test_0.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/config_test_1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/config_test_2.xml
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/config_test_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/config_test_3.xml
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/conflict-0.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/darwin
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/dependencies_test_packages.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/empty
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/good_variable
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/manifest_test_0.xml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/nolicense-0.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/nolicense-install.xml
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/nometa-0.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/nourl-install.xml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/only_comments
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/package-conflict.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.795513 autobuild-3.9.3/tests/data/package-test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.795513 autobuild-3.9.3/tests/data/package-test/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/package-test/LICENSES/test1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/package-test/autobuild-package.xml
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/package-test/file2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.795513 autobuild-3.9.3/tests/data/package-test/include/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/package-test/include/file1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.795513 autobuild-3.9.3/tests/data/package-test/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/package-test/lib/file3
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/package-update-install.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/packages-failures.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/data/packages-install.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 07:53:23.795513 autobuild-3.9.3/tests/executables/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/executables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/executables/echo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/executables/envtest.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/executables/noop.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_autobuild_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_build_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_configfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_executable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_filetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    41073 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_installables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_scm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_scm_git.py
--rw-r--r--   0 runner    (1001) docker     (127)    14739 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_source_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-01-20 07:53:00.000000 autobuild-3.9.3/tests/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:02.006347 autobuild-3.9.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:01.990347 autobuild-3.9.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 06:56:42.000000 autobuild-3.9.4/.github/dependabot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-02 06:56:42.000000 autobuild-3.9.4/.github/release.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:01.990347 autobuild-3.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-02 06:56:42.000000 autobuild-3.9.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-02 06:56:42.000000 autobuild-3.9.4/.github/workflows/cla.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-02 06:56:42.000000 autobuild-3.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-02 06:56:42.000000 autobuild-3.9.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-02 06:56:42.000000 autobuild-3.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 06:56:42.000000 autobuild-3.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-02 06:57:02.006347 autobuild-3.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-02 06:56:42.000000 autobuild-3.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:01.994346 autobuild-3.9.4/autobuild/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/archive_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/autobuild_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/autobuild_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13027 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/autobuild_tool_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/autobuild_tool_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/autobuild_tool_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/autobuild_tool_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43528 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/autobuild_tool_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/autobuild_tool_installables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/autobuild_tool_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18158 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/autobuild_tool_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/autobuild_tool_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39621 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/autobuild_tool_source_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/autobuild_tool_uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/build_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20366 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33521 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/configfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/hash_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:01.994346 autobuild-3.9.4/autobuild/scm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/scm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/scm/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13546 2024-04-02 06:56:42.000000 autobuild-3.9.4/autobuild/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 06:57:01.000000 autobuild-3.9.4/autobuild/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:02.006347 autobuild-3.9.4/autobuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-02 06:57:01.000000 autobuild-3.9.4/autobuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-02 06:57:01.000000 autobuild-3.9.4/autobuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:57:01.000000 autobuild-3.9.4/autobuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 06:57:01.000000 autobuild-3.9.4/autobuild.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 06:57:01.000000 autobuild-3.9.4/autobuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 06:57:01.000000 autobuild-3.9.4/autobuild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 06:57:02.006347 autobuild-3.9.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1441 2024-04-02 06:56:42.000000 autobuild-3.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:01.998346 autobuild-3.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/baseline_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/basetest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:01.998346 autobuild-3.9.4/tests/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/bin/autobuild
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/bin/autobuild.cmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:02.006347 autobuild-3.9.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/archive.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/archive.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/archive.tar.zst
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/archive.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    17012 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/argparse-1.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/autobuild-package-config.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/autobuild-package-disallowedpath-config.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/autobuild-package-missing-config.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/bad_assignment
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/bad_substitution
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/bad_variable
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/bingo-0.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/bogus-0.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/bogus-0.1-common-111.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/bogus-0.1-common-111.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/bogus-0.1-common-111.tar.zst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/bogus-0.1-common-111.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/bogus-0.2-common-222.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/bongo-0.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/config_test_0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/config_test_1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/config_test_2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/config_test_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/config_test_3.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/conflict-0.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/darwin
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/dependencies_test_packages.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/empty
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/good_variable
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/manifest_test_0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/nolicense-0.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/nolicense-install.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/nometa-0.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/nourl-install.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/only_comments
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/package-conflict.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:02.006347 autobuild-3.9.4/tests/data/package-test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:02.006347 autobuild-3.9.4/tests/data/package-test/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/package-test/LICENSES/test1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/package-test/autobuild-package.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/package-test/file2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:02.006347 autobuild-3.9.4/tests/data/package-test/include/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/package-test/include/file1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:02.006347 autobuild-3.9.4/tests/data/package-test/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/package-test/lib/file3
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/package-update-install.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/packages-failures.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/data/packages-install.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:57:02.006347 autobuild-3.9.4/tests/executables/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/executables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/executables/echo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/executables/envtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/executables/noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_autobuild_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_build_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_configfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41073 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_installables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_scm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_scm_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14739 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_source_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-02 06:56:42.000000 autobuild-3.9.4/tests/test_update.py
```

### Comparing `autobuild-3.9.3/.github/workflows/ci.yaml` & `autobuild-3.9.4/.github/workflows/ci.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
           git config --global user.email "tests@example.com"
           pytest -v --cov=autobuild --cov-report=xml tests/
 
       - name: Build python package
         run: python -m build
 
       - name: Upload coverage
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         if: matrix.os == 'ubuntu-latest'
         with:
           env_vars: OS
 
       - uses: actions/upload-artifact@v4
         if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.11'
         with:
```

### Comparing `autobuild-3.9.3/.github/workflows/cla.yaml` & `autobuild-3.9.4/.github/workflows/cla.yaml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/LICENSE` & `autobuild-3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/PKG-INFO` & `autobuild-3.9.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobuild
-Version: 3.9.3
+Version: 3.9.4
 Summary: Linden Lab Automated Package Management and Build System
 Home-page: http://wiki.secondlife.com/wiki/Autobuild
 Author: Linden Research, Inc.
 Author-email: opensource-dev@lists.secondlife.com
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: llsd
+Requires-Dist: llsd>=1.2.4
 Requires-Dist: pydot
 Requires-Dist: pyzstd
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
```

### Comparing `autobuild-3.9.3/README.md` & `autobuild-3.9.4/README.md`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/archive_utils.py` & `autobuild-3.9.4/autobuild/archive_utils.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/autobuild_base.py` & `autobuild-3.9.4/autobuild/autobuild_base.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/autobuild_main.py` & `autobuild-3.9.4/autobuild/autobuild_main.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/autobuild_tool_build.py` & `autobuild-3.9.4/autobuild/autobuild_tool_build.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/autobuild_tool_configure.py` & `autobuild-3.9.4/autobuild/autobuild_tool_configure.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/autobuild_tool_edit.py` & `autobuild-3.9.4/autobuild/autobuild_tool_edit.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/autobuild_tool_graph.py` & `autobuild-3.9.4/autobuild/autobuild_tool_graph.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/autobuild_tool_install.py` & `autobuild-3.9.4/autobuild/autobuild_tool_install.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/autobuild_tool_installables.py` & `autobuild-3.9.4/autobuild/autobuild_tool_installables.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/autobuild_tool_manifest.py` & `autobuild-3.9.4/autobuild/autobuild_tool_manifest.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/autobuild_tool_package.py` & `autobuild-3.9.4/autobuild/autobuild_tool_package.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/autobuild_tool_print.py` & `autobuild-3.9.4/autobuild/autobuild_tool_print.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/autobuild_tool_source_environment.py` & `autobuild-3.9.4/autobuild/autobuild_tool_source_environment.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/autobuild_tool_uninstall.py` & `autobuild-3.9.4/autobuild/autobuild_tool_uninstall.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/build_id.py` & `autobuild-3.9.4/autobuild/build_id.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/common.py` & `autobuild-3.9.4/autobuild/common.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/configfile.py` & `autobuild-3.9.4/autobuild/configfile.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/executable.py` & `autobuild-3.9.4/autobuild/executable.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/hash_algorithms.py` & `autobuild-3.9.4/autobuild/hash_algorithms.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/interactive.py` & `autobuild-3.9.4/autobuild/interactive.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/scm/base.py` & `autobuild-3.9.4/autobuild/scm/base.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/scm/git.py` & `autobuild-3.9.4/autobuild/scm/git.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild/update.py` & `autobuild-3.9.4/autobuild/update.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/autobuild.egg-info/PKG-INFO` & `autobuild-3.9.4/autobuild.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobuild
-Version: 3.9.3
+Version: 3.9.4
 Summary: Linden Lab Automated Package Management and Build System
 Home-page: http://wiki.secondlife.com/wiki/Autobuild
 Author: Linden Research, Inc.
 Author-email: opensource-dev@lists.secondlife.com
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: llsd
+Requires-Dist: llsd>=1.2.4
 Requires-Dist: pydot
 Requires-Dist: pyzstd
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
```

### Comparing `autobuild-3.9.3/autobuild.egg-info/SOURCES.txt` & `autobuild-3.9.4/autobuild.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 .gitignore
 .pre-commit-config.yaml
-BuildParams
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 .github/dependabot.yaml
 .github/release.yaml
-.github/workflows/bump-major.yaml
 .github/workflows/ci.yaml
 .github/workflows/cla.yaml
 autobuild/__init__.py
 autobuild/archive_utils.py
 autobuild/autobuild_base.py
 autobuild/autobuild_main.py
 autobuild/autobuild_tool_build.py
```

### Comparing `autobuild-3.9.3/setup.py` & `autobuild-3.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,14 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: Unix',
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    install_requires=['llsd', 'pydot', 'pyzstd'],
+    install_requires=['llsd>=1.2.4', 'pydot', 'pyzstd'],
     extras_require={
         'dev': ['pytest', 'pytest-cov'],
         'build': ['build', 'setuptools_scm'],
     },
     python_requires='>=3.7',
 )
```

### Comparing `autobuild-3.9.3/tests/baseline_compare.py` & `autobuild-3.9.4/tests/baseline_compare.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/basetest.py` & `autobuild-3.9.4/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/argparse-1.1-common-111.tar.bz2` & `autobuild-3.9.4/tests/data/argparse-1.1-common-111.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/autobuild-package-config.xml` & `autobuild-3.9.4/tests/data/autobuild-package-config.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/autobuild-package-disallowedpath-config.xml` & `autobuild-3.9.4/tests/data/autobuild-package-disallowedpath-config.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/autobuild-package-missing-config.xml` & `autobuild-3.9.4/tests/data/autobuild-package-missing-config.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/bingo-0.1-common-111.tar.bz2` & `autobuild-3.9.4/tests/data/bingo-0.1-common-111.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/bogus-0.1-common-111.tar.bz2` & `autobuild-3.9.4/tests/data/bogus-0.1-common-111.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/bogus-0.1-common-111.tar.gz` & `autobuild-3.9.4/tests/data/bogus-0.1-common-111.tar.gz`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/bogus-0.1-common-111.tar.xz` & `autobuild-3.9.4/tests/data/bogus-0.1-common-111.tar.xz`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/bogus-0.1-common-111.tar.zst` & `autobuild-3.9.4/tests/data/bogus-0.1-common-111.tar.zst`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/bogus-0.1-common-111.zip` & `autobuild-3.9.4/tests/data/bogus-0.1-common-111.zip`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/bogus-0.2-common-222.tar.bz2` & `autobuild-3.9.4/tests/data/bogus-0.2-common-222.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/bongo-0.1-common-111.tar.bz2` & `autobuild-3.9.4/tests/data/bongo-0.1-common-111.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/config_test_0.xml` & `autobuild-3.9.4/tests/data/config_test_0.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/config_test_1.xml` & `autobuild-3.9.4/tests/data/config_test_1.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/config_test_2.xml` & `autobuild-3.9.4/tests/data/config_test_2.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/config_test_3.txt` & `autobuild-3.9.4/tests/data/config_test_3.txt`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/config_test_3.xml` & `autobuild-3.9.4/tests/data/config_test_3.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/conflict-0.1-common-111.tar.bz2` & `autobuild-3.9.4/tests/data/conflict-0.1-common-111.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/dependencies_test_packages.xml` & `autobuild-3.9.4/tests/data/dependencies_test_packages.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/manifest_test_0.xml` & `autobuild-3.9.4/tests/data/manifest_test_0.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/nolicense-0.1-common-111.tar.bz2` & `autobuild-3.9.4/tests/data/nolicense-0.1-common-111.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/nolicense-install.xml` & `autobuild-3.9.4/tests/data/nolicense-install.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/nourl-install.xml` & `autobuild-3.9.4/tests/data/nourl-install.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/package-conflict.xml` & `autobuild-3.9.4/tests/data/package-conflict.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/package-test/autobuild-package.xml` & `autobuild-3.9.4/tests/data/package-test/autobuild-package.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/package-update-install.xml` & `autobuild-3.9.4/tests/data/package-update-install.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/packages-failures.xml` & `autobuild-3.9.4/tests/data/packages-failures.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/data/packages-install.xml` & `autobuild-3.9.4/tests/data/packages-install.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/executables/__init__.py` & `autobuild-3.9.4/tests/executables/__init__.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/executables/envtest.py` & `autobuild-3.9.4/tests/executables/envtest.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/patch.py` & `autobuild-3.9.4/tests/patch.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_autobuild_main.py` & `autobuild-3.9.4/tests/test_autobuild_main.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_build.py` & `autobuild-3.9.4/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_build_id.py` & `autobuild-3.9.4/tests/test_build_id.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_configfile.py` & `autobuild-3.9.4/tests/test_configfile.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_configure.py` & `autobuild-3.9.4/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_edit.py` & `autobuild-3.9.4/tests/test_edit.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_executable.py` & `autobuild-3.9.4/tests/test_executable.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_filetype.py` & `autobuild-3.9.4/tests/test_filetype.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_graph.py` & `autobuild-3.9.4/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_install.py` & `autobuild-3.9.4/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_installables.py` & `autobuild-3.9.4/tests/test_installables.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_manifest.py` & `autobuild-3.9.4/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_package.py` & `autobuild-3.9.4/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_scm_base.py` & `autobuild-3.9.4/tests/test_scm_base.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_scm_git.py` & `autobuild-3.9.4/tests/test_scm_git.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_source_environment.py` & `autobuild-3.9.4/tests/test_source_environment.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.3/tests/test_update.py` & `autobuild-3.9.4/tests/test_update.py`

 * *Files identical despite different names*

