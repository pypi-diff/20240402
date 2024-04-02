# Comparing `tmp/immunopipe-1.3.2.tar.gz` & `tmp/immunopipe-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immunopipe-1.3.2.tar", max compression
+gzip compressed data, was "immunopipe-1.3.3.tar", max compression
```

## Comparing `immunopipe-1.3.2.tar` & `immunopipe-1.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35128 2024-03-19 20:16:18.819907 immunopipe-1.3.2/LICENSE
--rw-r--r--   0        0        0     1448 2024-03-19 20:16:18.819907 immunopipe-1.3.2/README.md
--rw-r--r--   0        0        0      143 2024-03-19 20:16:18.871907 immunopipe-1.3.2/immunopipe/__init__.py
--rw-r--r--   0        0        0      109 2024-03-19 20:16:18.871907 immunopipe-1.3.2/immunopipe/__main__.py
--rw-r--r--   0        0        0     7461 2024-03-19 20:16:18.871907 immunopipe-1.3.2/immunopipe/inhouse.py
--rw-r--r--   0        0        0      503 2024-03-19 20:16:18.871907 immunopipe-1.3.2/immunopipe/pipeline.py
--rw-r--r--   0        0        0    32543 2024-03-19 20:16:18.871907 immunopipe-1.3.2/immunopipe/processes.py
--rw-r--r--   0        0        0     1581 2024-03-19 20:16:18.871907 immunopipe-1.3.2/immunopipe/reports/CloneHeterogeneity.svelte
--rw-r--r--   0        0        0      683 2024-03-19 20:16:18.871907 immunopipe-1.3.2/immunopipe/reports/MarkersOverlapping.svelte
--rw-r--r--   0        0        0      101 2024-03-19 20:16:18.871907 immunopipe-1.3.2/immunopipe/reports/TCellSelection.svelte
--rw-r--r--   0        0        0     4769 2024-03-19 20:16:18.875907 immunopipe-1.3.2/immunopipe/scripts/CloneHeterogeneity.R
--rw-r--r--   0        0        0     2029 2024-03-19 20:16:18.875907 immunopipe-1.3.2/immunopipe/scripts/MarkersOverlapping.R
--rw-r--r--   0        0        0    15647 2024-03-19 20:16:18.875907 immunopipe-1.3.2/immunopipe/scripts/TCellSelection.R
--rw-r--r--   0        0        0     3281 2024-03-19 20:16:18.875907 immunopipe-1.3.2/immunopipe/validate_config.py
--rw-r--r--   0        0        0       22 2024-03-19 20:16:18.875907 immunopipe-1.3.2/immunopipe/version.py
--rw-r--r--   0        0        0     1107 2024-03-19 20:16:18.875907 immunopipe-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 immunopipe-1.3.2/setup.py
--rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 immunopipe-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-04-02 18:59:56.146269 immunopipe-1.3.3/LICENSE
+-rw-r--r--   0        0        0     1448 2024-04-02 18:59:56.146269 immunopipe-1.3.3/README.md
+-rw-r--r--   0        0        0      143 2024-04-02 18:59:56.198269 immunopipe-1.3.3/immunopipe/__init__.py
+-rw-r--r--   0        0        0      109 2024-04-02 18:59:56.198269 immunopipe-1.3.3/immunopipe/__main__.py
+-rw-r--r--   0        0        0     7461 2024-04-02 18:59:56.198269 immunopipe-1.3.3/immunopipe/inhouse.py
+-rw-r--r--   0        0        0      503 2024-04-02 18:59:56.198269 immunopipe-1.3.3/immunopipe/pipeline.py
+-rw-r--r--   0        0        0    32543 2024-04-02 18:59:56.202269 immunopipe-1.3.3/immunopipe/processes.py
+-rw-r--r--   0        0        0     1581 2024-04-02 18:59:56.202269 immunopipe-1.3.3/immunopipe/reports/CloneHeterogeneity.svelte
+-rw-r--r--   0        0        0      683 2024-04-02 18:59:56.202269 immunopipe-1.3.3/immunopipe/reports/MarkersOverlapping.svelte
+-rw-r--r--   0        0        0      101 2024-04-02 18:59:56.202269 immunopipe-1.3.3/immunopipe/reports/TCellSelection.svelte
+-rw-r--r--   0        0        0     4769 2024-04-02 18:59:56.202269 immunopipe-1.3.3/immunopipe/scripts/CloneHeterogeneity.R
+-rw-r--r--   0        0        0     2029 2024-04-02 18:59:56.202269 immunopipe-1.3.3/immunopipe/scripts/MarkersOverlapping.R
+-rw-r--r--   0        0        0    15647 2024-04-02 18:59:56.202269 immunopipe-1.3.3/immunopipe/scripts/TCellSelection.R
+-rw-r--r--   0        0        0     3281 2024-04-02 18:59:56.202269 immunopipe-1.3.3/immunopipe/validate_config.py
+-rw-r--r--   0        0        0       22 2024-04-02 18:59:56.202269 immunopipe-1.3.3/immunopipe/version.py
+-rw-r--r--   0        0        0     1181 2024-04-02 18:59:56.202269 immunopipe-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2487 1970-01-01 00:00:00.000000 immunopipe-1.3.3/setup.py
+-rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 immunopipe-1.3.3/PKG-INFO
```

### Comparing `immunopipe-1.3.2/LICENSE` & `immunopipe-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.2/README.md` & `immunopipe-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.2/immunopipe/inhouse.py` & `immunopipe-1.3.3/immunopipe/inhouse.py`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.2/immunopipe/processes.py` & `immunopipe-1.3.3/immunopipe/processes.py`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.2/immunopipe/reports/CloneHeterogeneity.svelte` & `immunopipe-1.3.3/immunopipe/reports/CloneHeterogeneity.svelte`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.2/immunopipe/reports/MarkersOverlapping.svelte` & `immunopipe-1.3.3/immunopipe/reports/MarkersOverlapping.svelte`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.2/immunopipe/scripts/CloneHeterogeneity.R` & `immunopipe-1.3.3/immunopipe/scripts/CloneHeterogeneity.R`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.2/immunopipe/scripts/MarkersOverlapping.R` & `immunopipe-1.3.3/immunopipe/scripts/MarkersOverlapping.R`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.2/immunopipe/scripts/TCellSelection.R` & `immunopipe-1.3.3/immunopipe/scripts/TCellSelection.R`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.2/immunopipe/validate_config.py` & `immunopipe-1.3.3/immunopipe/validate_config.py`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.2/pyproject.toml` & `immunopipe-1.3.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "immunopipe"
 description = "A pipeline for integrative analysis for scTCR- and scRNA-seq data"
 authors = [ "pwwang <pwwang@pwwang.com>",]
