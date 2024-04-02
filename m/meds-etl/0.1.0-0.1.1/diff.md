# Comparing `tmp/meds_etl-0.1.0.tar.gz` & `tmp/meds_etl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meds_etl-0.1.0.tar", last modified: Wed Mar 20 22:48:32 2024, max compression
+gzip compressed data, was "meds_etl-0.1.1.tar", last modified: Tue Apr  2 02:17:59 2024, max compression
```

## Comparing `meds_etl-0.1.0.tar` & `meds_etl-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-x---   0 esteinberg  (1064) ca-admin  (1001)        0 2024-03-20 22:48:32.714358 meds_etl-0.1.0/
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)      124 2024-03-20 16:08:44.000000 meds_etl-0.1.0/.flake8
-drwxr-x---   0 esteinberg  (1064) ca-admin  (1001)        0 2024-03-20 22:48:32.694358 meds_etl-0.1.0/.github/
-drwxr-x---   0 esteinberg  (1064) ca-admin  (1001)        0 2024-03-20 22:48:32.698358 meds_etl-0.1.0/.github/workflows/
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)     2638 2024-03-20 17:03:48.000000 meds_etl-0.1.0/.github/workflows/python-build.yml
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)      908 2024-03-20 16:08:44.000000 meds_etl-0.1.0/.github/workflows/python-test.yml
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)     3116 2024-03-20 16:08:44.000000 meds_etl-0.1.0/.gitignore
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)      530 2024-03-20 16:08:44.000000 meds_etl-0.1.0/.pre-commit-config.yaml
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)    11357 2024-03-20 16:08:44.000000 meds_etl-0.1.0/LICENSE
--rw-r--r--   0 esteinberg  (1064) ca-admin  (1001)     4608 2024-03-20 22:48:32.710358 meds_etl-0.1.0/PKG-INFO
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)     4227 2024-03-20 16:08:44.000000 meds_etl-0.1.0/README.md
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)      961 2024-03-20 17:18:21.000000 meds_etl-0.1.0/pyproject.toml
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)       38 2024-03-20 22:48:32.714358 meds_etl-0.1.0/setup.cfg
-drwxr-x---   0 esteinberg  (1064) ca-admin  (1001)        0 2024-03-20 22:48:32.694358 meds_etl-0.1.0/src/
-drwxr-x---   0 esteinberg  (1064) ca-admin  (1001)        0 2024-03-20 22:48:32.702358 meds_etl-0.1.0/src/meds_etl/
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)       50 2024-03-20 16:08:44.000000 meds_etl-0.1.0/src/meds_etl/__init__.py
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)      411 2024-03-20 22:48:32.000000 meds_etl-0.1.0/src/meds_etl/_version.py
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)    16526 2024-03-20 22:43:28.000000 meds_etl-0.1.0/src/meds_etl/flat.py
-drwxr-x---   0 esteinberg  (1064) ca-admin  (1001)        0 2024-03-20 22:48:32.706358 meds_etl-0.1.0/src/meds_etl/mimic/
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)    17871 2024-03-20 16:08:44.000000 meds_etl-0.1.0/src/meds_etl/mimic/__init__.py
-drwxr-x---   0 esteinberg  (1064) ca-admin  (1001)        0 2024-03-20 22:48:32.710358 meds_etl-0.1.0/src/meds_etl/mimic/concept_map/
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)     1144 2024-03-20 16:08:44.000000 meds_etl-0.1.0/src/meds_etl/mimic/concept_map/LICENSE
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)   361049 2024-03-20 16:08:44.000000 meds_etl-0.1.0/src/meds_etl/mimic/concept_map/d_labitems_to_loinc.csv
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)    79196 2024-03-20 16:08:44.000000 meds_etl-0.1.0/src/meds_etl/mimic/concept_map/inputevents_to_rxnorm.csv
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)    79970 2024-03-20 16:08:44.000000 meds_etl-0.1.0/src/meds_etl/mimic/concept_map/lab_itemid_to_loinc.csv
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)    34863 2024-03-20 16:08:44.000000 meds_etl-0.1.0/src/meds_etl/mimic/concept_map/meas_chartevents_main.csv
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)     5903 2024-03-20 16:08:44.000000 meds_etl-0.1.0/src/meds_etl/mimic/concept_map/meas_chartevents_value.csv
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)    32354 2024-03-20 16:08:44.000000 meds_etl-0.1.0/src/meds_etl/mimic/concept_map/numerics-summary.csv
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)    34008 2024-03-20 16:08:44.000000 meds_etl-0.1.0/src/meds_etl/mimic/concept_map/outputevents_to_loinc.csv
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)    25206 2024-03-20 16:08:44.000000 meds_etl-0.1.0/src/meds_etl/mimic/concept_map/proc_datetimeevents.csv
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)    21414 2024-03-20 16:08:44.000000 meds_etl-0.1.0/src/meds_etl/mimic/concept_map/proc_itemid.csv
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)     5744 2024-03-20 16:08:44.000000 meds_etl-0.1.0/src/meds_etl/mimic/concept_map/waveforms-summary.csv
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)    19222 2024-03-20 22:43:28.000000 meds_etl-0.1.0/src/meds_etl/omop.py
-drwxr-x---   0 esteinberg  (1064) ca-admin  (1001)        0 2024-03-20 22:48:32.710358 meds_etl-0.1.0/src/meds_etl.egg-info/
--rw-r--r--   0 esteinberg  (1064) ca-admin  (1001)     4608 2024-03-20 22:48:32.000000 meds_etl-0.1.0/src/meds_etl.egg-info/PKG-INFO
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)     1127 2024-03-20 22:48:32.000000 meds_etl-0.1.0/src/meds_etl.egg-info/SOURCES.txt
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)        1 2024-03-20 22:48:32.000000 meds_etl-0.1.0/src/meds_etl.egg-info/dependency_links.txt
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)      210 2024-03-20 22:48:32.000000 meds_etl-0.1.0/src/meds_etl.egg-info/entry_points.txt
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)       96 2024-03-20 22:48:32.000000 meds_etl-0.1.0/src/meds_etl.egg-info/requires.txt
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)        9 2024-03-20 22:48:32.000000 meds_etl-0.1.0/src/meds_etl.egg-info/top_level.txt
-drwxr-x---   0 esteinberg  (1064) ca-admin  (1001)        0 2024-03-20 22:48:32.710358 meds_etl-0.1.0/tests/
-drwxr-x---   0 esteinberg  (1064) ca-admin  (1001)        0 2024-03-20 22:48:32.710358 meds_etl-0.1.0/tests/data/
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)        0 2024-03-20 16:08:44.000000 meds_etl-0.1.0/tests/data/.gitkeep
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)     2796 2024-03-20 16:08:44.000000 meds_etl-0.1.0/tests/test_etl.py
--rw-r-----   0 esteinberg  (1064) ca-admin  (1001)     6769 2024-03-20 16:08:44.000000 meds_etl-0.1.0/tests/test_flat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.785429 meds_etl-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 02:17:55.000000 meds_etl-0.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.777429 meds_etl-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.777429 meds_etl-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-02 02:17:55.000000 meds_etl-0.1.1/.github/workflows/python-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-02 02:17:55.000000 meds_etl-0.1.1/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-02 02:17:55.000000 meds_etl-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-02 02:17:55.000000 meds_etl-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 02:17:55.000000 meds_etl-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-02 02:17:59.785429 meds_etl-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-02 02:17:55.000000 meds_etl-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 02:17:55.000000 meds_etl-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 02:17:59.785429 meds_etl-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.777429 meds_etl-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.781429 meds_etl-0.1.1/src/meds_etl/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17097 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/flat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.781429 meds_etl-0.1.1/src/meds_etl/mimic/
+-rw-r--r--   0 runner    (1001) docker     (127)    17871 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.785429 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   361049 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/d_labitems_to_loinc.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    79196 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/inputevents_to_rxnorm.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    79970 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/lab_itemid_to_loinc.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/meas_chartevents_main.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/meas_chartevents_value.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    32354 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/numerics-summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    34008 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/outputevents_to_loinc.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    25206 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/proc_datetimeevents.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21414 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/proc_itemid.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/waveforms-summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    34130 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/omop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.785429 meds_etl-0.1.1/src/meds_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.785429 meds_etl-0.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.785429 meds_etl-0.1.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:55.000000 meds_etl-0.1.1/tests/data/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-02 02:17:55.000000 meds_etl-0.1.1/tests/test_etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-02 02:17:55.000000 meds_etl-0.1.1/tests/test_flat.py
```

### Comparing `meds_etl-0.1.0/.github/workflows/python-build.yml` & `meds_etl-0.1.1/.github/workflows/python-build.yml`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/.github/workflows/python-test.yml` & `meds_etl-0.1.1/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/.gitignore` & `meds_etl-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/.pre-commit-config.yaml` & `meds_etl-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/LICENSE` & `meds_etl-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/PKG-INFO` & `meds_etl-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,46 @@
-Metadata-Version: 2.1
-Name: meds_etl
-Version: 0.1.0
-Summary: A data standard for working with event stream data
-License: Apache-2.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyarrow>=8
-Requires-Dist: polars>=0.20.10
-Requires-Dist: jsonschema>=4.0.0
-Requires-Dist: meds==0.1.3
-Requires-Dist: typing_extensions>=4.0
-Requires-Dist: datasets>=2.0.0
-
 # meds_etl
 
 A collection of ETLs from common data formats to Medical Event Data Standard (MEDS)
 
 This package library currently supports:
 
 - MIMIC-IV
 - OMOP v5
 - MEDS FLAT, a flat version of MEDS
+
 ## Setup
 Create an environment of your choice:
-```
+```bash
 conda create -n meds_etl
 ```
 Install the package
