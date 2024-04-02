# Comparing `tmp/edulint-3.6.0.tar.gz` & `tmp/edulint-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-gg9aabub/edulint-3.6.0.tar", last modified: Wed Mar 13 09:12:16 2024, max compression
+gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-u3f0ls7o/edulint-3.6.1.tar", last modified: Tue Apr  2 15:49:40 2024, max compression
```

## Comparing `edulint-3.6.0.tar` & `edulint-3.6.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:16.000000 edulint-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-13 09:12:09.000000 edulint-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-03-13 09:12:16.000000 edulint-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-03-13 09:12:09.000000 edulint-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/config/arg.py
--rw-r--r--   0 runner    (1001) docker     (127)    17889 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/config/file_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint/config/files/
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/config/files/cs0.toml
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/config/files/default.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/config/files/empty.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/config/language_translations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/config/option_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/config/raw_flake8_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/config/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6122 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/edulint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/explanations.py
--rw-r--r--   0 runner    (1001) docker     (127)   195728 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/explanations.toml
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint/linting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint/linting/checkers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/checkers/basic_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    25119 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/checkers/duplication_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/checkers/improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/checkers/modified_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/checkers/python_ta_checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24301 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/checkers/short_problems.py
--rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/checkers/simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/checkers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/nonparsing_checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/process_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/linting/tweakers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/option_parses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint/prepare_explanations/
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/prepare_explanations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint/prepare_explanations/pylint_data/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/prepare_explanations/pylint_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15048 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/prepare_explanations/pylint_data/pylint_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint/prepare_explanations/thonny_data/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/prepare_explanations/thonny_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
--rw-r--r--   0 runner    (1001) docker     (127)   155599 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/prepare_explanations/thonny_data/thonny_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint/versions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/versions/pypi_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/versions/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-03-13 09:12:09.000000 edulint-3.6.0/edulint/versions/version_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-13 09:12:16.000000 edulint-3.6.0/edulint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-13 09:12:09.000000 edulint-3.6.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      518 2024-03-13 09:12:09.000000 edulint-3.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-13 09:12:16.000000 edulint-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-13 09:12:09.000000 edulint-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:12:16.000000 edulint-3.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    15534 2024-03-13 09:12:09.000000 edulint-3.6.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-03-13 09:12:09.000000 edulint-3.6.0/tests/test_duplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-03-13 09:12:09.000000 edulint-3.6.0/tests/test_improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    28932 2024-03-13 09:12:09.000000 edulint-3.6.0/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-03-13 09:12:09.000000 edulint-3.6.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-03-13 09:12:09.000000 edulint-3.6.0/tests/test_short_problems.py
--rw-r--r--   0 runner    (1001) docker     (127)    15806 2024-03-13 09:12:09.000000 edulint-3.6.0/tests/test_simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-03-13 09:12:09.000000 edulint-3.6.0/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:40.000000 edulint-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 15:49:32.000000 edulint-3.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-02 15:49:40.000000 edulint-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-02 15:49:32.000000 edulint-3.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/config/arg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17889 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/config/file_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint/config/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/config/files/cs0.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/config/files/default.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/config/files/empty.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/config/language_translations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/config/option_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/config/raw_flake8_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/config/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6156 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/edulint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/explanations.py
+-rw-r--r--   0 runner    (1001) docker     (127)   195728 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/explanations.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint/linting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint/linting/checkers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/checkers/basic_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25119 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/checkers/duplication_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/checkers/improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/checkers/modified_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/checkers/python_ta_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24301 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/checkers/short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/checkers/simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/checkers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/nonparsing_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/process_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/linting/tweakers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/option_parses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint/prepare_explanations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/prepare_explanations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint/prepare_explanations/pylint_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/prepare_explanations/pylint_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15048 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/prepare_explanations/pylint_data/pylint_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint/prepare_explanations/thonny_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/prepare_explanations/thonny_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
+-rw-r--r--   0 runner    (1001) docker     (127)   155599 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/prepare_explanations/thonny_data/thonny_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/versions/pypi_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/versions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-02 15:49:32.000000 edulint-3.6.1/edulint/versions/version_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 15:49:40.000000 edulint-3.6.1/edulint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 15:49:32.000000 edulint-3.6.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      518 2024-04-02 15:49:32.000000 edulint-3.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-02 15:49:40.000000 edulint-3.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-02 15:49:32.000000 edulint-3.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:49:40.000000 edulint-3.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15534 2024-04-02 15:49:32.000000 edulint-3.6.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-02 15:49:32.000000 edulint-3.6.1/tests/test_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-02 15:49:32.000000 edulint-3.6.1/tests/test_improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28932 2024-04-02 15:49:32.000000 edulint-3.6.1/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-02 15:49:32.000000 edulint-3.6.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-04-02 15:49:32.000000 edulint-3.6.1/tests/test_short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15806 2024-04-02 15:49:32.000000 edulint-3.6.1/tests/test_simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-02 15:49:32.000000 edulint-3.6.1/tests/test_visitors.py
```

### Comparing `edulint-3.6.0/LICENSE` & `edulint-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/PKG-INFO` & `edulint-3.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 3.6.0
+Version: 3.6.1
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-3.6.0/README.md` & `edulint-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/config/config.py` & `edulint-3.6.1/edulint/config/config.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/config/file_config.py` & `edulint-3.6.1/edulint/config/file_config.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/config/files/cs0.toml` & `edulint-3.6.1/edulint/config/files/cs0.toml`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/config/files/default.toml` & `edulint-3.6.1/edulint/config/files/default.toml`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/config/files/empty.toml` & `edulint-3.6.1/edulint/config/files/empty.toml`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/config/language_translations.py` & `edulint-3.6.1/edulint/config/language_translations.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/config/option_sets.py` & `edulint-3.6.1/edulint/config/option_sets.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/config/raw_flake8_patterns.py` & `edulint-3.6.1/edulint/config/raw_flake8_patterns.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/config/utils.py` & `edulint-3.6.1/edulint/config/utils.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/edulint.py` & `edulint-3.6.1/edulint/edulint.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,22 +103,24 @@
                 result.append(full_path)
         return result
 
     return extract_files_rec(None, files_or_dirs, [])
 
 
 def to_json(
-    configs: List[Tuple[ImmutableConfig, LangTranslations]], problems: List[Problem]
+    configs: List[Tuple[List[str], ImmutableConfig, LangTranslations]], problems: List[Problem]
 ) -> str:
     def config_to_json(obj: Any) -> str:
         if isinstance(obj, ImmutableConfig):
             return {arg.option.to_name(): arg.val for arg in obj.config}
         raise TypeError(f"Object of type {type(obj)} is not JSON serializable")
 
-    config_json = json.dumps([config for config, translation in configs], default=config_to_json)
+    config_json = json.dumps(
+        [config for _files, config, _translation in configs], default=config_to_json
+    )
     problems_json = Problem.schema().dumps(problems, indent=2, many=True)
     return f'{{"configs": {config_json}, "problems": {problems_json}}}'
 
 
 def check_for_updates(is_check_disabled: bool = False):
     if is_check_disabled:
         return
```

