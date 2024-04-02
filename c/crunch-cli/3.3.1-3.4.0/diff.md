# Comparing `tmp/crunch-cli-3.3.1.tar.gz` & `tmp/crunch-cli-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-3.3.1.tar", last modified: Thu Mar 28 14:56:53 2024, max compression
+gzip compressed data, was "crunch-cli-3.4.0.tar", last modified: Tue Apr  2 12:34:26 2024, max compression
```

## Comparing `crunch-cli-3.3.1.tar` & `crunch-cli-3.4.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:53.460240 crunch-cli-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-03-28 14:56:53.456240 crunch-cli-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:53.448240 crunch-cli-3.3.1/crunch/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:53.448240 crunch-cli-3.3.1/crunch/api/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:53.452240 crunch-cli-3.3.1/crunch/api/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/competition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/crunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/data_release.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/enum_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/quickstarter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/round.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/domain/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/api/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:53.452240 crunch-cli-3.3.1/crunch/checker/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/checker/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/checker/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16408 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:53.452240 crunch-cli-3.3.1/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/command/quickstarter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/command/update_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/monkey_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:53.452240 crunch-cli-3.3.1/crunch/orthogonalization/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/orthogonalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/orthogonalization/_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/orthogonalization/orthogonalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:53.456240 crunch-cli-3.3.1/crunch/runner/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17612 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/runner/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    13908 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/runner/cloud_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/runner/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/runner/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:53.456240 crunch-cli-3.3.1/crunch/scoring/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/scoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:53.456240 crunch-cli-3.3.1/crunch/scoring/_format/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/scoring/_format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/scoring/_format/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/scoring/_format/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/scoring/reducers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/scoring/score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/scoring/scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/store.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:53.456240 crunch-cli-3.3.1/crunch/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/crunch/vendor/datacrunch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:53.456240 crunch-cli-3.3.1/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-03-28 14:56:53.000000 crunch-cli-3.3.1/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-03-28 14:56:53.000000 crunch-cli-3.3.1/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:56:53.000000 crunch-cli-3.3.1/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-28 14:56:53.000000 crunch-cli-3.3.1/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:56:53.000000 crunch-cli-3.3.1/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-28 14:56:53.000000 crunch-cli-3.3.1/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-28 14:56:53.000000 crunch-cli-3.3.1/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 14:56:53.460240 crunch-cli-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-28 14:56:41.000000 crunch-cli-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:34:26.119532 crunch-cli-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-02 12:34:26.119532 crunch-cli-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:34:26.107532 crunch-cli-3.4.0/crunch/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:34:26.107532 crunch-cli-3.4.0/crunch/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:34:26.111532 crunch-cli-3.4.0/crunch/api/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/competition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/crunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/data_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/enum_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/quickstarter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/round.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/domain/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/api/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:34:26.111532 crunch-cli-3.4.0/crunch/checker/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/checker/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/checker/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16408 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:34:26.115532 crunch-cli-3.4.0/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/command/quickstarter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/command/update_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/monkey_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:34:26.115532 crunch-cli-3.4.0/crunch/orthogonalization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/orthogonalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/orthogonalization/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/orthogonalization/orthogonalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:34:26.115532 crunch-cli-3.4.0/crunch/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17612 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/runner/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13908 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/runner/cloud_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/runner/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/runner/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:34:26.115532 crunch-cli-3.4.0/crunch/scoring/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/scoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:34:26.119532 crunch-cli-3.4.0/crunch/scoring/_format/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/scoring/_format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/scoring/_format/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/scoring/_format/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/scoring/reducers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/scoring/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/scoring/scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:34:26.119532 crunch-cli-3.4.0/crunch/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/crunch/vendor/datacrunch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:34:26.119532 crunch-cli-3.4.0/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-02 12:34:26.000000 crunch-cli-3.4.0/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-02 12:34:26.000000 crunch-cli-3.4.0/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:34:26.000000 crunch-cli-3.4.0/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 12:34:26.000000 crunch-cli-3.4.0/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:34:26.000000 crunch-cli-3.4.0/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-02 12:34:26.000000 crunch-cli-3.4.0/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 12:34:26.000000 crunch-cli-3.4.0/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:34:26.119532 crunch-cli-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-02 12:34:21.000000 crunch-cli-3.4.0/setup.py
```

### Comparing `crunch-cli-3.3.1/PKG-INFO` & `crunch-cli-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crunch-cli
-Version: 3.3.1
+Version: 3.4.0
 Summary: crunch-cli - CLI of the CrunchDAO Platform
 Home-page: https://github.com/crunchdao/crunch-cli
 Author: Enzo CACERES
 Author-email: enzo.caceres@crunchdao.com
 Keywords: package development template
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `crunch-cli-3.3.1/README.md` & `crunch-cli-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/auth.py` & `crunch-cli-3.4.0/crunch/api/auth.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/client.py` & `crunch-cli-3.4.0/crunch/api/client.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/__init__.py` & `crunch-cli-3.4.0/crunch/api/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/check.py` & `crunch-cli-3.4.0/crunch/api/domain/check.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/competition.py` & `crunch-cli-3.4.0/crunch/api/domain/competition.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/crunch.py` & `crunch-cli-3.4.0/crunch/api/domain/crunch.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/data_release.py` & `crunch-cli-3.4.0/crunch/api/domain/data_release.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/library.py` & `crunch-cli-3.4.0/crunch/api/domain/library.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/metric.py` & `crunch-cli-3.4.0/crunch/api/domain/metric.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/phase.py` & `crunch-cli-3.4.0/crunch/api/domain/phase.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/prediction.py` & `crunch-cli-3.4.0/crunch/api/domain/prediction.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/project.py` & `crunch-cli-3.4.0/crunch/api/domain/project.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/quickstarter.py` & `crunch-cli-3.4.0/crunch/api/domain/quickstarter.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/round.py` & `crunch-cli-3.4.0/crunch/api/domain/round.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,28 +37,30 @@
         return PhaseCollection(
             round=self,
             client=self._client
         )
 
     def orthogonalize(
         self,
-        dataframe: pandas.DataFrame
+        dataframe: pandas.DataFrame,
+        timeout=60
     ):
         from .score import Score
 
         with tempfile.NamedTemporaryFile(suffix=".parquet") as tmp:
             dataframe.to_parquet(tmp, index=False)
             tmp.seek(0)
 
             result = self._client.api.orthogonalize(
                 self.competition.resource_identifier,
                 self.resource_identifier,
                 [
                     ("predictionFile", ('prediction.parquet', tmp, "application/x-tar"))
-                ]
+                ],
+                timeout=timeout
             )
 
         return Score.from_dict_array(result, None)
 
 
 class RoundCollection(Collection):
 
@@ -142,17 +144,19 @@
             json=True
         )
 
     def orthogonalize(
         self,
         competition_identifier,
         round_identifier,
-        files
+        files,
+        timeout=60
     ):
         return self._result(
             self.post(
                 f"/v1/competitions/{competition_identifier}/rounds/{round_identifier}/orthogonalize",
                 data={},  # push token will be added
-                files=tuple(files)
+                files=tuple(files),
+                timeout=timeout
             ),
             json=True
         )
```

