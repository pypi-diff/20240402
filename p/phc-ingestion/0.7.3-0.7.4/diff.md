# Comparing `tmp/phc-ingestion-0.7.3.tar.gz` & `tmp/phc-ingestion-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.7.3.tar", last modified: Thu Feb  8 22:24:23 2024, max compression
+gzip compressed data, was "phc-ingestion-0.7.4.tar", last modified: Mon Apr  1 22:07:20 2024, max compression
```

## Comparing `phc-ingestion-0.7.3.tar` & `phc-ingestion-0.7.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0       16 2024-02-08 22:23:41.327410 phc-ingestion-0.7.3/PYPI.md
--rw-r--r--   0        0        0        0 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1636 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1640 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      747 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/util/hla.py
--rw-r--r--   0        0        0      555 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4976 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    23255 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     5022 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     3324 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3151 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0    10987 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     2163 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0        0 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/generic/__init__.py
--rw-r--r--   0        0        0     1548 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/generic/process.py
--rw-r--r--   0        0        0     2814 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/generic/utils.py
--rw-r--r--   0        0        0       46 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3074 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8522 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     5451 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     7341 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2047 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0       68 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/shared_util/types.py
--rw-r--r--   0        0        0     5398 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/vcf_standardization/Variant.py
--rw-r--r--   0        0        0        0 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/vcf_standardization/__init__.py
--rw-r--r--   0        0        0     2289 2024-02-08 22:23:41.331410 phc-ingestion-0.7.3/ingestion/vcf_standardization/standardize.py
--rw-r--r--   0        0        0        0 2024-02-08 22:23:41.335410 phc-ingestion-0.7.3/ingestion/vcf_standardization/util/__init__.py
--rw-r--r--   0        0        0     1061 2024-02-08 22:23:41.335410 phc-ingestion-0.7.3/ingestion/vcf_standardization/util/af_helpers.py
--rw-r--r--   0        0        0      823 2024-02-08 22:23:41.335410 phc-ingestion-0.7.3/ingestion/vcf_standardization/util/dp_helpers.py
--rw-r--r--   0        0        0     2471 2024-02-08 22:23:41.335410 phc-ingestion-0.7.3/ingestion/vcf_standardization/util/read_write.py
--rw-r--r--   0        0        0     1009 2024-02-08 22:23:41.335410 phc-ingestion-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 phc-ingestion-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/PYPI.md
+-rw-r--r--   0        0        0        0 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1636 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1640 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      747 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/hla.py
+-rw-r--r--   0        0        0      555 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4976 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    23579 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     5022 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     3324 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3151 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0    10987 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     2163 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0        0 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/generic/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/generic/process.py
+-rw-r--r--   0        0        0     2814 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/generic/utils.py
+-rw-r--r--   0        0        0       46 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8522 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     5451 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7341 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2047 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0       68 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/shared_util/types.py
+-rw-r--r--   0        0        0     5398 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/Variant.py
+-rw-r--r--   0        0        0        0 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/__init__.py
+-rw-r--r--   0        0        0     2289 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/standardize.py
+-rw-r--r--   0        0        0        0 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/util/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/util/af_helpers.py
+-rw-r--r--   0        0        0      823 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/util/dp_helpers.py
+-rw-r--r--   0        0        0     2471 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/util/read_write.py
+-rw-r--r--   0        0        0     1009 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 phc-ingestion-0.7.4/PKG-INFO
```

### Comparing `phc-ingestion-0.7.3/ingestion/caris/process.py` & `phc-ingestion-0.7.4/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/caris/util/cnv.py` & `phc-ingestion-0.7.4/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.7.4/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.7.4/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/caris/util/hla.py` & `phc-ingestion-0.7.4/ingestion/caris/util/hla.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.7.4/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/caris/util/json.py` & `phc-ingestion-0.7.4/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/caris/util/metadata.py` & `phc-ingestion-0.7.4/ingestion/caris/util/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -440,15 +440,22 @@
             if (
                 "clinical genes" in test["testName"].lower()
                 and "test_cancellation_reason" not in test.keys()
                 and test["testMethodology"] == "Seq"
             ):
                 # They don't always do exome sequencing
                 ingest_status["exome_performed"] = True
-                for info in test["testResults"]:
+                # Sometimes, if there is only a single test result,
+                # Caris will set it as a dict instead of a list
+                test_results = (
+                    [test["testResults"]]
+                    if isinstance(test["testResults"], dict)
+                    else test["testResults"]
+                )
+                for info in test_results:
                     if "tumorMutationBurden" in info.keys():
                         tmb = info["tumorMutationBurden"]["mutationBurdenCall"].lower()
                         tmbScore = info["tumorMutationBurden"]["mutationBurdenScore"]
                         if not tmbScore:
                             continue
                         tmbUnit = info["tumorMutationBurden"]["mutationBurdenUnit"]
                         # Convert from their format, which is "21 per Mb"
```

### Comparing `phc-ingestion-0.7.3/ingestion/caris/util/structural.py` & `phc-ingestion-0.7.4/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/caris/util/tsv.py` & `phc-ingestion-0.7.4/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/caris/util/vcf.py` & `phc-ingestion-0.7.4/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/foundation/process.py` & `phc-ingestion-0.7.4/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.7.4/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.7.4/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.7.4/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.7.4/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/generic/process.py` & `phc-ingestion-0.7.4/ingestion/generic/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/generic/utils.py` & `phc-ingestion-0.7.4/ingestion/generic/utils.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/nextgen/process.py` & `phc-ingestion-0.7.4/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.7.4/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.7.4/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.7.4/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.7.4/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.7.4/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.7.4/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.7.4/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.7.4/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.7.4/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/vcf_standardization/Variant.py` & `phc-ingestion-0.7.4/ingestion/vcf_standardization/Variant.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/vcf_standardization/standardize.py` & `phc-ingestion-0.7.4/ingestion/vcf_standardization/standardize.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/vcf_standardization/util/af_helpers.py` & `phc-ingestion-0.7.4/ingestion/vcf_standardization/util/af_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/vcf_standardization/util/dp_helpers.py` & `phc-ingestion-0.7.4/ingestion/vcf_standardization/util/dp_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/ingestion/vcf_standardization/util/read_write.py` & `phc-ingestion-0.7.4/ingestion/vcf_standardization/util/read_write.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.3/pyproject.toml` & `phc-ingestion-0.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.7.3"
+version = "0.7.4"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

