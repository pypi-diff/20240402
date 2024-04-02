# Comparing `tmp/pheval_exomiser-0.2.0.tar.gz` & `tmp/pheval_exomiser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheval_exomiser-0.2.0.tar", max compression
+gzip compressed data, was "pheval_exomiser-0.2.1.tar", max compression
```

## Comparing `pheval_exomiser-0.2.0.tar` & `pheval_exomiser-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     5871 2024-02-19 10:14:01.262560 pheval_exomiser-0.2.0/README.md
--rw-r--r--   0        0        0     1199 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/__init__.py
--rw-r--r--   0        0        0      350 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/cli.py
--rw-r--r--   0        0        0      517 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/constants.py
--rw-r--r--   0        0        0        0 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/post_process/__init__.py
--rw-r--r--   0        0        0      901 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/post_process/post_process.py
--rw-r--r--   0        0        0    10410 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/post_process/post_process_results_format.py
--rw-r--r--   0        0        0        0 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/prepare/__init__.py
--rw-r--r--   0        0        0    16088 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/prepare/create_batch_commands.py
--rw-r--r--   0        0        0     2427 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/prepare/tool_specific_configuration_options.py
--rw-r--r--   0        0        0     8877 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/prepare/write_application_properties.py
--rw-r--r--   0        0        0    14452 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/prepare/yaml_to_family_phenopacket.py
--rw-r--r--   0        0        0        0 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/run/__init__.py
--rw-r--r--   0        0        0     6892 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/run/run.py
--rw-r--r--   0        0        0     2548 2024-02-19 10:14:01.266560 pheval_exomiser-0.2.0/src/pheval_exomiser/runner.py
--rw-r--r--   0        0        0     6684 1970-01-01 00:00:00.000000 pheval_exomiser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6246 2024-04-02 10:42:15.432924 pheval_exomiser-0.2.1/README.md
+-rw-r--r--   0        0        0     1199 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/__init__.py
+-rw-r--r--   0        0        0      350 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/cli.py
+-rw-r--r--   0        0        0      517 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/constants.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/post_process/__init__.py
+-rw-r--r--   0        0        0      901 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/post_process/post_process.py
+-rw-r--r--   0        0        0    12112 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/post_process/post_process_results_format.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/prepare/__init__.py
+-rw-r--r--   0        0        0    16190 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/prepare/create_batch_commands.py
+-rw-r--r--   0        0        0     2661 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/prepare/tool_specific_configuration_options.py
+-rw-r--r--   0        0        0     8933 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/prepare/write_application_properties.py
+-rw-r--r--   0        0        0    14452 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/prepare/yaml_to_family_phenopacket.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/run/__init__.py
+-rw-r--r--   0        0        0     6892 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/run/run.py
+-rw-r--r--   0        0        0     2548 2024-04-02 10:42:15.436924 pheval_exomiser-0.2.1/src/pheval_exomiser/runner.py
+-rw-r--r--   0        0        0     7059 1970-01-01 00:00:00.000000 pheval_exomiser-0.2.1/PKG-INFO
```

### Comparing `pheval_exomiser-0.2.0/README.md` & `pheval_exomiser-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,18 @@
   analysis_configuration_file: preset-exome-analysis.yml
   max_jobs: 0
   application_properties:
     remm_version:
     cadd_version:
     hg19_data_version: 2302
     hg19_local_frequency_path: # name of hg19 local frequency file 
+    hg19_whitelist_path: 2302_hg19_clinvar_whitelist.tsv.gz # only required for Exomiser v13.3.0 and earlier, can be left blank for Exomiser v14.0.0 onwards.
     hg38_data_version: 2302
     hg38_local_frequency_path: # name of hg38 local frequency file 
+    hg38_whitelist_path:
     phenotype_data_version: 2302
     cache_type:
     cache_caffeine_spec:
   post_process:
     score_name: combinedScore
     sort_order: DESCENDING
 ```
@@ -48,14 +50,16 @@
 
 The Exomiser input data directories (phenotype database and variant database) should also be located in the input directory - or a symlink pointing to the location.
 
 The `exomiser_software_directory` points to the name of the Exomiser distribution directory located in the input directory.
 
 The analysis configuration file (in this case: `preset-exome-analysis.yml`) should be located within the input directory.
 
+The whitelist paths for the hg19 and hg38 dbs need only be specified for Exomiser v13.3.0 and earlier (unless specifying your own whitelist), as Exomiser v14.0.0 now includes this in the db.
+
 If using optional databases, such as REMM/CADD/local frequency the optional data input should look like so in the input
 directory:
 
 ```tree
 ├── cadd
 │   └── {{CADD-VERSION}}
 │       ├── hg19
