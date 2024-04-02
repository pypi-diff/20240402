# Comparing `tmp/cellxgene_lamin-0.2.0.tar.gz` & `tmp/cellxgene_lamin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_lamin-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cellxgene_lamin-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cellxgene_lamin-0.2.0.tar` & `cellxgene_lamin-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     4813 2024-03-28 08:26:09.828983 cellxgene_lamin-0.2.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-09-05 14:07:08.719114 cellxgene_lamin-0.2.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-09-05 14:07:08.719576 cellxgene_lamin-0.2.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1252 2024-03-01 14:34:33.549343 cellxgene_lamin-0.2.0/.gitignore
--rw-r--r--   0        0        0     1444 2024-03-26 16:54:13.777899 cellxgene_lamin-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-09-05 14:07:08.699075 cellxgene_lamin-0.2.0/LICENSE
--rw-r--r--   0        0        0      607 2024-03-26 16:54:13.778817 cellxgene_lamin-0.2.0/README.md
--rw-r--r--   0        0        0      444 2024-03-28 13:00:21.054564 cellxgene_lamin-0.2.0/cellxgene_lamin/__init__.py
--rw-r--r--   0        0        0     6936 2024-03-28 11:40:09.462254 cellxgene_lamin-0.2.0/cellxgene_lamin/_annotate.py
--rw-r--r--   0        0        0      538 2024-03-19 11:05:18.090849 cellxgene_lamin-0.2.0/cellxgene_lamin/_curate.py
--rw-r--r--   0        0        0      796 2024-01-17 12:35:32.450804 cellxgene_lamin-0.2.0/cellxgene_lamin/_cxg_rest.py
--rw-r--r--   0        0        0     1834 2024-01-17 12:35:32.451118 cellxgene_lamin-0.2.0/cellxgene_lamin/_features.py
--rw-r--r--   0        0        0     1409 2024-03-19 11:05:18.091120 cellxgene_lamin-0.2.0/cellxgene_lamin/_fields.py
--rw-r--r--   0        0        0     2024 2024-02-01 06:48:25.424516 cellxgene_lamin-0.2.0/cellxgene_lamin/_gene.py
--rw-r--r--   0        0        0     1435 2024-03-26 16:54:13.779949 cellxgene_lamin-0.2.0/cellxgene_lamin/_labels.py
--rw-r--r--   0        0        0     3819 2024-03-26 16:54:13.780676 cellxgene_lamin-0.2.0/cellxgene_lamin/_ontology.py
--rw-r--r--   0        0        0     1538 2024-03-26 16:54:13.781190 cellxgene_lamin-0.2.0/cellxgene_lamin/_organism.py
--rw-r--r--   0        0        0     1334 2024-03-19 11:05:18.091640 cellxgene_lamin-0.2.0/cellxgene_lamin/datasets.py
--rw-r--r--   0        0        0    11534 2024-03-28 11:40:09.462616 cellxgene_lamin-0.2.0/docs/cellxgene-annotate.ipynb
--rw-r--r--   0        0        0    17787 2024-03-28 11:40:09.463235 cellxgene_lamin-0.2.0/docs/cellxgene.ipynb
--rw-r--r--   0        0        0     6229 2024-03-28 13:00:35.915322 cellxgene_lamin-0.2.0/docs/changelog.md
--rw-r--r--   0        0        0      148 2024-03-28 11:40:09.464328 cellxgene_lamin-0.2.0/docs/index.md
--rw-r--r--   0        0        0      594 2024-01-17 12:35:32.452724 cellxgene_lamin-0.2.0/docs/notebooks.md
--rw-r--r--   0        0        0   443766 2024-01-30 09:11:06.175677 cellxgene_lamin-0.2.0/docs/notebooks/cencus-release-2023-12-15-LTS.ipynb
--rw-r--r--   0        0        0    71734 2024-01-30 09:11:06.176308 cellxgene_lamin-0.2.0/docs/notebooks/census-release-2023-07-25.ipynb
--rw-r--r--   0        0        0   351322 2023-12-13 19:44:16.010428 cellxgene_lamin-0.2.0/docs/notebooks/census-release-2023-11-13.ipynb
--rw-r--r--   0        0        0   104755 2024-01-08 15:58:36.215190 cellxgene_lamin-0.2.0/docs/notebooks/census-release-2023-12-06.ipynb
--rw-r--r--   0        0        0    33056 2023-11-16 10:21:52.333881 cellxgene_lamin-0.2.0/docs/notebooks/files-meta.ipynb
--rw-r--r--   0        0        0    20552 2023-11-20 21:49:43.209635 cellxgene_lamin-0.2.0/docs/notebooks/files.ipynb
--rw-r--r--   0        0        0    36950 2023-11-16 15:44:17.995317 cellxgene_lamin-0.2.0/docs/notebooks/meta-human.ipynb
--rw-r--r--   0        0        0  1299626 2023-11-16 15:44:17.997804 cellxgene_lamin-0.2.0/docs/notebooks/meta-mouse.ipynb
--rw-r--r--   0        0        0     8775 2024-03-15 08:45:18.041258 cellxgene_lamin-0.2.0/docs/query-census.ipynb
--rw-r--r--   0        0        0      176 2023-11-23 20:23:34.120310 cellxgene_lamin-0.2.0/lamin-project.yaml
--rw-r--r--   0        0        0     2278 2024-03-28 11:40:09.464889 cellxgene_lamin-0.2.0/noxfile.py
--rw-r--r--   0        0        0     3860 2024-03-28 12:50:18.838166 cellxgene_lamin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      464 2024-03-28 11:40:09.465624 cellxgene_lamin-0.2.0/tests/test_notebooks.py
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 cellxgene_lamin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5051 2024-04-02 09:35:42.292041 cellxgene_lamin-0.2.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-03-19 12:35:39.229740 cellxgene_lamin-0.2.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1252 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1444 2024-03-27 14:52:05.525051 cellxgene_lamin-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/LICENSE
+-rw-r--r--   0        0        0      607 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/README.md
+-rw-r--r--   0        0        0      444 2024-04-02 09:49:14.604374 cellxgene_lamin-0.2.1/cellxgene_lamin/__init__.py
+-rw-r--r--   0        0        0     6951 2024-04-02 09:35:42.292041 cellxgene_lamin-0.2.1/cellxgene_lamin/_annotate.py
+-rw-r--r--   0        0        0      538 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/cellxgene_lamin/_curate.py
+-rw-r--r--   0        0        0      796 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/cellxgene_lamin/_cxg_rest.py
+-rw-r--r--   0        0        0     1834 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/cellxgene_lamin/_features.py
+-rw-r--r--   0        0        0     1409 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/cellxgene_lamin/_fields.py
+-rw-r--r--   0        0        0     2024 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/cellxgene_lamin/_gene.py
+-rw-r--r--   0        0        0     1435 2024-03-26 15:16:11.446346 cellxgene_lamin-0.2.1/cellxgene_lamin/_labels.py
+-rw-r--r--   0        0        0     3819 2024-03-26 15:16:11.446346 cellxgene_lamin-0.2.1/cellxgene_lamin/_ontology.py
+-rw-r--r--   0        0        0     1538 2024-03-26 15:16:11.446346 cellxgene_lamin-0.2.1/cellxgene_lamin/_organism.py
+-rw-r--r--   0        0        0     1334 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/cellxgene_lamin/datasets.py
+-rw-r--r--   0        0        0    11323 2024-04-02 09:35:42.292041 cellxgene_lamin-0.2.1/docs/cellxgene-annotate.ipynb
+-rw-r--r--   0        0        0    17787 2024-03-28 12:38:15.901980 cellxgene_lamin-0.2.1/docs/cellxgene.ipynb
+-rw-r--r--   0        0        0     6674 2024-04-02 09:49:41.607896 cellxgene_lamin-0.2.1/docs/changelog.md
+-rw-r--r--   0        0        0      148 2024-03-28 12:38:15.901980 cellxgene_lamin-0.2.1/docs/index.md
+-rw-r--r--   0        0        0      594 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/docs/notebooks.md
+-rw-r--r--   0        0        0   443766 2024-03-19 17:00:30.489432 cellxgene_lamin-0.2.1/docs/notebooks/cencus-release-2023-12-15-LTS.ipynb
+-rw-r--r--   0        0        0    71734 2024-03-19 17:00:30.489432 cellxgene_lamin-0.2.1/docs/notebooks/census-release-2023-07-25.ipynb
+-rw-r--r--   0        0        0   351322 2024-03-19 17:00:30.492765 cellxgene_lamin-0.2.1/docs/notebooks/census-release-2023-11-13.ipynb
+-rw-r--r--   0        0        0   104755 2024-03-19 17:00:30.492765 cellxgene_lamin-0.2.1/docs/notebooks/census-release-2023-12-06.ipynb
+-rw-r--r--   0        0        0    33056 2024-03-19 17:00:30.492765 cellxgene_lamin-0.2.1/docs/notebooks/files-meta.ipynb
+-rw-r--r--   0        0        0    20552 2024-03-19 17:00:30.492765 cellxgene_lamin-0.2.1/docs/notebooks/files.ipynb
+-rw-r--r--   0        0        0    36950 2024-03-19 17:00:30.492765 cellxgene_lamin-0.2.1/docs/notebooks/meta-human.ipynb
+-rw-r--r--   0        0        0  1299626 2024-03-19 17:00:30.496099 cellxgene_lamin-0.2.1/docs/notebooks/meta-mouse.ipynb
+-rw-r--r--   0        0        0     8775 2024-03-27 14:56:24.485955 cellxgene_lamin-0.2.1/docs/query-census.ipynb
+-rw-r--r--   0        0        0      176 2024-03-19 12:35:39.259740 cellxgene_lamin-0.2.1/lamin-project.yaml
+-rw-r--r--   0        0        0     1927 2024-04-02 09:35:42.292041 cellxgene_lamin-0.2.1/noxfile.py
+-rw-r--r--   0        0        0     3860 2024-04-02 09:49:20.917752 cellxgene_lamin-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      464 2024-03-28 12:38:15.901980 cellxgene_lamin-0.2.1/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 cellxgene_lamin-0.2.1/PKG-INFO
```

### Comparing `cellxgene_lamin-0.2.0/.github/workflows/build.yml` & `cellxgene_lamin-0.2.1/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -73,24 +73,30 @@
         if: ${{ failure() && github.event_name == 'repository_dispatch' }}
         env:
           SLACK_BOT_TOKEN: ${{ secrets.SLACK_GITHUB_ACTION }}
         with:
           channel: lamindb-mirror-github-actions
           status: FAILURE
           color: danger
