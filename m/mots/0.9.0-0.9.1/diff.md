# Comparing `tmp/mots-0.9.0.tar.gz` & `tmp/mots-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mots-0.9.0.tar", last modified: Fri Jun  2 18:07:40 2023, max compression
+gzip compressed data, was "mots-0.9.1.tar", last modified: Thu Jul 27 19:25:03 2023, max compression
```

## Comparing `mots-0.9.0.tar` & `mots-0.9.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.488805 mots-0.9.0/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.480805 mots-0.9.0/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3101 2023-06-02 18:07:00.000000 mots-0.9.0/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-02 18:07:00.000000 mots-0.9.0/.coveragerc
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-06-02 18:07:00.000000 mots-0.9.0/.flake8
--rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-06-02 18:07:00.000000 mots-0.9.0/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2023-06-02 18:07:00.000000 mots-0.9.0/.readthedocs.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-06-02 18:07:00.000000 mots-0.9.0/AUTHORS
--rw-r--r--   0 circleci  (1001) circleci  (1002)      495 2023-06-02 18:07:00.000000 mots-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16727 2023-06-02 18:07:00.000000 mots-0.9.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3813 2023-06-02 18:07:00.000000 mots-0.9.0/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-06-02 18:07:40.488805 mots-0.9.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      984 2023-06-02 18:07:00.000000 mots-0.9.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-06-02 18:07:00.000000 mots-0.9.0/docker-compose.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.480805 mots-0.9.0/documentation/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-06-02 18:07:00.000000 mots-0.9.0/documentation/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2153 2023-06-02 18:07:00.000000 mots-0.9.0/documentation/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13728 2023-06-02 18:07:00.000000 mots-0.9.0/documentation/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2023-06-02 18:07:00.000000 mots-0.9.0/mots.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      795 2023-06-02 18:07:00.000000 mots-0.9.0/mots.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2023-06-02 18:07:00.000000 mots-0.9.0/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.484805 mots-0.9.0/requirements/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-06-02 18:07:00.000000 mots-0.9.0/requirements/base.in
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      159 2023-06-02 18:07:00.000000 mots-0.9.0/requirements/get_filename
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33052 2023-06-02 18:07:00.000000 mots-0.9.0/requirements/python3.10.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35675 2023-06-02 18:07:00.000000 mots-0.9.0/requirements/python3.7.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33297 2023-06-02 18:07:00.000000 mots-0.9.0/requirements/python3.8.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33276 2023-06-02 18:07:00.000000 mots-0.9.0/requirements/python3.9.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1053 2023-06-02 18:07:40.488805 mots-0.9.0/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.480805 mots-0.9.0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.484805 mots-0.9.0/src/mots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      505 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2489 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/bmo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      808 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/ci.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15263 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14341 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/directory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6454 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/export.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/logging.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/mach_interface.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6937 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/module.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/pmo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2748 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.484805 mots-0.9.0/src/mots/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2211 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/templates/directory.template.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2381 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/templates/directory.template.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-06-02 18:07:00.000000 mots-0.9.0/src/mots/yaml.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.484805 mots-0.9.0/src/mots.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-06-02 18:07:40.000000 mots-0.9.0/src/mots.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-06-02 18:07:40.000000 mots-0.9.0/src/mots.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-02 18:07:40.000000 mots-0.9.0/src/mots.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       54 2023-06-02 18:07:40.000000 mots-0.9.0/src/mots.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-06-02 18:07:40.000000 mots-0.9.0/src/mots.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-06-02 18:07:40.000000 mots-0.9.0/src/mots.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 18:07:40.488805 mots-0.9.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4618 2023-06-02 18:07:00.000000 mots-0.9.0/tests/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9829 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7046 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_directory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5225 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_export.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5727 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_module.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_style.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4489 2023-06-02 18:07:00.000000 mots-0.9.0/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 19:25:03.908908 mots-0.9.1/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 19:25:03.904908 mots-0.9.1/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3101 2023-07-27 19:24:27.000000 mots-0.9.1/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-07-27 19:24:27.000000 mots-0.9.1/.coveragerc
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-07-27 19:24:27.000000 mots-0.9.1/.flake8
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-07-27 19:24:27.000000 mots-0.9.1/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2023-07-27 19:24:27.000000 mots-0.9.1/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-07-27 19:24:27.000000 mots-0.9.1/AUTHORS
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      495 2023-07-27 19:24:27.000000 mots-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16727 2023-07-27 19:24:27.000000 mots-0.9.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3813 2023-07-27 19:24:27.000000 mots-0.9.1/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-07-27 19:25:03.908908 mots-0.9.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      984 2023-07-27 19:24:27.000000 mots-0.9.1/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-07-27 19:24:27.000000 mots-0.9.1/docker-compose.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 19:25:03.904908 mots-0.9.1/documentation/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-07-27 19:24:27.000000 mots-0.9.1/documentation/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2153 2023-07-27 19:24:27.000000 mots-0.9.1/documentation/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13728 2023-07-27 19:24:27.000000 mots-0.9.1/documentation/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2023-07-27 19:24:27.000000 mots-0.9.1/mots.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      795 2023-07-27 19:24:27.000000 mots-0.9.1/mots.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2023-07-27 19:24:27.000000 mots-0.9.1/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 19:25:03.904908 mots-0.9.1/requirements/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-07-27 19:24:27.000000 mots-0.9.1/requirements/base.in
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      159 2023-07-27 19:24:27.000000 mots-0.9.1/requirements/get_filename
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33222 2023-07-27 19:24:27.000000 mots-0.9.1/requirements/python3.10.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35845 2023-07-27 19:24:27.000000 mots-0.9.1/requirements/python3.7.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33467 2023-07-27 19:24:27.000000 mots-0.9.1/requirements/python3.8.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33446 2023-07-27 19:24:27.000000 mots-0.9.1/requirements/python3.9.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1053 2023-07-27 19:25:03.908908 mots-0.9.1/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 19:25:03.900908 mots-0.9.1/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 19:25:03.908908 mots-0.9.1/src/mots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      505 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2489 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/bmo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      808 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/ci.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15305 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14373 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/directory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6454 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/export.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/logging.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/mach_interface.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6937 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/module.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/pmo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2748 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 19:25:03.908908 mots-0.9.1/src/mots/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2211 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/templates/directory.template.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2381 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/templates/directory.template.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2952 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-07-27 19:24:27.000000 mots-0.9.1/src/mots/yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 19:25:03.908908 mots-0.9.1/src/mots.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-07-27 19:25:03.000000 mots-0.9.1/src/mots.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-07-27 19:25:03.000000 mots-0.9.1/src/mots.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-27 19:25:03.000000 mots-0.9.1/src/mots.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       54 2023-07-27 19:25:03.000000 mots-0.9.1/src/mots.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-07-27 19:25:03.000000 mots-0.9.1/src/mots.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-07-27 19:25:03.000000 mots-0.9.1/src/mots.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 19:25:03.908908 mots-0.9.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4618 2023-07-27 19:24:27.000000 mots-0.9.1/tests/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-07-27 19:24:27.000000 mots-0.9.1/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9829 2023-07-27 19:24:27.000000 mots-0.9.1/tests/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7046 2023-07-27 19:24:27.000000 mots-0.9.1/tests/test_directory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5225 2023-07-27 19:24:27.000000 mots-0.9.1/tests/test_export.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5727 2023-07-27 19:24:27.000000 mots-0.9.1/tests/test_module.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2023-07-27 19:24:27.000000 mots-0.9.1/tests/test_settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-07-27 19:24:27.000000 mots-0.9.1/tests/test_style.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4489 2023-07-27 19:24:27.000000 mots-0.9.1/tests/test_utils.py
```

### Comparing `mots-0.9.0/.circleci/config.yml` & `mots-0.9.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/LICENSE` & `mots-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/Makefile` & `mots-0.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/PKG-INFO` & `mots-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mots
-Version: 0.9.0
+Version: 0.9.1
 Summary: Module Ownership in Tree System
 Home-page: https://github.com/mozilla-conduit/mots
 Author: Zeid Zabaneh
 Author-email: zeid@mozilla.com
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mots-0.9.0/README.md` & `mots-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/docker-compose.yml` & `mots-0.9.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/documentation/Makefile` & `mots-0.9.1/documentation/Makefile`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/documentation/conf.py` & `mots-0.9.1/documentation/conf.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/documentation/index.rst` & `mots-0.9.1/documentation/index.rst`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/mots.yaml` & `mots-0.9.1/mots.yaml`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/requirements/python3.10.txt` & `mots-0.9.1/requirements/python3.8.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --generate-hashes --output-file=requirements/python3.10.txt --resolver=backtracking requirements/base.in
+#    pip-compile --generate-hashes --output-file=requirements/python3.8.txt --resolver=backtracking requirements/base.in
 #
 alabaster==0.7.12 \
     --hash=sha256:446438bdcca0e05bd45ea2de1668c1d9b032e1a9154c2c259092d77031ddd359 \
     --hash=sha256:a661d72d58e6ea8a57f7a86e37d86716863ee5e92788398526d58b26a4e4dc02
     # via sphinx
 attrs==22.1.0 \
     --hash=sha256:29adc2665447e5191d0e7c568fde78b21f9672d344281d0c6e1ab085429b22b6 \
@@ -43,17 +43,17 @@
     --hash=sha256:085f7f33c15bd408dd9b17a4ad77c577db66d76203e5984b1bd59baeee948b2a \
     --hash=sha256:0d03255c47eb9bd2f26aa9bb7f2107732e7e8fe195ca2f64709fcf3b0a4a085c
     # via readme-renderer
 build==0.9.0 \
     --hash=sha256:1a07724e891cbd898923145eb7752ee7653674c511378eb9c7691aab1612bc3c \
     --hash=sha256:38a7a2b7a0bdc61a42a0a67509d88c71ecfc37b393baba770fae34e20929ff69
     # via -r requirements/base.in
-certifi==2022.12.7 \
-    --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
-    --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
+certifi==2023.7.22 \
+    --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
+    --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
     # via requests
 cffi==1.15.1 \
     --hash=sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5 \
     --hash=sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef \
     --hash=sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104 \
     --hash=sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426 \
     --hash=sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405 \
@@ -177,36 +177,38 @@
     --hash=sha256:de3001a203182842a4630e7b8d1a2c7c07ec1b45d3084a83d5d227a3806f530f \
     --hash=sha256:e07f4a4a9b41583d6eabec04f8b68076ab3cd44c20bd29332c6572dda36f372e \
     --hash=sha256:ef8674b0ee8cc11e2d574e3e2998aea5df5ab242e012286824ea3c6970580e53 \
     --hash=sha256:f4f05d88d9a80ad3cac6244d36dd89a3c00abc16371769f1340101d3cb899fc3 \
     --hash=sha256:f642e90754ee3e06b0e7e51bce3379590e76b7f76b708e1a71ff043f87025c84 \
     --hash=sha256:fc2af30ed0d5ae0b1abdb4ebdce598eafd5b35397d4d75deb341a614d333d987
     # via pytest-cov
-cryptography==39.0.1 \
-    --hash=sha256:0f8da300b5c8af9f98111ffd512910bc792b4c77392a9523624680f7956a99d4 \
-    --hash=sha256:35f7c7d015d474f4011e859e93e789c87d21f6f4880ebdc29896a60403328f1f \
-    --hash=sha256:5aa67414fcdfa22cf052e640cb5ddc461924a045cacf325cd164e65312d99502 \
-    --hash=sha256:5d2d8b87a490bfcd407ed9d49093793d0f75198a35e6eb1a923ce1ee86c62b41 \
-    --hash=sha256:6687ef6d0a6497e2b58e7c5b852b53f62142cfa7cd1555795758934da363a965 \
-    --hash=sha256:6f8ba7f0328b79f08bdacc3e4e66fb4d7aab0c3584e0bd41328dce5262e26b2e \
-    --hash=sha256:706843b48f9a3f9b9911979761c91541e3d90db1ca905fd63fee540a217698bc \
-    --hash=sha256:807ce09d4434881ca3a7594733669bd834f5b2c6d5c7e36f8c00f691887042ad \
-    --hash=sha256:83e17b26de248c33f3acffb922748151d71827d6021d98c70e6c1a25ddd78505 \
-    --hash=sha256:96f1157a7c08b5b189b16b47bc9db2332269d6680a196341bf30046330d15388 \
-    --hash=sha256:aec5a6c9864be7df2240c382740fcf3b96928c46604eaa7f3091f58b878c0bb6 \
-    --hash=sha256:b0afd054cd42f3d213bf82c629efb1ee5f22eba35bf0eec88ea9ea7304f511a2 \
-    --hash=sha256:ced4e447ae29ca194449a3f1ce132ded8fcab06971ef5f618605aacaa612beac \
-    --hash=sha256:d1f6198ee6d9148405e49887803907fe8962a23e6c6f83ea7d98f1c0de375695 \
-    --hash=sha256:e124352fd3db36a9d4a21c1aa27fd5d051e621845cb87fb851c08f4f75ce8be6 \
-    --hash=sha256:e422abdec8b5fa8462aa016786680720d78bdce7a30c652b7fadf83a4ba35336 \
-    --hash=sha256:ef8b72fa70b348724ff1218267e7f7375b8de4e8194d1636ee60510aae104cd0 \
-    --hash=sha256:f0c64d1bd842ca2633e74a1a28033d139368ad959872533b1bab8c80e8240a0c \
-    --hash=sha256:f24077a3b5298a5a06a8e0536e3ea9ec60e4c7ac486755e5fb6e6ea9b3500106 \
-    --hash=sha256:fdd188c8a6ef8769f148f88f859884507b954cc64db6b52f66ef199bb9ad660a \
-    --hash=sha256:fe913f20024eb2cb2f323e42a64bdf2911bb9738a15dba7d3cce48151034e3a8
+cryptography==41.0.2 \
+    --hash=sha256:01f1d9e537f9a15b037d5d9ee442b8c22e3ae11ce65ea1f3316a41c78756b711 \
+    --hash=sha256:079347de771f9282fbfe0e0236c716686950c19dee1b76240ab09ce1624d76d7 \
+    --hash=sha256:182be4171f9332b6741ee818ec27daff9fb00349f706629f5cbf417bd50e66fd \
+    --hash=sha256:192255f539d7a89f2102d07d7375b1e0a81f7478925b3bc2e0549ebf739dae0e \
+    --hash=sha256:2a034bf7d9ca894720f2ec1d8b7b5832d7e363571828037f9e0c4f18c1b58a58 \
+    --hash=sha256:342f3767e25876751e14f8459ad85e77e660537ca0a066e10e75df9c9e9099f0 \
+    --hash=sha256:439c3cc4c0d42fa999b83ded80a9a1fb54d53c58d6e59234cfe97f241e6c781d \
+    --hash=sha256:49c3222bb8f8e800aead2e376cbef687bc9e3cb9b58b29a261210456a7783d83 \
+    --hash=sha256:674b669d5daa64206c38e507808aae49904c988fa0a71c935e7006a3e1e83831 \
+    --hash=sha256:7a9a3bced53b7f09da251685224d6a260c3cb291768f54954e28f03ef14e3766 \
+    --hash=sha256:7af244b012711a26196450d34f483357e42aeddb04128885d95a69bd8b14b69b \
+    --hash=sha256:7d230bf856164de164ecb615ccc14c7fc6de6906ddd5b491f3af90d3514c925c \
+    --hash=sha256:84609ade00a6ec59a89729e87a503c6e36af98ddcd566d5f3be52e29ba993182 \
+    --hash=sha256:9a6673c1828db6270b76b22cc696f40cde9043eb90373da5c2f8f2158957f42f \
+    --hash=sha256:9b6d717393dbae53d4e52684ef4f022444fc1cce3c48c38cb74fca29e1f08eaa \
+    --hash=sha256:9c3fe6534d59d071ee82081ca3d71eed3210f76ebd0361798c74abc2bcf347d4 \
+    --hash=sha256:a719399b99377b218dac6cf547b6ec54e6ef20207b6165126a280b0ce97e0d2a \
+    --hash=sha256:b332cba64d99a70c1e0836902720887fb4529ea49ea7f5462cf6640e095e11d2 \
+    --hash=sha256:d124682c7a23c9764e54ca9ab5b308b14b18eba02722b8659fb238546de83a76 \
+    --hash=sha256:d73f419a56d74fef257955f51b18d046f3506270a5fd2ac5febbfa259d6c0fa5 \
+    --hash=sha256:f0dc40e6f7aa37af01aba07277d3d64d5a03dc66d682097541ec4da03cc140ee \
+    --hash=sha256:f14ad275364c8b4e525d018f6716537ae7b6d369c094805cae45300847e0894f \
+    --hash=sha256:f772610fe364372de33d76edcd313636a25684edb94cee53fd790195f5989d14
     # via secretstorage
 docutils==0.17.1 \
     --hash=sha256:686577d2e4c32380bb50cbb22f575ed742d58168cee37e99117a854bcd88f125 \
     --hash=sha256:cf316c8370a737a022b72b56874f6602acf974a37a9fba42ec2876387549fc61
     # via
     #   readme-renderer
     #   sphinx
@@ -234,14 +236,15 @@
     --hash=sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a
     # via sphinx
 importlib-metadata==5.1.0 \
     --hash=sha256:d5059f9f1e8e41f80e9c56c2ee58811450c31984dfa625329ffd7c0dad88a73b \
     --hash=sha256:d84d17e21670ec07990e1044a99efe8d615d860fd176fc29ef5c306068fda313
     # via
     #   keyring
+    #   sphinx
     #   twine
 iniconfig==1.1.1 \
     --hash=sha256:011e24c64b7f47f6ebd835bb12a743f2fbe9a26d4cecaa7f53bc4f35ee9da8b3 \
     --hash=sha256:bc3af051d7d14b2ee5ef9969666def0cd1a000e121eaea580d4a313df4b37f32
     # via pytest
 jaraco-classes==3.2.3 \
     --hash=sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158 \
@@ -354,17 +357,17 @@
     --hash=sha256:1d41b7c459ba0ee6c345f2eb9ae827cab14a7533a88c5c6f7e94923f72df92dc \
     --hash=sha256:6987826d6775056839940041beef5c08cc7e3d71d63149b48e36727f70144dc4
     # via flake8-docstrings
 pyflakes==3.0.1 \
     --hash=sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf \
     --hash=sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd
     # via flake8
-pygments==2.13.0 \
-    --hash=sha256:56a8508ae95f98e2b9bdf93a6be5ae3f7d8af858b43e02c5a2ff083726be40c1 \
-    --hash=sha256:f643f331ab57ba3c9d89212ee4a2dabc6e94f117cf4eefde99a0574720d14c42
+pygments==2.15.0 \
+    --hash=sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094 \
+    --hash=sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500
     # via
     #   readme-renderer
     #   rich
     #   sphinx
 pytest==7.2.0 \
     --hash=sha256:892f933d339f068883b6fd5a459f03d85bfcb355e4981e146d2c7616c21fef71 \
     --hash=sha256:c4014eb40e10f11f355ad4e3c2fb2c6c6d1919c73f3b5a433de4708202cade59
@@ -499,14 +502,20 @@
     #   coverage
     #   pep517
     #   pytest
 twine==4.0.2 \
     --hash=sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8 \
     --hash=sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8
     # via -r requirements/base.in
+typing-extensions==4.4.0 \
+    --hash=sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa \
+    --hash=sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e
+    # via
+    #   black
+    #   rich
 urllib3==1.26.13 \
     --hash=sha256:47cc05d99aaa09c9e72ed5809b60e7ba354e64b59c9c173ac3018642d8bb41fc \
     --hash=sha256:c083dd0dce68dbfbe1129d5271cb90f9447dea7d52097c6e0126120c521ddea8
     # via
     #   requests
     #   twine
 webencodings==0.5.1 \
```

