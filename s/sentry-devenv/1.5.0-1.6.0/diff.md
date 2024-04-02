# Comparing `tmp/sentry_devenv-1.5.0.tar.gz` & `tmp/sentry_devenv-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_devenv-1.5.0.tar", last modified: Mon Mar 25 20:14:55 2024, max compression
+gzip compressed data, was "sentry_devenv-1.6.0.tar", last modified: Tue Apr  2 18:38:59 2024, max compression
```

## Comparing `sentry_devenv-1.5.0.tar` & `sentry_devenv-1.6.0.tar`

### file list

```diff
@@ -1,76 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:55.448857 sentry_devenv-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-25 20:14:55.448857 sentry_devenv-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:55.440857 sentry_devenv-1.5.0/devenv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:55.440857 sentry_devenv-1.5.0/devenv/checks/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/checks/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/doctor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:55.440857 sentry_devenv-1.5.0/devenv/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib/brew.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib/colima.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib/direnv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib/limactl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib/proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib/venv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib/volta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:55.444857 sentry_devenv-1.5.0/devenv/lib_check/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib_check/brew.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/lib_check/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/pin_gha.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/pythons.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/devenv/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:55.448857 sentry_devenv-1.5.0/sentry_devenv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-25 20:14:55.000000 sentry_devenv-1.5.0/sentry_devenv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-25 20:14:55.000000 sentry_devenv-1.5.0/sentry_devenv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 20:14:55.000000 sentry_devenv-1.5.0/sentry_devenv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-25 20:14:55.000000 sentry_devenv-1.5.0/sentry_devenv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-25 20:14:55.000000 sentry_devenv-1.5.0/sentry_devenv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-25 20:14:55.000000 sentry_devenv-1.5.0/sentry_devenv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-25 20:14:55.448857 sentry_devenv-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:55.444857 sentry_devenv-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:55.444857 sentry_devenv-1.5.0/tests/doctor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:55.436857 sentry_devenv-1.5.0/tests/doctor/devenv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:55.448857 sentry_devenv-1.5.0/tests/doctor/devenv/checks/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/devenv/checks/bad_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/devenv/checks/bad_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/devenv/checks/broken_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/devenv/checks/broken_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/devenv/checks/failing_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/devenv/checks/failing_check_with_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/devenv/checks/no_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/devenv/checks/no_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/devenv/checks/no_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/devenv/checks/passing_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/test_attempt_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/test_filter_failing_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/test_load_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/test_prompt_for_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/doctor/test_run_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:14:55.448857 sentry_devenv-1.5.0/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/lib/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/lib/test_brew.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/lib/test_direnv.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/lib/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/lib/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/lib/test_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/lib/test_venv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/lib/test_volta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-25 20:14:51.000000 sentry_devenv-1.5.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.139887 sentry_devenv-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-02 18:38:59.139887 sentry_devenv-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.127887 sentry_devenv-1.6.0/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.127887 sentry_devenv-1.6.0/ci/integration/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.127887 sentry_devenv-1.6.0/ci/integration/repo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.127887 sentry_devenv-1.6.0/ci/integration/repo/devenv/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/ci/integration/repo/devenv/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.131887 sentry_devenv-1.6.0/devenv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.131887 sentry_devenv-1.6.0/devenv/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/checks/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/doctor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.131887 sentry_devenv-1.6.0/devenv/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/brew.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/colima.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/direnv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/limactl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/tenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/venv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/volta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.131887 sentry_devenv-1.6.0/devenv/lib_check/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib_check/brew.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib_check/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/pin_gha.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/pythons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.139887 sentry_devenv-1.6.0/sentry_devenv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-02 18:38:59.000000 sentry_devenv-1.6.0/sentry_devenv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-02 18:38:59.000000 sentry_devenv-1.6.0/sentry_devenv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:38:59.000000 sentry_devenv-1.6.0/sentry_devenv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 18:38:59.000000 sentry_devenv-1.6.0/sentry_devenv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 18:38:59.000000 sentry_devenv-1.6.0/sentry_devenv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 18:38:59.000000 sentry_devenv-1.6.0/sentry_devenv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-02 18:38:59.139887 sentry_devenv-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.135887 sentry_devenv-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.135887 sentry_devenv-1.6.0/tests/doctor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.127887 sentry_devenv-1.6.0/tests/doctor/devenv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.135887 sentry_devenv-1.6.0/tests/doctor/devenv/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/bad_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/bad_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/broken_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/broken_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/failing_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/failing_check_with_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/no_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/no_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/no_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/passing_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/test_attempt_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/test_filter_failing_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/test_load_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/test_prompt_for_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/test_run_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.139887 sentry_devenv-1.6.0/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_brew.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_direnv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_venv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_volta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/utils.py
```

### Comparing `sentry_devenv-1.5.0/PKG-INFO` & `sentry_devenv-1.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_devenv
-Version: 1.5.0
+Version: 1.6.0
 Summary: Utilities for setting up a Sentry development environment
 Author-email: Joshua Li <joshua.li@sentry.io>, Ian Woodard <ian.woodard@sentry.io>, Buck Evan <buck.evan@sentry.io>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `sentry_devenv-1.5.0/README.md` & `sentry_devenv-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/bootstrap.py` & `sentry_devenv-1.6.0/devenv/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,18 @@
 help = "Bootstraps the development environment."
 ExitCode: TypeAlias = "str | int | None"
 
 
 def main(coderoot: str, argv: Sequence[str] | None = None) -> ExitCode:
     parser = argparse.ArgumentParser(description=help)
     parser.add_argument(
-        "repo",
-        type=str,
-        nargs="?",
-        default="sentry",
-        choices=("sentry", "getsentry"),
+        "repo", type=str, nargs="?", default="sentry", choices=("sentry", "ops")
     )
     args = parser.parse_args(argv)
 
-    if args.repo == "getsentry":
-        # Setting up sentry means we're setting up both repos.
-        args.repo = "sentry"
-
-    if args.repo not in {"sentry"}:
-        return f"repo {args.repo} not supported yet!"
-
     if not CI and shutil.which("xcrun"):
         # xcode-select --install will take a while,
         # and involves elevated permissions with a GUI,
         # so best to just let the user go through that separately then retrying,
         # rather than waiting for it.
         # There is a way to perform a headless install but it's more complex
         # (refer to how homebrew does it).
@@ -86,15 +75,48 @@
             )
 
     brew.install()
     direnv.install()
 
     os.makedirs(coderoot, exist_ok=True)
 
-    if args.repo == "sentry":
+    if args.repo == "ops":
+        if not os.path.exists(f"{coderoot}/ops"):
+            proc.run(
+                (
+                    "git",
+                    "-C",
+                    coderoot,
+                    "clone",
+                    "--filter=blob:none",
+                    "git@github.com:getsentry/ops",
+                ),
+                exit=True,
+            )
+        if not os.path.exists(f"{coderoot}/terraform-modules"):
+            proc.run(
+                (
+                    "git",
+                    "-C",
+                    coderoot,
+                    "clone",
+                    "--filter=blob:none",
+                    "git@github.com:getsentry/terraform-modules",
+                ),
+                exit=True,
+            )
+        proc.run(("devenv", "sync"), cwd=f"{coderoot}/ops")
+        print(
+            f"""
+    All done! Please close this terminal window and start a fresh one.
+
+    ops repo is at: {coderoot}/ops
+    """
+        )
+    elif args.repo == "sentry":
         if not os.path.exists(f"{coderoot}/sentry"):
             # git@ clones forces the use of cloning through SSH which is what we want,
             # though CI must clone open source repos via https (no git authentication)
             additional_flags = (
                 (
                     "--depth",
                     "1",
@@ -175,16 +197,17 @@
             proc.run(
                 ("make", "bootstrap"),
                 env={"VIRTUAL_ENV": f"{coderoot}/getsentry/.venv"},
                 pathprepend=f"{coderoot}/getsentry/.devenv/bin:{coderoot}/getsentry/.venv/bin",
                 cwd=f"{coderoot}/getsentry",
             )
 
-    print(
-        f"""
-All done! Please close this terminal window and start a fresh one.
+        print(
+            f"""
+    All done! Please close this terminal window and start a fresh one.
+
+    Sentry has been set up in {coderoot}/sentry. cd into it and you should
+    be able to run `sentry devserver`.
+    """
+        )
 
-Sentry has been set up in {coderoot}/sentry. cd into it and you should
-be able to run `sentry devserver`.
-"""
-    )
     return 0
```

