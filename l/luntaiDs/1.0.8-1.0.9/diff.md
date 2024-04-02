# Comparing `tmp/luntaiDs-1.0.8.tar.gz` & `tmp/luntaiDs-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luntaiDs-1.0.8.tar", last modified: Fri Jan 19 03:19:28 2024, max compression
+gzip compressed data, was "luntaiDs-1.0.9.tar", last modified: Tue Jan 30 04:07:58 2024, max compression
```

## Comparing `luntaiDs-1.0.8.tar` & `luntaiDs-1.0.9.tar`

### file list

```diff
@@ -1,75 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.291789 luntaiDs-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-01-19 03:19:28.291789 luntaiDs-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.279789 luntaiDs-1.0.8/SimpleDs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.283789 luntaiDs-1.0.8/SimpleDs/CommonTools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.283789 luntaiDs-1.0.8/SimpleDs/CommonTools/SnapStructure/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/SnapStructure/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5245 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/SnapStructure/dependency.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18055 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/SnapStructure/structure.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2515 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/SnapStructure/tools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/accessor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6686 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/data_structure.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17614 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/dbapi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11342 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/dtyper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1014 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/login.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8399 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/remote.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      964 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15108 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/sparker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14748 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/CommonTools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.283789 luntaiDs-1.0.8/SimpleDs/ModelingTools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.283789 luntaiDs-1.0.8/SimpleDs/ModelingTools/CustomModel/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/CustomModel/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10289 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/CustomModel/calibration.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5822 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/CustomModel/custom.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5234 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/CustomModel/linear.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8736 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/CustomModel/ordinal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.283789 luntaiDs-1.0.8/SimpleDs/ModelingTools/Evaluation/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/Evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/Evaluation/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17947 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/Evaluation/plots.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25750 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/Evaluation/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.283789 luntaiDs-1.0.8/SimpleDs/ModelingTools/Explore/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/Explore/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30371 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/Explore/plots.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11101 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/Explore/preview.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31509 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/Explore/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.287789 luntaiDs-1.0.8/SimpleDs/ModelingTools/FeatureEngineer/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/FeatureEngineer/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1952 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/FeatureEngineer/featureHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/FeatureEngineer/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/FeatureEngineer/preprocessing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   113107 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/FeatureEngineer/transformers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11028 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/ModelServing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.287789 luntaiDs-1.0.8/SimpleDs/ModelingTools/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2521 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/utils/analytical_dtype.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      415 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/utils/checks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/utils/parallel.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1372 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ModelingTools/utils/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.287789 luntaiDs-1.0.8/SimpleDs/ProviderTools/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ProviderTools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.287789 luntaiDs-1.0.8/SimpleDs/ProviderTools/aws/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ProviderTools/aws/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17405 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ProviderTools/aws/s3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9122 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ProviderTools/aws/snap_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.287789 luntaiDs-1.0.8/SimpleDs/ProviderTools/clickhouse/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ProviderTools/clickhouse/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10770 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ProviderTools/clickhouse/dbapi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2448 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ProviderTools/clickhouse/dtyper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10431 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ProviderTools/clickhouse/snap_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.287789 luntaiDs-1.0.8/SimpleDs/ProviderTools/teradata/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ProviderTools/teradata/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2379 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/SimpleDs/ProviderTools/teradata/dbapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:19:28.291789 luntaiDs-1.0.8/SimpleDs/luntaiDs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-01-19 03:19:28.000000 luntaiDs-1.0.8/SimpleDs/luntaiDs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-01-19 03:19:28.000000 luntaiDs-1.0.8/SimpleDs/luntaiDs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 03:19:28.000000 luntaiDs-1.0.8/SimpleDs/luntaiDs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-19 03:19:28.000000 luntaiDs-1.0.8/SimpleDs/luntaiDs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-19 03:19:28.000000 luntaiDs-1.0.8/SimpleDs/luntaiDs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-01-19 03:19:12.000000 luntaiDs-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-19 03:19:28.291789 luntaiDs-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.754569 luntaiDs-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-01-30 04:07:58.754569 luntaiDs-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.746569 luntaiDs-1.0.9/SimpleDs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.746569 luntaiDs-1.0.9/SimpleDs/CommonTools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.746569 luntaiDs-1.0.9/SimpleDs/CommonTools/SnapStructure/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/SnapStructure/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5245 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/SnapStructure/dependency.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26210 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/SnapStructure/structure.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2515 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/SnapStructure/tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/accessor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6686 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/data_structure.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17614 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/dbapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11342 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/dtyper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1014 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/obj_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      964 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15108 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/sparker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14748 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/CommonTools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.746569 luntaiDs-1.0.9/SimpleDs/ModelingTools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.750569 luntaiDs-1.0.9/SimpleDs/ModelingTools/CustomModel/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/CustomModel/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10289 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/CustomModel/calibration.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5822 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/CustomModel/custom.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5234 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/CustomModel/linear.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8736 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/CustomModel/ordinal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.750569 luntaiDs-1.0.9/SimpleDs/ModelingTools/Evaluation/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/Evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/Evaluation/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17947 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/Evaluation/plots.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25750 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/Evaluation/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.750569 luntaiDs-1.0.9/SimpleDs/ModelingTools/Explore/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/Explore/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30371 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/Explore/plots.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11101 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/Explore/preview.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31509 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/Explore/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.750569 luntaiDs-1.0.9/SimpleDs/ModelingTools/FeatureEngineer/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/FeatureEngineer/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1952 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/FeatureEngineer/featureHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/FeatureEngineer/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/FeatureEngineer/preprocessing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   113107 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/FeatureEngineer/transformers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11028 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/ModelServing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.750569 luntaiDs-1.0.9/SimpleDs/ModelingTools/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2521 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/utils/analytical_dtype.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      415 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/utils/checks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/utils/parallel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1372 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ModelingTools/utils/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.750569 luntaiDs-1.0.9/SimpleDs/ProviderTools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.750569 luntaiDs-1.0.9/SimpleDs/ProviderTools/aws/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/aws/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17699 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/aws/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.754569 luntaiDs-1.0.9/SimpleDs/ProviderTools/clickhouse/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/clickhouse/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10770 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/clickhouse/dbapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2448 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/clickhouse/dtyper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10607 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/clickhouse/snap_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.754569 luntaiDs-1.0.9/SimpleDs/ProviderTools/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17625 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/gcp/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.754569 luntaiDs-1.0.9/SimpleDs/ProviderTools/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/ssh/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/ssh/snap_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.754569 luntaiDs-1.0.9/SimpleDs/ProviderTools/teradata/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/teradata/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2379 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/SimpleDs/ProviderTools/teradata/dbapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:07:58.754569 luntaiDs-1.0.9/SimpleDs/luntaiDs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-01-30 04:07:58.000000 luntaiDs-1.0.9/SimpleDs/luntaiDs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-01-30 04:07:58.000000 luntaiDs-1.0.9/SimpleDs/luntaiDs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 04:07:58.000000 luntaiDs-1.0.9/SimpleDs/luntaiDs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-30 04:07:58.000000 luntaiDs-1.0.9/SimpleDs/luntaiDs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-30 04:07:58.000000 luntaiDs-1.0.9/SimpleDs/luntaiDs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-01-30 04:07:34.000000 luntaiDs-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-30 04:07:58.754569 luntaiDs-1.0.9/setup.cfg
```

### Comparing `luntaiDs-1.0.8/LICENSE` & `luntaiDs-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/PKG-INFO` & `luntaiDs-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luntaiDs
-Version: 1.0.8
+Version: 1.0.9
 Summary: Make Data Scientist life Easier Tool
 Home-page: https://github.com/luntaixiax/luntai-ds
 Author: Ailun Qian (luntaixia)
 Author-email: ailunqian124@gmail.com
 License: MIT License
         
         Copyright (c) 2023 luntaixiax