### Comparing `mots-0.9.0/requirements/python3.7.txt` & `mots-0.9.1/requirements/python3.7.txt`

 * *Files 3% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     --hash=sha256:085f7f33c15bd408dd9b17a4ad77c577db66d76203e5984b1bd59baeee948b2a \
     --hash=sha256:0d03255c47eb9bd2f26aa9bb7f2107732e7e8fe195ca2f64709fcf3b0a4a085c
     # via readme-renderer
 build==0.9.0 \
     --hash=sha256:1a07724e891cbd898923145eb7752ee7653674c511378eb9c7691aab1612bc3c \
     --hash=sha256:38a7a2b7a0bdc61a42a0a67509d88c71ecfc37b393baba770fae34e20929ff69
     # via -r requirements/base.in
-certifi==2022.12.7 \
-    --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
-    --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
+certifi==2023.7.22 \
+    --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
+    --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
     # via requests
 cffi==1.15.1 \
     --hash=sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5 \
     --hash=sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef \
     --hash=sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104 \
     --hash=sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426 \
     --hash=sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405 \
@@ -177,36 +177,38 @@
     --hash=sha256:de3001a203182842a4630e7b8d1a2c7c07ec1b45d3084a83d5d227a3806f530f \
     --hash=sha256:e07f4a4a9b41583d6eabec04f8b68076ab3cd44c20bd29332c6572dda36f372e \
     --hash=sha256:ef8674b0ee8cc11e2d574e3e2998aea5df5ab242e012286824ea3c6970580e53 \
     --hash=sha256:f4f05d88d9a80ad3cac6244d36dd89a3c00abc16371769f1340101d3cb899fc3 \
     --hash=sha256:f642e90754ee3e06b0e7e51bce3379590e76b7f76b708e1a71ff043f87025c84 \
     --hash=sha256:fc2af30ed0d5ae0b1abdb4ebdce598eafd5b35397d4d75deb341a614d333d987
     # via pytest-cov