-```
+```bash
 python -m pip install .
 ```
+
 ## MIMIC-IV
 
 In order to run the MIMIC-IV ETL, simply run the following command:
 
-`meds_etl_mimic mimiciv mimiciv_meds` where mimiciv is a download of MIMIC-IV and mimiciv_meds will be the destination path for the dataset.
+```bash
+meds_etl_mimic [PATH_TO_SOURCE_MIMIC] [PATH_TO_OUTPUT]
+```
+
+where `[PATH_TO_SOURCE_MIMIC]` is a download of MIMIC-IV and `[PATH_TO_OUTPUT]` will be the destination path for the MEDS dataset.
 
 ## OMOP
 
-In order to run the MIMIC-IV ETL, simply run the following command:
+In order to run the OMOP ETL, simply run the following command:
+
+```bash
+meds_etl_omop [PATH_TO_SOURCE_OMOP] [PATH_TO_OUTPUT]
+```
 
-`meds_etl_omop omop omop_meds` where omop is a folder containing csv files (optionally gzipped) for an OMOP dataset. Each table should either be a csv file with the table name (such as person.csv) or a folder with the table name containing csv files.
+where `[PATH_TO_SOURCE_OMOP]` is a folder containing csv files (optionally gzipped) for an OMOP dataset and `[PATH_TO_OUTPUT]` will be the destination path for the MEDS dataset. Each OMOP table should either be a csv file with the table name (such as person.csv) or a folder with the table name containing csv files.
 
 ## Unit tests
 
 Tests can be run from the project root with the following command:
 
 ```
 pytest -v