### Comparing `sentry_devenv-1.5.0/devenv/checks/test.py` & `sentry_devenv-1.6.0/devenv/checks/test.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/constants.py` & `sentry_devenv-1.6.0/devenv/constants.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/doctor.py` & `sentry_devenv-1.6.0/devenv/doctor.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/lib/archive.py` & `sentry_devenv-1.6.0/devenv/lib/archive.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/lib/brew.py` & `sentry_devenv-1.6.0/devenv/lib/brew.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/lib/colima.py` & `sentry_devenv-1.6.0/devenv/lib/colima.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/lib/config.py` & `sentry_devenv-1.6.0/devenv/lib/config.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/lib/direnv.py` & `sentry_devenv-1.6.0/devenv/lib/direnv.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/lib/fs.py` & `sentry_devenv-1.6.0/devenv/lib/fs.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/lib/gcloud.py` & `sentry_devenv-1.6.0/devenv/lib/gcloud.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/lib/github.py` & `sentry_devenv-1.6.0/devenv/lib/github.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/lib/limactl.py` & `sentry_devenv-1.6.0/devenv/lib/limactl.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/lib/proc.py` & `sentry_devenv-1.6.0/devenv/lib/proc.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/lib/venv.py` & `sentry_devenv-1.6.0/devenv/lib/venv.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/lib/volta.py` & `sentry_devenv-1.6.0/devenv/lib/volta.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/lib_check/brew.py` & `sentry_devenv-1.6.0/devenv/lib_check/brew.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/main.py` & `sentry_devenv-1.6.0/devenv/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,20 @@
             "To ignore, use devenv --nocoderoot [COMMAND]\n"
             f"To change your code root, you can edit {config_path}.\n"
         )
         return 1
 
     # the remaining tools are repo-specific
     reporoot = gitroot()