```

### Comparing `luntaiDs-1.0.8/SimpleDs/CommonTools/SnapStructure/dependency.py` & `luntaiDs-1.0.9/SimpleDs/CommonTools/SnapStructure/dependency.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/CommonTools/SnapStructure/structure.py` & `luntaiDs-1.0.9/SimpleDs/CommonTools/SnapStructure/structure.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import pyspark
 from tqdm.auto import tqdm
 
 from CommonTools.SnapStructure.tools import get_file_list_pattern, match_date_from_str
 from CommonTools.dbapi import baseDbInf, dbIO
 from CommonTools.sparker import SparkConnector
 from CommonTools.utils import str2dt
+from CommonTools.obj_storage import ObjStorage
 
     
 class SnapshotDataManagerBase:
     @classmethod
     def setup(cls, spark_connector: SparkConnector = None, default_engine:str = 'pandas'):
         if spark_connector:
             cls.sc = spark_connector
@@ -240,15 +241,15 @@
         :param dst_table: destination table
         :return:
         """
         new = self.duplicate(dst_schema, dst_table)
         self.drop()
         return new
 
-    def duplicate(self, dst_schema: str, dst_table: str):
+    def duplicate(self, dst_schema: str, dst_table: str) -> SnapshotDataManagerBase:
         """duplicate the existing schema.table to new one, the existing one will be kept
 
         :param dst_schema: destination schema
         :param dst_table: destination table
         :return:
         """
         raise NotImplementedError("")
@@ -280,16 +281,16 @@
         )
         cls.ROOT_DIR = root_dir
         cls.default_engine = default_engine
         
     def __init__(self, schema:str, table:str):
         """virtual database management interface
 
-        :param schema: the virtual schema , e.g., RAW, PROCESSED
-        :param table:  the virtual table under each schema, e.g., CLNT_GENERAL, BDA_GENERAL
+        :param schema: the virtual schema
+        :param table:  the virtual table under each schema
         """
         super().__init__(schema = schema, table = table)
         dir = os.path.join(self.ROOT_DIR, schema, table)
         self.dir = dir  # the root path of the table under each schema
         self.init_table()
 
     def init_table(self):
@@ -424,26 +425,15 @@
     def drop(self):
         """drop the whole table
 
         :return:
         """
         shutil.rmtree(self.dir)
 
-    def migrate(self, dst_schema: str, dst_table: str):
-        """move from the existing schema.table to new one, the existing one will be deleted
-
-        :param dst_schema: destination schema
-        :param dst_table: destination table
-        :return:
-        """
-        new = self.duplicate(dst_schema, dst_table)
-        self.drop()
-        return new
-
-    def duplicate(self, dst_schema: str, dst_table: str):
+    def duplicate(self, dst_schema: str, dst_table: str) -> SnapshotDataManagerLocalFS:
         new = SnapshotDataManagerLocalFS(schema = dst_schema, table = dst_table)
         copy_tree(self.dir, new.dir)
         return new
 
     def disk_space(self, snap_dt, unit='MB') -> float:
         """get the size of the snap date file (pandas) or folder (pyspark partitions)
 
