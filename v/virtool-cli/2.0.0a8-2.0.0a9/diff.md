# Comparing `tmp/virtool_cli-2.0.0a8.tar.gz` & `tmp/virtool_cli-2.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtool_cli-2.0.0a8.tar", max compression
+gzip compressed data, was "virtool_cli-2.0.0a9.tar", max compression
```

## Comparing `virtool_cli-2.0.0a8.tar` & `virtool_cli-2.0.0a9.tar`

### file list

```diff
@@ -1,47 +1,49 @@
--rw-r--r--   0        0        0      881 2024-01-17 23:35:26.887979 virtool_cli-2.0.0a8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/add/__init__.py
--rw-r--r--   0        0        0     2984 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/add/add_accession_auto.py
--rw-r--r--   0        0        0     2905 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/add/add_accessions.py
--rw-r--r--   0        0        0     4430 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/add/add_otu.py
--rw-r--r--   0        0        0     2478 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/add/cli.py
--rw-r--r--   0        0        0     1118 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/add/format.py
--rw-r--r--   0        0        0     3685 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/add/helpers.py
--rw-r--r--   0        0        0      780 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/add/write.py
--rw-r--r--   0        0        0     6004 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/build.py
--rw-r--r--   0        0        0        0 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/check/__init__.py
--rw-r--r--   0        0        0      844 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/check/check_otu.py
--rw-r--r--   0        0        0     1576 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/check/check_reference.py
--rw-r--r--   0        0        0     6703 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/check/checkup.py
--rw-r--r--   0        0        0     1477 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/check/cli.py
--rw-r--r--   0        0        0      333 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/cli.py
--rw-r--r--   0        0        0     4534 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/divide.py
--rw-r--r--   0        0        0     3275 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/hmm.py
--rw-r--r--   0        0        0     1980 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/init.py
--rw-r--r--   0        0        0     2272 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/migrate.py
--rw-r--r--   0        0        0     3692 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/ref.py
--rw-r--r--   0        0        0        0 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/update/__init__.py
--rw-r--r--   0        0        0     1713 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/update/cli.py
--rw-r--r--   0        0        0     1598 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/update/update.py
--rw-r--r--   0        0        0     2513 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/update/update_otu.py
--rw-r--r--   0        0        0     7783 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/update/update_ref.py
--rw-r--r--   0        0        0        0 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/utils/__init__.py
--rw-r--r--   0        0        0      733 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/utils/cache.py
--rw-r--r--   0        0        0     9295 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/utils/format.py
--rw-r--r--   0        0        0     1715 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/utils/id_generator.py
--rw-r--r--   0        0        0     1843 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/utils/logging.py
--rw-r--r--   0        0        0     6210 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/utils/ncbi.py
--rw-r--r--   0        0        0     1411 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/utils/parse.py
--rw-r--r--   0        0        0     3672 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/utils/reference.py
--rw-r--r--   0        0        0     7382 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/utils/storage.py
--rw-r--r--   0        0        0        0 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/vfam/__init__.py
--rw-r--r--   0        0        0     6406 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/vfam/annotation.py
--rw-r--r--   0        0        0     2469 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/vfam/cmd.py
--rw-r--r--   0        0        0     4249 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/vfam/collapse.py
--rw-r--r--   0        0        0       54 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/vfam/console.py
--rw-r--r--   0        0        0     7458 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/vfam/curate.py
--rw-r--r--   0        0        0     4961 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/vfam/filter.py
--rw-r--r--   0        0        0     4875 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/vfam/markov.py
--rw-r--r--   0        0        0     3274 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/vfam/msa.py
--rw-r--r--   0        0        0     5980 2024-01-17 23:35:13.087941 virtool_cli-2.0.0a8/virtool_cli/vfam/polyprotein.py
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 virtool_cli-2.0.0a8/PKG-INFO
+-rw-r--r--   0        0        0      881 2024-01-23 22:41:22.464902 virtool_cli-2.0.0a9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-23 22:41:08.636876 virtool_cli-2.0.0a9/virtool_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-23 22:41:08.636876 virtool_cli-2.0.0a9/virtool_cli/add/__init__.py
+-rw-r--r--   0        0        0     2984 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/add/add_accession_auto.py
+-rw-r--r--   0        0        0     2905 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/add/add_accessions.py
+-rw-r--r--   0        0        0     4365 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/add/add_otu.py
+-rw-r--r--   0        0        0     2478 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/add/cli.py
+-rw-r--r--   0        0        0     1118 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/add/format.py
+-rw-r--r--   0        0        0     3685 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/add/helpers.py
+-rw-r--r--   0        0        0      780 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/add/write.py
+-rw-r--r--   0        0        0     6004 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/build.py
+-rw-r--r--   0        0        0        0 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/check/__init__.py
+-rw-r--r--   0        0        0      780 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/check/check_otu.py
+-rw-r--r--   0        0        0     1511 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/check/check_reference.py
+-rw-r--r--   0        0        0     6703 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/check/checkup.py
+-rw-r--r--   0        0        0     1477 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/check/cli.py
+-rw-r--r--   0        0        0      333 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/cli.py
+-rw-r--r--   0        0        0     4469 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/divide.py
+-rw-r--r--   0        0        0     3275 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/hmm.py
+-rw-r--r--   0        0        0     1915 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/init.py
+-rw-r--r--   0        0        0     2397 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/migrate.py
+-rw-r--r--   0        0        0     3692 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/ref.py
+-rw-r--r--   0        0        0        0 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/update/__init__.py
+-rw-r--r--   0        0        0     3255 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/update/cli.py
+-rw-r--r--   0        0        0     3528 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/update/uncache.py
+-rw-r--r--   0        0        0     2923 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/update/update.py
+-rw-r--r--   0        0        0     3109 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/update/update_otu.py
+-rw-r--r--   0        0        0     9053 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/update/update_ref.py
+-rw-r--r--   0        0        0     3739 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/update/writer.py
+-rw-r--r--   0        0        0        0 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/utils/__init__.py
+-rw-r--r--   0        0        0      733 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/utils/cache.py
+-rw-r--r--   0        0        0     8037 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/utils/format.py
+-rw-r--r--   0        0        0     1715 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/utils/id_generator.py
+-rw-r--r--   0        0        0     1843 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/utils/logging.py
+-rw-r--r--   0        0        0     6541 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/utils/ncbi.py
+-rw-r--r--   0        0        0     1411 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/utils/parse.py
+-rw-r--r--   0        0        0     3670 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/utils/reference.py
+-rw-r--r--   0        0        0     7382 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/utils/storage.py
+-rw-r--r--   0        0        0        0 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/vfam/__init__.py
+-rw-r--r--   0        0        0     6406 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/vfam/annotation.py
+-rw-r--r--   0        0        0     2469 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/vfam/cmd.py
+-rw-r--r--   0        0        0     4249 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/vfam/collapse.py
+-rw-r--r--   0        0        0       54 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/vfam/console.py
+-rw-r--r--   0        0        0     7458 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/vfam/curate.py
+-rw-r--r--   0        0        0     4961 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/vfam/filter.py
+-rw-r--r--   0        0        0     4875 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/vfam/markov.py
+-rw-r--r--   0        0        0     3274 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/vfam/msa.py
+-rw-r--r--   0        0        0     5980 2024-01-23 22:41:08.640876 virtool_cli-2.0.0a9/virtool_cli/vfam/polyprotein.py
+-rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 virtool_cli-2.0.0a9/PKG-INFO
```

### Comparing `virtool_cli-2.0.0a8/pyproject.toml` & `virtool_cli-2.0.0a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "virtool-cli"
-version = "2.0.0-alpha.8"
+version = "2.0.0-alpha.9"
 authors = [
     "Ian Boyes <igboyes@gmail.com>",
     "Jake Alexander",
     "Lilly Roberts",
     "Shelley Gao"
 ]
 maintainers = [
```

### Comparing `virtool_cli-2.0.0a8/virtool_cli/add/add_accession_auto.py` & `virtool_cli-2.0.0a9/virtool_cli/add/add_accession_auto.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/add/add_accessions.py` & `virtool_cli-2.0.0a9/virtool_cli/add/add_accessions.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/add/add_otu.py` & `virtool_cli-2.0.0a9/virtool_cli/add/add_otu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from pathlib import Path
 import asyncio
 import structlog
 from urllib.error import HTTPError
 
-from virtool_cli.utils.logging import DEFAULT_LOGGER, DEBUG_LOGGER
+from virtool_cli.utils.logging import configure_logger
 from virtool_cli.utils.reference import is_v1, generate_otu_dirname, get_unique_otu_ids
 from virtool_cli.utils.id_generator import generate_unique_ids
 from virtool_cli.utils.ncbi import fetch_taxonomy_record
 from virtool_cli.utils.cache import generate_taxid_table
 
 OTU_KEYS = ["_id", "name", "abbreviation", "schema", "taxid"]
 
@@ -25,15 +25,15 @@
 
     Requests updates for a single OTU directory
 
     :param taxid: NCBI Taxon ID as an integer
     :param src_path: Path to a reference directory
     :param debugging: Enables verbose logs for debugging purposes
     """
-    structlog.configure(wrapper_class=DEBUG_LOGGER if debugging else DEFAULT_LOGGER)
+    configure_logger(debugging)
     logger = base_logger.bind(src=str(src_path))
 
     if is_v1(src_path):
         logger.critical(
             'Reference folder "src" is a deprecated v1 reference.'
             + 'Run "virtool ref migrate" before trying again.'
         )
```

### Comparing `virtool_cli-2.0.0a8/virtool_cli/add/cli.py` & `virtool_cli-2.0.0a9/virtool_cli/add/cli.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/add/format.py` & `virtool_cli-2.0.0a9/virtool_cli/add/format.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/add/helpers.py` & `virtool_cli-2.0.0a9/virtool_cli/add/helpers.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/add/write.py` & `virtool_cli-2.0.0a9/virtool_cli/add/write.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/build.py` & `virtool_cli-2.0.0a9/virtool_cli/build.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/check/check_otu.py` & `virtool_cli-2.0.0a9/virtool_cli/check/check_otu.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from pathlib import Path
 import structlog
-from virtool_cli.utils.logging import DEBUG_LOGGER, DEFAULT_LOGGER
+
+from virtool_cli.utils.logging import configure_logger
 from virtool_cli.check.checkup import check_otu
 
 base_logger = structlog.get_logger()
 
 
 def run(otu_path: Path, debugging: bool = False):
     """
     CLI entry point for doctor.checkup.run()
 
     :param otu_path: Path to an OTU directory
     :param debugging: Enables verbose logs for debugging purposes
     """
-    structlog.configure(wrapper_class=DEBUG_LOGGER if debugging else DEFAULT_LOGGER)
+    configure_logger(debugging)
     logger = base_logger.bind(otu_path=str(otu_path), verbose=debugging)
 
     logger.debug("Debug flag is enabled")
 
     if check_otu(otu_path):
         logger.info("Reference folder is valid.", valid_result=True)
         print(True)
```

### Comparing `virtool_cli-2.0.0a8/virtool_cli/check/check_reference.py` & `virtool_cli-2.0.0a9/virtool_cli/check/check_reference.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from pathlib import Path
 import structlog
 
+from virtool_cli.utils.logging import configure_logger
 from virtool_cli.check.checkup import check_otu
-from virtool_cli.utils.logging import DEBUG_LOGGER, DEFAULT_LOGGER
 from virtool_cli.utils.reference import get_otu_paths
 
 base_logger = structlog.get_logger()
 
 
 def run(src_path: Path, debugging: bool = False):
     """
     CLI entry point for doctor.checkup.run()
 
     :param src_path: Path to a given reference directory
     :param debugging: Enables verbose logs for debugging purposes
     """
-    structlog.configure(wrapper_class=DEBUG_LOGGER if debugging else DEFAULT_LOGGER)
+    configure_logger(debugging)
     logger = base_logger.bind(src=str(src_path), verbose=debugging)
 
     logger.debug("Debug flag is enabled")
 
     if check_reference(src_path):
         logger.info("Reference folder is valid.", valid_result=True)
     else:
```

### Comparing `virtool_cli-2.0.0a8/virtool_cli/check/checkup.py` & `virtool_cli-2.0.0a9/virtool_cli/check/checkup.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/check/cli.py` & `virtool_cli-2.0.0a9/virtool_cli/check/cli.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/divide.py` & `virtool_cli-2.0.0a9/virtool_cli/divide.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from pathlib import Path
 import asyncio
 import shutil
 import aiofiles
 import structlog
 
-from virtool_cli.utils.logging import DEBUG_LOGGER, DEFAULT_LOGGER
+from virtool_cli.utils.logging import configure_logger
 from virtool_cli.utils.reference import generate_otu_dirname
 
 base_logger = structlog.get_logger()
 
 OTU_KEYS = ["_id", "name", "abbreviation", "schema", "taxid"]
 
 ISOLATE_KEYS = ["id", "source_type", "source_name", "default"]
@@ -29,15 +29,15 @@
     """
     Divide a reference.json file from Virtool into a src tree structure.
 
     :param reference_path: Path to a reference.json file
     :param output_path: Path to the where the src tree should be generated
     :param debugging: Enables verbose logs for debugging purposes
     """
-    structlog.configure(wrapper_class=DEBUG_LOGGER if debugging else DEFAULT_LOGGER)
+    configure_logger(debugging)
     logger = base_logger.bind(reference=str(reference_path), output=str(output_path))
 
     logger.info(f"Dividing {output_path.name} into {reference_path.name}...")
 
     asyncio.run(divide_reference_file(reference_path, output_path))
```

### Comparing `virtool_cli-2.0.0a8/virtool_cli/hmm.py` & `virtool_cli-2.0.0a9/virtool_cli/hmm.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/init.py` & `virtool_cli-2.0.0a9/virtool_cli/init.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 from pathlib import Path
 from shutil import copytree
 import structlog
-from virtool_cli.utils.logging import DEFAULT_LOGGER, DEBUG_LOGGER
+from virtool_cli.utils.logging import configure_logger
 
 base_logger = structlog.get_logger()
 
 
 def run(repo_path: Path, debugging: bool = False):
     """
     Creates an empty repository for Virtool reference data
 
     :param repo_path: Path to repository src directory
     :param debugging: Enables verbose logs for debugging purposes
     """
-    structlog.configure(wrapper_class=DEBUG_LOGGER if debugging else DEFAULT_LOGGER)
+    configure_logger(debugging)
     logger = base_logger.bind(repo=str(repo_path))
 
     try:
         logger.info("Creating new reference database at path...")
         initialize_reference(repo_path)
     except FileNotFoundError as e:
         logger.exception(e)
```

### Comparing `virtool_cli-2.0.0a8/virtool_cli/migrate.py` & `virtool_cli-2.0.0a9/virtool_cli/migrate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from pathlib import Path
 import asyncio
 import structlog
+import json
 
-from virtool_cli.utils.logging import DEFAULT_LOGGER, DEBUG_LOGGER
+from virtool_cli.utils.logging import configure_logger
 from virtool_cli.utils.reference import generate_otu_dirname, is_v1
 from virtool_cli.utils.storage import read_otu
 
 base_logger = structlog.get_logger()
 
 
 def run(src_path: Path, debugging: bool = False):
     """
     :param src_path: Path to a src database directory
     :param debugging: Enables verbose logs for debugging purposes
     """
-    structlog.configure(wrapper_class=DEBUG_LOGGER if debugging else DEFAULT_LOGGER)
+    configure_logger(debugging)
     logger = base_logger.bind(src_path=str(src_path))
 
     if not is_v1(src_path):
         logger.info("Reference in src_path is already v2")
 
         return
 
@@ -45,14 +46,16 @@
         otu_paths = [otu for otu in alpha.iterdir() if otu.is_dir()]
 
         alpha_logger.debug(
             f"Flattening bin '{alpha.name}'", otus=[otu.name for otu in otu_paths]
         )
 
         for otu_path in otu_paths:
+            init_exclusions(otu_path)
+
             otu = await read_otu(otu_path)
             new_name = generate_otu_dirname(otu.get("name"), otu.get("_id"))
             new_path = src_path / new_name
 
             alpha_logger.debug(
                 f"Renaming '{otu_path.relative_to(src_path)}'"
                 + f"to '{new_path.relative_to(src_path)}'..."
@@ -64,7 +67,12 @@
         try:
             for chaff in alpha.iterdir():
                 chaff.unlink()
             alpha.rmdir()
         except Exception as e:
             alpha_logger.error("Bin deletion failed")
             alpha_logger.exception(e)
+
+
+def init_exclusions(otu_path):
+    with open(otu_path / "exclusions.json", "w") as f:
+        json.dump([], f, indent=4, sort_keys=True)
```

### Comparing `virtool_cli-2.0.0a8/virtool_cli/ref.py` & `virtool_cli-2.0.0a9/virtool_cli/ref.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/update/cli.py` & `virtool_cli-2.0.0a9/virtool_cli/update/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
 import click
 
 from virtool_cli.update.update_ref import run as run_update_all
 from virtool_cli.update.update_otu import run as run_update_single
+from virtool_cli.update.uncache import run as run_update_uncache
 
 
 @click.group("update")
 def update():
     """
     Commands related to updates
     """
@@ -17,41 +18,109 @@
 @click.option(
     "-src",
     "--src_path",
     required=True,
     type=click.Path(exists=True, file_okay=False, path_type=Path),
     help="the path to a reference directory",
 )
-@click.option("--evaluate/--no-evaluate", default=False, help="Enable auto-filtering")
-@click.option("--debug/--no-debug", default=False, help="Enable debugging logs")
-def reference(src_path, evaluate, debug):
-    """Fetch new sequences and isolates for all OTU in a given reference directory."""
+@click.option(
+    "--filter",
+    default="*",
+    type=str,
+    help="entry point for glob filter",
+)
+@click.option(
+    "--dry/--not-dry",
+    default=False,
+    help="Write to default cache directory instead of reference directory"
+)
+@click.option(
+    "--evaluate/--no-evaluate",
+    default=False,
+    help="Enable auto-evaluation"
+)
+@click.option(
+    "--debug/--no-debug",
+    default=False,
+    help="Enable debugging logs"
+)
+def reference(src_path, filter, evaluate, dry, debug):
+    """Fetch new NCBI data for all OTU in a given reference directory."""
     try:
-        run_update_all(src_path, auto_evaluate=evaluate, debugging=debug)
+        run_update_all(src_path, filter, auto_evaluate=evaluate, dry_run=dry, debugging=debug)
     except (FileNotFoundError, NotADirectoryError) as e:
         click.echo("Not a valid reference directory", err=True)
 
 
 @update.command()
 @click.option(
     "-otu",
     "--otu_path",
     required=True,
     type=click.Path(exists=True, file_okay=False, path_type=Path),
     help="the path to a single OTU directory",
 )
-@click.option("--evaluate/--no-evaluate", default=False, help="Enable auto-filtering")
-@click.option("--debug/--no-debug", default=False, help="Enable debugging logs")
-def otu(otu_path, evaluate, debug):
-    """Fetch new sequences and isolates for a given OTU directory."""
+@click.option(
+    "--dry/--not-dry",
+    default=False,
+    help="Write to default cache directory instead of reference directory"
+)
+@click.option(
+    "--evaluate/--no-evaluate",
+    default=False,
+    help="Enable auto-evaluation"
+)
+@click.option(
+    "--debug/--no-debug",
+    default=False,
+    help="Enable debugging logs"
+)
+def otu(otu_path, evaluate, dry, debug):
+    """Fetch new NCBI data for a given OTU directory."""
 
     try:
         run_update_single(
-            otu_path, auto_evaluate=evaluate, debugging=debug
+            otu_path, auto_evaluate=evaluate, dry_run=dry, debugging=debug
         )
 
     except (FileNotFoundError, NotADirectoryError) as e:
         click.echo("Not a valid reference directory", err=True)
 
 
+@update.command()
+@click.option(
+    "-cache",
+    "--cache_path",
+    required=True,
+    type=click.Path(exists=True, file_okay=False, path_type=Path),
+    help="the path to a cache directory",
+)
+@click.option(
+    "-src",
+    "--src_path",
+    required=True,
+    type=click.Path(exists=True, file_okay=False, path_type=Path),
+    help="the path to a reference directory",
+)
+@click.option(
+    "--evaluate/--no-evaluate",
+    default=False,
+    help="Enable auto-evaluation ()"
+)
+@click.option(
+    "--debug/--no-debug",
+    default=False,
+    help="Enable debugging logs"
+)
+def uncache(cache_path, src_path, evaluate, debug):
+    """
+        Write cached sequence data under reference directory.
+        Read cached sequence data from a cache directory and write to a reference directory.
+    """
+    try:
+        run_update_uncache(cache_path, src_path, auto_evaluate=evaluate, debugging=debug)
+    except (FileNotFoundError, NotADirectoryError) as e:
+        click.echo("Not a valid reference directory", err=True)
+
+
 if __name__ == "__main__":
     update()
```

### Comparing `virtool_cli-2.0.0a8/virtool_cli/update/update_otu.py` & `virtool_cli-2.0.0a9/virtool_cli/update/update_otu.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 from pathlib import Path
 import asyncio
 import structlog
 
-from virtool_cli.utils.logging import DEFAULT_LOGGER, DEBUG_LOGGER
+from virtool_cli.utils.logging import configure_logger
 from virtool_cli.utils.reference import get_otu_paths, get_unique_ids
-from virtool_cli.utils.format import process_records
 from virtool_cli.utils.storage import read_otu, write_records
-from virtool_cli.update.update import get_no_fetch_set, request_new_records
+from virtool_cli.update.update import get_no_fetch_set, request_new_records, process_records
+from virtool_cli.update.writer import cache_new_sequences
 
 base_logger = structlog.get_logger()
 
 
 def run(
     otu_path: Path,
     auto_evaluate: bool = False,
+    dry_run: bool = False,
     debugging: bool = False,
 ):
     """
     CLI entry point for update.update.run()
 
-    Requests updates for a single OTU directory
-    Searches the catalog for a matching catalog listing and requests new updates if it finds one.
+    Requests updates for a single OTU directory.
+    Inspects OTU contents and exclusions and requests relevant accession if found.
 
     :param otu_path: Path to an OTU directory
     :param auto_evaluate: Auto-evaluation flag, enables automatic filtering for fetched results
+    :param dry_run: Caching flag, writes all update data to a single file under
+        "{repo_path}/.cache/updates/{otu_id}.json",
+        instead of the reference directory
     :param debugging: Enables verbose logs for debugging purposes
     """
-    structlog.configure(wrapper_class=DEBUG_LOGGER if debugging else DEFAULT_LOGGER)
+    configure_logger(debugging)
     logger = base_logger.bind(otu_path=str(otu_path))
 
     if auto_evaluate:
         logger.warning(
             "Auto-evaluation is in active development and may produce false negatives."
         )
 
-    asyncio.run(update_otu(otu_path, auto_evaluate))
+    asyncio.run(update_otu(otu_path, auto_evaluate, dry_run))
 
 
 async def update_otu(
-    otu_path: Path, auto_evaluate: bool = False
+    otu_path: Path, auto_evaluate: bool = False, dry_run: bool = False
 ):
     """
     Requests new records for a single taxon ID
     and writes new data under the corresponding path.
 
-    :param otu_path: Path to a OTU directory
+    :param otu_path: Path to an OTU directory
     :param auto_evaluate: Auto-evaluation flag, enables automatic filtering for fetched results
+    :param dry_run:
     """
     src_path = otu_path.parent
+
+    # List all isolate and sequence IDs presently in src
+    unique_iso, unique_seq = await get_unique_ids(get_otu_paths(src_path))
+
     metadata = await read_otu(otu_path)
 
     no_fetch_set = await get_no_fetch_set(otu_path)
 
     otu_id = metadata.get('_id')
     taxid = metadata.get('taxid')
 
@@ -60,23 +69,31 @@
     try:
         record_data = await request_new_records(taxid, no_fetch_set, logger)
     except Exception as e:
         logger.exception(e)
         return
 
     if not record_data:
+        logger.debug("No records found.")
         return
 
     otu_updates = await process_records(
         records=record_data,
         metadata=metadata,
         no_fetch_set=no_fetch_set,
         auto_evaluate=auto_evaluate,
         logger=logger
     )
     if not otu_updates:
         return
 
-    # List all isolate and sequence IDs presently in src
-    unique_iso, unique_seq = await get_unique_ids(get_otu_paths(src_path))
-
-    await write_records(otu_path, otu_updates, unique_iso, unique_seq, logger=logger)
+    if dry_run:
+        cache_path = src_path.parent / ".cache"
+        update_cache_path = cache_path / "updates"
+        update_cache_path.mkdir(exist_ok=True)
+
+        await cache_new_sequences(otu_updates, otu_id, update_cache_path)
+
+        if not update_cache_path / f"{otu_id}.json".exists():
+            logger.error("Write failed")
+    else:
+        await write_records(otu_path, otu_updates, unique_iso, unique_seq, logger=logger)
```

### Comparing `virtool_cli-2.0.0a8/virtool_cli/utils/cache.py` & `virtool_cli-2.0.0a9/virtool_cli/utils/cache.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/utils/format.py` & `virtool_cli-2.0.0a9/virtool_cli/utils/format.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,12 @@
 from Bio.SeqIO import SeqRecord
 from structlog import BoundLogger, get_logger
 from typing import Tuple
 
 
-async def process_records(
-    records: list,
-    metadata: dict,
-    no_fetch_set: set,
-    auto_evaluate: bool = True,
-    logger: BoundLogger = get_logger(),
-) -> list:
-    """
-    Takes sequence records and:
-        1) Evaluates whether those records should be added to the database,
-        2) Formats the records into a smaller dictionary
-        3) Returns new formatted dicts in a list
-
-    WARNING: Auto-evaluation is still under active development, especially multipartite filtering
-
-    :param records: SeqRecords retrieved from the NCBI Nucleotide database
-    :param metadata:
-    :param no_fetch_set:
-    :param auto_evaluate: Boolean flag for whether automatic evaluation functions
-        should be run
-    :param logger: Optional entry point for a shared BoundLogger
-    :return: A list of valid sequences formatted for the Virtool reference database
-    """
-    try:
-        otu_updates, auto_excluded = await process_default(
-            records, metadata, no_fetch_set, logger
-        )
-    except Exception as e:
-        logger.exception(e)
-        raise e
-
-    if auto_excluded:
-        logger.info(
-            "Consider adding these accessions to the exclusion list",
-            auto_excluded=auto_excluded,
-        )
-
-    if otu_updates:
-        return otu_updates
-
-    return []
-
-
 async def process_default(
     records: list, metadata: dict, filter_set: set, logger: BoundLogger = get_logger()
 ) -> Tuple[list, list]:
     """
     Format new sequences from NCBI Taxonomy if they do not already exist in the reference.
 
     :param records: A list of SeqRecords from NCBI Taxonomy