```

### Comparing `pheval_exomiser-0.2.0/pyproject.toml` & `pheval_exomiser-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pheval_exomiser"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Yasemin Bridges <y.bridges@qmul.ac.uk>",
     "Julius Jacobsen <j.jacobsen@qmul.ac.uk>",
     "Nico Matentzoglu <nicolas.matentzoglu@gmail.com>",
     "Vinícius de Souza <souzadevinicius@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "pheval_exomiser", from = "src" }]
```

### Comparing `pheval_exomiser-0.2.0/src/pheval_exomiser/constants.py` & `pheval_exomiser-0.2.1/src/pheval_exomiser/constants.py`

 * *Files identical despite different names*

### Comparing `pheval_exomiser-0.2.0/src/pheval_exomiser/post_process/post_process.py` & `pheval_exomiser-0.2.1/src/pheval_exomiser/post_process/post_process.py`

 * *Files identical despite different names*

### Comparing `pheval_exomiser-0.2.0/src/pheval_exomiser/post_process/post_process_results_format.py` & `pheval_exomiser-0.2.1/src/pheval_exomiser/post_process/post_process_results_format.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,14 +57,15 @@
                     )
                 )
 
         return simplified_exomiser_result
 
 
 class PhEvalVariantResultFromExomiserJsonCreator:
+
     def __init__(self, exomiser_json_result: [dict], score_name: str):
         self.exomiser_json_result = exomiser_json_result
         self.score_name = score_name
 
     @staticmethod
     def _find_chromosome(result_entry: dict) -> str:
         """Return chromosome from Exomiser result entry."""
@@ -93,33 +94,59 @@
         else:
             return ""
 
     def _find_relevant_score(self, result_entry) -> float:
         """Return score from Exomiser result entry."""
         return round(result_entry[self.score_name], 4)
 
-    def extract_pheval_variant_requirements(self) -> [PhEvalVariantResult]:
+    def _filter_for_acmg_assignments(
+        self, variant: PhEvalVariantResult, score: float, variant_acmg_assignments: dict
+    ) -> bool:
+        """Filter variants if they meet the PATHOGENIC or LIKELY_PATHOGENIC ACMG classification."""
+        for assignment in variant_acmg_assignments:
+            if variant == PhEvalVariantResult(
+                chromosome=self._find_chromosome(assignment["variantEvaluation"]),
+                start=self._find_start_pos(assignment["variantEvaluation"]),
+                end=self._find_end_pos(assignment["variantEvaluation"]),
+                ref=self._find_ref(assignment["variantEvaluation"]),
+                alt=self._find_alt(assignment["variantEvaluation"]),
+                score=score,
+            ) and (
+                assignment["acmgClassification"] == "PATHOGENIC"
+                or assignment["acmgClassification"] == "LIKELY_PATHOGENIC"
+            ):
+                return True
+
+    def extract_pheval_variant_requirements(
+        self, use_acmg_filter: bool = False
+    ) -> [PhEvalVariantResult]:
         """Extract data required to produce PhEval variant output."""
         simplified_exomiser_result = []
         for result_entry in self.exomiser_json_result:
             for gene_hit in result_entry["geneScores"]:
                 if self.score_name in result_entry:
                     if "contributingVariants" in gene_hit:
                         score = self._find_relevant_score(result_entry)