-version = "1.3.2"
+version = "1.3.3"
 license = "GNU General Public License v3.0"
 readme = "README.md"
 homepage = "https://github.com/pwwang/immunopipe"
 repository = "https://github.com/pwwang/immunopipe"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pipen-diagram = { version = "^0.11", optional = true }
 pipen-runinfo = { version = "^0.6", optional = true }
+pyyaml-include = "1.*" # https://github.com/copier-org/copier/issues/1568
 # pipen-report and pipen-board are required by biopipen
-biopipen = "^0.27.1"
+biopipen = "^0.27.2"
 
 [tool.poetry.extras]
 diagram = ["pipen-diagram"]
 runinfo = ["pipen-runinfo"]
 
 [tool.poetry.group.docs.dependencies]
 pipen-cli-ref = "^0.3"
```

### Comparing `immunopipe-1.3.2/setup.py` & `immunopipe-1.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 packages = \
 ['immunopipe']
 
 package_data = \
 {'': ['*'], 'immunopipe': ['reports/*', 'scripts/*']}
 
 install_requires = \
-['biopipen>=0.27.1,<0.28.0']
+['biopipen>=0.27.2,<0.28.0', 'pyyaml-include==1.*']
 
 extras_require = \
 {'diagram': ['pipen-diagram>=0.11,<0.12'],
  'runinfo': ['pipen-runinfo>=0.6,<0.7']}
 
 entry_points = \
 {'console_scripts': ['immunopipe = immunopipe.pipeline:main']}
 
 setup_kwargs = {
     'name': 'immunopipe',
-    'version': '1.3.2',
+    'version': '1.3.3',
     'description': 'A pipeline for integrative analysis for scTCR- and scRNA-seq data',
     'long_description': '<p align="center">\n  <img height="120" style="height: 120px" src="https://github.com/pwwang/immunopipe/blob/dev/docs/logo.png?raw=true" />\n</p>\n<p align="center">Integrative analysis for single-cell RNA sequencing and single-cell TCR sequencing data</p>\n<hr />\n\n`immunopipe` is a pipeline based on [`pipen`](https://github.com/pwwang/pipen) framework. It includes a set of processes for scTCR- and scRNA-seq data analysis in `R`, `python` and `bash`. The pipeline is designed to be flexible and configurable.\n\n<p align="center">\n  <img src="https://github.com/pwwang/immunopipe/blob/dev/docs/immunopipe.ms.png?raw=true" />\n</p>\n\nSee a more detailed flowchart [here](https://github.com/pwwang/immunopipe/blob/dev/docs/immunopipe.flowchart.png?raw=true).\n\n## Documentaion\n\n[https://pwwang.github.io/immunopipe](https://pwwang.github.io/immunopipe)\n\n## Proposing more analyses\n\nIf you have any suggestions for more analyses, please feel free to open an issue [here](https://github.com/pwwang/immunopipe/issues/new)\n\n## Example\n\n[https://github.com/pwwang/immunopipe-example](https://github.com/pwwang/immunopipe-example)\n\n## Gallery\n\nThere are some datasets with both scRNA-seq and scTCR-seq data available in the publications. The data were reanalyzed using `immunopipe` with the configurations provided in each repository, where the results are also available.\n\nCheck out the [gallery](https://pwwang.github.io/immunopipe/gallery) for more details.\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/immunopipe',
```

### Comparing `immunopipe-1.3.2/PKG-INFO` & `immunopipe-1.3.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: immunopipe
-Version: 1.3.2
+Version: 1.3.3
 Summary: A pipeline for integrative analysis for scTCR- and scRNA-seq data
 Home-page: https://github.com/pwwang/immunopipe
 License: GNU General Public License v3.0
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: diagram
 Provides-Extra: runinfo
-Requires-Dist: biopipen (>=0.27.1,<0.28.0)
+Requires-Dist: biopipen (>=0.27.2,<0.28.0)
 Requires-Dist: pipen-diagram (>=0.11,<0.12) ; extra == "diagram"
 Requires-Dist: pipen-runinfo (>=0.6,<0.7) ; extra == "runinfo"
+Requires-Dist: pyyaml-include (==1.*)
 Project-URL: Repository, https://github.com/pwwang/immunopipe
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img height="120" style="height: 120px" src="https://github.com/pwwang/immunopipe/blob/dev/docs/logo.png?raw=true" />
 </p>
 <p align="center">Integrative analysis for single-cell RNA sequencing and single-cell TCR sequencing data</p>
```