-    repo = reporoot.split("/")[-1]
 
+    fake_reporoot = os.getenv("CI_DEVENV_INTEGRATION_FAKE_REPOROOT")
+    if fake_reporoot:
+        reporoot = fake_reporoot
+
+    repo = reporoot.split("/")[-1]
     context = {"repo": repo, "reporoot": reporoot}
 
     if args.command == "doctor":
         return doctor.main(context, remainder)
     if args.command == "sync":
         return sync.main(context, remainder)
```

### Comparing `sentry_devenv-1.5.0/devenv/pin_gha.py` & `sentry_devenv-1.6.0/devenv/pin_gha.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/pythons.py` & `sentry_devenv-1.6.0/devenv/pythons.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/devenv/sync.py` & `sentry_devenv-1.6.0/devenv/sync.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/pyproject.toml` & `sentry_devenv-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sentry_devenv"
-version = "1.5.0"
+version = "1.6.0"
 authors = [
   { name="Joshua Li", email="joshua.li@sentry.io" },
   { name="Ian Woodard", email="ian.woodard@sentry.io" },
   { name="Buck Evan", email="buck.evan@sentry.io" },
 ]
 description = "Utilities for setting up a Sentry development environment"
 readme = "README.md"
```

### Comparing `sentry_devenv-1.5.0/sentry_devenv.egg-info/PKG-INFO` & `sentry_devenv-1.6.0/sentry_devenv.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_devenv
-Version: 1.5.0
+Version: 1.6.0
 Summary: Utilities for setting up a Sentry development environment
 Author-email: Joshua Li <joshua.li@sentry.io>, Ian Woodard <ian.woodard@sentry.io>, Buck Evan <buck.evan@sentry.io>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `sentry_devenv-1.5.0/sentry_devenv.egg-info/SOURCES.txt` & `sentry_devenv-1.6.0/sentry_devenv.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 pyproject.toml
 setup.cfg
+ci/integration/repo/devenv/sync.py
 devenv/__init__.py
 devenv/__main__.py
 devenv/bootstrap.py
 devenv/constants.py
 devenv/doctor.py
 devenv/main.py
 devenv/pin_gha.py
@@ -19,14 +20,15 @@
 devenv/lib/config.py
 devenv/lib/direnv.py
 devenv/lib/fs.py
 devenv/lib/gcloud.py
 devenv/lib/github.py
 devenv/lib/limactl.py
 devenv/lib/proc.py
+devenv/lib/tenv.py
 devenv/lib/venv.py
 devenv/lib/volta.py
 devenv/lib_check/__init__.py
 devenv/lib_check/brew.py
 devenv/lib_check/types.py
 sentry_devenv.egg-info/PKG-INFO
 sentry_devenv.egg-info/SOURCES.txt
```

### Comparing `sentry_devenv-1.5.0/tests/doctor/test_attempt_fix.py` & `sentry_devenv-1.6.0/tests/doctor/test_attempt_fix.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/tests/doctor/test_filter_failing_checks.py` & `sentry_devenv-1.6.0/tests/doctor/test_filter_failing_checks.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/tests/doctor/test_load_checks.py` & `sentry_devenv-1.6.0/tests/doctor/test_load_checks.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/tests/doctor/test_prompt_for_fix.py` & `sentry_devenv-1.6.0/tests/doctor/test_prompt_for_fix.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/tests/doctor/test_run_checks.py` & `sentry_devenv-1.6.0/tests/doctor/test_run_checks.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/tests/lib/test_archive.py` & `sentry_devenv-1.6.0/tests/lib/test_archive.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/tests/lib/test_brew.py` & `sentry_devenv-1.6.0/tests/lib/test_brew.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/tests/lib/test_direnv.py` & `sentry_devenv-1.6.0/tests/lib/test_direnv.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/tests/lib/test_fs.py` & `sentry_devenv-1.6.0/tests/lib/test_fs.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/tests/lib/test_github.py` & `sentry_devenv-1.6.0/tests/lib/test_github.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/tests/lib/test_proc.py` & `sentry_devenv-1.6.0/tests/lib/test_proc.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/tests/lib/test_venv.py` & `sentry_devenv-1.6.0/tests/lib/test_venv.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/tests/lib/test_volta.py` & `sentry_devenv-1.6.0/tests/lib/test_volta.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.5.0/tests/test_main.py` & `sentry_devenv-1.6.0/tests/test_main.py`

 * *Files identical despite different names*