@@ -99,13 +95,36 @@
     },
     {
       'time': 1990-12-28,
       'measurements': [{'code': 'ICD10CM/E11.4', 'metadata': {'arbitrary_metadata_column': 'anything'}}],
     },
   ]
 }
+```
 
 We also support an inverse ETL, converting from MEDS to MEDS Flat.
 
 The command for this is `meds_etl_to_flat`. For example:
 
 `meds_etl_to_flat meds meds_flat` where meds is a folder containing a MEDS dataset and meds_flat is the folder that will store the resulting MEDS Flat dataset.
+
+## Troubleshooting
+
+**Polars incompatible with Mac M1**
+
+If you get this error when running `meds_etl`:
+
+```bash
+RuntimeWarning: Missing required CPU features.
+
+The following required CPU features were not detected:
+    avx, fma
+Continuing to use this version of Polars on this processor will likely result in a crash.
+Install the `polars-lts-cpu` package instead of `polars` to run Polars with better compatibility.
+```
+
+Then you'll need to install the run the following:
+
+```bash
+pip uninstall polars
+pip install polars-lts-cpu
+```
```

### Comparing `meds_etl-0.1.0/README.md` & `meds_etl-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,61 @@
+Metadata-Version: 2.1
+Name: meds_etl
+Version: 0.1.1
+Summary: A data standard for working with event stream data
+License: Apache-2.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyarrow>=8
+Requires-Dist: polars>=0.20.10
+Requires-Dist: jsonschema>=4.0.0
+Requires-Dist: meds==0.1.3
+Requires-Dist: typing_extensions>=4.0
+Requires-Dist: datasets>=2.0.0
+Requires-Dist: tqdm>=4.6.0
+
 # meds_etl
 
 A collection of ETLs from common data formats to Medical Event Data Standard (MEDS)
 
 This package library currently supports:
 
 - MIMIC-IV
 - OMOP v5
 - MEDS FLAT, a flat version of MEDS