@@ -466,8 +456,204 @@
         """
         f = self.get_default_file_path(snap_dt)
         if os.path.isdir(f):
             # if it is a folder (partition files), it should has a .__SUCCESS.crc file generated by pyspark
             return "._SUCCESS.crc" in os.listdir(f)
         else:
             # if a single file, the size must be exceed the valid threshold
-            return self.disk_space(snap_dt, unit = 'MB') > size_threshold
+            return self.disk_space(snap_dt, unit = 'MB') > size_threshold
+        
+        
+class SnapshotDataManagerObjStorage(SnapshotDataManagerBase):
+    """files are saved as object storage under each schema.table
+    """
+
+    @classmethod
+    def setup(cls, bucket: str,  root_dir: str, obja: ObjStorage, spark_connector: SparkConnector = None, default_engine:str = 'pandas'):
+        super(SnapshotDataManagerObjStorage, cls).setup(
+            spark_connector = spark_connector,
+            default_engine = default_engine
+        )
+        cls.bucket = bucket
+        cls.ROOT_DIR = root_dir if not root_dir.startswith("/") else root_dir[1:]
+        cls.obja = obja
+        cls.obja.enter_bucket(bucket_name=bucket)
+    
+    def __init__(self, schema:str, table:str):
+        """virtual database management interface
+
+        :param schema: the virtual schema
+        :param table:  the virtual table under each schema
+        """
+        super().__init__(schema = schema, table = table)
+        dir = os.path.join(self.ROOT_DIR, schema, table)
+        self.dir = dir  # the root path of the table under each schema
+
+    def get_filename(self, snap_dt: date) -> str:
+        return f"{self.table}_{snap_dt}.parquet"
+
+    def get_default_file_path(self, snap_dt: date) -> str:
+        return os.path.join(self.dir, self.get_filename(snap_dt))
+    
+    def get_file_path_with_obj_storage_prefix(self, snap_dt: date) -> str:
+        return f"{self.get_uri_protocol}://{self.bucket}/{self.get_default_file_path(snap_dt=snap_dt)}"
+
+    def _save(self, df: pd.DataFrame, snap_dt: date, **kws):
+        """The pure logic to save pandas dataframe to the system, without handling existing record problem
+
+        :param pd.DataFrame df: _description_
+        :param date snap_dt: _description_
+        :raises NotImplementedError: _description_
+        """
+        self.obja.save_parquet(
+            df = df,
+            remote_path = self.get_default_file_path(snap_dt=snap_dt),
+            **kws
+        )
+    
+    def get_existing_snap_dts(self) -> List[date]:
+        df = self.obja.list_objs(remote_path = self.dir)
+        if df is None:
+            return []
+        existing_snaps = list(set(map(
+            str2dt,
+            (
+                df
+                .loc[
+                    (df['Key'].str.startswith(pat = f"{self.dir}/"))
+                    & (df['Key'].str.endswith(pat = ".parquet")), 
+                    'Key']
+                .str.replace(self.dir, "")
+                .apply(match_date_from_str)
+                .tolist()
+            )
+        )))
+        existing_snaps.sort()
+        return existing_snaps
+    
+    def read(self, snap_dt: date, **kws) -> pd.DataFrame:
+        """Read as pandas dataframe (one snapshot date) data
+
+        :param snap_dt: snap_dt to load
+        :return:
+        """
+        filepath = self.get_default_file_path(snap_dt=snap_dt)
+        return self.obja.read_parquet(remote_path = filepath, **kws)
+    
+
+    def reads(self, snap_dts: List[date], partition_key: str = None, **kws) -> pd.DataFrame:
+        """reads as pandas dataframe (vertically concat of several given snap dates data)
+
+        :param snap_dts: list of snap dates to read
+        :param partition_key: when vertically combining, need partition key to tell apart, typically its something like SNAP_DT
+                if not specified, will bypass checking step
+        :return:
+        """
+        # do the checks to ensure successful concatenation
+        li =  []
+        columns = pd.Index([])
+        for snap_dt in tqdm(snap_dts):
+            df_partition = self.read(snap_dt=snap_dt, **kws)
+            if partition_key is not None and partition_key not in df_partition.columns:
+                raise ValueError(f"{self.schema}.{self.table}: Partition Key {partition_key} not found in {snap_dt}")
+            if len(columns) > 0 and len(columns.union(df_partition.columns)) != len(columns):
+                # if new column set has a different length than the previous one, means the columns are not same across all the table partitions
+                raise ValueError(f"{self.schema}.{self.table}: Columns not consistent for snapshot {snap_dt}")
+            li.append(df_partition)
+
+        return pd.concat(li, axis = 0, ignore_index = True)
+    
+    def load(self, snap_dt: date, **kws) -> pyspark.sql.DataFrame:
+        """Read as spark dataframe (one snapshot date) data, and can also access from sc temporary view
+
+        :param snap_dt: snap_dt to load
+        :return:
+        """
+        filepath = self.get_file_path_with_obj_storage_prefix(snap_dt)
+        if hasattr(self, "sc"):
+            df = self.sc.read_parquet(filepath, **kws)
+            df.createOrReplaceTempView(f"{self.table}")
+            return df
+        else:
+            ValueError("No Spark Connector Specified, please call .setup() to bind a spark connector")
+    
+    def loads(self, snap_dts: List[date], partition_key: str = None, **kws) -> pyspark.sql.DataFrame:
+        """reads as pyspark dataframe (vertically concat of several given snap dates data)
+
+        :param snap_dts: list of snap dates to read
+        :param partition_key: when vertically combining, need partition key to tell apart, typically its something like SNAP_DT
+                if not specified, will bypass checking step
+        :return:
+        """
+        file_paths = [self.get_file_path_with_obj_storage_prefix(snap_dt) for snap_dt in snap_dts]
+        if hasattr(self, "sc"):
+            df = self.sc.read_parquet(*file_paths, **kws) # spark will automatically stack all tables together
+            # do the partition check
+            if partition_key is not None and partition_key not in df.columns:
+                raise ValueError(f"{self.schema}.{self.table}: Partition Key {partition_key} not found")
+
+            # pick up random snapshot data to check the columns are consistent
+            one_columns = self.load_random_snap().columns
+            if len(one_columns) != len(pd.Index(one_columns).union(df.columns)):
+                raise ValueError(f"{self.schema}.{self.table}: Columns not consistent in one of the snapshot data")
+
+            df.createOrReplaceTempView(f"{self.table}")
+            return df
+        else:
+            ValueError("No Spark Connector Specified, please call .setup() to bind a spark connector")
+    
+    def delete(self, snap_dt: date):
+        """Delete a snap shot dataframe, could be partitions
+
+        :param snap_dt: which snap date to delete
+        :return:
+        """
+        filepath = self.get_default_file_path(snap_dt=snap_dt)
+        if self.obja.list_objs(filepath) is None or len(self.s3a.list_objs(filepath)) == 1:
+            # it is not folder
+            self.obja.delete_obj(remote_path = filepath)
+        else:
+            # it is a folder, i.e., partitions
+            self.obja.delete_folder(remote_folder_path = filepath)
+
+    def drop(self):
+        """drop the whole table
+
+        :return:
+        """
+        self.obja.delete_folder(remote_folder_path = self.dir)
+
+    def duplicate(self, dst_schema: str, dst_table: str) -> SnapshotDataManagerObjStorage:
+        """duplicate the existing schema.table to new one, the existing one will be kept
+
+        :param dst_schema: destination schema
+        :param dst_table: destination table
+        :return:
+        """
+        new = SnapshotDataManagerObjStorage(schema = dst_schema, table = dst_table)
+        for snap_dt in tqdm(self.get_existing_snap_dts()):
+            from_filename = self.get_default_file_path(snap_dt=snap_dt)
+            to_filename = new.get_default_file_path(snap_dt=snap_dt)
+            self.obja.copy_obj(
+                from_path = from_filename,
+                to_path = to_filename
+            )
+        return new
+        
+    def disk_space(self, snap_dt, unit='MB') -> float:
+        """get the size of the snap date on disk
+
+        :param snap_dt:
+        :param unit: {KB, MB, GB}
+        """
+        #key = self.obja.get_obj(remote_path=self.get_default_file_path(snap_dt=snap_dt))
+        #size_bytes = key['ContentLength'] # in kb
+        size_bytes = self.obja.list_objs(remote_path=self.get_default_file_path(snap_dt=snap_dt))['Size'].sum()
+        scale = {'KB': 1, 'MB': 2, 'GB': 3}.get(unit, 0)
+        size = size_bytes / (1024 ** scale)
+        return size
+    
+    def is_valid(self, snap_dt, size_threshold: float = 0.5) -> bool:
+        """Check if the file is valid
+        
+        """
+        return self.disk_space(snap_dt, unit = 'MB') > size_threshold
```

### Comparing `luntaiDs-1.0.8/SimpleDs/CommonTools/SnapStructure/tools.py` & `luntaiDs-1.0.9/SimpleDs/CommonTools/SnapStructure/tools.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/CommonTools/data_structure.py` & `luntaiDs-1.0.9/SimpleDs/CommonTools/data_structure.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/CommonTools/dbapi.py` & `luntaiDs-1.0.9/SimpleDs/CommonTools/dbapi.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/CommonTools/dtyper.py` & `luntaiDs-1.0.9/SimpleDs/CommonTools/dtyper.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/CommonTools/login.py` & `luntaiDs-1.0.9/SimpleDs/CommonTools/login.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/CommonTools/remote.py` & `luntaiDs-1.0.9/SimpleDs/ProviderTools/ssh/sftp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import contextlib
 import fnmatch
 import os
 import glob
+from typing import List
 import paramiko
 import logging
 from stat import S_ISDIR, S_ISREG
 from tqdm.auto import tqdm
 
-class MyRemote:
-    def __init__(self, host, port, username, password, private_key_file=None):
+class SFTP:
+    def __init__(self, host: str, port: int, username: str, password: str, private_key_file: str=None):
         """Remote server operations using paramiko
 
         :param host: ip address of the remote server
         :param port: port number of the remote server
         :param username: username to login
         :param password: password to login, could be None if private key file is provided
         :param private_key_file: the path to the private key file (id_rsa, should be in openSSH format)