-cryptography==39.0.1 \
-    --hash=sha256:0f8da300b5c8af9f98111ffd512910bc792b4c77392a9523624680f7956a99d4 \
-    --hash=sha256:35f7c7d015d474f4011e859e93e789c87d21f6f4880ebdc29896a60403328f1f \
-    --hash=sha256:5aa67414fcdfa22cf052e640cb5ddc461924a045cacf325cd164e65312d99502 \
-    --hash=sha256:5d2d8b87a490bfcd407ed9d49093793d0f75198a35e6eb1a923ce1ee86c62b41 \
-    --hash=sha256:6687ef6d0a6497e2b58e7c5b852b53f62142cfa7cd1555795758934da363a965 \
-    --hash=sha256:6f8ba7f0328b79f08bdacc3e4e66fb4d7aab0c3584e0bd41328dce5262e26b2e \
-    --hash=sha256:706843b48f9a3f9b9911979761c91541e3d90db1ca905fd63fee540a217698bc \
-    --hash=sha256:807ce09d4434881ca3a7594733669bd834f5b2c6d5c7e36f8c00f691887042ad \
-    --hash=sha256:83e17b26de248c33f3acffb922748151d71827d6021d98c70e6c1a25ddd78505 \
-    --hash=sha256:96f1157a7c08b5b189b16b47bc9db2332269d6680a196341bf30046330d15388 \
-    --hash=sha256:aec5a6c9864be7df2240c382740fcf3b96928c46604eaa7f3091f58b878c0bb6 \
-    --hash=sha256:b0afd054cd42f3d213bf82c629efb1ee5f22eba35bf0eec88ea9ea7304f511a2 \
-    --hash=sha256:ced4e447ae29ca194449a3f1ce132ded8fcab06971ef5f618605aacaa612beac \
-    --hash=sha256:d1f6198ee6d9148405e49887803907fe8962a23e6c6f83ea7d98f1c0de375695 \
-    --hash=sha256:e124352fd3db36a9d4a21c1aa27fd5d051e621845cb87fb851c08f4f75ce8be6 \
-    --hash=sha256:e422abdec8b5fa8462aa016786680720d78bdce7a30c652b7fadf83a4ba35336 \
-    --hash=sha256:ef8b72fa70b348724ff1218267e7f7375b8de4e8194d1636ee60510aae104cd0 \
-    --hash=sha256:f0c64d1bd842ca2633e74a1a28033d139368ad959872533b1bab8c80e8240a0c \
-    --hash=sha256:f24077a3b5298a5a06a8e0536e3ea9ec60e4c7ac486755e5fb6e6ea9b3500106 \
-    --hash=sha256:fdd188c8a6ef8769f148f88f859884507b954cc64db6b52f66ef199bb9ad660a \
-    --hash=sha256:fe913f20024eb2cb2f323e42a64bdf2911bb9738a15dba7d3cce48151034e3a8
+cryptography==41.0.2 \
+    --hash=sha256:01f1d9e537f9a15b037d5d9ee442b8c22e3ae11ce65ea1f3316a41c78756b711 \
+    --hash=sha256:079347de771f9282fbfe0e0236c716686950c19dee1b76240ab09ce1624d76d7 \
+    --hash=sha256:182be4171f9332b6741ee818ec27daff9fb00349f706629f5cbf417bd50e66fd \
+    --hash=sha256:192255f539d7a89f2102d07d7375b1e0a81f7478925b3bc2e0549ebf739dae0e \
+    --hash=sha256:2a034bf7d9ca894720f2ec1d8b7b5832d7e363571828037f9e0c4f18c1b58a58 \
+    --hash=sha256:342f3767e25876751e14f8459ad85e77e660537ca0a066e10e75df9c9e9099f0 \
+    --hash=sha256:439c3cc4c0d42fa999b83ded80a9a1fb54d53c58d6e59234cfe97f241e6c781d \
+    --hash=sha256:49c3222bb8f8e800aead2e376cbef687bc9e3cb9b58b29a261210456a7783d83 \
+    --hash=sha256:674b669d5daa64206c38e507808aae49904c988fa0a71c935e7006a3e1e83831 \
+    --hash=sha256:7a9a3bced53b7f09da251685224d6a260c3cb291768f54954e28f03ef14e3766 \
+    --hash=sha256:7af244b012711a26196450d34f483357e42aeddb04128885d95a69bd8b14b69b \
+    --hash=sha256:7d230bf856164de164ecb615ccc14c7fc6de6906ddd5b491f3af90d3514c925c \
+    --hash=sha256:84609ade00a6ec59a89729e87a503c6e36af98ddcd566d5f3be52e29ba993182 \
+    --hash=sha256:9a6673c1828db6270b76b22cc696f40cde9043eb90373da5c2f8f2158957f42f \
+    --hash=sha256:9b6d717393dbae53d4e52684ef4f022444fc1cce3c48c38cb74fca29e1f08eaa \
+    --hash=sha256:9c3fe6534d59d071ee82081ca3d71eed3210f76ebd0361798c74abc2bcf347d4 \
+    --hash=sha256:a719399b99377b218dac6cf547b6ec54e6ef20207b6165126a280b0ce97e0d2a \
+    --hash=sha256:b332cba64d99a70c1e0836902720887fb4529ea49ea7f5462cf6640e095e11d2 \
+    --hash=sha256:d124682c7a23c9764e54ca9ab5b308b14b18eba02722b8659fb238546de83a76 \
+    --hash=sha256:d73f419a56d74fef257955f51b18d046f3506270a5fd2ac5febbfa259d6c0fa5 \
+    --hash=sha256:f0dc40e6f7aa37af01aba07277d3d64d5a03dc66d682097541ec4da03cc140ee \
+    --hash=sha256:f14ad275364c8b4e525d018f6716537ae7b6d369c094805cae45300847e0894f \
+    --hash=sha256:f772610fe364372de33d76edcd313636a25684edb94cee53fd790195f5989d14
     # via secretstorage
 docutils==0.17.1 \
     --hash=sha256:686577d2e4c32380bb50cbb22f575ed742d58168cee37e99117a854bcd88f125 \
     --hash=sha256:cf316c8370a737a022b72b56874f6602acf974a37a9fba42ec2876387549fc61
     # via
     #   readme-renderer
     #   sphinx