+
 ## Setup
 Create an environment of your choice:
-```
+```bash
 conda create -n meds_etl
 ```
 Install the package
-```
+```bash
 python -m pip install .
 ```
+
 ## MIMIC-IV
 
 In order to run the MIMIC-IV ETL, simply run the following command:
 
-`meds_etl_mimic mimiciv mimiciv_meds` where mimiciv is a download of MIMIC-IV and mimiciv_meds will be the destination path for the dataset.
+```bash
+meds_etl_mimic [PATH_TO_SOURCE_MIMIC] [PATH_TO_OUTPUT]
+```
+
+where `[PATH_TO_SOURCE_MIMIC]` is a download of MIMIC-IV and `[PATH_TO_OUTPUT]` will be the destination path for the MEDS dataset.
 
 ## OMOP
 
-In order to run the MIMIC-IV ETL, simply run the following command:
+In order to run the OMOP ETL, simply run the following command:
+
+```bash
+meds_etl_omop [PATH_TO_SOURCE_OMOP] [PATH_TO_OUTPUT]
+```
 
-`meds_etl_omop omop omop_meds` where omop is a folder containing csv files (optionally gzipped) for an OMOP dataset. Each table should either be a csv file with the table name (such as person.csv) or a folder with the table name containing csv files.
+where `[PATH_TO_SOURCE_OMOP]` is a folder containing csv files (optionally gzipped) for an OMOP dataset and `[PATH_TO_OUTPUT]` will be the destination path for the MEDS dataset. Each OMOP table should either be a csv file with the table name (such as person.csv) or a folder with the table name containing csv files.
 
 ## Unit tests
 
 Tests can be run from the project root with the following command:
 
 ```
 pytest -v
@@ -85,13 +110,36 @@
     },
     {
       'time': 1990-12-28,
       'measurements': [{'code': 'ICD10CM/E11.4', 'metadata': {'arbitrary_metadata_column': 'anything'}}],
     },
   ]
 }
+```
 
 We also support an inverse ETL, converting from MEDS to MEDS Flat.
 
 The command for this is `meds_etl_to_flat`. For example:
 
 `meds_etl_to_flat meds meds_flat` where meds is a folder containing a MEDS dataset and meds_flat is the folder that will store the resulting MEDS Flat dataset.
+
+## Troubleshooting
+
+**Polars incompatible with Mac M1**
+
+If you get this error when running `meds_etl`:
+
+```bash
+RuntimeWarning: Missing required CPU features.
+
+The following required CPU features were not detected:
+    avx, fma
+Continuing to use this version of Polars on this processor will likely result in a crash.
+Install the `polars-lts-cpu` package instead of `polars` to run Polars with better compatibility.
+```
+
+Then you'll need to install the run the following:
+
+```bash
+pip uninstall polars
+pip install polars-lts-cpu
+```
```

### Comparing `meds_etl-0.1.0/pyproject.toml` & `meds_etl-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 dependencies = [
     "pyarrow >= 8",
     "polars >= 0.20.10",
     "jsonschema >= 4.0.0",
     "meds == 0.1.3",
     "typing_extensions >= 4.0",
     "datasets >= 2.0.0",
+    "tqdm >= 4.6.0"
 ]
 
 [project.scripts]
 meds_etl_mimic = "meds_etl.mimic:main"
 meds_etl_omop = "meds_etl.omop:main"
 meds_etl_from_flat = "meds_etl.flat:convert_flat_to_meds_main"
 meds_etl_to_flat = "meds_etl.flat:convert_meds_to_flat_main"
```

### Comparing `meds_etl-0.1.0/src/meds_etl/flat.py` & `meds_etl-0.1.1/src/meds_etl/flat.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import tempfile
 from typing import Iterable, List, Literal, Set, TextIO, Tuple, cast
 
 import meds
 import polars as pl
 import pyarrow as pa
 import pyarrow.parquet as pq
+from tqdm import tqdm
 
 mp = multiprocessing.get_context("forkserver")
 if mp is None:
     # Could not get forkserver, just use the default
     mp = multiprocessing.get_context()
 
 Format = Literal["csv", "parquet", "compressed_csv"]
@@ -252,15 +253,15 @@
         fname = os.path.join(temp_dir, str(shard_index), filename)
         shard.write_parquet(fname, compression="uncompressed")
 
 
 def process_parquet_file(
     event_file: str, *, temp_dir: str, num_shards: int, time_formats: Iterable[str], metadata_columns: List[str]
 ):