@@ -36,31 +37,34 @@
 
         :param bash_cmd: bash command string
         :return: stdin_, stdout_, stderr_
         """
         stdin_, stdout_, stderr_ = self.ssh.exec_command(bash_cmd)
         return stdin_, stdout_, stderr_
 
-    def getFilePath(self, file):
+    def getFilePath(self, file: str):
         return f"SFTP://{self.username}@{self.host}:{self.port}/{file}"
 
-    def ls(self, remoteFolderPath: str, pattern: str = None):
+    def ls(self, remoteFolderPath: str, pattern: str = None, verbose: bool = False) -> List[str]:
         """List files under a specific folder, and can specify filetype to filter
 
         :param remoteFolderPath: the remote folder path to list file
         :param pattern: the pattern regrex string for file filters, e.g., pattern = "*.csv" will only show all csv files
+        :param verbose: whether to show the list
         :return:
         """
         with self.getSFTP() as sftp:
             file_list = sftp.listdir(remoteFolderPath)
             if pattern:
                 file_list = list(filter(lambda x: fnmatch.fnmatch(x, pattern), file_list))
-        print(f"{len(file_list)} files found under {remoteFolderPath}:")
-        for i, file in enumerate(file_list):
-            print(i, file)
+        if verbose:
+            print(f"{len(file_list)} files found under {remoteFolderPath}:")
+            for i, file in enumerate(file_list):
+                print(i, file)
+        return file_list
 
     def mkdir(self, path: str, mode: int = 511, ignore_existing: bool = False) -> int:
         """create a remote directory
 
         :param path: the remote directory path to create
         :param mode: mode of the file
         :param ignore_existing: if True, will not do anything when the remote folder already exists