### Comparing `edulint-3.6.0/edulint/explanations.py` & `edulint-3.6.1/edulint/explanations.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/explanations.toml` & `edulint-3.6.1/edulint/explanations.toml`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linters.py` & `edulint-3.6.1/edulint/linters.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/checkers/basic_checker.py` & `edulint-3.6.1/edulint/linting/checkers/basic_checker.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/checkers/duplication_checker.py` & `edulint-3.6.1/edulint/linting/checkers/duplication_checker.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/checkers/improper_loop.py` & `edulint-3.6.1/edulint/linting/checkers/improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/checkers/modified_listener.py` & `edulint-3.6.1/edulint/linting/checkers/modified_listener.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/checkers/python_ta_checkers.py` & `edulint-3.6.1/edulint/linting/checkers/python_ta_checkers.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/checkers/short_problems.py` & `edulint-3.6.1/edulint/linting/checkers/short_problems.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/checkers/simplifiable_if.py` & `edulint-3.6.1/edulint/linting/checkers/simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/checkers/utils.py` & `edulint-3.6.1/edulint/linting/checkers/utils.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/linting.py` & `edulint-3.6.1/edulint/linting/linting.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/nonparsing_checkers.py` & `edulint-3.6.1/edulint/linting/nonparsing_checkers.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/overrides.py` & `edulint-3.6.1/edulint/linting/overrides.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/problem.py` & `edulint-3.6.1/edulint/linting/problem.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/process_handler.py` & `edulint-3.6.1/edulint/linting/process_handler.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/linting/tweakers.py` & `edulint-3.6.1/edulint/linting/tweakers.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/option_parses.py` & `edulint-3.6.1/edulint/option_parses.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/options.py` & `edulint-3.6.1/edulint/options.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/prepare_explanations/__init__.py` & `edulint-3.6.1/edulint/prepare_explanations/__init__.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py` & `edulint-3.6.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/prepare_explanations/pylint_data/pylint_messages.py` & `edulint-3.6.1/edulint/prepare_explanations/pylint_data/pylint_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py` & `edulint-3.6.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py` & `edulint-3.6.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/prepare_explanations/thonny_data/thonny_messages.py` & `edulint-3.6.1/edulint/prepare_explanations/thonny_data/thonny_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py` & `edulint-3.6.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/versions/pypi_helper.py` & `edulint-3.6.1/edulint/versions/pypi_helper.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/versions/utils.py` & `edulint-3.6.1/edulint/versions/utils.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint/versions/version_checker.py` & `edulint-3.6.1/edulint/versions/version_checker.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/edulint.egg-info/PKG-INFO` & `edulint-3.6.1/edulint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 3.6.0
+Version: 3.6.1
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-3.6.0/edulint.egg-info/SOURCES.txt` & `edulint-3.6.1/edulint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/requirements.txt` & `edulint-3.6.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/setup.cfg` & `edulint-3.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/setup.py` & `edulint-3.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/tests/test_config.py` & `edulint-3.6.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/tests/test_duplication.py` & `edulint-3.6.1/tests/test_duplication.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/tests/test_improper_loop.py` & `edulint-3.6.1/tests/test_improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/tests/test_lint.py` & `edulint-3.6.1/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/tests/test_main.py` & `edulint-3.6.1/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import pytest
 from edulint.edulint import main
 from os.path import join