### Comparing `crunch-cli-3.3.1/crunch/api/domain/run.py` & `crunch-cli-3.4.0/crunch/api/domain/run.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/runner.py` & `crunch-cli-3.4.0/crunch/api/domain/runner.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/score.py` & `crunch-cli-3.4.0/crunch/api/domain/score.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/submission.py` & `crunch-cli-3.4.0/crunch/api/domain/submission.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/domain/user.py` & `crunch-cli-3.4.0/crunch/api/domain/user.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/errors.py` & `crunch-cli-3.4.0/crunch/api/errors.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/identifiers.py` & `crunch-cli-3.4.0/crunch/api/identifiers.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/api/resource.py` & `crunch-cli-3.4.0/crunch/api/resource.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/checker/checker.py` & `crunch-cli-3.4.0/crunch/checker/checker.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/checker/functions.py` & `crunch-cli-3.4.0/crunch/checker/functions.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/cli.py` & `crunch-cli-3.4.0/crunch/cli.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/command/convert.py` & `crunch-cli-3.4.0/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/command/download.py` & `crunch-cli-3.4.0/crunch/command/download.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/command/push.py` & `crunch-cli-3.4.0/crunch/command/push.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/command/quickstarter.py` & `crunch-cli-3.4.0/crunch/command/quickstarter.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/command/setup.py` & `crunch-cli-3.4.0/crunch/command/setup.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/command/test.py` & `crunch-cli-3.4.0/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/constants.py` & `crunch-cli-3.4.0/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/ensure.py` & `crunch-cli-3.4.0/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/inline.py` & `crunch-cli-3.4.0/crunch/inline.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/library.py` & `crunch-cli-3.4.0/crunch/library.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/monkey_patches.py` & `crunch-cli-3.4.0/crunch/monkey_patches.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/orthogonalization/__init__.py` & `crunch-cli-3.4.0/crunch/orthogonalization/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,25 +31,26 @@
 ) -> typing.Optional[pandas.DataFrame]:
     ...
 
 
 def run(
     prediction: pandas.DataFrame,
     as_dataframe=True,
-    max_retry=3
+    max_retry=3,
+    timeout=60,
 ):
     if runner.is_inside:
         scores = run_from_runner(prediction)
     else:
         max_retry = max(1, max_retry)
         for retry in range(1, max_retry + 1):
             try:
-                scores = run_via_api(prediction)
+                scores = run_via_api(prediction, timeout)
                 break
-            except requests.ConnectionError:
+            except (requests.ConnectionError, requests.Timeout):
                 if retry == max_retry:
                     raise
 
     if not as_dataframe:
         return scores
 
     if not len(scores):
```

### Comparing `crunch-cli-3.3.1/crunch/orthogonalization/orthogonalize.py` & `crunch-cli-3.4.0/crunch/orthogonalization/orthogonalize.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 import pandas
 
 from .. import __version__, api, vendor
 
 
 def run_via_api(
     dataframe: pandas.DataFrame,
+    timeout: int,
 ) -> typing.List[api.Score]:
     _, project = api.Client.from_project()
 
     competition = project.competition
     round = competition.rounds.current
 
-    return round.orthogonalize(dataframe)
+    return round.orthogonalize(
+        dataframe,
+        timeout=timeout
+    )
 
 
 def run_from_runner(
     dataframe: pandas.DataFrame,
 ) -> typing.List[api.Score]:
     from ._runner import delegate
     return delegate(dataframe)
```

### Comparing `crunch-cli-3.3.1/crunch/runner/cloud.py` & `crunch-cli-3.4.0/crunch/runner/cloud.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/runner/cloud_executor.py` & `crunch-cli-3.4.0/crunch/runner/cloud_executor.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/runner/local.py` & `crunch-cli-3.4.0/crunch/runner/local.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/runner/runner.py` & `crunch-cli-3.4.0/crunch/runner/runner.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/scoring/_format/dag.py` & `crunch-cli-3.4.0/crunch/scoring/_format/dag.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/scoring/_format/timeseries.py` & `crunch-cli-3.4.0/crunch/scoring/_format/timeseries.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/scoring/score.py` & `crunch-cli-3.4.0/crunch/scoring/score.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/scoring/scorers.py` & `crunch-cli-3.4.0/crunch/scoring/scorers.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/store.py` & `crunch-cli-3.4.0/crunch/store.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/tester.py` & `crunch-cli-3.4.0/crunch/tester.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/utils.py` & `crunch-cli-3.4.0/crunch/utils.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/vendor/__init__.py` & `crunch-cli-3.4.0/crunch/vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch/vendor/datacrunch.py` & `crunch-cli-3.4.0/crunch/vendor/datacrunch.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/crunch_cli.egg-info/PKG-INFO` & `crunch-cli-3.4.0/crunch_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crunch-cli
-Version: 3.3.1
+Version: 3.4.0
 Summary: crunch-cli - CLI of the CrunchDAO Platform
 Home-page: https://github.com/crunchdao/crunch-cli
 Author: Enzo CACERES
 Author-email: enzo.caceres@crunchdao.com
 Keywords: package development template
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `crunch-cli-3.3.1/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-3.4.0/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch-cli-3.3.1/setup.py` & `crunch-cli-3.4.0/setup.py`

 * *Files identical despite different names*