@@ -59,15 +16,15 @@
     :return: A list of processed new sequences/isolates and
         a set of automatically excluded accessions
     """
     auto_excluded = []
     otu_updates = []
 
     for seq_data in records:
-        [accession, _] = seq_data.id.split(".")
+        accession = seq_data.id.split(".")[0]
         seq_qualifier_data = get_qualifiers(seq_data.features)
 
         if accession in filter_set:
             logger.debug("Accession already exists", accession=seq_data.id)
             continue
 
         if check_source_type(seq_qualifier_data) is None:
@@ -113,15 +70,15 @@
         seq_dict['segment'] = record_segment[0]
 
     return seq_dict
 
 
 def format_isolate(source_name: str, source_type: str, isolate_id: str) -> dict:
     """
-    Formats a
+    Formats raw isolate data for storage in a reference directory
 
     :param source_name: Assigned source name for an accession
     :param source_type: Assigned source type for an accession
     :param isolate_id: Unique ID number for this new isolate
     :return: A dict containing the new isolate.json contents
     """
     isolate = {
```

### Comparing `virtool_cli-2.0.0a8/virtool_cli/utils/id_generator.py` & `virtool_cli-2.0.0a9/virtool_cli/utils/id_generator.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/utils/logging.py` & `virtool_cli-2.0.0a9/virtool_cli/utils/logging.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/utils/ncbi.py` & `virtool_cli-2.0.0a9/virtool_cli/utils/ncbi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import asyncio
 from Bio import Entrez, SeqIO
 from urllib.error import HTTPError
+from http.client import IncompleteRead
 
 Entrez.email = os.environ.get("NCBI_EMAIL")
 Entrez.api_key = os.environ.get("NCBI_API_KEY")
 
 NCBI_REQUEST_INTERVAL = 0.3 if Entrez.email and Entrez.api_key else 0.8
 
 
@@ -19,19 +20,23 @@
     upstream_accessions = []
 
     try:
         elink_results = Entrez.elink(
             dbfrom="taxonomy", db="nuccore",
             id=str(taxon_id), idtype="acc"
         )
+    except IncompleteRead:
+        raise HTTPError("IncompleteRead")
+    except HTTPError as e:
+        raise e
+
+    try:
         entrez_acclist = Entrez.read(elink_results)
-    except HTTPError:
-        return []
-    except RuntimeError:
-        return []
+    except RuntimeError as e:
+        raise e
 
     if not entrez_acclist:
         return []
     
     for linksetdb in entrez_acclist[0]["LinkSetDb"][0]["Link"]:
         upstream_accessions.append(str(linksetdb["Id"]))
 
@@ -50,14 +55,16 @@
         handle = Entrez.efetch(
             db="nuccore", id=fetch_list,
             rettype="gb", retmode="text"
         )
         ncbi_records = SeqIO.to_dict(SeqIO.parse(handle, "gb"))
         handle.close()
 
+    except IncompleteRead:
+        raise HTTPError("IncompleteRead")
     except HTTPError as e:
         raise e
 
     if ncbi_records is None:
         return []
     
     try:
@@ -77,15 +84,17 @@
     :param name: Name of a given OTU
     :return: Taxonomy id for the given OTU
     """
     try:
         handle = Entrez.esearch(db="taxonomy", term=name)
         record = Entrez.read(handle)
         handle.close()