+import sys
+import json
 
-
-def compare_output(monkeypatch, capsys, argv, output):
+def run(monkeypatch, capsys, argv) -> str:
     monkeypatch.setattr("sys.argv", ["script"] + argv)
     main()
     captured = capsys.readouterr()
-    import sys
 
     print(captured.err, file=sys.stderr)
-    assert captured.out == output
+
+    return captured.out
+
+def compare_output(monkeypatch, capsys, argv, output):
+    assert run(monkeypatch, capsys, argv) == output
 
 
 @pytest.mark.parametrize(
     "argv,output",
     [
         ([join("tests", "data", "hello_world.py")], ""),
         (
@@ -28,14 +32,25 @@
             f"{join('tests', 'data', 'custom_flake8_pylint.py')}:2:5: F841 local variable 'a' is assigned to but never used [default]\n",
         ),
     ],
 )
 def test_single_file_stdout(monkeypatch, capsys, argv, output):
     compare_output(monkeypatch, capsys, argv, output)
 
+@pytest.mark.parametrize(
+    "argv",
+    [
+        [join("tests", "data", "hello_world.py")],
+        [join("tests", "data", "custom_nonpep_assign.py")],
+    ],
+)
+def test_single_file_stdout_json(monkeypatch, capsys, argv):
+    out = run(monkeypatch, capsys, argv + ["--json"])
+    result = json.loads(out)
+    assert result
 
 @pytest.mark.parametrize(
     "argv,output",
     [
         (
             [
                 join("tests", "data", "hello_world.py"),
```

### Comparing `edulint-3.6.0/tests/test_short_problems.py` & `edulint-3.6.1/tests/test_short_problems.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/tests/test_simplifiable_if.py` & `edulint-3.6.1/tests/test_simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-3.6.0/tests/test_visitors.py` & `edulint-3.6.1/tests/test_visitors.py`

 * *Files identical despite different names*