-    """Convert a MEDS Flat parquet file to MEDS."""
+    """Partition MEDS Flat files into shards based on patient ID and write to disk"""
     logging.info("Working on ", event_file)
 
     table = pl.scan_parquet(event_file)
 
     cleaned_event_file = os.path.basename(event_file).split(".")[0]
     fname = f"{cleaned_event_file}.parquet"
     create_and_write_shards_from_table(table, temp_dir, num_shards, time_formats, metadata_columns, fname)
@@ -341,15 +342,15 @@
             parquet_tasks.append(full_flat_file)
 
     random.seed(3422342)
     random.shuffle(csv_tasks)
     random.shuffle(parquet_tasks)
 
     if num_proc != 1:
-        with mp.get_context("spawn").Pool(num_proc) as pool:
+        with mp.get_context("spawn").Pool(num_proc, maxtasksperchild=1) as pool:
             metadata_columns_set = set()
             for columns in pool.imap_unordered(get_csv_columns, csv_tasks):
                 metadata_columns_set |= columns
             for columns in pool.imap_unordered(get_parquet_columns, parquet_tasks):
                 metadata_columns_set |= columns
 
             metadata_columns_set -= KNOWN_COLUMNS
@@ -368,18 +369,21 @@
                 process_parquet_file,
                 temp_dir=temp_dir,
                 num_shards=num_shards,
                 time_formats=time_formats,
                 metadata_columns=metadata_columns,
             )
 
-            for _ in pool.imap_unordered(csv_processor, csv_tasks):
-                pass
-            for _ in pool.imap_unordered(parquet_processor, parquet_tasks):
-                pass
+            print("Partitioning MEDS Flat files into shards based on patient ID and writing to disk...")
+            with tqdm(total=len(csv_tasks)) as pbar:
+                for _ in pool.imap_unordered(csv_processor, csv_tasks):
+                    pbar.update()
+            with tqdm(total=len(parquet_tasks)) as pbar:
+                for _ in pool.imap_unordered(parquet_processor, parquet_tasks):
+                    pbar.update()
     else:
         metadata_columns_set = set()
         for task in csv_tasks:
             metadata_columns_set |= get_csv_columns(task)
         for task in parquet_tasks:
             metadata_columns_set |= get_parquet_columns(task)
 
@@ -398,27 +402,29 @@
             process_parquet_file,
             temp_dir=temp_dir,
             num_shards=num_shards,
             time_formats=time_formats,
             metadata_columns=metadata_columns,
         )
 
-        for task in csv_tasks:
+        for task in tqdm(csv_tasks, total=len(csv_tasks)):
             csv_processor(task)
-        for task in parquet_tasks:
+        for task in tqdm(parquet_tasks, total=len(parquet_tasks)):
             parquet_processor(task)
 
     shutil.rmtree(decompressed_dir)
 
     logging.info("Processing each shard")
 
     data_dir = os.path.join(target_meds_path, "data")
     os.mkdir(data_dir)
 
-    for shard_index in range(num_shards):
+    print("Collating source table data, shard by shard, to create patient timelines...")
+    print("(Gathering measurements into events, events into timelines)")
+    for shard_index in tqdm(range(num_shards), total=num_shards):
         logging.info("Processing shard ", shard_index)
         shard_dir = os.path.join(temp_dir, str(shard_index))
 
         if len(os.listdir(shard_dir)) == 0:
             continue
 
         events = [pl.scan_parquet(os.path.join(shard_dir, a)) for a in os.listdir(shard_dir)]
```

### Comparing `meds_etl-0.1.0/src/meds_etl/mimic/__init__.py` & `meds_etl-0.1.1/src/meds_etl/mimic/__init__.py`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/src/meds_etl/mimic/concept_map/LICENSE` & `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/LICENSE`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/src/meds_etl/mimic/concept_map/d_labitems_to_loinc.csv` & `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/d_labitems_to_loinc.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/src/meds_etl/mimic/concept_map/inputevents_to_rxnorm.csv` & `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/inputevents_to_rxnorm.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/src/meds_etl/mimic/concept_map/lab_itemid_to_loinc.csv` & `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/lab_itemid_to_loinc.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/src/meds_etl/mimic/concept_map/meas_chartevents_main.csv` & `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/meas_chartevents_main.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/src/meds_etl/mimic/concept_map/meas_chartevents_value.csv` & `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/meas_chartevents_value.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/src/meds_etl/mimic/concept_map/numerics-summary.csv` & `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/numerics-summary.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/src/meds_etl/mimic/concept_map/outputevents_to_loinc.csv` & `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/outputevents_to_loinc.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/src/meds_etl/mimic/concept_map/proc_datetimeevents.csv` & `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/proc_datetimeevents.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/src/meds_etl/mimic/concept_map/proc_itemid.csv` & `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/proc_itemid.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/src/meds_etl/mimic/concept_map/waveforms-summary.csv` & `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/waveforms-summary.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/src/meds_etl.egg-info/PKG-INFO` & `meds_etl-0.1.1/src/meds_etl.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,61 @@
 Metadata-Version: 2.1
 Name: meds_etl