@@ -360,17 +362,17 @@
     --hash=sha256:1d41b7c459ba0ee6c345f2eb9ae827cab14a7533a88c5c6f7e94923f72df92dc \
     --hash=sha256:6987826d6775056839940041beef5c08cc7e3d71d63149b48e36727f70144dc4
     # via flake8-docstrings
 pyflakes==2.4.0 \
     --hash=sha256:05a85c2872edf37a4ed30b0cce2f6093e1d0581f8c19d7393122da7e25b2b24c \
     --hash=sha256:3bb3a3f256f4b7968c9c788781e4ff07dce46bdf12339dcda61053375426ee2e
     # via flake8
-pygments==2.13.0 \
-    --hash=sha256:56a8508ae95f98e2b9bdf93a6be5ae3f7d8af858b43e02c5a2ff083726be40c1 \
-    --hash=sha256:f643f331ab57ba3c9d89212ee4a2dabc6e94f117cf4eefde99a0574720d14c42
+pygments==2.15.0 \
+    --hash=sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094 \
+    --hash=sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500
     # via
     #   readme-renderer
     #   rich
     #   sphinx
 pytest==7.2.0 \
     --hash=sha256:892f933d339f068883b6fd5a459f03d85bfcb355e4981e146d2c7616c21fef71 \
     --hash=sha256:c4014eb40e10f11f355ad4e3c2fb2c6c6d1919c73f3b5a433de4708202cade59