@@ -100,15 +104,15 @@
         :return: the file context handler, can be accepted by pandas, json
         """
         with self.getSFTP() as sftp:
             fileObject = sftp.file(fullFilePath, mode)
             yield fileObject
             fileObject.close()
 
-    def download(self, remoteFilePath, localFilePath):
+    def download(self, remoteFilePath: str, localFilePath: str):
         """download a file from remote server to local
 
         :param remoteFilePath:
         :param localFilePath:
         :return:
         """
         with self.getSFTP() as sftp:
@@ -147,26 +151,26 @@
                         if not fnmatch.fnmatch(item.filename, pattern):
                             continue
                     sftp.get(remoteSubFolder, localSubFolder)
 
                     if verbose:
                         logging.info(f"Successfully download File {item.filename}")
 
-    def upload(self, localFilePath, remoteFilePath):
+    def upload(self, localFilePath: str, remoteFilePath: str):
         """Upload a file from local to remote server
 
         :param localFilePath:
         :param remoteFilePath:
         :return:
         """
         with self.getSFTP() as sftp:
             sftp.put(localFilePath, remoteFilePath)
             logging.info(f"Successfully upload File from {localFilePath} to {self.getFilePath(remoteFilePath)}")
 
-    def upload_folder(self, localFolderPath, remoteFolderPath, pattern: str = None, verbose: bool = False):
+    def upload_folder(self, localFolderPath: str, remoteFolderPath: str, pattern: str = None, verbose: bool = False):
         """download a remote folder to local
 
         :param localFolderPath:
         :param remoteFolderPath:
         :param pattern: the wildcard for file mask. e.g. *.csv to include only csv files
         :param verbose: if True, will print uploading details
         :return:
@@ -188,14 +192,24 @@
 
                     if verbose:
                         logging.info(f"Successfully uploaded File {item}")
                 else:
                     self.mkdir(remoteSubFolder, mode=511, ignore_existing=False)
                     self.upload_folder(localSubFolder, remoteSubFolder, pattern=pattern, verbose=verbose)
 
+    def copy(self, from_path: str, to_path: str):
+        cmd = f"cp {from_path} {to_path}"
+        self.bash(cmd)
+    
+    
+    def delete(self, remoteFolderPath: str):
+        with self.getSFTP() as sftp:
+            sftp.remove(remoteFolderPath)
+    
+    
     def delete_folder(self, remoteFolderPath: str):
         """Delete a folder recursively
 
         :param remoteFolderPath: the remote folder path to be deleted
         :return:
         """
         with self.getSFTP() as sftp:
@@ -205,11 +219,20 @@
                 if S_ISDIR(item.st_mode):
                     self.delete_folder(rpath)
                 else:
                     sftp.remove(rpath)
 
             sftp.rmdir(remoteFolderPath)
             logging.info(f"Successfully delete folder: {remoteFolderPath}")