-    except Exception as e:
+    except IncompleteRead:
+        raise HTTPError("IncompleteRead")
+    except HTTPError as e:
         raise e
 
     try:
         taxid = int(record["IdList"][0])
     except IndexError:
         taxid = None
 
@@ -99,14 +108,16 @@
     :param taxon_id: NCBI Taxonomy UID
     :return: The taxonomic rank of this Taxonomy record as a string
     """
     try:
         handle = Entrez.efetch(db="taxonomy", id=taxon_id, rettype="docsum", retmode="xml")
         record = Entrez.read(handle)
         handle.close()
+    except IncompleteRead:
+        raise HTTPError("IncompleteRead")
     except HTTPError:
         raise HTTPError
 
     if record:
         return record.pop()
 
     return {}
```

### Comparing `virtool_cli-2.0.0a8/virtool_cli/utils/parse.py` & `virtool_cli-2.0.0a9/virtool_cli/utils/parse.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/utils/reference.py` & `virtool_cli-2.0.0a9/virtool_cli/utils/reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,9 +115,7 @@
     """
     unique_otus = [
         otu_path.stem.split("--")[1]
         for otu_path in src_path.iterdir()
         if otu_path.is_dir()
     ]
     return unique_otus
-
-
```

### Comparing `virtool_cli-2.0.0a8/virtool_cli/utils/storage.py` & `virtool_cli-2.0.0a9/virtool_cli/utils/storage.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/vfam/annotation.py` & `virtool_cli-2.0.0a9/virtool_cli/vfam/annotation.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/vfam/cmd.py` & `virtool_cli-2.0.0a9/virtool_cli/vfam/cmd.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/vfam/collapse.py` & `virtool_cli-2.0.0a9/virtool_cli/vfam/collapse.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/vfam/curate.py` & `virtool_cli-2.0.0a9/virtool_cli/vfam/curate.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/vfam/filter.py` & `virtool_cli-2.0.0a9/virtool_cli/vfam/filter.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/vfam/markov.py` & `virtool_cli-2.0.0a9/virtool_cli/vfam/markov.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/vfam/msa.py` & `virtool_cli-2.0.0a9/virtool_cli/vfam/msa.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/virtool_cli/vfam/polyprotein.py` & `virtool_cli-2.0.0a9/virtool_cli/vfam/polyprotein.py`

 * *Files identical despite different names*

### Comparing `virtool_cli-2.0.0a8/PKG-INFO` & `virtool_cli-2.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virtool-cli
-Version: 2.0.0a8
+Version: 2.0.0a9
 Summary: CLI Tool for working with Virtool data
 License: MIT
 Author: Ian Boyes
 Author-email: igboyes@gmail.com
 Maintainer: Ian Boyes
 Maintainer-email: igboyes@gmail.com
 Requires-Python: >=3.10,<4.0
```

