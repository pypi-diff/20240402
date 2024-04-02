# Comparing `tmp/apicurio_datahub_kafka-1.1.6.tar.gz` & `tmp/apicurio_datahub_kafka-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicurio_datahub_kafka-1.1.6.tar", last modified: Mon Apr  1 07:17:48 2024, max compression
+gzip compressed data, was "apicurio_datahub_kafka-2.0.1.tar", last modified: Tue Apr  2 02:35:53 2024, max compression
```

## Comparing `apicurio_datahub_kafka-1.1.6.tar` & `apicurio_datahub_kafka-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cg         (501) staff       (20)        0 2024-04-01 07:17:48.664227 apicurio_datahub_kafka-1.1.6/
--rw-r--r--   0 cg         (501) staff       (20)     1074 2024-03-22 07:49:18.000000 apicurio_datahub_kafka-1.1.6/LICENSE
--rw-r--r--   0 cg         (501) staff       (20)      147 2024-04-01 07:17:48.663592 apicurio_datahub_kafka-1.1.6/PKG-INFO
--rw-r--r--   0 cg         (501) staff       (20)      380 2024-03-27 08:53:34.000000 apicurio_datahub_kafka-1.1.6/README.md
--rw-r--r--   0 cg         (501) staff       (20)       38 2024-04-01 07:17:48.664481 apicurio_datahub_kafka-1.1.6/setup.cfg
--rw-r--r--   0 cg         (501) staff       (20)      305 2024-04-01 07:16:34.000000 apicurio_datahub_kafka-1.1.6/setup.py
-drwxr-xr-x   0 cg         (501) staff       (20)        0 2024-04-01 07:17:48.621858 apicurio_datahub_kafka-1.1.6/src/
-drwxr-xr-x   0 cg         (501) staff       (20)        0 2024-04-01 07:17:48.643147 apicurio_datahub_kafka-1.1.6/src/apicurio_datahub_kafka.egg-info/
--rw-r--r--   0 cg         (501) staff       (20)      147 2024-04-01 07:17:48.000000 apicurio_datahub_kafka-1.1.6/src/apicurio_datahub_kafka.egg-info/PKG-INFO
--rw-r--r--   0 cg         (501) staff       (20)      353 2024-04-01 07:17:48.000000 apicurio_datahub_kafka-1.1.6/src/apicurio_datahub_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 cg         (501) staff       (20)        1 2024-04-01 07:17:48.000000 apicurio_datahub_kafka-1.1.6/src/apicurio_datahub_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 cg         (501) staff       (20)       21 2024-04-01 07:17:48.000000 apicurio_datahub_kafka-1.1.6/src/apicurio_datahub_kafka.egg-info/requires.txt
--rw-r--r--   0 cg         (501) staff       (20)       15 2024-04-01 07:17:48.000000 apicurio_datahub_kafka-1.1.6/src/apicurio_datahub_kafka.egg-info/top_level.txt
-drwxr-xr-x   0 cg         (501) staff       (20)        0 2024-04-01 07:17:48.661620 apicurio_datahub_kafka-1.1.6/src/apicurio_kafka/
--rw-r--r--   0 cg         (501) staff       (20)        0 2024-03-22 07:49:18.000000 apicurio_datahub_kafka-1.1.6/src/apicurio_kafka/__init__.py
--rw-r--r--   0 cg         (501) staff       (20)    10050 2024-04-01 07:16:34.000000 apicurio_datahub_kafka-1.1.6/src/apicurio_kafka/apicurio_schema_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:35:53.325906 apicurio_datahub_kafka-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-02 02:35:48.000000 apicurio_datahub_kafka-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-02 02:35:53.325906 apicurio_datahub_kafka-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-02 02:35:48.000000 apicurio_datahub_kafka-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 02:35:53.325906 apicurio_datahub_kafka-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-02 02:35:48.000000 apicurio_datahub_kafka-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:35:53.325906 apicurio_datahub_kafka-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:35:53.325906 apicurio_datahub_kafka-2.0.1/src/apicurio_datahub_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-02 02:35:53.000000 apicurio_datahub_kafka-2.0.1/src/apicurio_datahub_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-02 02:35:53.000000 apicurio_datahub_kafka-2.0.1/src/apicurio_datahub_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:35:53.000000 apicurio_datahub_kafka-2.0.1/src/apicurio_datahub_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 02:35:53.000000 apicurio_datahub_kafka-2.0.1/src/apicurio_datahub_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 02:35:53.000000 apicurio_datahub_kafka-2.0.1/src/apicurio_datahub_kafka.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:35:53.325906 apicurio_datahub_kafka-2.0.1/src/apicurio_kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:35:48.000000 apicurio_datahub_kafka-2.0.1/src/apicurio_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-04-02 02:35:48.000000 apicurio_datahub_kafka-2.0.1/src/apicurio_kafka/apicurio_schema_registry.py
```

### Comparing `apicurio_datahub_kafka-1.1.6/LICENSE` & `apicurio_datahub_kafka-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apicurio_datahub_kafka-1.1.6/src/apicurio_kafka/apicurio_schema_registry.py` & `apicurio_datahub_kafka-2.0.1/src/apicurio_kafka/apicurio_schema_registry.py`

 * *Files identical despite different names*