-                        for cv in gene_hit["contributingVariants"]:
-                            simplified_exomiser_result.append(
-                                PhEvalVariantResult(
-                                    chromosome=self._find_chromosome(cv),
-                                    start=self._find_start_pos(cv),
-                                    end=self._find_end_pos(cv),
-                                    ref=self._find_ref(cv),
-                                    alt=self._find_alt(cv),
-                                    score=score,
-                                )
+                        contributing_variants = gene_hit["contributingVariants"]
+                        variant_acmg_assignments = gene_hit["acmgAssignments"]
+                        for cv in contributing_variants:
+                            variant = PhEvalVariantResult(
+                                chromosome=self._find_chromosome(cv),
+                                start=self._find_start_pos(cv),
+                                end=self._find_end_pos(cv),
+                                ref=self._find_ref(cv),
+                                alt=self._find_alt(cv),
+                                score=score,
                             )
+                            if use_acmg_filter and self._filter_for_acmg_assignments(
+                                variant, score, variant_acmg_assignments
+                            ):
+                                simplified_exomiser_result.append(variant)
+                            if not use_acmg_filter:
+                                simplified_exomiser_result.append(variant)
         return simplified_exomiser_result
 
 
 class PhEvalDiseaseResultFromExomiserJsonCreator:
     def __init__(self, exomiser_json_result: [dict]):
         self.exomiser_json_result = exomiser_json_result
 
@@ -162,14 +189,15 @@
     results_dir: Path,
     output_dir: Path,
     score_name: str,
     sort_order: str,
     variant_analysis: bool,
     gene_analysis: bool,
     disease_analysis: bool,
+    include_acmg: bool = False,
 ) -> None:
     """Write standardised gene/variant/disease results from default Exomiser json output."""
     for exomiser_json_result in files_with_suffix(results_dir, ".json"):
         exomiser_result = read_exomiser_json_result(exomiser_json_result)
         if gene_analysis:
             pheval_gene_requirements = PhEvalGeneResultFromExomiserJsonCreator(
                 exomiser_result, score_name
@@ -179,15 +207,15 @@
                 sort_order_str=sort_order,
                 output_dir=output_dir,
                 tool_result_path=trim_exomiser_result_filename(exomiser_json_result),
             )
         if variant_analysis:
             pheval_variant_requirements = PhEvalVariantResultFromExomiserJsonCreator(
                 exomiser_result, score_name
-            ).extract_pheval_variant_requirements()
+            ).extract_pheval_variant_requirements(include_acmg)
             generate_pheval_result(
                 pheval_result=pheval_variant_requirements,
                 sort_order_str=sort_order,
                 output_dir=output_dir,
                 tool_result_path=trim_exomiser_result_filename(exomiser_json_result),
             )
         if disease_analysis:
@@ -251,22 +279,30 @@
 )
 @click.option(
     "--disease-analysis/--no-disease-analysis",
     type=bool,
     default=False,
     help="Specify whether to create PhEval disease results.",
 )
+@click.option(
+    "--include-acmg",
+    is_flag=True,
+    type=bool,
+    default=False,
+    help="Specify whether to include ACMG filter for PATHOGENIC or LIKELY_PATHOGENIC classifications.",
+)
 def post_process_exomiser_results(
     output_dir: Path,
     results_dir: Path,
     score_name: str,
     sort_order: str,
     gene_analysis: bool,
     variant_analysis: bool,
     disease_analysis: bool,
+    include_acmg: bool,
 ):
     """Post-process Exomiser json results into PhEval gene and variant outputs."""
     (
         output_dir.joinpath("pheval_gene_results").mkdir(parents=True, exist_ok=True)
         if gene_analysis
         else None
     )
@@ -284,8 +320,9 @@
         results_dir,
         output_dir,
         score_name,
         sort_order,
         variant_analysis,
         gene_analysis,
         disease_analysis,
+        include_acmg,
     )
```

### Comparing `pheval_exomiser-0.2.0/src/pheval_exomiser/prepare/create_batch_commands.py` & `pheval_exomiser-0.2.1/src/pheval_exomiser/prepare/create_batch_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,14 +178,16 @@
                 + str(command_arguments.analysis_yaml)
                 + " --sample "
                 + str(command_arguments.sample)
                 + " --vcf "
                 + str(command_arguments.vcf_file)
                 + " --assembly "
                 + command_arguments.vcf_assembly
+                + " --output-filename "
+                + f"{command_arguments.sample.stem}-exomiser"
             )
         except IOError:
             print("Error writing ", self.file)
 
     def write_results_dir(self, command_arguments: ExomiserCommandLineArguments) -> None:
         """Write results directory for exomiser ≥13.2.0 to run."""
         try:
```

### Comparing `pheval_exomiser-0.2.0/src/pheval_exomiser/prepare/tool_specific_configuration_options.py` & `pheval_exomiser-0.2.1/src/pheval_exomiser/prepare/tool_specific_configuration_options.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,26 +7,30 @@
     """
     Class for defining the application.properties configurations.
     Args:
         remm_version (str): Version of the REMM database
         cadd_version (str): Version of the CADD database
         hg19_data_version (str): Data version of the hg19 Exomiser data
         hg19_local_frequency_path (Path): The file name of the hg19 local frequency file
+        hg19_whitelist_path (Path): The file name of the hg19 whitelist.
         hg38_data_version (str): Data version of the hg38 Exomiser data
         hg38_local_frequency_path (Path): The file name of the hg38 local frequency file
+        hg38_whitelist_path (Path): The file name of the hg38 whitelist.
         phenotype_data_version (str): Data version of the Exomiser phenotype data
         cache_caffeine_spec (int): Cache limit
     """
 
     remm_version: str = Field(None)
     cadd_version: str = Field(None)
     hg19_data_version: str = Field(None)
     hg19_local_frequency_path: Path = Field(None)
+    hg19_whitelist_path: Path = Field(None)
     hg38_data_version: str = Field(None)
     hg38_local_frequency_path: Path = Field(None)