-
-
-if __name__ == '__main__':
-    logging.basicConfig(level = logging.INFO)
+            
+    def size(self, remoteFilePath: str) -> int:
+        with self.getSFTP() as sftp:
+            stat = sftp.lstat(remoteFilePath)
+            if S_ISDIR(stat.st_mode):
+                # if a folder
+                size = 0
+                for f in self.ls(remoteFilePath):
+                    fpath = os.path.join(remoteFilePath, f)
+                    size += self.size(fpath)
+            else:
+                size = stat.st_size
+        return size
```

### Comparing `luntaiDs-1.0.8/SimpleDs/CommonTools/settings.py` & `luntaiDs-1.0.9/SimpleDs/CommonTools/settings.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/CommonTools/sparker.py` & `luntaiDs-1.0.9/SimpleDs/CommonTools/sparker.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/CommonTools/utils.py` & `luntaiDs-1.0.9/SimpleDs/CommonTools/utils.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/CustomModel/calibration.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/CustomModel/calibration.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/CustomModel/custom.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/CustomModel/custom.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/CustomModel/linear.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/CustomModel/linear.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/CustomModel/ordinal.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/CustomModel/ordinal.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/Evaluation/metrics.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/Evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/Evaluation/plots.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/Evaluation/plots.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/Evaluation/validator.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/Evaluation/validator.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/Explore/plots.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/Explore/plots.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/Explore/preview.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/Explore/preview.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/Explore/profiling.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/Explore/profiling.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/FeatureEngineer/featureHelper.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/FeatureEngineer/featureHelper.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/FeatureEngineer/feature_selection.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/FeatureEngineer/feature_selection.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/FeatureEngineer/preprocessing.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/FeatureEngineer/preprocessing.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/FeatureEngineer/transformers.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/FeatureEngineer/transformers.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/ModelServing.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/ModelServing.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/utils/analytical_dtype.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/utils/analytical_dtype.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/utils/parallel.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ModelingTools/utils/support.py` & `luntaiDs-1.0.9/SimpleDs/ModelingTools/utils/support.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ProviderTools/aws/s3.py` & `luntaiDs-1.0.9/SimpleDs/ProviderTools/aws/s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,25 @@
 import io
 import os
 
 from botocore.exceptions import ClientError
 import logging
 import pandas as pd
 import boto3
+from CommonTools.obj_storage import ObjStorage, remove_begin_slash, add_tail_slash
 
-def remove_begin_slash(url: str):
-    if url.startswith('/'):
-        prefix = str(url)[1:]
-    else:
-        prefix = str(url)
-    return prefix
-
-def add_tail_slash(url: str):
-    if url.endswith('/'):
-        return str(url)
-    else:
-        return str(url) + '/'
-
-class S3Accessor:
+class S3Accessor(ObjStorage):
     def __init__(self, aws_access_key_id=None, aws_secret_access_key=None,
                  aws_session_token=None, region_name=None,
                  botocore_session=None, profile_name=None,
                  service_name:str = 's3', api_version=None,
                  use_ssl=None, verify=None, endpoint_url=None,
                  config=None
                  ):
+        self.region_name = region_name
         try:
             self.session = boto3.Session(
                 aws_access_key_id = aws_access_key_id,
                 aws_secret_access_key = aws_secret_access_key,
                 aws_session_token = aws_session_token,
                 region_name = region_name,
                 botocore_session = botocore_session,
@@ -48,28 +37,34 @@
                 config = config
             )
 
         except Exception as e:
             logging.error(f"Boto3 failed to create client to access {service_name} \n{e}")
         else:
             logging.info("Boto3 session/client/resource created successfully.")
+            
+    def get_uri_protocol(self) -> str:
+        return "s3a"
 
-    def list_buckets(self):
+    def list_buckets(self) -> pd.DataFrame:
         return pd.DataFrame.from_records(self.client.list_buckets()['Buckets'])
 
-    def create_bucket(self, bucket_name: str, region_name: str = 'ca-central-1') -> int:
+    def create_bucket(self, bucket_name: str) -> int:
         """Create a new bucket
 
         :param bucket_name: name of the bucket
-        :param region_name: region on S3
         :return:
         """
+        if self.region_name:
+            region_config = {'LocationConstraint': self.region_name}
+        else:
+            region_config = None
         self.client.create_bucket(
             Bucket = bucket_name,
-            CreateBucketConfiguration = {'LocationConstraint': region_name}
+            CreateBucketConfiguration = region_config
         )
         return 1
 
     def get_bucket(self, bucket_name: str = None):
         return self.resource.Bucket(bucket_name)
 
     def get_buckets(self):
@@ -228,15 +223,15 @@
         from_bucket_name = self.if_not_exist_return_default_bucket(from_bucket_name)
         to_bucket_name = self.if_not_exist_return_default_bucket(to_bucket_name)
 
         copy_source = {
             'Bucket': from_bucket_name,
             'Key': remove_begin_slash(from_path)
         }
-        self.client.copy(copy_source, to_bucket_name, to_path)
+        self.client.copy(copy_source, to_bucket_name, remove_begin_slash(to_path))
 
 
     def upload_file(self, local_path: str, remote_path: str, bucket_name: str = None, multipart_threshold: int = 1000000000000):
         '''upload file from local machine to S3
 
         :param local_path: local file path that you would like to upload to S3, suggest to be absolute path
         :param remote_path: remote path on MinIO (excluding bucket path); could either start with / or not
@@ -256,15 +251,15 @@
                 self.client.upload_file(local_path, bucket_name, key)
         except Exception as e:
             logging.error(f'File upload FAILED from {local_path} to {key}:\n'+ str(e))
         else:
             logging.info(f'File uploaded successfully from {local_path} to {key}:')
 
     def download_file(self, remote_path: str, local_path: str, bucket_name: str = None):
-        '''download file from MinIO to local machine
+        '''download file from S3 to local machine
 
         :param remote_path: remote path on S3 (excluding bucket); could either start with / or not
         :param local_path: local file path that you would like to save the file from MinIO, suggest to be absolute path
         :param bucket_name
         :return:
         '''
         key = remove_begin_slash(remote_path)
