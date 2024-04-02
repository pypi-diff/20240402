# Comparing `tmp/idds-atlas-2.1.8.tar.gz` & `tmp/idds-atlas-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-atlas-2.1.8.tar", last modified: Wed Jan 31 16:35:24 2024, max compression
+gzip compressed data, was "idds-atlas-2.1.9.tar", last modified: Wed Jan 31 17:27:21 2024, max compression
```

## Comparing `idds-atlas-2.1.8.tar` & `idds-atlas-2.1.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.375240 idds-atlas-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-31 16:35:24.375240 idds-atlas-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.363240 idds-atlas-2.1.8/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.367240 idds-atlas-2.1.8/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.367240 idds-atlas-2.1.8/lib/idds/atlas/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.367240 idds-atlas-2.1.8/lib/idds/atlas/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/notifier/messaging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.367240 idds-atlas-2.1.8/lib/idds/atlas/processing/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/processing/activelearning_condor_poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/processing/activelearning_condor_submitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/processing/base_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/processing/condor_poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/processing/condor_submitter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2495 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/processing/hyperparameteropt_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (127)    16647 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/processing/hyperparameteropt_condor_poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/processing/hyperparameteropt_condor_submitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/processing/hyperparameteropt_nevergrad.py
--rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/processing/stagein_poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/processing/stagein_submitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.371240 idds-atlas-2.1.8/lib/idds/atlas/rucio/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/rucio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/rucio/base_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/rucio/collection_lister.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/rucio/collection_metadata_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/rucio/contents_lister.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/rucio/contents_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/rucio/rule_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/rucio/rule_poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/rucio/rule_submitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.371240 idds-atlas-2.1.8/lib/idds/atlas/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/transformer/activelearning_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/transformer/base_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/transformer/hyperparameteropt_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/transformer/stagein_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 16:35:22.000000 idds-atlas-2.1.8/lib/idds/atlas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.371240 idds-atlas-2.1.8/lib/idds/atlas/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20599 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflow/atlasactuatorwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflow/atlascondorwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    22890 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflow/atlasdagwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    35598 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflow/atlashpowork.py
--rw-r--r--   0 runner    (1001) docker     (127)    21759 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflow/atlaslocalpandawork.py
--rw-r--r--   0 runner    (1001) docker     (127)    37771 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflow/atlaspandawork.py
--rw-r--r--   0 runner    (1001) docker     (127)    21026 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflow/atlasstageinwork.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.375240 idds-atlas-2.1.8/lib/idds/atlas/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20605 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlasactuatorwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlascondorwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlasdagwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    35487 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlashpowork.py
--rw-r--r--   0 runner    (1001) docker     (127)    21763 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlaslocalpandawork.py
--rw-r--r--   0 runner    (1001) docker     (127)    38527 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlaspandawork.py
--rw-r--r--   0 runner    (1001) docker     (127)    21030 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlasstageinwork.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.375240 idds-atlas-2.1.8/lib/idds_atlas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-31 16:35:24.000000 idds-atlas-2.1.8/lib/idds_atlas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-01-31 16:35:24.000000 idds-atlas-2.1.8/lib/idds_atlas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 16:35:24.000000 idds-atlas-2.1.8/lib/idds_atlas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-31 16:35:24.000000 idds-atlas-2.1.8/lib/idds_atlas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 16:35:24.000000 idds-atlas-2.1.8/lib/idds_atlas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 16:35:24.375240 idds-atlas-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-01-31 16:35:12.000000 idds-atlas-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.363240 idds-atlas-2.1.8/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:24.375240 idds-atlas-2.1.8/tools/env/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-01-31 16:35:22.000000 idds-atlas-2.1.8/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.669882 idds-atlas-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-31 17:27:21.669882 idds-atlas-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.661882 idds-atlas-2.1.9/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.661882 idds-atlas-2.1.9/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.661882 idds-atlas-2.1.9/lib/idds/atlas/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.661882 idds-atlas-2.1.9/lib/idds/atlas/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/notifier/messaging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.665882 idds-atlas-2.1.9/lib/idds/atlas/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/processing/activelearning_condor_poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/processing/activelearning_condor_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/processing/base_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/processing/condor_poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/processing/condor_submitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2495 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/processing/hyperparameteropt_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16647 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/processing/hyperparameteropt_condor_poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/processing/hyperparameteropt_condor_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/processing/hyperparameteropt_nevergrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/processing/stagein_poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/processing/stagein_submitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.665882 idds-atlas-2.1.9/lib/idds/atlas/rucio/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/rucio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/rucio/base_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/rucio/collection_lister.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/rucio/collection_metadata_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/rucio/contents_lister.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/rucio/contents_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/rucio/rule_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/rucio/rule_poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/rucio/rule_submitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.665882 idds-atlas-2.1.9/lib/idds/atlas/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/transformer/activelearning_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/transformer/base_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/transformer/hyperparameteropt_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/transformer/stagein_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 17:27:19.000000 idds-atlas-2.1.9/lib/idds/atlas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.669882 idds-atlas-2.1.9/lib/idds/atlas/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20599 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflow/atlasactuatorwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflow/atlascondorwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22890 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflow/atlasdagwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35598 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflow/atlashpowork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21759 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflow/atlaslocalpandawork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37771 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflow/atlaspandawork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21026 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflow/atlasstageinwork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.669882 idds-atlas-2.1.9/lib/idds/atlas/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20605 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlasactuatorwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlascondorwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlasdagwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35487 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlashpowork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21763 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlaslocalpandawork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38527 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlaspandawork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21030 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlasstageinwork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.669882 idds-atlas-2.1.9/lib/idds_atlas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-31 17:27:21.000000 idds-atlas-2.1.9/lib/idds_atlas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-01-31 17:27:21.000000 idds-atlas-2.1.9/lib/idds_atlas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 17:27:21.000000 idds-atlas-2.1.9/lib/idds_atlas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-31 17:27:21.000000 idds-atlas-2.1.9/lib/idds_atlas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 17:27:21.000000 idds-atlas-2.1.9/lib/idds_atlas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 17:27:21.669882 idds-atlas-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-01-31 17:27:09.000000 idds-atlas-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.661882 idds-atlas-2.1.9/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:21.669882 idds-atlas-2.1.9/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-01-31 17:27:19.000000 idds-atlas-2.1.9/tools/env/environment.yml
```

### Comparing `idds-atlas-2.1.8/LICENSE.rst` & `idds-atlas-2.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/PKG-INFO` & `idds-atlas-2.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-atlas
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Requires-Dist: flake8
 Requires-Dist: pytest
 Requires-Dist: nose
 Requires-Dist: stomp.py
 Requires-Dist: panda-client-light
 Requires-Dist: rucio-clients
 Requires-Dist: rucio-clients-atlas
