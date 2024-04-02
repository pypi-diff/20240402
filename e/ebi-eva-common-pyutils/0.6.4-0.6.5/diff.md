# Comparing `tmp/ebi_eva_common_pyutils-0.6.4.tar.gz` & `tmp/ebi_eva_common_pyutils-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebi_eva_common_pyutils-0.6.4.tar", last modified: Thu Mar 21 11:32:14 2024, max compression
+gzip compressed data, was "ebi_eva_common_pyutils-0.6.5.tar", last modified: Tue Apr  2 10:55:50 2024, max compression
```

## Comparing `ebi_eva_common_pyutils-0.6.4.tar` & `ebi_eva_common_pyutils-0.6.5.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:14.617351 ebi_eva_common_pyutils-0.6.4/
--rw-r--r--   0 tcezard    (502) staff       (20)     2779 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/CHANGELOG.md
--rw-r--r--   0 tcezard    (502) staff       (20)    11357 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/LICENSE
--rw-r--r--   0 tcezard    (502) staff       (20)       28 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/MANIFEST.in
--rw-r--r--   0 tcezard    (502) staff       (20)      541 2024-03-21 11:32:14.617504 ebi_eva_common_pyutils-0.6.4/PKG-INFO
--rw-r--r--   0 tcezard    (502) staff       (20)     1434 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/README.md
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:14.606483 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/__init__.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:14.609526 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/assembly/
--rw-r--r--   0 tcezard    (502) staff       (20)       67 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/assembly/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     3142 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/assembly/assembly.py
--rw-r--r--   0 tcezard    (502) staff       (20)     4018 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/assembly_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     2340 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/command_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     1192 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/common_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     4828 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/config.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:14.610177 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/contig_alias/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/contig_alias/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     3056 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/contig_alias/contig_alias.py
--rw-r--r--   0 tcezard    (502) staff       (20)     1465 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/ena_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     1375 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/file_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     5093 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/logger.py
--rw-r--r--   0 tcezard    (502) staff       (20)     4859 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/ncbi_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     2285 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/network_utils.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:14.611454 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/reference/
--rw-r--r--   0 tcezard    (502) staff       (20)      134 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/reference/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)    12162 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/reference/assembly.py
--rw-r--r--   0 tcezard    (502) staff       (20)     3911 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/reference/sequence.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:14.612131 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/taxonomy/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/taxonomy/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     2259 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/taxonomy/taxonomy.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:14.612767 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/variation/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/variation/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     5230 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/variation/contig_utils.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:14.608798 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils.egg-info/
--rw-r--r--   0 tcezard    (502) staff       (20)      541 2024-03-21 11:32:14.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 tcezard    (502) staff       (20)     1653 2024-03-21 11:32:14.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 tcezard    (502) staff       (20)        1 2024-03-21 11:32:14.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 tcezard    (502) staff       (20)       97 2024-03-21 11:32:14.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils.egg-info/requires.txt
--rw-r--r--   0 tcezard    (502) staff       (20)       48 2024-03-21 11:32:14.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils.egg-info/top_level.txt
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:14.615520 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     4989 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/archive_directory.py
--rw-r--r--   0 tcezard    (502) staff       (20)     7909 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/config_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)    15090 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/metadata_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     3575 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/mongo_utils.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:14.616311 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/mongodb/
--rw-r--r--   0 tcezard    (502) staff       (20)       76 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/mongodb/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     9596 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/mongodb/mongo_database.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-03-21 11:32:14.617029 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/nextflow/
--rw-r--r--   0 tcezard    (502) staff       (20)      122 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/nextflow/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)    10114 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py
--rw-r--r--   0 tcezard    (502) staff       (20)     4398 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/pg_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)    15265 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/spring_properties.py
--rw-r--r--   0 tcezard    (502) staff       (20)      225 2024-03-21 11:32:14.618047 ebi_eva_common_pyutils-0.6.4/setup.cfg
--rw-r--r--   0 tcezard    (502) staff       (20)      926 2024-03-21 11:32:13.000000 ebi_eva_common_pyutils-0.6.4/setup.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/
+-rw-rw-r--   0 april     (1000) april     (1000)     2909 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/CHANGELOG.md
+-rw-rw-r--   0 april     (1000) april     (1000)    11357 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/LICENSE
+-rw-rw-r--   0 april     (1000) april     (1000)       28 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/MANIFEST.in
+-rw-r--r--   0 april     (1000) april     (1000)      817 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/PKG-INFO
+-rw-rw-r--   0 april     (1000) april     (1000)     1434 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/README.md
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.216831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/
+-rw-rw-r--   0 april     (1000) april     (1000)        0 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/__init__.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/assembly/
+-rw-rw-r--   0 april     (1000) april     (1000)       67 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/assembly/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)     3142 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/assembly/assembly.py
+-rw-rw-r--   0 april     (1000) april     (1000)     4018 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/assembly_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     2340 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/command_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     1192 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/common_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     4828 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/config.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/contig_alias/
+-rw-rw-r--   0 april     (1000) april     (1000)        0 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/contig_alias/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)     3056 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/contig_alias/contig_alias.py
+-rw-rw-r--   0 april     (1000) april     (1000)     1465 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/ena_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     1375 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/file_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     5093 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/logger.py
+-rw-rw-r--   0 april     (1000) april     (1000)     4859 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/ncbi_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     2648 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/network_utils.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/reference/
+-rw-rw-r--   0 april     (1000) april     (1000)      134 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/reference/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)    12162 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/reference/assembly.py
+-rw-rw-r--   0 april     (1000) april     (1000)     3911 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/reference/sequence.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/taxonomy/
+-rw-rw-r--   0 april     (1000) april     (1000)        0 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/taxonomy/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)     2259 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/taxonomy/taxonomy.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/variation/
+-rw-rw-r--   0 april     (1000) april     (1000)        0 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/variation/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)     5230 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/variation/contig_utils.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/
+-rw-r--r--   0 april     (1000) april     (1000)      817 2024-04-02 10:55:50.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/PKG-INFO
+-rw-rw-r--   0 april     (1000) april     (1000)     1773 2024-04-02 10:55:50.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 april     (1000) april     (1000)        1 2024-04-02 10:55:50.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 april     (1000) april     (1000)       97 2024-04-02 10:55:50.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/requires.txt
+-rw-rw-r--   0 april     (1000) april     (1000)       48 2024-04-02 10:55:50.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/top_level.txt
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/
+-rw-rw-r--   0 april     (1000) april     (1000)        0 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)     4989 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/archive_directory.py
+-rw-rw-r--   0 april     (1000) april     (1000)     7909 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/config_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)    15090 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/metadata_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     3575 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/mongo_utils.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/mongodb/
+-rw-rw-r--   0 april     (1000) april     (1000)       76 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/mongodb/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)     9596 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/mongodb/mongo_database.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/nextflow/
+-rw-rw-r--   0 april     (1000) april     (1000)      122 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/nextflow/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)    10114 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py
+-rw-rw-r--   0 april     (1000) april     (1000)     4398 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/pg_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)    15265 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/spring_properties.py
+-rw-rw-r--   0 april     (1000) april     (1000)      225 2024-04-02 10:55:50.224830 ebi_eva_common_pyutils-0.6.5/setup.cfg
+-rw-rw-r--   0 april     (1000) april     (1000)      926 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/setup.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2024-04-02 10:55:50.220831 ebi_eva_common_pyutils-0.6.5/tests/
+-rw-rw-r--   0 april     (1000) april     (1000)      724 2024-04-02 10:55:49.000000 ebi_eva_common_pyutils-0.6.5/tests/test_common.py
```

### Comparing `ebi_eva_common_pyutils-0.6.4/CHANGELOG.md` & `ebi_eva_common_pyutils-0.6.5/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 
 Changelog for ebi_eva_common_pyutils
 ===========================
 