@@ -274,34 +269,34 @@
             self.client.download_file(bucket_name, key, local_path)
         except Exception as e:
             logging.error(f'File download FAILED from {key} to {local_path}:\n'+ str(e))
         else:
             logging.info(f'File download successfully from {key} to {local_path}:')
 
 
-    def read_obj(self, remote_path: str, bucket_name: str = None):
+    def read_obj(self, remote_path: str, bucket_name: str = None) -> bytes:
         """read obj from S3 without downloading
 
         :param remote_path:  remote path to read on S3 (excluding bucket); could either start with / or not
         :param Bucket:
         :return: a buffer (io.StringIO() or io.BytesIO() which can pass to file reader
         """
 
         bucket_name = self.if_not_exist_return_default_bucket(bucket_name)
 
         obj = self.client.get_object(Bucket = bucket_name, Key= remove_begin_slash(remote_path))
         return obj['Body'].read()
 
-    def save_obj(self, body, remote_path: str, bucket_name: str = None) -> 1:
+    def save_obj(self, body: bytes, remote_path: str, bucket_name: str = None) -> 1:
         bucket_name = self.if_not_exist_return_default_bucket(bucket_name)
 
         self.resource.Object(bucket_name, remove_begin_slash(remote_path)).put(Body = body)
         return 1
 
-    def read_obj_to_iobuffer(self, remote_path: str, bucket_name: str = None):
+    def read_obj_to_iobuffer(self, remote_path: str, bucket_name: str = None) -> io.BytesIO:
         obj = self.read_obj(remote_path, bucket_name)
         buffer = io.BytesIO(obj)
         return buffer
 
     def save_iobuffer_to_obj(self, buffer: io.BytesIO, remote_path: str, bucket_name: str = None):
         self.save_obj(buffer.getvalue(), remote_path, bucket_name)
 
@@ -368,26 +363,31 @@
         :param remote_root_path: root path where the folder will be created on S3 (excluding bucket path)
         :param bucket_name:
         :param multipart_threshold: an argument controlling uploading size per partition
         :return:
         """
         local_folder_path = os.path.abspath(local_folder_path)
         local_parent_dir_path = os.path.dirname(local_folder_path)
+        bucket_name = self.if_not_exist_return_default_bucket(bucket_name)
 
         for path, subdirs, files in os.walk(local_folder_path):
 
             dirname = path.replace(local_parent_dir_path, '')
             for file in files:
                 local_filepath = os.path.join(path, file)
                 remote_filepath = os.path.join(dirname, file)
                 if os.path.sep == '\\':
                     remote_filepath = remote_filepath.replace("\\", "/")
                 remote_filepath = add_tail_slash(remove_begin_slash(remote_root_path)) +  remove_begin_slash(remote_filepath)
 
-                self.upload_file(local_path = local_filepath, remote_path = remote_filepath, bucket_name = bucket_name, multipart_threshold = multipart_threshold)
+                if multipart_threshold:
+                    config = boto3.s3.transfer.TransferConfig(multipart_threshold = multipart_threshold)
+                    self.client.upload_file(local_filepath, bucket_name, remote_filepath, Config = config)
+                else:
+                    self.client.upload_file(local_filepath, bucket_name, remote_filepath)
 
         logging.info(f"Successfully upload folder from {local_folder_path} to {remote_root_path}")
 
 
     def download_folder(self, remote_folder_path: str, local_root_path: str, bucket_name: str = None):
         """
 
@@ -400,13 +400,13 @@
         bucket_name = self.if_not_exist_return_default_bucket(bucket_name)
 
         for obj in self.resource.Bucket(bucket_name).objects.filter(Prefix = remote_folder_path):
             remote_filepath = obj.key
             local_filepath = os.path.join(local_root_path, os.path.relpath(remote_filepath, remote_folder_path))
             if not os.path.exists(os.path.dirname(local_filepath)):
                 os.makedirs(os.path.dirname(local_filepath))
-            if remote_filepath[-1] == '/':  # bypass void path
+            if remote_filepath.endswith("/"):  # bypass void path
                 continue
 
-            self.download_file(remote_path = remote_filepath, local_path = local_filepath, bucket_name = bucket_name)
+            self.client.download_file(bucket_name, remote_filepath, local_filepath)
 
         logging.info(f"Successfully download folder from {remote_folder_path} to {local_root_path}")
```

### Comparing `luntaiDs-1.0.8/SimpleDs/ProviderTools/clickhouse/dbapi.py` & `luntaiDs-1.0.9/SimpleDs/ProviderTools/clickhouse/dbapi.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ProviderTools/clickhouse/dtyper.py` & `luntaiDs-1.0.9/SimpleDs/ProviderTools/clickhouse/dtyper.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/ProviderTools/clickhouse/snap_struct.py` & `luntaiDs-1.0.9/SimpleDs/ProviderTools/clickhouse/snap_struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+from __future__ import annotations
 from datetime import date
 import logging
 from typing import List
 import pandas as pd
 import pyspark
 from CommonTools.sparker import SparkConnector
 from CommonTools.utils import dt2str, str2dt