+      - name: upload docs
+        if: ${{ matrix.group == 'census' || matrix.group == 'validator' }}
+        uses: actions/upload-artifact@v2
+        with:
+          name: docs_${{ matrix.group }}
+          path: docs_${{ matrix.group }}
 
   docs:
     needs: test
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: checkout lndocs
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           repository: laminlabs/lndocs
           ssh-key: ${{ secrets.READ_LNDOCS }}
           path: lndocs
           ref: main
       - uses: aws-actions/configure-aws-credentials@v1
         with:
```

### Comparing `cellxgene_lamin-0.2.0/.github/workflows/latest-changes.yml` & `cellxgene_lamin-0.2.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/.gitignore` & `cellxgene_lamin-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/.pre-commit-config.yaml` & `cellxgene_lamin-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/LICENSE` & `cellxgene_lamin-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/README.md` & `cellxgene_lamin-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/cellxgene_lamin/_annotate.py` & `cellxgene_lamin-0.2.1/cellxgene_lamin/_annotate.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,25 +53,25 @@
 
 class Annotate(AnnDataAnnotator):
     """Annotation flow of AnnData based on CELLxGENE schema."""
 
     def __init__(
         self,
         adata: Union[ad.AnnData, str, Path],
-        var_field: FieldAttr = bt.Gene.ensembl_gene_id,
-        obs_fields: Dict[str, FieldAttr] = CellxGeneFields.OBS_FIELDS,
+        var_index: FieldAttr = bt.Gene.ensembl_gene_id,
+        categoricals: Dict[str, FieldAttr] = CellxGeneFields.OBS_FIELDS,
         using: str = "laminlabs/cellxgene",
         verbosity: str = "hint",
         **kwargs,
     ):
         add_defaults_to_obs_fields(adata, **kwargs)
         super().__init__(
             adata=adata,
-            var_field=var_field,
-            obs_fields=_restrict_obs_fields(adata, obs_fields),
+            var_index=var_index,
+            categoricals=_restrict_obs_fields(adata, categoricals),
             using=using,
             verbosity=verbosity,
         )
         self._schema_version = "5.1.0"
         self._schema_reference = "https://github.com/chanzuckerberg/single-cell-curation/blob/main/schema/5.1.0/schema.md"
         self._pinned_ontologies: Dict[str, str] = {
             "cl": "2024-01-04",
@@ -103,16 +103,16 @@
                    This parameter is required if the AnnData object is not a part of a collection.
 
         Returns:
             An AnnData object which adheres to the cellxgene-schema.
         """
         if self._validated is None:
             validate_categories_in_df(
-                self._adata.obs,
-                fields=self.obs_fields,
+                df=self._adata.obs,
+                fields=self.categoricals,
                 using=self._using,
             )
 
         adata_cxg = self._adata.copy()
 
         reserved_names = {
             "ethnicity",
@@ -136,17 +136,17 @@
             raise ValueError(
                 f"AnnData must not contain obs columns {matched_columns} which are"
                 " reserved from previous schema versions."
             )
 
         # convert name column to ontology_term_id column
         for column in adata_cxg.obs.columns:
-            if column in self.obs_fields and not column.endswith("_ontology_term_id"):
+            if column in self.categoricals and not column.endswith("_ontology_term_id"):
                 mapped_column = convert_name_to_ontology_id(
-                    adata_cxg.obs[column], field=self.obs_fields.get(column)
+                    adata_cxg.obs[column], field=self.categoricals.get(column)
                 )
                 if mapped_column is not None:
                     adata_cxg.obs[f"{column}_ontology_term_id"] = mapped_column
 
         # drop the name columns for ontologies
         drop_columns = [
             i
```

### Comparing `cellxgene_lamin-0.2.0/cellxgene_lamin/_curate.py` & `cellxgene_lamin-0.2.1/cellxgene_lamin/_curate.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/cellxgene_lamin/_cxg_rest.py` & `cellxgene_lamin-0.2.1/cellxgene_lamin/_cxg_rest.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/cellxgene_lamin/_features.py` & `cellxgene_lamin-0.2.1/cellxgene_lamin/_features.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/cellxgene_lamin/_fields.py` & `cellxgene_lamin-0.2.1/cellxgene_lamin/_fields.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/cellxgene_lamin/_gene.py` & `cellxgene_lamin-0.2.1/cellxgene_lamin/_gene.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/cellxgene_lamin/_labels.py` & `cellxgene_lamin-0.2.1/cellxgene_lamin/_labels.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/cellxgene_lamin/_ontology.py` & `cellxgene_lamin-0.2.1/cellxgene_lamin/_ontology.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/cellxgene_lamin/_organism.py` & `cellxgene_lamin-0.2.1/cellxgene_lamin/_organism.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/cellxgene_lamin/datasets.py` & `cellxgene_lamin-0.2.1/cellxgene_lamin/datasets.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/docs/cellxgene-annotate.ipynb` & `cellxgene_lamin-0.2.1/docs/cellxgene-annotate.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962847222222222%*

 * *Differences: {"'cells'": "{19: {'source': ['annotate.categoricals']}, 23: {'source': "*

 * *            '[\'annotate.add_validated_from("all")\']}, 25: {\'source\': '*

 * *            '[\'annotate.add_new_from("donor_id")\']}, 27: {\'source\': [\'tissues = '*

 * *            "annotate.lookup().tissue']}, 30: {'source': "*

 * *            '[\'annotate.add_validated_from("tissue")\']}, 38: {\'source\': {insert: [(1, '*

 * *            '\'artifact = annotate.save_artifact(description="test h5ad file")\')], delete: [1]}}, '*

 * *            "43: {'sourc […]*

```diff
@@ -194,15 +194,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "884daca8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "annotate.obs_fields"
+                "annotate.categoricals"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "24e00633",
             "metadata": {},
@@ -236,15 +236,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d214b7e5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "annotate.update_registry(feature=\"all\")"
+                "annotate.add_validated_from(\"all\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9d30cf05",
             "metadata": {},
             "source": [
@@ -254,15 +254,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "5c1453b0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "annotate.update_registry(feature=\"donor_id\", validated_only=False)"
+                "annotate.add_new_from(\"donor_id\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0861e207",
             "metadata": {},
             "source": [
@@ -272,15 +272,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ba61e42a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "tissues = annotate.lookup()[\"tissue\"]"
+                "tissues = annotate.lookup().tissue"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e56e2fcb",
             "metadata": {},
@@ -305,15 +305,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "bc7c7e4a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "annotate.update_registry(\"tissue\")"
+                "annotate.add_validated_from(\"tissue\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1f3cd3a9",
             "metadata": {},
             "source": [
@@ -383,15 +383,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "f12ec345",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# this will modify the AnnData object by adding required columns and categories\n",
-                "artifact = annotate.register_artifact(description=\"test h5ad file\")"
+                "artifact = annotate.save_artifact(description=\"test h5ad file\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4fc354e4",
             "metadata": {},
             "source": [
@@ -428,15 +428,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "8940e83c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# register a new collection\n",
-                "collection = annotate.register_collection(\n",
+                "collection = annotate.save_collection(\n",
                 "    artifact,  # registered artifact above, can also pass a list of artifacts\n",
                 "    name=(  # title of the publication\n",
                 "        \"Cross-tissue immune cell analysis reveals tissue-specific features in humans\"\n",
                 "        \" (for test demo only)\"\n",
                 "    ),\n",
                 "    description=\"10.1126/science.abl5197\",  # DOI of the publication\n",
                 "    reference=\"E-MTAB-11536\",  # accession number (e.g. GSE#, E-MTAB#, etc.)\n",
@@ -451,24 +451,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "collection.artifact"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "6e963036",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "artifact.collection"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "id": "9eea92a2",
             "metadata": {},
             "source": [
                 "## Return an input h5ad file for cellxgene-schema"
             ]
         },
```

### Comparing `cellxgene_lamin-0.2.0/docs/cellxgene.ipynb` & `cellxgene_lamin-0.2.1/docs/cellxgene.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/docs/changelog.md` & `cellxgene_lamin-0.2.1/docs/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+:sparkles: Pin lamindb 0.69.5 | [47](https://github.com/laminlabs/cellxgene-lamin/pull/47) | [Zethson](https://github.com/Zethson) | 2024-04-02 |
+⬆️ Update Annotate | [46](https://github.com/laminlabs/cellxgene-lamin/pull/46) | [sunnyosun](https://github.com/sunnyosun) | 2024-03-31 |
+:art: Run census & annotate in parallel | [45](https://github.com/laminlabs/cellxgene-lamin/pull/45) | [Zethson](https://github.com/Zethson) | 2024-03-30 |
 ⬆️ Pin lamindb to 0.69.3 | [42](https://github.com/laminlabs/cellxgene-lamin/pull/42) | [Zethson](https://github.com/Zethson) | 2024-03-28 | 0.2.0
 🚚 Rename Validate to Annotate | [43](https://github.com/laminlabs/cellxgene-lamin/pull/43) | [sunnyosun](https://github.com/sunnyosun) | 2024-03-28 |
 Fix census notebook execution not being shown | [41](https://github.com/laminlabs/cellxgene-lamin/pull/41) | [Zethson](https://github.com/Zethson) | 2024-03-27 |
 Fix notebook execution rendering | [39](https://github.com/laminlabs/cellxgene-lamin/pull/39) | [Zethson](https://github.com/Zethson) | 2024-03-27 |
 Add 5.1.0 pinned ontologies & ruff | [37](https://github.com/laminlabs/cellxgene-lamin/pull/37) | [Zethson](https://github.com/Zethson) | 2024-03-19 |
 ✨ Moved cellxgene-lamin-validator here | [36](https://github.com/laminlabs/cellxgene-lamin/pull/36) | [sunnyosun](https://github.com/sunnyosun) | 2024-03-19 | 0.1.0
 💚 Fix CI | [34](https://github.com/laminlabs/cellxgene-lamin/pull/34) | [sunnyosun](https://github.com/sunnyosun) | 2024-03-01 |
```

### Comparing `cellxgene_lamin-0.2.0/docs/notebooks.md` & `cellxgene_lamin-0.2.1/docs/notebooks.md`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/docs/notebooks/cencus-release-2023-12-15-LTS.ipynb` & `cellxgene_lamin-0.2.1/docs/notebooks/cencus-release-2023-12-15-LTS.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/docs/notebooks/census-release-2023-07-25.ipynb` & `cellxgene_lamin-0.2.1/docs/notebooks/census-release-2023-07-25.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/docs/notebooks/census-release-2023-11-13.ipynb` & `cellxgene_lamin-0.2.1/docs/notebooks/census-release-2023-11-13.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/docs/notebooks/census-release-2023-12-06.ipynb` & `cellxgene_lamin-0.2.1/docs/notebooks/census-release-2023-12-06.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/docs/notebooks/files-meta.ipynb` & `cellxgene_lamin-0.2.1/docs/notebooks/files-meta.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/docs/notebooks/files.ipynb` & `cellxgene_lamin-0.2.1/docs/notebooks/files.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/docs/notebooks/meta-human.ipynb` & `cellxgene_lamin-0.2.1/docs/notebooks/meta-human.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/docs/notebooks/meta-mouse.ipynb` & `cellxgene_lamin-0.2.1/docs/notebooks/meta-mouse.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/docs/query-census.ipynb` & `cellxgene_lamin-0.2.1/docs/query-census.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.0/pyproject.toml` & `cellxgene_lamin-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
     "requests",
-    "lamindb[aws,jupyter,bionty,zarr] == 0.69.3"
+    "lamindb[aws,jupyter,bionty,zarr] == 0.69.5"
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/cellxgene-lamin"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `cellxgene_lamin-0.2.0/PKG-INFO` & `cellxgene_lamin-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: cellxgene_lamin
-Version: 0.2.0
+Version: 0.2.1
 Summary: Manage cellxgene metadata using LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests
-Requires-Dist: lamindb[aws,jupyter,bionty,zarr] == 0.69.3
+Requires-Dist: lamindb[aws,jupyter,bionty,zarr] == 0.69.5
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: nbproject_test ; extra == "dev"
 Project-URL: Home, https://github.com/laminlabs/cellxgene-lamin
 Provides-Extra: dev
```