+    hg38_whitelist_path: Path = Field(None)
     phenotype_data_version: str = Field(None)
     cache_type: str = Field(None)
     cache_caffeine_spec: int = Field(None)
 
 
 class PostProcessing(BaseModel):
     """
```

### Comparing `pheval_exomiser-0.2.0/src/pheval_exomiser/prepare/write_application_properties.py` & `pheval_exomiser-0.2.1/src/pheval_exomiser/prepare/write_application_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,24 +140,26 @@
         """Write the phenotype data version to application.properties file."""
         self.application_properties.write(
             f"exomiser.phenotype.data-version={self.configurations.application_properties.phenotype_data_version}\n"
         )
 
     def write_hg19_white_list_path(self) -> None:
         """Write the hg19 whitelist path to application.properties file."""
-        if self.configurations.application_properties.hg19_data_version is not None:
+        if self.configurations.application_properties.hg19_whitelist_path is not None:
             self.application_properties.write(
-                "exomiser.hg19.variant-white-list-path=${exomiser.hg19.data-version}_hg19_clinvar_whitelist.tsv.gz\n"
+                f"exomiser.hg19.variant-white-list-path="
+                f"{self.configurations.application_properties.hg19_whitelist_path}\n"
             )
 
     def write_hg38_white_list_path(self) -> None:
         """Write the hg38 whitelist path to application.properties file."""
-        if self.configurations.application_properties.hg38_data_version is not None:
+        if self.configurations.application_properties.hg38_whitelist_path is not None:
             self.application_properties.write(
-                "exomiser.hg38.variant-white-list-path=${exomiser.hg38.data-version}_hg38_clinvar_whitelist.tsv.gz\n"
+                f"exomiser.hg38.variant-white-list-path="
+                f"{self.configurations.application_properties.hg38_whitelist_path}\n"
             )
 
     def write_cache_type(self):
         """Write the cache type to application.properties file."""
         if self.configurations.application_properties.cache_type is not None:
             self.application_properties.write(
                 f"spring.cache.type=" f"{self.configurations.application_properties.cache_type}\n"
```

### Comparing `pheval_exomiser-0.2.0/src/pheval_exomiser/prepare/yaml_to_family_phenopacket.py` & `pheval_exomiser-0.2.1/src/pheval_exomiser/prepare/yaml_to_family_phenopacket.py`

 * *Files identical despite different names*

### Comparing `pheval_exomiser-0.2.0/src/pheval_exomiser/run/run.py` & `pheval_exomiser-0.2.1/src/pheval_exomiser/run/run.py`

 * *Files identical despite different names*

### Comparing `pheval_exomiser-0.2.0/src/pheval_exomiser/runner.py` & `pheval_exomiser-0.2.1/src/pheval_exomiser/runner.py`

 * *Files identical despite different names*

### Comparing `pheval_exomiser-0.2.0/PKG-INFO` & `pheval_exomiser-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheval_exomiser
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Yasemin Bridges
 Author-email: y.bridges@qmul.ac.uk
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -54,16 +54,18 @@
   analysis_configuration_file: preset-exome-analysis.yml
   max_jobs: 0
   application_properties:
     remm_version:
     cadd_version:
     hg19_data_version: 2302
     hg19_local_frequency_path: # name of hg19 local frequency file 
+    hg19_whitelist_path: 2302_hg19_clinvar_whitelist.tsv.gz # only required for Exomiser v13.3.0 and earlier, can be left blank for Exomiser v14.0.0 onwards.
     hg38_data_version: 2302
     hg38_local_frequency_path: # name of hg38 local frequency file 
+    hg38_whitelist_path:
     phenotype_data_version: 2302
     cache_type:
     cache_caffeine_spec:
   post_process:
     score_name: combinedScore
     sort_order: DESCENDING
 ```
@@ -71,14 +73,16 @@
 
 The Exomiser input data directories (phenotype database and variant database) should also be located in the input directory - or a symlink pointing to the location.
 
 The `exomiser_software_directory` points to the name of the Exomiser distribution directory located in the input directory.
 
 The analysis configuration file (in this case: `preset-exome-analysis.yml`) should be located within the input directory.
 
+The whitelist paths for the hg19 and hg38 dbs need only be specified for Exomiser v13.3.0 and earlier (unless specifying your own whitelist), as Exomiser v14.0.0 now includes this in the db.
+
 If using optional databases, such as REMM/CADD/local frequency the optional data input should look like so in the input
 directory:
 
 ```tree
 ├── cadd
 │   └── {{CADD-VERSION}}
 │       ├── hg19
```