+## 0.6.5 (2024-04-02)
+---------------------
+
+- Ensure that the port forwarding command is running before returning the process.
+
+
 ## 0.6.4 (2024-03-21)
 ---------------------
 
 - Update Mongodb client to use mongosh instead of the legacy mongo.
 
 ## 0.6.3 (2024-02-22)
 ---------------------
```

### Comparing `ebi_eva_common_pyutils-0.6.4/LICENSE` & `ebi_eva_common_pyutils-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/README.md` & `ebi_eva_common_pyutils-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/assembly/assembly.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/assembly/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/assembly_utils.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/assembly_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/command_utils.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/common_utils.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/common_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/config.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/config.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/contig_alias/contig_alias.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/contig_alias/contig_alias.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/ena_utils.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/ena_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/file_utils.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/logger.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/logger.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/ncbi_utils.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/ncbi_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/network_utils.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/network_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import time
 
 import requests
 import subprocess
 from retry import retry
 
 from ebi_eva_common_pyutils.logger import logging_config as log_cfg
 
@@ -39,14 +39,21 @@
     logger.error("Could not forward to any local port!")
 
 
 def forward_remote_port_to_local_port(remote_host: str, remote_port: int, local_port: int) -> int:
     port_forward_command = 'ssh -N -L{0}:localhost:{1} {2}'.format(local_port, remote_port, remote_host)
     logger.info("Forwarding port to local port using command: " + port_forward_command)
     proc = subprocess.Popen(port_forward_command.split(" "))