```

### Comparing `mots-0.9.0/requirements/python3.8.txt` & `mots-0.9.1/requirements/python3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --generate-hashes --output-file=requirements/python3.8.txt --resolver=backtracking requirements/base.in
+#    pip-compile --generate-hashes --output-file=requirements/python3.10.txt --resolver=backtracking requirements/base.in
 #
 alabaster==0.7.12 \
     --hash=sha256:446438bdcca0e05bd45ea2de1668c1d9b032e1a9154c2c259092d77031ddd359 \
     --hash=sha256:a661d72d58e6ea8a57f7a86e37d86716863ee5e92788398526d58b26a4e4dc02
     # via sphinx
 attrs==22.1.0 \
     --hash=sha256:29adc2665447e5191d0e7c568fde78b21f9672d344281d0c6e1ab085429b22b6 \
@@ -43,17 +43,17 @@
     --hash=sha256:085f7f33c15bd408dd9b17a4ad77c577db66d76203e5984b1bd59baeee948b2a \
     --hash=sha256:0d03255c47eb9bd2f26aa9bb7f2107732e7e8fe195ca2f64709fcf3b0a4a085c
     # via readme-renderer
 build==0.9.0 \
     --hash=sha256:1a07724e891cbd898923145eb7752ee7653674c511378eb9c7691aab1612bc3c \
     --hash=sha256:38a7a2b7a0bdc61a42a0a67509d88c71ecfc37b393baba770fae34e20929ff69
     # via -r requirements/base.in
-certifi==2022.12.7 \
-    --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
-    --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
+certifi==2023.7.22 \
+    --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
+    --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
     # via requests
 cffi==1.15.1 \
     --hash=sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5 \
     --hash=sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef \
     --hash=sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104 \
     --hash=sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426 \
     --hash=sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405 \
@@ -177,36 +177,38 @@
     --hash=sha256:de3001a203182842a4630e7b8d1a2c7c07ec1b45d3084a83d5d227a3806f530f \
     --hash=sha256:e07f4a4a9b41583d6eabec04f8b68076ab3cd44c20bd29332c6572dda36f372e \
     --hash=sha256:ef8674b0ee8cc11e2d574e3e2998aea5df5ab242e012286824ea3c6970580e53 \
     --hash=sha256:f4f05d88d9a80ad3cac6244d36dd89a3c00abc16371769f1340101d3cb899fc3 \
     --hash=sha256:f642e90754ee3e06b0e7e51bce3379590e76b7f76b708e1a71ff043f87025c84 \
     --hash=sha256:fc2af30ed0d5ae0b1abdb4ebdce598eafd5b35397d4d75deb341a614d333d987
     # via pytest-cov