@@ -19,16 +20,16 @@
         super(SnapshotDataManagerCHSQL, cls).setup(spark_connector = spark_connector)
         cls.ch_conf = ch_conf
         cls.ch = ClickhouseCRUD(ch_conf)
 
     def __init__(self, schema:str, table:str, snap_dt_key: str):
         """database management interface
 
-        :param schema: schema , e.g., RAW, PROCESSED
-        :param table:  table under each schema, e.g., CLNT_GENERAL, BDA_GENERAL
+        :param schema: schema
+        :param table:  table under each schema
         :param snap_dt_key: snap date column name for all tables
         """
         super().__init__(schema = schema, table = table)
         self.snap_dt_key = snap_dt_key
 
     def is_exist(self) -> bool:
         return self.ch.is_exist(schema=self.schema, table=self.table)
@@ -229,18 +230,24 @@
     def drop(self):
         """drop the whole table
 
         :return:
         """
         self.ch.drop_table(schema=self.schema, table=self.table)
 
-    def duplicate(self, dst_schema: str, dst_table: str):
+    def duplicate(self, dst_schema: str, dst_table: str) -> SnapshotDataManagerCHSQL:
         sql = """insert into {dst_schema:Identifier}.{dst_table:Identifier} select * from {src_schema:Identifier}.{src_table:Identifier}"""
         args = dict(dst_schema = dst_schema, dst_table = dst_table, src_schema = self.schema, src_table = self.table)
-        return self.ch.client.command(cmd = sql, parameters = args)
+        self.ch.client.command(cmd = sql, parameters = args)
+        new = SnapshotDataManagerCHSQL(
+            schema = dst_schema,
+            table = dst_table,
+            snap_dt_key = self.snap_dt_key
+        )
+        return new
 
     def disk_space(self, snap_dt, unit='MB') -> float:
         """get the size of the snap date file (pandas) or folder (pyspark partitions)
 
         :param snap_dt:
         :param unit: {KB, MB, GB}
         """
```

### Comparing `luntaiDs-1.0.8/SimpleDs/ProviderTools/teradata/dbapi.py` & `luntaiDs-1.0.9/SimpleDs/ProviderTools/teradata/dbapi.py`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/SimpleDs/luntaiDs.egg-info/PKG-INFO` & `luntaiDs-1.0.9/SimpleDs/luntaiDs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luntaiDs
-Version: 1.0.8
+Version: 1.0.9
 Summary: Make Data Scientist life Easier Tool
 Home-page: https://github.com/luntaixiax/luntai-ds
 Author: Ailun Qian (luntaixia)
 Author-email: ailunqian124@gmail.com
 License: MIT License
         
         Copyright (c) 2023 luntaixiax
```

### Comparing `luntaiDs-1.0.8/SimpleDs/luntaiDs.egg-info/SOURCES.txt` & `luntaiDs-1.0.9/SimpleDs/luntaiDs.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 setup.cfg
 SimpleDs/CommonTools/__init__.py
 SimpleDs/CommonTools/accessor.py
 SimpleDs/CommonTools/data_structure.py
 SimpleDs/CommonTools/dbapi.py
 SimpleDs/CommonTools/dtyper.py
 SimpleDs/CommonTools/login.py
-SimpleDs/CommonTools/remote.py
+SimpleDs/CommonTools/obj_storage.py
 SimpleDs/CommonTools/settings.py
 SimpleDs/CommonTools/sparker.py
 SimpleDs/CommonTools/utils.py
 SimpleDs/CommonTools/SnapStructure/__init__.py
 SimpleDs/CommonTools/SnapStructure/dependency.py
 SimpleDs/CommonTools/SnapStructure/structure.py
 SimpleDs/CommonTools/SnapStructure/tools.py
@@ -41,19 +41,23 @@
 SimpleDs/ModelingTools/utils/analytical_dtype.py
 SimpleDs/ModelingTools/utils/checks.py
 SimpleDs/ModelingTools/utils/parallel.py
 SimpleDs/ModelingTools/utils/support.py
 SimpleDs/ProviderTools/__init__.py
 SimpleDs/ProviderTools/aws/__init__.py
 SimpleDs/ProviderTools/aws/s3.py
-SimpleDs/ProviderTools/aws/snap_struct.py
 SimpleDs/ProviderTools/clickhouse/__init__.py
 SimpleDs/ProviderTools/clickhouse/dbapi.py
 SimpleDs/ProviderTools/clickhouse/dtyper.py
 SimpleDs/ProviderTools/clickhouse/snap_struct.py
+SimpleDs/ProviderTools/gcp/__init__.py
+SimpleDs/ProviderTools/gcp/gcs.py
+SimpleDs/ProviderTools/ssh/__init__.py
+SimpleDs/ProviderTools/ssh/sftp.py
+SimpleDs/ProviderTools/ssh/snap_struct.py
 SimpleDs/ProviderTools/teradata/__init__.py
 SimpleDs/ProviderTools/teradata/dbapi.py
 SimpleDs/luntaiDs.egg-info/PKG-INFO
 SimpleDs/luntaiDs.egg-info/SOURCES.txt
 SimpleDs/luntaiDs.egg-info/dependency_links.txt
 SimpleDs/luntaiDs.egg-info/requires.txt
 SimpleDs/luntaiDs.egg-info/top_level.txt
```

### Comparing `luntaiDs-1.0.8/pyproject.toml` & `luntaiDs-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `luntaiDs-1.0.8/setup.cfg` & `luntaiDs-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = luntaiDs
-version = 1.0.8
+version = 1.0.9
 author = luntaixia
 author_email = ailunqian124@gmail.com
 url = https://github.com/luntaixiax/luntai-ds
 description = Make Data Scientist life Easier Tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