-Requires-Dist: idds-common==2.1.8
-Requires-Dist: idds-workflow==2.1.8
+Requires-Dist: idds-common==2.1.9
+Requires-Dist: idds-workflow==2.1.9
 
 idds-atlas
 ====
 
 idds-atlas subpackage is for CERN ATLAS specific functions and plugins.
 With it, iDDS can support CERN ATLAS workflows.
```

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/notifier/messaging.py` & `idds-atlas-2.1.9/lib/idds/atlas/notifier/messaging.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/processing/activelearning_condor_poller.py` & `idds-atlas-2.1.9/lib/idds/atlas/processing/activelearning_condor_poller.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/processing/activelearning_condor_submitter.py` & `idds-atlas-2.1.9/lib/idds/atlas/processing/activelearning_condor_submitter.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/processing/base_plugin.py` & `idds-atlas-2.1.9/lib/idds/atlas/processing/base_plugin.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/processing/condor_poller.py` & `idds-atlas-2.1.9/lib/idds/atlas/processing/condor_poller.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/processing/condor_submitter.py` & `idds-atlas-2.1.9/lib/idds/atlas/processing/condor_submitter.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/processing/hyperparameteropt_bayesian.py` & `idds-atlas-2.1.9/lib/idds/atlas/processing/hyperparameteropt_bayesian.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/processing/hyperparameteropt_condor_poller.py` & `idds-atlas-2.1.9/lib/idds/atlas/processing/hyperparameteropt_condor_poller.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/processing/hyperparameteropt_condor_submitter.py` & `idds-atlas-2.1.9/lib/idds/atlas/processing/hyperparameteropt_condor_submitter.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/processing/hyperparameteropt_nevergrad.py` & `idds-atlas-2.1.9/lib/idds/atlas/processing/hyperparameteropt_nevergrad.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/processing/stagein_poller.py` & `idds-atlas-2.1.9/lib/idds/atlas/processing/stagein_poller.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/processing/stagein_submitter.py` & `idds-atlas-2.1.9/lib/idds/atlas/processing/stagein_submitter.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/rucio/base_plugin.py` & `idds-atlas-2.1.9/lib/idds/atlas/rucio/base_plugin.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/rucio/collection_lister.py` & `idds-atlas-2.1.9/lib/idds/atlas/rucio/collection_lister.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/rucio/collection_metadata_reader.py` & `idds-atlas-2.1.9/lib/idds/atlas/rucio/collection_metadata_reader.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/rucio/contents_lister.py` & `idds-atlas-2.1.9/lib/idds/atlas/rucio/contents_lister.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/rucio/contents_register.py` & `idds-atlas-2.1.9/lib/idds/atlas/rucio/contents_register.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/rucio/rule_creator.py` & `idds-atlas-2.1.9/lib/idds/atlas/rucio/rule_creator.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/rucio/rule_poller.py` & `idds-atlas-2.1.9/lib/idds/atlas/rucio/rule_poller.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/rucio/rule_submitter.py` & `idds-atlas-2.1.9/lib/idds/atlas/rucio/rule_submitter.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/transformer/activelearning_transformer.py` & `idds-atlas-2.1.9/lib/idds/atlas/transformer/activelearning_transformer.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/transformer/base_plugin.py` & `idds-atlas-2.1.9/lib/idds/atlas/transformer/base_plugin.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/transformer/hyperparameteropt_transformer.py` & `idds-atlas-2.1.9/lib/idds/atlas/transformer/hyperparameteropt_transformer.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/transformer/stagein_transformer.py` & `idds-atlas-2.1.9/lib/idds/atlas/transformer/stagein_transformer.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflow/atlasactuatorwork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflow/atlasactuatorwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflow/atlascondorwork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflow/atlascondorwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflow/atlasdagwork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflow/atlasdagwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflow/atlashpowork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflow/atlashpowork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflow/atlaslocalpandawork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflow/atlaslocalpandawork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflow/atlaspandawork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflow/atlaspandawork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflow/atlasstageinwork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflow/atlasstageinwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlasactuatorwork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlasactuatorwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlascondorwork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlascondorwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlasdagwork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlasdagwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlashpowork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlashpowork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlaslocalpandawork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlaslocalpandawork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlaspandawork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlaspandawork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds/atlas/workflowv2/atlasstageinwork.py` & `idds-atlas-2.1.9/lib/idds/atlas/workflowv2/atlasstageinwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/lib/idds_atlas.egg-info/PKG-INFO` & `idds-atlas-2.1.9/lib/idds_atlas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-atlas
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Requires-Dist: flake8
 Requires-Dist: pytest
 Requires-Dist: nose
 Requires-Dist: stomp.py
 Requires-Dist: panda-client-light
 Requires-Dist: rucio-clients
 Requires-Dist: rucio-clients-atlas
-Requires-Dist: idds-common==2.1.8
-Requires-Dist: idds-workflow==2.1.8
+Requires-Dist: idds-common==2.1.9
+Requires-Dist: idds-workflow==2.1.9
 
 idds-atlas
 ====
 
 idds-atlas subpackage is for CERN ATLAS specific functions and plugins.
 With it, iDDS can support CERN ATLAS workflows.
```

### Comparing `idds-atlas-2.1.8/lib/idds_atlas.egg-info/SOURCES.txt` & `idds-atlas-2.1.9/lib/idds_atlas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-atlas-2.1.8/setup.py` & `idds-atlas-2.1.9/setup.py`

 * *Files identical despite different names*