-cryptography==39.0.1 \
-    --hash=sha256:0f8da300b5c8af9f98111ffd512910bc792b4c77392a9523624680f7956a99d4 \
-    --hash=sha256:35f7c7d015d474f4011e859e93e789c87d21f6f4880ebdc29896a60403328f1f \
-    --hash=sha256:5aa67414fcdfa22cf052e640cb5ddc461924a045cacf325cd164e65312d99502 \
-    --hash=sha256:5d2d8b87a490bfcd407ed9d49093793d0f75198a35e6eb1a923ce1ee86c62b41 \
-    --hash=sha256:6687ef6d0a6497e2b58e7c5b852b53f62142cfa7cd1555795758934da363a965 \
-    --hash=sha256:6f8ba7f0328b79f08bdacc3e4e66fb4d7aab0c3584e0bd41328dce5262e26b2e \
-    --hash=sha256:706843b48f9a3f9b9911979761c91541e3d90db1ca905fd63fee540a217698bc \
-    --hash=sha256:807ce09d4434881ca3a7594733669bd834f5b2c6d5c7e36f8c00f691887042ad \
-    --hash=sha256:83e17b26de248c33f3acffb922748151d71827d6021d98c70e6c1a25ddd78505 \
-    --hash=sha256:96f1157a7c08b5b189b16b47bc9db2332269d6680a196341bf30046330d15388 \
-    --hash=sha256:aec5a6c9864be7df2240c382740fcf3b96928c46604eaa7f3091f58b878c0bb6 \
-    --hash=sha256:b0afd054cd42f3d213bf82c629efb1ee5f22eba35bf0eec88ea9ea7304f511a2 \
-    --hash=sha256:ced4e447ae29ca194449a3f1ce132ded8fcab06971ef5f618605aacaa612beac \
-    --hash=sha256:d1f6198ee6d9148405e49887803907fe8962a23e6c6f83ea7d98f1c0de375695 \
-    --hash=sha256:e124352fd3db36a9d4a21c1aa27fd5d051e621845cb87fb851c08f4f75ce8be6 \
-    --hash=sha256:e422abdec8b5fa8462aa016786680720d78bdce7a30c652b7fadf83a4ba35336 \
-    --hash=sha256:ef8b72fa70b348724ff1218267e7f7375b8de4e8194d1636ee60510aae104cd0 \
-    --hash=sha256:f0c64d1bd842ca2633e74a1a28033d139368ad959872533b1bab8c80e8240a0c \
-    --hash=sha256:f24077a3b5298a5a06a8e0536e3ea9ec60e4c7ac486755e5fb6e6ea9b3500106 \
-    --hash=sha256:fdd188c8a6ef8769f148f88f859884507b954cc64db6b52f66ef199bb9ad660a \
-    --hash=sha256:fe913f20024eb2cb2f323e42a64bdf2911bb9738a15dba7d3cce48151034e3a8
+cryptography==41.0.2 \
+    --hash=sha256:01f1d9e537f9a15b037d5d9ee442b8c22e3ae11ce65ea1f3316a41c78756b711 \
+    --hash=sha256:079347de771f9282fbfe0e0236c716686950c19dee1b76240ab09ce1624d76d7 \
+    --hash=sha256:182be4171f9332b6741ee818ec27daff9fb00349f706629f5cbf417bd50e66fd \
+    --hash=sha256:192255f539d7a89f2102d07d7375b1e0a81f7478925b3bc2e0549ebf739dae0e \
+    --hash=sha256:2a034bf7d9ca894720f2ec1d8b7b5832d7e363571828037f9e0c4f18c1b58a58 \
+    --hash=sha256:342f3767e25876751e14f8459ad85e77e660537ca0a066e10e75df9c9e9099f0 \
+    --hash=sha256:439c3cc4c0d42fa999b83ded80a9a1fb54d53c58d6e59234cfe97f241e6c781d \
+    --hash=sha256:49c3222bb8f8e800aead2e376cbef687bc9e3cb9b58b29a261210456a7783d83 \
+    --hash=sha256:674b669d5daa64206c38e507808aae49904c988fa0a71c935e7006a3e1e83831 \
+    --hash=sha256:7a9a3bced53b7f09da251685224d6a260c3cb291768f54954e28f03ef14e3766 \
+    --hash=sha256:7af244b012711a26196450d34f483357e42aeddb04128885d95a69bd8b14b69b \
+    --hash=sha256:7d230bf856164de164ecb615ccc14c7fc6de6906ddd5b491f3af90d3514c925c \
+    --hash=sha256:84609ade00a6ec59a89729e87a503c6e36af98ddcd566d5f3be52e29ba993182 \
+    --hash=sha256:9a6673c1828db6270b76b22cc696f40cde9043eb90373da5c2f8f2158957f42f \
+    --hash=sha256:9b6d717393dbae53d4e52684ef4f022444fc1cce3c48c38cb74fca29e1f08eaa \
+    --hash=sha256:9c3fe6534d59d071ee82081ca3d71eed3210f76ebd0361798c74abc2bcf347d4 \
+    --hash=sha256:a719399b99377b218dac6cf547b6ec54e6ef20207b6165126a280b0ce97e0d2a \
+    --hash=sha256:b332cba64d99a70c1e0836902720887fb4529ea49ea7f5462cf6640e095e11d2 \
+    --hash=sha256:d124682c7a23c9764e54ca9ab5b308b14b18eba02722b8659fb238546de83a76 \
+    --hash=sha256:d73f419a56d74fef257955f51b18d046f3506270a5fd2ac5febbfa259d6c0fa5 \
+    --hash=sha256:f0dc40e6f7aa37af01aba07277d3d64d5a03dc66d682097541ec4da03cc140ee \
+    --hash=sha256:f14ad275364c8b4e525d018f6716537ae7b6d369c094805cae45300847e0894f \
+    --hash=sha256:f772610fe364372de33d76edcd313636a25684edb94cee53fd790195f5989d14
     # via secretstorage
 docutils==0.17.1 \
     --hash=sha256:686577d2e4c32380bb50cbb22f575ed742d58168cee37e99117a854bcd88f125 \
     --hash=sha256:cf316c8370a737a022b72b56874f6602acf974a37a9fba42ec2876387549fc61
     # via
     #   readme-renderer
     #   sphinx
@@ -234,15 +236,14 @@
     --hash=sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a
     # via sphinx
 importlib-metadata==5.1.0 \
     --hash=sha256:d5059f9f1e8e41f80e9c56c2ee58811450c31984dfa625329ffd7c0dad88a73b \
     --hash=sha256:d84d17e21670ec07990e1044a99efe8d615d860fd176fc29ef5c306068fda313
     # via
     #   keyring
-    #   sphinx
     #   twine
 iniconfig==1.1.1 \
     --hash=sha256:011e24c64b7f47f6ebd835bb12a743f2fbe9a26d4cecaa7f53bc4f35ee9da8b3 \
     --hash=sha256:bc3af051d7d14b2ee5ef9969666def0cd1a000e121eaea580d4a313df4b37f32
     # via pytest
 jaraco-classes==3.2.3 \
     --hash=sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158 \
@@ -355,17 +356,17 @@
     --hash=sha256:1d41b7c459ba0ee6c345f2eb9ae827cab14a7533a88c5c6f7e94923f72df92dc \
     --hash=sha256:6987826d6775056839940041beef5c08cc7e3d71d63149b48e36727f70144dc4
     # via flake8-docstrings
 pyflakes==3.0.1 \
     --hash=sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf \
     --hash=sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd
     # via flake8
-pygments==2.13.0 \
-    --hash=sha256:56a8508ae95f98e2b9bdf93a6be5ae3f7d8af858b43e02c5a2ff083726be40c1 \
-    --hash=sha256:f643f331ab57ba3c9d89212ee4a2dabc6e94f117cf4eefde99a0574720d14c42
+pygments==2.15.0 \
+    --hash=sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094 \
+    --hash=sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500
     # via
     #   readme-renderer
     #   rich
     #   sphinx
 pytest==7.2.0 \
     --hash=sha256:892f933d339f068883b6fd5a459f03d85bfcb355e4981e146d2c7616c21fef71 \
     --hash=sha256:c4014eb40e10f11f355ad4e3c2fb2c6c6d1919c73f3b5a433de4708202cade59
@@ -500,20 +501,14 @@
     #   coverage
     #   pep517
     #   pytest
 twine==4.0.2 \
     --hash=sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8 \
     --hash=sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8
     # via -r requirements/base.in
-typing-extensions==4.4.0 \
-    --hash=sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa \
-    --hash=sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e
-    # via
-    #   black
-    #   rich
 urllib3==1.26.13 \
     --hash=sha256:47cc05d99aaa09c9e72ed5809b60e7ba354e64b59c9c173ac3018642d8bb41fc \
     --hash=sha256:c083dd0dce68dbfbe1129d5271cb90f9447dea7d52097c6e0126120c521ddea8
     # via
     #   requests
     #   twine
 webencodings==0.5.1 \
