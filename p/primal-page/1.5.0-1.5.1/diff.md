# Comparing `tmp/primal_page-1.5.0.tar.gz` & `tmp/primal_page-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primal_page-1.5.0.tar", max compression
+gzip compressed data, was "primal_page-1.5.1.tar", max compression
```

## Comparing `primal_page-1.5.0.tar` & `primal_page-1.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    16507 2024-03-29 17:51:43.993609 primal_page-1.5.0/README.md
--rw-r--r--   0        0        0       22 2024-03-29 17:57:29.405159 primal_page-1.5.0/primal_page/__init__.py
--rw-r--r--   0        0        0     6457 2024-03-28 12:37:49.209826 primal_page-1.5.0/primal_page/bedfiles.py
--rw-r--r--   0        0        0     8570 2024-03-28 12:36:56.862086 primal_page-1.5.0/primal_page/build_index.py
--rw-r--r--   0        0        0     3106 2024-03-28 12:28:04.284143 primal_page-1.5.0/primal_page/download.py
--rw-r--r--   0        0        0    28125 2024-03-29 17:57:10.155442 primal_page-1.5.0/primal_page/main.py
--rw-r--r--   0        0        0     1790 2024-03-28 14:11:51.480952 primal_page-1.5.0/primal_page/modify.py
--rw-r--r--   0        0        0     5574 2024-03-29 09:47:36.111159 primal_page-1.5.0/primal_page/schemas.py
--rw-r--r--   0        0        0      892 2024-03-29 17:52:38.239864 primal_page-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    16973 1970-01-01 00:00:00.000000 primal_page-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    17347 2024-04-01 22:08:40.025579 primal_page-1.5.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-01 22:09:43.252047 primal_page-1.5.1/primal_page/__init__.py
+-rw-r--r--   0        0        0     6457 2024-03-28 12:37:49.209826 primal_page-1.5.1/primal_page/bedfiles.py
+-rw-r--r--   0        0        0     8570 2024-03-28 12:36:56.862086 primal_page-1.5.1/primal_page/build_index.py
+-rw-r--r--   0        0        0     3106 2024-03-28 12:28:04.284143 primal_page-1.5.1/primal_page/download.py
+-rw-r--r--   0        0        0    28125 2024-04-01 21:00:06.373740 primal_page-1.5.1/primal_page/main.py
+-rw-r--r--   0        0        0     1959 2024-04-01 21:15:05.696388 primal_page-1.5.1/primal_page/modify.py
+-rw-r--r--   0        0        0     5574 2024-03-29 09:47:36.111159 primal_page-1.5.1/primal_page/schemas.py
+-rw-r--r--   0        0        0      996 2024-04-01 22:09:34.860450 primal_page-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0    17980 1970-01-01 00:00:00.000000 primal_page-1.5.1/PKG-INFO
```

### Comparing `primal_page-1.5.0/README.md` & `primal_page-1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,207 @@
 # Primal-Page
 
 [![CI](https://github.com/ChrisgKent/primal-page/actions/workflows/pytest.yml/badge.svg)](https://github.com/ChrisgKent/primal-page/actions/workflows/pytest.yml)
 
 
-This is the tooling for working with the primerschemes index
+Tooling and schemas for the primerschemes index
 
 ## Contents
 
-[cli](https://github.com/ChrisgKent/primal-page?tab=readme-ov-file#cli)
+[Installation](https://github.com/ChrisgKent/primal-page?tab=readme-ov-file#installation)
 
-[schemas](https://github.com/ChrisgKent/primal-page?tab=readme-ov-file#new-schemas)
+[Quick Start](https://github.com/ChrisgKent/primal-page?tab=readme-ov-file#quick-start)
+
+[Schemas](https://github.com/ChrisgKent/primal-page?tab=readme-ov-file#new-schemas)
+
+[CLI](https://github.com/ChrisgKent/primal-page?tab=readme-ov-file#cli)
+
+# Installation
+
+```
+pip install primal-page
+```
+
+# Quick Start
+
+Each version of a primerscheme has three parts; `{schemename}/{ampliconsize}/{version}`, which when combined these form the schemes unique identifier.
+
+For a scheme to be added to the repo it requires three essental files. 
+- `primer.bed`: Contains the primer infomation.   
+- `reference.fasta`: Contains the reference genomes.
+- `info.json`: Contains key metadata for the scheme.
+
+The `primal-page create` command will generates the `info.json` and parses a bed file and a fasta file into `primer.bed` and `reference.fasta`
+
+Additional files are copied into the schemes work directory. 
+
+## Example
+### Adding a minimal scheme
+
+For a simple scheme, only fasta file (--reference) and a bed file (--primerbed) are required. Alongside metadata of --schemename, --algorithmversion, --species, --authors.
+
+```
+primal-page create \
+    --schemename example-scheme \
+    --algorithmversion ps:100 \
+    --ampliconsize 500 \
+    --species 123  \
+    --schemeversion v1.0.0 \
+    --primerbed ~/'minimal-scheme/minimal.bed' \
+    --reference '~/minimal-scheme/ref.fasta' \
+    --authors "me" \
+    --authors "you" /
+    '~/minimal-scheme' 
+```
+
+### Adding a custom scheme to quick-lab/primerschemes
+
+
+> create a local fork of https://github.com/quick-lab/primerschemes
+
+> Add the files to the forks primerschemes folder
+```
+primal-page create primal-page create ... --output ~/primerschemes/primerschemes
+```
+
+> Create a pull request 
+
+
+# New Schemas
+
+## info.json
+
+This is the main metadata file for each primerscheme.
+
+- `ampliconsize`: PositiveInt
+- `schemeversion`: Following format listed below
+- `schemename`: Following format listed below
+- `primer_bed_md5`: MD5 hash of the schemes primer.bed file
+- `reference_fasta_md5`: MD5 hash of the schemes reference.fasta file
+- `status`: 
+    - `withdrawn`: Removed due to major issue
+    - `deprecated`: Newer scheme is recommended
+    - `autogenerated`: Scheme has been autogenerated using species-agnostic pipelines
+    - `draft`: Scheme has been inspected in silico
+    - `tested`: Scheme has been tested in the laboratory
+    - `validated`: Scheme has been validated and/or published
+- `citations`: How the scheme should be cited if used. DOI links are recommended, however, tweets/blogs are all allowed
+- `authors`: The person or organisation who generated the scheme. It is recommended that only corresponding/primary authors are included, with all other contributors recognised in the `citations` field
+- `algorithmversion`: The algorithm and the version used to generate the scheme
+- `species`: A list of organisms targeted by this scheme. NCBI TaxIds are recommend
+- `license`: The name of the license the primerscheme is offered under
+- `primerclass`: The class of scheme. Only `primerscheme` at the moment
+- `infoschema`: The version of the info.json 
+- `articbedversion`: The version of the primer.bed (See below)
+- `description`: A free text description to describe the primerscheme
+- `derivedfrom`: To show if this scheme has been based on another primerscheme. 
+- `collections`: A collection of vocab to provide filtering/grouping of schemes.
+    - `ARTIC`: Developed with the ARTIC network
+    - `MODJADJI`: Developed with MODJADJI
+    - `QUICK-LAB`: Developed with QUICK-LAB
+    - `COMMUNITY`: Developed by the COMMUNITY
+    - `WASTE-WATER`: Scheme capable of recovering genomes from high Ct samples (~30) samples, like wastewater. Typically 400bp schemes
+    - `CLINAL-ISOLATES`: Scheme capable of recovering genomes from medium Ct samples (~25) samples.  Typically ~1000bp schemes
+    - `WHOLE-GENOME`: Scheme that can theoretically recover a full genome
+    - `PANEL`: Scheme that can recover sections of a target genome
+    - `MULTI-TARGET`: Scheme that contains more than one target
+
+## PrimerNames Versions
+
+Expected primernames (col3) in the primer.bed file
+
+### `V1`
+
+This is the first standard for primernames. It follows the general pattern of `{scheme-name|uuid}_{amplicon-number}_{LEFT|RIGHT}` and an optional `{_alt}` to denote spike in primers.
+
+Regex:
+
+ ```V1_PRIMERNAME = r"^[a-zA-Z0-9\-]+_[0-9]+_(LEFT|RIGHT)(_ALT[0-9]*|_alt[0-9]*)*$"```
+
+Example:
+```
+SARS-CoV-2_10_LEFT
+SARS-CoV-2_10_LEFT_alt1
+```
+
+
+### `V2`
+
+This follows the pattern of `{scheme-name|uuid}_{amplicon-number}_{LEFT|RIGHT}_{primer-number}`. 
+- This now enforces that splitting on `_` will produce a consistent length, allowing the safe indexing of attributes. 
+- `primer-number` is not enforced to be continuous. Therefore, the `_0` numbered primer should not be thought of as the `original` and all other numbers as `alts`.
+
+
+Example:
+```
+SARS-CoV-2_10_LEFT_0
+SARS-CoV-2_10_LEFT_1
+```
+
+Regex:
+
+```V2_PRIMERNAME = r"^[a-zA-Z0-9\-]+_[0-9]+_(LEFT|RIGHT)_[0-9]+$"```
+
+
+## ARTIC-primer.bed Versions
+
+These are rough guidelines for the format of the primer.bed file. The general format is based on the [.bed file](https://en.wikipedia.org/wiki/BED_(file_format)) and maintains compatibility with other tools.
+
+colnames and indexes:
+- `0 - chrom`: The name of the reference genome the primers are indexed to
+- `1 - chromStart`: 0-based inclusive start coordinate
+- `2 - chromEnd`: 0-based non-inclusive end coordinate
+- `3 - primer-name`: Name of each primer
+- `4 - pool`: The pool each primer should be added into. 1 based.
+- `5 - strand`: Either `+` (forward) or `-` (reverse) primer
+- `6 - primer-sequence`: The 5'-3' sequence of the primer
+
+
+
+### V1
+> Depreciated 
+
+This was the original 6-col bedfile used very early in PrimalSchemes development, which excluded primer-sequence. 
+
+### V2
+> Legacy
+
+This uses the 7 columns described above, alongside `V1:primernames`.
+- Single chrom (reference) is expected
+- No header lines
+
+### V3
+> Current
+
+This uses the 7 columns described above, alongside `V2:primernames`.
+- Multiple chrom (references)
+- Circular primers are allowed. The start of x_LEFT can be greater than the end of x_RIGHT
+- Header lines are used. Denoted with the `#` character 
+
+ 
+## Scheme Version
+
+In the form of `v{Major}.{Minor}.{Patch}`
+- Major: New scheme being generated with differant input params
+- Minor: Change to primers. Either additional / removal of primers
+- Patch: No change to primers. Often used for rebalancing or change in formatting
+
+
+Regex:
+
+`VERSION_PATTERN = r"^v\d+\.\d+\.\d+$"`
+
+
+## Scheme Name
+
+Must only contain `a-z`, `0-9`, and `-`. Cannot start or end with `-`
+
+Regex:
+
+`SCHEMENAME_PATTERN = r"^[a-z0-9][a-z0-9-]*[a-z0-9]$"`
 
 # CLI
 
 **Usage**:
 
 ```console
 $ [OPTIONS] COMMAND [ARGS]...
@@ -423,172 +611,8 @@
 
 * `SCHEMEINFO`: The path to info.json  [required]
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
-# Examples
-
-### Adding a minimal scheme
-
-For a simple scheme, only fasta file (--reference) and a bed file (--primerbed) are required. Alongside metadata of --schemename, --algorithmversion, --species, --authors.
-
-```
-primal-page create \
-    --schemename example-scheme \
-    --algorithmversion ps:100 \
-    --ampliconsize 500 \
-    --species 123  \
-    --schemeversion v1.0.0 \
-    --primerbed 'minimal-scheme/minimal.bed' \
-    --reference 'minimal-scheme/ref.fasta' \
-    --authors me \
-    --authors you /
-    'minimal-scheme' 
-```
-
-### Adding a custom scheme to quick-lab/primerschemes
-
-
-> create a local fork of https://github.com/quick-lab/primerschemes
-
-> Add the files to the forks primerschemes folder
-```
-primal-page create primal-page create ... --output ~/primerschemes/primerschemes
-```
-
-> Create a pull request 
-
-
-# New Schemas
-
-## info.json
-
-This is the main metadata file for each primerscheme.
-
-- `ampliconsize`: PositiveInt
-- `schemeversion`: Following format listed below
-- `schemename`: Following format listed below
-- `primer_bed_md5`: MD5 hash of the schemes primer.bed file
-- `reference_fasta_md5`: MD5 hash of the schemes reference.fasta file
-- `status`: 
-    - `withdrawn`: Removed due to major issue
-    - `deprecated`: Newer scheme is recommended
-    - `autogenerated`: Scheme has been autogenerated using species-agnostic pipelines
-    - `draft`: Scheme has been inspected in silico
-    - `tested`: Scheme has been tested in the laboratory
-    - `validated`: Scheme has been validated and/or published
-- `citations`: How the scheme should be cited if used. DOI links are recommended, however, tweets/blogs are all allowed
-- `authors`: The person or organisation who generated the scheme. It is recommended that only corresponding/primary authors are included, with all other contributors recognised in the `citations` field
-- `algorithmversion`: The algorithm and the version used to generate the scheme
-- `species`: A list of organisms targeted by this scheme. NCBI TaxIds are recommend
-- `license`: The name of the license the primerscheme is offered under
-- `primerclass`: The class of scheme. Only `primerscheme` at the moment
-- `infoschema`: The version of the info.json 
-- `articbedversion`: The version of the primer.bed (See below)
-- `description`: A free text description to describe the primerscheme
-- `derivedfrom`: To show if this scheme has been based on another primerscheme. 
-- `collections`: A collection of vocab to provide filtering/grouping of schemes.
-    - `ARTIC`: Developed with the ARTIC network
-    - `MODJADJI`: Developed with MODJADJI
-    - `QUICK-LAB`: Developed with QUICK-LAB
-    - `COMMUNITY`: Developed by the COMMUNITY
-    - `WASTE-WATER`: Scheme capable of recovering genomes from high Ct samples (~30) samples, like wastewater. Typically 400bp schemes
-    - `CLINAL-ISOLATES`: Scheme capable of recovering genomes from medium Ct samples (~25) samples.  Typically ~1000bp schemes
-    - `WHOLE-GENOME`: Scheme that can theoretically recover a full genome
-    - `PANEL`: Scheme that can recover sections of a target genome
-    - `MULTI-TARGET`: Scheme that contains more than one target
-
-## PrimerNames Versions
-
-Expected primernames (col3) in the primer.bed file
-
-### `V1`
-
-This is the first standard for primernames. It follows the general pattern of `{scheme-name|uuid}_{amplicon-number}_{LEFT|RIGHT}` and an optional `{_alt}` to denote spike in primers.
-
-Regex:
-
- ```V1_PRIMERNAME = r"^[a-zA-Z0-9\-]+_[0-9]+_(LEFT|RIGHT)(_ALT[0-9]*|_alt[0-9]*)*$"```
-
-Example:
-```
-SARS-CoV-2_10_LEFT
-SARS-CoV-2_10_LEFT_alt1
-```
-
-
-### `V2`
-
-This follows the pattern of `{scheme-name|uuid}_{amplicon-number}_{LEFT|RIGHT}_{primer-number}`. 
-- This now enforces that splitting on `_` will produce a consistent length, allowing the safe indexing of attributes. 
-- `primer-number` is not enforced to be continuous. Therefore, the `_0` numbered primer should not be thought of as the `original` and all other numbers as `alts`.
-
-
-Example:
-```
-SARS-CoV-2_10_LEFT_0
-SARS-CoV-2_10_LEFT_1
-```
-
-Regex:
-
-```V2_PRIMERNAME = r"^[a-zA-Z0-9\-]+_[0-9]+_(LEFT|RIGHT)_[0-9]+$"```
-
-
-## ARTIC-primer.bed Versions
-
-These are rough guidelines for the format of the primer.bed file. The general format is based on the [.bed file](https://en.wikipedia.org/wiki/BED_(file_format)) and maintains compatibility with other tools.
-
-colnames and indexes:
-- `0 - chrom`: The name of the reference genome the primers are indexed to
-- `1 - chromStart`: 0-based inclusive start coordinate
-- `2 - chromEnd`: 0-based non-inclusive end coordinate
-- `3 - primer-name`: Name of each primer
-- `4 - pool`: The pool each primer should be added into. 1 based.
-- `5 - strand`: Either `+` (forward) or `-` (reverse) primer
-- `6 - primer-sequence`: The 5'-3' sequence of the primer
-
-
-
-### V1
-> Depreciated 
-
-This was the original 6-col bedfile used very early in PrimalSchemes development, which excluded primer-sequence. 
-
-### V2
-> Legacy
-
-This uses the 7 columns described above, alongside `V1:primernames`.
-- Single chrom (reference) is expected
-- No header lines
-
-### V3
-> Current
-
-This uses the 7 columns described above, alongside `V2:primernames`.
-- Multiple chrom (references)
-- Circular primers are allowed. The start of x_LEFT can be greater than the end of x_RIGHT
-- Header lines are used. Denoted with the `#` character 
-
- 
-## Scheme Version
-
-In the form of `v{Major}.{Minor}.{Patch}`
-- Major: New scheme being generated with differant input params
-- Minor: Change to primers. Either additional / removal of primers
-- Patch: No change to primers. Often used for rebalancing or change in formatting
-
-
-Regex:
-
-`VERSION_PATTERN = r"^v\d+\.\d+\.\d+$"`
-
-
-## Scheme Name
-
-Must only contain `a-z`, `0-9`, and `-`. Cannot start or end with `-`
-
-Regex:
-
-`SCHEMENAME_PATTERN = r"^[a-z0-9][a-z0-9-]*[a-z0-9]$"`
+# Examples
```

### Comparing `primal_page-1.5.0/primal_page/bedfiles.py` & `primal_page-1.5.1/primal_page/bedfiles.py`

 * *Files identical despite different names*

### Comparing `primal_page-1.5.0/primal_page/build_index.py` & `primal_page-1.5.1/primal_page/build_index.py`

 * *Files identical despite different names*

### Comparing `primal_page-1.5.0/primal_page/download.py` & `primal_page-1.5.1/primal_page/download.py`

 * *Files identical despite different names*

### Comparing `primal_page-1.5.0/primal_page/main.py` & `primal_page-1.5.1/primal_page/main.py`

 * *Files identical despite different names*

### Comparing `primal_page-1.5.0/primal_page/modify.py` & `primal_page-1.5.1/primal_page/modify.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,18 @@
     """
 
     with open(path / "README.md", "w") as readme:
         readme.write(
             f"# {info.schemename} {info.ampliconsize}bp {info.schemeversion}\n\n"
         )
 
+        readme.write(
+            f"[primalscheme labs](https://labs.primalscheme.com/detail/{info.schemename}/{info.ampliconsize}/{info.schemeversion})\n\n"
+        )
+
         if info.description is not None:
             readme.write("## Description\n\n")
             readme.write(f"{info.description}\n\n")
 
         readme.write("## Overviews\n\n")
         for png in pngs:
             readme.write(f"![{png.name}](work/{png.name})\n\n")
```

### Comparing `primal_page-1.5.0/primal_page/schemas.py` & `primal_page-1.5.1/primal_page/schemas.py`

 * *Files identical despite different names*

### Comparing `primal_page-1.5.0/pyproject.toml` & `primal_page-1.5.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "primal-page"
-version = "1.5.0"
-description = ""
+version = "1.5.1"
+description = "Tooling and schemas for the primerschemes index"
 authors = ["ChrisKent <chrisgkent@gmail.com>"]
 readme = "README.md"
+repository = "https://github.com/ChrisgKent/primal-page"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^2.4.2"
 typer = {extras = ["all"], version = "^0.9.0"}
 requests = "^2.31.0"
```

### Comparing `primal_page-1.5.0/PKG-INFO` & `primal_page-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,224 @@
 Metadata-Version: 2.1
 Name: primal-page
-Version: 1.5.0
-Summary: 
+Version: 1.5.1
+Summary: Tooling and schemas for the primerschemes index
+Home-page: https://github.com/ChrisgKent/primal-page
 Author: ChrisKent
 Author-email: chrisgkent@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Project-URL: Repository, https://github.com/ChrisgKent/primal-page
 Description-Content-Type: text/markdown
 
 # Primal-Page
 
 [![CI](https://github.com/ChrisgKent/primal-page/actions/workflows/pytest.yml/badge.svg)](https://github.com/ChrisgKent/primal-page/actions/workflows/pytest.yml)
 
 
-This is the tooling for working with the primerschemes index
+Tooling and schemas for the primerschemes index
 
 ## Contents
 
-[cli](https://github.com/ChrisgKent/primal-page?tab=readme-ov-file#cli)
+[Installation](https://github.com/ChrisgKent/primal-page?tab=readme-ov-file#installation)
 
-[schemas](https://github.com/ChrisgKent/primal-page?tab=readme-ov-file#new-schemas)
+[Quick Start](https://github.com/ChrisgKent/primal-page?tab=readme-ov-file#quick-start)
+
+[Schemas](https://github.com/ChrisgKent/primal-page?tab=readme-ov-file#new-schemas)
+
+[CLI](https://github.com/ChrisgKent/primal-page?tab=readme-ov-file#cli)
+
+# Installation
+
+```
+pip install primal-page
+```
+
+# Quick Start
+
+Each version of a primerscheme has three parts; `{schemename}/{ampliconsize}/{version}`, which when combined these form the schemes unique identifier.
+
+For a scheme to be added to the repo it requires three essental files. 
+- `primer.bed`: Contains the primer infomation.   
+- `reference.fasta`: Contains the reference genomes.
+- `info.json`: Contains key metadata for the scheme.
+
+The `primal-page create` command will generates the `info.json` and parses a bed file and a fasta file into `primer.bed` and `reference.fasta`
+
+Additional files are copied into the schemes work directory. 
+
+## Example
+### Adding a minimal scheme
+
+For a simple scheme, only fasta file (--reference) and a bed file (--primerbed) are required. Alongside metadata of --schemename, --algorithmversion, --species, --authors.
+
+```
+primal-page create \
+    --schemename example-scheme \
+    --algorithmversion ps:100 \
+    --ampliconsize 500 \
+    --species 123  \
+    --schemeversion v1.0.0 \
+    --primerbed ~/'minimal-scheme/minimal.bed' \
+    --reference '~/minimal-scheme/ref.fasta' \
+    --authors "me" \
+    --authors "you" /
+    '~/minimal-scheme' 
+```
+
+### Adding a custom scheme to quick-lab/primerschemes
+
+
+> create a local fork of https://github.com/quick-lab/primerschemes
+
+> Add the files to the forks primerschemes folder
+```
+primal-page create primal-page create ... --output ~/primerschemes/primerschemes
+```
+
+> Create a pull request 
+
+
+# New Schemas
+
+## info.json
+
+This is the main metadata file for each primerscheme.
+
+- `ampliconsize`: PositiveInt
+- `schemeversion`: Following format listed below
+- `schemename`: Following format listed below
+- `primer_bed_md5`: MD5 hash of the schemes primer.bed file
+- `reference_fasta_md5`: MD5 hash of the schemes reference.fasta file
+- `status`: 
+    - `withdrawn`: Removed due to major issue
+    - `deprecated`: Newer scheme is recommended
+    - `autogenerated`: Scheme has been autogenerated using species-agnostic pipelines
+    - `draft`: Scheme has been inspected in silico
+    - `tested`: Scheme has been tested in the laboratory
+    - `validated`: Scheme has been validated and/or published
+- `citations`: How the scheme should be cited if used. DOI links are recommended, however, tweets/blogs are all allowed
+- `authors`: The person or organisation who generated the scheme. It is recommended that only corresponding/primary authors are included, with all other contributors recognised in the `citations` field
+- `algorithmversion`: The algorithm and the version used to generate the scheme
+- `species`: A list of organisms targeted by this scheme. NCBI TaxIds are recommend
+- `license`: The name of the license the primerscheme is offered under
+- `primerclass`: The class of scheme. Only `primerscheme` at the moment
+- `infoschema`: The version of the info.json 
+- `articbedversion`: The version of the primer.bed (See below)
+- `description`: A free text description to describe the primerscheme
+- `derivedfrom`: To show if this scheme has been based on another primerscheme. 
+- `collections`: A collection of vocab to provide filtering/grouping of schemes.
+    - `ARTIC`: Developed with the ARTIC network
+    - `MODJADJI`: Developed with MODJADJI
+    - `QUICK-LAB`: Developed with QUICK-LAB
+    - `COMMUNITY`: Developed by the COMMUNITY
+    - `WASTE-WATER`: Scheme capable of recovering genomes from high Ct samples (~30) samples, like wastewater. Typically 400bp schemes
+    - `CLINAL-ISOLATES`: Scheme capable of recovering genomes from medium Ct samples (~25) samples.  Typically ~1000bp schemes
+    - `WHOLE-GENOME`: Scheme that can theoretically recover a full genome
+    - `PANEL`: Scheme that can recover sections of a target genome
+    - `MULTI-TARGET`: Scheme that contains more than one target
+
+## PrimerNames Versions
+
+Expected primernames (col3) in the primer.bed file
+
+### `V1`
+
+This is the first standard for primernames. It follows the general pattern of `{scheme-name|uuid}_{amplicon-number}_{LEFT|RIGHT}` and an optional `{_alt}` to denote spike in primers.
+
+Regex:
+
+ ```V1_PRIMERNAME = r"^[a-zA-Z0-9\-]+_[0-9]+_(LEFT|RIGHT)(_ALT[0-9]*|_alt[0-9]*)*$"```
+
+Example:
+```
+SARS-CoV-2_10_LEFT
+SARS-CoV-2_10_LEFT_alt1
+```
+
+
+### `V2`
+
+This follows the pattern of `{scheme-name|uuid}_{amplicon-number}_{LEFT|RIGHT}_{primer-number}`. 
+- This now enforces that splitting on `_` will produce a consistent length, allowing the safe indexing of attributes. 
+- `primer-number` is not enforced to be continuous. Therefore, the `_0` numbered primer should not be thought of as the `original` and all other numbers as `alts`.
+
+
+Example:
+```
+SARS-CoV-2_10_LEFT_0
+SARS-CoV-2_10_LEFT_1
+```
+
+Regex:
+
+```V2_PRIMERNAME = r"^[a-zA-Z0-9\-]+_[0-9]+_(LEFT|RIGHT)_[0-9]+$"```
+
+
+## ARTIC-primer.bed Versions
+
+These are rough guidelines for the format of the primer.bed file. The general format is based on the [.bed file](https://en.wikipedia.org/wiki/BED_(file_format)) and maintains compatibility with other tools.
+
+colnames and indexes:
+- `0 - chrom`: The name of the reference genome the primers are indexed to
+- `1 - chromStart`: 0-based inclusive start coordinate
+- `2 - chromEnd`: 0-based non-inclusive end coordinate
+- `3 - primer-name`: Name of each primer
+- `4 - pool`: The pool each primer should be added into. 1 based.
+- `5 - strand`: Either `+` (forward) or `-` (reverse) primer
+- `6 - primer-sequence`: The 5'-3' sequence of the primer
+
+
+
+### V1
+> Depreciated 
+
+This was the original 6-col bedfile used very early in PrimalSchemes development, which excluded primer-sequence. 
+
+### V2
+> Legacy
+
+This uses the 7 columns described above, alongside `V1:primernames`.
+- Single chrom (reference) is expected
+- No header lines
+
+### V3
+> Current
+
+This uses the 7 columns described above, alongside `V2:primernames`.
+- Multiple chrom (references)
+- Circular primers are allowed. The start of x_LEFT can be greater than the end of x_RIGHT
+- Header lines are used. Denoted with the `#` character 
+
+ 
+## Scheme Version
+
+In the form of `v{Major}.{Minor}.{Patch}`
+- Major: New scheme being generated with differant input params
+- Minor: Change to primers. Either additional / removal of primers
+- Patch: No change to primers. Often used for rebalancing or change in formatting
+
+
+Regex:
+
+`VERSION_PATTERN = r"^v\d+\.\d+\.\d+$"`
+
+
+## Scheme Name
+
+Must only contain `a-z`, `0-9`, and `-`. Cannot start or end with `-`
+
+Regex:
+
+`SCHEMENAME_PATTERN = r"^[a-z0-9][a-z0-9-]*[a-z0-9]$"`
 
 # CLI
 
 **Usage**:
 
 ```console
 $ [OPTIONS] COMMAND [ARGS]...
@@ -439,172 +629,7 @@
 * `SCHEMEINFO`: The path to info.json  [required]
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 # Examples
-
-### Adding a minimal scheme
-
-For a simple scheme, only fasta file (--reference) and a bed file (--primerbed) are required. Alongside metadata of --schemename, --algorithmversion, --species, --authors.
-
-```
-primal-page create \
-    --schemename example-scheme \
-    --algorithmversion ps:100 \
-    --ampliconsize 500 \
-    --species 123  \
-    --schemeversion v1.0.0 \
-    --primerbed 'minimal-scheme/minimal.bed' \
-    --reference 'minimal-scheme/ref.fasta' \
-    --authors me \
-    --authors you /
-    'minimal-scheme' 
-```
-
-### Adding a custom scheme to quick-lab/primerschemes
-
-
-> create a local fork of https://github.com/quick-lab/primerschemes
-
-> Add the files to the forks primerschemes folder
-```
-primal-page create primal-page create ... --output ~/primerschemes/primerschemes
-```
-
-> Create a pull request 
-
-
-# New Schemas
-
-## info.json
-
-This is the main metadata file for each primerscheme.
-
-- `ampliconsize`: PositiveInt
-- `schemeversion`: Following format listed below
-- `schemename`: Following format listed below
-- `primer_bed_md5`: MD5 hash of the schemes primer.bed file
-- `reference_fasta_md5`: MD5 hash of the schemes reference.fasta file
-- `status`: 
-    - `withdrawn`: Removed due to major issue
-    - `deprecated`: Newer scheme is recommended
-    - `autogenerated`: Scheme has been autogenerated using species-agnostic pipelines
-    - `draft`: Scheme has been inspected in silico
-    - `tested`: Scheme has been tested in the laboratory
-    - `validated`: Scheme has been validated and/or published
-- `citations`: How the scheme should be cited if used. DOI links are recommended, however, tweets/blogs are all allowed
-- `authors`: The person or organisation who generated the scheme. It is recommended that only corresponding/primary authors are included, with all other contributors recognised in the `citations` field
-- `algorithmversion`: The algorithm and the version used to generate the scheme
-- `species`: A list of organisms targeted by this scheme. NCBI TaxIds are recommend
-- `license`: The name of the license the primerscheme is offered under
-- `primerclass`: The class of scheme. Only `primerscheme` at the moment
-- `infoschema`: The version of the info.json 
-- `articbedversion`: The version of the primer.bed (See below)
-- `description`: A free text description to describe the primerscheme
-- `derivedfrom`: To show if this scheme has been based on another primerscheme. 
-- `collections`: A collection of vocab to provide filtering/grouping of schemes.
-    - `ARTIC`: Developed with the ARTIC network
-    - `MODJADJI`: Developed with MODJADJI
-    - `QUICK-LAB`: Developed with QUICK-LAB
-    - `COMMUNITY`: Developed by the COMMUNITY
-    - `WASTE-WATER`: Scheme capable of recovering genomes from high Ct samples (~30) samples, like wastewater. Typically 400bp schemes
-    - `CLINAL-ISOLATES`: Scheme capable of recovering genomes from medium Ct samples (~25) samples.  Typically ~1000bp schemes
-    - `WHOLE-GENOME`: Scheme that can theoretically recover a full genome
-    - `PANEL`: Scheme that can recover sections of a target genome
-    - `MULTI-TARGET`: Scheme that contains more than one target
-
-## PrimerNames Versions
-
-Expected primernames (col3) in the primer.bed file
-
-### `V1`
-
-This is the first standard for primernames. It follows the general pattern of `{scheme-name|uuid}_{amplicon-number}_{LEFT|RIGHT}` and an optional `{_alt}` to denote spike in primers.
-
-Regex:
-
- ```V1_PRIMERNAME = r"^[a-zA-Z0-9\-]+_[0-9]+_(LEFT|RIGHT)(_ALT[0-9]*|_alt[0-9]*)*$"```
-
-Example:
-```
-SARS-CoV-2_10_LEFT
-SARS-CoV-2_10_LEFT_alt1
-```
-
-
-### `V2`
-
-This follows the pattern of `{scheme-name|uuid}_{amplicon-number}_{LEFT|RIGHT}_{primer-number}`. 
-- This now enforces that splitting on `_` will produce a consistent length, allowing the safe indexing of attributes. 
-- `primer-number` is not enforced to be continuous. Therefore, the `_0` numbered primer should not be thought of as the `original` and all other numbers as `alts`.
-
-
-Example:
-```
-SARS-CoV-2_10_LEFT_0
-SARS-CoV-2_10_LEFT_1
-```
-
-Regex:
-
-```V2_PRIMERNAME = r"^[a-zA-Z0-9\-]+_[0-9]+_(LEFT|RIGHT)_[0-9]+$"```
-
-
-## ARTIC-primer.bed Versions
-
-These are rough guidelines for the format of the primer.bed file. The general format is based on the [.bed file](https://en.wikipedia.org/wiki/BED_(file_format)) and maintains compatibility with other tools.
-
-colnames and indexes:
-- `0 - chrom`: The name of the reference genome the primers are indexed to
-- `1 - chromStart`: 0-based inclusive start coordinate
-- `2 - chromEnd`: 0-based non-inclusive end coordinate
-- `3 - primer-name`: Name of each primer
-- `4 - pool`: The pool each primer should be added into. 1 based.
-- `5 - strand`: Either `+` (forward) or `-` (reverse) primer
-- `6 - primer-sequence`: The 5'-3' sequence of the primer
-
-
-
-### V1
-> Depreciated 
-
-This was the original 6-col bedfile used very early in PrimalSchemes development, which excluded primer-sequence. 
-
-### V2
-> Legacy
-
-This uses the 7 columns described above, alongside `V1:primernames`.
-- Single chrom (reference) is expected
-- No header lines
-
-### V3
-> Current
-
-This uses the 7 columns described above, alongside `V2:primernames`.
-- Multiple chrom (references)
-- Circular primers are allowed. The start of x_LEFT can be greater than the end of x_RIGHT
-- Header lines are used. Denoted with the `#` character 
-
- 
-## Scheme Version
-
-In the form of `v{Major}.{Minor}.{Patch}`
-- Major: New scheme being generated with differant input params
-- Minor: Change to primers. Either additional / removal of primers
-- Patch: No change to primers. Often used for rebalancing or change in formatting
-
-
-Regex:
-
-`VERSION_PATTERN = r"^v\d+\.\d+\.\d+$"`
-
-
-## Scheme Name
-
-Must only contain `a-z`, `0-9`, and `-`. Cannot start or end with `-`
-
-Regex:
-
-`SCHEMENAME_PATTERN = r"^[a-z0-9][a-z0-9-]*[a-z0-9]$"`
-
```