-Version: 0.1.0
+Version: 0.1.1
 Summary: A data standard for working with event stream data
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow>=8
 Requires-Dist: polars>=0.20.10
 Requires-Dist: jsonschema>=4.0.0
 Requires-Dist: meds==0.1.3
 Requires-Dist: typing_extensions>=4.0
 Requires-Dist: datasets>=2.0.0
+Requires-Dist: tqdm>=4.6.0
 
 # meds_etl
 
 A collection of ETLs from common data formats to Medical Event Data Standard (MEDS)
 
 This package library currently supports:
 
 - MIMIC-IV
 - OMOP v5
 - MEDS FLAT, a flat version of MEDS
+
 ## Setup
 Create an environment of your choice:
-```
+```bash
 conda create -n meds_etl
 ```
 Install the package
-```
+```bash
 python -m pip install .
 ```
+
 ## MIMIC-IV
 
 In order to run the MIMIC-IV ETL, simply run the following command:
 
-`meds_etl_mimic mimiciv mimiciv_meds` where mimiciv is a download of MIMIC-IV and mimiciv_meds will be the destination path for the dataset.
+```bash
+meds_etl_mimic [PATH_TO_SOURCE_MIMIC] [PATH_TO_OUTPUT]
+```
+
+where `[PATH_TO_SOURCE_MIMIC]` is a download of MIMIC-IV and `[PATH_TO_OUTPUT]` will be the destination path for the MEDS dataset.
 
 ## OMOP
 
-In order to run the MIMIC-IV ETL, simply run the following command:
+In order to run the OMOP ETL, simply run the following command:
 
-`meds_etl_omop omop omop_meds` where omop is a folder containing csv files (optionally gzipped) for an OMOP dataset. Each table should either be a csv file with the table name (such as person.csv) or a folder with the table name containing csv files.
+```bash
+meds_etl_omop [PATH_TO_SOURCE_OMOP] [PATH_TO_OUTPUT]
+```
+
+where `[PATH_TO_SOURCE_OMOP]` is a folder containing csv files (optionally gzipped) for an OMOP dataset and `[PATH_TO_OUTPUT]` will be the destination path for the MEDS dataset. Each OMOP table should either be a csv file with the table name (such as person.csv) or a folder with the table name containing csv files.
 
 ## Unit tests
 
 Tests can be run from the project root with the following command:
 
 ```
 pytest -v
@@ -99,13 +110,36 @@
     },
     {
       'time': 1990-12-28,
       'measurements': [{'code': 'ICD10CM/E11.4', 'metadata': {'arbitrary_metadata_column': 'anything'}}],
     },
   ]
 }
+```
 
 We also support an inverse ETL, converting from MEDS to MEDS Flat.
 
 The command for this is `meds_etl_to_flat`. For example:
 
 `meds_etl_to_flat meds meds_flat` where meds is a folder containing a MEDS dataset and meds_flat is the folder that will store the resulting MEDS Flat dataset.
+
+## Troubleshooting
+
+**Polars incompatible with Mac M1**
+
+If you get this error when running `meds_etl`:
+
+```bash
+RuntimeWarning: Missing required CPU features.
+
+The following required CPU features were not detected:
+    avx, fma
+Continuing to use this version of Polars on this processor will likely result in a crash.
+Install the `polars-lts-cpu` package instead of `polars` to run Polars with better compatibility.
+```
+
+Then you'll need to install the run the following:
+
+```bash
+pip uninstall polars
+pip install polars-lts-cpu
+```
```

### Comparing `meds_etl-0.1.0/src/meds_etl.egg-info/SOURCES.txt` & `meds_etl-0.1.1/src/meds_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/tests/test_etl.py` & `meds_etl-0.1.1/tests/test_etl.py`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.0/tests/test_flat.py` & `meds_etl-0.1.1/tests/test_flat.py`

 * *Files identical despite different names*