```

### Comparing `mots-0.9.0/requirements/python3.9.txt` & `mots-0.9.1/requirements/python3.9.txt`

 * *Files 3% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     --hash=sha256:085f7f33c15bd408dd9b17a4ad77c577db66d76203e5984b1bd59baeee948b2a \
     --hash=sha256:0d03255c47eb9bd2f26aa9bb7f2107732e7e8fe195ca2f64709fcf3b0a4a085c
     # via readme-renderer
 build==0.9.0 \
     --hash=sha256:1a07724e891cbd898923145eb7752ee7653674c511378eb9c7691aab1612bc3c \
     --hash=sha256:38a7a2b7a0bdc61a42a0a67509d88c71ecfc37b393baba770fae34e20929ff69
     # via -r requirements/base.in
-certifi==2022.12.7 \
-    --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
-    --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
+certifi==2023.7.22 \
+    --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
+    --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
     # via requests
 cffi==1.15.1 \
     --hash=sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5 \
     --hash=sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef \
     --hash=sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104 \
     --hash=sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426 \
     --hash=sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405 \
@@ -177,36 +177,38 @@
     --hash=sha256:de3001a203182842a4630e7b8d1a2c7c07ec1b45d3084a83d5d227a3806f530f \
     --hash=sha256:e07f4a4a9b41583d6eabec04f8b68076ab3cd44c20bd29332c6572dda36f372e \
     --hash=sha256:ef8674b0ee8cc11e2d574e3e2998aea5df5ab242e012286824ea3c6970580e53 \
     --hash=sha256:f4f05d88d9a80ad3cac6244d36dd89a3c00abc16371769f1340101d3cb899fc3 \
     --hash=sha256:f642e90754ee3e06b0e7e51bce3379590e76b7f76b708e1a71ff043f87025c84 \
     --hash=sha256:fc2af30ed0d5ae0b1abdb4ebdce598eafd5b35397d4d75deb341a614d333d987
     # via pytest-cov
-cryptography==39.0.1 \
-    --hash=sha256:0f8da300b5c8af9f98111ffd512910bc792b4c77392a9523624680f7956a99d4 \
-    --hash=sha256:35f7c7d015d474f4011e859e93e789c87d21f6f4880ebdc29896a60403328f1f \
-    --hash=sha256:5aa67414fcdfa22cf052e640cb5ddc461924a045cacf325cd164e65312d99502 \
-    --hash=sha256:5d2d8b87a490bfcd407ed9d49093793d0f75198a35e6eb1a923ce1ee86c62b41 \
-    --hash=sha256:6687ef6d0a6497e2b58e7c5b852b53f62142cfa7cd1555795758934da363a965 \
-    --hash=sha256:6f8ba7f0328b79f08bdacc3e4e66fb4d7aab0c3584e0bd41328dce5262e26b2e \
-    --hash=sha256:706843b48f9a3f9b9911979761c91541e3d90db1ca905fd63fee540a217698bc \
-    --hash=sha256:807ce09d4434881ca3a7594733669bd834f5b2c6d5c7e36f8c00f691887042ad \
-    --hash=sha256:83e17b26de248c33f3acffb922748151d71827d6021d98c70e6c1a25ddd78505 \
-    --hash=sha256:96f1157a7c08b5b189b16b47bc9db2332269d6680a196341bf30046330d15388 \
-    --hash=sha256:aec5a6c9864be7df2240c382740fcf3b96928c46604eaa7f3091f58b878c0bb6 \
-    --hash=sha256:b0afd054cd42f3d213bf82c629efb1ee5f22eba35bf0eec88ea9ea7304f511a2 \
-    --hash=sha256:ced4e447ae29ca194449a3f1ce132ded8fcab06971ef5f618605aacaa612beac \
-    --hash=sha256:d1f6198ee6d9148405e49887803907fe8962a23e6c6f83ea7d98f1c0de375695 \
-    --hash=sha256:e124352fd3db36a9d4a21c1aa27fd5d051e621845cb87fb851c08f4f75ce8be6 \
-    --hash=sha256:e422abdec8b5fa8462aa016786680720d78bdce7a30c652b7fadf83a4ba35336 \
-    --hash=sha256:ef8b72fa70b348724ff1218267e7f7375b8de4e8194d1636ee60510aae104cd0 \
-    --hash=sha256:f0c64d1bd842ca2633e74a1a28033d139368ad959872533b1bab8c80e8240a0c \
-    --hash=sha256:f24077a3b5298a5a06a8e0536e3ea9ec60e4c7ac486755e5fb6e6ea9b3500106 \
-    --hash=sha256:fdd188c8a6ef8769f148f88f859884507b954cc64db6b52f66ef199bb9ad660a \
-    --hash=sha256:fe913f20024eb2cb2f323e42a64bdf2911bb9738a15dba7d3cce48151034e3a8
+cryptography==41.0.2 \
+    --hash=sha256:01f1d9e537f9a15b037d5d9ee442b8c22e3ae11ce65ea1f3316a41c78756b711 \
+    --hash=sha256:079347de771f9282fbfe0e0236c716686950c19dee1b76240ab09ce1624d76d7 \
+    --hash=sha256:182be4171f9332b6741ee818ec27daff9fb00349f706629f5cbf417bd50e66fd \
+    --hash=sha256:192255f539d7a89f2102d07d7375b1e0a81f7478925b3bc2e0549ebf739dae0e \
+    --hash=sha256:2a034bf7d9ca894720f2ec1d8b7b5832d7e363571828037f9e0c4f18c1b58a58 \
+    --hash=sha256:342f3767e25876751e14f8459ad85e77e660537ca0a066e10e75df9c9e9099f0 \
+    --hash=sha256:439c3cc4c0d42fa999b83ded80a9a1fb54d53c58d6e59234cfe97f241e6c781d \
+    --hash=sha256:49c3222bb8f8e800aead2e376cbef687bc9e3cb9b58b29a261210456a7783d83 \
+    --hash=sha256:674b669d5daa64206c38e507808aae49904c988fa0a71c935e7006a3e1e83831 \
+    --hash=sha256:7a9a3bced53b7f09da251685224d6a260c3cb291768f54954e28f03ef14e3766 \
+    --hash=sha256:7af244b012711a26196450d34f483357e42aeddb04128885d95a69bd8b14b69b \
+    --hash=sha256:7d230bf856164de164ecb615ccc14c7fc6de6906ddd5b491f3af90d3514c925c \
+    --hash=sha256:84609ade00a6ec59a89729e87a503c6e36af98ddcd566d5f3be52e29ba993182 \
+    --hash=sha256:9a6673c1828db6270b76b22cc696f40cde9043eb90373da5c2f8f2158957f42f \
+    --hash=sha256:9b6d717393dbae53d4e52684ef4f022444fc1cce3c48c38cb74fca29e1f08eaa \
+    --hash=sha256:9c3fe6534d59d071ee82081ca3d71eed3210f76ebd0361798c74abc2bcf347d4 \
+    --hash=sha256:a719399b99377b218dac6cf547b6ec54e6ef20207b6165126a280b0ce97e0d2a \
+    --hash=sha256:b332cba64d99a70c1e0836902720887fb4529ea49ea7f5462cf6640e095e11d2 \
+    --hash=sha256:d124682c7a23c9764e54ca9ab5b308b14b18eba02722b8659fb238546de83a76 \
+    --hash=sha256:d73f419a56d74fef257955f51b18d046f3506270a5fd2ac5febbfa259d6c0fa5 \
+    --hash=sha256:f0dc40e6f7aa37af01aba07277d3d64d5a03dc66d682097541ec4da03cc140ee \
+    --hash=sha256:f14ad275364c8b4e525d018f6716537ae7b6d369c094805cae45300847e0894f \
+    --hash=sha256:f772610fe364372de33d76edcd313636a25684edb94cee53fd790195f5989d14
     # via secretstorage
 docutils==0.17.1 \
     --hash=sha256:686577d2e4c32380bb50cbb22f575ed742d58168cee37e99117a854bcd88f125 \
     --hash=sha256:cf316c8370a737a022b72b56874f6602acf974a37a9fba42ec2876387549fc61
     # via
     #   readme-renderer
     #   sphinx
@@ -355,17 +357,17 @@
     --hash=sha256:1d41b7c459ba0ee6c345f2eb9ae827cab14a7533a88c5c6f7e94923f72df92dc \
     --hash=sha256:6987826d6775056839940041beef5c08cc7e3d71d63149b48e36727f70144dc4
     # via flake8-docstrings
 pyflakes==3.0.1 \
     --hash=sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf \
     --hash=sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd
     # via flake8
-pygments==2.13.0 \
-    --hash=sha256:56a8508ae95f98e2b9bdf93a6be5ae3f7d8af858b43e02c5a2ff083726be40c1 \
-    --hash=sha256:f643f331ab57ba3c9d89212ee4a2dabc6e94f117cf4eefde99a0574720d14c42
+pygments==2.15.0 \
+    --hash=sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094 \
+    --hash=sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500
     # via
     #   readme-renderer
     #   rich
     #   sphinx
 pytest==7.2.0 \
     --hash=sha256:892f933d339f068883b6fd5a459f03d85bfcb355e4981e146d2c7616c21fef71 \
     --hash=sha256:c4014eb40e10f11f355ad4e3c2fb2c6c6d1919c73f3b5a433de4708202cade59
```