+    time.sleep(5)
+    # Ensure that the process is still running
+    poll = proc.poll()
+    if poll is not None:
+        # The process already completed which mean it most likely crashed
+        logger.error(f'Port Forwarding {remote_host}:{remote_port} -> {local_port} failed!')
+        raise subprocess.CalledProcessError(proc.returncode, proc.args)
     return proc.pid
 
 
 @retry(exceptions=(ConnectionError, requests.RequestException), logger=logger,
        tries=4, delay=2, backoff=1.2, jitter=(1, 3))
 def json_request(url: str, payload: dict = None, method=requests.get) -> dict:
     """Makes a request of a specified type (by default GET) with the specified URL and payload, attempts to parse the
```

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/reference/assembly.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/reference/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/reference/sequence.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/reference/sequence.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/taxonomy/taxonomy.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/taxonomy/taxonomy.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils/variation/contig_utils.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils/variation/contig_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_common_pyutils.egg-info/SOURCES.txt` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_common_pyutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+/tmp/ebi_eva_common_pyutils-v0.6.5-999yjogj/gitclone/ebi_eva_internal_pyutils/archive_directory.py
 ebi_eva_common_pyutils/__init__.py
 ebi_eva_common_pyutils/assembly_utils.py
 ebi_eva_common_pyutils/command_utils.py
 ebi_eva_common_pyutils/common_utils.py
 ebi_eva_common_pyutils/config.py
 ebi_eva_common_pyutils/ena_utils.py
 ebi_eva_common_pyutils/file_utils.py
@@ -36,8 +37,9 @@
 ebi_eva_internal_pyutils/metadata_utils.py
 ebi_eva_internal_pyutils/mongo_utils.py
 ebi_eva_internal_pyutils/pg_utils.py
 ebi_eva_internal_pyutils/spring_properties.py
 ebi_eva_internal_pyutils/mongodb/__init__.py
 ebi_eva_internal_pyutils/mongodb/mongo_database.py
 ebi_eva_internal_pyutils/nextflow/__init__.py
-ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py
+ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py
+tests/test_common.py
```

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/archive_directory.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/archive_directory.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/config_utils.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/metadata_utils.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/mongo_utils.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/mongo_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/mongodb/mongo_database.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/mongodb/mongo_database.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/pg_utils.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/pg_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/ebi_eva_internal_pyutils/spring_properties.py` & `ebi_eva_common_pyutils-0.6.5/ebi_eva_internal_pyutils/spring_properties.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.4/setup.py` & `ebi_eva_common_pyutils-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages
 
 setup(
     name='ebi_eva_common_pyutils',
     scripts=[os.path.join(os.path.dirname(__file__), 'ebi_eva_internal_pyutils', 'archive_directory.py')],
     packages=find_packages(),
-    version='0.6.4',
+    version='0.6.5',
     license='Apache',
     description='EBI EVA - Common Python Utilities',
     url='https://github.com/EBIVariation/eva-common-pyutils',
     keywords=['EBI', 'EVA', 'PYTHON', 'UTILITIES'],
     install_requires=['requests', 'lxml', 'pyyaml', 'cached-property', 'retry'],
     extras_require={'eva-internal': ['psycopg2-binary', 'pymongo', 'networkx<=2.5']},
     classifiers=[
```