### Comparing `mots-0.9.0/setup.cfg` & `mots-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots/bmo.py` & `mots-0.9.1/src/mots/bmo.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots/ci.py` & `mots-0.9.1/src/mots/ci.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots/cli.py` & `mots-0.9.1/src/mots/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,24 +160,24 @@
     # Render output based on provided format.
     output = export_to_format(directory, frmt)
 
     if not args.out:
         # Explicit output path was not provided, try to get it from config.
         if file_config.config.get("export", {}).get("path"):
             out_path = Path(file_config.config["export"]["path"])
-            with out_path.open("w", encoding="utf-8") as f:
+            with out_path.open("w", encoding="utf-8", newline="\n") as f:
                 logger.info(f"Writing output to specified file path ({out_path})...")
                 f.write(output)
         else:
             # No output path could be determined, so output to standard out.
             print(output)
     else:
         # TODO: do more checks here to make sure we don't overwrite important things.
         logger.info(f"Writing output to specified file path ({args.out})...")
-        with args.out.open("w", encoding="utf-8") as f:
+        with args.out.open("w", encoding="utf-8", newline="\n") as f:
             f.write(output)
 
 
 def export_and_clean(args: argparse.Namespace) -> None:
     """Run clean, export, and clean again to save users keystrokes."""
     # The first clean checks mots.yaml for any issues and synchronizes with BMO.
     clean(args)
@@ -215,15 +215,15 @@
 
     overrides[key] = _type(value)
     value_output = value if not is_secure else "*" * 10
     logger.info(
         f"{key} is now set to {value_output} ({_type.__name__}) in overrides file."
     )
 
-    with settings.OVERRIDES_FILE.open("w", encoding="utf-8") as f:
+    with settings.OVERRIDES_FILE.open("w", encoding="utf-8", newline="\n") as f:
         yaml.dump(overrides, f)
 
 
 def read(args: argparse.Namespace):
     """Print the value of a specified settings variable.
 
     If no key is provided, prints all available settings variables.
```

### Comparing `mots-0.9.0/src/mots/config.py` & `mots-0.9.1/src/mots/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         return errors
 
     def write(self, hashes: dict | None = None):
         """Write configuration to file, and update the timestamp and hashes."""
         logger.debug(f"Writing configuration to {self.path}")
         self.config["updated_at"] = datetime.now().isoformat()
         self.config["hashes"] = hashes or {}
-        with self.path.open("w") as f:
+        with self.path.open("w", encoding="utf-8", newline="\n") as f:
             yaml.dump(self.config, f)
 
 
 def reference_anchor_for_module(
     index: int,
     person: dict,
     key: str,
```

### Comparing `mots-0.9.0/src/mots/directory.py` & `mots-0.9.1/src/mots/directory.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots/export.py` & `mots-0.9.1/src/mots/export.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots/logging.py` & `mots-0.9.1/src/mots/logging.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots/mach_interface.py` & `mots-0.9.1/src/mots/mach_interface.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots/module.py` & `mots-0.9.1/src/mots/module.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots/pmo.py` & `mots-0.9.1/src/mots/pmo.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots/settings.py` & `mots-0.9.1/src/mots/settings.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots/templates/directory.template.md` & `mots-0.9.1/src/mots/templates/directory.template.md`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots/templates/directory.template.rst` & `mots-0.9.1/src/mots/templates/directory.template.rst`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots/utils.py` & `mots-0.9.1/src/mots/utils.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots/yaml.py` & `mots-0.9.1/src/mots/yaml.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/src/mots.egg-info/PKG-INFO` & `mots-0.9.1/src/mots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mots
-Version: 0.9.0
+Version: 0.9.1
 Summary: Module Ownership in Tree System
 Home-page: https://github.com/mozilla-conduit/mots
 Author: Zeid Zabaneh
 Author-email: zeid@mozilla.com
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mots-0.9.0/src/mots.egg-info/SOURCES.txt` & `mots-0.9.1/src/mots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/tests/conftest.py` & `mots-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/tests/test_config.py` & `mots-0.9.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/tests/test_directory.py` & `mots-0.9.1/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/tests/test_export.py` & `mots-0.9.1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/tests/test_module.py` & `mots-0.9.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/tests/test_settings.py` & `mots-0.9.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/tests/test_style.py` & `mots-0.9.1/tests/test_style.py`

 * *Files identical despite different names*

### Comparing `mots-0.9.0/tests/test_utils.py` & `mots-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

